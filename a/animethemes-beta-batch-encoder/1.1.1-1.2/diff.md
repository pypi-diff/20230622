# Comparing `tmp/animethemes-beta-batch-encoder-1.1.1.tar.gz` & `tmp/animethemes-beta-batch-encoder-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animethemes-beta-batch-encoder-1.1.1.tar", last modified: Tue Jun 20 06:40:47 2023, max compression
+gzip compressed data, was "animethemes-beta-batch-encoder-1.2.tar", last modified: Thu Jun 22 20:31:02 2023, max compression
```

## Comparing `animethemes-beta-batch-encoder-1.1.1.tar` & `animethemes-beta-batch-encoder-1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 06:40:47.398305 animethemes-beta-batch-encoder-1.1.1/
--rw-rw-rw-   0        0        0     1082 2023-06-16 19:11:39.000000 animethemes-beta-batch-encoder-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     4720 2023-06-20 06:40:47.398305 animethemes-beta-batch-encoder-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3810 2023-06-18 16:30:02.000000 animethemes-beta-batch-encoder-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 06:40:47.375304 animethemes-beta-batch-encoder-1.1.1/animethemes_beta_batch_encoder.egg-info/
--rw-rw-rw-   0        0        0     4720 2023-06-20 06:40:46.000000 animethemes-beta-batch-encoder-1.1.1/animethemes_beta_batch_encoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      703 2023-06-20 06:40:46.000000 animethemes-beta-batch-encoder-1.1.1/animethemes_beta_batch_encoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 06:40:46.000000 animethemes-beta-batch-encoder-1.1.1/animethemes_beta_batch_encoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-20 06:40:46.000000 animethemes-beta-batch-encoder-1.1.1/animethemes_beta_batch_encoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-20 06:40:46.000000 animethemes-beta-batch-encoder-1.1.1/animethemes_beta_batch_encoder.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 06:40:47.396306 animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/
--rw-rw-rw-   0        0        0        0 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/__init__.py
--rw-rw-rw-   0        0        0     7406 2023-06-18 16:30:18.000000 animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/__main__.py
--rw-rw-rw-   0        0        0     1280 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_bitrate_mode.py
--rw-rw-rw-   0        0        0     2615 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_colorspace.py
--rw-rw-rw-   0        0        0    13495 2023-06-16 19:01:34.000000 animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_encode_webm.py
--rw-rw-rw-   0        0        0     3814 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_encoding_config.py
--rw-rw-rw-   0        0        0     5145 2023-06-18 16:06:11.000000 animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_interface.py
--rw-rw-rw-   0        0        0     2527 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_loudnorm_filter.py
--rw-rw-rw-   0        0        0      779 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_seek.py
--rw-rw-rw-   0        0        0     6874 2023-06-18 15:20:40.000000 animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_seek_collector.py
--rw-rw-rw-   0        0        0     6594 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_source_file.py
--rw-rw-rw-   0        0        0     1375 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_utils.py
--rw-rw-rw-   0        0        0       42 2023-06-20 06:40:47.398305 animethemes-beta-batch-encoder-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1221 2023-06-20 06:39:48.000000 animethemes-beta-batch-encoder-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 20:31:02.647549 animethemes-beta-batch-encoder-1.2/
+-rw-rw-rw-   0        0        0     1082 2023-06-16 19:11:39.000000 animethemes-beta-batch-encoder-1.2/LICENSE
+-rw-rw-rw-   0        0        0     5014 2023-06-22 20:31:02.646547 animethemes-beta-batch-encoder-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4106 2023-06-22 20:14:45.000000 animethemes-beta-batch-encoder-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 20:31:02.631548 animethemes-beta-batch-encoder-1.2/animethemes_beta_batch_encoder.egg-info/
+-rw-rw-rw-   0        0        0     5014 2023-06-22 20:31:02.000000 animethemes-beta-batch-encoder-1.2/animethemes_beta_batch_encoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2023-06-22 20:31:02.000000 animethemes-beta-batch-encoder-1.2/animethemes_beta_batch_encoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 20:31:02.000000 animethemes-beta-batch-encoder-1.2/animethemes_beta_batch_encoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-22 20:31:02.000000 animethemes-beta-batch-encoder-1.2/animethemes_beta_batch_encoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-22 20:31:02.000000 animethemes-beta-batch-encoder-1.2/animethemes_beta_batch_encoder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 20:31:02.645547 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/
+-rw-rw-rw-   0        0        0        0 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/__init__.py
+-rw-rw-rw-   0        0        0     7944 2023-06-22 19:10:50.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/__main__.py
+-rw-rw-rw-   0        0        0     1280 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_bitrate_mode.py
+-rw-rw-rw-   0        0        0     2615 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_colorspace.py
+-rw-rw-rw-   0        0        0    13543 2023-06-22 18:39:34.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_encode_webm.py
+-rw-rw-rw-   0        0        0     4115 2023-06-22 08:05:47.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_encoding_config.py
+-rw-rw-rw-   0        0        0     6848 2023-06-22 20:08:15.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_interface.py
+-rw-rw-rw-   0        0        0     2527 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_loudnorm_filter.py
+-rw-rw-rw-   0        0        0      779 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_seek.py
+-rw-rw-rw-   0        0        0     6874 2023-06-22 19:02:20.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_seek_collector.py
+-rw-rw-rw-   0        0        0     6594 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_source_file.py
+-rw-rw-rw-   0        0        0     1375 2023-06-09 04:17:22.000000 animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_utils.py
+-rw-rw-rw-   0        0        0       42 2023-06-22 20:31:02.647549 animethemes-beta-batch-encoder-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-06-22 20:09:55.000000 animethemes-beta-batch-encoder-1.2/setup.py
```

### Comparing `animethemes-beta-batch-encoder-1.1.1/LICENSE` & `animethemes-beta-batch-encoder-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.1.1/PKG-INFO` & `animethemes-beta-batch-encoder-1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animethemes-beta-batch-encoder
-Version: 1.1.1
+Version: 1.2
 Summary: Generate/Execute FFmpeg commands for files in acting directory
 Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
 Author: AnimeThemes
 Author-email: admin@animethemes.moe
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -37,15 +37,15 @@
 
 **Install:**
 
     pip install animethemes-beta-batch-encoder
 
 ### Usage
 
