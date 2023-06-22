# Comparing `tmp/opensoundscape-0.9.0.tar.gz` & `tmp/opensoundscape-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensoundscape-0.9.0.tar", max compression
+gzip compressed data, was "opensoundscape-0.9.1.tar", max compression
```

## Comparing `opensoundscape-0.9.0.tar` & `opensoundscape-0.9.1.tar`

### file list

```diff
@@ -1,36 +1,69 @@
--rw-r--r--   0        0        0     1081 2022-09-07 19:54:53.274476 opensoundscape-0.9.0/LICENSE
--rw-r--r--   0        0        0     4141 2023-04-28 16:25:08.326479 opensoundscape-0.9.0/README.md
--rw-r--r--   0        0        0      835 2023-04-28 16:25:08.662321 opensoundscape-0.9.0/opensoundscape/__init__.py
--rw-r--r--   0        0        0    30818 2023-04-28 16:25:08.663789 opensoundscape-0.9.0/opensoundscape/annotations.py
--rw-r--r--   0        0        0     6740 2023-04-28 16:25:08.664111 opensoundscape-0.9.0/opensoundscape/aru.py
--rw-r--r--   0        0        0    51145 2023-04-28 16:25:08.665360 opensoundscape-0.9.0/opensoundscape/audio.py
--rw-r--r--   0        0        0     4121 2023-01-18 14:19:19.795886 opensoundscape-0.9.0/opensoundscape/data_selection.py
--rw-r--r--   0        0        0    46865 2023-04-28 16:25:08.667564 opensoundscape-0.9.0/opensoundscape/localization.py
--rw-r--r--   0        0        0     2755 2023-04-28 16:25:08.669350 opensoundscape-0.9.0/opensoundscape/logging.py
--rw-r--r--   0        0        0     8174 2023-04-04 20:56:27.927318 opensoundscape-0.9.0/opensoundscape/metrics.py
--rw-r--r--   0        0        0      180 2023-04-28 16:25:08.669653 opensoundscape-0.9.0/opensoundscape/ml/__init__.py
--rw-r--r--   0        0        0     5759 2023-04-28 16:25:08.672220 opensoundscape-0.9.0/opensoundscape/ml/cam.py
--rw-r--r--   0        0        0    74373 2023-04-28 16:25:08.674300 opensoundscape-0.9.0/opensoundscape/ml/cnn.py
--rw-r--r--   0        0        0    28247 2023-04-28 16:25:08.675387 opensoundscape-0.9.0/opensoundscape/ml/cnn_architectures.py
--rw-r--r--   0        0        0     6763 2023-04-28 16:25:08.676839 opensoundscape-0.9.0/opensoundscape/ml/datasets.py
--rw-r--r--   0        0        0     5970 2023-04-28 16:25:08.681611 opensoundscape-0.9.0/opensoundscape/ml/loss.py
--rw-r--r--   0        0        0     8248 2023-04-28 16:25:08.692391 opensoundscape-0.9.0/opensoundscape/ml/safe_dataset.py
--rw-r--r--   0        0        0     4319 2023-04-28 16:25:08.692659 opensoundscape-0.9.0/opensoundscape/ml/sampling.py
--rw-r--r--   0        0        0     4233 2023-04-28 16:25:08.693097 opensoundscape-0.9.0/opensoundscape/ml/utils.py
--rw-r--r--   0        0        0      125 2022-09-07 19:54:53.425139 opensoundscape-0.9.0/opensoundscape/preprocess/__init__.py
--rw-r--r--   0        0        0    25550 2023-04-28 16:25:08.694576 opensoundscape-0.9.0/opensoundscape/preprocess/actions.py
--rw-r--r--   0        0        0      730 2023-01-18 14:19:19.798767 opensoundscape-0.9.0/opensoundscape/preprocess/img_augment.py
--rw-r--r--   0        0        0    11929 2023-04-28 16:25:08.695323 opensoundscape-0.9.0/opensoundscape/preprocess/preprocessors.py
--rw-r--r--   0        0        0     2622 2023-01-18 14:19:19.803780 opensoundscape-0.9.0/opensoundscape/preprocess/tensor_augment.py
--rw-r--r--   0        0        0     2604 2023-01-18 14:19:19.804368 opensoundscape-0.9.0/opensoundscape/preprocess/utils.py
--rw-r--r--   0        0        0        0 2022-09-07 19:54:53.431876 opensoundscape-0.9.0/opensoundscape/resources/__init__.py
--rw-r--r--   0        0        0    42432 2022-09-07 19:54:53.432206 opensoundscape-0.9.0/opensoundscape/resources/species_table.csv
--rw-r--r--   0        0        0     8817 2023-04-28 16:25:08.695756 opensoundscape-0.9.0/opensoundscape/ribbit.py
--rw-r--r--   0        0        0     5042 2023-04-28 16:25:08.696268 opensoundscape-0.9.0/opensoundscape/sample.py
--rw-r--r--   0        0        0    22972 2023-04-28 16:25:08.697235 opensoundscape-0.9.0/opensoundscape/signal_processing.py
--rw-r--r--   0        0        0    32681 2023-04-28 16:25:08.697671 opensoundscape-0.9.0/opensoundscape/spectrogram.py
--rw-r--r--   0        0        0     1901 2023-01-18 14:19:19.808150 opensoundscape-0.9.0/opensoundscape/taxa.py
--rw-r--r--   0        0        0    12684 2023-04-28 16:25:08.698570 opensoundscape-0.9.0/opensoundscape/utils.py
--rw-r--r--   0        0        0     1687 2023-04-28 16:25:08.701571 opensoundscape-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     5757 1970-01-01 00:00:00.000000 opensoundscape-0.9.0/setup.py
--rw-r--r--   0        0        0     5642 1970-01-01 00:00:00.000000 opensoundscape-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2022-09-07 19:54:53.274476 opensoundscape-0.9.1/LICENSE
+-rw-r--r--   0        0        0     5212 2023-06-22 16:15:11.733024 opensoundscape-0.9.1/README.md
+-rw-r--r--   0        0        0     6148 2023-04-03 14:10:27.489554 opensoundscape-0.9.1/opensoundscape/.DS_Store
+-rw-r--r--   0        0        0       37 2022-12-19 23:38:55.202198 opensoundscape-0.9.1/opensoundscape/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2022-12-19 23:38:55.202391 opensoundscape-0.9.1/opensoundscape/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2022-12-19 23:38:55.201971 opensoundscape-0.9.1/opensoundscape/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2022-12-19 23:38:55.202593 opensoundscape-0.9.1/opensoundscape/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2022-12-19 23:38:55.202869 opensoundscape-0.9.1/opensoundscape/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      816 2023-06-22 16:15:12.075479 opensoundscape-0.9.1/opensoundscape/__init__.py
+-rw-r--r--   0        0        0    32734 2023-06-22 16:15:12.077455 opensoundscape-0.9.1/opensoundscape/annotations.py
+-rw-r--r--   0        0        0    53429 2023-06-22 16:15:12.078677 opensoundscape-0.9.1/opensoundscape/audio.py
+-rw-r--r--   0        0        0     4129 2023-06-22 16:15:12.079586 opensoundscape-0.9.1/opensoundscape/data_selection.py
+-rw-r--r--   0        0        0    47629 2023-06-22 16:15:12.080384 opensoundscape-0.9.1/opensoundscape/localization.py
+-rw-r--r--   0        0        0     2755 2023-04-28 16:25:08.669350 opensoundscape-0.9.1/opensoundscape/logging.py
+-rw-r--r--   0        0        0     8046 2023-06-22 16:15:12.083463 opensoundscape-0.9.1/opensoundscape/metrics.py
+-rw-r--r--   0        0        0      180 2023-04-28 16:25:08.669653 opensoundscape-0.9.1/opensoundscape/ml/__init__.py
+-rw-r--r--   0        0        0      397 2023-05-26 16:34:12.420325 opensoundscape-0.9.1/opensoundscape/ml/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      395 2023-04-28 16:25:42.669721 opensoundscape-0.9.1/opensoundscape/ml/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4763 2023-05-26 16:34:12.431908 opensoundscape-0.9.1/opensoundscape/ml/__pycache__/cam.cpython-310.pyc
+-rw-r--r--   0        0        0     4761 2023-04-28 16:25:42.686673 opensoundscape-0.9.1/opensoundscape/ml/__pycache__/cam.cpython-39.pyc
+-rw-r--r--   0        0        0    45844 2023-05-26 16:34:12.624384 opensoundscape-0.9.1/opensoundscape/ml/__pycache__/cnn.cpython-310.pyc
+-rw-r--r--   0        0        0    45682 2023-06-22 16:15:48.822915 opensoundscape-0.9.1/opensoundscape/ml/__pycache__/cnn.cpython-39.pyc
+-rw-r--r--   0        0        0    19983 2023-05-26 16:34:12.446146 opensoundscape-0.9.1/opensoundscape/ml/__pycache__/cnn_architectures.cpython-310.pyc
+-rw-r--r--   0        0        0    20795 2023-06-22 16:15:46.783547 opensoundscape-0.9.1/opensoundscape/ml/__pycache__/cnn_architectures.cpython-39.pyc
+-rw-r--r--   0        0        0     6256 2023-05-26 16:34:12.713379 opensoundscape-0.9.1/opensoundscape/ml/__pycache__/datasets.cpython-310.pyc
+-rw-r--r--   0        0        0     6250 2023-06-22 16:15:48.956161 opensoundscape-0.9.1/opensoundscape/ml/__pycache__/datasets.cpython-39.pyc
+-rw-r--r--   0        0        0     5258 2023-01-18 14:19:24.183641 opensoundscape-0.9.1/opensoundscape/ml/__pycache__/grad_cam.cpython-39.pyc
+-rw-r--r--   0        0        0     5326 2023-05-26 16:34:12.695422 opensoundscape-0.9.1/opensoundscape/ml/__pycache__/loss.cpython-310.pyc
+-rw-r--r--   0        0        0     5375 2023-04-28 16:25:44.107816 opensoundscape-0.9.1/opensoundscape/ml/__pycache__/loss.cpython-39.pyc
+-rw-r--r--   0        0        0     6855 2023-05-26 16:34:12.705672 opensoundscape-0.9.1/opensoundscape/ml/__pycache__/safe_dataset.cpython-310.pyc
+-rw-r--r--   0        0        0     6827 2023-04-28 16:25:44.115374 opensoundscape-0.9.1/opensoundscape/ml/__pycache__/safe_dataset.cpython-39.pyc
+-rw-r--r--   0        0        0     5002 2023-05-26 16:34:12.644482 opensoundscape-0.9.1/opensoundscape/ml/__pycache__/sampling.cpython-310.pyc
+-rw-r--r--   0        0        0     4982 2023-06-22 16:15:48.866086 opensoundscape-0.9.1/opensoundscape/ml/__pycache__/sampling.cpython-39.pyc
+-rw-r--r--   0        0        0     4124 2023-05-26 16:34:12.635259 opensoundscape-0.9.1/opensoundscape/ml/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     4070 2023-06-22 16:15:48.853809 opensoundscape-0.9.1/opensoundscape/ml/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0        0        0     5759 2023-04-28 16:25:08.672220 opensoundscape-0.9.1/opensoundscape/ml/cam.py
+-rw-r--r--   0        0        0    74205 2023-06-22 16:15:12.084861 opensoundscape-0.9.1/opensoundscape/ml/cnn.py
+-rw-r--r--   0        0        0    28276 2023-06-22 16:15:12.086283 opensoundscape-0.9.1/opensoundscape/ml/cnn_architectures.py
+-rw-r--r--   0        0        0     6761 2023-06-22 16:15:12.087275 opensoundscape-0.9.1/opensoundscape/ml/datasets.py
+-rw-r--r--   0        0        0     5970 2023-04-28 16:25:08.681611 opensoundscape-0.9.1/opensoundscape/ml/loss.py
+-rw-r--r--   0        0        0     8248 2023-04-28 16:25:08.692391 opensoundscape-0.9.1/opensoundscape/ml/safe_dataset.py
+-rw-r--r--   0        0        0     4324 2023-06-22 16:15:12.088098 opensoundscape-0.9.1/opensoundscape/ml/sampling.py
+-rw-r--r--   0        0        0     4161 2023-06-22 16:15:12.088752 opensoundscape-0.9.1/opensoundscape/ml/utils.py
+-rw-r--r--   0        0        0      125 2022-09-07 19:54:53.425139 opensoundscape-0.9.1/opensoundscape/preprocess/__init__.py
+-rw-r--r--   0        0        0      326 2023-05-26 16:34:12.651627 opensoundscape-0.9.1/opensoundscape/preprocess/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      324 2022-09-09 22:08:25.205912 opensoundscape-0.9.1/opensoundscape/preprocess/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    19582 2023-05-26 16:34:12.663489 opensoundscape-0.9.1/opensoundscape/preprocess/__pycache__/actions.cpython-310.pyc
+-rw-r--r--   0        0        0    19689 2023-06-22 16:15:48.895172 opensoundscape-0.9.1/opensoundscape/preprocess/__pycache__/actions.cpython-39.pyc
+-rw-r--r--   0        0        0      969 2023-05-26 16:34:12.682981 opensoundscape-0.9.1/opensoundscape/preprocess/__pycache__/img_augment.cpython-310.pyc
+-rw-r--r--   0        0        0      967 2023-01-18 14:19:24.388987 opensoundscape-0.9.1/opensoundscape/preprocess/__pycache__/img_augment.cpython-39.pyc
+-rw-r--r--   0        0        0     9443 2023-05-26 16:34:12.686349 opensoundscape-0.9.1/opensoundscape/preprocess/__pycache__/preprocessors.cpython-310.pyc
+-rw-r--r--   0        0        0     9419 2023-06-22 16:15:48.936372 opensoundscape-0.9.1/opensoundscape/preprocess/__pycache__/preprocessors.cpython-39.pyc
+-rw-r--r--   0        0        0     2749 2023-05-26 16:34:12.669516 opensoundscape-0.9.1/opensoundscape/preprocess/__pycache__/tensor_augment.cpython-310.pyc
+-rw-r--r--   0        0        0     2887 2023-01-18 14:19:24.378731 opensoundscape-0.9.1/opensoundscape/preprocess/__pycache__/tensor_augment.cpython-39.pyc
+-rw-r--r--   0        0        0     2867 2023-05-26 16:34:12.675285 opensoundscape-0.9.1/opensoundscape/preprocess/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     2877 2023-01-18 14:19:24.382816 opensoundscape-0.9.1/opensoundscape/preprocess/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0        0        0    25696 2023-06-22 16:15:12.089560 opensoundscape-0.9.1/opensoundscape/preprocess/actions.py
+-rw-r--r--   0        0        0      730 2023-01-18 14:19:19.798767 opensoundscape-0.9.1/opensoundscape/preprocess/img_augment.py
+-rw-r--r--   0        0        0    12021 2023-06-22 16:15:12.090214 opensoundscape-0.9.1/opensoundscape/preprocess/preprocessors.py
+-rw-r--r--   0        0        0     2622 2023-01-18 14:19:19.803780 opensoundscape-0.9.1/opensoundscape/preprocess/tensor_augment.py
+-rw-r--r--   0        0        0     2604 2023-01-18 14:19:19.804368 opensoundscape-0.9.1/opensoundscape/preprocess/utils.py
+-rw-r--r--   0        0        0      156 2023-06-15 19:13:05.187993 opensoundscape-0.9.1/opensoundscape/resources/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     8825 2023-06-22 16:15:12.091210 opensoundscape-0.9.1/opensoundscape/ribbit.py
+-rw-r--r--   0        0        0     5217 2023-06-22 16:15:12.092104 opensoundscape-0.9.1/opensoundscape/sample.py
+-rw-r--r--   0        0        0    24153 2023-06-22 16:15:12.095595 opensoundscape-0.9.1/opensoundscape/signal_processing.py
+-rw-r--r--   0        0        0    32654 2023-06-22 16:15:12.096821 opensoundscape-0.9.1/opensoundscape/spectrogram.py
+-rw-r--r--   0        0        0    11598 2023-06-22 16:15:12.097753 opensoundscape-0.9.1/opensoundscape/utils.py
+-rw-r--r--   0        0        0     1707 2023-06-22 16:15:12.102100 opensoundscape-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     6833 1970-01-01 00:00:00.000000 opensoundscape-0.9.1/PKG-INFO
```

### Comparing `opensoundscape-0.9.0/LICENSE` & `opensoundscape-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opensoundscape-0.9.0/README.md` & `opensoundscape-0.9.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -8,44 +8,44 @@
 These utilities can be strung together to create data analysis pipelines. OpenSoundscape is designed to be run on any scale of computer: laptop, desktop, or computing cluster.
 
 OpenSoundscape is currently in active development. If you find a bug, please submit an issue. If you have another question about OpenSoundscape, please email Sam Lapp (`sam.lapp` at `pitt.edu`).
 
 
 #### Suggested Citation
 ```
-Lapp, Rhinehart, Freeland-Haynes, Khilnani, Syunkova, and Kitzes, 2023. "OpenSoundscape v0.9.0".
+Lapp, Rhinehart, Freeland-Haynes, Khilnani, Syunkova, and Kitzes, 2023. "OpenSoundscape v0.9.1".
 ```
 
 # Installation
 
-OpenSoundscape can be installed on Windows, Mac, and Linux machines. It has been tested on Python 3.8, and 3.9. For Apple Silicon (M1 chip) users, Python 3.9 is recommended and may be required to avoid dependency issues.
+OpenSoundscape can be installed on Windows, Mac, and Linux machines. It has been tested on Python 3.8, 3.9, 3.10, and 3.11. For Apple Silicon (M1 chip) users, Python >=3.9 is recommended and may be required to avoid dependency issues.
 
