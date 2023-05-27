# Comparing `tmp/python_omnilogic_local-0.2.1.tar.gz` & `tmp/python_omnilogic_local-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_omnilogic_local-0.2.1.tar", max compression
+gzip compressed data, was "python_omnilogic_local-0.3.0.tar", max compression
```

## Comparing `python_omnilogic_local-0.2.1.tar` & `python_omnilogic_local-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1696 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/__init__.py
--rwxr-xr-x   0        0        0    18696 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/api.py
--rwxr-xr-x   0        0        0     3633 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/cli.py
--rw-r--r--   0        0        0        0 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/models/__init__.py
--rw-r--r--   0        0        0       51 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/models/const.py
--rw-r--r--   0        0        0     1532 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/models/filter_diagnostics.py
--rw-r--r--   0        0        0      407 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/models/leadmessage.py
--rw-r--r--   0        0        0     7641 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/models/mspconfig.py
--rw-r--r--   0        0        0     8961 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/models/telemetry.py
--rw-r--r--   0        0        0     1476 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/models/util.py
--rw-r--r--   0        0        0     7903 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/protocol.py
--rw-r--r--   0        0        0     6119 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/types.py
--rw-r--r--   0        0        0      359 2023-05-26 20:08:10.418216 python_omnilogic_local-0.2.1/pyomnilogic_local/util.py
--rw-r--r--   0        0        0     5227 2023-05-26 20:08:11.310222 python_omnilogic_local-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1696 2023-05-27 01:45:17.337699 python_omnilogic_local-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 01:45:17.337699 python_omnilogic_local-0.3.0/pyomnilogic_local/__init__.py
+-rwxr-xr-x   0        0        0    20177 2023-05-27 01:45:17.337699 python_omnilogic_local-0.3.0/pyomnilogic_local/api.py
+-rwxr-xr-x   0        0        0     3931 2023-05-27 01:45:17.337699 python_omnilogic_local-0.3.0/pyomnilogic_local/cli.py
+-rw-r--r--   0        0        0        0 2023-05-27 01:45:17.337699 python_omnilogic_local-0.3.0/pyomnilogic_local/models/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-27 01:45:17.337699 python_omnilogic_local-0.3.0/pyomnilogic_local/models/const.py
+-rw-r--r--   0        0        0     1532 2023-05-27 01:45:17.337699 python_omnilogic_local-0.3.0/pyomnilogic_local/models/filter_diagnostics.py
+-rw-r--r--   0        0        0      407 2023-05-27 01:45:17.337699 python_omnilogic_local-0.3.0/pyomnilogic_local/models/leadmessage.py
+-rw-r--r--   0        0        0     7655 2023-05-27 01:45:17.337699 python_omnilogic_local-0.3.0/pyomnilogic_local/models/mspconfig.py
+-rw-r--r--   0        0        0     9510 2023-05-27 01:45:17.337699 python_omnilogic_local-0.3.0/pyomnilogic_local/models/telemetry.py
+-rw-r--r--   0        0        0     1476 2023-05-27 01:45:17.337699 python_omnilogic_local-0.3.0/pyomnilogic_local/models/util.py
+-rw-r--r--   0        0        0     7903 2023-05-27 01:45:17.337699 python_omnilogic_local-0.3.0/pyomnilogic_local/protocol.py
+-rw-r--r--   0        0        0     6304 2023-05-27 01:45:17.337699 python_omnilogic_local-0.3.0/pyomnilogic_local/types.py
+-rw-r--r--   0        0        0      359 2023-05-27 01:45:17.337699 python_omnilogic_local-0.3.0/pyomnilogic_local/util.py
+-rw-r--r--   0        0        0     5227 2023-05-27 01:45:18.277707 python_omnilogic_local-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.3.0/PKG-INFO
```

### Comparing `python_omnilogic_local-0.2.1/README.md` & `python_omnilogic_local-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.2.1/pyomnilogic_local/api.py` & `python_omnilogic_local-0.3.0/pyomnilogic_local/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,21 @@
 import xml.etree.ElementTree as ET
 
 from .models.filter_diagnostics import FilterDiagnostics
 from .models.mspconfig import MSPConfig
 from .models.telemetry import Telemetry
 from .models.util import to_pydantic
 from .protocol import OmniLogicProtocol
