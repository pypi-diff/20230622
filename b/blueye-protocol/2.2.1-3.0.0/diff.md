# Comparing `tmp/blueye_protocol-2.2.1.tar.gz` & `tmp/blueye.protocol-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueye_protocol-2.2.1.tar", max compression
+gzip compressed data, was "blueye.protocol-3.0.0.tar", max compression
```

## Comparing `blueye_protocol-2.2.1.tar` & `blueye.protocol-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,13 @@
--rw-r--r--   0        0        0     7652 2023-06-22 11:46:18.358066 blueye_protocol-2.2.1/LICENSE
--rw-r--r--   0        0        0     2748 2023-06-22 11:46:18.358066 blueye_protocol-2.2.1/README.md
--rw-r--r--   0        0        0      128 2023-06-22 11:46:18.358066 blueye_protocol-2.2.1/blueye/__init__.py
--rw-r--r--   0        0        0      311 2023-06-22 11:46:18.358066 blueye_protocol-2.2.1/blueye/protocol/__init__.py
--rw-r--r--   0        0        0     1329 2023-06-22 11:46:18.358066 blueye_protocol-2.2.1/blueye/protocol/exceptions.py
--rw-r--r--   0        0        0    12634 2023-06-22 11:46:18.358066 blueye_protocol-2.2.1/blueye/protocol/protos.py
--rw-r--r--   0        0        0     8283 2023-06-22 11:46:18.358066 blueye_protocol-2.2.1/blueye/protocol/types/__init__.py
--rw-r--r--   0        0        0    10626 2023-06-22 11:46:18.358066 blueye_protocol-2.2.1/blueye/protocol/types/control.py
--rw-r--r--   0        0        0    56952 2023-06-22 11:46:18.358066 blueye_protocol-2.2.1/blueye/protocol/types/message_formats.py
--rw-r--r--   0        0        0     8447 2023-06-22 11:46:18.358066 blueye_protocol-2.2.1/blueye/protocol/types/req_rep.py
--rw-r--r--   0        0        0    14669 2023-06-22 11:46:18.358066 blueye_protocol-2.2.1/blueye/protocol/types/telemetry.py
--rw-r--r--   0        0        0        0 2023-06-22 11:46:18.358066 blueye_protocol-2.2.1/blueye/protocol/v2/__init__.py
--rwxr-xr-x   0        0        0     5219 2023-06-22 11:46:18.358066 blueye_protocol-2.2.1/blueye/protocol/v2/tcp_client.py
--rw-r--r--   0        0        0    37722 2023-06-22 11:46:18.358066 blueye_protocol-2.2.1/blueye/protocol/v2/tcp_protocol_class.py
--rwxr-xr-x   0        0        0     2744 2023-06-22 11:46:18.358066 blueye_protocol-2.2.1/blueye/protocol/v2/udp_client.py
--rw-r--r--   0        0        0    23217 2023-06-22 11:46:18.358066 blueye_protocol-2.2.1/blueye/protocol/v2/udp_protocol_dict.py
--rwxr-xr-x   0        0        0     3738 2023-06-22 11:46:18.358066 blueye_protocol-2.2.1/blueye/protocol/v2/udp_protocol_parser.py
--rw-r--r--   0        0        0     1041 2023-06-22 11:46:18.358066 blueye_protocol-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     3606 1970-01-01 00:00:00.000000 blueye_protocol-2.2.1/setup.py
--rw-r--r--   0        0        0     3613 1970-01-01 00:00:00.000000 blueye_protocol-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0      608 2022-09-15 09:34:34.569966 blueye.protocol-3.0.0/README.md
+-rw-r--r--   0        0        0      173 2022-09-15 09:34:34.569966 blueye.protocol-3.0.0/blueye/__init__.py
+-rw-r--r--   0        0        0    10054 2022-09-15 09:34:59.514605 blueye.protocol-3.0.0/blueye/protocol/__init__.py
+-rw-r--r--   0        0        0       76 2022-09-15 09:34:59.514605 blueye.protocol-3.0.0/blueye/protocol/py.typed
+-rw-r--r--   0        0        0      601 2022-09-15 09:34:59.514605 blueye.protocol-3.0.0/blueye/protocol/services/__init__.py
+-rw-r--r--   0        0        0     6621 2022-09-15 09:34:59.514605 blueye.protocol-3.0.0/blueye/protocol/types/__init__.py
+-rw-r--r--   0        0        0     8621 2022-09-15 09:34:59.514605 blueye.protocol-3.0.0/blueye/protocol/types/control.py
+-rw-r--r--   0        0        0    48847 2022-09-15 09:34:59.514605 blueye.protocol-3.0.0/blueye/protocol/types/message_formats.py
+-rw-r--r--   0        0        0     5985 2022-09-15 09:34:59.514605 blueye.protocol-3.0.0/blueye/protocol/types/req_rep.py
+-rw-r--r--   0        0        0    10713 2022-09-15 09:34:59.514605 blueye.protocol-3.0.0/blueye/protocol/types/telemetry.py
+-rw-r--r--   0        0        0      696 2022-09-15 09:34:34.573966 blueye.protocol-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1374 2022-09-15 09:35:00.250462 blueye.protocol-3.0.0/setup.py
+-rw-r--r--   0        0        0     1417 2022-09-15 09:35:00.250781 blueye.protocol-3.0.0/PKG-INFO
```

### Comparing `blueye_protocol-2.2.1/blueye/protocol/protos.py` & `blueye.protocol-3.0.0/blueye/protocol/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,34 +11,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from .types.control import ActivateGuestPortsCtrl
 from .types.control import AutoAltitudeCtrl
 from .types.control import AutoDepthCtrl
 from .types.control import AutoHeadingCtrl
 from .types.control import CancelCalibrationCtrl
-from .types.control import DeactivateGuestPortsCtrl
 from .types.control import FinishCalibrationCtrl
-from .types.control import GenericServoCtrl
 from .types.control import GripperCtrl
 from .types.control import GuestportLightsCtrl
-from .types.control import LaserCtrl
 from .types.control import LightsCtrl
 from .types.control import MotionInputCtrl
-from .types.control import MultibeamServoCtrl
 from .types.control import PilotGPSPositionCtrl
 from .types.control import PingerConfigurationCtrl
 from .types.control import RecordCtrl
 from .types.control import ResetOdometerCtrl
 from .types.control import ResetPositionCtrl
-from .types.control import RestartGuestPortsCtrl
 from .types.control import StartCalibrationCtrl
 from .types.control import StationKeepingCtrl
 from .types.control import SystemTimeCtrl
 from .types.control import TakePictureCtrl
 from .types.control import TiltStabilizationCtrl
 from .types.control import TiltVelocityCtrl
 from .types.control import WatchdogCtrl
@@ -57,143 +51,112 @@
 from .types.message_formats import Camera
 from .types.message_formats import CameraParameters
 from .types.message_formats import CanisterHumidity
 from .types.message_formats import CanisterTemperature
 from .types.message_formats import ClientInfo
 from .types.message_formats import ConnectedClient
 from .types.message_formats import ConnectionDuration
-from .types.message_formats import ControlForce
 from .types.message_formats import ControlMode
 from .types.message_formats import ControllerHealth
 from .types.message_formats import CpProbe
 from .types.message_formats import Depth
 from .types.message_formats import DepthUnit
 from .types.message_formats import DiveTime
 from .types.message_formats import DroneInfo
 from .types.message_formats import ErrorFlags
 from .types.message_formats import FontSize
 from .types.message_formats import ForwardDistance
 from .types.message_formats import Framerate
-from .types.message_formats import GenericServo
 from .types.message_formats import GripperVelocities
 from .types.message_formats import GuestPortConnectorInfo
-from .types.message_formats import GuestPortCurrent
 from .types.message_formats import GuestPortDevice
 from .types.message_formats import GuestPortDeviceID
 from .types.message_formats import GuestPortDeviceList
 from .types.message_formats import GuestPortError
 from .types.message_formats import GuestPortInfo
-from .types.message_formats import GuestPortNumber
-from .types.message_formats import GuestPortRestartInfo
-from .types.message_formats import HeadingSource
-from .types.message_formats import Imu
 from .types.message_formats import IperfStatus
-from .types.message_formats import Laser
 from .types.message_formats import LatLongPosition
 from .types.message_formats import Lights
 from .types.message_formats import LogoType
-from .types.message_formats import MedusaSpectrometerData
 from .types.message_formats import Model
 from .types.message_formats import MotionInput
-from .types.message_formats import MultibeamServo
 from .types.message_formats import NStreamers
 from .types.message_formats import NavigationSensorID
 from .types.message_formats import NavigationSensorStatus
 from .types.message_formats import OverlayParameters
 from .types.message_formats import PingerConfiguration
 from .types.message_formats import PositionEstimate
 from .types.message_formats import PressureSensorType
 from .types.message_formats import RecordOn
 from .types.message_formats import RecordState
 from .types.message_formats import Reference
-from .types.message_formats import ResetCoordinateSource
-from .types.message_formats import ResetPositionSettings
 from .types.message_formats import Resolution
 from .types.message_formats import StationKeepingState
 from .types.message_formats import StorageSpace
 from .types.message_formats import SystemTime
 from .types.message_formats import TemperatureUnit
 from .types.message_formats import ThicknessGauge
 from .types.message_formats import ThicknessUnit
 from .types.message_formats import TiltAngle
 from .types.message_formats import TiltStabilizationState
 from .types.message_formats import TiltVelocity
-from .types.message_formats import Vector3
 from .types.message_formats import WaterDensity
 from .types.message_formats import WaterTemperature
 from .types.message_formats import WeatherVaningState
 from .types.req_rep import ConnectClientRep
 from .types.req_rep import ConnectClientReq
