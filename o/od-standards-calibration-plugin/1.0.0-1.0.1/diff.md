# Comparing `tmp/od_standards_calibration_plugin-1.0.0-py3-none-any.whl.zip` & `tmp/od_standards_calibration_plugin-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,11 @@
-Zip file size: 14703 bytes, number of entries: 12
+Zip file size: 8752 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      119 b- defN 23-Jun-20 18:50 od_standards_calibration_plugin/__init__.py
--rw-r--r--  2.0 unx    12926 b- defN 23-Apr-25 02:18 od_standards_calibration_plugin/led_calibration.py
--rw-r--r--  2.0 unx    18346 b- defN 23-Jun-20 18:44 od_standards_calibration_plugin/od_calibration_from_standards.py
--rw-r--r--  2.0 unx     6885 b- defN 23-Apr-25 02:18 od_standards_calibration_plugin/test_led_calibration.py
--rw-r--r--  2.0 unx     6885 b- defN 23-Jun-21 15:28 od_standards_calibration_plugin/test_od_standards_calibration.py
+-rw-r--r--  2.0 unx    18352 b- defN 23-Jun-22 18:49 od_standards_calibration_plugin/od_calibration_from_standards.py
 -rw-r--r--  2.0 unx      137 b- defN 23-Jun-20 18:56 od_standards_calibration_plugin/ui/contrib/jobs/od_standards_calibration_plugin.yaml
--rw-rw-r--  2.0 unx     1055 b- defN 23-Jun-21 16:30 od_standards_calibration_plugin-1.0.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1338 b- defN 23-Jun-21 16:30 od_standards_calibration_plugin-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 16:30 od_standards_calibration_plugin-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       87 b- defN 23-Jun-21 16:30 od_standards_calibration_plugin-1.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       32 b- defN 23-Jun-21 16:30 od_standards_calibration_plugin-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1331 b- defN 23-Jun-21 16:30 od_standards_calibration_plugin-1.0.0.dist-info/RECORD
-12 files, 49233 bytes uncompressed, 12355 bytes compressed:  74.9%
+-rw-rw-r--  2.0 unx     1055 b- defN 23-Jun-22 20:32 od_standards_calibration_plugin-1.0.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     1220 b- defN 23-Jun-22 20:32 od_standards_calibration_plugin-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 20:32 od_standards_calibration_plugin-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       87 b- defN 23-Jun-22 20:32 od_standards_calibration_plugin-1.0.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       32 b- defN 23-Jun-22 20:32 od_standards_calibration_plugin-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      990 b- defN 23-Jun-22 20:32 od_standards_calibration_plugin-1.0.1.dist-info/RECORD
+9 files, 22084 bytes uncompressed, 6970 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -1,37 +1,28 @@
 Filename: od_standards_calibration_plugin/__init__.py
 Comment: 
 
-Filename: od_standards_calibration_plugin/led_calibration.py
-Comment: 
-
 Filename: od_standards_calibration_plugin/od_calibration_from_standards.py
 Comment: 
 
-Filename: od_standards_calibration_plugin/test_led_calibration.py
-Comment: 
-
-Filename: od_standards_calibration_plugin/test_od_standards_calibration.py
-Comment: 
-
 Filename: od_standards_calibration_plugin/ui/contrib/jobs/od_standards_calibration_plugin.yaml
 Comment: 
 
-Filename: od_standards_calibration_plugin-1.0.0.dist-info/LICENSE.txt
+Filename: od_standards_calibration_plugin-1.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: od_standards_calibration_plugin-1.0.0.dist-info/METADATA
+Filename: od_standards_calibration_plugin-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: od_standards_calibration_plugin-1.0.0.dist-info/WHEEL
+Filename: od_standards_calibration_plugin-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: od_standards_calibration_plugin-1.0.0.dist-info/entry_points.txt
+Filename: od_standards_calibration_plugin-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: od_standards_calibration_plugin-1.0.0.dist-info/top_level.txt
+Filename: od_standards_calibration_plugin-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: od_standards_calibration_plugin-1.0.0.dist-info/RECORD
+Filename: od_standards_calibration_plugin-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## od_standards_calibration_plugin/od_calibration_from_standards.py

```diff
@@ -329,15 +329,15 @@
         maximum_od600=max(od600_values),
         minimum_od600=0,
         minimum_voltage=min(voltages),
         maximum_voltage=max(voltages),
         curve_data_=curve_data_,
         curve_type=curve_type,
         voltages=voltages,
-        od600_values=od600_values,
+        inferred_od600s=od600_values,
         ir_led_intensity=float(config["od_config"]["ir_led_intensity"]),
         pd_channel=signal_channel,
     )
 
     with local_persistant_storage("od_calibrations") as cache:
         cache[name] = encode(data_blob)
 
@@ -447,15 +447,15 @@
 
 
 def display(name: str | None) -> None:
     from pprint import pprint
 
     def display_from_calibration_blob(data_blob) -> None:
         voltages = data_blob["voltages"]
-        ods = data_blob["od600_values"]
+        ods = data_blob["inferred_od600s"]
         name, angle = data_blob["name"], data_blob["angle"]
         click.echo()
         click.echo(click.style(f"Calibration `{name}`", underline=True, bold=True))
         plot_data(
             ods,
             voltages,
             title=f"`{name}`, calibration of {angle}°",
```

## Comparing `od_standards_calibration_plugin-1.0.0.dist-info/LICENSE.txt` & `od_standards_calibration_plugin-1.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `od_standards_calibration_plugin-1.0.0.dist-info/METADATA` & `od_standards_calibration_plugin-1.0.1.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: od-standards-calibration-plugin
-Version: 1.0.0
+Version: 1.0.1
 Summary: Calibrate OD using a set of standards.
 Home-page: https://github.com/odcambc/od_standards_calibration_plugin
 Author: Chris Macdonald
 Author-email: christian.macdonald@ucsf.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -18,9 +18,8 @@
 
 Type into your command line:
 
 ```
 pio run od_calibration_from_standards
 ```
 
-To perform this calibration, insert your vial containing media into the Pioreactor and submerge your light probe. Follow the prompts on the command line. The plugin will increase the light intensity, and prompt you to record the readings from your light probe. A calibration line of best fit will be generated based on your light probe readings.
-
+To perform this calibration, prepare a set of standards in individual vials with known OD (at least 10 mL volume) and with stir bars. Run the above command and follow the prompts. A calibration based on fitting will be produced.
```

