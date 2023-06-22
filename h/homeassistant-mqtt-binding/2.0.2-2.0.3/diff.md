# Comparing `tmp/homeassistant_mqtt_binding-2.0.2.tar.gz` & `tmp/homeassistant_mqtt_binding-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeassistant_mqtt_binding-2.0.2.tar", max compression
+gzip compressed data, was "homeassistant_mqtt_binding-2.0.3.tar", max compression
```

## Comparing `homeassistant_mqtt_binding-2.0.2.tar` & `homeassistant_mqtt_binding-2.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1065 2023-01-27 16:20:17.191127 homeassistant_mqtt_binding-2.0.2/LICENSE
--rw-r--r--   0        0        0     2276 2023-01-27 16:20:17.191127 homeassistant_mqtt_binding-2.0.2/README.md
--rw-r--r--   0        0        0        0 2023-01-27 16:20:17.191127 homeassistant_mqtt_binding-2.0.2/ha_mqtt/__init__.py
--rw-r--r--   0        0        0     2487 2023-01-27 16:20:17.191127 homeassistant_mqtt_binding-2.0.2/ha_mqtt/ha_device.py
--rw-r--r--   0        0        0     8774 2023-01-27 16:20:17.192127 homeassistant_mqtt_binding-2.0.2/ha_mqtt/mqtt_device_base.py
--rw-r--r--   0        0        0     1340 2023-01-27 16:20:17.192127 homeassistant_mqtt_binding-2.0.2/ha_mqtt/mqtt_sensor.py
--rw-r--r--   0        0        0     1110 2023-01-27 16:20:17.192127 homeassistant_mqtt_binding-2.0.2/ha_mqtt/mqtt_siren.py
--rw-r--r--   0        0        0     3279 2023-01-27 16:20:17.192127 homeassistant_mqtt_binding-2.0.2/ha_mqtt/mqtt_switch.py
--rw-r--r--   0        0        0      593 2023-01-27 16:20:17.192127 homeassistant_mqtt_binding-2.0.2/ha_mqtt/mqtt_thermometer.py
--rw-r--r--   0        0        0     3272 2023-01-27 16:20:17.192127 homeassistant_mqtt_binding-2.0.2/ha_mqtt/util.py
--rw-r--r--   0        0        0     1117 2023-01-27 16:20:17.192127 homeassistant_mqtt_binding-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     3049 1970-01-01 00:00:00.000000 homeassistant_mqtt_binding-2.0.2/setup.py
--rw-r--r--   0        0        0     3244 1970-01-01 00:00:00.000000 homeassistant_mqtt_binding-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-22 18:10:25.706954 homeassistant_mqtt_binding-2.0.3/LICENSE
+-rw-r--r--   0        0        0     2404 2023-06-22 18:10:25.706954 homeassistant_mqtt_binding-2.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 18:10:25.732954 homeassistant_mqtt_binding-2.0.3/ha_mqtt/__init__.py
+-rw-r--r--   0        0        0     2607 2023-06-22 18:10:25.707954 homeassistant_mqtt_binding-2.0.3/ha_mqtt/ha_device.py
+-rw-r--r--   0        0        0     8922 2023-06-22 18:10:25.707954 homeassistant_mqtt_binding-2.0.3/ha_mqtt/mqtt_device_base.py
+-rw-r--r--   0        0        0     1377 2023-06-22 18:10:25.707954 homeassistant_mqtt_binding-2.0.3/ha_mqtt/mqtt_sensor.py
+-rw-r--r--   0        0        0     1190 2023-06-22 18:10:25.707954 homeassistant_mqtt_binding-2.0.3/ha_mqtt/mqtt_siren.py
+-rw-r--r--   0        0        0     3279 2023-06-22 18:10:25.707954 homeassistant_mqtt_binding-2.0.3/ha_mqtt/mqtt_switch.py
+-rw-r--r--   0        0        0      615 2023-06-22 18:10:25.707954 homeassistant_mqtt_binding-2.0.3/ha_mqtt/mqtt_thermometer.py
+-rw-r--r--   0        0        0        0 2023-06-22 18:10:25.732954 homeassistant_mqtt_binding-2.0.3/ha_mqtt/py.typed
+-rw-r--r--   0        0        0     3272 2023-06-22 18:10:25.707954 homeassistant_mqtt_binding-2.0.3/ha_mqtt/util.py
+-rw-r--r--   0        0        0     1117 2023-06-22 18:10:25.708954 homeassistant_mqtt_binding-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3324 1970-01-01 00:00:00.000000 homeassistant_mqtt_binding-2.0.3/PKG-INFO
```

### Comparing `homeassistant_mqtt_binding-2.0.2/LICENSE` & `homeassistant_mqtt_binding-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `homeassistant_mqtt_binding-2.0.2/README.md` & `homeassistant_mqtt_binding-2.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Homeassistant MQTT Binding for python
+[![PyPI version](https://badge.fury.io/py/homeassistant-mqtt-binding.svg)](https://badge.fury.io/py/homeassistant-mqtt-binding)
 
 This package enables you to implement arbitrary devices in python supported in homeassistant. The communication with
 homeassistant is handled by MQTT. For example you could write an simple program running on a raspberry pi controlling an
 LED. By exposing this configuration to homeassistant you can easily control the LED via HA.
 
 The base class handles the following things automatically:
```