-Most users should install OpenSoundscape via pip: `pip install opensoundscape==0.9.0`. Contributors and advanced users can also use Poetry to install OpenSoundscape.
+Most users should install OpenSoundscape via pip: `pip install opensoundscape==0.9.1`. Contributors and advanced users can also use Poetry to install OpenSoundscape.
 
 For more detailed instructions on how to install OpenSoundscape and use it in Jupyter, see the [documentation](http://opensoundscape.org).
 
 # Features & Tutorials
 OpenSoundscape includes functions to:
 * load and manipulate audio files
 * create and manipulate spectrograms
 * train CNNs on spectrograms with PyTorch
 * run pre-trained CNNs to detect vocalizations
 * detect periodic vocalizations with RIBBIT
 * load and manipulate Raven annotations
+* estimate the location of sound sources from synchronized recordings
 
 OpenSoundscape can also be used with our library of publicly available trained machine learning models for the detection of 500 common North American bird species.
 
 For full API documentation and tutorials on how to use OpenSoundscape to work with audio and spectrograms, train machine learning models, apply trained machine learning models to acoustic data, and detect periodic vocalizations using RIBBIT, see the [documentation](http://opensoundscape.org).
 
 # Quick Start
 
 Using Audio and Spectrogram classes
 ```python
-from opensoundscape.audio import Audio
-from opensoundscape.spectrogram import Spectrogram
+from opensoundscape import Audio, Spectrogram
 
 #load an audio file and trim out a 5 second clip
 my_audio = Audio.from_file("/path/to/audio.wav")
 clip_5s = my_audio.trim(0,5)
 
 #create a spectrogram and plot it
 my_spec = Spectrogram.from_audio(clip_5s)
@@ -74,25 +74,52 @@
 model = load_model('/path/to/saved.model')
 scores = model.predict(files)
 
 #scores is a dataframe with MultiIndex: file, start_time, end_time
 #containing inference scores for each class and each audio window
 ```
 
-Training a CNN with labeled audio data
+Training a CNN using audio files and Raven annotations 
+
+
+```python
+from sklearn.model_selection import train_test_split
+from opensoundscape import BoxedAnnotations, CNN
+
+# assume we have a list of raven annotation files and corresponding audio files
+# load the annotations into OpenSoundscape
+all_annotations = BoxedAnnotations.from_raven_files(raven_file_paths,audio_file_paths)
+
+# pick classes to train the model on. These should occur in the annotated data
+class_list = ['IBWO','BLJA']
+
+# create labels for fixed-duration (2 second) clips 
+labels = all_annotations.one_hot_clip_labels(
+  cip_duration=2,
+  clip_overlap=0,
+  min_label_overlap=0.25,
+  class_subset=class_list
+)
+
+# split the labels into training and validation sets
+train_df, validation_df = train_test_split(labels, test_size=0.3)
+
+# create a CNN and train on the labeled data
+model = CNN(architecture='resnet18', sample_duration=2, classes=class_list)
+model.train(train_df, validation_df, epochs=20, num_workers=8, batch_size=256)
+```
+
+Training a CNN with labeled audio data (one label per audio file):
+
 ```python
 from opensoundscape import CNN
 from sklearn.model_selection import train_test_split
 
 #load a DataFrame of one-hot audio clip labels
 df = pd.read_csv('my_labels.csv') #index: paths; columns: classes
 train_df, validation_df = train_test_split(df,test_size=0.2)
 
-#create a CNN and train on 2-second spectrograms for 2 epochs
-model = CNN('resnet18',classes=df.columns,sample_duration=2.0)
-model.train(
-  train_df,
-  validation_df,
-  epochs=2
-)
+#create a CNN and train on 2-second spectrograms for 20 epochs
+model = CNN('resnet18', classes=df.columns, sample_duration=2.0)
+model.train(train_df, validation_df, epochs=20)
 #the best model is automatically saved to a file `./best.model`
 ```
```

### Comparing `opensoundscape-0.9.0/opensoundscape/__init__.py` & `opensoundscape-0.9.1/opensoundscape/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 from . import annotations
 from . import audio
-from . import aru
 from . import data_selection
 from . import utils
 from . import localization
 from . import metrics
 from . import ribbit
 from . import sample
 from . import signal_processing
 from . import spectrogram
-from . import taxa
 from . import ml
 from . import preprocess
-from . import resources
 from . import logging
 
 # expose some modules at the top level
 from .ml import cnn
 from .preprocess import preprocessors, actions
 
 # expose some classes at the top level
 from .audio import Audio
 from .spectrogram import Spectrogram
 from .ml.cnn import CNN, load_model
 from .ml.datasets import AudioFileDataset, AudioSplittingDataset
 from .preprocess.actions import Action
 from .preprocess.preprocessors import SpectrogramPreprocessor
 from .sample import AudioSample
+from .annotations import BoxedAnnotations
```

### Comparing `opensoundscape-0.9.0/opensoundscape/annotations.py` & `opensoundscape-0.9.1/opensoundscape/annotations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """functions and classes for manipulating annotations of audio
 
 includes BoxedAnnotations class and utilities to combine or "diff" annotations,
 etc.
 """
 from pathlib import Path
-from itertools import chain
+import itertools
 import pandas as pd
 import numpy as np
 import warnings
 
 from opensoundscape.utils import (
     overlap,
     overlap_fraction,
@@ -39,25 +39,26 @@
 
         Args:
             df: DataFrame of frequency-time labels. Columns must include:
                 - "annotation": string or numeric labels (can be None/nan)
                 - "start_time": left bound, sec since beginning of audio
                 - "end_time": right bound, sec since beginning of audio
                 optional columns:
-                - "file": name or path of corresponding audio file
+                - "audio_file": name or path of corresponding audio file
                 - "low_f": lower frequency bound (values can be None/nan)
                 - "high_f": upper frequency bound (values can be None/nan)
             Note: other columns will be retained in the .df
 
         Returns:
             BoxedAnnotations object
 
         """
         standard_cols = [
-            "file",
+            "audio_file",
+            "raven_file",
             "annotation",
             "start_time",
             "end_time",
             "low_f",
             "high_f",
         ]
         required_cols = ["annotation", "start_time", "end_time"]
@@ -76,90 +77,122 @@
 
     def _repr_html_(self):
         return self.df._repr_html_()
 
     @classmethod
     def from_raven_files(
         cls,
-        raven_paths,
+        raven_files,
         audio_files=None,
-        annotation_column_idx=7,
+        annotation_column_idx=8,
+        annotation_column_name=None,
         keep_extra_columns=True,
     ):
         """load annotations from Raven .txt files
 
         Args:
-            raven_paths: list of raven .txt file paths (as str or pathlib.Path)
+            raven_files: list of raven .txt file paths (as str or pathlib.Path)
             audio_files: (list) optionally specify audio files corresponding to each
-                raven file (length should match raven_paths)
+                raven file (length should match raven_files)
             annotation_column_idx: (int) position of column containing annotations
-                - [default: 7] will be correct if the first user-created column
-                in Raven contains annotations
+                - [default: 8] will be correct if the first user-created column
+                in Raven contains annotations. First column is 1, second is 2 etc.
                 - pass `None` to load the raven file without explicitly
                 assigning a column as the annotation column. The resulting
                 object's `.df` will have an `annotation` column with nan values!
+                NOTE: If `annotatino_column_name` is passed, this argument is ignored.
+            annotation_column_name: (str) name of the column containing annotations
+                - default: None will use annotation-column_idx to find the annotation column
+                - if not None, this value overrides annotation_column_idx, and the column with
+                this name will be used as the annotations.
             keep_extra_columns: keep or discard extra Raven file columns
                 (always keeps start_time, end_time, low_f, high_f, annotation
                 audio_file). [default: True]
                 - True: keep all
                 - False: keep none
                 - or iterable of specific columns to keep
 
         Returns:
             BoxedAnnotations object containing annotations from the Raven files
             (the .df attribute is a dataframe containing each annotation)
         """
         all_file_dfs = []
-        for i, raven_path in enumerate(raven_paths):
-            df = pd.read_csv(raven_path, delimiter="\t")
-            if annotation_column_idx is not None:
+        for i, raven_file in enumerate(raven_files):
+            df = pd.read_csv(raven_file, delimiter="\t")
+            if annotation_column_name is not None:
+                # annotation_column_name argument takes precedence over
+                # annotation_column_idx. If it is passed, we use it and ignore
+                # annotation_column_idx!
+                if annotation_column_name in list(df.columns):
+                    df = df.rename(
+                        columns={
+                            annotation_column_name: "annotation",
+                        }
+                    )
+                else:
+                    # to be flexible, we'll give nan values if the column is missing
+                    df["annotation"] = np.nan
+
+            elif annotation_column_idx is not None:
+                # use the column number to specify which column contains annotations
+                # first column is 1, second is 2, etc (default: 8th column)
                 df = df.rename(
                     columns={
-                        df.columns[annotation_column_idx]: "annotation",
+                        df.columns[annotation_column_idx - 1]: "annotation",
                     }
                 )
-            else:
-                # user laoded table without specifying annotation column
+            else:  # None was passed to annotatino_column_idx
                 # we'll create an empty `annotation` column
                 df["annotation"] = np.nan
 
             # rename Raven columns to standard opensoundscape names
             df = df.rename(
                 columns={
                     "Begin Time (s)": "start_time",
                     "End Time (s)": "end_time",
                     "Low Freq (Hz)": "low_f",
                     "High Freq (Hz)": "high_f",
                 }
             )
 
+            # add column containing the raven file path
+            df["raven_file"] = raven_file
+
             # remove undesired columns
             standard_columns = ["start_time", "end_time", "low_f", "high_f"]
             if annotation_column_idx is not None:
                 standard_columns.append("annotation")
-
             if hasattr(keep_extra_columns, "__iter__"):
                 # keep the desired columns
-                df = df[standard_columns + list(keep_extra_columns)]
+                # if values in keep_extra_columns are missing, fill with nan
+                df = df.reindex(
+                    columns=standard_columns + list(keep_extra_columns),
+                    fill_value=np.nan,
+                )
             elif not keep_extra_columns:
                 # only keep required columns
-                df = df[standard_columns]
+                df = df.reindex(columns=standard_columns)
             else:
                 # keep all columns
                 pass
 
             # add audio file column
             if audio_files is not None:
-                df["file"] = audio_files[i]
+                df["audio_file"] = audio_files[i]
             else:
-                df["file"] = np.nan
+                df["audio_file"] = np.nan
 
             all_file_dfs.append(df)
 
-        return cls(df=pd.concat(all_file_dfs).reset_index())
+        # we drop the original index from the Raven annotations when we combine tables
+        # if the dataframes have different columns, we fill missing columns with nan values
+        # and keep all unique columns
+        all_annotations = pd.concat(all_file_dfs).reset_index(drop=True)
+
+        return cls(df=all_annotations)
 
     def to_raven_files(self, save_dir):  # TODO implement to_csv
         """save annotations to a Raven-compatible tab-separated text files
 
         Creates one file per unique audio file in 'file' column of self.df
 
         Args:
@@ -185,33 +218,33 @@
                 "low_f": "Low Freq (Hz)",
                 "high_f": "High Freq (Hz)",
             }
         )
 
         # we will create one selection table for each file
         # this list may contain NaN, which we handle below
-        unique_files = df["file"].unique()
+        unique_files = df["audio_file"].unique()
 
         # If file names are no unique, raise an Exception
         # otherwise, multiple selection table files with the same name would be
         # written to one directory
         file_stems = set([Path(f).stem for f in unique_files])
         if len(file_stems) < len(unique_files):  # TODO write test for this exception
             raise Exception(
                 "File names were not unique! Some files in different folders have the same name. "
                 "Consider subsetting .df to avoid this issue"
             )
 
         for file in unique_files:
             # for NaN values of file, call the output file "unspecified.selections.txt"
             if not file == file:
-                file_df = df[df["file"].isnull()]
+                file_df = df[df["audio_file"].isnull()]
                 fname = "unspecified_audio.selections.txt"
             else:
-                file_df = df[df["file"] == file]
+                file_df = df[df["audio_file"] == file]
                 fname = f"{Path(file).stem}.selections.txt"
             file_df.to_csv(f"{save_dir}/{fname}", sep="\t", index=False)
 
     def subset(self, classes):
         """subset annotations to those from a list of classes
 
         out-of-place operation (returns new filtered BoxedAnnotations object)
@@ -428,17 +461,17 @@
             df = df[df["annotation"].isin(classes)]
 
         # the clip_df should have ['file','start_time','end_time'] as the index
         clip_df[classes] = float("nan")  # add columns for each class
 
         for (file, start, end) in clip_df.index:
             if not file == file:  # file is NaN, get corresponding rows
-                file_df = df[df["file"].isnull()]
+                file_df = df[df["audio_file"].isnull()]
             else:  # subset annotations to this file
-                file_df = df[df.file == file]
+                file_df = df[df["audio_file"] == file]
 
             # warn user if no annotations correspond to this file
             if warn_no_annotations and len(file_df) == 0:
                 warnings.warn(
                     f"No annotations matched the file {file}. All "
                     "clip labels will be zero for this file."
                 )
@@ -506,15 +539,15 @@
                     clip with clip_duration length
         Returns:
             dataframe with index ['file','start_time','end_time'] and columns=classes
         """
 
         # generate list of start and end times for each clip
         # if user passes None for full_duration, try to get the duration from each audio file
-        files = self.df["file"].unique()
+        files = self.df["audio_file"].unique()
         if full_duration is None:
             try:
                 clip_df = make_clip_df(
                     files=[f for f in files if f == f],  # remove NaN if present
                     clip_duration=clip_duration,
                     clip_overlap=clip_overlap,
                     final_clip=final_clip,
@@ -697,15 +730,15 @@
         classes=None: list of classes for one-hot labels. if None,
             taken to be the unique set of values in `labels`
     Returns:
         one_hot: 2d array with 0 for absent and 1 for present
         class_subset: list of classes corresponding to columns in the array
     """
     if class_subset is None:
-        class_subset = list(set(chain(*labels)))
+        class_subset = list(set(itertools.chain(*labels)))
 
     one_hot = np.zeros([len(labels), len(class_subset)]).astype(int)
     for i, sample_labels in enumerate(labels):
         for label in sample_labels:
             if label in class_subset:
                 one_hot[i, class_subset.index(label)] = 1
```

### Comparing `opensoundscape-0.9.0/opensoundscape/audio.py` & `opensoundscape-0.9.1/opensoundscape/audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 resampled audio, you would instead write
 ```
 audio_object = audio_object.resample(22050)
 ```
 
 """
 import warnings
-from datetime import timedelta, datetime
+import datetime
 from pathlib import Path
 import json
 import io
-from urllib.request import urlopen
+import urllib
 
 import numpy as np
-from scipy.fftpack import fft as scipyfft
-from scipy.fft import fftfreq
+import scipy
+
 import librosa
 import soundfile
 import IPython.display
+from aru_metadata_parser.parse import parse_audiomoth_metadata
+from aru_metadata_parser.utils import load_metadata
 
 import opensoundscape
-from opensoundscape.utils import generate_clip_times_df, load_metadata
-from opensoundscape.aru import parse_audiomoth_metadata
+from opensoundscape.utils import generate_clip_times_df
 from opensoundscape.signal_processing import tdoa
-from scipy.signal import butter, sosfiltfilt
 
 DEFAULT_RESAMPLE_TYPE = "soxr_hq"  # changed from kaiser_fast in v0.9.0
 
 
 class OpsoLoadAudioInputError(Exception):
     """Custom exception indicating we can't load input"""
 
@@ -273,20 +273,21 @@
         ## Determine start time / offset ##
         if start_timestamp is not None:
             # user should have provied a localized timestamp as the start_timestamp
             assert (
                 offset is None
             ), "You must not specify both `start_timestamp` and `offset`"
             assert (
-                type(start_timestamp) == datetime and start_timestamp.tzinfo is not None
+                type(start_timestamp) == datetime.datetime
+                and start_timestamp.tzinfo is not None
             ), "start_timestamp must be a localized datetime object"
             assert (
                 metadata is not None
                 and "recording_start_time" in metadata
-                and type(metadata["recording_start_time"]) == datetime
+                and type(metadata["recording_start_time"]) == datetime.datetime
             ), (
                 "metadata did not contain start time timestamp in key `recording_start_time`. "
                 "This key is automatically created when parsing AudioMoth metadata."
             )
             audio_start = metadata["recording_start_time"]
             offset = (start_timestamp - audio_start).total_seconds()
             if offset < 0:
@@ -320,15 +321,15 @@
         # out of bounds warning/exception user if no samples or too short
         if len(samples) == 0:
             error_msg = "audio object has zero samples"
             if out_of_bounds_mode == "raise":
                 raise AudioOutOfBoundsError(error_msg)
             elif out_of_bounds_mode == "warn":
                 warnings.warn(error_msg)
-        elif duration is not None and len(samples) < duration * sr:
+        elif duration is not None and len(samples) < np.floor(duration * sr):
             if offset < 0:
                 error_msg = "requested time period begins before start of recording"
             else:
                 error_msg = (
                     f"Audio object is shorter than requested duration: "
                     f"{len(samples)/sr} sec instead of {duration} sec"
                 )
@@ -348,15 +349,15 @@
 
             # if we loaded part we don't know the file size anymore
             if offset != 0 or duration is not None:
                 metadata["filesize"] = np.nan
 
             # if the offset > 0, we need to update the timestamp
             if "recording_start_time" in metadata and offset > 0:
-                metadata["recording_start_time"] += timedelta(seconds=offset)
+                metadata["recording_start_time"] += datetime.timedelta(seconds=offset)
 
         return cls(samples, sr, resample_type=resample_type, metadata=metadata)
 
     @classmethod
     def from_bytesio(
         cls, bytesio, sample_rate=None, resample_type=DEFAULT_RESAMPLE_TYPE
     ):
@@ -399,15 +400,17 @@
             sample_rate: The final sampling rate of Audio object [default: None]
                 - if None, retains original sample rate
             resample_type: The librosa method to do resampling [default: "kaiser_fast"]
 
         Returns:
             Audio object
         """
-        samples, original_sample_rate = soundfile.read(io.BytesIO(urlopen(url).read()))
+        samples, original_sample_rate = soundfile.read(
+            io.BytesIO(urllib.request.urlopen(url).read())
+        )
         samples = samples.mean(1)  # sum to mono
         if sample_rate is not None and sample_rate != original_sample_rate:
             samples = librosa.resample(
                 samples,
                 orig_sr=original_sample_rate,
                 target_sr=sample_rate,
                 res_type=resample_type,
@@ -490,15 +493,17 @@
 
         # update metadata with new start time and duration
         if self.metadata is None:
             metadata = None
         else:
             metadata = self.metadata.copy()
             if "recording_start_time" in metadata:
-                metadata["recording_start_time"] += timedelta(seconds=start_time)
+                metadata["recording_start_time"] += datetime.timedelta(
+                    seconds=start_time
+                )
 
             if "duration" in metadata:
                 metadata["duration"] = len(samples_trimmed) / self.sample_rate
 
         return self._spawn(
             samples=samples_trimmed,
             metadata=metadata,
@@ -539,42 +544,78 @@
                 metadata["duration"] = len(samples_extended) / self.sample_rate
 
         return self._spawn(
             samples=samples_extended,
             metadata=metadata,
         )
 
-    def extend(self, length):
-        """Extend audio file by adding silence to the end
+    def extend_to(self, duration):
+        """Extend audio file to desired duration by adding silence to the end
+
+        If duration is less than the Audio's .duration, the Audio object is trimmed.
+        Otherwise, silence is added to the end of the Audio object to achieve the desired
+        duration.
 
         Args:
-            length: the final duration in seconds of the extended audio object
+            duration: the final duration in seconds of the audio object
 
         Returns:
             a new Audio object of the desired duration
         """
 
-        total_samples_needed = round(length * self.sample_rate)
-        samples_extended = np.pad(
-            self.samples, pad_width=(0, total_samples_needed - len(self.samples))
-        )
+        target_n_samples = round(duration * self.sample_rate)
+        current_n_samples = len(self.samples)
+
+        if target_n_samples > current_n_samples:
+            # add 0's to the end of the sample array
+            new_samples = np.pad(
+                self.samples, pad_width=(0, target_n_samples - current_n_samples)
+            )
+        elif target_n_samples < current_n_samples:
+            # trim to desired samples (similar to self.trim())
+            new_samples = self.samples[0:target_n_samples]
 
         # update metadata to reflect new duration
         if self.metadata is None:
             metadata = None
         else:
             metadata = self.metadata.copy()
             if "duration" in metadata:
-                metadata["duration"] = len(samples_extended) / self.sample_rate
+                metadata["duration"] = len(new_samples) / self.sample_rate
 
         return self._spawn(
-            samples=samples_extended,
+            samples=new_samples,
             metadata=metadata,
         )
 
+    def extend_by(self, duration):
+        """Extend audio file by adding `duration` seconds of silence to the end
+
+        Args:
+            duration: the final duration in seconds of the audio object
+
+        Returns:
+            a new Audio object with silence added to the end
+        """
+        assert duration >= 0, f"`duration` to extend by must be >=0, got {duration}"
+
+        # create desired duration of silent audio and concatenate to the end
+        silence = Audio.silence(duration=duration, sample_rate=self.sample_rate)
+        new_audio = concat([self, silence])
+
+        # add metadata and update to reflect new duration
+        if self.metadata is None:
+            new_audio.metadata = None
+        else:
+            new_audio.metadata = self.metadata.copy()
+            if "duration" in new_audio.metadata:
+                new_audio.metadata["duration"] = new_audio.duration
+
+        return new_audio
+
     def bandpass(self, low_f, high_f, order):
         """Bandpass audio signal with a butterworth filter
 
         Uses a phase-preserving algorithm (scipy.signal's butter and solfiltfilt)
 
         Args:
             low_f: low frequency cutoff (-3 dB)  in Hz of bandpass filter
@@ -602,18 +643,18 @@
 
         Returns:
             fft, frequencies
         """
 
         # Compute the fft (fast fourier transform) of the selected clip
         N = len(self.samples)
-        fft = scipyfft(self.samples)
+        fft = scipy.fft.fft(self.samples)
 
         # create the frequencies corresponding to fft bins
-        freq = fftfreq(N, d=1 / self.sample_rate)
+        freq = scipy.fft.fftfreq(N, d=1 / self.sample_rate)
 
         # remove negative frequencies and scale magnitude by 2.0/N:
         fft = 2.0 / N * fft[0 : int(N / 2)]
         frequencies = freq[0 : int(N / 2)]
         fft = np.abs(fft)
 
         return fft, frequencies
@@ -777,21 +818,20 @@
             final_clip=final_clip,
         )
 
         clips = [None] * len(clip_df)
         for idx, (start, end) in enumerate(
             zip(clip_df["start_time"], clip_df["end_time"])
         ):
-
             # Trim the clip to desired range
             audio_clip = self.trim(start, end)
 
             # Extend the final clip if necessary
             if end > duration and final_clip == "extend":
-                audio_clip = audio_clip.extend(clip_duration)
+                audio_clip = audio_clip.extend_to(clip_duration)
 
             # Add clip to list of clips
             clips[idx] = audio_clip
 
         if len(clips) == 0:
             warnings.warn(
                 f"Given Audio object with duration of `{duration}` "
@@ -1090,86 +1130,88 @@
         if offsets is not None:
             audio = concat(
                 [Audio.silence(duration=offsets[i], sample_rate=sample_rate), audio]
             )
 
         # pad or truncate to correct length
         if audio.duration < duration:
-            audio = audio.extend(duration)
+            audio = audio.extend_to(duration)
         elif audio.duration > duration:
             audio = audio.trim(0, duration)
 
         # add samples to mixdown
         mixdown += audio.samples
 
     # limit sample values to clip_range
     if clip_range is not None:
         mixdown = np.clip(mixdown, clip_range[0], clip_range[1])
 
     return audio_objects[0]._spawn(samples=mixdown, sample_rate=sample_rate)
 
 
 def estimate_delay(
-    audio,
+    primary_audio,
     reference_audio,
+    max_delay,
     bandpass_range=None,
     bandpass_order=9,
     cc_filter="phat",
     return_cc_max=False,
-    max_delay=None,
     skip_ref_bandpass=False,
 ):
-    """Use generalized cross correlation to estimate time delay between signals
+    """
+    Use generalized cross correlation to estimate time delay between 2 audio objects containing the same signal. The audio objects must be time-synchronized
 
-    optionally bandpass audio signals to a frequency range
+    Optionally bandpass audio signals to a frequency range
 
     For example, if audio is delayed by 1 second compared to reference_audio,
     result is 1.0.
 
     Args:
-        audio, reference_audio: audio objects
+        primary_audio: audio object containing the signal of interest
+        reference_audio: audio object containing the reference signal.
+        max_delay: maximum time delay to consider, in seconds. Must be less than the duration of the primary audio.
+            (see `opensoundscape.signal_processing.tdoa`)
         bandpass_range: if None, no bandpass filter is performed
             otherwise [low_f,high_f]
         bandpass_order: order of Butterworth bandpass filter
         cc_filter: generalized cross correlation type, see
             opensoundscape.signal_processing.gcc() [default: 'phat']
         return_cc_max: if True, returns cross correlation max value as second argument
             (see `opensoundscape.signal_processing.tdoa`)
-        max_delay: maximum time delay to consider, in seconds
-            (see `opensoundscape.signal_processing.tdoa`) [default: None] allows any delay
         skip_ref_bandpass: [default: False] if True, skip the bandpass operation for the
             reference_audio object, only apply it to `audio`
     Returns:
         estimated time delay (seconds) from reference_audio to audio
 
         if return_cc_max is True, also returns a second value, the max of the cross correlation
         of the two signals
 
     Note: resamples reference_audio if its sample rate does not match audio
     """
     # sample rates must match
-    sr = audio.sample_rate
+    sr = primary_audio.sample_rate
     if reference_audio.sample_rate != sr:
         reference_audio = reference_audio.resample(sr)
 
     # apply audio-domain butterworth bandpass filter if desired
     if bandpass_range is not None:
         l, h = bandpass_range  # extract low and high frequencies
-        audio = audio.bandpass(l, h, bandpass_order)
+        primary_audio = primary_audio.bandpass(l, h, bandpass_order)
         if not skip_ref_bandpass:
             reference_audio = reference_audio.bandpass(l, h, bandpass_order)
 
     # estimate time delay from reference_audio to audio using generalized cross correlation
     return tdoa(
-        audio.samples,
+        primary_audio.samples,
         reference_audio.samples,
+        max_delay=max_delay,
         cc_filter=cc_filter,
         sample_rate=sr,
         return_max=return_cc_max,
-        max_delay=max_delay,
     )
 
 
 def parse_opso_metadata(comment_string):
     """parse metadata saved by opensoundcsape as json in comment field
 
     Parses a json string which opensoundscape saves to the comment metadata field
@@ -1192,15 +1234,15 @@
     )
 
     metadata = json.loads(comment_string[13:])
     metadata_version = metadata["opso_metadata_version"]
     if metadata_version == "v0.1":
         # parse and re-format according to opso_metadata_v0.1 formatting
         if "recording_start_time" in metadata:
-            metadata["recording_start_time"] = datetime.fromisoformat(
+            metadata["recording_start_time"] = datetime.datetime.fromisoformat(
                 metadata["recording_start_time"]
             )
     # elif: # implement parsing of future metadata versions here
     else:
         raise NotImplementedError(
             f"Parsing opso_metadata version {metadata_version} "
             "has not been implemented."
@@ -1289,14 +1331,18 @@
 
     return metadata
 
 
 def _write_metadata(metadata, metadata_format, path):
     """write metadata using one of the supported formats
 
+    metadata fields containing empty strings `''` will be replaced by a string
+    containing a single space `' '` as a workaround to
+    https://github.com/bastibe/python-soundfile/issues/386.
+
     Args:
         metadata: dictionary of metadata
         metadata_format: one of 'opso','opso_metadata_v0.1','soundfile'
             (see Audio.wave documentation)
         path: file path to save metadata in with soundfile
     """
     metadata = metadata.copy()  # avoid changing the existing object
@@ -1320,15 +1366,21 @@
             "date",
             "album",
             "license",
             "tracknumber",
             "genre",
         ]:
             if field in metadata and metadata[field] is not None:
-                s.__setattr__(field, metadata[field])
+                value = str(metadata[field])
+                # replace empty strings with a single space, because
+                # empty string as value causes error (see
+                # https://github.com/bastibe/python-soundfile/issues/386)
+                if len(value) < 1:
+                    value = " "
+                s.__setattr__(field, value)
 
 
 def butter_bandpass(low_f, high_f, sample_rate, order=9):
     """generate coefficients for bandpass_filter()
 
     Args:
         low_f: low frequency of butterworth bandpass filter
@@ -1338,15 +1390,17 @@
 
     Returns:
         set of coefficients used in sosfiltfilt()
     """
     nyq = 0.5 * sample_rate
     low = low_f / nyq
     high = high_f / nyq
-    sos = butter(order, [low, high], analog=False, btype="band", output="sos")
+    sos = scipy.signal.butter(
+        order, [low, high], analog=False, btype="band", output="sos"
+    )
     return sos
 
 
 def bandpass_filter(signal, low_f, high_f, sample_rate, order=9):
     """perform a butterworth bandpass filter on a discrete time signal
     using scipy.signal's butter and sosfiltfilt (phase-preserving filtering)
 
@@ -1357,15 +1411,15 @@
         sample_rate: samples per second (Hz)
         order: higher values -> steeper dropoff [default: 9]
 
     Returns:
         filtered time signal
     """
     sos = butter_bandpass(low_f, high_f, sample_rate, order=order)
-    return sosfiltfilt(sos, signal)
+    return scipy.signal.sosfiltfilt(sos, signal)
 
 
 def clipping_detector(samples, threshold=0.6):
     """count the number of samples above a threshold value
 
     Args:
         samples: a time series of float values
```

### Comparing `opensoundscape-0.9.0/opensoundscape/data_selection.py` & `opensoundscape-0.9.1/opensoundscape/data_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """tools for subsetting and resampling collections"""
-from itertools import repeat
+import itertools
 import pandas as pd
 
 
 def resample(
     df,
     n_samples_per_class,
     upsample=True,
@@ -55,15 +55,15 @@
         # and the samples with an 'extra' representation if upsampling
         random_df = sub_df.sample(
             n=remainder, replace=with_replace, random_state=random_state
         )
 
         # if upsampling, repeat all of the samples as many times as necessary
         if num_replicates > 0:
-            repeat_df = pd.concat(repeat(sub_df, num_replicates))
+            repeat_df = pd.concat(itertools.repeat(sub_df, num_replicates))
             class_dfs[idx] = pd.concat([repeat_df, random_df])
         else:
             class_dfs[idx] = random_df
 
     return pd.concat(class_dfs)
 
 
@@ -96,12 +96,12 @@
         sub_df = input_df[input_df[label_column] == unique_label]
         num_replicates, remainder = divmod(max_count, sub_df.shape[0])
 
         random_df = sub_df.sample(
             n=remainder, replace=with_replace, random_state=random_state
         )
 
-        repeat_df = pd.concat(repeat(sub_df, num_replicates))
+        repeat_df = pd.concat(itertools.repeat(sub_df, num_replicates))
 
         dfs[idx] = pd.concat([repeat_df, random_df])
 
     return pd.concat(dfs)
```

### Comparing `opensoundscape-0.9.0/opensoundscape/localization.py` & `opensoundscape-0.9.1/opensoundscape/localization.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,292 +1,286 @@
 """Tools for localizing audio events from synchronized recording arrays"""
 import warnings
 import numpy as np
-import pandas as pd
-from opensoundscape.audio import Audio
-from scipy.signal import correlate, correlation_lags
 
-import opensoundscape.signal_processing as sp
+from opensoundscape.audio import Audio
 from opensoundscape import audio
 
 # define defaults for physical constants
 SPEED_OF_SOUND = 343  # default value in meters per second
 
 
 class InsufficientReceiversError(Exception):
     """raised when there are not enough receivers to localize an event"""
 
     pass
 
 
 class SpatialEvent:
     """
-    Class that estimates the position of a single sound event
+    Class that estimates the location of a single sound event
 
-    Uses reciever positions and time-of-arrival of sounds to estimate
-    soud source position
+    Uses receiver locations and time-of-arrival of sounds to estimate
+    sound source location
     """
 
     def __init__(
         self,
         receiver_files,
-        receiver_positions,
+        receiver_locations,
+        max_delay,
         start_time=0,
         duration=None,
         class_name=None,
         bandpass_range=None,
         cc_threshold=None,
-        max_delay=None,
     ):
         """initialize SpatialEvent
 
         Args:
             receiver_files: list of audio files, one for each reciever
-            receiver_positions: list of [x,y] or [x,y,z] cartesian position of each receiver in meters
-            start_time: start position of detection relative to start of audio file, for cross correlation
+            receiver_locations: list of [x,y] or [x,y,z] cartesian location] of each receiver in meters
+            max_delay: maximum time delay (in seconds) to consider for time-delay-of-arrival estimate. Cannot be longer than the 1/2 the duration.
+            start_time: start location] of detection relative to start of audio file, for cross correlation
             duration: duration of audio segment to use for cross-correlation
             class_name=None: (str) name of detection's class
             tdoas=None: optionally specify relative time difference of arrival of event at each receiver, in