-from .types.req_rep import DisconnectClientRep
-from .types.req_rep import DisconnectClientReq
-from .types.req_rep import GetBatteryRep
-from .types.req_rep import GetBatteryReq
 from .types.req_rep import GetCameraParametersRep
 from .types.req_rep import GetCameraParametersReq
 from .types.req_rep import GetOverlayParametersRep
 from .types.req_rep import GetOverlayParametersReq
 from .types.req_rep import PingRep
 from .types.req_rep import PingReq
 from .types.req_rep import SetCameraParametersRep
 from .types.req_rep import SetCameraParametersReq
 from .types.req_rep import SetOverlayParametersRep
 from .types.req_rep import SetOverlayParametersReq
-from .types.req_rep import SetPubFrequencyRep
-from .types.req_rep import SetPubFrequencyReq
 from .types.req_rep import SetThicknessGaugeParametersRep
 from .types.req_rep import SetThicknessGaugeParametersReq
 from .types.req_rep import SyncTimeRep
 from .types.req_rep import SyncTimeReq
 from .types.telemetry import AltitudeTel
 from .types.telemetry import AttitudeTel
 from .types.telemetry import BatteryBQ40Z50Tel
 from .types.telemetry import BatteryTel
 from .types.telemetry import CPUTemperatureTel
-from .types.telemetry import CalibratedImuTel
 from .types.telemetry import CalibrationStateTel
-from .types.telemetry import CanisterBottomHumidityTel
-from .types.telemetry import CanisterBottomTemperatureTel
-from .types.telemetry import CanisterTopHumidityTel
-from .types.telemetry import CanisterTopTemperatureTel
+from .types.telemetry import CanisterHumidityTel
+from .types.telemetry import CanisterTemperatureTel
 from .types.telemetry import ConnectedClientsTel
-from .types.telemetry import ControlForceTel
 from .types.telemetry import ControlModeTel
 from .types.telemetry import ControllerHealthTel
 from .types.telemetry import CpProbeTel
 from .types.telemetry import DataStorageSpaceTel
 from .types.telemetry import DepthTel
 from .types.telemetry import DiveTimeTel
 from .types.telemetry import DroneInfoTel
 from .types.telemetry import DroneTimeTel
 from .types.telemetry import ErrorFlagsTel
 from .types.telemetry import ForwardDistanceTel
-from .types.telemetry import GenericServoTel
-from .types.telemetry import GuestPortCurrentTel
 from .types.telemetry import GuestPortLightsTel
-from .types.telemetry import Imu1Tel
-from .types.telemetry import Imu2Tel
 from .types.telemetry import IperfTel
-from .types.telemetry import LaserTel
 from .types.telemetry import LightsTel
