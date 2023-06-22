# Comparing `tmp/hstrat-1.7.2.tar.gz` & `tmp/hstrat-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstrat-1.7.2.tar", last modified: Sat May 20 23:11:05 2023, max compression
+gzip compressed data, was "hstrat-1.7.3.tar", last modified: Thu Jun 22 05:25:14 2023, max compression
```

## Comparing `hstrat-1.7.2.tar` & `hstrat-1.7.3.tar`

### file list

```diff
@@ -1,1404 +1,1404 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.063534 hstrat-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-20 23:10:06.000000 hstrat-1.7.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-20 23:10:06.000000 hstrat-1.7.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 23:10:06.000000 hstrat-1.7.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-20 23:10:06.000000 hstrat-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-20 23:10:06.000000 hstrat-1.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    68177 2023-05-20 23:11:05.067534 hstrat-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    66934 2023-05-20 23:10:06.000000 hstrat-1.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.815520 hstrat-1.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-20 23:10:06.000000 hstrat-1.7.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.799519 hstrat-1.7.2/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.815520 hstrat-1.7.2/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-20 23:10:06.000000 hstrat-1.7.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-20 23:10:06.000000 hstrat-1.7.2/docs/_templates/autosummary/exception.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-20 23:10:06.000000 hstrat-1.7.2/docs/_templates/autosummary/function.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-20 23:10:06.000000 hstrat-1.7.2/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-20 23:10:06.000000 hstrat-1.7.2/docs/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.839522 hstrat-1.7.2/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    69918 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/bitstring_inference.png
--rw-r--r--   0 runner    (1001) docker     (123)   237331 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/hcat-banner.png
--rw-r--r--   0 runner    (1001) docker     (123)   113105 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/hcat.png
--rw-r--r--   0 runner    (1001) docker     (123)   924857 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/hstrat-hcat.png
--rw-r--r--   0 runner    (1001) docker     (123)    44446 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/hstrat-wordmark.png
--rw-r--r--   0 runner    (1001) docker     (123)    60937 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=mrca-uncertainty-absolute-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    60008 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=mrca-uncertainty-relative-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    89035 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=strata-retained-frac-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)   112642 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=strata-retained-num-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    80813 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=stratum-retention-dripplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    56714 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=mrca-uncertainty-absolute-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    69617 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=mrca-uncertainty-relative-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    83008 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=strata-retained-frac-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    94236 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=strata-retained-num-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    81128 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=stratum-retention-dripplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    60777 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=mrca-uncertainty-absolute-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    59070 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=mrca-uncertainty-relative-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    80948 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=strata-retained-frac-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)   100055 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=strata-retained-num-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    77735 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=stratum-retention-dripplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    60777 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=mrca-uncertainty-absolute-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    59070 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=mrca-uncertainty-relative-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    72749 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=strata-retained-frac-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    65982 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=strata-retained-num-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    75996 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=stratum-retention-dripplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    56620 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=mrca-uncertainty-absolute-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    55430 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=mrca-uncertainty-relative-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    74645 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=strata-retained-frac-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    74609 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=strata-retained-num-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    76740 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=stratum-retention-dripplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    60777 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=mrca-uncertainty-absolute-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    59070 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=mrca-uncertainty-relative-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    67091 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=strata-retained-frac-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    48318 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=strata-retained-num-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    74434 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=stratum-retention-dripplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    56620 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=mrca-uncertainty-absolute-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    55430 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=mrca-uncertainty-relative-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    69965 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=strata-retained-frac-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    53653 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=strata-retained-num-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    74896 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=stratum-retention-dripplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    59115 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=mrca-uncertainty-absolute-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    67020 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=mrca-uncertainty-relative-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    77604 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=strata-retained-frac-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    58469 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=strata-retained-num-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    86774 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=stratum-retention-dripplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    60913 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=mrca-uncertainty-absolute-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    60401 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=mrca-uncertainty-relative-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    85089 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=strata-retained-frac-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    88742 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=strata-retained-num-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    83927 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=stratum-retention-dripplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    60937 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=mrca-uncertainty-absolute-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    60008 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=mrca-uncertainty-relative-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    91737 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=strata-retained-frac-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)   136543 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=strata-retained-num-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    80779 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=stratum-retention-dripplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    56714 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=mrca-uncertainty-absolute-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    69617 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=mrca-uncertainty-relative-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    85268 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=strata-retained-frac-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    93241 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=strata-retained-num-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    81212 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=stratum-retention-dripplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    60777 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=mrca-uncertainty-absolute-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    59070 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=mrca-uncertainty-relative-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    68434 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=strata-retained-frac-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    48191 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=strata-retained-num-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    75488 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=stratum-retention-dripplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    56655 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=mrca-uncertainty-absolute-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    53214 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=mrca-uncertainty-relative-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    74082 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=strata-retained-frac-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    51752 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=strata-retained-num-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    81657 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=stratum-retention-dripplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    59065 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=mrca-uncertainty-absolute-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    56729 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=mrca-uncertainty-relative-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    71884 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=strata-retained-frac-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    52659 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=strata-retained-num-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    75944 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=stratum-retention-dripplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    56679 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=mrca-uncertainty-absolute-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    57055 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=mrca-uncertainty-relative-barplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    75986 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=strata-retained-frac-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    57295 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=strata-retained-num-lineplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    80650 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=stratum-retention-dripplot+ext=.png
--rw-r--r--   0 runner    (1001) docker     (123)    32103 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/pruning.png
--rw-r--r--   0 runner    (1001) docker     (123)    31068 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/pruning_distribution.png
--rw-r--r--   0 runner    (1001) docker     (123)    46766 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/pruning_intensity.png
--rw-r--r--   0 runner    (1001) docker     (123)    34644 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/assets/stratigraph_inference.png
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     5936 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/index_stage1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/index_stage2.rst
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-20 23:10:07.000000 hstrat-1.7.2/docs/indices.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.843522 hstrat-1.7.2/hstrat/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.863523 hstrat-1.7.2/hstrat/_auxiliary_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_AnyTreeAscendingIter.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_AnyTreeFastLeafIter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_AnyTreeFastLevelOrderIter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_AnyTreeFastPostOrderIter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_AnyTreeFastPreOrderIter.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_BioPhyloTree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_CopyableSeriesItemsIter.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_HereditaryStratigraphicArtifact.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_RecursionLimit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_RngStateContext.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_ScalarFormatterFixedPrecision.py
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_aggregate_phylogenies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_assign_contiguous_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_assign_root_ancestor_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_collapse_unifurcations.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_convert_root_ancestor_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_find_chronological_inconsistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_find_leaf_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_find_root_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_has_compact_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_has_contiguous_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_has_multiple_roots.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_is_asexual.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_is_chronologically_ordered.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_is_sexual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_is_topologically_sorted.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_make_ancestor_id_col.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_make_ancestor_list_col.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_make_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_parse_ancestor_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_parse_ancestor_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_reroot_at_id_asexual.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_splay_polytomies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_to_working_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_topological_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_try_add_ancestor_id_col.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_unfurl_lineage_asexual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_all_same.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_all_unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_anynode_deepcopy_except_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_anytree_calc_leaf_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_anytree_cardinality.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_anytree_has_grandparent.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_anytree_has_sibling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_anytree_iterative_deepcopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_anytree_peel_sibling_to_cousin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_anytree_tree_to_alife_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_apply_swaps.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_argsort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_as_compact_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_as_nullable_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_assign_intersecting_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_bit_ceil.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_bit_floor.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_capitalize_n.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_caretdown_marker.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_caretup_marker.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_check_testing_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_cmp.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_cmp_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_consume.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_coshuffled.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_count_unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_curried_binary_search_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_deep_listify.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_demark.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_div_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_find_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_flag_last.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_flat_len.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_generate_n.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_generate_omission_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_get_hstrat_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_get_nullable_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_get_nullable_vals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_give_len.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_indices_of_unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_intersect_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_is_base64.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_is_in.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_is_in_coverage_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_is_in_unit_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_is_nondecreasing.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_is_nonincreasing.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_is_strictly_decreasing.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_is_strictly_increasing.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_is_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_iter_chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_iter_monotonic_equivalencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_iter_monotonic_equivalencies_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_iter_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_jit_numba_dict_t.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_jit_numba_integer_array_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_jit_numpy_bool_t.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_jit_numpy_int64_t.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_launder_impl_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_log_once_in_a_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_make_intersecting_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_memoize_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_min_array_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_numpy_fromiter_polyfill.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_numpy_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_numpy_index_flat.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_omit_last.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_parse_from_numeral_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_popcount.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_raises.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_random_choice_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_release_cur_mpl_fig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_render_to_base64url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_render_to_numeral_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_reversed_enumerate.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_reversed_range.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_scale_luminosity.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_seed_random.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_splicewhile.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_swap_rows_and_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_to_tril.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_unfurl_lineage_with_contiguous_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_unpairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_unzip.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_with_omission.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_with_rng_state_context.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/_auxiliary_lib/_zip_strict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.863523 hstrat-1.7.2/hstrat/frozen_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/frozen_instrumentation/_HereditaryStratigraphicAssemblage.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/frozen_instrumentation/_HereditaryStratigraphicAssemblageSpecimen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/frozen_instrumentation/_HereditaryStratigraphicSpecimen.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/frozen_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.863523 hstrat-1.7.2/hstrat/genome_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)    22102 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/genome_instrumentation/_HereditaryStratigraphicColumn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/genome_instrumentation/_HereditaryStratigraphicColumnBundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/genome_instrumentation/_HereditaryStratum.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/genome_instrumentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.863523 hstrat-1.7.2/hstrat/genome_instrumentation/stratum_ordered_stores/
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/genome_instrumentation/stratum_ordered_stores/_HereditaryStratumOrderedStoreDict.py
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/genome_instrumentation/stratum_ordered_stores/_HereditaryStratumOrderedStoreList.py
--rw-r--r--   0 runner    (1001) docker     (123)    15003 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/genome_instrumentation/stratum_ordered_stores/_HereditaryStratumOrderedStoreTree.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/genome_instrumentation/stratum_ordered_stores/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.863523 hstrat-1.7.2/hstrat/genome_instrumentation/stratum_ordered_stores/_detail/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/genome_instrumentation/stratum_ordered_stores/_detail/_HereditaryStratumOrderedStoreBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/genome_instrumentation/stratum_ordered_stores/_detail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.863523 hstrat-1.7.2/hstrat/hstrat/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/hstrat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.867523 hstrat-1.7.2/hstrat/juxtaposition/
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_calc_definitive_max_rank_of_first_retained_disparity_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_calc_definitive_max_rank_of_last_retained_commonality_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_calc_definitive_min_ranks_since_first_retained_disparity_with.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_calc_definitive_min_ranks_since_last_retained_commonality_with.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_calc_min_implausible_spurious_consecutive_differentia_collisions_between.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_calc_probability_differentia_collision_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_calc_rank_of_first_retained_disparity_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_calc_rank_of_last_retained_commonality_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_calc_ranks_since_first_retained_disparity_with.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_calc_ranks_since_last_retained_commonality_with.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_diff_retained_ranks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_get_last_common_stratum_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_get_nth_common_rank_between.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.867523 hstrat-1.7.2/hstrat/juxtaposition/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl/_dispatch_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.867523 hstrat-1.7.2/hstrat/juxtaposition/_impl_column/
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl_column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl_column/_calc_rank_of_first_retained_disparity_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl_column/_calc_rank_of_first_retained_disparity_between_bsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl_column/_calc_rank_of_first_retained_disparity_between_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl_column/_calc_rank_of_last_retained_commonality_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl_column/_calc_rank_of_last_retained_commonality_between_bsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl_column/_calc_rank_of_last_retained_commonality_between_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl_column/_calc_rank_of_parity_segue_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl_column/_iter_mutual_ranks.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl_column/_iter_ranks_of_retained_commonality_between.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.871523 hstrat-1.7.2/hstrat/juxtaposition/_impl_specimen/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl_specimen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl_specimen/_calc_rank_of_first_retained_disparity_between.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl_specimen/_calc_rank_of_last_retained_commonality_between.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl_specimen/_calc_rank_of_parity_segue_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl_specimen/_calc_rank_of_parity_segue_between_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl_specimen/_iter_mutual_rank_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl_specimen/_iter_mutual_ranks.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/juxtaposition/_impl_specimen/_iter_ranks_of_retained_commonality_between.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.871523 hstrat-1.7.2/hstrat/phylogenetic_inference/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.871523 hstrat-1.7.2/hstrat/phylogenetic_inference/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/estimators/_estimate_rank_of_mrca_maximum_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/estimators/_estimate_rank_of_mrca_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/estimators/_estimate_rank_of_mrca_unbiased.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.879524 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_ballpark_patristic_distance_between.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_ballpark_rank_of_mrca_between.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_ballpark_ranks_since_mrca_with.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_calc_patristic_distance_bounds_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_calc_rank_of_earliest_detectable_mrca_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_calc_rank_of_mrca_bounds_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_calc_rank_of_mrca_bounds_provided_confidence_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_calc_rank_of_mrca_uncertainty_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_calc_ranks_since_earliest_detectable_mrca_with.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_calc_ranks_since_mrca_bounds_provided_confidence_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_calc_ranks_since_mrca_bounds_with.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_calc_ranks_since_mrca_uncertainty_with.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_does_definitively_have_no_common_ancestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_does_have_any_common_ancestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_estimate_patristic_distance_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_estimate_rank_of_mrca_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_estimate_ranks_since_mrca_with.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.883524 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_impl/_estimate_rank_of_mrca_maximum_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_impl/_estimate_rank_of_mrca_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_impl/_estimate_rank_of_mrca_unbiased.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_impl/_extract_common_retained_ranks_through_first_retained_disparity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.883524 hstrat-1.7.2/hstrat/phylogenetic_inference/population/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/population/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/population/_build_distance_matrix_biopython.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/population/_build_distance_matrix_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/population/_calc_rank_of_earliest_detectable_mrca_among.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/population/_calc_rank_of_mrca_bounds_among.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/population/_calc_rank_of_mrca_uncertainty_among.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/population/_does_definitively_share_no_common_ancestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/population/_does_share_any_common_ancestor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.883524 hstrat-1.7.2/hstrat/phylogenetic_inference/priors/
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/priors/_ArbitraryPrior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/priors/_BubbleWrappedPrior.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/priors/_ExponentialPrior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/priors/_GeometricPrior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/priors/_UniformPrior.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/priors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.887524 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_build_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_build_tree_nj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_build_tree_trie.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_build_tree_trie_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_build_tree_upgma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.887524 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/_TrieInnerNode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/_TrieLeafNode.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/_append_genesis_organism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/_build_tree_biopython_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/_build_trie_from_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/_estimate_origin_times.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/_find_chronological_root.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/_find_chronological_roots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/_time_calibrate_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.891524 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/trie_postprocess/
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/trie_postprocess/_AssignDestructionTimeYoungestPlusOneTriePostprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/trie_postprocess/_AssignOriginTimeExpectedValueTriePostprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/trie_postprocess/_AssignOriginTimeNaiveTriePostprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/trie_postprocess/_AssignOriginTimeNodeRankTriePostprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/trie_postprocess/_CompoundTriePostprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/trie_postprocess/_PeelBackConjoinedLeavesTriePostprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/trie_postprocess/_SampleAncestralRollbacksTriePostprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/phylogenetic_inference/tree/trie_postprocess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.891524 hstrat-1.7.2/hstrat/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/serialization/_assemblage_from_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/serialization/_col_from_records.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/serialization/_col_to_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/serialization/_col_to_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/serialization/_col_to_specimen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.891524 hstrat-1.7.2/hstrat/serialization/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/serialization/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/serialization/_impl/_col_records_from_pop_records.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/serialization/_impl/_policy_from_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/serialization/_pack_differentiae.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/serialization/_pop_from_records.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/serialization/_pop_to_assemblage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/serialization/_pop_to_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/serialization/_pop_to_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/serialization/_specimen_from_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/serialization/_unassemblage_from_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/serialization/_unpack_differentiae.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.891524 hstrat-1.7.2/hstrat/stratum_retention_strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.891524 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.895525 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_detail/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_detail/_PolicyCouplerBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_detail/_PolicyCouplerFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_detail/_PolicySpecBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_detail/_UnsatisfiableParameterizationRequestError.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_detail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.895525 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyAbsUpperBoundPessimalRankBruteForce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyAbsUpperBoundWorstCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyRelExactFromAbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyRelUpperBoundPessimalRankBruteForce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyRelUpperBoundWorstCase.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcNumStrataRetainedUpperBoundWorstCase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_GenDropRanksFromPredKeepRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.895525 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_PolicySpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.895525 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_enact/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_enact/_GenDropRanks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.895525 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_enact/_GenDropRanks_/
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_enact/_GenDropRanks_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_enact/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.895525 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_impl/_calc_provided_uncertainty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.899525 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.903525 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.903525 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_PolicySpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.903525 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_enact/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_enact/_GenDropRanks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.907525 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_enact/_GenDropRanks_/
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_enact/_GenDropRanks_/_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_enact/_GenDropRanks_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_enact/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.907525 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_impl/_calc_provided_uncertainty.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.907525 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.911525 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.911525 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_PolicySpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.911525 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_enact/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_enact/_GenDropRanks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.911525 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_enact/_GenDropRanks_/
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_enact/_GenDropRanks_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_enact/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.915526 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.915526 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.915526 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_PolicySpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.919526 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_enact/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_enact/_GenDropRanks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.919526 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_enact/_GenDropRanks_/
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_enact/_GenDropRanks_/_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_enact/_GenDropRanks_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_enact/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.919526 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_calc_common_ratio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_get_retained_ranks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_rank_backstops.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_rank_cutoffs.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_rank_seps.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_target_ranks.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_target_recencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.923526 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.923526 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.923526 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_PolicySpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.923526 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_enact/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_enact/_GenDropRanks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.923526 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_enact/_GenDropRanks_/
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_enact/_GenDropRanks_/_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_enact/_GenDropRanks_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_enact/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.927526 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_common_ratio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_rank_backstop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_rank_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_rank_sep.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_target_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_target_recency.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_get_retained_ranks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_iter_priority_ranks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.927526 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.927526 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.927526 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_PolicySpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.931527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_enact/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_enact/_GenDropRanks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.931527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_enact/_GenDropRanks_/
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_enact/_GenDropRanks_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_enact/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.931527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.931527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.935527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_PolicySpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.935527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_enact/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_enact/_GenDropRanks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.935527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_enact/_GenDropRanks_/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_enact/_GenDropRanks_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_enact/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.935527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.935527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.939527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_PolicySpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.939527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_enact/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_enact/_GenDropRanks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.939527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_enact/_GenDropRanks_/
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_enact/_GenDropRanks_/_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_enact/_GenDropRanks_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_enact/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.939527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_impl/_decide_if_discard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.943527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.943527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_scry/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_scry/_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_scry/_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_scry/_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_scry/_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_scry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.943527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_PolicySpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.943527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_enact/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_enact/_GenDropRanks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.943527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_enact/_GenDropRanks_/
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_enact/_GenDropRanks_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_enact/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.943527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_impl/_calc_provided_uncertainty.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_impl/_num_to_condemn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.947527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.947527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.947527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_PolicySpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.947527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_impl/_calc_geom_seq_nth_root_transition_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_impl/_calc_provided_degree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_impl/_calc_provided_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_impl/_pick_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.947527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_PolicySpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.947527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_enact/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_enact/_GenDropRanks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.951527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_enact/_GenDropRanks_/
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_enact/_GenDropRanks_/_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_enact/_GenDropRanks_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_enact/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.951527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_impl/_decide_if_discard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.951527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.951527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_scry/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_scry/_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_scry/_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_scry/_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_scry/_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_scry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.951527 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_MrcaUncertaintyAbsExactEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_MrcaUncertaintyAbsUpperBoundEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_MrcaUncertaintyRelExactEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_MrcaUncertaintyRelUpperBoundEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_NumStrataRetainedExactEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_NumStrataRetainedUpperBoundEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.955528 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_detail/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_detail/_policy_param_focalizer_t.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.955528 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/_PropertyAtLeastParameterizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/_PropertyAtMostParameterizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/_PropertyExactlyParameterizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.955528 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/_detail/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/_detail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/_detail/_policy_evaluator_t.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.955528 hstrat-1.7.2/hstrat/stratum_retention_viz/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_viz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.955528 hstrat-1.7.2/hstrat/stratum_retention_viz/animate/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_viz/animate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_viz/animate/_policy_panel_animate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_viz/animate/_stratum_retention_animate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.955528 hstrat-1.7.2/hstrat/stratum_retention_viz/ascii/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_viz/ascii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_viz/ascii/_col_to_ascii.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.959528 hstrat-1.7.2/hstrat/stratum_retention_viz/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_viz/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_viz/plot/_mrca_uncertainty_absolute_barplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_viz/plot/_mrca_uncertainty_relative_barplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_viz/plot/_policy_panel_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_viz/plot/_strata_retained_frac_lineplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_viz/plot/_strata_retained_num_lineplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/stratum_retention_viz/plot/_stratum_retention_dripplot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.959528 hstrat-1.7.2/hstrat/test_drive/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.959528 hstrat-1.7.2/hstrat/test_drive/descend_template_phylogeny/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/descend_template_phylogeny/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_alifestd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_biopython.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_dendropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_networkx.py
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_posthoc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.959528 hstrat-1.7.2/hstrat/test_drive/generate_template_phylogeny/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/generate_template_phylogeny/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8873 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.959528 hstrat-1.7.2/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/_apply_island_migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/_apply_mutation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/_apply_niche_invasions.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/_get_island_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/_get_niche_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/_select_parents.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.963528 hstrat-1.7.2/hstrat/test_drive/perfect_tracking/
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/perfect_tracking/_DecantingPhyloTracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/perfect_tracking/_GarbageCollectingPhyloTracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.963528 hstrat-1.7.2/hstrat/test_drive/perfect_tracking/_GarbageCollectingPhyloTracker_/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/perfect_tracking/_GarbageCollectingPhyloTracker_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/perfect_tracking/_GarbageCollectingPhyloTracker_/_discern_referenced_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/perfect_tracking/_PerfectBacktrackHandle.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/perfect_tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/perfect_tracking/_compile_perfect_backtrack_phylogeny.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/perfect_tracking/_compile_phylogeny_from_lineage_iters.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-20 23:10:07.000000 hstrat-1.7.2/hstrat/test_drive/perfect_tracking/_iter_perfect_backtrack_lineage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.843522 hstrat-1.7.2/hstrat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    68177 2023-05-20 23:11:04.000000 hstrat-1.7.2/hstrat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)   124850 2023-05-20 23:11:04.000000 hstrat-1.7.2/hstrat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 23:11:04.000000 hstrat-1.7.2/hstrat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-20 23:11:04.000000 hstrat-1.7.2/hstrat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-20 23:11:04.000000 hstrat-1.7.2/hstrat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-20 23:10:07.000000 hstrat-1.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-20 23:11:05.067534 hstrat-1.7.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      195 2023-05-20 23:10:07.000000 hstrat-1.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.963528 hstrat-1.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.963528 hstrat-1.7.2/tests/test_hstrat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.967528 hstrat-1.7.2/tests/test_hstrat/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/assets/grandchild.newick
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/assets/grandchild_and_aunt.newick
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/assets/grandchild_and_auntuncle.newick
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/assets/grandtriplets.newick
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/assets/grandtriplets_and_aunt.newick
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/assets/grandtriplets_and_auntuncle.newick
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/assets/grandtwins.newick
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/assets/grandtwins_and_aunt.newick
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/assets/grandtwins_and_auntuncle.newick
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/assets/greatgrandtwins_and_auntuncle.newick
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/assets/justroot.newick
--rw-r--r--   0 runner    (1001) docker     (123)   110110 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/assets/nk_ecoeaselection.csv
--rw-r--r--   0 runner    (1001) docker     (123)    50218 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/assets/nk_lexicaseselection.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/assets/nk_tournamentselection.csv
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/assets/onlychild.newick
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/assets/triplets.newick
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/assets/twins.newick
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/run_tests.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.987530 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.995530 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-ancestor_list-syntax1.csv
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-ancestor_list-syntax2.csv
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-ancestor_list-syntax3.csv
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-ancestor_list-syntax4.csv
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-duplicate-id1.csv
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-duplicate-id2.csv
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-duplicate-id3.csv
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-mismatched-ancestor_id-ancestor_list-columns1.csv
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-mismatched-ancestor_id-ancestor_list-columns2.csv
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-mismatched-ancestor_id-ancestor_list-columns3.csv
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-missing-ancestor_list-column1.csv
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-missing-ancestor_list-column2.csv
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-missing-id-column.csv
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-negative-id1.csv
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-negative-id2.csv
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-negative-id3.csv
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-nonexistant-ancestor_id-id1.csv
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-nonexistant-ancestor_id-id2.csv
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-nonexistant-ancestor_id-id3.csv
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-nonexistant-ancestor_id-id4.csv
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-nonexistant-ancestor_list-id.csv
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny-empty-list-notation.csv
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny-noncompact1.csv
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny-noncompact2.csv
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny-uniq.csv
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny.csv
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-ancestor_list-syntax1.csv
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-ancestor_list-syntax2.csv
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-ancestor_list-syntax3.csv
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-ancestor_list-syntax4.csv
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-duplicate-id1.csv
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-duplicate-id2.csv
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-duplicate-id3.csv
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-mismatched-ancestor_id-ancestor_list-columns1.csv
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-mismatched-ancestor_id-ancestor_list-columns2.csv
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-missing-id-column.csv
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-negative-id1.csv
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-negative-id2.csv
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-negative-id3.csv
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-nonexistant-ancestor_list-id.csv
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny-empty-list-notation.csv
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny-noncompact1.csv
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny-noncompact2.csv
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny-uniq.csv
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny.csv
--rw-r--r--   0 runner    (1001) docker     (123)   110110 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/nk_ecoeaselection.csv
--rw-r--r--   0 runner    (1001) docker     (123)    50218 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/nk_lexicaseselection.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/nk_tournamentselection.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeAscendingIter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeFastLeafIter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeFastLevelOrderIter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeFastPostOrderIter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeFastPreOrderIter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_CopyableSeriesItemsIter.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_HereditaryStratigraphicArtifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_RngStateContext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_aggregate_phylogenies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_assign_contiguous_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_assign_root_ancestor_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_collapse_unifurcations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_convert_root_ancestor_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_find_chronological_inconsistency.py
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_find_leaf_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_find_root_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_has_compact_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_has_contiguous_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_has_multiple_roots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_is_asexual.py
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_is_chronologically_ordered.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_is_sexual.py
--rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_is_topologically_sorted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_make_ancestor_id_col.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_make_ancestor_list_col.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_make_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_parse_ancestor_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_parse_ancestor_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_reroot_at_id_asexual.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_splay_polytomies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_to_working_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_topological_sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_try_add_ancestor_id_col.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_unfurl_lineage_asexual.py
--rw-r--r--   0 runner    (1001) docker     (123)    10407 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_all_same.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_all_unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_anynode_deepcopy_except_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_anytree_calc_leaf_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_anytree_cardinality.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_anytree_has_grandparent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_anytree_has_sibling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_anytree_iterative_deepcopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_anytree_peel_sibling_to_cousin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_anytree_tree_to_alife_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_apply_swaps.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_argsort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_as_compact_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_as_nullable_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_assign_intersecting_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_bit_ceil.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_bit_floor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_capitalize_n.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_cmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_cmp_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_consume.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_coshuffled.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_count_unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_curried_binary_search_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_deep_listify.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_demark.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_div_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_find_bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_flag_last.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_flat_len.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_generate_n.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_generate_omission_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_get_hstrat_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_get_nullable_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_get_nullable_vals.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_give_len.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_indices_of_unique.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_intersect_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_is_base64.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_is_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_is_nondecreasing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_is_nonincreasing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_is_strictly_decreasing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_is_strictly_increasing.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_is_subset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_iter_chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_iter_monotonic_equivalencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_iter_monotonic_equivalencies_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_iter_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_make_intersecting_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_memoize_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_min_array_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_numpy_fromiter_polyfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_numpy_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_numpy_index_flat.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_omit_last.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_pairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_parse_from_numeral_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_popcount.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_raises.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_random_choice_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_render_to_base64url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_render_to_numeral_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_reversed_enumerate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_reversed_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_seed_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_splicewhile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_swap_rows_and_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_to_tril.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_unfurl_lineage_with_contiguous_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_unpairwise.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_unzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_with_omission.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_with_rng_state_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_zip_strict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.995530 hstrat-1.7.2/tests/test_hstrat/test_frozen_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_frozen_instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_frozen_instrumentation/test_HereditaryStratigraphicAssemblage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_frozen_instrumentation/test_HereditaryStratigraphicAssemblageSpecimen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_frozen_instrumentation/test_HereditaryStratigraphicSpecimen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.999530 hstrat-1.7.2/tests/test_hstrat/test_genome_instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_genome_instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27700 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_genome_instrumentation/test_HereditaryStratigraphicColumn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_genome_instrumentation/test_HereditaryStratigraphicColumnBundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_genome_instrumentation/test_HereditaryStratum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.999530 hstrat-1.7.2/tests/test_hstrat/test_genome_instrumentation/test_stratum_ordered_stores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_genome_instrumentation/test_stratum_ordered_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16916 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_genome_instrumentation/test_stratum_ordered_stores/test_HereditaryStratumOrderedStoreDict.py
--rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_genome_instrumentation/test_stratum_ordered_stores/test_HereditaryStratumOrderedStoreList.py
--rw-r--r--   0 runner    (1001) docker     (123)    19044 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_genome_instrumentation/test_stratum_ordered_stores/test_HereditaryStratumOrderedStoreTree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:04.999530 hstrat-1.7.2/tests/test_hstrat/test_hstrat/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_hstrat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_hstrat/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.003530 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_definitive_max_rank_of_first_retained_disparity_between.py
--rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_definitive_max_rank_of_last_retained_commonality_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_definitive_min_ranks_since_first_retained_disparity_with.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_definitive_min_ranks_since_last_retained_commonality_with.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_min_implausible_spurious_consecutive_differentia_collisions_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_probability_differentia_collision_between.py
--rw-r--r--   0 runner    (1001) docker     (123)    34817 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_rank_of_first_retained_disparity_between.py
--rw-r--r--   0 runner    (1001) docker     (123)    28695 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_rank_of_last_retained_commonality_between.py
--rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_ranks_since_first_retained_disparity_with.py
--rw-r--r--   0 runner    (1001) docker     (123)    15682 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_ranks_since_last_retained_commonality_with.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_diff_retained_ranks.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_get_last_common_stratum_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_get_nth_common_rank_between.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.003530 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_impl/test_dispatch_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.003530 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_impl_column/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_impl_column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22298 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_impl_column/test_iter_ranks_of_retained_commonality_between_generic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.003530 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_impl_specimen/
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_impl_specimen/test_calc_rank_of_first_retained_disparity_between_specimen_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_impl_specimen/test_calc_rank_of_last_retained_commonality_between_specimen_naive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.003530 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.003530 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_estimators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_estimators/test_estimate_rank_of_mrca_maximum_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_estimators/test_estimate_rank_of_mrca_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_estimators/test_estimate_rank_of_mrca_unbiased.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.007531 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_ballpark_patristic_distance_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_ballpark_rank_of_mrca_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_ballpark_ranks_since_mrca_with.py
--rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_patristic_distance_bounds_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_rank_of_earliest_detectable_mrca_between.py
--rw-r--r--   0 runner    (1001) docker     (123)    22500 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_rank_of_mrca_bounds_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_rank_of_mrca_bounds_provided_confidence_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    18837 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_rank_of_mrca_uncertainty_between.py
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_ranks_since_earliest_detectable_mrca_with.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_ranks_since_mrca_bounds_provided_confidence_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    18764 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_ranks_since_mrca_bounds_with.py
--rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_ranks_since_mrca_uncertainty_with.py
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_does_definitively_have_no_common_ancestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_does_have_any_common_ancestor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14073 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_estimate_patristic_distance_between.py
--rw-r--r--   0 runner    (1001) docker     (123)    28321 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_estimate_rank_of_mrca_between.py
--rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_estimate_ranks_since_mrca_with.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.007531 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_population/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_population/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_population/test_build_distance_matrix_biopython.py
--rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_population/test_build_distance_matrix_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_population/test_calc_rank_of_earliest_detectable_mrca_among.py
--rw-r--r--   0 runner    (1001) docker     (123)    23442 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_population/test_calc_rank_of_mrca_bounds_among.py
--rw-r--r--   0 runner    (1001) docker     (123)    23811 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_population/test_calc_rank_of_mrca_uncertainty_among.py
--rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_population/test_does_definitively_share_no_common_ancestor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_population/test_does_share_any_common_ancestor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.011531 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_priors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_priors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_ArbitraryPrior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_BubbleWrappedPrior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_ExponentialPrior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_GeometricPrior.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_UniformPrior.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.011531 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.011531 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/_descend_unifurcations.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/_load_dendropy_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/_setup_dendropy_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/_tree_quartet_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/_tree_unweighted_robinson_foulds_distance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.015531 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/grandchild.newick
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/grandchild_and_aunt.newick
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/grandchild_and_auntuncle.newick
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/grandtriplets.newick
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/grandtriplets_and_aunt.newick
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/grandtriplets_and_auntuncle.newick
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/grandtwins.newick
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/grandtwins_and_aunt.newick
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/grandtwins_and_auntuncle.newick
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/greatgrandtwins_and_auntuncle.newick
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/justroot.newick
--rw-r--r--   0 runner    (1001) docker     (123)   110110 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/nk_ecoeaselection.csv
--rw-r--r--   0 runner    (1001) docker     (123)    50218 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/nk_lexicaseselection.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/nk_tournamentselection.csv
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/onlychild.newick
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/triplets.newick
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/twins.newick
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree_nj.py
--rw-r--r--   0 runner    (1001) docker     (123)    15756 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree_trie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree_trie_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree_upgma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.019531 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/
--rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_TrieInnerNode.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_TrieLeafNode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_append_genesis_organism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_estimate_origin_times.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_find_chronological_root.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_find_chronological_roots.py
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_time_calibrate_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.019531 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_AssignDestructionTimeYoungestPlusOneTriePostprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_AssignOriginTimeExpectedValueTriePostprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_AssignOriginTimeNaiveTriePostprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_AssignOriginTimeNodeRankTriePostprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_CompoundTriePostprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_PeelBackConjoinedLeavesTriePostprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_SampleAncestralRollbacksTriePostprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_bias_adjustment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.023532 hstrat-1.7.2/tests/test_hstrat/test_serialization/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_serialization/test_assemblage_from_records.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_serialization/test_col_to_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_serialization/test_col_to_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_serialization/test_col_to_specimen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.023532 hstrat-1.7.2/tests/test_hstrat/test_serialization/test_impl/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_serialization/test_impl/test_col_records_from_pop_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_serialization/test_pack_differentiae.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_serialization/test_pop_to_assemblage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_serialization/test_pop_to_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_serialization/test_pop_to_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_serialization/test_specimen_from_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_serialization/test_unassemblage_from_records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_serialization/test_unpack_differentiae.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.023532 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.023532 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.023532 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_PolicySpec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.027532 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_PolicySpec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.031532 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_PolicySpec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.035532 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_PolicySpec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.035532 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_PolicySpec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.039532 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_PolicySpec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.043532 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_PolicySpec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.047533 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_PolicySpec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.047533 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_PolicySpec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.051533 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.051533 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/impl/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/impl/iter_backing_policy_transition_ranks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcRankAtColumnIndex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.051533 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_GenDropRanks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_GenDropRanks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_GenDropRanks/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_GenDropRanks/test_impl_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_GenDropRanks/test_policy_consistency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.051533 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_backing_policy_transition_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_eq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_implementation_consistency_at_backing_policy_transitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_only_dwindling_over_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_ranks_sorted_and_unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_ranks_valid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_zero_and_last_ranks_retained.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_PolicySpec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.055533 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_impl/test_calc_geom_seq_nth_root_transition_rank.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_impl/test_iter_backing_policy_transition_ranks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.055533 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyAbsExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyRelExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyRelUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcNumStrataRetainedExact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcNumStrataRetainedUpperBound.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcRankAtColumnIndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_GenDropRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_IterRetainedRanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_Policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_PolicySpec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.059533 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18532 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_MrcaUncertaintyAbsExactEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_MrcaUncertaintyAbsUpperBoundEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19284 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_MrcaUncertaintyRelExactEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19242 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_MrcaUncertaintyRelUpperBoundEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_NumStrataRetainedExactEvaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_NumStrataRetainedUpperBoundEvaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.059533 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.059533 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_animate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_animate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_animate/test_policy_panel_animate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_animate/test_stratum_retention_animate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.059533 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_mrca_uncertainty_absolute_barplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_mrca_uncertainty_relative_barplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_policy_panel_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_strata_retained_frac_lineplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_strata_retained_num_lineplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_stratum_retention_dripplot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.063534 hstrat-1.7.2/tests/test_hstrat/test_test_drive/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:11:05.063534 hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/grandchild.newick
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/grandchild_and_aunt.newick
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/grandchild_and_auntuncle.newick
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/grandtriplets.newick
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/grandtriplets_and_aunt.newick
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/grandtriplets_and_auntuncle.newick
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/grandtwins.newick
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/grandtwins_and_aunt.newick
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/grandtwins_and_auntuncle.newick
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/greatgrandtwins_and_auntuncle.newick
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/justroot.newick
--rw-r--r--   0 runner    (1001) docker     (123)   110110 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/nk_ecoeaselection.csv
--rw-r--r--   0 runner    (1001) docker     (123)    50218 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/nk_lexicaseselection.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/nk_tournamentselection.csv
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/onlychild.newick
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/triplets.newick
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/twins.newick
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_DecantingPhyloTracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_GarbageCollectingPhyloTracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny.py
--rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_alifestd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_biopython.py
--rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_dendropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_networkx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_posthoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_evolve_fitness_trait_population.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-20 23:10:07.000000 hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_perfect_tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.259609 hstrat-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-22 05:24:26.000000 hstrat-1.7.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-22 05:24:26.000000 hstrat-1.7.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-22 05:24:26.000000 hstrat-1.7.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-22 05:24:26.000000 hstrat-1.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-22 05:24:26.000000 hstrat-1.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    68177 2023-06-22 05:25:14.259609 hstrat-1.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    66934 2023-06-22 05:24:26.000000 hstrat-1.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:13.959606 hstrat-1.7.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:13.943606 hstrat-1.7.3/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:13.959606 hstrat-1.7.3/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/_templates/autosummary/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/_templates/autosummary/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:13.987606 hstrat-1.7.3/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    69918 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/bitstring_inference.png
+-rw-r--r--   0 runner    (1001) docker     (123)   237331 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/hcat-banner.png
+-rw-r--r--   0 runner    (1001) docker     (123)   113105 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/hcat.png
+-rw-r--r--   0 runner    (1001) docker     (123)   924857 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/hstrat-hcat.png
+-rw-r--r--   0 runner    (1001) docker     (123)    44446 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/hstrat-wordmark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60937 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=mrca-uncertainty-absolute-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60008 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=mrca-uncertainty-relative-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    89035 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=strata-retained-frac-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)   112642 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=strata-retained-num-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    80813 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=stratum-retention-dripplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56714 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=mrca-uncertainty-absolute-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    69617 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=mrca-uncertainty-relative-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    83008 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=strata-retained-frac-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    94236 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=strata-retained-num-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    81128 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=stratum-retention-dripplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60777 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=mrca-uncertainty-absolute-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    59070 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=mrca-uncertainty-relative-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    80948 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=strata-retained-frac-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)   100055 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=strata-retained-num-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    77735 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=stratum-retention-dripplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60777 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=mrca-uncertainty-absolute-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    59070 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=mrca-uncertainty-relative-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    72749 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=strata-retained-frac-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    65982 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=strata-retained-num-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    75996 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=stratum-retention-dripplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56620 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=mrca-uncertainty-absolute-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    55430 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=mrca-uncertainty-relative-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    74645 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=strata-retained-frac-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    74609 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=strata-retained-num-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    76740 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=stratum-retention-dripplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60777 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=mrca-uncertainty-absolute-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    59070 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=mrca-uncertainty-relative-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    67091 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=strata-retained-frac-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    48318 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=strata-retained-num-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    74434 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=stratum-retention-dripplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56620 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=mrca-uncertainty-absolute-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    55430 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=mrca-uncertainty-relative-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    69965 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=strata-retained-frac-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53653 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=strata-retained-num-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    74896 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=stratum-retention-dripplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    59115 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=mrca-uncertainty-absolute-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    67020 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=mrca-uncertainty-relative-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    77604 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=strata-retained-frac-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    58469 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=strata-retained-num-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86774 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=stratum-retention-dripplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60913 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=mrca-uncertainty-absolute-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60401 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=mrca-uncertainty-relative-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85089 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=strata-retained-frac-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    88742 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=strata-retained-num-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    83927 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=stratum-retention-dripplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60937 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=mrca-uncertainty-absolute-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60008 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=mrca-uncertainty-relative-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    91737 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=strata-retained-frac-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)   136543 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=strata-retained-num-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    80779 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=stratum-retention-dripplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56714 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=mrca-uncertainty-absolute-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    69617 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=mrca-uncertainty-relative-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85268 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=strata-retained-frac-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    93241 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=strata-retained-num-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    81212 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=stratum-retention-dripplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60777 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=mrca-uncertainty-absolute-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    59070 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=mrca-uncertainty-relative-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68434 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=strata-retained-frac-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    48191 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=strata-retained-num-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    75488 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=stratum-retention-dripplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56655 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=mrca-uncertainty-absolute-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53214 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=mrca-uncertainty-relative-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    74082 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=strata-retained-frac-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51752 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=strata-retained-num-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    81657 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=stratum-retention-dripplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    59065 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=mrca-uncertainty-absolute-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56729 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=mrca-uncertainty-relative-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71884 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=strata-retained-frac-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52659 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=strata-retained-num-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    75944 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=stratum-retention-dripplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56679 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=mrca-uncertainty-absolute-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57055 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=mrca-uncertainty-relative-barplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    75986 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=strata-retained-frac-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57295 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=strata-retained-num-lineplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    80650 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=stratum-retention-dripplot+ext=.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32103 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/pruning.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31068 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/pruning_distribution.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46766 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/pruning_intensity.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34644 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/assets/stratigraph_inference.png
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5936 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/index_stage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/index_stage2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-22 05:24:26.000000 hstrat-1.7.3/docs/indices.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:13.987606 hstrat-1.7.3/hstrat/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.015606 hstrat-1.7.3/hstrat/_auxiliary_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_AnyTreeAscendingIter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_AnyTreeFastLeafIter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_AnyTreeFastLevelOrderIter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_AnyTreeFastPostOrderIter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_AnyTreeFastPreOrderIter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_BioPhyloTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_CopyableSeriesItemsIter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_HereditaryStratigraphicArtifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_RecursionLimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_RngStateContext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_ScalarFormatterFixedPrecision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_aggregate_phylogenies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_assign_contiguous_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_assign_root_ancestor_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_collapse_unifurcations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_convert_root_ancestor_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_find_chronological_inconsistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_find_leaf_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_find_root_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_has_compact_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_has_contiguous_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_has_multiple_roots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_is_asexual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_is_chronologically_ordered.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_is_sexual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_is_topologically_sorted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_make_ancestor_id_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_make_ancestor_list_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_make_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_parse_ancestor_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_parse_ancestor_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_reroot_at_id_asexual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_splay_polytomies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_to_working_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_topological_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_try_add_ancestor_id_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_unfurl_lineage_asexual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_all_same.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_all_unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_anynode_deepcopy_except_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_anytree_calc_leaf_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_anytree_cardinality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_anytree_has_grandparent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_anytree_has_sibling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_anytree_iterative_deepcopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_anytree_peel_sibling_to_cousin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_anytree_tree_to_alife_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_apply_swaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_argsort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_as_compact_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_as_nullable_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_assign_intersecting_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_bit_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_bit_floor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_capitalize_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_caretdown_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_caretup_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_check_testing_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_cmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_cmp_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_consume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_coshuffled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_count_unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_curried_binary_search_jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_deep_listify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_demark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_div_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_find_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_flag_last.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_flat_len.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_generate_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_generate_omission_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_get_hstrat_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_get_nullable_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_get_nullable_vals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_give_len.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_indices_of_unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_intersect_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_is_base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_is_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_is_in_coverage_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_is_in_unit_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_is_nondecreasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_is_nonincreasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_is_strictly_decreasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_is_strictly_increasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_is_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_iter_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_iter_monotonic_equivalencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_iter_monotonic_equivalencies_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_iter_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_jit_numba_dict_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_jit_numba_integer_array_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_jit_numpy_bool_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_jit_numpy_int64_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_launder_impl_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_log_once_in_a_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_make_intersecting_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_memoize_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_min_array_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_numpy_fromiter_polyfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_numpy_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_numpy_index_flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_omit_last.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_parse_from_numeral_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_popcount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_raises.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_random_choice_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_release_cur_mpl_fig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_render_to_base64url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_render_to_numeral_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_reversed_enumerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_reversed_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_scale_luminosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_seed_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_splicewhile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_swap_rows_and_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_to_tril.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_unfurl_lineage_with_contiguous_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_unpairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_unzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_with_omission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_with_rng_state_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/_auxiliary_lib/_zip_strict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.015606 hstrat-1.7.3/hstrat/frozen_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/frozen_instrumentation/_HereditaryStratigraphicAssemblage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/frozen_instrumentation/_HereditaryStratigraphicAssemblageSpecimen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/frozen_instrumentation/_HereditaryStratigraphicSpecimen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/frozen_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.019606 hstrat-1.7.3/hstrat/genome_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)    22118 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/genome_instrumentation/_HereditaryStratigraphicColumn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/genome_instrumentation/_HereditaryStratigraphicColumnBundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/genome_instrumentation/_HereditaryStratum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/genome_instrumentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.019606 hstrat-1.7.3/hstrat/genome_instrumentation/stratum_ordered_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/genome_instrumentation/stratum_ordered_stores/_HereditaryStratumOrderedStoreDict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/genome_instrumentation/stratum_ordered_stores/_HereditaryStratumOrderedStoreList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15003 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/genome_instrumentation/stratum_ordered_stores/_HereditaryStratumOrderedStoreTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/genome_instrumentation/stratum_ordered_stores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.019606 hstrat-1.7.3/hstrat/genome_instrumentation/stratum_ordered_stores/_detail/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/genome_instrumentation/stratum_ordered_stores/_detail/_HereditaryStratumOrderedStoreBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/genome_instrumentation/stratum_ordered_stores/_detail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.019606 hstrat-1.7.3/hstrat/hstrat/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/hstrat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.023606 hstrat-1.7.3/hstrat/juxtaposition/
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_calc_definitive_max_rank_of_first_retained_disparity_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_calc_definitive_max_rank_of_last_retained_commonality_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_calc_definitive_min_ranks_since_first_retained_disparity_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_calc_definitive_min_ranks_since_last_retained_commonality_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_calc_min_implausible_spurious_consecutive_differentia_collisions_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_calc_probability_differentia_collision_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_calc_rank_of_first_retained_disparity_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_calc_rank_of_last_retained_commonality_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_calc_ranks_since_first_retained_disparity_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_calc_ranks_since_last_retained_commonality_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_diff_retained_ranks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_get_last_common_stratum_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_get_nth_common_rank_between.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.023606 hstrat-1.7.3/hstrat/juxtaposition/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl/_dispatch_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.023606 hstrat-1.7.3/hstrat/juxtaposition/_impl_column/
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl_column/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl_column/_calc_rank_of_first_retained_disparity_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl_column/_calc_rank_of_first_retained_disparity_between_bsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl_column/_calc_rank_of_first_retained_disparity_between_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl_column/_calc_rank_of_last_retained_commonality_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl_column/_calc_rank_of_last_retained_commonality_between_bsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl_column/_calc_rank_of_last_retained_commonality_between_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl_column/_calc_rank_of_parity_segue_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl_column/_iter_mutual_ranks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl_column/_iter_ranks_of_retained_commonality_between.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.023606 hstrat-1.7.3/hstrat/juxtaposition/_impl_specimen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl_specimen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl_specimen/_calc_rank_of_first_retained_disparity_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl_specimen/_calc_rank_of_last_retained_commonality_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl_specimen/_calc_rank_of_parity_segue_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl_specimen/_calc_rank_of_parity_segue_between_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl_specimen/_iter_mutual_rank_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl_specimen/_iter_mutual_ranks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/juxtaposition/_impl_specimen/_iter_ranks_of_retained_commonality_between.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.027607 hstrat-1.7.3/hstrat/phylogenetic_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.027607 hstrat-1.7.3/hstrat/phylogenetic_inference/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/estimators/_estimate_rank_of_mrca_maximum_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/estimators/_estimate_rank_of_mrca_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/estimators/_estimate_rank_of_mrca_unbiased.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.031607 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_ballpark_patristic_distance_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_ballpark_rank_of_mrca_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_ballpark_ranks_since_mrca_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_calc_patristic_distance_bounds_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_calc_rank_of_earliest_detectable_mrca_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_calc_rank_of_mrca_bounds_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_calc_rank_of_mrca_bounds_provided_confidence_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_calc_rank_of_mrca_uncertainty_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_calc_ranks_since_earliest_detectable_mrca_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_calc_ranks_since_mrca_bounds_provided_confidence_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_calc_ranks_since_mrca_bounds_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_calc_ranks_since_mrca_uncertainty_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_does_definitively_have_no_common_ancestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_does_have_any_common_ancestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_estimate_patristic_distance_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_estimate_rank_of_mrca_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_estimate_ranks_since_mrca_with.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.031607 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_impl/_estimate_rank_of_mrca_maximum_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_impl/_estimate_rank_of_mrca_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_impl/_estimate_rank_of_mrca_unbiased.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_impl/_extract_common_retained_ranks_through_first_retained_disparity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.031607 hstrat-1.7.3/hstrat/phylogenetic_inference/population/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/population/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/population/_build_distance_matrix_biopython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/population/_build_distance_matrix_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/population/_calc_rank_of_earliest_detectable_mrca_among.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/population/_calc_rank_of_mrca_bounds_among.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/population/_calc_rank_of_mrca_uncertainty_among.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/population/_does_definitively_share_no_common_ancestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/population/_does_share_any_common_ancestor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.031607 hstrat-1.7.3/hstrat/phylogenetic_inference/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/priors/_ArbitraryPrior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/priors/_BubbleWrappedPrior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/priors/_ExponentialPrior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/priors/_GeometricPrior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/priors/_UniformPrior.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/priors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.035607 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_build_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_build_tree_nj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_build_tree_trie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_build_tree_trie_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_build_tree_upgma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.035607 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)    10945 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/_TrieInnerNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/_TrieLeafNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/_append_genesis_organism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/_build_tree_biopython_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/_build_trie_from_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/_estimate_origin_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/_find_chronological_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/_find_chronological_roots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/_time_calibrate_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.035607 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/trie_postprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/trie_postprocess/_AssignDestructionTimeYoungestPlusOneTriePostprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/trie_postprocess/_AssignOriginTimeExpectedValueTriePostprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/trie_postprocess/_AssignOriginTimeNaiveTriePostprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/trie_postprocess/_AssignOriginTimeNodeRankTriePostprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/trie_postprocess/_CompoundTriePostprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/trie_postprocess/_PeelBackConjoinedLeavesTriePostprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/trie_postprocess/_SampleAncestralRollbacksTriePostprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/phylogenetic_inference/tree/trie_postprocess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.039607 hstrat-1.7.3/hstrat/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/serialization/_assemblage_from_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/serialization/_col_from_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/serialization/_col_to_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/serialization/_col_to_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/serialization/_col_to_specimen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.039607 hstrat-1.7.3/hstrat/serialization/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/serialization/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/serialization/_impl/_col_records_from_pop_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/serialization/_impl/_policy_from_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/serialization/_pack_differentiae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/serialization/_pop_from_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/serialization/_pop_to_assemblage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/serialization/_pop_to_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/serialization/_pop_to_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/serialization/_specimen_from_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/serialization/_unassemblage_from_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/serialization/_unpack_differentiae.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.039607 hstrat-1.7.3/hstrat/stratum_retention_strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.039607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.039607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_detail/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_detail/_PolicyCouplerBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_detail/_PolicyCouplerFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_detail/_PolicySpecBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_detail/_UnsatisfiableParameterizationRequestError.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_detail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.039607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyAbsUpperBoundPessimalRankBruteForce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyAbsUpperBoundWorstCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyRelExactFromAbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyRelUpperBoundPessimalRankBruteForce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyRelUpperBoundWorstCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcNumStrataRetainedUpperBoundWorstCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_GenDropRanksFromPredKeepRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.039607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_PolicySpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.039607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_enact/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_enact/_GenDropRanks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.039607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_enact/_GenDropRanks_/
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_enact/_GenDropRanks_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_enact/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.043607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_impl/_calc_provided_uncertainty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.043607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.043607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.043607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_PolicySpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.043607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_enact/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_enact/_GenDropRanks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.043607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_enact/_GenDropRanks_/
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_enact/_GenDropRanks_/_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_enact/_GenDropRanks_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_enact/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.043607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_impl/_calc_provided_uncertainty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.047607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.047607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.047607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_PolicySpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.047607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_enact/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_enact/_GenDropRanks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.047607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_enact/_GenDropRanks_/
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_enact/_GenDropRanks_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_enact/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.047607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.047607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.051607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_PolicySpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.051607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_enact/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_enact/_GenDropRanks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.051607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_enact/_GenDropRanks_/
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_enact/_GenDropRanks_/_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_enact/_GenDropRanks_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_enact/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.051607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_calc_common_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_get_retained_ranks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_rank_backstops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_rank_cutoffs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_rank_seps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_target_ranks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_target_recencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.051607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.051607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.051607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_PolicySpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.055607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_enact/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_enact/_GenDropRanks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.055607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_enact/_GenDropRanks_/
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_enact/_GenDropRanks_/_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_enact/_GenDropRanks_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_enact/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.055607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_common_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_rank_backstop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_rank_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_rank_sep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_target_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_target_recency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_get_retained_ranks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_iter_priority_ranks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.055607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.055607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.055607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_PolicySpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.055607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_enact/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_enact/_GenDropRanks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.063607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_enact/_GenDropRanks_/
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_enact/_GenDropRanks_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_enact/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.063607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.063607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.067607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_PolicySpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.071607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_enact/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_enact/_GenDropRanks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.071607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_enact/_GenDropRanks_/
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_enact/_GenDropRanks_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_enact/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.075607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.075607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.075607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_PolicySpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.075607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_enact/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_enact/_GenDropRanks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.075607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_enact/_GenDropRanks_/
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_enact/_GenDropRanks_/_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_enact/_GenDropRanks_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_enact/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.075607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_impl/_decide_if_discard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.079607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.079607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_scry/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_scry/_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_scry/_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_scry/_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_scry/_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_scry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.083607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_PolicySpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.083607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_enact/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_enact/_GenDropRanks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.087607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_enact/_GenDropRanks_/
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_enact/_GenDropRanks_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_enact/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.087607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_impl/_calc_provided_uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_impl/_num_to_condemn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.091607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.095607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.095607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_PolicySpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.099607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_impl/_calc_geom_seq_nth_root_transition_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_impl/_calc_provided_degree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_impl/_calc_provided_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_impl/_pick_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.099607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_PolicySpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.099607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_enact/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_enact/_GenDropRanks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.099607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_enact/_GenDropRanks_/
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_enact/_GenDropRanks_/_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_enact/_GenDropRanks_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_enact/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.103607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_impl/_decide_if_discard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.103607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.107607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_scry/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_scry/_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_scry/_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_scry/_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_scry/_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_scry/_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_scry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.111607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_MrcaUncertaintyAbsExactEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_MrcaUncertaintyAbsUpperBoundEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_MrcaUncertaintyRelExactEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_MrcaUncertaintyRelUpperBoundEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_NumStrataRetainedExactEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_NumStrataRetainedUpperBoundEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.111607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_detail/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_detail/_policy_param_focalizer_t.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.111607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/_PropertyAtLeastParameterizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/_PropertyAtMostParameterizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/_PropertyExactlyParameterizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.111607 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/_detail/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/_detail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/_detail/_policy_evaluator_t.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.111607 hstrat-1.7.3/hstrat/stratum_retention_viz/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_viz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.111607 hstrat-1.7.3/hstrat/stratum_retention_viz/animate/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_viz/animate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_viz/animate/_policy_panel_animate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_viz/animate/_stratum_retention_animate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.111607 hstrat-1.7.3/hstrat/stratum_retention_viz/ascii/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_viz/ascii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_viz/ascii/_col_to_ascii.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.115607 hstrat-1.7.3/hstrat/stratum_retention_viz/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_viz/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_viz/plot/_mrca_uncertainty_absolute_barplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_viz/plot/_mrca_uncertainty_relative_barplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_viz/plot/_policy_panel_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_viz/plot/_strata_retained_frac_lineplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_viz/plot/_strata_retained_num_lineplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7219 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/stratum_retention_viz/plot/_stratum_retention_dripplot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.115607 hstrat-1.7.3/hstrat/test_drive/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.115607 hstrat-1.7.3/hstrat/test_drive/descend_template_phylogeny/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/descend_template_phylogeny/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_alifestd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_biopython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_dendropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_networkx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_posthoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.115607 hstrat-1.7.3/hstrat/test_drive/generate_template_phylogeny/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/generate_template_phylogeny/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8873 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.119607 hstrat-1.7.3/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/_apply_island_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/_apply_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/_apply_niche_invasions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/_get_island_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/_get_niche_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/_select_parents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.119607 hstrat-1.7.3/hstrat/test_drive/perfect_tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/perfect_tracking/_DecantingPhyloTracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/perfect_tracking/_GarbageCollectingPhyloTracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.119607 hstrat-1.7.3/hstrat/test_drive/perfect_tracking/_GarbageCollectingPhyloTracker_/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/perfect_tracking/_GarbageCollectingPhyloTracker_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/perfect_tracking/_GarbageCollectingPhyloTracker_/_discern_referenced_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/perfect_tracking/_PerfectBacktrackHandle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/perfect_tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/perfect_tracking/_compile_perfect_backtrack_phylogeny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/perfect_tracking/_compile_phylogeny_from_lineage_iters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-22 05:24:26.000000 hstrat-1.7.3/hstrat/test_drive/perfect_tracking/_iter_perfect_backtrack_lineage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:13.987606 hstrat-1.7.3/hstrat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    68177 2023-06-22 05:25:13.000000 hstrat-1.7.3/hstrat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)   124850 2023-06-22 05:25:13.000000 hstrat-1.7.3/hstrat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 05:25:13.000000 hstrat-1.7.3/hstrat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-22 05:25:13.000000 hstrat-1.7.3/hstrat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 05:25:13.000000 hstrat-1.7.3/hstrat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-22 05:24:26.000000 hstrat-1.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-22 05:25:14.259609 hstrat-1.7.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      195 2023-06-22 05:24:26.000000 hstrat-1.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.119607 hstrat-1.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.123607 hstrat-1.7.3/tests/test_hstrat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.127607 hstrat-1.7.3/tests/test_hstrat/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/assets/grandchild.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/assets/grandchild_and_aunt.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/assets/grandchild_and_auntuncle.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/assets/grandtriplets.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/assets/grandtriplets_and_aunt.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/assets/grandtriplets_and_auntuncle.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/assets/grandtwins.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/assets/grandtwins_and_aunt.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/assets/grandtwins_and_auntuncle.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/assets/greatgrandtwins_and_auntuncle.newick
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/assets/justroot.newick
+-rw-r--r--   0 runner    (1001) docker     (123)   110110 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/assets/nk_ecoeaselection.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    50218 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/assets/nk_lexicaseselection.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/assets/nk_tournamentselection.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/assets/onlychild.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/assets/triplets.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/assets/twins.newick
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/run_tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.155608 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.167608 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-ancestor_list-syntax1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-ancestor_list-syntax2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-ancestor_list-syntax3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-ancestor_list-syntax4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-duplicate-id1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-duplicate-id2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-duplicate-id3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-mismatched-ancestor_id-ancestor_list-columns1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-mismatched-ancestor_id-ancestor_list-columns2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-mismatched-ancestor_id-ancestor_list-columns3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-missing-ancestor_list-column1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-missing-ancestor_list-column2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-missing-id-column.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-negative-id1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-negative-id2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-negative-id3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-nonexistant-ancestor_id-id1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-nonexistant-ancestor_id-id2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-nonexistant-ancestor_id-id3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-nonexistant-ancestor_id-id4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny--invalid-nonexistant-ancestor_list-id.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny-empty-list-notation.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny-noncompact1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny-noncompact2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny-uniq.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-asexual-phylogeny.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-ancestor_list-syntax1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-ancestor_list-syntax2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-ancestor_list-syntax3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-ancestor_list-syntax4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-duplicate-id1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-duplicate-id2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-duplicate-id3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-mismatched-ancestor_id-ancestor_list-columns1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-mismatched-ancestor_id-ancestor_list-columns2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-missing-id-column.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-negative-id1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-negative-id2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-negative-id3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny--invalid-nonexistant-ancestor_list-id.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny-empty-list-notation.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny-noncompact1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny-noncompact2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny-uniq.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/example-standard-toy-sexual-phylogeny.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   110110 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/nk_ecoeaselection.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    50218 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/nk_lexicaseselection.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/nk_tournamentselection.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeAscendingIter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeFastLeafIter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeFastLevelOrderIter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeFastPostOrderIter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeFastPreOrderIter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_CopyableSeriesItemsIter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_HereditaryStratigraphicArtifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_RngStateContext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_aggregate_phylogenies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_assign_contiguous_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_assign_root_ancestor_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_collapse_unifurcations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_convert_root_ancestor_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_find_chronological_inconsistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_find_leaf_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_find_root_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_has_compact_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_has_contiguous_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_has_multiple_roots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_is_asexual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_is_chronologically_ordered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_is_sexual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8858 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_is_topologically_sorted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_make_ancestor_id_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_make_ancestor_list_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_make_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_parse_ancestor_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_parse_ancestor_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_reroot_at_id_asexual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_splay_polytomies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_to_working_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_topological_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_try_add_ancestor_id_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_unfurl_lineage_asexual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10407 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_all_same.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_all_unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_anynode_deepcopy_except_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_anytree_calc_leaf_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_anytree_cardinality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_anytree_has_grandparent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_anytree_has_sibling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_anytree_iterative_deepcopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_anytree_peel_sibling_to_cousin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_anytree_tree_to_alife_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_apply_swaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_argsort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_as_compact_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_as_nullable_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_assign_intersecting_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_bit_ceil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_bit_floor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_capitalize_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_cmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_cmp_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_consume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_coshuffled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_count_unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_curried_binary_search_jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_deep_listify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_demark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_div_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_find_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_flag_last.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_flat_len.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_generate_n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_generate_omission_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_get_hstrat_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_get_nullable_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_get_nullable_vals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_give_len.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_indices_of_unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_intersect_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_is_base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_is_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_is_nondecreasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_is_nonincreasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_is_strictly_decreasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_is_strictly_increasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_is_subset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_iter_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_iter_monotonic_equivalencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_iter_monotonic_equivalencies_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_iter_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_make_intersecting_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_memoize_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_min_array_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_numpy_fromiter_polyfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_numpy_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_numpy_index_flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_omit_last.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_pairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_parse_from_numeral_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_popcount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_raises.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_random_choice_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_render_to_base64url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_render_to_numeral_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_reversed_enumerate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_reversed_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_seed_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_splicewhile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_swap_rows_and_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_to_tril.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_unfurl_lineage_with_contiguous_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_unpairwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_unzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_with_omission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_with_rng_state_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_zip_strict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.167608 hstrat-1.7.3/tests/test_hstrat/test_frozen_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_frozen_instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_frozen_instrumentation/test_HereditaryStratigraphicAssemblage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_frozen_instrumentation/test_HereditaryStratigraphicAssemblageSpecimen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_frozen_instrumentation/test_HereditaryStratigraphicSpecimen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.167608 hstrat-1.7.3/tests/test_hstrat/test_genome_instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_genome_instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27700 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_genome_instrumentation/test_HereditaryStratigraphicColumn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_genome_instrumentation/test_HereditaryStratigraphicColumnBundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_genome_instrumentation/test_HereditaryStratum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.167608 hstrat-1.7.3/tests/test_hstrat/test_genome_instrumentation/test_stratum_ordered_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_genome_instrumentation/test_stratum_ordered_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16916 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_genome_instrumentation/test_stratum_ordered_stores/test_HereditaryStratumOrderedStoreDict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16821 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_genome_instrumentation/test_stratum_ordered_stores/test_HereditaryStratumOrderedStoreList.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19044 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_genome_instrumentation/test_stratum_ordered_stores/test_HereditaryStratumOrderedStoreTree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.171608 hstrat-1.7.3/tests/test_hstrat/test_hstrat/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_hstrat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_hstrat/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.171608 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_definitive_max_rank_of_first_retained_disparity_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_definitive_max_rank_of_last_retained_commonality_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_definitive_min_ranks_since_first_retained_disparity_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_definitive_min_ranks_since_last_retained_commonality_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_min_implausible_spurious_consecutive_differentia_collisions_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_probability_differentia_collision_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34817 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_rank_of_first_retained_disparity_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28695 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_rank_of_last_retained_commonality_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_ranks_since_first_retained_disparity_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15682 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_ranks_since_last_retained_commonality_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_diff_retained_ranks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_get_last_common_stratum_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_get_nth_common_rank_between.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.175608 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_impl/test_dispatch_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.175608 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_impl_column/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_impl_column/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22298 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_impl_column/test_iter_ranks_of_retained_commonality_between_generic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.175608 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_impl_specimen/
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_impl_specimen/test_calc_rank_of_first_retained_disparity_between_specimen_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_impl_specimen/test_calc_rank_of_last_retained_commonality_between_specimen_naive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.175608 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.175608 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_estimators/test_estimate_rank_of_mrca_maximum_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_estimators/test_estimate_rank_of_mrca_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_estimators/test_estimate_rank_of_mrca_unbiased.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.179608 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_ballpark_patristic_distance_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_ballpark_rank_of_mrca_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_ballpark_ranks_since_mrca_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_patristic_distance_bounds_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_rank_of_earliest_detectable_mrca_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22500 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_rank_of_mrca_bounds_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_rank_of_mrca_bounds_provided_confidence_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18837 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_rank_of_mrca_uncertainty_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_ranks_since_earliest_detectable_mrca_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_ranks_since_mrca_bounds_provided_confidence_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18764 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_ranks_since_mrca_bounds_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_ranks_since_mrca_uncertainty_with.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_does_definitively_have_no_common_ancestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_does_have_any_common_ancestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14073 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_estimate_patristic_distance_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28321 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_estimate_rank_of_mrca_between.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_estimate_ranks_since_mrca_with.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.183608 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_population/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_population/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_population/test_build_distance_matrix_biopython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_population/test_build_distance_matrix_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_population/test_calc_rank_of_earliest_detectable_mrca_among.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23442 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_population/test_calc_rank_of_mrca_bounds_among.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23811 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_population/test_calc_rank_of_mrca_uncertainty_among.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_population/test_does_definitively_share_no_common_ancestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_population/test_does_share_any_common_ancestor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.183608 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_priors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_priors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_ArbitraryPrior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_BubbleWrappedPrior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_ExponentialPrior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_GeometricPrior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_UniformPrior.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.187608 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.187608 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/_descend_unifurcations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/_load_dendropy_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/_setup_dendropy_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/_tree_quartet_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/_tree_unweighted_robinson_foulds_distance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.191608 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/grandchild.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/grandchild_and_aunt.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/grandchild_and_auntuncle.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/grandtriplets.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/grandtriplets_and_aunt.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/grandtriplets_and_auntuncle.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/grandtwins.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/grandtwins_and_aunt.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/grandtwins_and_auntuncle.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/greatgrandtwins_and_auntuncle.newick
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/justroot.newick
+-rw-r--r--   0 runner    (1001) docker     (123)   110110 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/nk_ecoeaselection.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    50218 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/nk_lexicaseselection.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/nk_tournamentselection.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/onlychild.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/triplets.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/twins.newick
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree_nj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15756 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree_trie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree_trie_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree_upgma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.191608 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)    12148 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_TrieInnerNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_TrieLeafNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_append_genesis_organism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_estimate_origin_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_find_chronological_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_find_chronological_roots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_time_calibrate_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.195608 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_AssignDestructionTimeYoungestPlusOneTriePostprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11731 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_AssignOriginTimeExpectedValueTriePostprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_AssignOriginTimeNaiveTriePostprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_AssignOriginTimeNodeRankTriePostprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_CompoundTriePostprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_PeelBackConjoinedLeavesTriePostprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_SampleAncestralRollbacksTriePostprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_bias_adjustment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.199608 hstrat-1.7.3/tests/test_hstrat/test_serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_serialization/test_assemblage_from_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_serialization/test_col_to_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_serialization/test_col_to_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_serialization/test_col_to_specimen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.199608 hstrat-1.7.3/tests/test_hstrat/test_serialization/test_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_serialization/test_impl/test_col_records_from_pop_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_serialization/test_pack_differentiae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_serialization/test_pop_to_assemblage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_serialization/test_pop_to_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_serialization/test_pop_to_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_serialization/test_specimen_from_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_serialization/test_unassemblage_from_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_serialization/test_unpack_differentiae.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.199608 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.199608 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.203608 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_PolicySpec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.207608 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_PolicySpec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.211608 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_PolicySpec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.215608 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7837 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_PolicySpec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.219608 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_PolicySpec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.223608 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_PolicySpec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.227608 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_PolicySpec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.231608 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_PolicySpec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.235608 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_PolicySpec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.239609 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.239609 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/impl/iter_backing_policy_transition_ranks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcRankAtColumnIndex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.239609 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_GenDropRanks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_GenDropRanks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_GenDropRanks/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_GenDropRanks/test_impl_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_GenDropRanks/test_policy_consistency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.243609 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_backing_policy_transition_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_eq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_implementation_consistency_at_backing_policy_transitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_only_dwindling_over_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_ranks_sorted_and_unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_ranks_valid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_zero_and_last_ranks_retained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_PolicySpec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.243609 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_impl/test_calc_geom_seq_nth_root_transition_rank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_impl/test_iter_backing_policy_transition_ranks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.247609 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyAbsExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyAbsUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyRelExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyRelUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcNumStrataRetainedExact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcNumStrataRetainedUpperBound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcRankAtColumnIndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_GenDropRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_IterRetainedRanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_PolicySpec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.247609 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18532 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_MrcaUncertaintyAbsExactEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_MrcaUncertaintyAbsUpperBoundEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19284 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_MrcaUncertaintyRelExactEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19242 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_MrcaUncertaintyRelUpperBoundEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_NumStrataRetainedExactEvaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_NumStrataRetainedUpperBoundEvaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.247609 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.251609 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_animate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_animate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_animate/test_policy_panel_animate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_animate/test_stratum_retention_animate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.251609 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_mrca_uncertainty_absolute_barplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_mrca_uncertainty_relative_barplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_policy_panel_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_strata_retained_frac_lineplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_strata_retained_num_lineplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_stratum_retention_dripplot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.255609 hstrat-1.7.3/tests/test_hstrat/test_test_drive/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:25:14.259609 hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/grandchild.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/grandchild_and_aunt.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/grandchild_and_auntuncle.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/grandtriplets.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/grandtriplets_and_aunt.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/grandtriplets_and_auntuncle.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/grandtwins.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/grandtwins_and_aunt.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/grandtwins_and_auntuncle.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/greatgrandtwins_and_auntuncle.newick
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/justroot.newick
+-rw-r--r--   0 runner    (1001) docker     (123)   110110 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/nk_ecoeaselection.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    50218 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/nk_lexicaseselection.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/nk_tournamentselection.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/onlychild.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/triplets.newick
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/twins.newick
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_DecantingPhyloTracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_GarbageCollectingPhyloTracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_alifestd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_biopython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10085 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_dendropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_networkx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_posthoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_evolve_fitness_trait_population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-22 05:24:26.000000 hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_perfect_tracking.py
```

### Comparing `hstrat-1.7.2/CONTRIBUTING.rst` & `hstrat-1.7.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/LICENSE` & `hstrat-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/PKG-INFO` & `hstrat-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6873 7472  : 2.1.Name: hstr
 00000020: 6174 0a56 6572 7369 6f6e 3a20 312e 372e  at.Version: 1.7.
