# Comparing `tmp/libmata-0.68.0.tar.gz` & `tmp/libmata-0.69.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmata-0.68.0.tar", last modified: Tue Jun 20 13:18:17 2023, max compression
+gzip compressed data, was "libmata-0.69.0.tar", last modified: Thu Jun 22 05:26:37 2023, max compression
```

## Comparing `libmata-0.68.0.tar` & `libmata-0.69.0.tar`

### file list

```diff
@@ -1,422 +1,422 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.963143 libmata-0.68.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-06-20 13:18:17.963143 libmata-0.68.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)  1876374 2023-06-20 13:15:59.802600 libmata-0.68.0/libmata.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-06-20 13:15:13.974416 libmata-0.68.0/libmata.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    69663 2023-06-20 13:15:13.974416 libmata-0.68.0/libmata.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.947143 libmata-0.68.0/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.951143 libmata-0.68.0/mata/3rdparty/
--rw-r--r--   0 runner    (1001) docker     (123)    79534 2023-06-20 13:15:13.926414 libmata-0.68.0/mata/3rdparty/args.hxx
--rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-06-20 13:15:13.934414 libmata-0.68.0/mata/3rdparty/catch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   417675 2023-06-20 13:15:13.930414 libmata-0.68.0/mata/3rdparty/catch.hpp.1.9.3
--rw-r--r--   0 runner    (1001) docker     (123)   416932 2023-06-20 13:15:13.934414 libmata-0.68.0/mata/3rdparty/catch.hpp.2.0.1
--rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-06-20 13:15:13.934414 libmata-0.68.0/mata/3rdparty/catch.hpp.2.13.9
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.951143 libmata-0.68.0/mata/3rdparty/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)   104287 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/Doxyfile.in
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/README
--rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/RELEASE.NOTES
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.955143 libmata-0.68.0/mata/3rdparty/cudd/cplusplus/
--rw-r--r--   0 runner    (1001) docker     (123)   118373 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cplusplus/testmulti.cc
--rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cplusplus/testobj.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.955143 libmata-0.68.0/mata/3rdparty/cudd/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAPI.c
--rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAddApply.c
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAddFind.c
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAddInv.c
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c
--rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAnneal.c
--rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddApa.c
--rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddApprox.c
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c
--rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddBddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddBridge.c
--rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddCheck.c
--rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddClip.c
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddCompose.c
--rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddDecomp.c
--rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddEssent.c
--rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-06-20 13:15:13.954415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddExact.c
--rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddExport.c
--rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddGenCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddGenetic.c
--rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddHarwell.c
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddInit.c
--rw-r--r--   0 runner    (1001) docker     (123)    47195 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddInteract.c
--rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddLCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c
--rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddLinear.c
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddLiteral.c
--rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddMatMult.c
--rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddPriority.c
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddRead.c
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddRef.c
--rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddReorder.c
--rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddSat.c
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddSign.c
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddSolve.c
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddSplit.c
--rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c
--rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c
--rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c
--rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddTable.c
--rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddWindow.c
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddCount.c
--rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c
--rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-06-20 13:15:13.958415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c
--rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddLin.c
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddPort.c
--rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddReord.c
--rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c
--rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c
--rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/cudd/r7x8.1.mat
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/cudd/test_cudd.test.in
--rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/cudd/testcudd.c
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/cudd/testextra.c
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/cudd_config.h.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.955143 libmata-0.68.0/mata/3rdparty/cudd/dddmp/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/README.dddmp
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/README.testdddmp
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES
--rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmp.h
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c
--rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.959143 libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/cmdIndex.html
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/commands.html
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/credit.html
--rw-r--r--   0 runner    (1001) docker     (123)    64661 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps
--rw-r--r--   0 runner    (1001) docker     (123)    64648 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps
--rw-r--r--   0 runner    (1001) docker     (123)    23413 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFile.html
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFunc.html
--rw-r--r--   0 runner    (1001) docker     (123)   127869 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html
--rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-20 13:15:13.962415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmpExt.html
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html
--rw-r--r--   0 runner    (1001) docker     (123)    27862 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmpTitle.html
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/packages.html
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/pkgIndex.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.959143 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/0.add
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/0.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/1.add
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/2.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/3.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4.cnf
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4.max1
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4.max2
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/5.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/one.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/s27RP1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd.bis
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp2.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/varauxids.ord
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/varnames.ord
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/zero.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/test_dddmp.test.in
--rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/dddmp/testdddmp.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.959143 libmata-0.68.0/mata/3rdparty/cudd/doc/
--rw-r--r--   0 runner    (1001) docker     (123)    97463 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/doc/cudd.tex.in
--rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/doc/phase.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.959143 libmata-0.68.0/mata/3rdparty/cudd/epd/
--rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/epd/epd.c
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/epd/epd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/epd/epdInt.h
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/groups.dox
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.943143 libmata-0.68.0/mata/3rdparty/cudd/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.943143 libmata-0.68.0/mata/3rdparty/cudd/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.959143 libmata-0.68.0/mata/3rdparty/cudd/include/mata/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h
--rw-r--r--   0 runner    (1001) docker     (123)    29061 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.959143 libmata-0.68.0/mata/3rdparty/cudd/mtr/
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/mtr/mtr.h
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/mtr/mtrBasic.c
--rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/mtr/mtrGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/mtr/mtrInt.h
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/mtr/test.groups
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/mtr/test_mtr.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/mtr/testmtr.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.959143 libmata-0.68.0/mata/3rdparty/cudd/st/
--rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/st/st.c
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/st/st.h
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/st/test_st.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/st/testst.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.959143 libmata-0.68.0/mata/3rdparty/cudd/util/
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/util/cpu_stats.c
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/util/cpu_time.c
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/util/cstringstream.c
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/util/cstringstream.h
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/util/datalimit.c
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/util/pathsearch.c
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/util/pipefork.c
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/util/prtime.c
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/util/safe_mem.c
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-20 13:15:13.966415 libmata-0.68.0/mata/3rdparty/cudd/util/strsav.c
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/cudd/util/texpand.c
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/cudd/util/ucbqsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/cudd/util/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.955143 libmata-0.68.0/mata/3rdparty/cudd-min/
--rw-r--r--   0 runner    (1001) docker     (123)    57591 2023-06-20 13:15:13.934414 libmata-0.68.0/mata/3rdparty/cudd-min/bnet.c
--rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-06-20 13:15:13.934414 libmata-0.68.0/mata/3rdparty/cudd-min/bnet.h
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-06-20 13:15:13.934414 libmata-0.68.0/mata/3rdparty/cudd-min/chkMterm.c
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-06-20 13:15:13.934414 libmata-0.68.0/mata/3rdparty/cudd-min/config.h
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-06-20 13:15:13.934414 libmata-0.68.0/mata/3rdparty/cudd-min/cpu_stats.c
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-20 13:15:13.934414 libmata-0.68.0/mata/3rdparty/cudd-min/cpu_time.c
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-20 13:15:13.934414 libmata-0.68.0/mata/3rdparty/cudd-min/cstringstream.c
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-20 13:15:13.934414 libmata-0.68.0/mata/3rdparty/cudd-min/cstringstream.h
--rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-06-20 13:15:13.934414 libmata-0.68.0/mata/3rdparty/cudd-min/cudd.h
--rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-06-20 13:15:13.934414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddAPI.c
--rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-06-20 13:15:13.934414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddAddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-06-20 13:15:13.934414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddAddApply.c
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddAddFind.c
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddAddInv.c
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddAddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddAddNeg.c
--rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddAddWalsh.c
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddAndAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddAnneal.c
--rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddApa.c
--rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddApprox.c
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddBddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddBddCorr.c
--rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddBddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddBridge.c
--rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddCheck.c
--rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddClip.c
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddCompose.c
--rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddDecomp.c
--rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddEssent.c
--rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddExact.c
--rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddExport.c
--rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddGenCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddGenetic.c
--rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-06-20 13:15:13.938414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddHarwell.c
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddInit.c
--rw-r--r--   0 runner    (1001) docker     (123)    47179 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddInteract.c
--rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddLCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddLevelQ.c
--rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddLinear.c
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddLiteral.c
--rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddMatMult.c
--rw-r--r--   0 runner    (1001) docker     (123)   118352 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddObj.cc
--rw-r--r--   0 runner    (1001) docker     (123)    29046 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddObj.hh
--rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddPriority.c
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddRead.c
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddRef.c
--rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddReorder.c
--rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddSat.c
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddSign.c
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddSolve.c
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddSplit.c
--rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddSubsetHB.c
--rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddSubsetSP.c
--rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddSymmetry.c
--rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-06-20 13:15:13.942414 libmata-0.68.0/mata/3rdparty/cudd-min/cuddTable.c
--rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/cuddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/cuddWindow.c
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddCount.c
--rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddFuncs.c
--rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddIsop.c
--rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddLin.c
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddPort.c
--rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddReord.c
--rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddSetop.c
--rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddSymm.c
--rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/datalimit.c
--rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/dddmp.h
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/dddmpBinary.c
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/dddmpConvert.c
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/dddmpDbg.c
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/dddmpInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/dddmpLoad.c
--rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/dddmpLoadCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/dddmpNodeAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/dddmpNodeBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/dddmpNodeCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/dddmpStoreAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/dddmpStoreBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/dddmpStoreCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/dddmpStoreMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/dddmpUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/epd.c
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/epd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-06-20 13:15:13.946415 libmata-0.68.0/mata/3rdparty/cudd-min/epdInt.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.943143 libmata-0.68.0/mata/3rdparty/cudd-min/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.943143 libmata-0.68.0/mata/3rdparty/cudd-min/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.955143 libmata-0.68.0/mata/3rdparty/cudd-min/include/mata/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h
--rw-r--r--   0 runner    (1001) docker     (123)    29047 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh
--rw-r--r--   0 runner    (1001) docker     (123)    42502 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/main.c
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/mtr.h
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/mtrBasic.c
--rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/mtrGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/mtrInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    80087 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/ntr.c
--rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/ntr.h
--rw-r--r--   0 runner    (1001) docker     (123)    60542 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/ntrBddTest.c
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/ntrHeap.c
--rw-r--r--   0 runner    (1001) docker     (123)    56481 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/ntrMflow.c
--rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/ntrShort.c
--rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/ntrZddTest.c
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/pathsearch.c
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/pipefork.c
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/prtime.c
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/safe_mem.c
--rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/st.c
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/st.h
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/strsav.c
--rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/testcudd.c
--rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/testdddmp.c
--rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/testextra.c
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/testmtr.c
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/testmulti.cc
--rw-r--r--   0 runner    (1001) docker     (123)    23917 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/testobj.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/testst.c
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/texpand.c
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/ucbqsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-20 13:15:13.950415 libmata-0.68.0/mata/3rdparty/cudd-min/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.959143 libmata-0.68.0/mata/3rdparty/re2/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.959143 libmata-0.68.0/mata/3rdparty/re2/re2/
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/bitmap256.h
--rw-r--r--   0 runner    (1001) docker     (123)    36693 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/compile.cc
--rw-r--r--   0 runner    (1001) docker     (123)    76014 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/parse.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/perl_groups.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/pod_array.h
--rw-r--r--   0 runner    (1001) docker     (123)    31484 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/prog.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/prog.h
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/re2.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15355 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/re2.h
--rw-r--r--   0 runner    (1001) docker     (123)    20718 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/regexp.cc
--rw-r--r--   0 runner    (1001) docker     (123)    21348 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/regexp.h
--rw-r--r--   0 runner    (1001) docker     (123)    19503 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/simplify.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/sparse_array.h
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/sparse_set.h
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/stringpiece.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/stringpiece.h
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/tostring.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/unicode_casefold.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/unicode_casefold.h
--rw-r--r--   0 runner    (1001) docker     (123)   124977 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/unicode_groups.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/unicode_groups.h
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/re2/walker-inl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.959143 libmata-0.68.0/mata/3rdparty/re2/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/util/logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/util/mutex.h
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/util/rune.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/util/strutil.cc
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/util/strutil.h
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/util/utf.h
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/re2/util/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.943143 libmata-0.68.0/mata/3rdparty/simlib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.943143 libmata-0.68.0/mata/3rdparty/simlib/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.943143 libmata-0.68.0/mata/3rdparty/simlib/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.959143 libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.959143 libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh
--rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-20 13:15:13.970415 libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-20 13:15:13.974416 libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.959143 libmata-0.68.0/mata/3rdparty/simlib/src/
--rw-r--r--   0 runner    (1001) docker     (123)    18209 2023-06-20 13:15:13.974416 libmata-0.68.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-20 13:18:17.851142 libmata-0.68.0/mata/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-06-20 13:18:17.851142 libmata-0.68.0/mata/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 13:18:17.851142 libmata-0.68.0/mata/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.947143 libmata-0.68.0/mata/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.963143 libmata-0.68.0/mata/include/mata/
--rw-r--r--   0 runner    (1001) docker     (123)    17016 2023-06-20 13:15:13.978416 libmata-0.68.0/mata/include/mata/afa.hh
--rw-r--r--   0 runner    (1001) docker     (123)    14741 2023-06-20 13:15:13.978416 libmata-0.68.0/mata/include/mata/alphabet.hh
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-06-20 13:15:13.978416 libmata-0.68.0/mata/include/mata/closed-set.hh
--rw-r--r--   0 runner    (1001) docker     (123)    10229 2023-06-20 13:15:13.978416 libmata-0.68.0/mata/include/mata/inter-aut.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-20 13:15:13.978416 libmata-0.68.0/mata/include/mata/mintermization.hh
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-20 13:15:13.978416 libmata-0.68.0/mata/include/mata/nfa-algorithms.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-20 13:15:13.978416 libmata-0.68.0/mata/include/mata/nfa-plumbing.hh
--rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-06-20 13:15:13.978416 libmata-0.68.0/mata/include/mata/nfa-strings.hh
--rw-r--r--   0 runner    (1001) docker     (123)    43482 2023-06-20 13:15:13.978416 libmata-0.68.0/mata/include/mata/nfa.hh
--rw-r--r--   0 runner    (1001) docker     (123)    16704 2023-06-20 13:15:13.978416 libmata-0.68.0/mata/include/mata/number-predicate.hh
--rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-06-20 13:15:13.978416 libmata-0.68.0/mata/include/mata/ord-vector.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-20 13:15:13.978416 libmata-0.68.0/mata/include/mata/parser.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-20 13:15:13.978416 libmata-0.68.0/mata/include/mata/re2parser.hh
--rw-r--r--   0 runner    (1001) docker     (123)    12550 2023-06-20 13:15:13.978416 libmata-0.68.0/mata/include/mata/synchronized-iterator.hh
--rw-r--r--   0 runner    (1001) docker     (123)    13958 2023-06-20 13:15:13.978416 libmata-0.68.0/mata/include/mata/util.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.963143 libmata-0.68.0/mata/src/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 13:15:13.982416 libmata-0.68.0/mata/src/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.963143 libmata-0.68.0/mata/src/afa/
--rw-r--r--   0 runner    (1001) docker     (123)    37976 2023-06-20 13:15:13.982416 libmata-0.68.0/mata/src/afa/afa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-20 13:15:13.982416 libmata-0.68.0/mata/src/alphabet.cc
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-20 13:15:13.982416 libmata-0.68.0/mata/src/config.cc.in
--rw-r--r--   0 runner    (1001) docker     (123)    26404 2023-06-20 13:15:13.982416 libmata-0.68.0/mata/src/inter-aut.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-06-20 13:15:13.982416 libmata-0.68.0/mata/src/mintermization.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.963143 libmata-0.68.0/mata/src/nfa/
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-20 13:15:13.982416 libmata-0.68.0/mata/src/nfa/nfa-complement.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-20 13:15:13.982416 libmata-0.68.0/mata/src/nfa/nfa-concatenation.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-06-20 13:15:13.982416 libmata-0.68.0/mata/src/nfa/nfa-inclusion.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-20 13:15:13.982416 libmata-0.68.0/mata/src/nfa/nfa-intersection.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-20 13:15:13.982416 libmata-0.68.0/mata/src/nfa/nfa-universal.cc
--rw-r--r--   0 runner    (1001) docker     (123)    75093 2023-06-20 13:15:13.982416 libmata-0.68.0/mata/src/nfa/nfa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11745 2023-06-20 13:15:13.982416 libmata-0.68.0/mata/src/parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)    30710 2023-06-20 13:15:13.982416 libmata-0.68.0/mata/src/re2parser.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:18:17.963143 libmata-0.68.0/mata/src/strings/
--rw-r--r--   0 runner    (1001) docker     (123)    17710 2023-06-20 13:15:13.982416 libmata-0.68.0/mata/src/strings/nfa-noodlification.cc
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-06-20 13:15:13.982416 libmata-0.68.0/mata/src/strings/nfa-segmentation.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-20 13:15:13.982416 libmata-0.68.0/mata/src/strings/nfa-strings.cc
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-20 13:15:13.974416 libmata-0.68.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-06-20 13:15:13.974416 libmata-0.68.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.371559 libmata-0.69.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-06-22 05:26:37.371559 libmata-0.69.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)  1874807 2023-06-22 05:23:37.206935 libmata-0.69.0/libmata.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11915 2023-06-22 05:22:39.442795 libmata-0.69.0/libmata.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    69661 2023-06-22 05:22:39.442795 libmata-0.69.0/libmata.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.347558 libmata-0.69.0/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.347558 libmata-0.69.0/mata/3rdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)    79536 2023-06-22 05:22:39.382795 libmata-0.69.0/mata/3rdparty/args.hxx
+-rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-06-22 05:22:39.390795 libmata-0.69.0/mata/3rdparty/catch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   417675 2023-06-22 05:22:39.386795 libmata-0.69.0/mata/3rdparty/catch.hpp.1.9.3
+-rw-r--r--   0 runner    (1001) docker     (123)   416932 2023-06-22 05:22:39.390795 libmata-0.69.0/mata/3rdparty/catch.hpp.2.0.1
+-rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-06-22 05:22:39.390795 libmata-0.69.0/mata/3rdparty/catch.hpp.2.13.9
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.347558 libmata-0.69.0/mata/3rdparty/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)   104287 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/Doxyfile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/README
+-rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/RELEASE.NOTES
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.355558 libmata-0.69.0/mata/3rdparty/cudd/cplusplus/
+-rw-r--r--   0 runner    (1001) docker     (123)   118858 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cplusplus/testmulti.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cplusplus/testobj.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.359558 libmata-0.69.0/mata/3rdparty/cudd/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAPI.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAddApply.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAddFind.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAddInv.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAnneal.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddApa.c
+-rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddApprox.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddBddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddBridge.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddCheck.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddClip.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddCompose.c
+-rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddDecomp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-06-22 05:22:39.418795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddEssent.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddExact.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddExport.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddGenCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddGenetic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddHarwell.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddInit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47195 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddInteract.c
+-rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddLCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddLinear.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddLiteral.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddMatMult.c
+-rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddPriority.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddRead.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddRef.c
+-rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddReorder.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddSat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddSign.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddSolve.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddSplit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c
+-rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-06-22 05:22:39.422795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c
+-rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddTable.c
+-rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddWindow.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddCount.c
+-rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddLin.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddPort.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddReord.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/cudd/r7x8.1.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/cudd/test_cudd.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/cudd/testcudd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/cudd/testextra.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/cudd_config.h.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.359558 libmata-0.69.0/mata/3rdparty/cudd/dddmp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/README.dddmp
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/README.testdddmp
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES
+-rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-06-22 05:22:39.426795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.363558 libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/cmdIndex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/commands.html
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/credit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    64661 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps
+-rw-r--r--   0 runner    (1001) docker     (123)    64648 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps
+-rw-r--r--   0 runner    (1001) docker     (123)    23413 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFile.html
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFunc.html
+-rw-r--r--   0 runner    (1001) docker     (123)   127869 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html
+-rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmpExt.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)    27862 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmpTitle.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/packages.html
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/pkgIndex.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.363558 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/0.add
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/0.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/1.add
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/2.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/3.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4.max1
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4.max2
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/5.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/one.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/s27RP1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd.bis
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp2.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/varauxids.ord
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/varnames.ord
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/zero.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-22 05:22:39.430795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/test_dddmp.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/dddmp/testdddmp.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.363558 libmata-0.69.0/mata/3rdparty/cudd/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    97463 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/doc/cudd.tex.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/doc/phase.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.363558 libmata-0.69.0/mata/3rdparty/cudd/epd/
+-rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/epd/epd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/epd/epd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/epd/epdInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/groups.dox
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.339558 libmata-0.69.0/mata/3rdparty/cudd/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.339558 libmata-0.69.0/mata/3rdparty/cudd/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.363558 libmata-0.69.0/mata/3rdparty/cudd/include/mata/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29098 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.363558 libmata-0.69.0/mata/3rdparty/cudd/mtr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/mtr/mtr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/mtr/mtrBasic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/mtr/mtrGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/mtr/mtrInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/mtr/test.groups
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/mtr/test_mtr.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/mtr/testmtr.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.363558 libmata-0.69.0/mata/3rdparty/cudd/st/
+-rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/st/st.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/st/st.h
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/st/test_st.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/st/testst.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.363558 libmata-0.69.0/mata/3rdparty/cudd/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/util/cpu_stats.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/util/cpu_time.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/util/cstringstream.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/util/cstringstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/util/datalimit.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/util/pathsearch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/util/pipefork.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/util/prtime.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/util/safe_mem.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/util/strsav.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/util/texpand.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/util/ucbqsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/cudd/util/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.355558 libmata-0.69.0/mata/3rdparty/cudd-min/
+-rw-r--r--   0 runner    (1001) docker     (123)    57591 2023-06-22 05:22:39.390795 libmata-0.69.0/mata/3rdparty/cudd-min/bnet.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-06-22 05:22:39.390795 libmata-0.69.0/mata/3rdparty/cudd-min/bnet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-06-22 05:22:39.390795 libmata-0.69.0/mata/3rdparty/cudd-min/chkMterm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-06-22 05:22:39.390795 libmata-0.69.0/mata/3rdparty/cudd-min/config.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-06-22 05:22:39.390795 libmata-0.69.0/mata/3rdparty/cudd-min/cpu_stats.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-22 05:22:39.390795 libmata-0.69.0/mata/3rdparty/cudd-min/cpu_time.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-22 05:22:39.390795 libmata-0.69.0/mata/3rdparty/cudd-min/cstringstream.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-06-22 05:22:39.390795 libmata-0.69.0/mata/3rdparty/cudd-min/cstringstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-06-22 05:22:39.390795 libmata-0.69.0/mata/3rdparty/cudd-min/cudd.h
+-rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-06-22 05:22:39.394795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddAPI.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-06-22 05:22:39.394795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddAddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-06-22 05:22:39.394795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddAddApply.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-06-22 05:22:39.394795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddAddFind.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-22 05:22:39.394795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddAddInv.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-06-22 05:22:39.394795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddAddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-22 05:22:39.394795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddAddNeg.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-06-22 05:22:39.398795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddAddWalsh.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-06-22 05:22:39.398795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddAndAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-06-22 05:22:39.398795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddAnneal.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-06-22 05:22:39.398795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddApa.c
+-rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-06-22 05:22:39.398795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddApprox.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-22 05:22:39.398795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddBddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-06-22 05:22:39.398795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddBddCorr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-06-22 05:22:39.398795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddBddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-06-22 05:22:39.398795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddBridge.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-06-22 05:22:39.398795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-06-22 05:22:39.398795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddCheck.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-06-22 05:22:39.398795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddClip.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-06-22 05:22:39.398795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-06-22 05:22:39.398795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddCompose.c
+-rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-06-22 05:22:39.402795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddDecomp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-06-22 05:22:39.402795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddEssent.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-06-22 05:22:39.402795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddExact.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-06-22 05:22:39.402795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddExport.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-06-22 05:22:39.402795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddGenCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-06-22 05:22:39.402795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddGenetic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-06-22 05:22:39.402795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-06-22 05:22:39.402795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddHarwell.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-06-22 05:22:39.402795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddInit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47179 2023-06-22 05:22:39.402795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-06-22 05:22:39.402795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddInteract.c
+-rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-06-22 05:22:39.402795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddLCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-06-22 05:22:39.402795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddLevelQ.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-06-22 05:22:39.402795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddLinear.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-22 05:22:39.402795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddLiteral.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-06-22 05:22:39.402795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddMatMult.c
+-rw-r--r--   0 runner    (1001) docker     (123)   118352 2023-06-22 05:22:39.402795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddObj.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    29046 2023-06-22 05:22:39.402795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddObj.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddPriority.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddRead.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddRef.c
+-rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddReorder.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddSat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddSign.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddSolve.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddSplit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddSubsetHB.c
+-rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddSubsetSP.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddSymmetry.c
+-rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddTable.c
+-rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddWindow.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddCount.c
+-rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddFuncs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddIsop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddLin.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddPort.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddReord.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-06-22 05:22:39.406795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddSetop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddSymm.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/datalimit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/dddmp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/dddmpBinary.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/dddmpConvert.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/dddmpDbg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/dddmpInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/dddmpLoad.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/dddmpLoadCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/dddmpNodeAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/dddmpNodeBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/dddmpNodeCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/dddmpStoreAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/dddmpStoreBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/dddmpStoreCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/dddmpStoreMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/dddmpUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/epd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/epd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/epdInt.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.339558 libmata-0.69.0/mata/3rdparty/cudd-min/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.339558 libmata-0.69.0/mata/3rdparty/cudd-min/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.355558 libmata-0.69.0/mata/3rdparty/cudd-min/include/mata/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29047 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    42502 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/main.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/mtr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/mtrBasic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/mtrGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-06-22 05:22:39.410795 libmata-0.69.0/mata/3rdparty/cudd-min/mtrInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80087 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/ntr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/ntr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    60542 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/ntrBddTest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/ntrHeap.c
+-rw-r--r--   0 runner    (1001) docker     (123)    56481 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/ntrMflow.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/ntrShort.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/ntrZddTest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/pathsearch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/pipefork.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/prtime.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/safe_mem.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/st.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/st.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/strsav.c
+-rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/testcudd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/testdddmp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/testextra.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/testmtr.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/testmulti.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23917 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/testobj.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/testst.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/texpand.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/ucbqsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-22 05:22:39.414795 libmata-0.69.0/mata/3rdparty/cudd-min/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.363558 libmata-0.69.0/mata/3rdparty/re2/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/re2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/re2/CONTRIBUTORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/re2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.367558 libmata-0.69.0/mata/3rdparty/re2/re2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-22 05:22:39.434795 libmata-0.69.0/mata/3rdparty/re2/re2/bitmap256.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36693 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/compile.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    76014 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/parse.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/perl_groups.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/pod_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31484 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/prog.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10788 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/prog.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/re2.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/re2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20718 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/regexp.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    21350 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/regexp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19503 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/simplify.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/sparse_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/sparse_set.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/stringpiece.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/stringpiece.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/tostring.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/unicode_casefold.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/unicode_casefold.h
+-rw-r--r--   0 runner    (1001) docker     (123)   124977 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/unicode_groups.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/unicode_groups.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/re2/walker-inl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.367558 libmata-0.69.0/mata/3rdparty/re2/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/util/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/util/mutex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/util/rune.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/util/strutil.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/util/strutil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/util/utf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/re2/util/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.343558 libmata-0.69.0/mata/3rdparty/simlib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.343558 libmata-0.69.0/mata/3rdparty/simlib/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.343558 libmata-0.69.0/mata/3rdparty/simlib/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.367558 libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.367558 libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    19297 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-06-22 05:22:39.438795 libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-22 05:22:39.442795 libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-22 05:22:39.442795 libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-06-22 05:22:39.442795 libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-22 05:22:39.442795 libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-22 05:22:39.442795 libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.367558 libmata-0.69.0/mata/3rdparty/simlib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    18325 2023-06-22 05:22:39.442795 libmata-0.69.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-22 05:26:37.211558 libmata-0.69.0/mata/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-06-22 05:26:37.211558 libmata-0.69.0/mata/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 05:26:37.211558 libmata-0.69.0/mata/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.343558 libmata-0.69.0/mata/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.367558 libmata-0.69.0/mata/include/mata/
+-rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/include/mata/afa.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/include/mata/alphabet.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    19025 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/include/mata/closed-set.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/include/mata/inter-aut.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/include/mata/mintermization.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/include/mata/nfa-algorithms.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/include/mata/nfa-plumbing.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/include/mata/nfa-strings.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    44007 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/include/mata/nfa.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    16535 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/include/mata/number-predicate.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    15503 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/include/mata/ord-vector.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/include/mata/parser.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/include/mata/re2parser.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12656 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/include/mata/synchronized-iterator.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    13958 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/include/mata/util.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.371559 libmata-0.69.0/mata/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/src/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.371559 libmata-0.69.0/mata/src/afa/
+-rw-r--r--   0 runner    (1001) docker     (123)    38372 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/src/afa/afa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/src/alphabet.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/src/config.cc.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26602 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/src/inter-aut.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/src/mintermization.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.371559 libmata-0.69.0/mata/src/nfa/
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/src/nfa/nfa-complement.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/src/nfa/nfa-concatenation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/src/nfa/nfa-inclusion.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/src/nfa/nfa-intersection.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-22 05:22:39.450796 libmata-0.69.0/mata/src/nfa/nfa-universal.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    75245 2023-06-22 05:22:39.454795 libmata-0.69.0/mata/src/nfa/nfa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-06-22 05:22:39.454795 libmata-0.69.0/mata/src/parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    31732 2023-06-22 05:22:39.454795 libmata-0.69.0/mata/src/re2parser.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:26:37.371559 libmata-0.69.0/mata/src/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)    17716 2023-06-22 05:22:39.454795 libmata-0.69.0/mata/src/strings/nfa-noodlification.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-06-22 05:22:39.454795 libmata-0.69.0/mata/src/strings/nfa-segmentation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-22 05:22:39.454795 libmata-0.69.0/mata/src/strings/nfa-strings.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-22 05:22:39.442795 libmata-0.69.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8279 2023-06-22 05:22:39.442795 libmata-0.69.0/setup.py
```

### Comparing `libmata-0.68.0/PKG-INFO` & `libmata-0.69.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmata
-Version: 0.68.0
+Version: 0.69.0
 Summary: The automata library
 Home-page: https://github.com/verifit/mata
 Author: Lukáš Holík <holik@fit.vutbr.cz>, Ondřej Lengál <lengal@fit.vutbr.cz>, Martin Hruška <ihruskam@fit.vutbr.cz>, Tomáš Fiedor <ifiedortom@fit.vutbr.cz>, David Chocholatý <chocholaty.david@protonmail.com>, Juraj Síč <sicjuraj@fit.vutbr.cz>, Tomáš Vojnar <vojnar@fit.vutbr.cz>
 Author-email: lengal@fit.vutbr.cz
 License: UNKNOWN
 Keywords: automata,finite automata,alternating automata
 Platform: UNKNOWN