-        python -m beta_batch_encoder [-h] [--generate | -g] [--execute | -e] [--file [FILE]] [--configfile [CONFIGFILE]] --loglevel [{debug,info,error}]
+        python -m beta_batch_encoder [-h] [--generate | -g] [--execute | -e] [--custom | -c] [--file [FILE]] [--configfile [CONFIGFILE]] --loglevel [{debug,info,error}]
 
 **Mode**
 
 `--generate` generates commands from input files in the current directory.
 
 The user will be prompted for values that are not determined programmatically, such as inclusion/exclusion of a source file candidate, start time, end time, output file name and new audio filters.
 
@@ -53,14 +53,18 @@
 
 By default, the program looks for a file named `commands.txt` in the current directory. This file name can be specified by the `--file` argument.
 
 `--generate` and `--execute` generates commands from input files in the current directory and executes the commands sequentially.
 
 `None` will give modes options to run.
 
+**Custom**
+
+`--custom` customizes options like Create Preview, Limit Size Enable, CRFs and Encoding Modes for each output file. Default configs are specified in the `--file` argument.
+
 **File**
 
 The file that commands are written to or read from.
 
 By default, the program will write to or read from `commands.txt` in the current directory.
 
 **Config File**
@@ -95,14 +99,16 @@
 
 `Threads` is the number of threads used to encode. Default is 4.
 
 `LimitSizeEnable` is a flag for including the `-fs` argument to terminate an encode when it exceeds the allowed size. Default is True.
 
 `AlternateSourceEnable` is a flag for alternate command lines between source files. Default is False.
 