-00000030: 320a 5375 6d6d 6172 793a 2068 7374 7261  2.Summary: hstra
+00000030: 330a 5375 6d6d 6172 793a 2068 7374 7261  3.Summary: hstra
 00000040: 7420 656e 6162 6c65 7320 7068 796c 6f67  t enables phylog
 00000050: 656e 6574 6963 2069 6e66 6572 656e 6365  enetic inference
 00000060: 206f 6e20 6469 7374 7269 6275 7465 6420   on distributed 
 00000070: 6469 6769 7461 6c20 6576 6f6c 7574 696f  digital evolutio
 00000080: 6e20 706f 7075 6c61 7469 6f6e 730a 4175  n populations.Au
 00000090: 7468 6f72 2d65 6d61 696c 3a20 4d61 7474  thor-email: Matt
 000000a0: 6865 7720 416e 6472 6573 204d 6f72 656e  hew Andres Moren
```

### Comparing `hstrat-1.7.2/README.md` & `hstrat-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/Makefile` & `hstrat-1.7.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/_templates/autosummary/class.rst` & `hstrat-1.7.3/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/_templates/autosummary/module.rst` & `hstrat-1.7.3/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/bitstring_inference.png` & `hstrat-1.7.3/docs/assets/bitstring_inference.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/hcat-banner.png` & `hstrat-1.7.3/docs/assets/hcat-banner.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/hcat.png` & `hstrat-1.7.3/docs/assets/hcat.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/hstrat-hcat.png` & `hstrat-1.7.3/docs/assets/hstrat-hcat.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/hstrat-wordmark.png` & `hstrat-1.7.3/docs/assets/hstrat-wordmark.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=mrca-uncertainty-absolute-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=mrca-uncertainty-absolute-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=mrca-uncertainty-relative-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=mrca-uncertainty-relative-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=strata-retained-frac-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=strata-retained-frac-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=strata-retained-num-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=strata-retained-num-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=stratum-retention-dripplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-19+viz=stratum-retention-dripplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=mrca-uncertainty-absolute-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=mrca-uncertainty-absolute-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=mrca-uncertainty-relative-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=mrca-uncertainty-relative-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=strata-retained-frac-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=strata-retained-frac-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=strata-retained-num-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=strata-retained-num-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=stratum-retention-dripplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-79+viz=stratum-retention-dripplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=mrca-uncertainty-absolute-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=mrca-uncertainty-absolute-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=mrca-uncertainty-relative-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=mrca-uncertainty-relative-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=strata-retained-frac-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=strata-retained-frac-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=strata-retained-num-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=strata-retained-num-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=stratum-retention-dripplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=curbed-recency-proportional-resolution-stratum-retention-algorithm-size-curb-8+viz=stratum-retention-dripplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=mrca-uncertainty-absolute-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=mrca-uncertainty-absolute-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=mrca-uncertainty-relative-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=mrca-uncertainty-relative-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=strata-retained-frac-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=strata-retained-frac-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=strata-retained-num-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=strata-retained-num-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=stratum-retention-dripplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-2+viz=stratum-retention-dripplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=mrca-uncertainty-absolute-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=mrca-uncertainty-absolute-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=mrca-uncertainty-relative-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=mrca-uncertainty-relative-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=strata-retained-frac-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=strata-retained-frac-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=strata-retained-num-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=strata-retained-num-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=stratum-retention-dripplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=depth-proportional-resolution-stratum-retention-algorithm-resolution-8+viz=stratum-retention-dripplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=mrca-uncertainty-absolute-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=mrca-uncertainty-absolute-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=mrca-uncertainty-relative-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=mrca-uncertainty-relative-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=strata-retained-frac-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=strata-retained-frac-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=strata-retained-num-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=strata-retained-num-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=stratum-retention-dripplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-128+viz=stratum-retention-dripplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=mrca-uncertainty-absolute-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=mrca-uncertainty-absolute-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=mrca-uncertainty-relative-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=mrca-uncertainty-relative-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=strata-retained-frac-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=strata-retained-frac-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=strata-retained-num-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=strata-retained-num-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=stratum-retention-dripplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=fixed-resolution-stratum-retention-algorithm-resolution-32+viz=stratum-retention-dripplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=mrca-uncertainty-absolute-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=mrca-uncertainty-absolute-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=mrca-uncertainty-relative-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=mrca-uncertainty-relative-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=strata-retained-frac-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=strata-retained-frac-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=strata-retained-num-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=strata-retained-num-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=stratum-retention-dripplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-1024-interspersal-2+viz=stratum-retention-dripplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=mrca-uncertainty-absolute-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=mrca-uncertainty-absolute-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=mrca-uncertainty-relative-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=mrca-uncertainty-relative-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=strata-retained-frac-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=strata-retained-frac-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=strata-retained-num-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=strata-retained-num-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=stratum-retention-dripplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=nth-root-geometric-sequence-stratum-retention-algorithm-degree-6-interspersal-2+viz=stratum-retention-dripplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=mrca-uncertainty-absolute-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=mrca-uncertainty-absolute-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=mrca-uncertainty-relative-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=mrca-uncertainty-relative-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=strata-retained-frac-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=strata-retained-frac-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=strata-retained-num-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=strata-retained-num-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=stratum-retention-dripplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-0+viz=stratum-retention-dripplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=mrca-uncertainty-absolute-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=mrca-uncertainty-absolute-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=mrca-uncertainty-relative-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=mrca-uncertainty-relative-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=strata-retained-frac-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=strata-retained-frac-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=strata-retained-num-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=strata-retained-num-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=stratum-retention-dripplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=recency-proportional-resolution-stratum-retention-algorithm-resolution-6+viz=stratum-retention-dripplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=mrca-uncertainty-absolute-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=mrca-uncertainty-absolute-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=mrca-uncertainty-relative-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=mrca-uncertainty-relative-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=strata-retained-frac-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=strata-retained-frac-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=strata-retained-num-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=strata-retained-num-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=stratum-retention-dripplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-1+viz=stratum-retention-dripplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=mrca-uncertainty-absolute-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=mrca-uncertainty-absolute-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=mrca-uncertainty-relative-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=mrca-uncertainty-relative-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=strata-retained-frac-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=strata-retained-frac-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=strata-retained-num-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=strata-retained-num-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=stratum-retention-dripplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-depth-proportional-resolution-stratum-retention-algorithm-resolution-7+viz=stratum-retention-dripplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=mrca-uncertainty-absolute-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=mrca-uncertainty-absolute-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=mrca-uncertainty-relative-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=mrca-uncertainty-relative-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=strata-retained-frac-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=strata-retained-frac-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=strata-retained-num-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=strata-retained-num-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=stratum-retention-dripplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-1-interspersal-2+viz=stratum-retention-dripplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=mrca-uncertainty-absolute-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=mrca-uncertainty-absolute-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=mrca-uncertainty-relative-barplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=mrca-uncertainty-relative-barplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=strata-retained-frac-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=strata-retained-frac-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=strata-retained-num-lineplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=strata-retained-num-lineplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=stratum-retention-dripplot+ext=.png` & `hstrat-1.7.3/docs/assets/num_generations=256+policy=tapered-nth-root-geometric-sequence-stratum-retention-algorithm-degree-4-interspersal-2+viz=stratum-retention-dripplot+ext=.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/pruning.png` & `hstrat-1.7.3/docs/assets/pruning.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/pruning_distribution.png` & `hstrat-1.7.3/docs/assets/pruning_distribution.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/pruning_intensity.png` & `hstrat-1.7.3/docs/assets/pruning_intensity.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/assets/stratigraph_inference.png` & `hstrat-1.7.3/docs/assets/stratigraph_inference.png`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/docs/conf.py` & `hstrat-1.7.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/__init__.py` & `hstrat-1.7.3/hstrat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for hstrat."""
 
 __author__ = """Matthew Andres Moreno"""
 __email__ = "m.more500@gmail.com"
-__version__ = "1.7.2"
+__version__ = "1.7.3"
 
 from . import (
     _auxiliary_lib,
     frozen_instrumentation,
     genome_instrumentation,
     juxtaposition,
     phylogenetic_inference,
```

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_AnyTreeAscendingIter.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_AnyTreeAscendingIter.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_AnyTreeFastLeafIter.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_AnyTreeFastLeafIter.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_AnyTreeFastLevelOrderIter.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_AnyTreeFastLevelOrderIter.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_AnyTreeFastPostOrderIter.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_AnyTreeFastPostOrderIter.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_AnyTreeFastPreOrderIter.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_AnyTreeFastPreOrderIter.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_BioPhyloTree.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_BioPhyloTree.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_CopyableSeriesItemsIter.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_CopyableSeriesItemsIter.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_RecursionLimit.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_RecursionLimit.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_RngStateContext.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_RngStateContext.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_ScalarFormatterFixedPrecision.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_ScalarFormatterFixedPrecision.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/__init__.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_aggregate_phylogenies.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_aggregate_phylogenies.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_assign_contiguous_ids.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_assign_contiguous_ids.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_assign_root_ancestor_token.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_assign_root_ancestor_token.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_collapse_unifurcations.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_collapse_unifurcations.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_convert_root_ancestor_token.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_convert_root_ancestor_token.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_find_chronological_inconsistency.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_find_chronological_inconsistency.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_find_leaf_ids.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_find_leaf_ids.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_is_topologically_sorted.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_is_topologically_sorted.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_make_ancestor_id_col.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_make_ancestor_id_col.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_make_ancestor_list_col.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_make_ancestor_list_col.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_reroot_at_id_asexual.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_reroot_at_id_asexual.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_splay_polytomies.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_splay_polytomies.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_to_working_format.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_to_working_format.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_topological_sort.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_topological_sort.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_try_add_ancestor_id_col.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_try_add_ancestor_id_col.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_unfurl_lineage_asexual.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_unfurl_lineage_asexual.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_alifestd_validate.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_alifestd_validate.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_anynode_deepcopy_except_neighbors.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_anynode_deepcopy_except_neighbors.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_anytree_calc_leaf_counts.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_anytree_calc_leaf_counts.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_anytree_iterative_deepcopy.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_anytree_iterative_deepcopy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_anytree_peel_sibling_to_cousin.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_anytree_peel_sibling_to_cousin.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_anytree_tree_to_alife_dataframe.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_anytree_tree_to_alife_dataframe.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_apply_swaps.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_apply_swaps.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_argsort.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_argsort.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_as_compact_type.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_as_compact_type.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_as_nullable_type.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_as_nullable_type.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_assign_intersecting_subsets.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_assign_intersecting_subsets.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_check_testing_requirements.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_check_testing_requirements.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_cmp.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_cmp.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_cmp_approx.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_cmp_approx.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_consume.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_consume.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_coshuffled.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_coshuffled.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_curried_binary_search_jit.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_curried_binary_search_jit.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_deep_listify.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_deep_listify.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_find_bounds.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_find_bounds.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_flag_last.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_flag_last.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_flat_len.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_flat_len.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_generate_n.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_generate_n.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_generate_omission_subsets.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_generate_omission_subsets.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_get_nullable_mask.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_get_nullable_mask.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_get_nullable_vals.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_get_nullable_vals.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_give_len.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_give_len.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_indices_of_unique.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_indices_of_unique.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_intersect_ranges.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_intersect_ranges.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_is_base64.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_is_base64.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_is_in.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_is_in.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_is_in_coverage_run.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_is_in_coverage_run.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_iter_chunks.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_iter_chunks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_iter_monotonic_equivalencies.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_iter_monotonic_equivalencies.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_iter_monotonic_equivalencies_reverse.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_iter_monotonic_equivalencies_reverse.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_iter_slices.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_iter_slices.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_jit.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_jit.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_jit_numba_dict_t.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_jit_numba_dict_t.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_jit_numba_integer_array_ts.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_jit_numba_integer_array_ts.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_jit_numpy_bool_t.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_jit_numpy_bool_t.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_jit_numpy_int64_t.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_jit_numpy_int64_t.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_make_intersecting_subsets.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_make_intersecting_subsets.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_memoize_generator.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_memoize_generator.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_min_array_dtype.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_min_array_dtype.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_numpy_fromiter_polyfill.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_numpy_fromiter_polyfill.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_numpy_index.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_numpy_index.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_numpy_index_flat.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_numpy_index_flat.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_pairwise.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_pairwise.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_parse_from_numeral_system.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_parse_from_numeral_system.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_raises.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_raises.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_random_choice_generator.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_random_choice_generator.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_render_to_base64url.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_render_to_base64url.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_render_to_numeral_system.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_render_to_numeral_system.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_reversed_enumerate.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_reversed_enumerate.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_scale_luminosity.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_scale_luminosity.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_splicewhile.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_splicewhile.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_to_tril.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_to_tril.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_unfurl_lineage_with_contiguous_ids.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_unfurl_lineage_with_contiguous_ids.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_unpairwise.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_unpairwise.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_unzip.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_unzip.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_with_omission.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_with_omission.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_with_rng_state_context.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_with_rng_state_context.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/_auxiliary_lib/_zip_strict.py` & `hstrat-1.7.3/hstrat/_auxiliary_lib/_zip_strict.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/frozen_instrumentation/_HereditaryStratigraphicAssemblage.py` & `hstrat-1.7.3/hstrat/frozen_instrumentation/_HereditaryStratigraphicAssemblage.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/frozen_instrumentation/_HereditaryStratigraphicAssemblageSpecimen.py` & `hstrat-1.7.3/hstrat/frozen_instrumentation/_HereditaryStratigraphicAssemblageSpecimen.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/frozen_instrumentation/_HereditaryStratigraphicSpecimen.py` & `hstrat-1.7.3/hstrat/frozen_instrumentation/_HereditaryStratigraphicSpecimen.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/frozen_instrumentation/__init__.py` & `hstrat-1.7.3/hstrat/frozen_instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/genome_instrumentation/_HereditaryStratigraphicColumn.py` & `hstrat-1.7.3/hstrat/genome_instrumentation/_HereditaryStratigraphicColumn.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,15 +290,17 @@
 
         # update generation counter
         self._num_strata_deposited += num_stratum_depositions
 
     def _PurgeColumn(self: "HereditaryStratigraphicColumn") -> None:
         """Discard stored strata according to the configured retention policy.
 
-        Implementation detail. Called after a new stratum has been appended to the column's store but before it is considered fully deposited (i.e., it is reflected in the column's internal deposition counter).
+        Implementation detail. Called after a new stratum has been appended to
+        the column's store but before it is considered fully deposited (i.e.,
+        it is reflected in the column's internal deposition counter).
         """
         condemned_ranks = self._stratum_retention_policy.GenDropRanks(
             num_stratum_depositions_completed=self.GetNumStrataDeposited(),
             retained_ranks=self.IterRetainedRanks(),
         )
         self._stratum_ordered_store.DelRanks(
             ranks=condemned_ranks,
```

### Comparing `hstrat-1.7.2/hstrat/genome_instrumentation/_HereditaryStratigraphicColumnBundle.py` & `hstrat-1.7.3/hstrat/genome_instrumentation/_HereditaryStratigraphicColumnBundle.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/genome_instrumentation/_HereditaryStratum.py` & `hstrat-1.7.3/hstrat/genome_instrumentation/_HereditaryStratum.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/genome_instrumentation/__init__.py` & `hstrat-1.7.3/hstrat/genome_instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/genome_instrumentation/stratum_ordered_stores/_HereditaryStratumOrderedStoreDict.py` & `hstrat-1.7.3/hstrat/genome_instrumentation/stratum_ordered_stores/_HereditaryStratumOrderedStoreDict.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/genome_instrumentation/stratum_ordered_stores/_HereditaryStratumOrderedStoreList.py` & `hstrat-1.7.3/hstrat/genome_instrumentation/stratum_ordered_stores/_HereditaryStratumOrderedStoreList.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/genome_instrumentation/stratum_ordered_stores/_HereditaryStratumOrderedStoreTree.py` & `hstrat-1.7.3/hstrat/genome_instrumentation/stratum_ordered_stores/_HereditaryStratumOrderedStoreTree.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/genome_instrumentation/stratum_ordered_stores/__init__.py` & `hstrat-1.7.3/hstrat/genome_instrumentation/stratum_ordered_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/hstrat/__init__.py` & `hstrat-1.7.3/hstrat/hstrat/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/__init__.py` & `hstrat-1.7.3/hstrat/juxtaposition/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_calc_definitive_max_rank_of_first_retained_disparity_between.py` & `hstrat-1.7.3/hstrat/juxtaposition/_calc_definitive_max_rank_of_first_retained_disparity_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_calc_definitive_max_rank_of_last_retained_commonality_between.py` & `hstrat-1.7.3/hstrat/juxtaposition/_calc_definitive_max_rank_of_last_retained_commonality_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_calc_definitive_min_ranks_since_first_retained_disparity_with.py` & `hstrat-1.7.3/hstrat/juxtaposition/_calc_definitive_min_ranks_since_first_retained_disparity_with.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_calc_definitive_min_ranks_since_last_retained_commonality_with.py` & `hstrat-1.7.3/hstrat/juxtaposition/_calc_definitive_min_ranks_since_last_retained_commonality_with.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_calc_min_implausible_spurious_consecutive_differentia_collisions_between.py` & `hstrat-1.7.3/hstrat/juxtaposition/_calc_min_implausible_spurious_consecutive_differentia_collisions_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_calc_probability_differentia_collision_between.py` & `hstrat-1.7.3/hstrat/juxtaposition/_calc_probability_differentia_collision_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_calc_rank_of_first_retained_disparity_between.py` & `hstrat-1.7.3/hstrat/juxtaposition/_calc_rank_of_first_retained_disparity_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_calc_rank_of_last_retained_commonality_between.py` & `hstrat-1.7.3/hstrat/juxtaposition/_calc_rank_of_last_retained_commonality_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_calc_ranks_since_first_retained_disparity_with.py` & `hstrat-1.7.3/hstrat/juxtaposition/_calc_ranks_since_first_retained_disparity_with.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_calc_ranks_since_last_retained_commonality_with.py` & `hstrat-1.7.3/hstrat/juxtaposition/_calc_ranks_since_last_retained_commonality_with.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_diff_retained_ranks.py` & `hstrat-1.7.3/hstrat/juxtaposition/_diff_retained_ranks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_get_last_common_stratum_between.py` & `hstrat-1.7.3/hstrat/juxtaposition/_get_last_common_stratum_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_get_nth_common_rank_between.py` & `hstrat-1.7.3/hstrat/juxtaposition/_get_nth_common_rank_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_impl/_dispatch_impl.py` & `hstrat-1.7.3/hstrat/juxtaposition/_impl/_dispatch_impl.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_impl_column/__init__.py` & `hstrat-1.7.3/hstrat/juxtaposition/_impl_column/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_impl_column/_calc_rank_of_first_retained_disparity_between.py` & `hstrat-1.7.3/hstrat/juxtaposition/_impl_column/_calc_rank_of_first_retained_disparity_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_impl_column/_calc_rank_of_first_retained_disparity_between_bsearch.py` & `hstrat-1.7.3/hstrat/juxtaposition/_impl_column/_calc_rank_of_first_retained_disparity_between_bsearch.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_impl_column/_calc_rank_of_first_retained_disparity_between_generic.py` & `hstrat-1.7.3/hstrat/juxtaposition/_impl_column/_calc_rank_of_first_retained_disparity_between_generic.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_impl_column/_calc_rank_of_last_retained_commonality_between.py` & `hstrat-1.7.3/hstrat/juxtaposition/_impl_column/_calc_rank_of_last_retained_commonality_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_impl_column/_calc_rank_of_last_retained_commonality_between_bsearch.py` & `hstrat-1.7.3/hstrat/juxtaposition/_impl_column/_calc_rank_of_last_retained_commonality_between_bsearch.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_impl_column/_calc_rank_of_last_retained_commonality_between_generic.py` & `hstrat-1.7.3/hstrat/juxtaposition/_impl_column/_calc_rank_of_last_retained_commonality_between_generic.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_impl_column/_calc_rank_of_parity_segue_between.py` & `hstrat-1.7.3/hstrat/juxtaposition/_impl_column/_calc_rank_of_parity_segue_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_impl_column/_iter_mutual_ranks.py` & `hstrat-1.7.3/hstrat/juxtaposition/_impl_column/_iter_mutual_ranks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_impl_column/_iter_ranks_of_retained_commonality_between.py` & `hstrat-1.7.3/hstrat/juxtaposition/_impl_column/_iter_ranks_of_retained_commonality_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_impl_specimen/__init__.py` & `hstrat-1.7.3/hstrat/juxtaposition/_impl_specimen/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_impl_specimen/_calc_rank_of_first_retained_disparity_between.py` & `hstrat-1.7.3/hstrat/juxtaposition/_impl_specimen/_calc_rank_of_first_retained_disparity_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_impl_specimen/_calc_rank_of_last_retained_commonality_between.py` & `hstrat-1.7.3/hstrat/juxtaposition/_impl_specimen/_calc_rank_of_last_retained_commonality_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_impl_specimen/_calc_rank_of_parity_segue_between_naive.py` & `hstrat-1.7.3/hstrat/juxtaposition/_impl_specimen/_calc_rank_of_parity_segue_between_naive.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_impl_specimen/_iter_mutual_rank_indices.py` & `hstrat-1.7.3/hstrat/juxtaposition/_impl_specimen/_iter_mutual_rank_indices.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_impl_specimen/_iter_mutual_ranks.py` & `hstrat-1.7.3/hstrat/juxtaposition/_impl_specimen/_iter_mutual_ranks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/juxtaposition/_impl_specimen/_iter_ranks_of_retained_commonality_between.py` & `hstrat-1.7.3/hstrat/juxtaposition/_impl_specimen/_iter_ranks_of_retained_commonality_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/estimators/__init__.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/estimators/_estimate_rank_of_mrca_maximum_likelihood.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/estimators/_estimate_rank_of_mrca_maximum_likelihood.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/estimators/_estimate_rank_of_mrca_naive.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/estimators/_estimate_rank_of_mrca_naive.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/estimators/_estimate_rank_of_mrca_unbiased.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/estimators/_estimate_rank_of_mrca_unbiased.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/__init__.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_ballpark_patristic_distance_between.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_ballpark_patristic_distance_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_ballpark_rank_of_mrca_between.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_ballpark_rank_of_mrca_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_ballpark_ranks_since_mrca_with.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_ballpark_ranks_since_mrca_with.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_calc_patristic_distance_bounds_between.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_calc_patristic_distance_bounds_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_calc_rank_of_earliest_detectable_mrca_between.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_calc_rank_of_earliest_detectable_mrca_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_calc_rank_of_mrca_bounds_between.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_calc_rank_of_mrca_bounds_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_calc_rank_of_mrca_bounds_provided_confidence_level.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_calc_rank_of_mrca_bounds_provided_confidence_level.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_calc_rank_of_mrca_uncertainty_between.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_calc_rank_of_mrca_uncertainty_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_calc_ranks_since_earliest_detectable_mrca_with.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_calc_ranks_since_earliest_detectable_mrca_with.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_calc_ranks_since_mrca_bounds_provided_confidence_level.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_calc_ranks_since_mrca_bounds_provided_confidence_level.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_calc_ranks_since_mrca_bounds_with.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_calc_ranks_since_mrca_bounds_with.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_calc_ranks_since_mrca_uncertainty_with.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_calc_ranks_since_mrca_uncertainty_with.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_does_definitively_have_no_common_ancestor.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_does_definitively_have_no_common_ancestor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_does_have_any_common_ancestor.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_does_have_any_common_ancestor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_estimate_patristic_distance_between.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_estimate_patristic_distance_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_estimate_rank_of_mrca_between.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_estimate_rank_of_mrca_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_estimate_ranks_since_mrca_with.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_estimate_ranks_since_mrca_with.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_impl/__init__.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_impl/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_impl/_estimate_rank_of_mrca_maximum_likelihood.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_impl/_estimate_rank_of_mrca_maximum_likelihood.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_impl/_estimate_rank_of_mrca_naive.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_impl/_estimate_rank_of_mrca_naive.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_impl/_estimate_rank_of_mrca_unbiased.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_impl/_estimate_rank_of_mrca_unbiased.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/pairwise/_impl/_extract_common_retained_ranks_through_first_retained_disparity.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/pairwise/_impl/_extract_common_retained_ranks_through_first_retained_disparity.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/population/__init__.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/population/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/population/_build_distance_matrix_biopython.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/population/_build_distance_matrix_biopython.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/population/_build_distance_matrix_numpy.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/population/_build_distance_matrix_numpy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/population/_calc_rank_of_earliest_detectable_mrca_among.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/population/_calc_rank_of_earliest_detectable_mrca_among.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/population/_calc_rank_of_mrca_bounds_among.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/population/_calc_rank_of_mrca_bounds_among.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/population/_calc_rank_of_mrca_uncertainty_among.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/population/_calc_rank_of_mrca_uncertainty_among.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/population/_does_definitively_share_no_common_ancestor.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/population/_does_definitively_share_no_common_ancestor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/population/_does_share_any_common_ancestor.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/population/_does_share_any_common_ancestor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/priors/_ArbitraryPrior.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/priors/_ArbitraryPrior.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/priors/_BubbleWrappedPrior.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/priors/_BubbleWrappedPrior.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/priors/_ExponentialPrior.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/priors/_ExponentialPrior.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/priors/_GeometricPrior.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/priors/_GeometricPrior.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/priors/_UniformPrior.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/priors/_UniformPrior.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/priors/__init__.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/priors/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/__init__.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_build_tree.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_build_tree.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_build_tree_nj.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_build_tree_nj.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_build_tree_trie.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_build_tree_trie.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_build_tree_trie_ensemble.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_build_tree_trie_ensemble.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_build_tree_upgma.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_build_tree_upgma.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/_TrieInnerNode.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/_TrieInnerNode.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/_TrieLeafNode.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/_TrieLeafNode.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/__init__.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/_append_genesis_organism.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/_append_genesis_organism.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/_build_tree_biopython_distance.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/_build_tree_biopython_distance.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/_build_trie_from_artifacts.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/_build_trie_from_artifacts.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/_estimate_origin_times.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/_estimate_origin_times.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/_find_chronological_roots.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/_find_chronological_roots.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/_impl/_time_calibrate_tree.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/_impl/_time_calibrate_tree.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/trie_postprocess/_AssignDestructionTimeYoungestPlusOneTriePostprocessor.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/trie_postprocess/_AssignDestructionTimeYoungestPlusOneTriePostprocessor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/trie_postprocess/_AssignOriginTimeExpectedValueTriePostprocessor.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/trie_postprocess/_AssignOriginTimeExpectedValueTriePostprocessor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/trie_postprocess/_AssignOriginTimeNaiveTriePostprocessor.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/trie_postprocess/_AssignOriginTimeNaiveTriePostprocessor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/trie_postprocess/_AssignOriginTimeNodeRankTriePostprocessor.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/trie_postprocess/_AssignOriginTimeNodeRankTriePostprocessor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/trie_postprocess/_CompoundTriePostprocessor.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/trie_postprocess/_CompoundTriePostprocessor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/trie_postprocess/_PeelBackConjoinedLeavesTriePostprocessor.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/trie_postprocess/_PeelBackConjoinedLeavesTriePostprocessor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/trie_postprocess/_SampleAncestralRollbacksTriePostprocessor.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/trie_postprocess/_SampleAncestralRollbacksTriePostprocessor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/phylogenetic_inference/tree/trie_postprocess/__init__.py` & `hstrat-1.7.3/hstrat/phylogenetic_inference/tree/trie_postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/serialization/__init__.py` & `hstrat-1.7.3/hstrat/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/serialization/_assemblage_from_records.py` & `hstrat-1.7.3/hstrat/serialization/_assemblage_from_records.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/serialization/_col_from_records.py` & `hstrat-1.7.3/hstrat/serialization/_col_from_records.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/serialization/_col_to_dataframe.py` & `hstrat-1.7.3/hstrat/serialization/_col_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/serialization/_col_to_records.py` & `hstrat-1.7.3/hstrat/serialization/_col_to_records.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/serialization/_col_to_specimen.py` & `hstrat-1.7.3/hstrat/serialization/_col_to_specimen.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/serialization/_impl/_col_records_from_pop_records.py` & `hstrat-1.7.3/hstrat/serialization/_impl/_col_records_from_pop_records.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/serialization/_pack_differentiae.py` & `hstrat-1.7.3/hstrat/serialization/_pack_differentiae.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/serialization/_pop_from_records.py` & `hstrat-1.7.3/hstrat/serialization/_pop_from_records.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/serialization/_pop_to_assemblage.py` & `hstrat-1.7.3/hstrat/serialization/_pop_to_assemblage.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/serialization/_pop_to_dataframe.py` & `hstrat-1.7.3/hstrat/serialization/_pop_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/serialization/_pop_to_records.py` & `hstrat-1.7.3/hstrat/serialization/_pop_to_records.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/serialization/_specimen_from_records.py` & `hstrat-1.7.3/hstrat/serialization/_specimen_from_records.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/serialization/_unassemblage_from_records.py` & `hstrat-1.7.3/hstrat/serialization/_unassemblage_from_records.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/serialization/_unpack_differentiae.py` & `hstrat-1.7.3/hstrat/serialization/_unpack_differentiae.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/__init__.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/__init__.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_detail/_PolicyCouplerFactory.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_detail/_PolicyCouplerFactory.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyAbsUpperBoundPessimalRankBruteForce.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyAbsUpperBoundPessimalRankBruteForce.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyAbsUpperBoundWorstCase.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyAbsUpperBoundWorstCase.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyRelExactFromAbs.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyRelExactFromAbs.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyRelUpperBoundPessimalRankBruteForce.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyRelUpperBoundPessimalRankBruteForce.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyRelUpperBoundWorstCase.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcMrcaUncertaintyRelUpperBoundWorstCase.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcNumStrataRetainedUpperBoundWorstCase.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_CalcNumStrataRetainedUpperBoundWorstCase.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_GenDropRanksFromPredKeepRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/_GenDropRanksFromPredKeepRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/__init__.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/_impl/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_Policy.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_PolicySpec.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/__init__.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_impl/_calc_provided_uncertainty.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_impl/_calc_provided_uncertainty.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/_CalcNumStrataRetainedExact.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/_CalcNumStrataRetainedExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/_CalcRankAtColumnIndex.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/_CalcRankAtColumnIndex.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/_IterRetainedRanks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_algo/_scry/_IterRetainedRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_Policy.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_PolicySpec.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/__init__.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_enact/_GenDropRanks_/_GenDropRanks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_enact/_GenDropRanks_/_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_impl/_calc_provided_uncertainty.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_impl/_calc_provided_uncertainty.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcNumStrataRetainedUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_invar/_CalcNumStrataRetainedUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/_CalcMrcaUncertaintyAbsExact.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/_CalcMrcaUncertaintyAbsExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/_CalcNumStrataRetainedExact.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/_CalcNumStrataRetainedExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/_CalcRankAtColumnIndex.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/_CalcRankAtColumnIndex.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/_IterRetainedRanks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/depth_proportional_resolution_tapered_algo/_scry/_IterRetainedRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_Policy.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_PolicySpec.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/__init__.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/_CalcNumStrataRetainedExact.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/_CalcNumStrataRetainedExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/_CalcRankAtColumnIndex.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/_CalcRankAtColumnIndex.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/_IterRetainedRanks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/fixed_resolution_algo/_scry/_IterRetainedRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_Policy.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_PolicySpec.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/__init__.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_enact/_GenDropRanks_/_GenDropRanks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_enact/_GenDropRanks_/_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/__init__.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_get_retained_ranks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_get_retained_ranks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_rank_backstops.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_rank_backstops.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_rank_cutoffs.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_rank_cutoffs.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_rank_seps.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_rank_seps.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_target_ranks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_target_ranks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_target_recencies.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_impl/_iter_target_recencies.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcNumStrataRetainedUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_invar/_CalcNumStrataRetainedUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/_CalcMrcaUncertaintyAbsExact.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/_CalcMrcaUncertaintyAbsExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/_CalcNumStrataRetainedExact.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/_CalcNumStrataRetainedExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/_CalcRankAtColumnIndex.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/_CalcRankAtColumnIndex.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/_IterRetainedRanks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_algo/_scry/_IterRetainedRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_Policy.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_PolicySpec.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/__init__.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_enact/_GenDropRanks_/_GenDropRanks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_enact/_GenDropRanks_/_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/__init__.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_common_ratio.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_common_ratio.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_rank_backstop.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_rank_backstop.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_rank_cutoff.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_rank_cutoff.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_rank_sep.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_rank_sep.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_target_rank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_target_rank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_target_recency.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_calc_target_recency.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_get_retained_ranks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_get_retained_ranks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_iter_priority_ranks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_impl/_iter_priority_ranks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcNumStrataRetainedUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_invar/_CalcNumStrataRetainedUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/_CalcMrcaUncertaintyAbsExact.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/_CalcMrcaUncertaintyAbsExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/_CalcNumStrataRetainedExact.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/_CalcNumStrataRetainedExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/_CalcRankAtColumnIndex.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/_CalcRankAtColumnIndex.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/_IterRetainedRanks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/geom_seq_nth_root_tapered_algo/_scry/_IterRetainedRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_Policy.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_PolicySpec.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/__init__.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/_CalcNumStrataRetainedExact.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/_CalcNumStrataRetainedExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/_CalcRankAtColumnIndex.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/_CalcRankAtColumnIndex.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/_IterRetainedRanks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/nominal_resolution_algo/_scry/_IterRetainedRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_Policy.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_PolicySpec.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/__init__.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/_CalcNumStrataRetainedExact.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/_CalcNumStrataRetainedExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/_CalcRankAtColumnIndex.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/_CalcRankAtColumnIndex.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/_IterRetainedRanks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/perfect_resolution_algo/_scry/_IterRetainedRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_Policy.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_PolicySpec.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/__init__.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_enact/_GenDropRanks_/_GenDropRanks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_enact/_GenDropRanks_/_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/pseudostochastic_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_Policy.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_PolicySpec.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/__init__.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_enact/_GenDropRanks_/_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_impl/_calc_provided_uncertainty.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_impl/_calc_provided_uncertainty.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_impl/_num_to_condemn.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_impl/_num_to_condemn.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_invar/_CalcNumStrataRetainedUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/_CalcMrcaUncertaintyAbsExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/_CalcNumStrataRetainedExact.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/_CalcNumStrataRetainedExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/_CalcRankAtColumnIndex.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/_CalcRankAtColumnIndex.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/_IterRetainedRanks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_algo/_scry/_IterRetainedRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_Policy.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_PolicySpec.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/__init__.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_impl/_calc_geom_seq_nth_root_transition_rank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_impl/_calc_geom_seq_nth_root_transition_rank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_impl/_calc_provided_resolution.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_impl/_calc_provided_resolution.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_impl/_pick_policy.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/recency_proportional_resolution_curbed_algo/_impl/_pick_policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_Policy.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_PolicySpec.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/__init__.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_enact/_GenDropRanks_/_FromPredKeepRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_enact/_GenDropRanks_/_GenDropRanks.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_enact/_GenDropRanks_/_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_algorithms/stochastic_algo/_invar/_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_MrcaUncertaintyAbsExactEvaluator.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_MrcaUncertaintyAbsExactEvaluator.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_MrcaUncertaintyAbsUpperBoundEvaluator.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_MrcaUncertaintyAbsUpperBoundEvaluator.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_MrcaUncertaintyRelExactEvaluator.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_MrcaUncertaintyRelExactEvaluator.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_MrcaUncertaintyRelUpperBoundEvaluator.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_MrcaUncertaintyRelUpperBoundEvaluator.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_NumStrataRetainedExactEvaluator.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_NumStrataRetainedExactEvaluator.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_NumStrataRetainedUpperBoundEvaluator.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/_NumStrataRetainedUpperBoundEvaluator.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/__init__.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_evaluators/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/_PropertyAtLeastParameterizer.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/_PropertyAtLeastParameterizer.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/_PropertyAtMostParameterizer.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/_PropertyAtMostParameterizer.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/_PropertyExactlyParameterizer.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/_PropertyExactlyParameterizer.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/__init__.py` & `hstrat-1.7.3/hstrat/stratum_retention_strategy/stratum_retention_policy_parameterizers/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_viz/animate/_policy_panel_animate.py` & `hstrat-1.7.3/hstrat/stratum_retention_viz/animate/_policy_panel_animate.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     do_show: bool = False,
     save_as: typing.Optional[str] = None,
 ) -> mpl_animation.FuncAnimation:
     """Animate evolution of column and its properties under a retention policy.
 
     Parameters
     ----------
-    stratum_retention_policy: any
+    stratum_retention_policy : any
         Object specifying stratum retention policy.
-    num_generations: int
+    num_generations : int
         Number of generations to plot.
     do_show : bool, optional
         Whether to show() the plot automatically.
     save_as : str, optional
         If set, save animation as file type specified.
     """
     fig = plt.figure(figsize=(8, 6), dpi=80)