```

### Comparing `libmata-0.68.0/libmata.cpp` & `libmata-0.69.0/libmata.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -2251,17 +2251,14 @@
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE unsigned long __Pyx_PyInt_As_unsigned_long(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_int(unsigned int value);
-
 /* PrintOne.proto */
 static int __Pyx_PrintOne(PyObject* stream, PyObject *o);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* SwapException.proto */
@@ -27406,23 +27403,23 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7libmata_12Segmentation_4get_epsilon_depths(struct __pyx_obj_7libmata_Segmentation *__pyx_v_self) {
-  std::unordered_map<unsigned int,std::vector<Mata::Nfa::Trans> >  __pyx_v_c_epsilon_transitions;
+  std::unordered_map<size_t,std::vector<Mata::Nfa::Trans> >  __pyx_v_c_epsilon_transitions;
   PyObject *__pyx_v_result = NULL;
-  std::pair<unsigned int,std::vector<Mata::Nfa::Trans> >  __pyx_v_epsilon_depth_pair;
+  std::pair<size_t,std::vector<Mata::Nfa::Trans> >  __pyx_v_epsilon_depth_pair;
   Mata::Nfa::Trans __pyx_v_trans;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  std::unordered_map<unsigned int,std::vector<Mata::Nfa::Trans> > ::iterator __pyx_t_2;
-  std::pair<unsigned int,std::vector<Mata::Nfa::Trans> >  __pyx_t_3;
+  std::unordered_map<size_t,std::vector<Mata::Nfa::Trans> > ::iterator __pyx_t_2;
+  std::pair<size_t,std::vector<Mata::Nfa::Trans> >  __pyx_t_3;
   std::vector<Mata::Nfa::Trans> ::iterator __pyx_t_4;
   std::vector<Mata::Nfa::Trans>  *__pyx_t_5;
   Mata::Nfa::Trans __pyx_t_6;
   int __pyx_t_7;
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
@@ -27433,34 +27430,34 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_epsilon_depths", 0);
 
   /* "libmata.pyx":1663
  *         :return: Map of depths to lists of -transitions.
  *         """
- *         cdef umap[unsigned, vector[CTrans]] c_epsilon_transitions = self.thisptr.get_epsilon_depths()             # <<<<<<<<<<<<<<
+ *         cdef umap[size_t, vector[CTrans]] c_epsilon_transitions = self.thisptr.get_epsilon_depths()             # <<<<<<<<<<<<<<
  *         result = {}
  *         for epsilon_depth_pair in c_epsilon_transitions:
  */
   __pyx_v_c_epsilon_transitions = __pyx_v_self->thisptr->get_epsilon_depths();
 
   /* "libmata.pyx":1664
  *         """
- *         cdef umap[unsigned, vector[CTrans]] c_epsilon_transitions = self.thisptr.get_epsilon_depths()
+ *         cdef umap[size_t, vector[CTrans]] c_epsilon_transitions = self.thisptr.get_epsilon_depths()
  *         result = {}             # <<<<<<<<<<<<<<
  *         for epsilon_depth_pair in c_epsilon_transitions:
  *             for trans in epsilon_depth_pair.second:
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1664, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_result = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "libmata.pyx":1665
- *         cdef umap[unsigned, vector[CTrans]] c_epsilon_transitions = self.thisptr.get_epsilon_depths()
+ *         cdef umap[size_t, vector[CTrans]] c_epsilon_transitions = self.thisptr.get_epsilon_depths()
  *         result = {}
  *         for epsilon_depth_pair in c_epsilon_transitions:             # <<<<<<<<<<<<<<
  *             for trans in epsilon_depth_pair.second:
  *                 if epsilon_depth_pair.first not in result:
  */
   __pyx_t_2 = __pyx_v_c_epsilon_transitions.begin();
   for (;;) {
@@ -27487,15 +27484,15 @@
       /* "libmata.pyx":1667
  *         for epsilon_depth_pair in c_epsilon_transitions:
  *             for trans in epsilon_depth_pair.second:
  *                 if epsilon_depth_pair.first not in result:             # <<<<<<<<<<<<<<
  *                     result[epsilon_depth_pair.first] = []
  * 
  */
-      __pyx_t_1 = __Pyx_PyInt_From_unsigned_int(__pyx_v_epsilon_depth_pair.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1667, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_epsilon_depth_pair.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1667, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_7 = (__Pyx_PyDict_ContainsTF(__pyx_t_1, __pyx_v_result, Py_NE)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(1, 1667, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_8 = (__pyx_t_7 != 0);
       if (__pyx_t_8) {
 
         /* "libmata.pyx":1668
@@ -27503,15 +27500,15 @@
  *                 if epsilon_depth_pair.first not in result:
  *                     result[epsilon_depth_pair.first] = []             # <<<<<<<<<<<<<<
  * 
  *                 result[epsilon_depth_pair.first].append(Trans(trans.src, trans.symb, trans.tgt))
  */
         __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1668, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
-        __pyx_t_9 = __Pyx_PyInt_From_unsigned_int(__pyx_v_epsilon_depth_pair.first); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 1668, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyInt_FromSize_t(__pyx_v_epsilon_depth_pair.first); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 1668, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         if (unlikely(PyDict_SetItem(__pyx_v_result, __pyx_t_9, __pyx_t_1) < 0)) __PYX_ERR(1, 1668, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
         /* "libmata.pyx":1667
  *         for epsilon_depth_pair in c_epsilon_transitions:
@@ -27525,15 +27522,15 @@
       /* "libmata.pyx":1670
  *                     result[epsilon_depth_pair.first] = []
  * 
  *                 result[epsilon_depth_pair.first].append(Trans(trans.src, trans.symb, trans.tgt))             # <<<<<<<<<<<<<<
  * 
  *         return result
  */
-      __pyx_t_1 = __Pyx_PyInt_From_unsigned_int(__pyx_v_epsilon_depth_pair.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1670, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_epsilon_depth_pair.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1670, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_9 = __Pyx_PyDict_GetItem(__pyx_v_result, __pyx_t_1); if (unlikely(!__pyx_t_9)) __PYX_ERR(1, 1670, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __pyx_t_1 = __Pyx_PyInt_FromSize_t(__pyx_v_trans.src); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1670, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __pyx_t_10 = __Pyx_PyInt_FromSize_t(__pyx_v_trans.symb); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 1670, __pyx_L1_error)
@@ -27564,15 +27561,15 @@
  *             for trans in epsilon_depth_pair.second:             # <<<<<<<<<<<<<<
  *                 if epsilon_depth_pair.first not in result:
  *                     result[epsilon_depth_pair.first] = []
  */
     }
 
     /* "libmata.pyx":1665
- *         cdef umap[unsigned, vector[CTrans]] c_epsilon_transitions = self.thisptr.get_epsilon_depths()
+ *         cdef umap[size_t, vector[CTrans]] c_epsilon_transitions = self.thisptr.get_epsilon_depths()
  *         result = {}
  *         for epsilon_depth_pair in c_epsilon_transitions:             # <<<<<<<<<<<<<<
  *             for trans in epsilon_depth_pair.second:
  *                 if epsilon_depth_pair.first not in result:
  */
   }
 
@@ -43519,52 +43516,14 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_int(unsigned int value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const unsigned int neg_one = (unsigned int) -1, const_zero = (unsigned int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(unsigned int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(unsigned int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(unsigned int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(unsigned int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(unsigned int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(unsigned int),
-                                     little, !is_unsigned);
-    }
-}
-
 /* PrintOne */
 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION < 3
 static int __Pyx_PrintOne(PyObject* f, PyObject *o) {
     if (!f) {
         if (!(f = __Pyx_GetStdout()))
             return -1;
     }
```

### Comparing `libmata-0.68.0/libmata.pxd` & `libmata-0.69.0/libmata.pxd`

 * *Files 0% similar despite different names*

```diff
@@ -329,15 +329,15 @@
     cdef cset[vector[Symbol]] get_shortest_words(CNfa&)
 
 
 cdef extern from "mata/nfa-strings.hh" namespace "Mata::Strings::SegNfa":
     cdef cppclass CSegmentation "Mata::Strings::SegNfa::Segmentation":
         CSegmentation(CNfa&, cset[Symbol]) except +
 
-        ctypedef unsigned EpsilonDepth
+        ctypedef size_t EpsilonDepth
         ctypedef umap[EpsilonDepth, TransitionSequence] EpsilonDepthTransitions
 
         EpsilonDepthTransitions get_epsilon_depths()
         AutSequence get_segments()
 
     ctypedef vector[vector[shared_ptr[CNfa]]] NoodleSequence
```

### Comparing `libmata-0.68.0/libmata.pyx` & `libmata-0.69.0/libmata.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1656,15 +1656,15 @@
         del self.thisptr
 
     def get_epsilon_depths(self):
         """Get segmentation depths for ε-transitions.
 
         :return: Map of depths to lists of ε-transitions.
         """
-        cdef umap[unsigned, vector[CTrans]] c_epsilon_transitions = self.thisptr.get_epsilon_depths()
+        cdef umap[size_t, vector[CTrans]] c_epsilon_transitions = self.thisptr.get_epsilon_depths()
         result = {}
         for epsilon_depth_pair in c_epsilon_transitions:
             for trans in epsilon_depth_pair.second:
                 if epsilon_depth_pair.first not in result:
                     result[epsilon_depth_pair.first] = []
 
                 result[epsilon_depth_pair.first].append(Trans(trans.src, trans.symb, trans.tgt))
```

### Comparing `libmata-0.68.0/mata/3rdparty/args.hxx` & `libmata-0.69.0/mata/3rdparty/args.hxx`

 * *Files 0% similar despite different names*

```diff
@@ -1582,15 +1582,15 @@
     template <
         typename T,
         typename Reader = ValueReader<T>>
     class ValueFlag : public ValueFlagBase
     {
         private:
             T value;
-            Reader reader;
+            Reader reader{};
 
         public:
 
             ValueFlag(Group &group_, const std::string &name_, const std::string &help_, Matcher &&matcher_, const T &defaultValue_ = T(), const bool extraError_ = false): ValueFlagBase(name_, help_, std::move(matcher_), extraError_), value(defaultValue_)
             {
                 group_.Add(*this);
             }
```

### Comparing `libmata-0.68.0/mata/3rdparty/catch.hpp` & `libmata-0.69.0/mata/3rdparty/catch.hpp`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/catch.hpp.1.9.3` & `libmata-0.69.0/mata/3rdparty/catch.hpp.1.9.3`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/catch.hpp.2.0.1` & `libmata-0.69.0/mata/3rdparty/catch.hpp.2.0.1`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/catch.hpp.2.13.9` & `libmata-0.69.0/mata/3rdparty/catch.hpp.2.13.9`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/Doxyfile.in` & `libmata-0.69.0/mata/3rdparty/cudd/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/LICENSE` & `libmata-0.69.0/mata/3rdparty/cudd/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/README` & `libmata-0.69.0/mata/3rdparty/cudd/README`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/RELEASE.NOTES` & `libmata-0.69.0/mata/3rdparty/cudd/RELEASE.NOTES`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc` & `libmata-0.69.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc`

 * *Files 0% similar despite different names*

```diff
@@ -181,14 +181,29 @@
 	    cout << "Copy DD constructor for node " << hex << node << dec <<
 		" ref = " << Cudd_Regular(node)->ref << "\n";
 	}
     }
 
 } // DD::DD
 
+DD& DD::operator=(const DD& other) {
+    if (this != &other) {
+        this->p = other.p;
+        if (this->node) { Cudd_Deref(this->node); }
+        this->node = other.node;
+        if (this->node) {
+            Cudd_Ref(this->node);
+            if (this->p->verbose) {
+                cout << "Copy DD assignment for node " << hex << node << dec <<
+                     " ref = " << Cudd_Regular(node)->ref << "\n";
+            }
+        }
+    }
+    return *this;
+} // DD::operator=
 
 DD::~DD() {}
 
 
 inline DdManager *
 DD::checkSameManager(
   const DD &other) const
```

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in` & `libmata-0.69.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cplusplus/testmulti.cc` & `libmata-0.69.0/mata/3rdparty/cudd/cplusplus/testmulti.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cplusplus/testobj.cc` & `libmata-0.69.0/mata/3rdparty/cudd/cplusplus/testobj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAPI.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAPI.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAddApply.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAddApply.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAddFind.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAddFind.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAddInv.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAddInv.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAddIte.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddAnneal.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddAnneal.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddApa.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddApa.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddApprox.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddApprox.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddBddIte.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddBddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddBridge.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddBridge.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddCache.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddCheck.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddCheck.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddClip.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddClip.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddCof.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddCompose.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddCompose.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddDecomp.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddDecomp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddEssent.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddEssent.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddExact.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddExact.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddExport.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddExport.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddGenCof.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddGenCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddGenetic.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddGenetic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddGroup.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddHarwell.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddHarwell.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddInit.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddInit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddInt.h` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddInteract.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddInteract.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddLCache.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddLCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddLinear.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddLinear.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddLiteral.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddLiteral.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddMatMult.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddMatMult.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddPriority.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddPriority.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddRead.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddRead.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddRef.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddRef.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddReorder.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddReorder.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddSat.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddSat.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddSign.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddSign.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddSolve.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddSolve.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddSplit.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddSplit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddTable.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddTable.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddUtil.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddWindow.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddWindow.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddCount.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddCount.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddLin.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddLin.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddPort.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddPort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddReord.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddReord.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/test_cudd.test.in` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/test_cudd.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/testcudd.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/testcudd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd/testextra.c` & `libmata-0.69.0/mata/3rdparty/cudd/cudd/testextra.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/cudd_config.h.in` & `libmata-0.69.0/mata/3rdparty/cudd/cudd_config.h.in`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/README.dddmp` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/README.dddmp`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/README.testdddmp` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/README.testdddmp`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmp.h` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmp.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpInt.h` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/1.add` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/1.add`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/1.bdd` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/1.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/2.bdd` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/2.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/3.bdd` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/3.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4.bdd` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4.cnf` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4.cnf`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4.max1` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4.max1`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4.max2` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4.max2`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/dddmp/testdddmp.c` & `libmata-0.69.0/mata/3rdparty/cudd/dddmp/testdddmp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/doc/cudd.tex.in` & `libmata-0.69.0/mata/3rdparty/cudd/doc/cudd.tex.in`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/doc/phase.pdf` & `libmata-0.69.0/mata/3rdparty/cudd/doc/phase.pdf`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/epd/epd.c` & `libmata-0.69.0/mata/3rdparty/cudd/epd/epd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/epd/epd.h` & `libmata-0.69.0/mata/3rdparty/cudd/epd/epd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/epd/epdInt.h` & `libmata-0.69.0/mata/3rdparty/cudd/epd/epdInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/groups.dox` & `libmata-0.69.0/mata/3rdparty/cudd/groups.dox`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h` & `libmata-0.69.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddObj.hh`

 * *Files 0% similar despite different names*

```diff
@@ -201,17 +201,17 @@
       int threshold = 0,
       bool safe = false,
       double quality = 1.0) const;
     BDD RemapUnderApprox(int numVars, int threshold = 0, double quality = 1.0)
 	const;
     BDD RemapOverApprox(int numVars, int threshold = 0, double quality = 1.0)
 	const;
-    BDD BiasedUnderApprox(const BDD& bias, int numVars, int threshold = 0, 
+    BDD BiasedUnderApprox(const BDD& bias, int numVars, int threshold = 0,
                           double quality1 = 1.0, double quality0 = 1.0) const;
-    BDD BiasedOverApprox(const BDD& bias, int numVars, int threshold = 0, 
+    BDD BiasedOverApprox(const BDD& bias, int numVars, int threshold = 0,
                          double quality1 = 1.0, double quality0 = 1.0) const;
     BDD ExistAbstract(const BDD& cube, unsigned int limit = 0) const;
     BDD XorExistAbstract(const BDD& g, const BDD& cube) const;
     BDD UnivAbstract(const BDD& cube) const;
     BDD BooleanDiff(int x) const;
     bool VarIsDependent(const BDD& var) const;
     double Correlation(const BDD& g) const;
@@ -698,51 +698,51 @@
     void Srandom(int32_t seed) const;
     void zddPrintSubtable() const;
     void zddReduceHeap(Cudd_ReorderingType heuristic = CUDD_REORDER_SIFT,
                        int minsize = 0) const;
     void zddShuffleHeap(int * permutation) const;
     void zddSymmProfile(int lower, int upper) const;
     void DumpDot(
-      const std::vector<BDD>& nodes, 
-      char const * const * inames = 0, 
-      char const * const * onames = 0, 
+      const std::vector<BDD>& nodes,
+      char const * const * inames = 0,
+      char const * const * onames = 0,
       FILE * fp = stdout) const;
     void DumpDaVinci(
-      const std::vector<BDD>& nodes, 
+      const std::vector<BDD>& nodes,
       char const * const * inames = 0,
       char const * const * onames = 0,
       FILE * fp = stdout) const;
     void DumpBlif(
-      const std::vector<BDD>& nodes, 
+      const std::vector<BDD>& nodes,
       char const * const * inames = 0,
       char const * const * onames = 0,
       char * mname = 0,
       FILE * fp = stdout,
       int mv = 0) const;
     void DumpDDcal(
-      const std::vector<BDD>& nodes, 
-      char const * const * inames = 0, 
-      char const * const * onames = 0, 
+      const std::vector<BDD>& nodes,
+      char const * const * inames = 0,
+      char const * const * onames = 0,
       FILE * fp = stdout) const;
     void DumpFactoredForm(
-      const std::vector<BDD>& nodes, 
+      const std::vector<BDD>& nodes,
       char const * const * inames = 0,
       char const * const * onames = 0,
       FILE * fp = stdout) const;
     BDD VectorSupport(const std::vector<BDD>& roots) const;
-    std::vector<unsigned int> 
+    std::vector<unsigned int>
     SupportIndices(const std::vector<BDD>& roots) const;
-    std::vector<unsigned int> 
+    std::vector<unsigned int>
     SupportIndices(const std::vector<ADD>& roots) const;
     int nodeCount(const std::vector<BDD>& roots) const;
     int VectorSupportSize(const std::vector<BDD>& roots) const;
     void DumpDot(
       const std::vector<ADD>& nodes,
-      char const * const * inames = 0, 
-      char const * const * onames = 0, 
+      char const * const * inames = 0,
+      char const * const * onames = 0,
       FILE * fp = stdout) const;
     void DumpDaVinci(
       const std::vector<ADD>& nodes,
       char const * const * inames = 0,
       char const * const * onames = 0,
       FILE * fp = stdout) const;
     BDD VectorSupport(const std::vector<ADD>& roots) const;
```

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/mtr/mtr.h` & `libmata-0.69.0/mata/3rdparty/cudd/mtr/mtr.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/mtr/mtrBasic.c` & `libmata-0.69.0/mata/3rdparty/cudd/mtr/mtrBasic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/mtr/mtrGroup.c` & `libmata-0.69.0/mata/3rdparty/cudd/mtr/mtrGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/mtr/mtrInt.h` & `libmata-0.69.0/mata/3rdparty/cudd/mtr/mtrInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/mtr/test_mtr.test.in` & `libmata-0.69.0/mata/3rdparty/cudd/mtr/test_mtr.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/mtr/testmtr.c` & `libmata-0.69.0/mata/3rdparty/cudd/mtr/testmtr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/st/st.c` & `libmata-0.69.0/mata/3rdparty/cudd/st/st.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/st/st.h` & `libmata-0.69.0/mata/3rdparty/cudd/st/st.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/st/testst.c` & `libmata-0.69.0/mata/3rdparty/cudd/st/testst.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/util/cpu_stats.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cpu_stats.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/util/cpu_time.c` & `libmata-0.69.0/mata/3rdparty/cudd/util/cpu_time.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/util/cstringstream.c` & `libmata-0.69.0/mata/3rdparty/cudd/util/cstringstream.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/util/cstringstream.h` & `libmata-0.69.0/mata/3rdparty/cudd/util/cstringstream.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/util/datalimit.c` & `libmata-0.69.0/mata/3rdparty/cudd/util/datalimit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/util/pathsearch.c` & `libmata-0.69.0/mata/3rdparty/cudd/util/pathsearch.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/util/pipefork.c` & `libmata-0.69.0/mata/3rdparty/cudd/util/pipefork.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/util/prtime.c` & `libmata-0.69.0/mata/3rdparty/cudd/util/prtime.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/util/safe_mem.c` & `libmata-0.69.0/mata/3rdparty/cudd/util/safe_mem.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/util/strsav.c` & `libmata-0.69.0/mata/3rdparty/cudd/util/strsav.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/util/texpand.c` & `libmata-0.69.0/mata/3rdparty/cudd/util/texpand.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/util/ucbqsort.c` & `libmata-0.69.0/mata/3rdparty/cudd/util/ucbqsort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd/util/util.h` & `libmata-0.69.0/mata/3rdparty/cudd/util/util.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/bnet.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/bnet.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/bnet.h` & `libmata-0.69.0/mata/3rdparty/cudd-min/bnet.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/chkMterm.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/chkMterm.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/config.h` & `libmata-0.69.0/mata/3rdparty/cudd-min/config.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cpu_stats.c` & `libmata-0.69.0/mata/3rdparty/cudd/util/cpu_stats.c`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,14 @@
   LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
   ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
   POSSIBILITY OF SUCH DAMAGE.
   @endparblock
 
 */
 
-#define _BSD_SOURCE
 #include "util.h"
 
 #if HAVE_SYS_TIME_H == 1
 #include <sys/time.h>
 #endif
 #if HAVE_SYS_RESOURCE_H == 1
 #include <sys/resource.h>
```

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cpu_time.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cpu_time.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cstringstream.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cstringstream.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cstringstream.h` & `libmata-0.69.0/mata/3rdparty/cudd-min/cstringstream.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cudd.h` & `libmata-0.69.0/mata/3rdparty/cudd-min/cudd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddAPI.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddAPI.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddAddAbs.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddAddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddAddApply.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddAddApply.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddAddFind.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddAddFind.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddAddInv.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddAddInv.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddAddIte.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddAddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddAddNeg.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddAddNeg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddAddWalsh.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddAddWalsh.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddAndAbs.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddAndAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddAnneal.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddAnneal.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddApa.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddApa.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddApprox.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddApprox.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddBddAbs.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddBddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddBddCorr.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddBddCorr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddBddIte.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddBddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddBridge.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddBridge.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddCache.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddCheck.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddCheck.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddClip.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddClip.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddCof.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddCompose.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddCompose.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddDecomp.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddDecomp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddEssent.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddEssent.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddExact.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddExact.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddExport.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddExport.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddGenCof.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddGenCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddGenetic.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddGenetic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddGroup.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddHarwell.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddHarwell.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddInit.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddInit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddInt.h` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddInteract.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddInteract.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddLCache.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddLCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddLevelQ.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddLevelQ.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddLinear.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddLinear.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddLiteral.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddLiteral.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddMatMult.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddMatMult.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddObj.cc` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddObj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddObj.hh` & `libmata-0.69.0/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh`

 * *Files 0% similar despite different names*

```diff
@@ -754,7 +754,8 @@
       FILE * fp = stdout) const;
     std::string OrderString(void) const;
 
 }; // Cudd
 
 
 #endif
+
```

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddPriority.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddPriority.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddRead.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddRead.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddRef.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddRef.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddReorder.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddReorder.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddSat.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddSat.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddSign.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddSign.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddSolve.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddSolve.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddSplit.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddSplit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddSubsetHB.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddSubsetHB.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddSubsetSP.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddSubsetSP.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddSymmetry.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddSymmetry.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddTable.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddTable.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddUtil.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddWindow.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddWindow.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddCount.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddCount.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddFuncs.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddFuncs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddGroup.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddIsop.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddIsop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddLin.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddLin.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddMisc.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddPort.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddPort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddReord.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddReord.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddSetop.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddSetop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddSymm.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddSymm.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/cuddZddUtil.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/cuddZddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/datalimit.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/datalimit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/dddmp.h` & `libmata-0.69.0/mata/3rdparty/cudd-min/dddmp.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/dddmpBinary.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/dddmpBinary.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/dddmpConvert.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/dddmpConvert.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/dddmpDbg.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/dddmpDbg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/dddmpInt.h` & `libmata-0.69.0/mata/3rdparty/cudd-min/dddmpInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/dddmpLoad.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/dddmpLoad.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/dddmpLoadCnf.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/dddmpLoadCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/dddmpNodeAdd.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/dddmpNodeAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/dddmpNodeBdd.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/dddmpNodeBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/dddmpNodeCnf.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/dddmpNodeCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/dddmpStoreAdd.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/dddmpStoreAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/dddmpStoreBdd.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/dddmpStoreBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/dddmpStoreCnf.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/dddmpStoreCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/dddmpStoreMisc.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/dddmpStoreMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/dddmpUtil.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/dddmpUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/epd.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/epd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/epd.h` & `libmata-0.69.0/mata/3rdparty/cudd-min/epd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/epdInt.h` & `libmata-0.69.0/mata/3rdparty/cudd-min/epdInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h` & `libmata-0.69.0/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh` & `libmata-0.69.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh`

 * *Files 0% similar despite different names*

```diff
@@ -89,14 +89,16 @@
     inline void checkReturnValue(int result, int expected = 1)
 	const;
     DD();
     DD(Capsule *cap, DdNode *ddNode);
     DD(Cudd const & manager, DdNode *ddNode);
     DD(const DD &from);
     ~DD();
+
+    DD& operator=(const DD& other);
 public:
     // This operator should be declared explicit, but there are still too many
     // compilers out there that do not support this C++11 feature.
     operator bool() const { return node; }
     DdManager * manager() const;
     DdNode * getNode() const;
     DdNode * getRegularNode() const;
@@ -201,17 +203,17 @@
       int threshold = 0,
       bool safe = false,
       double quality = 1.0) const;
     BDD RemapUnderApprox(int numVars, int threshold = 0, double quality = 1.0)
 	const;
     BDD RemapOverApprox(int numVars, int threshold = 0, double quality = 1.0)
 	const;
-    BDD BiasedUnderApprox(const BDD& bias, int numVars, int threshold = 0,
+    BDD BiasedUnderApprox(const BDD& bias, int numVars, int threshold = 0, 
                           double quality1 = 1.0, double quality0 = 1.0) const;
-    BDD BiasedOverApprox(const BDD& bias, int numVars, int threshold = 0,
+    BDD BiasedOverApprox(const BDD& bias, int numVars, int threshold = 0, 
                          double quality1 = 1.0, double quality0 = 1.0) const;
     BDD ExistAbstract(const BDD& cube, unsigned int limit = 0) const;
     BDD XorExistAbstract(const BDD& g, const BDD& cube) const;
     BDD UnivAbstract(const BDD& cube) const;
     BDD BooleanDiff(int x) const;
     bool VarIsDependent(const BDD& var) const;
     double Correlation(const BDD& g) const;
@@ -698,51 +700,51 @@
     void Srandom(int32_t seed) const;
     void zddPrintSubtable() const;
     void zddReduceHeap(Cudd_ReorderingType heuristic = CUDD_REORDER_SIFT,
                        int minsize = 0) const;
     void zddShuffleHeap(int * permutation) const;
     void zddSymmProfile(int lower, int upper) const;
     void DumpDot(
-      const std::vector<BDD>& nodes,
-      char const * const * inames = 0,
-      char const * const * onames = 0,
+      const std::vector<BDD>& nodes, 
+      char const * const * inames = 0, 
+      char const * const * onames = 0, 
       FILE * fp = stdout) const;
     void DumpDaVinci(
-      const std::vector<BDD>& nodes,
+      const std::vector<BDD>& nodes, 
       char const * const * inames = 0,
       char const * const * onames = 0,
       FILE * fp = stdout) const;
     void DumpBlif(
-      const std::vector<BDD>& nodes,
+      const std::vector<BDD>& nodes, 
       char const * const * inames = 0,
       char const * const * onames = 0,
       char * mname = 0,
       FILE * fp = stdout,
       int mv = 0) const;
     void DumpDDcal(
-      const std::vector<BDD>& nodes,
-      char const * const * inames = 0,
-      char const * const * onames = 0,
+      const std::vector<BDD>& nodes, 
+      char const * const * inames = 0, 
+      char const * const * onames = 0, 
       FILE * fp = stdout) const;
     void DumpFactoredForm(
-      const std::vector<BDD>& nodes,
+      const std::vector<BDD>& nodes, 
       char const * const * inames = 0,
       char const * const * onames = 0,
       FILE * fp = stdout) const;
     BDD VectorSupport(const std::vector<BDD>& roots) const;
-    std::vector<unsigned int>
+    std::vector<unsigned int> 
     SupportIndices(const std::vector<BDD>& roots) const;
-    std::vector<unsigned int>
+    std::vector<unsigned int> 
     SupportIndices(const std::vector<ADD>& roots) const;
     int nodeCount(const std::vector<BDD>& roots) const;
     int VectorSupportSize(const std::vector<BDD>& roots) const;
     void DumpDot(
       const std::vector<ADD>& nodes,
-      char const * const * inames = 0,
-      char const * const * onames = 0,
+      char const * const * inames = 0, 
+      char const * const * onames = 0, 
       FILE * fp = stdout) const;
     void DumpDaVinci(
       const std::vector<ADD>& nodes,
       char const * const * inames = 0,
       char const * const * onames = 0,
       FILE * fp = stdout) const;
     BDD VectorSupport(const std::vector<ADD>& roots) const;
@@ -754,8 +756,7 @@
       FILE * fp = stdout) const;
     std::string OrderString(void) const;
 
 }; // Cudd
 
 
 #endif
-
```

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/main.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/main.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/mtr.h` & `libmata-0.69.0/mata/3rdparty/cudd-min/mtr.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/mtrBasic.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/mtrBasic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/mtrGroup.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/mtrGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/mtrInt.h` & `libmata-0.69.0/mata/3rdparty/cudd-min/mtrInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/ntr.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/ntr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/ntr.h` & `libmata-0.69.0/mata/3rdparty/cudd-min/ntr.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/ntrBddTest.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/ntrBddTest.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/ntrHeap.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/ntrHeap.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/ntrMflow.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/ntrMflow.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/ntrShort.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/ntrShort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/ntrZddTest.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/ntrZddTest.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/pathsearch.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/pathsearch.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/pipefork.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/pipefork.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/prtime.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/prtime.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/safe_mem.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/safe_mem.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/st.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/st.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/st.h` & `libmata-0.69.0/mata/3rdparty/cudd-min/st.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/strsav.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/strsav.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/testcudd.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/testcudd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/testdddmp.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/testdddmp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/testextra.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/testextra.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/testmtr.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/testmtr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/testmulti.cc` & `libmata-0.69.0/mata/3rdparty/cudd-min/testmulti.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/testobj.cc` & `libmata-0.69.0/mata/3rdparty/cudd-min/testobj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/testst.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/testst.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/texpand.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/texpand.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/ucbqsort.c` & `libmata-0.69.0/mata/3rdparty/cudd-min/ucbqsort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/cudd-min/util.h` & `libmata-0.69.0/mata/3rdparty/cudd-min/util.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/CONTRIBUTORS` & `libmata-0.69.0/mata/3rdparty/re2/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/LICENSE` & `libmata-0.69.0/mata/3rdparty/re2/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/bitmap256.h` & `libmata-0.69.0/mata/3rdparty/re2/re2/bitmap256.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/compile.cc` & `libmata-0.69.0/mata/3rdparty/re2/re2/compile.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/parse.cc` & `libmata-0.69.0/mata/3rdparty/re2/re2/parse.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/perl_groups.cc` & `libmata-0.69.0/mata/3rdparty/re2/re2/perl_groups.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/pod_array.h` & `libmata-0.69.0/mata/3rdparty/re2/re2/pod_array.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/prog.cc` & `libmata-0.69.0/mata/3rdparty/re2/re2/prog.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/prog.h` & `libmata-0.69.0/mata/3rdparty/re2/re2/prog.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/re2.cc` & `libmata-0.69.0/mata/3rdparty/re2/re2/re2.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/re2.h` & `libmata-0.69.0/mata/3rdparty/re2/re2/re2.h`

 * *Files 1% similar despite different names*

```diff
@@ -228,14 +228,15 @@
 // pre-compiled regular expression.  An "RE2" object is safe for
 // concurrent use by multiple threads.
 class RE2 {
  public:
   // We convert user-passed pointers into special Arg objects
   class Options;
 
+  RE2() = default;
   ~RE2();
 
   // If RE2 could not be created properly, returns an error string.
   // Else returns the empty string.
   const std::string& error() const { return *error_; }
 
   // Returns the underlying Regexp; not for general use.
@@ -368,27 +369,27 @@
     bool perl_classes_;
     bool word_boundary_;
     bool one_line_;
   };
  private:
 
   std::string pattern_;         // string regular expression
-  re2::Regexp* entire_regexp_;  // parsed regular expression
-  const std::string* error_;    // error indicator (or points to empty string)
+  re2::Regexp* entire_regexp_{};  // parsed regular expression
+  const std::string* error_{};    // error indicator (or points to empty string)
   std::string error_arg_;       // fragment of regexp showing error
   std::string prefix_;          // required prefix (before suffix_regexp_)
-  re2::Regexp* suffix_regexp_;  // parsed regular expression, prefix_ removed
-  re2::Prog* prog_;             // compiled program for regexp
+  re2::Regexp* suffix_regexp_{};  // parsed regular expression, prefix_ removed
+  re2::Prog* prog_{};             // compiled program for regexp
 
   // Reverse Prog for DFA execution only
-  mutable re2::Prog* rprog_;
+  mutable re2::Prog* rprog_{};
   // Map from capture names to indices
-  mutable const std::map<std::string, int>* named_groups_;
+  mutable const std::map<std::string, int>* named_groups_{};
   // Map from capture indices to names
-  mutable const std::map<int, std::string>* group_names_;
+  mutable const std::map<int, std::string>* group_names_{};
 
   RE2(const RE2&) = delete;
   RE2& operator=(const RE2&) = delete;
 };
 
 }  // namespace re2
```

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/regexp.cc` & `libmata-0.69.0/mata/3rdparty/re2/re2/regexp.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/regexp.h` & `libmata-0.69.0/mata/3rdparty/re2/re2/regexp.h`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
 
   // Returns text describing error, e.g.:
   //   "Bad character class: [z-a]"
   std::string Text() const;
 
  private:
   RegexpStatusCode code_;  // Kind of error
-  StringPiece error_arg_;  // Piece of regexp containing syntax error.
+  StringPiece error_arg_{};  // Piece of regexp containing syntax error.
   std::string* tmp_;       // Temporary storage, possibly where error_arg_ is.
 
   RegexpStatus(const RegexpStatus&) = delete;
   RegexpStatus& operator=(const RegexpStatus&) = delete;
 };
 
 // Compiled form; see prog.h
```

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/simplify.cc` & `libmata-0.69.0/mata/3rdparty/re2/re2/simplify.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/sparse_array.h` & `libmata-0.69.0/mata/3rdparty/re2/re2/sparse_array.h`

 * *Files 2% similar despite different names*

```diff
@@ -302,15 +302,15 @@
 bool SparseArray<Value>::has_index(int i) const {
   assert(i >= 0);
   assert(i < max_size());
   if (static_cast<uint32_t>(i) >= static_cast<uint32_t>(max_size())) {
     return false;
   }
   // Unsigned comparison avoids checking sparse_[i] < 0.
-  return (uint32_t)sparse_[i] < (uint32_t)size_ &&
+  return static_cast<uint32_t>(sparse_[i]) < static_cast<uint32_t>(size_) &&
          dense_[sparse_[i]].index_ == i;
 }
 
 template<typename Value>
 void SparseArray<Value>::create_index(int i) {
   assert(!has_index(i));
   assert(size_ < max_size());
```

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/sparse_set.h` & `libmata-0.69.0/mata/3rdparty/re2/re2/sparse_set.h`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,15 @@
 bool SparseSetT<Value>::contains(int i) const {
   assert(i >= 0);
   assert(i < max_size());
   if (static_cast<uint32_t>(i) >= static_cast<uint32_t>(max_size())) {
     return false;
   }
   // Unsigned comparison avoids checking sparse_[i] < 0.
-  return (uint32_t)sparse_[i] < (uint32_t)size_ &&
+  return static_cast<uint32_t>(sparse_[i]) < static_cast<uint32_t>(size_) &&
          dense_[sparse_[i]] == i;
 }
 
 template<typename Value>
 void SparseSetT<Value>::create_index(int i) {
   assert(!contains(i));
   assert(size_ < max_size());
```

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/stringpiece.cc` & `libmata-0.69.0/mata/3rdparty/re2/re2/stringpiece.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/stringpiece.h` & `libmata-0.69.0/mata/3rdparty/re2/re2/stringpiece.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/tostring.cc` & `libmata-0.69.0/mata/3rdparty/re2/re2/tostring.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/unicode_casefold.cc` & `libmata-0.69.0/mata/3rdparty/re2/re2/unicode_casefold.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/unicode_casefold.h` & `libmata-0.69.0/mata/3rdparty/re2/re2/unicode_casefold.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/unicode_groups.cc` & `libmata-0.69.0/mata/3rdparty/re2/re2/unicode_groups.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/unicode_groups.h` & `libmata-0.69.0/mata/3rdparty/re2/re2/unicode_groups.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/re2/walker-inl.h` & `libmata-0.69.0/mata/3rdparty/re2/re2/walker-inl.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/util/logging.h` & `libmata-0.69.0/mata/3rdparty/re2/util/logging.h`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
       Flush();
     }
   }
   std::ostream& stream() { return str_; }
 
  private:
   bool flushed_;
-  std::ostringstream str_;
+  std::ostringstream str_{};
 
   LogMessage(const LogMessage&) = delete;
   LogMessage& operator=(const LogMessage&) = delete;
 };
 
 // Silence "destructor never returns" warning for ~LogMessageFatal().
 // Since this is a header file, push and then pop to limit the scope.
```

### Comparing `libmata-0.68.0/mata/3rdparty/re2/util/mutex.h` & `libmata-0.69.0/mata/3rdparty/re2/util/mutex.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/util/rune.cc` & `libmata-0.69.0/mata/3rdparty/re2/util/rune.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/util/strutil.cc` & `libmata-0.69.0/mata/3rdparty/re2/util/strutil.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/util/utf.h` & `libmata-0.69.0/mata/3rdparty/re2/util/utf.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/re2/util/util.h` & `libmata-0.69.0/mata/3rdparty/re2/util/util.h`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh` & `libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 #include <mata/simlib/util/smart_set.hh>
 
 
 namespace Simlib { class ExplicitLTS; }
 
 class Simlib::ExplicitLTS {
 
-	size_t states_;
+	size_t states_{};
 	size_t transitions_;
 	std::vector<
 		std::pair<
 			std::vector<std::vector<size_t>>,
 			std::vector<std::vector<size_t>>
 		>
 	> data_;
```

### Comparing `libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh` & `libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh` & `libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh` & `libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh` & `libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh` & `libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh` & `libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh` & `libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh` & `libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh`

 * *Files 12% similar despite different names*

```diff
@@ -47,25 +47,29 @@
 			next(nullptr),
 			key(key),
 			count(count)
 		{ }
 	};
 
 	GCC_DIAG_OFF(effc++)
-	class Iterator : public std::iterator<std::input_iterator_tag, Key>
-	{
+	class Iterator {
 	GCC_DIAG_ON(effc++)
 
 	private:
 
 		const Element* element_;
 
 	public:
+        using iterator_category = std::input_iterator_tag;
+        using value_type = int;
+        using difference_type = int;
+        using pointer = int*;
+        using reference = int&;
 
-		explicit Iterator(const Element* element) :
+        explicit Iterator(const Element* element) :
 			element_(element)
 		{ }
 
 		Iterator& operator++()
 		{
 			assert(nullptr != element_);
```

### Comparing `libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh` & `libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh`

 * *Files 4% similar despite different names*

```diff
@@ -124,16 +124,21 @@
 		return true;
 
 	}
 
 public:
 
 	GCC_DIAG_OFF(effc++)
-	struct IteratorBase : public std::iterator<std::input_iterator_tag, size_t> {
+	struct IteratorBase {
 	GCC_DIAG_ON(effc++)
+        using iterator_category = std::input_iterator_tag;
+        using value_type = int;
+        using difference_type = int;
+        using pointer = int*;
+        using reference = int&;
 
 		Element* el_;
 
 		explicit IteratorBase(Element* el) : el_(el) {}
 		~IteratorBase() = default;
 
 		bool operator==(const IteratorBase& rhs) const { return this->el_ == rhs.el_; }
```

### Comparing `libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh` & `libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh` & `libmata-0.69.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc` & `libmata-0.69.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,19 @@
 			}
 
 			states->block_ = this;
 			states = states->next_;
 		} while (states != this->states_);
 	}
 
+    Block(Block&) = default;
+
+    Block& operator=(const Block&) = delete;
+    Block& operator=(Block&&) = delete;
+
 	void move_to_tmp(StateListElem* elem)
 	{
 		this->tmp_.push_back(elem);
 	}
 
 	static bool check_list(StateListElem* elem, size_t size)
 	{
```

### Comparing `libmata-0.68.0/mata/LICENSE` & `libmata-0.69.0/mata/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/README.md` & `libmata-0.69.0/mata/README.md`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/include/mata/afa.hh` & `libmata-0.69.0/mata/include/mata/afa.hh`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 #include <algorithm>
 #include <cassert>
 #include <cstdint>
 #include <set>
 #include <unordered_map>
 #include <unordered_set>
+#include <utility>
 #include <vector>
 #include <memory>
 
 #include "mata/alphabet.hh"
 #include "mata/nfa.hh"
 #include "mata/parser.hh"
 #include "mata/util.hh"
@@ -80,16 +81,16 @@
 struct Trans
 {
     State src; // source state
     Symbol symb; // transition symbol
     Nodes dst; // a vector of vectors of states
 
     Trans() : src(), symb(), dst() { }
-    Trans(State src, Symbol symb, Node dst) : src(src), symb(symb), dst(Nodes(dst)) { }
-    Trans(State src, Symbol symb, Nodes dst) : src(src), symb(symb), dst(dst) { }
+    Trans(const State src, const Symbol symb, const Node& dst) : src(src), symb(symb), dst(Nodes{ dst }) {}
+    Trans(const State src, const Symbol symb, Nodes dst) : src(src), symb(symb), dst(std::move(dst)) {}
 
     bool operator==(const Trans& rhs) const
     { // {{{
         return src == rhs.src && symb == rhs.symb && dst == rhs.dst ;
     } // operator== }}}
     bool operator!=(const Trans& rhs) const { return !this->operator==(rhs); }
 
@@ -101,19 +102,19 @@
 /* A tuple (result_node, precondition). The node result_node is a predecessor
 * of a given node 'N' if the node 'precondition' is its subset. */
 struct InverseResults{
 
     Node result_node{};
     Node precondition{};
 
-    InverseResults() : result_node(), precondition() { }
-    InverseResults(State state, Node precondition) : result_node(Node(state)),
-    precondition(precondition) { }
-    InverseResults(Node result_node, Node precondition) : result_node(result_node),
-    precondition(precondition) { }
+    InverseResults() : result_node(), precondition() {}
+    InverseResults(State state, Node precondition)
+        : result_node(Node(state)), precondition(std::move(precondition)) {}
+    InverseResults(Node result_node, Node precondition)
+        : result_node(std::move(result_node)), precondition(std::move(precondition)) {}
 
     bool operator==(const InverseResults& rhs) const
     { // {{{
         return precondition == rhs.precondition && result_node == rhs.result_node;
     } // operator== }}}
 
     bool operator!=(const InverseResults& rhs) const
@@ -132,22 +133,22 @@
 /**
  * A tuple (state, symb, inverseResults). The structure inverseResults contains tuples (inverseResult,
  * precondition). If a node is a subset of 'precondition', the 'inverseResult' is a predecessor
  * of the given node which is accessible through the symbol 'symb'.
  * The state 'state' is always part of all 'preconditions' and it is a minimal element of them.
  */
 struct InverseTrans {
-    State state;
-    Symbol symb;
+    State state{};
+    Symbol symb{};
     std::vector<InverseResults> inverseResults{};
 
-    InverseTrans() : symb(), inverseResults() { }
-    InverseTrans(Symbol symb) : symb(symb), inverseResults(std::vector<InverseResults>()) { }
-    InverseTrans(Symbol symb, InverseResults inverseResults_) : symb(symb) { inverseResults.push_back(inverseResults_); }
-    InverseTrans(State state, Symbol symb, InverseResults inverseResults_)
+    InverseTrans() = default;
+    explicit InverseTrans(Symbol symb) : symb(symb), inverseResults(std::vector<InverseResults>()) { }
+    InverseTrans(Symbol symb, const InverseResults& inverseResults_) : symb(symb) { inverseResults.push_back(inverseResults_); }
+    InverseTrans(State state, Symbol symb, const InverseResults& inverseResults_)
         : state(state), symb(symb) { inverseResults.push_back(inverseResults_); }
 }; // struct InverseTrans
 
 using InverseTransRelation = std::vector<std::vector<InverseTrans>>;
 
 struct Afa;
 
@@ -193,15 +194,15 @@
     } // }}}
     bool has_initial(State state) const
     { // {{{
         return has_initial(Node({state}));
     } // }}}
     bool has_initial(Node node) const
     { // {{{
-        return StateClosedSet(upward_closed_set, 0, transitionrelation.size()-1, initialstates).contains(node);
+        return StateClosedSet(ClosedSetType::upward_closed_set, 0, transitionrelation.size()-1, initialstates).contains(node);
     } // }}}
     void add_final(State state) { this->finalstates.insert(state); }
     void add_final(const std::vector<State> vec)
     { // {{{
         for (const State& st : vec) { this->add_final(st); }
     } // }}}
     bool has_final(State state) const
@@ -230,60 +231,60 @@
     } // }}}
     void add_inverse_trans(State src, Symbol symb, Nodes dst)
     { // {{{
         this->add_inverse_trans({src, symb, dst});
     } // }}}
 
     std::vector<InverseResults> perform_inverse_trans(State src, Symbol symb) const;
-    std::vector<InverseResults> perform_inverse_trans(Node src, Symbol symb) const;
+    std::vector<InverseResults> perform_inverse_trans(const Node& src, Symbol symb) const;
 
     bool has_trans(const Trans& trans) const;
     bool has_trans(State src, Symbol symb, Node dst) const
     { // {{{
         return this->has_trans({src, symb, Nodes(dst)});
     } // }}}
     bool has_trans(State src, Symbol symb, Nodes dst) const
     { // {{{
         return this->has_trans({src, symb, dst});
     } // }}}
 
     std::vector<Trans> get_trans_from_state(State state) const;
     Trans get_trans_from_state(State state, Symbol symbol) const;
 
-    bool trans_empty() const {!transitionrelation.size();};// no transitions
+    bool trans_empty() const { return transitionrelation.empty(); }// no transitions
     size_t trans_size() const;/// number of transitions; has linear time complexity
 
 
     StateClosedSet post(State state, Symbol symb) const;
-    StateClosedSet post(Node node, Symbol symb) const;
-    StateClosedSet post(Nodes nodes, Symbol symb) const;
-    StateClosedSet post(StateClosedSet closed_set, Symbol symb) const;
-
-    StateClosedSet post(Node node) const;
-    StateClosedSet post(Nodes nodes) const;
-
-    StateClosedSet post(StateClosedSet closed_set) const;
-
-    StateClosedSet pre(Node node, Symbol symb) const;
-    StateClosedSet pre(State state, Symbol symb) const { return pre(Node(state), symb); };
-    StateClosedSet pre(Nodes nodes, Symbol symb) const;
-    StateClosedSet pre(StateClosedSet closed_set, Symbol symb) const;
+    StateClosedSet post(const Node& node, Symbol symb) const;
+    StateClosedSet post(const Nodes& nodes, Symbol symb) const;
+    StateClosedSet post(const StateClosedSet& closed_set, Symbol symb) const;
+
+    StateClosedSet post(const Node& node) const;
+    StateClosedSet post(const Nodes& nodes) const;
+
+    StateClosedSet post(const StateClosedSet& closed_set) const;
+
+    StateClosedSet pre(const Node& node, Symbol symb) const;
+    StateClosedSet pre(const State state, const Symbol symb) const { return pre(Node(state), symb); };
+    StateClosedSet pre(const Nodes& nodes, Symbol symb) const;
+    StateClosedSet pre(const StateClosedSet& closed_set, Symbol symb) const;
 
-    StateClosedSet pre(Node node) const;
-    StateClosedSet pre(Nodes nodes) const;
+    StateClosedSet pre(const Node& node) const;
+    StateClosedSet pre(const Nodes& nodes) const;
 
     StateClosedSet pre(StateClosedSet closed_set) const { return pre(closed_set.antichain()); };
 
     StateClosedSet get_initial_nodes() const;
 
     StateClosedSet get_non_initial_nodes() const {
-        return StateClosedSet{ upward_closed_set, 0, transitionrelation.size()-1, initialstates }.complement();
+        return StateClosedSet{ ClosedSetType::upward_closed_set, 0, transitionrelation.size()-1, initialstates }.complement();
     };
     StateClosedSet get_final_nodes() const {
-        return { downward_closed_set, 0, transitionrelation.size()-1, finalstates };
+        return { ClosedSetType::downward_closed_set, 0, transitionrelation.size()-1, finalstates };
     };
 
     /**
      * @brief This function returns an upward-closed set of all the nodes which are non-final.
      * @return Closed set of non-final nodes.
      */
     StateClosedSet get_non_final_nodes() const;
@@ -391,15 +392,19 @@
     revert(&result, aut);
     return result;
 }
 
 /// Removing epsilon transitions
 void remove_epsilon(Afa* result, const Afa& aut, Symbol epsilon);
 
-inline Afa remove_epsilon(const Afa& aut, Symbol epsilon) { return remove_epsilon(aut, epsilon); }
+inline Afa remove_epsilon(const Afa& aut, Symbol epsilon) {
+    Afa result{};
+    remove_epsilon(&result, aut, epsilon);
+    return result;
+}
 
 /// Minimizes an AFA.  The method can be set using @p params
 void minimize(
     Afa*               result,
     const Afa&         aut,
     const StringDict&  params = {});
```

### Comparing `libmata-0.68.0/mata/include/mata/alphabet.hh` & `libmata-0.69.0/mata/include/mata/alphabet.hh`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,15 @@
     EnumAlphabet(EnumAlphabet&& rhs) = default;
 
     Util::OrdVector<Symbol> get_alphabet_symbols() const override { return m_symbols; }
     Util::OrdVector<Symbol> get_complement(const Util::OrdVector<Symbol>& symbols) const override {
         return m_symbols.difference(symbols);
     }
 
-    std::string reverse_translate_symbol(const Symbol symbol) const override;
+    std::string reverse_translate_symbol(Symbol symbol) const override;
 
 private:
     EnumAlphabet& operator=(const EnumAlphabet& rhs);
 
 public:
     /**
      * @brief Expand alphabet by symbols from the passed @p symbols.
@@ -279,15 +279,15 @@
      */
     explicit OnTheFlyAlphabet(const std::vector<std::string>& symbol_names, Symbol init_symbol = 0)
             : symbol_map(), next_symbol_value(init_symbol) { add_symbols_from(symbol_names); }
 
     Util::OrdVector<Symbol> get_alphabet_symbols() const override;
     Util::OrdVector<Symbol> get_complement(const Util::OrdVector<Symbol>& symbols) const override;
 
-    std::string reverse_translate_symbol(const Symbol symbol) const override;
+    std::string reverse_translate_symbol(Symbol symbol) const override;
 
 private:
     OnTheFlyAlphabet& operator=(const OnTheFlyAlphabet& rhs);
 
 public:
     /**
      * @brief Expand alphabet by symbols from the passed @p symbol_names.
@@ -310,15 +310,15 @@
             add_new_symbol(*first, next_symbol_value);
         }
     }
     OnTheFlyAlphabet(std::initializer_list<std::string> l) : OnTheFlyAlphabet(l.begin(), l.end()) {}
 
     Symbol translate_symb(const std::string& str) override;
 
-    virtual std::vector<Symbol> translate_word(const std::vector<std::string>& word) const;
+    virtual std::vector<Symbol> translate_word(const std::vector<std::string>& word) const override;
 
     /**
      * @brief Add new symbol to the alphabet with the value of @c next_symbol_value.
      *
      * Throws an exception when the adding fails.
      *
      * @param[in] key User-space representation of the symbol.
```

### Comparing `libmata-0.68.0/mata/include/mata/closed-set.hh` & `libmata-0.69.0/mata/include/mata/closed-set.hh`

 * *Files 10% similar despite different names*

```diff
@@ -71,15 +71,18 @@
 
 namespace Mata {
 
 // Ordered vector.
 template<typename T> using OrdVec = Mata::Util::OrdVector<T>;
 
 // A closed set could be upward-closed or downward-closed.
-enum ClosedSetType {upward_closed_set, downward_closed_set};
+enum class ClosedSetType { upward_closed_set, downward_closed_set };
+
+template <typename T> struct ClosedSet;
+template <typename T> std::ostream& operator<<(std::ostream& os, const ClosedSet<T>& cs);
 
 /**
  * @brief Closed set.
  *
  * Contains discrete range borders, its type and the corresponding anti-chain. It is necessary to be able to evaluate
  *  relation operators <, <=, >, >=, ==, != over instances of this datatype T.
  * @tparam T Datatype the closed set contains.
@@ -87,122 +90,122 @@
 template <typename T>
 struct ClosedSet {
     using Node = OrdVec<T>;
     using Nodes = OrdVec<Node>;
 
     private:
 
-       ClosedSetType type_{upward_closed_set}; // upward_closed or downward_closed sets
+       ClosedSetType type_{ ClosedSetType::upward_closed_set }; // upward_closed or downward_closed sets.
        T min_val_;
        T max_val_;
        Nodes antichain_{};
 
     public:
 
        // constructors
        ClosedSet() : type_(), min_val_(), max_val_(), antichain_() { }
 
        // inserting a single value of the datatype T
-       ClosedSet(ClosedSetType type, T min_val, T max_val, T value)
+       ClosedSet(const ClosedSetType type, const T& min_val, const T& max_val, const T& value)
            : type_(type), min_val_(min_val), max_val_(max_val), antichain_(Nodes(value)) {
            assert(min_val <= max_val);
            assert(min_val <= value && value <= max_val);
        }
 
        // inserting a single vector of the datatype T
-       ClosedSet(ClosedSetType type, T min_val, T max_val, Node node)
+       ClosedSet(ClosedSetType type, const T& min_val, const T& max_val, const Node& node)
            : type_(type), min_val_(min_val), max_val_(max_val), antichain_(Node(node)) {
            assert(min_val <= max_val);
            assert(in_interval(node));
        }
 
        // inserting a whole antichain
-       ClosedSet(ClosedSetType type, T min_val, T max_val, Nodes antichain = Nodes())
+       ClosedSet(const ClosedSetType type, const T& min_val, const T& max_val, const Nodes& antichain = Nodes())
            : type_(type), min_val_(min_val), max_val_(max_val) {
            assert(min_val <= max_val);
            insert(antichain);
        }
 
        // operators
 
        // Two closed sets are equivalent iff their type, borders
        // and corresponding antichains are the same
-       bool operator==(ClosedSet<T> rhs) const
+       bool operator==(const ClosedSet<T>& rhs) const
         { // {{{
             return type_ == rhs.type && min_val_ == rhs.min_val &&
             max_val_ == rhs.max_val && antichain_ == rhs.antichain;
         } // operator== }}}
 
        // Two closed sets are not equivalent iff their type,
        // borders or corresponding antichains differ
-       bool operator!=(ClosedSet<T> rhs) const
+       bool operator!=(const ClosedSet<T>& rhs) const
         { // {{{
             return type_ != rhs.type_ || min_val_ != rhs.min_val_ ||
             max_val_ != rhs.max_val_ || antichain_ != rhs.antichain_;
         } // operator!= }}}
 
         // A closed set is considered to be smaller than the other one iff
         // it is a subset of the other one
         // It is not possible to perform <=-comparisons accros upward- and downward-closed
         // sets, each argument has to be upward- or downward-closed set
-        bool operator<=(ClosedSet<T> rhs) const
+        bool operator<=(const ClosedSet<T>& rhs) const
         { // {{{
             assert(type_ == rhs.type_ && min_val_ == rhs.min_val_ && max_val_ == rhs.max_val_ &&
             "Types and borders of given closed sets must be the same to perform their <=-comparison.");
             return rhs.contains(antichain_);
         } // operator<= }}}
 
         // A closed set is considered to be bigger than the other one iff
         // it is a superset of the other one
         // It is not possible to perform <=-comparisons of accros upward-
         // and downward-closed sets, each argument
         // has to be upward- or downward-closed set
-        bool operator>=(ClosedSet<T> rhs) const
+        bool operator>=(const ClosedSet<T>& rhs) const
         { // {{{
             assert(type_ == rhs.type_ && min_val_ == rhs.min_val_ && max_val_ == rhs.max_val_ &&
             "Types and borders of given closed sets must be the same to perform their <=-comparison.");
             return contains(rhs.antichain);
         } // operator<= }}}
 
         // Text representation of a closed set
-        friend std::ostream& operator<<(std::ostream& os, const ClosedSet<T> cs);
+        friend std::ostream& operator<< <> (std::ostream& os, const ClosedSet<T>& cs);
 
-        bool is_upward_closed() const {return type_ == upward_closed_set;};
-        bool is_downward_closed() const {return type_ == downward_closed_set;};
+        bool is_upward_closed() const { return type_ == ClosedSetType::upward_closed_set; };
+        bool is_downward_closed() const { return type_ == ClosedSetType::downward_closed_set; };
 
-        ClosedSetType type() {return type_;}
-        const ClosedSetType type() const {return type_;}
+        ClosedSetType type() { return type_; }
+        ClosedSetType type() const { return type_; }
 
-        Nodes antichain() {return antichain_;}
-        const Nodes antichain() const {return antichain_;}
+        Nodes antichain() { return antichain_;}
+        Nodes antichain() const { return antichain_; }
 
-        T get_min() {return min_val_;}
-        const T get_min() const {return min_val_;}
+        T get_min() { return min_val_; }
+        T get_min() const { return min_val_; }
 
-        T get_max() {return max_val_;}
-        const T get_max() const {return max_val_;}
+        T get_max() { return max_val_; }
+        T get_max() const { return max_val_; }
 
-        bool contains (Node node) const;
-        bool contains (Nodes nodes) const;
+        bool contains (const Node& node) const;
+        bool contains (const Nodes& nodes) const;
 
-        bool in_interval (Node node) const;
+        bool in_interval (const Node& node) const;
 
-        void insert(T el) {insert(Node(el));};
-        void insert(Node node);
-        void insert(Nodes nodes) {for(auto node : nodes) insert(node);};
+        void insert(const T& el) { insert(Node(el)); }
+        void insert(const Node& node);
+        void insert(const Nodes& nodes) {for (const auto& node: nodes) insert(node); }
 
-        ClosedSet Union (const ClosedSet rhs) const;
-        ClosedSet intersection (const ClosedSet rhs) const;
+        ClosedSet Union (const ClosedSet& rhs) const;
+        ClosedSet intersection (const ClosedSet& rhs) const;
         ClosedSet complement () const;
 }; // class ClosedSet.
 
 template<typename T>
-std::ostream& operator<<(std::ostream& os, const ClosedSet<T> cs) {
+std::ostream& operator<<(std::ostream& os, const ClosedSet<T>& cs) {
     std::string strType = "TYPE: ";
-    strType += cs.type() == upward_closed_set ? "UPWARD CLOSED" : "DOWNWARD CLOSED";
+    strType += cs.type() == ClosedSetType::upward_closed_set ? "UPWARD CLOSED" : "DOWNWARD CLOSED";
     strType += "\n";
     std::string strInterval = "INTERVAL: " + std::to_string(cs.get_min()) + " - " + std::to_string(cs.get_max()) + "\n";
     std::string strValues = "ANTICHAIN: {";
     for(auto node : cs.antichain()) {
         strValues += "{";
         for(auto state : node) {
             strValues += " " + std::to_string(state);
@@ -216,23 +219,23 @@
 /** This function decides whether a set of elements is part of the closed set
 * by subset-compraring the input with all elements of the antichain
 * @brief decides whether the closed set contains a given element
 * @param node a given ordered vector of elements of the type T
 * @return true iff the given ordered vector belongs to the current closed set
 */
 template <typename T>
-bool ClosedSet<T>::contains(Node node) const {
-    if(type_ == upward_closed_set) {
+bool ClosedSet<T>::contains(const Node& node) const {
+    if(type_ == ClosedSetType::upward_closed_set) {
         for(auto element : antichain_) {
             if(element.IsSubsetOf(node)) {
                 return true;
             }
         }
     }
-    else if(type_ == downward_closed_set) {
+    else if(type_ == ClosedSetType::downward_closed_set) {
         for(auto element : antichain_) {
             if(node.IsSubsetOf(element)) {
                 return true;
             }
         }
     }
     return false;
@@ -241,15 +244,15 @@
 /** This function decides whether a set of sets of elements is a part of the closed set
 * by subset-compraring the input with all elements of the antichain
 * @brief decides whether the closed set contains a given set of sets of elements
 * @param nodes a given ordered vector of ordered vectors of elements of the type T
 * @return true iff the given ordered vector of ordered vectors belongs to the current closed set
 */
 template <typename T>
-bool ClosedSet<T>::contains(Nodes nodes) const {
+bool ClosedSet<T>::contains(const Nodes& nodes) const {
     for(auto node : nodes) {
         if(!contains(node)) {
             return false;
         }
     }
     return true;
 }
@@ -257,30 +260,30 @@
 /** This function decides whether a given ordered vector of elements of the datatype T
 * belongs to the discrete interval of the current closed set
 * @brief decides whether the given vector respects the borders
 * @param node a given ordered vector of elements of the type T which will be inspected
 * @return true iff the given ordered vector respects the borders
 */
 template <typename T>
-bool ClosedSet<T>::in_interval(Node node) const {
+bool ClosedSet<T>::in_interval(const Node& node) const {
     for(auto value : node) {
         if(value < min_val_ || value > max_val_) {
             return false;
         }
     }
     return true;
 }
 
 /** Adds a new element to the closed set. If the element is already contained in the closed
 * set, the closed set remains unchanged. Otherwise, the antichain will be recomputed.
 * @brief inserts a new element to the closed set
 * @param node a given node which will be added to the closed set
 */
 template <typename T>
-void ClosedSet<T>::insert(Node node) {
+void ClosedSet<T>::insert(const Node& node) {
     assert(in_interval(node) && "Each element of the given node has to respect " &&
     "the carrier of the closed set.");
     // If the closed set is empty, the antichain could be simply changed
     // by adding the given node as the only node to the antichain
     if(antichain_.empty()) {
         antichain_.insert(node);
         return;
@@ -296,29 +299,29 @@
 
     // If the closed set is upward-closed, we have to erase all the elements of
     // the antichain which are supersets of the inserted node
     // Example: Let us have an upward-closed set ↑{{0, 1}, {2}} with a corresponding
     // antichain {{0, 1}, {2}}. If we add {0} to the closed set, the element {0, 1}
     // needs to be erased from the antichain since the set {{0}, {0, 1}, {2}} contains
     // <=-comparable elements and the result should be upward-closed.
-    if(type_ == upward_closed_set) {
+    if(type_ == ClosedSetType::upward_closed_set) {
         for(auto element : antichain_) {
             if(node.IsSubsetOf(element)) {
                 to_erase.insert(element);
             }
         }
     }
 
     // If the closed set is downward-closed, we have to erase all the elements of
     // the antichain which are subsets of the inserted node
     // Example: Let us have an upward-closed set ↓{{0, 1}, {2}} with a corresponding
     // antichain {{0, 1}, {2}}. If we add {1, 2} to the closed set, the element {2}
     // needs to be erased from the antichain since the set {{0}, {1, 2}, {2}} contains
     // <=-comparable elements and the result should be downward-closed.
-    else if(type_ == downward_closed_set) {
+    else if(type_ == ClosedSetType::downward_closed_set) {
         for(auto element : antichain_) {
             if(element.IsSubsetOf(node)) {
                 to_erase.insert(element);
             }
         }
     }
 
@@ -332,46 +335,46 @@
 * This function simply adds all the
 * elements of the antichain of the first closed set to the second closed set
 * @brief performs an union over closed sets
 * @param rhs a given closed set which will be unioned with the current one
 * @return an union of the given closed sets
 */
 template <typename T>
-ClosedSet<T> ClosedSet<T>::Union(const ClosedSet<T> rhs) const {
+ClosedSet<T> ClosedSet<T>::Union(const ClosedSet<T>& rhs) const {
     assert(type_ == rhs.type_ && min_val_ == rhs.min_val_ && max_val_ == rhs.max_val_ &&
     "Types and borders of given closed sets must be the same to compute their union.");
     ClosedSet<T> result(type_, min_val_, max_val_, antichain_);
     result.insert(rhs.antichain());
     return result;
 }
 
 /** Performs an intersection over two closed sets with the same type and carrier.
 * @brief performs an intersection over closed sets
 * @param rhs a given closed set which will be intersectioned with the current one
 * @return an intersection of the given closed sets
 */
 template <typename T>
-ClosedSet<T> ClosedSet<T>::intersection(const ClosedSet<T> rhs) const {
+ClosedSet<T> ClosedSet<T>::intersection(const ClosedSet<T>& rhs) const {
     assert(type_ == rhs.type_ && min_val_ == rhs.min_val_ && max_val_ == rhs.max_val_ &&
     "Types and borders of given closed sets must be the same to compute their union.");
     ClosedSet<T> result(type_, min_val_, max_val_);
 
     // Iterates through all the tuples from Antichan1 X Antichan2
     // and creates an union of them
-    if(type_ == upward_closed_set) {
+    if(type_ == ClosedSetType::upward_closed_set) {
         for(auto element1 : antichain_) {
             for(auto element2 : rhs.antichain()) {
                result.insert(element1.Union(element2));
             }
         }
     }
 
     // Iterates through all the tuples from Antichan1 X Antichan2
     // and creates an intersection of them
-    if(type_ == downward_closed_set) {
+    if(type_ == ClosedSetType::downward_closed_set) {
         for(auto element1 : antichain_) {
             for(auto element2 : rhs.antichain()) {
                result.insert(element1.intersection(element2));
             }
         }
     }
     return result;
@@ -383,21 +386,21 @@
 * @brief performs a complementation over a closed set
 * @return a complement of a closed set
 */
 template <typename T>
 ClosedSet<T> ClosedSet<T>::complement() const {
     // The complement of an upward-closed set is
     // always downward-closed and vice versa.
-    ClosedSetType new_type = upward_closed_set;
-    if(type_ == upward_closed_set) {
-        new_type = downward_closed_set;
+    ClosedSetType new_type = ClosedSetType::upward_closed_set;
+    if(type_ == ClosedSetType::upward_closed_set) {
+        new_type = ClosedSetType::downward_closed_set;
     }
     ClosedSet<T> result = ClosedSet(new_type, get_min(), get_max(), antichain());
 
-    if(type_ == upward_closed_set) {
+    if(type_ == ClosedSetType::upward_closed_set) {
         // Initially, a complement contains all possible elements
         // which will be then (possibly) removed.
         Node initialValues{};
         for(long unsigned i = 0; i <= max_val_; ++i) {
             initialValues.insert(i);
         }
         result.insert(initialValues);
@@ -407,45 +410,45 @@
         // all elements of the carrier except of xn
         // For example, for a node {0, 2, 3} (the maximal element is 4),
         // we create a set {{1, 2, 3, 4}, {0, 1, 3, 4}, {0, 1, 2, 4}}.
         // This set corresponds to an antichain of a new downward-closed set.
         // The result will be an intersection of all downward-closed sets
         // created using this procedure.
         for(const auto& element : antichain()) {
-            ClosedSet preparingAntichain(downward_closed_set, get_min(), get_max());
-            for(int i = 0; i <= max_val_; ++i) {
+            ClosedSet preparingAntichain(ClosedSetType::downward_closed_set, get_min(), get_max());
+            for(T i = 0; i <= max_val_; ++i) {
                 if(!element.count(i)) {
                     continue;
                 }
                 Node candidates{};
-                for(int j = 0; j <= max_val_; ++j) {
-                    if(i!=j) {
+                for(T j = 0; j <= max_val_; ++j) {
+                    if(i != j) {
                         candidates.insert(j);
                     }
                 }
                 preparingAntichain.insert(candidates);
             }
             result = result.intersection(preparingAntichain);
         }
     }
 
-    else if(type_ == downward_closed_set) {
+    else if(type_ == ClosedSetType::downward_closed_set) {
         // Initially, a complement contains all possible elements
         // which will be then (possibly) removed.
         result.insert(Node());
 
         // For each element of the closed set {xa, xb, xc, ...}, we
         // create a set of all sets Xa, Xb, Xc,... such that Xn contains
         // only xn. For example, for a node {0, 2, 3}, we create a set
         // {{0}, {2}, {3}}.
         // This set corresponds to an antichain of a new upward-closed set.
         // The result will be an intersection of all upward-closed sets
         // created using this procedure.
         for(Node element : antichain()) {
-            ClosedSet preparingAntichain(upward_closed_set, min_val_, max_val_);
+            ClosedSet preparingAntichain(ClosedSetType::upward_closed_set, min_val_, max_val_);
             for(T i = min_val_; i <= max_val_; ++i) {
                 Node candidates{i};
                 if(!element.count(i)) {
                     preparingAntichain.insert({i});
                 }
             }
             result = result.intersection(preparingAntichain);
```

### Comparing `libmata-0.68.0/mata/include/mata/inter-aut.hh` & `libmata-0.69.0/mata/include/mata/inter-aut.hh`

 * *Files 4% similar despite different names*

```diff
@@ -103,42 +103,49 @@
         : type(t), raw(std::move(raw)), name(std::move(name)), operator_type(OperatorType::NOT_OPERATOR), operand_type(operand) {}
 
     FormulaNode(Type t, const std::string& raw)
         : type(t), raw(raw), name(raw), operator_type(OperatorType::NOT_OPERATOR), operand_type(OperandType::NOT_OPERAND) {}
 
     FormulaNode(const FormulaNode& n)
         : type(n.type), raw(n.raw), name(n.name), operator_type(n.operator_type), operand_type(n.operand_type) {}
+
+    FormulaNode& operator=(const FormulaNode& other) = default;
+    FormulaNode& operator=(FormulaNode&& other) = default;
 };
 
 /**
  * Structure representing a transition formula using a graph.
  * A node of graph consists of node itself and set of children nodes.
  * Nodes are operators and operands of the formula.
  * E.g., a formula q1 & s1 will be transformed to a tree with & as a root node
  * and q1 and s2 being children nodes of the root.
  */
 struct FormulaGraph {
-    FormulaNode node;
-    std::vector<FormulaGraph> children;
+    FormulaNode node{};
+    std::vector<FormulaGraph> children{};
 
-    FormulaGraph() : node(), children() {}
+    FormulaGraph() = default;
     FormulaGraph(const FormulaNode& n) : node(n), children() {}
     FormulaGraph(const FormulaGraph& g) : node(g.node), children(g.children) {}
 
+    FormulaGraph& operator=(const Mata::FormulaGraph& other) = default;
+    FormulaGraph& operator=(Mata::FormulaGraph&& other) noexcept = default;
+
     std::unordered_set<std::string> collect_node_names() const;
     void print_tree(std::ostream& os) const;
 };
 
 /**
  * Structure for a general intermediate representation of parsed automaton.
  * It contains information about type of automata, type of naming of nodes, symbols and states
  * and type of alphabet. It contains also the transitions formula and formula for initial and final
  * states. The formulas are represented as tree where nodes are either operands or operators.
  */
 struct IntermediateAut {
+public:
     /**
      * Type of automaton. So far we support nondeterministic finite automata (NFA) and
      * alternating finite automata (AFA)
      */
     enum class AutomatonType {
         NFA,
         AFA
@@ -168,37 +175,36 @@
     enum class AlphabetType {
         EXPLICIT,
         BITVECTOR,
         CLASS,
         INTERVALS
     };
 
-public:
     Naming state_naming = Naming::MARKED;
     Naming symbol_naming = Naming::MARKED;
     Naming node_naming = Naming::MARKED;
-    AlphabetType alphabet_type;
-    AutomatonType automaton_type;
+    AlphabetType alphabet_type{};
+    AutomatonType automaton_type{};
 
     // The vectors represent the given sets when enumeration is used.
-    std::vector<std::string> states_names;
-    std::vector<std::string> symbols_names;
-    std::vector<std::string> nodes_names;
+    std::vector<std::string> states_names{};
+    std::vector<std::string> symbols_names{};
+    std::vector<std::string> nodes_names{};
 
-    FormulaGraph initial_formula;
-    FormulaGraph final_formula;
+    FormulaGraph initial_formula{};
+    FormulaGraph final_formula{};
 
     bool initial_enumerated = false;
     bool final_enumerated = false;
 
     /**
      * Transitions are pairs where the first member is left-hand side of transition (i.e., a state)
      * and the second item is a graph representing transition formula (which can contain symbols, nodes, and states).
      */
-    struct std::vector<std::pair<FormulaNode, FormulaGraph>> transitions;
+    struct std::vector<std::pair<FormulaNode, FormulaGraph>> transitions{};
 
     /**
      * Returns symbolic part of transition. That may be just a symbol or bitvector formula.
      * This function is supported only for NFA where transitions have a rhs state at the end of right
      * handed side of transition.
      * @param transition Transition from which symbol is returned
      * @return Graph representing symbol. It maybe just an explicit symbol or graph representing bitvector formula
```

### Comparing `libmata-0.68.0/mata/include/mata/mintermization.hh` & `libmata-0.69.0/mata/include/mata/mintermization.hh`

 * *Files 2% similar despite different names*

```diff
@@ -24,63 +24,64 @@
 namespace Mata {
 
 class Mintermization {
 private: // data types
     struct OptionalBdd {
         enum class TYPE {NOTHING_E, BDD_E};
 
-        TYPE type;
-        BDD val;
+        TYPE type{};
+        BDD val{};
 
+        OptionalBdd() = default;
         explicit OptionalBdd(TYPE t) : type(t) {}
         explicit OptionalBdd(const BDD& bdd) : type(TYPE::BDD_E), val(bdd) {}
         OptionalBdd(TYPE t, const BDD& bdd) : type(t), val(bdd) {}
 
         OptionalBdd operator*(const OptionalBdd& b) const;
         OptionalBdd operator+(const OptionalBdd& b) const;
         OptionalBdd operator!() const;
     };
 
     using DisjunctStatesPair = std::pair<const FormulaGraph *, const FormulaGraph *>;
 
 private: // private data members
-    Cudd bdd_mng; // Manager of BDDs from lib cubdd, it allocates and manages BDDs.
-    std::unordered_map<std::string, BDD> symbol_to_bddvar;
-    std::unordered_map<const FormulaGraph *, BDD> trans_to_bddvar;
-    std::unordered_map<const FormulaNode*, std::vector<DisjunctStatesPair>> lhs_to_disjuncts_and_states;
-    std::unordered_set<BDD> bdds; // bdds created from transitions
+    Cudd bdd_mng{}; // Manager of BDDs from lib cubdd, it allocates and manages BDDs.
+    std::unordered_map<std::string, BDD> symbol_to_bddvar{};
+    std::unordered_map<const FormulaGraph *, BDD> trans_to_bddvar{};
+    std::unordered_map<const FormulaNode*, std::vector<DisjunctStatesPair>> lhs_to_disjuncts_and_states{};
+    std::unordered_set<BDD> bdds{}; // bdds created from transitions
 
 private:
     void trans_to_bdd_nfa(const IntermediateAut& aut);
     void trans_to_bdd_afa(const IntermediateAut& aut);
 
 public:
     /**
      * Takes a set of BDDs and build a minterm tree over it.
      * The leaves of BDDs, which are minterms of input set, are returned
-     * @param bdds BDDs for which minterms are computed
+     * @param source_bdds BDDs for which minterms are computed
      * @return Computed minterms
      */
-    std::unordered_set<BDD> compute_minterms(const std::unordered_set<BDD>& bdds);
+    std::unordered_set<BDD> compute_minterms(const std::unordered_set<BDD>& source_bdds);
 
     /**
      * Transforms a graph representing formula at transition to bdd.
      * @param graph Graph to be transformed
      * @return Resulting BDD
      */
-    const BDD graph_to_bdd_nfa(const FormulaGraph& graph);
+    BDD graph_to_bdd_nfa(const FormulaGraph& graph);
 
     /**
      * Transforms a graph representing formula at transition to bdd.
      * This version of method is a more general one and accepts also
      * formula including states.
      * @param graph Graph to be transformed
      * @return Resulting BDD
      */
-    const OptionalBdd graph_to_bdd_afa(const FormulaGraph& graph);
+    OptionalBdd graph_to_bdd_afa(const FormulaGraph& graph);
 
     /**
      * Method mintermizes given automaton which has bitvector alphabet.
      * It transforms its transitions to BDDs, then build a minterm tree over the BDDs
      * and finally transforms automaton to explicit one.
      * @param aut Automaton to be mintermized.
      * @return Mintermized automaton
```

### Comparing `libmata-0.68.0/mata/include/mata/nfa-algorithms.hh` & `libmata-0.69.0/mata/include/mata/nfa-algorithms.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/include/mata/nfa-plumbing.hh` & `libmata-0.69.0/mata/include/mata/nfa-plumbing.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/include/mata/nfa-strings.hh` & `libmata-0.69.0/mata/include/mata/nfa-strings.hh`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 using EpsCntVector = std::vector<unsigned>;
 
 /**
 * Class executing segmentation operations for a given segment automaton. Works only with segment automata.
 */
 class Segmentation {
 public:
-    using EpsilonDepth = unsigned; ///< Depth of ε-transitions.
+    using EpsilonDepth = size_t; ///< Depth of ε-transitions.
     /// Dictionary of lists of ε-transitions grouped by their depth.
     /// For each depth 'i' we have 'depths[i]' which contains a list of ε-transitions of depth 'i'.
     using EpsilonDepthTransitions = std::unordered_map<EpsilonDepth, TransSequence>;
     using EpsilonDepthTransitionMap = std::unordered_map<EpsilonDepth, std::unordered_map<State,TransSequence>>;
 
     /**
      * Prepare automaton @p aut for segmentation.
```

### Comparing `libmata-0.68.0/mata/include/mata/nfa.hh` & `libmata-0.69.0/mata/include/mata/nfa.hh`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,16 @@
 using State = unsigned long;
 using StateSet = Mata::Util::OrdVector<State>;
 
 template<typename T> using Set = Mata::Util::OrdVector<T>;
 
 using WordSet = std::set<std::vector<Symbol>>;
 struct Run {
-    std::vector<Symbol> word; ///< A finite-length word.
-    std::vector<State> path; ///< A finite-length path through automaton.
+    std::vector<Symbol> word{}; ///< A finite-length word.
+    std::vector<State> path{}; ///< A finite-length path through automaton.
 };
 
 using StringToStateMap = std::unordered_map<std::string, State>;
 
 using StateToStringMap = std::unordered_map<State, std::string>;
 // using StateToPostMap = StateMap<PostSymb>; ///< Transitions.
 /// Mapping of states to states, used, for example, to map original states to reindexed states of new automaton, etc.
@@ -78,18 +78,19 @@
 using StringMap = std::unordered_map<std::string, std::string>;
 
 /*TODO: What about to
  * have names Set, UMap/OMap, State, Symbol, Sequence... and name by Set<State>, UMap<State>, ...
  * maybe something else is needed for the more complex maps*/
 
 struct Limits {
-    static const State maxState = std::numeric_limits<State>::max();
-    static const State minState = std::numeric_limits<State>::min();
-    static const Symbol maxSymbol = std::numeric_limits<Symbol>::max();
-    static const Symbol minSymbol = std::numeric_limits<Symbol>::min();
+public:
+    static const State min_state = std::numeric_limits<State>::min();
+    static const State max_state = std::numeric_limits<State>::max();
+    static const Symbol min_symbol = std::numeric_limits<Symbol>::min();
+    static const Symbol max_symbol = std::numeric_limits<Symbol>::max();
 };
 
 /*TODO: Ideally remove functions using this struct as a parameter.
  * unpack the trans. relation to transitions is inefficient, goes against the hairs of the library.
  * Do we want to support it?
  */
 /// A single transition.
@@ -169,24 +170,24 @@
     StateSet::const_iterator cend() const { return targets.cend(); }
 
     size_t count(State s) const { return targets.count(s); }
     bool empty() const { return targets.empty(); }
     size_t size() const { return targets.size(); }
 
     void insert(State s);
-    void insert(StateSet states);
+    void insert(const StateSet& states);
 
     // THIS BREAKS THE SORTEDNESS INVARIANT,
     // dangerous,
     // but useful for adding states in a random order to sort later (supposedly more efficient than inserting in a random order)
     void inline push_back(const State s) { targets.push_back(s); }
 
     void remove(State s) { targets.remove(s); }
 
-    const std::vector<State>::iterator find(State s) const { targets.find(s); }
+    std::vector<State>::const_iterator find(State s) const { return targets.find(s); }
     std::vector<State>::iterator find(State s) { return targets.find(s); }
 };
 
 /**
  * Post is a data structure representing possible transitions over different symbols.
  * It is an ordered vector containing possible Moves (i.e., pair of symbol and target states.
  * Vector is ordered by symbols which are numbers.
@@ -195,26 +196,29 @@
 private:
     using super = Util::OrdVector<Move>;
 public:
     using super::iterator, super::const_iterator;
     using super::begin, super::end, super::cbegin, super::cend;
     using super::OrdVector;
     using super::operator=;
-    using super::find;
     using super::insert;
     using super::reserve;
     using super::remove;
     using super::empty, super::size;
     using super::ToVector;
     using super::erase;
     // dangerous, breaks the sortedness invariant
     using super::push_back;
     // is adding non-const version as well ok?
     using super::back;
     using super::filter;
+
+    using super::find;
+    iterator find(const Symbol symbol) { return super::find({ symbol, {} }); }
+    const_iterator find(const Symbol symbol) const { return super::find({ symbol, {} }); }
 }; // struct Post.
 
 /**
  * Delta is a data structure for representing transition relation.
  * Its underlying data structure is vector of Post structures.
  * Each index of vector corresponds to one state, that is a number of
  * state is an index to the vector of Posts.
@@ -241,20 +245,19 @@
     // Get a non const reference to post of a state, which allows modifying the post.
     //
     // BEWARE, IT HAS A SIDE EFFECT.
     //
     // Namely, it allocates the post of the state if it was not allocated yet. This in turn may cause that
     // the entire post data structure is re-allocated, iterators to it get invalidated ...
     // Use the constant [] operator below if possible.
-    // Or, to prevent the side effect form happening, one might want to make sure that posts of all states in the automaton
+    // Or, to prevent the side effect from happening, one might want to make sure that posts of all states in the automaton
     // are allocated, e.g., write an NFA method that allocate delta for all states of the NFA.
     // But it feels fragile, before doing something like that, better think and talk to people.
     Post& get_mutable_post(State q);
 
-    // TODO: why do we have the code of all these methods in the header file? Should we move it out?
     // TODO: Explain what is returned from this method.
     std::vector<State> defragment(Util::NumberPredicate<State> & is_staying);
 
     // Get a constant reference to the post of a state. No side effects.
     const Post & operator[] (State q) const;
 
     void emplace_back() { posts.emplace_back(); }
@@ -287,19 +290,25 @@
     /**
      * Iterator over transitions. It iterates over triples (lhs, symbol, rhs) where lhs and rhs are states.
      */
     struct const_iterator {
     private:
         const std::vector<Post>& post;
         size_t current_state;
-        Post::const_iterator post_iterator;
-        StateSet::const_iterator targets_position;
+        Post::const_iterator post_iterator{};
+        StateSet::const_iterator targets_position{};
         bool is_end;
 
     public:
+        using iterator_category = std::bidirectional_iterator_tag;
+        using value_type = int;
+        using difference_type = int;
+        using pointer = int*;
+        using reference = int&;
+
         explicit const_iterator(const std::vector<Post>& post_p, bool ise = false);
 
         const_iterator(const std::vector<Post>& post_p, size_t as,
                        Post::const_iterator pi, StateSet::const_iterator ti, bool ise = false) :
                 post(post_p), current_state(as), post_iterator(pi), targets_position(ti), is_end(ise) {};
 
         const_iterator(const const_iterator& other) = default;
@@ -322,16 +331,18 @@
     const_iterator begin() const { return cbegin(); }
     const_iterator end() const { return cend(); }
 
 private:
     State find_max_state();
 }; // struct Delta.
 
+bool operator==(const Delta::const_iterator& a, const Delta::const_iterator& b);
+
 /// An epsilon symbol which is now defined as the maximal value of data type used for symbols.
-constexpr Symbol EPSILON = Limits::maxSymbol;
+constexpr Symbol EPSILON = Limits::max_symbol;
 
 /**
  * A struct representing an NFA.
  */
 struct Nfa {
 public:
     /**
@@ -352,15 +363,15 @@
     //  dictionary in the attributes.
     std::unordered_map<std::string, void*> attributes{};
 
 public:
     explicit Nfa(Delta delta = {}, Util::NumberPredicate<State> initial_states = {},
                  Util::NumberPredicate<State> final_states = {}, Alphabet* alphabet = nullptr)
         : delta(std::move(delta)), initial(std::move(initial_states)), final(std::move(final_states)), alphabet(alphabet) {}
-        
+
     /**
      * @brief Construct a new explicit NFA with num_of_states states and optionally set initial and final states.
      *
      * @param[in] num_of_states Number of states for which to preallocate Delta.
      */
     explicit Nfa(const unsigned long num_of_states, StateSet initial_states = {},
                  StateSet final_states = {}, Alphabet* alphabet = nullptr)
@@ -474,15 +485,15 @@
      * Useful states are reachable and terminating states.
      * @return Set of useful states.
      * TODO: with the new get_useful_states, we can delete this probably.
      */
     StateSet get_useful_states_old() const;
 
     //I just want to return something as constant reference to the thing, without copying anything, how?
-    const Util::NumberPredicate<State> get_useful_states() const;
+    Util::NumberPredicate<State> get_useful_states() const;
 
     /**
      * @brief Remove inaccessible (unreachable) and not co-accessible (non-terminating) states.
      *
      * Remove states which are not accessible (unreachable; state is accessible when the state is the endpoint of a path
      * starting from an initial state) or not co-accessible (non-terminating; state is co-accessible when the state is
      * the starting point of a path ending in a final state).
@@ -507,15 +518,20 @@
     Nfa get_trimmed_automaton(StateToStateMap* state_map = nullptr) const;
 
     /**
      * Remove epsilon transitions from the automaton.
      */
     void remove_epsilon(Symbol epsilon = EPSILON);
 
-    size_t get_num_of_trans() const; ///< Number of transitions; contains linear time complexity.
+    /**
+     * @brief Get a number of transitions in the whole automaton.
+     *
+     * The operation has constant time complexity.
+     */
+    size_t get_num_of_trans() const { return static_cast<size_t>(std::distance(delta.begin(), delta.end())); }
 
     /**
      * Get transitions as a sequence of @c Trans.
      * @return Sequence of transitions as @c Trans.
      */
     TransSequence get_trans_as_sequence() const;
```

### Comparing `libmata-0.68.0/mata/include/mata/number-predicate.hh` & `libmata-0.69.0/mata/include/mata/number-predicate.hh`

 * *Files 2% similar despite different names*

```diff
@@ -85,54 +85,48 @@
             } else {
                 prune_elements();
             }
         }
     }
 
 public:
-    NumberPredicate(Number size,bool val,bool track_elements = true)
-        : elements_are_exact(true), tracking_elements(track_elements), predicate(size, val) {
+    NumberPredicate(Number size, bool val, bool track_elements = true)
+        : predicate(size, val), elements_are_exact(true), tracking_elements(track_elements) {
         if (tracking_elements && val) {
             elements.reserve(size);
             for (Number e = 0;e<size;++e)
                 elements.push_back(e);
         }
         if (!val)
             cardinality = 0;
         else
             cardinality = size;
-    };
-
-    NumberPredicate(bool track_elements = true)
-        : elements_are_exact(true), tracking_elements(track_elements), cardinality(0) {};
-
-    NumberPredicate(std::initializer_list <Number> list, bool track_elements = true)
-        : elements_are_exact(true), tracking_elements(track_elements), cardinality(0) {
-        for (auto q: list)
-            add(q);
     }
 
-    NumberPredicate(std::vector <Number> list, bool track_elements = true)
-        : elements_are_exact(true), tracking_elements(track_elements), cardinality(0) {
-        add(list);
+    NumberPredicate() = default;
+    explicit NumberPredicate(const bool track_elements) : tracking_elements(track_elements) {}
+    NumberPredicate(std::initializer_list<Number> list, bool track_elements = true)
+        : tracking_elements(track_elements) {
+        for (const auto& q: list) { add(q); }
     }
 
-    NumberPredicate(const std::vector<bool> & bv, bool track_elements = true)
-        : elements_are_exact(true), tracking_elements(track_elements), cardinality(0) {
+    explicit NumberPredicate(const std::vector<Number>& list, const bool track_elements = true)
+        : tracking_elements(track_elements) { add(list); }
+
+    explicit NumberPredicate(const std::vector<bool>& bv, bool track_elements = true)
+        : tracking_elements(track_elements) {
         predicate.reserve(bv.size());
         for (size_t i = 0;i<bv.size();i++) {
-            if (bv[i])
-                add(i);
+            if (bv[i]) { add(i); }
         }
     }
 
-    explicit NumberPredicate(Mata::Util::OrdVector<Number> vec, bool track_elements = true)
-        : elements_are_exact(true), tracking_elements(track_elements), cardinality(0) {
-        for (auto q: vec)
-            add(q);
+    explicit NumberPredicate(const Mata::Util::OrdVector<Number>& vec, bool track_elements = true)
+        : tracking_elements(track_elements) {
+        for (const auto& q: vec) { add(q); }
     }
 
     NumberPredicate(const NumberPredicate<Number>& rhs) = default;
     NumberPredicate(NumberPredicate<Number>&& other) noexcept
         : predicate{ std::move(other.predicate) }, elements{ std::move(other.elements) },
           elements_are_exact{ other.elements_are_exact}, tracking_elements{ other.tracking_elements },
           cardinality{ other.cardinality} {
```

### Comparing `libmata-0.68.0/mata/include/mata/ord-vector.hh` & `libmata-0.69.0/mata/include/mata/ord-vector.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/include/mata/parser.hh` & `libmata-0.69.0/mata/include/mata/parser.hh`

 * *Files 13% similar despite different names*

```diff
@@ -43,17 +43,14 @@
 	std::list<BodyLine> body;
 
 	ParsedSection() : type(), dict(), body() {}
 
 	/// Is the section empty?
 	bool empty() const { return type.empty() && dict.empty() && body.empty(); }
 
-	/// Output stream operator
-	friend std::ostream& operator<<(std::ostream& os, const ParsedSection& parsec);
-
 	/// Equality operator
 	bool operator==(const ParsedSection& rhs) const;
 	bool operator!=(const ParsedSection& rhs) const { return !(*this == rhs); }
 
 	/// subscript operator for the key-value store
 	const std::vector<std::string>& operator[](const std::string& key) const;
 
@@ -77,8 +74,13 @@
 ParsedSection parse_mf_section(const std::string& input, bool keepQuotes = false);
 
 /// registers dispatcher
 void init();
 
 } // namespace Mata::Parser.
 
+namespace std {
+    /// Output stream operator
+    std::ostream& operator<<(std::ostream& os, const Mata::Parser::ParsedSection& parsec);
+}
+
 #endif /* MATA_PARSER_HH_ */
```

### Comparing `libmata-0.68.0/mata/include/mata/re2parser.hh` & `libmata-0.69.0/mata/include/mata/re2parser.hh`

 * *Files 17% similar despite different names*

```diff
@@ -22,12 +22,12 @@
 
 /**
  * @brief Parser from regular expression to automata.
  *
  * Currently supported automata types are NFA and AFA.
  */
 namespace Mata::Parser {
-    void create_nfa(Nfa::Nfa* nfa, const std::string &pattern, bool use_epsilon = false, int epsilon_value = 306,
-                    bool use_reduction = true);
+    void create_nfa(Nfa::Nfa* nfa, const std::string &pattern, bool use_epsilon = false, Mata::Symbol epsilon_value = 306,
+                    bool use_reduce = true);
 }
 
 #endif // MATA_RE2PARSER_HH
```

### Comparing `libmata-0.68.0/mata/include/mata/synchronized-iterator.hh` & `libmata-0.69.0/mata/include/mata/synchronized-iterator.hh`

 * *Files 1% similar despite different names*

```diff
@@ -50,29 +50,29 @@
  * opposed to creating a new one for each iteration.
  */
 
 /// Class implementing synchronized iteration.
 template<typename Iterator> class SynchronizedIterator {
 public:
 
-    std::vector<Iterator> positions;
-    std::vector<Iterator> ends;
+    std::vector<Iterator> positions{};
+    std::vector<Iterator> ends{};
 
     /// @param size Number of elements to reserve up-front for positions and ends.
     explicit SynchronizedIterator(const int size = 0) {
         positions.reserve(size);
         ends.reserve(size);
     };
 
     /** This is supposed to be called only before an iteration,
      * after constructor of reset.
      * Calling after advance breaks the iterator.
      * Specifies begin and end of one vector, to initialise before the iteration starts.
      */
-    virtual void push_back (const Iterator &begin, const Iterator &end) {
+    virtual void push_back(const Iterator& begin, const Iterator& end) {
         // Btw, I don't know what I am doing with the const & parameter passing,
         // begin is actually incremented in advance ...? But tests do pass ...
         this->positions.emplace_back(begin);
         this->ends.emplace_back(end);
     };
 
 
@@ -86,16 +86,18 @@
         if (size > 0) {
             positions.reserve(size);
             ends.reserve(size);
         }
     };
 
     virtual bool advance() = 0;
-    virtual const std::vector<Iterator> get_current() = 0;
-};
+    virtual std::vector<Iterator> get_current() = 0;
+
+    virtual ~SynchronizedIterator() = default;
+}; // class SynchronizedIterator.
 
 
 
 template<typename Iterator>
 class SynchronizedUniversalIterator: public SynchronizedIterator<Iterator> {
 public:
 
@@ -156,36 +158,34 @@
             }
         }
         this->synchronized_at_current_minimum = true;
         return true;
     }
 
     /// Returns the vector of current positions.
-    const std::vector<Iterator> get_current() {
+    std::vector<Iterator> get_current() {
         // How to return so that things don't get copied?
         // Or maybe we should return a copy of positions anyway, to prevent a side effect of advance?
         // Instead of returning a vector, we could also provide iterators through the result.
         return this->positions;
     };
 
     explicit SynchronizedUniversalIterator(const int size=0) : SynchronizedIterator<Iterator>(size) {};
 
     void reset(const int size = 0) {
         SynchronizedIterator < Iterator > ::reset(size);
         this->synchronized_at_current_minimum = false;
     };
-};
+}; // class SynchronizedUniversalIterator.
 
 template<typename Iterator>
 class SynchronizedExistentialIterator : public SynchronizedIterator<Iterator> {
 public:
-
-    std::vector<Iterator> currently_synchronized; // Positions that are currently synchronized.
-
-    Iterator next_minimum; // the value we should synchronise on after the first next call of advance().
+    std::vector<Iterator> currently_synchronized{}; // Positions that are currently synchronized.
+    Iterator next_minimum{}; // The value we should synchronise on after the first next call of advance().
 
     bool is_synchronized() { return !currently_synchronized.empty(); }
 
     Iterator get_current_minimum() {
         if (currently_synchronized.empty()) {
             throw std::runtime_error("Trying to get minimum from sync. ex. iterator which has no minimum. Don't do "
                                      "that ever again or your nose falls off!");
@@ -246,15 +246,15 @@
 
     /**
      * @brief Returns the vector of current still active positions.
      *
      * Beware, thy will be ordered differently from how there were input into the iterator.
      * This is due to swapping of the emptied positions with positions at the end.
      */
-    const std::vector<Iterator> get_current() { return this->currently_synchronized; };
+    std::vector<Iterator> get_current() { return this->currently_synchronized; };
 
     void push_back (const Iterator &begin, const Iterator &end) {
 
         // Empty vector would not have any effect (unlike in the case of the universal iterator).
         if (begin == end) return;
 
         // Initialise next_minimum as the first position at the first vector.
```

### Comparing `libmata-0.68.0/mata/include/mata/util.hh` & `libmata-0.69.0/mata/include/mata/util.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/src/afa/afa.cc` & `libmata-0.69.0/mata/src/afa/afa.cc`

 * *Files 6% similar despite different names*

```diff
@@ -27,18 +27,17 @@
 using std::tie;
 
 using namespace Mata::Util;
 using namespace Mata::Afa;
 
 const std::string Mata::Afa::TYPE_AFA = "AFA";
 
-std::ostream& std::operator<<(std::ostream& os, const Mata::Afa::Trans& trans)
-{ // {{{
-	std::string result = "(" + std::to_string(trans.src) + ", " 
-                       + std::to_string(trans.symb) + ", " 
+std::ostream& std::operator<<(std::ostream& os, const Mata::Afa::Trans& trans) {
+	std::string result = "(" + std::to_string(trans.src) + ", "
+                       + std::to_string(trans.symb) + ", "
                        + std::to_string(trans.dst) + ")";
 	return os << result;
 } // operator<<(ostream, Trans) }}}
 
 /** This function adds a new transition to the automaton. It changes a transition
 * relation. The transition is added to the transition relation it its current form.
 * @brief adds a new transition
@@ -54,20 +53,20 @@
 	for(auto & transVec : transitionrelation[trans.src])
 	{
 		if(transVec.symb == trans.symb)
 		{
 			// Before the dst nodes are added to the transition, we want to get rid
 			// of redundant clauses. For example, in context of the formula
 			// (1 || (1 && 2)), the clause (1 && 2) could be deleted
-			auto cl = StateClosedSet(upward_closed_set, 0, transitionrelation.size()-1, transVec.dst);
+			auto cl = StateClosedSet(ClosedSetType::upward_closed_set, 0, transitionrelation.size()-1, transVec.dst);
 			cl.insert(trans.dst);
-			transVec.dst = cl.antichain();	
+			transVec.dst = cl.antichain();
 			return;
 		}
-	}    
+	}
 
 	// If there is no result, a new transition will be created
 	transitionrelation[trans.src].push_back(trans);
 
 } // add_trans }}}
 
 /** This function gets a vector of all transitions which are possible to
@@ -77,15 +76,15 @@
 * @return a vector of transitions
 */
 std::vector<Trans> Afa::get_trans_from_state(State state) const
 {
 	assert(state < transitionrelation.size() &&
 	"It is not possible to perform transitions from an non-existing state.");
 	std::vector<Trans> result = std::vector<Trans>();
-	for(auto transition : transitionrelation[state])
+	for(const auto& transition : transitionrelation[state])
 	{
 		result.push_back(transition);
 	}
 	return result;
 }
 
 /** This function gets a vector of all transitions which are possible to
@@ -103,15 +102,15 @@
 	for(auto transition : transitionrelation[state])
 	{
 		if(transition.symb == symbol)
 		{
 			return transition;
 		}
 	}
-	return Trans(state, symbol, Nodes());
+    return { state, symbol, Nodes{} };
 }
 
 
 /** This function adds a new inverse transition to the automaton
 * It changes an inverse transition relation.
 * @brief adds a new inverse transition
 * @param trans a given TRANSITION (it will be inverted within this function)
@@ -122,36 +121,36 @@
 	// Iterating through all the nodes which were given as a destination of the current transition
 	for(auto node : trans.dst)
 	{
 
 		// If there is already a memory cell which corresponds to the current dst node and a
 		// transition symbol, we have to find it and add the 'src' state to the corresponding
 		// result_node vector. Let us recall that the inverse transition datatype is a vector
-		// of vectors of tuples (symbol, vector_of_inverse_results). Each InverseResult is 
+		// of vectors of tuples (symbol, vector_of_inverse_results). Each InverseResult is
 		// a tuple (result_node, precondition). If there exists such a tuple, where
 		// the precondition corresponds to the current dst node, we can simply add the current
 		// 'src' state to the result_node. Since the corresponding tuple (result_node,
 		// precondition) would be identical for all states of the current node, we can store it
-		// to the memory only once. For this purpose, we choose the minimal element from 
+		// to the memory only once. For this purpose, we choose the minimal element from
 		// the current node. Then, it is sufficient to choose the minimal element of the dst
-		// node and look if there exists such a tuple (result_node, precondition), where 
+		// node and look if there exists such a tuple (result_node, precondition), where
 		// precondition == dst node in context of the current symbol.
 		//
-		// Example: We have transitions (0, a, {0, 1}), (0, b, {1}). 
+		// Example: We have transitions (0, a, {0, 1}), (0, b, {1}).
 		// The inverse transition data structure looks like this:
 		//
 		// 0 -> {('a', {(result_node:{0}, precondition:{0, 1})})}
 		// 1 -> {('a', {}),
 		//      ('b', {(result_node:{0}, precondition:{1})})}
 		//
 		// Now, we want to add the transition (1, a, {0, 1}), so we choose the minimal element
 		// of the dst node {0, 1}, access the corresponding element of the inverse transition
 		// relation and look if there exists a tuple (result_node, precondition),
 		// where precondition == {0, 1}.  If so, we add 1 to the result_node. The result:
-		//	
+		//
 		// 0 -> {('a', {(result_node:{0, 1}, precondition:{0, 1})})}
 		// 1 -> {('a', {}),
 		//      ('b', {(result_node:{0}, precondition:{1})})}
 		bool found = false;
 
 		State storeTo = *(node.begin());
 
@@ -173,28 +172,26 @@
 
 		// Otherwise, we need to create a new tuple (result_node, precondition)
 		// == ({src state}, node) and store it to the vector given by the minimal
 		// state of the current node and the current symbol
 
 		// If there is no tuple (symbol, vector_of_pointers) in context of the current
 		// state and symbol because the symbol has not been used yet, we need to create it
-		if(perform_inverse_trans(storeTo, trans.symb).empty())
-		{
-			inverseTransRelation[storeTo].push_back
-			(InverseTrans(trans.src, trans.symb, InverseResults(trans.src, node)));
+		if(perform_inverse_trans(storeTo, trans.symb).empty()) {
+			inverseTransRelation[storeTo].emplace_back(trans.src, trans.symb, InverseResults(trans.src, node));
 			continue;
-		} 
+		}
 
 		// Otherwise, we need to find the appropriate tuple (symbol, inverse_results)
 		// and store the inverse result to the vector of inverse results
 		for(auto & transVec : inverseTransRelation[storeTo])
 		{
 			if(transVec.symb == trans.symb)
 			{
-			    transVec.inverseResults.push_back(InverseResults(trans.src, node));
+			    transVec.inverseResults.emplace_back(trans.src, node);
 			    break;
 			}
 		}
 	}
 
 } // add_inverse_trans }}}
 
@@ -214,48 +211,46 @@
 // POST
 //
 // Inspection of the automaton in the forward fashion
 //
 //***************************************************
 
 /** This function takes a single state and a symbol and returns all the nodes
-* which are accessible from the node {state} in one step using the given symbol. 
+* which are accessible from the node {state} in one step using the given symbol.
 * The output will be represented as a ClosedSet to omit the neccessity
 * to explicitly return all the proper nodes. The result is always an upward closed set!
 * @param state a source state
 * @param symb a symbol used to perform a transition
 * @return closed set of nodes
 */
-StateClosedSet Afa::post(State state, Symbol symb) const
-{
-	return StateClosedSet(upward_closed_set, 0, transitionrelation.size()-1, 
-	get_trans_from_state(state, symb).dst);
-} // post }}}
+StateClosedSet Afa::post(const State state, const Symbol symb) const {
+	return { ClosedSetType::upward_closed_set, 0, transitionrelation.size()-1, get_trans_from_state(state, symb).dst };
+}
 
 /** This function takes a single node and a symbol and returns all the nodes
-* which are accessible from the node in one step using the given symbol. 
+* which are accessible from the node in one step using the given symbol.
 * The output will be represented as a ClosedSet to omit the neccessity
 * to explicitly return all the proper nodes. We will perform a transition
 * for each state of the given node and then, we perform an intersection
 * over these subresults. The result is always an upward closed set!
 * @param node a source set of states
 * @param symb a symbol used to perform a transition
 * @return closed set of nodes
 */
-StateClosedSet Afa::post(Node node, Symbol symb) const
+StateClosedSet Afa::post(const Node& node, const Symbol symb) const
 {
 	// initially, the result is empty
-	StateClosedSet result = StateClosedSet(upward_closed_set, 0, transitionrelation.size()-1);
+	StateClosedSet result = StateClosedSet(ClosedSetType::upward_closed_set, 0, transitionrelation.size()-1);
 	if(node.empty())
 	{
 		result.insert(node);
 		return result;
 	}
 
-	// we get the first result without any changes and then, we will 
+	// we get the first result without any changes and then, we will
 	// perform several intersections over it
 	bool used = false;
 	for(auto state : node)
 	{
 		if(!used)
 		{
 			result.insert(post(state, symb).antichain());
@@ -273,104 +268,104 @@
 * to explicitly return all the proper nodes. We will perform a transition for each node
 * of the given set of nodes and then, we perform an union over these subresults.
 * The result is always an upward closed set!
 * @param nodes a source set of sets of states
 * @param symb a symbol used to perform a transition
 * @return closed set of nodes
 */
-StateClosedSet Afa::post(Nodes nodes, Symbol symb) const
+StateClosedSet Afa::post(const Nodes& nodes, const Symbol symb) const
 {
 	// initially, the result is empty
-	StateClosedSet result = StateClosedSet(upward_closed_set, 0, transitionrelation.size()-1);
-	for(auto node : nodes)
+	StateClosedSet result = StateClosedSet{ ClosedSetType::upward_closed_set, 0, transitionrelation.size()-1 };
+	for(const auto& node : nodes)
 	{
 		result.insert(post(node, symb).antichain());
 	}
 	return result;
 } // post }}}
 
-/** This function allows us to perform post directly over the closed set. 
-* The output will be represented as a ClosedSet to omit the neccessity to 
+/** This function allows us to perform post directly over the closed set.
+* The output will be represented as a ClosedSet to omit the neccessity to
 * explicitly return all the proper nodes. We will perform a transition for
 * each node of the antichain of the given set of nodes and then we perform
 * an union over these subresults. The result is always an upward closed set!
 * @param closed_set an upward closed set which will be used to perform a transition
 * @param symb a symbol used to perform a transition
 * @return closed set of nodes
 */
-StateClosedSet Afa::post(StateClosedSet closed_set, Symbol symb) const
+StateClosedSet Afa::post(const StateClosedSet& closed_set, const Symbol symb) const
 {
-	assert(closed_set.type() == Mata::upward_closed_set && "The predicate transformer " &&
+	assert(closed_set.type() == Mata::ClosedSetType::upward_closed_set && "The predicate transformer " &&
 	" post can be computed only over upward-closed sets.");
 	return post(closed_set.antichain(), symb);
 } // post }}}
 
 
-/** This function takes a single node and and returns all the nodes which are 
+/** This function takes a single node and and returns all the nodes which are
 * accessible from the node in one step using any symbol. The output will be
-* represented as a ClosedSet to omit the neccessity to explicitly return all 
-* the proper nodes. We will perform a transition for each state of the given 
+* represented as a ClosedSet to omit the neccessity to explicitly return all
+* the proper nodes. We will perform a transition for each state of the given
 * node and then, we perform an intersection over these subresults.
 * The result is always an upward closed set!
 * @param node a source set of states
 * @return closed set of nodes
 */
-StateClosedSet Afa::post(Node node) const
+StateClosedSet Afa::post(const Node& node) const
 {
 	if(node.empty())
 	{
-		return StateClosedSet(upward_closed_set, 0, transitionrelation.size()-1, Nodes{Node{}});
+		return StateClosedSet(ClosedSetType::upward_closed_set, 0, transitionrelation.size()-1, Nodes{Node{}});
 	}
-	StateClosedSet result = StateClosedSet(upward_closed_set, 0, transitionrelation.size()-1);
+	StateClosedSet result = StateClosedSet(ClosedSetType::upward_closed_set, 0, transitionrelation.size()-1);
 
 	// It is sufficient to access the first element of the node
 	// to collect all required symbols of the alphabet. If there is another symbol used
 	// in context of another state of the node, it won't affect the result. The result for
 	// such symbol will be empty since it is not used in context of all states
 	// stored in the node
-	for(auto transVec : transitionrelation[*(node.begin())])
+	for(const auto& transVec : transitionrelation[*(node.begin())])
 	{
 		result.insert(post(node, transVec.symb).antichain());
 	}
 	return result;
 } // post }}}
 
-/** This function allows us to perfom "post" and use the whole alphabet 
-* to perform individual transitions. The output will be represented as 
+/** This function allows us to perfom "post" and use the whole alphabet
+* to perform individual transitions. The output will be represented as
 * a ClosedSet to omit the neccessity to explicitly return all the proper nodes.
 * We will perform a transition for each node of the antichain of the given set
 * of nodes and then we perform an union over these subresults.
 * The result is always an upward closed set!
 * @param nodes a set of sets of nodes used to perform a transition
 * @return closed set of nodes
 */
-StateClosedSet Afa::post(Nodes nodes) const
+StateClosedSet Afa::post(const Nodes& nodes) const
 {
-	StateClosedSet result(upward_closed_set, 0, transitionrelation.size()-1);
-	for(auto node : nodes)
+	StateClosedSet result(ClosedSetType::upward_closed_set, 0, transitionrelation.size()-1);
+	for(const auto& node : nodes)
 	{
 		result.insert(post(node).antichain());
 	}
 	return result;
 } // post }}}
 
 
-/** This function allows us to perfom "post" and use the whole alphabet 
-* to perform individual transitions directly over the closed set. 
+/** This function allows us to perfom "post" and use the whole alphabet
+* to perform individual transitions directly over the closed set.
 * The output will be represented as a ClosedSet to omit the neccessity to
-* explicitly return all the proper nodes. We will perform a transition 
+* explicitly return all the proper nodes. We will perform a transition
 * for each node of the antichain of the given set
 * of nodes and then we perform an union over these subresults.
 * The result is always an upward closed set!
 * @param nodes a set of sets of nodes used to perform a transition
 * @return closed set of nodes
 */
-StateClosedSet Afa::post(StateClosedSet closed_set) const 
+StateClosedSet Afa::post(const StateClosedSet& closed_set) const
 {
-	assert(closed_set.type() == Mata::upward_closed_set && "The predicate transformer " &&
+	assert(closed_set.type() == Mata::ClosedSetType::upward_closed_set && "The predicate transformer " &&
 	" post can be computed only over upward-closed sets.");
 	return post(closed_set.antichain());
 };
 
 // The end of the definitions of the "post" functions
 
 //***************************************************
@@ -385,35 +380,35 @@
 * of inverse results according to the given source state and symbol.
 * Otherwise, it gives us an empty vector which means that the result does not exist.
 * @brief performs an inverse transition using a single state and symbol
 * @param src a source state
 * @param symb a symbol used to perform an inverse transition
 * @return a vector of the inverse results
 */
-std::vector<InverseResults> Afa::perform_inverse_trans(State src, Symbol symb) const
+std::vector<InverseResults> Afa::perform_inverse_trans(const State src, const Symbol symb) const
 {
-	for(auto element : this->inverseTransRelation[src])
+	for(const auto& element : this->inverseTransRelation[src])
 	{
 		if(element.symb == symb)
 		{
 		    return element.inverseResults;
 		}
 	}
-	return std::vector<InverseResults>();
+	return {};
 }  // perform_inverse_trans }}}
 
 /** This function inspects an inverse transition relation and returns a vector
 * of inverse results according to the given source states and symbol.
 * Otherwise, it gives us an empty vector which means that the result does not exist.
 * @brief performs an inverse transition using a single state and symbol
 * @param node source states
 * @param symb a symbol used to perform an inverse transition
 * @return a vector of the inverse results
 */
-std::vector<InverseResults> Afa::perform_inverse_trans(Node node, Symbol symb) const
+std::vector<InverseResults> Afa::perform_inverse_trans(const Node& node, Symbol symb) const
 {
 	std::vector<InverseResults> result{};
 	for(auto state : node)
 	{
 		auto subresult = perform_inverse_trans(state, symb);
 		result.insert(result.end(), subresult.begin(), subresult.end());
 	}
@@ -425,143 +420,139 @@
 * The output will be represented as ClosedSet to omit the neccessity
 * to explicitly return all the proper nodes.
 * The result is always a downward closed set!
 * @param node source nodes
 * @param symb a symbol used to perform an inverse transition
 * @return closed set of nodes
 */
-StateClosedSet Afa::pre(Node node, Symbol symb) const
+StateClosedSet Afa::pre(const Node& node, Symbol symb) const
 {
 	std::vector<InverseResults> candidates = perform_inverse_trans(node, symb);
 	Node result{};
-	for(auto candidate : candidates)
+	for(const auto& candidate : candidates)
 	{
 		if(candidate.precondition.IsSubsetOf(node))
 		{
 			for(auto el : candidate.result_node)
 			{
 				result.insert(el);
 			}
 		}
 	}
-	return StateClosedSet(downward_closed_set, 0, transitionrelation.size()-1, result);
+	return { ClosedSetType::downward_closed_set, 0, transitionrelation.size()-1, result };
 } // pre }}}
 
 /** This function takes a set of nodes and a symbol and returns all the nodes
 * which are able to access the given nodes in one step using the given symbol.
 * The output will be represented as ClosedSet to omit the neccessity
 * to explicitly return all the proper nodes. The result is always a downward closed set!
 * @param nodes source nodes
 * @param symb a symbol used to perform an inverse transition
 * @return closed set of nodes
 */
-StateClosedSet Afa::pre(Nodes nodes, Symbol symb) const
+StateClosedSet Afa::pre(const Nodes& nodes, Symbol symb) const
 {
-	StateClosedSet result(downward_closed_set, 0, transitionrelation.size()-1);
-	for(auto node : nodes)
+	StateClosedSet result(ClosedSetType::downward_closed_set, 0, transitionrelation.size()-1);
+	for(const auto& node : nodes)
 	{
 		result = result.Union(pre(node, symb));
 	}
 	return result;
 } // pre }}}
 
 /** This function performs 'pre' directly over the given closed set
 * and the given symbol. The result is always a downward closed set!
 * @param closed_set a closed set
 * @param symb a symbol used to perform an inverse transition
 * @return closed set of nodes
 */
-StateClosedSet Afa::pre(StateClosedSet closed_set, Symbol symb) const
+StateClosedSet Afa::pre(const StateClosedSet& closed_set, const Symbol symb) const
 {
-	assert(closed_set.type() == downward_closed_set && "The predicate transformer " &&
+	assert(closed_set.type() == ClosedSetType::downward_closed_set && "The predicate transformer " &&
 	"pre can be computed only over downward-closed sets.");
 	return pre(closed_set.antichain(), symb);
 } // pre }}}
 
 /** This function allows us to perfom pre over a node and use the whole
-* alphabet to perform individual transitions. The result is always 
+* alphabet to perform individual transitions. The result is always
 * a downward closed set!
 * @param node a set of states
 * @return closed set of nodes
 */
-StateClosedSet Afa::pre(Node node) const
+StateClosedSet Afa::pre(const Node& node) const
 {
 	if(node.empty())
 	{
-		return StateClosedSet(downward_closed_set, 0, transitionrelation.size()-1, Nodes{Node{}});
+		return StateClosedSet(ClosedSetType::downward_closed_set, 0, transitionrelation.size()-1, Nodes{Node{}});
 	}
-	StateClosedSet result(downward_closed_set, 0, transitionrelation.size()-1);
+	StateClosedSet result(ClosedSetType::downward_closed_set, 0, transitionrelation.size()-1);
 
 	// It is sufficient to access the first element of the node
 	// to collect all required symbols of the alphabet. If there is another symbol used
 	// in context of another state of the node, it won't affect the result. The result for
 	// such symbol will be empty since it is not used in context of all states
 	// stored in the node
-	for(auto transVec : inverseTransRelation[*(node.begin())])
+	for(const auto& transVec : inverseTransRelation[*(node.begin())])
 	{
 		result.insert(pre(node, transVec.symb).antichain());
 	}
 	return result;
 } // pre }}}
 
 /** This function allows us to perfom pre over a set of nodes and use
-* the whole alphabet to perform individual transitions 
+* the whole alphabet to perform individual transitions
 * The result is always a downward closed set!
 * @param nodes a set of sets of states
 * @return closed set of nodes
 */
-StateClosedSet Afa::pre(Nodes nodes) const
-{
-	StateClosedSet result(downward_closed_set, 0, transitionrelation.size()-1);
-	for(auto node : nodes)
-	{
-		result.insert(pre(node).antichain());
-	}
+StateClosedSet Afa::pre(const Nodes& nodes) const {
+	StateClosedSet result{ ClosedSetType::downward_closed_set, 0, transitionrelation.size() - 1 };
+	for(const auto& node : nodes) { result.insert(pre(node).antichain()); }
 	return result;
 } // pre }}}
 
 // The end of the definitions of the "pre" functions
 ////////////////////////////////////////////////////
 
 bool Afa::has_trans(const Trans& trans) const
 { // {{{
 	Nodes res = get_trans_from_state(trans.src, trans.symb).dst;
-	if(res.size() && res.IsSubsetOf(trans.dst))
+	if(!res.empty() && res.IsSubsetOf(trans.dst))
 	{
 		return true;
 	}
 	return false;
 } // has_trans }}}
 
 
 size_t Afa::trans_size() const
 { // {{{
 	size_t result = 0;
-	for(auto state : transitionrelation)
+	for(const auto& state : transitionrelation)
 	{
 		result += state.size();
 	}
 	return result;
 } // trans_size() }}}
 
 StateClosedSet Afa::get_non_final_nodes() const {
-	StateClosedSet result(upward_closed_set, 0, transitionrelation.size()-1);
+	StateClosedSet result(ClosedSetType::upward_closed_set, 0, transitionrelation.size()-1);
 	auto transSize = transitionrelation.size();
 	for(State state = 0; state < transSize; ++state)
 	{
 		if(!has_final(state))
 		{
 			result.insert(state);
 		}
 	}
 	return result;
 }
 
 StateClosedSet Afa::get_initial_nodes() const {
-    StateClosedSet result = StateClosedSet(upward_closed_set, 0, transitionrelation.size()-1);
+    StateClosedSet result = StateClosedSet(ClosedSetType::upward_closed_set, 0, transitionrelation.size()-1);
     for(const auto& node : initialstates)
     {
         result.insert(node);
     }
     return result;
 }
 
@@ -575,123 +566,127 @@
 bool Mata::Afa::are_state_disjoint(const Afa& lhs, const Afa& rhs)
 { // {{{
   assert(&lhs);
   assert(&rhs);
 
   // TODO
   assert(false);
+  return {};
 } // are_disjoint }}}
 
 
 void Mata::Afa::union_norename(
 	Afa*        result,
 	const Afa&  lhs,
 	const Afa&  rhs)
 { // {{{
-	assert(nullptr != result);
+    assert(nullptr != result);
 
-  assert(&lhs);
-  assert(&rhs);
+    assert(&lhs);
+    assert(&rhs);
 
-  // TODO
-  assert(false);
+    // TODO
+    assert(false);
 } // union_norename }}}
 
 
 Afa Mata::Afa::union_rename(
 	const Afa&  lhs,
 	const Afa&  rhs)
 { // {{{
   assert(&lhs);
   assert(&rhs);
 
   // TODO
   assert(false);
+  return {};
 } // union_rename }}}
 
 
 bool Mata::Afa::is_lang_empty(const Afa& aut, Path* cex)
 { // {{{
   assert(&aut);
   assert(&cex);
 
   // TODO
   assert(false);
+  return {};
 } // is_lang_empty }}}
 
 
 bool Mata::Afa::is_lang_empty_cex(const Afa& aut, Word* cex)
 { // {{{
 	assert(nullptr != cex);
 
   assert(&aut);
   assert(&cex);
 
   // TODO
   assert(false);
+  return {};
 } // is_lang_empty_cex }}}
 
-/** This function decides whether the given automaton is empty using 
+/** This function decides whether the given automaton is empty using
 * an antichain-based emptiness test working in the concrete domain
 * in the forward fashion
 * @param aut a given automaton
 * @return true iff the automaton is empty
 */
 bool Mata::Afa::antichain_concrete_forward_emptiness_test_old(const Afa& aut)
 {
     // We will iteratively build a set of reachable nodes (next) until
 	// we reach a fixed point or until we find out that there exists
 	// a final node which is reachable (is not part of goal).
     // We will perform each operation directly over antichains.
     // Note that the fixed point always exists so the while loop always terminates.
     StateClosedSet goal = aut.get_non_final_nodes();
-    StateClosedSet current = StateClosedSet(upward_closed_set, 0, aut.get_num_of_states()-1);
+    StateClosedSet current = StateClosedSet(ClosedSetType::upward_closed_set, 0, aut.get_num_of_states()-1);
     StateClosedSet next = aut.get_initial_nodes();
 
     while(current != next)
     {
 		current = next;
 		next = current.Union(aut.post(current));
 		if(!(next <= goal)) // inclusion test
 		{
 		    return false;
 		}
     }
     return true;
 }
 
-/** This function decides whether the given automaton is empty using 
+/** This function decides whether the given automaton is empty using
 * an antichain-based emptiness test working in the concrete domain
 * in the forward fashion
 * @param aut a given automaton
 * @return true iff the automaton is empty
 */
 bool Mata::Afa::antichain_concrete_forward_emptiness_test_new(const Afa& aut)
 {
 	StateClosedSet goal = aut.get_non_final_nodes();
 	StateClosedSet result = aut.get_initial_nodes();
 	std::set<Node> processed = std::set<Node>();
 	std::vector<Node> worklist = std::vector<Node>();
-	for(Node node : aut.get_initial_nodes().antichain())
+	for(const Node& node : aut.get_initial_nodes().antichain())
 	{
 		worklist.push_back(node);
 	}
 
 	if(!(result <= goal))
 	{
 		return false;
 	}
 
-	while(!worklist.empty()) 
+	while(!worklist.empty())
 	{
 		Node current = worklist.back();
 		worklist.pop_back();
 		auto post_current = aut.post(current);
 		result = result.Union(post_current);
-		for(Node node : post_current.antichain())
+		for(const Node& node : post_current.antichain())
 		{
 			if(!goal.contains(node))
 			{
 			    return false;
 			}
 			if(!processed.count(node))
 			{
@@ -699,29 +694,29 @@
 			}
 		}
 		processed.insert(current);
 	}
 	return true;
 }
 
-/** This function decides whether the given automaton is empty using 
+/** This function decides whether the given automaton is empty using
 * an antichain-based emptiness test working in the concrete domain
 * in the backward fashion
 * @param aut a given automaton
 * @return true iff the automaton is empty
 */
 bool Mata::Afa::antichain_concrete_backward_emptiness_test_old(const Afa& aut)
 {
 	// We will iteratively build a set of terminating nodes (next)
 	// until we reach a fixed point or until we find out that there exists
 	// an initial node which is terminating (is not part of goal).
 	// We will perform each operation directly over antichains
 	// Note that the fixed point always exists so the while loop always terminates
 	StateClosedSet goal = aut.get_non_initial_nodes();
-	StateClosedSet current = StateClosedSet(downward_closed_set, 0, aut.get_num_of_states()-1);
+	StateClosedSet current = StateClosedSet(ClosedSetType::downward_closed_set, 0, aut.get_num_of_states()-1);
 	StateClosedSet next = aut.get_final_nodes();
 
 	while(current != next)
 	{
 		current = next;
 		next = current.Union(aut.pre(current));
 		if(!(next <= goal))
@@ -729,43 +724,43 @@
 			return false;
 		}
 	}
 	return true;
 }
 
 
-/** This function decides whether the given automaton is empty using 
+/** This function decides whether the given automaton is empty using
 * an antichain-based emptiness test working in the concrete domain
 * in the backward fashion
 * @param aut a given automaton
 * @return true iff the automaton is empty
 */
 bool Mata::Afa::antichain_concrete_backward_emptiness_test_new(const Afa& aut)
 {
 	StateClosedSet goal = aut.get_non_initial_nodes();
 	StateClosedSet result = aut.get_final_nodes();
 	std::set<Node> processed = std::set<Node>();
 	std::vector<Node> worklist = std::vector<Node>();
-	for(Node node : aut.get_final_nodes().antichain())
+	for(const Node& node : aut.get_final_nodes().antichain())
 	{
 		worklist.push_back(node);
 	}
 
 	if(!(result <= goal))
 	{
 		return false;
 	}
 
-	while(!worklist.empty()) 
+	while(!worklist.empty())
 	{
 		Node current = worklist.back();
 		worklist.pop_back();
 		auto pre_current = aut.pre(current);
 		result = result.Union(pre_current);
-		for(Node node : pre_current.antichain())
+		for(const Node& node : pre_current.antichain())
 		{
 			if(!goal.contains(node))
 			{
 				return false;
 			}
 			if(!processed.count(node))
 			{
@@ -838,15 +833,15 @@
 		std::string init_res = "( ";
 		bool first = true;
 		for (State s : node) {
 			bool_str_pair bsp = state_namer(s);
 			if (!bsp.first) { throw std::runtime_error("cannot translate state " + std::to_string(s)); }
 			if(!first) {init_res += " & ";}
 			init_res += bsp.second;
-			first = false;		
+			first = false;
 		}
 		init_res += " )";
 		init_states.push_back(init_res);
 	}
 	parsec.dict["Initial"] = init_states;
 
 	// construct final states
@@ -951,30 +946,27 @@
 			State state = get_state_name(str);
 			aut.finalstates.insert(state);
 		}
 	}
 
 	for (const auto& body_line : parsec.body) {
 		if (body_line.size() < 2) {
-			// clean up
-      clean_up();
+            clean_up();
 
-      throw std::runtime_error("Invalid transition: " +
-        std::to_string(body_line));
+            throw std::runtime_error("Invalid transition: " + std::to_string(body_line));
 		}
 
-		State src_state = get_state_name(body_line[0]);
     std::string formula;
     for (size_t i = 1; i < body_line.size(); ++i) {
       formula += body_line[i] + " ";
     }
 
 	// TODO: Transform a positive Boolean formula from the string format
 	// to the inner representation (src state, symbol on transition, ordered
-	// vector of ordered vectors of states which corresponds to the formula in DNF) 
+	// vector of ordered vectors of states which corresponds to the formula in DNF)
 	// Call the "add_trans" and "add_inverse_trans" functions over the
 	// parsed formula to add it do the automaton
 
 	}
 
 	// do the dishes and take out garbage
 	clean_up();
@@ -1043,26 +1035,26 @@
         while (is_node_operator(init_graph->node, FormulaNode::OperatorType::OR))
         {  // Processes each clause separately
             assert(init_graph->children[1].node.is_operand() ||
                    is_node_operator(init_graph->children[1].node, FormulaNode::OperatorType::AND) ||
                    "Clause should be conjunction or single state");
             // Conjunction is the right son of initent node
             Node initial_node;
-            for (const auto s : init_graph->children[1].collect_node_names())
+            for (const auto& s : init_graph->children[1].collect_node_names())
                 initial_node.insert(get_state_name(s));
             aut.add_initial(initial_node);
 
             // jump to another clause which is the left son of initent node
             init_graph = &init_graph->children.front();
         }
         assert(init_graph->node.is_operand() ||
                is_node_operator(init_graph->node, FormulaNode::OperatorType::AND) ||
                        "Remaining clause should be conjunction or single element");
         Node initial_node;
-        for (const auto s : init_graph->collect_node_names())
+        for (const auto& s : init_graph->collect_node_names())
             initial_node.insert(get_state_name(s));
         aut.add_initial(initial_node);
     }
 
     for (const auto& trans : inter_aut.transitions)
     {
         State src_state = get_state_name(trans.first.name);
@@ -1164,14 +1156,15 @@
 bool Mata::Afa::is_complete(const Afa& aut, const Alphabet& alphabet)
 { // {{{
   assert(&aut);
   assert(&alphabet);
 
   // TODO
   assert(false);
+  return {};
 } // is_complete }}}
 
 bool Mata::Afa::accepts_epsilon(const Afa& aut) {
     return std::any_of(aut.initialstates.cbegin(), aut.initialstates.cend(),
         [&aut](const Node& node) { return node.IsSubsetOf(aut.finalstates); });
 }
```

### Comparing `libmata-0.68.0/mata/src/alphabet.cc` & `libmata-0.69.0/mata/src/alphabet.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/src/inter-aut.cc` & `libmata-0.69.0/mata/src/inter-aut.cc`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         else if (type == "chars")
             return Mata::IntermediateAut::Naming::CHARS;
         else if (type == "utf")
             return Mata::IntermediateAut::Naming::UTF;
 
         assert(false && "Unknown naming type - a naming type should be always defined correctly otherwise it is"
                         "impossible to parse automaton correctly");
+        return {};
     }
 
     Mata::IntermediateAut::AlphabetType get_alphabet_type(const std::string &type)
     {
         assert(type.find('-') != std::string::npos);
         const std::string& alph_type = type.substr(type.find('-')+1, std::string::npos);
 
@@ -64,14 +65,15 @@
             return Mata::IntermediateAut::AlphabetType::EXPLICIT;
         } else if (alph_type == "intervals") {
             return Mata::IntermediateAut::AlphabetType::INTERVALS;
         }
 
         assert(false && "Unknown alphabet type - an alphabet type should be always defined correctly otherwise it is"
                         "impossible to parse automaton correctly");
+        return {};
     }
 
     bool is_naming_marker(const Mata::IntermediateAut::Naming naming)
     {
         return naming == Mata::IntermediateAut::Naming::MARKED;
     }
 
@@ -222,39 +224,42 @@
                     while (!opstack.back().is_leftpar()) {
                         output.push_back(opstack.back());
                         opstack.pop_back();
                     }
                     opstack.pop_back();
                     break;
                 case Mata::FormulaNode::Type::OPERATOR:
-                    for (int j = opstack.size()-1; j >= 0; --j) {
-                        assert(!opstack[j].is_operand());
-                        if (opstack[j].is_leftpar())
+                    for (int j = static_cast<int>(opstack.size())-1; j >= 0; --j) {
+                        size_t j_size_t{ static_cast<size_t>(j) };
+                        assert(!opstack[j_size_t].is_operand());
+                        if (opstack[j_size_t].is_leftpar())
                             break;
-                        if (lower_precedence(node.operator_type, opstack[j].operator_type)) {
-                            output.push_back(opstack[j]);
+                        if (lower_precedence(node.operator_type, opstack[j_size_t].operator_type)) {
+                            output.push_back(opstack[j_size_t]);
                             opstack.erase(opstack.begin()+j);
                         }
                     }
                     opstack.push_back(node);
                     break;
                 default: assert(false);
             }
         }
 
         while (!opstack.empty()) {
             output.push_back(opstack.back());
             opstack.pop_back();
         }
 
+        #ifndef NDEBUG
         for (const auto& node : output) {
             assert(node.is_operator() || (node.name != "!" && node.name != "&" && node.name != "|"));
             assert(node.is_leftpar() || node.name != "(");
             assert(node.is_rightpar() || node.name != ")");
         }
+        #endif // #ifndef NDEBUG.
 
         return output;
     }
 
     /**
      * Create a graph for a postfix representation of transition formula
      * @param postfix A postfix representation of transition formula
@@ -414,15 +419,15 @@
             const FormulaGraph *gr = stack.back();
             stack.pop_back();
             if (gr->node.is_operator() && gr->node.operator_type == FormulaNode::OperatorType::OR)
                 trans_disjuncts++;
             for (const auto &ch: gr->children)
                 stack.push_back(&ch);
         }
-        res += std::max(trans_disjuncts, (size_t) 1);
+        res += std::max(trans_disjuncts, 1ul);
     }
 
     return res;
 }
 
 /**
  * Parses a transition by firstly transforming transition formula to postfix form and then creating
@@ -455,30 +460,32 @@
             assert(false && "Unknown NFA type");
 
         postfix.push_back(Mata::FormulaNode(
                 Mata::FormulaNode::Type::OPERATOR, "&", "&", Mata::FormulaNode::OperatorType::AND));
     } else
         postfix = infix_to_postfix(aut, rhs);
 
+    #ifndef NDEBUG
     for (const auto& node : postfix) {
         assert(node.is_operator() || (node.name != "!" && node.name != "&" && node.name != "|"));
         assert(node.is_leftpar() || node.name != "(");
         assert(node.is_rightpar() || node.name != ")");
     }
+    #endif // #ifndef NDEBUG.
     const Mata::FormulaGraph graph = postfix_to_graph(postfix);
 
-    aut.transitions.push_back(std::pair<Mata::FormulaNode,Mata::FormulaGraph>(lhs, graph));
+    aut.transitions.emplace_back(lhs, graph);
 }
 
 std::unordered_set<std::string> Mata::FormulaGraph::collect_node_names() const
 {
     std::unordered_set<std::string> res;
     std::vector<const Mata::FormulaGraph *> stack;
 
-    stack.push_back(reinterpret_cast<const FormulaGraph *const>(&(this->node)));
+    stack.push_back(reinterpret_cast<const FormulaGraph*>(&(this->node)));
     while (!stack.empty()) {
         const FormulaGraph* g = stack.back();
         assert(g != nullptr);
         stack.pop_back();
 
         if (g->node.type == FormulaNode::Type::UNKNOWN)
            continue; // skip undefined nodes
```

### Comparing `libmata-0.68.0/mata/src/mintermization.cc` & `libmata-0.69.0/mata/src/mintermization.cc`

 * *Files 2% similar despite different names*

```diff
@@ -74,36 +74,36 @@
 void Mata::Mintermization::trans_to_bdd_afa(const IntermediateAut &aut)
 {
     assert(aut.is_afa());
 
     for (const auto& trans : aut.transitions) {
         lhs_to_disjuncts_and_states[&trans.first] = std::vector<DisjunctStatesPair>();
         if (trans.second.node.is_state()) { // node from state to state
-            lhs_to_disjuncts_and_states[&trans.first].push_back(DisjunctStatesPair(&trans.second, &trans.second));
+            lhs_to_disjuncts_and_states[&trans.first].emplace_back(&trans.second, &trans.second);
         }
         // split transition to disjuncts
         const FormulaGraph *act_graph = &trans.second;
 
         if (!trans.second.node.is_state() && act_graph->node.is_operator() && act_graph->node.operator_type != FormulaNode::OperatorType::OR) // there are no disjuncts
-            lhs_to_disjuncts_and_states[&trans.first].push_back(DisjunctStatesPair(act_graph, detect_state_part(
-                    act_graph)));
+            lhs_to_disjuncts_and_states[&trans.first].emplace_back(act_graph, detect_state_part(
+                    act_graph));
         else if (!trans.second.node.is_state()) {
             while (act_graph->node.is_operator() && act_graph->node.operator_type == FormulaNode::OperatorType::OR) {
                 // map lhs to disjunct and its state formula. The content of disjunct is right son of actual graph
                 // since the left one is a rest of formula
-                lhs_to_disjuncts_and_states[&trans.first].push_back(DisjunctStatesPair(&act_graph->children[1],
+                lhs_to_disjuncts_and_states[&trans.first].emplace_back(&act_graph->children[1],
                                                                                        detect_state_part(
-                                                                                           &act_graph->children[1])));
+                                                                                           &act_graph->children[1]));
                 act_graph = &(act_graph->children.front());
             }
 
             // take care of last disjunct
-            lhs_to_disjuncts_and_states[&trans.first].push_back(DisjunctStatesPair(act_graph,
+            lhs_to_disjuncts_and_states[&trans.first].emplace_back(act_graph,
                                                                                    detect_state_part(
-                                                                                           act_graph)));
+                                                                                           act_graph));
         }
 
         // Foreach disjunct create a BDD
         for (const DisjunctStatesPair& ds_pair : lhs_to_disjuncts_and_states[&trans.first]) {
             // create bdd for the whole disjunct
             const auto bdd = (ds_pair.first == ds_pair.second) ? // disjunct contains only states
                     OptionalBdd(bdd_mng.bddOne()) : // transition from state to states -> add true as symbol
@@ -113,18 +113,18 @@
                 continue;
             trans_to_bddvar[ds_pair.first] = bdd.val;
             bdds.insert(bdd.val);
         }
     }
 }
 
-std::unordered_set<BDD> Mata::Mintermization::compute_minterms(const std::unordered_set<BDD>& bdds)
+std::unordered_set<BDD> Mata::Mintermization::compute_minterms(const std::unordered_set<BDD>& source_bdds)
 {
     std::unordered_set<BDD> stack{ bdd_mng.bddOne() };
-    for (BDD b : bdds) {
+    for (const BDD& b: source_bdds) {
         std::unordered_set<BDD> next;
         /**
          * TODO: Possible optimization - we can remember which transition belongs to the currently processed bdds
          * and mintermize automaton somehow directly here. However, it would be better to do such optimization
          * in copy of this function and this one keep clean and straightforward.
          */
         for (const auto& minterm : stack) {
@@ -139,15 +139,15 @@
         }
         stack = next;
     }
 
     return stack;
 }
 
-const Mata::Mintermization::OptionalBdd Mata::Mintermization::graph_to_bdd_afa(const FormulaGraph &graph)
+Mata::Mintermization::OptionalBdd Mata::Mintermization::graph_to_bdd_afa(const FormulaGraph &graph)
 {
     const FormulaNode& node = graph.node;
 
     if (node.is_operand()) {
         if (node.is_state())
             return OptionalBdd(OptionalBdd::TYPE::NOTHING_E);
         if (symbol_to_bddvar.count(node.name)) {
@@ -174,17 +174,18 @@
             const OptionalBdd op1 = graph_to_bdd_afa(graph.children[0]);
             return !op1;
         } else
             assert(false && "Unknown type of operation. It should conjunction, disjunction, or negation.");
     }
 
     assert(false);
+    return {};
 }
 
-const BDD Mata::Mintermization::graph_to_bdd_nfa(const FormulaGraph &graph)
+BDD Mata::Mintermization::graph_to_bdd_nfa(const FormulaGraph &graph)
 {
     const FormulaNode& node = graph.node;
 
     if (node.is_operand()) {
         if (symbol_to_bddvar.count(node.name)) {
             return symbol_to_bddvar.at(node.name);
         } else {
@@ -209,14 +210,15 @@
             const BDD op1 = graph_to_bdd_nfa(graph.children[0]);
             return !op1;
         } else
             assert(false);
     }
 
     assert(false);
+    return {};
 }
 
 void Mata::Mintermization::minterms_to_aut_nfa(Mata::IntermediateAut& res, const Mata::IntermediateAut& aut,
                                            const std::unordered_set<BDD>& minterms)
 {
     for (const auto& trans : aut.transitions) {
             // for each t=(q1,s,q2)
```

### Comparing `libmata-0.68.0/mata/src/nfa/nfa-complement.cc` & `libmata-0.69.0/mata/src/nfa/nfa-complement.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/src/nfa/nfa-concatenation.cc` & `libmata-0.69.0/mata/src/nfa/nfa-concatenation.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/src/nfa/nfa-inclusion.cc` & `libmata-0.69.0/mata/src/nfa/nfa-inclusion.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/src/nfa/nfa-intersection.cc` & `libmata-0.69.0/mata/src/nfa/nfa-intersection.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/src/nfa/nfa-universal.cc` & `libmata-0.69.0/mata/src/nfa/nfa-universal.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/src/nfa/nfa.cc` & `libmata-0.69.0/mata/src/nfa/nfa.cc`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
 #include <algorithm>
 #include <list>
 #include <unordered_set>
+#include <iterator>
 
 // MATA headers
 #include <mata/nfa.hh>
 #include <mata/nfa-algorithms.hh>
 #include <mata/simlib/explicit_lts.hh>
 
 using std::tie;
@@ -30,14 +31,19 @@
 using namespace Mata::Nfa;
 using Mata::Symbol;
 
 using StateBoolArray = std::vector<bool>; ///< Bool array for states in the automaton.
 
 const std::string Mata::Nfa::TYPE_NFA = "NFA";
 
+const State Limits::min_state;
+const State Limits::max_state;
+const Symbol Limits::min_symbol;
+const Symbol Limits::max_symbol;
+
 namespace {
     Simlib::Util::BinaryRelation compute_fw_direct_simulation(const Nfa& aut) {
         Symbol maxSymbol = 0;
         const size_t state_num = aut.size();
         Simlib::ExplicitLTS LTSforSimulation(state_num);
 
         for (const auto& transition : aut.delta) {
@@ -374,15 +380,15 @@
 
 bool Delta::empty() const
 {
     return this->begin() == this->end();
 }
 
 Delta::const_iterator::const_iterator(const std::vector<Post>& post_p, bool ise) :
-    post(post_p), current_state(0), is_end(ise)
+    post(post_p), current_state(0), is_end{ ise }
 {
     const size_t post_size = post.size();
     for (size_t i = 0; i < post_size; ++i) {
         if (!post[i].empty()) {
             current_state = i;
             post_iterator = post[i].begin();
             targets_position = post_iterator->targets.begin();
@@ -434,21 +440,22 @@
     this->current_state = x.current_state;
     this->is_end = x.is_end;
 
     return *this;
 }
 
 bool Mata::Nfa::operator==(const Delta::const_iterator& a, const Delta::const_iterator& b) {
-    if (a.is_end && b.is_end)
+    if (a.is_end && b.is_end) {
         return true;
-    else if ((a.is_end && !b.is_end) || (!a.is_end && b.is_end))
+    } else if ((a.is_end && !b.is_end) || (!a.is_end && b.is_end)) {
         return false;
-    else
+    } else {
         return a.current_state == b.current_state && a.post_iterator == b.post_iterator
                && a.targets_position == b.targets_position;
+    }
 }
 
 State Delta::find_max_state() {
     size_t max = 0;
     State src = 0;
     for (Post & p: posts) {
         if (src > max)
@@ -473,15 +480,15 @@
     return posts[q];
 }
 
 std::vector<State> Delta::defragment(NumberPredicate<State>& is_staying) {
     //first, indexes of post are filtered (places of to be removed states are taken by states on their right)
     size_t move_index{ 0 };
     posts.erase(
-            std::remove_if(posts.begin(), posts.end(), [&](Post& _post) -> bool {
+            std::remove_if(posts.begin(), posts.end(), [&](Post&) -> bool {
                 size_t prev{ move_index };
                 ++move_index;
                 return !is_staying[prev];
             }),
             posts.end()
     );
 
@@ -622,30 +629,26 @@
 
 // A data structure to store things in the depth first search within dfs in the trim.
 // It stores a state and the state of the iteration through the successors of the state.
 struct StackLevel {
     State state;
     Post::const_iterator post_it;
     Post::const_iterator post_end;
-    StateSet::const_iterator targets_it;
-    StateSet::const_iterator targets_end;
+    StateSet::const_iterator targets_it{};
+    StateSet::const_iterator targets_end{};
 
-    StackLevel(State q, const Delta & delta):
-            state(q),
-            post_it(delta[q].cbegin()),
-            post_end(delta[q].cend())
-    {
+    StackLevel(State q, const Delta & delta) : state(q), post_it(delta[q].cbegin()), post_end(delta[q].cend()) {
         if (post_it != post_end) {
             targets_it = post_it->cbegin();
             targets_end = post_it->cend();
         }
     };
 };
 
-const NumberPredicate<State> Nfa::get_useful_states() const
+NumberPredicate<State> Nfa::get_useful_states() const
 {
 #ifdef _STATIC_STRUCTURES_
     // STATIC SEEMS TO GIVE LIKE 5-10% SPEEDUP
     static std::vector<StackLevel> stack;
     //tracking elements seems to cost more than it saves, switching it off
     static NumberPredicate<State> reached(false);
     static NumberPredicate<State> reached_and_reaching(false);
@@ -952,27 +955,27 @@
 
     //Now make the delta of the reversed automaton.
     //Important: since sources are ordered, when adding them as targets, we can just push them back.
     result.delta.reserve(num_of_states);
 
     // adding non-e transitions
     for (const Symbol symbol: symbols) {
-        for (int i = 0; i<sources[symbol].size(); ++i) {
+        for (size_t i{ 0 }; i < sources[symbol].size(); ++i) {
             State tgt_state =sources[symbol][i];
             State src_state =targets[symbol][i];
             Post & src_post = result.delta.get_mutable_post(src_state);
             if (src_post.empty() || src_post.back().symbol != symbol) {
                 src_post.push_back(Move(symbol));
             }
             src_post.back().push_back(tgt_state);
         }
     }
 
     // adding e-transitions
-    for (int i = 0; i<e_sources.size(); ++i) {
+    for (size_t i{ 0 }; i < e_sources.size(); ++i) {
         State tgt_state =e_sources[i];
         State src_state =e_targets[i];
         Post & src_post = result.delta.get_mutable_post(src_state);
         if (src_post.empty() || src_post.back().symbol != EPSILON) {
             src_post.push_back(Move(EPSILON));
         }
         src_post.back().push_back(tgt_state);
@@ -1034,15 +1037,15 @@
                     //move->insert(sourceState);
             }
         }
     }
 
     //sorting the targets
     for (State q = 0, states_num = result.delta.num_of_states(); q < states_num; ++q) {
-        Post & post = result.delta.get_mutable_post(q);
+        //Post & post = result.delta.get_mutable_post(q);
         //Util::sort_and_rmdupl(post);
         for (auto m = result.delta.get_mutable_post(q).begin(); m != result.delta.get_mutable_post(q).end(); ++m) {
             sort_and_rmdupl(m->targets);
         }
     }
 
     return result;
@@ -1179,16 +1182,19 @@
     return !are_disjoint(cur, aut.final);
 }
 
 /// serializes Nfa into a ParsedSection
 Mata::Parser::ParsedSection Mata::Nfa::serialize(
         const Nfa&                aut,
         const SymbolToStringMap*  symbol_map,
-        const StateToStringMap*   state_map)
-{assert(false);}
+        const StateToStringMap*   state_map) {
+    (void)aut; (void)symbol_map; (void)state_map;
+    assert(false && "Unimplemented.");
+    return {};
+}
 
 bool Mata::Nfa::is_lang_empty(const Nfa& aut, Run* cex)
 { // {{{
     std::list<State> worklist(
             aut.initial.begin(), aut.initial.end());
     std::unordered_set<State> processed(
             aut.initial.begin(), aut.initial.end());
@@ -1330,34 +1336,21 @@
 {
     TransSequence trans_sequence{};
 
     for (const auto& transition_from_state: delta[state_from])
     {
         for (State state_to: transition_from_state.targets)
         {
-            trans_sequence.push_back(Trans{ state_from, transition_from_state.symbol, state_to });
+            trans_sequence.emplace_back(state_from, transition_from_state.symbol, state_to);
         }
     }
 
     return trans_sequence;
 }
 
-
-size_t Nfa::get_num_of_trans() const
-{
-    size_t num_of_transitions{};
-
-    for (const auto& state_transitions: delta)
-    {
-        ++num_of_transitions;
-    }
-
-    return num_of_transitions;
-}
-
 Nfa Nfa::get_one_letter_aut(Symbol abstract_symbol) const {
     Nfa digraph{size(), StateSet(initial), StateSet(final) };
     collect_directed_transitions(*this, abstract_symbol, digraph);
     return digraph;
 }
 
 void Nfa::get_one_letter_aut(Nfa& result) const {
@@ -1872,21 +1865,22 @@
     if (nfa.alphabet != nullptr) {
         os << "|alphabet: " << *(nfa.alphabet);
     }
     // TODO: If the default implementation for state_dict is implemented, consider printing the state dictionary with
     //  std::to_string(<state_dict_object>);
 
     os << " }";
+    return os;
 }
 
 // Other versions, maybe an interesting experiment with speed of data structures.
-// returns symbols appearing in Delta, pushes back to vector and then sorts
+// Returns symbols appearing in Delta, pushes back to vector and then sorts
 Mata::Util::OrdVector<Symbol> Nfa::get_used_symbols_vec() const {
 #ifdef _STATIC_STRUCTURES_
-    static std::vector<Symbol>  symbols{};
+    static std::vector<Symbol> symbols{};
     symbols.clear();
 #else
     std::vector<Symbol>  symbols{};
 #endif
     for (State q = 0; q< delta.num_of_states(); ++q) {
         const Post & post = delta[q];
         for (const Move & move: post) {
@@ -1931,15 +1925,15 @@
     //symbols.dont_track_elements();
     for (State q = 0; q< delta.num_of_states(); ++q) {
         const Post & post = delta[q];
         for (const Move & move: post) {
             symbols.add(move.symbol);
         }
     }
-    //TODO: is it neccessary toreturn ordered vector? Would the number predicate suffice?
+    //TODO: is it necessary to return ordered vector? Would the number predicate suffice?
     return symbols;
 }
 
 // returns symbols appearing in Delta, adds to NumberPredicate,
 // Seems to be the fastest option, but could have problems with large maximum symbols
 std::vector<bool> Nfa::get_used_symbols_bv() const {
 #ifdef _STATIC_STRUCTURES_
@@ -1973,16 +1967,16 @@
     }
     return max;
 }
 
  void Nfa::unify_initial() {
     if (initial.empty() || initial.size() == 1) { return; }
     const State new_initial_state{add_state() };
-    for (const auto& orig_initial_state: initial) {
-        const auto moves{ get_moves_from(orig_initial_state) };
+    for (const State orig_initial_state: initial) {
+        const Post& moves{ get_moves_from(orig_initial_state) };
         for (const auto& transitions: moves) {
             for (const State state_to: transitions.targets) {
                 delta.add(new_initial_state, transitions.symbol, state_to);
             }
         }
         if (final[orig_initial_state]) { final.add(new_initial_state); }
     }
@@ -2001,17 +1995,18 @@
         if (initial[orig_final_state]) { initial.add(new_final_state); }
     }
     final.clear();
     final.add(new_final_state);
 }
 
 void Mata::Nfa::fill_alphabet(const Mata::Nfa::Nfa& nfa, OnTheFlyAlphabet& alphabet) {
-    size_t nfa_num_of_states{nfa.size() };
+    const size_t nfa_num_of_states{ nfa.size() };
     for (Mata::Nfa::State state{ 0 }; state < nfa_num_of_states; ++state) {
-        for (const auto state_transitions: nfa.delta) {
+        // TODO: Rewrite to not create 'Trans' instances and iterate over same symbols all the time.
+        for (const Trans& state_transitions: nfa.delta) {
             alphabet.update_next_symbol_value(state_transitions.symb);
             alphabet.try_add_new_symbol(std::to_string(state_transitions.symb), state_transitions.symb);
         }
     }
 }
 
 void Nfa::add_symbols_to(OnTheFlyAlphabet& alphabet) const {
@@ -2041,15 +2036,15 @@
     for (size_t i = 0; i < delta_size; ++i) {
         delta.get_mutable_post(i) = Post();
     }
 }
 
 State Nfa::add_state() {
     const size_t num_of_states{ size() };
-    delta.increase_size(num_of_states + 1 );
+    delta.increase_size(num_of_states + 1);
     return num_of_states;
 }
 
 State Nfa::add_state(State state) {
     if (state >= delta.num_of_states()) {
         delta.increase_size(state + 1);
     }
@@ -2188,12 +2183,12 @@
 
 void Move::insert(State s) {
     if (targets.find(s) == targets.end()) {
         targets.insert(s);
     }
 }
 
-void Move::insert(StateSet states) {
+void Move::insert(const StateSet& states) {
     for (State s : states) {
         insert(s);
     }
 }
```

### Comparing `libmata-0.68.0/mata/src/parser.cc` & `libmata-0.69.0/mata/src/parser.cc`

 * *Files 2% similar despite different names*

```diff
@@ -87,45 +87,44 @@
 				if (std::isspace(ch)) { /* do nothing */ }
 				else if ('"' == ch) {
 					state = TokenizerState::QUOTED;
 					*quoted = true;
 				} else if ('#' == ch) { // clear the rest of the line
 					std::string aux;
 					std::getline(input, aux);
-					return std::string();
+					return {};
 				} else if ('(' == ch || ')' == ch) {
 					return std::to_string(static_cast<char>(ch));
 				} else {
-					result += ch;
+					result += static_cast<char>(ch);
 					state = TokenizerState::UNQUOTED;
 				}
 				break;
 			}
 			case TokenizerState::UNQUOTED: {
 				if (std::isspace(ch)) { return result; }
 				else if ('#' == ch) { // clear the rest of the line
 					std::string aux;
 					std::getline(input, aux);
 					return result;
 				} else if ('"' == ch) {
 					std::string context;
 					std::getline(input, context);
-					throw std::runtime_error("misplaced quotes: " + result + "_\"_" +
-						context);
+					throw std::runtime_error("misplaced quotes: " + result + "_\"_" + context);
 				} else if ('(' == ch || ')' == ch) {
 					input.unget();
 					return result;
 				} else if ('@' == ch || '%' == ch) {
 					std::string context;
 					std::getline(input, context);
 					throw std::runtime_error(std::to_string("misplaced character \'") +
 						static_cast<char>(ch) + "\' in string \"" + result +
 						static_cast<char>(ch) + context + "\"");
 				} else {
-					result += ch;
+					result += static_cast<char>(ch);
 				}
 				break;
 			}
 			case TokenizerState::QUOTED: {
 				if ('"' == ch) {
 					ch = input.peek();
 					if (!std::isspace(ch) && ('#' != ch) && (')' != ch) &&
@@ -136,20 +135,20 @@
 						throw std::runtime_error("misplaced quotes: \"" + result + "_\"_" +
 							context);
 					}
 
 					return result;
 				} else if ('\\' == ch) {
 					state = TokenizerState::QUOTED_ESCAPE;
-				} else { result += ch; }
+				} else { result += static_cast<char>(ch); }
 				break;
 			}
 			case TokenizerState::QUOTED_ESCAPE: {
 				if ('"' != ch) { result += '\\'; }
-				result += ch;
+				result += static_cast<char>(ch);
 				state = TokenizerState::QUOTED;
 				break;
 			}
 			default: { // LCOV_EXCL_START
 				throw std::runtime_error("Invalid tokenizer state");
 			} // LCOV_EXCL_STOP
 		}
@@ -175,15 +174,15 @@
 	bool first = true;
 	while (stream.good())
 	{
 		bool quoted;
 		std::string token = get_token_from_line(stream, &quoted);
 		if (!quoted && token.empty()) { break; }
 
-		result.push_back({ token, quoted });
+		result.emplace_back(token, quoted);
 
 		if (!first && !quoted)
 		{
 			assert(!token.empty());
 			if ('@' == token[0])
 			{
 				throw std::runtime_error("invalid position of @TYPE: " + line);
@@ -196,15 +195,15 @@
 
 		first = false;
 	}
 
 	return result;
 } // tokenize_line(string) }}}
 
-std::vector<std::pair<std::string, bool>> split_tokens(std::vector<std::pair<std::string, bool>> tokens)
+std::vector<std::pair<std::string, bool>> split_tokens(const std::vector<std::pair<std::string, bool>>& tokens)
 { // {{{
     std::vector<std::pair<std::string, bool>> result;
     for (const auto& token : tokens) {
         if (token.second) { // is quoted?
             result.push_back(token);
             continue;
         }
@@ -214,27 +213,25 @@
         const size_t size = token_string.size();
         for (size_t i = 0; i < size; ++i) {
             if (is_logical_operator(token_string[i])) {
                 const std::string token_candidate = token_string.substr(last_operator, i - last_operator);
 
                 // there is token before logical operator (this is case of binary operators, e.g., a&b)
                 if (!token_candidate.empty())
-                    result.push_back(std::make_pair(token_candidate, false));
-                result.push_back(std::make_pair(std::string(1,token_string[i]), false));
+                    result.emplace_back(token_candidate, false);
+                result.emplace_back(std::string(1,token_string[i]), false);
                 last_operator = i+1;
             }
         }
 
         const size_t length = token_string.length();
         if (last_operator == 0) {
             result.push_back(token);
         } else if (last_operator != length){ // operator was not last, we need parse rest of token
-            result.push_back(std::make_pair(
-                    token_string.substr(last_operator, length-last_operator), false));
-        }
+            result.emplace_back(token_string.substr(last_operator, length-last_operator), false); }
     }
 
     return result;
 } // split_tokens(std::vector) }}}
 } // anonymous namespace
 
 
@@ -372,15 +369,15 @@
 				tie(it, std::ignore) =
 					result.dict.insert({ key, std::vector<std::string>() });
 			}
 
 			std::vector<std::string>& val_list = it->second;
 			std::transform(token_line.begin() + 1, token_line.end(),
 				std::back_inserter(val_list),
-				[](const std::pair<std::string, bool> token) { return token.first; });
+				[](const std::pair<std::string, bool>& token) { return token.first; });
 		} else {
 			BodyLine stripped_token_line;
 			std::transform(token_line.begin(), token_line.end(),
 				std::back_inserter(stripped_token_line),
 				[&](const std::pair<std::string, bool>& token) {
 					if (keepQuotes && token.second) return "\"" + token.first + "\"";
 					else return token.first;
@@ -415,15 +412,15 @@
 bool Mata::Parser::ParsedSection::operator==(const ParsedSection& rhs) const {
     return
         this->type == rhs.type &&
         this->dict == rhs.dict &&
         this->body == rhs.body;
 }
 
-std::ostream& Mata::Parser::operator<<(std::ostream& os, const ParsedSection& parsec) {
+std::ostream& std::operator<<(std::ostream& os, const ParsedSection& parsec) {
     os << "@" << parsec.type << "\n";
     for (const auto& string_list_pair : parsec.dict) {
         os << "%" << string_list_pair.first;
         for (const std::string& str : string_list_pair.second) {
             os << " " << str;
         }
         os << "\n";
```

### Comparing `libmata-0.68.0/mata/src/re2parser.cc` & `libmata-0.69.0/mata/src/re2parser.cc`

 * *Files 9% similar despite different names*

```diff
@@ -13,23 +13,19 @@
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
 #include <iostream>
 
-// MATA headers
-#include <mata/alphabet.hh>
-#include <mata/re2parser.hh>
-
-// RE2 headers
-#include <re2/re2/regexp.h>
-#include <re2/re2/prog.h>
-#include <re2/util/logging.h>
-
+#include "mata/alphabet.hh"
+#include "mata/nfa.hh"
+#include "mata/re2parser.hh"
+#include "re2/re2/regexp.h"
+#include "re2/re2/prog.h"
 
 namespace {
     class RegexParser {
     private:
         /**
          * Holds all state cache vectors needed throughout the computation. Vector index is the state number
          * state_mapping for each state (vector index), it holds a vector of states that map to it (cause by epsilon transitions)
@@ -49,15 +45,15 @@
     public:
         /**
          * Default RE2 options
          */
         RE2::Options options;
         StateCache state_cache;
 
-        std::vector<std::vector<std::pair<int, int>>> outgoingEdges;
+        std::vector<std::vector<std::pair<Mata::Symbol, Mata::Nfa::State>>> outgoingEdges;
 
         RegexParser() = default;
 
         /**
          * Creates parsed regex (ie. Regexp*) from string regex_string
          * @param regex_string Regex to be parsed as a string
          * @return Parsed regex as RE2 Regexp*
@@ -82,42 +78,42 @@
         /**
          * Converts re2's prog to mata::Nfa::Nfa
          * @param prog Prog* to create mata::Nfa::Nfa from
          * @param use_epsilon whether to create NFA with epsilon transitions or not
          * @param epsilon_value value, that will represent epsilon on transitions
          * @return mata::Nfa::Nfa created from prog
          */
-        void convert_pro_to_nfa(Mata::Nfa::Nfa* output_nfa, re2::Prog* prog, bool use_epsilon, int epsilon_value) {
-            const int start_state = prog->start();
-            const int prog_size = prog->size();
+        void convert_pro_to_nfa(Mata::Nfa::Nfa* output_nfa, re2::Prog* prog, bool use_epsilon, Mata::Symbol epsilon_value) {
+            const auto start_state = static_cast<size_t>(prog->start());
+            const auto prog_size = static_cast<size_t>(prog->size());
             // The same symbol in lowercase and uppercase is 32 symbols from each other in ASCII
             const int ascii_shift_value = 32;
             int empty_flag;
             std::vector<Mata::Symbol> symbols;
             Mata::Nfa::Nfa explicit_nfa(prog_size);
 
             // Vectors are saved in this->state_cache after this
             this->create_state_cache(prog, use_epsilon);
             // If there are more potential start states, the one without a self-loop should be chosen as a new start state
-            int initial_state_index = 0;
-            int out_state;
+            size_t initial_state_index = 0;
+            Mata::Nfa::State out_state;
             bool self_loop;
             if (this->state_cache.state_mapping[start_state].size() > 1) {
               // There are more potential start states, e.g. there are epsilon transitions from the original start state to
               // more than one state. The new start state should be without a self loop if there is such a state. The new
               // start state can't be a state that was originally final, because it does not have any outgoing edges.
               re2::Prog::Inst *inst;
-              for (auto potential_start_state: this->state_cache.state_mapping[start_state]) {
+              for (Mata::Nfa::State potential_start_state: this->state_cache.state_mapping[start_state]) {
                 self_loop = false;
-                inst = prog->inst(potential_start_state);
+                inst = prog->inst(static_cast<int>(potential_start_state));
                 if (inst->opcode() == re2::kInstMatch) {
                   initial_state_index++;
                   continue;
                 }
-                out_state = inst->out();
+                out_state = static_cast<Mata::Nfa::State>(inst->out());
                 for (auto mapped_state: this->state_cache.state_mapping[out_state]) {
                   if (potential_start_state == mapped_state) {
                     self_loop = true;
                     initial_state_index++;
                     break;
                   }
                 }
@@ -130,32 +126,32 @@
               }
             }
 
             explicit_nfa.initial.add(this->state_cache.state_mapping[start_state][initial_state_index]);
             this->state_cache.has_state_incoming_edge[this->state_cache.state_mapping[start_state][initial_state_index]] = true;
 
             // Used for epsilon closure, it contains tuples (state_reachable_by_epsilon_transitions, source_state_of_epsilon_transitions)
-            std::vector<std::pair<int, int>> copyEdgesFromTo;
+            std::vector<std::pair<Mata::Nfa::State, Mata::Nfa::State >> copyEdgesFromTo;
 
             // If the start state is nop or cap, and has a transition to more different states. We are creating a new
             // start state as one of the states reachable by epsilon from the start state. We must also include
             // transitions of the other epsilon reachable states to the new start state.
             if (this->state_cache.is_state_nop_or_cap[start_state] && this->state_cache.state_mapping[start_state].size() > 1) {
-                for (int index = 0; index < this->state_cache.state_mapping[start_state].size(); index++) {
+                for (size_t index = 0; index < this->state_cache.state_mapping[start_state].size(); index++) {
                     for (auto state: this->state_cache.state_mapping[this->state_cache.state_mapping[start_state][index]]) {
                         copyEdgesFromTo.emplace_back(state, this->state_cache.state_mapping[start_state][initial_state_index]);
                     }
                 }
             }
 
-            this->outgoingEdges = std::vector<std::vector<std::pair<int, int>>> (prog_size);
+            this->outgoingEdges = std::vector<std::vector<std::pair<Mata::Symbol, Mata::Nfa::State>>> (prog_size);
 
             // We traverse all the states and create corresponding states and edges in mata::Nfa::Nfa
-            for (int current_state = start_state; current_state < prog_size; current_state++) {
-                re2::Prog::Inst *inst = prog->inst(current_state);
+            for (Mata::Nfa::State current_state = start_state; current_state < prog_size; current_state++) {
+                re2::Prog::Inst *inst = prog->inst(static_cast<int>(current_state));
                 // Every type of state can be final (due to epsilon transition), so we check it regardless of its type
                 if (this->state_cache.is_final_state[current_state]) {
                     this->make_state_final(current_state, explicit_nfa);
                 }
                 switch (inst->opcode()) {
                     default:
                         LOG(DFATAL) << "unhandled " << inst->opcode() << " in convertProgTomata::Nfa::Nfa";
@@ -202,20 +198,21 @@
                             symbols.push_back(303);
                         }
                         // \B - not \b
                         if (empty_flag & re2::kEmptyNonWordBoundary) {
                             // TODO Symbol?
                             symbols.push_back(304);
                         }
+                        break;
                     // kInstByteRange represents states with a "byte range" on the outgoing transition(s)
                     // (it can also be a single byte)
                     case re2::kInstByteRange:
                         if (symbols.empty()) {
                             // Save all symbols that can be used on the current transition
-                            for (long int symbol = inst->lo(); symbol <= inst->hi(); symbol++) {
+                            for (auto symbol = static_cast<Mata::Symbol>(inst->lo()); symbol <= static_cast<Mata::Symbol>(inst->hi()); symbol++) {
                                 symbols.push_back(symbol);
                                 // Foldcase causes RE2 to do a case-insensitive match, so transitions will be made for
                                 // both uppercase and lowercase symbols
                                 if (inst->foldcase()) {
                                     symbols.push_back(symbol-ascii_shift_value);
                                 }
                             }
@@ -236,15 +233,15 @@
                 }
             }
             if (!use_epsilon) {
                 // We will traverse the vector in reversed order. Like that, we will also handle chains of epsilon transitions
                 // 2 -(eps)-> 3 -(eps)-> 4 -(a)-> 5.... We first need to copy transitions of state 4 to state 3, and then
                 // we can copy transition of state 3 (which now have copied transitions of state 4) to state 2
                 for (auto copyEdgeFromTo = copyEdgesFromTo.rbegin(); copyEdgeFromTo != copyEdgesFromTo.rend(); copyEdgeFromTo++) {
-                    re2::Prog::Inst *inst = prog->inst(copyEdgeFromTo->first);
+                    re2::Prog::Inst *inst = prog->inst(static_cast<int>(copyEdgeFromTo->first));
                     // kInstMatch states in RE2 does not have outgoing edges. The other state will also be final
                     if (inst->opcode() == re2::kInstMatch) {
                         this->make_state_final(copyEdgeFromTo->second, explicit_nfa);
                         this->state_cache.is_final_state[copyEdgeFromTo->second] = true;
                         continue;
                     }
                     // The state is final if there are epsilon transition(s) leading to a final state
@@ -275,24 +272,24 @@
          * @param statesFrom states that will be used as source states
          * @param inst RE2 instruction for the current state, it is used to determine the target state for each transition
          * @param symbols symbols that will be used on each transition
          * @param nfa ExplicitNFA in which the transitions should be created
          * @param use_epsilon whether to create NFA with epsilon transitions or not
          * @param epsilon_value value, that will represent epsilon on transitions
          */
-        void create_explicit_nfa_transitions(int currentState, re2::Prog::Inst *inst,
-                                                       const std::vector<Mata::Symbol>& symbols,
-                                                       Mata::Nfa::Nfa &nfa, bool use_epsilon, int epsilon_value) {
+        void create_explicit_nfa_transitions(Mata::Nfa::State currentState, re2::Prog::Inst *inst,
+                                             const std::vector<Mata::Symbol>& symbols,
+                                             Mata::Nfa::Nfa &nfa, bool use_epsilon, Mata::Symbol epsilon_value) {
             for (auto mappedState: this->state_cache.state_mapping[currentState]) {
-                for (auto mappedTargetState: this->state_cache.state_mapping[inst->out()]) {
+                for (auto mappedTargetState: this->state_cache.state_mapping[static_cast<unsigned long>(inst->out())]) {
                     // There can be more symbols on the edge
                     for (auto symbol: symbols) {
                         if (!use_epsilon) {
                             // Save all outgoing edges. The vector will be used to get rid of epsilon transitions
-                            this->outgoingEdges[mappedState].push_back({symbol, mappedTargetState});
+                            this->outgoingEdges[mappedState].emplace_back(symbol, mappedTargetState);
                         }
                         if (this->state_cache.has_state_incoming_edge[mappedState]) {
                             this->state_cache.has_state_incoming_edge[mappedTargetState] = true;
                             nfa.delta.add(mappedState, symbol, mappedTargetState);
                         }
                     }
                 }
@@ -322,131 +319,132 @@
         /**
          * Creates all state cache vectors needed throughout the computation and saves them
          * to the private variable state_cache
          * It creates state cache for creating ExplicitNFA without epsilon transitions
          * @param prog RE2 prog corresponding to the parsed regex
          */
         void create_state_cache_without_epsilon(re2::Prog *prog) {
-            std::vector<bool> default_false_vec(prog->size(), false);
+            std::vector<bool> default_false_vec(static_cast<size_t>(prog->size()), false);
             this->state_cache = {
                 // state_mapping holds states that map to each state (index) due to epsilon transitions
                 {},
                 // is_final_state holds true for states that are final, false for the rest
                 default_false_vec,
                 // is_state_nop_or_cap holds true for states that have type nop or cap, false for the rest
                 default_false_vec,
                 // is_last holds true for states that are last, false for the rest
                 default_false_vec,
                 // has_state_incoming_edge holds true for states with an incoming edge, false for the rest
                 default_false_vec,
             };
-            const int start_state = prog->start();
-            const int prog_size = prog->size();
+            const auto start_state = static_cast<size_t>(prog->start());
+            const auto prog_size = static_cast<size_t>(prog->size());
 
             // Used for the first loop through states
             std::vector<Mata::Nfa::State> tmp_state_mapping(prog_size);
             for (Mata::Nfa::State state = 0; state < prog_size; state++) {
                 tmp_state_mapping[state] = state;
                 this->state_cache.state_mapping.push_back({state});
             }
 
             // When there is nop or capture type of state, we will be appending to it
-            int append_to_state = -1;
+            Mata::Nfa::State append_to_state = Mata::Nfa::Limits::max_state;
             Mata::Nfa::State mapped_parget_state;
-            std::vector<int> states_for_second_check(prog_size);
+            std::vector<Mata::Nfa::State> states_for_second_check(prog_size);
 
             for (Mata::Nfa::State state = start_state; state < prog_size; state++) {
-                re2::Prog::Inst *inst = prog->inst(state);
+                re2::Prog::Inst *inst = prog->inst(static_cast<int>(state));
                 if (inst->last()) {
                     this->state_cache.is_last[state] = true;
                 }
 
                 if (inst->opcode() == re2::kInstCapture || inst->opcode() == re2::kInstNop) {
                     this->state_cache.state_mapping[state] = this->get_mapped_states(prog, state, inst);
                     this->state_cache.is_state_nop_or_cap[state] = true;
                     mapped_parget_state = tmp_state_mapping[static_cast<Mata::Nfa::State>(inst->out())];
                     tmp_state_mapping[state] = mapped_parget_state;
-                    if (append_to_state != -1) {
+                    if (append_to_state != Mata::Nfa::Limits::max_state) {
                         // Nop or capture type of state may or may not have an incoming edge, the target state should have
                         // it only if the current state has it
                         if (this->state_cache.has_state_incoming_edge[state]) {
                             this->state_cache.has_state_incoming_edge[mapped_parget_state] = true;
                         }
                         tmp_state_mapping[append_to_state] = mapped_parget_state;
                     } else {
                         append_to_state = state;
                     }
                 } else if (inst->opcode() == re2::kInstMatch) {
                     this->state_cache.is_final_state[state] = true;
-                    if (append_to_state != -1 && this->state_cache.has_state_incoming_edge[append_to_state]) {
+                    if (append_to_state != Mata::Nfa::Limits::max_state
+                        && this->state_cache.has_state_incoming_edge[append_to_state]) {
                       this->state_cache.has_state_incoming_edge[state] = true;
                     }
-                    append_to_state = -1;
+                    append_to_state = Mata::Nfa::Limits::max_state;
                 } else {
                     // Other types of states will always have an incoming edge so the target state will always have it too
-                    this->state_cache.has_state_incoming_edge[inst->out()] = true;
-                    if (inst->out() < state) {
-                      for (auto mapped_state: this->state_cache.state_mapping[inst->out()]) {
+                    this->state_cache.has_state_incoming_edge[static_cast<size_t>(inst->out())] = true;
+                    if (static_cast<size_t>(inst->out()) < state) {
+                      for (auto mapped_state: this->state_cache.state_mapping[static_cast<size_t>(inst->out())]) {
                         if (mapped_state == state) {
                           this->state_cache.has_state_incoming_edge[state] = true;
-                        } else if (prog->inst(mapped_state)->opcode() == re2::kInstMatch) {
+                        } else if (prog->inst(static_cast<int>(mapped_state))->opcode() == re2::kInstMatch) {
                           this->state_cache.has_state_incoming_edge[mapped_state] = true;
                         }
                       }
                     } else {
                       states_for_second_check.push_back(state);
                     }
-                    append_to_state = -1;
+                    append_to_state = Mata::Nfa::Limits::max_state;
                 }
             }
             // There could be epsilon transitions leading back to the same state. In such case, the state
             // should have incoming edge set
             for (auto state_to_check: states_for_second_check) {
-              re2::Prog::Inst *inst = prog->inst(state_to_check);
-              for (auto mapped_state: this->state_cache.state_mapping[inst->out()]) {
+              re2::Prog::Inst *inst = prog->inst(static_cast<int>(state_to_check));
+              for (auto mapped_state: this->state_cache.state_mapping[static_cast<size_t>(inst->out())]) {
                 this->state_cache.has_state_incoming_edge[mapped_state] = true;
               }
             }
         }
 
         /**
           * Creates all state cache vectors needed throughout the computation and saves them to the private variable state_cache.
           * It creates state cache for creating ExplicitNFA with epsilon transitions
           * @param prog RE2 prog corresponding to the parsed regex
           */
         void create_state_cache_with_epsilon(re2::Prog *prog) {
-            std::vector<bool> defaultFalseVec(prog->size(), false);
-            std::vector<bool> defaultTrueVec(prog->size(), true);
+            std::vector<bool> defaultFalseVec(static_cast<size_t>(prog->size()), false);
+            std::vector<bool> defaultTrueVec(static_cast<size_t>(prog->size()), true);
             this->state_cache = {
                     {}, // stateMapping all states are mapped to itself when using epsilon transitions
                     defaultFalseVec, // is_final_state holds true for states that are final, false for the rest
                     defaultFalseVec, // is_state_nop_or_cap not used when using epsilon transition
                     defaultFalseVec, // is_last holds true for states that are last, false for the rest
                     defaultTrueVec, // has_state_incoming_edge holds true all states
             };
-            const int progSize = prog->size();
+            const auto progSize = static_cast<size_t>(prog->size());
 
             for (Mata::Nfa::State state = 0; state < progSize; state++) {
                 this->state_cache.state_mapping.push_back({state});
-                re2::Prog::Inst *inst = prog->inst(state);
+                re2::Prog::Inst *inst = prog->inst(static_cast<int>(state));
                 if (inst->last()) {
                     this->state_cache.is_last[state] = true;
                 }
                 if (inst->opcode() == re2::kInstMatch) {
                     this->state_cache.is_final_state[state] = true;
                 }
             }
         }
 
         /**
          * Makes all states mapped to the state parameter final in the mata::Nfa::Nfa
          * @param state State which should be made final
          * @param nfa mata::Nfa::Nfa in which the states will be made final
          */
-        void make_state_final(int state, Mata::Nfa::Nfa &nfa) {
+        void make_state_final(Mata::Nfa::State state, Mata::Nfa::Nfa &nfa) {
             for (auto target_state: this->state_cache.state_mapping[state]) {
                 // States without an incoming edge should not be in the automata
                 if (!this->state_cache.has_state_incoming_edge[target_state]) {
                     continue;
                 }
                 nfa.final.add(target_state);
             }
@@ -455,19 +453,19 @@
         /**
          * Renumbers the states of the input_nfa to be from <0, numberOfStates>
          * @param program_size Size of the RE2 prog
          * @param input_nfa mata::Nfa::Nfa which states should be renumbered
          * @return Same mata::Nfa::Nfa as input_nfa but with states from interval <0, numberOfStates>
          */
         static Mata::Nfa::Nfa renumber_states(Mata::Nfa::Nfa* output_nfa,
-                                              int program_size,
+                                              size_t program_size,
                                               Mata::Nfa::Nfa &input_nfa) {
-            std::vector<unsigned long> renumbered_states(program_size, -1);
+            std::vector<Mata::Nfa::State> renumbered_states(program_size, Mata::Nfa::Limits::max_state);
             Mata::Nfa::Nfa& renumbered_explicit_nfa = *output_nfa;
-            for (int state = 0; state < program_size; state++) {
+            for (Mata::Nfa::State state{ 0 }; state < program_size; state++) {
                 const auto& transition_list = input_nfa.get_moves_from(state);
                 // If the transition list is empty, the state is not used
                 if (transition_list.empty()) {
                     continue;
                 } else {
                     // addNewState returns next unused state of the new NFA, so we map it to the original state
                     renumbered_states[state] = renumbered_explicit_nfa.add_state();
@@ -477,19 +475,19 @@
             for (auto state: input_nfa.final) {
                 if (static_cast<int>(renumbered_states[state]) == -1) {
                     renumbered_states[state] = renumbered_explicit_nfa.add_state();
                 }
                 renumbered_explicit_nfa.final.add(renumbered_states[state]);
             }
 
-            for (int state = 0; state < program_size; state++) {
+            for (Mata::Nfa::State state{ 0 }; state < program_size; state++) {
                 const auto& transition_list = input_nfa.get_moves_from(state);
                 for (const auto& transition: transition_list) {
                     for (auto stateTo: transition.targets) {
-                        if (static_cast<int>(renumbered_states[stateTo]) == -1) {
+                        if (renumbered_states[stateTo] == Mata::Nfa::Limits::max_state) {
                             renumbered_states[stateTo] = renumbered_explicit_nfa.add_state();
                         }
                         assert(renumbered_states[state] <= renumbered_explicit_nfa.size());
                         assert(renumbered_states[stateTo] <= renumbered_explicit_nfa.size());
                         renumbered_explicit_nfa.delta.add(renumbered_states[state], transition.symbol,
                                                           renumbered_states[stateTo]);
                     }
@@ -508,48 +506,48 @@
          * Gets all states that are mapped to the state (i.e., states that are within epsilon transitions chain)
          * @param prog RE2 prog corresponding to the parsed regex
          * @param state State for which the mapped states should be computed
          * @param inst RE2 instruction for the state
          * @return All states that are mapped to the state
          */
         std::vector<Mata::Nfa::State> get_mapped_states(
-                re2::Prog* prog, int state, re2::Prog::Inst *inst) {
+                re2::Prog* prog, Mata::Nfa::State state, re2::Prog::Inst *inst) {
             std::vector<Mata::Nfa::State> mappedStates;
             std::vector<Mata::Nfa::State> statesToCheck;
             std::set<Mata::Nfa::State> checkedStates;
 
             statesToCheck.push_back(state);
             while (!statesToCheck.empty()) {
                 state = statesToCheck.back();
-                inst = prog->inst(state);
+                inst = prog->inst(static_cast<int>(state));
                 checkedStates.insert(state);
                 statesToCheck.pop_back();
                 // If the state is not last, it also has an epsilon transition which we must follow
                 if (!inst->last()) {
-                    re2::Prog::Inst *nextInst = prog->inst(state + 1);
+                    re2::Prog::Inst *nextInst = prog->inst(static_cast<int>(state + 1));
                     if (nextInst->last()) {
                         this->state_cache.is_last[state + 1] = true;
                     }
                     if (checkedStates.count(state+1) == 0) {
                         statesToCheck.push_back(state+1);
                     }
                 } else if (inst->opcode() != re2::kInstCapture && inst->opcode() != re2::kInstNop) {
                     // It is state with "normal" transition. It is the last state in the epsilon transitions chain
                     mappedStates.push_back(state);
                     continue;
                 }
                 re2::Prog::Inst *outInst = prog->inst(inst->out());
                 if (outInst->opcode() == re2::kInstCapture || outInst->opcode() == re2::kInstNop) {
                     // The state has outgoing epsilon transition which we must follow
-                    if (checkedStates.count(inst->out()) == 0) {
-                        statesToCheck.push_back(inst->out());
+                    if (checkedStates.count(static_cast<Mata::Nfa::State>(inst->out())) == 0) {
+                        statesToCheck.push_back(static_cast<Mata::Nfa::State>(inst->out()));
                     }
                 } else {
                     // It is state with "normal" transition. It is the last state in the epsilon transitions chain
-                    mappedStates.push_back(inst->out());
+                    mappedStates.push_back(static_cast<Mata::Nfa::State>(inst->out()));
                 }
             }
             return mappedStates;
         }
         };
 }
 
@@ -557,15 +555,15 @@
  * The main method, it creates NFA from regex
  * @param pattern regex as string
  * @param use_epsilon whether to create NFA with epsilon transitions or not
  * @param epsilon_value value, that will represent epsilon on transitions
  * @param use_reduce if set to true the result is trimmed and reduced using simulation reduction
  * @return mata::Nfa::Nfa corresponding to pattern
  */
-void Mata::Parser::create_nfa(Nfa::Nfa* nfa, const std::string& pattern, bool use_epsilon, int epsilon_value, bool use_reduce) {
+void Mata::Parser::create_nfa(Nfa::Nfa* nfa, const std::string& pattern, bool use_epsilon, Mata::Symbol epsilon_value, bool use_reduce) {
     if (nfa == nullptr) {
         throw std::runtime_error("create_nfa: nfa should not be NULL");
     }
 
     RegexParser regexParser{};
     auto parsed_regex = regexParser.parse_regex_string(pattern);
     auto program = parsed_regex->CompileToProg(regexParser.options.max_mem() * 2 / 3);
```

### Comparing `libmata-0.68.0/mata/src/strings/nfa-noodlification.cc` & `libmata-0.69.0/mata/src/strings/nfa-noodlification.cc`

 * *Files 1% similar despite different names*

```diff
@@ -193,17 +193,17 @@
     State unused_state = aut.size(); // get some State not used in aut
     std::map<std::pair<State, State>, std::shared_ptr<Nfa::Nfa>> segments_one_initial_final;
     segs_one_initial_final(segments, include_empty, unused_state, segments_one_initial_final);
 
     const auto& epsilon_depths_map{ segmentation.get_epsilon_depth_trans_map() };
 
     struct SegItem {
-        NoodleSubst noodle;
-        State fin;
-        size_t seg_id;
+        NoodleSubst noodle{};
+        State fin{};
+        size_t seg_id{};
     };
 
     NoodleSubstSequence noodles{};
     std::deque<SegItem> lifo;
 
     for(const State& fn : segments[0].final) {
         SegItem new_item;
```

### Comparing `libmata-0.68.0/mata/src/strings/nfa-segmentation.cc` & `libmata-0.69.0/mata/src/strings/nfa-segmentation.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/mata/src/strings/nfa-strings.cc` & `libmata-0.69.0/mata/src/strings/nfa-strings.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.68.0/setup.py` & `libmata-0.69.0/setup.py`

 * *Files identical despite different names*

