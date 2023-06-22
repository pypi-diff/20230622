# Comparing `tmp/niceml-0.4.0.tar.gz` & `tmp/niceml-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niceml-0.4.0.tar", max compression
+gzip compressed data, was "niceml-0.4.1.tar", max compression
```

## Comparing `niceml-0.4.0.tar` & `niceml-0.4.1.tar`

### file list

```diff
@@ -1,326 +1,326 @@
--rw-r--r--   0        0        0     1068 2023-06-05 20:18:16.123982 niceml-0.4.0/LICENSE
--rw-r--r--   0        0        0     1135 2023-06-05 20:18:16.123982 niceml-0.4.0/README.md
--rw-r--r--   0        0        0       22 2023-06-05 20:18:58.048643 niceml-0.4.0/niceml/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/cli/__init__.py
--rw-r--r--   0        0        0     3070 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/cli/clicommands.py
--rw-r--r--   0        0        0      228 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/cli/climain.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/config/__init__.py
--rw-r--r--   0        0        0     9485 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/config/configschemas.py
--rw-r--r--   0        0        0      889 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/config/envconfig.py
--rw-r--r--   0        0        0     3907 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/config/hydra.py
--rw-r--r--   0        0        0      744 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/config/subsetnames.py
--rw-r--r--   0        0        0      310 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/config/trainparams.py
--rw-r--r--   0        0        0      506 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/config/writeopconfig.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dagster/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dagster/jobs/__init__.py
--rw-r--r--   0        0        0     2432 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dagster/jobs/jobs.py
--rw-r--r--   0        0        0      512 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dagster/jobs/repository.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dagster/ops/__init__.py
--rw-r--r--   0        0        0     2090 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dagster/ops/analysis.py
--rw-r--r--   0        0        0     2317 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dagster/ops/copyexp.py
--rw-r--r--   0        0        0     3900 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dagster/ops/cropnumbers.py
--rw-r--r--   0        0        0      921 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dagster/ops/datageneration.py
--rw-r--r--   0        0        0     3396 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dagster/ops/evalcopyexp.py
--rw-r--r--   0        0        0     2058 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dagster/ops/experiment.py
--rw-r--r--   0        0        0     1176 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dagster/ops/exptests.py
--rw-r--r--   0        0        0     4556 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dagster/ops/imagetotable.py
--rw-r--r--   0        0        0     2220 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dagster/ops/localizeexperiment.py
--rw-r--r--   0        0        0     5799 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dagster/ops/prediction.py
--rw-r--r--   0        0        0     3003 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dagster/ops/splitdata.py
--rw-r--r--   0        0        0     2889 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dagster/ops/train.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dagster/resources/__init__.py
--rw-r--r--   0        0        0     3668 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dagster/resources/locations.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/__init__.py
--rw-r--r--   0        0        0     6736 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/binprobvisu.py
--rw-r--r--   0        0        0     4033 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/cam.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/components/__init__.py
--rw-r--r--   0        0        0     3870 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/components/downloadexpviscomponent.py
--rw-r--r--   0        0        0     4603 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/components/expviscomponent.py
--rw-r--r--   0        0        0     1835 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/components/linearviscomponent.py
--rw-r--r--   0        0        0     1329 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/components/metaviscomponent.py
--rw-r--r--   0        0        0     3769 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/components/prefixviscomponent.py
--rw-r--r--   0        0        0     2892 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/components/selectionviscomponent.py
--rw-r--r--   0        0        0     1446 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/configviscomponent.py
--rw-r--r--   0        0        0     3006 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/dashboard.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/expvisuhelper.py
--rw-r--r--   0        0        0     3126 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/imagenetdataloggerviscomponent.py
--rw-r--r--   0        0        0     3294 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/metricviscomponent.py
--rw-r--r--   0        0        0      293 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/netdataloggerviscomponent.py
--rw-r--r--   0        0        0     5961 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/remotettrainutils.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/visualizers/__init__.py
--rw-r--r--   0        0        0     3125 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/visualizers/boundingboxvisualizer.py
--rw-r--r--   0        0        0     4554 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/visualizers/imagevisualizer.py
--rw-r--r--   0        0        0     3206 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/dashboard/visualizers/maskvisualizer.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/augmentation/__init__.py
--rw-r--r--   0        0        0      362 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/augmentation/augmentation.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datadescriptions/__init__.py
--rw-r--r--   0        0        0     2369 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datadescriptions/clsdatadescription.py
--rw-r--r--   0        0        0      260 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datadescriptions/datadescription.py
--rw-r--r--   0        0        0     1247 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datadescriptions/inputdatadescriptions.py
--rw-r--r--   0        0        0     2687 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datadescriptions/objdetdatadescription.py
--rw-r--r--   0        0        0     5136 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datadescriptions/outputdatadescriptions.py
--rw-r--r--   0        0        0     2734 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datadescriptions/regdatadescription.py
--rw-r--r--   0        0        0     2996 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datadescriptions/semsegdatadescritption.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datainfolistings/__init__.py
--rw-r--r--   0        0        0     4942 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datainfolistings/clsdatainfolisting.py
--rw-r--r--   0        0        0      493 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datainfolistings/datainfolisting.py
--rw-r--r--   0        0        0     3905 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datainfolistings/objdetdatainfolisting.py
--rw-r--r--   0        0        0     2585 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datainfolistings/semsegdatainfolisting.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datainfos/__init__.py
--rw-r--r--   0        0        0     2388 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datainfos/clsdatainfo.py
--rw-r--r--   0        0        0      458 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datainfos/datainfo.py
--rw-r--r--   0        0        0      755 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datainfos/imagedatainfo.py
--rw-r--r--   0        0        0     1120 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datainfos/objdetdatainfo.py
--rw-r--r--   0        0        0     1112 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datainfos/semsegdatainfo.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataiterators/__init__.py
--rw-r--r--   0        0        0     2783 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataiterators/boundingboxdataiterator.py
--rw-r--r--   0        0        0      560 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataiterators/dataiterator.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataloaders/__init__.py
--rw-r--r--   0        0        0     2229 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataloaders/cachedimageloader.py
--rw-r--r--   0        0        0     1094 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataloaders/clsdataloader.py
--rw-r--r--   0        0        0      747 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataloaders/dataloader.py
--rw-r--r--   0        0        0     2934 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataloaders/dfloaders.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataloaders/factories/__init__.py
--rw-r--r--   0        0        0      516 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataloaders/factories/dfloaderfactory.py
--rw-r--r--   0        0        0      509 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataloaders/factories/imageloaderfactory.py
--rw-r--r--   0        0        0     1572 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataloaders/imageloaders.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataloaders/interfaces/__init__.py
--rw-r--r--   0        0        0      338 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataloaders/interfaces/dfloader.py
--rw-r--r--   0        0        0      753 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataloaders/interfaces/imageloader.py
--rw-r--r--   0        0        0     1137 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataloaders/objdetdataloader.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataloaders/semseg/__init__.py
--rw-r--r--   0        0        0     1615 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataloaders/semseg/cytransformmaskimage.pyx
--rw-r--r--   0        0        0     1938 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataloaders/semseg/semsegdataloader.py
--rw-r--r--   0        0        0      844 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/dataloaders/semseg/transformmaskimage.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datasets/__init__.py
--rw-r--r--   0        0        0     4453 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datasets/clsclassinfo.py
--rw-r--r--   0        0        0     1546 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datasets/dataset.py
--rw-r--r--   0        0        0     4914 2023-06-05 20:18:16.131982 niceml-0.4.0/niceml/data/datasets/dfdataset.py
--rw-r--r--   0        0        0     5362 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/datasets/genericdataset.py
--rw-r--r--   0        0        0     1088 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/datasets/healthdataset.py
--rw-r--r--   0        0        0     1147 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/datasets/sinusdataset.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/datashuffler/__init__.py
--rw-r--r--   0        0        0      603 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/datashuffler/datashuffler.py
--rw-r--r--   0        0        0      536 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/datashuffler/defaultshuffler.py
--rw-r--r--   0        0        0     2613 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/datashuffler/uniformdistributionshuffler.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/datastatsgenerator/__init__.py
--rw-r--r--   0        0        0      426 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/datastatsgenerator/datastatsgenerator.py
--rw-r--r--   0        0        0      472 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/datastatsgenerator/defaultstatsgenerator.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/netdataloggers/__init__.py
--rw-r--r--   0        0        0     1952 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/netdataloggers/netdatalogger.py
--rw-r--r--   0        0        0     4732 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/netdataloggers/objdetnetdatalogger.py
--rw-r--r--   0        0        0     5023 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/netdataloggers/semsegnetdatalogger.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/storages/__init__.py
--rw-r--r--   0        0        0     3013 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/storages/fsfilesystemstorage.py
--rw-r--r--   0        0        0     3485 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/storages/fsspecstorage.py
--rw-r--r--   0        0        0     2306 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/storages/localstorage.py
--rw-r--r--   0        0        0      898 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/storages/storagehandler.py
--rw-r--r--   0        0        0      973 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/data/storages/storageinterface.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/callbacks/__init__.py
--rw-r--r--   0        0        0     3566 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/callbacks/callback_factories.py
--rw-r--r--   0        0        0     1662 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/callbacks/csvlogger.py
--rw-r--r--   0        0        0     4227 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/callbacks/modelcheckpoint.py
--rw-r--r--   0        0        0      922 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/callbacks/nancheckcallback.py
--rw-r--r--   0        0        0      929 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/kerasmetrics.py
--rw-r--r--   0        0        0     1404 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/kerasmodelloader.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/learners/__init__.py
--rw-r--r--   0        0        0     2344 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/learners/defaultlearner.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/losses/__init__.py
--rw-r--r--   0        0        0     1488 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/losses/categoricalfocalloss.py
--rw-r--r--   0        0        0     3957 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/losses/objdetlosses.py
--rw-r--r--   0        0        0     2055 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/losses/semseglosses.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/metrics/__init__.py
--rw-r--r--   0        0        0     3048 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/metrics/objdetmetrics.py
--rw-r--r--   0        0        0     2212 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/metrics/semsegmetrics.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/modelcompiler/__init__.py
--rw-r--r--   0        0        0     2136 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/modelcompiler/defaultmodelcompiler.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/models/__init__.py
--rw-r--r--   0        0        0     3701 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/models/clsmodelfactory.py
--rw-r--r--   0        0        0     2530 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/models/layerfactory.py
--rw-r--r--   0        0        0     1569 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/models/loadweightsmodelfactory.py
--rw-r--r--   0        0        0     1979 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/models/mlp.py
--rw-r--r--   0        0        0     2250 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/models/mobilenet.py
--rw-r--r--   0        0        0     1813 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/models/premodellayers.py
--rw-r--r--   0        0        0     7749 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/models/retinanet.py
--rw-r--r--   0        0        0    11007 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/models/unets.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/optimizers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/optimizers/schedules/__init__.py
--rw-r--r--   0        0        0     1158 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/dlframeworks/tensorflow/optimizers/schedules/cycliclrschedule.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/__init__.py
--rw-r--r--   0        0        0     4437 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/confextractionmetafunction.py
--rw-r--r--   0        0        0     1431 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/expdatalocalstorageloader.py
--rw-r--r--   0        0        0     3277 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/expdatastorageloader.py
--rw-r--r--   0        0        0     4447 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/experimentcontext.py
--rw-r--r--   0        0        0    14860 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/experimentdata.py
--rw-r--r--   0        0        0     2109 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/experimentdownloader.py
--rw-r--r--   0        0        0      673 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/experimenterrors.py
--rw-r--r--   0        0        0     3122 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/experimentinfo.py
--rw-r--r--   0        0        0    12258 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/experimentmanager.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/experimenttests/__init__.py
--rw-r--r--   0        0        0     1790 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/experimenttests/checkfilesfolderstest.py
--rw-r--r--   0        0        0      904 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/experimenttests/exptests.py
--rw-r--r--   0        0        0     1667 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/experimenttests/metriccheck.py
--rw-r--r--   0        0        0     2320 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/experimenttests/testinitializer.py
--rw-r--r--   0        0        0     3521 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/experimenttests/validateexps.py
--rw-r--r--   0        0        0     3007 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/expfilenames.py
--rw-r--r--   0        0        0     3153 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/expoutinitializer.py
--rw-r--r--   0        0        0     1199 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/exppathfinder.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/filters/__init__.py
--rw-r--r--   0        0        0     1922 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/filters/datefilter.py
--rw-r--r--   0        0        0      547 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/filters/experimentfilter.py
--rw-r--r--   0        0        0     2142 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/filters/expselectionfilter.py
--rw-r--r--   0        0        0     1867 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/filters/selectboxfilter.py
--rw-r--r--   0        0        0     2911 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/filters/sliderfilter.py
--rw-r--r--   0        0        0     2304 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/loaddatafunctions.py
--rw-r--r--   0        0        0      828 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/loadexpinfo.py
--rw-r--r--   0        0        0     6149 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/localexperimentcache.py
--rw-r--r--   0        0        0     2683 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/metafunctions.py
--rw-r--r--   0        0        0     1598 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/metainfotables.py
--rw-r--r--   0        0        0     3300 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/metalists.py
--rw-r--r--   0        0        0      512 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/metatablefactory.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/schemas/__init__.py
--rw-r--r--   0        0        0      669 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/schemas/baseexpschema.py
--rw-r--r--   0        0        0      637 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/schemas/expdocstring.py
--rw-r--r--   0        0        0     2533 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/schemas/expmember.py
--rw-r--r--   0        0        0     1416 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/schemas/objdetexpschema.py
--rw-r--r--   0        0        0     1210 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/schemas/parquetframeexpmember.py
--rw-r--r--   0        0        0     1474 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/schemas/sampleexpschemas.py
--rw-r--r--   0        0        0      390 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/schemas/schemalist.py
--rw-r--r--   0        0        0      788 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/schemas/schemavalidation.py
--rw-r--r--   0        0        0     2179 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/experiments/schemas/yamlexpmember.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mkdocs/__init__.py
--rw-r--r--   0        0        0      517 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mkdocs/mdgraph.py
--rw-r--r--   0        0        0      839 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mkdocs/mdjob.py
--rw-r--r--   0        0        0     1042 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mkdocs/mdop.py
--rw-r--r--   0        0        0     1189 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mkdocs/mdtable.py
--rw-r--r--   0        0        0     1422 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mkdocs/schemadocgeneration.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mlcomponents/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mlcomponents/callbacks/__init__.py
--rw-r--r--   0        0        0      921 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mlcomponents/callbacks/callbackinitializer.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mlcomponents/learners/__init__.py
--rw-r--r--   0        0        0     1125 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mlcomponents/learners/fitgenerators.py
--rw-r--r--   0        0        0      994 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mlcomponents/learners/learner.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mlcomponents/modelcompiler/__init__.py
--rw-r--r--   0        0        0      575 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mlcomponents/modelcompiler/modelcompiler.py
--rw-r--r--   0        0        0      563 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mlcomponents/modelcompiler/modelcustomloadobjects.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mlcomponents/modelloader/__init__.py
--rw-r--r--   0        0        0      600 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mlcomponents/modelloader/modelloader.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mlcomponents/models/__init__.py
--rw-r--r--   0        0        0      160 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mlcomponents/models/modelbundle.py
--rw-r--r--   0        0        0      476 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mlcomponents/models/modelfactory.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.135982 niceml-0.4.0/niceml/mlcomponents/objdet/__init__.py
--rw-r--r--   0        0        0     7607 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/objdet/anchorencoding.py
--rw-r--r--   0        0        0     2905 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/objdet/anchorgenerator.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/predictionhandlers/__init__.py
--rw-r--r--   0        0        0     1404 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/predictionhandlers/combinationpredictionhandler.py
--rw-r--r--   0        0        0     6251 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/predictionhandlers/objdetpredictionhandler.py
--rw-r--r--   0        0        0     1383 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/predictionhandlers/predictionhandler.py
--rw-r--r--   0        0        0    10584 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/predictionhandlers/semsegpredictionhandler.py
--rw-r--r--   0        0        0     4896 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/predictionhandlers/tensorpredictionhandler.py
--rw-r--r--   0        0        0     2550 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/predictionhandlers/vectorpredictionhandler.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/__init__.py
--rw-r--r--   0        0        0      836 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/analyzer.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/dataframes/__init__.py
--rw-r--r--   0        0        0     4118 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/dataframes/clsmetric.py
--rw-r--r--   0        0        0     2320 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/dataframes/dfanalyzer.py
--rw-r--r--   0        0        0     3806 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/dataframes/multilabeltobinary.py
--rw-r--r--   0        0        0     3328 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/dataframes/regmetric.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/instancefinders/__init__.py
--rw-r--r--   0        0        0     1709 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/instancefinders/instancecontour.py
--rw-r--r--   0        0        0      603 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/instancefinders/instancefinder.py
--rw-r--r--   0        0        0     1658 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/instancefinders/maskinstance.py
--rw-r--r--   0        0        0     3007 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/instancefinders/multichannelinstancefinder.py
--rw-r--r--   0        0        0      723 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/multiresultanalyzer.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/tensors/__init__.py
--rw-r--r--   0        0        0     1181 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/tensors/cytensoriou.pyx
--rw-r--r--   0        0        0     2412 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/tensors/semsegdataiterator.py
--rw-r--r--   0        0        0      611 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/tensors/tensordataiterators.py
--rw-r--r--   0        0        0     1959 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/tensors/tensordfmetricwrapper.py
--rw-r--r--   0        0        0     3051 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/tensors/tensorgraphanalyzer.py
--rw-r--r--   0        0        0     2223 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/tensors/tensoriou.py
--rw-r--r--   0        0        0     1357 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/tensors/tensormetric.py
--rw-r--r--   0        0        0     1698 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/tensors/tensorvisualizer.py
--rw-r--r--   0        0        0     2208 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/resultanalyzers/tensors/zarrdataiterator.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/targettransformer/__init__.py
--rw-r--r--   0        0        0      630 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/targettransformer/imageinputtransformer.py
--rw-r--r--   0        0        0     1770 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/targettransformer/objdettargettransformer.py
--rw-r--r--   0        0        0     2410 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/targettransformer/semsegtargettransformer.py
--rw-r--r--   0        0        0      649 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/targettransformer/targettransformer.py
--rw-r--r--   0        0        0     1854 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/mlcomponents/targettransformer/targettransformercls.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/py.typed
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/scripts/__init__.py
--rw-r--r--   0        0        0     2031 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/scripts/hydraconfreader.py
--rw-r--r--   0        0        0      745 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/scripts/rundatatests.py
--rw-r--r--   0        0        0     2457 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/scripts/splitdatasetindex.py
--rw-r--r--   0        0        0     1530 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/storages/abs.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/utilities/__init__.py
--rw-r--r--   0        0        0   207256 2023-06-05 20:18:16.139982 niceml-0.4.0/niceml/utilities/assets/bg_images/andrew-neel-slRYlH9ttzc-unsplash.jpg
--rw-r--r--   0        0        0   585133 2023-06-05 20:18:16.143982 niceml-0.4.0/niceml/utilities/assets/bg_images/karthik-sreenivas-1N_78ShYQFg-unsplash.jpg
--rw-r--r--   0        0        0   292520 2023-06-05 20:18:16.143982 niceml-0.4.0/niceml/utilities/assets/bg_images/neha-maheen-mahfin-FtiAj6ggKnU-unsplash.jpg
--rw-r--r--   0        0        0   424191 2023-06-05 20:18:16.143982 niceml-0.4.0/niceml/utilities/assets/bg_images/yousef-espanioly-8ja-Ns8iqO4-unsplash.jpg
--rw-r--r--   0        0        0    48852 2023-06-05 20:18:16.143982 niceml-0.4.0/niceml/utilities/assets/fonts/DMMono-Regular.ttf
--rw-r--r--   0        0        0    72744 2023-06-05 20:18:16.143982 niceml-0.4.0/niceml/utilities/assets/fonts/Dosis-Regular.ttf
--rw-r--r--   0        0        0    33040 2023-06-05 20:18:16.143982 niceml-0.4.0/niceml/utilities/assets/fonts/Heebo-Regular.ttf
--rw-r--r--   0        0        0    38304 2023-06-05 20:18:16.143982 niceml-0.4.0/niceml/utilities/assets/fonts/Karla-Regular.ttf
--rw-r--r--   0        0        0   129796 2023-06-05 20:18:16.147982 niceml-0.4.0/niceml/utilities/assets/fonts/OpenSans-Regular.ttf
--rw-r--r--   0        0        0    63900 2023-06-05 20:18:16.147982 niceml-0.4.0/niceml/utilities/assets/fonts/Oswald-Regular.ttf
--rw-r--r--   0        0        0    67476 2023-06-05 20:18:16.147982 niceml-0.4.0/niceml/utilities/assets/fonts/OxygenMono-Regular.ttf
--rw-r--r--   0        0        0    86908 2023-06-05 20:18:16.147982 niceml-0.4.0/niceml/utilities/assets/fonts/RobotoMono-Regular.ttf
--rw-r--r--   0        0        0   124236 2023-06-05 20:18:16.147982 niceml-0.4.0/niceml/utilities/assets/fonts/Rubik-Regular.ttf
--rw-r--r--   0        0        0   299684 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/assets/fonts/Ubuntu-Regular.ttf
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/boundingboxes/__init__.py
--rw-r--r--   0        0        0     8325 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/boundingboxes/bboxconversion.py
--rw-r--r--   0        0        0     3619 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/boundingboxes/bboxdrawing.py
--rw-r--r--   0        0        0     2459 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/boundingboxes/bboxencoding.py
--rw-r--r--   0        0        0     3748 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/boundingboxes/bboxlabeling.py
--rw-r--r--   0        0        0    10406 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/boundingboxes/boundingbox.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/boundingboxes/filtering/__init__.py
--rw-r--r--   0        0        0     3515 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/boundingboxes/filtering/nmsfilter.py
--rw-r--r--   0        0        0     2978 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/boundingboxes/filtering/predictionfilter.py
--rw-r--r--   0        0        0      231 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/boundingboxes/filtering/predictionfiltertype.py
--rw-r--r--   0        0        0     1427 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/boundingboxes/filtering/thresholdfilter.py
--rw-r--r--   0        0        0     3995 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/boundingboxes/filtering/unifiedboxfilter.py
--rw-r--r--   0        0        0     3163 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/chartutils.py
--rw-r--r--   0        0        0     3094 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/checksums.py
--rw-r--r--   0        0        0     2752 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/colorutils.py
--rw-r--r--   0        0        0     3633 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/commonutils.py
--rw-r--r--   0        0        0     3292 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/copyutils.py
--rw-r--r--   0        0        0     1229 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/encoding.py
--rw-r--r--   0        0        0     3846 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/factoryutils.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/filtering/__init__.py
--rw-r--r--   0        0        0     2138 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/filtering/probabilityclassselector.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/fsspec/__init__.py
--rw-r--r--   0        0        0     3020 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/fsspec/locationutils.py
--rw-r--r--   0        0        0     1938 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/gitutils.py
--rw-r--r--   0        0        0     3582 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/hydrautils.py
--rw-r--r--   0        0        0     1716 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/idutils.py
--rw-r--r--   0        0        0    18139 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/imagegeneration.py
--rw-r--r--   0        0        0     2720 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/imageloading.py
--rw-r--r--   0        0        0     4667 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/imagesize.py
--rw-r--r--   0        0        0     4951 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/imageutils.py
--rw-r--r--   0        0        0     3066 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/instancelabeling.py
--rw-r--r--   0        0        0     2256 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/instancelabelmatching.py
--rw-r--r--   0        0        0     5785 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/ioumatrix.py
--rw-r--r--   0        0        0     9836 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/ioutils.py
--rw-r--r--   0        0        0      284 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/logutils.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/masks/__init__.py
--rw-r--r--   0        0        0     1208 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/masks/cymaskdownscale.pyx
--rw-r--r--   0        0        0     1371 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/masks/maskdownscale.py
--rw-r--r--   0        0        0     8463 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/matchingresult.py
--rw-r--r--   0        0        0     2553 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/omegaconfutils.py
--rw-r--r--   0        0        0     2032 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/pytestutils.py
--rw-r--r--   0        0        0     6961 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/readwritelock.py
--rw-r--r--   0        0        0      590 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/regexutils.py
--rw-r--r--   0        0        0        0 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/semseg/__init__.py
--rw-r--r--   0        0        0     1885 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/semseg/semsegdrawing.py
--rw-r--r--   0        0        0     1664 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/semseg/semseginstancelabeling.py
--rw-r--r--   0        0        0     1457 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/sinusgeneration.py
--rw-r--r--   0        0        0     5710 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/splitutils.py
--rw-r--r--   0        0        0     1317 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/thumbnailshower.py
--rw-r--r--   0        0        0      472 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/timeutils.py
--rw-r--r--   0        0        0     2789 2023-06-05 20:18:16.151982 niceml-0.4.0/niceml/utilities/userselection.py
--rw-r--r--   0        0        0     3657 2023-06-05 20:18:58.088643 niceml-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4357 1970-01-01 00:00:00.000000 niceml-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-22 07:54:29.092107 niceml-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1135 2023-06-22 07:54:29.092107 niceml-0.4.1/README.md
+-rw-r--r--   0        0        0       22 2023-06-22 07:55:09.688805 niceml-0.4.1/niceml/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/cli/__init__.py
+-rw-r--r--   0        0        0     3070 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/cli/clicommands.py
+-rw-r--r--   0        0        0      228 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/cli/climain.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/config/__init__.py
+-rw-r--r--   0        0        0     9485 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/config/configschemas.py
+-rw-r--r--   0        0        0      889 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/config/envconfig.py
+-rw-r--r--   0        0        0     3907 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/config/hydra.py
+-rw-r--r--   0        0        0      744 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/config/subsetnames.py
+-rw-r--r--   0        0        0      310 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/config/trainparams.py
+-rw-r--r--   0        0        0      506 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/config/writeopconfig.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dagster/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dagster/jobs/__init__.py
+-rw-r--r--   0        0        0     2432 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dagster/jobs/jobs.py
+-rw-r--r--   0        0        0      512 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dagster/jobs/repository.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dagster/ops/__init__.py
+-rw-r--r--   0        0        0     2090 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dagster/ops/analysis.py
+-rw-r--r--   0        0        0     2317 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dagster/ops/copyexp.py
+-rw-r--r--   0        0        0     3900 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dagster/ops/cropnumbers.py
+-rw-r--r--   0        0        0      921 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dagster/ops/datageneration.py
+-rw-r--r--   0        0        0     3396 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dagster/ops/evalcopyexp.py
+-rw-r--r--   0        0        0     2058 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dagster/ops/experiment.py
+-rw-r--r--   0        0        0     1176 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dagster/ops/exptests.py
+-rw-r--r--   0        0        0     4556 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dagster/ops/imagetotable.py
+-rw-r--r--   0        0        0     2220 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dagster/ops/localizeexperiment.py
+-rw-r--r--   0        0        0     5799 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dagster/ops/prediction.py
+-rw-r--r--   0        0        0     3003 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dagster/ops/splitdata.py
+-rw-r--r--   0        0        0     2889 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dagster/ops/train.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dagster/resources/__init__.py
+-rw-r--r--   0        0        0     3668 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dagster/resources/locations.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/__init__.py
+-rw-r--r--   0        0        0     6736 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/binprobvisu.py
+-rw-r--r--   0        0        0     4033 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/cam.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/components/__init__.py
+-rw-r--r--   0        0        0     3870 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/components/downloadexpviscomponent.py
+-rw-r--r--   0        0        0     4603 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/components/expviscomponent.py
+-rw-r--r--   0        0        0     1835 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/components/linearviscomponent.py
+-rw-r--r--   0        0        0     1329 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/components/metaviscomponent.py
+-rw-r--r--   0        0        0     3769 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/components/prefixviscomponent.py
+-rw-r--r--   0        0        0     2892 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/components/selectionviscomponent.py
+-rw-r--r--   0        0        0     1446 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/configviscomponent.py
+-rw-r--r--   0        0        0     3006 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/dashboard.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/expvisuhelper.py
+-rw-r--r--   0        0        0     3126 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/imagenetdataloggerviscomponent.py
+-rw-r--r--   0        0        0     3294 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/metricviscomponent.py
+-rw-r--r--   0        0        0      293 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/netdataloggerviscomponent.py
+-rw-r--r--   0        0        0     5961 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/remotettrainutils.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/visualizers/__init__.py
+-rw-r--r--   0        0        0     3125 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/visualizers/boundingboxvisualizer.py
+-rw-r--r--   0        0        0     4554 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/visualizers/imagevisualizer.py
+-rw-r--r--   0        0        0     3206 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/dashboard/visualizers/maskvisualizer.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/augmentation/__init__.py
+-rw-r--r--   0        0        0      362 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/augmentation/augmentation.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/datadescriptions/__init__.py
+-rw-r--r--   0        0        0     2369 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/datadescriptions/clsdatadescription.py
+-rw-r--r--   0        0        0      260 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/datadescriptions/datadescription.py
+-rw-r--r--   0        0        0     1247 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/datadescriptions/inputdatadescriptions.py
+-rw-r--r--   0        0        0     2687 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/datadescriptions/objdetdatadescription.py
+-rw-r--r--   0        0        0     5136 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/datadescriptions/outputdatadescriptions.py
+-rw-r--r--   0        0        0     2734 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/datadescriptions/regdatadescription.py
+-rw-r--r--   0        0        0     2996 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/datadescriptions/semsegdatadescritption.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/datainfolistings/__init__.py
+-rw-r--r--   0        0        0     4942 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/datainfolistings/clsdatainfolisting.py
+-rw-r--r--   0        0        0      493 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/datainfolistings/datainfolisting.py
+-rw-r--r--   0        0        0     3905 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/datainfolistings/objdetdatainfolisting.py
+-rw-r--r--   0        0        0     2585 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/datainfolistings/semsegdatainfolisting.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/datainfos/__init__.py
+-rw-r--r--   0        0        0     2388 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/datainfos/clsdatainfo.py
+-rw-r--r--   0        0        0      458 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/datainfos/datainfo.py
+-rw-r--r--   0        0        0      755 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/datainfos/imagedatainfo.py
+-rw-r--r--   0        0        0     1120 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/datainfos/objdetdatainfo.py
+-rw-r--r--   0        0        0     1112 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/datainfos/semsegdatainfo.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/dataiterators/__init__.py
+-rw-r--r--   0        0        0     2783 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/dataiterators/boundingboxdataiterator.py
+-rw-r--r--   0        0        0      560 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/dataiterators/dataiterator.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/dataloaders/__init__.py
+-rw-r--r--   0        0        0     2229 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/dataloaders/cachedimageloader.py
+-rw-r--r--   0        0        0     1094 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/dataloaders/clsdataloader.py
+-rw-r--r--   0        0        0      747 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/dataloaders/dataloader.py
+-rw-r--r--   0        0        0     2934 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/dataloaders/dfloaders.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/dataloaders/factories/__init__.py
+-rw-r--r--   0        0        0      516 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/dataloaders/factories/dfloaderfactory.py
+-rw-r--r--   0        0        0      509 2023-06-22 07:54:29.100107 niceml-0.4.1/niceml/data/dataloaders/factories/imageloaderfactory.py
+-rw-r--r--   0        0        0     1572 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/dataloaders/imageloaders.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/dataloaders/interfaces/__init__.py
+-rw-r--r--   0        0        0      338 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/dataloaders/interfaces/dfloader.py
+-rw-r--r--   0        0        0      753 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/dataloaders/interfaces/imageloader.py
+-rw-r--r--   0        0        0     1137 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/dataloaders/objdetdataloader.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/dataloaders/semseg/__init__.py
+-rw-r--r--   0        0        0     1615 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/dataloaders/semseg/cytransformmaskimage.pyx
+-rw-r--r--   0        0        0     1938 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/dataloaders/semseg/semsegdataloader.py
+-rw-r--r--   0        0        0      844 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/dataloaders/semseg/transformmaskimage.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/datasets/__init__.py
+-rw-r--r--   0        0        0     4453 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/datasets/clsclassinfo.py
+-rw-r--r--   0        0        0     1546 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/datasets/dataset.py
+-rw-r--r--   0        0        0     4914 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/datasets/dfdataset.py
+-rw-r--r--   0        0        0     5362 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/datasets/genericdataset.py
+-rw-r--r--   0        0        0     1088 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/datasets/healthdataset.py
+-rw-r--r--   0        0        0     1147 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/datasets/sinusdataset.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/datashuffler/__init__.py
+-rw-r--r--   0        0        0      603 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/datashuffler/datashuffler.py
+-rw-r--r--   0        0        0      536 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/datashuffler/defaultshuffler.py
+-rw-r--r--   0        0        0     2613 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/datashuffler/uniformdistributionshuffler.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/datastatsgenerator/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/datastatsgenerator/datastatsgenerator.py
+-rw-r--r--   0        0        0      472 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/datastatsgenerator/defaultstatsgenerator.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/netdataloggers/__init__.py
+-rw-r--r--   0        0        0     1952 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/netdataloggers/netdatalogger.py
+-rw-r--r--   0        0        0     4732 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/netdataloggers/objdetnetdatalogger.py
+-rw-r--r--   0        0        0     5023 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/netdataloggers/semsegnetdatalogger.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/storages/__init__.py
+-rw-r--r--   0        0        0     3013 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/storages/fsfilesystemstorage.py
+-rw-r--r--   0        0        0     3485 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/storages/fsspecstorage.py
+-rw-r--r--   0        0        0     2306 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/storages/localstorage.py
+-rw-r--r--   0        0        0      898 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/storages/storagehandler.py
+-rw-r--r--   0        0        0      973 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/data/storages/storageinterface.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/callbacks/__init__.py
+-rw-r--r--   0        0        0     3566 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/callbacks/callback_factories.py
+-rw-r--r--   0        0        0     1662 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/callbacks/csvlogger.py
+-rw-r--r--   0        0        0     4227 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/callbacks/modelcheckpoint.py
+-rw-r--r--   0        0        0      922 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/callbacks/nancheckcallback.py
+-rw-r--r--   0        0        0      929 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/kerasmetrics.py
+-rw-r--r--   0        0        0     1404 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/kerasmodelloader.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/learners/__init__.py
+-rw-r--r--   0        0        0     2344 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/learners/defaultlearner.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/losses/__init__.py
+-rw-r--r--   0        0        0     1488 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/losses/categoricalfocalloss.py
+-rw-r--r--   0        0        0     3957 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/losses/objdetlosses.py
+-rw-r--r--   0        0        0     2055 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/losses/semseglosses.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/metrics/__init__.py
+-rw-r--r--   0        0        0     3048 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/metrics/objdetmetrics.py
+-rw-r--r--   0        0        0     2212 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/metrics/semsegmetrics.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/modelcompiler/__init__.py
+-rw-r--r--   0        0        0     2136 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/modelcompiler/defaultmodelcompiler.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/models/__init__.py
+-rw-r--r--   0        0        0     3701 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/models/clsmodelfactory.py
+-rw-r--r--   0        0        0     2530 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/models/layerfactory.py
+-rw-r--r--   0        0        0     1569 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/models/loadweightsmodelfactory.py
+-rw-r--r--   0        0        0     1979 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/models/mlp.py
+-rw-r--r--   0        0        0     2250 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/models/mobilenet.py
+-rw-r--r--   0        0        0     1813 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/models/premodellayers.py
+-rw-r--r--   0        0        0     7749 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/models/retinanet.py
+-rw-r--r--   0        0        0    11007 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/models/unets.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/optimizers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/optimizers/schedules/__init__.py
+-rw-r--r--   0        0        0     1158 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/dlframeworks/tensorflow/optimizers/schedules/cycliclrschedule.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/__init__.py
+-rw-r--r--   0        0        0     4437 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/confextractionmetafunction.py
+-rw-r--r--   0        0        0     1431 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/expdatalocalstorageloader.py
+-rw-r--r--   0        0        0     3277 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/expdatastorageloader.py
+-rw-r--r--   0        0        0     4447 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/experimentcontext.py
+-rw-r--r--   0        0        0    14860 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/experimentdata.py
+-rw-r--r--   0        0        0     2109 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/experimentdownloader.py
+-rw-r--r--   0        0        0      673 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/experimenterrors.py
+-rw-r--r--   0        0        0     3122 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/experimentinfo.py
+-rw-r--r--   0        0        0    12258 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/experimentmanager.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/experimenttests/__init__.py
+-rw-r--r--   0        0        0     1790 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/experimenttests/checkfilesfolderstest.py
+-rw-r--r--   0        0        0      904 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/experimenttests/exptests.py
+-rw-r--r--   0        0        0     1667 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/experimenttests/metriccheck.py
+-rw-r--r--   0        0        0     2320 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/experimenttests/testinitializer.py
+-rw-r--r--   0        0        0     3521 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/experimenttests/validateexps.py
+-rw-r--r--   0        0        0     3007 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/expfilenames.py
+-rw-r--r--   0        0        0     3153 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/expoutinitializer.py
+-rw-r--r--   0        0        0     1199 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/exppathfinder.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/filters/__init__.py
+-rw-r--r--   0        0        0     1922 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/filters/datefilter.py
+-rw-r--r--   0        0        0      547 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/filters/experimentfilter.py
+-rw-r--r--   0        0        0     2142 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/filters/expselectionfilter.py
+-rw-r--r--   0        0        0     1867 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/filters/selectboxfilter.py
+-rw-r--r--   0        0        0     2911 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/filters/sliderfilter.py
+-rw-r--r--   0        0        0     2304 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/loaddatafunctions.py
+-rw-r--r--   0        0        0      828 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/loadexpinfo.py
+-rw-r--r--   0        0        0     6149 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/localexperimentcache.py
+-rw-r--r--   0        0        0     2683 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/metafunctions.py
+-rw-r--r--   0        0        0     1598 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/metainfotables.py
+-rw-r--r--   0        0        0     3300 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/metalists.py
+-rw-r--r--   0        0        0      512 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/metatablefactory.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/schemas/__init__.py
+-rw-r--r--   0        0        0      669 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/schemas/baseexpschema.py
+-rw-r--r--   0        0        0      637 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/schemas/expdocstring.py
+-rw-r--r--   0        0        0     2533 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/schemas/expmember.py
+-rw-r--r--   0        0        0     1416 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/schemas/objdetexpschema.py
+-rw-r--r--   0        0        0     1210 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/schemas/parquetframeexpmember.py
+-rw-r--r--   0        0        0     1474 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/schemas/sampleexpschemas.py
+-rw-r--r--   0        0        0      390 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/schemas/schemalist.py
+-rw-r--r--   0        0        0      788 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/schemas/schemavalidation.py
+-rw-r--r--   0        0        0     2179 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/experiments/schemas/yamlexpmember.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/mkdocs/__init__.py
+-rw-r--r--   0        0        0      517 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/mkdocs/mdgraph.py
+-rw-r--r--   0        0        0      839 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/mkdocs/mdjob.py
+-rw-r--r--   0        0        0     1042 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/mkdocs/mdop.py
+-rw-r--r--   0        0        0     1189 2023-06-22 07:54:29.104107 niceml-0.4.1/niceml/mkdocs/mdtable.py
+-rw-r--r--   0        0        0     1422 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mkdocs/schemadocgeneration.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/callbacks/__init__.py
+-rw-r--r--   0        0        0      921 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/callbacks/callbackinitializer.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/learners/__init__.py
+-rw-r--r--   0        0        0     1125 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/learners/fitgenerators.py
+-rw-r--r--   0        0        0      994 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/learners/learner.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/modelcompiler/__init__.py
+-rw-r--r--   0        0        0      575 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/modelcompiler/modelcompiler.py
+-rw-r--r--   0        0        0      563 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/modelcompiler/modelcustomloadobjects.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/modelloader/__init__.py
+-rw-r--r--   0        0        0      600 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/modelloader/modelloader.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/models/__init__.py
+-rw-r--r--   0        0        0      160 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/models/modelbundle.py
+-rw-r--r--   0        0        0      476 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/models/modelfactory.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/objdet/__init__.py
+-rw-r--r--   0        0        0     7607 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/objdet/anchorencoding.py
+-rw-r--r--   0        0        0     2905 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/objdet/anchorgenerator.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/predictionhandlers/__init__.py
+-rw-r--r--   0        0        0     1404 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/predictionhandlers/combinationpredictionhandler.py
+-rw-r--r--   0        0        0     6251 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/predictionhandlers/objdetpredictionhandler.py
+-rw-r--r--   0        0        0     1383 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/predictionhandlers/predictionhandler.py
+-rw-r--r--   0        0        0    10584 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/predictionhandlers/semsegpredictionhandler.py
+-rw-r--r--   0        0        0     4896 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/predictionhandlers/tensorpredictionhandler.py
+-rw-r--r--   0        0        0     2550 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/predictionhandlers/vectorpredictionhandler.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/__init__.py
+-rw-r--r--   0        0        0      836 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/analyzer.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/dataframes/__init__.py
+-rw-r--r--   0        0        0     4118 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/dataframes/clsmetric.py
+-rw-r--r--   0        0        0     2320 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/dataframes/dfanalyzer.py
+-rw-r--r--   0        0        0     3806 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/dataframes/multilabeltobinary.py
+-rw-r--r--   0        0        0     3328 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/dataframes/regmetric.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/instancefinders/__init__.py
+-rw-r--r--   0        0        0     1709 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/instancefinders/instancecontour.py
+-rw-r--r--   0        0        0      603 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/instancefinders/instancefinder.py
+-rw-r--r--   0        0        0     1658 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/instancefinders/maskinstance.py
+-rw-r--r--   0        0        0     3007 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/instancefinders/multichannelinstancefinder.py
+-rw-r--r--   0        0        0      723 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/multiresultanalyzer.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/tensors/__init__.py
+-rw-r--r--   0        0        0     1181 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/tensors/cytensoriou.pyx
+-rw-r--r--   0        0        0     2412 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/tensors/semsegdataiterator.py
+-rw-r--r--   0        0        0      611 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/tensors/tensordataiterators.py
+-rw-r--r--   0        0        0     1959 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/tensors/tensordfmetricwrapper.py
+-rw-r--r--   0        0        0     3051 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/tensors/tensorgraphanalyzer.py
+-rw-r--r--   0        0        0     2223 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/tensors/tensoriou.py
+-rw-r--r--   0        0        0     1357 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/tensors/tensormetric.py
+-rw-r--r--   0        0        0     1698 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/tensors/tensorvisualizer.py
+-rw-r--r--   0        0        0     2208 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/resultanalyzers/tensors/zarrdataiterator.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/targettransformer/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/targettransformer/imageinputtransformer.py
+-rw-r--r--   0        0        0     1770 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/targettransformer/objdettargettransformer.py
+-rw-r--r--   0        0        0     2410 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/targettransformer/semsegtargettransformer.py
+-rw-r--r--   0        0        0      649 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/targettransformer/targettransformer.py
+-rw-r--r--   0        0        0     1854 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/mlcomponents/targettransformer/targettransformercls.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/py.typed
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/scripts/__init__.py
+-rw-r--r--   0        0        0     2031 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/scripts/hydraconfreader.py
+-rw-r--r--   0        0        0      745 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/scripts/rundatatests.py
+-rw-r--r--   0        0        0     2457 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/scripts/splitdatasetindex.py
+-rw-r--r--   0        0        0     1530 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/storages/abs.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/utilities/__init__.py
+-rw-r--r--   0        0        0   207256 2023-06-22 07:54:29.108107 niceml-0.4.1/niceml/utilities/assets/bg_images/andrew-neel-slRYlH9ttzc-unsplash.jpg
+-rw-r--r--   0        0        0   585133 2023-06-22 07:54:29.112107 niceml-0.4.1/niceml/utilities/assets/bg_images/karthik-sreenivas-1N_78ShYQFg-unsplash.jpg
+-rw-r--r--   0        0        0   292520 2023-06-22 07:54:29.112107 niceml-0.4.1/niceml/utilities/assets/bg_images/neha-maheen-mahfin-FtiAj6ggKnU-unsplash.jpg
+-rw-r--r--   0        0        0   424191 2023-06-22 07:54:29.112107 niceml-0.4.1/niceml/utilities/assets/bg_images/yousef-espanioly-8ja-Ns8iqO4-unsplash.jpg
+-rw-r--r--   0        0        0    48852 2023-06-22 07:54:29.112107 niceml-0.4.1/niceml/utilities/assets/fonts/DMMono-Regular.ttf
+-rw-r--r--   0        0        0    72744 2023-06-22 07:54:29.112107 niceml-0.4.1/niceml/utilities/assets/fonts/Dosis-Regular.ttf
+-rw-r--r--   0        0        0    33040 2023-06-22 07:54:29.112107 niceml-0.4.1/niceml/utilities/assets/fonts/Heebo-Regular.ttf
+-rw-r--r--   0        0        0    38304 2023-06-22 07:54:29.116107 niceml-0.4.1/niceml/utilities/assets/fonts/Karla-Regular.ttf
+-rw-r--r--   0        0        0   129796 2023-06-22 07:54:29.116107 niceml-0.4.1/niceml/utilities/assets/fonts/OpenSans-Regular.ttf
+-rw-r--r--   0        0        0    63900 2023-06-22 07:54:29.116107 niceml-0.4.1/niceml/utilities/assets/fonts/Oswald-Regular.ttf
+-rw-r--r--   0        0        0    67476 2023-06-22 07:54:29.116107 niceml-0.4.1/niceml/utilities/assets/fonts/OxygenMono-Regular.ttf
+-rw-r--r--   0        0        0    86908 2023-06-22 07:54:29.116107 niceml-0.4.1/niceml/utilities/assets/fonts/RobotoMono-Regular.ttf
+-rw-r--r--   0        0        0   124236 2023-06-22 07:54:29.116107 niceml-0.4.1/niceml/utilities/assets/fonts/Rubik-Regular.ttf
+-rw-r--r--   0        0        0   299684 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/assets/fonts/Ubuntu-Regular.ttf
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/boundingboxes/__init__.py
+-rw-r--r--   0        0        0     8325 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/boundingboxes/bboxconversion.py
+-rw-r--r--   0        0        0     3619 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/boundingboxes/bboxdrawing.py
+-rw-r--r--   0        0        0     2459 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/boundingboxes/bboxencoding.py
+-rw-r--r--   0        0        0     3748 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/boundingboxes/bboxlabeling.py
+-rw-r--r--   0        0        0    10406 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/boundingboxes/boundingbox.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/boundingboxes/filtering/__init__.py
+-rw-r--r--   0        0        0     3515 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/boundingboxes/filtering/nmsfilter.py
+-rw-r--r--   0        0        0     2978 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/boundingboxes/filtering/predictionfilter.py
+-rw-r--r--   0        0        0      231 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/boundingboxes/filtering/predictionfiltertype.py
+-rw-r--r--   0        0        0     1427 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/boundingboxes/filtering/thresholdfilter.py
+-rw-r--r--   0        0        0     3995 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/boundingboxes/filtering/unifiedboxfilter.py
+-rw-r--r--   0        0        0     3163 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/chartutils.py
+-rw-r--r--   0        0        0     3094 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/checksums.py
+-rw-r--r--   0        0        0     2752 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/colorutils.py
+-rw-r--r--   0        0        0     3633 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/commonutils.py
+-rw-r--r--   0        0        0     3292 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/copyutils.py
+-rw-r--r--   0        0        0     1229 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/encoding.py
+-rw-r--r--   0        0        0     3846 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/factoryutils.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/filtering/__init__.py
+-rw-r--r--   0        0        0     2138 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/filtering/probabilityclassselector.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/fsspec/__init__.py
+-rw-r--r--   0        0        0     3020 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/fsspec/locationutils.py
+-rw-r--r--   0        0        0     1938 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/gitutils.py
+-rw-r--r--   0        0        0     3582 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/hydrautils.py
+-rw-r--r--   0        0        0     1716 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/idutils.py
+-rw-r--r--   0        0        0    18139 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/imagegeneration.py
+-rw-r--r--   0        0        0     2720 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/imageloading.py
+-rw-r--r--   0        0        0     4667 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/imagesize.py
+-rw-r--r--   0        0        0     4951 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/imageutils.py
+-rw-r--r--   0        0        0     3066 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/instancelabeling.py
+-rw-r--r--   0        0        0     2256 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/instancelabelmatching.py
+-rw-r--r--   0        0        0     5785 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/ioumatrix.py
+-rw-r--r--   0        0        0     9836 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/ioutils.py
+-rw-r--r--   0        0        0      284 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/logutils.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/masks/__init__.py
+-rw-r--r--   0        0        0     1208 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/masks/cymaskdownscale.pyx
+-rw-r--r--   0        0        0     1371 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/masks/maskdownscale.py
+-rw-r--r--   0        0        0     8463 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/matchingresult.py
+-rw-r--r--   0        0        0     2553 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/omegaconfutils.py
+-rw-r--r--   0        0        0     2032 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/pytestutils.py
+-rw-r--r--   0        0        0     6961 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/readwritelock.py
+-rw-r--r--   0        0        0      590 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/regexutils.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/semseg/__init__.py
+-rw-r--r--   0        0        0     1885 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/semseg/semsegdrawing.py
+-rw-r--r--   0        0        0     1664 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/semseg/semseginstancelabeling.py
+-rw-r--r--   0        0        0     1457 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/sinusgeneration.py
+-rw-r--r--   0        0        0     5710 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/splitutils.py
+-rw-r--r--   0        0        0     1317 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/thumbnailshower.py
+-rw-r--r--   0        0        0      472 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/timeutils.py
+-rw-r--r--   0        0        0     2789 2023-06-22 07:54:29.120107 niceml-0.4.1/niceml/utilities/userselection.py
+-rw-r--r--   0        0        0     3657 2023-06-22 07:55:09.724805 niceml-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4357 1970-01-01 00:00:00.000000 niceml-0.4.1/PKG-INFO
```

### Comparing `niceml-0.4.0/LICENSE` & `niceml-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/README.md` & `niceml-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/cli/clicommands.py` & `niceml-0.4.1/niceml/cli/clicommands.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/config/configschemas.py` & `niceml-0.4.1/niceml/config/configschemas.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/config/envconfig.py` & `niceml-0.4.1/niceml/config/envconfig.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/config/hydra.py` & `niceml-0.4.1/niceml/config/hydra.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/config/subsetnames.py` & `niceml-0.4.1/niceml/config/subsetnames.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dagster/jobs/jobs.py` & `niceml-0.4.1/niceml/dagster/jobs/jobs.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dagster/jobs/repository.py` & `niceml-0.4.1/niceml/dagster/jobs/repository.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dagster/ops/analysis.py` & `niceml-0.4.1/niceml/dagster/ops/analysis.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dagster/ops/copyexp.py` & `niceml-0.4.1/niceml/dagster/ops/copyexp.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dagster/ops/cropnumbers.py` & `niceml-0.4.1/niceml/dagster/ops/cropnumbers.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dagster/ops/datageneration.py` & `niceml-0.4.1/niceml/dagster/ops/datageneration.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dagster/ops/evalcopyexp.py` & `niceml-0.4.1/niceml/dagster/ops/evalcopyexp.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dagster/ops/experiment.py` & `niceml-0.4.1/niceml/dagster/ops/experiment.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dagster/ops/exptests.py` & `niceml-0.4.1/niceml/dagster/ops/exptests.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dagster/ops/imagetotable.py` & `niceml-0.4.1/niceml/dagster/ops/imagetotable.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dagster/ops/localizeexperiment.py` & `niceml-0.4.1/niceml/dagster/ops/localizeexperiment.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dagster/ops/prediction.py` & `niceml-0.4.1/niceml/dagster/ops/prediction.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dagster/ops/splitdata.py` & `niceml-0.4.1/niceml/dagster/ops/splitdata.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dagster/ops/train.py` & `niceml-0.4.1/niceml/dagster/ops/train.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dagster/resources/locations.py` & `niceml-0.4.1/niceml/dagster/resources/locations.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dashboard/binprobvisu.py` & `niceml-0.4.1/niceml/dashboard/binprobvisu.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dashboard/cam.py` & `niceml-0.4.1/niceml/dashboard/cam.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dashboard/components/downloadexpviscomponent.py` & `niceml-0.4.1/niceml/dashboard/components/downloadexpviscomponent.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dashboard/components/expviscomponent.py` & `niceml-0.4.1/niceml/dashboard/components/expviscomponent.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dashboard/components/linearviscomponent.py` & `niceml-0.4.1/niceml/dashboard/components/linearviscomponent.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dashboard/components/metaviscomponent.py` & `niceml-0.4.1/niceml/dashboard/components/metaviscomponent.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dashboard/components/prefixviscomponent.py` & `niceml-0.4.1/niceml/dashboard/components/prefixviscomponent.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dashboard/components/selectionviscomponent.py` & `niceml-0.4.1/niceml/dashboard/components/selectionviscomponent.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dashboard/configviscomponent.py` & `niceml-0.4.1/niceml/dashboard/configviscomponent.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dashboard/dashboard.py` & `niceml-0.4.1/niceml/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dashboard/imagenetdataloggerviscomponent.py` & `niceml-0.4.1/niceml/dashboard/imagenetdataloggerviscomponent.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dashboard/metricviscomponent.py` & `niceml-0.4.1/niceml/dashboard/metricviscomponent.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dashboard/remotettrainutils.py` & `niceml-0.4.1/niceml/dashboard/remotettrainutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dashboard/visualizers/boundingboxvisualizer.py` & `niceml-0.4.1/niceml/dashboard/visualizers/boundingboxvisualizer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dashboard/visualizers/imagevisualizer.py` & `niceml-0.4.1/niceml/dashboard/visualizers/imagevisualizer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dashboard/visualizers/maskvisualizer.py` & `niceml-0.4.1/niceml/dashboard/visualizers/maskvisualizer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datadescriptions/clsdatadescription.py` & `niceml-0.4.1/niceml/data/datadescriptions/clsdatadescription.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datadescriptions/inputdatadescriptions.py` & `niceml-0.4.1/niceml/data/datadescriptions/inputdatadescriptions.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datadescriptions/objdetdatadescription.py` & `niceml-0.4.1/niceml/data/datadescriptions/objdetdatadescription.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datadescriptions/outputdatadescriptions.py` & `niceml-0.4.1/niceml/data/datadescriptions/outputdatadescriptions.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datadescriptions/regdatadescription.py` & `niceml-0.4.1/niceml/data/datadescriptions/regdatadescription.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datadescriptions/semsegdatadescritption.py` & `niceml-0.4.1/niceml/data/datadescriptions/semsegdatadescritption.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datainfolistings/clsdatainfolisting.py` & `niceml-0.4.1/niceml/data/datainfolistings/clsdatainfolisting.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datainfolistings/objdetdatainfolisting.py` & `niceml-0.4.1/niceml/data/datainfolistings/objdetdatainfolisting.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datainfolistings/semsegdatainfolisting.py` & `niceml-0.4.1/niceml/data/datainfolistings/semsegdatainfolisting.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datainfos/clsdatainfo.py` & `niceml-0.4.1/niceml/data/datainfos/clsdatainfo.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datainfos/imagedatainfo.py` & `niceml-0.4.1/niceml/data/datainfos/imagedatainfo.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datainfos/objdetdatainfo.py` & `niceml-0.4.1/niceml/data/datainfos/objdetdatainfo.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datainfos/semsegdatainfo.py` & `niceml-0.4.1/niceml/data/datainfos/semsegdatainfo.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/dataiterators/boundingboxdataiterator.py` & `niceml-0.4.1/niceml/data/dataiterators/boundingboxdataiterator.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/dataiterators/dataiterator.py` & `niceml-0.4.1/niceml/data/dataiterators/dataiterator.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/dataloaders/cachedimageloader.py` & `niceml-0.4.1/niceml/data/dataloaders/cachedimageloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/dataloaders/clsdataloader.py` & `niceml-0.4.1/niceml/data/dataloaders/clsdataloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/dataloaders/dataloader.py` & `niceml-0.4.1/niceml/data/dataloaders/dataloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/dataloaders/dfloaders.py` & `niceml-0.4.1/niceml/data/dataloaders/dfloaders.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/dataloaders/factories/dfloaderfactory.py` & `niceml-0.4.1/niceml/data/dataloaders/factories/dfloaderfactory.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/dataloaders/imageloaders.py` & `niceml-0.4.1/niceml/data/dataloaders/imageloaders.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/dataloaders/interfaces/imageloader.py` & `niceml-0.4.1/niceml/data/dataloaders/interfaces/imageloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/dataloaders/objdetdataloader.py` & `niceml-0.4.1/niceml/data/dataloaders/objdetdataloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/dataloaders/semseg/cytransformmaskimage.pyx` & `niceml-0.4.1/niceml/data/dataloaders/semseg/cytransformmaskimage.pyx`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/dataloaders/semseg/semsegdataloader.py` & `niceml-0.4.1/niceml/data/dataloaders/semseg/semsegdataloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/dataloaders/semseg/transformmaskimage.py` & `niceml-0.4.1/niceml/data/dataloaders/semseg/transformmaskimage.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datasets/clsclassinfo.py` & `niceml-0.4.1/niceml/data/datasets/clsclassinfo.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datasets/dataset.py` & `niceml-0.4.1/niceml/data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datasets/dfdataset.py` & `niceml-0.4.1/niceml/data/datasets/dfdataset.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datasets/genericdataset.py` & `niceml-0.4.1/niceml/data/datasets/genericdataset.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datasets/healthdataset.py` & `niceml-0.4.1/niceml/data/datasets/healthdataset.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datasets/sinusdataset.py` & `niceml-0.4.1/niceml/data/datasets/sinusdataset.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datashuffler/datashuffler.py` & `niceml-0.4.1/niceml/data/datashuffler/datashuffler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datashuffler/defaultshuffler.py` & `niceml-0.4.1/niceml/data/datashuffler/defaultshuffler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/datashuffler/uniformdistributionshuffler.py` & `niceml-0.4.1/niceml/data/datashuffler/uniformdistributionshuffler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/netdataloggers/netdatalogger.py` & `niceml-0.4.1/niceml/data/netdataloggers/netdatalogger.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/netdataloggers/objdetnetdatalogger.py` & `niceml-0.4.1/niceml/data/netdataloggers/objdetnetdatalogger.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/netdataloggers/semsegnetdatalogger.py` & `niceml-0.4.1/niceml/data/netdataloggers/semsegnetdatalogger.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/storages/fsfilesystemstorage.py` & `niceml-0.4.1/niceml/data/storages/fsfilesystemstorage.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/storages/fsspecstorage.py` & `niceml-0.4.1/niceml/data/storages/fsspecstorage.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/storages/localstorage.py` & `niceml-0.4.1/niceml/data/storages/localstorage.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/storages/storagehandler.py` & `niceml-0.4.1/niceml/data/storages/storagehandler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/data/storages/storageinterface.py` & `niceml-0.4.1/niceml/data/storages/storageinterface.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/callbacks/callback_factories.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/callbacks/callback_factories.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/callbacks/csvlogger.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/callbacks/csvlogger.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/callbacks/modelcheckpoint.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/callbacks/modelcheckpoint.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/callbacks/nancheckcallback.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/callbacks/nancheckcallback.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/kerasmetrics.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/kerasmetrics.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/kerasmodelloader.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/kerasmodelloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/learners/defaultlearner.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/learners/defaultlearner.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/losses/categoricalfocalloss.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/losses/categoricalfocalloss.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/losses/objdetlosses.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/losses/objdetlosses.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/losses/semseglosses.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/losses/semseglosses.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/metrics/objdetmetrics.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/metrics/objdetmetrics.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/metrics/semsegmetrics.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/metrics/semsegmetrics.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/modelcompiler/defaultmodelcompiler.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/modelcompiler/defaultmodelcompiler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/models/clsmodelfactory.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/models/clsmodelfactory.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/models/layerfactory.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/models/layerfactory.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/models/loadweightsmodelfactory.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/models/loadweightsmodelfactory.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/models/mlp.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/models/mlp.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/models/mobilenet.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/models/mobilenet.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/models/premodellayers.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/models/premodellayers.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/models/retinanet.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/models/retinanet.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/models/unets.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/models/unets.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/dlframeworks/tensorflow/optimizers/schedules/cycliclrschedule.py` & `niceml-0.4.1/niceml/dlframeworks/tensorflow/optimizers/schedules/cycliclrschedule.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/confextractionmetafunction.py` & `niceml-0.4.1/niceml/experiments/confextractionmetafunction.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/expdatalocalstorageloader.py` & `niceml-0.4.1/niceml/experiments/expdatalocalstorageloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/expdatastorageloader.py` & `niceml-0.4.1/niceml/experiments/expdatastorageloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/experimentcontext.py` & `niceml-0.4.1/niceml/experiments/experimentcontext.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/experimentdata.py` & `niceml-0.4.1/niceml/experiments/experimentdata.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/experimentdownloader.py` & `niceml-0.4.1/niceml/experiments/experimentdownloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/experimenterrors.py` & `niceml-0.4.1/niceml/experiments/experimenterrors.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/experimentinfo.py` & `niceml-0.4.1/niceml/experiments/experimentinfo.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/experimentmanager.py` & `niceml-0.4.1/niceml/experiments/experimentmanager.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/experimenttests/checkfilesfolderstest.py` & `niceml-0.4.1/niceml/experiments/experimenttests/checkfilesfolderstest.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/experimenttests/exptests.py` & `niceml-0.4.1/niceml/experiments/experimenttests/exptests.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/experimenttests/metriccheck.py` & `niceml-0.4.1/niceml/experiments/experimenttests/metriccheck.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/experimenttests/testinitializer.py` & `niceml-0.4.1/niceml/experiments/experimenttests/testinitializer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/experimenttests/validateexps.py` & `niceml-0.4.1/niceml/experiments/experimenttests/validateexps.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/expfilenames.py` & `niceml-0.4.1/niceml/experiments/expfilenames.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/expoutinitializer.py` & `niceml-0.4.1/niceml/experiments/expoutinitializer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/exppathfinder.py` & `niceml-0.4.1/niceml/experiments/exppathfinder.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/filters/datefilter.py` & `niceml-0.4.1/niceml/experiments/filters/datefilter.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/filters/experimentfilter.py` & `niceml-0.4.1/niceml/experiments/filters/experimentfilter.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/filters/expselectionfilter.py` & `niceml-0.4.1/niceml/experiments/filters/expselectionfilter.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/filters/selectboxfilter.py` & `niceml-0.4.1/niceml/experiments/filters/selectboxfilter.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/filters/sliderfilter.py` & `niceml-0.4.1/niceml/experiments/filters/sliderfilter.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/loaddatafunctions.py` & `niceml-0.4.1/niceml/experiments/loaddatafunctions.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/loadexpinfo.py` & `niceml-0.4.1/niceml/experiments/loadexpinfo.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/localexperimentcache.py` & `niceml-0.4.1/niceml/experiments/localexperimentcache.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/metafunctions.py` & `niceml-0.4.1/niceml/experiments/metafunctions.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/metainfotables.py` & `niceml-0.4.1/niceml/experiments/metainfotables.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/metalists.py` & `niceml-0.4.1/niceml/experiments/metalists.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/metatablefactory.py` & `niceml-0.4.1/niceml/experiments/metatablefactory.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/schemas/baseexpschema.py` & `niceml-0.4.1/niceml/experiments/schemas/baseexpschema.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/schemas/expdocstring.py` & `niceml-0.4.1/niceml/experiments/schemas/expdocstring.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/schemas/expmember.py` & `niceml-0.4.1/niceml/experiments/schemas/expmember.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/schemas/objdetexpschema.py` & `niceml-0.4.1/niceml/experiments/schemas/objdetexpschema.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/schemas/parquetframeexpmember.py` & `niceml-0.4.1/niceml/experiments/schemas/parquetframeexpmember.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/schemas/sampleexpschemas.py` & `niceml-0.4.1/niceml/experiments/schemas/sampleexpschemas.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/schemas/schemavalidation.py` & `niceml-0.4.1/niceml/experiments/schemas/schemavalidation.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/experiments/schemas/yamlexpmember.py` & `niceml-0.4.1/niceml/experiments/schemas/yamlexpmember.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mkdocs/mdgraph.py` & `niceml-0.4.1/niceml/mkdocs/mdgraph.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mkdocs/mdjob.py` & `niceml-0.4.1/niceml/mkdocs/mdjob.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mkdocs/mdop.py` & `niceml-0.4.1/niceml/mkdocs/mdop.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mkdocs/mdtable.py` & `niceml-0.4.1/niceml/mkdocs/mdtable.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mkdocs/schemadocgeneration.py` & `niceml-0.4.1/niceml/mkdocs/schemadocgeneration.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/callbacks/callbackinitializer.py` & `niceml-0.4.1/niceml/mlcomponents/callbacks/callbackinitializer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/learners/fitgenerators.py` & `niceml-0.4.1/niceml/mlcomponents/learners/fitgenerators.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/learners/learner.py` & `niceml-0.4.1/niceml/mlcomponents/learners/learner.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/modelcompiler/modelcompiler.py` & `niceml-0.4.1/niceml/mlcomponents/modelcompiler/modelcompiler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/modelcompiler/modelcustomloadobjects.py` & `niceml-0.4.1/niceml/mlcomponents/modelcompiler/modelcustomloadobjects.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/modelloader/modelloader.py` & `niceml-0.4.1/niceml/mlcomponents/modelloader/modelloader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/objdet/anchorencoding.py` & `niceml-0.4.1/niceml/mlcomponents/objdet/anchorencoding.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/objdet/anchorgenerator.py` & `niceml-0.4.1/niceml/mlcomponents/objdet/anchorgenerator.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/predictionhandlers/combinationpredictionhandler.py` & `niceml-0.4.1/niceml/mlcomponents/predictionhandlers/combinationpredictionhandler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/predictionhandlers/objdetpredictionhandler.py` & `niceml-0.4.1/niceml/mlcomponents/predictionhandlers/objdetpredictionhandler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/predictionhandlers/predictionhandler.py` & `niceml-0.4.1/niceml/mlcomponents/predictionhandlers/predictionhandler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/predictionhandlers/semsegpredictionhandler.py` & `niceml-0.4.1/niceml/mlcomponents/predictionhandlers/semsegpredictionhandler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/predictionhandlers/tensorpredictionhandler.py` & `niceml-0.4.1/niceml/mlcomponents/predictionhandlers/tensorpredictionhandler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/predictionhandlers/vectorpredictionhandler.py` & `niceml-0.4.1/niceml/mlcomponents/predictionhandlers/vectorpredictionhandler.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/resultanalyzers/analyzer.py` & `niceml-0.4.1/niceml/mlcomponents/resultanalyzers/analyzer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/resultanalyzers/dataframes/clsmetric.py` & `niceml-0.4.1/niceml/mlcomponents/resultanalyzers/dataframes/clsmetric.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/resultanalyzers/dataframes/dfanalyzer.py` & `niceml-0.4.1/niceml/mlcomponents/resultanalyzers/dataframes/dfanalyzer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/resultanalyzers/dataframes/multilabeltobinary.py` & `niceml-0.4.1/niceml/mlcomponents/resultanalyzers/dataframes/multilabeltobinary.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/resultanalyzers/dataframes/regmetric.py` & `niceml-0.4.1/niceml/mlcomponents/resultanalyzers/dataframes/regmetric.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/resultanalyzers/instancefinders/instancecontour.py` & `niceml-0.4.1/niceml/mlcomponents/resultanalyzers/instancefinders/instancecontour.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/resultanalyzers/instancefinders/instancefinder.py` & `niceml-0.4.1/niceml/mlcomponents/resultanalyzers/instancefinders/instancefinder.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/resultanalyzers/instancefinders/maskinstance.py` & `niceml-0.4.1/niceml/mlcomponents/resultanalyzers/instancefinders/maskinstance.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/resultanalyzers/instancefinders/multichannelinstancefinder.py` & `niceml-0.4.1/niceml/mlcomponents/resultanalyzers/instancefinders/multichannelinstancefinder.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/resultanalyzers/multiresultanalyzer.py` & `niceml-0.4.1/niceml/mlcomponents/resultanalyzers/multiresultanalyzer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/resultanalyzers/tensors/cytensoriou.pyx` & `niceml-0.4.1/niceml/mlcomponents/resultanalyzers/tensors/cytensoriou.pyx`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/resultanalyzers/tensors/semsegdataiterator.py` & `niceml-0.4.1/niceml/mlcomponents/resultanalyzers/tensors/semsegdataiterator.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/resultanalyzers/tensors/tensordataiterators.py` & `niceml-0.4.1/niceml/mlcomponents/resultanalyzers/tensors/tensordataiterators.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/resultanalyzers/tensors/tensordfmetricwrapper.py` & `niceml-0.4.1/niceml/mlcomponents/resultanalyzers/tensors/tensordfmetricwrapper.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/resultanalyzers/tensors/tensorgraphanalyzer.py` & `niceml-0.4.1/niceml/mlcomponents/resultanalyzers/tensors/tensorgraphanalyzer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/resultanalyzers/tensors/tensoriou.py` & `niceml-0.4.1/niceml/mlcomponents/resultanalyzers/tensors/tensoriou.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/resultanalyzers/tensors/tensormetric.py` & `niceml-0.4.1/niceml/mlcomponents/resultanalyzers/tensors/tensormetric.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/resultanalyzers/tensors/tensorvisualizer.py` & `niceml-0.4.1/niceml/mlcomponents/resultanalyzers/tensors/tensorvisualizer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/resultanalyzers/tensors/zarrdataiterator.py` & `niceml-0.4.1/niceml/mlcomponents/resultanalyzers/tensors/zarrdataiterator.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/targettransformer/imageinputtransformer.py` & `niceml-0.4.1/niceml/mlcomponents/targettransformer/imageinputtransformer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/targettransformer/objdettargettransformer.py` & `niceml-0.4.1/niceml/mlcomponents/targettransformer/objdettargettransformer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/targettransformer/semsegtargettransformer.py` & `niceml-0.4.1/niceml/mlcomponents/targettransformer/semsegtargettransformer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/targettransformer/targettransformer.py` & `niceml-0.4.1/niceml/mlcomponents/targettransformer/targettransformer.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/mlcomponents/targettransformer/targettransformercls.py` & `niceml-0.4.1/niceml/mlcomponents/targettransformer/targettransformercls.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/scripts/hydraconfreader.py` & `niceml-0.4.1/niceml/scripts/hydraconfreader.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/scripts/rundatatests.py` & `niceml-0.4.1/niceml/scripts/rundatatests.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/scripts/splitdatasetindex.py` & `niceml-0.4.1/niceml/scripts/splitdatasetindex.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/storages/abs.py` & `niceml-0.4.1/niceml/storages/abs.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/assets/bg_images/andrew-neel-slRYlH9ttzc-unsplash.jpg` & `niceml-0.4.1/niceml/utilities/assets/bg_images/andrew-neel-slRYlH9ttzc-unsplash.jpg`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/assets/bg_images/karthik-sreenivas-1N_78ShYQFg-unsplash.jpg` & `niceml-0.4.1/niceml/utilities/assets/bg_images/karthik-sreenivas-1N_78ShYQFg-unsplash.jpg`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/assets/bg_images/neha-maheen-mahfin-FtiAj6ggKnU-unsplash.jpg` & `niceml-0.4.1/niceml/utilities/assets/bg_images/neha-maheen-mahfin-FtiAj6ggKnU-unsplash.jpg`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/assets/bg_images/yousef-espanioly-8ja-Ns8iqO4-unsplash.jpg` & `niceml-0.4.1/niceml/utilities/assets/bg_images/yousef-espanioly-8ja-Ns8iqO4-unsplash.jpg`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/assets/fonts/DMMono-Regular.ttf` & `niceml-0.4.1/niceml/utilities/assets/fonts/DMMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/assets/fonts/Dosis-Regular.ttf` & `niceml-0.4.1/niceml/utilities/assets/fonts/Dosis-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/assets/fonts/Heebo-Regular.ttf` & `niceml-0.4.1/niceml/utilities/assets/fonts/Heebo-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/assets/fonts/Karla-Regular.ttf` & `niceml-0.4.1/niceml/utilities/assets/fonts/Karla-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/assets/fonts/OpenSans-Regular.ttf` & `niceml-0.4.1/niceml/utilities/assets/fonts/OpenSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/assets/fonts/Oswald-Regular.ttf` & `niceml-0.4.1/niceml/utilities/assets/fonts/Oswald-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/assets/fonts/OxygenMono-Regular.ttf` & `niceml-0.4.1/niceml/utilities/assets/fonts/OxygenMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/assets/fonts/RobotoMono-Regular.ttf` & `niceml-0.4.1/niceml/utilities/assets/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/assets/fonts/Rubik-Regular.ttf` & `niceml-0.4.1/niceml/utilities/assets/fonts/Rubik-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/assets/fonts/Ubuntu-Regular.ttf` & `niceml-0.4.1/niceml/utilities/assets/fonts/Ubuntu-Regular.ttf`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/boundingboxes/bboxconversion.py` & `niceml-0.4.1/niceml/utilities/boundingboxes/bboxconversion.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/boundingboxes/bboxdrawing.py` & `niceml-0.4.1/niceml/utilities/boundingboxes/bboxdrawing.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/boundingboxes/bboxencoding.py` & `niceml-0.4.1/niceml/utilities/boundingboxes/bboxencoding.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/boundingboxes/bboxlabeling.py` & `niceml-0.4.1/niceml/utilities/boundingboxes/bboxlabeling.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/boundingboxes/boundingbox.py` & `niceml-0.4.1/niceml/utilities/boundingboxes/boundingbox.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/boundingboxes/filtering/nmsfilter.py` & `niceml-0.4.1/niceml/utilities/boundingboxes/filtering/nmsfilter.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/boundingboxes/filtering/predictionfilter.py` & `niceml-0.4.1/niceml/utilities/boundingboxes/filtering/predictionfilter.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/boundingboxes/filtering/thresholdfilter.py` & `niceml-0.4.1/niceml/utilities/boundingboxes/filtering/thresholdfilter.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/boundingboxes/filtering/unifiedboxfilter.py` & `niceml-0.4.1/niceml/utilities/boundingboxes/filtering/unifiedboxfilter.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/chartutils.py` & `niceml-0.4.1/niceml/utilities/chartutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/checksums.py` & `niceml-0.4.1/niceml/utilities/checksums.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/colorutils.py` & `niceml-0.4.1/niceml/utilities/colorutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/commonutils.py` & `niceml-0.4.1/niceml/utilities/commonutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/copyutils.py` & `niceml-0.4.1/niceml/utilities/copyutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/encoding.py` & `niceml-0.4.1/niceml/utilities/encoding.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/factoryutils.py` & `niceml-0.4.1/niceml/utilities/factoryutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/filtering/probabilityclassselector.py` & `niceml-0.4.1/niceml/utilities/filtering/probabilityclassselector.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/fsspec/locationutils.py` & `niceml-0.4.1/niceml/utilities/fsspec/locationutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/gitutils.py` & `niceml-0.4.1/niceml/utilities/gitutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/hydrautils.py` & `niceml-0.4.1/niceml/utilities/hydrautils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/idutils.py` & `niceml-0.4.1/niceml/utilities/idutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/imagegeneration.py` & `niceml-0.4.1/niceml/utilities/imagegeneration.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/imageloading.py` & `niceml-0.4.1/niceml/utilities/imageloading.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/imagesize.py` & `niceml-0.4.1/niceml/utilities/imagesize.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/imageutils.py` & `niceml-0.4.1/niceml/utilities/imageutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/instancelabeling.py` & `niceml-0.4.1/niceml/utilities/instancelabeling.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/instancelabelmatching.py` & `niceml-0.4.1/niceml/utilities/instancelabelmatching.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/ioumatrix.py` & `niceml-0.4.1/niceml/utilities/ioumatrix.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/ioutils.py` & `niceml-0.4.1/niceml/utilities/ioutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/masks/cymaskdownscale.pyx` & `niceml-0.4.1/niceml/utilities/masks/cymaskdownscale.pyx`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/masks/maskdownscale.py` & `niceml-0.4.1/niceml/utilities/masks/maskdownscale.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/matchingresult.py` & `niceml-0.4.1/niceml/utilities/matchingresult.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/omegaconfutils.py` & `niceml-0.4.1/niceml/utilities/omegaconfutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/pytestutils.py` & `niceml-0.4.1/niceml/utilities/pytestutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/readwritelock.py` & `niceml-0.4.1/niceml/utilities/readwritelock.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/regexutils.py` & `niceml-0.4.1/niceml/utilities/regexutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/semseg/semsegdrawing.py` & `niceml-0.4.1/niceml/utilities/semseg/semsegdrawing.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/semseg/semseginstancelabeling.py` & `niceml-0.4.1/niceml/utilities/semseg/semseginstancelabeling.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/sinusgeneration.py` & `niceml-0.4.1/niceml/utilities/sinusgeneration.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/splitutils.py` & `niceml-0.4.1/niceml/utilities/splitutils.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/thumbnailshower.py` & `niceml-0.4.1/niceml/utilities/thumbnailshower.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/niceml/utilities/userselection.py` & `niceml-0.4.1/niceml/utilities/userselection.py`

 * *Files identical despite different names*

### Comparing `niceml-0.4.0/pyproject.toml` & `niceml-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "niceml"
-version = "0.4.0"
+version = "0.4.1"
 description = "Welcome to niceML 🍦, a Python-based MLOps framework that uses TensorFlow and Dagster. This framework streamlines the development, and maintenance of machine learning models, providing an end-to-end solution for building efficient and scalable pipelines."
 authors = [
     "Denis Stalz-John <denis.stalz-john@codecentric.de>",
     "Nils Uhrberg <nils.uhrberg@codecentric.de>",
     "Anke Koke <anke.koke@codecentric.de>"
 ]
 readme = "README.md"