-                seconds. If not None, should be list of same length as receiver_files and receiver_positions
+                seconds. If not None, should be list of same length as receiver_files and receiver_locations
             bandpass_range: [low,high] frequency for audio bandpass before cross-correlation
                 default [None]: does not perform audio bandpass before cross-correlation
             cc_threshold: float, default=None. During localization from time delays, discard time delays and
-                associated positions if max cross correlation value was lower than this threshold.
-                default: None uses all delays and positions regardless of max cc value
-            max_delay: maximum time delay (in seconds) to consider for cross correlation
-                (see `opensoundscape.signal_processing.tdoa`)
+                associated locations if max cross correlation value was lower than this threshold.
+                default: None uses all delays and locations regardless of max cc value
+
 
         Methods:
             estimate_delays:
                 use generalized cross correlation to find time delays of arrival
                 of the event at each receiver
             estimate_location:
-                perform tdoa based position estimation
+                perform tdoa based location estimation
                 - calls estimate_delays() if needed
-            calculate_distance_residuals:
-                compute residuals (descrepancies) between tdoa and estimated position
-            calculate_residual_rms:
-                compute the root mean square value of the tdoa distance residuals
 
         """
         self.receiver_files = receiver_files
-        self.receiver_positions = np.array(receiver_positions)
+        self.receiver_locations = np.array(receiver_locations)
         self.start_time = start_time
         self.duration = duration
         self.class_name = class_name
         self.bandpass_range = bandpass_range
         self.cc_threshold = cc_threshold
         self.max_delay = max_delay
 
+        # check that max_delay is not longer than the duration of the audio and raise a value error if it is
+        if self.max_delay >= self.duration:
+            raise ValueError(
+                f"max_delay ({self.max_delay}) is longer than duration ({self.duration}) of audio clips."
+            )
         # initialize attributes to store values calculated by methods
         self.tdoas = None  # time delay at each receiver
         self.cc_maxs = None  # max of cross correlation for each time delay
-        self.position_estimate = None  # cartesian position estimate in meters
+        self.location_estimate = None  # cartesian location estimate in meters
         self.residual_rms = None
 
         # could implement this later:
         # hidden attributes store estimates and error metrics
         # from gillette and soundfinder localization algorithms
-        # self._gillette_position_estimate = None
+        # self._gillette_location_estimate = None
         # self._gillette_error = None
-        # self._soundfinder_position_estimate = None
+        # self._soundfinder_location_estimate = None
         # self._soundfinder_pseudorange_error = None
 
     def estimate_location(
         self,
         algorithm="gillette",
         cc_threshold=None,
         min_n_receivers=3,
         speed_of_sound=SPEED_OF_SOUND,
     ):
         """
         estimate spatial location of this event
 
-        uses self.tdoas and self.receiver_positions to estimate event location
+        uses self.tdoas and self.receiver_locations to estimate event location
 
-        Note: if self.tdoas or self.receiver_positions is None, first calls
+        Note: if self.tdoas or self.receiver_locations is None, first calls
         self.estimate_delays() to estimate these values
 
         Localization is performed in 2d or 3d according to the dimensions of
-        self.receiver_positions (x,y) or (x,y,z)
+        self.receiver_locations (x,y) or (x,y,z)
 
         Args:
             algorithm: 'gillette' or 'soundfinder', see localization.localize()
             cc_threshold: see SpatialEvent documentation
             min_n_receivers: if number of receivers with cross correlation exceeding
                 the threshold is fewer than this, raises InsufficientReceiversError
-                instead of estimating a spatial position
+                instead of estimating a spatial location
 
         Returns:
-            position estimate as cartesian coordinates (x,y) or (x,y,z) (units: meters)
+            location estimate as cartesian coordinates (x,y) or (x,y,z) (units: meters)
 
         Raises:
             InsufficientReceiversError if the number of receivers with cross correlation
                 maximums exceeding `cc_threshold` is less than `min_n_receivers`
 
         Effects:
-            sets the value of self.position_estimate to the same value as the returned position
+            sets the value of self.location_estimate to the same value as the returned location
         """
+        # if cc_threshold is None, use the value stored in the object
         if cc_threshold is None:
             cc_threshold = self.cc_threshold
 
         # perform generalized cross correlation to estimate time delays
         # (unless values are already stored in attributes)
         if self.tdoas is None or self.cc_maxs is None:
             self.estimate_delays()
 
-        # filter by cross correlation threshold, removing time delays + positions
+        # filter by cross correlation threshold, removing time delays + locations
         # if cross correlation did not exceed a minimum value
         # (low max cross correlation values indicate low confidence that the time
         # delay truly represents two recordings of the same sound event)
         tdoas = self.tdoas
-        positions = self.receiver_positions
+        locations = self.receiver_locations
+        receiver_files = np.array(
+            self.receiver_files
+        )  # needs to be np array to access using a boolean mask
         if cc_threshold is not None:
             tdoas = tdoas[self.cc_maxs > cc_threshold]
-            positions = positions[self.cc_maxs > cc_threshold]
+            locations = locations[self.cc_maxs > cc_threshold]
+            receiver_files = receiver_files[
+                self.cc_maxs > cc_threshold
+            ]  # fails is receiver_files is not a np.array
 
         # assert there are enough receivers remaining to localize the event
         if len(tdoas) < min_n_receivers:
             raise InsufficientReceiversError(
                 f"Number of tdoas exceeding cc threshold ({len(tdoas)} was fewer "
                 f"than min_n_receivers ({min_n_receivers})"
             )
 
-        # estimate location from receiver positions and relative time of arrival
-        # TODO: enable returning error estimates
-        self.position_estimate = localize(
-            receiver_positions=positions,
+        # Store which receivers were used for localization. The location is estimated only from these.
+        self.receivers_used = receiver_files
+
+        # Estimate location from receiver locations and relative Times of Arrival
+        self.location_estimate = localize(
+            receiver_locations=locations,
             tdoas=tdoas,
             algorithm=algorithm,
             speed_of_sound=speed_of_sound,
         )
 
-        # calculate rms distance residual, descrepancy between tdoas and estimated position
-        self.residual_rms = self.calculate_residual_rms(speed_of_sound=speed_of_sound)
+        # Store the distance residuals (only for the receivers used) as an attribute
+        self.distance_residuals = calculate_tdoa_residuals(
+            receiver_locations=locations,
+            tdoas=tdoas,
+            location_estimate=self.location_estimate,
+            speed_of_sound=speed_of_sound,
+        )
 
-        return self.position_estimate
+        # Calculate root mean square of distance residuals and store as attribute
+        self.residual_rms = np.sqrt(np.mean(self.distance_residuals**2))
+
+        self.cc_threshold = (
+            cc_threshold  # update to ensure that the value most recently used is stored
+        )
 
-    def estimate_delays(self, bandpass_range=None, cc_filter="phat", max_delay=None):
+        return self.location_estimate
+
+    def estimate_delays(self, max_delay, bandpass_range=None, cc_filter="phat"):
         """estimate time delay of event relative to receiver_files[0] with gcc
 
         Performs Generalized Cross Correlation of each file against the first,
             extracting the segment of audio of length self.duration at self.start_time
 
         Assumes audio files are synchronized such that they start at the same time
 
         Args:
+            max_delay: only delays in +/- this range (seconds) will be considered for possible delay
+                (see opensoundscape.signal_processing.tdoa())
             bandpass_range: bandpass audio to [low, high] frequencies in Hz before
                 cross correlation; if None, defaults to self.bandpass_range
             cc_filter: filter for generalized cross correlation, see
                 opensoundscape.signal_processing.gcc()
-            max_delay: only consider values in +/- this range (seconds) for possible delay
-                (see opensoundscape.signal_processing.tdoa())
-                - default None allows any delay time
 
         Returns:
             list of time delays, list of max cross correlation values
 
             each list is the same length as self.receiver_files, and each
             value corresponds to the cross correlation of one file relative
             to the first file (self.receiver_files[0])
 
         Effects:
             sets self.tdoas and self.cc_maxs with the same values as those returned
         """
         start, dur = self.start_time, self.duration
-        audio1 = Audio.from_file(self.receiver_files[0], offset=start, duration=dur)
+
+        audio1 = Audio.from_file(
+            self.receiver_files[0],
+            offset=start - max_delay,
+            duration=dur + 2 * max_delay,
+        )
 
         # bandpass once now to avoid repeating operation for each receiver
         if bandpass_range is not None:
             audio1 = audio1.bandpass(bandpass_range[0], bandpass_range[1], order=9)
 
         # estimate time difference of arrival (tdoa) for each file relative to the first
         # skip the first because we don't need to cross correlate a file with itself
         tdoas = [0]  # first file's delay to itself is zero
-        cc_maxs = [1]
-        for file in self.receiver_files[1:]:
-            audio2 = Audio.from_file(file, offset=start, duration=dur)
-            tdoa, cc_max = audio.estimate_delay(
-                audio=audio2,
-                reference_audio=audio1,
-                bandpass_range=bandpass_range,
-                cc_filter=cc_filter,
-                return_cc_max=True,
-                max_delay=max_delay,
-                skip_ref_bandpass=True,
+        cc_maxs = [1]  # set first file's cc_max to 1
+
+        # catch the receivers that have an issue and should be discarded
+        # e.g. their file starts or end during the time-window, so estimate_delays is not possible
+        bad_receivers_index = []
+
+        for index, file in enumerate(self.receiver_files[1:]):
+            audio2 = Audio.from_file(
+                file, offset=start - max_delay, duration=dur + 2 * max_delay
             )
-            tdoas.append(tdoa)
-            cc_maxs.append(cc_max)
+
+            # catch edge cases where the audio lengths do not match.
+            if (
+                abs(len(audio2.samples) - len(audio1.samples)) > 1
+            ):  # allow for 1 sample difference
+                bad_receivers_index.append(index + 1)
+            else:
+                tdoa, cc_max = audio.estimate_delay(
+                    primary_audio=audio2,
+                    reference_audio=audio1,
+                    max_delay=max_delay,
+                    bandpass_range=bandpass_range,
+                    cc_filter=cc_filter,
+                    return_cc_max=True,
+                    skip_ref_bandpass=True,
+                )
+                tdoas.append(tdoa)
+                cc_maxs.append(cc_max)
 
         self.tdoas = np.array(tdoas)
         self.cc_maxs = np.array(cc_maxs)
 
-        return self.tdoas, self.cc_maxs
-
-    def calculate_distance_residuals(self, speed_of_sound=SPEED_OF_SOUND):
-        """calculate distance residuals for each receiver from tdoa localization
-
-        The residual represents the discrepancy between (difference in distance
-        of each reciever to estimated position) and (observed tdoa), and has
-        units of meters.
-
-        Args:
-            speed_of_sound: speed of sound in m/s
-
-        Returns:
-            array of residuals (units are meters), one for each receiver
-
-        Effects:
-            stores the returned residuals as self.distance_residuals
-        """
-        if self.tdoas is None or self.position_estimate is None:
-            warnings.warn(
-                "missing self.tdoas or self.position_estimate, "
-                "returning None for distance_residuals"
+        # delete the bad receivers from this SpatialEvent
+        if len(bad_receivers_index) > 0:
+            print(
+                f"Warning: {len(bad_receivers_index)} receivers were discarded because their audio files were not the same length as the primary receiver."
             )
-            return None
-
-        # store the calcualted tdoas as an attribute
-        self.distance_residuals = calculate_tdoa_residuals(
-            receiver_positions=self.receiver_positions,
-            tdoas=self.tdoas,
-            position_estimate=self.position_estimate,
-            speed_of_sound=speed_of_sound,
-        )
-
-        # return the same residuals
-        # TODO I think this is bad programming because the array could be modified
-        # same issue with other methods of this class
-        return self.distance_residuals
-
-    def calculate_residual_rms(self, speed_of_sound=SPEED_OF_SOUND):
-        """calculate the root mean square distance residual from tdoa localization
-
-        Args:
-            speed_of_sound: speed of sound in meters per second
-
-        Returns:
-            root mean square value of residuals, in meters
-            - returns None if self.tdoas or self.position_estimate
-                are None
-
-        See also: `SpatialEvent.calculate_distance_residuals()`
-        """
-        if self.tdoas is None or self.position_estimate is None:
-            warnings.warn(
-                "missing `self.tdoas` or `self.position_estimate`, "
-                "returning None for residual rms"
+            # drop the bad receivers from the list of files and locations
+            self.receiver_files = [
+                file
+                for index, file in enumerate(self.receiver_files)
+                if index not in bad_receivers_index
+            ]
+
+            self.receiver_locations = np.array(
+                [
+                    location
+                    for index, location in enumerate(self.receiver_locations)
+                    if index not in bad_receivers_index
+                ]
             )
-            return None
-
-        # calculate the residual distance for each reciever
-        # this represents the discrepancy between (difference in distance
-        # of each reciever to estimated position) and (observed tdoa)
-        residuals = self.calculate_distance_residuals(speed_of_sound)
-        return np.sqrt(np.mean(residuals**2))
+        return self.tdoas, self.cc_maxs
 
 
 class SynchronizedRecorderArray:
     """
     Class with utilities for localizing sound events from array of recorders
 
     Methods
@@ -297,49 +291,50 @@
         create_candidate_events()
             Create SpatialEvent objects for all simultaneous, spatially clustered detections of a class
 
         Then, attempts to localize each candidate event via time delay of arrival information:
         For each candidate event:
             - calculate relative time of arrival with generalized cross correlation (event.estimate_delays())
             - if enough cross correlation values exceed a threshold, attempt to localize the event
-                using the time delays and spatial positions of each receiver with event.estimate_location()
+                using the time delays and spatial locations of each receiver with event.estimate_location()
             - if the residual distance rms value is below a cutoff threshold, consider the event
                 to be successfully localized
     """
 
     def __init__(
         self,
         file_coords,
     ):
         """
         Args:
             file_coords : pandas.DataFrame
-                DataFrame with index filepath, and columns for x, y, (z) positions of reciever that
+                DataFrame with index filepath, and columns for x, y, (z) locations of reciever that
                 recorded the audio file, in meters.
                 Third coordinate is optional. Localization algorithms are in 2d if columns are (x,y) and
                 3d if columns are (x,y,z). When running .localize_detections() or .create_candidate_events(),
                 Each audio file in `detections` must have a corresponding
-                row in `file_coords` specifiying the position of the reciever that recorded the file.
+                row in `file_coords` specifiying the location of the reciever that recorded the file.
         """
         self.file_coords = file_coords
 
     def localize_detections(
         self,
         detections,
         max_receiver_dist,
+        max_delay=None,
         min_n_receivers=3,
         localization_algorithm="gillette",
         cc_threshold=0,
         cc_filter="phat",
-        max_delay=None,
         bandpass_ranges=None,
         residual_threshold=np.inf,
+        return_unlocalized=False,
     ):
         """
-        Attempt to localize positions for all detections
+        Attempt to localize locations for all detections
 
         Algorithm
         ----------
         The user provides a table of class detections from each recorder with timestamps.
         The object's self.file_coords dataframe contains a table listing the spatial location of the
         recorder for each unique audio file in the table of detections. The audio recordings must
         be synchronized such that timestamps from each recording correspond to the exact same real-world time.
@@ -377,79 +372,85 @@
             If the max value of the cross correlation is below `cc_threshold`, the corresponding time delay
             is discarded and not used during localization. This provides a way of filtering out
             undesired time delays that do not correspond to two recordings of the same sound event.
 
             If the number of estimated time delays in the candidate event is fewer than `min_n_receivers`
             after filtering by cross correlation threshold, the candidate event is discarded.
 
-        3. Estimate positions
+        3. Estimate locations
 
-            The position of the event is estimated based on the positions and time delays of
+            The location of the event is estimated based on the locations and time delays of
             each detection.
 
-            Position estimation from the positions and time delays at a set of receivers is performed
+            location estimation from the locations and time delays at a set of receivers is performed
             using one of two algorithms, described in `localization_algorithm` below.
 
         4. Filter by spatial residual error
 
             The residual errors represent descrepencies between (a) time of arrival of
-            the event at a reciever and (b) distance from reciever to estimated position.
+            the event at a reciever and (b) distance from reciever to estimated location.
 
-            Estimated positions are discarded if the root mean squared spatial residual is
+            Estimated locations are discarded if the root mean squared spatial residual is
             greater than `residual_rms_threshold`
 
 
         Args:
             detections: a dictionary of detections, with multi-index (file,start_time,end_time), and
                 one column per class with 0/1 values for non-detection/detection
                 The times in the index imply the same real world time across all files: eg 0 seconds assumes
                 that the audio files all started at the same time, not on different dates/times
             max_receiver_dist : float (meters)
                 Radius around a recorder in which to use other recorders for localizing an event.
                 Simultaneous detections at receivers within this distance (meters)
                 of a receiver with a detection will be used to attempt to localize the event.
+            max_delay : float, optional
+                Maximum absolute value of time delay estimated during cross correlation of two signals
+                For instance, 0.2 means that the maximal cross-correlation in the range of
+                delays between -0.2 to 0.2 seconds will be used to estimate the time delay.
+                if None (default), the max delay is set to max_receiver_dist / SPEED_OF_SOUND
             min_n_receivers : int
                 Minimum number of receivers that must detect an event for it to be localized
                 [default: 3]
             localization_algorithm : str, optional
-                algorithm to use for estimating the position of a sound event from the positions and
+                algorithm to use for estimating the location of a sound event from the locations and
                 time delays of a set of detections. [Default: 'gillette']
                 Options:
                     - 'gillette': linear closed-form algorithm of Gillette and Silverman 2008 [1]
-                    - 'soundfinder': GPS position algorithm of Wilson et al. 2014 [2]
+                    - 'soundfinder': GPS location algorithm of Wilson et al. 2014 [2]
             cc_threshold : float, optional
                 Threshold for cross correlation: if the max value of the cross correlation is below
                 this value, the corresponding time delay is discarded and not used during localization.
                 Default of 0 does not discard any delays.
             cc_filter : str, optional
                 Filter to use for generalized cross correlation. See signalprocessing.gcc function for options.
                 Default is "phat".
-            max_delay : float, optional
-                Maximum absolute value of time delay estimated during cross correlation of two signals
-                For instance, 0.2 means that cross correlation will be maximized in the range of
-                delays between -0.2 to 0.2 seconds.
-                Default: None does not restrict the range, finding delay that maximizes cross correlation
             bandpass_ranges : dict, optional
                 Dictionary of form {"class name": [low_f, high_f]} for audio bandpass filtering during
                 cross correlation. [Default: None] does not bandpass audio. Bandpassing audio to the
                 frequency range of the relevant sound is recommended for best cross correlation results.
             residual_threshold: discard localized events if the root mean squared residual exceeds this value
                 (distance in meters) [default: np.inf does not filter out any events by residual]
+            return_unlocalized: bool, optional. If True, returns the unlocalized events as well.
+                Two lists [localized_events, unlocalized events] will be returned.
 
         Returns:
-            2 lists: list of localized events, list of un-localized events
-            events are of class SpatialEvent
+            A list of localized events, each of which is a SpatialEvent object.
+            If return_unlocalized is True, returns:
+                        2 lists: list of localized events, list of un-localized events
 
         [1] M. D. Gillette and H. F. Silverman, "A Linear Closed-Form Algorithm for Source Localization
         From Time-Differences of Arrival," IEEE Signal Processing Letters
 
         [2]  Wilson, David R., Matthew Battiston, John Brzustowski, and Daniel J. Mennill.
         “Sound Finder: A New Software Approach for Localizing Animals Recorded with a Microphone Array.”
         Bioacoustics 23, no. 2 (May 4, 2014): 99–112. https://doi.org/10.1080/09524622.2013.827588.
         """
+        # set max_delay if not provided
+        if max_delay is None:
+            max_delay = max_receiver_dist / SPEED_OF_SOUND
 
         # check that all files have coordinates in file_coords
         if len(self.check_files_missing_coordinates(detections)) > 0:
             raise UserWarning(
                 "WARNING: Not all audio files have corresponding coordinates in self.file_coords."
                 "Check file_coords.index contains each file in detections.index. "
                 "Use self.check_files_missing_coordinates() for list of files. "
@@ -480,96 +481,103 @@
         for event in candidate_events:
             # choose bandpass range based on this event's detected class
             if bandpass_ranges is not None:
                 bandpass_range = bandpass_ranges[event.class_name]
             else:
                 bandpass_range = None
 
-            # perform gcc to estiamte relative time of arrival at each receiver
+            # perform gcc to estimate relative time of arrival at each receiver
             # relative to the first in the list (reference receiver)
             event.estimate_delays(
                 bandpass_range=bandpass_range,
                 cc_filter=cc_filter,
                 max_delay=max_delay,
             )
 
-            # estimate positions of sound event using time delays and receiver positions
+            # estimate locations of sound event using time delays and receiver locations
             try:
                 event.estimate_location(
                     algorithm=localization_algorithm,
                     cc_threshold=cc_threshold,
                     min_n_receivers=min_n_receivers,
                     speed_of_sound=SPEED_OF_SOUND,
                 )
             except InsufficientReceiversError:
                 # this occurs if not enough receivers had high enough cross correlation scores
                 # to continue with localization (<min_n_receivers)
                 unlocalized_events.append(event)
                 continue
 
             # event.residual_rms is computed at the end of event.estimate_location
-            # and represents descrepency (in meters) between tdoas and estimated position
-            # check if residuals are small enough that we consider this a good position estimate
+            # and represents discrepency (in meters) between tdoas and estimated location
+            # check if residuals are small enough that we consider this a good location estimate
             # TODO: use max instead of mean?
             if event.residual_rms < residual_threshold:
                 localized_events.append(event)
             else:
                 unlocalized_events.append(event)
 
         # unlocalized events include those with too few receivers (after cc threshold)
         # and those with too large of a spatial residual rms
-        return localized_events, unlocalized_events
+        if return_unlocalized:
+            return localized_events, unlocalized_events
+        else:
+            return localized_events
 
     def check_files_missing_coordinates(self, detections):
         files_missing_coordinates = []
         files = list(detections.reset_index()["file"].unique())
         for file in files:
             if str(file) not in self.file_coords.index:
                 files_missing_coordinates.append(file)
         return files_missing_coordinates
 
     def create_candidate_events(
         self,
         detections,
         min_n_receivers,
         max_receiver_dist,
+        max_delay=None,
     ):
         """
         Takes the detections dictionary and groups detections that are within `max_receiver_dist` of each other.
         args:
             detections: a dictionary of detections, with multi-index (file,start_time,end_time), and
                 one column per class with 0/1 values for non-detection/detection
                 The times in the index imply the same real world time across all files: eg 0 seconds assumes
                 that the audio files all started at the same time, not on different dates/times
             min_n_receivers: if fewer nearby receivers have a simultaneous detection, do not create candidate event