-from .types.telemetry import MedusaSpectrometerDataTel
-from .types.telemetry import MultibeamServoTel
 from .types.telemetry import NStreamersTel
 from .types.telemetry import PilotGPSPositionTel
 from .types.telemetry import PositionEstimateTel
 from .types.telemetry import RecordStateTel
 from .types.telemetry import ReferenceTel
 from .types.telemetry import ThicknessGaugeTel
 from .types.telemetry import TiltAngleTel
 from .types.telemetry import TiltStabilizationTel
 from .types.telemetry import VideoStorageSpaceTel
 from .types.telemetry import WaterTemperatureTel
 
 
 __all__ = (
-    'ActivateGuestPortsCtrl',
     'Altitude',
     'AltitudeTel',
     'Attitude',
     'AttitudeTel',
     'AutoAltitudeCtrl',
     'AutoAltitudeState',
     'AutoDepthCtrl',
@@ -202,104 +165,75 @@
     'AutoHeadingState',
     'Battery',
     'BatteryBQ40Z50',
     'BatteryBQ40Z50Tel',
     'BatteryTel',
     'CPUTemperature',
     'CPUTemperatureTel',
-    'CalibratedImuTel',
     'CalibrationState',
     'CalibrationStateTel',
     'Camera',
     'CameraParameters',
     'CancelCalibrationCtrl',
-    'CanisterBottomHumidityTel',
-    'CanisterBottomTemperatureTel',
     'CanisterHumidity',
+    'CanisterHumidityTel',
     'CanisterTemperature',
-    'CanisterTopHumidityTel',
-    'CanisterTopTemperatureTel',
+    'CanisterTemperatureTel',
     'ClientInfo',
     'ConnectClientRep',
     'ConnectClientReq',
     'ConnectedClient',
     'ConnectedClientsTel',
     'ConnectionDuration',
-    'ControlForce',
-    'ControlForceTel',
     'ControlMode',
     'ControlModeTel',
     'ControllerHealth',
     'ControllerHealthTel',
     'CpProbe',
     'CpProbeTel',
     'DataStorageSpaceTel',
-    'DeactivateGuestPortsCtrl',
     'Depth',
     'DepthTel',
     'DepthUnit',
-    'DisconnectClientRep',
-    'DisconnectClientReq',
     'DiveTime',
     'DiveTimeTel',
     'DroneInfo',
     'DroneInfoTel',
     'DroneTimeTel',
     'ErrorFlags',
     'ErrorFlagsTel',
     'FinishCalibrationCtrl',
     'FontSize',
     'ForwardDistance',
     'ForwardDistanceTel',
     'Framerate',
-    'GenericServo',
-    'GenericServoCtrl',
-    'GenericServoTel',
-    'GetBatteryRep',
-    'GetBatteryReq',
     'GetCameraParametersRep',
     'GetCameraParametersReq',
     'GetOverlayParametersRep',
     'GetOverlayParametersReq',
     'GripperCtrl',
     'GripperVelocities',
     'GuestPortConnectorInfo',
-    'GuestPortCurrent',
-    'GuestPortCurrentTel',
     'GuestPortDevice',
     'GuestPortDeviceID',
     'GuestPortDeviceList',
     'GuestPortError',
     'GuestPortInfo',
     'GuestPortLightsTel',
-    'GuestPortNumber',
-    'GuestPortRestartInfo',
     'GuestportLightsCtrl',
-    'HeadingSource',
-    'Imu',
-    'Imu1Tel',
-    'Imu2Tel',
     'IperfStatus',
     'IperfTel',
-    'Laser',
-    'LaserCtrl',
-    'LaserTel',
     'LatLongPosition',
     'Lights',
     'LightsCtrl',
     'LightsTel',
     'LogoType',
-    'MedusaSpectrometerData',
-    'MedusaSpectrometerDataTel',
     'Model',
     'MotionInput',
     'MotionInputCtrl',
-    'MultibeamServo',
-    'MultibeamServoCtrl',
-    'MultibeamServoTel',
     'NStreamers',
     'NStreamersTel',
     'NavigationSensorID',
     'NavigationSensorStatus',
     'OverlayParameters',
     'PilotGPSPositionCtrl',
     'PilotGPSPositionTel',
@@ -312,26 +246,21 @@
     'PressureSensorType',
     'RecordCtrl',
     'RecordOn',
     'RecordState',
     'RecordStateTel',
     'Reference',
     'ReferenceTel',
-    'ResetCoordinateSource',
     'ResetOdometerCtrl',
     'ResetPositionCtrl',
-    'ResetPositionSettings',
     'Resolution',
-    'RestartGuestPortsCtrl',
     'SetCameraParametersRep',
     'SetCameraParametersReq',
     'SetOverlayParametersRep',
     'SetOverlayParametersReq',
-    'SetPubFrequencyRep',
-    'SetPubFrequencyReq',
     'SetThicknessGaugeParametersRep',
     'SetThicknessGaugeParametersReq',
     'StartCalibrationCtrl',
     'StationKeepingCtrl',
     'StationKeepingState',
     'StorageSpace',
     'SyncTimeRep',
@@ -346,15 +275,14 @@
     'TiltAngle',
     'TiltAngleTel',
     'TiltStabilizationCtrl',
     'TiltStabilizationState',
     'TiltStabilizationTel',
     'TiltVelocity',
     'TiltVelocityCtrl',
-    'Vector3',
     'VideoStorageSpaceTel',
     'WatchdogCtrl',
     'WaterDensity',
     'WaterDensityCtrl',
     'WaterTemperature',
     'WaterTemperatureTel',
     'WeatherVaningCtrl',
```

### Comparing `blueye_protocol-2.2.1/blueye/protocol/types/__init__.py` & `blueye.protocol-3.0.0/blueye/protocol/types/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 # limitations under the License.
 #
 
 from .message_formats import (
     BinlogRecord,
     MotionInput,
     Lights,
-    Laser,
     LatLongPosition,
     ConnectionDuration,
     AutoHeadingState,
     AutoDepthState,
     AutoAltitudeState,
     StationKeepingState,
     WeatherVaningState,
@@ -42,18 +41,16 @@
     CanisterHumidity,
     Battery,
     BatteryBQ40Z50,
     Attitude,
     Altitude,
     ForwardDistance,
     PositionEstimate,
-    ResetPositionSettings,
     Depth,
     Reference,
-    ControlForce,
     ControllerHealth,
     DiveTime,
     RecordOn,
     StorageSpace,
     CalibrationState,
     IperfStatus,
     NStreamers,
@@ -64,84 +61,88 @@
     CameraParameters,
     OverlayParameters,
     NavigationSensorStatus,
     GuestPortDevice,
     GuestPortDeviceList,
     GuestPortConnectorInfo,
     GuestPortInfo,
-    GuestPortRestartInfo,
     ThicknessGauge,
     CpProbe,
-    GenericServo,
-    MultibeamServo,
-    GuestPortCurrent,
-    Vector3,
-    Imu,
-    MedusaSpectrometerData,
-    HeadingSource,
-    ResetCoordinateSource,
     Model,
     PressureSensorType,
     Resolution,
     Framerate,
     Camera,
     TemperatureUnit,
     LogoType,
     DepthUnit,
     ThicknessUnit,
     FontSize,
     GuestPortDeviceID,
-    GuestPortNumber,
     NavigationSensorID,
     GuestPortError,
 )
+from .control import (
+    MotionInputCtrl,
+    TiltVelocityCtrl,
+    LightsCtrl,
+    GuestportLightsCtrl,
+    PilotGPSPositionCtrl,
+    WatchdogCtrl,
+    RecordCtrl,
+    TakePictureCtrl,
+    StartCalibrationCtrl,
+    CancelCalibrationCtrl,
+    FinishCalibrationCtrl,
+    AutoHeadingCtrl,
+    AutoDepthCtrl,
+    AutoAltitudeCtrl,
+    StationKeepingCtrl,
+    WeatherVaningCtrl,
+    ResetPositionCtrl,
+    ResetOdometerCtrl,
+    TiltStabilizationCtrl,
+    WaterDensityCtrl,
+    PingerConfigurationCtrl,
+    SystemTimeCtrl,
+    GripperCtrl,
+)
 from .telemetry import (
     AttitudeTel,
     AltitudeTel,
     ForwardDistanceTel,
     PositionEstimateTel,
     DepthTel,
     ReferenceTel,
-    ControlForceTel,
     ControllerHealthTel,
     LightsTel,
     GuestPortLightsTel,
-    LaserTel,
     PilotGPSPositionTel,
     RecordStateTel,
     BatteryTel,
     BatteryBQ40Z50Tel,
     DiveTimeTel,
     DroneTimeTel,
     WaterTemperatureTel,
     CPUTemperatureTel,
-    CanisterTopTemperatureTel,
-    CanisterBottomTemperatureTel,
-    CanisterTopHumidityTel,
-    CanisterBottomHumidityTel,
+    CanisterTemperatureTel,
+    CanisterHumidityTel,
     VideoStorageSpaceTel,
     DataStorageSpaceTel,
     CalibrationStateTel,
     TiltStabilizationTel,
     IperfTel,
     NStreamersTel,
     TiltAngleTel,
     DroneInfoTel,
     ErrorFlagsTel,
     ControlModeTel,
     ThicknessGaugeTel,
     CpProbeTel,
     ConnectedClientsTel,
-    GenericServoTel,
-    MultibeamServoTel,
-    GuestPortCurrentTel,
-    CalibratedImuTel,
-    Imu1Tel,
-    Imu2Tel,
-    MedusaSpectrometerDataTel,
 )
 from .req_rep import (
     SetOverlayParametersReq,
     SetOverlayParametersRep,
     GetOverlayParametersReq,
     GetOverlayParametersRep,
     SetCameraParametersReq,
@@ -152,58 +153,20 @@
     SyncTimeRep,
     PingReq,
     PingRep,
     SetThicknessGaugeParametersReq,
     SetThicknessGaugeParametersRep,
     ConnectClientReq,
     ConnectClientRep,
-    DisconnectClientReq,
-    DisconnectClientRep,
-    GetBatteryReq,
-    GetBatteryRep,
-    SetPubFrequencyReq,
-    SetPubFrequencyRep,
-)
-from .control import (
-    MotionInputCtrl,
-    TiltVelocityCtrl,
-    LightsCtrl,
-    GuestportLightsCtrl,
-    LaserCtrl,
-    PilotGPSPositionCtrl,
-    WatchdogCtrl,
-    RecordCtrl,
-    TakePictureCtrl,
-    StartCalibrationCtrl,
-    CancelCalibrationCtrl,
-    FinishCalibrationCtrl,
-    AutoHeadingCtrl,
-    AutoDepthCtrl,
-    AutoAltitudeCtrl,
-    StationKeepingCtrl,
-    WeatherVaningCtrl,
-    ResetPositionCtrl,
-    ResetOdometerCtrl,
-    TiltStabilizationCtrl,
-    WaterDensityCtrl,
-    PingerConfigurationCtrl,
-    SystemTimeCtrl,
-    GripperCtrl,
-    GenericServoCtrl,
-    MultibeamServoCtrl,
-    DeactivateGuestPortsCtrl,
-    ActivateGuestPortsCtrl,
-    RestartGuestPortsCtrl,
 )
 
 __all__ = (
     'BinlogRecord',
     'MotionInput',
     'Lights',
-    'Laser',
     'LatLongPosition',
     'ConnectionDuration',
     'AutoHeadingState',
     'AutoDepthState',
     'AutoAltitudeState',
     'StationKeepingState',
     'WeatherVaningState',
@@ -222,18 +185,16 @@
     'CanisterHumidity',
     'Battery',
     'BatteryBQ40Z50',
     'Attitude',
     'Altitude',
     'ForwardDistance',
     'PositionEstimate',
-    'ResetPositionSettings',
     'Depth',
     'Reference',
-    'ControlForce',
     'ControllerHealth',
     'DiveTime',
     'RecordOn',
     'StorageSpace',
     'CalibrationState',
     'IperfStatus',
     'NStreamers',
@@ -244,82 +205,84 @@
     'CameraParameters',
     'OverlayParameters',
     'NavigationSensorStatus',
     'GuestPortDevice',
     'GuestPortDeviceList',
     'GuestPortConnectorInfo',
     'GuestPortInfo',
-    'GuestPortRestartInfo',
     'ThicknessGauge',
     'CpProbe',
-    'GenericServo',
-    'MultibeamServo',
-    'GuestPortCurrent',
-    'Vector3',
-    'Imu',
-    'MedusaSpectrometerData',
-    'HeadingSource',
-    'ResetCoordinateSource',
     'Model',
     'PressureSensorType',
     'Resolution',
     'Framerate',
     'Camera',
     'TemperatureUnit',
     'LogoType',
     'DepthUnit',
     'ThicknessUnit',
     'FontSize',
     'GuestPortDeviceID',
-    'GuestPortNumber',
     'NavigationSensorID',
     'GuestPortError',
+    'MotionInputCtrl',
+    'TiltVelocityCtrl',
+    'LightsCtrl',
+    'GuestportLightsCtrl',
+    'PilotGPSPositionCtrl',
+    'WatchdogCtrl',
+    'RecordCtrl',
+    'TakePictureCtrl',
+    'StartCalibrationCtrl',
+    'CancelCalibrationCtrl',
+    'FinishCalibrationCtrl',
+    'AutoHeadingCtrl',
+    'AutoDepthCtrl',
+    'AutoAltitudeCtrl',
+    'StationKeepingCtrl',
+    'WeatherVaningCtrl',
+    'ResetPositionCtrl',
+    'ResetOdometerCtrl',
+    'TiltStabilizationCtrl',
+    'WaterDensityCtrl',
+    'PingerConfigurationCtrl',
+    'SystemTimeCtrl',
+    'GripperCtrl',
     'AttitudeTel',
     'AltitudeTel',
     'ForwardDistanceTel',
     'PositionEstimateTel',
     'DepthTel',
     'ReferenceTel',
-    'ControlForceTel',
     'ControllerHealthTel',
     'LightsTel',
     'GuestPortLightsTel',
-    'LaserTel',
     'PilotGPSPositionTel',
     'RecordStateTel',
     'BatteryTel',
     'BatteryBQ40Z50Tel',
     'DiveTimeTel',
     'DroneTimeTel',
     'WaterTemperatureTel',
     'CPUTemperatureTel',
-    'CanisterTopTemperatureTel',
-    'CanisterBottomTemperatureTel',
-    'CanisterTopHumidityTel',
-    'CanisterBottomHumidityTel',
+    'CanisterTemperatureTel',
+    'CanisterHumidityTel',
     'VideoStorageSpaceTel',
     'DataStorageSpaceTel',
     'CalibrationStateTel',
     'TiltStabilizationTel',
     'IperfTel',
     'NStreamersTel',
     'TiltAngleTel',
     'DroneInfoTel',
     'ErrorFlagsTel',
     'ControlModeTel',
     'ThicknessGaugeTel',
     'CpProbeTel',
     'ConnectedClientsTel',
-    'GenericServoTel',
-    'MultibeamServoTel',
-    'GuestPortCurrentTel',
-    'CalibratedImuTel',
-    'Imu1Tel',
-    'Imu2Tel',
-    'MedusaSpectrometerDataTel',
     'SetOverlayParametersReq',
     'SetOverlayParametersRep',
     'GetOverlayParametersReq',
     'GetOverlayParametersRep',
     'SetCameraParametersReq',
     'SetCameraParametersRep',
     'GetCameraParametersReq',
@@ -328,43 +291,8 @@
     'SyncTimeRep',
     'PingReq',
     'PingRep',
     'SetThicknessGaugeParametersReq',
     'SetThicknessGaugeParametersRep',
     'ConnectClientReq',
     'ConnectClientRep',
-    'DisconnectClientReq',
-    'DisconnectClientRep',
-    'GetBatteryReq',
-    'GetBatteryRep',
-    'SetPubFrequencyReq',
-    'SetPubFrequencyRep',
-    'MotionInputCtrl',
-    'TiltVelocityCtrl',
-    'LightsCtrl',
-    'GuestportLightsCtrl',
-    'LaserCtrl',
-    'PilotGPSPositionCtrl',
-    'WatchdogCtrl',
-    'RecordCtrl',
-    'TakePictureCtrl',
-    'StartCalibrationCtrl',
-    'CancelCalibrationCtrl',
-    'FinishCalibrationCtrl',
-    'AutoHeadingCtrl',
-    'AutoDepthCtrl',
-    'AutoAltitudeCtrl',
-    'StationKeepingCtrl',
-    'WeatherVaningCtrl',
-    'ResetPositionCtrl',
-    'ResetOdometerCtrl',
-    'TiltStabilizationCtrl',
-    'WaterDensityCtrl',
-    'PingerConfigurationCtrl',
-    'SystemTimeCtrl',
-    'GripperCtrl',
-    'GenericServoCtrl',
-    'MultibeamServoCtrl',
-    'DeactivateGuestPortsCtrl',
-    'ActivateGuestPortsCtrl',
-    'RestartGuestPortsCtrl',
 )
```

### Comparing `blueye_protocol-2.2.1/blueye/protocol/types/control.py` & `blueye.protocol-3.0.0/blueye/protocol/types/control.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 __protobuf__ = proto.module(
     package='blueye.protocol',
     manifest={
         'MotionInputCtrl',
         'TiltVelocityCtrl',
         'LightsCtrl',
         'GuestportLightsCtrl',
-        'LaserCtrl',
         'PilotGPSPositionCtrl',
         'WatchdogCtrl',
         'RecordCtrl',
         'TakePictureCtrl',
         'StartCalibrationCtrl',
         'CancelCalibrationCtrl',
         'FinishCalibrationCtrl',
@@ -44,19 +43,14 @@
         'ResetPositionCtrl',
         'ResetOdometerCtrl',
         'TiltStabilizationCtrl',
         'WaterDensityCtrl',
         'PingerConfigurationCtrl',
         'SystemTimeCtrl',
         'GripperCtrl',
-        'GenericServoCtrl',
-        'MultibeamServoCtrl',
-        'DeactivateGuestPortsCtrl',
-        'ActivateGuestPortsCtrl',
-        'RestartGuestPortsCtrl',
     },
 )
 
 
 class MotionInputCtrl(proto.Message):
     r"""-
 
@@ -116,29 +110,14 @@
     """
 
     lights = proto.Field(proto.MESSAGE, number=1,
         message=message_formats.Lights,
     )
 
 
-class LaserCtrl(proto.Message):
-    r"""-
-
-    Issue a command to set the laser intensity.
-
-    Attributes:
-        laser (blueye.protocol.types.Laser):
-            Message with the desired laser intensity.
-    """
-
-    laser = proto.Field(proto.MESSAGE, number=1,
-        message=message_formats.Laser,
-    )
-
-
 class PilotGPSPositionCtrl(proto.Message):
     r"""-
 
     Issue a command with the GPS position of the pilot.
 
     Attributes:
         position (blueye.protocol.types.LatLongPosition):
@@ -295,24 +274,16 @@
     )
 
 
 class ResetPositionCtrl(proto.Message):
     r"""-
 
     Issue a command to reset the position estimate.
-
-    Attributes:
-        settings (blueye.protocol.types.ResetPositionSettings):
-            Reset settings.
     """
 
-    settings = proto.Field(proto.MESSAGE, number=1,
-        message=message_formats.ResetPositionSettings,
-    )
-
 
 class ResetOdometerCtrl(proto.Message):
     r"""-
 
     Issue a command to reset the odometer.
     """
 
@@ -389,68 +360,8 @@
     """
 
     gripper_velocities = proto.Field(proto.MESSAGE, number=1,
         message=message_formats.GripperVelocities,
     )
 
 
-class GenericServoCtrl(proto.Message):
-    r"""-
-
-    Issue a command to set a generic servo value.
-
-    Attributes:
-        servo (blueye.protocol.types.GenericServo):
-            Message with the desired servo value.
-    """
-
-    servo = proto.Field(proto.MESSAGE, number=1,
-        message=message_formats.GenericServo,
-    )
-
-
-class MultibeamServoCtrl(proto.Message):
-    r"""-
-
-    Issue a command to set multibeam servo angle.
-
-    Attributes:
-        servo (blueye.protocol.types.MultibeamServo):
-            Message with the desired servo angle.
-    """
-
-    servo = proto.Field(proto.MESSAGE, number=1,
-        message=message_formats.MultibeamServo,
-    )
-
-
-class DeactivateGuestPortsCtrl(proto.Message):
-    r"""-
-
-    Deactivate the guest port power
-    """
-
-
-class ActivateGuestPortsCtrl(proto.Message):
-    r"""-
-
-    Activated the guest port power
-    """
-
-
-class RestartGuestPortsCtrl(proto.Message):
-    r"""-
-
-    Restart the guest ports by turning power on and off
-
-    Attributes:
-        restart_info (blueye.protocol.types.GuestPortRestartInfo):
-            Message with information about how long to
-            keep the guest ports off.
-    """
-
-    restart_info = proto.Field(proto.MESSAGE, number=1,
-        message=message_formats.GuestPortRestartInfo,
-    )
-
-
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `blueye_protocol-2.2.1/blueye/protocol/types/message_formats.py` & `blueye.protocol-3.0.0/blueye/protocol/types/message_formats.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,34 +21,30 @@
 from google.protobuf import any_pb2 as gp_any  # type: ignore
 from google.protobuf import timestamp_pb2 as timestamp  # type: ignore
 
 
 __protobuf__ = proto.module(
     package='blueye.protocol',
     manifest={
-        'HeadingSource',
-        'ResetCoordinateSource',
         'Model',
         'PressureSensorType',
         'Resolution',
         'Framerate',
         'Camera',
         'TemperatureUnit',
         'LogoType',
         'DepthUnit',
         'ThicknessUnit',
         'FontSize',
         'GuestPortDeviceID',
-        'GuestPortNumber',
         'NavigationSensorID',
         'GuestPortError',
         'BinlogRecord',
         'MotionInput',
         'Lights',
-        'Laser',
         'LatLongPosition',
         'ConnectionDuration',
         'AutoHeadingState',
         'AutoDepthState',
         'AutoAltitudeState',
         'StationKeepingState',
         'WeatherVaningState',
@@ -67,18 +63,16 @@
         'CanisterHumidity',
         'Battery',
         'BatteryBQ40Z50',
         'Attitude',
         'Altitude',
         'ForwardDistance',
         'PositionEstimate',
-        'ResetPositionSettings',
         'Depth',
         'Reference',
-        'ControlForce',
         'ControllerHealth',
         'DiveTime',
         'RecordOn',
         'StorageSpace',
         'CalibrationState',
         'IperfStatus',
         'NStreamers',
@@ -89,44 +83,20 @@
         'CameraParameters',
         'OverlayParameters',
         'NavigationSensorStatus',
         'GuestPortDevice',
         'GuestPortDeviceList',
         'GuestPortConnectorInfo',
         'GuestPortInfo',
-        'GuestPortRestartInfo',
         'ThicknessGauge',
         'CpProbe',
-        'GenericServo',
-        'MultibeamServo',
-        'GuestPortCurrent',
-        'Vector3',
-        'Imu',
-        'MedusaSpectrometerData',
     },
 )
 
 
-class HeadingSource(proto.Enum):
-    r"""-
-
-    Heading source used during reset of the position estimate.
-    """
-    HEADING_SOURCE_UNSPECIFIED = 0
-    HEADING_SOURCE_DRONE_COMPASS = 1
-    HEADING_SOURCE_MANUAL_INPUT = 2
-
-
-class ResetCoordinateSource(proto.Enum):
-    r""""""
-    RESET_COORDINATE_SOURCE_UNSPECIFIED = 0
-    RESET_COORDINATE_SOURCE_DEVICE_GPS = 1
-    RESET_COORDINATE_SOURCE_MANUAL = 2
-
-
 class Model(proto.Enum):
     r"""-
 
     Drone models produced by Blueye
     """
     MODEL_UNSPECIFIED = 0
     MODEL_PIONEER = 1
@@ -254,34 +224,14 @@
     GUEST_PORT_DEVICE_ID_BLUE_ROBOTICS_PING360_SONAR = 15
     GUEST_PORT_DEVICE_ID_TRITECH_GEMINI_720IM = 16
     GUEST_PORT_DEVICE_ID_BLUEYE_LIGHT_PAIR = 17
     GUEST_PORT_DEVICE_ID_TRITECH_GEMINI_MICRON = 18
     GUEST_PORT_DEVICE_ID_OCEAN_TOOLS_DIGICP = 19
     GUEST_PORT_DEVICE_ID_TRITECH_GEMINI_720IK = 20
     GUEST_PORT_DEVICE_ID_NORTEK_NUCLEUS_1000 = 21
-    GUEST_PORT_DEVICE_ID_BLUEYE_GENERIC_SERVO = 22
-    GUEST_PORT_DEVICE_ID_BLUEYE_MULTIBEAM_SERVO = 23
-    GUEST_PORT_DEVICE_ID_BLUE_ROBOTICS_DETACHABLE_NEWTON = 24
-    GUEST_PORT_DEVICE_ID_INSITU_AQUA_TROLL_500 = 25
-    GUEST_PORT_DEVICE_ID_MEDUSA_RADIOMETRICS_MS100 = 26
-    GUEST_PORT_DEVICE_ID_LASER_TOOLS_SEA_BEAM = 27
-    GUEST_PORT_DEVICE_ID_SPOT_X_LASER_SCALERS = 28
-    GUEST_PORT_DEVICE_ID_BLUEPRINT_SUBSEA_OCULUS_M1200D = 29
-    GUEST_PORT_DEVICE_ID_BLUEPRINT_SUBSEA_OCULUS_M3000D = 30
-
-
-class GuestPortNumber(proto.Enum):
-    r"""-
-
-    GuestPort number.
-    """
-    GUEST_PORT_NUMBER_UNSPECIFIED = 0
-    GUEST_PORT_NUMBER_PORT_1 = 1
-    GUEST_PORT_NUMBER_PORT_2 = 2
-    GUEST_PORT_NUMBER_PORT_3 = 3
 
 
 class NavigationSensorID(proto.Enum):
     r"""-
 
     List of navigation sensors that can be used by the position observer
     """
@@ -389,56 +339,39 @@
         value (float):
             Light intensity (0..1)
     """
 
     value = proto.Field(proto.FLOAT, number=1)
 
 
-class Laser(proto.Message):
-    r"""-
-
-    Laser message used to represent the intensity of connected laser.
-
-    If the laser does not support dimming but only on and off, a value
-    of 0 turns the laser off, and any value above 0 turns the laser on.
-
-    Attributes:
-        value (float):
-            Laser intensity, any value above 0 turns the
-            laser on (0..1)
-    """
-
-    value = proto.Field(proto.FLOAT, number=1)
-
-
 class LatLongPosition(proto.Message):
     r"""-
 
-    Latitude and longitude position in WGS 84 decimal degrees format.
+    Latitude and longitude position in WGS 84 format.
 
     Attributes:
         latitude (float):
-            Latitude (°)
+            Latitude
         longitude (float):
-            Longitude (°)
+            Longitude
     """
 
     latitude = proto.Field(proto.DOUBLE, number=1)
 
     longitude = proto.Field(proto.DOUBLE, number=2)
 
 
 class ConnectionDuration(proto.Message):
     r"""-
 
     Connection duration of a remote client.
 
     Attributes:
         value (int):
-            time since connected to drone (s)
+            time in seconds since connected to drone
     """
 
     value = proto.Field(proto.INT32, number=1)
 
 
 class AutoHeadingState(proto.Message):
     r"""-
@@ -642,19 +575,19 @@
 
     Camera recording state.
 
     Attributes:
         main_is_recording (bool):
             If the main camera is recording
         main_seconds (int):
-            Main record time (s)
+            Main record time in seconds
         guestport_is_recording (bool):
             If the guestport camera is recording
         guestport_seconds (int):
-            Guestport record time (s)
+            Guestport record time in seconds
     """
 
     main_is_recording = proto.Field(proto.BOOL, number=1)
 
     main_seconds = proto.Field(proto.INT32, number=2)
 
     guestport_is_recording = proto.Field(proto.BOOL, number=3)
@@ -668,15 +601,15 @@
     Water density.
 
     Used to specify the water density the drone is operating in, to
     achieve more accruate depth measurements.
 
     Attributes:
         value (float):
-            Salinity (kg/l)
+            Salinity in kg/l
     """
 
     value = proto.Field(proto.FLOAT, number=1)
 
 
 class PingerConfiguration(proto.Message):
     r"""-
@@ -704,75 +637,81 @@
     r"""-
 
     Water temperature measured by the drone's combined depth and
     temperature sensor.
 
     Attributes:
         value (float):
-            Water temperature (°C)
+            Water temperature in °C
     """
 
     value = proto.Field(proto.FLOAT, number=1)
 
 
 class CPUTemperature(proto.Message):
     r"""-
 
     CPU temperature.
 
     Attributes:
         value (float):
-            CPU temperature (°C)
+            CPU temperature in °C
     """
 
     value = proto.Field(proto.FLOAT, number=1)
 
 
 class CanisterTemperature(proto.Message):
     r"""-
 
     Canister temperature.
 
-    Temperature measured in the top or bottom canister of the drone.
+    Temperature measured in the top and bottom canister of the drone.
 
     Attributes:
-        temperature (float):
-            Temperature (°C)
+        top (float):
+            Temperature in °C
+        bottom (float):
+            Temperature in °C
     """
 
-    temperature = proto.Field(proto.FLOAT, number=3)
+    top = proto.Field(proto.FLOAT, number=1)
+
+    bottom = proto.Field(proto.FLOAT, number=2)
 
 
 class CanisterHumidity(proto.Message):
     r"""-
 
     Canister humidity.
 
-    Humidity measured in the top or bottom canister of the drone.
-
     Attributes:
-        humidity (float):
-            Air humidity (%)
+        top (float):
+            Air humidity in %
+        bottom (float):
+            Air humidity in %
     """
 
-    humidity = proto.Field(proto.FLOAT, number=3)
+    top = proto.Field(proto.FLOAT, number=1)
+
+    bottom = proto.Field(proto.FLOAT, number=2)
 
 
 class Battery(proto.Message):
     r"""-
 
     Essential battery information.
 
     Attributes:
         voltage (float):
-            Battery voltage (V)
+            Battery voltage in V
         level (float):
             Battery level (0..1)
         temperature (float):
-            Battery temperature (°C)
+            Battery temperature in °C
     """
 
     voltage = proto.Field(proto.FLOAT, number=1)
 
     level = proto.Field(proto.FLOAT, number=2)
 
     temperature = proto.Field(proto.FLOAT, number=3)
@@ -790,43 +729,44 @@
         voltage (blueye.protocol.types.BatteryBQ40Z50.Voltage):
             Voltage of the battery cells
         temperature (blueye.protocol.types.BatteryBQ40Z50.Temperature):
             Temperature of the battery cells
         status (blueye.protocol.types.BatteryBQ40Z50.BatteryStatus):
             Battery status flags
         current (float):
-            Current (A)
+            Current in A
         average_current (float):
-            Average current (A)
+            Average current in A
         relative_state_of_charge (float):
             Relative state of charge (0..1)
         absolute_state_of_charge (float):
             Absolute state of charge (0..1)
         remaining_capacity (float):
-            Remaining capacity (Ah)
+            Remaining capacity in Ah
         full_charge_capacity (float):
-            Full charge capacity (Ah)
+            Full charge capacity in Ah
         runtime_to_empty (int):
-            Runtime to empty (s)
+            Runtime to empty in seconds
         average_time_to_empty (int):
-            Average time to empty (s)
+            Average time to empty in seconds
         average_time_to_full (int):
-            Average time to full (s)
+            Average time to full in seconds
         time_to_full_at_current_rate (int):
-            Time to fully charged at current rate (s)
+            Time to fully charged at current rate in
+            seconds
         time_to_empty_at_current_rate (int):
-            Time to empty at current rate (s)
+            Time to empty at current rate in seconds
         charging_current (float):
-            Charging current (A)
+            Charging current in A
         charging_voltage (float):
-            Charging voltage (V)
+            Charging voltage in V
         cycle_count (int):
             Number of charging cycles
         design_capacity (float):
-            Design capacity (Ah)
+            Design capacity in Ah
         manufacture_date (google.protobuf.timestamp_pb2.Timestamp):
             Manufacture date
         serial_number (int):
             Serial number
         manufacturer_name (str):
             Manufacturer name
         device_name (str):
@@ -837,23 +777,23 @@
     class Voltage(proto.Message):
         r"""-
 
         Battery voltage levels.
 
         Attributes:
             total (float):
-                Battery pack voltage level (V)
+                Battery pack voltage level in V
             cell_1 (float):
-                Cell 1 voltage level (V)
+                Cell 1 voltage level in V
             cell_2 (float):
-                Vell 2 voltage level (V)
+                Vell 2 voltage level in V
             cell_3 (float):
-                Cell 3 voltage level (V)
+                Cell 3 voltage level in V
             cell_4 (float):
-                Cell 4 voltage level (V)
+                Cell 4 voltage level in V
         """
 
         total = proto.Field(proto.FLOAT, number=1)
 
         cell_1 = proto.Field(proto.FLOAT, number=2)
 
         cell_2 = proto.Field(proto.FLOAT, number=3)
@@ -865,23 +805,23 @@
     class Temperature(proto.Message):
         r"""-
 
         Battery temperature.
 
         Attributes:
             average (float):
-                Average temperature accross cells (°C)
+                Average temperature accross cells in °C
             cell_1 (float):
-                Cell 1 temperature (°C)
+                Cell 1 temperature in °C
             cell_2 (float):
-                Cell 2 temperature (°C)
+                Cell 2 temperature in °C
             cell_3 (float):
-                Cell 3 temperature (°C)
+                Cell 3 temperature in °C
             cell_4 (float):
-                Cell 4 temperature (°C)
+                Cell 4 temperature in °C
         """
 
         average = proto.Field(proto.FLOAT, number=1)
 
         cell_1 = proto.Field(proto.FLOAT, number=2)
 
         cell_2 = proto.Field(proto.FLOAT, number=3)
@@ -1016,19 +956,19 @@
 class Attitude(proto.Message):
     r"""-
 
     The attitude of the drone.
 
     Attributes:
         roll (float):
-            Roll angle (-180°..180°)
+            Roll angle (-180..180)
         pitch (float):
-            Pitch angle (-180°..180°)
+            Pitch angle (-180..180)
         yaw (float):
-            Yaw angle (-180°..180°)
+            Yaw angle (-180..180)
     """
 
     roll = proto.Field(proto.FLOAT, number=1)
 
     pitch = proto.Field(proto.FLOAT, number=2)
 
     yaw = proto.Field(proto.FLOAT, number=3)
@@ -1037,15 +977,15 @@
 class Altitude(proto.Message):
     r"""-
 
     Drone altitude over seabed, typically obtained from a DVL.
 
     Attributes:
         value (float):
-            Drone altitude over seabed (m)
+            Drone altitude over seabed in m
         is_valid (bool):
             If altitude is valid or not
     """
 
     value = proto.Field(proto.FLOAT, number=1)
 
     is_valid = proto.Field(proto.BOOL, number=2)
@@ -1055,15 +995,15 @@
     r"""-
 
     Distance to an object infront of the drone, typically obtained from
     an 1D pinger.
 
     Attributes:
         value (float):
-            Distance in front of drone (m)
+            Distance in front of drone in m
         is_valid (bool):
             If distance reading is valid or not
     """
 
     value = proto.Field(proto.FLOAT, number=1)
 
     is_valid = proto.Field(proto.BOOL, number=2)
@@ -1125,83 +1065,49 @@
     )
 
     navigation_sensors = proto.RepeatedField(proto.MESSAGE, number=11,
         message='NavigationSensorStatus',
     )
 
 
-class ResetPositionSettings(proto.Message):
-    r"""-
-
-    ResetPositionSettings used during reset of the position estimate.
-
-    Attributes:
-        heading_source_during_reset (blueye.protocol.types.HeadingSource):
-            Option to use the drone compass or due North
-            as heading during reset
-        manual_heading (float):
-            Heading in degrees (0-359)
-        reset_coordinate_source (blueye.protocol.types.ResetCoordinateSource):
-            Option to use the device GPS or a manual
-            coordinate.
-        reset_coordinate (blueye.protocol.types.LatLongPosition):
-            Reset coordinate in decimal degrees
-    """
-
-    heading_source_during_reset = proto.Field(proto.ENUM, number=1,
-        enum='HeadingSource',
-    )
-
-    manual_heading = proto.Field(proto.FLOAT, number=2)
-
-    reset_coordinate_source = proto.Field(proto.ENUM, number=3,
-        enum='ResetCoordinateSource',
-    )
-
-    reset_coordinate = proto.Field(proto.MESSAGE, number=4,
-        message='LatLongPosition',
-    )
-
-
 class Depth(proto.Message):
     r"""-
 
     Water depth of the drone.
 
     Attributes:
         value (float):
-            Drone depth below surface (m)
+            Drone depth below surface in m
     """
 
     value = proto.Field(proto.FLOAT, number=1)
 
 
 class Reference(proto.Message):
     r"""-
 
     Reference for the control system. Note that the internal heading
     referece is not relative to North. Use (ControlHealth.heading_error
     + pose.yaw) instead.
 
     Attributes:
         surge (float):
-            Reference from joystick surge input (0..1)
+            Reference from joystick surge input
         sway (float):
-            Reference from joystick sway input (0..1)
+            Reference from joystick sway input
         heave (float):
-            Reference from joystick heave input (0..1)
+            Reference from joystick heave input
         yaw (float):
-            Reference from joystick yaw input (0..1)
+            Reference from joystick yaw input
         depth (float):
-            Reference drone depth below surface (m)
+            Reference drone depth below surface in m
         heading (float):
-            Reference used in auto heading mode, gyro
-            based (°)
+            Reference used in auto heading mode
         altitude (float):
-            Reference used in auto altitude mode (m)
+            Reference used in auto altitude mode
     """
 
     surge = proto.Field(proto.FLOAT, number=1)
 
     sway = proto.Field(proto.FLOAT, number=2)
 
     heave = proto.Field(proto.FLOAT, number=3)
@@ -1211,53 +1117,27 @@
     depth = proto.Field(proto.FLOAT, number=5)
 
     heading = proto.Field(proto.FLOAT, number=6)
 
     altitude = proto.Field(proto.FLOAT, number=7)
 
 
-class ControlForce(proto.Message):
-    r"""-
-
-    Control Force is used for showing the requested control force in
-    each direction in Newtons.
-
-    Attributes:
-        surge (float):
-            Force in surge (N)
-        sway (float):
-            Force in sway (N)
-        heave (float):
-            Force in heave (N)
-        yaw (float):
-            Moment in yaw (Nm)
-    """
-
-    surge = proto.Field(proto.FLOAT, number=1)
-
-    sway = proto.Field(proto.FLOAT, number=2)
-
-    heave = proto.Field(proto.FLOAT, number=3)
-
-    yaw = proto.Field(proto.FLOAT, number=4)
-
-
 class ControllerHealth(proto.Message):
     r"""-
 
     Controller health is used for showing the state of the controller
     with an relative error and load from 0 to 1.
 
     Attributes:
         depth_error (float):
-            Depth error in meters (m)
+            Depth error in meters
         depth_health (float):
             Depth controller load (0..1)
         heading_error (float):
-            Heading error in degrees (°)
+            Heading error in degrees
         heading_health (float):
             Heading controller load (0..1)
     """
 
     depth_error = proto.Field(proto.FLOAT, number=1)
 
     depth_health = proto.Field(proto.FLOAT, number=2)
@@ -1304,17 +1184,17 @@
 class StorageSpace(proto.Message):
     r"""-
 
     Storage space.
 
     Attributes:
         total_space (int):
-            Total bytes of storage space (B)
+            Total bytes of storage space
         free_space (int):
-            Available bytes of storage space (B)
+            Available bytes of storage space
     """
 
     total_space = proto.Field(proto.INT64, number=1)
 
     free_space = proto.Field(proto.INT64, number=2)
 
 
@@ -1382,19 +1262,19 @@
 class IperfStatus(proto.Message):
     r"""-
 
     Connection speed between drone and Surface Unit.
 
     Attributes:
         sent (float):
-            Transfer rate from drone to Surface Unit
-            (Mbit/s)
+            Transfer rate from drone to Surface Unit in
+            Mbit/s
         received (float):
-            Transfer rate from Surface Unit to drone
-            (Mbit/s)
+            Transfer rate from Surface Unit to drone in
+            Mbit/s
     """
 
     sent = proto.Field(proto.FLOAT, number=1)
 
     received = proto.Field(proto.FLOAT, number=2)
 
 
@@ -1420,29 +1300,29 @@
 class TiltAngle(proto.Message):
     r"""-
 
     Angle of tilt camera in degrees.
 
     Attributes:
         value (float):
-            Tilt angle (°)
+            Tilt angle in degrees °
     """
 
     value = proto.Field(proto.FLOAT, number=1)
 
 
 class TiltVelocity(proto.Message):
     r"""-
 
     Relative velocity of tilt
 
     Attributes:
         value (float):
-            Relative angular velocity of tilt (-1..1),
-            negative means down and positive means up
+            Relative angular velocity of tilt (-1 to 1,
+            negative means down and positive means up)
     """
 
     value = proto.Field(proto.FLOAT, number=1)
 
 
 class DroneInfo(proto.Message):
     r"""-
@@ -1589,22 +1469,14 @@
             BB serial number error
         ds_serial (bool):
             DS serial number error
         gp_current_read (bool):
             Error reading GP current
         gp_current (bool):
             Max GP current exceeded
-        gp1_bat_current (bool):
-            Max battery current exceeded on GP1
-        gp2_bat_current (bool):
-            Max battery current exceeded on GP2
-        gp3_bat_current (bool):
-            Max battery current exceeded on GP3
-        gp_20v_current (bool):
-            Max 20V current exceeded on GP
     """
 
     pmu_comm_ack = proto.Field(proto.BOOL, number=1)
 
     pmu_comm_stream = proto.Field(proto.BOOL, number=2)
 
     depth_read = proto.Field(proto.BOOL, number=3)
@@ -1675,43 +1547,36 @@
 
     ds_serial = proto.Field(proto.BOOL, number=36)
 
     gp_current_read = proto.Field(proto.BOOL, number=37)
 
     gp_current = proto.Field(proto.BOOL, number=38)
 
-    gp1_bat_current = proto.Field(proto.BOOL, number=39)
-
-    gp2_bat_current = proto.Field(proto.BOOL, number=40)
-
-    gp3_bat_current = proto.Field(proto.BOOL, number=41)
-
-    gp_20v_current = proto.Field(proto.BOOL, number=42)
-
 
 class CameraParameters(proto.Message):
     r"""-
 
     Camera parameters.
 
     Attributes:
         h264_bitrate (int):
-            Bitrate of the h264 stream (bit/sec)
+            Bitrate of the h264 stream
         mjpg_bitrate (int):
             Bitrate of the MJPG stream used for still
-            pictures (bit/sec)
+            pictures
         exposure (int):
-            Shutter speed (1/10000 \* s), -1 for automatic exposure
+            Shutter speed in 10000/th second (-1 for
+            automatic exposure)
         white_balance (int):
-            White balance temperature (2800..9300), -1
-            for automatic white balance
+            White balance temperature in range 2800..9300
+            (-1 for automatic white balance)
         hue (int):
-            Hue (-40..40), 0 as default
+            Hue in range -40..40 (0 as default)
         gain (float):
-            Iso gain (0..1)
+            Iso gain in range 0.0-1.0
         resolution (blueye.protocol.types.Resolution):
             Stream, recording and image resolution
         framerate (blueye.protocol.types.Framerate):
             Stream and recording framerate
         camera (blueye.protocol.types.Camera):
             Which camera the parameters belong to.
     """
@@ -1764,16 +1629,14 @@
             If date should be included
         distance_enabled (bool):
             If distance should be included
         altitude_enabled (bool):
             If altitude should be included
         cp_probe_enabled (bool):
             If cp-probe should be included
-        medusa_enabled (bool):
-            If medusa measurement should be included
         drone_location_enabled (bool):
             If the drone location coordinates should be
             included
         logo_type (blueye.protocol.types.LogoType):
             Which logo should be used
         depth_unit (blueye.protocol.types.DepthUnit):
             Which unit should be used for depth: Meter,
@@ -1781,30 +1644,32 @@
         temperature_unit (blueye.protocol.types.TemperatureUnit):
             Which unit should be used for temperature:
             Celcius or Fahrenheit
         thickness_unit (blueye.protocol.types.ThicknessUnit):
             Which unit should be used for thickness:
             Millimeters or Inches
         timezone_offset (int):
-            Timezone offset from UTC (min)
+            Timezone offset from UTC
         margin_width (int):
-            Horizontal margins of text elements (px)
+            Horizontal margins of text elements
         margin_height (int):
-            Vertical margins of text elements (px)
+            Vertical margins of text elements
         font_size (blueye.protocol.types.FontSize):
             Font size of text elements
         title (str):
             Optional title
         subtitle (str):
             Optional subtitle
         date_format (str):
             Posix strftime format string for time stamp
         shading (float):
-            Pixel intensity to subtract from text
-            background (0..1), 0: transparent, 1: black
+            -
+
+            Pixel intensity to subtract from text background (range is
+            0.0-1.0), (0 is transparent and 1 is black)
     """
 
     temperature_enabled = proto.Field(proto.BOOL, number=1)
 
     depth_enabled = proto.Field(proto.BOOL, number=2)
 
     heading_enabled = proto.Field(proto.BOOL, number=3)
@@ -1817,16 +1682,14 @@
 
     distance_enabled = proto.Field(proto.BOOL, number=20)
 
     altitude_enabled = proto.Field(proto.BOOL, number=21)
 
     cp_probe_enabled = proto.Field(proto.BOOL, number=22)
 
-    medusa_enabled = proto.Field(proto.BOOL, number=24)
-
     drone_location_enabled = proto.Field(proto.BOOL, number=23)
 
     logo_type = proto.Field(proto.ENUM, number=6,
         enum='LogoType',
     )
 
     depth_unit = proto.Field(proto.ENUM, number=7,
@@ -1890,15 +1753,15 @@
         manufacturer (str):
             Manufacturer name
         name (str):
             Device name
         serial_number (str):
             Serial number
         depth_rating (float):
-            Depth rating (m)
+            Depth rating in meters
         required_blunux_version (str):
             Required Blunux version (x.y.z)
     """
 
     device_id = proto.Field(proto.ENUM, number=1,
         enum='GuestPortDeviceID',
     )
@@ -1935,30 +1798,24 @@
     GuestPort connector information.
 
     Attributes:
         device_list (blueye.protocol.types.GuestPortDeviceList):
             List of devices on this connector
         error (blueye.protocol.types.GuestPortError):
             Guest port error
-        guest_port_number (blueye.protocol.types.GuestPortNumber):
-            Guest port the connector is connected to
     """
 
     device_list = proto.Field(proto.MESSAGE, number=1, oneof='connected_device',
         message='GuestPortDeviceList',
     )
 
     error = proto.Field(proto.ENUM, number=2, oneof='connected_device',
         enum='GuestPortError',
     )
 
-    guest_port_number = proto.Field(proto.ENUM, number=3,
-        enum='GuestPortNumber',
-    )
-
 
 class GuestPortInfo(proto.Message):
     r"""-
 
     GuestPort information.
 
     Attributes:
@@ -1979,40 +1836,27 @@
     )
 
     gp3 = proto.Field(proto.MESSAGE, number=3,
         message='GuestPortConnectorInfo',
     )
 
 
-class GuestPortRestartInfo(proto.Message):
-    r"""-
-
-    GuestPort restart information.
-
-    Attributes:
-        power_off_duration (float):
-            Duration to keep the guest ports off (s)
-    """
-
-    power_off_duration = proto.Field(proto.DOUBLE, number=1)
-
-
 class ThicknessGauge(proto.Message):
     r"""-
 
     Thickness measurement data from a Cygnus Thickness Gauge.
 
     Attributes:
         thickness_measurement (float):
             Thickness measurement of a steel plate
         echo_count (int):
             Indicating the quality of the reading when
             invalid (0-3)
         sound_velocity (int):
-            Speed of sound in the steel member (m/s)
+            Speed of sound in the steel member
         is_measurement_valid (bool):
             Indicating if the measurement is valid
     """
 
     thickness_measurement = proto.Field(proto.FLOAT, number=1)
 
     echo_count = proto.Field(proto.UINT32, number=2)
@@ -2025,171 +1869,18 @@
 class CpProbe(proto.Message):
     r"""-
 
     Reading from a Cathodic Protection Potential probe.
 
     Attributes:
         measurement (float):
-            Potential measurement (V)
+            Potential measurement in V
         is_measurement_valid (bool):
             Indicating if the measurement is valid
     """
 
     measurement = proto.Field(proto.FLOAT, number=1)
 
     is_measurement_valid = proto.Field(proto.BOOL, number=2)
 
 
-class GenericServo(proto.Message):
-    r"""-
-
-    Servo message used to represent the angle of the servo.
-
-    Attributes:
-        value (float):
-            Servo value (0..1)
-        guest_port_number (blueye.protocol.types.GuestPortNumber):
-            Guest port the servo is on
-    """
-
-    value = proto.Field(proto.FLOAT, number=1)
-
-    guest_port_number = proto.Field(proto.ENUM, number=2,
-        enum='GuestPortNumber',
-    )
-
-
-class MultibeamServo(proto.Message):
-    r"""-
-
-    Servo message used to represent the angle of the servo.
-
-    Attributes:
-        angle (float):
-            Servo degrees (-30..30)
-    """
-
-    angle = proto.Field(proto.FLOAT, number=1)
-
-
-class GuestPortCurrent(proto.Message):
-    r"""-
-
-    GuestPort current readings.
-
-    Attributes:
-        gp1_bat (float):
-            Current on GP1 battery voltage (A)
-        gp2_bat (float):
-            Current on GP2 battery voltage (A)
-        gp3_bat (float):
-            Current on GP3 battery voltage (A)
-        gp_20v (float):
-            Current on common 20V supply (A)
-    """
-
-    gp1_bat = proto.Field(proto.DOUBLE, number=1)
-
-    gp2_bat = proto.Field(proto.DOUBLE, number=2)
-
-    gp3_bat = proto.Field(proto.DOUBLE, number=3)
-
-    gp_20v = proto.Field(proto.DOUBLE, number=4)
-
-
-class Vector3(proto.Message):
-    r"""-
-
-    Vector with 3 elements
-
-    Attributes:
-        x (float):
-            x-component
-        y (float):
-            y-component
-        z (float):
-            z-component
-    """
-
-    x = proto.Field(proto.DOUBLE, number=1)
-
-    y = proto.Field(proto.DOUBLE, number=2)
-
-    z = proto.Field(proto.DOUBLE, number=3)
-
-
-class Imu(proto.Message):
-    r"""-
-
-    Imu data in drone body frame
-
-    x - forward y - right z - down
-
-    Attributes:
-        accelerometer (blueye.protocol.types.Vector3):
-            Acceleration (g)
-        gyroscope (blueye.protocol.types.Vector3):
-            Angular velocity (rad/s)
-        magnetometer (blueye.protocol.types.Vector3):
-            Magnetic field (μT)
-        temperature (float):
-            Temperature (°C)
-    """
-
-    accelerometer = proto.Field(proto.MESSAGE, number=1,
-        message='Vector3',
-    )
-
-    gyroscope = proto.Field(proto.MESSAGE, number=2,
-        message='Vector3',
-    )
-
-    magnetometer = proto.Field(proto.MESSAGE, number=3,
-        message='Vector3',
-    )
-
-    temperature = proto.Field(proto.FLOAT, number=4)
-
-
-class MedusaSpectrometerData(proto.Message):
-    r"""-
-
-    Medusa gamma ray sensor spectrometer data
-
-    Attributes:
-        drone_time (google.protobuf.timestamp_pb2.Timestamp):
-            Time stamp when the data is received
-        sensor_time (google.protobuf.timestamp_pb2.Timestamp):
-            Time stamp the sensor reports
-        realtime (float):
-            Time the sensor actually measured (s)
-        livetime (float):
-            Time the measurement took (s)
-        total (int):
-            Total counts inside the spectrum
-        countrate (int):
-            Counts per second inside the spectrum
-            (rounded)
-        cosmics (int):
-            Detected counts above the last channel
-    """
-
-    drone_time = proto.Field(proto.MESSAGE, number=6,
-        message=timestamp.Timestamp,
-    )
-
-    sensor_time = proto.Field(proto.MESSAGE, number=7,
-        message=timestamp.Timestamp,
-    )
-
-    realtime = proto.Field(proto.FLOAT, number=1)
-
-    livetime = proto.Field(proto.FLOAT, number=2)
-
-    total = proto.Field(proto.UINT32, number=3)
-
-    countrate = proto.Field(proto.UINT32, number=4)
-
-    cosmics = proto.Field(proto.UINT32, number=5)
-
-
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `blueye_protocol-2.2.1/blueye/protocol/types/req_rep.py` & `blueye.protocol-3.0.0/blueye/protocol/types/req_rep.py`

 * *Files 20% similar despite different names*

```diff
@@ -36,20 +36,14 @@
         'SyncTimeRep',
         'PingReq',
         'PingRep',
         'SetThicknessGaugeParametersReq',
         'SetThicknessGaugeParametersRep',
         'ConnectClientReq',
         'ConnectClientRep',
-        'DisconnectClientReq',
-        'DisconnectClientRep',
-        'GetBatteryReq',
-        'GetBatteryRep',
-        'SetPubFrequencyReq',
-        'SetPubFrequencyRep',
     },
 )
 
 
 class SetOverlayParametersReq(proto.Message):
     r"""-
 
@@ -253,96 +247,8 @@
     client_id_in_control = proto.Field(proto.UINT32, number=2)
 
     connected_clients = proto.RepeatedField(proto.MESSAGE, number=3,
         message=message_formats.ConnectedClient,
     )
 
 
-class DisconnectClientReq(proto.Message):
-    r"""-
-
-    Disconnect a client from the drone.
-
-    This request will remove the client from the list of connected
-    clients. It allows clients to disconnect instantly, without waiting
-    for a watchdog to clear the client in control, or promote a new
-    client to be in control.
-
-    Attributes:
-        client_id (int):
-            The assigned ID of the client to disconnect.
-    """
-
-    client_id = proto.Field(proto.UINT32, number=1)
-
-
-class DisconnectClientRep(proto.Message):
-    r"""-
-
-    Response after disconnecting a client from the drone.
-
-    Contains information about which clients are connected and in
-    control.
-
-    Attributes:
-        client_id_in_control (int):
-            The ID of the client in control of the drone.
-        connected_clients (Sequence[blueye.protocol.types.ConnectedClient]):
-            List of connected clients.
-    """
-
-    client_id_in_control = proto.Field(proto.UINT32, number=1)
-
-    connected_clients = proto.RepeatedField(proto.MESSAGE, number=2,
-        message=message_formats.ConnectedClient,
-    )
-
-
-class GetBatteryReq(proto.Message):
-    r"""Request essential battery information.
-    Can be used to instantly get battery information,
-    instead of having to wait for the BatteryTel message to be
-    received.
-    """
-
-
-class GetBatteryRep(proto.Message):
-    r"""Response with essential battery information.
-
-    Attributes:
-        battery (blueye.protocol.types.Battery):
-            Essential battery information.
-    """
-
-    battery = proto.Field(proto.MESSAGE, number=1,
-        message=message_formats.Battery,
-    )
-
-
-class SetPubFrequencyReq(proto.Message):
-    r"""Request to update the publish frequency
-
-    Attributes:
-        message_type (str):
-            Message name, f. ex. "AttitudeTel".
-        frequency (float):
-            Publish frequency (max 100 Hz).
-    """
-
-    message_type = proto.Field(proto.STRING, number=1)
-
-    frequency = proto.Field(proto.FLOAT, number=2)
-
-
-class SetPubFrequencyRep(proto.Message):
-    r"""Response aftrer updating publish frequency
-
-    Attributes:
-        success (bool):
-            True if message name valid and frequency
-            successfully updated.
-    """
-
-    success = proto.Field(proto.BOOL, number=1)
-
-
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `blueye_protocol-2.2.1/blueye/protocol/types/telemetry.py` & `blueye.protocol-3.0.0/blueye/protocol/types/telemetry.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,51 +26,40 @@
     manifest={
         'AttitudeTel',
         'AltitudeTel',
         'ForwardDistanceTel',
         'PositionEstimateTel',
         'DepthTel',
         'ReferenceTel',
-        'ControlForceTel',
         'ControllerHealthTel',
         'LightsTel',
         'GuestPortLightsTel',
-        'LaserTel',
         'PilotGPSPositionTel',
         'RecordStateTel',
         'BatteryTel',
         'BatteryBQ40Z50Tel',
         'DiveTimeTel',
         'DroneTimeTel',
         'WaterTemperatureTel',
         'CPUTemperatureTel',
-        'CanisterTopTemperatureTel',
-        'CanisterBottomTemperatureTel',
-        'CanisterTopHumidityTel',
-        'CanisterBottomHumidityTel',
+        'CanisterTemperatureTel',
+        'CanisterHumidityTel',
         'VideoStorageSpaceTel',
         'DataStorageSpaceTel',
         'CalibrationStateTel',
         'TiltStabilizationTel',
         'IperfTel',
         'NStreamersTel',
         'TiltAngleTel',
         'DroneInfoTel',
         'ErrorFlagsTel',
         'ControlModeTel',
         'ThicknessGaugeTel',
         'CpProbeTel',
         'ConnectedClientsTel',
-        'GenericServoTel',
-        'MultibeamServoTel',
-        'GuestPortCurrentTel',
-        'CalibratedImuTel',
-        'Imu1Tel',
-        'Imu2Tel',
-        'MedusaSpectrometerDataTel',
     },
 )
 
 
 class AttitudeTel(proto.Message):
     r"""-
 