```

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_viz/animate/_stratum_retention_animate.py` & `hstrat-1.7.3/hstrat/stratum_retention_viz/animate/_stratum_retention_animate.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,17 @@
     draw_extinct_history: bool = True,
     draw_extinct_placeholders: bool = False,
 ) -> mpl_animation.FuncAnimation:
     """Animate evolution of strata histories under a stratum retention policy.
 
     Parameters
     ----------
-    stratum_retention_policy: any
+    stratum_retention_policy : any
         Object specifying stratum retention policy.
-    num_generations: int
+    num_generations : int
         Number of generations to plot.
     do_show : bool, optional
         Whether to show() the plot automatically.
     save_as : str, optional
         If set, save animation as file type specified.
     """
     fig = plt.figure(figsize=(6, 6), dpi=80)
```

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_viz/ascii/_col_to_ascii.py` & `hstrat-1.7.3/hstrat/stratum_retention_viz/ascii/_col_to_ascii.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,34 @@
 
 def col_to_ascii(
     column: HereditaryStratigraphicColumn,
     discarded_strata: bool = True,
     key: bool = True,
     time_bookends: bool = True,
 ) -> str:
+    """Create an ASCII table representation of HereditaryStratigraphicColumn
+    state.
+
+    Parameters
+    ----------
+    column : HereditaryStratigraphicColumn
+        The HereditaryStratigraphicColumn object to be converted.
+    discarded_strata : bool, default True
+        Include discarded strata in the output?
+    key : bool, default True
+        Append a legend to the output?
+    time_bookends : bool, default True
+        Prepend and append "MOST ANCIENT" and "MOST RECENT" to the table?
+
+    Returns
+    -------
+    str
+        The ASCII representation of the HereditaryStratigraphicColumn object
+        in tabular format.
+    """
     df = col_to_dataframe(column)
     df.set_index("rank", inplace=True)
 
     table = PrettyTable()
     table.field_names = [
         "stratum rank",
         "stratum index",
```

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_viz/plot/__init__.py` & `hstrat-1.7.3/hstrat/stratum_retention_viz/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_viz/plot/_mrca_uncertainty_absolute_barplot.py` & `hstrat-1.7.3/hstrat/stratum_retention_viz/plot/_mrca_uncertainty_absolute_barplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
     Plots absolute uncertainty for MRCA estimation over column ranks
     (positions) in a hereditary stratigraphic column at a particular generation
     under a particular stratum retention policy.
 
     Parameters
     ----------
-    stratum_retention_policy: Callable
+    stratum_retention_policy : Callable
         Object specifying stratum retention policy.
-    num_generations: int
+    num_generations : int
         Number of generations to plot.
     ax : matplotlib/pylab axes, optional
         If a valid matplotlib.axes.Axes instance, the plot is drawn in that
         Axes. By default (None), a new axes is created.
     do_show : bool, optional
         Whether to show() the plot automatically.
     """
```

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_viz/plot/_mrca_uncertainty_relative_barplot.py` & `hstrat-1.7.3/hstrat/stratum_retention_viz/plot/_mrca_uncertainty_relative_barplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 
     Plots relative uncertainty for MRCA estimation over column ranks
     (positions) in a hereditary stratigraphic column at a particular generation
     under a particular stratum retention policy.
 
     Parameters
     ----------
-    stratum_retention_policy: Callable
+    stratum_retention_policy : Callable
         Object specifying stratum retention policy.
-    num_generations: int
+    num_generations : int
         Number of generations to plot.
     ax : matplotlib/pylab axes, optional
         If a valid matplotlib.axes.Axes instance, the plot is drawn in that
         Axes. By default (None), a new axes is created.
     do_show : bool, optional
         Whether to show() the plot automatically.
     """
```

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_viz/plot/_policy_panel_plot.py` & `hstrat-1.7.3/hstrat/stratum_retention_viz/plot/_policy_panel_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 ) -> plt.matplotlib.figure.Figure:
     """Holisticaly sketch stratum retention policy at a particular generation.
 
     Produces a composite multipanel plot.
 
     Parameters
     ----------
-    stratum_retention_policy: any
+    stratum_retention_policy : any
         Object specifying stratum retention policy.
-    num_generations: int
+    num_generations : int
         Number of generations to plot.
     do_show : bool, optional
         Whether to show() the plot automatically.
     fig : matplotlib/pylab figure, optional
         If a valid matplotlib.figure.Figure instance, the plot is drawn in that
         Figure. By default (None), a new figure is created.
     """
```

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_viz/plot/_strata_retained_frac_lineplot.py` & `hstrat-1.7.3/hstrat/stratum_retention_viz/plot/_strata_retained_frac_lineplot.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     do_show: bool = False,
     ax: typing.Optional[plt.matplotlib.axes.Axes] = None,
 ) -> plt.matplotlib.axes.Axes:
     """Plot fraction deposited strata that are retained at each generation.
 
     Parameters
     ----------
-    stratum_retention_policy: any
+    stratum_retention_policy : any
         Object specifying stratum retention policy.
-    num_generations: int
+    num_generations : int
         Number of generations to plot.
     ax : matplotlib/pylab axes, optional
         If a valid matplotlib.axes.Axes instance, the plot is drawn in that
         Axes. By default (None), a new axes is created.
     do_show : bool, optional
         Whether to show() the plot automatically.
     """
```

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_viz/plot/_strata_retained_num_lineplot.py` & `hstrat-1.7.3/hstrat/stratum_retention_viz/plot/_strata_retained_num_lineplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     do_show: bool = False,
     ax: typing.Optional[plt.matplotlib.axes.Axes] = None,
 ) -> plt.matplotlib.axes.Axes:
     """Plot number deposited strata that are retained at each generation.
 
     Parameters
     ----------
-    stratum_retention_policy: any
+    stratum_retention_policy : any
         Object specifying stratum retention policy.
-    num_generations: int
+    num_generations : int
         Number of generations to plot.
     ax : matplotlib/pylab axes, optional
         If a valid matplotlib.axes.Axes instance, the plot is drawn in that
         Axes. By default (None), a new axes is created.
     do_show : bool, optional
         Whether to show() the plot automatically.
     """
```

### Comparing `hstrat-1.7.2/hstrat/stratum_retention_viz/plot/_stratum_retention_dripplot.py` & `hstrat-1.7.3/hstrat/stratum_retention_viz/plot/_stratum_retention_dripplot.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,49 +14,62 @@
     stratum_retention_policy: typing.Any,
     num_generations: int,
     do_show: bool = False,
     ax: typing.Optional[plt.matplotlib.axes.Axes] = None,
     draw_extant_history: bool = True,
     draw_extinct_history: bool = True,
     draw_extinct_placeholders: bool = False,
+    progress_wrap: typing.Callable = lambda x: x,
 ) -> plt.matplotlib.axes.Axes:
     """Show history of retained and purged strata at a particular generation.
 
     Plots position of retained strata within a hereditary stratigraphic
     column over successive depositions under a particular stratum retention
     policy.
 
     Parameters
     ----------
-    stratum_retention_policy: any
+    stratum_retention_policy : any
         Object specifying stratum retention policy.
-    num_generations: int
+    num_generations : int
         Number of generations to plot.
+    do_show : bool, optional
+        Whether to show() the plot automatically.
     ax : matplotlib/pylab axes, optional
         If a valid matplotlib.axes.Axes instance, the plot is drawn in that
         Axes. By default (None), a new axes is created.
-    do_show : bool, optional
-        Whether to show() the plot automatically.
+    progress_wrap : Callable, default identity function
+        Wrapper applied around generation iterator and row generator for final
+        phylogeny compilation process.
+
+        Pass tqdm or equivalent to display progress bars.
     """
     if ax is None:
         fig = plt.figure()
         ax = fig.add_subplot(1, 1, 1)
     elif not isinstance(ax, plt.matplotlib.axes.Axes):
         raise ValueError(f"Invalid argument for ax: {ax}")
 
-    column = HereditaryStratigraphicColumn(
-        stratum_retention_policy=stratum_retention_policy,
+    # instantiate column if IterRetainedRanks not available
+    column_t = typing.Optional[HereditaryStratigraphicColumn]
+    column: column_t = opyt.apply_if_or_else(
+        stratum_retention_policy.IterRetainedRanks,
+        lambda __: None,
+        lambda: HereditaryStratigraphicColumn(
+            stratum_retention_policy=stratum_retention_policy,
+        ),
     )
-    for gen in range(1, num_generations):
+
+    for gen in progress_wrap(range(1, num_generations)):
         for rank in stratum_retention_policy.GenDropRanks(
             gen,
-            opyt.apply_if_or_value(
+            opyt.apply_if_or_else(
                 stratum_retention_policy.IterRetainedRanks,
                 lambda x: x(gen),
-                column.IterRetainedRanks(),
+                lambda: column.IterRetainedRanks(),
             ),
         ):
             if draw_extinct_placeholders:
                 ax.plot(
                     rank,
                     num_generations - 1,
                     ms=20 / max(0.2 * num_generations, 1),
@@ -108,20 +121,20 @@
                 marker="v",
                 markerfacecolor=scale_luminosity(
                     "r", max(10 / max(0.2 * num_generations, 1), 1)
                 ),
                 markeredgecolor="r",
                 markeredgewidth=2 / max(0.05 * num_generations, 1),
             )
-        column.DepositStratum()
+        opyt.apply_if(column, lambda x: x.DepositStratum())
 
-    for remaining_rank in opyt.apply_if_or_value(
+    for remaining_rank in opyt.apply_if_or_else(
         stratum_retention_policy.IterRetainedRanks,
         lambda x: x(num_generations),
-        column.IterRetainedRanks(),
+        lambda: column.IterRetainedRanks(),
     ):
         ax.plot(
             remaining_rank,
             num_generations - 1,
             ms=20 / max(0.2 * num_generations, 1),
             marker="v",
             markerfacecolor="None",
```

### Comparing `hstrat-1.7.2/hstrat/test_drive/__init__.py` & `hstrat-1.7.3/hstrat/test_drive/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/descend_template_phylogeny/__init__.py` & `hstrat-1.7.3/hstrat/test_drive/descend_template_phylogeny/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny.py` & `hstrat-1.7.3/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_alifestd.py` & `hstrat-1.7.3/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_alifestd.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_biopython.py` & `hstrat-1.7.3/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_biopython.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_dendropy.py` & `hstrat-1.7.3/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_dendropy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_naive.py` & `hstrat-1.7.3/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_naive.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_networkx.py` & `hstrat-1.7.3/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_networkx.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_posthoc.py` & `hstrat-1.7.3/hstrat/test_drive/descend_template_phylogeny/_descend_template_phylogeny_posthoc.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population.py` & `hstrat-1.7.3/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/__init__.py` & `hstrat-1.7.3/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/_apply_island_migrations.py` & `hstrat-1.7.3/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/_apply_island_migrations.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/_apply_niche_invasions.py` & `hstrat-1.7.3/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/_apply_niche_invasions.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/_select_parents.py` & `hstrat-1.7.3/hstrat/test_drive/generate_template_phylogeny/_evolve_fitness_trait_population_/_select_parents.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/perfect_tracking/_DecantingPhyloTracker.py` & `hstrat-1.7.3/hstrat/test_drive/perfect_tracking/_DecantingPhyloTracker.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/perfect_tracking/_GarbageCollectingPhyloTracker.py` & `hstrat-1.7.3/hstrat/test_drive/perfect_tracking/_GarbageCollectingPhyloTracker.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/perfect_tracking/_GarbageCollectingPhyloTracker_/_discern_referenced_rows.py` & `hstrat-1.7.3/hstrat/test_drive/perfect_tracking/_GarbageCollectingPhyloTracker_/_discern_referenced_rows.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/perfect_tracking/_PerfectBacktrackHandle.py` & `hstrat-1.7.3/hstrat/test_drive/perfect_tracking/_PerfectBacktrackHandle.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/perfect_tracking/__init__.py` & `hstrat-1.7.3/hstrat/test_drive/perfect_tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/perfect_tracking/_compile_perfect_backtrack_phylogeny.py` & `hstrat-1.7.3/hstrat/test_drive/perfect_tracking/_compile_perfect_backtrack_phylogeny.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat/test_drive/perfect_tracking/_compile_phylogeny_from_lineage_iters.py` & `hstrat-1.7.3/hstrat/test_drive/perfect_tracking/_compile_phylogeny_from_lineage_iters.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat.egg-info/PKG-INFO` & `hstrat-1.7.3/hstrat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6873 7472  : 2.1.Name: hstr
 00000020: 6174 0a56 6572 7369 6f6e 3a20 312e 372e  at.Version: 1.7.
-00000030: 320a 5375 6d6d 6172 793a 2068 7374 7261  2.Summary: hstra
+00000030: 330a 5375 6d6d 6172 793a 2068 7374 7261  3.Summary: hstra
 00000040: 7420 656e 6162 6c65 7320 7068 796c 6f67  t enables phylog
 00000050: 656e 6574 6963 2069 6e66 6572 656e 6365  enetic inference
 00000060: 206f 6e20 6469 7374 7269 6275 7465 6420   on distributed 
 00000070: 6469 6769 7461 6c20 6576 6f6c 7574 696f  digital evolutio
 00000080: 6e20 706f 7075 6c61 7469 6f6e 730a 4175  n populations.Au
 00000090: 7468 6f72 2d65 6d61 696c 3a20 4d61 7474  thor-email: Matt
 000000a0: 6865 7720 416e 6472 6573 204d 6f72 656e  hew Andres Moren
```

### Comparing `hstrat-1.7.2/hstrat.egg-info/SOURCES.txt` & `hstrat-1.7.3/hstrat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/hstrat.egg-info/requires.txt` & `hstrat-1.7.3/hstrat.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/pyproject.toml` & `hstrat-1.7.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 description = "hstrat enables phylogenetic inference on distributed digital evolution populations"
 license = {text = "MIT license"}
 name  =  "hstrat"
 keywords = [
   "hstrat",
 ]
 requires-python = ">=3.7"
-version = "1.7.2"
+version = "1.7.3"
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.urls]
 homepage = "https://github.com/mmore500/hstrat"
```

### Comparing `hstrat-1.7.2/tests/test_hstrat/assets/nk_ecoeaselection.csv` & `hstrat-1.7.3/tests/test_hstrat/assets/nk_ecoeaselection.csv`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/assets/nk_lexicaseselection.csv` & `hstrat-1.7.3/tests/test_hstrat/assets/nk_lexicaseselection.csv`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/assets/nk_tournamentselection.csv` & `hstrat-1.7.3/tests/test_hstrat/assets/nk_tournamentselection.csv`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/conftest.py` & `hstrat-1.7.3/tests/test_hstrat/conftest.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/nk_ecoeaselection.csv` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/nk_ecoeaselection.csv`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/nk_lexicaseselection.csv` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/nk_lexicaseselection.csv`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/assets/nk_tournamentselection.csv` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/assets/nk_tournamentselection.csv`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeAscendingIter.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeAscendingIter.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeFastLeafIter.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeFastLeafIter.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeFastLevelOrderIter.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeFastLevelOrderIter.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeFastPostOrderIter.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeFastPostOrderIter.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeFastPreOrderIter.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_AnyTreeFastPreOrderIter.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_CopyableSeriesItemsIter.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_CopyableSeriesItemsIter.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_RngStateContext.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_RngStateContext.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_aggregate_phylogenies.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_aggregate_phylogenies.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_assign_contiguous_ids.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_assign_contiguous_ids.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_assign_root_ancestor_token.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_assign_root_ancestor_token.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_collapse_unifurcations.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_collapse_unifurcations.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_convert_root_ancestor_token.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_convert_root_ancestor_token.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_find_chronological_inconsistency.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_find_chronological_inconsistency.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_find_leaf_ids.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_find_leaf_ids.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_find_root_ids.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_find_root_ids.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_has_compact_ids.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_has_compact_ids.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_has_contiguous_ids.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_has_contiguous_ids.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_has_multiple_roots.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_has_multiple_roots.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_is_asexual.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_is_asexual.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_is_chronologically_ordered.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_is_chronologically_ordered.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_is_sexual.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_is_sexual.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_is_topologically_sorted.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_is_topologically_sorted.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_make_ancestor_id_col.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_make_ancestor_id_col.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_make_ancestor_list_col.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_make_ancestor_list_col.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_parse_ancestor_id.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_parse_ancestor_id.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_parse_ancestor_ids.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_parse_ancestor_ids.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_reroot_at_id_asexual.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_reroot_at_id_asexual.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_splay_polytomies.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_splay_polytomies.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_to_working_format.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_to_working_format.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_topological_sort.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_topological_sort.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_try_add_ancestor_id_col.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_try_add_ancestor_id_col.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_unfurl_lineage_asexual.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_unfurl_lineage_asexual.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_alifestd_validate.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_alifestd_validate.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_all_same.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_all_same.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_all_unique.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_all_unique.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_anynode_deepcopy_except_neighbors.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_anynode_deepcopy_except_neighbors.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_anytree_calc_leaf_counts.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_anytree_calc_leaf_counts.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_anytree_cardinality.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_anytree_cardinality.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_anytree_has_grandparent.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_anytree_has_grandparent.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_anytree_has_sibling.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_anytree_has_sibling.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_anytree_iterative_deepcopy.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_anytree_iterative_deepcopy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_anytree_peel_sibling_to_cousin.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_anytree_peel_sibling_to_cousin.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_anytree_tree_to_alife_dataframe.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_anytree_tree_to_alife_dataframe.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_apply_swaps.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_apply_swaps.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_as_compact_type.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_as_compact_type.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_as_nullable_type.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_as_nullable_type.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_assign_intersecting_subsets.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_assign_intersecting_subsets.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_bit_ceil.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_bit_ceil.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_bit_floor.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_bit_floor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_capitalize_n.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_capitalize_n.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_cmp.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_cmp.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_cmp_approx.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_cmp_approx.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_consume.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_consume.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_coshuffled.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_coshuffled.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_count_unique.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_count_unique.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_curried_binary_search_jit.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_curried_binary_search_jit.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_deep_listify.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_deep_listify.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_demark.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_demark.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_find_bounds.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_find_bounds.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_flag_last.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_flag_last.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_flat_len.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_flat_len.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_generate_omission_subsets.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_generate_omission_subsets.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_get_nullable_mask.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_get_nullable_mask.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_get_nullable_vals.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_get_nullable_vals.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_give_len.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_give_len.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_indices_of_unique.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_indices_of_unique.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_is_base64.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_is_base64.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_is_nondecreasing.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_is_nondecreasing.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_is_nonincreasing.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_is_nonincreasing.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_is_strictly_decreasing.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_is_strictly_decreasing.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_is_strictly_increasing.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_is_strictly_increasing.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_is_subset.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_is_subset.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_iter_chunks.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_iter_chunks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_iter_monotonic_equivalencies.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_iter_monotonic_equivalencies.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_iter_monotonic_equivalencies_reverse.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_iter_monotonic_equivalencies_reverse.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_iter_slices.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_iter_slices.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_make_intersecting_subsets.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_make_intersecting_subsets.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_memoize_generator.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_memoize_generator.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_min_array_dtype.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_min_array_dtype.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_numpy_fromiter_polyfill.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_numpy_fromiter_polyfill.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_numpy_index.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_numpy_index.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_numpy_index_flat.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_numpy_index_flat.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_pairwise.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_pairwise.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_parse_from_numeral_system.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_parse_from_numeral_system.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_random_choice_generator.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_random_choice_generator.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_render_to_numeral_system.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_render_to_numeral_system.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_reversed_enumerate.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_reversed_enumerate.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_reversed_range.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_reversed_range.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_seed_random.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_seed_random.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_splicewhile.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_splicewhile.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_swap_rows_and_indices.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_swap_rows_and_indices.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_to_tril.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_to_tril.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_unfurl_lineage_with_contiguous_ids.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_unfurl_lineage_with_contiguous_ids.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_unpairwise.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_unpairwise.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_unzip.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_unzip.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_with_omission.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_with_omission.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_with_rng_state_context.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_with_rng_state_context.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_auxiliary_lib/test_zip_strict.py` & `hstrat-1.7.3/tests/test_hstrat/test_auxiliary_lib/test_zip_strict.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_frozen_instrumentation/test_HereditaryStratigraphicAssemblage.py` & `hstrat-1.7.3/tests/test_hstrat/test_frozen_instrumentation/test_HereditaryStratigraphicAssemblage.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_frozen_instrumentation/test_HereditaryStratigraphicAssemblageSpecimen.py` & `hstrat-1.7.3/tests/test_hstrat/test_frozen_instrumentation/test_HereditaryStratigraphicAssemblageSpecimen.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_frozen_instrumentation/test_HereditaryStratigraphicSpecimen.py` & `hstrat-1.7.3/tests/test_hstrat/test_frozen_instrumentation/test_HereditaryStratigraphicSpecimen.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_genome_instrumentation/test_HereditaryStratigraphicColumn.py` & `hstrat-1.7.3/tests/test_hstrat/test_genome_instrumentation/test_HereditaryStratigraphicColumn.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_genome_instrumentation/test_HereditaryStratigraphicColumnBundle.py` & `hstrat-1.7.3/tests/test_hstrat/test_genome_instrumentation/test_HereditaryStratigraphicColumnBundle.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_genome_instrumentation/test_HereditaryStratum.py` & `hstrat-1.7.3/tests/test_hstrat/test_genome_instrumentation/test_HereditaryStratum.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_genome_instrumentation/test_stratum_ordered_stores/test_HereditaryStratumOrderedStoreDict.py` & `hstrat-1.7.3/tests/test_hstrat/test_genome_instrumentation/test_stratum_ordered_stores/test_HereditaryStratumOrderedStoreDict.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_genome_instrumentation/test_stratum_ordered_stores/test_HereditaryStratumOrderedStoreList.py` & `hstrat-1.7.3/tests/test_hstrat/test_genome_instrumentation/test_stratum_ordered_stores/test_HereditaryStratumOrderedStoreList.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_genome_instrumentation/test_stratum_ordered_stores/test_HereditaryStratumOrderedStoreTree.py` & `hstrat-1.7.3/tests/test_hstrat/test_genome_instrumentation/test_stratum_ordered_stores/test_HereditaryStratumOrderedStoreTree.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_definitive_max_rank_of_first_retained_disparity_between.py` & `hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_definitive_max_rank_of_first_retained_disparity_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_definitive_max_rank_of_last_retained_commonality_between.py` & `hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_definitive_max_rank_of_last_retained_commonality_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_definitive_min_ranks_since_first_retained_disparity_with.py` & `hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_definitive_min_ranks_since_first_retained_disparity_with.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_definitive_min_ranks_since_last_retained_commonality_with.py` & `hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_definitive_min_ranks_since_last_retained_commonality_with.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_min_implausible_spurious_consecutive_differentia_collisions_between.py` & `hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_min_implausible_spurious_consecutive_differentia_collisions_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_probability_differentia_collision_between.py` & `hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_probability_differentia_collision_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_rank_of_first_retained_disparity_between.py` & `hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_rank_of_first_retained_disparity_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_rank_of_last_retained_commonality_between.py` & `hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_rank_of_last_retained_commonality_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_ranks_since_first_retained_disparity_with.py` & `hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_ranks_since_first_retained_disparity_with.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_calc_ranks_since_last_retained_commonality_with.py` & `hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_calc_ranks_since_last_retained_commonality_with.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_diff_retained_ranks.py` & `hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_diff_retained_ranks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_get_nth_common_rank_between.py` & `hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_get_nth_common_rank_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_impl/test_dispatch_impl.py` & `hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_impl/test_dispatch_impl.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_impl_column/test_iter_ranks_of_retained_commonality_between_generic.py` & `hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_impl_column/test_iter_ranks_of_retained_commonality_between_generic.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_impl_specimen/test_calc_rank_of_first_retained_disparity_between_specimen_naive.py` & `hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_impl_specimen/test_calc_rank_of_first_retained_disparity_between_specimen_naive.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_juxtaposition/test_impl_specimen/test_calc_rank_of_last_retained_commonality_between_specimen_naive.py` & `hstrat-1.7.3/tests/test_hstrat/test_juxtaposition/test_impl_specimen/test_calc_rank_of_last_retained_commonality_between_specimen_naive.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_estimators/test_estimate_rank_of_mrca_maximum_likelihood.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_estimators/test_estimate_rank_of_mrca_maximum_likelihood.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_estimators/test_estimate_rank_of_mrca_naive.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_estimators/test_estimate_rank_of_mrca_naive.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_estimators/test_estimate_rank_of_mrca_unbiased.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_estimators/test_estimate_rank_of_mrca_unbiased.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_ballpark_patristic_distance_between.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_ballpark_patristic_distance_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_ballpark_rank_of_mrca_between.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_ballpark_rank_of_mrca_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_ballpark_ranks_since_mrca_with.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_ballpark_ranks_since_mrca_with.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_patristic_distance_bounds_between.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_patristic_distance_bounds_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_rank_of_earliest_detectable_mrca_between.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_rank_of_earliest_detectable_mrca_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_rank_of_mrca_bounds_between.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_rank_of_mrca_bounds_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_rank_of_mrca_bounds_provided_confidence_level.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_rank_of_mrca_bounds_provided_confidence_level.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_rank_of_mrca_uncertainty_between.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_rank_of_mrca_uncertainty_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_ranks_since_earliest_detectable_mrca_with.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_ranks_since_earliest_detectable_mrca_with.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_ranks_since_mrca_bounds_provided_confidence_level.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_ranks_since_mrca_bounds_provided_confidence_level.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_ranks_since_mrca_bounds_with.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_ranks_since_mrca_bounds_with.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_ranks_since_mrca_uncertainty_with.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_calc_ranks_since_mrca_uncertainty_with.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_does_definitively_have_no_common_ancestor.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_does_definitively_have_no_common_ancestor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_does_have_any_common_ancestor.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_does_have_any_common_ancestor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_estimate_patristic_distance_between.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_estimate_patristic_distance_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_estimate_rank_of_mrca_between.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_estimate_rank_of_mrca_between.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_estimate_ranks_since_mrca_with.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_pairwise/test_estimate_ranks_since_mrca_with.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_population/test_build_distance_matrix_biopython.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_population/test_build_distance_matrix_biopython.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_population/test_build_distance_matrix_numpy.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_population/test_build_distance_matrix_numpy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_population/test_calc_rank_of_earliest_detectable_mrca_among.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_population/test_calc_rank_of_earliest_detectable_mrca_among.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_population/test_calc_rank_of_mrca_bounds_among.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_population/test_calc_rank_of_mrca_bounds_among.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_population/test_calc_rank_of_mrca_uncertainty_among.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_population/test_calc_rank_of_mrca_uncertainty_among.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_population/test_does_definitively_share_no_common_ancestor.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_population/test_does_definitively_share_no_common_ancestor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_population/test_does_share_any_common_ancestor.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_population/test_does_share_any_common_ancestor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_ArbitraryPrior.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_ArbitraryPrior.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_BubbleWrappedPrior.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_BubbleWrappedPrior.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_ExponentialPrior.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_ExponentialPrior.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_GeometricPrior.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_GeometricPrior.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_UniformPrior.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_priors/test_UniformPrior.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/__init__.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/__init__.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/_tree_quartet_distance.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/_tree_quartet_distance.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/_tree_unweighted_robinson_foulds_distance.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/_impl/_tree_unweighted_robinson_foulds_distance.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/nk_ecoeaselection.csv` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/nk_ecoeaselection.csv`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/nk_lexicaseselection.csv` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/nk_lexicaseselection.csv`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/nk_tournamentselection.csv` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/assets/nk_tournamentselection.csv`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree_nj.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree_nj.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree_trie.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree_trie.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree_trie_ensemble.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree_trie_ensemble.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree_upgma.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_build_tree_upgma.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_TrieInnerNode.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_TrieInnerNode.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_TrieLeafNode.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_TrieLeafNode.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_append_genesis_organism.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_append_genesis_organism.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_estimate_origin_times.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_estimate_origin_times.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_find_chronological_root.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_find_chronological_root.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_find_chronological_roots.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_find_chronological_roots.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_time_calibrate_tree.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_impl/test_time_calibrate_tree.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_AssignDestructionTimeYoungestPlusOneTriePostprocessor.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_AssignDestructionTimeYoungestPlusOneTriePostprocessor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_AssignOriginTimeExpectedValueTriePostprocessor.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_AssignOriginTimeExpectedValueTriePostprocessor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_AssignOriginTimeNaiveTriePostprocessor.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_AssignOriginTimeNaiveTriePostprocessor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_AssignOriginTimeNodeRankTriePostprocessor.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_AssignOriginTimeNodeRankTriePostprocessor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_CompoundTriePostprocessor.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_CompoundTriePostprocessor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_PeelBackConjoinedLeavesTriePostprocessor.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_PeelBackConjoinedLeavesTriePostprocessor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_SampleAncestralRollbacksTriePostprocessor.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_SampleAncestralRollbacksTriePostprocessor.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_bias_adjustment.py` & `hstrat-1.7.3/tests/test_hstrat/test_phylogenetic_inference/test_tree/test_trie_postprocess/test_bias_adjustment.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_serialization/test_assemblage_from_records.py` & `hstrat-1.7.3/tests/test_hstrat/test_serialization/test_assemblage_from_records.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_serialization/test_col_to_dataframe.py` & `hstrat-1.7.3/tests/test_hstrat/test_serialization/test_col_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_serialization/test_col_to_records.py` & `hstrat-1.7.3/tests/test_hstrat/test_serialization/test_col_to_records.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_serialization/test_col_to_specimen.py` & `hstrat-1.7.3/tests/test_hstrat/test_serialization/test_col_to_specimen.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_serialization/test_impl/test_col_records_from_pop_records.py` & `hstrat-1.7.3/tests/test_hstrat/test_serialization/test_impl/test_col_records_from_pop_records.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_serialization/test_pack_differentiae.py` & `hstrat-1.7.3/tests/test_hstrat/test_serialization/test_pack_differentiae.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_serialization/test_pop_to_assemblage.py` & `hstrat-1.7.3/tests/test_hstrat/test_serialization/test_pop_to_assemblage.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_serialization/test_pop_to_dataframe.py` & `hstrat-1.7.3/tests/test_hstrat/test_serialization/test_pop_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_serialization/test_pop_to_records.py` & `hstrat-1.7.3/tests/test_hstrat/test_serialization/test_pop_to_records.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_serialization/test_specimen_from_records.py` & `hstrat-1.7.3/tests/test_hstrat/test_serialization/test_specimen_from_records.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_serialization/test_unassemblage_from_records.py` & `hstrat-1.7.3/tests/test_hstrat/test_serialization/test_unassemblage_from_records.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_serialization/test_unpack_differentiae.py` & `hstrat-1.7.3/tests/test_hstrat/test_serialization/test_unpack_differentiae.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyRelExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyRelExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcNumStrataRetainedExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcNumStrataRetainedExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcNumStrataRetainedUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcNumStrataRetainedUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcRankAtColumnIndex.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_CalcRankAtColumnIndex.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_GenDropRanks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_IterRetainedRanks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_IterRetainedRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_Policy.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_PolicySpec.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_algo/test_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyAbsExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyAbsExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyRelExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyRelExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyRelUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyRelUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcNumStrataRetainedExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcNumStrataRetainedExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcNumStrataRetainedUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcNumStrataRetainedUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcRankAtColumnIndex.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_CalcRankAtColumnIndex.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_GenDropRanks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_IterRetainedRanks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_IterRetainedRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_Policy.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_PolicySpec.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_depth_proportional_resolution_tapered_algo/test_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyRelExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyRelExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcNumStrataRetainedExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcNumStrataRetainedExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcNumStrataRetainedUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcNumStrataRetainedUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcRankAtColumnIndex.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_CalcRankAtColumnIndex.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_GenDropRanks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_IterRetainedRanks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_IterRetainedRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_Policy.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_PolicySpec.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_fixed_resolution_algo/test_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyAbsExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyAbsExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyAbsUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyAbsUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyRelExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyRelExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyRelUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyRelUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcNumStrataRetainedExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcNumStrataRetainedExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcNumStrataRetainedUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcNumStrataRetainedUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcRankAtColumnIndex.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_CalcRankAtColumnIndex.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_GenDropRanks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_IterRetainedRanks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_IterRetainedRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_Policy.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_PolicySpec.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_algo/test_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyAbsExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyAbsExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyRelExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyRelExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyRelUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyRelUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcNumStrataRetainedExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcNumStrataRetainedExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcNumStrataRetainedUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcNumStrataRetainedUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcRankAtColumnIndex.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_CalcRankAtColumnIndex.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_GenDropRanks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_IterRetainedRanks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_IterRetainedRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_Policy.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_PolicySpec.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_geom_seq_nth_root_tapered_algo/test_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyRelExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyRelExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcNumStrataRetainedExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcNumStrataRetainedExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcNumStrataRetainedUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcNumStrataRetainedUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcRankAtColumnIndex.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_CalcRankAtColumnIndex.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_GenDropRanks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_IterRetainedRanks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_IterRetainedRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_Policy.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_PolicySpec.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_nominal_resolution_algo/test_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyRelExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyRelExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcNumStrataRetainedExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcNumStrataRetainedExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcNumStrataRetainedUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcNumStrataRetainedUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcRankAtColumnIndex.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_CalcRankAtColumnIndex.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_GenDropRanks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_IterRetainedRanks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_IterRetainedRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_Policy.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_PolicySpec.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_perfect_resolution_algo/test_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyAbsUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyAbsUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyRelUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyRelUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcNumStrataRetainedUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_CalcNumStrataRetainedUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_GenDropRanks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_Policy.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_PolicySpec.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_pseudostochastic_algo/test_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyRelExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyRelExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcNumStrataRetainedExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcNumStrataRetainedExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcNumStrataRetainedUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcNumStrataRetainedUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcRankAtColumnIndex.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_CalcRankAtColumnIndex.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_GenDropRanks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_IterRetainedRanks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_IterRetainedRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_Policy.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_PolicySpec.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_algo/test_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/impl/iter_backing_policy_transition_ranks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/impl/iter_backing_policy_transition_ranks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyAbsExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyAbsExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyAbsUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyAbsUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyRelExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyRelExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyRelUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyRelUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcNumStrataRetainedExact.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcNumStrataRetainedExact.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcNumStrataRetainedUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcNumStrataRetainedUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcRankAtColumnIndex.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_CalcRankAtColumnIndex.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_GenDropRanks/test_eq.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_GenDropRanks/test_eq.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_GenDropRanks/test_impl_consistency.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_GenDropRanks/test_impl_consistency.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_GenDropRanks/test_policy_consistency.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_GenDropRanks/test_policy_consistency.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_backing_policy_transition_consistency.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_backing_policy_transition_consistency.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_eq.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_eq.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_implementation_consistency_at_backing_policy_transitions.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_implementation_consistency_at_backing_policy_transitions.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_only_dwindling_over_time.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_only_dwindling_over_time.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_ranks_sorted_and_unique.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_ranks_sorted_and_unique.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_ranks_valid.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_ranks_valid.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_zero_and_last_ranks_retained.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_IterRetainedRanks/test_zero_and_last_ranks_retained.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_Policy.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_PolicySpec.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_impl/test_calc_geom_seq_nth_root_transition_rank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_impl/test_calc_geom_seq_nth_root_transition_rank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_impl/test_iter_backing_policy_transition_ranks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_recency_proportional_resolution_curbed_algo/test_impl/test_iter_backing_policy_transition_ranks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyAbsUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyAbsUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyAbsUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyAbsUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyRelUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyRelUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyRelUpperBoundAtPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcMrcaUncertaintyRelUpperBoundPessimalRank.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcNumStrataRetainedUpperBound.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_CalcNumStrataRetainedUpperBound.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_GenDropRanks.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_GenDropRanks.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_Policy.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_Policy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_PolicySpec.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_algorithms/test_stochastic_algo/test_PolicySpec.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_MrcaUncertaintyAbsExactEvaluator.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_MrcaUncertaintyAbsExactEvaluator.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_MrcaUncertaintyAbsUpperBoundEvaluator.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_MrcaUncertaintyAbsUpperBoundEvaluator.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_MrcaUncertaintyRelExactEvaluator.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_MrcaUncertaintyRelExactEvaluator.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_MrcaUncertaintyRelUpperBoundEvaluator.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_MrcaUncertaintyRelUpperBoundEvaluator.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_NumStrataRetainedExactEvaluator.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_NumStrataRetainedExactEvaluator.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_NumStrataRetainedUpperBoundEvaluator.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_strategy/test_stratum_retention_policy_evaluators/test_NumStrataRetainedUpperBoundEvaluator.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/conftest.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/conftest.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_animate/test_policy_panel_animate.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_animate/test_policy_panel_animate.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_animate/test_stratum_retention_animate.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_animate/test_stratum_retention_animate.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_mrca_uncertainty_absolute_barplot.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_mrca_uncertainty_absolute_barplot.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_mrca_uncertainty_relative_barplot.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_mrca_uncertainty_relative_barplot.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_policy_panel_plot.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_policy_panel_plot.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_strata_retained_frac_lineplot.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_strata_retained_frac_lineplot.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_strata_retained_num_lineplot.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_strata_retained_num_lineplot.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_stratum_retention_dripplot.py` & `hstrat-1.7.3/tests/test_hstrat/test_stratum_retention_viz/test_plot/test_stratum_retention_dripplot.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/nk_ecoeaselection.csv` & `hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/nk_ecoeaselection.csv`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/nk_lexicaseselection.csv` & `hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/nk_lexicaseselection.csv`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_test_drive/assets/nk_tournamentselection.csv` & `hstrat-1.7.3/tests/test_hstrat/test_test_drive/assets/nk_tournamentselection.csv`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_DecantingPhyloTracker.py` & `hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_DecantingPhyloTracker.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_GarbageCollectingPhyloTracker.py` & `hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_GarbageCollectingPhyloTracker.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny.py` & `hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_alifestd.py` & `hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_alifestd.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_biopython.py` & `hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_biopython.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_dendropy.py` & `hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_dendropy.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_naive.py` & `hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_naive.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_networkx.py` & `hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_networkx.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_posthoc.py` & `hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_descend_template_phylogeny_posthoc.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_evolve_fitness_trait_population.py` & `hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_evolve_fitness_trait_population.py`

 * *Files identical despite different names*

### Comparing `hstrat-1.7.2/tests/test_hstrat/test_test_drive/test_perfect_tracking.py` & `hstrat-1.7.3/tests/test_hstrat/test_test_drive/test_perfect_tracking.py`

 * *Files identical despite different names*