@@ -50,15 +50,15 @@
 pympler = "^1.0.1"
 cattrs = "^22.2.0"
 isodate = "^0.6.1"
 scikit-learn = "^1.2.2"
 pandera = "^0.14.5"
 schema = "^0.7.5"
 copier = "^7.2.0"
-dagster = "1.3.3"
+dagster = "1.3.9"
 tornado = ">=6.0.3,<6.3.1"
 networkx = "^3.1"
 mkdocs-gen-files = "^0.5.0"
 toml = "^0.10.2"
 invoke = ">=1.4.1,<2"
 dagit = "^1.3.3"
 albumentations = "^1.3.0"
```

### Comparing `niceml-0.4.0/PKG-INFO` & `niceml-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niceml
-Version: 0.4.0
+Version: 0.4.1
 Summary: Welcome to niceML 🍦, a Python-based MLOps framework that uses TensorFlow and Dagster. This framework streamlines the development, and maintenance of machine learning models, providing an end-to-end solution for building efficient and scalable pipelines.
 Keywords: tensorflow,scikit-learn,streamlit
 Author: Denis Stalz-John
 Author-email: denis.stalz-john@codecentric.de
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.11.*
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -33,15 +33,15 @@
 Requires-Dist: albumentations (>=1.3.0,<2.0.0)
 Requires-Dist: altair (>=4.2.2,<5.0.0) ; extra == "visu"
 Requires-Dist: cattrs (>=22.2.0,<23.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: copier (>=7.2.0,<8.0.0)
 Requires-Dist: cython (>=0.29.34,<0.30.0)
 Requires-Dist: dagit (>=1.3.3,<2.0.0)
-Requires-Dist: dagster (==1.3.3)
+Requires-Dist: dagster (==1.3.9)
 Requires-Dist: fastparquet (>=2023.2.0,<2024.0.0)
 Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
 Requires-Dist: invoke (>=1.4.1,<2)
 Requires-Dist: isodate (>=0.6.1,<0.7.0)
 Requires-Dist: mkdocs-gen-files (>=0.5.0,<0.6.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
```