+`CreatePreview` is a flag for create a command line to preview seeks. Default is False.
+
 `IncludeUnfiltered` is a flag for including or excluding an encode without video filters for each bitrate control mode and CRF pairing. Default is True.
 
 `VideoFilters` is a configuration item list used for named video filtergraphs for each bitrate control mode and CRF pairing.
 
 **Logging**
 
 Determines the level of the logging for the program.
```

### Comparing `animethemes-beta-batch-encoder-1.1.1/README.md` & `animethemes-beta-batch-encoder-1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 **Install:**
 
     pip install animethemes-beta-batch-encoder
 
 ### Usage
 
-        python -m beta_batch_encoder [-h] [--generate | -g] [--execute | -e] [--file [FILE]] [--configfile [CONFIGFILE]] --loglevel [{debug,info,error}]
+        python -m beta_batch_encoder [-h] [--generate | -g] [--execute | -e] [--custom | -c] [--file [FILE]] [--configfile [CONFIGFILE]] --loglevel [{debug,info,error}]
 
 **Mode**
 
 `--generate` generates commands from input files in the current directory.
 
 The user will be prompted for values that are not determined programmatically, such as inclusion/exclusion of a source file candidate, start time, end time, output file name and new audio filters.
 
@@ -31,14 +31,18 @@
 
 By default, the program looks for a file named `commands.txt` in the current directory. This file name can be specified by the `--file` argument.
 
 `--generate` and `--execute` generates commands from input files in the current directory and executes the commands sequentially.
 
 `None` will give modes options to run.
 
+**Custom**
+
+`--custom` customizes options like Create Preview, Limit Size Enable, CRFs and Encoding Modes for each output file. Default configs are specified in the `--file` argument.
+
 **File**
 
 The file that commands are written to or read from.
 
 By default, the program will write to or read from `commands.txt` in the current directory.
 
 **Config File**
@@ -73,14 +77,16 @@
 
 `Threads` is the number of threads used to encode. Default is 4.
 
 `LimitSizeEnable` is a flag for including the `-fs` argument to terminate an encode when it exceeds the allowed size. Default is True.
 
 `AlternateSourceEnable` is a flag for alternate command lines between source files. Default is False.
 
+`CreatePreview` is a flag for create a command line to preview seeks. Default is False.
+
 `IncludeUnfiltered` is a flag for including or excluding an encode without video filters for each bitrate control mode and CRF pairing. Default is True.
 
 `VideoFilters` is a configuration item list used for named video filtergraphs for each bitrate control mode and CRF pairing.
 
 **Logging**
 
 Determines the level of the logging for the program.
```

### Comparing `animethemes-beta-batch-encoder-1.1.1/animethemes_beta_batch_encoder.egg-info/PKG-INFO` & `animethemes-beta-batch-encoder-1.2/animethemes_beta_batch_encoder.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animethemes-beta-batch-encoder
-Version: 1.1.1
+Version: 1.2
 Summary: Generate/Execute FFmpeg commands for files in acting directory
 Home-page: https://github.com/AnimeThemes/animethemes-batch-encoder
 Author: AnimeThemes
 Author-email: admin@animethemes.moe
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -37,15 +37,15 @@
 
 **Install:**
 
     pip install animethemes-beta-batch-encoder
 
 ### Usage
 
-        python -m beta_batch_encoder [-h] [--generate | -g] [--execute | -e] [--file [FILE]] [--configfile [CONFIGFILE]] --loglevel [{debug,info,error}]
+        python -m beta_batch_encoder [-h] [--generate | -g] [--execute | -e] [--custom | -c] [--file [FILE]] [--configfile [CONFIGFILE]] --loglevel [{debug,info,error}]
 
 **Mode**
 
 `--generate` generates commands from input files in the current directory.
 
 The user will be prompted for values that are not determined programmatically, such as inclusion/exclusion of a source file candidate, start time, end time, output file name and new audio filters.
 