### Comparing `homeassistant_mqtt_binding-2.0.2/ha_mqtt/ha_device.py` & `homeassistant_mqtt_binding-2.0.3/ha_mqtt/ha_device.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 this module contains the HaDevice class
 """
 
 #  Copyright (c) 2022 - Andreas Philipp
 #  This code is published under the MIT license
 
 import json
+from typing import Any, Dict, List
 
 
 class HaDevice:
     """
     Class for configuring a device that groups multiple entities in homeassistant
     """
 
@@ -21,58 +22,60 @@
         constructor
         :param name: friendly name of the device
         :param unique_id: one unique identifier that is used by HA to assign entities to this device
         """
         self._name = name
         self.config = {
             "name": name,
-            "identifiers": [unique_id]
+            "identifiers": [unique_id],
         }
 
     def __str__(self):
         return f"{self._name}: {self.get_json()}"
 
-    def add_config_option(self, key: str, value, override: bool = False):
+    def add_config_option(self, key: str, value: Any, override: bool = False):
         """
         adds an arbitrary item to the device config.
         It must be json serializable (preferred lists, dicts and key/value pairs)
         :param key key to assign the setting to
         :param value settings item to be written to the config
         :param override if set to true, override an existing item if present
         """
         if self.config.get(key) and not override:
             raise ValueError(
-                "You are trying to override an existing config option. Specify 'override = True' if this was intended")
+                "You are trying to override an existing config option. "
+                "Specify 'override = True' if this was intended"
+            )
         self.config[key] = value
 
     @property
-    def identifiers(self) -> list:
+    def identifiers(self) -> List[str]:
         """
         gets all set identifiers of this device
         :return: list containing the identifiers
         """
-        return self.config.get("identifiers", [])
+        return self.config.get("identifiers", [])  # type: ignore
 
     def append_identifier(self, identifier: str):
         """
         appends a new identifier to the identifier list
         Make sur eto only use unique identifiers
         :param identifier: the identifier to add
         :raises ValueError: if the identifier already exists in the list
         """
         if identifier in self.config["identifiers"]:
             raise ValueError("identifier is already present")
-        self.config["identifiers"].append(identifier)
+        self.config["identifiers"].append(identifier)  # type: ignore
 
     def get_json(self) -> str:
         """
         returns the json representation of the current configuration
         :return: json representation of the config
         """
         return json.dumps(self.config)
 
-    def get_dict(self) -> dict:
+    def get_dict(self) -> Dict[str, Any]:
         """
         returns the current configuration dict
         :return: dict containing the config
         """
         return self.config
```

### Comparing `homeassistant_mqtt_binding-2.0.2/ha_mqtt/mqtt_device_base.py` & `homeassistant_mqtt_binding-2.0.3/ha_mqtt/mqtt_device_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,33 +5,40 @@
 #  Copyright (c) 2022 - Andreas Philipp
 #  This code is published under the MIT license
 
 import json
 import logging
 import time
 from dataclasses import dataclass
+from typing import Any, Dict, Optional, Union
 
 from paho.mqtt.client import Client, MQTTMessage
 