@@ -149,85 +138,53 @@
     """
 
     reference = proto.Field(proto.MESSAGE, number=1,
         message=message_formats.Reference,
     )
 
 
-class ControlForceTel(proto.Message):
-    r"""
-
-    Attributes:
-        control_force (blueye.protocol.types.ControlForce):
-
-    """
-
-    control_force = proto.Field(proto.MESSAGE, number=1,
-        message=message_formats.ControlForce,
-    )
-
-
 class ControllerHealthTel(proto.Message):
     r"""
 
     Attributes:
         controller_health (blueye.protocol.types.ControllerHealth):
 
     """
 
     controller_health = proto.Field(proto.MESSAGE, number=1,
         message=message_formats.ControllerHealth,
     )
 
 
 class LightsTel(proto.Message):
-    r"""-
-
-    Receive the status of the main lights of the drone.
+    r"""
 
     Attributes:
         lights (blueye.protocol.types.Lights):
 
     """
 
     lights = proto.Field(proto.MESSAGE, number=1,
         message=message_formats.Lights,
     )
 
 
 class GuestPortLightsTel(proto.Message):
-    r"""-
-
-    Receive the status of any guest port lights connected to the drone.
+    r"""
 
     Attributes:
         lights (blueye.protocol.types.Lights):
 
     """
 
     lights = proto.Field(proto.MESSAGE, number=1,
         message=message_formats.Lights,
     )
 
 
-class LaserTel(proto.Message):
-    r"""-
-
-    Receive the status of any lasers connected to the drone.
-
-    Attributes:
-        laser (blueye.protocol.types.Laser):
-
-    """
-
-    laser = proto.Field(proto.MESSAGE, number=1,
-        message=message_formats.Laser,
-    )
-
-
 class PilotGPSPositionTel(proto.Message):
     r"""
 
     Attributes:
         position (blueye.protocol.types.LatLongPosition):
 
     """
@@ -247,33 +204,32 @@
 
     record_state = proto.Field(proto.MESSAGE, number=1,
         message=message_formats.RecordState,
     )
 
 
 class BatteryTel(proto.Message):
-    r"""Receive essential information about the battery status.
+    r"""
 
     Attributes:
         battery (blueye.protocol.types.Battery):
-            Essential battery information.
+
     """
 
     battery = proto.Field(proto.MESSAGE, number=1,
         message=message_formats.Battery,
     )
 
 
 class BatteryBQ40Z50Tel(proto.Message):