@@ -53,14 +53,18 @@
 
 By default, the program looks for a file named `commands.txt` in the current directory. This file name can be specified by the `--file` argument.
 
 `--generate` and `--execute` generates commands from input files in the current directory and executes the commands sequentially.
 
 `None` will give modes options to run.
 
+**Custom**
+
+`--custom` customizes options like Create Preview, Limit Size Enable, CRFs and Encoding Modes for each output file. Default configs are specified in the `--file` argument.
+
 **File**
 
 The file that commands are written to or read from.
 
 By default, the program will write to or read from `commands.txt` in the current directory.
 
 **Config File**
@@ -95,14 +99,16 @@
 
 `Threads` is the number of threads used to encode. Default is 4.
 
 `LimitSizeEnable` is a flag for including the `-fs` argument to terminate an encode when it exceeds the allowed size. Default is True.
 
 `AlternateSourceEnable` is a flag for alternate command lines between source files. Default is False.
 
+`CreatePreview` is a flag for create a command line to preview seeks. Default is False.
+
 `IncludeUnfiltered` is a flag for including or excluding an encode without video filters for each bitrate control mode and CRF pairing. Default is True.
 
 `VideoFilters` is a configuration item list used for named video filtergraphs for each bitrate control mode and CRF pairing.
 
 **Logging**
 
 Determines the level of the logging for the program.
```

### Comparing `animethemes-beta-batch-encoder-1.1.1/animethemes_beta_batch_encoder.egg-info/SOURCES.txt` & `animethemes-beta-batch-encoder-1.2/animethemes_beta_batch_encoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/__main__.py` & `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 from ._source_file import SourceFile
 from ._utils import commandfile_arg_type
 from ._utils import configfile_arg_type
 from appdirs import AppDirs
 
 import argparse
 import configparser
+import copy
 import logging
 import os
 import shutil
 import subprocess
 import sys
 
 
 def main():
     # Load/Validate Arguments
     parser = argparse.ArgumentParser(prog='beta_batch_encoder',
                                      description='Generate/Execute FFmpeg commands for files in acting directory',
                                      formatter_class=argparse.RawTextHelpFormatter)
-    parser.add_argument('--generate', '-g', action='store_true',help='Generate commands and write to file')
+    parser.add_argument('--generate', '-g', action='store_true', help='Generate commands and write to file')
     parser.add_argument('--execute', '-e', action='store_true', help='Execute commands from file')