-from ha_mqtt.ha_device import HaDevice
-from ha_mqtt.util import EntityCategory
+from .ha_device import HaDevice
+from .util import EntityCategory
 
 
 @dataclass
 class MqttDeviceSettings:
     """
     class for storing settings like name and unique ID
 
     :param name: Friendly name of the device to be shown in homeassistant
     :param unique_id: unique id to identify this device against homeassistant
     :param client: paho mqtt client instance
     """
 
-    def __init__(self, name: str, unique_id: str, client: Client, device: HaDevice = None,
-                 entity_type: EntityCategory = EntityCategory.PRIMARY):
+    def __init__(
+        self,
+        name: str,
+        unique_id: str,
+        client: Client,
+        device: Optional[HaDevice] = None,
+        entity_type: EntityCategory = EntityCategory.PRIMARY,
+    ):
         assert isinstance(unique_id, str), "the unique ID must be a string"
         self.device = device
         self.name = name
         self.unique_id = unique_id
         self.client = client
         self.entity_type = entity_type
 
@@ -112,15 +119,15 @@
         self._logger = logging.getLogger(self.name)
 
         self.base_topic = f"{self.__class__.base_topic}/{self.__class__.device_type}/{self._unique_id}"
         self.avail_topic = f"{self.base_topic}/available"
         self.config_topic = f"{self.base_topic}/config"
         self.state_topic = f"{self.base_topic}/state"
 