-    r"""Receive detailed information about a battery using the
-    BQ40Z50 battery management system.
+    r"""
 
     Attributes:
         battery (blueye.protocol.types.BatteryBQ40Z50):
-            Detailed battery information.
+
     """
 
     battery = proto.Field(proto.MESSAGE, number=1,
         message=message_formats.BatteryBQ40Z50,
     )
 
 
@@ -332,59 +288,33 @@
     """
 
     temperature = proto.Field(proto.MESSAGE, number=1,
         message=message_formats.CPUTemperature,
     )
 
 
-class CanisterTopTemperatureTel(proto.Message):
-    r"""Receive temperature information from the top canister.
+class CanisterTemperatureTel(proto.Message):
+    r"""
 
     Attributes:
         temperature (blueye.protocol.types.CanisterTemperature):
-            Temperature information.
-    """
-
-    temperature = proto.Field(proto.MESSAGE, number=1,
-        message=message_formats.CanisterTemperature,
-    )
-
 
-class CanisterBottomTemperatureTel(proto.Message):
-    r"""Receive temperature information from the bottom canister.
-
-    Attributes:
-        temperature (blueye.protocol.types.CanisterTemperature):
-            Temperature information.
     """
 
     temperature = proto.Field(proto.MESSAGE, number=1,
         message=message_formats.CanisterTemperature,
     )
 
 
-class CanisterTopHumidityTel(proto.Message):
-    r"""Receive humidity information from the top canister.
+class CanisterHumidityTel(proto.Message):
+    r"""
 
     Attributes:
         humidity (blueye.protocol.types.CanisterHumidity):
-            Humidity information
-    """
-
-    humidity = proto.Field(proto.MESSAGE, number=1,
-        message=message_formats.CanisterHumidity,
-    )
 