-from .types import ColorLogicBrightness, ColorLogicShow, ColorLogicSpeed, MessageType
+from .types import (
+    ColorLogicBrightness,
+    ColorLogicShow,
+    ColorLogicSpeed,
+    HeaterMode,
+    MessageType,
+)
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class OmniLogicAPI:
     def __init__(self, controller_ip: str, controller_port: int, response_timeout: float) -> None:
         self.controller_ip = controller_ip
@@ -161,14 +167,42 @@
         parameter = ET.SubElement(parameters_element, "Parameter", name="Temp", dataType="int", unit=unit, alias="Data")
         parameter.text = str(temperature)
 
         req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
 
         return await self.async_send_message(MessageType.SET_SOLAR_SET_POINT_COMMAND, req_body, False)
 
+    async def async_set_heater_mode(self, pool_id: int, equipment_id: int, mode: HeaterMode) -> None:
+        """async_set_heater_enable handles sending a SetHeaterEnable XML API call to the Hayward Omni pool controller
+
+        Args:
+            pool_id (int): The Pool/BodyOfWater ID that you want to address
+            equipment_id (int): Which equipment_id within that Pool to address
+            enabled (bool, optional): Turn the heater on (True) or off (False)
+
+        Returns:
+            _type_: _description_
+        """
+        body_element = ET.Element("Request", {"xmlns": "http://nextgen.hayward.com/api"})
+
+        name_element = ET.SubElement(body_element, "Name")
+        name_element.text = "SetUIHeaterModeCmd"
+
+        parameters_element = ET.SubElement(body_element, "Parameters")
+        parameter = ET.SubElement(parameters_element, "Parameter", name="poolId", dataType="int")
+        parameter.text = str(pool_id)
+        parameter = ET.SubElement(parameters_element, "Parameter", name="HeaterID", dataType="int", alias="EquipmentID")
+        parameter.text = str(equipment_id)
+        parameter = ET.SubElement(parameters_element, "Parameter", name="Mode", dataType="int", alias="Data")
+        parameter.text = str(mode.value)
+
+        req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
+
+        return await self.async_send_message(MessageType.SET_HEATER_MODE_COMMAND, req_body, False)
+
     async def async_set_heater_enable(self, pool_id: int, equipment_id: int, enabled: int | bool) -> None:
         """async_set_heater_enable handles sending a SetHeaterEnable XML API call to the Hayward Omni pool controller
 
         Args:
             pool_id (int): The Pool/BodyOfWater ID that you want to address
             equipment_id (int): Which equipment_id within that Pool to address
             enabled (bool, optional): Turn the heater on (True) or off (False)
```

### Comparing `python_omnilogic_local-0.2.1/pyomnilogic_local/cli.py` & `python_omnilogic_local-0.3.0/pyomnilogic_local/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,14 +68,19 @@
     # Turn the heater on and off
     # await omni.async_set_heater_enable(POOL_ID, HEATER_EQUIPMENT_ID, True)
     # await omni.async_set_heater_enable(POOL_ID, HEATER_EQUIPMENT_ID, False)
 
     # Adjust solar heater set point
     # await omni.async_set_solar_heater(POOL_ID, HEATER_EQUIPMENT_ID, 90, "F")
 
+    # Set the heater to heat/cool/auto
+    # await omni.async_set_heater_mode(POOL_ID, HEATER_EQUIPMENT_ID, HeaterMode.HEAT)
+    # await omni.async_set_heater_mode(POOL_ID, HEATER_EQUIPMENT_ID, HeaterMode.COOL)
+    # await omni.async_set_heater_mode(POOL_ID, HEATER_EQUIPMENT_ID, HeaterMode.AUTO)
+
     # Turn a variable speed pump on to 50%
     # await omni.async_set_filter_speed(POOL_ID, PUMP_EQUIPMENT_ID, 50)
     # Turn the pump off
     # await omni.async_set_equipment(POOL_ID, PUMP_EQUIPMENT_ID, False)
 
     # Activate a light show
     # await omni.async_set_light_show(
```

### Comparing `python_omnilogic_local-0.2.1/pyomnilogic_local/models/filter_diagnostics.py` & `python_omnilogic_local-0.3.0/pyomnilogic_local/models/filter_diagnostics.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.2.1/pyomnilogic_local/models/mspconfig.py` & `python_omnilogic_local-0.3.0/pyomnilogic_local/models/mspconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,25 +107,25 @@
 class MSPHeaterEquip(OmniBase):
     omni_type: OmniType = OmniType.HEATER_EQUIP
     type: Literal["PET_HEATER"] = Field(alias="Type")
     heater_type: HeaterType = Field(alias="Heater-Type")
     enabled: Literal["yes", "no"] = Field(alias="Enabled")
     min_filter_speed: int = Field(alias="Min-Speed-For-Operation")
     sensor_id: int = Field(alias="Sensor-System-Id")
-    supports_cooling: Literal["yes", "no"] = Field(alias="SupportsCooling")
+    supports_cooling: Literal["yes", "no"] | None = Field(alias="SupportsCooling")
 
 
 # This is the entry for the VirtualHeater, it does not use OmniBase because it has no name attribute
 class MSPVirtualHeater(OmniBase):
     _sub_devices = {"heater_equipment"}
 
     omni_type: OmniType = OmniType.VIRT_HEATER
     enabled: Literal["yes", "no"] = Field(alias="Enabled")
     set_point: int = Field(alias="Current-Set-Point")
-    solar_set_point: int = Field(alias="SolarSetPoint")
+    solar_set_point: int | None = Field(alias="SolarSetPoint")
     max_temp: int = Field(alias="Max-Settable-Water-Temp")
     min_temp: int = Field(alias="Min-Settable-Water-Temp")
     heater_equipment: list[MSPHeaterEquip] | None
 
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
```

### Comparing `python_omnilogic_local-0.2.1/pyomnilogic_local/models/telemetry.py` & `python_omnilogic_local-0.3.0/pyomnilogic_local/models/telemetry.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     ColorLogicBrightness,
     ColorLogicPowerState,
     ColorLogicShow,
     ColorLogicSpeed,
     FilterState,
     FilterValvePosition,
     FilterWhyOn,
+    HeaterMode,
     HeaterState,
     OmniType,
     PumpState,
     RelayState,
     ValveActuatorState,
 )
 
@@ -134,15 +135,15 @@
 
 class TelemetryVirtualHeater(BaseModel):
     omni_type: OmniType = OmniType.VIRT_HEATER
     system_id: int = Field(alias="@systemId")
     current_set_point: int = Field(alias="@Current-Set-Point")
     enabled: bool = Field(alias="@enable")
     solar_set_point: int = Field(alias="@SolarSetPoint")
-    mode: int = Field(alias="@Mode")
+    mode: HeaterMode = Field(alias="@Mode")
     silent_mode: int = Field(alias="@SilentMode")
     why_on: int = Field(alias="@whyHeaterIsOn")
 
 
 TelemetryType: TypeAlias = (
     TelemetryBackyard
     | TelemetryBoW
@@ -186,15 +187,21 @@
             ...
 
         @overload
         def xml_postprocessor(path: Any, key: Any, value: Any) -> tuple[Any, Any]:
             ...
 
         def xml_postprocessor(path: Any, key: Any, value: SupportsInt | Any) -> tuple[Any, SupportsInt | Any]:
-            """Post process XML to attempt to convert values to int."""
+            """Post process XML to attempt to convert values to int.
+
+            Pydantic can coerce values natively, but the Omni API returns values as strings of numbers (I.E. "2", "5", etc) and we need them
+            coerced into int enums.  Pydantic only seems to be able to handle one coercion, so it could coerce an int into an Enum, but it
+            cannot coerce a string into an int and then into the Enum. We help it out a little bit here by pre-emptively coercing any
+            string ints into an int, then pydantic handles the int to enum coercion if necessary.
+            """
             newvalue: SupportsInt | Any
 
             try:
                 newvalue = int(value)
             except (ValueError, TypeError):
                 newvalue = value
```

### Comparing `python_omnilogic_local-0.2.1/pyomnilogic_local/models/util.py` & `python_omnilogic_local-0.3.0/pyomnilogic_local/models/util.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.2.1/pyomnilogic_local/protocol.py` & `python_omnilogic_local-0.3.0/pyomnilogic_local/protocol.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.2.1/pyomnilogic_local/types.py` & `python_omnilogic_local-0.3.0/pyomnilogic_local/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class MessageType(Enum):
     XML_ACK = 0000
     REQUEST_CONFIGURATION = 1
     SET_FILTER_SPEED = 9
     SET_HEATER_COMMAND = 11
     REQUEST_LOG_CONFIG = 31
     SET_SOLAR_SET_POINT_COMMAND = 40
+    SET_HEATER_MODE_COMMAND = 42
     SET_HEATER_ENABLED = 147
     SET_EQUIPMENT = 164
     CREATE_SCHEDULE = 230
     DELETE_SCHEDULE = 231
     GET_TELEMETRY = 300
     GET_ALARM_LIST = 304
     SET_STANDALONE_LIGHT_SHOW = 308
@@ -220,14 +221,20 @@
     HEAT_PUMP = "HTR_HEAT_PUMP"
     SOLAR = "HTR_SOLAR"
     ELECTRIC = "HTR_ELECTRIC"
     GEOTHERMAL = "HTR_GEOTHERMAL"
     SMART = "HTR_SMART"
 
 
+class HeaterMode(PrettyEnum):
+    HEAT = 0
+    COOL = 1
+    AUTO = 2
+
+
 class PumpState(PrettyEnum):
     OFF = 0
     ON = 1
 
 
 class PumpType(str, PrettyEnum):
     SINGLE_SPEED = "PMP_SINGLE_SPEED"
@@ -273,21 +280,23 @@
 
 
 class SensorType(str, PrettyEnum):
     AIR_TEMP = "SENSOR_AIR_TEMP"
     SOLAR_TEMP = "SENSOR_SOLAR_TEMP"
     WATER_TEMP = "SENSOR_WATER_TEMP"
     FLOW = "SENSOR_FLOW"
+    EXT_INPUT = "SENSOR_EXT_INPUT"
 
 
 class SensorUnits(str, PrettyEnum):
     FAHRENHEIT = "UNITS_FAHRENHEIT"
     CELSIUS = "UNITS_CELSIUS"
     PPM = "UNITS_PPM"
     GRAMS_PER_LITER = "UNITS_GRAMS_PER_LITER"
     MILLIVOLTS = "UNITS_MILLIVOLTS"
     NO_UNITS = "UNITS_NO_UNITS"
+    ACTIVE_INACTIVE = "UNITS_ACTIVE_INACTIVE"
 
 
 class ValveActuatorState(PrettyEnum):
     OFF = 0
     ON = 1
```

### Comparing `python_omnilogic_local-0.2.1/pyproject.toml` & `python_omnilogic_local-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-omnilogic-local"
-version = "0.2.1"
+version = "0.3.0"
 description = "A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API"
 authors = ["cryptk <cryptk@users.noreply.github.com>", "djtimca", "garionphx"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cryptk/python-omnilogic-local"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `python_omnilogic_local-0.2.1/PKG-INFO` & `python_omnilogic_local-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-omnilogic-local
-Version: 0.2.1
+Version: 0.3.0
 Summary: A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API
 Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0
 Author: cryptk
 Author-email: cryptk@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.2.1 Summary: A
+Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.3.0 Summary: A
 library for local control of Hayward OmniHub/OmniLogic pool controllers using
 their local API Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0 Author: cryptk Author-email:
 cryptk@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
```