-            `max_receiver_dist`: the maximum distance between recorders to consider a detection as a single event
+            max_receiver_dist: the maximum distance between recorders to consider a detection as a single event
+            max_delay: the maximum delay (in seconds) to consider between receivers for a single event
+                if None, defaults to max_receiver_dist / SPEED_OF_SOUND
         returns:
             a list of SpatialEvent objects to attempt to localize
         """
+        if max_delay is None:
+            max_delay = max_receiver_dist / SPEED_OF_SOUND
         # pre-generate a dictionary listing all close files for each audio file
         # dictionary will have a key for each audio file, and value listing all other receivers
         # within max_receiver_dist of that receiver
         #
         # eg {ARU_0.mp3: [ARU_1.mp3, ARU_2.mp3...], ARU_1... }
         nearby_files_dict = self.make_nearby_files_dict(max_receiver_dist)
 
         # generate SpatialEvents for each detection, if enough nearby
         # receivers also had a detection at the same time
         # each SpatialEvent object contains the time and class name of a
-        # detected event, a set of receivers' audio files, and receiver positions
+        # detected event, a set of receivers' audio files, and receiver locations
         # and represents a single sound event that we will try to localize
         #
         # events will be redundant because each reciever with detection potentially
         # results in its own event containing nearby detections
         candidate_events = []  # list of SpatialEvents to try to localize
 
         # iterate through all classes in detections (0/1) dataframe
         # with index (file,start_time,end_time), column for each class
         for cls_i in detections.columns:
-
             # select one column: contains 0/1 for each file and clip time period
             # (index: (file,start_time,end_time), values: 0 or 1) for a single class
             det_cls = detections[[cls_i]]
 
             # filter detection dataframe to select detections of this class
             det_cls = det_cls[det_cls[cls_i] > 0]
 
@@ -594,26 +602,27 @@
                     # then, subset files with detections to those that are nearby
                     close_det_files = [f for f in files_w_dets if f in close_receivers]
 
                     # if enough receivers, create a SpatialEvent using this set of receivers
                     # +1 to count the reference receiver
                     if len(close_det_files) + 1 >= min_n_receivers:
                         receiver_files = [ref_file] + close_det_files
-                        receiver_positions = [
+                        receiver_locations = [
                             self.file_coords.loc[r] for r in receiver_files
                         ]
                         # find the clip end time
                         clip = dets_at_time_i.loc[ref_file, time_i, :]
                         clip_end = clip.reset_index()["end_time"].values[0]
 
                         # create a SpatialEvent for this cluster of simultaneous detections
                         candidate_events.append(
                             SpatialEvent(
                                 receiver_files=receiver_files,
-                                receiver_positions=receiver_positions,
+                                receiver_locations=receiver_locations,
+                                max_delay=max_delay,
                                 start_time=time_i,
                                 duration=clip_end - time_i,
                                 class_name=cls_i,
                             )
                         )
 
         return candidate_events
@@ -639,15 +648,15 @@
 
         Returns:
             dictionary with keys for each file and values = list of nearby recordings
         """
         aru_files = self.file_coords.index.values
         nearby_files_dict = dict()
         for aru in aru_files:  # make an entry in the dictionary for each file
-            reference_receiver = self.file_coords.loc[aru]  # position of receiver
+            reference_receiver = self.file_coords.loc[aru]  # location of receiver
             other_receivers = self.file_coords.drop([aru])
             distances = np.array(other_receivers) - np.array(reference_receiver)
             euclid_distances = [np.linalg.norm(d) for d in distances]
 
             # boolean mask for whether recorder is close enough
             mask = [r <= r_max for r in euclid_distances]
             nearby_files_dict[aru] = list(other_receivers[mask].index)
@@ -706,72 +715,71 @@
 
 
 def travel_time(source, receiver, speed_of_sound):
     """
     Calculate time required for sound to travel from a souce to a receiver
 
     Args:
-        source: cartesian position [x,y] or [x,y,z] of sound source, in meters
-        receiver: cartesian position [x,y] or [x,y,z] of sound receiver, in meters
+        source: cartesian location [x,y] or [x,y,z] of sound source, in meters
+        receiver: cartesian location [x,y] or [x,y,z] of sound receiver, in meters
         speed_of_sound: speed of sound in m/s
 
     Returns:
         time in seconds for sound to travel from source to receiver
     """
     distance = np.linalg.norm(np.array(source) - np.array(receiver))
     return distance / speed_of_sound
 
 
-def localize(receiver_positions, tdoas, algorithm, speed_of_sound=SPEED_OF_SOUND):
+def localize(receiver_locations, tdoas, algorithm, speed_of_sound=SPEED_OF_SOUND):
     """
     Perform TDOA localization on a sound event.
     Args:
-        receiver_positions: a list of [x,y,z] positions for each receiver
-            Positions should be in meters, e.g., the UTM coordinate system.
+        receiver_locations: a list of [x,y,z] locations for each receiver
+            locations should be in meters, e.g., the UTM coordinate system.
         tdoas: a list of TDOA times (onset times) for each recorder
             The times should be in seconds.
         speed_of_sound: speed of sound in m/s
         algorithm: the algorithm to use for localization
             Options: 'soundfinder', 'gillette'
     Returns:
-        The estimated source position in meters.
+        The estimated source location in meters.
     """
     if algorithm == "soundfinder":
-        estimate = soundfinder_localize(receiver_positions, tdoas, speed_of_sound)
+        estimate = soundfinder_localize(receiver_locations, tdoas, speed_of_sound)
     elif algorithm == "gillette":
-        estimate = gillette_localize(receiver_positions, tdoas, speed_of_sound)
+        estimate = gillette_localize(receiver_locations, tdoas, speed_of_sound)
     else:
         raise ValueError(
             f"Unknown algorithm: {algorithm}. Implemented for 'soundfinder' and 'gillette'"
         )
     return estimate
 
 
 def soundfinder_localize(
-    receiver_positions,
+    receiver_locations,
     arrival_times,
     speed_of_sound=SPEED_OF_SOUND,
     invert_alg="gps",  # options: 'gps'
     center=True,  # True for original Sound Finder behavior
     pseudo=True,  # False for original Sound Finder
 ):
-
     """
     Use the soundfinder algorithm to perform TDOA localization on a sound event
     Localize a sound event given relative arrival times at multiple receivers.
     This function implements a localization algorithm from the
     equations described in [1]. Localization can be performed in a global coordinate
-    system in meters (i.e., UTM), or relative to recorder positions
+    system in meters (i.e., UTM), or relative to recorder locations
     in meters.
 
     This implementation follows [2] with corresponding variable names.
 
     Args:
-        receiver_positions: a list of [x,y,z] positions for each receiver
-          Positions should be in meters, e.g., the UTM coordinate system.
+        receiver_locations: a list of [x,y,z] locations for each receiver
+          locations should be in meters, e.g., the UTM coordinate system.
         arrival_times: a list of TDOA times (onset times) for each recorder
           The times should be in seconds.
         speed of sound: speed of sound in m/s
         invert_alg: what inversion algorithm to use (only 'gps' is implemented)
         center: whether to center recorders before computing localization
           result. Computes localization relative to centered plot, then
           translates solution back to original recorder locations.
@@ -783,43 +791,43 @@
     Returns:
         The solution (x,y,z) in meters.
 
     [1]  Wilson, David R., Matthew Battiston, John Brzustowski, and Daniel J. Mennill.
     “Sound Finder: A New Software Approach for Localizing Animals Recorded with a Microphone Array.”
     Bioacoustics 23, no. 2 (May 4, 2014): 99–112. https://doi.org/10.1080/09524622.2013.827588.
 
-    [2] Global Positioning Systems handout, 2002
+    [2] Global locationing Systems handout, 2002
     http://web.archive.org/web/20110719232148/http://www.macalester.edu/~halverson/math36/GPS.pdf
     """
 
     # make sure our inputs follow consistent format
-    receiver_positions = np.array(receiver_positions).astype("float64")
+    receiver_locations = np.array(receiver_locations).astype("float64")
     arrival_times = np.array(arrival_times).astype("float64")
 
     # The number of dimensions in which to perform localization
-    dim = receiver_positions.shape[1]
+    dim = receiver_locations.shape[1]
     assert dim in [2, 3], "localization only works in 2 or 3 dimensions"
 
     ##### Shift coordinate system to center receivers around origin #####
     if center:
-        p_mean = np.mean(receiver_positions, 0)
-        receiver_positions = np.array([p - p_mean for p in receiver_positions])
+        p_mean = np.mean(receiver_locations, 0)
+        receiver_locations = np.array([p - p_mean for p in receiver_locations])
 
     ##### Compute B, a, and e #####
     # these correspond to [2] and are defined directly after equation 6
 
     # Find the pseudorange, rho, for each recorder
     # pseudorange (minus a constant) ~= distances from source to each receiver
     rho = np.array([arrival_times * (-1 * speed_of_sound)]).T
 
-    # Concatenate the pseudorange column with x,y,z position to form matrix B
-    B = np.concatenate((receiver_positions, rho), axis=1)
+    # Concatenate the pseudorange column with x,y,z location to form matrix B
+    B = np.concatenate((receiver_locations, rho), axis=1)
 
     # e is a vector of ones
-    e = np.ones(receiver_positions.shape[0])
+    e = np.ones(receiver_locations.shape[0])
 
     # a is a 1/2 times a vector of squared Lorentz norms
     a = 0.5 * np.apply_along_axis(lorentz_ip, axis=1, arr=B)
 
     # choose between two algorithms to invert the matrix
     if invert_alg != "gps":
         raise NotImplementedError
@@ -904,15 +912,15 @@
         u0 += shift
         u1 += shift
 
     # Select and return quadratic solution
     if pseudo:
         # Return the solution with the lower estimate of b, error in pseudorange
         # drop the estimate of b (error in pseudorange) from the return values,
-        # returning just the position vector
+        # returning just the location vector
         if abs(u0[-1]) <= abs(u1[-1]):
             return u0[0:-1]
         else:
             return u1[0:-1]
 
     else:
         # use the sum of squares discrepancy to choose the solution
@@ -921,27 +929,27 @@
 
         # Compute sum of squares discrepancies for each solution
         s0 = float(np.sum((np.matmul(B, u0) - np.add(a, lamb[0] * e)) ** 2))
         s1 = float(np.sum((np.matmul(B, u1) - np.add(a, lamb[1] * e)) ** 2))
 
         # Return the solution with lower sum of squares discrepancy
         # drop the final value, which is the estimate of b, error in the pseudorange,
-        # returning just the position vector
+        # returning just the location vector
         if s0 < s1:
             return u0[0:-1]
         else:
             return u1[0:-1]
 
 
-def gillette_localize(receiver_positions, arrival_times, speed_of_sound=SPEED_OF_SOUND):
+def gillette_localize(receiver_locations, arrival_times, speed_of_sound=SPEED_OF_SOUND):
     """
     Uses the Gillette and Silverman [1] localization algorithm to localize a sound event from a set of TDOAs.
     Args:
-        receiver_positions: a list of [x,y] or [x,y,z] positions for each receiver
-            Positions should be in meters, e.g., the UTM coordinate system.
+        receiver_locations: a list of [x,y] or [x,y,z] locations for each receiver
+            locations should be in meters, e.g., the UTM coordinate system.
         arrival_times: a list of TDOA times (arrival times) for each receiver
             The times should be in seconds.
         speed_of_sound: speed of sound in m/s
     Returns:
         coords: a tuple of (x,y,z) coordinates of the sound source
 
 
@@ -957,23 +965,23 @@
         raise ValueError(
             "Arrival times must be relative to a reference receiver. Therefore one arrival"
             " time must be 0 (corresponding to arrival at the reference receiver) None of your "
             "TDOAs are zero. Please check your arrival_times."
         )
 
     # make sure our inputs follow consistent format
-    receiver_positions = np.array(receiver_positions).astype("float64")
+    receiver_locations = np.array(receiver_locations).astype("float64")
     arrival_times = np.array(arrival_times).astype("float64")
 
     # The number of dimensions in which to perform localization
-    dim = receiver_positions.shape[1]
+    dim = receiver_locations.shape[1]
 
     # find which is the reference receiver and reorder, so reference receiver is first
     ref_receiver = np.argmin(abs(arrival_times))
-    ordered_receivers = np.roll(receiver_positions, -ref_receiver, axis=0)
+    ordered_receivers = np.roll(receiver_locations, -ref_receiver, axis=0)
     ordered_tdoas = np.roll(arrival_times, -ref_receiver, axis=0)
 
     # Gillette silverman solves Ax = w, where x is the solution vector, A is a matrix, and w is a vector
     # Matrix A according to Gillette and Silverman (2008)
     A = np.zeros((len(ordered_tdoas) - 1, dim + 1))
     for column in range(dim + 1):
         if column < dim:
@@ -994,60 +1002,60 @@
     # pseudorange = answer[0][dim]
     # residuals = answer[1]
 
     return coords
 
 
 def calculate_tdoa_residuals(
-    receiver_positions, tdoas, position_estimate, speed_of_sound
+    receiver_locations, tdoas, location_estimate, speed_of_sound
 ):
     """
     Calculate the residual distances of the TDOA localization algorithm
 
     The residual represents the discrepancy between (difference in distance
-    of each reciever to estimated position) and (observed tdoa), and has
+    of each reciever to estimated location) and (observed tdoa), and has
     units of meters. Residuals are calculated as follows:
 
         expected = calculated time difference of arrival between reference and
-            another receiver, based on the positions of the receivers and
-            estimated event position
+            another receiver, based on the locations of the receivers and
+            estimated event location
         observed = observed tdoas provided to localization algorithm
 
         residual time = expected - observed (in seconds)
 
         residual distance = speed of sound * residual time (in meters)
 
     Args:
-        receiver_position: The list of coordinates (in m) of each receiver,
+        receiver_location: The list of coordinates (in m) of each receiver,
             as [x,y] for 2d or or [x,y,z] for 3d.
         tdoas: List of time delays of arival for the sound at each receiver,
             relative to the first receiver in the list (tdoas[0] should be 0)
-        position_estimate: The estimated position of the sound, as (x,y) or (x,y,z) in meters
+        location_estimate: The estimated location of the sound, as (x,y) or (x,y,z) in meters
         speed_of_sound: The speed of sound in m/s
 
     Returns:
         np.array containing the residuals in units of meters, one per receiver
     """
     # ensure all are numpy arrays
-    receiver_positions = np.array(receiver_positions)
+    receiver_locations = np.array(receiver_locations)
     tdoas = np.array(tdoas)
-    position_estimate = np.array(position_estimate)
+    location_estimate = np.array(location_estimate)
 
     # Calculate the TDOA residuals
 
-    # calculate time sound would take to travel from the estimated position
+    # calculate time sound would take to travel from the estimated location
     # to each receiver (distance/speed=time)
-    distances = [np.linalg.norm(r - position_estimate) for r in receiver_positions]
+    distances = [np.linalg.norm(r - location_estimate) for r in receiver_locations]
     travel_times = np.array(distances) / speed_of_sound
 
     # the expected time _difference_ of arrival for any receiver vs the
     # reference receiver is the difference in travel times from the
-    # position estimate to each of the receivers compared to the first
+    # location estimate to each of the receivers compared to the first
     expected_tdoas = travel_times - travel_times[0]
 
     # the time residual is the difference between the observed tdoa values
-    # and those expected according to the estimated position
+    # and those expected according to the estimated location
     # first value will be 0 by definition
     time_residuals = expected_tdoas - tdoas
 
     # convert residuals from units of time (s) to distance (m) via speed of sound
     return time_residuals * speed_of_sound
```

### Comparing `opensoundscape-0.9.0/opensoundscape/logging.py` & `opensoundscape-0.9.1/opensoundscape/logging.py`

 * *Files identical despite different names*

### Comparing `opensoundscape-0.9.0/opensoundscape/metrics.py` & `opensoundscape-0.9.1/opensoundscape/metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 #!/usr/bin/env python
-from sklearn.metrics import (
-    jaccard_score,
-    hamming_loss,
-    precision_recall_fscore_support,
-    confusion_matrix,
-    average_precision_score,
-    roc_auc_score,
-)
+import sklearn.metrics as M
 import pandas as pd
 
 # from scipy.sparse import csr_matrix
 import numpy as np
 import torch
-from torch.nn.functional import one_hot
 
 
 def predict_single_target_labels(scores):
     """Generate boolean single target predicted labels from continuous scores
 
     For each row, the single highest scoring class will be labeled 1 and
     all other classes will be labeled 0.
@@ -51,15 +43,15 @@
         return_type = "torch"
     else:
         raise ValueError(
             f"Expected input type numpy.ndarray, torch.tensor, list, "
             f"or pandas.DataFrame. Got {type(scores)}."
         )
 
-    preds = one_hot(scores.argmax(1), len(scores[0]))
+    preds = torch.nn.functional.one_hot(scores.argmax(1), len(scores[0]))
 
     if return_type == "pandas":
         return pd.DataFrame(preds.numpy(), index=df.index, columns=df.columns)
     elif return_type == "numpy":
         return preds.numpy()
     elif return_type == "list":
         return preds.tolist()