-
-class CanisterBottomHumidityTel(proto.Message):
-    r"""Receive humidity information from the bottom canister.
-
-    Attributes:
-        humidity (blueye.protocol.types.CanisterHumidity):
-            Humidity information
     """
 
     humidity = proto.Field(proto.MESSAGE, number=1,
         message=message_formats.CanisterHumidity,
     )
 
 
@@ -568,113 +498,8 @@
     client_id_in_control = proto.Field(proto.UINT32, number=1)
 
     connected_clients = proto.RepeatedField(proto.MESSAGE, number=2,
         message=message_formats.ConnectedClient,
     )
 
 
-class GenericServoTel(proto.Message):
-    r"""-
-
-    State of a generic servo
-
-    Attributes:
-        servo (blueye.protocol.types.GenericServo):
-            Servo state
-    """
-
-    servo = proto.Field(proto.MESSAGE, number=1,
-        message=message_formats.GenericServo,
-    )
-
-
-class MultibeamServoTel(proto.Message):
-    r"""-
-
-    State of the servo installed in the multibeam
-
-    Attributes:
-        servo (blueye.protocol.types.MultibeamServo):
-            Multibeam servo state
-    """
-
-    servo = proto.Field(proto.MESSAGE, number=1,
-        message=message_formats.MultibeamServo,
-    )
-
-
-class GuestPortCurrentTel(proto.Message):
-    r"""-
-
-    GuestPort current readings
-
-    Attributes:
-        current (blueye.protocol.types.GuestPortCurrent):
-
-    """
-
-    current = proto.Field(proto.MESSAGE, number=1,
-        message=message_formats.GuestPortCurrent,
-    )
-
-
-class CalibratedImuTel(proto.Message):
-    r"""-
-
-    Calibrated IMU data
-
-    Attributes:
-        imu (blueye.protocol.types.Imu):
-
-    """
-
-    imu = proto.Field(proto.MESSAGE, number=1,
-        message=message_formats.Imu,
-    )
-
-
-class Imu1Tel(proto.Message):
-    r"""-
-
-    Raw IMU data from IMU 1
-
-    Attributes:
-        imu (blueye.protocol.types.Imu):
-
-    """
-
-    imu = proto.Field(proto.MESSAGE, number=1,
-        message=message_formats.Imu,
-    )
-
-
-class Imu2Tel(proto.Message):
-    r"""-
-
-    Raw IMU data from IMU 2
-
-    Attributes:
-        imu (blueye.protocol.types.Imu):
-
-    """
-
-    imu = proto.Field(proto.MESSAGE, number=1,
-        message=message_formats.Imu,
-    )
-
-
-class MedusaSpectrometerDataTel(proto.Message):
-    r"""-
-
-    Medusa gamma ray sensor spectrometer data
-
-    Attributes:
-        data (blueye.protocol.types.MedusaSpectrometerData):
-
-    """
-
-    data = proto.Field(proto.MESSAGE, number=1,
-        message=message_formats.MedusaSpectrometerData,
-    )
-
-
 __all__ = tuple(sorted(__protobuf__.manifest))
```

