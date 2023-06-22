# Comparing `tmp/iminuit-2.8.4.tar.gz` & `tmp/iminuit-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iminuit-2.8.4.tar", last modified: Mon Oct 11 09:28:35 2021, max compression
+gzip compressed data, was "iminuit-2.9.0.tar", last modified: Sun Jan  9 14:13:19 2022, max compression
```

## Comparing `iminuit-2.8.4.tar` & `iminuit-2.9.0.tar`

### file list

```diff
@@ -1,322 +1,326 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 09:28:35.619011 iminuit-2.8.4/
--rw-r--r--   0 runner    (1001) docker     (121)     4321 2021-10-11 09:28:10.000000 iminuit-2.8.4/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      347 2021-10-11 09:28:10.000000 iminuit-2.8.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2021-10-11 09:28:10.000000 iminuit-2.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      537 2021-10-11 09:28:10.000000 iminuit-2.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5778 2021-10-11 09:28:35.619011 iminuit-2.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3386 2021-10-11 09:28:10.000000 iminuit-2.8.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3217 2021-10-11 09:28:10.000000 iminuit-2.8.4/cmake_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 09:28:35.574999 iminuit-2.8.4/extern/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 09:28:35.583001 iminuit-2.8.4/extern/pybind11/
--rw-r--r--   0 runner    (1001) docker     (121)    10364 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1684 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 09:28:35.574999 iminuit-2.8.4/extern/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 09:28:35.587002 iminuit-2.8.4/extern/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (121)    21412 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (121)     6118 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (121)    95557 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (121)     8185 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (121)      120 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (121)     2037 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 09:28:35.587002 iminuit-2.8.4/extern/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (121)    27823 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (121)    40452 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (121)     3602 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (121)    16397 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (121)    16375 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (121)    29086 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (121)     7843 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (121)     5079 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (121)     3709 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (121)     6084 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (121)    69310 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (121)     9085 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (121)     2049 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (121)   111558 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (121)    66118 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/pytypes.h
--rw-r--r--   0 runner    (1001) docker     (121)    14136 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (121)    23912 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 09:28:35.587002 iminuit-2.8.4/extern/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (121)     2295 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     3105 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     9977 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    14003 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     9172 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     7276 2021-10-11 09:28:27.000000 iminuit-2.8.4/extern/pybind11/tools/pybind11Tools.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 09:28:35.574999 iminuit-2.8.4/extern/root/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 09:28:35.574999 iminuit-2.8.4/extern/root/math/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 09:28:35.574999 iminuit-2.8.4/extern/root/math/minuit2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 09:28:35.587002 iminuit-2.8.4/extern/root/math/minuit2/inc/
--rw-r--r--   0 runner    (1001) docker     (121)     2299 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/LinkDef.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 09:28:35.599006 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/
--rw-r--r--   0 runner    (1001) docker     (121)     3998 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ABObj.h
--rw-r--r--   0 runner    (1001) docker     (121)     1732 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ABProd.h
--rw-r--r--   0 runner    (1001) docker     (121)     2186 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ABSum.h
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ABTypes.h
--rw-r--r--   0 runner    (1001) docker     (121)     1365 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/AnalyticalGradientCalculator.h
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/BFGSErrorUpdator.h
--rw-r--r--   0 runner    (1001) docker     (121)     1529 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/CombinedMinimizer.h
--rw-r--r--   0 runner    (1001) docker     (121)     2039 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/CombinedMinimumBuilder.h
--rw-r--r--   0 runner    (1001) docker     (121)     2322 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ContoursError.h
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/DavidonErrorUpdator.h
--rw-r--r--   0 runner    (1001) docker     (121)     1873 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ExternalInternalGradientCalculator.h
--rw-r--r--   0 runner    (1001) docker     (121)     1424 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FCNAdapter.h
--rw-r--r--   0 runner    (1001) docker     (121)     3487 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FCNBase.h
--rw-r--r--   0 runner    (1001) docker     (121)     2175 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FCNGradAdapter.h
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FCNGradientBase.h
--rw-r--r--   0 runner    (1001) docker     (121)     3908 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliBuilder.h
--rw-r--r--   0 runner    (1001) docker     (121)     4646 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliChi2FCN.h
--rw-r--r--   0 runner    (1001) docker     (121)     3090 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliErrorUpdator.h
--rw-r--r--   0 runner    (1001) docker     (121)     3991 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliFCNAdapter.h
--rw-r--r--   0 runner    (1001) docker     (121)     4452 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliFCNBase.h
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliGradientCalculator.h
--rw-r--r--   0 runner    (1001) docker     (121)     4510 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliMaximumLikelihoodFCN.h
--rw-r--r--   0 runner    (1001) docker     (121)     5835 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliMinimizer.h
--rw-r--r--   0 runner    (1001) docker     (121)     5632 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliStandardChi2FCN.h
--rw-r--r--   0 runner    (1001) docker     (121)     3505 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliStandardMaximumLikelihoodFCN.h
--rw-r--r--   0 runner    (1001) docker     (121)     1859 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FunctionGradient.h
--rw-r--r--   0 runner    (1001) docker     (121)     2723 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FunctionMinimizer.h
--rw-r--r--   0 runner    (1001) docker     (121)     4948 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FunctionMinimum.h
--rw-r--r--   0 runner    (1001) docker     (121)     1440 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/GenericFunction.h
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/GradientCalculator.h
--rw-r--r--   0 runner    (1001) docker     (121)     1968 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/HessianGradientCalculator.h
--rw-r--r--   0 runner    (1001) docker     (121)     1771 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/InitialGradientCalculator.h
--rw-r--r--   0 runner    (1001) docker     (121)    14081 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/LASymMatrix.h
--rw-r--r--   0 runner    (1001) docker     (121)    11017 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/LAVector.h
--rw-r--r--   0 runner    (1001) docker     (121)     2746 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/LaInverse.h
--rw-r--r--   0 runner    (1001) docker     (121)     2828 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/LaOuterProduct.h
--rw-r--r--   0 runner    (1001) docker     (121)     2520 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/LaProd.h
--rw-r--r--   0 runner    (1001) docker     (121)     3278 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/LaSum.h
--rw-r--r--   0 runner    (1001) docker     (121)     4211 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MPIProcess.h
--rw-r--r--   0 runner    (1001) docker     (121)     1438 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MatrixInverse.h
--rw-r--r--   0 runner    (1001) docker     (121)     1829 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MinimumBuilder.h
--rw-r--r--   0 runner    (1001) docker     (121)     2962 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MinimumError.h
--rw-r--r--   0 runner    (1001) docker     (121)      951 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MinimumErrorUpdator.h
--rw-r--r--   0 runner    (1001) docker     (121)     1792 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MinimumParameters.h
--rw-r--r--   0 runner    (1001) docker     (121)     1761 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MinimumSeed.h
--rw-r--r--   0 runner    (1001) docker     (121)     1393 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MinimumSeedGenerator.h
--rw-r--r--   0 runner    (1001) docker     (121)     3236 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MinimumState.h
--rw-r--r--   0 runner    (1001) docker     (121)     3392 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MinosError.h
--rw-r--r--   0 runner    (1001) docker     (121)    13014 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/Minuit2Minimizer.h
--rw-r--r--   0 runner    (1001) docker     (121)     5347 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MinuitParameter.h
--rw-r--r--   0 runner    (1001) docker     (121)     4767 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnApplication.h
--rw-r--r--   0 runner    (1001) docker     (121)      676 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnConfig.h
--rw-r--r--   0 runner    (1001) docker     (121)     2292 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnContours.h
--rw-r--r--   0 runner    (1001) docker     (121)     1209 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnCovarianceSqueeze.h
--rw-r--r--   0 runner    (1001) docker     (121)     3170 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnCross.h
--rw-r--r--   0 runner    (1001) docker     (121)      951 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnEigen.h
--rw-r--r--   0 runner    (1001) docker     (121)     1756 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnFcn.h
--rw-r--r--   0 runner    (1001) docker     (121)     3977 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnFumiliMinimize.h
--rw-r--r--   0 runner    (1001) docker     (121)     1342 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnFunctionCross.h
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnGlobalCorrelationCoeff.h
--rw-r--r--   0 runner    (1001) docker     (121)     3593 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnHesse.h
--rw-r--r--   0 runner    (1001) docker     (121)     1816 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnLineSearch.h
--rw-r--r--   0 runner    (1001) docker     (121)     1898 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnMachinePrecision.h
--rw-r--r--   0 runner    (1001) docker     (121)      952 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnMatrix.h
--rw-r--r--   0 runner    (1001) docker     (121)     5422 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnMigrad.h
--rw-r--r--   0 runner    (1001) docker     (121)     5303 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnMinimize.h
--rw-r--r--   0 runner    (1001) docker     (121)     2446 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnMinos.h
--rw-r--r--   0 runner    (1001) docker     (121)     3476 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnParabola.h
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnParabolaFactory.h
--rw-r--r--   0 runner    (1001) docker     (121)     1661 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnParabolaPoint.h
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnParameterScan.h
--rw-r--r--   0 runner    (1001) docker     (121)     1446 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnPlot.h
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnPosDef.h
--rw-r--r--   0 runner    (1001) docker     (121)     5569 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnPrint.h
--rw-r--r--   0 runner    (1001) docker     (121)     2620 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnRefCountedPointer.h
--rw-r--r--   0 runner    (1001) docker     (121)     1526 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnReferenceCounter.h
--rw-r--r--   0 runner    (1001) docker     (121)     3427 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnScan.h
--rw-r--r--   0 runner    (1001) docker     (121)     1262 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnSeedGenerator.h
--rw-r--r--   0 runner    (1001) docker     (121)     3587 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnSimplex.h
--rw-r--r--   0 runner    (1001) docker     (121)     2838 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnStrategy.h
--rw-r--r--   0 runner    (1001) docker     (121)      799 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnTiny.h
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnTraceObject.h
--rw-r--r--   0 runner    (1001) docker     (121)     2704 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnUserCovariance.h
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnUserFcn.h
--rw-r--r--   0 runner    (1001) docker     (121)     6040 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnUserParameterState.h
--rw-r--r--   0 runner    (1001) docker     (121)     4228 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnUserParameters.h
--rw-r--r--   0 runner    (1001) docker     (121)     6363 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnUserTransformation.h
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnVectorTransform.h
--rw-r--r--   0 runner    (1001) docker     (121)     4744 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ModularFunctionMinimizer.h
--rw-r--r--   0 runner    (1001) docker     (121)     1375 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/NegativeG2LineSearch.h
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/Numerical2PGradientCalculator.h
--rw-r--r--   0 runner    (1001) docker     (121)     4880 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/NumericalDerivator.h
--rw-r--r--   0 runner    (1001) docker     (121)     4425 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ParametricFunction.h
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ScanBuilder.h
--rw-r--r--   0 runner    (1001) docker     (121)     1472 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ScanMinimizer.h
--rw-r--r--   0 runner    (1001) docker     (121)     1157 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/SimplexBuilder.h
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/SimplexMinimizer.h
--rw-r--r--   0 runner    (1001) docker     (121)     1815 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/SimplexParameters.h
--rw-r--r--   0 runner    (1001) docker     (121)     1300 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/SimplexSeedGenerator.h
--rw-r--r--   0 runner    (1001) docker     (121)     1309 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/SinParameterTransformation.h
--rw-r--r--   0 runner    (1001) docker     (121)     1566 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/SqrtLowParameterTransformation.h
--rw-r--r--   0 runner    (1001) docker     (121)     1602 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/SqrtUpParameterTransformation.h
--rw-r--r--   0 runner    (1001) docker     (121)     6384 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/StackAllocator.h
--rw-r--r--   0 runner    (1001) docker     (121)     2481 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/VariableMetricBuilder.h
--rw-r--r--   0 runner    (1001) docker     (121)      936 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/VariableMetricEDMEstimator.h
--rw-r--r--   0 runner    (1001) docker     (121)     1805 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/VariableMetricMinimizer.h
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/VectorOuterProduct.h
--rw-r--r--   0 runner    (1001) docker     (121)     1532 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/inc/TMinuit2TraceObject.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 09:28:35.611009 iminuit-2.8.4/extern/root/math/minuit2/src/
--rw-r--r--   0 runner    (1001) docker     (121)     2341 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/AnalyticalGradientCalculator.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     4460 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/BFGSErrorUpdator.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/BasicMinimumError.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1913 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/CombinedMinimumBuilder.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     4896 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/DavidonErrorUpdator.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/ExternalInternalGradientCalculator.cxx
--rw-r--r--   0 runner    (1001) docker     (121)    12578 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/FumiliBuilder.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     3262 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/FumiliErrorUpdator.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     3975 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/FumiliGradientCalculator.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     3706 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/FumiliMinimizer.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     3483 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/FumiliStandardChi2FCN.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     5923 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/FumiliStandardMaximumLikelihoodFCN.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     4968 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/HessianGradientCalculator.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     3770 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/InitialGradientCalculator.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1347 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/LaEigenValues.cxx
--rw-r--r--   0 runner    (1001) docker     (121)      838 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/LaInnerProduct.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/LaInverse.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     2640 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/LaOuterProduct.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/LaSumOfElements.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/LaVtMVSimilarity.cxx
--rw-r--r--   0 runner    (1001) docker     (121)    10206 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MPIProcess.cxx
--rw-r--r--   0 runner    (1001) docker     (121)      709 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MinimumBuilder.cxx
--rw-r--r--   0 runner    (1001) docker     (121)    44323 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/Minuit2Minimizer.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     6559 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnApplication.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     7308 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnContours.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     3493 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnCovarianceSqueeze.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnEigen.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnFcn.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnFumiliMinimize.cxx
--rw-r--r--   0 runner    (1001) docker     (121)    17186 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnFunctionCross.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1376 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnGlobalCorrelationCoeff.cxx
--rw-r--r--   0 runner    (1001) docker     (121)    15157 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnHesse.cxx
--rw-r--r--   0 runner    (1001) docker     (121)    25798 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnLineSearch.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnMachinePrecision.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     7207 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnMinos.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     2248 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnParabolaFactory.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     2590 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnParameterScan.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     2189 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnPlot.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     3308 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnPosDef.cxx
--rw-r--r--   0 runner    (1001) docker     (121)    13673 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnPrint.cxx
--rw-r--r--   0 runner    (1001) docker     (121)      828 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnPrintImpl.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnScan.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     6218 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnSeedGenerator.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnStrategy.cxx
--rw-r--r--   0 runner    (1001) docker     (121)      788 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnTiny.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1745 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnTraceObject.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnUserFcn.cxx
--rw-r--r--   0 runner    (1001) docker     (121)    18034 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnUserParameterState.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     5575 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnUserParameters.cxx
--rw-r--r--   0 runner    (1001) docker     (121)    17290 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/MnUserTransformation.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     9352 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/ModularFunctionMinimizer.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     4276 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/NegativeG2LineSearch.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     8456 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/Numerical2PGradientCalculator.cxx
--rw-r--r--   0 runner    (1001) docker     (121)    11256 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/NumericalDerivator.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1594 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/ParametricFunction.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1889 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/ScanBuilder.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     7882 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/SimplexBuilder.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/SimplexParameters.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     2234 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/SimplexSeedGenerator.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     2166 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/SinParameterTransformation.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1567 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/SqrtLowParameterTransformation.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1562 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/SqrtUpParameterTransformation.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     4072 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/TMinuit2TraceObject.cxx
--rw-r--r--   0 runner    (1001) docker     (121)    13571 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/VariableMetricBuilder.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/VariableMetricEDMEstimator.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     2768 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/mnbins.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     2402 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/mndasum.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     2304 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/mndaxpy.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     2418 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/mnddot.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/mndscal.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     9247 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/mndspmv.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     7151 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/mndspr.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     1869 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/mnlsame.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     6950 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/mnteigen.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     6393 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/mntplot.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     2060 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/mnvert.cxx
--rw-r--r--   0 runner    (1001) docker     (121)     2296 2021-10-11 09:28:32.000000 iminuit-2.8.4/extern/root/math/minuit2/src/mnxerbla.cxx
--rw-r--r--   0 runner    (1001) docker     (121)      441 2021-10-11 09:28:10.000000 iminuit-2.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2237 2021-10-11 09:28:35.619011 iminuit-2.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      305 2021-10-11 09:28:10.000000 iminuit-2.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 09:28:35.615010 iminuit-2.8.4/src/
--rw-r--r--   0 runner    (1001) docker     (121)      487 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/application.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      678 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/contours.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      328 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/equal.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1576 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/equal.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     4305 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/fcn.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/fcn.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2268 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/functionminimum.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     5986 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/functionminimum_extra.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1478 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/functionminimum_pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/hesse.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 09:28:35.615010 iminuit-2.8.4/src/iminuit/
--rw-r--r--   0 runner    (1001) docker     (121)      870 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/iminuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      539 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/iminuit/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (121)     9175 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/iminuit/_repr_html.py
--rw-r--r--   0 runner    (1001) docker     (121)     6335 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/iminuit/_repr_text.py
--rw-r--r--   0 runner    (1001) docker     (121)    26815 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/iminuit/cost.py
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/iminuit/experimental.py
--rw-r--r--   0 runner    (1001) docker     (121)     4467 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/iminuit/minimize.py
--rw-r--r--   0 runner    (1001) docker     (121)    71354 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/iminuit/minuit.py
--rw-r--r--   0 runner    (1001) docker     (121)    10255 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/iminuit/pdg_format.py
--rw-r--r--   0 runner    (1001) docker     (121)     1635 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/iminuit/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)    40811 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/iminuit/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      587 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/iminuit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 09:28:35.615010 iminuit-2.8.4/src/iminuit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5778 2021-10-11 09:28:35.000000 iminuit-2.8.4/src/iminuit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12975 2021-10-11 09:28:35.000000 iminuit-2.8.4/src/iminuit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-11 09:28:35.000000 iminuit-2.8.4/src/iminuit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-11 09:28:35.000000 iminuit-2.8.4/src/iminuit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      315 2021-10-11 09:28:35.000000 iminuit-2.8.4/src/iminuit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-10-11 09:28:35.000000 iminuit-2.8.4/src/iminuit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      481 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/lasymmatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      281 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/lasymmatrix.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      383 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/lavector.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      254 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/lavector.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      958 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/machineprecision.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      749 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/migrad.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3772 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/minimumstate.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/minos.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3132 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/minuitparameter.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      811 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/print.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      293 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/printimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/scan.cpp
--rw-r--r--   0 runner    (1001) docker     (121)      544 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/simplex.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     3454 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/strategy.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/type_caster.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/usercovariance.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     6241 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/userparameterstate.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2594 2021-10-11 09:28:10.000000 iminuit-2.8.4/src/usertransformation.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-11 09:28:35.619011 iminuit-2.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/fmin_bad.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/fmin_good.txt
--rw-r--r--   0 runner    (1001) docker     (121)      228 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/matrix.txt
--rw-r--r--   0 runner    (1001) docker     (121)      252 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/matrix_difficult_values.txt
--rw-r--r--   0 runner    (1001) docker     (121)      200 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/matrix_large.txt
--rw-r--r--   0 runner    (1001) docker     (121)      660 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/matrix_long_names.txt
--rw-r--r--   0 runner    (1001) docker     (121)      116 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/matrix_mini.txt
--rw-r--r--   0 runner    (1001) docker     (121)      595 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/merror.txt
--rw-r--r--   0 runner    (1001) docker     (121)      977 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/merrors.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/params.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/params_difficult_values.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/params_long_names.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1146 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/params_with_limits.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6762 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)    14995 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/test_cost.py
--rw-r--r--   0 runner    (1001) docker     (121)      233 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (121)     3261 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/test_describe.py
--rw-r--r--   0 runner    (1001) docker     (121)     1776 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/test_draw.py
--rw-r--r--   0 runner    (1001) docker     (121)      388 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/test_experimental.py
--rw-r--r--   0 runner    (1001) docker     (121)     1548 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/test_fmin_bad.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1590 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2425 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/test_issue.py
--rw-r--r--   0 runner    (1001) docker     (121)     4098 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/test_minimize.py
--rw-r--r--   0 runner    (1001) docker     (121)    37832 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/test_minuit.py
--rw-r--r--   0 runner    (1001) docker     (121)    10021 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/test_pdg_format.py
--rw-r--r--   0 runner    (1001) docker     (121)    18595 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (121)     3856 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/test_repr_pretty.py
--rw-r--r--   0 runner    (1001) docker     (121)     6816 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/test_scipy.py
--rw-r--r--   0 runner    (1001) docker     (121)      993 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/test_tabulate.py
--rw-r--r--   0 runner    (1001) docker     (121)    14529 2021-10-11 09:28:10.000000 iminuit-2.8.4/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 14:13:19.922676 iminuit-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     4321 2022-01-09 14:12:36.000000 iminuit-2.9.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-01-09 14:12:36.000000 iminuit-2.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-01-09 14:12:36.000000 iminuit-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      537 2022-01-09 14:12:36.000000 iminuit-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5202 2022-01-09 14:13:19.922676 iminuit-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-01-09 14:12:36.000000 iminuit-2.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3217 2022-01-09 14:12:36.000000 iminuit-2.9.0/cmake_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 14:13:19.874676 iminuit-2.9.0/extern/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 14:13:19.878676 iminuit-2.9.0/extern/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (121)    10999 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1684 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 14:13:19.874676 iminuit-2.9.0/extern/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 14:13:19.878676 iminuit-2.9.0/extern/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (121)    23583 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6131 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (121)    60217 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8692 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 14:13:19.882676 iminuit-2.9.0/extern/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (121)    27922 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (121)    48395 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5005 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (121)    16970 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (121)    21551 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (121)    42206 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (121)    29875 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (121)    11645 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5493 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4600 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6520 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8882 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (121)    72120 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (121)     8771 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (121)   118217 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (121)    76321 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 14:13:19.882676 iminuit-2.9.0/extern/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (121)     3527 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (121)    13812 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (121)    26460 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 14:13:19.882676 iminuit-2.9.0/extern/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (121)     2295 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     3105 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     9977 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)    14579 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     9588 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (121)     7447 2022-01-09 14:13:10.000000 iminuit-2.9.0/extern/pybind11/tools/pybind11Tools.cmake
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 14:13:19.874676 iminuit-2.9.0/extern/root/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 14:13:19.874676 iminuit-2.9.0/extern/root/math/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 14:13:19.874676 iminuit-2.9.0/extern/root/math/minuit2/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 14:13:19.882676 iminuit-2.9.0/extern/root/math/minuit2/inc/
+-rw-r--r--   0 runner    (1001) docker     (121)     2299 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/LinkDef.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 14:13:19.898676 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/
+-rw-r--r--   0 runner    (1001) docker     (121)     3998 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ABObj.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1732 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ABProd.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2186 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ABSum.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1991 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ABTypes.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/AnalyticalGradientCalculator.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/BFGSErrorUpdator.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/CombinedMinimizer.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2039 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/CombinedMinimumBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2322 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ContoursError.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/DavidonErrorUpdator.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1873 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ExternalInternalGradientCalculator.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1424 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FCNAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3487 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FCNBase.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FCNGradAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FCNGradientBase.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3908 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4646 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliChi2FCN.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3090 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliErrorUpdator.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3991 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliFCNAdapter.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4452 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliFCNBase.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliGradientCalculator.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4510 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliMaximumLikelihoodFCN.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5835 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliMinimizer.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5632 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliStandardChi2FCN.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3505 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliStandardMaximumLikelihoodFCN.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FunctionGradient.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2723 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FunctionMinimizer.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4948 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FunctionMinimum.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1440 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/GenericFunction.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/GradientCalculator.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1968 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/HessianGradientCalculator.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1771 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/InitialGradientCalculator.h
+-rw-r--r--   0 runner    (1001) docker     (121)    14081 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/LASymMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (121)    11017 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/LAVector.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2746 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/LaInverse.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2828 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/LaOuterProduct.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2520 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/LaProd.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3278 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/LaSum.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4211 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MPIProcess.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1438 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MatrixInverse.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1829 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MinimumBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2962 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MinimumError.h
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MinimumErrorUpdator.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1792 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MinimumParameters.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1761 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MinimumSeed.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1393 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MinimumSeedGenerator.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3236 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MinimumState.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3392 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MinosError.h
+-rw-r--r--   0 runner    (1001) docker     (121)    13014 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/Minuit2Minimizer.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5347 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MinuitParameter.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4767 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnApplication.h
+-rw-r--r--   0 runner    (1001) docker     (121)      676 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnConfig.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2292 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnContours.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1209 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnCovarianceSqueeze.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3170 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnCross.h
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnEigen.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1756 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnFcn.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3977 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnFumiliMinimize.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1342 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnFunctionCross.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnGlobalCorrelationCoeff.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3593 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnHesse.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnLineSearch.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1898 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnMachinePrecision.h
+-rw-r--r--   0 runner    (1001) docker     (121)      952 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5422 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnMigrad.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5303 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnMinimize.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2446 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnMinos.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3476 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnParabola.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnParabolaFactory.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1661 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnParabolaPoint.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnParameterScan.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1446 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnPlot.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnPosDef.h
+-rw-r--r--   0 runner    (1001) docker     (121)     5569 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnPrint.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnRefCountedPointer.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1526 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnReferenceCounter.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3427 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnScan.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1262 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnSeedGenerator.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3587 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnSimplex.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2838 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnStrategy.h
+-rw-r--r--   0 runner    (1001) docker     (121)      799 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnTiny.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnTraceObject.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2704 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnUserCovariance.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnUserFcn.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6040 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnUserParameterState.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4228 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnUserParameters.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6363 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnUserTransformation.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnVectorTransform.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4744 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ModularFunctionMinimizer.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1375 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/NegativeG2LineSearch.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1932 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/Numerical2PGradientCalculator.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4880 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/NumericalDerivator.h
+-rw-r--r--   0 runner    (1001) docker     (121)     4425 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ParametricFunction.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ScanBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1472 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ScanMinimizer.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1157 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/SimplexBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1503 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/SimplexMinimizer.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1815 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/SimplexParameters.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/SimplexSeedGenerator.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1309 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/SinParameterTransformation.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1566 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/SqrtLowParameterTransformation.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/SqrtUpParameterTransformation.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6384 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/StackAllocator.h
+-rw-r--r--   0 runner    (1001) docker     (121)     2481 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/VariableMetricBuilder.h
+-rw-r--r--   0 runner    (1001) docker     (121)      936 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/VariableMetricEDMEstimator.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1805 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/VariableMetricMinimizer.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/VectorOuterProduct.h
+-rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/inc/TMinuit2TraceObject.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 14:13:19.910676 iminuit-2.9.0/extern/root/math/minuit2/src/
+-rw-r--r--   0 runner    (1001) docker     (121)     2341 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/AnalyticalGradientCalculator.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     4460 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/BFGSErrorUpdator.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/BasicMinimumError.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/CombinedMinimumBuilder.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     4896 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/DavidonErrorUpdator.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/ExternalInternalGradientCalculator.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)    12578 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/FumiliBuilder.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     3262 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/FumiliErrorUpdator.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     3975 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/FumiliGradientCalculator.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     3706 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/FumiliMinimizer.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     3483 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/FumiliStandardChi2FCN.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     5923 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/FumiliStandardMaximumLikelihoodFCN.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     4968 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/HessianGradientCalculator.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     3770 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/InitialGradientCalculator.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1347 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/LaEigenValues.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)      838 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/LaInnerProduct.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/LaInverse.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     2640 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/LaOuterProduct.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/LaSumOfElements.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/LaVtMVSimilarity.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)    10206 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MPIProcess.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MinimumBuilder.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)    44323 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/Minuit2Minimizer.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     6559 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnApplication.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     7308 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnContours.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     3493 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnCovarianceSqueeze.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnEigen.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnFcn.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnFumiliMinimize.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)    17186 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnFunctionCross.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1376 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnGlobalCorrelationCoeff.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)    15157 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnHesse.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)    25798 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnLineSearch.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnMachinePrecision.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     7207 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnMinos.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     2248 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnParabolaFactory.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     2590 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnParameterScan.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     2189 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnPlot.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     3308 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnPosDef.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)    13673 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnPrint.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)      828 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnPrintImpl.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnScan.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     6218 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnSeedGenerator.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnStrategy.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)      788 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnTiny.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnTraceObject.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnUserFcn.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)    18034 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnUserParameterState.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     5575 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnUserParameters.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)    17290 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/MnUserTransformation.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     9352 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/ModularFunctionMinimizer.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     4276 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/NegativeG2LineSearch.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     8456 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/Numerical2PGradientCalculator.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)    11256 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/NumericalDerivator.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1594 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/ParametricFunction.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1889 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/ScanBuilder.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     7882 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/SimplexBuilder.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/SimplexParameters.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     2234 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/SimplexSeedGenerator.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     2166 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/SinParameterTransformation.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1567 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/SqrtLowParameterTransformation.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1562 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/SqrtUpParameterTransformation.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     4072 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/TMinuit2TraceObject.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)    13571 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/VariableMetricBuilder.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/VariableMetricEDMEstimator.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     2768 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/mnbins.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     2402 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/mndasum.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     2304 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/mndaxpy.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     2418 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/mnddot.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/mndscal.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     9247 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/mndspmv.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     7151 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/mndspr.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     1869 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/mnlsame.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     6950 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/mnteigen.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     6393 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/mntplot.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/mnvert.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)     2296 2022-01-09 14:13:16.000000 iminuit-2.9.0/extern/root/math/minuit2/src/mnxerbla.cxx
+-rw-r--r--   0 runner    (1001) docker     (121)      947 2022-01-09 14:12:36.000000 iminuit-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2277 2022-01-09 14:13:19.922676 iminuit-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      305 2022-01-09 14:12:36.000000 iminuit-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 14:13:19.914676 iminuit-2.9.0/src/
+-rw-r--r--   0 runner    (1001) docker     (121)      487 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/application.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      678 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/contours.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      328 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/equal.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1576 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/equal.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     4305 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/fcn.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/fcn.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2268 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/functionminimum.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     5986 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/functionminimum_extra.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1478 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/functionminimum_pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/hesse.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 14:13:19.914676 iminuit-2.9.0/src/iminuit/
+-rw-r--r--   0 runner    (1001) docker     (121)      870 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/iminuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      539 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/iminuit/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9175 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/iminuit/_repr_html.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6335 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/iminuit/_repr_text.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27619 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/iminuit/cost.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/iminuit/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4467 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/iminuit/minimize.py
+-rw-r--r--   0 runner    (1001) docker     (121)    71531 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/iminuit/minuit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10255 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/iminuit/pdg_format.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1635 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/iminuit/testing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40811 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/iminuit/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)      587 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/iminuit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 14:13:19.914676 iminuit-2.9.0/src/iminuit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5202 2022-01-09 14:13:19.000000 iminuit-2.9.0/src/iminuit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    13123 2022-01-09 14:13:19.000000 iminuit-2.9.0/src/iminuit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-09 14:13:19.000000 iminuit-2.9.0/src/iminuit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-09 14:13:19.000000 iminuit-2.9.0/src/iminuit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      315 2022-01-09 14:13:19.000000 iminuit-2.9.0/src/iminuit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-01-09 14:13:19.000000 iminuit-2.9.0/src/iminuit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      481 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/lasymmatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/lasymmatrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)      383 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/lavector.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/lavector.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)      958 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/machineprecision.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/migrad.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3772 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/minimumstate.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/minos.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3132 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/minuitparameter.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      811 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/print.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/printimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      367 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/scan.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/simplex.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     3454 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/strategy.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/type_caster.hpp
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/usercovariance.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     6241 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/userparameterstate.cpp
+-rw-r--r--   0 runner    (1001) docker     (121)     2594 2022-01-09 14:12:36.000000 iminuit-2.9.0/src/usertransformation.cpp
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-09 14:13:19.922676 iminuit-2.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/fmin_bad.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/fmin_good.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/matrix.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/matrix_difficult_values.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/matrix_large.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/matrix_long_names.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/matrix_mini.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      595 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/merror.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      977 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/merrors.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/params.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/params_difficult_values.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/params_long_names.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1146 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/params_with_limits.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6762 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15699 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/test_cost.py
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3261 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/test_describe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1776 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/test_draw.py
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/test_experimental.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1548 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/test_fmin_bad.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2425 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/test_issue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4098 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/test_minimize.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37832 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/test_minuit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10021 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/test_pdg_format.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18595 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3856 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/test_repr_pretty.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6816 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/test_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      993 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/test_tabulate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14529 2022-01-09 14:12:36.000000 iminuit-2.9.0/tests/test_util.py
```

### Comparing `iminuit-2.8.4/CMakeLists.txt` & `iminuit-2.9.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/LICENSE` & `iminuit-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/MANIFEST.in` & `iminuit-2.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/PKG-INFO` & `iminuit-2.9.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,121 +1,125 @@
 Metadata-Version: 2.1
 Name: iminuit
-Version: 2.8.4
+Version: 2.9.0
 Summary: Jupyter-friendly Python frontend for MINUIT2 in C++
 Home-page: http://github.com/scikit-hep/iminuit
 Author: Piti Ongmongkolkul and the iminuit team
 Maintainer: Hans Dembinski
 Maintainer-email: hans.dembinski@gmail.com
 License: MIT+LGPL
 Download-URL: https://pypi.python.org/pypi/iminuit
 Project-URL: Documentation, https://iminuit.readthedocs.io
 Project-URL: Source Code, http://github.com/scikit-hep/iminuit
-Description: .. |iminuit| image:: doc/_static/iminuit_logo.svg
-           :alt: iminuit
-           :target: http://iminuit.readthedocs.io/en/latest
-        
-        |iminuit|
-        =========
-        
-        .. skip-marker-do-not-remove
-        
-        .. image:: https://scikit-hep.org/assets/images/Scikit--HEP-Project-blue.svg
-           :target: https://scikit-hep.org
-        .. image:: https://img.shields.io/pypi/v/iminuit.svg
-           :target: https://pypi.org/project/iminuit
-        .. image:: https://img.shields.io/conda/vn/conda-forge/iminuit.svg
-           :target: https://github.com/conda-forge/iminuit-feedstock
-        .. image:: https://coveralls.io/repos/github/scikit-hep/iminuit/badge.svg?branch=develop
-           :target: https://coveralls.io/github/scikit-hep/iminuit?branch=develop
-        .. image:: https://readthedocs.org/projects/iminuit/badge/?version=stable
-           :target: https://iminuit.readthedocs.io/en/stable
-        .. image:: https://img.shields.io/pypi/l/iminuit
-        .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3949207.svg
-           :target: https://doi.org/10.5281/zenodo.3949207
-        .. image:: https://img.shields.io/badge/ascl-2108.024-blue.svg?colorB=262255
-           :target: https://ascl.net/2108.024
-           :alt: ascl:2108.024
-        
-        *iminuit* is a Jupyter-friendly Python interface for the *Minuit2* C++ library maintained by CERN's ROOT team.
-        
-        Minuit was designed to minimise statistical cost functions, for likelihood and least-squares fits of parametric models to data. It provides the best-fit parameters and error estimates from likelihood profile analysis.
-        
-        - Supported CPython versions: 3.6+
-        - Supported PyPy versions: 3.6
-        - Supported platforms: Linux, OSX and Windows.
-        
-        The iminuit package comes with additional features:
-        
-        - Builtin cost functions for statistical fits
-        
-          - Binned and unbinned maximum-likelihood
-          - Non-linear regression with (optionally robust) weighted least-squares
-          - Gaussian penalty terms
-          - Cost functions can be combined by adding them: ``total_cost = cost_1 + cost_2``
-        - Tools for numerical error propagation ``iminuit.util.propagate``
-        - Support for SciPy minimisers as alternatives to Minuit's Migrad algorithm (optional)
-        - Support for Numba accelerated functions (optional)
-        
-        Checkout our large and comprehensive list of `tutorials`_ that take you all the way from beginner to power user. For help and how-to questions, please use the `discussions`_ on GitHub.
-        
-        .. image:: https://mybinder.org/badge_logo.svg
-           :target: https://mybinder.org/v2/gh/scikit-hep/iminuit/develop?filepath=doc%2Ftutorial
-        
-        In a nutshell
-        -------------
-        
-        .. code-block:: python
-        
-            from iminuit import Minuit
-        
-            def cost_function(x, y, z):
-                return (x - 2) ** 2 + (y - 3) ** 2 + (z - 4) ** 2
-        
-            fcn.errordef = Minuit.LEAST_SQUARES
-        
-            m = Minuit(cost_function, x=0, y=0, z=0)
-        
-            m.migrad()  # run optimiser
-            print(m.values)  # x: 2, y: 3, z: 4
-        
-            m.hesse()   # run covariance estimator
-            print(m.errors)  # x: 1, y: 1, z: 1
-        
-        Versions
-        --------
-        
-        **The current 2.x series has introduced breaking interfaces changes with respect to the 1.x series.**
-        
-        All interface changes are documented in the `changelog`_ with recommendations how to upgrade. To keep existing scripts running, pin your major iminuit version to <2, i.e. ``pip install 'iminuit<2'`` installs the 1.x series.
-        
-        .. _changelog: https://iminuit.readthedocs.io/en/stable/changelog.html
-        .. _tutorials: https://iminuit.readthedocs.io/en/stable/tutorials.html
-        .. _discussions: https://github.com/scikit-hep/iminuit/discussions
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: doc
+License-File: LICENSE
+
+.. |iminuit| image:: doc/_static/iminuit_logo.svg
+   :alt: iminuit
+   :target: http://iminuit.readthedocs.io/en/latest
+
+|iminuit|
+=========
+
+.. skip-marker-do-not-remove
+
+.. image:: https://scikit-hep.org/assets/images/Scikit--HEP-Project-blue.svg
+   :target: https://scikit-hep.org
+.. image:: https://img.shields.io/pypi/v/iminuit.svg
+   :target: https://pypi.org/project/iminuit
+.. image:: https://img.shields.io/conda/vn/conda-forge/iminuit.svg
+   :target: https://github.com/conda-forge/iminuit-feedstock
+.. image:: https://coveralls.io/repos/github/scikit-hep/iminuit/badge.svg?branch=develop
+   :target: https://coveralls.io/github/scikit-hep/iminuit?branch=develop
+.. image:: https://readthedocs.org/projects/iminuit/badge/?version=stable
+   :target: https://iminuit.readthedocs.io/en/stable
+.. image:: https://img.shields.io/pypi/l/iminuit
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3949207.svg
+   :target: https://doi.org/10.5281/zenodo.3949207
+.. image:: https://img.shields.io/badge/ascl-2108.024-blue.svg?colorB=262255
+   :target: https://ascl.net/2108.024
+   :alt: ascl:2108.024
+
+*iminuit* is a Jupyter-friendly Python interface for the *Minuit2* C++ library maintained by CERN's ROOT team.
+
+Minuit was designed to minimise statistical cost functions, for likelihood and least-squares fits of parametric models to data. It provides the best-fit parameters and error estimates from likelihood profile analysis.
+
+- Supported CPython versions: 3.6+
+- Supported PyPy versions: 3.6
+- Supported platforms: Linux, OSX and Windows.
+
+The iminuit package comes with additional features:
+
+- Builtin cost functions for statistical fits
+
+  - Binned and unbinned maximum-likelihood
+  - Non-linear regression with (optionally robust) weighted least-squares
+  - Gaussian penalty terms
+  - Cost functions can be combined by adding them: ``total_cost = cost_1 + cost_2``
+- Tools for numerical error propagation ``iminuit.util.propagate``
+- Support for SciPy minimisers as alternatives to Minuit's Migrad algorithm (optional)
+- Support for Numba accelerated functions (optional)
+
+Checkout our large and comprehensive list of `tutorials`_ that take you all the way from beginner to power user. For help and how-to questions, please use the `discussions`_ on GitHub.
+
+.. image:: https://mybinder.org/badge_logo.svg
+   :target: https://mybinder.org/v2/gh/scikit-hep/iminuit/develop?filepath=doc%2Ftutorial
+
+In a nutshell
+-------------
+
+.. code-block:: python
+
+    from iminuit import Minuit
+
+    def cost_function(x, y, z):
+        return (x - 2) ** 2 + (y - 3) ** 2 + (z - 4) ** 2
+
+    cost_function.errordef = Minuit.LEAST_SQUARES
+
+    m = Minuit(cost_function, x=0, y=0, z=0)
+
+    m.migrad()  # run optimiser
+    print(m.values)  # x: 2, y: 3, z: 4
+
+    m.hesse()   # run covariance estimator
+    print(m.errors)  # x: 1, y: 1, z: 1
+
+Versions
+--------
+
+**The current 2.x series has introduced breaking interfaces changes with respect to the 1.x series.**
+
+All interface changes are documented in the `changelog`_ with recommendations how to upgrade. To keep existing scripts running, pin your major iminuit version to <2, i.e. ``pip install 'iminuit<2'`` installs the 1.x series.
+
+.. _changelog: https://iminuit.readthedocs.io/en/stable/changelog.html
+.. _tutorials: https://iminuit.readthedocs.io/en/stable/tutorials.html
+.. _discussions: https://github.com/scikit-hep/iminuit/discussions
+
+
```

### Comparing `iminuit-2.8.4/README.rst` & `iminuit-2.9.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 .. code-block:: python
 
     from iminuit import Minuit
 
     def cost_function(x, y, z):
         return (x - 2) ** 2 + (y - 3) ** 2 + (z - 4) ** 2
 
-    fcn.errordef = Minuit.LEAST_SQUARES
+    cost_function.errordef = Minuit.LEAST_SQUARES
 
     m = Minuit(cost_function, x=0, y=0, z=0)
 
     m.migrad()  # run optimiser
     print(m.values)  # x: 2, y: 3, z: 4
 
     m.hesse()   # run covariance estimator
```

### Comparing `iminuit-2.8.4/cmake_ext.py` & `iminuit-2.9.0/cmake_ext.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/pybind11/CMakeLists.txt` & `iminuit-2.9.0/extern/pybind11/CMakeLists.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,26 @@
 # Copyright (c) 2015 Wenzel Jakob <wenzel@inf.ethz.ch>
 #
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 
 cmake_minimum_required(VERSION 3.4)
 
-# The `cmake_minimum_required(VERSION 3.4...3.18)` syntax does not work with
+# The `cmake_minimum_required(VERSION 3.4...3.22)` syntax does not work with
 # some versions of VS that have a patched CMake 3.11. This forces us to emulate
 # the behavior using the following workaround:
-if(${CMAKE_VERSION} VERSION_LESS 3.18)
+if(${CMAKE_VERSION} VERSION_LESS 3.22)
   cmake_policy(VERSION ${CMAKE_MAJOR_VERSION}.${CMAKE_MINOR_VERSION})
 else()
-  cmake_policy(VERSION 3.18)
+  cmake_policy(VERSION 3.22)
+endif()
+
+# Avoid infinite recursion if tests include this as a subdirectory
+if(DEFINED PYBIND11_MASTER_PROJECT)
+  return()
 endif()
 
 # Extract project version from source
 file(STRINGS "${CMAKE_CURRENT_SOURCE_DIR}/include/pybind11/detail/common.h"
      pybind11_version_defines REGEX "#define PYBIND11_VERSION_(MAJOR|MINOR|PATCH) ")
 
 foreach(ver ${pybind11_version_defines})
@@ -41,21 +46,16 @@
 include(CMakePackageConfigHelpers)
 include(CMakeDependentOption)
 
 if(NOT pybind11_FIND_QUIETLY)
   message(STATUS "pybind11 v${pybind11_VERSION} ${pybind11_VERSION_TYPE}")
 endif()
 
-# Avoid infinite recursion if tests include this as a subdirectory
-if(DEFINED PYBIND11_MASTER_PROJECT)
-  set(PYBIND11_TEST OFF)
-endif()
-
 # Check if pybind11 is being used directly or via add_subdirectory
-if(CMAKE_SOURCE_DIR STREQUAL PROJECT_SOURCE_DIR AND NOT DEFINED PYBIND11_MASTER_PROJECT)
+if(CMAKE_SOURCE_DIR STREQUAL PROJECT_SOURCE_DIR)
   ### Warn if not an out-of-source builds
   if(CMAKE_CURRENT_SOURCE_DIR STREQUAL CMAKE_CURRENT_BINARY_DIR)
     set(lines
         "You are building in-place. If that is not what you intended to "
         "do, you can clean the source directory with:\n"
         "rm -r CMakeCache.txt CMakeFiles/ cmake_uninstall.cmake pybind11Config.cmake "
         "pybind11ConfigVersion.cmake tests/CMakeFiles/\n")
@@ -76,23 +76,28 @@
 
   if(CMAKE_CXX_STANDARD)
     set(CMAKE_CXX_EXTENSIONS OFF)
     set(CMAKE_CXX_STANDARD_REQUIRED ON)
   endif()
 
   set(pybind11_system "")
+
+  set_property(GLOBAL PROPERTY USE_FOLDERS ON)
 else()
   set(PYBIND11_MASTER_PROJECT OFF)
   set(pybind11_system SYSTEM)
 endif()
 
 # Options
 option(PYBIND11_INSTALL "Install pybind11 header files?" ${PYBIND11_MASTER_PROJECT})
 option(PYBIND11_TEST "Build pybind11 test suite?" ${PYBIND11_MASTER_PROJECT})
 option(PYBIND11_NOPYTHON "Disable search for Python" OFF)
+set(PYBIND11_INTERNALS_VERSION
+    ""
+    CACHE STRING "Override the ABI version, may be used to enable the unstable ABI.")
 
 cmake_dependent_option(
   USE_PYTHON_INCLUDE_DIR
   "Install pybind11 headers in Python include directory instead of default installation prefix"
   OFF "PYBIND11_INSTALL" OFF)
 
 cmake_dependent_option(PYBIND11_FINDPYTHON "Force new FindPython" OFF
@@ -101,33 +106,36 @@
 # NB: when adding a header don't forget to also add it to setup.py
 set(PYBIND11_HEADERS
     include/pybind11/detail/class.h
     include/pybind11/detail/common.h
     include/pybind11/detail/descr.h
     include/pybind11/detail/init.h
     include/pybind11/detail/internals.h
+    include/pybind11/detail/type_caster_base.h
     include/pybind11/detail/typeid.h
     include/pybind11/attr.h
     include/pybind11/buffer_info.h
     include/pybind11/cast.h
     include/pybind11/chrono.h
     include/pybind11/common.h
     include/pybind11/complex.h
     include/pybind11/options.h
     include/pybind11/eigen.h
     include/pybind11/embed.h
     include/pybind11/eval.h
+    include/pybind11/gil.h
     include/pybind11/iostream.h
     include/pybind11/functional.h
     include/pybind11/numpy.h
     include/pybind11/operators.h
     include/pybind11/pybind11.h
     include/pybind11/pytypes.h
     include/pybind11/stl.h
-    include/pybind11/stl_bind.h)
+    include/pybind11/stl_bind.h
+    include/pybind11/stl/filesystem.h)
 
 # Compare with grep and warn if mismatched
 if(PYBIND11_MASTER_PROJECT AND NOT CMAKE_VERSION VERSION_LESS 3.12)
   file(
     GLOB_RECURSE _pybind11_header_check
     LIST_DIRECTORIES false
     RELATIVE "${CMAKE_CURRENT_SOURCE_DIR}"
@@ -176,14 +184,18 @@
 
   target_include_directories(
     pybind11_headers ${pybind11_system} INTERFACE $<BUILD_INTERFACE:${pybind11_INCLUDE_DIR}>
                                                   $<INSTALL_INTERFACE:${CMAKE_INSTALL_INCLUDEDIR}>)
 
   target_compile_features(pybind11_headers INTERFACE cxx_inheriting_constructors cxx_user_literals
                                                      cxx_right_angle_brackets)
+  if(NOT "${PYBIND11_INTERNALS_VERSION}" STREQUAL "")
+    target_compile_definitions(
+      pybind11_headers INTERFACE "PYBIND11_INTERNALS_VERSION=${PYBIND11_INTERNALS_VERSION}")
+  endif()
 else()
   # It is invalid to install a target twice, too.
   set(PYBIND11_INSTALL OFF)
 endif()
 
 include("${CMAKE_CURRENT_SOURCE_DIR}/tools/pybind11Common.cmake")
 
@@ -196,14 +208,20 @@
 
 if(PYBIND11_INSTALL)
   install(DIRECTORY ${pybind11_INCLUDE_DIR}/pybind11 DESTINATION ${CMAKE_INSTALL_INCLUDEDIR})
   set(PYBIND11_CMAKECONFIG_INSTALL_DIR
       "${CMAKE_INSTALL_DATAROOTDIR}/cmake/${PROJECT_NAME}"
       CACHE STRING "install path for pybind11Config.cmake")
 
+  if(IS_ABSOLUTE "${CMAKE_INSTALL_INCLUDEDIR}")
+    set(pybind11_INCLUDEDIR "${CMAKE_INSTALL_FULL_INCLUDEDIR}")
+  else()
+    set(pybind11_INCLUDEDIR "\$\{PACKAGE_PREFIX_DIR\}/${CMAKE_INSTALL_INCLUDEDIR}")
+  endif()
+
   configure_package_config_file(
     tools/${PROJECT_NAME}Config.cmake.in "${CMAKE_CURRENT_BINARY_DIR}/${PROJECT_NAME}Config.cmake"
     INSTALL_DESTINATION ${PYBIND11_CMAKECONFIG_INSTALL_DIR})
 
   if(CMAKE_VERSION VERSION_LESS 3.14)
     # Remove CMAKE_SIZEOF_VOID_P from ConfigVersion.cmake since the library does
     # not depend on architecture specific settings or libraries.
```

### Comparing `iminuit-2.8.4/extern/pybind11/LICENSE` & `iminuit-2.9.0/extern/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/attr.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/attr.h`

 * *Files 5% similar despite different names*

```diff
@@ -8,39 +8,51 @@
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "cast.h"
 
+#include <functional>
+
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
 /// \addtogroup annotations
 /// @{
 
 /// Annotation for methods
-struct is_method { handle class_; is_method(const handle &c) : class_(c) { } };
+struct is_method { handle class_;
+    explicit is_method(const handle &c) : class_(c) {}
+};
 
 /// Annotation for operators
 struct is_operator { };
 
 /// Annotation for classes that cannot be subclassed
 struct is_final { };
 
 /// Annotation for parent scope
-struct scope { handle value; scope(const handle &s) : value(s) { } };
+struct scope { handle value;
+    explicit scope(const handle &s) : value(s) {}
+};
 
 /// Annotation for documentation
-struct doc { const char *value; doc(const char *value) : value(value) { } };
+struct doc { const char *value;
+    explicit doc(const char *value) : value(value) {}
+};
 
 /// Annotation for function names
-struct name { const char *value; name(const char *value) : value(value) { } };
+struct name { const char *value;
+    explicit name(const char *value) : value(value) {}
+};
 
 /// Annotation indicating that a function is an overload associated with a given "sibling"
-struct sibling { handle value; sibling(const handle &value) : value(value.ptr()) { } };
+struct sibling { handle value;
+    explicit sibling(const handle &value) : value(value.ptr()) {}
+};
 
 /// Annotation indicating that a class derives from another given type
 template <typename T> struct base {
 
     PYBIND11_DEPRECATED("base<T>() was deprecated in favor of specifying 'T' as a template argument to class_")
     base() { } // NOLINT(modernize-use-equals-default): breaks MSVC 2015 when adding an attribute
 };
@@ -58,22 +70,42 @@
 struct buffer_protocol { };
 
 /// Annotation which requests that a special metaclass is created for a type
 struct metaclass {
     handle value;
 
     PYBIND11_DEPRECATED("py::metaclass() is no longer required. It's turned on by default now.")
-    metaclass() { } // NOLINT(modernize-use-equals-default): breaks MSVC 2015 when adding an attribute
+    // NOLINTNEXTLINE(modernize-use-equals-default): breaks MSVC 2015 when adding an attribute
+    metaclass() {}
 
     /// Override pybind11's default metaclass
     explicit metaclass(handle value) : value(value) { }
 };
 
+/// Specifies a custom callback with signature `void (PyHeapTypeObject*)` that
+/// may be used to customize the Python type.
+///
+/// The callback is invoked immediately before `PyType_Ready`.
+///
+/// Note: This is an advanced interface, and uses of it may require changes to
+/// work with later versions of pybind11.  You may wish to consult the
+/// implementation of `make_new_python_type` in `detail/classes.h` to understand
+/// the context in which the callback will be run.
+struct custom_type_setup {
+    using callback = std::function<void(PyHeapTypeObject *heap_type)>;
+
+    explicit custom_type_setup(callback value) : value(std::move(value)) {}
+
+    callback value;
+};
+
 /// Annotation that marks a class as local to the module:
-struct module_local { const bool value; constexpr module_local(bool v = true) : value(v) { } };
+struct module_local { const bool value;
+    constexpr explicit module_local(bool v = true) : value(v) {}
+};
 
 /// Annotation to mark enums as an arithmetic type
 struct arithmetic { };
 
 /// Mark a function for addition at the beginning of the existing overload chain instead of the end
 struct prepend { };
 
@@ -119,15 +151,15 @@
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 /* Forward declarations */
 enum op_id : int;
 enum op_type : int;
 struct undefined_t;
 template <op_id id, op_type ot, typename L = undefined_t, typename R = undefined_t> struct op_;
-inline void keep_alive_impl(size_t Nurse, size_t Patient, function_call &call, handle ret);
+void keep_alive_impl(size_t Nurse, size_t Patient, function_call &call, handle ret);
 
 /// Internal data structure which holds metadata about a keyword argument
 struct argument_record {
     const char *name;  ///< Argument name
     const char *descr; ///< Human-readable version of the argument value
     handle value;      ///< Associated Python object
     bool convert : 1;  ///< True if the argument is allowed to convert when loading
@@ -138,15 +170,15 @@
 };
 
 /// Internal data structure which holds metadata about a bound function (signature, overloads, etc.)
 struct function_record {
     function_record()
         : is_constructor(false), is_new_style_constructor(false), is_stateless(false),
           is_operator(false), is_method(false), has_args(false),
-          has_kwargs(false), has_kw_only_args(false), prepend(false) { }
+          has_kwargs(false), prepend(false) { }
 
     /// Function name
     char *name = nullptr; /* why no C++ strings? They generate heavier code.. */
 
     // User-specified documentation string
     char *doc = nullptr;
 
@@ -185,25 +217,23 @@
 
     /// True if the function has a '*args' argument
     bool has_args : 1;
 
     /// True if the function has a '**kwargs' argument
     bool has_kwargs : 1;
 
-    /// True once a 'py::kw_only' is encountered (any following args are keyword-only)
-    bool has_kw_only_args : 1;
-
     /// True if this function is to be inserted at the beginning of the overload resolution chain
     bool prepend : 1;
 
     /// Number of arguments (including py::args and/or py::kwargs, if present)
     std::uint16_t nargs;
 
-    /// Number of trailing arguments (counted in `nargs`) that are keyword-only
-    std::uint16_t nargs_kw_only = 0;
+    /// Number of leading positional arguments, which are terminated by a py::args or py::kwargs
+    /// argument or by a py::kw_only annotation.
+    std::uint16_t nargs_pos = 0;
 
     /// Number of leading arguments (counted in `nargs`) that are positional-only
     std::uint16_t nargs_pos_only = 0;
 
     /// Python method object
     PyMethodDef *def = nullptr;
 
@@ -255,14 +285,17 @@
 
     /// Optional docstring
     const char *doc = nullptr;
 
     /// Custom metaclass (optional)
     handle metaclass;
 
+    /// Custom type setup.
+    custom_type_setup::callback custom_type_setup_callback;
+
     /// Multiple inheritance marker
     bool multiple_inheritance : 1;
 
     /// Does the class manage a __dict__?
     bool dynamic_attr : 1;
 
     /// Does the class implement the buffer protocol?
@@ -372,36 +405,39 @@
     static void init(const is_operator &, function_record *r) { r->is_operator = true; }
 };
 
 template <> struct process_attribute<is_new_style_constructor> : process_attribute_default<is_new_style_constructor> {
     static void init(const is_new_style_constructor &, function_record *r) { r->is_new_style_constructor = true; }
 };
 
-inline void process_kw_only_arg(const arg &a, function_record *r) {
-    if (!a.name || strlen(a.name) == 0)
-        pybind11_fail("arg(): cannot specify an unnamed argument after an kw_only() annotation");
-    ++r->nargs_kw_only;
+inline void check_kw_only_arg(const arg &a, function_record *r) {
+    if (r->args.size() > r->nargs_pos && (!a.name || a.name[0] == '\0'))
+        pybind11_fail("arg(): cannot specify an unnamed argument after a kw_only() annotation or args() argument");
+}
+
+inline void append_self_arg_if_needed(function_record *r) {
+    if (r->is_method && r->args.empty())
+        r->args.emplace_back("self", nullptr, handle(), /*convert=*/ true, /*none=*/ false);
 }
 
 /// Process a keyword argument attribute (*without* a default value)
 template <> struct process_attribute<arg> : process_attribute_default<arg> {
     static void init(const arg &a, function_record *r) {
-        if (r->is_method && r->args.empty())
-            r->args.emplace_back("self", nullptr, handle(), true /*convert*/, false /*none not allowed*/);
+        append_self_arg_if_needed(r);
         r->args.emplace_back(a.name, nullptr, handle(), !a.flag_noconvert, a.flag_none);
 
-        if (r->has_kw_only_args) process_kw_only_arg(a, r);
+        check_kw_only_arg(a, r);
     }
 };
 
 /// Process a keyword argument attribute (*with* a default value)
 template <> struct process_attribute<arg_v> : process_attribute_default<arg_v> {
     static void init(const arg_v &a, function_record *r) {
         if (r->is_method && r->args.empty())
-            r->args.emplace_back("self", nullptr /*descr*/, handle() /*parent*/, true /*convert*/, false /*none not allowed*/);
+            r->args.emplace_back("self", /*descr=*/ nullptr, /*parent=*/ handle(), /*convert=*/ true, /*none=*/ false);
 
         if (!a.value) {
 #if !defined(NDEBUG)
             std::string descr("'");
             if (a.name) descr += std::string(a.name) + ": ";
             descr += a.type + "'";
             if (r->is_method) {
@@ -418,29 +454,36 @@
             pybind11_fail("arg(): could not convert default argument "
                           "into a Python object (type not registered yet?). "
                           "Compile in debug mode for more information.");
 #endif
         }
         r->args.emplace_back(a.name, a.descr, a.value.inc_ref(), !a.flag_noconvert, a.flag_none);
 
-        if (r->has_kw_only_args) process_kw_only_arg(a, r);
+        check_kw_only_arg(a, r);
     }
 };
 
 /// Process a keyword-only-arguments-follow pseudo argument
 template <> struct process_attribute<kw_only> : process_attribute_default<kw_only> {
     static void init(const kw_only &, function_record *r) {
-        r->has_kw_only_args = true;
+        append_self_arg_if_needed(r);
+        if (r->has_args && r->nargs_pos != static_cast<std::uint16_t>(r->args.size()))
+            pybind11_fail("Mismatched args() and kw_only(): they must occur at the same relative argument location (or omit kw_only() entirely)");
+        r->nargs_pos = static_cast<std::uint16_t>(r->args.size());
     }
 };
 
 /// Process a positional-only-argument maker
 template <> struct process_attribute<pos_only> : process_attribute_default<pos_only> {
     static void init(const pos_only &, function_record *r) {
+        append_self_arg_if_needed(r);
         r->nargs_pos_only = static_cast<std::uint16_t>(r->args.size());
+        if (r->nargs_pos_only > r->nargs_pos)
+            pybind11_fail("pos_only(): cannot follow a py::args() argument");
+            // It also can't follow a kw_only, but a static_assert in pybind11.h checks that
     }
 };
 
 /// Process a parent class attribute.  Single inheritance only (class_ itself already guarantees that)
 template <typename T>
 struct process_attribute<T, enable_if_t<is_pyobject<T>::value>> : process_attribute_default<handle> {
     static void init(const handle &h, type_record *r) { r->bases.append(h); }
@@ -460,14 +503,21 @@
 
 template <>
 struct process_attribute<dynamic_attr> : process_attribute_default<dynamic_attr> {
     static void init(const dynamic_attr &, type_record *r) { r->dynamic_attr = true; }
 };
 
 template <>
+struct process_attribute<custom_type_setup> {
+    static void init(const custom_type_setup &value, type_record *r) {
+        r->custom_type_setup_callback = value.value;
+    }
+};
+
+template <>
 struct process_attribute<is_final> : process_attribute_default<is_final> {
     static void init(const is_final &, type_record *r) { r->is_final = true; }
 };
 
 template <>
 struct process_attribute<buffer_protocol> : process_attribute_default<buffer_protocol> {
     static void init(const buffer_protocol &, type_record *r) { r->buffer_protocol = true; }
@@ -511,28 +561,39 @@
     template <size_t N = Nurse, size_t P = Patient, enable_if_t<N == 0 || P == 0, int> = 0>
     static void postcall(function_call &call, handle ret) { keep_alive_impl(Nurse, Patient, call, ret); }
 };
 
 /// Recursively iterate over variadic template arguments
 template <typename... Args> struct process_attributes {
     static void init(const Args&... args, function_record *r) {
-        int unused[] = { 0, (process_attribute<typename std::decay<Args>::type>::init(args, r), 0) ... };
-        ignore_unused(unused);
+        PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(r);
+        PYBIND11_WORKAROUND_INCORRECT_GCC_UNUSED_BUT_SET_PARAMETER(r);
+        using expander = int[];
+        (void) expander{
+            0, ((void) process_attribute<typename std::decay<Args>::type>::init(args, r), 0)...};
     }
     static void init(const Args&... args, type_record *r) {
-        int unused[] = { 0, (process_attribute<typename std::decay<Args>::type>::init(args, r), 0) ... };
-        ignore_unused(unused);
+        PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(r);
+        PYBIND11_WORKAROUND_INCORRECT_GCC_UNUSED_BUT_SET_PARAMETER(r);
+        using expander = int[];
+        (void) expander{0,
+                        (process_attribute<typename std::decay<Args>::type>::init(args, r), 0)...};
     }
     static void precall(function_call &call) {
-        int unused[] = { 0, (process_attribute<typename std::decay<Args>::type>::precall(call), 0) ... };
-        ignore_unused(unused);
+        PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(call);
+        using expander = int[];
+        (void) expander{0,
+                        (process_attribute<typename std::decay<Args>::type>::precall(call), 0)...};
     }
     static void postcall(function_call &call, handle fn_ret) {
-        int unused[] = { 0, (process_attribute<typename std::decay<Args>::type>::postcall(call, fn_ret), 0) ... };
-        ignore_unused(unused);
+        PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(call, fn_ret);
+        PYBIND11_WORKAROUND_INCORRECT_GCC_UNUSED_BUT_SET_PARAMETER(fn_ret);
+        using expander = int[];
+        (void) expander{
+            0, (process_attribute<typename std::decay<Args>::type>::postcall(call, fn_ret), 0)...};
     }
 };
 
 template <typename T>
 using is_call_guard = is_instantiation<call_guard, T>;
 
 /// Extract the ``type`` from the first `call_guard` in `Extras...` (or `void_type` if none found)
@@ -540,12 +601,13 @@
 using extract_guard_t = typename exactly_one_t<is_call_guard, call_guard<>, Extra...>::type;
 
 /// Check the number of named arguments at compile time
 template <typename... Extra,
           size_t named = constexpr_sum(std::is_base_of<arg, Extra>::value...),
           size_t self  = constexpr_sum(std::is_same<is_method, Extra>::value...)>
 constexpr bool expected_num_args(size_t nargs, bool has_args, bool has_kwargs) {
+    PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(nargs, has_args, has_kwargs);
     return named == 0 || (self + named + size_t(has_args) + size_t(has_kwargs)) == nargs;
 }
 
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/buffer_info.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/buffer_info.h`

 * *Files 4% similar despite different names*

```diff
@@ -79,27 +79,25 @@
             {view->shape, view->shape + view->ndim},
             /* Though buffer::request() requests PyBUF_STRIDES, ctypes objects
              * ignore this flag and return a view with NULL strides.
              * When strides are NULL, build them manually.  */
             view->strides
             ? std::vector<ssize_t>(view->strides, view->strides + view->ndim)
             : detail::c_strides({view->shape, view->shape + view->ndim}, view->itemsize),
-            view->readonly) {
+            (view->readonly != 0)) {
         this->m_view = view;
         this->ownview = ownview;
     }
 
     buffer_info(const buffer_info &) = delete;
     buffer_info& operator=(const buffer_info &) = delete;
 
-    buffer_info(buffer_info &&other) {
-        (*this) = std::move(other);
-    }
+    buffer_info(buffer_info &&other) noexcept { (*this) = std::move(other); }
 
-    buffer_info& operator=(buffer_info &&rhs) {
+    buffer_info &operator=(buffer_info &&rhs) noexcept {
         ptr = rhs.ptr;
         itemsize = rhs.itemsize;
         size = rhs.size;
         format = std::move(rhs.format);
         ndim = rhs.ndim;
         shape = std::move(rhs.shape);
         strides = std::move(rhs.strides);
```

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/chrono.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/chrono.h`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,22 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "pybind11.h"
+
+#include <chrono>
 #include <cmath>
 #include <ctime>
-#include <chrono>
+#include <mutex>
+
+#include <time.h>
+
 #include <datetime.h>
 
 // Backport the PyDateTime_DELTA functions from Python3.3 if required
 #ifndef PyDateTime_DELTA_GET_DAYS
 #define PyDateTime_DELTA_GET_DAYS(o)         (((PyDateTime_Delta*)o)->days)
 #endif
 #ifndef PyDateTime_DELTA_GET_SECONDS
@@ -31,15 +36,15 @@
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 template <typename type> class duration_caster {
 public:
     using rep = typename type::rep;
     using period = typename type::period;
 
-    using days = std::chrono::duration<uint_fast32_t, std::ratio<86400>>;
+    using days = std::chrono::duration<int_least32_t, std::ratio<86400>>; // signed 25 bits required by the standard.
 
     bool load(handle src, bool) {
         using namespace std::chrono;
 
         // Lazy initialise the PyDateTime import
         if (!PyDateTimeAPI) { PyDateTime_IMPORT; }
 
@@ -49,19 +54,19 @@
             value = type(duration_cast<duration<rep, period>>(
                   days(PyDateTime_DELTA_GET_DAYS(src.ptr()))
                 + seconds(PyDateTime_DELTA_GET_SECONDS(src.ptr()))
                 + microseconds(PyDateTime_DELTA_GET_MICROSECONDS(src.ptr()))));
             return true;
         }
         // If invoked with a float we assume it is seconds and convert
-        else if (PyFloat_Check(src.ptr())) {
+        if (PyFloat_Check(src.ptr())) {
             value = type(duration_cast<duration<rep, period>>(duration<double>(PyFloat_AsDouble(src.ptr()))));
             return true;
         }
-        else return false;
+        return false;
     }
 
     // If this is a duration just return it back
     static const std::chrono::duration<rep, period>& get_duration(const std::chrono::duration<rep, period> &src) {
         return src;
     }
 
@@ -88,17 +93,33 @@
         auto dd = duration_cast<dd_t>(d);
         auto subd = d - dd;
         auto ss = duration_cast<ss_t>(subd);
         auto us = duration_cast<us_t>(subd - ss);
         return PyDelta_FromDSU(dd.count(), ss.count(), us.count());
     }
 
-    PYBIND11_TYPE_CASTER(type, _("datetime.timedelta"));
+    PYBIND11_TYPE_CASTER(type, const_name("datetime.timedelta"));
 };
 
+inline std::tm *localtime_thread_safe(const std::time_t *time, std::tm *buf) {
+#if (defined(__STDC_LIB_EXT1__) && defined(__STDC_WANT_LIB_EXT1__)) || defined(_MSC_VER)
+    if (localtime_s(buf, time))
+        return nullptr;
+    return buf;
+#else
+    static std::mutex mtx;
+    std::lock_guard<std::mutex> lock(mtx);
+    std::tm *tm_ptr = localtime(time);
+    if (tm_ptr != nullptr) {
+        *buf = *tm_ptr;
+    }
+    return tm_ptr;
+#endif
+}
+
 // This is for casting times on the system clock into datetime.datetime instances
 template <typename Duration> class type_caster<std::chrono::time_point<std::chrono::system_clock, Duration>> {
 public:
     using type = std::chrono::time_point<std::chrono::system_clock, Duration>;
     bool load(handle src, bool) {
         using namespace std::chrono;
 
@@ -157,27 +178,28 @@
         if (us.count() < 0)
             us += seconds(1);
 
         // Subtract microseconds BEFORE `system_clock::to_time_t`, because:
         // > If std::time_t has lower precision, it is implementation-defined whether the value is rounded or truncated.
         // (https://en.cppreference.com/w/cpp/chrono/system_clock/to_time_t)
         std::time_t tt = system_clock::to_time_t(time_point_cast<system_clock::duration>(src - us));
-        // this function uses static memory so it's best to copy it out asap just in case
-        // otherwise other code that is using localtime may break this (not just python code)
-        std::tm localtime = *std::localtime(&tt);
 
+        std::tm localtime;
+        std::tm *localtime_ptr = localtime_thread_safe(&tt, &localtime);
+        if (!localtime_ptr)
+            throw cast_error("Unable to represent system_clock in local time");
         return PyDateTime_FromDateAndTime(localtime.tm_year + 1900,
                                           localtime.tm_mon + 1,
                                           localtime.tm_mday,
                                           localtime.tm_hour,
                                           localtime.tm_min,
                                           localtime.tm_sec,
                                           us.count());
     }
-    PYBIND11_TYPE_CASTER(type, _("datetime.datetime"));
+    PYBIND11_TYPE_CASTER(type, const_name("datetime.datetime"));
 };
 
 // Other clocks that are not the system clock are not measured as datetime.datetime objects
 // since they are not measured on calendar time. So instead we just make them timedeltas
 // Or if they have passed us a time as a float we convert that
 template <typename Clock, typename Duration> class type_caster<std::chrono::time_point<Clock, Duration>>
 : public duration_caster<std::chrono::time_point<Clock, Duration>> {
```

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/complex.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/complex.h`

 * *Files 9% similar despite different names*

```diff
@@ -55,11 +55,11 @@
         return true;
     }
 
     static handle cast(const std::complex<T> &src, return_value_policy /* policy */, handle /* parent */) {
         return PyComplex_FromDoubles((double) src.real(), (double) src.imag());
     }
 
-    PYBIND11_TYPE_CASTER(std::complex<T>, _("complex"));
+    PYBIND11_TYPE_CASTER(std::complex<T>, const_name("complex"));
 };
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/detail/class.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/detail/class.h`

 * *Files 0% similar despite different names*

```diff
@@ -125,16 +125,17 @@
     PyObject *descr = _PyType_Lookup((PyTypeObject *) obj, name);
 
     // The following assignment combinations are possible:
     //   1. `Type.static_prop = value`             --> descr_set: `Type.static_prop.__set__(value)`
     //   2. `Type.static_prop = other_static_prop` --> setattro:  replace existing `static_prop`
     //   3. `Type.regular_attribute = value`       --> setattro:  regular attribute assignment
     const auto static_prop = (PyObject *) get_internals().static_property_type;
-    const auto call_descr_set = descr && value && PyObject_IsInstance(descr, static_prop)
-                                && !PyObject_IsInstance(value, static_prop);
+    const auto call_descr_set = (descr != nullptr) && (value != nullptr)
+                                && (PyObject_IsInstance(descr, static_prop) != 0)
+                                && (PyObject_IsInstance(value, static_prop) == 0);
     if (call_descr_set) {
         // Call `static_property.__set__()` instead of replacing the `static_property`.
 #if !defined(PYPY_VERSION)
         return Py_TYPE(descr)->tp_descr_set(descr, obj, value);
 #else
         if (PyObject *result = PyObject_CallMethod(descr, "__set__", "OO", obj, value)) {
             Py_DECREF(result);
@@ -158,17 +159,15 @@
  */
 extern "C" inline PyObject *pybind11_meta_getattro(PyObject *obj, PyObject *name) {
     PyObject *descr = _PyType_Lookup((PyTypeObject *) obj, name);
     if (descr && PyInstanceMethod_Check(descr)) {
         Py_INCREF(descr);
         return descr;
     }
-    else {
-        return PyType_Type.tp_getattro(obj, name);
-    }
+    return PyType_Type.tp_getattro(obj, name);
 }
 #endif
 
 /// metaclass `__call__` function that is used to create all pybind11 objects.
 extern "C" inline PyObject *pybind11_meta_call(PyObject *type, PyObject *args, PyObject *kwargs) {
 
     // use the default metaclass call to create/initialize the object
@@ -207,15 +206,15 @@
         found_type->second[0]->type == type) {
 
         auto *tinfo = found_type->second[0];
         auto tindex = std::type_index(*tinfo->cpptype);
         internals.direct_conversions.erase(tindex);
 
         if (tinfo->module_local)
-            registered_local_types_cpp().erase(tindex);
+            get_local_internals().registered_types_cpp.erase(tindex);
         else
             internals.registered_types_cpp.erase(tindex);
         internals.registered_types_py.erase(tinfo->type);
 
         // Actually just `std::erase_if`, but that's only available in C++20
         auto &cache = internals.inactive_override_cache;
         for (auto it = cache.begin(), last = cache.end(); it != last; ) {
@@ -325,15 +324,15 @@
 
 /// Instance creation function for all pybind11 types. It allocates the internal instance layout for
 /// holding C++ objects and holders.  Allocation is done lazily (the first time the instance is cast
 /// to a reference or pointer), and initialization is done by an `__init__` function.
 inline PyObject *make_new_instance(PyTypeObject *type) {
 #if defined(PYPY_VERSION)
     // PyPy gets tp_basicsize wrong (issue 2482) under multiple inheritance when the first inherited
-    // object is a a plain Python type (i.e. not derived from an extension type).  Fix it.
+    // object is a plain Python type (i.e. not derived from an extension type).  Fix it.
     ssize_t instance_size = static_cast<ssize_t>(sizeof(instance));
     if (type->tp_basicsize < instance_size) {
         type->tp_basicsize = instance_size;
     }
 #endif
     PyObject *self = type->tp_alloc(type, 0);
     auto inst = reinterpret_cast<instance *>(self);
@@ -560,15 +559,15 @@
     view->ndim = 1;
     view->internal = info;
     view->buf = info->ptr;
     view->itemsize = info->itemsize;
     view->len = view->itemsize;
     for (auto s : info->shape)
         view->len *= s;
-    view->readonly = info->readonly;
+    view->readonly = static_cast<int>(info->readonly);
     if ((flags & PyBUF_FORMAT) == PyBUF_FORMAT)
         view->format = const_cast<char *>(info->format.c_str());
     if ((flags & PyBUF_STRIDES) == PyBUF_STRIDES) {
         view->ndim = (int) info->ndim;
         view->strides = &info->strides[0];
         view->shape = &info->shape[0];
     }
@@ -680,19 +679,21 @@
 
     if (rec.dynamic_attr)
         enable_dynamic_attributes(heap_type);
 
     if (rec.buffer_protocol)
         enable_buffer_protocol(heap_type);
 
+    if (rec.custom_type_setup_callback)
+        rec.custom_type_setup_callback(heap_type);
+
     if (PyType_Ready(type) < 0)
         pybind11_fail(std::string(rec.name) + ": PyType_Ready failed (" + error_string() + ")!");
 
-    assert(rec.dynamic_attr ? PyType_HasFeature(type, Py_TPFLAGS_HAVE_GC)
-                            : !PyType_HasFeature(type, Py_TPFLAGS_HAVE_GC));
+    assert(!rec.dynamic_attr || PyType_HasFeature(type, Py_TPFLAGS_HAVE_GC));
 
     /* Register type with the parent scope */
     if (rec.scope)
         setattr(rec.scope, rec.name, (PyObject *) type);
     else
         Py_INCREF(type); // Keep it alive forever (reference leak)
```

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/detail/common.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/detail/common.h`

 * *Files 11% similar despite different names*

```diff
@@ -6,16 +6,20 @@
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #define PYBIND11_VERSION_MAJOR 2
-#define PYBIND11_VERSION_MINOR 6
-#define PYBIND11_VERSION_PATCH 2
+#define PYBIND11_VERSION_MINOR 9
+#define PYBIND11_VERSION_PATCH 0
+
+// Similar to Python's convention: https://docs.python.org/3/c-api/apiabiversion.html
+// Additional convention: 0xD = dev
+#define PYBIND11_VERSION_HEX 0x02090000
 
 #define PYBIND11_NAMESPACE_BEGIN(name) namespace name {
 #define PYBIND11_NAMESPACE_END(name) }
 
 // Robust support for some features and loading modules compiled against different pybind versions
 // requires forcing hidden visibility on pybind code, so we enforce this by setting the attribute on
 // the main `pybind11` namespace.
@@ -48,14 +52,17 @@
 // Compiler version assertions
 #if defined(__INTEL_COMPILER)
 #  if __INTEL_COMPILER < 1800
 #    error pybind11 requires Intel C++ compiler v18 or newer
 #  elif __INTEL_COMPILER < 1900 && defined(PYBIND11_CPP14)
 #    error pybind11 supports only C++11 with Intel C++ compiler v18. Use v19 or newer for C++14.
 #  endif
+/* The following pragma cannot be pop'ed:
+   https://community.intel.com/t5/Intel-C-Compiler/Inline-and-no-inline-warning/td-p/1216764 */
+#  pragma warning disable 2196 // warning #2196: routine is both "inline" and "noinline"
 #elif defined(__clang__) && !defined(__apple_build_version__)
 #  if __clang_major__ < 3 || (__clang_major__ == 3 && __clang_minor__ < 3)
 #    error pybind11 requires clang 3.3 or newer
 #  endif
 #elif defined(__clang__)
 // Apple changes clang version macros to its Xcode version; the first Xcode release based on
 // (upstream) clang 3.3 was Xcode 5:
@@ -78,21 +85,51 @@
 #  if defined(WIN32) || defined(_WIN32)
 #    define PYBIND11_EXPORT __declspec(dllexport)
 #  else
 #    define PYBIND11_EXPORT __attribute__ ((visibility("default")))
 #  endif
 #endif
 
-#if defined(_MSC_VER)
-#  define PYBIND11_NOINLINE __declspec(noinline)
+#if !defined(PYBIND11_EXPORT_EXCEPTION)
+#  ifdef __MINGW32__
+// workaround for:
+// error: 'dllexport' implies default visibility, but xxx has already been declared with a different visibility
+#    define PYBIND11_EXPORT_EXCEPTION
+#  else
+#    define PYBIND11_EXPORT_EXCEPTION PYBIND11_EXPORT
+#  endif
+#endif
+
+// For CUDA, GCC7, GCC8:
+// PYBIND11_NOINLINE_FORCED is incompatible with `-Wattributes -Werror`.
+// When defining PYBIND11_NOINLINE_FORCED, it is best to also use `-Wno-attributes`.
+// However, the measured shared-library size saving when using noinline are only
+// 1.7% for CUDA, -0.2% for GCC7, and 0.0% for GCC8 (using -DCMAKE_BUILD_TYPE=MinSizeRel,
+// the default under pybind11/tests).
+#if !defined(PYBIND11_NOINLINE_FORCED) && \
+    (defined(__CUDACC__) || (defined(__GNUC__) && (__GNUC__ == 7 || __GNUC__ == 8)))
+#  define PYBIND11_NOINLINE_DISABLED
+#endif
+
+// The PYBIND11_NOINLINE macro is for function DEFINITIONS.
+// In contrast, FORWARD DECLARATIONS should never use this macro:
+// https://stackoverflow.com/questions/9317473/forward-declaration-of-inline-functions
+#if defined(PYBIND11_NOINLINE_DISABLED) // Option for maximum portability and experimentation.
+#  define PYBIND11_NOINLINE inline
+#elif defined(_MSC_VER)
+#  define PYBIND11_NOINLINE __declspec(noinline) inline
 #else
-#  define PYBIND11_NOINLINE __attribute__ ((noinline))
+#  define PYBIND11_NOINLINE __attribute__ ((noinline)) inline
 #endif
 
-#if defined(PYBIND11_CPP14)
+#if defined(__MINGW32__)
+// For unknown reasons all PYBIND11_DEPRECATED member trigger a warning when declared
+// whether it is used or not
+#  define PYBIND11_DEPRECATED(reason)
+#elif defined(PYBIND11_CPP14)
 #  define PYBIND11_DEPRECATED(reason) [[deprecated(reason)]]
 #else
 #  define PYBIND11_DEPRECATED(reason) __attribute__((deprecated(reason)))
 #endif
 
 #if defined(PYBIND11_CPP17)
 #  define PYBIND11_MAYBE_UNUSED [[maybe_unused]]
@@ -110,21 +147,69 @@
 
 /// Include Python header, disable linking to pythonX_d.lib on Windows in debug mode
 #if defined(_MSC_VER)
 #  if (PY_MAJOR_VERSION == 3 && PY_MINOR_VERSION < 4)
 #    define HAVE_ROUND 1
 #  endif
 #  pragma warning(push)
-#  pragma warning(disable: 4510 4610 4512 4005)
+// C4505: 'PySlice_GetIndicesEx': unreferenced local function has been removed (PyPy only)
+#  pragma warning(disable: 4505)
 #  if defined(_DEBUG) && !defined(Py_DEBUG)
+// Workaround for a VS 2022 issue.
+// NOTE: This workaround knowingly violates the Python.h include order requirement:
+// https://docs.python.org/3/c-api/intro.html#include-files
+// See https://github.com/pybind/pybind11/pull/3497 for full context.
+#    include <yvals.h>
+#    if _MSVC_STL_VERSION >= 143
+#      include <crtdefs.h>
+#    endif
 #    define PYBIND11_DEBUG_MARKER
 #    undef _DEBUG
 #  endif
 #endif
 
+// https://en.cppreference.com/w/c/chrono/localtime
+#if defined(__STDC_LIB_EXT1__) && !defined(__STDC_WANT_LIB_EXT1__)
+#  define __STDC_WANT_LIB_EXT1__
+#endif
+
+#ifdef __has_include
+// std::optional (but including it in c++14 mode isn't allowed)
+#  if defined(PYBIND11_CPP17) && __has_include(<optional>)
+#    define PYBIND11_HAS_OPTIONAL 1
+#  endif
+// std::experimental::optional (but not allowed in c++11 mode)
+#  if defined(PYBIND11_CPP14) && (__has_include(<experimental/optional>) && \
+                                 !__has_include(<optional>))
+#    define PYBIND11_HAS_EXP_OPTIONAL 1
+#  endif
+// std::variant
+#  if defined(PYBIND11_CPP17) && __has_include(<variant>)
+#    define PYBIND11_HAS_VARIANT 1
+#  endif
+#elif defined(_MSC_VER) && defined(PYBIND11_CPP17)
+#  define PYBIND11_HAS_OPTIONAL 1
+#  define PYBIND11_HAS_VARIANT 1
+#endif
+
+#if defined(PYBIND11_CPP17)
+#  if defined(__has_include)
+#    if __has_include(<string_view>)
+#      define PYBIND11_HAS_STRING_VIEW
+#    endif
+#  elif defined(_MSC_VER)
+#    define PYBIND11_HAS_STRING_VIEW
+#  endif
+#endif
+
+#if defined(__cpp_lib_char8_t) && __cpp_lib_char8_t >= 201811L
+#  define PYBIND11_HAS_U8STRING
+#endif
+
+
 #include <Python.h>
 #include <frameobject.h>
 #include <pythread.h>
 
 /* Python #defines overrides on all sorts of core functions, which
    tends to weak havok in C++ codebases that expect these to work
    like regular functions (potentially with several overloads) */
@@ -158,29 +243,47 @@
 #include <stdexcept>
 #include <exception>
 #include <unordered_set>
 #include <unordered_map>
 #include <memory>
 #include <typeindex>
 #include <type_traits>
+#if defined(__has_include)
+#  if __has_include(<version>)
+#    include <version>
+#  endif
+#endif
+
+// #define PYBIND11_STR_LEGACY_PERMISSIVE
+// If DEFINED, pybind11::str can hold PyUnicodeObject or PyBytesObject
+//             (probably surprising and never documented, but this was the
+//             legacy behavior until and including v2.6.x). As a side-effect,
+//             pybind11::isinstance<str>() is true for both pybind11::str and
+//             pybind11::bytes.
+// If UNDEFINED, pybind11::str can only hold PyUnicodeObject, and
+//               pybind11::isinstance<str>() is true only for pybind11::str.
+//               However, for Python 2 only (!), the pybind11::str caster
+//               implicitly decodes bytes to PyUnicodeObject. This is to ease
+//               the transition from the legacy behavior to the non-permissive
+//               behavior.
 
 #if PY_MAJOR_VERSION >= 3 /// Compatibility macros for various Python versions
 #define PYBIND11_INSTANCE_METHOD_NEW(ptr, class_) PyInstanceMethod_New(ptr)
 #define PYBIND11_INSTANCE_METHOD_CHECK PyInstanceMethod_Check
 #define PYBIND11_INSTANCE_METHOD_GET_FUNCTION PyInstanceMethod_GET_FUNCTION
 #define PYBIND11_BYTES_CHECK PyBytes_Check
 #define PYBIND11_BYTES_FROM_STRING PyBytes_FromString
 #define PYBIND11_BYTES_FROM_STRING_AND_SIZE PyBytes_FromStringAndSize
 #define PYBIND11_BYTES_AS_STRING_AND_SIZE PyBytes_AsStringAndSize
 #define PYBIND11_BYTES_AS_STRING PyBytes_AsString
 #define PYBIND11_BYTES_SIZE PyBytes_Size
 #define PYBIND11_LONG_CHECK(o) PyLong_Check(o)
 #define PYBIND11_LONG_AS_LONGLONG(o) PyLong_AsLongLong(o)
-#define PYBIND11_LONG_FROM_SIGNED(o) PyLong_FromSsize_t((ssize_t) o)
-#define PYBIND11_LONG_FROM_UNSIGNED(o) PyLong_FromSize_t((size_t) o)
+#define PYBIND11_LONG_FROM_SIGNED(o) PyLong_FromSsize_t((ssize_t) (o))
+#define PYBIND11_LONG_FROM_UNSIGNED(o) PyLong_FromSize_t((size_t) (o))
 #define PYBIND11_BYTES_NAME "bytes"
 #define PYBIND11_STRING_NAME "str"
 #define PYBIND11_SLICE_OBJECT PyObject
 #define PYBIND11_FROM_STRING PyUnicode_FromString
 #define PYBIND11_STR_TYPE ::pybind11::str
 #define PYBIND11_BOOL_ATTR "__bool__"
 #define PYBIND11_NB_BOOL(ptr) ((ptr)->nb_bool)
@@ -250,23 +353,38 @@
                 "Python version mismatch: module was compiled for Python %s, " \
                 "but the interpreter version is incompatible: %s.",            \
                 compiled_ver, runtime_ver);                                    \
             return nullptr;                                                    \
         }                                                                      \
     }
 
+#if PY_VERSION_HEX >= 0x03030000
+
+#define PYBIND11_CATCH_INIT_EXCEPTIONS \
+        catch (pybind11::error_already_set &e) {                                 \
+            pybind11::raise_from(e, PyExc_ImportError, "initialization failed"); \
+            return nullptr;                                                      \
+        } catch (const std::exception &e) {                                      \
+            PyErr_SetString(PyExc_ImportError, e.what());                        \
+            return nullptr;                                                      \
+        }                                                                        \
+
+#else
+
 #define PYBIND11_CATCH_INIT_EXCEPTIONS \
         catch (pybind11::error_already_set &e) {                               \
             PyErr_SetString(PyExc_ImportError, e.what());                      \
             return nullptr;                                                    \
         } catch (const std::exception &e) {                                    \
             PyErr_SetString(PyExc_ImportError, e.what());                      \
             return nullptr;                                                    \
         }                                                                      \
 
+#endif
+
 /** \rst
     ***Deprecated in favor of PYBIND11_MODULE***
 
     This macro creates the entry point that will be invoked when the Python interpreter
     imports a plugin library. Please create a `module_` in the function body and return
     the pointer to its underlying Python object at the end.
 
@@ -307,38 +425,43 @@
 
             // Add bindings here
             m.def("foo", []() {
                 return "Hello, World!";
             });
         }
 \endrst */
-#define PYBIND11_MODULE(name, variable)                                        \
-    static ::pybind11::module_::module_def                                     \
-        PYBIND11_CONCAT(pybind11_module_def_, name) PYBIND11_MAYBE_UNUSED;     \
-    PYBIND11_MAYBE_UNUSED                                                      \
-    static void PYBIND11_CONCAT(pybind11_init_, name)(::pybind11::module_ &);  \
-    PYBIND11_PLUGIN_IMPL(name) {                                               \
-        PYBIND11_CHECK_PYTHON_VERSION                                          \
-        PYBIND11_ENSURE_INTERNALS_READY                                        \
-        auto m = ::pybind11::module_::create_extension_module(                 \
-            PYBIND11_TOSTRING(name), nullptr,                                  \
-            &PYBIND11_CONCAT(pybind11_module_def_, name));                     \
-        try {                                                                  \
-            PYBIND11_CONCAT(pybind11_init_, name)(m);                          \
-            return m.ptr();                                                    \
-        } PYBIND11_CATCH_INIT_EXCEPTIONS                                       \
-    }                                                                          \
-    void PYBIND11_CONCAT(pybind11_init_, name)(::pybind11::module_ &variable)
-
+#define PYBIND11_MODULE(name, variable)                                                           \
+    static ::pybind11::module_::module_def PYBIND11_CONCAT(pybind11_module_def_, name)            \
+        PYBIND11_MAYBE_UNUSED;                                                                    \
+    PYBIND11_MAYBE_UNUSED                                                                         \
+    static void PYBIND11_CONCAT(pybind11_init_, name)(::pybind11::module_ &);                     \
+    PYBIND11_PLUGIN_IMPL(name) {                                                                  \
+        PYBIND11_CHECK_PYTHON_VERSION                                                             \
+        PYBIND11_ENSURE_INTERNALS_READY                                                           \
+        auto m = ::pybind11::module_::create_extension_module(                                    \
+            PYBIND11_TOSTRING(name), nullptr, &PYBIND11_CONCAT(pybind11_module_def_, name));      \
+        try {                                                                                     \
+            PYBIND11_CONCAT(pybind11_init_, name)(m);                                             \
+            return m.ptr();                                                                       \
+        }                                                                                         \
+        PYBIND11_CATCH_INIT_EXCEPTIONS                                                            \
+    }                                                                                             \
+    void PYBIND11_CONCAT(pybind11_init_, name)(::pybind11::module_ & (variable))
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
 using ssize_t = Py_ssize_t;
 using size_t  = std::size_t;
 
+template <typename IntType>
+inline ssize_t ssize_t_cast(const IntType &val) {
+    static_assert(sizeof(IntType) <= sizeof(ssize_t), "Implicit narrowing is not permitted.");
+    return static_cast<ssize_t>(val);
+}
+
 /// Approach used to cast a previously unknown C++ instance into a Python object
 enum class return_value_policy : uint8_t {
     /** This is the default return value policy, which falls back to the policy
         return_value_policy::take_ownership when the return value is a pointer.
         Otherwise, it uses return_value::move or return_value::copy for rvalue
         and lvalue references, respectively. See below for a description of what
         all of these different policies do. */
@@ -686,56 +809,61 @@
 
 /// Returns true if the type looks like a lambda: that is, isn't a function, pointer or member
 /// pointer.  Note that this can catch all sorts of other things, too; this is intended to be used
 /// in a place where passing a lambda makes sense.
 template <typename T> using is_lambda = satisfies_none_of<remove_reference_t<T>,
         std::is_function, std::is_pointer, std::is_member_pointer>;
 
-/// Ignore that a variable is unused in compiler warnings
-inline void ignore_unused(const int *) { }
-
 // [workaround(intel)] Internal error on fold expression
 /// Apply a function over each element of a parameter pack
 #if defined(__cpp_fold_expressions) && !defined(__INTEL_COMPILER)
 // Intel compiler produces an internal error on this fold expression (tested with ICC 19.0.2)
 #define PYBIND11_EXPAND_SIDE_EFFECTS(PATTERN) (((PATTERN), void()), ...)
 #else
 using expand_side_effects = bool[];
 #define PYBIND11_EXPAND_SIDE_EFFECTS(PATTERN) (void)pybind11::detail::expand_side_effects{ ((PATTERN), void(), false)..., false }
 #endif
 
 PYBIND11_NAMESPACE_END(detail)
 
+#if defined(_MSC_VER)
+#  pragma warning(push)
+#  pragma warning(disable: 4275) // warning C4275: An exported class was derived from a class that wasn't exported. Can be ignored when derived from a STL class.
+#endif
 /// C++ bindings of builtin Python exceptions
-class builtin_exception : public std::runtime_error {
+class PYBIND11_EXPORT_EXCEPTION builtin_exception : public std::runtime_error {
 public:
     using std::runtime_error::runtime_error;
     /// Set the error using the Python C API
     virtual void set_error() const = 0;
 };
+#if defined(_MSC_VER)
+#  pragma warning(pop)
+#endif
 
 #define PYBIND11_RUNTIME_EXCEPTION(name, type) \
-    class name : public builtin_exception { public: \
+    class PYBIND11_EXPORT_EXCEPTION name : public builtin_exception { public: \
         using builtin_exception::builtin_exception; \
         name() : name("") { } \
         void set_error() const override { PyErr_SetString(type, what()); } \
     };
 
 PYBIND11_RUNTIME_EXCEPTION(stop_iteration, PyExc_StopIteration)
 PYBIND11_RUNTIME_EXCEPTION(index_error, PyExc_IndexError)
 PYBIND11_RUNTIME_EXCEPTION(key_error, PyExc_KeyError)
 PYBIND11_RUNTIME_EXCEPTION(value_error, PyExc_ValueError)
 PYBIND11_RUNTIME_EXCEPTION(type_error, PyExc_TypeError)
 PYBIND11_RUNTIME_EXCEPTION(buffer_error, PyExc_BufferError)
 PYBIND11_RUNTIME_EXCEPTION(import_error, PyExc_ImportError)
+PYBIND11_RUNTIME_EXCEPTION(attribute_error, PyExc_AttributeError)
 PYBIND11_RUNTIME_EXCEPTION(cast_error, PyExc_RuntimeError) /// Thrown when pybind11::cast or handle::call fail due to a type casting error
 PYBIND11_RUNTIME_EXCEPTION(reference_cast_error, PyExc_RuntimeError) /// Used internally
 
-[[noreturn]] PYBIND11_NOINLINE inline void pybind11_fail(const char *reason) { throw std::runtime_error(reason); }
-[[noreturn]] PYBIND11_NOINLINE inline void pybind11_fail(const std::string &reason) { throw std::runtime_error(reason); }
+[[noreturn]] PYBIND11_NOINLINE void pybind11_fail(const char *reason) { throw std::runtime_error(reason); }
+[[noreturn]] PYBIND11_NOINLINE void pybind11_fail(const std::string &reason) { throw std::runtime_error(reason); }
 
 template <typename T, typename SFINAE = void> struct format_descriptor { };
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 // Returns the index of the given type in the type char array below, and in the list in numpy.h
 // The order here is: bool; 8 ints ((signed,unsigned)x(8,16,32,64)bits); float,double,long double;
 // complex float,double,long double.  Note that the long double types only participate when long
@@ -772,15 +900,16 @@
 
 /// Dummy destructor wrapper that can be used to expose classes with a private destructor
 struct nodelete { template <typename T> void operator()(T*) { } };
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 template <typename... Args>
 struct overload_cast_impl {
-    constexpr overload_cast_impl() {}; // NOLINT(modernize-use-equals-default):  MSVC 2015 needs this
+    // NOLINTNEXTLINE(modernize-use-equals-default):  MSVC 2015 needs this
+    constexpr overload_cast_impl() {}
 
     template <typename Return>
     constexpr auto operator()(Return (*pf)(Args...)) const noexcept
                               -> decltype(pf) { return pf; }
 
     template <typename Return, typename Class>
     constexpr auto operator()(Return (Class::*pmf)(Args...), std::false_type = {}) const noexcept
@@ -828,34 +957,89 @@
 
     // Can construct from a pair of iterators
     template <typename It, typename = enable_if_t<is_input_iterator<It>::value>>
     any_container(It first, It last) : v(first, last) { }
 
     // Implicit conversion constructor from any arbitrary container type with values convertible to T
     template <typename Container, typename = enable_if_t<std::is_convertible<decltype(*std::begin(std::declval<const Container &>())), T>::value>>
+    // NOLINTNEXTLINE(google-explicit-constructor)
     any_container(const Container &c) : any_container(std::begin(c), std::end(c)) { }
 
     // initializer_list's aren't deducible, so don't get matched by the above template; we need this
     // to explicitly allow implicit conversion from one:
     template <typename TIn, typename = enable_if_t<std::is_convertible<TIn, T>::value>>
     any_container(const std::initializer_list<TIn> &c) : any_container(c.begin(), c.end()) { }
 
     // Avoid copying if given an rvalue vector of the correct type.
+    // NOLINTNEXTLINE(google-explicit-constructor)
     any_container(std::vector<T> &&v) : v(std::move(v)) { }
 
     // Moves the vector out of an rvalue any_container
+    // NOLINTNEXTLINE(google-explicit-constructor)
     operator std::vector<T> &&() && { return std::move(v); }
 
     // Dereferencing obtains a reference to the underlying vector
     std::vector<T> &operator*() { return v; }
     const std::vector<T> &operator*() const { return v; }
 
     // -> lets you call methods on the underlying vector
     std::vector<T> *operator->() { return &v; }
     const std::vector<T> *operator->() const { return &v; }
 };
 
 // Forward-declaration; see detail/class.h
 std::string get_fully_qualified_tp_name(PyTypeObject*);
 
+template <typename T>
+inline static std::shared_ptr<T> try_get_shared_from_this(std::enable_shared_from_this<T> *holder_value_ptr) {
+// Pre C++17, this code path exploits undefined behavior, but is known to work on many platforms.
+// Use at your own risk!
+// See also https://en.cppreference.com/w/cpp/memory/enable_shared_from_this, and in particular
+// the `std::shared_ptr<Good> gp1 = not_so_good.getptr();` and `try`-`catch` parts of the example.
+#if defined(__cpp_lib_enable_shared_from_this) && (!defined(_MSC_VER) || _MSC_VER >= 1912)
+    return holder_value_ptr->weak_from_this().lock();
+#else
+    try {
+        return holder_value_ptr->shared_from_this();
+    }
+    catch (const std::bad_weak_ptr &) {
+        return nullptr;
+    }
+#endif
+}
+
+// For silencing "unused" compiler warnings in special situations.
+template <typename... Args>
+#if defined(_MSC_VER) && _MSC_VER >= 1910 && _MSC_VER < 1920 // MSVC 2017
+constexpr
+#endif
+inline void silence_unused_warnings(Args &&...) {}
+
+// MSVC warning C4100: Unreferenced formal parameter
+#if defined(_MSC_VER) && _MSC_VER <= 1916
+#    define PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(...)                                         \
+        detail::silence_unused_warnings(__VA_ARGS__)
+#else
+#    define PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(...)
+#endif
+
+// GCC -Wunused-but-set-parameter  All GCC versions (as of July 2021).
+#if defined(__GNUG__) && !defined(__clang__) && !defined(__INTEL_COMPILER)
+#    define PYBIND11_WORKAROUND_INCORRECT_GCC_UNUSED_BUT_SET_PARAMETER(...)                   \
+        detail::silence_unused_warnings(__VA_ARGS__)
+#else
+#    define PYBIND11_WORKAROUND_INCORRECT_GCC_UNUSED_BUT_SET_PARAMETER(...)
+#endif
+
+#if defined(_MSC_VER) // All versions (as of July 2021).
+
+// warning C4127: Conditional expression is constant
+constexpr inline bool silence_msvc_c4127(bool cond) { return cond; }
+
+#    define PYBIND11_SILENCE_MSVC_C4127(...) ::pybind11::detail::silence_msvc_c4127(__VA_ARGS__)
+
+#else
+#    define PYBIND11_SILENCE_MSVC_C4127(...) __VA_ARGS__
+#endif
+
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/detail/descr.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/detail/descr.h`

 * *Files 26% similar despite different names*

```diff
@@ -19,82 +19,111 @@
 #else
 #  define PYBIND11_DESCR_CONSTEXPR const
 #endif
 
 /* Concatenate type signatures at compile time */
 template <size_t N, typename... Ts>
 struct descr {
-    char text[N + 1];
+    char text[N + 1]{'\0'};
 
-    constexpr descr() : text{'\0'} { }
+    constexpr descr() = default;
+    // NOLINTNEXTLINE(google-explicit-constructor)
     constexpr descr(char const (&s)[N+1]) : descr(s, make_index_sequence<N>()) { }
 
     template <size_t... Is>
     constexpr descr(char const (&s)[N+1], index_sequence<Is...>) : text{s[Is]..., '\0'} { }
 
     template <typename... Chars>
+    // NOLINTNEXTLINE(google-explicit-constructor)
     constexpr descr(char c, Chars... cs) : text{c, static_cast<char>(cs)..., '\0'} { }
 
     static constexpr std::array<const std::type_info *, sizeof...(Ts) + 1> types() {
         return {{&typeid(Ts)..., nullptr}};
     }
 };
 
 template <size_t N1, size_t N2, typename... Ts1, typename... Ts2, size_t... Is1, size_t... Is2>
 constexpr descr<N1 + N2, Ts1..., Ts2...> plus_impl(const descr<N1, Ts1...> &a, const descr<N2, Ts2...> &b,
                                                    index_sequence<Is1...>, index_sequence<Is2...>) {
+    PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(b);
     return {a.text[Is1]..., b.text[Is2]...};
 }
 
 template <size_t N1, size_t N2, typename... Ts1, typename... Ts2>
 constexpr descr<N1 + N2, Ts1..., Ts2...> operator+(const descr<N1, Ts1...> &a, const descr<N2, Ts2...> &b) {
     return plus_impl(a, b, make_index_sequence<N1>(), make_index_sequence<N2>());
 }
 
 template <size_t N>
-constexpr descr<N - 1> _(char const(&text)[N]) { return descr<N - 1>(text); }
-constexpr descr<0> _(char const(&)[1]) { return {}; }
+constexpr descr<N - 1> const_name(char const(&text)[N]) { return descr<N - 1>(text); }
+constexpr descr<0> const_name(char const(&)[1]) { return {}; }
 
 template <size_t Rem, size_t... Digits> struct int_to_str : int_to_str<Rem/10, Rem%10, Digits...> { };
 template <size_t...Digits> struct int_to_str<0, Digits...> {
     static constexpr auto digits = descr<sizeof...(Digits)>(('0' + Digits)...);
 };
 
 // Ternary description (like std::conditional)
 template <bool B, size_t N1, size_t N2>
-constexpr enable_if_t<B, descr<N1 - 1>> _(char const(&text1)[N1], char const(&)[N2]) {
-    return _(text1);
+constexpr enable_if_t<B, descr<N1 - 1>> const_name(char const(&text1)[N1], char const(&)[N2]) {
+    return const_name(text1);
 }
 template <bool B, size_t N1, size_t N2>
-constexpr enable_if_t<!B, descr<N2 - 1>> _(char const(&)[N1], char const(&text2)[N2]) {
-    return _(text2);
+constexpr enable_if_t<!B, descr<N2 - 1>> const_name(char const(&)[N1], char const(&text2)[N2]) {
+    return const_name(text2);
 }
 
 template <bool B, typename T1, typename T2>
-constexpr enable_if_t<B, T1> _(const T1 &d, const T2 &) { return d; }
+constexpr enable_if_t<B, T1> const_name(const T1 &d, const T2 &) { return d; }
 template <bool B, typename T1, typename T2>
-constexpr enable_if_t<!B, T2> _(const T1 &, const T2 &d) { return d; }
+constexpr enable_if_t<!B, T2> const_name(const T1 &, const T2 &d) { return d; }
 
-template <size_t Size> auto constexpr _() -> decltype(int_to_str<Size / 10, Size % 10>::digits) {
+template <size_t Size>
+auto constexpr const_name() -> remove_cv_t<decltype(int_to_str<Size / 10, Size % 10>::digits)> {
     return int_to_str<Size / 10, Size % 10>::digits;
 }
 
-template <typename Type> constexpr descr<1, Type> _() { return {'%'}; }
+template <typename Type> constexpr descr<1, Type> const_name() { return {'%'}; }
+
+// The "_" might be defined as a macro - don't define it if so.
+// Repeating the const_name code to avoid introducing a #define.
+#ifndef _
+template <size_t N>
+constexpr descr<N-1> _(char const(&text)[N]) { return const_name<N>(text); }
+template <bool B, size_t N1, size_t N2>
+constexpr enable_if_t<B, descr<N1 - 1>> _(char const(&text1)[N1], char const(&text2)[N2]) {
+    return const_name<B,N1,N2>(text1, text2);
+}
+template <bool B, size_t N1, size_t N2>
+constexpr enable_if_t<!B, descr<N2 - 1>> _(char const(&text1)[N1], char const(&text2)[N2]) {
+    return const_name<B,N1,N2>(text1, text2);
+}
+template <bool B, typename T1, typename T2>
+constexpr enable_if_t<B, T1> _(const T1 &d1, const T2 &d2) { return const_name<B,T1,T2>(d1, d2); }
+template <bool B, typename T1, typename T2>
+constexpr enable_if_t<!B, T2> _(const T1 &d1, const T2 &d2) { return const_name<B,T1,T2>(d1, d2); }
+
+template <size_t Size>
+auto constexpr _() -> remove_cv_t<decltype(int_to_str<Size / 10, Size % 10>::digits)> {
+    return const_name<Size>();
+}
+template <typename Type> constexpr descr<1, Type> _() { return const_name<Type>(); }
+#endif
 
 constexpr descr<0> concat() { return {}; }
 
 template <size_t N, typename... Ts>
 constexpr descr<N, Ts...> concat(const descr<N, Ts...> &descr) { return descr; }
 
 template <size_t N, typename... Ts, typename... Args>
 constexpr auto concat(const descr<N, Ts...> &d, const Args &...args)
     -> decltype(std::declval<descr<N + 2, Ts...>>() + concat(args...)) {
-    return d + _(", ") + concat(args...);
+    return d + const_name(", ") + concat(args...);
 }
 
 template <size_t N, typename... Ts>
 constexpr descr<N + 2, Ts...> type_descr(const descr<N, Ts...> &descr) {
-    return _("{") + descr + _("}");
+    return const_name("{") + descr + const_name("}");
 }
 
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/detail/init.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/detail/init.h`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 public:
     bool load(handle h, bool) {
         value = reinterpret_cast<value_and_holder *>(h.ptr());
         return true;
     }
 
     template <typename> using cast_op_type = value_and_holder &;
-    operator value_and_holder &() { return *value; }
-    static constexpr auto name = _<value_and_holder>();
+    explicit operator value_and_holder &() { return *value; }
+    static constexpr auto name = const_name<value_and_holder>();
 
 private:
     value_and_holder *value = nullptr;
 };
 
 PYBIND11_NAMESPACE_BEGIN(initimpl)
 
@@ -90,16 +90,17 @@
 
 // Pointer return v1: the factory function returns a class pointer for a registered class.
 // If we don't need an alias (because this class doesn't have one, or because the final type is
 // inherited on the Python side) we can simply take over ownership.  Otherwise we need to try to
 // construct an Alias from the returned base instance.
 template <typename Class>
 void construct(value_and_holder &v_h, Cpp<Class> *ptr, bool need_alias) {
+    PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(need_alias);
     no_nullptr(ptr);
-    if (Class::has_alias && need_alias && !is_alias<Class>(ptr)) {
+    if (PYBIND11_SILENCE_MSVC_C4127(Class::has_alias) && need_alias && !is_alias<Class>(ptr)) {
         // We're going to try to construct an alias by moving the cpp type.  Whether or not
         // that succeeds, we still need to destroy the original cpp pointer (either the
         // moved away leftover, if the alias construction works, or the value itself if we
         // throw an error), but we can't just call `delete ptr`: it might have a special
         // deleter, or might be shared_from_this.  So we construct a holder around it as if
         // it was a normal instance, then steal the holder away into a local variable; thus
         // the holder and destruction happens when we leave the C++ scope, and the holder
@@ -127,34 +128,36 @@
 }
 
 // Holder return: copy its pointer, and move or copy the returned holder into the new instance's
 // holder.  This also handles types like std::shared_ptr<T> and std::unique_ptr<T> where T is a
 // derived type (through those holder's implicit conversion from derived class holder constructors).
 template <typename Class>
 void construct(value_and_holder &v_h, Holder<Class> holder, bool need_alias) {
+    PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(need_alias);
     auto *ptr = holder_helper<Holder<Class>>::get(holder);
     no_nullptr(ptr);
     // If we need an alias, check that the held pointer is actually an alias instance
-    if (Class::has_alias && need_alias && !is_alias<Class>(ptr))
+    if (PYBIND11_SILENCE_MSVC_C4127(Class::has_alias) && need_alias && !is_alias<Class>(ptr))
         throw type_error("pybind11::init(): construction failed: returned holder-wrapped instance "
                          "is not an alias instance");
 
     v_h.value_ptr() = ptr;
     v_h.type->init_instance(v_h.inst, &holder);
 }
 
 // return-by-value version 1: returning a cpp class by value.  If the class has an alias and an
 // alias is required the alias must have an `Alias(Cpp &&)` constructor so that we can construct
 // the alias from the base when needed (i.e. because of Python-side inheritance).  When we don't
 // need it, we simply move-construct the cpp value into a new instance.
 template <typename Class>
 void construct(value_and_holder &v_h, Cpp<Class> &&result, bool need_alias) {
+    PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(need_alias);
     static_assert(std::is_move_constructible<Cpp<Class>>::value,
         "pybind11::init() return-by-value factory function requires a movable class");
-    if (Class::has_alias && need_alias)
+    if (PYBIND11_SILENCE_MSVC_C4127(Class::has_alias) && need_alias)
         construct_alias_from_cpp<Class>(is_alias_constructible<Class>{}, v_h, std::move(result));
     else
         v_h.value_ptr() = new Cpp<Class>(std::move(result));
 }
 
 // return-by-value version 2: returning a value of the alias type itself.  We move-construct an
 // Alias instance (even if no the python-side inheritance is involved).  The is intended for
@@ -215,15 +218,16 @@
 struct factory;
 
 // Specialization for py::init(Func)
 template <typename Func, typename Return, typename... Args>
 struct factory<Func, void_type (*)(), Return(Args...)> {
     remove_reference_t<Func> class_factory;
 
-    factory(Func &&f) : class_factory(std::forward<Func>(f)) { }
+    // NOLINTNEXTLINE(google-explicit-constructor)
+    factory(Func &&f) : class_factory(std::forward<Func>(f)) {}
 
     // The given class either has no alias or has no separate alias factory;
     // this always constructs the class itself.  If the class is registered with an alias
     // type and an alias instance is needed (i.e. because the final type is a Python class
     // inheriting from the C++ type) the returned value needs to either already be an alias
     // instance, or the alias needs to be constructible from a `Class &&` argument.
     template <typename Class, typename... Extra>
@@ -289,15 +293,21 @@
 }
 
 /// Set both the C++ and Python states
 template <typename Class, typename T, typename O,
           enable_if_t<std::is_convertible<O, handle>::value, int> = 0>
 void setstate(value_and_holder &v_h, std::pair<T, O> &&result, bool need_alias) {
     construct<Class>(v_h, std::move(result.first), need_alias);
-    setattr((PyObject *) v_h.inst, "__dict__", result.second);
+    auto d = handle(result.second);
+    if (PyDict_Check(d.ptr()) && PyDict_Size(d.ptr()) == 0) {
+        // Skipping setattr below, to not force use of py::dynamic_attr() for Class unnecessarily.
+        // See PR #2972 for details.
+        return;
+    }
+    setattr((PyObject *) v_h.inst, "__dict__", d);
 }
 
 /// Implementation for py::pickle(GetState, SetState)
 template <typename Get, typename Set,
           typename = function_signature_t<Get>, typename = function_signature_t<Set>>
 struct pickle_factory;
```

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/detail/internals.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/detail/internals.h`

 * *Files 15% similar despite different names*

```diff
@@ -7,48 +7,99 @@
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "../pytypes.h"
 
+/// Tracks the `internals` and `type_info` ABI version independent of the main library version.
+///
+/// Some portions of the code use an ABI that is conditional depending on this
+/// version number.  That allows ABI-breaking changes to be "pre-implemented".
+/// Once the default version number is incremented, the conditional logic that
+/// no longer applies can be removed.  Additionally, users that need not
+/// maintain ABI compatibility can increase the version number in order to take
+/// advantage of any functionality/efficiency improvements that depend on the
+/// newer ABI.
+///
+/// WARNING: If you choose to manually increase the ABI version, note that
+/// pybind11 may not be tested as thoroughly with a non-default ABI version, and
+/// further ABI-incompatible changes may be made before the ABI is officially
+/// changed to the new version.
+#ifndef PYBIND11_INTERNALS_VERSION
+#    define PYBIND11_INTERNALS_VERSION 4
+#endif
+
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
+
+using ExceptionTranslator = void (*)(std::exception_ptr);
+
 PYBIND11_NAMESPACE_BEGIN(detail)
+
 // Forward declarations
 inline PyTypeObject *make_static_property_type();
 inline PyTypeObject *make_default_metaclass();
 inline PyObject *make_object_base_type(PyTypeObject *metaclass);
 
 // The old Python Thread Local Storage (TLS) API is deprecated in Python 3.7 in favor of the new
 // Thread Specific Storage (TSS) API.
 #if PY_VERSION_HEX >= 0x03070000
-#    define PYBIND11_TLS_KEY_INIT(var) Py_tss_t *var = nullptr
-#    define PYBIND11_TLS_GET_VALUE(key) PyThread_tss_get((key))
-#    define PYBIND11_TLS_REPLACE_VALUE(key, value) PyThread_tss_set((key), (value))
-#    define PYBIND11_TLS_DELETE_VALUE(key) PyThread_tss_set((key), nullptr)
-#    define PYBIND11_TLS_FREE(key) PyThread_tss_free(key)
+// Avoid unnecessary allocation of `Py_tss_t`, since we cannot use
+// `Py_LIMITED_API` anyway.
+#    if PYBIND11_INTERNALS_VERSION > 4
+#        define PYBIND11_TLS_KEY_REF Py_tss_t &
+#        ifdef __GNUC__
+// Clang on macOS warns due to `Py_tss_NEEDS_INIT` not specifying an initializer
+// for every field.
+#            define PYBIND11_TLS_KEY_INIT(var)                                                    \
+                _Pragma("GCC diagnostic push")                                         /**/       \
+                    _Pragma("GCC diagnostic ignored \"-Wmissing-field-initializers\"") /**/       \
+                    Py_tss_t var                                                                  \
+                    = Py_tss_NEEDS_INIT;                                                          \
+                _Pragma("GCC diagnostic pop")
+#        else
+#            define PYBIND11_TLS_KEY_INIT(var) Py_tss_t var = Py_tss_NEEDS_INIT;
+#        endif
+#        define PYBIND11_TLS_KEY_CREATE(var) (PyThread_tss_create(&(var)) == 0)
+#        define PYBIND11_TLS_GET_VALUE(key) PyThread_tss_get(&(key))
+#        define PYBIND11_TLS_REPLACE_VALUE(key, value) PyThread_tss_set(&(key), (value))
+#        define PYBIND11_TLS_DELETE_VALUE(key) PyThread_tss_set(&(key), nullptr)
+#        define PYBIND11_TLS_FREE(key) PyThread_tss_delete(&(key))
+#    else
+#        define PYBIND11_TLS_KEY_REF Py_tss_t *
+#        define PYBIND11_TLS_KEY_INIT(var) Py_tss_t *var = nullptr;
+#        define PYBIND11_TLS_KEY_CREATE(var)                                                      \
+            (((var) = PyThread_tss_alloc()) != nullptr && (PyThread_tss_create((var)) == 0))
+#        define PYBIND11_TLS_GET_VALUE(key) PyThread_tss_get((key))
+#        define PYBIND11_TLS_REPLACE_VALUE(key, value) PyThread_tss_set((key), (value))
+#        define PYBIND11_TLS_DELETE_VALUE(key) PyThread_tss_set((key), nullptr)
+#        define PYBIND11_TLS_FREE(key) PyThread_tss_free(key)
+#    endif
 #else
-    // Usually an int but a long on Cygwin64 with Python 3.x
-#    define PYBIND11_TLS_KEY_INIT(var) decltype(PyThread_create_key()) var = 0
+// Usually an int but a long on Cygwin64 with Python 3.x
+#    define PYBIND11_TLS_KEY_REF decltype(PyThread_create_key())
+#    define PYBIND11_TLS_KEY_INIT(var) PYBIND11_TLS_KEY_REF var = 0;
+#    define PYBIND11_TLS_KEY_CREATE(var) (((var) = PyThread_create_key()) != -1)
 #    define PYBIND11_TLS_GET_VALUE(key) PyThread_get_key_value((key))
-#    if PY_MAJOR_VERSION < 3
-#        define PYBIND11_TLS_DELETE_VALUE(key)                               \
-             PyThread_delete_key_value(key)
-#        define PYBIND11_TLS_REPLACE_VALUE(key, value)                       \
-             do {                                                            \
-                 PyThread_delete_key_value((key));                           \
-                 PyThread_set_key_value((key), (value));                     \
-             } while (false)
+#    if PY_MAJOR_VERSION < 3 || defined(PYPY_VERSION)
+// On CPython < 3.4 and on PyPy, `PyThread_set_key_value` strangely does not set
+// the value if it has already been set.  Instead, it must first be deleted and
+// then set again.
+inline void tls_replace_value(PYBIND11_TLS_KEY_REF key, void *value) {
+    PyThread_delete_key_value(key);
+    PyThread_set_key_value(key, value);
+}
+#        define PYBIND11_TLS_DELETE_VALUE(key) PyThread_delete_key_value(key)
+#        define PYBIND11_TLS_REPLACE_VALUE(key, value)                                            \
+            ::pybind11::detail::tls_replace_value((key), (value))
 #    else
-#        define PYBIND11_TLS_DELETE_VALUE(key)                               \
-             PyThread_set_key_value((key), nullptr)
-#        define PYBIND11_TLS_REPLACE_VALUE(key, value)                       \
-             PyThread_set_key_value((key), (value))
+#        define PYBIND11_TLS_DELETE_VALUE(key) PyThread_set_key_value((key), nullptr)
+#        define PYBIND11_TLS_REPLACE_VALUE(key, value) PyThread_set_key_value((key), (value))
 #    endif
-#    define PYBIND11_TLS_FREE(key) (void)key
+#    define PYBIND11_TLS_FREE(key) (void) key
 #endif
 
 // Python loads modules by default with dlopen with the RTLD_LOCAL flag; under libc++ and possibly
 // other STLs, this means `typeid(A)` from one module won't equal `typeid(A)` from another module
 // even when `A` is the same, non-hidden-visibility type (e.g. from a common include).  Under
 // libstdc++, this doesn't happen: equality and the type_index hash are based on the type name,
 // which works.  If not under a known-good stl, provide our own name-based hash and equality
@@ -96,32 +147,41 @@
 struct internals {
     type_map<type_info *> registered_types_cpp; // std::type_index -> pybind11's type information
     std::unordered_map<PyTypeObject *, std::vector<type_info *>> registered_types_py; // PyTypeObject* -> base type_info(s)
     std::unordered_multimap<const void *, instance*> registered_instances; // void * -> instance*
     std::unordered_set<std::pair<const PyObject *, const char *>, override_hash> inactive_override_cache;
     type_map<std::vector<bool (*)(PyObject *, void *&)>> direct_conversions;
     std::unordered_map<const PyObject *, std::vector<PyObject *>> patients;
-    std::forward_list<void (*) (std::exception_ptr)> registered_exception_translators;
+    std::forward_list<ExceptionTranslator> registered_exception_translators;
     std::unordered_map<std::string, void *> shared_data; // Custom data to be shared across extensions
-    std::vector<PyObject *> loader_patient_stack; // Used by `loader_life_support`
+#if PYBIND11_INTERNALS_VERSION == 4
+    std::vector<PyObject *> unused_loader_patient_stack_remove_at_v5;
+#endif
     std::forward_list<std::string> static_strings; // Stores the std::strings backing detail::c_str()
     PyTypeObject *static_property_type;
     PyTypeObject *default_metaclass;
     PyObject *instance_base;
 #if defined(WITH_THREAD)
-    PYBIND11_TLS_KEY_INIT(tstate);
+    PYBIND11_TLS_KEY_INIT(tstate)
+#    if PYBIND11_INTERNALS_VERSION > 4
+    PYBIND11_TLS_KEY_INIT(loader_life_support_tls_key)
+#    endif // PYBIND11_INTERNALS_VERSION > 4
     PyInterpreterState *istate = nullptr;
     ~internals() {
+#    if PYBIND11_INTERNALS_VERSION > 4
+        PYBIND11_TLS_FREE(loader_life_support_tls_key);
+#    endif // PYBIND11_INTERNALS_VERSION > 4
+
         // This destructor is called *after* Py_Finalize() in finalize_interpreter().
-        // That *SHOULD BE* fine. The following details what happens when PyThread_tss_free is called.
-        // PYBIND11_TLS_FREE is PyThread_tss_free on python 3.7+. On older python, it does nothing.
-        // PyThread_tss_free calls PyThread_tss_delete and PyMem_RawFree.
-        // PyThread_tss_delete just calls TlsFree (on Windows) or pthread_key_delete (on *NIX). Neither
-        // of those have anything to do with CPython internals.
-        // PyMem_RawFree *requires* that the `tstate` be allocated with the CPython allocator.
+        // That *SHOULD BE* fine. The following details what happens when PyThread_tss_free is
+        // called. PYBIND11_TLS_FREE is PyThread_tss_free on python 3.7+. On older python, it does
+        // nothing. PyThread_tss_free calls PyThread_tss_delete and PyMem_RawFree.
+        // PyThread_tss_delete just calls TlsFree (on Windows) or pthread_key_delete (on *NIX).
+        // Neither of those have anything to do with CPython internals. PyMem_RawFree *requires*
+        // that the `tstate` be allocated with the CPython allocator.
         PYBIND11_TLS_FREE(tstate);
     }
 #endif
 };
 
 /// Additional type information which does not fit into the PyTypeObject.
 /// Changes to this struct also require bumping `PYBIND11_INTERNALS_VERSION`.
@@ -145,17 +205,14 @@
     bool simple_ancestors : 1;
     /* for base vs derived holder_type checks */
     bool default_holder : 1;
     /* true if this is a type registered with py::module_local */
     bool module_local : 1;
 };
 
-/// Tracks the `internals` and `type_info` ABI version independent of the main library version
-#define PYBIND11_INTERNALS_VERSION 4
-
 /// On MSVC, debug and release builds are not ABI-compatible!
 #if defined(_MSC_VER) && defined(_DEBUG)
 #  define PYBIND11_BUILD_TYPE "_debug"
 #else
 #  define PYBIND11_BUILD_TYPE ""
 #endif
 
@@ -249,15 +306,15 @@
     } catch (error_already_set &e)       { e.restore();   return;
     } catch (const builtin_exception &e) { e.set_error(); return;
     }
 }
 #endif
 
 /// Return a reference to the current `internals` data
-PYBIND11_NOINLINE inline internals &get_internals() {
+PYBIND11_NOINLINE internals &get_internals() {
     auto **&internals_pp = get_internals_pp();
     if (internals_pp && *internals_pp)
         return **internals_pp;
 
     // Ensure that the GIL is held since we will need to make Python calls.
     // Cannot use py::gil_scoped_acquire here since that constructor calls get_internals.
     struct gil_scoped_acquire_local {
@@ -272,55 +329,102 @@
         internals_pp = static_cast<internals **>(capsule(builtins[id]));
 
         // We loaded builtins through python's builtins, which means that our `error_already_set`
         // and `builtin_exception` may be different local classes than the ones set up in the
         // initial exception translator, below, so add another for our local exception classes.
         //
         // libstdc++ doesn't require this (types there are identified only by name)
+        // libc++ with CPython doesn't require this (types are explicitly exported)
+        // libc++ with PyPy still need it, awaiting further investigation
 #if !defined(__GLIBCXX__)
         (*internals_pp)->registered_exception_translators.push_front(&translate_local_exception);
 #endif
     } else {
         if (!internals_pp) internals_pp = new internals*();
         auto *&internals_ptr = *internals_pp;
         internals_ptr = new internals();
 #if defined(WITH_THREAD)
 
-        #if PY_VERSION_HEX < 0x03090000
-                PyEval_InitThreads();
-        #endif
+#    if PY_VERSION_HEX < 0x03090000
+        PyEval_InitThreads();
+#    endif
         PyThreadState *tstate = PyThreadState_Get();
-        #if PY_VERSION_HEX >= 0x03070000
-            internals_ptr->tstate = PyThread_tss_alloc();
-            if (!internals_ptr->tstate || PyThread_tss_create(internals_ptr->tstate))
-                pybind11_fail("get_internals: could not successfully initialize the TSS key!");
-            PyThread_tss_set(internals_ptr->tstate, tstate);
-        #else
-            internals_ptr->tstate = PyThread_create_key();
-            if (internals_ptr->tstate == -1)
-                pybind11_fail("get_internals: could not successfully initialize the TLS key!");
-            PyThread_set_key_value(internals_ptr->tstate, tstate);
-        #endif
+        if (!PYBIND11_TLS_KEY_CREATE(internals_ptr->tstate)) {
+            pybind11_fail("get_internals: could not successfully initialize the tstate TSS key!");
+        }
+        PYBIND11_TLS_REPLACE_VALUE(internals_ptr->tstate, tstate);
+
+#    if PYBIND11_INTERNALS_VERSION > 4
+        if (!PYBIND11_TLS_KEY_CREATE(internals_ptr->loader_life_support_tls_key)) {
+            pybind11_fail("get_internals: could not successfully initialize the "
+                          "loader_life_support TSS key!");
+        }
+#    endif
         internals_ptr->istate = tstate->interp;
 #endif
         builtins[id] = capsule(internals_pp);
         internals_ptr->registered_exception_translators.push_front(&translate_exception);
         internals_ptr->static_property_type = make_static_property_type();
         internals_ptr->default_metaclass = make_default_metaclass();
         internals_ptr->instance_base = make_object_base_type(internals_ptr->default_metaclass);
     }
     return **internals_pp;
 }
 
-/// Works like `internals.registered_types_cpp`, but for module-local registered types:
-inline type_map<type_info *> &registered_local_types_cpp() {
-    static type_map<type_info *> locals{};
-    return locals;
+// the internals struct (above) is shared between all the modules. local_internals are only
+// for a single module. Any changes made to internals may require an update to
+// PYBIND11_INTERNALS_VERSION, breaking backwards compatibility. local_internals is, by design,
+// restricted to a single module. Whether a module has local internals or not should not
+// impact any other modules, because the only things accessing the local internals is the
+// module that contains them.
+struct local_internals {
+    type_map<type_info *> registered_types_cpp;
+    std::forward_list<ExceptionTranslator> registered_exception_translators;
+#if defined(WITH_THREAD) && PYBIND11_INTERNALS_VERSION == 4
+
+    // For ABI compatibility, we can't store the loader_life_support TLS key in
+    // the `internals` struct directly.  Instead, we store it in `shared_data` and
+    // cache a copy in `local_internals`.  If we allocated a separate TLS key for
+    // each instance of `local_internals`, we could end up allocating hundreds of
+    // TLS keys if hundreds of different pybind11 modules are loaded (which is a
+    // plausible number).
+    PYBIND11_TLS_KEY_INIT(loader_life_support_tls_key)
+
+    // Holds the shared TLS key for the loader_life_support stack.
+    struct shared_loader_life_support_data {
+        PYBIND11_TLS_KEY_INIT(loader_life_support_tls_key)
+        shared_loader_life_support_data() {
+            if (!PYBIND11_TLS_KEY_CREATE(loader_life_support_tls_key)) {
+                pybind11_fail("local_internals: could not successfully initialize the "
+                              "loader_life_support TLS key!");
+            }
+        }
+        // We can't help but leak the TLS key, because Python never unloads extension modules.
+    };
+
+    local_internals() {
+        auto &internals = get_internals();
+        // Get or create the `loader_life_support_stack_key`.
+        auto &ptr = internals.shared_data["_life_support"];
+        if (!ptr) {
+            ptr = new shared_loader_life_support_data;
+        }
+        loader_life_support_tls_key
+            = static_cast<shared_loader_life_support_data *>(ptr)->loader_life_support_tls_key;
+    }
+#endif //  defined(WITH_THREAD) && PYBIND11_INTERNALS_VERSION == 4
+};
+
+/// Works like `get_internals`, but for things which are locally registered.
+inline local_internals &get_local_internals() {
+  static local_internals locals;
+  return locals;
 }
 
+
 /// Constructs a std::string with the given arguments, stores it in `internals`, and returns its
 /// `c_str()`.  Such strings objects have a long storage duration -- the internal strings are only
 /// cleared when the program exits or after interpreter shutdown (when embedding), and so are
 /// suitable for c-style strings needed by Python internals (such as PyTypeObject's tp_name).
 template <typename... Args>
 const char *c_str(Args &&...args) {
     auto &strings = get_internals().static_strings;
@@ -329,22 +433,22 @@
 }
 
 PYBIND11_NAMESPACE_END(detail)
 
 /// Returns a named pointer that is shared among all extension modules (using the same
 /// pybind11 version) running in the current interpreter. Names starting with underscores
 /// are reserved for internal usage. Returns `nullptr` if no matching entry was found.
-inline PYBIND11_NOINLINE void *get_shared_data(const std::string &name) {
+PYBIND11_NOINLINE void *get_shared_data(const std::string &name) {
     auto &internals = detail::get_internals();
     auto it = internals.shared_data.find(name);
     return it != internals.shared_data.end() ? it->second : nullptr;
 }
 
 /// Set the shared data that can be later recovered by `get_shared_data()`.
-inline PYBIND11_NOINLINE void *set_shared_data(const std::string &name, void *data) {
+PYBIND11_NOINLINE void *set_shared_data(const std::string &name, void *data) {
     detail::get_internals().shared_data[name] = data;
     return data;
 }
 
 /// Returns a typed reference to a shared data entry (by using `get_shared_data()`) if
 /// such entry exists. Otherwise, a new object of default-constructible type `T` is
 /// added to the shared data under the given name and a reference to it is returned.
```

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/detail/typeid.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/detail/typeid.h`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     for (size_t pos = 0;;) {
         pos = string.find(search, pos);
         if (pos == std::string::npos) break;
         string.erase(pos, search.length());
     }
 }
 
-PYBIND11_NOINLINE inline void clean_type_id(std::string &name) {
+PYBIND11_NOINLINE void clean_type_id(std::string &name) {
 #if defined(__GNUG__)
     int status = 0;
     std::unique_ptr<char, void (*)(void *)> res {
         abi::__cxa_demangle(name.c_str(), nullptr, nullptr, &status), std::free };
     if (status == 0)
         name = res.get();
 #else
```

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/eigen.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/eigen.h`

 * *Files 4% similar despite different names*

```diff
@@ -5,41 +5,39 @@
 
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
-#include "numpy.h"
+/* HINT: To suppress warnings originating from the Eigen headers, use -isystem.
+   See also:
+       https://stackoverflow.com/questions/2579576/i-dir-vs-isystem-dir
+       https://stackoverflow.com/questions/1741816/isystem-for-ms-visual-studio-c-compiler
+*/
 
-#if defined(__INTEL_COMPILER)
-#  pragma warning(disable: 1682) // implicit conversion of a 64-bit integral type to a smaller integral type (potential portability problem)
-#elif defined(__GNUG__) || defined(__clang__)
-#  pragma GCC diagnostic push
-#  pragma GCC diagnostic ignored "-Wconversion"
-#  pragma GCC diagnostic ignored "-Wdeprecated-declarations"
-#  ifdef __clang__
-//   Eigen generates a bunch of implicit-copy-constructor-is-deprecated warnings with -Wdeprecated
-//   under Clang, so disable that warning here:
-#    pragma GCC diagnostic ignored "-Wdeprecated"
-#  endif
-#  if __GNUC__ >= 7
-#    pragma GCC diagnostic ignored "-Wint-in-bool-context"
-#  endif
-#endif
+#include "numpy.h"
 
+// The C4127 suppression was introduced for Eigen 3.4.0. In theory we could
+// make it version specific, or even remove it later, but considering that
+// 1. C4127 is generally far more distracting than useful for modern template code, and
+// 2. we definitely want to ignore any MSVC warnings originating from Eigen code,
+// it is probably best to keep this around indefinitely.
 #if defined(_MSC_VER)
 #  pragma warning(push)
-#  pragma warning(disable: 4127) // warning C4127: Conditional expression is constant
-#  pragma warning(disable: 4996) // warning C4996: std::unary_negate is deprecated in C++17
+#  pragma warning(disable: 4127) // C4127: conditional expression is constant
 #endif
 
 #include <Eigen/Core>
 #include <Eigen/SparseCore>
 
+#if defined(_MSC_VER)
+#  pragma warning(pop)
+#endif
+
 // Eigen prior to 3.2.7 doesn't have proper move constructors--but worse, some classes get implicit
 // move constructors that break things.  We could detect this an explicitly copy, but an extra copy
 // of matrices seems highly undesirable.
 static_assert(EIGEN_VERSION_AT_LEAST(3,2,7), "Eigen support in pybind11 requires Eigen >= 3.2.7");
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
@@ -48,16 +46,20 @@
 template <typename MatrixType> using EigenDRef = Eigen::Ref<MatrixType, 0, EigenDStride>;
 template <typename MatrixType> using EigenDMap = Eigen::Map<MatrixType, 0, EigenDStride>;
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 #if EIGEN_VERSION_AT_LEAST(3,3,0)
 using EigenIndex = Eigen::Index;
+template<typename Scalar, int Flags, typename StorageIndex>
+using EigenMapSparseMatrix = Eigen::Map<Eigen::SparseMatrix<Scalar, Flags, StorageIndex>>;
 #else
 using EigenIndex = EIGEN_DEFAULT_DENSE_INDEX_TYPE;
+template<typename Scalar, int Flags, typename StorageIndex>
+using EigenMapSparseMatrix = Eigen::MappedSparseMatrix<Scalar, Flags, StorageIndex>;
 #endif
 
 // Matches Eigen::Map, Eigen::Ref, blocks, etc:
 template <typename T> using is_eigen_dense_map = all_of<is_template_base_of<Eigen::DenseBase, T>, std::is_base_of<Eigen::MapBase<T, Eigen::ReadOnlyAccessors>, T>>;
 template <typename T> using is_eigen_mutable_map = std::is_base_of<Eigen::MapBase<T, Eigen::WriteAccessors>, T>;
 template <typename T> using is_eigen_dense_plain = all_of<negation<is_eigen_dense_map<T>>, is_template_base_of<Eigen::PlainObjectBase, T>>;
 template <typename T> using is_eigen_sparse = is_template_base_of<Eigen::SparseMatrixBase, T>;
@@ -73,26 +75,25 @@
 // Captures numpy/eigen conformability status (returned by EigenProps::conformable()):
 template <bool EigenRowMajor> struct EigenConformable {
     bool conformable = false;
     EigenIndex rows = 0, cols = 0;
     EigenDStride stride{0, 0};      // Only valid if negativestrides is false!
     bool negativestrides = false;   // If true, do not use stride!
 
+    // NOLINTNEXTLINE(google-explicit-constructor)
     EigenConformable(bool fits = false) : conformable{fits} {}
     // Matrix type:
     EigenConformable(EigenIndex r, EigenIndex c,
             EigenIndex rstride, EigenIndex cstride) :
-        conformable{true}, rows{r}, cols{c} {
-        // TODO: when Eigen bug #747 is fixed, remove the tests for non-negativity. http://eigen.tuxfamily.org/bz/show_bug.cgi?id=747
-        if (rstride < 0 || cstride < 0) {
-            negativestrides = true;
-        } else {
-            stride = {EigenRowMajor ? rstride : cstride /* outer stride */,
-                      EigenRowMajor ? cstride : rstride /* inner stride */ };
-        }
+        conformable{true}, rows{r}, cols{c},
+        //TODO: when Eigen bug #747 is fixed, remove the tests for non-negativity. http://eigen.tuxfamily.org/bz/show_bug.cgi?id=747
+        stride{EigenRowMajor ? (rstride > 0 ? rstride : 0) : (cstride > 0 ? cstride : 0) /* outer stride */,
+               EigenRowMajor ? (cstride > 0 ? cstride : 0) : (rstride > 0 ? rstride : 0) /* inner stride */ },
+        negativestrides{rstride < 0 || cstride < 0} {
+
     }
     // Vector type:
     EigenConformable(EigenIndex r, EigenIndex c, EigenIndex stride)
         : EigenConformable(r, c, r == 1 ? c*stride : stride, c == 1 ? r : r*stride) {}
 
     template <typename props> bool stride_compatible() const {
         // To have compatible strides, we need (on both dimensions) one of fully dynamic strides,
@@ -100,14 +101,15 @@
         return
             !negativestrides &&
             (props::inner_stride == Eigen::Dynamic || props::inner_stride == stride.inner() ||
                 (EigenRowMajor ? cols : rows) == 1) &&
             (props::outer_stride == Eigen::Dynamic || props::outer_stride == stride.outer() ||
                 (EigenRowMajor ? rows : cols) == 1);
     }
+    // NOLINTNEXTLINE(google-explicit-constructor)
     operator bool() const { return conformable; }
 };
 
 template <typename Type> struct eigen_extract_stride { using type = Type; };
 template <typename PlainObjectType, int MapOptions, typename StrideType>
 struct eigen_extract_stride<Eigen::Map<PlainObjectType, MapOptions, StrideType>> { using type = StrideType; };
 template <typename PlainObjectType, int Options, typename StrideType>
@@ -149,67 +151,65 @@
         if (dims == 2) { // Matrix type: require exact match (or dynamic)
 
             EigenIndex
                 np_rows = a.shape(0),
                 np_cols = a.shape(1),
                 np_rstride = a.strides(0) / static_cast<ssize_t>(sizeof(Scalar)),
                 np_cstride = a.strides(1) / static_cast<ssize_t>(sizeof(Scalar));
-            if ((fixed_rows && np_rows != rows) || (fixed_cols && np_cols != cols))
+            if ((PYBIND11_SILENCE_MSVC_C4127(fixed_rows) && np_rows != rows) ||
+                (PYBIND11_SILENCE_MSVC_C4127(fixed_cols) && np_cols != cols))
                 return false;
 
             return {np_rows, np_cols, np_rstride, np_cstride};
         }
 
         // Otherwise we're storing an n-vector.  Only one of the strides will be used, but whichever
         // is used, we want the (single) numpy stride value.
         const EigenIndex n = a.shape(0),
               stride = a.strides(0) / static_cast<ssize_t>(sizeof(Scalar));
 
         if (vector) { // Eigen type is a compile-time vector
-            if (fixed && size != n)
+            if (PYBIND11_SILENCE_MSVC_C4127(fixed) && size != n)
                 return false; // Vector size mismatch
             return {rows == 1 ? 1 : n, cols == 1 ? 1 : n, stride};
         }
-        else if (fixed) {
+        if (fixed) {
             // The type has a fixed size, but is not a vector: abort
             return false;
         }
-        else if (fixed_cols) {
+        if (fixed_cols) {
             // Since this isn't a vector, cols must be != 1.  We allow this only if it exactly
             // equals the number of elements (rows is Dynamic, and so 1 row is allowed).
             if (cols != n) return false;
             return {1, n, stride};
-        }
-        else {
-            // Otherwise it's either fully dynamic, or column dynamic; both become a column vector
-            if (fixed_rows && rows != n) return false;
+        } // Otherwise it's either fully dynamic, or column dynamic; both become a column vector
+            if (PYBIND11_SILENCE_MSVC_C4127(fixed_rows) && rows != n) return false;
             return {n, 1, stride};
-        }
     }
 
     static constexpr bool show_writeable = is_eigen_dense_map<Type>::value && is_eigen_mutable_map<Type>::value;
     static constexpr bool show_order = is_eigen_dense_map<Type>::value;
     static constexpr bool show_c_contiguous = show_order && requires_row_major;
     static constexpr bool show_f_contiguous = !show_c_contiguous && show_order && requires_col_major;
 
     static constexpr auto descriptor =
-        _("numpy.ndarray[") + npy_format_descriptor<Scalar>::name +
-        _("[")  + _<fixed_rows>(_<(size_t) rows>(), _("m")) +
-        _(", ") + _<fixed_cols>(_<(size_t) cols>(), _("n")) +
-        _("]") +
+        const_name("numpy.ndarray[") + npy_format_descriptor<Scalar>::name +
+        const_name("[")  + const_name<fixed_rows>(const_name<(size_t) rows>(), const_name("m")) +
+        const_name(", ") + const_name<fixed_cols>(const_name<(size_t) cols>(), const_name("n")) +
+        const_name("]") +
         // For a reference type (e.g. Ref<MatrixXd>) we have other constraints that might need to be
         // satisfied: writeable=True (for a mutable reference), and, depending on the map's stride
         // options, possibly f_contiguous or c_contiguous.  We include them in the descriptor output
         // to provide some hint as to why a TypeError is occurring (otherwise it can be confusing to
         // see that a function accepts a 'numpy.ndarray[float64[3,2]]' and an error message that you
         // *gave* a numpy.ndarray of the right type and dimensions.
-        _<show_writeable>(", flags.writeable", "") +
-        _<show_c_contiguous>(", flags.c_contiguous", "") +
-        _<show_f_contiguous>(", flags.f_contiguous", "") +
-        _("]");
+        const_name<show_writeable>(", flags.writeable", "") +
+        const_name<show_c_contiguous>(", flags.c_contiguous", "") +
+        const_name<show_f_contiguous>(", flags.f_contiguous", "") +
+        const_name("]");
 };
 
 // Casts an Eigen type to numpy array.  If given a base, the numpy array references the src data,
 // otherwise it'll make a copy.  writeable lets you turn off the writeable flag for the array.
 template <typename props> handle eigen_array_cast(typename props::Type const &src, handle base = handle(), bool writeable = true) {
     constexpr ssize_t elem_size = sizeof(typename props::Scalar);
     array a;
@@ -340,16 +340,19 @@
     // const pointer return
     static handle cast(const Type *src, return_value_policy policy, handle parent) {
         return cast_impl(src, policy, parent);
     }
 
     static constexpr auto name = props::descriptor;
 
+    // NOLINTNEXTLINE(google-explicit-constructor)
     operator Type*() { return &value; }
+    // NOLINTNEXTLINE(google-explicit-constructor)
     operator Type&() { return value; }
+    // NOLINTNEXTLINE(google-explicit-constructor)
     operator Type&&() && { return std::move(value); }
     template <typename T> using cast_op_type = movable_cast_op_type<T>;
 
 private:
     Type value;
 };
 
@@ -465,15 +468,17 @@
         ref.reset();
         map.reset(new MapType(data(copy_or_ref), fits.rows, fits.cols, make_stride(fits.stride.outer(), fits.stride.inner())));
         ref.reset(new Type(*map));
 
         return true;
     }
 
+    // NOLINTNEXTLINE(google-explicit-constructor)
     operator Type*() { return ref.get(); }
+    // NOLINTNEXTLINE(google-explicit-constructor)
     operator Type&() { return *ref; }
     template <typename _T> using cast_op_type = pybind11::detail::cast_op_type<_T>;
 
 private:
     template <typename T = Type, enable_if_t<is_eigen_mutable_map<T>::value, int> = 0>
     Scalar *data(Array &a) { return a.mutable_data(); }
 
@@ -566,15 +571,17 @@
         auto outerIndices = array_t<StorageIndex>((object) obj.attr("indptr"));
         auto shape = pybind11::tuple((pybind11::object) obj.attr("shape"));
         auto nnz = obj.attr("nnz").cast<Index>();
 
         if (!values || !innerIndices || !outerIndices)
             return false;
 
-        value = Eigen::MappedSparseMatrix<Scalar, Type::Flags, StorageIndex>(
+        value = EigenMapSparseMatrix<Scalar,
+                                     Type::Flags & (Eigen::RowMajor | Eigen::ColMajor),
+                                     StorageIndex>(
             shape[0].cast<Index>(), shape[1].cast<Index>(), nnz,
             outerIndices.mutable_data(), innerIndices.mutable_data(), values.mutable_data());
 
         return true;
     }
 
     static handle cast(const Type &src, return_value_policy /* policy */, handle /* parent */) {
@@ -589,19 +596,13 @@
 
         return matrix_type(
             std::make_tuple(data, innerIndices, outerIndices),
             std::make_pair(src.rows(), src.cols())
         ).release();
     }
 
-    PYBIND11_TYPE_CASTER(Type, _<(Type::IsRowMajor) != 0>("scipy.sparse.csr_matrix[", "scipy.sparse.csc_matrix[")
-            + npy_format_descriptor<Scalar>::name + _("]"));
+    PYBIND11_TYPE_CASTER(Type, const_name<(Type::IsRowMajor) != 0>("scipy.sparse.csr_matrix[", "scipy.sparse.csc_matrix[")
+            + npy_format_descriptor<Scalar>::name + const_name("]"));
 };
 
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
-
-#if defined(__GNUG__) || defined(__clang__)
-#  pragma GCC diagnostic pop
-#elif defined(_MSC_VER)
-#  pragma warning(pop)
-#endif
```

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/eval.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/eval.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 /*
-    pybind11/exec.h: Support for evaluating Python expressions and statements
+    pybind11/eval.h: Support for evaluating Python expressions and statements
     from strings and files
 
     Copyright (c) 2016 Klemens Morgenstern <klemens.morgenstern@ed-chemnitz.de> and
                        Wenzel Jakob <wenzel.jakob@epfl.ch>
 
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
+#include <utility>
+
 #include "pybind11.h"
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 inline void ensure_builtins_in_globals(object &global) {
-    #if PY_VERSION_HEX < 0x03080000
+    #if defined(PYPY_VERSION) || PY_VERSION_HEX < 0x03080000
         // Running exec and eval on Python 2 and 3 adds `builtins` module under
         // `__builtins__` key to globals if not yet present.
         // Python 3.8 made PyRun_String behave similarly. Let's also do that for
-        // older versions, for consistency.
+        // older versions, for consistency. This was missing from PyPy3.8 7.3.7.
         if (!global.contains("__builtins__"))
             global["__builtins__"] = module_::import(PYBIND11_BUILTINS_MODULE);
     #else
         (void) global;
     #endif
 }
 
@@ -39,25 +41,25 @@
     eval_single_statement,
 
     /// Evaluate a string containing a sequence of statement. Returns \c none
     eval_statements
 };
 
 template <eval_mode mode = eval_expr>
-object eval(str expr, object global = globals(), object local = object()) {
+object eval(const str &expr, object global = globals(), object local = object()) {
     if (!local)
         local = global;
 
     detail::ensure_builtins_in_globals(global);
 
     /* PyRun_String does not accept a PyObject / encoding specifier,
        this seems to be the only alternative */
     std::string buffer = "# -*- coding: utf-8 -*-\n" + (std::string) expr;
 
-    int start;
+    int start = 0;
     switch (mode) {
         case eval_expr:             start = Py_eval_input;   break;
         case eval_single_statement: start = Py_single_input; break;
         case eval_statements:       start = Py_file_input;   break;
         default: pybind11_fail("invalid evaluation mode");
     }
 
@@ -71,16 +73,16 @@
 object eval(const char (&s)[N], object global = globals(), object local = object()) {
     /* Support raw string literals by removing common leading whitespace */
     auto expr = (s[0] == '\n') ? str(module_::import("textwrap").attr("dedent")(s))
                                : str(s);
     return eval<mode>(expr, global, local);
 }
 
-inline void exec(str expr, object global = globals(), object local = object()) {
-    eval<eval_statements>(expr, global, local);
+inline void exec(const str &expr, object global = globals(), object local = object()) {
+    eval<eval_statements>(expr, std::move(global), std::move(local));
 }
 
 template <size_t N>
 void exec(const char (&s)[N], object global = globals(), object local = object()) {
     eval<eval_statements>(s, global, local);
 }
 
@@ -101,15 +103,15 @@
 template <eval_mode mode = eval_statements>
 object eval_file(str fname, object global = globals(), object local = object()) {
     if (!local)
         local = global;
 
     detail::ensure_builtins_in_globals(global);
 
-    int start;
+    int start = 0;
     switch (mode) {
         case eval_expr:             start = Py_eval_input;   break;
         case eval_single_statement: start = Py_single_input; break;
         case eval_statements:       start = Py_file_input;   break;
         default: pybind11_fail("invalid evaluation mode");
     }
 
@@ -130,14 +132,23 @@
     closeFile = 0;
 #endif
     if (!f) {
         PyErr_Clear();
         pybind11_fail("File \"" + fname_str + "\" could not be opened!");
     }
 
+    // In Python2, this should be encoded by getfilesystemencoding.
+    // We don't boher setting it since Python2 is past EOL anyway.
+    // See PR#3233
+#if PY_VERSION_HEX >= 0x03000000
+    if (!global.contains("__file__")) {
+        global["__file__"] = std::move(fname);
+    }
+#endif
+
 #if PY_VERSION_HEX < 0x03000000 && defined(PYPY_VERSION)
     PyObject *result = PyRun_File(f, fname_str.c_str(), start, global.ptr(),
                                   local.ptr());
     (void) closeFile;
 #else
     PyObject *result = PyRun_FileEx(f, fname_str.c_str(), start, global.ptr(),
                                     local.ptr(), closeFile);
```

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/functional.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/functional.h`

 * *Files 10% similar despite different names*

```diff
@@ -39,43 +39,61 @@
            function via Python, every function call would normally involve
            a full C++ -> Python -> C++ roundtrip, which can be prohibitive.
            Here, we try to at least detect the case where the function is
            stateless (i.e. function pointer or lambda function without
            captured variables), in which case the roundtrip can be avoided.
          */
         if (auto cfunc = func.cpp_function()) {
-            auto c = reinterpret_borrow<capsule>(PyCFunction_GET_SELF(cfunc.ptr()));
-            auto rec = (function_record *) c;
-
-            if (rec && rec->is_stateless &&
-                    same_type(typeid(function_type), *reinterpret_cast<const std::type_info *>(rec->data[1]))) {
-                struct capture { function_type f; };
-                value = ((capture *) &rec->data)->f;
-                return true;
+            auto cfunc_self = PyCFunction_GET_SELF(cfunc.ptr());
+            if (isinstance<capsule>(cfunc_self)) {
+                auto c = reinterpret_borrow<capsule>(cfunc_self);
+                auto rec = (function_record *) c;
+
+                while (rec != nullptr) {
+                    if (rec->is_stateless
+                        && same_type(typeid(function_type),
+                                     *reinterpret_cast<const std::type_info *>(rec->data[1]))) {
+                        struct capture {
+                            function_type f;
+                        };
+                        value = ((capture *) &rec->data)->f;
+                        return true;
+                    }
+                    rec = rec->next;
+                }
             }
+            // PYPY segfaults here when passing builtin function like sum.
+            // Raising an fail exception here works to prevent the segfault, but only on gcc.
+            // See PR #1413 for full details
         }
 
         // ensure GIL is held during functor destruction
         struct func_handle {
             function f;
-            func_handle(function&& f_) : f(std::move(f_)) {}
-            func_handle(const func_handle& f_) {
+#if !(defined(_MSC_VER) && _MSC_VER == 1916 && defined(PYBIND11_CPP17))
+            // This triggers a syntax error under very special conditions (very weird indeed).
+            explicit
+#endif
+            func_handle(function &&f_) noexcept : f(std::move(f_)) {}
+            func_handle(const func_handle &f_) { operator=(f_); }
+            func_handle &operator=(const func_handle &f_) {
                 gil_scoped_acquire acq;
                 f = f_.f;
+                return *this;
             }
             ~func_handle() {
                 gil_scoped_acquire acq;
                 function kill_f(std::move(f));
             }
         };
 
         // to emulate 'move initialization capture' in C++11
         struct func_wrapper {
             func_handle hfunc;
-            func_wrapper(func_handle&& hf): hfunc(std::move(hf)) {}
+            explicit func_wrapper(func_handle &&hf) noexcept : hfunc(std::move(hf)) {}
             Return operator()(Args... args) const {
                 gil_scoped_acquire acq;
                 object retval(hfunc.f(std::forward<Args>(args)...));
                 /* Visual studio 2015 parser issue: need parentheses around this expression */
                 return (retval.template cast<Return>());
             }
         };
@@ -88,17 +106,16 @@
     static handle cast(Func &&f_, return_value_policy policy, handle /* parent */) {
         if (!f_)
             return none().inc_ref();
 
         auto result = f_.template target<function_type>();
         if (result)
             return cpp_function(*result, policy).release();
-        else
-            return cpp_function(std::forward<Func>(f_), policy).release();
+        return cpp_function(std::forward<Func>(f_), policy).release();
     }
 
-    PYBIND11_TYPE_CASTER(type, _("Callable[[") + concat(make_caster<Args>::name...) + _("], ")
-                               + make_caster<retval_type>::name + _("]"));
+    PYBIND11_TYPE_CASTER(type, const_name("Callable[[") + concat(make_caster<Args>::name...) + const_name("], ")
+                               + make_caster<retval_type>::name + const_name("]"));
 };
 
 PYBIND11_NAMESPACE_END(detail)
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/numpy.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/numpy.h`

 * *Files 3% similar despite different names*

```diff
@@ -21,34 +21,29 @@
 #include <string>
 #include <functional>
 #include <type_traits>
 #include <utility>
 #include <vector>
 #include <typeindex>
 
-#if defined(_MSC_VER)
-#  pragma warning(push)
-#  pragma warning(disable: 4127) // warning C4127: Conditional expression is constant
-#endif
-
 /* This will be true on all flat address space platforms and allows us to reduce the
    whole npy_intp / ssize_t / Py_intptr_t business down to just ssize_t for all size
    and dimension types (e.g. shape, strides, indexing), instead of inflicting this
    upon the library user. */
 static_assert(sizeof(::pybind11::ssize_t) == sizeof(Py_intptr_t), "ssize_t != Py_intptr_t");
 static_assert(std::is_signed<Py_intptr_t>::value, "Py_intptr_t must be signed");
 // We now can reinterpret_cast between py::ssize_t and Py_intptr_t (MSVC + PyPy cares)
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
 class array; // Forward declaration
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
-template <> struct handle_type_name<array> { static constexpr auto name = _("numpy.ndarray"); };
+template <> struct handle_type_name<array> { static constexpr auto name = const_name("numpy.ndarray"); };
 
 template <typename type, typename SFINAE = void> struct npy_format_descriptor;
 
 struct PyArrayDescr_Proxy {
     PyObject_HEAD
     PyObject *typeobj;
     char kind;
@@ -100,15 +95,15 @@
     }
 
     template<typename T> numpy_type_info *get_type_info(bool throw_if_missing = true) {
         return get_type_info(typeid(typename std::remove_cv<T>::type), throw_if_missing);
     }
 };
 
-inline PYBIND11_NOINLINE void load_numpy_internals(numpy_internals* &ptr) {
+PYBIND11_NOINLINE void load_numpy_internals(numpy_internals* &ptr) {
     ptr = &get_or_create_shared_data<numpy_internals>("_numpy_internals");
 }
 
 inline numpy_internals& get_numpy_internals() {
     static numpy_internals* ptr = nullptr;
     if (!ptr)
         load_numpy_internals(ptr);
@@ -160,18 +155,18 @@
             NPY_ULONG_, NPY_UINT_, NPY_USHORT_),
         NPY_INT64_ = platform_lookup<std::int64_t, long, long long, int>(
             NPY_LONG_, NPY_LONGLONG_, NPY_INT_),
         NPY_UINT64_ = platform_lookup<std::uint64_t, unsigned long, unsigned long long, unsigned int>(
             NPY_ULONG_, NPY_ULONGLONG_, NPY_UINT_),
     };
 
-    typedef struct {
+    struct PyArray_Dims {
         Py_intptr_t *ptr;
         int len;
-    } PyArray_Dims;
+    };
 
     static npy_api& get() {
         static npy_api api = lookup();
         return api;
     }
 
     bool PyArray_Check_(PyObject *obj) const {
@@ -199,32 +194,37 @@
     bool (*PyArray_EquivTypes_) (PyObject *, PyObject *);
     int (*PyArray_GetArrayParamsFromObject_)(PyObject *, PyObject *, unsigned char, PyObject **, int *,
                                              Py_intptr_t *, PyObject **, PyObject *);
     PyObject *(*PyArray_Squeeze_)(PyObject *);
     // Unused. Not removed because that affects ABI of the class.
     int (*PyArray_SetBaseObject_)(PyObject *, PyObject *);
     PyObject* (*PyArray_Resize_)(PyObject*, PyArray_Dims*, int, int);
+    PyObject* (*PyArray_Newshape_)(PyObject*, PyArray_Dims*, int);
+    PyObject* (*PyArray_View_)(PyObject*, PyObject*, PyObject*);
+
 private:
     enum functions {
         API_PyArray_GetNDArrayCFeatureVersion = 211,
         API_PyArray_Type = 2,
         API_PyArrayDescr_Type = 3,
         API_PyVoidArrType_Type = 39,
         API_PyArray_DescrFromType = 45,
         API_PyArray_DescrFromScalar = 57,
         API_PyArray_FromAny = 69,
         API_PyArray_Resize = 80,
         API_PyArray_CopyInto = 82,
         API_PyArray_NewCopy = 85,
         API_PyArray_NewFromDescr = 94,
         API_PyArray_DescrNewFromType = 96,
+        API_PyArray_Newshape = 135,
+        API_PyArray_Squeeze = 136,
+        API_PyArray_View = 137,
         API_PyArray_DescrConverter = 174,
         API_PyArray_EquivTypes = 182,
         API_PyArray_GetArrayParamsFromObject = 278,
-        API_PyArray_Squeeze = 136,
         API_PyArray_SetBaseObject = 282
     };
 
     static npy_api lookup() {
         module_ m = module_::import("numpy.core.multiarray");
         auto c = m.attr("_ARRAY_API");
 #if PY_MAJOR_VERSION >= 3
@@ -244,19 +244,22 @@
         DECL_NPY_API(PyArray_DescrFromScalar);
         DECL_NPY_API(PyArray_FromAny);
         DECL_NPY_API(PyArray_Resize);
         DECL_NPY_API(PyArray_CopyInto);
         DECL_NPY_API(PyArray_NewCopy);
         DECL_NPY_API(PyArray_NewFromDescr);
         DECL_NPY_API(PyArray_DescrNewFromType);
+        DECL_NPY_API(PyArray_Newshape);
+        DECL_NPY_API(PyArray_Squeeze);
+        DECL_NPY_API(PyArray_View);
         DECL_NPY_API(PyArray_DescrConverter);
         DECL_NPY_API(PyArray_EquivTypes);
         DECL_NPY_API(PyArray_GetArrayParamsFromObject);
-        DECL_NPY_API(PyArray_Squeeze);
         DECL_NPY_API(PyArray_SetBaseObject);
+
 #undef DECL_NPY_API
         return api;
     }
 };
 
 inline PyArray_Proxy* array_proxy(void* ptr) {
     return reinterpret_cast<PyArray_Proxy*>(ptr);
@@ -283,15 +286,15 @@
 template <typename T> struct is_complex : std::false_type { };
 template <typename T> struct is_complex<std::complex<T>> : std::true_type { };
 
 template <typename T> struct array_info_scalar {
     using type = T;
     static constexpr bool is_array = false;
     static constexpr bool is_empty = false;
-    static constexpr auto extents = _("");
+    static constexpr auto extents = const_name("");
     static void append_extents(list& /* shape */) { }
 };
 // Computes underlying type and a comma-separated list of extents for array
 // types (any mix of std::array and built-in arrays). An array of char is
 // treated as scalar because it gets special handling.
 template <typename T> struct array_info : array_info_scalar<T> { };
 template <typename T, size_t N> struct array_info<std::array<T, N>> {
@@ -302,35 +305,34 @@
 
     // appends the extents to shape
     static void append_extents(list& shape) {
         shape.append(N);
         array_info<T>::append_extents(shape);
     }
 
-    static constexpr auto extents = _<array_info<T>::is_array>(
-        concat(_<N>(), array_info<T>::extents), _<N>()
+    static constexpr auto extents = const_name<array_info<T>::is_array>(
+        concat(const_name<N>(), array_info<T>::extents), const_name<N>()
     );
 };
 // For numpy we have special handling for arrays of characters, so we don't include
 // the size in the array extents.
 template <size_t N> struct array_info<char[N]> : array_info_scalar<char[N]> { };
 template <size_t N> struct array_info<std::array<char, N>> : array_info_scalar<std::array<char, N>> { };
 template <typename T, size_t N> struct array_info<T[N]> : array_info<std::array<T, N>> { };
 template <typename T> using remove_all_extents_t = typename array_info<T>::type;
 
 template <typename T> using is_pod_struct = all_of<
     std::is_standard_layout<T>,     // since we're accessing directly in memory we need a standard layout type
-#if !defined(__GNUG__) || defined(_LIBCPP_VERSION) || defined(_GLIBCXX_USE_CXX11_ABI)
-    // _GLIBCXX_USE_CXX11_ABI indicates that we're using libstdc++ from GCC 5 or newer, independent
-    // of the actual compiler (Clang can also use libstdc++, but it always defines __GNUC__ == 4).
-    std::is_trivially_copyable<T>,
-#else
-    // GCC 4 doesn't implement is_trivially_copyable, so approximate it
+#if defined(__GLIBCXX__) && (__GLIBCXX__ < 20150422 || __GLIBCXX__ == 20150426 || __GLIBCXX__ == 20150623 || __GLIBCXX__ == 20150626 || __GLIBCXX__ == 20160803)
+    // libstdc++ < 5 (including versions 4.8.5, 4.9.3 and 4.9.4 which were released after 5)
+    // don't implement is_trivially_copyable, so approximate it
     std::is_trivially_destructible<T>,
     satisfies_any_of<T, std::has_trivial_copy_constructor, std::has_trivial_copy_assign>,
+#else
+    std::is_trivially_copyable<T>,
 #endif
     satisfies_none_of<T, std::is_reference, std::is_array, is_std_array, std::is_arithmetic, is_complex, std::is_enum>
 >;
 
 // Replacement for std::is_pod (deprecated in C++20)
 template <typename T> using is_pod = all_of<
     std::is_standard_layout<T>,
@@ -462,36 +464,38 @@
 class dtype : public object {
 public:
     PYBIND11_OBJECT_DEFAULT(dtype, object, detail::npy_api::get().PyArrayDescr_Check_);
 
     explicit dtype(const buffer_info &info) {
         dtype descr(_dtype_from_pep3118()(PYBIND11_STR_TYPE(info.format)));
         // If info.itemsize == 0, use the value calculated from the format string
-        m_ptr = descr.strip_padding(info.itemsize ? info.itemsize : descr.itemsize()).release().ptr();
+        m_ptr = descr.strip_padding(info.itemsize != 0 ? info.itemsize : descr.itemsize())
+                    .release()
+                    .ptr();
     }
 
     explicit dtype(const std::string &format) {
         m_ptr = from_args(pybind11::str(format)).release().ptr();
     }
 
-    dtype(const char *format) : dtype(std::string(format)) { }
+    explicit dtype(const char *format) : dtype(std::string(format)) {}
 
     dtype(list names, list formats, list offsets, ssize_t itemsize) {
         dict args;
-        args["names"] = names;
-        args["formats"] = formats;
-        args["offsets"] = offsets;
+        args["names"] = std::move(names);
+        args["formats"] = std::move(formats);
+        args["offsets"] = std::move(offsets);
         args["itemsize"] = pybind11::int_(itemsize);
-        m_ptr = from_args(args).release().ptr();
+        m_ptr = from_args(std::move(args)).release().ptr();
     }
 
     /// This is essentially the same as calling numpy.dtype(args) in Python.
     static dtype from_args(object args) {
         PyObject *ptr = nullptr;
-        if (!detail::npy_api::get().PyArray_DescrConverter_(args.ptr(), &ptr) || !ptr)
+        if ((detail::npy_api::get().PyArray_DescrConverter_(args.ptr(), &ptr) == 0) || !ptr)
             throw error_already_set();
         return reinterpret_steal<dtype>(ptr);
     }
 
     /// Return dtype associated with a C++ type.
     template <typename T> static dtype of() {
         return detail::npy_format_descriptor<typename std::remove_cv<T>::type>::dtype();
@@ -503,19 +507,29 @@
     }
 
     /// Returns true for structured data types.
     bool has_fields() const {
         return detail::array_descriptor_proxy(m_ptr)->names != nullptr;
     }
 
-    /// Single-character type code.
+    /// Single-character code for dtype's kind.
+    /// For example, floating point types are 'f' and integral types are 'i'.
     char kind() const {
         return detail::array_descriptor_proxy(m_ptr)->kind;
     }
 
+    /// Single-character for dtype's type.
+    /// For example, ``float`` is 'f', ``double`` 'd', ``int`` 'i', and ``long`` 'l'.
+    char char_() const {
+        // Note: The signature, `dtype::char_` follows the naming of NumPy's
+        // public Python API (i.e., ``dtype.char``), rather than its internal
+        // C API (``PyArray_Descr::type``).
+        return detail::array_descriptor_proxy(m_ptr)->type;
+    }
+
 private:
     static object _dtype_from_pep3118() {
         static PyObject *obj = module_::import("numpy.core._internal")
             .attr("_dtype_from_pep3118").cast<object>().release().ptr();
         return reinterpret_borrow<object>(obj);
     }
 
@@ -529,15 +543,15 @@
         std::vector<field_descr> field_descriptors;
 
         for (auto field : attr("fields").attr("items")()) {
             auto spec = field.cast<tuple>();
             auto name = spec[0].cast<pybind11::str>();
             auto format = spec[1].cast<tuple>()[0].cast<dtype>();
             auto offset = spec[1].cast<tuple>()[1].cast<pybind11::int_>();
-            if (!len(name) && format.kind() == 'V')
+            if ((len(name) == 0u) && format.kind() == 'V')
                 continue;
             field_descriptors.push_back({(PYBIND11_STR_TYPE) name, format.strip_padding(format.itemsize()), offset});
         }
 
         std::sort(field_descriptors.begin(), field_descriptors.end(),
                   [](const field_descr& a, const field_descr& b) {
                       return a.offset.cast<int>() < b.offset.cast<int>();
@@ -545,15 +559,15 @@
 
         list names, formats, offsets;
         for (auto& descr : field_descriptors) {
             names.append(descr.name);
             formats.append(descr.format);
             offsets.append(descr.offset);
         }
-        return dtype(names, formats, offsets, itemsize);
+        return dtype(std::move(names), std::move(formats), std::move(offsets), itemsize);
     }
 };
 
 class array : public buffer {
 public:
     PYBIND11_OBJECT_CVT(array, buffer, detail::npy_api::get().PyArray_Check_, raw_array)
 
@@ -732,29 +746,29 @@
     /**
      * Returns a proxy object that provides access to the array's data without bounds or
      * dimensionality checking.  Will throw if the array is missing the `writeable` flag.  Use with
      * care: the array must not be destroyed or reshaped for the duration of the returned object,
      * and the caller must take care not to access invalid dimensions or dimension indices.
      */
     template <typename T, ssize_t Dims = -1> detail::unchecked_mutable_reference<T, Dims> mutable_unchecked() & {
-        if (Dims >= 0 && ndim() != Dims)
+        if (PYBIND11_SILENCE_MSVC_C4127(Dims >= 0) && ndim() != Dims)
             throw std::domain_error("array has incorrect number of dimensions: " + std::to_string(ndim()) +
                     "; expected " + std::to_string(Dims));
         return detail::unchecked_mutable_reference<T, Dims>(mutable_data(), shape(), strides(), ndim());
     }
 
     /**
      * Returns a proxy object that provides const access to the array's data without bounds or
      * dimensionality checking.  Unlike `mutable_unchecked()`, this does not require that the
      * underlying array have the `writable` flag.  Use with care: the array must not be destroyed or
      * reshaped for the duration of the returned object, and the caller must take care not to access
      * invalid dimensions or dimension indices.
      */
     template <typename T, ssize_t Dims = -1> detail::unchecked_reference<T, Dims> unchecked() const & {
-        if (Dims >= 0 && ndim() != Dims)
+        if (PYBIND11_SILENCE_MSVC_C4127(Dims >= 0) && ndim() != Dims)
             throw std::domain_error("array has incorrect number of dimensions: " + std::to_string(ndim()) +
                     "; expected " + std::to_string(Dims));
         return detail::unchecked_reference<T, Dims>(data(), shape(), strides(), ndim());
     }
 
     /// Return a new view with all of the dimensions of length 1 removed
     array squeeze() {
@@ -775,14 +789,41 @@
         auto new_array = reinterpret_steal<object>(
             detail::npy_api::get().PyArray_Resize_(m_ptr, &d, int(refcheck), -1)
         );
         if (!new_array) throw error_already_set();
         if (isinstance<array>(new_array)) { *this = std::move(new_array); }
     }
 
+    /// Optional `order` parameter omitted, to be added as needed.
+    array reshape(ShapeContainer new_shape) {
+        detail::npy_api::PyArray_Dims d
+            = {reinterpret_cast<Py_intptr_t *>(new_shape->data()), int(new_shape->size())};
+        auto new_array
+            = reinterpret_steal<array>(detail::npy_api::get().PyArray_Newshape_(m_ptr, &d, 0));
+        if (!new_array) {
+            throw error_already_set();
+        }
+        return new_array;
+    }
+
+    /// Create a view of an array in a different data type.
+    /// This function may fundamentally reinterpret the data in the array.
+    /// It is the responsibility of the caller to ensure that this is safe.
+    /// Only supports the `dtype` argument, the `type` argument is omitted,
+    /// to be added as needed.
+    array view(const std::string &dtype) {
+        auto &api = detail::npy_api::get();
+        auto new_view = reinterpret_steal<array>(api.PyArray_View_(
+            m_ptr, dtype::from_args(pybind11::str(dtype)).release().ptr(), nullptr));
+        if (!new_view) {
+            throw error_already_set();
+        }
+        return new_view;
+    }
+
     /// Ensure that the argument is a NumPy array
     /// In case of an error, nullptr is returned and the Python error is cleared.
     static array ensure(handle h, int ExtraFlags = 0) {
         auto result = reinterpret_steal<array>(raw_array(h.ptr(), ExtraFlags));
         if (!result)
             PyErr_Clear();
         return result;
@@ -849,29 +890,31 @@
 
     PYBIND11_DEPRECATED("Use array_t<T>::ensure() instead")
     array_t(handle h, bool is_borrowed) : array(raw_array_t(h.ptr()), stolen_t{}) {
         if (!m_ptr) PyErr_Clear();
         if (!is_borrowed) Py_XDECREF(h.ptr());
     }
 
+    // NOLINTNEXTLINE(google-explicit-constructor)
     array_t(const object &o) : array(raw_array_t(o.ptr()), stolen_t{}) {
         if (!m_ptr) throw error_already_set();
     }
 
     explicit array_t(const buffer_info& info, handle base = handle()) : array(info, base) { }
 
     array_t(ShapeContainer shape, StridesContainer strides, const T *ptr = nullptr, handle base = handle())
         : array(std::move(shape), std::move(strides), ptr, base) { }
 
     explicit array_t(ShapeContainer shape, const T *ptr = nullptr, handle base = handle())
-        : array_t(private_ctor{}, std::move(shape),
-                ExtraFlags & f_style
-                ? detail::f_strides(*shape, itemsize())
-                : detail::c_strides(*shape, itemsize()),
-                ptr, base) { }
+        : array_t(private_ctor{},
+                  std::move(shape),
+                  (ExtraFlags & f_style) != 0 ? detail::f_strides(*shape, itemsize())
+                                              : detail::c_strides(*shape, itemsize()),
+                  ptr,
+                  base) {}
 
     explicit array_t(ssize_t count, const T *ptr = nullptr, handle base = handle())
         : array({count}, {}, ptr, base) { }
 
     constexpr ssize_t itemsize() const {
         return sizeof(T);
     }
@@ -974,15 +1017,15 @@
     }
 };
 
 template <typename T>
 struct format_descriptor<T, detail::enable_if_t<detail::array_info<T>::is_array>> {
     static std::string format() {
         using namespace detail;
-        static constexpr auto extents = _("(") + array_info<T>::extents + _(")");
+        static constexpr auto extents = const_name("(") + array_info<T>::extents + const_name(")");
         return extents.text + format_descriptor<remove_all_extents_t<T>>::format();
     }
 };
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 template <typename T, int ExtraFlags>
 struct pyobject_caster<array_t<T, ExtraFlags>> {
@@ -1009,31 +1052,36 @@
 };
 
 template <typename T, typename = void>
 struct npy_format_descriptor_name;
 
 template <typename T>
 struct npy_format_descriptor_name<T, enable_if_t<std::is_integral<T>::value>> {
-    static constexpr auto name = _<std::is_same<T, bool>::value>(
-        _("bool"), _<std::is_signed<T>::value>("numpy.int", "numpy.uint") + _<sizeof(T)*8>()
+    static constexpr auto name = const_name<std::is_same<T, bool>::value>(
+        const_name("bool"), const_name<std::is_signed<T>::value>("numpy.int", "numpy.uint") + const_name<sizeof(T)*8>()
     );
 };
 
 template <typename T>
 struct npy_format_descriptor_name<T, enable_if_t<std::is_floating_point<T>::value>> {
-    static constexpr auto name = _<std::is_same<T, float>::value || std::is_same<T, double>::value>(
-        _("numpy.float") + _<sizeof(T)*8>(), _("numpy.longdouble")
+    static constexpr auto name = const_name<std::is_same<T, float>::value
+                                   || std::is_same<T, const float>::value
+                                   || std::is_same<T, double>::value
+                                   || std::is_same<T, const double>::value>(
+        const_name("numpy.float") + const_name<sizeof(T)*8>(), const_name("numpy.longdouble")
     );
 };
 
 template <typename T>
 struct npy_format_descriptor_name<T, enable_if_t<is_complex<T>::value>> {
-    static constexpr auto name = _<std::is_same<typename T::value_type, float>::value
-                                   || std::is_same<typename T::value_type, double>::value>(
-        _("numpy.complex") + _<sizeof(typename T::value_type)*16>(), _("numpy.longcomplex")
+    static constexpr auto name = const_name<std::is_same<typename T::value_type, float>::value
+                                   || std::is_same<typename T::value_type, const float>::value
+                                   || std::is_same<typename T::value_type, double>::value
+                                   || std::is_same<typename T::value_type, const double>::value>(
+        const_name("numpy.complex") + const_name<sizeof(typename T::value_type)*16>(), const_name("numpy.longcomplex")
     );
 };
 
 template <typename T>
 struct npy_format_descriptor<T, enable_if_t<satisfies_any_of<T, std::is_arithmetic, is_complex>::value>>
     : npy_format_descriptor_name<T> {
 private:
@@ -1053,27 +1101,27 @@
         if (auto ptr = npy_api::get().PyArray_DescrFromType_(value))
             return reinterpret_steal<pybind11::dtype>(ptr);
         pybind11_fail("Unsupported buffer format!");
     }
 };
 
 #define PYBIND11_DECL_CHAR_FMT \
-    static constexpr auto name = _("S") + _<N>(); \
+    static constexpr auto name = const_name("S") + const_name<N>(); \
     static pybind11::dtype dtype() { return pybind11::dtype(std::string("S") + std::to_string(N)); }
 template <size_t N> struct npy_format_descriptor<char[N]> { PYBIND11_DECL_CHAR_FMT };
 template <size_t N> struct npy_format_descriptor<std::array<char, N>> { PYBIND11_DECL_CHAR_FMT };
 #undef PYBIND11_DECL_CHAR_FMT
 
 template<typename T> struct npy_format_descriptor<T, enable_if_t<array_info<T>::is_array>> {
 private:
     using base_descr = npy_format_descriptor<typename array_info<T>::type>;
 public:
     static_assert(!array_info<T>::is_empty, "Zero-sized arrays are not supported");
 
-    static constexpr auto name = _("(") + array_info<T>::extents + _(")") + base_descr::name;
+    static constexpr auto name = const_name("(") + array_info<T>::extents + const_name(")") + base_descr::name;
     static pybind11::dtype dtype() {
         list shape;
         array_info<T>::append_extents(shape);
         return pybind11::dtype::from_args(pybind11::make_tuple(base_descr::dtype(), shape));
     }
 };
 
@@ -1089,15 +1137,15 @@
     const char *name;
     ssize_t offset;
     ssize_t size;
     std::string format;
     dtype descr;
 };
 
-inline PYBIND11_NOINLINE void register_structured_dtype(
+PYBIND11_NOINLINE void register_structured_dtype(
     any_container<field_descriptor> fields,
     const std::type_info& tinfo, ssize_t itemsize,
     bool (*direct_converter)(PyObject *, void *&)) {
 
     auto& numpy_internals = get_numpy_internals();
     if (numpy_internals.get_type_info(tinfo, false))
         pybind11_fail("NumPy: dtype is already registered");
@@ -1113,15 +1161,18 @@
         if (!field.descr)
             pybind11_fail(std::string("NumPy: unsupported field dtype: `") +
                             field.name + "` @ " + tinfo.name());
         names.append(PYBIND11_STR_TYPE(field.name));
         formats.append(field.descr);
         offsets.append(pybind11::int_(field.offset));
     }
-    auto dtype_ptr = pybind11::dtype(names, formats, offsets, itemsize).release().ptr();
+    auto dtype_ptr
+        = pybind11::dtype(std::move(names), std::move(formats), std::move(offsets), itemsize)
+              .release()
+              .ptr();
 
     // There is an existing bug in NumPy (as of v1.11): trailing bytes are
     // not encoded explicitly into the format string. This will supposedly
     // get fixed in v1.12; for further details, see these:
     // - https://github.com/numpy/numpy/issues/7797
     // - https://github.com/numpy/numpy/pull/7798
     // Because of this, we won't use numpy's logic to generate buffer format
@@ -1273,15 +1324,15 @@
 
 class common_iterator {
 public:
     using container_type = std::vector<ssize_t>;
     using value_type = container_type::value_type;
     using size_type = container_type::size_type;
 
-    common_iterator() : p_ptr(0), m_strides() {}
+    common_iterator() : m_strides() {}
 
     common_iterator(void* ptr, const container_type& strides, const container_type& shape)
         : p_ptr(reinterpret_cast<char*>(ptr)), m_strides(strides.size()) {
         m_strides.back() = static_cast<value_type>(strides.back());
         for (size_type i = m_strides.size() - 1; i != 0; --i) {
             size_type j = i - 1;
             auto s = static_cast<value_type>(shape[i]);
@@ -1294,15 +1345,15 @@
     }
 
     void* data() const {
         return p_ptr;
     }
 
 private:
-    char* p_ptr;
+    char *p_ptr{0};
     container_type m_strides;
 };
 
 template <size_t N> class multi_array_iterator {
 public:
     using container_type = std::vector<ssize_t>;
 
@@ -1322,17 +1373,16 @@
 
     multi_array_iterator& operator++() {
         for (size_t j = m_index.size(); j != 0; --j) {
             size_t i = j - 1;
             if (++m_index[i] != m_shape[i]) {
                 increment_common_iterator(i);
                 break;
-            } else {
-                m_index[i] = 0;
             }
+            m_index[i] = 0;
         }
         return *this;
     }
 
     template <size_t K, class T = void> T* data() const {
         return reinterpret_cast<T*>(m_common_iterator[K].data());
     }
@@ -1475,16 +1525,15 @@
 template <typename Func, typename Return, typename... Args>
 struct vectorize_returned_array {
     using Type = array_t<Return>;
 
     static Type create(broadcast_trivial trivial, const std::vector<ssize_t> &shape) {
         if (trivial == broadcast_trivial::f_trivial)
             return array_t<Return, array::f_style>(shape);
-        else
-            return array_t<Return>(shape);
+        return array_t<Return>(shape);
     }
 
     static Return *mutable_data(Type &array) {
         return array.mutable_data();
     }
 
     static Return call(Func &f, Args &... args) {
@@ -1532,16 +1581,19 @@
 
     static constexpr size_t N = sizeof...(Args);
     static constexpr size_t NVectorized = constexpr_sum(vectorize_arg<Args>::vectorize...);
     static_assert(NVectorized >= 1,
             "pybind11::vectorize(...) requires a function with at least one vectorizable argument");
 
 public:
-    template <typename T>
-    explicit vectorize_helper(T &&f) : f(std::forward<T>(f)) { }
+    template <typename T,
+              // SFINAE to prevent shadowing the copy constructor.
+              typename = detail::enable_if_t<
+                  !std::is_same<vectorize_helper, typename std::decay<T>::type>::value>>
+    explicit vectorize_helper(T &&f) : f(std::forward<T>(f)) {}
 
     object operator()(typename vectorize_arg<Args>::type... args) {
         return run(args...,
                    make_index_sequence<N>(),
                    select_indices<vectorize_arg<Args>::vectorize...>(),
                    make_index_sequence<NVectorized>());
     }
@@ -1649,15 +1701,15 @@
 template <typename Func, typename Return, typename... Args>
 vectorize_helper<Func, Return, Args...>
 vectorize_extractor(const Func &f, Return (*) (Args ...)) {
     return detail::vectorize_helper<Func, Return, Args...>(f);
 }
 
 template <typename T, int Flags> struct handle_type_name<array_t<T, Flags>> {
-    static constexpr auto name = _("numpy.ndarray[") + npy_format_descriptor<T>::name + _("]");
+    static constexpr auto name = const_name("numpy.ndarray[") + npy_format_descriptor<T>::name + const_name("]");
 };
 
 PYBIND11_NAMESPACE_END(detail)
 
 // Vanilla pointer vectorizer:
 template <typename Return, typename... Args>
 detail::vectorize_helper<Return (*)(Args...), Return, Args...>
@@ -1683,11 +1735,7 @@
 template <typename Return, typename Class, typename... Args,
           typename Helper = detail::vectorize_helper<decltype(std::mem_fn(std::declval<Return (Class::*)(Args...) const>())), Return, const Class *, Args...>>
 Helper vectorize(Return (Class::*f)(Args...) const) {
     return Helper(std::mem_fn(f));
 }
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
-
-#if defined(_MSC_VER)
-#pragma warning(pop)
-#endif
```

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/operators.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/operators.h`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,14 @@
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
 #include "pybind11.h"
 
-#if defined(__clang__) && !defined(__INTEL_COMPILER)
-#  pragma clang diagnostic ignored "-Wunsequenced" // multiple unsequenced modifications to 'self' (when using def(py::self OP Type()))
-#elif defined(_MSC_VER)
-#  pragma warning(push)
-#  pragma warning(disable: 4127) // warning C4127: Conditional expression is constant
-#endif
-
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 /// Enumeration with all supported operator types
 enum op_id : int {
     op_add, op_sub, op_mul, op_div, op_mod, op_divmod, op_pow, op_lshift,
     op_rshift, op_and, op_xor, op_or, op_neg, op_pos, op_abs, op_invert,
@@ -54,15 +47,16 @@
     template <typename Class, typename... Extra> void execute(Class &cl, const Extra&... extra) const {
         using Base = typename Class::type;
         using L_type = conditional_t<std::is_same<L, self_t>::value, Base, L>;
         using R_type = conditional_t<std::is_same<R, self_t>::value, Base, R>;
         using op = op_impl<id, ot, Base, L_type, R_type>;
         cl.def(op::name(), &op::execute, is_operator(), extra...);
         #if PY_MAJOR_VERSION < 3
-        if (id == op_truediv || id == op_itruediv)
+        if (PYBIND11_SILENCE_MSVC_C4127(id == op_truediv) ||
+            PYBIND11_SILENCE_MSVC_C4127(id == op_itruediv))
             cl.def(id == op_itruediv ? "__idiv__" : ot == op_l ? "__div__" : "__rdiv__",
                     &op::execute, is_operator(), extra...);
         #endif
     }
     template <typename Class, typename... Extra> void execute_cast(Class &cl, const Extra&... extra) const {
         using Base = typename Class::type;
         using L_type = conditional_t<std::is_same<L, self_t>::value, Base, L>;
@@ -163,11 +157,7 @@
 PYBIND11_NAMESPACE_END(detail)
 
 using detail::self;
 // Add named operators so that they are accessible via `py::`.
 using detail::hash;
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
-
-#if defined(_MSC_VER)
-#  pragma warning(pop)
-#endif
```

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/options.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/pybind11.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/pybind11.h`

 * *Files 3% similar despite different names*

```diff
@@ -6,111 +6,138 @@
 
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
-#if defined(__INTEL_COMPILER)
-#  pragma warning push
-#  pragma warning disable 68    // integer conversion resulted in a change of sign
-#  pragma warning disable 186   // pointless comparison of unsigned integer with zero
-#  pragma warning disable 878   // incompatible exception specifications
-#  pragma warning disable 1334  // the "template" keyword used for syntactic disambiguation may only be used within a template
-#  pragma warning disable 1682  // implicit conversion of a 64-bit integral type to a smaller integral type (potential portability problem)
-#  pragma warning disable 1786  // function "strdup" was declared deprecated
-#  pragma warning disable 1875  // offsetof applied to non-POD (Plain Old Data) types is nonstandard
-#  pragma warning disable 2196  // warning #2196: routine is both "inline" and "noinline"
-#elif defined(_MSC_VER)
-#  pragma warning(push)
-#  pragma warning(disable: 4100) // warning C4100: Unreferenced formal parameter
-#  pragma warning(disable: 4127) // warning C4127: Conditional expression is constant
-#  pragma warning(disable: 4512) // warning C4512: Assignment operator was implicitly defined as deleted
-#  pragma warning(disable: 4800) // warning C4800: 'int': forcing value to bool 'true' or 'false' (performance warning)
-#  pragma warning(disable: 4996) // warning C4996: The POSIX name for this item is deprecated. Instead, use the ISO C and C++ conformant name
-#  pragma warning(disable: 4702) // warning C4702: unreachable code
-#  pragma warning(disable: 4522) // warning C4522: multiple assignment operators specified
-#  pragma warning(disable: 4505) // warning C4505: 'PySlice_GetIndicesEx': unreferenced local function has been removed (PyPy only)
-#elif defined(__GNUG__) && !defined(__clang__)
-#  pragma GCC diagnostic push
-#  pragma GCC diagnostic ignored "-Wunused-but-set-parameter"
-#  pragma GCC diagnostic ignored "-Wunused-but-set-variable"
-#  pragma GCC diagnostic ignored "-Wmissing-field-initializers"
-#  pragma GCC diagnostic ignored "-Wstrict-aliasing"
-#  pragma GCC diagnostic ignored "-Wattributes"
-#  if __GNUC__ >= 7
-#    pragma GCC diagnostic ignored "-Wnoexcept-type"
-#  endif
-#endif
-
 #include "attr.h"
+#include "gil.h"
 #include "options.h"
 #include "detail/class.h"
 #include "detail/init.h"
 
+#include <cstdlib>
 #include <memory>
+#include <new>
 #include <vector>
 #include <string>
 #include <utility>
 
+#include <string.h>
+
+#if defined(__cpp_lib_launder) && !(defined(_MSC_VER) && (_MSC_VER < 1914))
+#  define PYBIND11_STD_LAUNDER std::launder
+#  define PYBIND11_HAS_STD_LAUNDER 1
+#else
+#  define PYBIND11_STD_LAUNDER
+#  define PYBIND11_HAS_STD_LAUNDER 0
+#endif
 #if defined(__GNUG__) && !defined(__clang__)
 #  include <cxxabi.h>
 #endif
 
+/* https://stackoverflow.com/questions/46798456/handling-gccs-noexcept-type-warning
+   This warning is about ABI compatibility, not code health.
+   It is only actually needed in a couple places, but apparently GCC 7 "generates this warning if
+   and only if the first template instantiation ... involves noexcept" [stackoverflow], therefore
+   it could get triggered from seemingly random places, depending on user code.
+   No other GCC version generates this warning.
+ */
+#if defined(__GNUC__) && __GNUC__ == 7
+#    pragma GCC diagnostic push
+#    pragma GCC diagnostic ignored "-Wnoexcept-type"
+#endif
+
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
+PYBIND11_NAMESPACE_BEGIN(detail)
+
+// Apply all the extensions translators from a list
+// Return true if one of the translators completed without raising an exception
+// itself. Return of false indicates that if there are other translators
+// available, they should be tried.
+inline bool apply_exception_translators(std::forward_list<ExceptionTranslator>& translators) {
+    auto last_exception = std::current_exception();
+
+    for (auto &translator : translators) {
+        try {
+            translator(last_exception);
+            return true;
+        } catch (...) {
+            last_exception = std::current_exception();
+        }
+    }
+    return false;
+}
+
+#if defined(_MSC_VER)
+#    define PYBIND11_COMPAT_STRDUP _strdup
+#else
+#    define PYBIND11_COMPAT_STRDUP strdup
+#endif
+
+PYBIND11_NAMESPACE_END(detail)
+
 /// Wraps an arbitrary C++ function/method/lambda function/.. into a callable Python object
 class cpp_function : public function {
 public:
     cpp_function() = default;
+    // NOLINTNEXTLINE(google-explicit-constructor)
     cpp_function(std::nullptr_t) { }
 
     /// Construct a cpp_function from a vanilla function pointer
     template <typename Return, typename... Args, typename... Extra>
+    // NOLINTNEXTLINE(google-explicit-constructor)
     cpp_function(Return (*f)(Args...), const Extra&... extra) {
         initialize(f, f, extra...);
     }
 
     /// Construct a cpp_function from a lambda function (possibly with internal state)
     template <typename Func, typename... Extra,
               typename = detail::enable_if_t<detail::is_lambda<Func>::value>>
+    // NOLINTNEXTLINE(google-explicit-constructor)
     cpp_function(Func &&f, const Extra&... extra) {
         initialize(std::forward<Func>(f),
                    (detail::function_signature_t<Func> *) nullptr, extra...);
     }
 
     /// Construct a cpp_function from a class method (non-const, no ref-qualifier)
     template <typename Return, typename Class, typename... Arg, typename... Extra>
+    // NOLINTNEXTLINE(google-explicit-constructor)
     cpp_function(Return (Class::*f)(Arg...), const Extra&... extra) {
         initialize([f](Class *c, Arg... args) -> Return { return (c->*f)(std::forward<Arg>(args)...); },
                    (Return (*) (Class *, Arg...)) nullptr, extra...);
     }
 
     /// Construct a cpp_function from a class method (non-const, lvalue ref-qualifier)
     /// A copy of the overload for non-const functions without explicit ref-qualifier
     /// but with an added `&`.
     template <typename Return, typename Class, typename... Arg, typename... Extra>
+    // NOLINTNEXTLINE(google-explicit-constructor)
     cpp_function(Return (Class::*f)(Arg...)&, const Extra&... extra) {
-        initialize([f](Class *c, Arg... args) -> Return { return (c->*f)(args...); },
+        initialize([f](Class *c, Arg... args) -> Return { return (c->*f)(std::forward<Arg>(args)...); },
                    (Return (*) (Class *, Arg...)) nullptr, extra...);
     }
 
     /// Construct a cpp_function from a class method (const, no ref-qualifier)
     template <typename Return, typename Class, typename... Arg, typename... Extra>
+    // NOLINTNEXTLINE(google-explicit-constructor)
     cpp_function(Return (Class::*f)(Arg...) const, const Extra&... extra) {
         initialize([f](const Class *c, Arg... args) -> Return { return (c->*f)(std::forward<Arg>(args)...); },
                    (Return (*)(const Class *, Arg ...)) nullptr, extra...);
     }
 
     /// Construct a cpp_function from a class method (const, lvalue ref-qualifier)
     /// A copy of the overload for const functions without explicit ref-qualifier
     /// but with an added `&`.
     template <typename Return, typename Class, typename... Arg, typename... Extra>
+    // NOLINTNEXTLINE(google-explicit-constructor)
     cpp_function(Return (Class::*f)(Arg...) const&, const Extra&... extra) {
-        initialize([f](const Class *c, Arg... args) -> Return { return (c->*f)(args...); },
+        initialize([f](const Class *c, Arg... args) -> Return { return (c->*f)(std::forward<Arg>(args)...); },
                    (Return (*)(const Class *, Arg ...)) nullptr, extra...);
     }
 
     /// Return the function name
     object name() const { return attr("__name__"); }
 
 protected:
@@ -134,40 +161,53 @@
 
         /* Store the function including any extra state it might have (e.g. a lambda capture object) */
         // The unique_ptr makes sure nothing is leaked in case of an exception.
         auto unique_rec = make_function_record();
         auto rec = unique_rec.get();
 
         /* Store the capture object directly in the function record if there is enough space */
-        if (sizeof(capture) <= sizeof(rec->data)) {
+        if (PYBIND11_SILENCE_MSVC_C4127(sizeof(capture) <= sizeof(rec->data))) {
             /* Without these pragmas, GCC warns that there might not be
                enough space to use the placement new operator. However, the
                'if' statement above ensures that this is the case. */
-#if defined(__GNUG__) && !defined(__clang__) && __GNUC__ >= 6
+#if defined(__GNUG__) && __GNUC__ >= 6 && !defined(__clang__) && !defined(__INTEL_COMPILER)
 #  pragma GCC diagnostic push
 #  pragma GCC diagnostic ignored "-Wplacement-new"
 #endif
             new ((capture *) &rec->data) capture { std::forward<Func>(f) };
-#if defined(__GNUG__) && !defined(__clang__) && __GNUC__ >= 6
+#if defined(__GNUG__) && __GNUC__ >= 6 && !defined(__clang__) && !defined(__INTEL_COMPILER)
+#  pragma GCC diagnostic pop
+#endif
+#if defined(__GNUG__) && !PYBIND11_HAS_STD_LAUNDER && !defined(__INTEL_COMPILER)
+#  pragma GCC diagnostic push
+#  pragma GCC diagnostic ignored "-Wstrict-aliasing"
+#endif
+            // UB without std::launder, but without breaking ABI and/or
+            // a significant refactoring it's "impossible" to solve.
+            if (!std::is_trivially_destructible<capture>::value)
+                rec->free_data = [](function_record *r) {
+                    auto data = PYBIND11_STD_LAUNDER((capture *) &r->data);
+                    (void) data;
+                    data->~capture();
+                };
+#if defined(__GNUG__) && !PYBIND11_HAS_STD_LAUNDER && !defined(__INTEL_COMPILER)
 #  pragma GCC diagnostic pop
 #endif
-            if (!std::is_trivially_destructible<Func>::value)
-                rec->free_data = [](function_record *r) { ((capture *) &r->data)->~capture(); };
         } else {
             rec->data[0] = new capture { std::forward<Func>(f) };
             rec->free_data = [](function_record *r) { delete ((capture *) r->data[0]); };
         }
 
         /* Type casters for the function arguments and return value */
         using cast_in = argument_loader<Args...>;
         using cast_out = make_caster<
             conditional_t<std::is_void<Return>::value, void_type, Return>
         >;
 
-        static_assert(expected_num_args<Extra...>(sizeof...(Args), cast_in::has_args, cast_in::has_kwargs),
+        static_assert(expected_num_args<Extra...>(sizeof...(Args), cast_in::args_pos >= 0, cast_in::has_kwargs),
                       "The number of argument annotations does not match the number of function arguments");
 
         /* Dispatch code which converts function arguments and performs the actual function call */
         rec->impl = [](function_call &call) -> handle {
             cast_in args_converter;
 
             /* Try to cast the function arguments into the C++ domain */
@@ -194,38 +234,45 @@
 
             /* Invoke call policy post-call hook */
             process_attributes<Extra...>::postcall(call, result);
 
             return result;
         };
 
+        rec->nargs_pos = cast_in::args_pos >= 0
+            ? static_cast<std::uint16_t>(cast_in::args_pos)
+            : sizeof...(Args) - cast_in::has_kwargs; // Will get reduced more if we have a kw_only
+        rec->has_args = cast_in::args_pos >= 0;
+        rec->has_kwargs = cast_in::has_kwargs;
+
         /* Process any user-provided function attributes */
         process_attributes<Extra...>::init(extra..., rec);
 
         {
             constexpr bool has_kw_only_args = any_of<std::is_same<kw_only, Extra>...>::value,
                            has_pos_only_args = any_of<std::is_same<pos_only, Extra>...>::value,
-                           has_args = any_of<std::is_same<args, Args>...>::value,
                            has_arg_annotations = any_of<is_keyword<Extra>...>::value;
             static_assert(has_arg_annotations || !has_kw_only_args, "py::kw_only requires the use of argument annotations");
             static_assert(has_arg_annotations || !has_pos_only_args, "py::pos_only requires the use of argument annotations (for docstrings and aligning the annotations to the argument)");
-            static_assert(!(has_args && has_kw_only_args), "py::kw_only cannot be combined with a py::args argument");
+
+            static_assert(constexpr_sum(is_kw_only<Extra>::value...) <= 1, "py::kw_only may be specified only once");
+            static_assert(constexpr_sum(is_pos_only<Extra>::value...) <= 1, "py::pos_only may be specified only once");
+            constexpr auto kw_only_pos = constexpr_first<is_kw_only, Extra...>();
+            constexpr auto pos_only_pos = constexpr_first<is_pos_only, Extra...>();
+            static_assert(!(has_kw_only_args && has_pos_only_args) || pos_only_pos < kw_only_pos, "py::pos_only must come before py::kw_only");
         }
 
         /* Generate a readable signature describing the function's arguments and return value types */
-        static constexpr auto signature = _("(") + cast_in::arg_names + _(") -> ") + cast_out::name;
+        static constexpr auto signature = const_name("(") + cast_in::arg_names + const_name(") -> ") + cast_out::name;
         PYBIND11_DESCR_CONSTEXPR auto types = decltype(signature)::types();
 
         /* Register the function with Python from generic (non-templated) code */
         // Pass on the ownership over the `unique_rec` to `initialize_generic`. `rec` stays valid.
         initialize_generic(std::move(unique_rec), signature.text, types.data(), sizeof...(Args));
 
-        if (cast_in::has_args) rec->has_args = true;
-        if (cast_in::has_kwargs) rec->has_kwargs = true;
-
         /* Stash some additional information used by an important optimization in 'functional.h' */
         using FunctionType = Return (*)(Args...);
         constexpr bool is_function_ptr =
             std::is_convertible<Func, FunctionType>::value &&
             sizeof(capture) == sizeof(void *);
         if (is_function_ptr) {
             rec->is_stateless = true;
@@ -238,15 +285,15 @@
     class strdup_guard {
     public:
         ~strdup_guard() {
             for (auto s : strings)
                 std::free(s);
         }
         char *operator()(const char *s) {
-            auto t = strdup(s);
+            auto t = PYBIND11_COMPAT_STRDUP(s);
             strings.push_back(t);
             return t;
         }
         void release() {
             strings.clear();
         }
     private:
@@ -276,15 +323,16 @@
                 a.name = guarded_strdup(a.name);
             if (a.descr)
                 a.descr = guarded_strdup(a.descr);
             else if (a.value)
                 a.descr = guarded_strdup(repr(a.value).cast<std::string>().c_str());
         }
 
-        rec->is_constructor = !strcmp(rec->name, "__init__") || !strcmp(rec->name, "__setstate__");
+        rec->is_constructor
+            = (strcmp(rec->name, "__init__") == 0) || (strcmp(rec->name, "__setstate__") == 0);
 
 #if !defined(NDEBUG) && !defined(PYBIND11_DISABLE_NEW_STYLE_INIT_WARNING)
         if (rec->is_constructor && !rec->is_new_style_constructor) {
             const auto class_name = detail::get_fully_qualified_tp_name((PyTypeObject *) rec->scope.ptr());
             const auto func_name = std::string(rec->name);
             PyErr_WarnEx(
                 PyExc_FutureWarning,
@@ -295,44 +343,47 @@
             );
         }
 #endif
 
         /* Generate a proper function signature */
         std::string signature;
         size_t type_index = 0, arg_index = 0;
+        bool is_starred = false;
         for (auto *pc = text; *pc != '\0'; ++pc) {
             const auto c = *pc;
 
             if (c == '{') {
                 // Write arg name for everything except *args and **kwargs.
-                if (*(pc + 1) == '*')
+                is_starred = *(pc + 1) == '*';
+                if (is_starred)
                     continue;
                 // Separator for keyword-only arguments, placed before the kw
-                // arguments start
-                if (rec->nargs_kw_only > 0 && arg_index + rec->nargs_kw_only == args)
+                // arguments start (unless we are already putting an *args)
+                if (!rec->has_args && arg_index == rec->nargs_pos)
                     signature += "*, ";
                 if (arg_index < rec->args.size() && rec->args[arg_index].name) {
                     signature += rec->args[arg_index].name;
                 } else if (arg_index == 0 && rec->is_method) {
                     signature += "self";
                 } else {
                     signature += "arg" + std::to_string(arg_index - (rec->is_method ? 1 : 0));
                 }
                 signature += ": ";
             } else if (c == '}') {
                 // Write default value if available.
-                if (arg_index < rec->args.size() && rec->args[arg_index].descr) {
+                if (!is_starred && arg_index < rec->args.size() && rec->args[arg_index].descr) {
                     signature += " = ";
                     signature += rec->args[arg_index].descr;
                 }
                 // Separator for positional-only arguments (placed after the
                 // argument, rather than before like *
                 if (rec->nargs_pos_only > 0 && (arg_index + 1) == rec->nargs_pos_only)
                     signature += ", /";
-                arg_index++;
+                if (!is_starred)
+                    arg_index++;
             } else if (c == '%') {
                 const std::type_info *t = types[type_index++];
                 if (!t)
                     pybind11_fail("Internal error while parsing type signature (1)");
                 if (auto tinfo = detail::get_type_info(*t)) {
                     handle th((PyObject *) tinfo->type);
                     signature +=
@@ -350,15 +401,15 @@
                     signature += tname;
                 }
             } else {
                 signature += c;
             }
         }
 
-        if (arg_index != args || types[type_index] != nullptr)
+        if (arg_index != args - rec->has_args - rec->has_kwargs || types[type_index] != nullptr)
             pybind11_fail("Internal error while parsing type signature (2)");
 
 #if PY_MAJOR_VERSION < 3
         if (strcmp(rec->name, "__next__") == 0) {
             std::free(rec->name);
             rec->name = guarded_strdup("next");
         } else if (strcmp(rec->name, "__bool__") == 0) {
@@ -372,15 +423,16 @@
 
         if (rec->sibling && PYBIND11_INSTANCE_METHOD_CHECK(rec->sibling.ptr()))
             rec->sibling = PYBIND11_INSTANCE_METHOD_GET_FUNCTION(rec->sibling.ptr());
 
         detail::function_record *chain = nullptr, *chain_start = rec;
         if (rec->sibling) {
             if (PyCFunction_Check(rec->sibling.ptr())) {
-                auto rec_capsule = reinterpret_borrow<capsule>(PyCFunction_GET_SELF(rec->sibling.ptr()));
+                auto *self = PyCFunction_GET_SELF(rec->sibling.ptr());
+                capsule rec_capsule = isinstance<capsule>(self) ? reinterpret_borrow<capsule>(self) : capsule(self);
                 chain = (detail::function_record *) rec_capsule;
                 /* Never append a method to an overload chain of a parent class;
                    instead, hide the parent's overloads in this case */
                 if (!chain->scope.is(rec->scope))
                     chain = nullptr;
             }
             // Don't trigger for things like the default __init__, which are wrapper_descriptors that we are intentionally replacing
@@ -390,15 +442,16 @@
         }
 
         if (!chain) {
             /* No existing overload was found, create a new function object */
             rec->def = new PyMethodDef();
             std::memset(rec->def, 0, sizeof(PyMethodDef));
             rec->def->ml_name = rec->name;
-            rec->def->ml_meth = reinterpret_cast<PyCFunction>(reinterpret_cast<void (*) (void)>(*dispatcher));
+            rec->def->ml_meth
+                = reinterpret_cast<PyCFunction>(reinterpret_cast<void (*)()>(dispatcher));
             rec->def->ml_flags = METH_VARARGS | METH_KEYWORDS;
 
             capsule rec_capsule(unique_rec.release(), [](void *ptr) {
                 destruct((detail::function_record *) ptr);
             });
             guarded_strdup.release();
 
@@ -464,15 +517,15 @@
                 if (index > 0) signatures += "\n";
                 if (chain)
                     signatures += std::to_string(++index) + ". ";
                 signatures += rec->name;
                 signatures += it->signature;
                 signatures += "\n";
             }
-            if (it->doc && strlen(it->doc) > 0 && options::show_user_defined_docstrings()) {
+            if (it->doc && it->doc[0] != '\0' && options::show_user_defined_docstrings()) {
                 // If we're appending another docstring, and aren't printing function signatures, we
                 // need to append a newline first:
                 if (!options::show_function_signatures()) {
                     if (first_user_def) first_user_def = false;
                     else signatures += "\n";
                 }
                 if (options::show_function_signatures()) signatures += "\n";
@@ -481,15 +534,16 @@
             }
         }
 
         /* Install docstring */
         auto *func = (PyCFunctionObject *) m_ptr;
         std::free(const_cast<char *>(func->m_ml->ml_doc));
         // Install docstring if it's non-empty (when at least one option is enabled)
-        func->m_ml->ml_doc = signatures.empty() ? nullptr : strdup(signatures.c_str());
+        func->m_ml->ml_doc
+            = signatures.empty() ? nullptr : PYBIND11_COMPAT_STRDUP(signatures.c_str());
 
         if (rec->is_method) {
             m_ptr = PYBIND11_INSTANCE_METHOD_NEW(m_ptr, rec->scope.ptr());
             if (!m_ptr)
                 pybind11_fail("cpp_function::cpp_function(): Could not allocate instance method object");
             Py_DECREF(func);
         }
@@ -534,14 +588,15 @@
                 #endif
             }
             delete rec;
             rec = next;
         }
     }
 
+
     /// Main dispatch logic for calls to functions bound using pybind11
     static PyObject *dispatcher(PyObject *self, PyObject *args_in, PyObject *kwargs_in) {
         using namespace detail;
 
         /* Iterator over the list of potentially admissible overloads */
         const function_record *overloads = (function_record *) PyCapsule_GetPointer(self, nullptr),
                               *it = overloads;
@@ -550,16 +605,16 @@
         const auto n_args_in = (size_t) PyTuple_GET_SIZE(args_in);
 
         handle parent = n_args_in > 0 ? PyTuple_GET_ITEM(args_in, 0) : nullptr,
                result = PYBIND11_TRY_NEXT_OVERLOAD;
 
         auto self_value_and_holder = value_and_holder();
         if (overloads->is_constructor) {
-            if (!PyObject_TypeCheck(parent.ptr(), (PyTypeObject *) overloads->scope.ptr())) {
-                PyErr_SetString(PyExc_TypeError, "__init__(self, ...) called with invalid `self` argument");
+            if (!parent || !PyObject_TypeCheck(parent.ptr(), (PyTypeObject *) overloads->scope.ptr())) {
+                PyErr_SetString(PyExc_TypeError, "__init__(self, ...) called with invalid or missing `self` argument");
                 return nullptr;
             }
 
             const auto tinfo = get_type_info((PyTypeObject *) overloads->scope.ptr());
             const auto pi = reinterpret_cast<instance *>(parent.ptr());
             self_value_and_holder = pi->get_value_and_holder(tinfo, true);
 
@@ -582,15 +637,15 @@
             for (; it != nullptr; it = it->next) {
 
                 /* For each overload:
                    1. Copy all positional arguments we were given, also checking to make sure that
                       named positional arguments weren't *also* specified via kwarg.
                    2. If we weren't given enough, try to make up the omitted ones by checking
                       whether they were provided by a kwarg matching the `py::arg("name")` name.  If
-                      so, use it (and remove it from kwargs; if not, see if the function binding
+                      so, use it (and remove it from kwargs); if not, see if the function binding
                       provided a default that we can use.
                    3. Ensure that either all keyword arguments were "consumed", or that the function
                       takes a kwargs argument to accept unconsumed kwargs.
                    4. Any positional arguments still left get put into a tuple (for args), and any
                       leftover kwargs get put into a dict.
                    5. Pack everything into a vector; if we have py::args or py::kwargs, they are an
                       extra tuple or dict at the end of the positional arguments.
@@ -600,15 +655,15 @@
                    result other than PYBIND11_TRY_NEXT_OVERLOAD.
                  */
 
                 const function_record &func = *it;
                 size_t num_args = func.nargs;    // Number of positional arguments that we need
                 if (func.has_args) --num_args;   // (but don't count py::args
                 if (func.has_kwargs) --num_args; //  or py::kwargs)
-                size_t pos_args = num_args - func.nargs_kw_only;
+                size_t pos_args = func.nargs_pos;
 
                 if (!func.has_args && n_args_in > pos_args)
                     continue; // Too many positional arguments for this overload
 
                 if (n_args_in < pos_args && func.args.size() < pos_args)
                     continue; // Not enough positional arguments given, and not enough defaults to fill in the blanks
 
@@ -630,15 +685,15 @@
                     ++args_copied;
                 }
 
                 // 1. Copy any position arguments given.
                 bool bad_arg = false;
                 for (; args_copied < args_to_copy; ++args_copied) {
                     const argument_record *arg_rec = args_copied < func.args.size() ? &func.args[args_copied] : nullptr;
-                    if (kwargs_in && arg_rec && arg_rec->name && PyDict_GetItemString(kwargs_in, arg_rec->name)) {
+                    if (kwargs_in && arg_rec && arg_rec->name && dict_getitemstring(kwargs_in, arg_rec->name)) {
                         bad_arg = true;
                         break;
                     }
 
                     handle arg(PyTuple_GET_ITEM(args_in, args_copied));
                     if (arg_rec && !arg_rec->none && arg.is_none()) {
                         bad_arg = true;
@@ -646,14 +701,18 @@
                     }
                     call.args.push_back(arg);
                     call.args_convert.push_back(arg_rec ? arg_rec->convert : true);
                 }
                 if (bad_arg)
                     continue; // Maybe it was meant for another overload (issue #688)
 
+                // Keep track of how many position args we copied out in case we need to come back
+                // to copy the rest into a py::args argument.
+                size_t positional_args_copied = args_copied;
+
                 // We'll need to copy this if we steal some kwargs for defaults
                 dict kwargs = reinterpret_borrow<dict>(kwargs_in);
 
                 // 1.5. Fill in any missing pos_only args from defaults if they exist
                 if (args_copied < func.nargs_pos_only) {
                     for (; args_copied < func.nargs_pos_only; ++args_copied) {
                         const auto &arg_rec = func.args[args_copied];
@@ -678,32 +737,38 @@
                     bool copied_kwargs = false;
 
                     for (; args_copied < num_args; ++args_copied) {
                         const auto &arg_rec = func.args[args_copied];
 
                         handle value;
                         if (kwargs_in && arg_rec.name)
-                            value = PyDict_GetItemString(kwargs.ptr(), arg_rec.name);
+                            value = dict_getitemstring(kwargs.ptr(), arg_rec.name);
 
                         if (value) {
                             // Consume a kwargs value
                             if (!copied_kwargs) {
                                 kwargs = reinterpret_steal<dict>(PyDict_Copy(kwargs.ptr()));
                                 copied_kwargs = true;
                             }
-                            PyDict_DelItemString(kwargs.ptr(), arg_rec.name);
+                            if (PyDict_DelItemString(kwargs.ptr(), arg_rec.name) == -1) {
+                                throw error_already_set();
+                            }
                         } else if (arg_rec.value) {
                             value = arg_rec.value;
                         }
 
                         if (!arg_rec.none && value.is_none()) {
                             break;
                         }
 
                         if (value) {
+                            // If we're at the py::args index then first insert a stub for it to be replaced later
+                            if (func.has_args && call.args.size() == func.nargs_pos)
+                                call.args.push_back(none());
+
                             call.args.push_back(value);
                             call.args_convert.push_back(arg_rec.convert);
                         }
                         else
                             break;
                     }
 
@@ -718,24 +783,27 @@
                 // 4a. If we have a py::args argument, create a new tuple with leftovers
                 if (func.has_args) {
                     tuple extra_args;
                     if (args_to_copy == 0) {
                         // We didn't copy out any position arguments from the args_in tuple, so we
                         // can reuse it directly without copying:
                         extra_args = reinterpret_borrow<tuple>(args_in);
-                    } else if (args_copied >= n_args_in) {
+                    } else if (positional_args_copied >= n_args_in) {
                         extra_args = tuple(0);
                     } else {
-                        size_t args_size = n_args_in - args_copied;
+                        size_t args_size = n_args_in - positional_args_copied;
                         extra_args = tuple(args_size);
                         for (size_t i = 0; i < args_size; ++i) {
-                            extra_args[i] = PyTuple_GET_ITEM(args_in, args_copied + i);
+                            extra_args[i] = PyTuple_GET_ITEM(args_in, positional_args_copied + i);
                         }
                     }
-                    call.args.push_back(extra_args);
+                    if (call.args.size() <= func.nargs_pos)
+                        call.args.push_back(extra_args);
+                    else
+                        call.args[func.nargs_pos] = extra_args;
                     call.args_convert.push_back(false);
                     call.args_ref = std::move(extra_args);
                 }
 
                 // 4b. If we have a py::kwargs, pass on any remaining kwargs
                 if (func.has_kwargs) {
                     if (!kwargs.ptr())
@@ -812,35 +880,37 @@
             return nullptr;
 #ifdef __GLIBCXX__
         } catch ( abi::__forced_unwind& ) {
             throw;
 #endif
         } catch (...) {
             /* When an exception is caught, give each registered exception
-               translator a chance to translate it to a Python exception
-               in reverse order of registration.
+               translator a chance to translate it to a Python exception. First
+               all module-local translators will be tried in reverse order of
+               registration. If none of the module-locale translators handle
+               the exception (or there are no module-locale translators) then
+               the global translators will be tried, also in reverse order of
+               registration.
 
                A translator may choose to do one of the following:
 
                 - catch the exception and call PyErr_SetString or PyErr_SetObject
                   to set a standard (or custom) Python exception, or
                 - do nothing and let the exception fall through to the next translator, or
                 - delegate translation to the next translator by throwing a new type of exception. */
 
-            auto last_exception = std::current_exception();
-            auto &registered_exception_translators = get_internals().registered_exception_translators;
-            for (auto& translator : registered_exception_translators) {
-                try {
-                    translator(last_exception);
-                } catch (...) {
-                    last_exception = std::current_exception();
-                    continue;
-                }
+            auto &local_exception_translators = get_local_internals().registered_exception_translators;
+            if (detail::apply_exception_translators(local_exception_translators)) {
                 return nullptr;
             }
+            auto &exception_translators = get_internals().registered_exception_translators;
+            if (detail::apply_exception_translators(exception_translators)) {
+                return nullptr;
+            }
+
             PyErr_SetString(PyExc_SystemError, "Exception escaped from default exception translator!");
             return nullptr;
         }
 
         auto append_note_if_missing_header_is_suspected = [](std::string &msg) {
             if (msg.find("std::") != std::string::npos) {
                 msg += "\n\n"
@@ -916,31 +986,32 @@
                     }
                 }
             }
 
             append_note_if_missing_header_is_suspected(msg);
             PyErr_SetString(PyExc_TypeError, msg.c_str());
             return nullptr;
-        } else if (!result) {
+        }
+        if (!result) {
             std::string msg = "Unable to convert function return value to a "
                               "Python type! The signature was\n\t";
             msg += it->signature;
             append_note_if_missing_header_is_suspected(msg);
             PyErr_SetString(PyExc_TypeError, msg.c_str());
             return nullptr;
-        } else {
-            if (overloads->is_constructor && !self_value_and_holder.holder_constructed()) {
-                auto *pi = reinterpret_cast<instance *>(parent.ptr());
-                self_value_and_holder.type->init_instance(pi, nullptr);
-            }
-            return result.ptr();
         }
+        if (overloads->is_constructor && !self_value_and_holder.holder_constructed()) {
+            auto *pi = reinterpret_cast<instance *>(parent.ptr());
+            self_value_and_holder.type->init_instance(pi, nullptr);
+        }
+        return result.ptr();
     }
 };
 
+
 /// Wrapper for Python extension modules
 class module_ : public object {
 public:
     PYBIND11_OBJECT_DEFAULT(module_, object, PyModule_Check)
 
     /// Create a new top-level Python module with the given name and docstring
     PYBIND11_DEPRECATED("Use PYBIND11_MODULE or module_::create_extension_module instead")
@@ -1070,26 +1141,36 @@
 /// Return a dictionary representing the global variables in the current execution frame,
 /// or ``__main__.__dict__`` if there is no frame (usually when the interpreter is embedded).
 inline dict globals() {
     PyObject *p = PyEval_GetGlobals();
     return reinterpret_borrow<dict>(p ? p : module_::import("__main__").attr("__dict__").ptr());
 }
 
+#if PY_VERSION_HEX >= 0x03030000
+template <typename... Args,
+          typename = detail::enable_if_t<args_are_all_keyword_or_ds<Args...>()>>
+PYBIND11_DEPRECATED("make_simple_namespace should be replaced with py::module_::import(\"types\").attr(\"SimpleNamespace\") ")
+object make_simple_namespace(Args&&... args_) {
+    return module_::import("types").attr("SimpleNamespace")(std::forward<Args>(args_)...);
+}
+#endif
+
 PYBIND11_NAMESPACE_BEGIN(detail)
 /// Generic support for creating new Python heap types
 class generic_type : public object {
 public:
     PYBIND11_OBJECT_DEFAULT(generic_type, object, PyType_Check)
 protected:
     void initialize(const type_record &rec) {
         if (rec.scope && hasattr(rec.scope, "__dict__") && rec.scope.attr("__dict__").contains(rec.name))
             pybind11_fail("generic_type: cannot initialize type \"" + std::string(rec.name) +
                           "\": an object with that name is already defined");
 
-        if (rec.module_local ? get_local_type_info(*rec.type) : get_global_type_info(*rec.type))
+        if ((rec.module_local ? get_local_type_info(*rec.type) : get_global_type_info(*rec.type))
+            != nullptr)
             pybind11_fail("generic_type: type \"" + std::string(rec.name) +
                           "\" is already registered!");
 
         m_ptr = make_new_python_type(rec);
 
         /* Register supplemental type information in C++ dict */
         auto *tinfo = new detail::type_info();
@@ -1106,15 +1187,15 @@
         tinfo->default_holder = rec.default_holder;
         tinfo->module_local = rec.module_local;
 
         auto &internals = get_internals();
         auto tindex = std::type_index(*rec.type);
         tinfo->direct_conversions = &internals.direct_conversions[tindex];
         if (rec.module_local)
-            registered_local_types_cpp()[tindex] = tinfo;
+            get_local_internals().registered_types_cpp[tindex] = tinfo;
         else
             internals.registered_types_cpp[tindex] = tinfo;
         internals.registered_types_py[(PyTypeObject *) m_ptr] = { tinfo };
 
         if (rec.bases.size() > 1 || rec.multiple_inheritance) {
             mark_parents_nonsimple(tinfo->type);
             tinfo->simple_ancestors = false;
@@ -1159,16 +1240,17 @@
         tinfo->get_buffer_data = get_buffer_data;
     }
 
     // rec_func must be set for either fget or fset.
     void def_property_static_impl(const char *name,
                                   handle fget, handle fset,
                                   detail::function_record *rec_func) {
-        const auto is_static = rec_func && !(rec_func->is_method && rec_func->scope);
-        const auto has_doc = rec_func && rec_func->doc && pybind11::options::show_user_defined_docstrings();
+        const auto is_static = (rec_func != nullptr) && !(rec_func->is_method && rec_func->scope);
+        const auto has_doc = (rec_func != nullptr) && (rec_func->doc != nullptr)
+                             && pybind11::options::show_user_defined_docstrings();
         auto property = handle((PyObject *) (is_static ? get_internals().static_property_type
                                                        : &PyProperty_Type));
         attr(name) = property(fget.ptr() ? fget : none(),
                               fset.ptr() ? fset : none(),
                               /*deleter*/none(),
                               pybind11::str(has_doc ? rec_func->doc : ""));
     }
@@ -1292,15 +1374,15 @@
 
         /* Process optional arguments, if any */
         process_attributes<Extra...>::init(extra..., &record);
 
         generic_type::initialize(record);
 
         if (has_alias) {
-            auto &instances = record.module_local ? registered_local_types_cpp() : get_internals().registered_types_cpp;
+            auto &instances = record.module_local ? get_local_internals().registered_types_cpp : get_internals().registered_types_cpp;
             instances[std::type_index(typeid(type_alias))] = instances[std::type_index(typeid(type))];
         }
     }
 
     template <typename Base, detail::enable_if_t<is_base<Base>::value, int> = 0>
     static void add_base(detail::type_record &rec) {
         rec.add_base(typeid(Base), [](void *src) -> void * {
@@ -1339,20 +1421,22 @@
     class_ & def_cast(const detail::op_<id, ot, L, R> &op, const Extra&... extra) {
         op.execute_cast(*this, extra...);
         return *this;
     }
 
     template <typename... Args, typename... Extra>
     class_ &def(const detail::initimpl::constructor<Args...> &init, const Extra&... extra) {
+        PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(init);
         init.execute(*this, extra...);
         return *this;
     }
 
     template <typename... Args, typename... Extra>
     class_ &def(const detail::initimpl::alias_constructor<Args...> &init, const Extra&... extra) {
+        PYBIND11_WORKAROUND_INCORRECT_MSVC_C4100(init);
         init.execute(*this, extra...);
         return *this;
     }
 
     template <typename... Args, typename... Extra>
     class_ &def(detail::initimpl::factory<Args...> &&init, const Extra&... extra) {
         std::move(init).execute(*this, extra...);
@@ -1407,23 +1491,23 @@
         cpp_function fget([pm](const type &c) -> const D &{ return c.*pm; }, is_method(*this));
         def_property_readonly(name, fget, return_value_policy::reference_internal, extra...);
         return *this;
     }
 
     template <typename D, typename... Extra>
     class_ &def_readwrite_static(const char *name, D *pm, const Extra& ...extra) {
-        cpp_function fget([pm](object) -> const D &{ return *pm; }, scope(*this)),
-                     fset([pm](object, const D &value) { *pm = value; }, scope(*this));
+        cpp_function fget([pm](const object &) -> const D & { return *pm; }, scope(*this)),
+            fset([pm](const object &, const D &value) { *pm = value; }, scope(*this));
         def_property_static(name, fget, fset, return_value_policy::reference, extra...);
         return *this;
     }
 
     template <typename D, typename... Extra>
     class_ &def_readonly_static(const char *name, const D *pm, const Extra& ...extra) {
-        cpp_function fget([pm](object) -> const D &{ return *pm; }, scope(*this));
+        cpp_function fget([pm](const object &) -> const D & { return *pm; }, scope(*this));
         def_property_readonly_static(name, fget, return_value_policy::reference, extra...);
         return *this;
     }
 
     /// Uses return_value_policy::reference_internal by default
     template <typename Getter, typename... Extra>
     class_ &def_property_readonly(const char *name, const Getter &fget, const Extra& ...extra) {
@@ -1479,44 +1563,43 @@
                       "Argument annotations are not allowed for properties");
         auto rec_fget = get_function_record(fget), rec_fset = get_function_record(fset);
         auto *rec_active = rec_fget;
         if (rec_fget) {
            char *doc_prev = rec_fget->doc; /* 'extra' field may include a property-specific documentation string */
            detail::process_attributes<Extra...>::init(extra..., rec_fget);
            if (rec_fget->doc && rec_fget->doc != doc_prev) {
-              free(doc_prev);
-              rec_fget->doc = strdup(rec_fget->doc);
+              std::free(doc_prev);
+              rec_fget->doc = PYBIND11_COMPAT_STRDUP(rec_fget->doc);
            }
         }
         if (rec_fset) {
             char *doc_prev = rec_fset->doc;
             detail::process_attributes<Extra...>::init(extra..., rec_fset);
             if (rec_fset->doc && rec_fset->doc != doc_prev) {
-                free(doc_prev);
-                rec_fset->doc = strdup(rec_fset->doc);
+                std::free(doc_prev);
+                rec_fset->doc = PYBIND11_COMPAT_STRDUP(rec_fset->doc);
             }
             if (! rec_active) rec_active = rec_fset;
         }
         def_property_static_impl(name, fget, fset, rec_active);
         return *this;
     }
 
 private:
     /// Initialize holder object, variant 1: object derives from enable_shared_from_this
     template <typename T>
     static void init_holder(detail::instance *inst, detail::value_and_holder &v_h,
             const holder_type * /* unused */, const std::enable_shared_from_this<T> * /* dummy */) {
-        try {
-            auto sh = std::dynamic_pointer_cast<typename holder_type::element_type>(
-                    v_h.value_ptr<type>()->shared_from_this());
-            if (sh) {
-                new (std::addressof(v_h.holder<holder_type>())) holder_type(std::move(sh));
-                v_h.set_holder_constructed();
-            }
-        } catch (const std::bad_weak_ptr &) {}
+
+        auto sh = std::dynamic_pointer_cast<typename holder_type::element_type>(
+                detail::try_get_shared_from_this(v_h.value_ptr<type>()));
+        if (sh) {
+            new (std::addressof(v_h.holder<holder_type>())) holder_type(std::move(sh));
+            v_h.set_holder_constructed();
+        }
 
         if (!v_h.holder_constructed() && inst->owned) {
             new (std::addressof(v_h.holder<holder_type>())) holder_type(v_h.value_ptr<type>());
             v_h.set_holder_constructed();
         }
     }
 
@@ -1616,28 +1699,29 @@
         if (handle(kv.second[int_(0)]).equal(arg))
             return pybind11::str(kv.first);
     }
     return "???";
 }
 
 struct enum_base {
-    enum_base(handle base, handle parent) : m_base(base), m_parent(parent) { }
+    enum_base(const handle &base, const handle &parent) : m_base(base), m_parent(parent) { }
 
     PYBIND11_NOINLINE void init(bool is_arithmetic, bool is_convertible) {
         m_base.attr("__entries") = dict();
         auto property = handle((PyObject *) &PyProperty_Type);
         auto static_property = handle((PyObject *) get_internals().static_property_type);
 
         m_base.attr("__repr__") = cpp_function(
-            [](object arg) -> str {
+            [](const object &arg) -> str {
                 handle type = type::handle_of(arg);
                 object type_name = type.attr("__name__");
                 return pybind11::str("<{}.{}: {}>").format(type_name, enum_name(arg), int_(arg));
-            }, name("__repr__"), is_method(m_base)
-        );
+            },
+            name("__repr__"),
+            is_method(m_base));
 
         m_base.attr("name") = property(cpp_function(&enum_name, name("name"), is_method(m_base)));
 
         m_base.attr("__str__") = cpp_function(
             [](handle arg) -> str {
                 object type_name = type::handle_of(arg).attr("__name__");
                 return pybind11::str("{}.{}").format(type_name, enum_name(arg));
@@ -1667,38 +1751,44 @@
                 dict entries = arg.attr("__entries"), m;
                 for (auto kv : entries)
                     m[kv.first] = kv.second[int_(0)];
                 return m;
             }, name("__members__")), none(), none(), ""
         );
 
-        #define PYBIND11_ENUM_OP_STRICT(op, expr, strict_behavior)                     \
-            m_base.attr(op) = cpp_function(                                            \
-                [](object a, object b) {                                               \
-                    if (!type::handle_of(a).is(type::handle_of(b)))                    \
-                        strict_behavior;                                               \
-                    return expr;                                                       \
-                },                                                                     \
-                name(op), is_method(m_base), arg("other"))
-
-        #define PYBIND11_ENUM_OP_CONV(op, expr)                                        \
-            m_base.attr(op) = cpp_function(                                            \
-                [](object a_, object b_) {                                             \
-                    int_ a(a_), b(b_);                                                 \
-                    return expr;                                                       \
-                },                                                                     \
-                name(op), is_method(m_base), arg("other"))
-
-        #define PYBIND11_ENUM_OP_CONV_LHS(op, expr)                                    \
-            m_base.attr(op) = cpp_function(                                            \
-                [](object a_, object b) {                                              \
-                    int_ a(a_);                                                        \
-                    return expr;                                                       \
-                },                                                                     \
-                name(op), is_method(m_base), arg("other"))
+#define PYBIND11_ENUM_OP_STRICT(op, expr, strict_behavior)                                        \
+    m_base.attr(op) = cpp_function(                                                               \
+        [](const object &a, const object &b) {                                                    \
+            if (!type::handle_of(a).is(type::handle_of(b)))                                       \
+                strict_behavior; /* NOLINT(bugprone-macro-parentheses) */                         \
+            return expr;                                                                          \
+        },                                                                                        \
+        name(op),                                                                                 \
+        is_method(m_base),                                                                        \
+        arg("other"))
+
+#define PYBIND11_ENUM_OP_CONV(op, expr)                                                           \
+    m_base.attr(op) = cpp_function(                                                               \
+        [](const object &a_, const object &b_) {                                                  \
+            int_ a(a_), b(b_);                                                                    \
+            return expr;                                                                          \
+        },                                                                                        \
+        name(op),                                                                                 \
+        is_method(m_base),                                                                        \
+        arg("other"))
+
+#define PYBIND11_ENUM_OP_CONV_LHS(op, expr)                                                       \
+    m_base.attr(op) = cpp_function(                                                               \
+        [](const object &a_, const object &b) {                                                   \
+            int_ a(a_);                                                                           \
+            return expr;                                                                          \
+        },                                                                                        \
+        name(op),                                                                                 \
+        is_method(m_base),                                                                        \
+        arg("other"))
 
         if (is_convertible) {
             PYBIND11_ENUM_OP_CONV_LHS("__eq__", !b.is_none() &&  a.equal(b));
             PYBIND11_ENUM_OP_CONV_LHS("__ne__",  b.is_none() || !a.equal(b));
 
             if (is_arithmetic) {
                 PYBIND11_ENUM_OP_CONV("__lt__",   a <  b);
@@ -1707,16 +1797,18 @@
                 PYBIND11_ENUM_OP_CONV("__ge__",   a >= b);
                 PYBIND11_ENUM_OP_CONV("__and__",  a &  b);
                 PYBIND11_ENUM_OP_CONV("__rand__", a &  b);
                 PYBIND11_ENUM_OP_CONV("__or__",   a |  b);
                 PYBIND11_ENUM_OP_CONV("__ror__",  a |  b);
                 PYBIND11_ENUM_OP_CONV("__xor__",  a ^  b);
                 PYBIND11_ENUM_OP_CONV("__rxor__", a ^  b);
-                m_base.attr("__invert__") = cpp_function(
-                    [](object arg) { return ~(int_(arg)); }, name("__invert__"), is_method(m_base));
+                m_base.attr("__invert__")
+                    = cpp_function([](const object &arg) { return ~(int_(arg)); },
+                                   name("__invert__"),
+                                   is_method(m_base));
             }
         } else {
             PYBIND11_ENUM_OP_STRICT("__eq__",  int_(a).equal(int_(b)), return false);
             PYBIND11_ENUM_OP_STRICT("__ne__", !int_(a).equal(int_(b)), return true);
 
             if (is_arithmetic) {
                 #define PYBIND11_THROW throw type_error("Expected an enumeration of matching type!");
@@ -1729,18 +1821,18 @@
         }
 
         #undef PYBIND11_ENUM_OP_CONV_LHS
         #undef PYBIND11_ENUM_OP_CONV
         #undef PYBIND11_ENUM_OP_STRICT
 
         m_base.attr("__getstate__") = cpp_function(
-            [](object arg) { return int_(arg); }, name("__getstate__"), is_method(m_base));
+            [](const object &arg) { return int_(arg); }, name("__getstate__"), is_method(m_base));
 
         m_base.attr("__hash__") = cpp_function(
-            [](object arg) { return int_(arg); }, name("__hash__"), is_method(m_base));
+            [](const object &arg) { return int_(arg); }, name("__hash__"), is_method(m_base));
     }
 
     PYBIND11_NOINLINE void value(char const* name_, object value, const char *doc = nullptr) {
         dict entries = m_base.attr("__entries");
         str name(name_);
         if (entries.contains(name)) {
             std::string type_name = (std::string) str(m_base.attr("__name__"));
@@ -1757,31 +1849,48 @@
             m_parent.attr(kv.first) = kv.second[int_(0)];
     }
 
     handle m_base;
     handle m_parent;
 };
 
+template <bool is_signed, size_t length> struct equivalent_integer {};
+template <> struct equivalent_integer<true,  1> { using type = int8_t;   };
+template <> struct equivalent_integer<false, 1> { using type = uint8_t;  };
+template <> struct equivalent_integer<true,  2> { using type = int16_t;  };
+template <> struct equivalent_integer<false, 2> { using type = uint16_t; };
+template <> struct equivalent_integer<true,  4> { using type = int32_t;  };
+template <> struct equivalent_integer<false, 4> { using type = uint32_t; };
+template <> struct equivalent_integer<true,  8> { using type = int64_t;  };
+template <> struct equivalent_integer<false, 8> { using type = uint64_t; };
+
+template <typename IntLike>
+using equivalent_integer_t = typename equivalent_integer<std::is_signed<IntLike>::value, sizeof(IntLike)>::type;
+
 PYBIND11_NAMESPACE_END(detail)
 
 /// Binds C++ enumerations and enumeration classes to Python
 template <typename Type> class enum_ : public class_<Type> {
 public:
     using Base = class_<Type>;
     using Base::def;
     using Base::attr;
     using Base::def_property_readonly;
     using Base::def_property_readonly_static;
-    using Scalar = typename std::underlying_type<Type>::type;
+    using Underlying = typename std::underlying_type<Type>::type;
+    // Scalar is the integer representation of underlying type
+    using Scalar = detail::conditional_t<detail::any_of<
+        detail::is_std_char_type<Underlying>, std::is_same<Underlying, bool>
+    >::value, detail::equivalent_integer_t<Underlying>, Underlying>;
 
     template <typename... Extra>
     enum_(const handle &scope, const char *name, const Extra&... extra)
       : class_<Type>(scope, name, extra...), m_base(*this, scope) {
         constexpr bool is_arithmetic = detail::any_of<std::is_same<arithmetic, Extra>...>::value;
-        constexpr bool is_convertible = std::is_convertible<Type, Scalar>::value;
+        constexpr bool is_convertible = std::is_convertible<Type, Underlying>::value;
         m_base.init(is_arithmetic, is_convertible);
 
         def(init([](Scalar i) { return static_cast<Type>(i); }), arg("value"));
         def_property_readonly("value", [](Type value) { return (Scalar) value; });
         def("__int__", [](Type value) { return (Scalar) value; });
         #if PY_MAJOR_VERSION < 3
             def("__long__", [](Type value) { return (Scalar) value; });
@@ -1813,15 +1922,15 @@
 private:
     detail::enum_base m_base;
 };
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 
-inline void keep_alive_impl(handle nurse, handle patient) {
+PYBIND11_NOINLINE void keep_alive_impl(handle nurse, handle patient) {
     if (!nurse || !patient)
         pybind11_fail("Could not activate keep_alive!");
 
     if (patient.is_none() || nurse.is_none())
         return; /* Nothing to keep alive or nothing to be kept alive by */
 
     auto tinfo = all_type_info(Py_TYPE(nurse.ptr()));
@@ -1840,21 +1949,21 @@
         weakref wr(nurse, disable_lifesupport);
 
         patient.inc_ref(); /* reference patient and leak the weak reference */
         (void) wr.release();
     }
 }
 
-PYBIND11_NOINLINE inline void keep_alive_impl(size_t Nurse, size_t Patient, function_call &call, handle ret) {
+PYBIND11_NOINLINE void keep_alive_impl(size_t Nurse, size_t Patient, function_call &call, handle ret) {
     auto get_arg = [&](size_t n) {
         if (n == 0)
             return ret;
-        else if (n == 1 && call.init_self)
+        if (n == 1 && call.init_self)
             return call.init_self;
-        else if (n <= call.args.size())
+        if (n <= call.args.size())
             return call.args[n - 1];
         return handle();
     };
 
     keep_alive_impl(get_arg(Nurse), get_arg(Patient));
 }
 
@@ -1866,85 +1975,174 @@
         .emplace(type, std::vector<detail::type_info *>());
 #endif
     if (res.second) {
         // New cache entry created; set up a weak reference to automatically remove it if the type
         // gets destroyed:
         weakref((PyObject *) type, cpp_function([type](handle wr) {
             get_internals().registered_types_py.erase(type);
+
+            // TODO consolidate the erasure code in pybind11_meta_dealloc() in class.h
+            auto &cache = get_internals().inactive_override_cache;
+            for (auto it = cache.begin(), last = cache.end(); it != last; ) {
+                if (it->first == reinterpret_cast<PyObject *>(type))
+                    it = cache.erase(it);
+                else
+                    ++it;
+            }
+
             wr.dec_ref();
         })).release();
     }
 
     return res;
 }
 
-template <typename Iterator, typename Sentinel, bool KeyIterator, return_value_policy Policy>
+/* There are a large number of apparently unused template arguments because
+ * each combination requires a separate py::class_ registration.
+ */
+template <typename Access, return_value_policy Policy, typename Iterator, typename Sentinel, typename ValueType, typename... Extra>
 struct iterator_state {
     Iterator it;
     Sentinel end;
     bool first_or_done;
 };
 
-PYBIND11_NAMESPACE_END(detail)
+// Note: these helpers take the iterator by non-const reference because some
+// iterators in the wild can't be dereferenced when const. The & after Iterator
+// is required for MSVC < 16.9. SFINAE cannot be reused for result_type due to
+// bugs in ICC, NVCC, and PGI compilers. See PR #3293.
+template <typename Iterator, typename SFINAE = decltype(*std::declval<Iterator &>())>
+struct iterator_access {
+    using result_type = decltype(*std::declval<Iterator &>());
+    // NOLINTNEXTLINE(readability-const-return-type) // PR #3263
+    result_type operator()(Iterator &it) const {
+        return *it;
+    }
+};
 
-/// Makes a python iterator from a first and past-the-end C++ InputIterator.
-template <return_value_policy Policy = return_value_policy::reference_internal,
+template <typename Iterator, typename SFINAE = decltype((*std::declval<Iterator &>()).first) >
+class iterator_key_access {
+private:
+    using pair_type = decltype(*std::declval<Iterator &>());
+
+public:
+    /* If either the pair itself or the element of the pair is a reference, we
+     * want to return a reference, otherwise a value. When the decltype
+     * expression is parenthesized it is based on the value category of the
+     * expression; otherwise it is the declared type of the pair member.
+     * The use of declval<pair_type> in the second branch rather than directly
+     * using *std::declval<Iterator &>() is a workaround for nvcc
+     * (it's not used in the first branch because going via decltype and back
+     * through declval does not perfectly preserve references).
+     */
+    using result_type = conditional_t<
+        std::is_reference<decltype(*std::declval<Iterator &>())>::value,
+        decltype(((*std::declval<Iterator &>()).first)),
+        decltype(std::declval<pair_type>().first)
+    >;
+    result_type operator()(Iterator &it) const {
+        return (*it).first;
+    }
+};
+
+template <typename Iterator, typename SFINAE = decltype((*std::declval<Iterator &>()).second)>
+class iterator_value_access {
+private:
+    using pair_type = decltype(*std::declval<Iterator &>());
+
+public:
+    using result_type = conditional_t<
+        std::is_reference<decltype(*std::declval<Iterator &>())>::value,
+        decltype(((*std::declval<Iterator &>()).second)),
+        decltype(std::declval<pair_type>().second)
+    >;
+    result_type operator()(Iterator &it) const {
+        return (*it).second;
+    }
+};
+
+template <typename Access,
+          return_value_policy Policy,
           typename Iterator,
           typename Sentinel,
-          typename ValueType = decltype(*std::declval<Iterator>()),
+          typename ValueType,
           typename... Extra>
-iterator make_iterator(Iterator first, Sentinel last, Extra &&... extra) {
-    using state = detail::iterator_state<Iterator, Sentinel, false, Policy>;
+iterator make_iterator_impl(Iterator first, Sentinel last, Extra &&... extra) {
+    using state = detail::iterator_state<Access, Policy, Iterator, Sentinel, ValueType, Extra...>;
+    // TODO: state captures only the types of Extra, not the values
 
     if (!detail::get_type_info(typeid(state), false)) {
         class_<state>(handle(), "iterator", pybind11::module_local())
             .def("__iter__", [](state &s) -> state& { return s; })
             .def("__next__", [](state &s) -> ValueType {
                 if (!s.first_or_done)
                     ++s.it;
                 else
                     s.first_or_done = false;
                 if (s.it == s.end) {
                     s.first_or_done = true;
                     throw stop_iteration();
                 }
-                return *s.it;
+                return Access()(s.it);
+            // NOLINTNEXTLINE(readability-const-return-type) // PR #3263
             }, std::forward<Extra>(extra)..., Policy);
     }
 
     return cast(state{first, last, true});
 }
 
-/// Makes an python iterator over the keys (`.first`) of a iterator over pairs from a
-/// first and past-the-end InputIterator.
+PYBIND11_NAMESPACE_END(detail)
+
+/// Makes a python iterator from a first and past-the-end C++ InputIterator.
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Iterator,
           typename Sentinel,
-          typename KeyType = decltype((*std::declval<Iterator>()).first),
+          typename ValueType = typename detail::iterator_access<Iterator>::result_type,
           typename... Extra>
-iterator make_key_iterator(Iterator first, Sentinel last, Extra &&... extra) {
-    using state = detail::iterator_state<Iterator, Sentinel, true, Policy>;
+iterator make_iterator(Iterator first, Sentinel last, Extra &&... extra) {
+    return detail::make_iterator_impl<
+        detail::iterator_access<Iterator>,
+        Policy,
+        Iterator,
+        Sentinel,
+        ValueType,
+        Extra...>(first, last, std::forward<Extra>(extra)...);
+}
 
-    if (!detail::get_type_info(typeid(state), false)) {
-        class_<state>(handle(), "iterator", pybind11::module_local())
-            .def("__iter__", [](state &s) -> state& { return s; })
-            .def("__next__", [](state &s) -> KeyType {
-                if (!s.first_or_done)
-                    ++s.it;
-                else
-                    s.first_or_done = false;
-                if (s.it == s.end) {
-                    s.first_or_done = true;
-                    throw stop_iteration();
-                }
-                return (*s.it).first;
-            }, std::forward<Extra>(extra)..., Policy);
-    }
+/// Makes a python iterator over the keys (`.first`) of a iterator over pairs from a
+/// first and past-the-end InputIterator.
+template <return_value_policy Policy = return_value_policy::reference_internal,
+          typename Iterator,
+          typename Sentinel,
+          typename KeyType = typename detail::iterator_key_access<Iterator>::result_type,
+          typename... Extra>
+iterator make_key_iterator(Iterator first, Sentinel last, Extra &&...extra) {
+    return detail::make_iterator_impl<
+        detail::iterator_key_access<Iterator>,
+        Policy,
+        Iterator,
+        Sentinel,
+        KeyType,
+        Extra...>(first, last, std::forward<Extra>(extra)...);
+}
 
-    return cast(state{first, last, true});
+/// Makes a python iterator over the values (`.second`) of a iterator over pairs from a
+/// first and past-the-end InputIterator.
+template <return_value_policy Policy = return_value_policy::reference_internal,
+          typename Iterator,
+          typename Sentinel,
+          typename ValueType = typename detail::iterator_value_access<Iterator>::result_type,
+          typename... Extra>
+iterator make_value_iterator(Iterator first, Sentinel last, Extra &&...extra) {
+    return detail::make_iterator_impl<
+        detail::iterator_value_access<Iterator>,
+        Policy, Iterator,
+        Sentinel,
+        ValueType,
+        Extra...>(first, last, std::forward<Extra>(extra)...);
 }
 
 /// Makes an iterator over values of an stl container or other container supporting
 /// `std::begin()`/`std::end()`
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Type, typename... Extra> iterator make_iterator(Type &value, Extra&&... extra) {
     return make_iterator<Policy>(std::begin(value), std::end(value), extra...);
@@ -1953,18 +2151,25 @@
 /// Makes an iterator over the keys (`.first`) of a stl map-like container supporting
 /// `std::begin()`/`std::end()`
 template <return_value_policy Policy = return_value_policy::reference_internal,
           typename Type, typename... Extra> iterator make_key_iterator(Type &value, Extra&&... extra) {
     return make_key_iterator<Policy>(std::begin(value), std::end(value), extra...);
 }
 
+/// Makes an iterator over the values (`.second`) of a stl map-like container supporting
+/// `std::begin()`/`std::end()`
+template <return_value_policy Policy = return_value_policy::reference_internal,
+          typename Type, typename... Extra> iterator make_value_iterator(Type &value, Extra&&... extra) {
+    return make_value_iterator<Policy>(std::begin(value), std::end(value), extra...);
+}
+
 template <typename InputType, typename OutputType> void implicitly_convertible() {
     struct set_flag {
         bool &flag;
-        set_flag(bool &flag_) : flag(flag_) { flag_ = true; }
+        explicit set_flag(bool &flag_) : flag(flag_) { flag_ = true; }
         ~set_flag() { flag = false; }
     };
     auto implicit_caster = [](PyObject *obj, PyTypeObject *type) -> PyObject * {
         static bool currently_used = false;
         if (currently_used) // implicit conversions are non-reentrant
             return nullptr;
         set_flag flag_helper(currently_used);
@@ -1980,20 +2185,32 @@
 
     if (auto tinfo = detail::get_type_info(typeid(OutputType)))
         tinfo->implicit_conversions.push_back(implicit_caster);
     else
         pybind11_fail("implicitly_convertible: Unable to find type " + type_id<OutputType>());
 }
 
-template <typename ExceptionTranslator>
-void register_exception_translator(ExceptionTranslator&& translator) {
+
+inline void register_exception_translator(ExceptionTranslator &&translator) {
     detail::get_internals().registered_exception_translators.push_front(
         std::forward<ExceptionTranslator>(translator));
 }
 
+
+/**
+  * Add a new module-local exception translator. Locally registered functions
+  * will be tried before any globally registered exception translators, which
+  * will only be invoked if the module-local handlers do not deal with
+  * the exception.
+  */
+inline void register_local_exception_translator(ExceptionTranslator &&translator) {
+    detail::get_local_internals().registered_exception_translators.push_front(
+        std::forward<ExceptionTranslator>(translator));
+}
+
 /**
  * Wrapper to generate a new Python exception type.
  *
  * This should only be used with PyErr_SetString for now.
  * It is not (yet) possible to use as a py::base.
  * Template type argument is reserved for future use.
  */
@@ -2019,42 +2236,70 @@
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 // Returns a reference to a function-local static exception object used in the simple
 // register_exception approach below.  (It would be simpler to have the static local variable
 // directly in register_exception, but that makes clang <3.5 segfault - issue #1349).
 template <typename CppException>
 exception<CppException> &get_exception_object() { static exception<CppException> ex; return ex; }
-PYBIND11_NAMESPACE_END(detail)
 
-/**
- * Registers a Python exception in `m` of the given `name` and installs an exception translator to
- * translate the C++ exception to the created Python exception using the exceptions what() method.
- * This is intended for simple exception translations; for more complex translation, register the
- * exception object and translator directly.
- */
+// Helper function for register_exception and register_local_exception
 template <typename CppException>
-exception<CppException> &register_exception(handle scope,
-                                            const char *name,
-                                            handle base = PyExc_Exception) {
+exception<CppException> &register_exception_impl(handle scope,
+                                                const char *name,
+                                                handle base,
+                                                bool isLocal) {
     auto &ex = detail::get_exception_object<CppException>();
     if (!ex) ex = exception<CppException>(scope, name, base);
 
-    register_exception_translator([](std::exception_ptr p) {
+    auto register_func = isLocal ? &register_local_exception_translator
+                                 : &register_exception_translator;
+
+    register_func([](std::exception_ptr p) {
         if (!p) return;
         try {
             std::rethrow_exception(p);
         } catch (const CppException &e) {
             detail::get_exception_object<CppException>()(e.what());
         }
     });
     return ex;
 }
 
+PYBIND11_NAMESPACE_END(detail)
+
+/**
+ * Registers a Python exception in `m` of the given `name` and installs a translator to
+ * translate the C++ exception to the created Python exception using the what() method.
+ * This is intended for simple exception translations; for more complex translation, register the
+ * exception object and translator directly.
+ */
+template <typename CppException>
+exception<CppException> &register_exception(handle scope,
+                                            const char *name,
+                                            handle base = PyExc_Exception) {
+    return detail::register_exception_impl<CppException>(scope, name, base, false /* isLocal */);
+}
+
+/**
+ * Registers a Python exception in `m` of the given `name` and installs a translator to
+ * translate the C++ exception to the created Python exception using the what() method.
+ * This translator will only be used for exceptions that are thrown in this module and will be
+ * tried before global exception translators, including those registered with register_exception.
+ * This is intended for simple exception translations; for more complex translation, register the
+ * exception object and translator directly.
+ */
+template <typename CppException>
+exception<CppException> &register_local_exception(handle scope,
+                                                  const char *name,
+                                                  handle base = PyExc_Exception) {
+    return detail::register_exception_impl<CppException>(scope, name, base, true /* isLocal */);
+}
+
 PYBIND11_NAMESPACE_BEGIN(detail)
-PYBIND11_NOINLINE inline void print(tuple args, dict kwargs) {
+PYBIND11_NOINLINE void print(const tuple &args, const dict &kwargs) {
     auto strings = tuple(args.size());
     for (size_t i = 0; i < args.size(); ++i) {
         strings[i] = str(args[i]);
     }
     auto sep = kwargs.contains("sep") ? kwargs["sep"] : cast(" ");
     auto line = sep.attr("join")(strings);
 
@@ -2084,181 +2329,14 @@
 
 template <return_value_policy policy = return_value_policy::automatic_reference, typename... Args>
 void print(Args &&...args) {
     auto c = detail::collect_arguments<policy>(std::forward<Args>(args)...);
     detail::print(c.args(), c.kwargs());
 }
 
-#if defined(WITH_THREAD) && !defined(PYPY_VERSION)
-
-/* The functions below essentially reproduce the PyGILState_* API using a RAII
- * pattern, but there are a few important differences:
- *
- * 1. When acquiring the GIL from an non-main thread during the finalization
- *    phase, the GILState API blindly terminates the calling thread, which
- *    is often not what is wanted. This API does not do this.
- *
- * 2. The gil_scoped_release function can optionally cut the relationship
- *    of a PyThreadState and its associated thread, which allows moving it to
- *    another thread (this is a fairly rare/advanced use case).
- *
- * 3. The reference count of an acquired thread state can be controlled. This
- *    can be handy to prevent cases where callbacks issued from an external
- *    thread would otherwise constantly construct and destroy thread state data
- *    structures.
- *
- * See the Python bindings of NanoGUI (http://github.com/wjakob/nanogui) for an
- * example which uses features 2 and 3 to migrate the Python thread of
- * execution to another thread (to run the event loop on the original thread,
- * in this case).
- */
-
-class gil_scoped_acquire {
-public:
-    PYBIND11_NOINLINE gil_scoped_acquire() {
-        auto const &internals = detail::get_internals();
-        tstate = (PyThreadState *) PYBIND11_TLS_GET_VALUE(internals.tstate);
-
-        if (!tstate) {
-            /* Check if the GIL was acquired using the PyGILState_* API instead (e.g. if
-               calling from a Python thread). Since we use a different key, this ensures
-               we don't create a new thread state and deadlock in PyEval_AcquireThread
-               below. Note we don't save this state with internals.tstate, since we don't
-               create it we would fail to clear it (its reference count should be > 0). */
-            tstate = PyGILState_GetThisThreadState();
-        }
-
-        if (!tstate) {
-            tstate = PyThreadState_New(internals.istate);
-            #if !defined(NDEBUG)
-                if (!tstate)
-                    pybind11_fail("scoped_acquire: could not create thread state!");
-            #endif
-            tstate->gilstate_counter = 0;
-            PYBIND11_TLS_REPLACE_VALUE(internals.tstate, tstate);
-        } else {
-            release = detail::get_thread_state_unchecked() != tstate;
-        }
-
-        if (release) {
-            PyEval_AcquireThread(tstate);
-        }
-
-        inc_ref();
-    }
-
-    void inc_ref() {
-        ++tstate->gilstate_counter;
-    }
-
-    PYBIND11_NOINLINE void dec_ref() {
-        --tstate->gilstate_counter;
-        #if !defined(NDEBUG)
-            if (detail::get_thread_state_unchecked() != tstate)
-                pybind11_fail("scoped_acquire::dec_ref(): thread state must be current!");
-            if (tstate->gilstate_counter < 0)
-                pybind11_fail("scoped_acquire::dec_ref(): reference count underflow!");
-        #endif
-        if (tstate->gilstate_counter == 0) {
-            #if !defined(NDEBUG)
-                if (!release)
-                    pybind11_fail("scoped_acquire::dec_ref(): internal error!");
-            #endif
-            PyThreadState_Clear(tstate);
-            if (active)
-                PyThreadState_DeleteCurrent();
-            PYBIND11_TLS_DELETE_VALUE(detail::get_internals().tstate);
-            release = false;
-        }
-    }
-
-    /// This method will disable the PyThreadState_DeleteCurrent call and the
-    /// GIL won't be acquired. This method should be used if the interpreter
-    /// could be shutting down when this is called, as thread deletion is not
-    /// allowed during shutdown. Check _Py_IsFinalizing() on Python 3.7+, and
-    /// protect subsequent code.
-    PYBIND11_NOINLINE void disarm() {
-        active = false;
-    }
-
-    PYBIND11_NOINLINE ~gil_scoped_acquire() {
-        dec_ref();
-        if (release)
-           PyEval_SaveThread();
-    }
-private:
-    PyThreadState *tstate = nullptr;
-    bool release = true;
-    bool active = true;
-};
-
-class gil_scoped_release {
-public:
-    explicit gil_scoped_release(bool disassoc = false) : disassoc(disassoc) {
-        // `get_internals()` must be called here unconditionally in order to initialize
-        // `internals.tstate` for subsequent `gil_scoped_acquire` calls. Otherwise, an
-        // initialization race could occur as multiple threads try `gil_scoped_acquire`.
-        const auto &internals = detail::get_internals();
-        tstate = PyEval_SaveThread();
-        if (disassoc) {
-            auto key = internals.tstate;
-            PYBIND11_TLS_DELETE_VALUE(key);
-        }
-    }
-
-    /// This method will disable the PyThreadState_DeleteCurrent call and the
-    /// GIL won't be acquired. This method should be used if the interpreter
-    /// could be shutting down when this is called, as thread deletion is not
-    /// allowed during shutdown. Check _Py_IsFinalizing() on Python 3.7+, and
-    /// protect subsequent code.
-    PYBIND11_NOINLINE void disarm() {
-        active = false;
-    }
-
-    ~gil_scoped_release() {
-        if (!tstate)
-            return;
-        // `PyEval_RestoreThread()` should not be called if runtime is finalizing
-        if (active)
-            PyEval_RestoreThread(tstate);
-        if (disassoc) {
-            auto key = detail::get_internals().tstate;
-            PYBIND11_TLS_REPLACE_VALUE(key, tstate);
-        }
-    }
-private:
-    PyThreadState *tstate;
-    bool disassoc;
-    bool active = true;
-};
-#elif defined(PYPY_VERSION)
-class gil_scoped_acquire {
-    PyGILState_STATE state;
-public:
-    gil_scoped_acquire() { state = PyGILState_Ensure(); }
-    ~gil_scoped_acquire() { PyGILState_Release(state); }
-    void disarm() {}
-};
-
-class gil_scoped_release {
-    PyThreadState *state;
-public:
-    gil_scoped_release() { state = PyEval_SaveThread(); }
-    ~gil_scoped_release() { PyEval_RestoreThread(state); }
-    void disarm() {}
-};
-#else
-class gil_scoped_acquire {
-    void disarm() {}
-};
-class gil_scoped_release {
-    void disarm() {}
-};
-#endif
-
 error_already_set::~error_already_set() {
     if (m_type) {
         gil_scoped_acquire gil;
         error_scope scope;
         m_type.release().dec_ref();
         m_value.release().dec_ref();
         m_trace.release().dec_ref();
@@ -2283,24 +2361,50 @@
     if (override.is_cpp_function()) {
         cache.insert(key);
         return function();
     }
 
     /* Don't call dispatch code if invoked from overridden function.
        Unfortunately this doesn't work on PyPy. */
-#if !defined(PYPY_VERSION)
+#if !defined(PYPY_VERSION) && PY_VERSION_HEX < 0x030B0000
+    // TODO: Remove PyPy workaround for Python 3.11.
+    // Current API fails on 3.11 since co_varnames can be null.
+#if PY_VERSION_HEX >= 0x03090000
+    PyFrameObject *frame = PyThreadState_GetFrame(PyThreadState_Get());
+    if (frame != nullptr) {
+        PyCodeObject *f_code = PyFrame_GetCode(frame);
+        // f_code is guaranteed to not be NULL
+        if ((std::string) str(f_code->co_name) == name && f_code->co_argcount > 0) {
+            PyObject* locals = PyEval_GetLocals();
+            if (locals != nullptr && f_code->co_varnames != nullptr) {
+                PyObject *self_caller = dict_getitem(
+                    locals, PyTuple_GET_ITEM(f_code->co_varnames, 0)
+                );
+                if (self_caller == self.ptr()) {
+                    Py_DECREF(f_code);
+                    Py_DECREF(frame);
+                    return function();
+                }
+            }
+        }
+        Py_DECREF(f_code);
+        Py_DECREF(frame);
+    }
+#else
     PyFrameObject *frame = PyThreadState_Get()->frame;
-    if (frame && (std::string) str(frame->f_code->co_name) == name &&
-        frame->f_code->co_argcount > 0) {
+    if (frame != nullptr && (std::string) str(frame->f_code->co_name) == name
+        && frame->f_code->co_argcount > 0) {
         PyFrame_FastToLocals(frame);
-        PyObject *self_caller = PyDict_GetItem(
+        PyObject *self_caller = dict_getitem(
             frame->f_locals, PyTuple_GET_ITEM(frame->f_code->co_varnames, 0));
         if (self_caller == self.ptr())
             return function();
     }
+#endif
+
 #else
     /* PyPy currently doesn't provide a detailed cpyext emulation of
        frame objects, so we have to emulate this using Python. This
        is going to be slow..*/
     dict d; d["self"] = self; d["name"] = pybind11::str(name);
     PyObject *result = PyRun_String(
         "import inspect\n"
@@ -2333,26 +2437,27 @@
   :return: The Python method by this name from the object or an empty function wrapper.
  \endrst */
 template <class T> function get_override(const T *this_ptr, const char *name) {
     auto tinfo = detail::get_type_info(typeid(T));
     return tinfo ? detail::get_type_override(this_ptr, tinfo, name) : function();
 }
 
-#define PYBIND11_OVERRIDE_IMPL(ret_type, cname, name, ...) \
-    do { \
-        pybind11::gil_scoped_acquire gil; \
-        pybind11::function override = pybind11::get_override(static_cast<const cname *>(this), name); \
-        if (override) { \
-            auto o = override(__VA_ARGS__); \
-            if (pybind11::detail::cast_is_temporary_value_reference<ret_type>::value) { \
-                static pybind11::detail::override_caster_t<ret_type> caster; \
-                return pybind11::detail::cast_ref<ret_type>(std::move(o), caster); \
-            } \
-            else return pybind11::detail::cast_safe<ret_type>(std::move(o)); \
-        } \
+#define PYBIND11_OVERRIDE_IMPL(ret_type, cname, name, ...)                                        \
+    do {                                                                                          \
+        pybind11::gil_scoped_acquire gil;                                                         \
+        pybind11::function override                                                               \
+            = pybind11::get_override(static_cast<const cname *>(this), name);                     \
+        if (override) {                                                                           \
+            auto o = override(__VA_ARGS__);                                                       \
+            if (pybind11::detail::cast_is_temporary_value_reference<ret_type>::value) {           \
+                static pybind11::detail::override_caster_t<ret_type> caster;                      \
+                return pybind11::detail::cast_ref<ret_type>(std::move(o), caster);                \
+            }                                                                                     \
+            return pybind11::detail::cast_safe<ret_type>(std::move(o));                           \
+        }                                                                                         \
     } while (false)
 
 /** \rst
     Macro to populate the virtual method in the trampoline class. This macro tries to look up a method named 'fn'
     from the Python side, deals with the :ref:`gil` and necessary argument conversions to call this method and return
     the appropriate type. See :ref:`overriding_virtuals` for more information. This macro should be used when the method
     name in C is not the same as the method name in Python. For example with `__str__`.
@@ -2440,12 +2545,10 @@
 #define PYBIND11_OVERLOAD(ret_type, cname, fn, ...) \
     PYBIND11_OVERRIDE(PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), fn, __VA_ARGS__)
 #define PYBIND11_OVERLOAD_PURE(ret_type, cname, fn, ...) \
     PYBIND11_OVERRIDE_PURE(PYBIND11_TYPE(ret_type), PYBIND11_TYPE(cname), fn, __VA_ARGS__);
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
 
-#if defined(_MSC_VER) && !defined(__INTEL_COMPILER)
-#  pragma warning(pop)
-#elif defined(__GNUG__) && !defined(__clang__)
-#  pragma GCC diagnostic pop
+#if defined(__GNUC__) && __GNUC__ == 7
+#    pragma GCC diagnostic pop // -Wnoexcept-type
 #endif
```

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/pytypes.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/pytypes.h`

 * *Files 12% similar despite different names*

```diff
@@ -10,25 +10,33 @@
 #pragma once
 
 #include "detail/common.h"
 #include "buffer_info.h"
 #include <utility>
 #include <type_traits>
 
+#if defined(PYBIND11_HAS_OPTIONAL)
+#  include <optional>
+#endif
+
+#ifdef PYBIND11_HAS_STRING_VIEW
+#  include <string_view>
+#endif
+
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 
 /* A few forward declarations */
 class handle; class object;
 class str; class iterator;
 class type;
 struct arg; struct arg_v;
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 class args_proxy;
-inline bool isinstance_generic(handle obj, const std::type_info &tp);
+bool isinstance_generic(handle obj, const std::type_info &tp);
 
 // Accessor forward declarations
 template <typename Policy> class accessor;
 namespace accessor_policies {
     struct obj_attr;
     struct str_attr;
     struct generic_item;
@@ -174,14 +182,15 @@
         counting features.
 \endrst */
 class handle : public detail::object_api<handle> {
 public:
     /// The default constructor creates a handle with a ``nullptr``-valued pointer
     handle() = default;
     /// Creates a ``handle`` from the given raw Python object pointer
+    // NOLINTNEXTLINE(google-explicit-constructor)
     handle(PyObject *ptr) : m_ptr(ptr) { } // Allow implicit conversion from PyObject*
 
     /// Return the underlying ``PyObject *`` pointer
     PyObject *ptr() const { return m_ptr; }
     PyObject *&ptr() { return m_ptr; }
 
     /** \rst
@@ -250,16 +259,19 @@
       PyObject *tmp = m_ptr;
       m_ptr = nullptr;
       return handle(tmp);
     }
 
     object& operator=(const object &other) {
         other.inc_ref();
-        dec_ref();
+        // Use temporary variable to ensure `*this` remains valid while
+        // `Py_XDECREF` executes, in case `*this` is accessible from Python.
+        handle temp(m_ptr);
         m_ptr = other.m_ptr;
+        temp.dec_ref();
         return *this;
     }
 
     object& operator=(object &&other) noexcept {
         if (this != &other) {
             handle temp(m_ptr);
             m_ptr = other.m_ptr;
@@ -275,16 +287,18 @@
     template <typename T> T cast() &&;
 
 protected:
     // Tags for choosing constructors from raw PyObject *
     struct borrowed_t { };
     struct stolen_t { };
 
+    /// @cond BROKEN
     template <typename T> friend T reinterpret_borrow(handle);
     template <typename T> friend T reinterpret_steal(handle);
+    /// @endcond
 
 public:
     // Only accessible from derived classes and the reinterpret_* functions
     object(handle h, borrowed_t) : handle(h) { inc_ref(); }
     object(handle h, stolen_t) : handle(h) { }
 };
 
@@ -310,22 +324,26 @@
 
         PyObject *p = PyObject_Str(obj);
         py::str s = reinterpret_steal<py::str>(p); // <-- `p` must be already be a `str`
 \endrst */
 template <typename T> T reinterpret_steal(handle h) { return {h, object::stolen_t{}}; }
 
 PYBIND11_NAMESPACE_BEGIN(detail)
-inline std::string error_string();
+std::string error_string();
 PYBIND11_NAMESPACE_END(detail)
 
+#if defined(_MSC_VER)
+#  pragma warning(push)
+#  pragma warning(disable: 4275 4251) // warning C4275: An exported class was derived from a class that wasn't exported. Can be ignored when derived from a STL class.
+#endif
 /// Fetch and hold an error which was already set in Python.  An instance of this is typically
 /// thrown to propagate python-side errors back through C++ which can either be caught manually or
 /// else falls back to the function dispatcher (which then raises the captured error back to
 /// python).
-class error_already_set : public std::runtime_error {
+class PYBIND11_EXPORT_EXCEPTION error_already_set : public std::runtime_error {
 public:
     /// Constructs a new exception from the current Python error indicator, if any.  The current
     /// Python error indicator will be cleared.
     error_already_set() : std::runtime_error(detail::error_string()) {
         PyErr_Fetch(&m_type.ptr(), &m_value.ptr(), &m_trace.ptr());
     }
 
@@ -335,46 +353,93 @@
     inline ~error_already_set() override;
 
     /// Give the currently-held error back to Python, if any.  If there is currently a Python error
     /// already set it is cleared first.  After this call, the current object no longer stores the
     /// error variables (but the `.what()` string is still available).
     void restore() { PyErr_Restore(m_type.release().ptr(), m_value.release().ptr(), m_trace.release().ptr()); }
 
-    /// If it is impossible to raise the currently-held error, such as in destructor, we can write
-    /// it out using Python's unraisable hook (sys.unraisablehook). The error context should be
-    /// some object whose repr() helps identify the location of the error. Python already knows the
-    /// type and value of the error, so there is no need to repeat that. For example, __func__ could
-    /// be helpful. After this call, the current object no longer stores the error variables,
-    /// and neither does Python.
+    /// If it is impossible to raise the currently-held error, such as in a destructor, we can write
+    /// it out using Python's unraisable hook (`sys.unraisablehook`). The error context should be
+    /// some object whose `repr()` helps identify the location of the error. Python already knows the
+    /// type and value of the error, so there is no need to repeat that. After this call, the current
+    /// object no longer stores the error variables, and neither does Python.
     void discard_as_unraisable(object err_context) {
         restore();
         PyErr_WriteUnraisable(err_context.ptr());
     }
+    /// An alternate version of `discard_as_unraisable()`, where a string provides information on the
+    /// location of the error. For example, `__func__` could be helpful.
     void discard_as_unraisable(const char *err_context) {
         discard_as_unraisable(reinterpret_steal<object>(PYBIND11_FROM_STRING(err_context)));
     }
 
     // Does nothing; provided for backwards compatibility.
     PYBIND11_DEPRECATED("Use of error_already_set.clear() is deprecated")
     void clear() {}
 
     /// Check if the currently trapped error type matches the given Python exception class (or a
     /// subclass thereof).  May also be passed a tuple to search for any exception class matches in
     /// the given tuple.
-    bool matches(handle exc) const { return PyErr_GivenExceptionMatches(m_type.ptr(), exc.ptr()); }
+    bool matches(handle exc) const {
+        return (PyErr_GivenExceptionMatches(m_type.ptr(), exc.ptr()) != 0);
+    }
 
     const object& type() const { return m_type; }
     const object& value() const { return m_value; }
     const object& trace() const { return m_trace; }
 
 private:
     object m_type, m_value, m_trace;
 };
+#if defined(_MSC_VER)
+#  pragma warning(pop)
+#endif
+
+#if PY_VERSION_HEX >= 0x03030000
 
-/** \defgroup python_builtins _
+/// Replaces the current Python error indicator with the chosen error, performing a
+/// 'raise from' to indicate that the chosen error was caused by the original error.
+inline void raise_from(PyObject *type, const char *message) {
+    // Based on _PyErr_FormatVFromCause:
+    // https://github.com/python/cpython/blob/467ab194fc6189d9f7310c89937c51abeac56839/Python/errors.c#L405
+    // See https://github.com/pybind/pybind11/pull/2112 for details.
+    PyObject *exc = nullptr, *val = nullptr, *val2 = nullptr, *tb = nullptr;
+
+    assert(PyErr_Occurred());
+    PyErr_Fetch(&exc, &val, &tb);
+    PyErr_NormalizeException(&exc, &val, &tb);
+    if (tb != nullptr) {
+        PyException_SetTraceback(val, tb);
+        Py_DECREF(tb);
+    }
+    Py_DECREF(exc);
+    assert(!PyErr_Occurred());
+
+    PyErr_SetString(type, message);
+
+    PyErr_Fetch(&exc, &val2, &tb);
+    PyErr_NormalizeException(&exc, &val2, &tb);
+    Py_INCREF(val);
+    PyException_SetCause(val2, val);
+    PyException_SetContext(val2, val);
+    PyErr_Restore(exc, val2, tb);
+}
+
+/// Sets the current Python error indicator with the chosen error, performing a 'raise from'
+/// from the error contained in error_already_set to indicate that the chosen error was
+/// caused by the original error. After this function is called error_already_set will
+/// no longer contain an error.
+inline void raise_from(error_already_set& err, PyObject *type, const char *message) {
+    err.restore();
+    raise_from(type, message);
+}
+
+#endif
+
+/** \defgroup python_builtins const_name
     Unless stated otherwise, the following C++ functions behave the same
     as their Python counterparts.
  */
 
 /** \ingroup python_builtins
     \rst
     Return true if ``obj`` is an instance of ``T``. Type ``T`` must be a subclass of
@@ -427,27 +492,25 @@
     if (!result) { throw error_already_set(); }
     return reinterpret_steal<object>(result);
 }
 
 inline object getattr(handle obj, handle name, handle default_) {
     if (PyObject *result = PyObject_GetAttr(obj.ptr(), name.ptr())) {
         return reinterpret_steal<object>(result);
-    } else {
-        PyErr_Clear();
-        return reinterpret_borrow<object>(default_);
     }
+    PyErr_Clear();
+    return reinterpret_borrow<object>(default_);
 }
 
 inline object getattr(handle obj, const char *name, handle default_) {
     if (PyObject *result = PyObject_GetAttrString(obj.ptr(), name)) {
         return reinterpret_steal<object>(result);
-    } else {
-        PyErr_Clear();
-        return reinterpret_borrow<object>(default_);
     }
+    PyErr_Clear();
+    return reinterpret_borrow<object>(default_);
 }
 
 inline void setattr(handle obj, handle name, handle value) {
     if (PyObject_SetAttr(obj.ptr(), name.ptr(), value.ptr()) != 0) { throw error_already_set(); }
 }
 
 inline void setattr(handle obj, const char *name, handle value) {
@@ -472,33 +535,74 @@
 #endif
         if (PyMethod_Check(value.ptr()))
             value = PyMethod_GET_FUNCTION(value.ptr());
     }
     return value;
 }
 
+// Reimplementation of python's dict helper functions to ensure that exceptions
+// aren't swallowed (see #2862)
+
+// copied from cpython _PyDict_GetItemStringWithError
+inline PyObject * dict_getitemstring(PyObject *v, const char *key)
+{
+#if PY_MAJOR_VERSION >= 3
+    PyObject *kv = nullptr, *rv = nullptr;
+    kv = PyUnicode_FromString(key);
+    if (kv == NULL) {
+        throw error_already_set();
+    }
+
+    rv = PyDict_GetItemWithError(v, kv);
+    Py_DECREF(kv);
+    if (rv == NULL && PyErr_Occurred()) {
+        throw error_already_set();
+    }
+    return rv;
+#else
+    return PyDict_GetItemString(v, key);
+#endif
+}
+
+inline PyObject * dict_getitem(PyObject *v, PyObject *key)
+{
+#if PY_MAJOR_VERSION >= 3
+    PyObject *rv = PyDict_GetItemWithError(v, key);
+    if (rv == NULL && PyErr_Occurred()) {
+        throw error_already_set();
+    }
+    return rv;
+#else
+    return PyDict_GetItem(v, key);
+#endif
+}
+
 // Helper aliases/functions to support implicit casting of values given to python accessors/methods.
 // When given a pyobject, this simply returns the pyobject as-is; for other C++ type, the value goes
 // through pybind11::cast(obj) to convert it to an `object`.
 template <typename T, enable_if_t<is_pyobject<T>::value, int> = 0>
 auto object_or_cast(T &&o) -> decltype(std::forward<T>(o)) { return std::forward<T>(o); }
 // The following casting version is implemented in cast.h:
 template <typename T, enable_if_t<!is_pyobject<T>::value, int> = 0>
 object object_or_cast(T &&o);
 // Match a PyObject*, which we want to convert directly to handle via its converting constructor
 inline handle object_or_cast(PyObject *ptr) { return ptr; }
 
+#if defined(_MSC_VER) && _MSC_VER < 1920
+#  pragma warning(push)
+#  pragma warning(disable: 4522) // warning C4522: multiple assignment operators specified
+#endif
 template <typename Policy>
 class accessor : public object_api<accessor<Policy>> {
     using key_type = typename Policy::key_type;
 
 public:
     accessor(handle obj, key_type key) : obj(obj), key(std::move(key)) { }
     accessor(const accessor &) = default;
-    accessor(accessor &&) = default;
+    accessor(accessor &&) noexcept = default;
 
     // accessor overload required to override default assignment operator (templates are not allowed
     // to replace default compiler-generated assignments).
     void operator=(const accessor &a) && { std::move(*this).operator=(handle(a)); }
     void operator=(const accessor &a) & { operator=(handle(a)); }
 
     template <typename T> void operator=(T &&value) && {
@@ -516,14 +620,15 @@
     }
     template <typename T = Policy>
     PYBIND11_DEPRECATED("Use of obj[key] as bool is deprecated in favor of obj.contains(key)")
     explicit operator enable_if_t<std::is_same<T, accessor_policies::generic_item>::value, bool>() const {
         return obj.contains(key);
     }
 
+    // NOLINTNEXTLINE(google-explicit-constructor)
     operator object() const { return get_cache(); }
     PyObject *ptr() const { return get_cache().ptr(); }
     template <typename T> T cast() const { return get_cache().template cast<T>(); }
 
 private:
     object &get_cache() const {
         if (!cache) { cache = Policy::get(obj, key); }
@@ -531,14 +636,17 @@
     }
 
 private:
     handle obj;
     key_type key;
     mutable object cache;
 };
+#if defined(_MSC_VER) && _MSC_VER < 1920
+#  pragma warning(pop)
+#endif
 
 PYBIND11_NAMESPACE_BEGIN(accessor_policies)
 struct obj_attr {
     using key_type = object;
     static object get(handle obj, handle key) { return getattr(obj, key); }
     static void set(handle obj, handle key, handle val) { setattr(obj, key, val); }
 };
@@ -562,57 +670,63 @@
         if (PyObject_SetItem(obj.ptr(), key.ptr(), val.ptr()) != 0) { throw error_already_set(); }
     }
 };
 
 struct sequence_item {
     using key_type = size_t;
 
-    static object get(handle obj, size_t index) {
-        PyObject *result = PySequence_GetItem(obj.ptr(), static_cast<ssize_t>(index));
+    template <typename IdxType, detail::enable_if_t<std::is_integral<IdxType>::value, int> = 0>
+    static object get(handle obj, const IdxType &index) {
+        PyObject *result = PySequence_GetItem(obj.ptr(), ssize_t_cast(index));
         if (!result) { throw error_already_set(); }
         return reinterpret_steal<object>(result);
     }
 
-    static void set(handle obj, size_t index, handle val) {
+    template <typename IdxType, detail::enable_if_t<std::is_integral<IdxType>::value, int> = 0>
+    static void set(handle obj, const IdxType &index, handle val) {
         // PySequence_SetItem does not steal a reference to 'val'
-        if (PySequence_SetItem(obj.ptr(), static_cast<ssize_t>(index), val.ptr()) != 0) {
+        if (PySequence_SetItem(obj.ptr(), ssize_t_cast(index), val.ptr()) != 0) {
             throw error_already_set();
         }
     }
 };
 
 struct list_item {
     using key_type = size_t;
 
-    static object get(handle obj, size_t index) {
-        PyObject *result = PyList_GetItem(obj.ptr(), static_cast<ssize_t>(index));
+    template <typename IdxType, detail::enable_if_t<std::is_integral<IdxType>::value, int> = 0>
+    static object get(handle obj, const IdxType &index) {
+        PyObject *result = PyList_GetItem(obj.ptr(), ssize_t_cast(index));
         if (!result) { throw error_already_set(); }
         return reinterpret_borrow<object>(result);
     }
 
-    static void set(handle obj, size_t index, handle val) {
+    template <typename IdxType, detail::enable_if_t<std::is_integral<IdxType>::value, int> = 0>
+    static void set(handle obj, const IdxType &index, handle val) {
         // PyList_SetItem steals a reference to 'val'
-        if (PyList_SetItem(obj.ptr(), static_cast<ssize_t>(index), val.inc_ref().ptr()) != 0) {
+        if (PyList_SetItem(obj.ptr(), ssize_t_cast(index), val.inc_ref().ptr()) != 0) {
             throw error_already_set();
         }
     }
 };
 
 struct tuple_item {
     using key_type = size_t;
 
-    static object get(handle obj, size_t index) {
-        PyObject *result = PyTuple_GetItem(obj.ptr(), static_cast<ssize_t>(index));
+    template <typename IdxType, detail::enable_if_t<std::is_integral<IdxType>::value, int> = 0>
+    static object get(handle obj, const IdxType &index) {
+        PyObject *result = PyTuple_GetItem(obj.ptr(), ssize_t_cast(index));
         if (!result) { throw error_already_set(); }
         return reinterpret_borrow<object>(result);
     }
 
-    static void set(handle obj, size_t index, handle val) {
+    template <typename IdxType, detail::enable_if_t<std::is_integral<IdxType>::value, int> = 0>
+    static void set(handle obj, const IdxType &index, handle val) {
         // PyTuple_SetItem steals a reference to 'val'
-        if (PyTuple_SetItem(obj.ptr(), static_cast<ssize_t>(index), val.inc_ref().ptr()) != 0) {
+        if (PyTuple_SetItem(obj.ptr(), ssize_t_cast(index), val.inc_ref().ptr()) != 0) {
             throw error_already_set();
         }
     }
 };
 PYBIND11_NAMESPACE_END(accessor_policies)
 
 /// STL iterator template used for tuple, list, sequence and dict
@@ -626,15 +740,17 @@
     using value_type = typename Policy::value_type;
     using reference = typename Policy::reference;
     using pointer = typename Policy::pointer;
 
     generic_iterator() = default;
     generic_iterator(handle seq, ssize_t index) : Policy(seq, index) { }
 
+    // NOLINTNEXTLINE(readability-const-return-type) // PR #3263
     reference operator*() const { return Policy::dereference(); }
+    // NOLINTNEXTLINE(readability-const-return-type) // PR #3263
     reference operator[](difference_type n) const { return *(*this + n); }
     pointer operator->() const { return **this; }
 
     It &operator++() { Policy::increment(); return *this; }
     It operator++(int) { auto copy = *this; Policy::increment(); return copy; }
     It &operator--() { Policy::decrement(); return *this; }
     It operator--(int) { auto copy = *this; Policy::decrement(); return copy; }
@@ -656,28 +772,30 @@
 
 PYBIND11_NAMESPACE_BEGIN(iterator_policies)
 /// Quick proxy class needed to implement ``operator->`` for iterators which can't return pointers
 template <typename T>
 struct arrow_proxy {
     T value;
 
-    arrow_proxy(T &&value) : value(std::move(value)) { }
+    // NOLINTNEXTLINE(google-explicit-constructor)
+    arrow_proxy(T &&value) noexcept : value(std::move(value)) { }
     T *operator->() const { return &value; }
 };
 
 /// Lightweight iterator policy using just a simple pointer: see ``PySequence_Fast_ITEMS``
 class sequence_fast_readonly {
 protected:
     using iterator_category = std::random_access_iterator_tag;
     using value_type = handle;
-    using reference = const handle;
+    using reference = const handle; // PR #3263
     using pointer = arrow_proxy<const handle>;
 
     sequence_fast_readonly(handle obj, ssize_t n) : ptr(PySequence_Fast_ITEMS(obj.ptr()) + n) { }
 
+    // NOLINTNEXTLINE(readability-const-return-type) // PR #3263
     reference dereference() const { return *ptr; }
     void increment() { ++ptr; }
     void decrement() { --ptr; }
     void advance(ssize_t n) { ptr += n; }
     bool equal(const sequence_fast_readonly &b) const { return ptr == b.ptr; }
     ssize_t distance_to(const sequence_fast_readonly &b) const { return ptr - b.ptr; }
 
@@ -708,22 +826,27 @@
 };
 
 /// Python's dictionary protocol permits this to be a forward iterator
 class dict_readonly {
 protected:
     using iterator_category = std::forward_iterator_tag;
     using value_type = std::pair<handle, handle>;
-    using reference = const value_type;
+    using reference = const value_type; // PR #3263
     using pointer = arrow_proxy<const value_type>;
 
     dict_readonly() = default;
     dict_readonly(handle obj, ssize_t pos) : obj(obj), pos(pos) { increment(); }
 
+    // NOLINTNEXTLINE(readability-const-return-type) // PR #3263
     reference dereference() const { return {key, value}; }
-    void increment() { if (!PyDict_Next(obj.ptr(), &pos, &key, &value)) { pos = -1; } }
+    void increment() {
+        if (PyDict_Next(obj.ptr(), &pos, &key, &value) == 0) {
+            pos = -1;
+        }
+    }
     bool equal(const dict_readonly &b) const { return pos == b.pos; }
 
 private:
     handle obj;
     PyObject *key = nullptr, *value = nullptr;
     ssize_t pos = -1;
 };
@@ -741,24 +864,28 @@
 using dict_iterator = generic_iterator<iterator_policies::dict_readonly>;
 
 inline bool PyIterable_Check(PyObject *obj) {
     PyObject *iter = PyObject_GetIter(obj);
     if (iter) {
         Py_DECREF(iter);
         return true;
-    } else {
-        PyErr_Clear();
-        return false;
     }
+    PyErr_Clear();
+    return false;
 }
 
 inline bool PyNone_Check(PyObject *o) { return o == Py_None; }
 inline bool PyEllipsis_Check(PyObject *o) { return o == Py_Ellipsis; }
 
+#ifdef PYBIND11_STR_LEGACY_PERMISSIVE
 inline bool PyUnicode_Check_Permissive(PyObject *o) { return PyUnicode_Check(o) || PYBIND11_BYTES_CHECK(o); }
+#define PYBIND11_STR_CHECK_FUN detail::PyUnicode_Check_Permissive
+#else
+#define PYBIND11_STR_CHECK_FUN PyUnicode_Check
+#endif
 
 inline bool PyStaticMethod_Check(PyObject *o) { return o->ob_type == &PyStaticMethod_Type; }
 
 class kwargs_proxy : public handle {
 public:
     explicit kwargs_proxy(handle h) : handle(h) { }
 };
@@ -793,39 +920,48 @@
 #define PYBIND11_OBJECT_COMMON(Name, Parent, CheckFun) \
     public: \
         PYBIND11_DEPRECATED("Use reinterpret_borrow<"#Name">() or reinterpret_steal<"#Name">()") \
         Name(handle h, bool is_borrowed) : Parent(is_borrowed ? Parent(h, borrowed_t{}) : Parent(h, stolen_t{})) { } \
         Name(handle h, borrowed_t) : Parent(h, borrowed_t{}) { } \
         Name(handle h, stolen_t) : Parent(h, stolen_t{}) { } \
         PYBIND11_DEPRECATED("Use py::isinstance<py::python_type>(obj) instead") \
-        bool check() const { return m_ptr != nullptr && (bool) CheckFun(m_ptr); } \
+        bool check() const { return m_ptr != nullptr && (CheckFun(m_ptr) != 0); } \
         static bool check_(handle h) { return h.ptr() != nullptr && CheckFun(h.ptr()); } \
         template <typename Policy_> \
+        /* NOLINTNEXTLINE(google-explicit-constructor) */ \
         Name(const ::pybind11::detail::accessor<Policy_> &a) : Name(object(a)) { }
 
 #define PYBIND11_OBJECT_CVT(Name, Parent, CheckFun, ConvertFun) \
     PYBIND11_OBJECT_COMMON(Name, Parent, CheckFun) \
     /* This is deliberately not 'explicit' to allow implicit conversion from object: */ \
+    /* NOLINTNEXTLINE(google-explicit-constructor) */ \
     Name(const object &o) \
     : Parent(check_(o) ? o.inc_ref().ptr() : ConvertFun(o.ptr()), stolen_t{}) \
     { if (!m_ptr) throw error_already_set(); } \
+    /* NOLINTNEXTLINE(google-explicit-constructor) */ \
     Name(object &&o) \
     : Parent(check_(o) ? o.release().ptr() : ConvertFun(o.ptr()), stolen_t{}) \
     { if (!m_ptr) throw error_already_set(); }
 
+#define PYBIND11_OBJECT_CVT_DEFAULT(Name, Parent, CheckFun, ConvertFun) \
+    PYBIND11_OBJECT_CVT(Name, Parent, CheckFun, ConvertFun) \
+    Name() : Parent() { }
+
 #define PYBIND11_OBJECT_CHECK_FAILED(Name, o_ptr) \
     ::pybind11::type_error("Object of type '" + \
                            ::pybind11::detail::get_fully_qualified_tp_name(Py_TYPE(o_ptr)) + \
                            "' is not an instance of '" #Name "'")
 
 #define PYBIND11_OBJECT(Name, Parent, CheckFun) \
     PYBIND11_OBJECT_COMMON(Name, Parent, CheckFun) \
     /* This is deliberately not 'explicit' to allow implicit conversion from object: */ \
+    /* NOLINTNEXTLINE(google-explicit-constructor) */ \
     Name(const object &o) : Parent(o) \
     { if (m_ptr && !check_(m_ptr)) throw PYBIND11_OBJECT_CHECK_FAILED(Name, m_ptr); } \
+    /* NOLINTNEXTLINE(google-explicit-constructor) */ \
     Name(object &&o) : Parent(std::move(o)) \
     { if (m_ptr && !check_(m_ptr)) throw PYBIND11_OBJECT_CHECK_FAILED(Name, m_ptr); }
 
 #define PYBIND11_OBJECT_DEFAULT(Name, Parent, CheckFun) \
     PYBIND11_OBJECT(Name, Parent, CheckFun) \
     Name() : Parent() { }
 
@@ -841,15 +977,15 @@
     value using ``operator*()``.
 \endrst */
 class iterator : public object {
 public:
     using iterator_category = std::input_iterator_tag;
     using difference_type = ssize_t;
     using value_type = handle;
-    using reference = const handle;
+    using reference = const handle; // PR #3263
     using pointer = const handle *;
 
     PYBIND11_OBJECT_DEFAULT(iterator, object, PyIter_Check)
 
     iterator& operator++() {
         advance();
         return *this;
@@ -857,14 +993,15 @@
 
     iterator operator++(int) {
         auto rv = *this;
         advance();
         return rv;
     }
 
+    // NOLINTNEXTLINE(readability-const-return-type) // PR #3263
     reference operator*() const {
         if (m_ptr && !value.ptr()) {
             auto& self = const_cast<iterator &>(*this);
             self.advance();
         }
         return value;
     }
@@ -930,46 +1067,64 @@
     PYBIND11_OBJECT_DEFAULT(iterable, object, detail::PyIterable_Check)
 };
 
 class bytes;
 
 class str : public object {
 public:
-    PYBIND11_OBJECT_CVT(str, object, detail::PyUnicode_Check_Permissive, raw_str)
+    PYBIND11_OBJECT_CVT(str, object, PYBIND11_STR_CHECK_FUN, raw_str)
 
-    str(const char *c, size_t n)
-        : object(PyUnicode_FromStringAndSize(c, (ssize_t) n), stolen_t{}) {
+    template <typename SzType, detail::enable_if_t<std::is_integral<SzType>::value, int> = 0>
+    str(const char *c, const SzType &n)
+        : object(PyUnicode_FromStringAndSize(c, ssize_t_cast(n)), stolen_t{}) {
         if (!m_ptr) pybind11_fail("Could not allocate string object!");
     }
 
     // 'explicit' is explicitly omitted from the following constructors to allow implicit conversion to py::str from C++ string-like objects
+    // NOLINTNEXTLINE(google-explicit-constructor)
     str(const char *c = "")
         : object(PyUnicode_FromString(c), stolen_t{}) {
         if (!m_ptr) pybind11_fail("Could not allocate string object!");
     }
 
+    // NOLINTNEXTLINE(google-explicit-constructor)
     str(const std::string &s) : str(s.data(), s.size()) { }
 
+#ifdef PYBIND11_HAS_STRING_VIEW
+    // enable_if is needed to avoid "ambiguous conversion" errors (see PR #3521).
+    template <typename T, detail::enable_if_t<std::is_same<T, std::string_view>::value, int> = 0>
+    // NOLINTNEXTLINE(google-explicit-constructor)
+    str(T s) : str(s.data(), s.size()) { }
+
+# ifdef PYBIND11_HAS_U8STRING
+    // reinterpret_cast here is safe (C++20 guarantees char8_t has the same size/alignment as char)
+    // NOLINTNEXTLINE(google-explicit-constructor)
+    str(std::u8string_view s) : str(reinterpret_cast<const char*>(s.data()), s.size()) { }
+# endif
+
+#endif
+
     explicit str(const bytes &b);
 
     /** \rst
         Return a string representation of the object. This is analogous to
         the ``str()`` function in Python.
     \endrst */
     explicit str(handle h) : object(raw_str(h.ptr()), stolen_t{}) { if (!m_ptr) throw error_already_set(); }
 
+    // NOLINTNEXTLINE(google-explicit-constructor)
     operator std::string() const {
         object temp = *this;
         if (PyUnicode_Check(m_ptr)) {
             temp = reinterpret_steal<object>(PyUnicode_AsUTF8String(m_ptr));
             if (!temp)
-                pybind11_fail("Unable to extract string contents! (encoding issue)");
+                throw error_already_set();
         }
-        char *buffer;
-        ssize_t length;
+        char *buffer = nullptr;
+        ssize_t length = 0;
         if (PYBIND11_BYTES_AS_STRING_AND_SIZE(temp.ptr(), &buffer, &length))
             pybind11_fail("Unable to extract string contents! (invalid type)");
         return std::string(buffer, (size_t) length);
     }
 
     template <typename... Args>
     str format(Args &&...args) const {
@@ -1000,71 +1155,124 @@
 /// \addtogroup pytypes
 /// @{
 class bytes : public object {
 public:
     PYBIND11_OBJECT(bytes, object, PYBIND11_BYTES_CHECK)
 
     // Allow implicit conversion:
+    // NOLINTNEXTLINE(google-explicit-constructor)
     bytes(const char *c = "")
         : object(PYBIND11_BYTES_FROM_STRING(c), stolen_t{}) {
         if (!m_ptr) pybind11_fail("Could not allocate bytes object!");
     }
 
-    bytes(const char *c, size_t n)
-        : object(PYBIND11_BYTES_FROM_STRING_AND_SIZE(c, (ssize_t) n), stolen_t{}) {
+    template <typename SzType, detail::enable_if_t<std::is_integral<SzType>::value, int> = 0>
+    bytes(const char *c, const SzType &n)
+        : object(PYBIND11_BYTES_FROM_STRING_AND_SIZE(c, ssize_t_cast(n)), stolen_t{}) {
         if (!m_ptr) pybind11_fail("Could not allocate bytes object!");
     }
 
     // Allow implicit conversion:
+    // NOLINTNEXTLINE(google-explicit-constructor)
     bytes(const std::string &s) : bytes(s.data(), s.size()) { }
 
     explicit bytes(const pybind11::str &s);
 
+    // NOLINTNEXTLINE(google-explicit-constructor)
     operator std::string() const {
-        char *buffer;
-        ssize_t length;
+        char *buffer = nullptr;
+        ssize_t length = 0;
         if (PYBIND11_BYTES_AS_STRING_AND_SIZE(m_ptr, &buffer, &length))
             pybind11_fail("Unable to extract bytes contents!");
         return std::string(buffer, (size_t) length);
     }
+
+#ifdef PYBIND11_HAS_STRING_VIEW
+    // enable_if is needed to avoid "ambiguous conversion" errors (see PR #3521).
+    template <typename T, detail::enable_if_t<std::is_same<T, std::string_view>::value, int> = 0>
+    // NOLINTNEXTLINE(google-explicit-constructor)
+    bytes(T s) : bytes(s.data(), s.size()) { }
+
+    // Obtain a string view that views the current `bytes` buffer value.  Note that this is only
+    // valid so long as the `bytes` instance remains alive and so generally should not outlive the
+    // lifetime of the `bytes` instance.
+    // NOLINTNEXTLINE(google-explicit-constructor)
+    operator std::string_view() const {
+        char *buffer = nullptr;
+        ssize_t length = 0;
+        if (PYBIND11_BYTES_AS_STRING_AND_SIZE(m_ptr, &buffer, &length))
+            pybind11_fail("Unable to extract bytes contents!");
+        return {buffer, static_cast<size_t>(length)};
+    }
+#endif
+
 };
 // Note: breathe >= 4.17.0 will fail to build docs if the below two constructors
 // are included in the doxygen group; close here and reopen after as a workaround
 /// @} pytypes
 
 inline bytes::bytes(const pybind11::str &s) {
     object temp = s;
     if (PyUnicode_Check(s.ptr())) {
         temp = reinterpret_steal<object>(PyUnicode_AsUTF8String(s.ptr()));
         if (!temp)
             pybind11_fail("Unable to extract string contents! (encoding issue)");
     }
-    char *buffer;
-    ssize_t length;
+    char *buffer = nullptr;
+    ssize_t length = 0;
     if (PYBIND11_BYTES_AS_STRING_AND_SIZE(temp.ptr(), &buffer, &length))
         pybind11_fail("Unable to extract string contents! (invalid type)");
     auto obj = reinterpret_steal<object>(PYBIND11_BYTES_FROM_STRING_AND_SIZE(buffer, length));
     if (!obj)
         pybind11_fail("Could not allocate bytes object!");
     m_ptr = obj.release().ptr();
 }
 
 inline str::str(const bytes& b) {
-    char *buffer;
-    ssize_t length;
+    char *buffer = nullptr;
+    ssize_t length = 0;
     if (PYBIND11_BYTES_AS_STRING_AND_SIZE(b.ptr(), &buffer, &length))
         pybind11_fail("Unable to extract bytes contents!");
-    auto obj = reinterpret_steal<object>(PyUnicode_FromStringAndSize(buffer, (ssize_t) length));
+    auto obj = reinterpret_steal<object>(PyUnicode_FromStringAndSize(buffer, length));
     if (!obj)
         pybind11_fail("Could not allocate string object!");
     m_ptr = obj.release().ptr();
 }
 
 /// \addtogroup pytypes
 /// @{
+class bytearray : public object {
+public:
+    PYBIND11_OBJECT_CVT(bytearray, object, PyByteArray_Check, PyByteArray_FromObject)
+
+    template <typename SzType, detail::enable_if_t<std::is_integral<SzType>::value, int> = 0>
+    bytearray(const char *c, const SzType &n)
+        : object(PyByteArray_FromStringAndSize(c, ssize_t_cast(n)), stolen_t{}) {
+        if (!m_ptr) pybind11_fail("Could not allocate bytearray object!");
+    }
+
+    bytearray()
+        : bytearray("", 0) {}
+
+    explicit bytearray(const std::string &s) : bytearray(s.data(), s.size()) { }
+
+    size_t size() const { return static_cast<size_t>(PyByteArray_Size(m_ptr)); }
+
+    explicit operator std::string() const {
+        char *buffer = PyByteArray_AS_STRING(m_ptr);
+        ssize_t size = PyByteArray_GET_SIZE(m_ptr);
+        return std::string(buffer, static_cast<size_t>(size));
+    }
+};
+// Note: breathe >= 4.17.0 will fail to build docs if the below two constructors
+// are included in the doxygen group; close here and reopen after as a workaround
+/// @} pytypes
+
+/// \addtogroup pytypes
+/// @{
 class none : public object {
 public:
     PYBIND11_OBJECT(none, object, detail::PyNone_Check)
     none() : object(Py_None, borrowed_t{}) { }
 };
 
 class ellipsis : public object {
@@ -1074,57 +1282,58 @@
 };
 
 class bool_ : public object {
 public:
     PYBIND11_OBJECT_CVT(bool_, object, PyBool_Check, raw_bool)
     bool_() : object(Py_False, borrowed_t{}) { }
     // Allow implicit conversion from and to `bool`:
+    // NOLINTNEXTLINE(google-explicit-constructor)
     bool_(bool value) : object(value ? Py_True : Py_False, borrowed_t{}) { }
-    operator bool() const { return m_ptr && PyLong_AsLong(m_ptr) != 0; }
+    // NOLINTNEXTLINE(google-explicit-constructor)
+    operator bool() const { return (m_ptr != nullptr) && PyLong_AsLong(m_ptr) != 0; }
 
 private:
     /// Return the truth value of an object -- always returns a new reference
     static PyObject *raw_bool(PyObject *op) {
         const auto value = PyObject_IsTrue(op);
         if (value == -1) return nullptr;
-        return handle(value ? Py_True : Py_False).inc_ref().ptr();
+        return handle(value != 0 ? Py_True : Py_False).inc_ref().ptr();
     }
 };
 
 PYBIND11_NAMESPACE_BEGIN(detail)
 // Converts a value to the given unsigned type.  If an error occurs, you get back (Unsigned) -1;
 // otherwise you get back the unsigned long or unsigned long long value cast to (Unsigned).
 // (The distinction is critically important when casting a returned -1 error value to some other
 // unsigned type: (A)-1 != (B)-1 when A and B are unsigned types of different sizes).
 template <typename Unsigned>
 Unsigned as_unsigned(PyObject *o) {
-    if (sizeof(Unsigned) <= sizeof(unsigned long)
+    if (PYBIND11_SILENCE_MSVC_C4127(sizeof(Unsigned) <= sizeof(unsigned long))
 #if PY_VERSION_HEX < 0x03000000
-            || PyInt_Check(o)
+        || PyInt_Check(o)
 #endif
     ) {
         unsigned long v = PyLong_AsUnsignedLong(o);
         return v == (unsigned long) -1 && PyErr_Occurred() ? (Unsigned) -1 : (Unsigned) v;
     }
-    else {
-        unsigned long long v = PyLong_AsUnsignedLongLong(o);
-        return v == (unsigned long long) -1 && PyErr_Occurred() ? (Unsigned) -1 : (Unsigned) v;
-    }
+    unsigned long long v = PyLong_AsUnsignedLongLong(o);
+    return v == (unsigned long long) -1 && PyErr_Occurred() ? (Unsigned) -1 : (Unsigned) v;
 }
 PYBIND11_NAMESPACE_END(detail)
 
 class int_ : public object {
 public:
     PYBIND11_OBJECT_CVT(int_, object, PYBIND11_LONG_CHECK, PyNumber_Long)
     int_() : object(PyLong_FromLong(0), stolen_t{}) { }
     // Allow implicit conversion from C++ integral types:
     template <typename T,
               detail::enable_if_t<std::is_integral<T>::value, int> = 0>
+    // NOLINTNEXTLINE(google-explicit-constructor)
     int_(T value) {
-        if (sizeof(T) <= sizeof(long)) {
+        if (PYBIND11_SILENCE_MSVC_C4127(sizeof(T) <= sizeof(long))) {
             if (std::is_signed<T>::value)
                 m_ptr = PyLong_FromLong((long) value);
             else
                 m_ptr = PyLong_FromUnsignedLong((unsigned long) value);
         } else {
             if (std::is_signed<T>::value)
                 m_ptr = PyLong_FromLongLong((long long) value);
@@ -1132,68 +1341,93 @@
                 m_ptr = PyLong_FromUnsignedLongLong((unsigned long long) value);
         }
         if (!m_ptr) pybind11_fail("Could not allocate int object!");
     }
 
     template <typename T,
               detail::enable_if_t<std::is_integral<T>::value, int> = 0>
+    // NOLINTNEXTLINE(google-explicit-constructor)
     operator T() const {
         return std::is_unsigned<T>::value
             ? detail::as_unsigned<T>(m_ptr)
             : sizeof(T) <= sizeof(long)
               ? (T) PyLong_AsLong(m_ptr)
               : (T) PYBIND11_LONG_AS_LONGLONG(m_ptr);
     }
 };
 
 class float_ : public object {
 public:
     PYBIND11_OBJECT_CVT(float_, object, PyFloat_Check, PyNumber_Float)
     // Allow implicit conversion from float/double:
+    // NOLINTNEXTLINE(google-explicit-constructor)
     float_(float value) : object(PyFloat_FromDouble((double) value), stolen_t{}) {
         if (!m_ptr) pybind11_fail("Could not allocate float object!");
     }
+    // NOLINTNEXTLINE(google-explicit-constructor)
     float_(double value = .0) : object(PyFloat_FromDouble((double) value), stolen_t{}) {
         if (!m_ptr) pybind11_fail("Could not allocate float object!");
     }
+    // NOLINTNEXTLINE(google-explicit-constructor)
     operator float() const { return (float) PyFloat_AsDouble(m_ptr); }
+    // NOLINTNEXTLINE(google-explicit-constructor)
     operator double() const { return (double) PyFloat_AsDouble(m_ptr); }
 };
 
 class weakref : public object {
 public:
-    PYBIND11_OBJECT_DEFAULT(weakref, object, PyWeakref_Check)
+    PYBIND11_OBJECT_CVT_DEFAULT(weakref, object, PyWeakref_Check, raw_weakref)
     explicit weakref(handle obj, handle callback = {})
         : object(PyWeakref_NewRef(obj.ptr(), callback.ptr()), stolen_t{}) {
         if (!m_ptr) pybind11_fail("Could not allocate weak reference!");
     }
+
+private:
+    static PyObject *raw_weakref(PyObject *o) {
+        return PyWeakref_NewRef(o, nullptr);
+    }
 };
 
 class slice : public object {
 public:
     PYBIND11_OBJECT_DEFAULT(slice, object, PySlice_Check)
-    slice(ssize_t start_, ssize_t stop_, ssize_t step_) {
-        int_ start(start_), stop(stop_), step(step_);
+    slice(handle start, handle stop, handle step) {
         m_ptr = PySlice_New(start.ptr(), stop.ptr(), step.ptr());
-        if (!m_ptr) pybind11_fail("Could not allocate slice object!");
+        if (!m_ptr)
+            pybind11_fail("Could not allocate slice object!");
     }
+
+#ifdef PYBIND11_HAS_OPTIONAL
+    slice(std::optional<ssize_t> start, std::optional<ssize_t> stop, std::optional<ssize_t> step)
+        : slice(index_to_object(start), index_to_object(stop), index_to_object(step)) {}
+#else
+    slice(ssize_t start_, ssize_t stop_, ssize_t step_)
+        : slice(int_(start_), int_(stop_), int_(step_)) {}
+#endif
+
     bool compute(size_t length, size_t *start, size_t *stop, size_t *step,
                  size_t *slicelength) const {
         return PySlice_GetIndicesEx((PYBIND11_SLICE_OBJECT *) m_ptr,
                                     (ssize_t) length, (ssize_t *) start,
                                     (ssize_t *) stop, (ssize_t *) step,
                                     (ssize_t *) slicelength) == 0;
     }
     bool compute(ssize_t length, ssize_t *start, ssize_t *stop, ssize_t *step,
       ssize_t *slicelength) const {
       return PySlice_GetIndicesEx((PYBIND11_SLICE_OBJECT *) m_ptr,
           length, start,
           stop, step,
           slicelength) == 0;
     }
+
+private:
+    template <typename T>
+    static object index_to_object(T index) {
+        return index ? object(int_(*index)) : object(none());
+    }
 };
 
 class capsule : public object {
 public:
     PYBIND11_OBJECT_DEFAULT(capsule, object, PyCapsule_CheckExact)
     PYBIND11_DEPRECATED("Use reinterpret_borrow<capsule>() or reinterpret_steal<capsule>()")
     capsule(PyObject *ptr, bool is_borrowed) : object(is_borrowed ? object(ptr, borrowed_t{}) : object(ptr, stolen_t{})) { }
@@ -1221,50 +1455,59 @@
         if (!m_ptr)
             pybind11_fail("Could not allocate capsule object!");
 
         if (PyCapsule_SetContext(m_ptr, (void *) destructor) != 0)
             pybind11_fail("Could not set capsule context!");
     }
 
-    capsule(void (*destructor)()) {
+    explicit capsule(void (*destructor)()) {
         m_ptr = PyCapsule_New(reinterpret_cast<void *>(destructor), nullptr, [](PyObject *o) {
             auto destructor = reinterpret_cast<void (*)()>(PyCapsule_GetPointer(o, nullptr));
             destructor();
         });
 
         if (!m_ptr)
             pybind11_fail("Could not allocate capsule object!");
     }
 
+    // NOLINTNEXTLINE(google-explicit-constructor)
     template <typename T> operator T *() const {
         return get_pointer<T>();
     }
 
     /// Get the pointer the capsule holds.
     template<typename T = void>
     T* get_pointer() const {
         auto name = this->name();
         T *result = static_cast<T *>(PyCapsule_GetPointer(m_ptr, name));
-        if (!result) pybind11_fail("Unable to extract capsule contents!");
+        if (!result) {
+            PyErr_Clear();
+            pybind11_fail("Unable to extract capsule contents!");
+        }
         return result;
     }
 
     /// Replaces a capsule's pointer *without* calling the destructor on the existing one.
     void set_pointer(const void *value) {
-        if (PyCapsule_SetPointer(m_ptr, const_cast<void *>(value)) != 0)
+        if (PyCapsule_SetPointer(m_ptr, const_cast<void *>(value)) != 0) {
+            PyErr_Clear();
             pybind11_fail("Could not set capsule pointer");
+        }
     }
 
     const char *name() const { return PyCapsule_GetName(m_ptr); }
 };
 
 class tuple : public object {
 public:
     PYBIND11_OBJECT_CVT(tuple, object, PyTuple_Check, PySequence_Tuple)
-    explicit tuple(size_t size = 0) : object(PyTuple_New((ssize_t) size), stolen_t{}) {
+    template <typename SzType = ssize_t,
+              detail::enable_if_t<std::is_integral<SzType>::value, int> = 0>
+    // Some compilers generate link errors when using `const SzType &` here:
+    explicit tuple(SzType size = 0) : object(PyTuple_New(ssize_t_cast(size)), stolen_t{}) {
         if (!m_ptr) pybind11_fail("Could not allocate tuple object!");
     }
     size_t size() const { return (size_t) PyTuple_Size(m_ptr); }
     bool empty() const { return size() == 0; }
     detail::tuple_accessor operator[](size_t index) const { return {*this, index}; }
     detail::item_accessor operator[](handle h) const { return object::operator[](h); }
     detail::tuple_iterator begin() const { return {*this, 0}; }
@@ -1292,15 +1535,15 @@
               typename collector = detail::deferred_t<detail::unpacking_collector<>, Args...>>
     explicit dict(Args &&...args) : dict(collector(std::forward<Args>(args)...).kwargs()) { }
 
     size_t size() const { return (size_t) PyDict_Size(m_ptr); }
     bool empty() const { return size() == 0; }
     detail::dict_iterator begin() const { return {*this, 0}; }
     detail::dict_iterator end() const { return {}; }
-    void clear() const { PyDict_Clear(ptr()); }
+    void clear() /* py-non-const */ { PyDict_Clear(ptr()); }
     template <typename T> bool contains(T &&key) const {
         return PyDict_Contains(m_ptr, detail::object_or_cast(std::forward<T>(key)).ptr()) == 1;
     }
 
 private:
     /// Call the `dict` Python type -- always returns a new reference
     static PyObject *raw_dict(PyObject *op) {
@@ -1325,47 +1568,53 @@
     detail::sequence_iterator begin() const { return {*this, 0}; }
     detail::sequence_iterator end() const { return {*this, PySequence_Size(m_ptr)}; }
 };
 
 class list : public object {
 public:
     PYBIND11_OBJECT_CVT(list, object, PyList_Check, PySequence_List)
-    explicit list(size_t size = 0) : object(PyList_New((ssize_t) size), stolen_t{}) {
+    template <typename SzType = ssize_t,
+              detail::enable_if_t<std::is_integral<SzType>::value, int> = 0>
+    // Some compilers generate link errors when using `const SzType &` here:
+    explicit list(SzType size = 0) : object(PyList_New(ssize_t_cast(size)), stolen_t{}) {
         if (!m_ptr) pybind11_fail("Could not allocate list object!");
     }
     size_t size() const { return (size_t) PyList_Size(m_ptr); }
     bool empty() const { return size() == 0; }
     detail::list_accessor operator[](size_t index) const { return {*this, index}; }
     detail::item_accessor operator[](handle h) const { return object::operator[](h); }
     detail::list_iterator begin() const { return {*this, 0}; }
     detail::list_iterator end() const { return {*this, PyList_GET_SIZE(m_ptr)}; }
-    template <typename T> void append(T &&val) const {
+    template <typename T> void append(T &&val) /* py-non-const */ {
         PyList_Append(m_ptr, detail::object_or_cast(std::forward<T>(val)).ptr());
     }
-    template <typename T> void insert(size_t index, T &&val) const {
-        PyList_Insert(m_ptr, static_cast<ssize_t>(index),
-            detail::object_or_cast(std::forward<T>(val)).ptr());
+    template <typename IdxType,
+              typename ValType,
+              detail::enable_if_t<std::is_integral<IdxType>::value, int> = 0>
+    void insert(const IdxType &index, ValType &&val) /* py-non-const */ {
+        PyList_Insert(
+            m_ptr, ssize_t_cast(index), detail::object_or_cast(std::forward<ValType>(val)).ptr());
     }
 };
 
 class args : public tuple { PYBIND11_OBJECT_DEFAULT(args, tuple, PyTuple_Check) };
 class kwargs : public dict { PYBIND11_OBJECT_DEFAULT(kwargs, dict, PyDict_Check)  };
 
 class set : public object {
 public:
     PYBIND11_OBJECT_CVT(set, object, PySet_Check, PySet_New)
     set() : object(PySet_New(nullptr), stolen_t{}) {
         if (!m_ptr) pybind11_fail("Could not allocate set object!");
     }
     size_t size() const { return (size_t) PySet_Size(m_ptr); }
     bool empty() const { return size() == 0; }
-    template <typename T> bool add(T &&val) const {
+    template <typename T> bool add(T &&val) /* py-non-const */ {
         return PySet_Add(m_ptr, detail::object_or_cast(std::forward<T>(val)).ptr()) == 0;
     }
-    void clear() const { PySet_Clear(m_ptr); }
+    void clear() /* py-non-const */ { PySet_Clear(m_ptr); }
     template <typename T> bool contains(T &&val) const {
         return PySet_Contains(m_ptr, detail::object_or_cast(std::forward<T>(val)).ptr()) == 1;
     }
 };
 
 class function : public object {
 public:
@@ -1453,15 +1702,15 @@
         detail::any_container<ssize_t> strides, bool readonly = false);
 
     static memoryview from_buffer(
         const void *ptr, ssize_t itemsize, const char *format,
         detail::any_container<ssize_t> shape,
         detail::any_container<ssize_t> strides) {
         return memoryview::from_buffer(
-            const_cast<void*>(ptr), itemsize, format, shape, strides, true);
+            const_cast<void *>(ptr), itemsize, format, std::move(shape), std::move(strides), true);
     }
 
     template<typename T>
     static memoryview from_buffer(
         T *ptr, detail::any_container<ssize_t> shape,
         detail::any_container<ssize_t> strides, bool readonly = false) {
         return memoryview::from_buffer(
@@ -1499,26 +1748,33 @@
             pybind11_fail("Could not allocate memoryview object!");
         return memoryview(object(ptr, stolen_t{}));
     }
 
     static memoryview from_memory(const void *mem, ssize_t size) {
         return memoryview::from_memory(const_cast<void*>(mem), size, true);
     }
+
+#ifdef PYBIND11_HAS_STRING_VIEW
+    static memoryview from_memory(std::string_view mem) {
+        return from_memory(const_cast<char*>(mem.data()), static_cast<ssize_t>(mem.size()), true);
+    }
+#endif
+
 #endif
 };
 
-#ifndef DOXYGEN_SHOULD_SKIP_THIS
+/// @cond DUPLICATE
 inline memoryview memoryview::from_buffer(
     void *ptr, ssize_t itemsize, const char* format,
     detail::any_container<ssize_t> shape,
     detail::any_container<ssize_t> strides, bool readonly) {
     size_t ndim = shape->size();
     if (ndim != strides->size())
         pybind11_fail("memoryview: shape length doesn't match strides length");
-    ssize_t size = ndim ? 1 : 0;
+    ssize_t size = ndim != 0u ? 1 : 0;
     for (size_t i = 0; i < ndim; ++i)
         size *= (*shape)[i];
     Py_buffer view;
     view.buf = ptr;
     view.obj = nullptr;
     view.len = size * itemsize;
     view.readonly = static_cast<int>(readonly);
@@ -1530,15 +1786,15 @@
     view.suboffsets = nullptr;
     view.internal = nullptr;
     PyObject* obj = PyMemoryView_FromBuffer(&view);
     if (!obj)
         throw error_already_set();
     return memoryview(object(obj, stolen_t{}));
 }
-#endif  // DOXYGEN_SHOULD_SKIP_THIS
+/// @endcond
 /// @} pytypes
 
 /// \addtogroup python_builtins
 /// @{
 
 /// Get the length of a Python object.
 inline size_t len(handle h) {
```

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/stl.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/stl.h`

 * *Files 8% similar despite different names*

```diff
@@ -5,51 +5,34 @@
 
     All rights reserved. Use of this source code is governed by a
     BSD-style license that can be found in the LICENSE file.
 */
 
 #pragma once
 
+#include "detail/common.h"
 #include "pybind11.h"
 #include <set>
 #include <unordered_set>
 #include <map>
 #include <unordered_map>
 #include <iostream>
 #include <list>
 #include <deque>
 #include <valarray>
 
-#if defined(_MSC_VER)
-#pragma warning(push)
-#pragma warning(disable: 4127) // warning C4127: Conditional expression is constant
+// See `detail/common.h` for implementation of these guards.
+#if defined(PYBIND11_HAS_OPTIONAL)
+#  include <optional>
+#elif defined(PYBIND11_HAS_EXP_OPTIONAL)
+#  include <experimental/optional>
 #endif
 
-#ifdef __has_include
-// std::optional (but including it in c++14 mode isn't allowed)
-#  if defined(PYBIND11_CPP17) && __has_include(<optional>)
-#    include <optional>
-#    define PYBIND11_HAS_OPTIONAL 1
-#  endif
-// std::experimental::optional (but not allowed in c++11 mode)
-#  if defined(PYBIND11_CPP14) && (__has_include(<experimental/optional>) && \
-                                 !__has_include(<optional>))
-#    include <experimental/optional>
-#    define PYBIND11_HAS_EXP_OPTIONAL 1
-#  endif
-// std::variant
-#  if defined(PYBIND11_CPP17) && __has_include(<variant>)
-#    include <variant>
-#    define PYBIND11_HAS_VARIANT 1
-#  endif
-#elif defined(_MSC_VER) && defined(PYBIND11_CPP17)
-#  include <optional>
+#if defined(PYBIND11_HAS_VARIANT)
 #  include <variant>
-#  define PYBIND11_HAS_OPTIONAL 1
-#  define PYBIND11_HAS_VARIANT 1
 #endif
 
 PYBIND11_NAMESPACE_BEGIN(PYBIND11_NAMESPACE)
 PYBIND11_NAMESPACE_BEGIN(detail)
 
 /// Extracts an const lvalue reference or rvalue reference for U based on the type of T (e.g. for
 /// forwarding a container element).  Typically used indirect via forwarded_type(), below.
@@ -91,15 +74,15 @@
             auto value_ = reinterpret_steal<object>(key_conv::cast(forward_like<T>(value), policy, parent));
             if (!value_ || !s.add(value_))
                 return handle();
         }
         return s.release();
     }
 
-    PYBIND11_TYPE_CASTER(type, _("Set[") + key_conv::name + _("]"));
+    PYBIND11_TYPE_CASTER(type, const_name("Set[") + key_conv::name + const_name("]"));
 };
 
 template <typename Type, typename Key, typename Value> struct map_caster {
     using key_conv   = make_caster<Key>;
     using value_conv = make_caster<Value>;
 
     bool load(handle src, bool convert) {
@@ -133,58 +116,61 @@
             if (!key || !value)
                 return handle();
             d[key] = value;
         }
         return d.release();
     }
 
-    PYBIND11_TYPE_CASTER(Type, _("Dict[") + key_conv::name + _(", ") + value_conv::name + _("]"));
+    PYBIND11_TYPE_CASTER(Type, const_name("Dict[") + key_conv::name + const_name(", ") + value_conv::name + const_name("]"));
 };
 
 template <typename Type, typename Value> struct list_caster {
     using value_conv = make_caster<Value>;
 
     bool load(handle src, bool convert) {
-        if (!isinstance<sequence>(src) || isinstance<str>(src))
+        if (!isinstance<sequence>(src) || isinstance<bytes>(src) || isinstance<str>(src))
             return false;
         auto s = reinterpret_borrow<sequence>(src);
         value.clear();
         reserve_maybe(s, &value);
         for (auto it : s) {
             value_conv conv;
             if (!conv.load(it, convert))
                 return false;
             value.push_back(cast_op<Value &&>(std::move(conv)));
         }
         return true;
     }
 
 private:
-    template <typename T = Type,
-              enable_if_t<std::is_same<decltype(std::declval<T>().reserve(0)), void>::value, int> = 0>
-    void reserve_maybe(sequence s, Type *) { value.reserve(s.size()); }
-    void reserve_maybe(sequence, void *) { }
+    template <
+        typename T                                                                          = Type,
+        enable_if_t<std::is_same<decltype(std::declval<T>().reserve(0)), void>::value, int> = 0>
+    void reserve_maybe(const sequence &s, Type *) {
+        value.reserve(s.size());
+    }
+    void reserve_maybe(const sequence &, void *) {}
 
 public:
     template <typename T>
     static handle cast(T &&src, return_value_policy policy, handle parent) {
         if (!std::is_lvalue_reference<T>::value)
             policy = return_value_policy_override<Value>::policy(policy);
         list l(src.size());
-        size_t index = 0;
+        ssize_t index = 0;
         for (auto &&value : src) {
             auto value_ = reinterpret_steal<object>(value_conv::cast(forward_like<T>(value), policy, parent));
             if (!value_)
                 return handle();
-            PyList_SET_ITEM(l.ptr(), (ssize_t) index++, value_.release().ptr()); // steals a reference
+            PyList_SET_ITEM(l.ptr(), index++, value_.release().ptr()); // steals a reference
         }
         return l.release();
     }
 
-    PYBIND11_TYPE_CASTER(Type, _("List[") + value_conv::name + _("]"));
+    PYBIND11_TYPE_CASTER(Type, const_name("List[") + value_conv::name + const_name("]"));
 };
 
 template <typename Type, typename Alloc> struct type_caster<std::vector<Type, Alloc>>
  : list_caster<std::vector<Type, Alloc>, Type> { };
 
 template <typename Type, typename Alloc> struct type_caster<std::deque<Type, Alloc>>
  : list_caster<std::deque<Type, Alloc>, Type> { };
@@ -223,25 +209,25 @@
         }
         return true;
     }
 
     template <typename T>
     static handle cast(T &&src, return_value_policy policy, handle parent) {
         list l(src.size());
-        size_t index = 0;
+        ssize_t index = 0;
         for (auto &&value : src) {
             auto value_ = reinterpret_steal<object>(value_conv::cast(forward_like<T>(value), policy, parent));
             if (!value_)
                 return handle();
-            PyList_SET_ITEM(l.ptr(), (ssize_t) index++, value_.release().ptr()); // steals a reference
+            PyList_SET_ITEM(l.ptr(), index++, value_.release().ptr()); // steals a reference
         }
         return l.release();
     }
 
-    PYBIND11_TYPE_CASTER(ArrayType, _("List[") + value_conv::name + _<Resizable>(_(""), _("[") + _<Size>() + _("]")) + _("]"));
+    PYBIND11_TYPE_CASTER(ArrayType, const_name("List[") + value_conv::name + const_name<Resizable>(const_name(""), const_name("[") + const_name<Size>() + const_name("]")) + const_name("]"));
 };
 
 template <typename Type, size_t Size> struct type_caster<std::array<Type, Size>>
  : array_caster<std::array<Type, Size>, Type, false, Size> { };
 
 template <typename Type> struct type_caster<std::valarray<Type>>
  : array_caster<std::valarray<Type>, Type, true> { };
@@ -255,42 +241,43 @@
 template <typename Key, typename Value, typename Compare, typename Alloc> struct type_caster<std::map<Key, Value, Compare, Alloc>>
   : map_caster<std::map<Key, Value, Compare, Alloc>, Key, Value> { };
 
 template <typename Key, typename Value, typename Hash, typename Equal, typename Alloc> struct type_caster<std::unordered_map<Key, Value, Hash, Equal, Alloc>>
   : map_caster<std::unordered_map<Key, Value, Hash, Equal, Alloc>, Key, Value> { };
 
 // This type caster is intended to be used for std::optional and std::experimental::optional
-template<typename T> struct optional_caster {
-    using value_conv = make_caster<typename T::value_type>;
+template<typename Type, typename Value = typename Type::value_type> struct optional_caster {
+    using value_conv = make_caster<Value>;
 
-    template <typename T_>
-    static handle cast(T_ &&src, return_value_policy policy, handle parent) {
+    template <typename T>
+    static handle cast(T &&src, return_value_policy policy, handle parent) {
         if (!src)
             return none().inc_ref();
         if (!std::is_lvalue_reference<T>::value) {
-            policy = return_value_policy_override<T>::policy(policy);
+            policy = return_value_policy_override<Value>::policy(policy);
         }
-        return value_conv::cast(*std::forward<T_>(src), policy, parent);
+        return value_conv::cast(*std::forward<T>(src), policy, parent);
     }
 
     bool load(handle src, bool convert) {
         if (!src) {
             return false;
-        } else if (src.is_none()) {
+        }
+        if (src.is_none()) {
             return true;  // default-constructed value is already empty
         }
         value_conv inner_caster;
         if (!inner_caster.load(src, convert))
             return false;
 
-        value.emplace(cast_op<typename T::value_type &&>(std::move(inner_caster)));
+        value.emplace(cast_op<Value &&>(std::move(inner_caster)));
         return true;
     }
 
-    PYBIND11_TYPE_CASTER(T, _("Optional[") + value_conv::name + _("]"));
+    PYBIND11_TYPE_CASTER(Type, const_name("Optional[") + value_conv::name + const_name("]"));
 };
 
 #if defined(PYBIND11_HAS_OPTIONAL)
 template<typename T> struct type_caster<std::optional<T>>
     : public optional_caster<std::optional<T>> {};
 
 template<> struct type_caster<std::nullopt_t>
@@ -362,27 +349,27 @@
     template <typename Variant>
     static handle cast(Variant &&src, return_value_policy policy, handle parent) {
         return visit_helper<V>::call(variant_caster_visitor{policy, parent},
                                      std::forward<Variant>(src));
     }
 
     using Type = V<Ts...>;
-    PYBIND11_TYPE_CASTER(Type, _("Union[") + detail::concat(make_caster<Ts>::name...) + _("]"));
+    PYBIND11_TYPE_CASTER(Type, const_name("Union[") + detail::concat(make_caster<Ts>::name...) + const_name("]"));
 };
 
 #if defined(PYBIND11_HAS_VARIANT)
 template <typename... Ts>
 struct type_caster<std::variant<Ts...>> : variant_caster<std::variant<Ts...>> { };
 #endif
 
 PYBIND11_NAMESPACE_END(detail)
 
 inline std::ostream &operator<<(std::ostream &os, const handle &obj) {
+#ifdef PYBIND11_HAS_STRING_VIEW
+    os << str(obj).cast<std::string_view>();
+#else
     os << (std::string) str(obj);
+#endif
     return os;
 }
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
-
-#if defined(_MSC_VER)
-#pragma warning(pop)
-#endif
```

### Comparing `iminuit-2.8.4/extern/pybind11/include/pybind11/stl_bind.h` & `iminuit-2.9.0/extern/pybind11/include/pybind11/stl_bind.h`

 * *Files 12% similar despite different names*

```diff
@@ -124,19 +124,19 @@
     };
 
     cl.def("append",
            [](Vector &v, const T &value) { v.push_back(value); },
            arg("x"),
            "Add an item to the end of the list");
 
-    cl.def(init([](iterable it) {
+    cl.def(init([](const iterable &it) {
         auto v = std::unique_ptr<Vector>(new Vector());
         v->reserve(len_hint(it));
         for (handle h : it)
-           v->push_back(h.cast<T>());
+            v->push_back(h.cast<T>());
         return v.release();
     }));
 
     cl.def("clear",
         [](Vector &v) {
             v.clear();
         },
@@ -147,35 +147,36 @@
        [](Vector &v, const Vector &src) {
            v.insert(v.end(), src.begin(), src.end());
        },
        arg("L"),
        "Extend the list by appending all the items in the given list"
     );
 
-    cl.def("extend",
-       [](Vector &v, iterable it) {
-           const size_t old_size = v.size();
-           v.reserve(old_size + len_hint(it));
-           try {
-               for (handle h : it) {
-                   v.push_back(h.cast<T>());
-               }
-           } catch (const cast_error &) {
-               v.erase(v.begin() + static_cast<typename Vector::difference_type>(old_size), v.end());
-               try {
-                   v.shrink_to_fit();
-               } catch (const std::exception &) {
-                   // Do nothing
-               }
-               throw;
-           }
-       },
-       arg("L"),
-       "Extend the list by appending all the items in the given list"
-    );
+    cl.def(
+        "extend",
+        [](Vector &v, const iterable &it) {
+            const size_t old_size = v.size();
+            v.reserve(old_size + len_hint(it));
+            try {
+                for (handle h : it) {
+                    v.push_back(h.cast<T>());
+                }
+            } catch (const cast_error &) {
+                v.erase(v.begin() + static_cast<typename Vector::difference_type>(old_size),
+                        v.end());
+                try {
+                    v.shrink_to_fit();
+                } catch (const std::exception &) {
+                    // Do nothing
+                }
+                throw;
+            }
+        },
+        arg("L"),
+        "Extend the list by appending all the items in the given list");
 
     cl.def("insert",
         [](Vector &v, DiffType i, const T &x) {
             // Can't use wrap_i; i == v.size() is OK
             if (i < 0)
                 i += v.size();
             if (i < 0 || (SizeType)i > v.size())
@@ -186,104 +187,103 @@
         "Insert an item at a given position."
     );
 
     cl.def("pop",
         [](Vector &v) {
             if (v.empty())
                 throw index_error();
-            T t = v.back();
+            T t = std::move(v.back());
             v.pop_back();
             return t;
         },
         "Remove and return the last item"
     );
 
     cl.def("pop",
         [wrap_i](Vector &v, DiffType i) {
             i = wrap_i(i, v.size());
-            T t = v[(SizeType) i];
-            v.erase(v.begin() + i);
+            T t = std::move(v[(SizeType) i]);
+            v.erase(std::next(v.begin(), i));
             return t;
         },
         arg("i"),
         "Remove and return the item at index ``i``"
     );
 
     cl.def("__setitem__",
         [wrap_i](Vector &v, DiffType i, const T &t) {
             i = wrap_i(i, v.size());
             v[(SizeType)i] = t;
         }
     );
 
     /// Slicing protocol
-    cl.def("__getitem__",
+    cl.def(
+        "__getitem__",
         [](const Vector &v, slice slice) -> Vector * {
-            size_t start, stop, step, slicelength;
+            size_t start = 0, stop = 0, step = 0, slicelength = 0;
 
             if (!slice.compute(v.size(), &start, &stop, &step, &slicelength))
                 throw error_already_set();
 
             auto *seq = new Vector();
             seq->reserve((size_t) slicelength);
 
             for (size_t i=0; i<slicelength; ++i) {
                 seq->push_back(v[start]);
                 start += step;
             }
             return seq;
         },
         arg("s"),
-        "Retrieve list elements using a slice object"
-    );
+        "Retrieve list elements using a slice object");
 
-    cl.def("__setitem__",
-        [](Vector &v, slice slice,  const Vector &value) {
-            size_t start, stop, step, slicelength;
+    cl.def(
+        "__setitem__",
+        [](Vector &v, slice slice, const Vector &value) {
+            size_t start = 0, stop = 0, step = 0, slicelength = 0;
             if (!slice.compute(v.size(), &start, &stop, &step, &slicelength))
                 throw error_already_set();
 
             if (slicelength != value.size())
                 throw std::runtime_error("Left and right hand size of slice assignment have different sizes!");
 
             for (size_t i=0; i<slicelength; ++i) {
                 v[start] = value[i];
                 start += step;
             }
         },
-        "Assign list elements using a slice object"
-    );
+        "Assign list elements using a slice object");
 
     cl.def("__delitem__",
         [wrap_i](Vector &v, DiffType i) {
             i = wrap_i(i, v.size());
             v.erase(v.begin() + i);
         },
         "Delete the list elements at index ``i``"
     );
 
-    cl.def("__delitem__",
+    cl.def(
+        "__delitem__",
         [](Vector &v, slice slice) {
-            size_t start, stop, step, slicelength;
+            size_t start = 0, stop = 0, step = 0, slicelength = 0;
 
             if (!slice.compute(v.size(), &start, &stop, &step, &slicelength))
                 throw error_already_set();
 
             if (step == 1 && false) {
                 v.erase(v.begin() + (DiffType) start, v.begin() + DiffType(start + slicelength));
             } else {
                 for (size_t i = 0; i < slicelength; ++i) {
                     v.erase(v.begin() + DiffType(start));
                     start += step - 1;
                 }
             }
         },
-        "Delete list elements using a slice object"
-    );
-
+        "Delete list elements using a slice object");
 }
 
 // If the type has an operator[] that doesn't return a reference (most notably std::vector<bool>),
 // we have to access by copying; otherwise we return by reference.
 template <typename Vector> using vector_needs_copy = negation<
     std::is_same<decltype(std::declval<Vector>()[typename Vector::size_type()]), typename Vector::value_type &>>;
 
@@ -396,34 +396,33 @@
     // numpy.h declares this for arbitrary types, but it may raise an exception and crash hard at runtime if PYBIND11_NUMPY_DTYPE hasn't been called, so check here
     format_descriptor<T>::format();
 
     cl.def_buffer([](Vector& v) -> buffer_info {
         return buffer_info(v.data(), static_cast<ssize_t>(sizeof(T)), format_descriptor<T>::format(), 1, {v.size()}, {sizeof(T)});
     });
 
-    cl.def(init([](buffer buf) {
+    cl.def(init([](const buffer &buf) {
         auto info = buf.request();
         if (info.ndim != 1 || info.strides[0] % static_cast<ssize_t>(sizeof(T)))
             throw type_error("Only valid 1D buffers can be copied to a vector");
         if (!detail::compare_buffer_info<T>::compare(info) || (ssize_t) sizeof(T) != info.itemsize)
             throw type_error("Format mismatch (Python: " + info.format + " C++: " + format_descriptor<T>::format() + ")");
 
         T *p = static_cast<T*>(info.ptr);
         ssize_t step = info.strides[0] / static_cast<ssize_t>(sizeof(T));
         T *end = p + info.shape[0] * step;
         if (step == 1) {
             return Vector(p, end);
         }
-        else {
-            Vector vec;
-            vec.reserve((size_t) info.shape[0]);
-            for (; p != end; p += step)
-                vec.push_back(*p);
-            return vec;
-        }
+        Vector vec;
+        vec.reserve((size_t) info.shape[0]);
+        for (; p != end; p += step)
+            vec.push_back(*p);
+        return vec;
+
     }));
 
     return;
 }
 
 template <typename Vector, typename Class_, typename... Args>
 void vector_buffer_impl(Class_&, std::false_type) {}
@@ -592,53 +591,89 @@
             s << '}';
             return s.str();
         },
         "Return the canonical string representation of this map."
     );
 }
 
+template<typename Map>
+struct keys_view
+{
+    Map &map;
+};
+
+template<typename Map>
+struct values_view
+{
+    Map &map;
+};
+
+template<typename Map>
+struct items_view
+{
+    Map &map;
+};
 
 PYBIND11_NAMESPACE_END(detail)
 
 template <typename Map, typename holder_type = std::unique_ptr<Map>, typename... Args>
 class_<Map, holder_type> bind_map(handle scope, const std::string &name, Args&&... args) {
     using KeyType = typename Map::key_type;
     using MappedType = typename Map::mapped_type;
+    using KeysView = detail::keys_view<Map>;
+    using ValuesView = detail::values_view<Map>;
+    using ItemsView = detail::items_view<Map>;
     using Class_ = class_<Map, holder_type>;
 
     // If either type is a non-module-local bound type then make the map binding non-local as well;
     // otherwise (e.g. both types are either module-local or converting) the map will be
     // module-local.
     auto tinfo = detail::get_type_info(typeid(MappedType));
     bool local = !tinfo || tinfo->module_local;
     if (local) {
         tinfo = detail::get_type_info(typeid(KeyType));
         local = !tinfo || tinfo->module_local;
     }
 
     Class_ cl(scope, name.c_str(), pybind11::module_local(local), std::forward<Args>(args)...);
+    class_<KeysView> keys_view(
+        scope, ("KeysView[" + name + "]").c_str(), pybind11::module_local(local));
+    class_<ValuesView> values_view(
+        scope, ("ValuesView[" + name + "]").c_str(), pybind11::module_local(local));
+    class_<ItemsView> items_view(
+        scope, ("ItemsView[" + name + "]").c_str(), pybind11::module_local(local));
 
     cl.def(init<>());
 
     // Register stream insertion operator (if possible)
     detail::map_if_insertion_operator<Map, Class_>(cl, name);
 
     cl.def("__bool__",
         [](const Map &m) -> bool { return !m.empty(); },
         "Check whether the map is nonempty"
     );
 
     cl.def("__iter__",
            [](Map &m) { return make_key_iterator(m.begin(), m.end()); },
-           keep_alive<0, 1>() /* Essential: keep list alive while iterator exists */
+           keep_alive<0, 1>() /* Essential: keep map alive while iterator exists */
+    );
+
+    cl.def("keys",
+           [](Map &m) { return KeysView{m}; },
+           keep_alive<0, 1>() /* Essential: keep map alive while view exists */
+    );
+
+    cl.def("values",
+           [](Map &m) { return ValuesView{m}; },
+           keep_alive<0, 1>() /* Essential: keep map alive while view exists */
     );
 
     cl.def("items",
-           [](Map &m) { return make_iterator(m.begin(), m.end()); },
-           keep_alive<0, 1>() /* Essential: keep list alive while iterator exists */
+           [](Map &m) { return ItemsView{m}; },
+           keep_alive<0, 1>() /* Essential: keep map alive while view exists */
     );
 
     cl.def("__getitem__",
         [](Map &m, const KeyType &k) -> MappedType & {
             auto it = m.find(k);
             if (it == m.end())
               throw key_error();
@@ -651,14 +686,16 @@
         [](Map &m, const KeyType &k) -> bool {
             auto it = m.find(k);
             if (it == m.end())
               return false;
            return true;
         }
     );
+    // Fallback for when the object is not of the key type
+    cl.def("__contains__", [](Map &, const object &) -> bool { return false; });
 
     // Assignment provided only if the type is copyable
     detail::map_assignment<Map, Class_>(cl);
 
     cl.def("__delitem__",
            [](Map &m, const KeyType &k) {
                auto it = m.find(k);
@@ -666,11 +703,45 @@
                    throw key_error();
                m.erase(it);
            }
     );
 
     cl.def("__len__", &Map::size);
 
+    keys_view.def("__len__", [](KeysView &view) { return view.map.size(); });
+    keys_view.def("__iter__",
+        [](KeysView &view) {
+            return make_key_iterator(view.map.begin(), view.map.end());
+        },
+        keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
+    );
+    keys_view.def("__contains__",
+        [](KeysView &view, const KeyType &k) -> bool {
+            auto it = view.map.find(k);
+            if (it == view.map.end())
+                return false;
+            return true;
+        }
+    );
+    // Fallback for when the object is not of the key type
+    keys_view.def("__contains__", [](KeysView &, const object &) -> bool { return false; });
+
+    values_view.def("__len__", [](ValuesView &view) { return view.map.size(); });
+    values_view.def("__iter__",
+        [](ValuesView &view) {
+            return make_value_iterator(view.map.begin(), view.map.end());
+        },
+        keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
+    );
+
+    items_view.def("__len__", [](ItemsView &view) { return view.map.size(); });
+    items_view.def("__iter__",
+        [](ItemsView &view) {
+            return make_iterator(view.map.begin(), view.map.end());
+        },
+        keep_alive<0, 1>() /* Essential: keep view alive while iterator exists */
+    );
+
     return cl;
 }
 
 PYBIND11_NAMESPACE_END(PYBIND11_NAMESPACE)
```

### Comparing `iminuit-2.8.4/extern/pybind11/tools/FindCatch.cmake` & `iminuit-2.9.0/extern/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/pybind11/tools/FindEigen3.cmake` & `iminuit-2.9.0/extern/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/pybind11/tools/FindPythonLibsNew.cmake` & `iminuit-2.9.0/extern/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/pybind11/tools/pybind11Common.cmake` & `iminuit-2.9.0/extern/pybind11/tools/pybind11Common.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
     pybind11_strip(target) - strip target after building on linux/macOS
     pybind11_find_import(module) - See if a module is installed.
 
 #]======================================================]
 
 # CMake 3.10 has an include_guard command, but we can't use that yet
+# include_guard(global) (pre-CMake 3.10)
 if(TARGET pybind11::lto)
   return()
 endif()
 
 # If we are in subdirectory mode, all IMPORTED targets must be GLOBAL. If we
 # are in CONFIG mode, they should be "normal" targets instead.
 # In CMake 3.11+ you can promote a target to global after you create it,
@@ -111,36 +112,40 @@
     PROPERTY INTERFACE_LINK_OPTIONS "$<$<PLATFORM_ID:Darwin>:LINKER:-undefined,dynamic_lookup>")
 endif()
 
 # ------------------------ Windows extras -------------------------
 
 add_library(pybind11::windows_extras IMPORTED INTERFACE ${optional_global})
 
-if(MSVC)
-  # /MP enables multithreaded builds (relevant when there are many files), /bigobj is
-  # needed for bigger binding projects due to the limit to 64k addressable sections
+if(MSVC) # That's also clang-cl
+  # /bigobj is needed for bigger binding projects due to the limit to 64k
+  # addressable sections
   set_property(
     TARGET pybind11::windows_extras
     APPEND
     PROPERTY INTERFACE_COMPILE_OPTIONS /bigobj)
 
-  if(CMAKE_VERSION VERSION_LESS 3.11)
-    set_property(
-      TARGET pybind11::windows_extras
-      APPEND
-      PROPERTY INTERFACE_COMPILE_OPTIONS $<$<NOT:$<CONFIG:Debug>>:/MP>)
-  else()
-    # Only set these options for C++ files.  This is important so that, for
-    # instance, projects that include other types of source files like CUDA
-    # .cu files don't get these options propagated to nvcc since that would
-    # cause the build to fail.
-    set_property(
-      TARGET pybind11::windows_extras
-      APPEND
-      PROPERTY INTERFACE_COMPILE_OPTIONS $<$<NOT:$<CONFIG:Debug>>:$<$<COMPILE_LANGUAGE:CXX>:/MP>>)
+  # /MP enables multithreaded builds (relevant when there are many files) for MSVC
+  if("${CMAKE_CXX_COMPILER_ID}" STREQUAL "MSVC") # no Clang no Intel
+    if(CMAKE_VERSION VERSION_LESS 3.11)
+      set_property(
+        TARGET pybind11::windows_extras
+        APPEND
+        PROPERTY INTERFACE_COMPILE_OPTIONS $<$<NOT:$<CONFIG:Debug>>:/MP>)
+    else()
+      # Only set these options for C++ files.  This is important so that, for
+      # instance, projects that include other types of source files like CUDA
+      # .cu files don't get these options propagated to nvcc since that would
+      # cause the build to fail.
+      set_property(
+        TARGET pybind11::windows_extras
+        APPEND
+        PROPERTY INTERFACE_COMPILE_OPTIONS
+                 $<$<NOT:$<CONFIG:Debug>>:$<$<COMPILE_LANGUAGE:CXX>:/MP>>)
+    endif()
   endif()
 endif()
 
 # ----------------------- Optimize binary size --------------------------
 
 add_library(pybind11::opt_size IMPORTED INTERFACE ${optional_global})
 
@@ -294,31 +299,44 @@
     set(${linkerflags_out}
         "${linkerflags}"
         PARENT_SCOPE)
   endif()
 endfunction()
 
 function(_pybind11_generate_lto target prefer_thin_lto)
+  if(MINGW)
+    message(STATUS "${target} disabled (problems with undefined symbols for MinGW for now)")
+    return()
+  endif()
+
   if(CMAKE_CXX_COMPILER_ID MATCHES "GNU|Clang")
     set(cxx_append "")
     set(linker_append "")
     if(CMAKE_CXX_COMPILER_ID MATCHES "Clang" AND NOT APPLE)
       # Clang Gold plugin does not support -Os; append -O3 to MinSizeRel builds to override it
       set(linker_append ";$<$<CONFIG:MinSizeRel>:-O3>")
-    elseif(CMAKE_CXX_COMPILER_ID MATCHES "GNU")
+    elseif(CMAKE_CXX_COMPILER_ID MATCHES "GNU" AND NOT MINGW)
       set(cxx_append ";-fno-fat-lto-objects")
     endif()
 
-    if(CMAKE_CXX_COMPILER_ID MATCHES "Clang" AND prefer_thin_lto)
+    if(CMAKE_SYSTEM_PROCESSOR MATCHES "ppc64le" OR CMAKE_SYSTEM_PROCESSOR MATCHES "mips64")
+      set(NO_FLTO_ARCH TRUE)
+    else()
+      set(NO_FLTO_ARCH FALSE)
+    endif()
+
+    if(CMAKE_CXX_COMPILER_ID MATCHES "Clang"
+       AND prefer_thin_lto
+       AND NOT NO_FLTO_ARCH)
       _pybind11_return_if_cxx_and_linker_flags_work(
         HAS_FLTO_THIN "-flto=thin${cxx_append}" "-flto=thin${linker_append}"
         PYBIND11_LTO_CXX_FLAGS PYBIND11_LTO_LINKER_FLAGS)
     endif()
 
-    if(NOT HAS_FLTO_THIN)
+    if(NOT HAS_FLTO_THIN AND NOT NO_FLTO_ARCH)
       _pybind11_return_if_cxx_and_linker_flags_work(
         HAS_FLTO "-flto${cxx_append}" "-flto${linker_append}" PYBIND11_LTO_CXX_FLAGS
         PYBIND11_LTO_LINKER_FLAGS)
     endif()
   elseif(CMAKE_CXX_COMPILER_ID MATCHES "Intel")
     # Intel equivalent to LTO is called IPO
     _pybind11_return_if_cxx_and_linker_flags_work(HAS_INTEL_IPO "-ipo" "-ipo"
```

### Comparing `iminuit-2.8.4/extern/pybind11/tools/pybind11NewTools.cmake` & `iminuit-2.9.0/extern/pybind11/tools/pybind11NewTools.cmake`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # tools/pybind11NewTools.cmake -- Build system for the pybind11 modules
 #
 # Copyright (c) 2020 Wenzel Jakob <wenzel@inf.ethz.ch> and Henry Schreiner
 #
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 
+if(CMAKE_VERSION VERSION_LESS 3.12)
+  message(FATAL_ERROR "You cannot use the new FindPython module with CMake < 3.12")
+endif()
+
+include_guard(GLOBAL)
+
 get_property(
   is_config
   TARGET pybind11::headers
   PROPERTY IMPORTED)
 
 if(pybind11_FIND_QUIETLY)
   set(_pybind11_quiet QUIET)
 else()
   set(_pybind11_quiet "")
 endif()
 
-if(CMAKE_VERSION VERSION_LESS 3.12)
-  message(FATAL_ERROR "You cannot use the new FindPython module with CMake < 3.12")
-endif()
-
 if(NOT Python_FOUND
    AND NOT Python3_FOUND
    AND NOT Python2_FOUND)
   if(NOT DEFINED Python_FIND_IMPLEMENTATIONS)
     set(Python_FIND_IMPLEMENTATIONS CPython PyPy)
   endif()
 
@@ -78,14 +80,23 @@
 if(NOT DEFINED ${_Python}_EXECUTABLE)
   message(
     FATAL_ERROR
       "${_Python} was found without the Interpreter component. Pybind11 requires this component.")
 
 endif()
 
+if(NOT ${_Python}_EXECUTABLE STREQUAL PYBIND11_PYTHON_EXECUTABLE_LAST)
+  # Detect changes to the Python version/binary in subsequent CMake runs, and refresh config if needed
+  unset(PYTHON_IS_DEBUG CACHE)
+  unset(PYTHON_MODULE_EXTENSION CACHE)
+  set(PYBIND11_PYTHON_EXECUTABLE_LAST
+      "${${_Python}_EXECUTABLE}"
+      CACHE INTERNAL "Python executable during the last CMake run")
+endif()
+
 if(NOT DEFINED PYTHON_IS_DEBUG)
   # Debug check - see https://stackoverflow.com/questions/646518/python-how-to-detect-debug-Interpreter
   execute_process(
     COMMAND "${${_Python}_EXECUTABLE}" "-c"
             "import sys; sys.exit(hasattr(sys, 'gettotalrefcount'))"
     RESULT_VARIABLE _PYTHON_IS_DEBUG)
   set(PYTHON_IS_DEBUG
@@ -226,15 +237,15 @@
   endif()
 
   if(NOT DEFINED CMAKE_CUDA_VISIBILITY_PRESET)
     set_target_properties(${target_name} PROPERTIES CUDA_VISIBILITY_PRESET "hidden")
   endif()
 
   # If we don't pass a WITH_SOABI or WITHOUT_SOABI, use our own default handling of extensions
-  if(NOT ARG_WITHOUT_SOABI OR NOT "WITH_SOABI" IN_LIST ARG_UNPARSED_ARGUMENTS)
+  if(NOT ARG_WITHOUT_SOABI AND NOT "WITH_SOABI" IN_LIST ARG_UNPARSED_ARGUMENTS)
     pybind11_extension(${target_name})
   endif()
 
   if(ARG_NO_EXTRAS)
     return()
   endif()
```

### Comparing `iminuit-2.8.4/extern/pybind11/tools/pybind11Tools.cmake` & `iminuit-2.9.0/extern/pybind11/tools/pybind11Tools.cmake`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # tools/pybind11Tools.cmake -- Build system for the pybind11 modules
 #
 # Copyright (c) 2020 Wenzel Jakob <wenzel.jakob@epfl.ch>
 #
 # All rights reserved. Use of this source code is governed by a
 # BSD-style license that can be found in the LICENSE file.
 
+# include_guard(global) (pre-CMake 3.10)
+if(TARGET pybind11::python_headers)
+  return()
+endif()
+
 # Built-in in CMake 3.5+
 include(CMakeParseArguments)
 
 if(pybind11_FIND_QUIETLY)
   set(_pybind11_quiet QUIET)
 else()
   set(_pybind11_quiet "")
@@ -34,46 +39,40 @@
   set(PYBIND11_PYTHON_VERSION
       ""
       CACHE STRING "Python version to use for compiling modules")
 endif()
 
 # A user can set versions manually too
 set(Python_ADDITIONAL_VERSIONS
-    "3.10;3.9;3.8;3.7;3.6;3.5;3.4"
+    "3.11;3.10;3.9;3.8;3.7;3.6;3.5;3.4"
     CACHE INTERNAL "")
 
 list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_LIST_DIR}")
 find_package(PythonLibsNew ${PYBIND11_PYTHON_VERSION} MODULE REQUIRED ${_pybind11_quiet})
 list(REMOVE_AT CMAKE_MODULE_PATH -1)
 
+# Makes a normal variable a cached variable
+macro(_PYBIND11_PROMOTE_TO_CACHE NAME)
+  set(_tmp_ptc "${${NAME}}")
+  # CMake 3.21 complains if a cached variable is shadowed by a normal one
+  unset(${NAME})
+  set(${NAME}
+      "${_tmp_ptc}"
+      CACHE INTERNAL "")
+endmacro()
+
 # Cache variables so pybind11_add_module can be used in parent projects
-set(PYTHON_INCLUDE_DIRS
-    ${PYTHON_INCLUDE_DIRS}
-    CACHE INTERNAL "")
-set(PYTHON_LIBRARIES
-    ${PYTHON_LIBRARIES}
-    CACHE INTERNAL "")
-set(PYTHON_MODULE_PREFIX
-    ${PYTHON_MODULE_PREFIX}
-    CACHE INTERNAL "")
-set(PYTHON_MODULE_EXTENSION
-    ${PYTHON_MODULE_EXTENSION}
-    CACHE INTERNAL "")
-set(PYTHON_VERSION_MAJOR
-    ${PYTHON_VERSION_MAJOR}
-    CACHE INTERNAL "")
-set(PYTHON_VERSION_MINOR
-    ${PYTHON_VERSION_MINOR}
-    CACHE INTERNAL "")
-set(PYTHON_VERSION
-    ${PYTHON_VERSION}
-    CACHE INTERNAL "")
-set(PYTHON_IS_DEBUG
-    "${PYTHON_IS_DEBUG}"
-    CACHE INTERNAL "")
+_pybind11_promote_to_cache(PYTHON_INCLUDE_DIRS)
+_pybind11_promote_to_cache(PYTHON_LIBRARIES)
+_pybind11_promote_to_cache(PYTHON_MODULE_PREFIX)
+_pybind11_promote_to_cache(PYTHON_MODULE_EXTENSION)
+_pybind11_promote_to_cache(PYTHON_VERSION_MAJOR)
+_pybind11_promote_to_cache(PYTHON_VERSION_MINOR)
+_pybind11_promote_to_cache(PYTHON_VERSION)
+_pybind11_promote_to_cache(PYTHON_IS_DEBUG)
 
 if(PYBIND11_MASTER_PROJECT)
   if(PYTHON_MODULE_EXTENSION MATCHES "pypy")
     if(NOT DEFINED PYPY_VERSION)
       execute_process(
         COMMAND ${PYTHON_EXECUTABLE} -c
                 [=[import sys; sys.stdout.write(".".join(map(str, sys.pypy_version_info[:3])))]=]
```

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/LinkDef.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/LinkDef.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ABObj.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ABObj.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ABProd.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ABProd.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ABSum.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ABSum.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ABTypes.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ABTypes.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/AnalyticalGradientCalculator.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/AnalyticalGradientCalculator.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/BFGSErrorUpdator.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/BFGSErrorUpdator.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/CombinedMinimizer.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/CombinedMinimizer.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/CombinedMinimumBuilder.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/CombinedMinimumBuilder.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ContoursError.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ContoursError.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/DavidonErrorUpdator.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/DavidonErrorUpdator.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ExternalInternalGradientCalculator.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ExternalInternalGradientCalculator.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FCNAdapter.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FCNAdapter.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FCNBase.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FCNBase.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FCNGradAdapter.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FCNGradAdapter.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FCNGradientBase.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FCNGradientBase.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliBuilder.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliBuilder.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliChi2FCN.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliChi2FCN.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliErrorUpdator.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliErrorUpdator.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliFCNAdapter.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliFCNAdapter.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliFCNBase.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliFCNBase.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliGradientCalculator.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliGradientCalculator.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliMaximumLikelihoodFCN.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliMaximumLikelihoodFCN.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliMinimizer.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliMinimizer.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliStandardChi2FCN.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliStandardChi2FCN.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FumiliStandardMaximumLikelihoodFCN.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FumiliStandardMaximumLikelihoodFCN.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FunctionGradient.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FunctionGradient.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FunctionMinimizer.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FunctionMinimizer.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/FunctionMinimum.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/FunctionMinimum.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/GenericFunction.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/GenericFunction.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/GradientCalculator.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/GradientCalculator.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/HessianGradientCalculator.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/HessianGradientCalculator.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/InitialGradientCalculator.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/InitialGradientCalculator.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/LASymMatrix.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/LASymMatrix.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/LAVector.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/LAVector.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/LaInverse.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/LaInverse.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/LaOuterProduct.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/LaOuterProduct.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/LaProd.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/LaProd.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/LaSum.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/LaSum.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MPIProcess.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MPIProcess.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MatrixInverse.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MatrixInverse.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MinimumBuilder.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MinimumBuilder.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MinimumError.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MinimumError.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MinimumErrorUpdator.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MinimumErrorUpdator.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MinimumParameters.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MinimumParameters.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MinimumSeed.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MinimumSeed.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MinimumSeedGenerator.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MinimumSeedGenerator.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MinimumState.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MinimumState.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MinosError.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MinosError.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/Minuit2Minimizer.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/Minuit2Minimizer.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MinuitParameter.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MinuitParameter.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnApplication.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnApplication.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnConfig.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnConfig.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnContours.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnContours.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnCovarianceSqueeze.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnCovarianceSqueeze.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnCross.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnCross.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnEigen.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnEigen.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnFcn.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnFcn.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnFumiliMinimize.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnFumiliMinimize.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnFunctionCross.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnFunctionCross.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnGlobalCorrelationCoeff.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnGlobalCorrelationCoeff.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnHesse.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnHesse.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnLineSearch.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnLineSearch.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnMachinePrecision.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnMachinePrecision.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnMatrix.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnMatrix.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnMigrad.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnMigrad.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnMinimize.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnMinimize.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnMinos.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnMinos.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnParabola.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnParabola.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnParabolaFactory.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnParabolaFactory.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnParabolaPoint.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnParabolaPoint.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnParameterScan.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnParameterScan.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnPlot.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnPlot.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnPosDef.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnPosDef.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnPrint.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnPrint.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnRefCountedPointer.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnRefCountedPointer.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnReferenceCounter.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnReferenceCounter.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnScan.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnScan.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnSeedGenerator.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnSeedGenerator.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnSimplex.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnSimplex.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnStrategy.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnStrategy.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnTiny.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnTiny.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnTraceObject.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnTraceObject.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnUserCovariance.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnUserCovariance.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnUserFcn.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnUserFcn.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnUserParameterState.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnUserParameterState.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnUserParameters.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnUserParameters.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnUserTransformation.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnUserTransformation.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/MnVectorTransform.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/MnVectorTransform.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ModularFunctionMinimizer.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ModularFunctionMinimizer.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/NegativeG2LineSearch.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/NegativeG2LineSearch.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/Numerical2PGradientCalculator.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/Numerical2PGradientCalculator.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/NumericalDerivator.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/NumericalDerivator.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ParametricFunction.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ParametricFunction.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ScanBuilder.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ScanBuilder.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/ScanMinimizer.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/ScanMinimizer.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/SimplexBuilder.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/SimplexBuilder.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/SimplexMinimizer.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/SimplexMinimizer.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/SimplexParameters.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/SimplexParameters.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/SimplexSeedGenerator.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/SimplexSeedGenerator.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/SinParameterTransformation.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/SinParameterTransformation.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/SqrtLowParameterTransformation.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/SqrtLowParameterTransformation.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/SqrtUpParameterTransformation.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/SqrtUpParameterTransformation.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/StackAllocator.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/StackAllocator.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/VariableMetricBuilder.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/VariableMetricBuilder.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/VariableMetricEDMEstimator.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/VariableMetricEDMEstimator.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/VariableMetricMinimizer.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/VariableMetricMinimizer.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/Minuit2/VectorOuterProduct.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/Minuit2/VectorOuterProduct.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/inc/TMinuit2TraceObject.h` & `iminuit-2.9.0/extern/root/math/minuit2/inc/TMinuit2TraceObject.h`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/AnalyticalGradientCalculator.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/AnalyticalGradientCalculator.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/BFGSErrorUpdator.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/BFGSErrorUpdator.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/BasicMinimumError.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/BasicMinimumError.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/CombinedMinimumBuilder.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/CombinedMinimumBuilder.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/DavidonErrorUpdator.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/DavidonErrorUpdator.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/ExternalInternalGradientCalculator.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/ExternalInternalGradientCalculator.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/FumiliBuilder.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/FumiliBuilder.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/FumiliErrorUpdator.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/FumiliErrorUpdator.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/FumiliGradientCalculator.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/FumiliGradientCalculator.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/FumiliMinimizer.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/FumiliMinimizer.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/FumiliStandardChi2FCN.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/FumiliStandardChi2FCN.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/FumiliStandardMaximumLikelihoodFCN.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/FumiliStandardMaximumLikelihoodFCN.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/HessianGradientCalculator.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/HessianGradientCalculator.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/InitialGradientCalculator.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/InitialGradientCalculator.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/LaEigenValues.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/LaEigenValues.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/LaInnerProduct.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/LaInnerProduct.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/LaInverse.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/LaInverse.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/LaOuterProduct.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/LaOuterProduct.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/LaSumOfElements.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/LaSumOfElements.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/LaVtMVSimilarity.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/LaVtMVSimilarity.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MPIProcess.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MPIProcess.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MinimumBuilder.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MinimumBuilder.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/Minuit2Minimizer.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/Minuit2Minimizer.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnApplication.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnApplication.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnContours.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnContours.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnCovarianceSqueeze.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnCovarianceSqueeze.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnEigen.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnEigen.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnFcn.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnFcn.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnFumiliMinimize.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnFumiliMinimize.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnFunctionCross.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnFunctionCross.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnGlobalCorrelationCoeff.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnGlobalCorrelationCoeff.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnHesse.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnHesse.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnLineSearch.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnLineSearch.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnMachinePrecision.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnMachinePrecision.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnMinos.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnMinos.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnParabolaFactory.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnParabolaFactory.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnParameterScan.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnParameterScan.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnPlot.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnPlot.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnPosDef.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnPosDef.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnPrint.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnPrint.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnPrintImpl.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnPrintImpl.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnScan.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnScan.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnSeedGenerator.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnSeedGenerator.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnStrategy.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnStrategy.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnTiny.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnTiny.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnTraceObject.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnTraceObject.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnUserFcn.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnUserFcn.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnUserParameterState.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnUserParameterState.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnUserParameters.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnUserParameters.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/MnUserTransformation.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/MnUserTransformation.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/ModularFunctionMinimizer.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/ModularFunctionMinimizer.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/NegativeG2LineSearch.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/NegativeG2LineSearch.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/Numerical2PGradientCalculator.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/Numerical2PGradientCalculator.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/NumericalDerivator.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/NumericalDerivator.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/ParametricFunction.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/ParametricFunction.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/ScanBuilder.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/ScanBuilder.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/SimplexBuilder.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/SimplexBuilder.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/SimplexParameters.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/SimplexParameters.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/SimplexSeedGenerator.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/SimplexSeedGenerator.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/SinParameterTransformation.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/SinParameterTransformation.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/SqrtLowParameterTransformation.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/SqrtLowParameterTransformation.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/SqrtUpParameterTransformation.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/SqrtUpParameterTransformation.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/TMinuit2TraceObject.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/TMinuit2TraceObject.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/VariableMetricBuilder.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/VariableMetricBuilder.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/VariableMetricEDMEstimator.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/VariableMetricEDMEstimator.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/mnbins.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/mnbins.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/mndasum.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/mndasum.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/mndaxpy.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/mndaxpy.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/mnddot.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/mnddot.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/mndscal.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/mndscal.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/mndspmv.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/mndspmv.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/mndspr.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/mndspr.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/mnlsame.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/mnlsame.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/mnteigen.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/mnteigen.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/mntplot.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/mntplot.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/mnvert.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/mnvert.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/extern/root/math/minuit2/src/mnxerbla.cxx` & `iminuit-2.9.0/extern/root/math/minuit2/src/mnxerbla.cxx`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/setup.cfg` & `iminuit-2.9.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 	Programming Language :: C++
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Software Development
 	Topic :: Scientific/Engineering :: Physics
 	Topic :: Scientific/Engineering :: Mathematics
 	Operating System :: Microsoft :: Windows
@@ -68,15 +69,15 @@
 	scipy
 	sphinx
 	sphinx_rtd_theme
 	tabulate
 	nbsphinx
 	boost_histogram
 doc = 
-	sphinx==4.1
+	sphinx>=4.1
 	sphinx-rtd-theme
 	nbsphinx
 	ipykernel
 	matplotlib
 
 [check-manifest]
 ignore =
```

### Comparing `iminuit-2.8.4/src/contours.cpp` & `iminuit-2.9.0/src/contours.cpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/equal.hpp` & `iminuit-2.9.0/src/equal.hpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/fcn.cpp` & `iminuit-2.9.0/src/fcn.cpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/fcn.hpp` & `iminuit-2.9.0/src/fcn.hpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/functionminimum.cpp` & `iminuit-2.9.0/src/functionminimum.cpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/functionminimum_extra.cpp` & `iminuit-2.9.0/src/functionminimum_extra.cpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/functionminimum_pickle.cpp` & `iminuit-2.9.0/src/functionminimum_pickle.cpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/hesse.cpp` & `iminuit-2.9.0/src/hesse.cpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/iminuit/__init__.py` & `iminuit-2.9.0/src/iminuit/__init__.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/iminuit/_deprecated.py` & `iminuit-2.9.0/src/iminuit/_deprecated.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/iminuit/_repr_html.py` & `iminuit-2.9.0/src/iminuit/_repr_html.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/iminuit/_repr_text.py` & `iminuit-2.9.0/src/iminuit/_repr_text.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/iminuit/cost.py` & `iminuit-2.9.0/src/iminuit/cost.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,52 +33,43 @@
 should perform well. If you have trouble with your own implementations, try these.
 
 The binned versions of the log-likelihood fits support weighted samples. For each bin
 of the histogram, the sum of weights and the sum of squared weights is needed then, see
 class documentation for details.
 """
 
-from .util import describe, make_func_code, merge_signatures, PerformanceWarning
+from .util import (
+    describe,
+    make_func_code,
+    merge_signatures,
+    PerformanceWarning,
+)
 import numpy as np
 from collections.abc import Sequence
+import abc
 from typing import Tuple, Callable, Union
 import warnings
 
 
 def _sum_log_x(x):
     return np.sum(np.log(x + 1e-323))
 
 
-def _spd_transform(n, mu):
-    # Scaled Poisson distribution from Bohm and Zech, NIMA 748 (2014) 1-6
-    v, var = np.transpose(n)
-    s = v / (var + 1e-323)
-    return v * s, mu * s
-
-
 def _log_poisson_part(n, mu):
     # add n log(n) to keep sum small, required to not loose accuracy in Minuit
     return n * (np.log(n + 1e-323) - np.log(mu + 1e-323))
 
 
 def _sum_log_poisson_part(n, mu):
-    if n.ndim == 2:
-        n2, mu2 = _spd_transform(n, mu)
-    else:
-        n2, mu2 = n, mu
-    return np.sum(_log_poisson_part(n2, mu2))
+    return np.sum(_log_poisson_part(n, mu))
 
 
 def _sum_log_poisson(n, mu):
-    if n.ndim == 2:
-        n2, mu2 = _spd_transform(n, mu)
-    else:
-        n2, mu2 = n, mu
     # subtract n to keep sum small, required to not loose accuracy in Minuit
-    return np.sum(mu2 - n2 + _log_poisson_part(n2, mu2))
+    return np.sum(mu - n + _log_poisson_part(n, mu))
 
 
 def _z_squared(y, ye, ym):
     z = (y - ym) / ye
     return z * z
 
 
@@ -94,20 +85,14 @@
 # If numba is available, use it to accelerate computations in float32 and float64
 # precision. Fall back to plain numpy for float128 which is not currently supported
 # by numba.
 try:
     import numba as nb
     from numba.extending import overload
 
-    _spd_transform_np = _spd_transform
-
-    @overload(_spd_transform, inline="always")
-    def _spd_transform_ol(n, mu):
-        return _spd_transform_np  # pragma: no cover
-
     _log_poisson_part_np = _log_poisson_part
 
     @overload(_log_poisson_part, inline="always")
     def _log_poisson_part_ol(n, mu):
         return _log_poisson_part_np  # pragma: no cover
 
     _z_squared_np = _z_squared
@@ -181,56 +166,57 @@
 
     del nb
     del overload
 except ModuleNotFoundError:  # pragma: no cover
     pass
 
 
-class Cost:
+class Cost(abc.ABC):
     """Base class for all cost functions."""
 
-    __slots__ = "_func_code", "_verbose", "_ndata"
+    __slots__ = ("_func_code", "_verbose")
 
     @property
     def errordef(self):
         """For internal use."""
         return 1.0
 
     @property
     def func_code(self):
         """For internal use."""
         return self._func_code
 
     @property
+    @abc.abstractmethod
+    def ndata(self):
+        """
+        Return number of points in least-squares fits or bins in a binned fit.
+
+        Infinity is returned if the cost function is unbinned. This is used by Minuit
+        to compute the reduced chi2, a goodness-of-fit estimate.
+        """
+        ...  # pragma: no cover
+
+    @property
     def verbose(self):
         """
         Access verbosity level.
 
         Set this to 1 to print all function calls with input and output.
         """
         return self._verbose
 
     @verbose.setter
     def verbose(self, value: int):
         self._verbose = value
 
-    @property
-    def ndata(self):
-        """
-        Return number of points in least-squares fits or bins in a binned fit.
-
-        Infinity is returned if the cost function is unbinned.
-        """
-        return self._ndata
-
-    def __init__(self, args: Tuple[str], ndata: float, verbose: int):
+    def __init__(self, args: Tuple[str], verbose: int):
         """For internal use."""
         self._func_code = make_func_code(args)
         self._verbose = verbose
-        self._ndata = ndata
 
     def __add__(self, rhs):
         """
         Add two cost functions to form a combined cost function.
 
         Returns
         -------
@@ -278,56 +264,23 @@
     """
 
     __slots__ = "value"
 
     def __init__(self, value: float):
         """Initialize constant with a value."""
         self.value = value
-        super().__init__((), 0.0, False)
-
-    def _call(self, args):
-        return self.value
+        super().__init__((), False)
 
-
-class MaskedCost(Cost):
-    """Base class for cost functions that support data masking."""
-
-    __slots__ = "_mask", "_masked"
-
-    def __init__(self, args, ndata, verbose):
-        """For internal use."""
-        super().__init__(args, ndata, verbose)
-        self.mask = None
-
-    @property
-    def mask(self):
-        """Boolean array, array of indices, or None.
-
-        If not None, only values selected by the mask are considered. The mask acts on
-        the first dimension of a value array, i.e. values[mask]. Default is None.
-        """
-        return self._mask
-
-    @property
+    @Cost.ndata.getter
     def ndata(self):
-        """
-        Return number of points in least-squares fits or bins in a binned fit.
+        """See Cost.ndata."""
+        return 0
 
-        Infinity is returned if the cost function is unbinned.
-        """
-        n = np.sum(~self._mask) if self._mask is not None else 0
-        return self._ndata - n
-
-    @mask.setter
-    def mask(self, mask):
-        self._mask = None if mask is None else np.asarray(mask)
-        self._masked = self._make_masked()
-
-    def _make_masked(self):
-        return self._data if self._mask is None else self._data[self._mask]
+    def _call(self, args):
+        return self.value
 
 
 class CostSum(Cost, Sequence):
     """Sum of cost functions.
 
     Users do not need to create objects of this class themselves. They should just add
     cost functions, for example::
@@ -374,53 +327,98 @@
                 self._items += item._items
             elif isinstance(item, (int, float)):
                 if item != 0:
                     self._items.append(Constant(item))
             else:
                 self._items.append(item)
         args, self._maps = merge_signatures(self._items)
-        super().__init__(
-            args, sum(c.ndata for c in self._items), max(c.verbose for c in self._items)
-        )
+        super().__init__(args, max(c.verbose for c in self._items))
 
     def _call(self, args):
         r = 0.0
         for c, map in zip(self._items, self._maps):
             c_args = tuple(args[i] for i in map)
             r += c._call(c_args)
         return r
 
+    @Cost.ndata.getter
+    def ndata(self):
+        """See Cost.ndata."""
+        return sum(c.ndata for c in self._items)
+
     def __len__(self):
         """Return number of constituent cost functions."""
         return self._items.__len__()
 
     def __getitem__(self, key):
         """Get constituent cost function by index."""
         return self._items.__getitem__(key)
 
 
-class UnbinnedCost(MaskedCost):
-    """Base class for unbinned cost functions."""
+class MaskedCost(Cost):
+    """Base class for cost functions that support data masking."""
 
-    __slots__ = "_data", "_model"
+    __slots__ = "_data", "_mask", "_masked"
+
+    def __init__(self, args, data, verbose):
+        """For internal use."""
+        super().__init__(args, verbose)
+        if np.ndim(data) > 1:
+            self._data = np.transpose(data)
+        self._data = data
+        self.mask = None  # triggers update of _masked, _ndata
+
+    @property
+    def mask(self):
+        """Boolean array, array of indices, or None.
+
+        If not None, only values selected by the mask are considered. The mask acts on
+        the first dimension of a value array, i.e. values[mask]. Default is None.
+        """
+        return self._mask
+
+    @mask.setter
+    def mask(self, mask):
+        self._mask = None if mask is None else np.asarray(mask)
+        self._update_masked()
 
     @property
     def data(self):
-        """Unbinned samples."""
+        """Return data samples."""
         return self._data
 
     @data.setter
     def data(self, value):
         self._data[:] = value
+        self._update_masked()
+
+    @Cost.ndata.getter
+    def ndata(self):
+        """See Cost.ndata."""
+        return len(self._masked)
+
+    def _update_masked(self):
+        self._masked = self._data if self._mask is None else self._data[self._mask]
+
+
+class UnbinnedCost(MaskedCost):
+    """Base class for unbinned cost functions."""
+
+    __slots__ = "_model"
+
+    @Cost.ndata.getter
+    def ndata(self):
+        """See Cost.ndata."""
+        # unbinned likelihoods have infinite degrees of freedom
+        return np.inf
 
     def __init__(self, data, model: Callable, verbose):
         """For internal use."""
-        self._data = _norm(data)
         self._model = model
-        super().__init__(describe(model)[1:], np.inf, verbose)
+        super().__init__(describe(model)[1:], _norm(data), verbose)
 
 
 class UnbinnedNLL(UnbinnedCost):
     """Unbinned negative log-likelihood.
 
     Use this if only the shape of the fitted PDF is of interest and the original
     unbinned data is available.
@@ -497,56 +495,83 @@
         )
         return 2.0 * (ns - _sum_log_x(spdf))
 
 
 class BinnedCost(MaskedCost):
     """Base class for binned cost functions."""
 
-    __slots__ = "_n", "_xe", "_model"
+    __slots__ = "_xe", "_model"
+
+    def _weighted(self):
+        return self._data.ndim > self._xe.ndim
+
+    def _prepare_data(self, value):
+        assert self._xe is not None
+
+        n = _norm(value)
+        xe = self._xe
+
+        if n.ndim == xe.ndim:
+            is_weighted = False
+        else:
+            is_weighted = True
+            if n.ndim > xe.ndim + 1 or n.ndim < xe.ndim:
+                raise ValueError("n must either have same dimension as xe or one extra")
+
+        if np.any(
+            np.array(n.shape[:-1] if is_weighted else n.shape) + 1 != self._xe.shape
+        ):
+            raise ValueError("n and xe have incompatible shapes")
+
+        if is_weighted:
+            if n.shape[-1] != 2:
+                raise ValueError("n must have shape (..., 2)")
+            # Scale factor from Bohm and Zech, NIMA 748 (2014) 1-6
+            v = n[..., 0]
+            var = n[..., 1]
+            s = v / (var + 1e-323)
+            return np.column_stack((v, var, v * s, s))
+
+        return n
 
     @property
-    def n(self):
+    def data(self):
         """Access bin counts."""
-        return self._n
+        if self._weighted():
+            return self._data[:, :2]
+        return self._data
+
+    @data.setter
+    def data(self, value):
+        # calling the property's setter from the base class is clunky
+        super(__class__, self.__class__).data.__set__(self, self._prepare_data(value))
 
-    @n.setter
-    def n(self, value):
-        self._n[:] = value
+    n = data
 
     @property
     def xe(self):
         """Access bin edges."""
         return self._xe
 
     @xe.setter
     def xe(self, value):
         self.xe[:] = value
 
     def __init__(self, n, xe, model, verbose):
         """For internal use."""
-        self._n = _norm(n)
         self._xe = _norm(xe)
         self._model = model
-
-        if self._n.ndim > 2:
-            raise ValueError("n must be at most 2-dimensional")
-
-        if self._n.ndim == 2 and self._n.shape[1] != 2:
-            raise ValueError("n must shape (N x 2) if 2-dimensional")
-
-        if np.any((np.array(self._n.shape[0]) + 1) != self._xe.shape):
-            raise ValueError("n and xe have incompatible shapes")
-
-        super().__init__(describe(model)[1:], len(n), verbose)
+        super().__init__(describe(model)[1:], self._prepare_data(n), verbose)
 
 
 class BinnedNLL(BinnedCost):
     """Binned negative log-likelihood.
 
     Use this if only the shape of the fitted PDF is of interest and the data is binned.
+    This cost function works with normal and weighted histograms. See init for details.
     """
 
     __slots__ = ()
 
     @property
     def cdf(self):
         """Get cumulative density function."""
@@ -574,30 +599,35 @@
         super().__init__(n, xe, cdf, verbose)
 
     def _call(self, args):
         cdf = self._model(self._xe, *args)
         cdf = _check_model_output(cdf)
         prob = np.diff(cdf)
         n = self._masked
-        ma = self._mask
+        ma = self.mask
         if ma is not None:
             prob = prob[ma]
-        mu = np.sum(n) * prob
-        # + np.sum(mu) can be skipped, it is effectively constant
+            prob /= np.sum(prob)  # normalise probability
+        if self._weighted():
+            mu = np.sum(n[:, 0]) * prob
+            # apply Bohm-Zech scaling, see Bohm and Zech, NIMA 748 (2014) 1-6
+            mu *= n[:, 3]
+            n = n[:, 2]
+        else:
+            mu = np.sum(n) * prob
+        # + np.sum(mu) is skipped, it is constant since sum(prob) = 1
         return 2.0 * _sum_log_poisson_part(n, mu)
 
-    def _make_masked(self):
-        return self._n if self._mask is None else self._n[self._mask]
-
 
 class ExtendedBinnedNLL(BinnedCost):
     """Binned extended negative log-likelihood.
 
     Use this if shape and normalization of the fitted PDF are of interest and the data
-    is binned.
+    is binned. This cost function works with normal and weighted histograms. See init
+    for details.
     """
 
     __slots__ = ()
 
     @property
     def scaled_cdf(self):
         """Get integrated density model."""
@@ -623,58 +653,65 @@
         """
         super().__init__(n, xe, scaled_cdf, verbose)
 
     def _call(self, args):
         scdf = self._model(self._xe, *args)
         scdf = _check_model_output(scdf)
         mu = np.diff(scdf)
-        ma = self._mask
+        ma = self.mask
         n = self._masked
         if ma is not None:
             mu = mu[ma]
+        if self._weighted():
+            # apply Bohm-Zech scaling, see Bohm and Zech, NIMA 748 (2014) 1-6
+            mu *= n[:, 3]
+            n = n[:, 2]
         return 2.0 * _sum_log_poisson(n, mu)
 
-    def _make_masked(self):
-        return self._n if self._mask is None else self._n[self._mask]
-
 
 class LeastSquares(MaskedCost):
     """Least-squares cost function (aka chisquare function).
 
     Use this if you have data of the form (x, y +/- yerror).
     """
 
-    __slots__ = "_loss", "_cost", "_x", "_y", "_yerror", "_model"
+    __slots__ = "_loss", "_cost", "_model"
 
     @property
     def x(self):
         """Get explanatory variables."""
-        return self._x
+        return self.data[:, 0]
 
     @x.setter
     def x(self, value):
-        self._x[:] = value
+        d = self.data
+        d[:, 0] = _norm(value)
+        self.data = d  # this also resets the masked
 
     @property
     def y(self):
         """Get samples."""
-        return self._y
+        return self.data[:, 1]
 
     @y.setter
     def y(self, value):
-        self._y[:] = value
+        d = self.data
+        d[:, 1] = _norm(value)
+        self.data = d  # this also resets the masked
 
     @property
     def yerror(self):
         """Get sample uncertainties."""
-        return self._yerror
+        return self.data[:, 2]
 
     @yerror.setter
     def yerror(self, value):
-        self._yerror[:] = value
+        d = self.data
+        d[:, 2] = _norm(value)
+        self.data = d
 
     @property
     def model(self):
         """Get model of the form y = f(x, par0, [par1, ...])."""
         return self._model
 
     @property
@@ -740,44 +777,26 @@
         shows the standard potential in comparison with the weaker soft-l1 potential, in
         which outliers act with a constant force independent of their distance.
 
         .. plot:: plots/loss.py
         """
         x = _norm(x)
         y = _norm(y)
+        data = np.column_stack(np.broadcast_arrays(x, y, yerror))
 
-        if len(x) != len(y):
-            raise ValueError("x and y must have same length")
-
-        yerror = np.asarray(yerror, dtype=float)
-        if yerror.ndim == 0:
-            yerror = yerror * np.ones_like(y)
-        elif yerror.shape != y.shape:
-            raise ValueError("y and yerror must have same shape")
-
-        self._x = x
-        self._y = y
-        self._yerror = yerror
         self._model = model
         self.loss = loss
-        super().__init__(describe(self._model)[1:], len(x), verbose)
+        super().__init__(describe(self._model)[1:], data, verbose)
 
     def _call(self, args):
-        x, y, yerror = self._masked
+        x, y, yerror = self._masked.T
         ym = self._model(x, *args)
         ym = _check_model_output(ym)
         return self._cost(y, yerror, ym)
 
-    def _make_masked(self):
-        ma = self._mask
-        if ma is None:
-            return self._x, self._y, self._yerror
-        else:
-            return self._x[ma], self._y[ma], self._yerror[ma]
-
 
 class NormalConstraint(Cost):
     """
     Gaussian penalty for one or several parameters.
 
     The Gaussian penalty acts like a pseudo-measurement of the parameter itself, based
     on a (multi-variate) normal distribution. Penalties can be set for one or
@@ -819,15 +838,15 @@
         if isinstance(args, str):
             args = [args]
         self._value = _norm(value)
         self._cov = _norm(error)
         if self._cov.ndim < 2:
             self._cov **= 2
         self._covinv = _covinv(self._cov)
-        super().__init__(args, len(self._value), False)
+        super().__init__(args, False)
 
     @property
     def covariance(self):
         """
         Get expected covariance of parameters.
 
         Can be 1D (diagonal of covariance matrix) or 2D (full covariance matrix).
@@ -850,14 +869,19 @@
 
     def _call(self, args):
         delta = self._value - args
         if self._covinv.ndim < 2:
             return np.sum(delta ** 2 * self._covinv)
         return np.einsum("i,ij,j", delta, self._covinv, delta)
 
+    @Cost.ndata.getter
+    def ndata(self):
+        """See Cost.ndata."""
+        return len(self._value)
+
 
 def _norm(value):
     value = np.atleast_1d(value)
     dtype = value.dtype
     if dtype.kind != "f":
         value = value.astype(np.float64)
     return value
```

### Comparing `iminuit-2.8.4/src/iminuit/experimental.py` & `iminuit-2.9.0/src/iminuit/experimental.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/iminuit/minimize.py` & `iminuit-2.9.0/src/iminuit/minimize.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/iminuit/minuit.py` & `iminuit-2.9.0/src/iminuit/minuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1837,32 +1837,35 @@
         ContourSet
             Instance of a ContourSet class from matplot.contour.
 
         See Also
         --------
         mncontour
         """
+        from matplotlib import __version__ as mpl_version
         from matplotlib import pyplot as plt
         from matplotlib.path import Path
         from matplotlib.contour import ContourSet
 
+        mpl_version = tuple(map(int, mpl_version.split(".")))
+
         cls = cl if isinstance(cl, Iterable) else [cl]
 
         c_val = []
         c_pts = []
         codes = []
+        n_lineto = size - 2 if mpl_version < (3, 5) else size - 1
         for cl in cls:  # type:ignore
             pts = self.mncontour(x, y, cl=cl, size=size)
-            # add extra point whose coordinates are ignored
+            # add extra point whose coordinates are ignored to close the contour
             pts = np.append(pts, pts[:1], axis=0)
+
             c_val.append(cl if cl is not None else 0.68)
             c_pts.append([pts])  # level can have more than one contour in mpl
-            codes.append(
-                [[Path.MOVETO] + [Path.LINETO] * (size - 2) + [Path.CLOSEPOLY]]
-            )
+            codes.append([[Path.MOVETO] + [Path.LINETO] * n_lineto + [Path.CLOSEPOLY]])
         assert len(c_val) == len(codes), f"{len(c_val)} {len(codes)}"
         cs = ContourSet(plt.gca(), c_val, c_pts, codes)
         plt.clabel(cs)
         plt.xlabel(x)
         plt.ylabel(y)
 
         return cs
```

### Comparing `iminuit-2.8.4/src/iminuit/pdg_format.py` & `iminuit-2.9.0/src/iminuit/pdg_format.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/iminuit/testing.py` & `iminuit-2.9.0/src/iminuit/testing.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/iminuit/util.py` & `iminuit-2.9.0/src/iminuit/util.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/iminuit/version.py` & `iminuit-2.9.0/src/iminuit/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,11 +3,11 @@
 # We use the semantic version scheme: MAJOR.MINOR.MAINTENANCE
 # - See https://packaging.python.org/guides/distributing-packages-using-setuptools
 # - Increase MAJOR when making breaking changes
 # - Increase MINOR when adding backward-compatible features
 # - Increase MAINTENANCE when fixing bugs without adding features
 # - During development, add suffix .devN with N >= 0
 # - For release candidates, add suffix .rcN with N >= 0
-version = "2.8.4"
+version = "2.9.0"
 
 # We list the corresponding ROOT version of the C++ Minuit2 library here
 root_version = "v6-25-01-1694-g187368db19"
```

### Comparing `iminuit-2.8.4/src/iminuit.egg-info/PKG-INFO` & `iminuit-2.9.0/src/iminuit.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,121 +1,125 @@
 Metadata-Version: 2.1
 Name: iminuit
-Version: 2.8.4
+Version: 2.9.0
 Summary: Jupyter-friendly Python frontend for MINUIT2 in C++
 Home-page: http://github.com/scikit-hep/iminuit
 Author: Piti Ongmongkolkul and the iminuit team
 Maintainer: Hans Dembinski
 Maintainer-email: hans.dembinski@gmail.com
 License: MIT+LGPL
 Download-URL: https://pypi.python.org/pypi/iminuit
 Project-URL: Documentation, https://iminuit.readthedocs.io
 Project-URL: Source Code, http://github.com/scikit-hep/iminuit
-Description: .. |iminuit| image:: doc/_static/iminuit_logo.svg
-           :alt: iminuit
-           :target: http://iminuit.readthedocs.io/en/latest
-        
-        |iminuit|
-        =========
-        
-        .. skip-marker-do-not-remove
-        
-        .. image:: https://scikit-hep.org/assets/images/Scikit--HEP-Project-blue.svg
-           :target: https://scikit-hep.org
-        .. image:: https://img.shields.io/pypi/v/iminuit.svg
-           :target: https://pypi.org/project/iminuit
-        .. image:: https://img.shields.io/conda/vn/conda-forge/iminuit.svg
-           :target: https://github.com/conda-forge/iminuit-feedstock
-        .. image:: https://coveralls.io/repos/github/scikit-hep/iminuit/badge.svg?branch=develop
-           :target: https://coveralls.io/github/scikit-hep/iminuit?branch=develop
-        .. image:: https://readthedocs.org/projects/iminuit/badge/?version=stable
-           :target: https://iminuit.readthedocs.io/en/stable
-        .. image:: https://img.shields.io/pypi/l/iminuit
-        .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3949207.svg
-           :target: https://doi.org/10.5281/zenodo.3949207
-        .. image:: https://img.shields.io/badge/ascl-2108.024-blue.svg?colorB=262255
-           :target: https://ascl.net/2108.024
-           :alt: ascl:2108.024
-        
-        *iminuit* is a Jupyter-friendly Python interface for the *Minuit2* C++ library maintained by CERN's ROOT team.
-        
-        Minuit was designed to minimise statistical cost functions, for likelihood and least-squares fits of parametric models to data. It provides the best-fit parameters and error estimates from likelihood profile analysis.
-        
-        - Supported CPython versions: 3.6+
-        - Supported PyPy versions: 3.6
-        - Supported platforms: Linux, OSX and Windows.
-        
-        The iminuit package comes with additional features:
-        
-        - Builtin cost functions for statistical fits
-        
-          - Binned and unbinned maximum-likelihood
-          - Non-linear regression with (optionally robust) weighted least-squares
-          - Gaussian penalty terms
-          - Cost functions can be combined by adding them: ``total_cost = cost_1 + cost_2``
-        - Tools for numerical error propagation ``iminuit.util.propagate``
-        - Support for SciPy minimisers as alternatives to Minuit's Migrad algorithm (optional)
-        - Support for Numba accelerated functions (optional)
-        
-        Checkout our large and comprehensive list of `tutorials`_ that take you all the way from beginner to power user. For help and how-to questions, please use the `discussions`_ on GitHub.
-        
-        .. image:: https://mybinder.org/badge_logo.svg
-           :target: https://mybinder.org/v2/gh/scikit-hep/iminuit/develop?filepath=doc%2Ftutorial
-        
-        In a nutshell
-        -------------
-        
-        .. code-block:: python
-        
-            from iminuit import Minuit
-        
-            def cost_function(x, y, z):
-                return (x - 2) ** 2 + (y - 3) ** 2 + (z - 4) ** 2
-        
-            fcn.errordef = Minuit.LEAST_SQUARES
-        
-            m = Minuit(cost_function, x=0, y=0, z=0)
-        
-            m.migrad()  # run optimiser
-            print(m.values)  # x: 2, y: 3, z: 4
-        
-            m.hesse()   # run covariance estimator
-            print(m.errors)  # x: 1, y: 1, z: 1
-        
-        Versions
-        --------
-        
-        **The current 2.x series has introduced breaking interfaces changes with respect to the 1.x series.**
-        
-        All interface changes are documented in the `changelog`_ with recommendations how to upgrade. To keep existing scripts running, pin your major iminuit version to <2, i.e. ``pip install 'iminuit<2'`` installs the 1.x series.
-        
-        .. _changelog: https://iminuit.readthedocs.io/en/stable/changelog.html
-        .. _tutorials: https://iminuit.readthedocs.io/en/stable/tutorials.html
-        .. _discussions: https://github.com/scikit-hep/iminuit/discussions
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 Provides-Extra: doc
+License-File: LICENSE
+
+.. |iminuit| image:: doc/_static/iminuit_logo.svg
+   :alt: iminuit
+   :target: http://iminuit.readthedocs.io/en/latest
+
+|iminuit|
+=========
+
+.. skip-marker-do-not-remove
+
+.. image:: https://scikit-hep.org/assets/images/Scikit--HEP-Project-blue.svg
+   :target: https://scikit-hep.org
+.. image:: https://img.shields.io/pypi/v/iminuit.svg
+   :target: https://pypi.org/project/iminuit
+.. image:: https://img.shields.io/conda/vn/conda-forge/iminuit.svg
+   :target: https://github.com/conda-forge/iminuit-feedstock
+.. image:: https://coveralls.io/repos/github/scikit-hep/iminuit/badge.svg?branch=develop
+   :target: https://coveralls.io/github/scikit-hep/iminuit?branch=develop
+.. image:: https://readthedocs.org/projects/iminuit/badge/?version=stable
+   :target: https://iminuit.readthedocs.io/en/stable
+.. image:: https://img.shields.io/pypi/l/iminuit
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3949207.svg
+   :target: https://doi.org/10.5281/zenodo.3949207
+.. image:: https://img.shields.io/badge/ascl-2108.024-blue.svg?colorB=262255
+   :target: https://ascl.net/2108.024
+   :alt: ascl:2108.024
+
+*iminuit* is a Jupyter-friendly Python interface for the *Minuit2* C++ library maintained by CERN's ROOT team.
+
+Minuit was designed to minimise statistical cost functions, for likelihood and least-squares fits of parametric models to data. It provides the best-fit parameters and error estimates from likelihood profile analysis.
+
+- Supported CPython versions: 3.6+
+- Supported PyPy versions: 3.6
+- Supported platforms: Linux, OSX and Windows.
+
+The iminuit package comes with additional features:
+
+- Builtin cost functions for statistical fits
+
+  - Binned and unbinned maximum-likelihood
+  - Non-linear regression with (optionally robust) weighted least-squares
+  - Gaussian penalty terms
+  - Cost functions can be combined by adding them: ``total_cost = cost_1 + cost_2``
+- Tools for numerical error propagation ``iminuit.util.propagate``
+- Support for SciPy minimisers as alternatives to Minuit's Migrad algorithm (optional)
+- Support for Numba accelerated functions (optional)
+
+Checkout our large and comprehensive list of `tutorials`_ that take you all the way from beginner to power user. For help and how-to questions, please use the `discussions`_ on GitHub.
+
+.. image:: https://mybinder.org/badge_logo.svg
+   :target: https://mybinder.org/v2/gh/scikit-hep/iminuit/develop?filepath=doc%2Ftutorial
+
+In a nutshell
+-------------
+
+.. code-block:: python
+
+    from iminuit import Minuit
+
+    def cost_function(x, y, z):
+        return (x - 2) ** 2 + (y - 3) ** 2 + (z - 4) ** 2
+
+    cost_function.errordef = Minuit.LEAST_SQUARES
+
+    m = Minuit(cost_function, x=0, y=0, z=0)
+
+    m.migrad()  # run optimiser
+    print(m.values)  # x: 2, y: 3, z: 4
+
+    m.hesse()   # run covariance estimator
+    print(m.errors)  # x: 1, y: 1, z: 1
+
+Versions
+--------
+
+**The current 2.x series has introduced breaking interfaces changes with respect to the 1.x series.**
+
+All interface changes are documented in the `changelog`_ with recommendations how to upgrade. To keep existing scripts running, pin your major iminuit version to <2, i.e. ``pip install 'iminuit<2'`` installs the 1.x series.
+
+.. _changelog: https://iminuit.readthedocs.io/en/stable/changelog.html
+.. _tutorials: https://iminuit.readthedocs.io/en/stable/tutorials.html
+.. _discussions: https://github.com/scikit-hep/iminuit/discussions
+
+
```

### Comparing `iminuit-2.8.4/src/iminuit.egg-info/SOURCES.txt` & `iminuit-2.9.0/src/iminuit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,31 @@
 extern/pybind11/include/pybind11/chrono.h
 extern/pybind11/include/pybind11/common.h
 extern/pybind11/include/pybind11/complex.h
 extern/pybind11/include/pybind11/eigen.h
 extern/pybind11/include/pybind11/embed.h
 extern/pybind11/include/pybind11/eval.h
 extern/pybind11/include/pybind11/functional.h
+extern/pybind11/include/pybind11/gil.h
 extern/pybind11/include/pybind11/iostream.h
 extern/pybind11/include/pybind11/numpy.h
 extern/pybind11/include/pybind11/operators.h
 extern/pybind11/include/pybind11/options.h
 extern/pybind11/include/pybind11/pybind11.h
 extern/pybind11/include/pybind11/pytypes.h
 extern/pybind11/include/pybind11/stl.h
 extern/pybind11/include/pybind11/stl_bind.h
 extern/pybind11/include/pybind11/detail/class.h
 extern/pybind11/include/pybind11/detail/common.h
 extern/pybind11/include/pybind11/detail/descr.h
 extern/pybind11/include/pybind11/detail/init.h
 extern/pybind11/include/pybind11/detail/internals.h
+extern/pybind11/include/pybind11/detail/type_caster_base.h
 extern/pybind11/include/pybind11/detail/typeid.h
+extern/pybind11/include/pybind11/stl/filesystem.h
 extern/pybind11/tools/FindCatch.cmake
 extern/pybind11/tools/FindEigen3.cmake
 extern/pybind11/tools/FindPythonLibsNew.cmake
 extern/pybind11/tools/pybind11Common.cmake
 extern/pybind11/tools/pybind11NewTools.cmake
 extern/pybind11/tools/pybind11Tools.cmake
 extern/root/math/minuit2/inc/LinkDef.h
```

### Comparing `iminuit-2.8.4/src/machineprecision.cpp` & `iminuit-2.9.0/src/machineprecision.cpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/main.cpp` & `iminuit-2.9.0/src/main.cpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/migrad.cpp` & `iminuit-2.9.0/src/migrad.cpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/minimumstate.cpp` & `iminuit-2.9.0/src/minimumstate.cpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/minos.cpp` & `iminuit-2.9.0/src/minos.cpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/minuitparameter.cpp` & `iminuit-2.9.0/src/minuitparameter.cpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/print.cpp` & `iminuit-2.9.0/src/print.cpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/simplex.cpp` & `iminuit-2.9.0/src/simplex.cpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/strategy.cpp` & `iminuit-2.9.0/src/strategy.cpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/type_caster.hpp` & `iminuit-2.9.0/src/type_caster.hpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/usercovariance.cpp` & `iminuit-2.9.0/src/usercovariance.cpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/userparameterstate.cpp` & `iminuit-2.9.0/src/userparameterstate.cpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/src/usertransformation.cpp` & `iminuit-2.9.0/src/usertransformation.cpp`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/fmin_bad.txt` & `iminuit-2.9.0/tests/fmin_bad.txt`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/fmin_good.txt` & `iminuit-2.9.0/tests/fmin_good.txt`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/matrix_long_names.txt` & `iminuit-2.9.0/tests/matrix_long_names.txt`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/merror.txt` & `iminuit-2.9.0/tests/merror.txt`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/merrors.txt` & `iminuit-2.9.0/tests/merrors.txt`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/params.txt` & `iminuit-2.9.0/tests/params.txt`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/params_difficult_values.txt` & `iminuit-2.9.0/tests/params_difficult_values.txt`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/params_long_names.txt` & `iminuit-2.9.0/tests/params_long_names.txt`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/params_with_limits.txt` & `iminuit-2.9.0/tests/params_with_limits.txt`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/test_core.py` & `iminuit-2.9.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/test_cost.py` & `iminuit-2.9.0/tests/test_cost.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from iminuit.cost import (
     CostSum,
     UnbinnedNLL,
     BinnedNLL,
     ExtendedUnbinnedNLL,
     ExtendedBinnedNLL,
     LeastSquares,
+    Constant,
     NormalConstraint,
     _log_poisson_part,
-    _spd_transform,
     PerformanceWarning,
 )
 from collections.abc import Sequence
 
 stats = pytest.importorskip("scipy.stats")
 norm = stats.norm
 
@@ -36,21 +36,36 @@
 def binned(unbinned):
     mle, x = unbinned
     nx, xe = np.histogram(x, bins=50, range=(-3, 3))
     assert np.sum(nx == 0) > 0
     return mle, nx, xe
 
 
+def pdf(x, mu, sigma):
+    return norm(mu, sigma).pdf(x)
+
+
+def cdf(x, mu, sigma):
+    return norm(mu, sigma).cdf(x)
+
+
+def scaled_cdf(x, n, mu, sigma):
+    return n * norm(mu, sigma).cdf(x)
+
+
+def test_Constant():
+    c = Constant(2.5)
+    assert c.value == 2.5
+    assert c.ndata == 0
+
+
 @pytest.mark.parametrize("verbose", (0, 1))
 def test_UnbinnedNLL(unbinned, verbose):
     mle, x = unbinned
 
-    def pdf(x, mu, sigma):
-        return norm(mu, sigma).pdf(x)
-
     cost = UnbinnedNLL(x, pdf, verbose=verbose)
     assert cost.ndata == np.inf
 
     m = Minuit(cost, mu=0, sigma=1)
     m.limits["sigma"] = (0, None)
     m.migrad()
     assert_allclose(m.values, mle[1:], atol=1e-3)
@@ -79,17 +94,14 @@
     assert_equal(m.fmin.reduced_chi2, np.nan)
 
 
 @pytest.mark.parametrize("verbose", (0, 1))
 def test_BinnedNLL(binned, verbose):
     mle, nx, xe = binned
 
-    def cdf(x, mu, sigma):
-        return norm(mu, sigma).cdf(x)
-
     cost = BinnedNLL(nx, xe, cdf, verbose=verbose)
     assert cost.ndata == len(nx)
 
     m = Minuit(cost, mu=0, sigma=1)
     m.limits["sigma"] = (0, None)
     m.migrad()
     # binning loses information compared to unbinned case
@@ -97,29 +109,31 @@
     assert m.errors["mu"] == pytest.approx(1000 ** -0.5, rel=0.05)
     assert m.ndof == len(nx) - 2
 
     assert_allclose(m.fmin.reduced_chi2, 1, atol=0.15)
 
 
 def test_weighted_BinnedNLL():
-    def cdf(x, a):
-        return 1 - np.exp(-a * x)
-
     xe = np.array([0, 1, 10])
-    p = np.diff(cdf(xe, 1))
+    p = np.diff(expon_cdf(xe, 1))
     n = p * 1000
-    m1 = Minuit(BinnedNLL(n, xe, cdf), 1)
+    c = BinnedNLL(n, xe, expon_cdf)
+
+    c = BinnedNLL(n, xe, expon_cdf)
+    assert_equal(c.data, n)
+    m1 = Minuit(c, 1)
     m1.migrad()
     assert m1.values[0] == pytest.approx(1, rel=1e-2)
 
     w = np.transpose((n, 4 * n))
-    m2 = Minuit(BinnedNLL(w, xe, cdf), 1)
+    c = BinnedNLL(w, xe, expon_cdf)
+    assert_equal(c.data, w)
+    m2 = Minuit(c, 1)
     m2.migrad()
     assert m2.values[0] == pytest.approx(1, rel=1e-2)
-
     assert m2.errors[0] == pytest.approx(2 * m1.errors[0], rel=1e-2)
 
 
 def test_BinnedNLL_bad_input_1():
     with pytest.raises(ValueError):
         BinnedNLL([1], [1], lambda x, a: 0)
 
@@ -130,21 +144,23 @@
 
 
 def test_BinnedNLL_bad_input_3():
     with pytest.raises(ValueError):
         BinnedNLL([[1, 2, 3]], [1], lambda x, a: 0)
 
 
+def test_BinnedNLL_bad_input_4():
+    with pytest.raises(ValueError, match="n must have shape"):
+        BinnedNLL([[1, 2, 3]], [1, 2], lambda x, a: 0)
+
+
 @pytest.mark.parametrize("verbose", (0, 1))
 def test_ExtendedBinnedNLL(binned, verbose):
     mle, nx, xe = binned
 
-    def scaled_cdf(x, n, mu, sigma):
-        return n * norm(mu, sigma).cdf(x)
-
     cost = ExtendedBinnedNLL(nx, xe, scaled_cdf, verbose=verbose)
     assert cost.ndata == len(nx)
 
     m = Minuit(cost, n=mle[0], mu=0, sigma=1)
     m.limits["n"] = (0, None)
     m.limits["sigma"] = (0, None)
     m.migrad()
@@ -153,27 +169,24 @@
     assert m.errors["mu"] == pytest.approx(1000 ** -0.5, rel=0.05)
     assert m.ndof == len(nx) - 3
 
     assert_allclose(m.fmin.reduced_chi2, 1, 0.1)
 
 
 def test_weighted_ExtendedBinnedNLL():
-    def cdf(x, a, b):
-        return b * (1 - np.exp(-a * x))
-
     xe = np.array([0, 1, 10])
-    n = np.diff(cdf(xe, 1, 100))
-    m1 = Minuit(ExtendedBinnedNLL(n, xe, cdf), 1, 100)
+    n = np.diff(expon_cdf(xe, 1))
+    m1 = Minuit(ExtendedBinnedNLL(n, xe, expon_cdf), 1)
     m1.migrad()
-    assert_allclose(m1.values, (1, 100), rtol=1e-2)
+    assert_allclose(m1.values, (1,), rtol=1e-2)
 
     w = np.transpose((n, 4 * n))
-    m2 = Minuit(ExtendedBinnedNLL(w, xe, cdf), 1, 100)
+    m2 = Minuit(ExtendedBinnedNLL(w, xe, expon_cdf), 1)
     m2.migrad()
-    assert_allclose(m2.values, (1, 100), rtol=1e-2)
+    assert_allclose(m2.values, (1,), rtol=1e-2)
 
     assert m2.errors[0] == pytest.approx(2 * m1.errors[0], rel=1e-2)
 
 
 def test_ExtendedBinnedNLL_bad_input():
     with pytest.raises(ValueError):
         ExtendedBinnedNLL([1], [1], lambda x, a: 0)
@@ -206,18 +219,18 @@
     assert m.ndof == len(x) - 2
 
     assert_allclose(m.fmin.reduced_chi2, 1, atol=5e-2)
 
 
 def test_LeastSquares_bad_input():
     with pytest.raises(ValueError):
-        LeastSquares([1, 2], [1], [1], lambda x, a: 0)
+        LeastSquares([1, 2], [], [1], lambda x, a: 0)
 
     with pytest.raises(ValueError):
-        LeastSquares([1, 2], [1, 2], [1], lambda x, a: 0)
+        LeastSquares([1, 2], [3, 4, 5], [1], lambda x, a: 0)
 
     with pytest.raises(ValueError):
         LeastSquares([1], [1], [1], lambda x, a: 0, loss="foo")
 
 
 def test_UnbinnedNLL_mask():
     c = UnbinnedNLL([1, np.nan, 2], lambda x, a: x + a)
@@ -332,14 +345,26 @@
 
     assert m.ndof == 1
     m.migrad()
     assert m.valid
     assert_equal(m.values, [1.5])
 
 
+def test_LeastSquares_mask_2():
+    c = LeastSquares([1, 2], [1, 5], 1, lambda x, a: a * x)
+    assert c(2) == pytest.approx(2)
+    c.mask = [False, True]
+    assert c(2) == pytest.approx(1)
+    c.x = [2, 2]
+    c.y = [4, 4]
+    c.yerror = [2, 2]
+    assert c(2) == pytest.approx(0)
+    assert c(1) == pytest.approx(1)
+
+
 def test_LeastSquares_properties():
     def model(x, a):
         return a
 
     c = LeastSquares(1, 2, 3, model)
     assert_equal(c.x, [1])
     assert_equal(c.y, [2])
@@ -499,23 +524,14 @@
     assert_equal(nc.covariance, (9, 16))
     nc.value = (2, 3)
     nc.covariance = (1, 2)
     assert_equal(nc.value, (2, 3))
     assert_equal(nc.covariance, (1, 2))
 
 
-def test_spd_transform():
-    n = np.array([(0.0, 0.0)])
-    assert_allclose(_spd_transform(n, 0), [[0], [0]])
-    assert_allclose(_spd_transform(n, 1), [[0], [0]])
-    n = np.array([(0.0, 1.0)])
-    assert_allclose(_spd_transform(n, 0), [[0], [0]])
-    assert_allclose(_spd_transform(n, 1), [[0], [0]])
-
-
 def test_log_poisson_part():
     assert _log_poisson_part(0, 0) == 0
     assert _log_poisson_part(0, 1) == 0
     assert _log_poisson_part(1, 0) == pytest.approx(743, abs=1)
     n = np.array([(0.0, 0.0)])
     assert_allclose(_log_poisson_part(n, 0), 0)
     assert_allclose(_log_poisson_part(n, 1), 0)
@@ -552,7 +568,28 @@
         ExtendedBinnedNLL([1], [1.0, 2.0], model)(1)
 
     with pytest.warns(PerformanceWarning):
         UnbinnedNLL([1], model)(1)
 
     with pytest.warns(PerformanceWarning):
         ExtendedUnbinnedNLL([1], lambda x, a: (1, model(x, a)))(1)
+
+
+@pytest.mark.parametrize("klass", (BinnedNLL, ExtendedBinnedNLL))
+def test_update_data_with_mask(klass):
+    xe = np.arange(0, 4)
+    nx = np.diff(expon_cdf(xe, 1))
+    nx[0] += 1
+    c = klass(nx.copy(), xe, expon_cdf)
+
+    c.mask = [False, True, True]
+    assert c(1) == 0
+    nx[0] += 1
+    c.n = nx
+    assert c(1) == 0
+    nx[1] += 1
+    c.n = nx
+    assert c(1) != 0
+    nx[0] -= 2
+    c.mask = (True, False, True)
+    c.n = nx
+    assert c(1) == 0
```

### Comparing `iminuit-2.8.4/tests/test_describe.py` & `iminuit-2.9.0/tests/test_describe.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/test_draw.py` & `iminuit-2.9.0/tests/test_draw.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/test_fmin_bad.txt` & `iminuit-2.9.0/tests/test_fmin_bad.txt`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/test_functions.py` & `iminuit-2.9.0/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/test_issue.py` & `iminuit-2.9.0/tests/test_issue.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/test_minimize.py` & `iminuit-2.9.0/tests/test_minimize.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/test_minuit.py` & `iminuit-2.9.0/tests/test_minuit.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/test_pdg_format.py` & `iminuit-2.9.0/tests/test_pdg_format.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/test_repr.py` & `iminuit-2.9.0/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/test_repr_pretty.py` & `iminuit-2.9.0/tests/test_repr_pretty.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/test_scipy.py` & `iminuit-2.9.0/tests/test_scipy.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/test_tabulate.py` & `iminuit-2.9.0/tests/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `iminuit-2.8.4/tests/test_util.py` & `iminuit-2.9.0/tests/test_util.py`

 * *Files identical despite different names*