+    parser.add_argument('--custom', '-c', action='store_true', help='Customize some options for each seek')
     parser.add_argument('--file', nargs='?', default='commands.txt', type=commandfile_arg_type,
                         help='1: Name of file commands are written to (default: commands.txt)\n'
                              '2: Name of file commands are executed from (default: commands.txt)\n'
                              '3: Name of file commands are written to (default: commands.txt)')
     parser.add_argument('--configfile', nargs='?', default='beta_batch_encoder.ini', type=configfile_arg_type,
                         help='Name of config file (default: beta_batch_encoder.ini)\n'
                              'If the file does not exist, default configuration will be written\n'
@@ -55,14 +57,15 @@
     if not os.path.exists(config_file):
         config['Encoding'] = {EncodingConfig.config_allowed_filetypes: EncodingConfig.default_allowed_filetypes,
                               EncodingConfig.config_encoding_modes: EncodingConfig.default_encoding_modes,
                               EncodingConfig.config_crfs: EncodingConfig.default_crfs,
                               EncodingConfig.config_threads: EncodingConfig.default_threads,
                               EncodingConfig.config_limit_size_enable: EncodingConfig.default_limit_size_enable,
                               EncodingConfig.config_alternate_source_files: EncodingConfig.default_alternate_source_files,
+                              EncodingConfig.create_preview: EncodingConfig.default_create_preview,
                               EncodingConfig.config_include_unfiltered: EncodingConfig.default_include_unfiltered,
                               EncodingConfig.config_default_video_stream: '',
                               EncodingConfig.config_default_audio_stream: ''}
         config['VideoFilters'] = EncodingConfig.default_video_filters
 
         os.makedirs(os.path.dirname(config_file), exist_ok=True)
         with open(config_file, 'w', encoding='utf8') as f:
@@ -104,18 +107,24 @@
                 seek_collector = None
                 while not is_collector_valid:
                     print(f'\033[92mSource File: {file}\033[0m')
                     seek_collector = SeekCollector(file_value)
                     is_collector_valid = seek_collector.is_valid()
 
                 for seek in seek_collector.get_seek_list():
+                    new_encoding_config = copy.copy(encoding_config)
+                    if args.custom:
+                        print(f'\033[92mOutput Name: {seek.output_name}\033[0m')
+                        new_encoding_config = Interface.custom_options(new_encoding_config)
+                        
                     logging.info(f'Generating commands with seek ss: \'{seek.ss}\', to: \'{seek.to}\'')
                     encode_webm = EncodeWebM(file_value, seek)
-                    load_commands = encode_webm.get_commands(encoding_config)
+                    load_commands = encode_webm.get_commands(new_encoding_config)
                     commands = commands + load_commands
+
             except KeyboardInterrupt:
                 logging.info(f'Exiting from inclusion of file \'{file}\' after keyboard interrupt')
         
         # Alternate lines per source files
         if encoding_config.alternate_source_files == True:
             output_list = []
             lines_per_source = len(load_commands)
```

### Comparing `animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_bitrate_mode.py` & `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_bitrate_mode.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_colorspace.py` & `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_colorspace.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_encode_webm.py` & `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_encode_webm.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,16 @@
 
         logging.debug(
             f'[EncodeWebm.get_commands] encoding_modes: \'{encoding_config.encoding_modes}\', '
             f'crfs: \'{encoding_config.crfs}\', '
             f'include_unfiltered: \'{encoding_config.include_unfiltered}\', '
             f'video_filters: \'{encoding_config.video_filters}\'')
         
-        file_commands.append(self.preview_seek(webm_filename=self.get_webm_filename()))
+        if encoding_config.create_preview:
+            file_commands.append(self.preview_seek(webm_filename=self.get_webm_filename()))
 
         for encoding_mode in encoding_config.encoding_modes:
             if BitrateMode.CBR.name == encoding_mode.upper():
                 file_commands.append(self.get_first_pass(BitrateMode.CBR, threads=encoding_config.threads))
                 if encoding_config.include_unfiltered:
                     file_commands.append(self.get_second_pass(BitrateMode.CBR,
                                                               threads=encoding_config.threads,
```

### Comparing `animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_encoding_config.py` & `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_encoding_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,41 +5,44 @@
     # Config keys
     config_allowed_filetypes = 'AllowedFileTypes'
     config_encoding_modes = 'EncodingModes'
     config_crfs = 'CRFs'
     config_threads = 'Threads'
     config_limit_size_enable = 'LimitSizeEnable'
     config_alternate_source_files = 'AlternateSourceFiles'
+    config_create_preview = 'CreatePreview'
     config_include_unfiltered = 'IncludeUnfiltered'
 
     # Default Config keys
     config_default_video_stream = 'DefaultVideoStream'
     config_default_audio_stream = 'DefaultAudioStream'
 
     # Default config values
     default_allowed_filetypes = '.avi,.m2ts,.mkv,.mp4,.wmv'
     default_encoding_modes = f'{BitrateMode.VBR.name},{BitrateMode.CBR.name}'
     default_crfs = '12,15,18,21,24'
     default_threads = '4'
     default_limit_size_enable = True
     default_alternate_source_files = False
+    default_create_preview = False
     default_include_unfiltered = True
     default_video_filters = {'filtered': 'hqdn3d=0:0:3:3,gradfun,unsharp',
                              'lightdenoise': 'hqdn3d=0:0:3:3',
                              'heavydenoise': 'hqdn3d=1.5:1.5:6:6',
                              'unsharp': 'unsharp'}
 
-    def __init__(self, allowed_filetypes, encoding_modes, crfs, threads, limit_size_enable, alternate_source_files, include_unfiltered, video_filters, default_video_stream,
+    def __init__(self, allowed_filetypes, encoding_modes, crfs, threads, limit_size_enable, alternate_source_files, create_preview, include_unfiltered, video_filters, default_video_stream,
                  default_audio_stream):
         self.allowed_filetypes = allowed_filetypes
         self.encoding_modes = encoding_modes
         self.crfs = crfs
         self.threads = threads
         self.limit_size_enable = limit_size_enable
         self.alternate_source_files = alternate_source_files
+        self.create_preview = create_preview
         self.include_unfiltered = include_unfiltered
         self.video_filters = video_filters
         self.default_video_stream = default_video_stream
         self.default_audio_stream = default_audio_stream
 
     @classmethod
     def from_config(cls, config):
@@ -48,22 +51,23 @@
         encoding_modes = config['Encoding'].get(EncodingConfig.config_encoding_modes,
                                                 EncodingConfig.default_encoding_modes).split(',')
         crfs = config['Encoding'].get(EncodingConfig.config_crfs, EncodingConfig.default_crfs).split(',')
         threads = config['Encoding'].get(EncodingConfig.config_threads,
                                          EncodingConfig.default_threads)
         limit_size_enable = config.getboolean('Encoding', EncodingConfig.config_limit_size_enable, fallback=EncodingConfig.default_limit_size_enable)
         alternate_source_files = config.getboolean('Encoding', EncodingConfig.config_alternate_source_files, fallback=EncodingConfig.default_alternate_source_files)
+        create_preview = config.getboolean('Encoding', EncodingConfig.config_create_preview, fallback=EncodingConfig.default_create_preview)
         include_unfiltered = config.getboolean('Encoding', EncodingConfig.config_include_unfiltered,
                                                fallback=EncodingConfig.default_include_unfiltered)
         video_filters = config.items('VideoFilters', EncodingConfig.default_video_filters)
 
         default_video_stream = config['Encoding'].get(EncodingConfig.config_default_video_stream)
         default_audio_stream = config['Encoding'].get(EncodingConfig.config_default_audio_stream)
 
-        return cls(allowed_filetypes, encoding_modes, crfs, threads, limit_size_enable, alternate_source_files, include_unfiltered, video_filters, default_video_stream,
+        return cls(allowed_filetypes, encoding_modes, crfs, threads, limit_size_enable, alternate_source_files, create_preview, include_unfiltered, video_filters, default_video_stream,
                    default_audio_stream)
 
     def get_default_stream(self, stream_type):
         if stream_type == 'video':
             return self.default_video_stream
         elif stream_type == 'audio':
             return self.default_audio_stream
```

### Comparing `animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_interface.py` & `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_interface.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,30 +4,25 @@
 
 class Interface:
     # Time Duration Specification: https://ffmpeg.org/ffmpeg-utils.html#time-duration-syntax
     time_pattern = re.compile('^([0-5]?\d:){1,2}[0-5]?\d(?=\.\d+$|$)|\d+(?=\.\d+$|$)')
 
     # Prompt the mode options to run to the user
     def choose_mode():
-        modes = {
-            'Generate commands': 1,
-            'Execute commands': 2,
-            'Generate and execute commands': 3
-        }
-
-        question = [inquirer.List('mode', message='Mode (Enter)', choices=list(modes.keys()))]
+        modes = [('Generate commands', 1), ('Execute commands', 2), ('Generate and execute commands', 3)]
+        question = [inquirer.List('mode', message='Mode (Enter)', choices=modes)]
         answer = inquirer.prompt(question)
 
         logging.debug(f'[Interface.choose_mode] answer["mode"]: \'{answer["mode"]}\'')
 
-        return modes[answer['mode']]
+        return answer['mode']
     
     # Prompt the source files to choose
     def choose_source_files(source_files):
-        question = [inquirer.Checkbox('source_files', message='Source Files (Space)', choices=source_files)]
+        question = [inquirer.Checkbox('source_files', message='Source Files (Space to select)', choices=source_files)]
         answer = inquirer.prompt(question)
 
         logging.debug(f'[Interface.choose_source_files] answer["source_files"]: \'{answer["source_files"]}\'')
 
         return answer['source_files']
     
     # Prompt the audio filters options
@@ -109,8 +104,42 @@
             f'audio_filters["Fade Out"]["Start Time"]: \'{audio_filters["Fade Out"]["Start Time"]}\', '
             f'audio_filters["Fade Out"]["Exp"]: \'{audio_filters["Fade Out"]["Exp"]}\', '
             f'audio_filters["Mute"]["Start Time"]: \'{audio_filters["Mute"]["Start Time"]}\', '
             f'audio_filters["Mute"]["End Time"]: \'{audio_filters["Mute"]["End Time"]}\', '
             f'audio_filters["Custom"]: \'{audio_filters["Custom"]}\''
         )
 
-        return ','.join(audio_filters_list)
+        return ','.join(audio_filters_list)
+
+    # Prompt custom options if requested
+    def custom_options(encoding_config):
+        create_preview = encoding_config.create_preview
+        limit_size_enable = encoding_config.limit_size_enable
+        crfs = encoding_config.crfs
+        encoding_modes = encoding_config.encoding_modes
+
+        validate_crfs = lambda _, x: all(y.strip().isdigit() for y in x.split(','))
+        validate_encoding_modes = lambda _, x: all(y.strip().upper() in ['VBR', 'CBR', 'CQ'] for y in x.split(','))
+
+        questions = [
+            inquirer.Confirm('create_preview', message=f'Create Preview?', default=create_preview),
+            inquirer.Confirm('limit_size_enable', message=f'Limit Size Enable?', default=limit_size_enable),
+            inquirer.Text('crfs', message='CRFs', default=','.join(crfs), validate=validate_crfs),
+            inquirer.Text('encoding_modes', message='Encoding Modes', default=','.join(encoding_modes), validate=validate_encoding_modes)
+        ]
+
+        answer = inquirer.prompt(questions)
+
+        encoding_config.create_preview = answer['create_preview']
+        encoding_config.limit_size_enable = answer['limit_size_enable']
+        encoding_config.crfs = answer['crfs'].split(',')
+        encoding_config.encoding_modes = answer['encoding_modes'].split(',')
+
+        logging.debug(
+            f'[Interface.custom_options] '
+            f'encoding_config.create_preview: \'{encoding_config.create_preview}\', '
+            f'encoding_config.limit_size_enable: \'{encoding_config.create_preview}\', '
+            f'encoding_config.crfs: \'{encoding_config.crfs}\', '
+            f'encoding_config.encoding_modes: \'{encoding_config.encoding_modes}\''
+        )
+
+        return encoding_config
```

### Comparing `animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_loudnorm_filter.py` & `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_loudnorm_filter.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_seek.py` & `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_seek.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_seek_collector.py` & `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_seek_collector.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_source_file.py` & `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_source_file.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.1.1/beta_batch_encoder/_utils.py` & `animethemes-beta-batch-encoder-1.2/beta_batch_encoder/_utils.py`

 * *Files identical despite different names*

### Comparing `animethemes-beta-batch-encoder-1.1.1/setup.py` & `animethemes-beta-batch-encoder-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='animethemes-beta-batch-encoder',
-    version='1.1.1',
+    version='1.2',
     author='AnimeThemes',
     author_email='admin@animethemes.moe',
     url='https://github.com/AnimeThemes/animethemes-batch-encoder',
     description='Generate/Execute FFmpeg commands for files in acting directory',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