-        self.conf_dict = {
+        self.conf_dict: Dict[str, Any] = {
             'name': self.name,
             'state_topic': self.state_topic,
             'availability_topic': self.avail_topic,
             'unique_id': self._unique_id,
 
         }
         if self._entity_type != EntityCategory.PRIMARY:
@@ -177,24 +184,27 @@
     def post_discovery(self):
         """
         run additional tasks after sending out the discovery command
         Useful in subclasses to run initialization of internal values
         Runs synchronously.
         """
 
-    def publish_state(self, payload: object, retain: bool = True):
+    def publish_state(
+        self,
+        payload: Union[str, bytes, bytearray, int, float, None],
+        retain: bool = True,
+    ):
         """
         publishes a payload on the device's state topic
 
         :param payload: payload to publish
         :param retain: set to True to send as a retained message
         """
 
-        self._logger.debug("publishing payload '%s' for %s",
-                           payload, self._unique_id)
+        self._logger.debug("publishing payload '%s' for %s", payload, self._unique_id)
 
         self._client.publish(self.state_topic, payload, retain=retain)
         time.sleep(0.01)
 
     def state_callback(self, client: Client, userdata: object, msg: MQTTMessage):
         """
         callback that gets executed when receiving a message on the state topic
@@ -223,15 +233,15 @@
     def delete_config(self):
         """
         delete the sensor from homeassistant,
         sends an empty payload to the config topic
         """
         self._client.publish(self.config_topic, "")
 
-    def _send_discovery(self, send_initial=True):
+    def _send_discovery(self, send_initial: bool = True):
         """
         sends discovery package to broker
 
         :param send_initial: determines if the classes' initital state should be sent or not
         """
         self._client.publish(self.config_topic, json.dumps(
             self.conf_dict), retain=True)
```

### Comparing `homeassistant_mqtt_binding-2.0.2/ha_mqtt/mqtt_sensor.py` & `homeassistant_mqtt_binding-2.0.3/ha_mqtt/mqtt_sensor.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,16 +24,21 @@
        Use :meth:`~ha_mqtt.mqtt_device_base.MqttDeviceBase.publish_state`
        to send the actual sensor data to homeassistant
 
     """
 
     device_type = "sensor"
 
-    def __init__(self, settings: MqttDeviceSettings, unit: str, device_class: HaDeviceClass
-                 , send_only=False):
+    def __init__(
+        self,
+        settings: MqttDeviceSettings,
+        unit: str,
+        device_class: HaDeviceClass,
+        send_only: bool = False,
+    ):
         """
         create sensor instance
         """
         self.device_class = device_class
         self.unit_of_measurement = unit
         super().__init__(settings, send_only)
```

### Comparing `homeassistant_mqtt_binding-2.0.2/ha_mqtt/mqtt_siren.py` & `homeassistant_mqtt_binding-2.0.3/ha_mqtt/mqtt_siren.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 """
 #  Copyright (c) 2022 - Andreas Philipp
 #  This code is published under the MIT license
 
 import json
 import threading
 
+from paho.mqtt.client import Client, MQTTMessage
+
 from . import util
 from .mqtt_switch import MqttSwitch
 
 
 class MqttSiren(MqttSwitch):
     """
     simple siren that runs a callback that can be used to
@@ -23,17 +25,18 @@
        The off callback runs synchronously.
 
 
     .. note::
        call `set_off()` in the end of your callback to automatically turn off the siren
        once the sound has been played
     """
+
     device_type = "siren"
 
-    def command_callback(self, client, userdata, msg):
+    def command_callback(self, client: Client, userdata: object, msg: MQTTMessage):
         cmd_dict = json.loads(msg.payload.decode("ascii"))
         cmd_str = cmd_dict.get("state", util.OFF)
         if cmd_str.encode("ascii") == util.ON:
             self.set_on()
             threading.Thread(target=self.callback_on, name="callback_thread").start()
         else:
             self.set_off()
```

### Comparing `homeassistant_mqtt_binding-2.0.2/ha_mqtt/mqtt_switch.py` & `homeassistant_mqtt_binding-2.0.3/ha_mqtt/mqtt_switch.py`

 * *Files identical despite different names*

### Comparing `homeassistant_mqtt_binding-2.0.2/ha_mqtt/mqtt_thermometer.py` & `homeassistant_mqtt_binding-2.0.3/ha_mqtt/mqtt_thermometer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 this module contains all classes for implementing mqtt thermometers
 """
 
 #  Copyright (c) 2022 - Andreas Philipp
 #  This code is published under the MIT license
 
-from .mqtt_sensor import MqttSensor, MqttDeviceSettings
+from .mqtt_sensor import MqttDeviceSettings, MqttSensor
 from .util import HaDeviceClass
 
 
 class MqttThermometer(MqttSensor):
     """
     subclass of MqttSensor, measures temperatures.
     The default unit is °C and can be changed in the constructor
     """
 
-    def __init__(self, settings: MqttDeviceSettings, unit: str = "°C", send_only=True):
+    def __init__(
+        self, settings: MqttDeviceSettings, unit: str = "°C", send_only: bool = True
+    ):
         super().__init__(settings, unit, HaDeviceClass.TEMPERATURE, send_only)
```

### Comparing `homeassistant_mqtt_binding-2.0.2/ha_mqtt/util.py` & `homeassistant_mqtt_binding-2.0.3/ha_mqtt/util.py`

 * *Files identical despite different names*

### Comparing `homeassistant_mqtt_binding-2.0.2/pyproject.toml` & `homeassistant_mqtt_binding-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "homeassistant-mqtt-binding"
-version = "2.0.2"
+version = "2.0.3"
 description = "Bindings to implement arbitrary homeassistant devices in python using mqtt as interface"
 authors = ["Andreas Philipp"]
 license = "MIT"
 readme = "README.md"
 repository = "https://gitlab.com/anphi/homeassistant-mqtt-binding"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `homeassistant_mqtt_binding-2.0.2/PKG-INFO` & `homeassistant_mqtt_binding-2.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: homeassistant-mqtt-binding
-Version: 2.0.2
+Version: 2.0.3
 Summary: Bindings to implement arbitrary homeassistant devices in python using mqtt as interface
 Home-page: https://gitlab.com/anphi/homeassistant-mqtt-binding
 License: MIT
 Author: Andreas Philipp
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Home Automation
 Requires-Dist: paho-mqtt (>=1.6,<2.0)
 Project-URL: Repository, https://gitlab.com/anphi/homeassistant-mqtt-binding
 Description-Content-Type: text/markdown
 
 # Homeassistant MQTT Binding for python
+[![PyPI version](https://badge.fury.io/py/homeassistant-mqtt-binding.svg)](https://badge.fury.io/py/homeassistant-mqtt-binding)
 
 This package enables you to implement arbitrary devices in python supported in homeassistant. The communication with
 homeassistant is handled by MQTT. For example you could write an simple program running on a raspberry pi controlling an
 LED. By exposing this configuration to homeassistant you can easily control the LED via HA.
 
 The base class handles the following things automatically:
```