@@ -155,15 +147,15 @@
         metrics_dict: dictionary of various overall and per-class metrics
     """
     metrics_dict = {}
 
     preds = predict_multi_target_labels(scores=scores, threshold=threshold)
 
     # Store per-class precision, recall, and f1
-    class_pre, class_rec, class_f1, _ = precision_recall_fscore_support(
+    class_pre, class_rec, class_f1, _ = M.precision_recall_fscore_support(
         targets, preds, average=None, zero_division=0
     )
 
     for i, class_i in enumerate(class_names):
         metrics_dict.update(
             {
                 class_i: {
@@ -176,27 +168,29 @@
 
     # macro scores are averaged across classes
     metrics_dict["precision"] = class_pre.mean()
     metrics_dict["recall"] = class_rec.mean()
     metrics_dict["f1"] = class_f1.mean()
 
     try:
-        metrics_dict["jaccard"] = jaccard_score(targets, preds, average="macro")
+        metrics_dict["jaccard"] = M.jaccard_score(targets, preds, average="macro")
     except ValueError:
         metrics_dict["jaccard"] = np.nan
     try:
-        metrics_dict["hamming_loss"] = hamming_loss(targets, preds)
+        metrics_dict["hamming_loss"] = M.hamming_loss(targets, preds)
     except ValueError:
         metrics_dict["hamming_loss"] = np.nan
     try:
-        metrics_dict["map"] = average_precision_score(targets, scores, average="macro")
+        metrics_dict["map"] = M.average_precision_score(
+            targets, scores, average="macro"
+        )
     except ValueError:
         metrics_dict["map"] = np.nan
     try:
-        metrics_dict["au_roc"] = roc_auc_score(targets, scores, average="macro")
+        metrics_dict["au_roc"] = M.roc_auc_score(targets, scores, average="macro")
     except ValueError:
         metrics_dict["au_roc"] = np.nan
 
     return metrics_dict
 
 
 def single_target_metrics(targets, scores):
@@ -223,25 +217,25 @@
     metrics_dict = {}
 
     preds = predict_single_target_labels(scores=scores)
 
     # Confusion matrix requires numbered-class not one-hot labels
     t = np.argmax(targets, 1)
     p = np.argmax(preds, 1)
-    metrics_dict["confusion_matrix"] = confusion_matrix(t, p)
+    metrics_dict["confusion_matrix"] = M.confusion_matrix(t, p)
 
     # precision, recall, and f1
-    pre, rec, f1, _ = precision_recall_fscore_support(
+    pre, rec, f1, _ = M.precision_recall_fscore_support(
         targets, preds, average=None, zero_division=0
     )
     metrics_dict.update({"precision": pre[1], "recall": rec[1], "f1": f1[1]})
 
     try:
-        metrics_dict["jaccard"] = jaccard_score(targets, preds, average="macro")
+        metrics_dict["jaccard"] = M.jaccard_score(targets, preds, average="macro")
     except ValueError:
         metrics_dict["jaccard"] = np.nan
     try:
-        metrics_dict["hamming_loss"] = hamming_loss(targets, preds)
+        metrics_dict["hamming_loss"] = M.hamming_loss(targets, preds)
     except ValueError:
         metrics_dict["hamming_loss"] = np.nan
 
     return metrics_dict
```

### Comparing `opensoundscape-0.9.0/opensoundscape/ml/cam.py` & `opensoundscape-0.9.1/opensoundscape/ml/cam.py`

 * *Files identical despite different names*

### Comparing `opensoundscape-0.9.0/opensoundscape/ml/cnn.py` & `opensoundscape-0.9.1/opensoundscape/ml/cnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,17 @@
 import copy
 import os
 import types
 import yaml
 
 import numpy as np
 import pandas as pd
-from pandas.core.indexes.multi import MultiIndex
 
 import torch
-import torch.optim as optim
 import torch.nn.functional as F
-from torch.utils.data import DataLoader
 
 import opensoundscape
 from opensoundscape.ml import cnn_architectures
 from opensoundscape.ml.utils import (
     BaseModule,
     apply_activation_layer,
 )
@@ -83,15 +80,14 @@
         architecture,
         classes,
         sample_duration,
         single_target=False,
         preprocessor_class=SpectrogramPreprocessor,
         sample_shape=(224, 224, 3),
     ):
-
         super(CNN, self).__init__()
 
         self.name = "CNN"
 
         # model characteristics
         self.current_epoch = 0
         self.classes = classes
@@ -108,16 +104,16 @@
         )
         self.loss_fn = None
         self.train_loader = None
         self.scheduler = None
 
         # to use a custom DataLoader or Sampler, change these attributes
         # to the custom class (init must take same arguments)
-        self.train_dataloader_cls = DataLoader
-        self.inference_dataloader_cls = DataLoader
+        self.train_dataloader_cls = torch.utils.data.DataLoader
+        self.inference_dataloader_cls = torch.utils.data.DataLoader
 
         ### architecture ###
         # can be a pytorch CNN such as Resnet18 or a custom object
         # must have .forward(), .train(), .eval(), .to(), .state_dict()
         # for convenience, also allows user to provide string matching
         # a key from cnn_architectures.ARCH_DICT
         num_channels = sample_shape[2]
@@ -164,15 +160,15 @@
             self.loss_cls = CrossEntropyLoss_hot
         else:  # for multi-target, use binary cross entropy
             self.loss_cls = BCEWithLogitsLoss_hot
 
         ### training parameters ###
         # optimizer
         self.opt_net = None  # don't set directly. initialized during training
-        self.optimizer_cls = optim.SGD  # or torch.optim.Adam, etc
+        self.optimizer_cls = torch.optim.SGD  # or torch.optim.Adam, etc
 
         # instead of putting "params" key here, we only add it during
         # _init_optimizer, just before initializing the optimizers
         # this avoids an issue when re-loading a model of
         # having the wrong .parameters() list
         self.optimizer_params = {
             # "params": self.network.parameters(),
@@ -291,15 +287,15 @@
             optim_state_dict = self.opt_net.state_dict()
             self.opt_net = self._init_optimizer()
             self.opt_net.load_state_dict(optim_state_dict)
         else:
             self.opt_net = self._init_optimizer()
 
         # Set up learning rate cooling schedule
-        self.scheduler = optim.lr_scheduler.StepLR(
+        self.scheduler = torch.optim.lr_scheduler.StepLR(
             self.opt_net,
             step_size=self.lr_update_interval,
             gamma=self.lr_cooling_factor,
             last_epoch=self.current_epoch - 1,
         )
 
     def _train_epoch(self, train_loader, wandb_session=None):
@@ -535,15 +531,14 @@
         # Initialize attributes
         self.log_interval = log_interval
         self.save_interval = save_interval
         self.save_path = save_path
 
         # Initialize Weights and Biases (wandb) logging ###
         if wandb_session is not None:
-
             # update the run config with information about the model
             wandb_session.config.update(self._generate_wandb_config())
 
             # update the run config with training parameters
             wandb_session.config.update(
                 dict(
                     epochs=epochs,
@@ -805,15 +800,15 @@
         if not self.architecture_name in cnn_architectures.list_architectures():
             warnings.warn(
                 f"""\n The value of `self.architecture_name` ({self.architecture_name})
                     is not an architecture that can be generated in OpenSoundscape. Using
                     CNN.from_torch_dict on the saved file will cause an error. To fix this,
                     you can use .save() instead of .save_torch_model, or change 
                     `self.architecture_name` to one of the architecture name strings listed by 
-                    opensoundscape.torch.architectures.cnn_architectures.list_architectures()
+                    opensoundscape.ml.cnn_architectures.list_architectures()
                     if this architecture is supported."""
             )
 
         os.makedirs(Path(path).parent, exist_ok=True)
 
         # save just the basics, loses preprocessing/other settings
         torch.save(
@@ -905,15 +900,18 @@
             "(c) (file,start_time,end_time) as MultiIndex"
         )
 
         # set up prediction Dataset, considering three possible cases:
         # (c1) user provided multi-index df with file,start_time,end_time of clips
         # (c2) user provided file list and wants clips to be split out automatically
         # (c3) split_files_into_clips=False -> one sample & one prediction per file provided
-        if type(samples) == pd.DataFrame and type(samples.index) == MultiIndex:  # c1
+        if (
+            type(samples) == pd.DataFrame
+            and type(samples.index) == pd.core.indexes.multi.MultiIndex
+        ):  # c1
             prediction_dataset = AudioFileDataset(
                 samples=samples, preprocessor=self.preprocessor
             )
         elif split_files_into_clips:  # c2
             prediction_dataset = AudioSplittingDataset(
                 samples=samples,
                 preprocessor=self.preprocessor,
@@ -934,17 +932,14 @@
                 "The columns of input samples df differ from `model.classes`."
             )
 
         if len(prediction_dataset) < 1:
             warnings.warn(
                 "prediction_dataset has zero samples. No predictions will be generated."
             )
-            prediction_dataset = AudioFileDataset(
-                samples=[], preprocessor=self.preprocessor
-            )
 
         # If unsafe_behavior= "substitute", a SafeDataset will not fail on bad files,
         # but will provide a different sample! Later we go back and replace scores
         # with np.nan for the bad samples (using safe_dataset._invalid_indices)
         # this approach to error handling feels hacky
         # however, returning None would break the batching of samples
         # "raise" behavior will raise exceptions
@@ -1070,15 +1065,14 @@
             batch_size=batch_size,
             num_workers=num_workers,
             raise_errors=raise_errors,
         )
 
         # Initialize Weights and Biases (wandb) logging
         if wandb_session is not None:
-
             # update the run config with information about the model
             wandb_session.config.update(self._generate_wandb_config())
 
             # update the run config with prediction parameters
             wandb_session.config.update(
                 dict(
                     batch_size=batch_size,
@@ -1341,15 +1335,14 @@
                     batch_maps = pd.Series(
                         {c: cam(batch_tensors, targets=target(c)) for c in classes}
                     )
 
             # update the AudioSample objects to include the activation maps
             # and create guided backprop maps, one at a time
             for i, sample in enumerate(samples):
-
                 if cam is None:
                     activation_maps = None
                 else:
                     # extract this sample's activation maps from batch (all classes)
                     activation_maps = pd.Series(
                         {c: batch_maps[c][i] for c in batch_maps.index}
                     )
@@ -1698,15 +1691,15 @@
     >=0.6.0, you must re-load the model
     using the original package version and save it's network's state dict, i.e.,
     `torch.save(model.network.state_dict(),path)`, then load the state dict
     to a new model object with model.load_weights(). See the
     `Predict with pre-trained CNN` tutorial for details.
 
     For models created with the same version of OpenSoundscape as the one
-    you are using, simply use opensoundscape.torch.models.cnn.load_model().
+    you are using, simply use opensoundscape.ml.cnn.load_model().
 
     Note: for future use of the loaded model, you can simply call
     `model.save(path)` after creating it, then reload it with
     `model = load_model(path)`.
     The saved model will be fully compatible with opensoundscape >=0.7.0.
 
     Examples:
```

### Comparing `opensoundscape-0.9.0/opensoundscape/ml/cnn_architectures.py` & `opensoundscape-0.9.1/opensoundscape/ml/cnn_architectures.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,37 +13,34 @@
 
 To use these wrappers, for example, if your
 model has 10 output classes, write
 
 `my_arch=resnet18(10)`
 
 Then you can initialize a model object from
-`opensoundscape.torch.models.cnn` with your architecture:
+`opensoundscape.ml.cnn` with your architecture:
 
 `model=CNN(my_arch,classes,sample_duration)`
 
 or override an existing model's architecture:
 
 `model.network = my_arch`
 
 Note: the InceptionV3 architecture must be used differently than other
 architectures - the easiest way is to simply use the InceptionV3 class in
-opensoundscape.torch.models.cnn.
+opensoundscape.ml.cnn.
 """
 import warnings
 
-from torchvision import models
-from torch import nn
 import torch
-from torchvision.models.inception import BasicConv2d
+import torchvision
 
 ARCH_DICT = dict()
 
 # inspiration from zhmiao/BirdMultiLabel
-import torch.nn as nn
 
 
 def register_arch(func):
     """add architecture to ARCH_DICT"""
     # register the model in dictionary
     ARCH_DICT[func.__name__] = func
     # return the function
@@ -78,15 +75,15 @@
         weights:
             string containing version name of the pre-trained classification weights to use for this architecture.
             if 'DEFAULT', model is loaded with best available weights (note that these may change across versions).
             Pre-trained weights available for each architecture are listed at https://pytorch.org/vision/stable/models.html
         num_channels:
             specify channels in input sample, eg [channels h,w] sample shape
     """
-    architecture_ft = models.resnet18(weights=weights)
+    architecture_ft = torchvision.models.resnet18(weights=weights)
     if freeze_feature_extractor:
         freeze_params(architecture_ft)
 
     # change number of output nodes
     architecture_ft.fc = change_fc_output_size(architecture_ft.fc, num_classes)
 
     # change input shape num_channels
@@ -115,15 +112,15 @@
         weights:
             string containing version name of the pre-trained classification weights to use for this architecture.
             if 'DEFAULT', model is loaded with best available weights (note that these may change across versions).
             Pre-trained weights available for each architecture are listed at https://pytorch.org/vision/stable/models.html
         num_channels:
             specify channels in input sample, eg [channels h,w] sample shape
     """
-    architecture_ft = models.resnet34(weights=weights)
+    architecture_ft = torchvision.models.resnet34(weights=weights)
     if freeze_feature_extractor:
         freeze_params(architecture_ft)
 
     # change number of output nodes
     architecture_ft.fc = change_fc_output_size(architecture_ft.fc, num_classes)
 
     # change input shape num_channels
@@ -152,15 +149,15 @@
         weights:
             string containing version name of the pre-trained classification weights to use for this architecture.
             if 'DEFAULT', model is loaded with best available weights (note that these may change across versions).
             Pre-trained weights available for each architecture are listed at https://pytorch.org/vision/stable/models.html
         num_channels:
             specify channels in input sample, eg [channels h,w] sample shape
     """
-    architecture_ft = models.resnet50(weights=weights)
+    architecture_ft = torchvision.models.resnet50(weights=weights)
     if freeze_feature_extractor:
         freeze_params(architecture_ft)
 
     # change number of output nodes
     architecture_ft.fc = change_fc_output_size(architecture_ft.fc, num_classes)
 
     # change input shape num_channels
@@ -189,15 +186,15 @@
         weights:
             string containing version name of the pre-trained classification weights to use for this architecture.
             if 'DEFAULT', model is loaded with best available weights (note that these may change across versions).
             Pre-trained weights available for each architecture are listed at https://pytorch.org/vision/stable/models.html
         num_channels:
             specify channels in input sample, eg [channels h,w] sample shape
     """
-    architecture_ft = models.resnet101(weights=weights)
+    architecture_ft = torchvision.models.resnet101(weights=weights)
     if freeze_feature_extractor:
         freeze_params(architecture_ft)
 
     # change number of output nodes
     architecture_ft.fc = change_fc_output_size(architecture_ft.fc, num_classes)
 
     # change input shape num_channels
@@ -226,15 +223,15 @@
         weights:
             string containing version name of the pre-trained classification weights to use for this architecture.
             if 'DEFAULT', model is loaded with best available weights (note that these may change across versions).
             Pre-trained weights available for each architecture are listed at https://pytorch.org/vision/stable/models.html
         num_channels:
             specify channels in input sample, eg [channels h,w] sample shape
     """
-    architecture_ft = models.resnet152(weights=weights)
+    architecture_ft = torchvision.models.resnet152(weights=weights)
     if freeze_feature_extractor:
         freeze_params(architecture_ft)
 
     # prevent weights of feature extractor from being trained, if desired
     if freeze_feature_extractor:
         freeze_params(architecture_ft)
 
@@ -267,15 +264,15 @@
         weights:
             string containing version name of the pre-trained classification weights to use for this architecture.
             if 'DEFAULT', model is loaded with best available weights (note that these may change across versions).
             Pre-trained weights available for each architecture are listed at https://pytorch.org/vision/stable/models.html
         num_channels:
             specify channels in input sample, eg [channels h,w] sample shape
     """
-    architecture_ft = models.alexnet(weights=weights)
+    architecture_ft = torchvision.models.alexnet(weights=weights)
     if freeze_feature_extractor:
         freeze_params(architecture_ft)
 
     # change number of output nodes
     architecture_ft.classifier[6] = change_fc_output_size(
         architecture_ft.classifier[6], num_classes
     )
@@ -307,15 +304,15 @@
             if True, feature block is frozen and only final layer is trained
         weights:
             string containing version name of the pre-trained classification weights to use for this architecture.
             if 'DEFAULT', model is loaded with best available weights (note that these may change across versions).
             Pre-trained weights available for each architecture are listed at https://pytorch.org/vision/stable/models.html
 
     """
-    architecture_ft = models.vgg11_bn(weights=weights)
+    architecture_ft = torchvision.models.vgg11_bn(weights=weights)
 
     if freeze_feature_extractor:
         freeze_params(architecture_ft)
 
     # change number of output nodes
     architecture_ft.classifier[6] = change_fc_output_size(
         architecture_ft.classifier[6], num_classes
@@ -349,15 +346,15 @@
         weights:
             string containing version name of the pre-trained classification weights to use for this architecture.
             if 'DEFAULT', model is loaded with best available weights (note that these may change across versions).
             Pre-trained weights available for each architecture are listed at https://pytorch.org/vision/stable/models.html
         num_channels:
             specify channels in input sample, eg [channels h,w] sample shape
     """
-    architecture_ft = models.squeezenet1_0(weights=weights)
+    architecture_ft = torchvision.models.squeezenet1_0(weights=weights)
 
     # prevent weights of feature extractor from being trained, if desired
     if freeze_feature_extractor:
         freeze_params(architecture_ft)
 
     # change number of output nodes
     # uses a conv2d, not a fully connected layera
@@ -400,15 +397,15 @@
             string containing version name of the pre-trained classification weights to use for this architecture.
             if 'DEFAULT', model is loaded with best available weights (note that these may change across versions).
             Pre-trained weights available for each architecture are listed at https://pytorch.org/vision/stable/models.html
         num_channels:
             specify channels in input sample, eg [channels h,w] sample shape
 
     """
-    architecture_ft = models.densenet121(weights=weights)
+    architecture_ft = torchvision.models.densenet121(weights=weights)
     if freeze_feature_extractor:
         freeze_params(architecture_ft)
 
     # change number of output nodes
     architecture_ft.classifier = change_fc_output_size(
         architecture_ft.classifier, num_classes
     )
@@ -429,46 +426,46 @@
     num_classes, freeze_feature_extractor=False, weights="DEFAULT", num_channels=3
 ):
     """Wrapper for Inception v3 architecture
 
     Input: 229x229
 
     WARNING: expects (299,299) sized images and has auxiliary output. See
-    InceptionV3 class in `opensoundscape.torch.models.cnn` for use.
+    InceptionV3 class in `opensoundscape.ml.cnn` for use.
 
     Args:
         num_classes:
             number of output nodes for the final layer
         freeze_feature_extractor:
             if False (default), entire network will have gradients and can train
             if True, feature block is frozen and only final layer is trained
         weights:
             string containing version name of the pre-trained classification weights to use for this architecture.
             if 'DEFAULT', model is loaded with best available weights (note that these may change across versions).
             Pre-trained weights available for each architecture are listed at https://pytorch.org/vision/stable/models.html
         num_channels:
             specify channels in input sample, eg [channels h,w] sample shape
     """
-    architecture_ft = models.inception_v3(weights=weights)
+    architecture_ft = torchvision.models.inception_v3(weights=weights)
     if freeze_feature_extractor:
         freeze_params(architecture_ft)
     # Handle the auxilary net
     num_ftrs = architecture_ft.AuxLogits.fc.in_features
-    architecture_ft.AuxLogits.fc = nn.Linear(num_ftrs, num_classes)
+    architecture_ft.AuxLogits.fc = torch.nn.Linear(num_ftrs, num_classes)
     # Handle the primary net
     num_ftrs = architecture_ft.fc.in_features
-    architecture_ft.fc = nn.Linear(num_ftrs, num_classes)
+    architecture_ft.fc = torch.nn.Linear(num_ftrs, num_classes)
     if num_channels != 3:
         warnings.warn(
             "Retaining weights while reshaping Inception "
             "number of input channels is not implemented. First conv2d will "
             "have random weights."
         )
 
-        architecture_ft.Conv2d_1a_3x3 = BasicConv2d(
+        architecture_ft.Conv2d_1a_3x3 = torchvision.models.inception.BasicConv2d(
             num_channels, 32, kernel_size=3, stride=2
         )
 
     # default target layers for activation maps like GradCAM and guided backpropagation
     architecture_ft.cam_target_layers = [architecture_ft.Mixed_7c]
 
     return architecture_ft
@@ -738,8 +735,8 @@
     Args:
         fc: the fully connected layer of the model that should
             be modified
         num_classes:
             number of output nodes for the new fc
     """
     num_ftrs = fc.in_features
-    return nn.Linear(num_ftrs, num_classes)
+    return torch.nn.Linear(num_ftrs, num_classes)
```

### Comparing `opensoundscape-0.9.0/opensoundscape/ml/datasets.py` & `opensoundscape-0.9.1/opensoundscape/ml/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 
     Effects:
         self.invalid_samples will contain a set of paths that did not successfully
             produce a list of clips with start/end times, if split_files_into_clips=True
     """
 
     def __init__(self, samples, preprocessor, bypass_augmentations=False):
-
         ## Input Validation ##
 
         # validate type of samples: list, np array, or df
         assert type(samples) in (list, np.ndarray, pd.DataFrame,), (
             f"samples must be type list/np.ndarray of file paths, "
             f"or pd.DataFrame with index containing path (or multi-index of "
             f"path, start_time, end_time). Got {type(samples)}."
@@ -94,15 +93,14 @@
         # if True skips Actions with .is_augmentation=True
         self.bypass_augmentations = bypass_augmentations
 
     def __len__(self):
         return self.label_df.shape[0]
 
     def __getitem__(self, idx, break_on_key=None, break_on_type=None):
-
         sample = AudioSample.from_series(self.label_df.iloc[idx])
 
         # preprocessor.forward will raise PreprocessingError if something fails
         sample = self.preprocessor.forward(
             sample,
             bypass_augmentations=self.bypass_augmentations,
             break_on_key=break_on_key,
```

### Comparing `opensoundscape-0.9.0/opensoundscape/ml/loss.py` & `opensoundscape-0.9.1/opensoundscape/ml/loss.py`

 * *Files identical despite different names*

### Comparing `opensoundscape-0.9.0/opensoundscape/ml/safe_dataset.py` & `opensoundscape-0.9.1/opensoundscape/ml/safe_dataset.py`

 * *Files identical despite different names*

### Comparing `opensoundscape-0.9.0/opensoundscape/ml/sampling.py` & `opensoundscape-0.9.1/opensoundscape/ml/sampling.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """classes for strategically sampling within a DataLoader"""
 import random
 import numpy as np
-from torch.utils.data.sampler import Sampler
 import torch
 import torch.utils.data
 
 
-class ImbalancedDatasetSampler(Sampler):
+class ImbalancedDatasetSampler(torch.utils.data.sampler.Sampler):
     """Samples elements randomly from a given list of indices for imbalanced dataset
     Args:
         indices (list, optional): a list of indices
         num_samples (int, optional): number of samples to draw
         callback_get_label func: a callback-like function which takes two arguments:
             dataset and index
 
@@ -106,15 +105,15 @@
         else:
             yield temp_tuple[j]
 
         i += 1
         j += 1
 
 
-class ClassAwareSampler(Sampler):
+class ClassAwareSampler(torch.utils.data.sampler.Sampler):
     """In each batch of samples, pick a limited number of classes to include and
     give even representation to each class"""
 
     def __init__(self, labels, num_samples_cls=1):
         num_classes = len(np.unique(labels))
         self.class_iter = RandomCycleIter(range(num_classes))
         cls_data_list = [list() for _ in range(num_classes)]
```

### Comparing `opensoundscape-0.9.0/opensoundscape/ml/utils.py` & `opensoundscape-0.9.1/opensoundscape/ml/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 """Utilties for .ml"""
 import warnings
 import pandas as pd
 import numpy as np
 import torch
-from torch import nn
 import torch.nn.functional as F
-from torch.utils.data import DataLoader
-from torch.nn.functional import softmax
 
 
 from opensoundscape.ml.sampling import ClassAwareSampler
 
 
-class BaseModule(nn.Module):
+class BaseModule(torch.nn.Module):
     """
     Base class for a pytorch model pipeline class.
 
     All child classes should define load, save, etc
     """
 
     name = None
@@ -66,15 +63,15 @@
     # we need to convert one-hot labels to digit labels for the CAS
     # first class name -> 0, next class name -> 1, etc
     digit_labels = dataset.df.values.argmax(1)
 
     # create the class aware sampler object and DataLoader
     sampler = ClassAwareSampler(digit_labels, num_samples_cls=2)
 
-    loader = DataLoader(
+    loader = torch.utils.data.DataLoader(
         dataset,
         batch_size=batch_size,
         shuffle=False,  # don't shuffle bc CAS does its own sampling
         num_workers=num_workers,
         pin_memory=True,
         sampler=sampler,
     )
@@ -123,25 +120,25 @@
         values with activation layer applied
 
     """
     if activation_layer is None:  # scores [-inf,inf]
         pass
     elif activation_layer == "softmax":
         # "softmax" activation: preds across all classes sum to 1
-        x = softmax(x, dim=1)
+        x = F.softmax(x, dim=1)
     elif activation_layer == "sigmoid":
         # map [-inf,inf] to [0,1]
         x = torch.sigmoid(x)
     elif activation_layer == "softmax_and_logit":
         # softmax, then remap scores from [0,1] to [-inf,inf]
         try:
-            x = torch.logit(softmax(x, dim=1))
+            x = torch.logit(F.softmax(x, dim=1))
         except NotImplementedError:
             # use cpu because mps aten::logit is not implemented yet
             warnings.warn("falling back to CPU for logit operation")
             original_device = x.device
-            x = torch.logit(softmax(x, dim=1).cpu()).to(original_device)
+            x = torch.logit(F.softmax(x, dim=1).cpu()).to(original_device)
 
     else:
         raise ValueError(f"invalid option for activation_layer: {activation_layer}")
 
     return x
```

### Comparing `opensoundscape-0.9.0/opensoundscape/preprocess/actions.py` & `opensoundscape-0.9.1/opensoundscape/preprocess/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 See the preprocessor module and Preprocessing tutorial
 for details on how to use and create your own actions.
 """
 import random
 import warnings
 import numpy as np
-from torchvision import transforms
+import torchvision
 import torch
 import pandas as pd
 
 from opensoundscape.audio import Audio, mix
 from opensoundscape.preprocess import tensor_augment as tensaug
 from opensoundscape.preprocess.utils import PreprocessingError, get_args, get_reqd_args
 from opensoundscape.sample import AudioSample
@@ -191,15 +191,15 @@
     if len(audio.samples) == 0:
         raise ValueError("recieved zero-length audio")
 
     if sample.target_duration is not None:
         if audio.duration + tol <= sample.target_duration:
             # input audio is not as long as desired length
             if extend:  # extend clip sith silence
-                audio = audio.extend(sample.target_duration)
+                audio = audio.extend_to(sample.target_duration)
             else:
                 raise ValueError(
                     f"the length of the original file ({audio.duration} "
                     f"sec) was less than the length to extract "
                     f"({sample.target_duration} sec). To extend short "
                     f"clips, use extend=True"
                 )
@@ -318,17 +318,17 @@
         contrast=0.3
         saturation=0.3
         hue=0
 
     Returns:
         modified tensor
     """
-    transform = transforms.Compose(
+    transform = torchvision.transforms.Compose(
         [
-            transforms.ColorJitter(
+            torchvision.transforms.ColorJitter(
                 brightness=brightness, contrast=contrast, saturation=saturation, hue=hue
             )
         ]
     )
     return transform(tensor)
 
 
@@ -351,16 +351,20 @@
     value is ~0. If normalization is applied after RandomAffine on a PIL image,
     use an intermediate fill color such as (122,122,122).
     """
 
     channels = tensor.shape[-3]
     fill = [fill] * channels
 
-    transform = transforms.Compose(
-        [transforms.RandomAffine(degrees=degrees, translate=translate, fill=fill)]
+    transform = torchvision.transforms.Compose(
+        [
+            torchvision.transforms.RandomAffine(
+                degrees=degrees, translate=translate, fill=fill
+            )
+        ]
     )
     return transform(tensor)
 
 
 def image_to_tensor(img, greyscale=False):
     """Convert PIL image to RGB or greyscale Tensor (PIL.Image -> Tensor)
 
@@ -372,15 +376,15 @@
             If True, converts image to one channel.
     """
     if greyscale:
         img = img.convert("L")
     else:
         img = img.convert("RGB")
 
-    transform = transforms.Compose([transforms.ToTensor()])
+    transform = torchvision.transforms.Compose([torchvision.transforms.ToTensor()])
     return transform(img)
 
 
 def scale_tensor(tensor, input_mean=0.5, input_std=0.5):
     """linear scaling of tensor values using torch.transforms.Normalize
 
     (Tensor->Tensor)
@@ -394,15 +398,17 @@
         input_std: standard deviation of input sample pixels (average across dataset)
         (these are NOT the target mu and sd, but the original mu and sd of img
         for which the output will have mu=0, std=1)
 
     Returns:
         modified tensor
     """
-    transform = transforms.Compose([transforms.Normalize(input_mean, input_std)])
+    transform = torchvision.transforms.Compose(
+        [torchvision.transforms.Normalize(input_mean, input_std)]
+    )
     return transform(tensor)
 
 
 def time_mask(tensor, max_masks=3, max_width=0.2):
     """add random vertical bars over sample (Tensor -> Tensor)
 
     Args:
@@ -477,15 +483,14 @@
         update_labels (bool): if True, labels of sample are updated to include
             labels of overlayed sample
 
     See overlay() for other arguments and default values.
     """
 
     def __init__(self, is_augmentation=True, **kwargs):
-
         super(Overlay, self).__init__(
             overlay,
             is_augmentation=is_augmentation,
             **kwargs,
         )
 
         self.returns_labels = True
@@ -607,17 +612,15 @@
     ## OVERLAY ##
     # iteratively perform overlays until stopping condition
     # each time, there is an overlay_prob probability of another overlay
     # up to a max number of max_overlay_num overlays
     overlays_performed = 0
 
     while overlay_prob > np.random.uniform() and overlays_performed < max_overlay_num:
-
         try:
-
             # lets pick a sample based on rules
             if overlay_class is None:
                 # choose any file from the overlay_df
                 overlay_path = random.choice(overlay_df.index)
 
             elif overlay_class == "different":
                 # Select a random file containing none of the classes this file contains
```

### Comparing `opensoundscape-0.9.0/opensoundscape/preprocess/img_augment.py` & `opensoundscape-0.9.1/opensoundscape/preprocess/img_augment.py`

 * *Files identical despite different names*

### Comparing `opensoundscape-0.9.0/opensoundscape/preprocess/preprocessors.py` & `opensoundscape-0.9.1/opensoundscape/preprocess/preprocessors.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,16 @@
         assert not action_index in self.pipeline, (
             f"action_index must be unique, but {action_index} is already"
             "in the pipeline. Provide a different name for this action."
         )
 
         if after_key is None and before_key is None:
             # put this action at the end of the index
-            self.pipeline = self.pipeline.append(pd.Series({action_index: action}))
+            new_item = pd.Series({action_index: action})
+            self.pipeline = pd.concat([self.pipeline, new_item])
         elif before_key is not None:
             self._insert_action_before(before_key, action_index, action)
         elif after_key is not None:
             self._insert_action_after(after_key, action_index, action)
 
     def remove_action(self, action_index):
         """alias for self.drop(...,inplace=True), removes an action
@@ -189,23 +190,25 @@
 
         return sample
 
     def _insert_action_before(self, idx, name, value):
         """insert an item before a spcific index in a series"""
         i = list(self.pipeline.index).index(idx)
         part1 = self.pipeline[0:i]
+        new_item = pd.Series([value], index=[name])
         part2 = self.pipeline[i:]
-        self.pipeline = part1.append(pd.Series([value], index=[name])).append(part2)
+        self.pipeline = pd.concat([part1, new_item, part2])
 
     def _insert_action_after(self, idx, name, value):
         """insert an item after a spcific index in a series"""
         i = list(self.pipeline.index).index(idx)
         part1 = self.pipeline[0 : i + 1]
+        new_item = pd.Series([value], index=[name])
         part2 = self.pipeline[i + 1 :]
-        self.pipeline = part1.append(pd.Series([value], index=[name])).append(part2)
+        self.pipeline = pd.concat([part1, new_item, part2])
 
 
 class SpectrogramPreprocessor(BasePreprocessor):
     """Child of BasePreprocessor that creates specrogram Tensors w/augmentation
 
     loads audio, creates spectrogram, performs augmentations, creates tensor
```

### Comparing `opensoundscape-0.9.0/opensoundscape/preprocess/tensor_augment.py` & `opensoundscape-0.9.1/opensoundscape/preprocess/tensor_augment.py`

 * *Files identical despite different names*

### Comparing `opensoundscape-0.9.0/opensoundscape/preprocess/utils.py` & `opensoundscape-0.9.1/opensoundscape/preprocess/utils.py`

 * *Files identical despite different names*

### Comparing `opensoundscape-0.9.0/opensoundscape/ribbit.py` & `opensoundscape-0.9.1/opensoundscape/ribbit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Detect periodic vocalizations with RIBBIT
 
 This module provides functionality to search audio for periodically fluctuating vocalizations.
 """
 import os
 import warnings
 
-from scipy import signal
+import scipy
 import numpy as np
 
 from opensoundscape.utils import generate_clip_times_df
 
 
 def calculate_pulse_score(
     amplitude, amplitude_sample_rate, pulse_rate_range, plot=False, nfft=1024
@@ -31,15 +31,17 @@
     """
 
     # input validation
     if len(amplitude) < 1:  # what is the minimum signal length?
         raise ValueError("amplitude does not have length > 0")
 
     # calculate amplitude modulation spectral density
-    frequencies, psd = signal.welch(amplitude, fs=amplitude_sample_rate, nfft=nfft)
+    frequencies, psd = scipy.signal.welch(
+        amplitude, fs=amplitude_sample_rate, nfft=nfft
+    )
 
     # look for the highest peak of power spectral density within pulse_rate_range
     min_rate = pulse_rate_range[0]
     max_rate = pulse_rate_range[1]
     psd_bandpassed = [
         psd[i] for i in range(len(psd)) if min_rate < frequencies[i] < max_rate
     ]
```

### Comparing `opensoundscape-0.9.0/opensoundscape/sample.py` & `opensoundscape-0.9.1/opensoundscape/sample.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,15 +114,21 @@
             labels=labels_series,
             trace=None,
         )
 
     @property
     def end_time(self):
         "calculate sample end time as start_time + duration"
-        return self.start_time + self.duration
+        if self.duration is None:
+            return None
+        else:
+            if self.start_time is None:
+                return self.duration
+            else:
+                return self.start_time + self.duration
 
 
 def collate_samples(samples):
     """generate batched tensors of data and labels (in a dictionary)
 
     returns collated samples: a dictionary with keys "samples" and "labels"
```

### Comparing `opensoundscape-0.9.0/opensoundscape/signal_processing.py` & `opensoundscape-0.9.1/opensoundscape/signal_processing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Signal processing tools for feature extraction and more"""
 import numpy as np
 import pandas as pd
-from scipy import signal
+import scipy
 import pywt
 import matplotlib.pyplot as plt
-from pywt import central_frequency
-from scipy.signal import correlation_lags, correlate as scipy_correlate
-from scipy.fft import next_fast_len
+import pywt
 import torch
 
 from opensoundscape.utils import inrange
 
 
 def frequency2scale(frequency, wavelet, sample_rate):
     """determine appropriate wavelet scale for desired center frequency
@@ -25,15 +23,15 @@
 
     Note: this function is not exactly an inverse of pywt.scale2frequency(),
     because that function returns frequency in sample-units (cycles/sample)
     rather than frequency in Hz (cycles/second). In other words,
     freuquency_hz = pywt.scale2frequency(w,scale)*sr.
     """
     # get center frequency of this wavelet
-    center_freq = central_frequency(wavelet)
+    center_freq = pywt.central_frequency(wavelet)
 
     # calculate scale
     return center_freq * sample_rate / frequency
 
 
 def cwt_peaks(
     audio,
@@ -80,15 +78,15 @@
     x = x[0]  # only used one frequency, so it's the first of the returned list
 
     ## process the cwt signal ##
 
     # normalize, square, hilbert envelope, normalize
     x = x / np.max(x)
     x = x**2
-    x = abs(signal.hilbert(x))
+    x = abs(scipy.signal.hilbert(x))
     x = x / np.max(x)
 
     # calcualte time vector for each point in cwt signal
     t = np.linspace(0, audio.duration, len(x))
 
     ## find peaks in cwt signal ##
 
@@ -96,22 +94,21 @@
     min_d = (
         None
         if peak_separation is None
         else np.round(peak_separation * audio.sample_rate)
     )
 
     # locate peaks
-    peak_idx, _ = signal.find_peaks(x, height=peak_threshold, distance=min_d)
+    peak_idx, _ = scipy.signal.find_peaks(x, height=peak_threshold, distance=min_d)
     peak_times = [t[i] for i in peak_idx]
     peak_levels = [x[i] for i in peak_idx]
 
     ## plotting ##
 
     if plot:
-
         # plot cwt signal and detected peaks
         plt.plot(t, x)
         plt.scatter(peak_times, peak_levels, c="red")
         plt.show()
 
         # plot a graph of delta-t (forward dif) vs t for all peaks
         peak_delta_ts = [
@@ -225,15 +222,14 @@
             building_sequence = True
             current_sequence_y.append(yi)
             current_sequence_t.append(ti)
         else:
             # invalid point
 
             if building_sequence:
-
                 # check: should we break the sequence or continue?
                 if i - last_used_index > max_skip or not inrange(dt, dt_range):
                     # one of the two continuation criterea was broken.
                     # break sequence.
 
                     # check if current sequence meets sequence criterea
                     sequence_length_sec = current_sequence_t[-1] - current_sequence_t[0]
@@ -456,15 +452,15 @@
         x = x / np.max(x)
     x_01 = (np.array(x) >= threshold).astype(int)
     starts, lengths = _get_ones_sequences(x_01)
 
     return np.array(starts) / sample_rate, np.array(lengths) / sample_rate
 
 
-def gcc(x, y, cc_filter="phat", epsilon=0.001, radius=None):
+def gcc(x, y, cc_filter="phat", epsilon=0.001):
     """
     Generalized cross correlation of two signals
 
     Computes a generalized cross correlation in frequency response.
 
     The generalized cross correlation algorithm described in Knapp and Carter [1].
 
@@ -474,18 +470,19 @@
     code adapted from github.com/axeber01/ngcc
 
     Args:
         x: 1d numpy array of audio samples
         y: 1d numpy array of audio samples
         cc_filter: which filter to use in the gcc.
             'phat' - Phase transform. Default.
-            'roth' -
+            'roth' - Roth correlation (1971)
             'scot' - Smoothed Coherence Transform,
             'ht' - Hannan and Thomson
             'cc' - normal cross correlation with no filter
+            'cc_norm' - normal cross correlation normalized by the length and amplitude of the signal
         epsilon: small value used to ensure denominator when applying a filter is non-zero.
 
     Returns:
         gcc: 1d numpy array of gcc values
 
     see also: tdoa() uses this function to estimate time delay between two signals
 
@@ -493,23 +490,28 @@
     The Generalized Correlation Method for Estimation of Time Delay. IEEE Trans. Acoust. Speech Signal Process, 24, 320-327.
     http://dx.doi.org/10.1109/TASSP.1976.1162830
     """
     # using torch speeds up our performance
     x = torch.Tensor(x)
     y = torch.Tensor(y)
 
+    if cc_filter == "cc_norm":
+        # zero - center the signals
+        x = x - torch.mean(x)
+        y = y - torch.mean(y)
+
     # pad the fft shape for "full" cross correlation of both signals
     n = x.shape[0] + y.shape[0] - 1
     if n % 2 != 0:
         n += 1
     # by choosing an optimal length rather than the shortest possible, we can
     # optimize fft speed
-    n_fast = next_fast_len(n, real=True)
+    n_fast = scipy.fft.next_fast_len(n, real=True)
 
-    # Take the reall Fast Fourier Transform of the signals
+    # Take the real Fast Fourier Transform of the signals
     X = torch.fft.rfft(x, n=n_fast)
     Y = torch.fft.rfft(y, n=n_fast)
 
     # multiply one by the complex conjugate of the other
     Gxy = X * torch.conj(Y)
 
     # Apply the filter in the fourier domain
@@ -526,83 +528,108 @@
 
     elif cc_filter == "ht":
         Gxx = X * torch.conj(X)
         Gyy = Y * torch.conj(Y)
         gamma_xy = Gxy / (torch.sqrt(Gxx * Gyy) + epsilon)
         coherence = torch.abs(gamma_xy) ** 2
         phi = coherence / (torch.abs(Gxy) * (1 - coherence) + epsilon)
-    elif cc_filter == "cc":
+    elif cc_filter == "cc" or cc_filter == "cc_norm":
         phi = 1.0
+
     else:
         raise ValueError(
-            "Unsupported cc_filter. Must be one of: 'ht', 'phat', 'roth','scot'"
+            "Unsupported cc_filter. Must be one of: 'phat', 'roth', 'ht', 'scot', 'cc', 'cc_norm'"
         )
     # Inverse FFT to get the GCC
     cc = torch.fft.irfft(Gxy * phi, n_fast)
 
     # reorder the cross-correlation coefficients, trimming out padded regions
     # order of outputs matches torch.correlate and scipy.signal.correlate
     cc = torch.concatenate((cc[-y.shape[0] + 1 :], cc[: x.shape[0]]))
 
+    # normalize the cross-correlation coefficients if using cc_norm
+    # this normalizes both by length and amplitude
+    if cc_filter == "cc_norm":
+        cc = cc / (
+            torch.linalg.vector_norm(x) * torch.linalg.vector_norm(y)
+        )  # implicitly assumes mean of x and y are 0
+
     return cc.numpy()
 
 
 def tdoa(
     signal,
     reference_signal,
+    max_delay,
     cc_filter="phat",
     sample_rate=1,
     return_max=False,
-    max_delay=None,
 ):
-    """estimate time difference of arrival between two signals
+    """Estimate time difference of arrival between two signals
 
     estimates time delay by finding the maximum of the generalized cross correlation (gcc)
     of two signals. The two signals are discrete-time series with the same sample rate.
 
+    Only the central portion of the signal, from max_delay after the start and max_delay before the end, is used for the calculation.
+    All of the reference signal is used.
+
     For example, if the signal arrives 2.5 seconds _after_ the reference signal, returns 2.5;
     if it arrives 0.5 seconds _before_ the reference signal, returns -0.5.
 
     Args:
-        signal, reference_signal: np.arrays or lists containing each signal
+        signal: np.array or list object containing the signal of interest
+        reference_signal: np.array or list containing the reference signal. Both audio recordings must be time-synchronized.
+        max_delay: maximum possible tdoa (seconds) between the two signals. Cannot be longer than 1/2 the duration of the signal.
+        The tdoa returned will be between -max_delay and +max_delay.
         cc_filter: see gcc()
         sample_rate: sample rate (Hz) of signals; both signals must have same sample rate
         return_max: if True, returns the maximum value of the generalized cross correlation
-        max_delay: maximum possible tdoa. Cross-correlations that correspond to time delays outside of this range are ignored.
+
             For example, if max_delay=0.5, the tdoa returned will be the delay between -0.5 and +0.5 seconds, that maximizes the cross-correlation.
             This is useful if you know the maximum possible delay between the two signals, and want to ignore any tdoas outside of that range.
             e.g. if receivers are 100m apart, and the speed of sound is 340m/s, then the maximum possible delay is 0.294 seconds.
     Returns:
         estimated delay from reference signal to signal, in seconds
         (note that default samping rate is 1.0 samples/second)
 
         if return_max is True, returns a second value, the maximum value of the
         result of generalized cross correlation
 
     See also: gcc() if you want the raw output of generalized cross correlation
     """
+    # check that the two signals are the same length
+
+    if (
+        len(reference_signal) - len(signal) > 1
+    ):  # allow 1 sample difference for rounding errors
+        raise ValueError("reference_signal and signal must be the same length.")
+
+    # check that the maximum delay is not longer than 1/2 the audio signal
+    audio_len = len(signal) / sample_rate
+    if max_delay >= audio_len / 2:
+        raise ValueError(
+            f"max_delay cannot be longer than 1/2 the signal. max_delay is {max_delay} seconds, signal is {audio_len} seconds long."
+        )
+    # trim the primary signal to just the central part
+    start = int(max_delay * sample_rate)
+    end = int(len(reference_signal) - max_delay * sample_rate)
+    signal = signal[start:end]
+
     # compute the generalized cross correlation between the signals
     cc = gcc(signal, reference_signal, cc_filter=cc_filter)
 
-    # generate the relative offsets for each index position of `cc`
-    lags = correlation_lags(len(signal), len(reference_signal))
+    # filter to only the 'valid' part of the cross correlation, where the signals overlap fully
+    cc = cc[len(signal) - 1 : -len(signal) + 1]
 
-    if max_delay:
-        max_lag = int(
-            max_delay * sample_rate
-        )  # convert max_delay to max_lag in samples
-        # slice cc and lags, so we only look at cross_correlations that are between -max_lag and +max_lag
-        boolean_mask = [lag < max_lag and lag > -max_lag for lag in lags]
-        cc = cc[boolean_mask]
-        lags = lags[boolean_mask]
-
-    # find the time delay using the index of the maximum cc value
-    # the maximum of the cc value represents GCC's estimate of the delay
-    # between the two signals, ie how much to shift one signal against the other
-    # to maximize their product
-    tdoa = lags[np.argmax(cc)] / sample_rate
+    # find max cc value
+    # if max is at 0 it indicates the signal arrives max_delay earlier than in the reference signal
+    lag = np.argmax(cc)
+
+    # convert lag to time delay
+    tdoa = (lag / sample_rate) - max_delay
+    max_cc = np.max(cc)
 
     if return_max:
-        return tdoa, max(cc)
+        return tdoa, np.max(cc)
 
     else:
         return tdoa
```

### Comparing `opensoundscape-0.9.0/opensoundscape/spectrogram.py` & `opensoundscape-0.9.1/opensoundscape/spectrogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python3
 """ spectrogram.py: Utilities for dealing with spectrograms
 """
 import warnings
 import os
 
-from scipy import signal
+import scipy
 import numpy as np
 import librosa.filters
-from skimage.transform import resize as skresize
+import skimage
 from PIL import Image
 import torch
+import matplotlib
 from matplotlib import pyplot as plt
-from matplotlib.cm import get_cmap
 import matplotlib.colors
 
 from opensoundscape.audio import Audio
 from opensoundscape.utils import min_max_scale, linear_scale
 
 
 class Spectrogram:
@@ -193,15 +193,15 @@
         elif overlap_fraction is not None:
             assert (
                 overlap_fraction >= 0 and overlap_fraction < 1
             ), "overlap_fraction must be >=0 and <1"
             overlap_samples = int(window_samples * overlap_fraction)
         # else: use the provided overlap_samples argument
 
-        frequencies, times, spectrogram = signal.spectrogram(
+        frequencies, times, spectrogram = scipy.signal.spectrogram(
             x=audio.samples,
             fs=audio.sample_rate,
             window=window_type,
             nperseg=int(window_samples),
             noverlap=int(overlap_samples),
             nfft=fft_size,
             scaling=scaling,
@@ -608,22 +608,22 @@
 
         # invert if desired
         if invert:
             array = 1 - array
 
         # apply colormaps
         if colormap is not None:  # apply a colormap to get RGB channels
-            cm = get_cmap(colormap)
+            cm = matplotlib.cm.get_cmap(colormap)
             array = cm(array)
 
         # resize and change channel dims
         if shape is None:
             shape = np.shape(array)
         out_shape = [shape[0], shape[1], channels]
-        array = skresize(array, out_shape)
+        array = skimage.transform.resize(array, out_shape)
 
         if return_type == "pil":  # expected shape of input is [h,w,c]
             # use correct type for img, and scale from 0-1 to 0-255
             array = np.uint8(array * 255)
             if array.shape[-1] == 1:
                 # PIL doesnt like [x,y,1] shape, wants [x,y] instead
                 array = array[:, :, 0]
```

### Comparing `opensoundscape-0.9.0/opensoundscape/utils.py` & `opensoundscape-0.9.1/opensoundscape/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Utilities for opensoundscape"""
 
-from datetime import datetime
+import datetime
+import warnings
 
 import numpy as np
 import pandas as pd
 import pytz
 import soundfile
-
 import librosa
 
 
 class GetDurationError(ValueError):
     """raised if librosa.get_duration(path=f) causes an error"""
 
     pass
@@ -72,38 +72,14 @@
     returns rescaled feature set and rescaling vector"""
     if rescaling_vector is None:
         rescaling_vector = 1 / np.nanmax(X, 0)
     rescaled_x = np.multiply(X, rescaling_vector).tolist()
     return rescaled_x, rescaling_vector
 
 
-def hex_to_time(s):
-    """convert a hexidecimal, Unix time string to a datetime timestamp in utc
-
-    Example usage:
-    ```
-    # Get the UTC timestamp
-    t = hex_to_time('5F16A04E')
-
-    # Convert it to a desired timezone
-    my_timezone = pytz.timezone("US/Mountain")
-    t = t.astimezone(my_timezone)
-    ```
-
-    Args:
-        s (string): hexadecimal Unix epoch time string, e.g. '5F16A04E'
-
-    Returns:
-        datetime.datetime object representing the date and time in UTC
-    """
-    sec = int(s, 16)
-    timestamp = datetime.utcfromtimestamp(sec).replace(tzinfo=pytz.utc)
-    return timestamp
-
-
 def min_max_scale(array, feature_range=(0, 1)):
     """rescale vaues in an a array linearly to feature_range"""
     bottom, top = feature_range
     array_min = np.min(array)
     array_max = np.max(array)
     scale_factor = (top - bottom) / (array_max - array_min)
     return scale_factor * (array - array_min) + bottom
@@ -141,43 +117,14 @@
     elif distribution == "uniform":
         return np.array(x) + np.random.uniform(-1 * width, width, size=np.shape(x))
     raise ValueError(
         f"distribution must be 'gaussian' or 'uniform'. Got {distribution}."
     )
 
 
-def load_metadata(path, raise_exceptions=False):
-    """use soundfile to load metadata from WAV or AIFF file
-
-    Args:
-        path: file path to WAV of AIFF file
-        raise_exceptions: if True, raises exception,
-            if False returns None if exception occurs
-            [default: False]
-
-    Returns:
-        dictionary containing audio file metadata
-    """
-
-    try:
-        with soundfile.SoundFile(path, "r") as f:
-            metadata = f.copy_metadata()
-            metadata["samplerate"] = f.samplerate
-            metadata["format"] = f.format
-            metadata["frames"] = f.frames
-            metadata["sections"] = f.sections
-            metadata["subtype"] = f.subtype
-            return metadata
-    except:
-        if raise_exceptions:
-            raise
-        else:
-            return None
-
-
 def generate_clip_times_df(
     full_duration,
     clip_duration,
     clip_overlap=0,
     final_clip=None,
     rounding_precision=10,
 ):
@@ -318,18 +265,17 @@
     else:
         assert hasattr(files, "__iter__"), (
             f"`files` should be a dataframe with paths as "
             f"the index, or an iterable of file paths. Got {type(files)}."
         )
         file_list = files
 
-    assert len(files) > 0, "files list has length zero!"
-
     clip_dfs = []
     invalid_samples = set()
+    idx_cols = ["file", "start_time", "end_time"]
     for f in file_list:
         try:
             t = librosa.get_duration(path=f)
             clips = generate_clip_times_df(
                 full_duration=t,
                 clip_duration=clip_duration,
                 clip_overlap=clip_overlap,
@@ -349,13 +295,21 @@
 
         if label_df is not None:
             # copy labels for this file to all of its clips
             clips[label_df.columns] = label_df.loc[f]
 
         clip_dfs.append(clips)
 
-    clip_df = pd.concat(clip_dfs).set_index(["file", "start_time", "end_time"])
+    if len(clip_dfs) > 0:
+        clip_df = pd.concat(clip_dfs).set_index(idx_cols)
+    else:
+        # warnings.warn(
+        #     f"No clips were created from file_list of length {len(file_list)}"
+        # )
+        # create an empty dataframe with the expected index and columns
+        label_cols = [] if label_df is None else label_df.columns
+        clip_df = pd.DataFrame(columns=idx_cols + label_cols).set_index(idx_cols)
 
     if return_invalid_samples:
         return clip_df, invalid_samples
     else:
         return clip_df
```

### Comparing `opensoundscape-0.9.0/pyproject.toml` & `opensoundscape-0.9.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opensoundscape"
-version = "0.9.0"
+version = "0.9.1"
 description = "Open source, scalable acoustic classification for ecology and conservation"
 authors = [
   "Sam Lapp <sammlapp@gmail.com>",
   "Tessa Rhinehart <tessa.rhinehart@gmail.com>",
   "Louis Freeland-Haynes <>",
   "Jatin Khilnani <>",
   "Sasha Syunkova <>",
@@ -13,52 +13,52 @@
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/jkitzes/opensoundscape"
 packages = [{include = "opensoundscape"}]
 include = ["opensoundscape/**/*.py"]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.10"
+python = ">=3.8"
 docopt = ">=0.6.2"
 librosa = ">=0.10.0"
-ray = ">=0.8.5"
-torch = ">=2.0.0"
+torch = ">=2.0.0, !=2.0.1"
 torchvision = ">=0.15.1"
 ipykernel = ">=5.2.0"
 pandas = ">=1.3"
 matplotlib = ">=3.2.1"
 schema = ">=0.7.2"
 jupyterlab = ">=2.1.4"
 scikit-image = ">=0.17.2"
-numba = ">=0.48.0"
+numba = ">=0.57.0"
 scikit-learn = ">=0.24.2"
 Jinja2 = "<3.0"
 ipython = ">=7.10"
 pywavelets = ">=1.2.0"
 Deprecated = "^1.2.13"
 soundfile = ">=0.11"
 wandb = "^0.13.4"
 pillow = ">=9.3.0"
 jupyter-server = ">=1.17.0"
 protobuf = ">=4.21.6"
 joblib = ">=1.2.0"
 certifi = ">=2022.12.7"
 grad-cam = ">=1.4.6"
 sentry-sdk = ">=1.14.0"
+aru-metadata-parser = ">=0.1.0"
 
 [tool.poetry.dev-dependencies]
 black = "~=22.8"
 pre-commit = ">=1.18"
 sphinx = ">=2.1"
 pytest = ">=5.1"
 sphinx-rtd-theme = ">=0.4.3"
 recommonmark = ">=0.6.0"
 nbsphinx = ">=0.7.1"
 m2r = ">=0.2"
-docutils = "=0.17"
+docutils = ">=0.20"
 
 [tool.black]
 line-length = 88
 target_version = ['py37', 'py38']
 include = '\.pyi?$'
 exclude = '''
 /(
```

