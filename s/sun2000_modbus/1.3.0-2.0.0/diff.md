# Comparing `tmp/sun2000_modbus-1.3.0.tar.gz` & `tmp/sun2000_modbus-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sun2000_modbus-1.3.0.tar", last modified: Tue Sep 27 19:37:54 2022, max compression
+gzip compressed data, was "sun2000_modbus-2.0.0.tar", last modified: Sat Mar 11 22:24:50 2023, max compression
```

## Comparing `sun2000_modbus-1.3.0.tar` & `sun2000_modbus-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      231 2022-09-27 19:37:49.316949 sun2000_modbus-1.3.0/.editorconfig
--rw-r--r--   0        0        0       21 2022-09-27 19:37:49.316949 sun2000_modbus-1.3.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      570 2022-09-27 19:37:49.316949 sun2000_modbus-1.3.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     1136 2022-09-27 19:37:49.316949 sun2000_modbus-1.3.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      444 2022-09-27 19:37:49.316949 sun2000_modbus-1.3.0/.gitignore
--rw-r--r--   0        0        0      385 2022-09-27 19:37:49.316949 sun2000_modbus-1.3.0/LEGAL
--rw-r--r--   0        0        0     1073 2022-09-27 19:37:49.316949 sun2000_modbus-1.3.0/LICENSE
--rw-r--r--   0        0        0    31219 2022-09-27 19:37:49.316949 sun2000_modbus-1.3.0/README.md
--rw-r--r--   0        0        0      689 2022-09-27 19:37:49.316949 sun2000_modbus-1.3.0/pyproject.toml
--rw-r--r--   0        0        0       16 2022-09-27 19:37:49.316949 sun2000_modbus-1.3.0/requirements.txt
--rw-r--r--   0        0        0       96 2022-09-27 19:37:49.640947 sun2000_modbus-1.3.0/sun2000_modbus/__init__.py
--rw-r--r--   0        0        0     1144 2022-09-27 19:37:49.316949 sun2000_modbus-1.3.0/sun2000_modbus/datatypes.py
--rw-r--r--   0        0        0     3317 2022-09-27 19:37:49.316949 sun2000_modbus-1.3.0/sun2000_modbus/inverter.py
--rw-r--r--   0        0        0     2783 2022-09-27 19:37:49.316949 sun2000_modbus-1.3.0/sun2000_modbus/mappings.py
--rw-r--r--   0        0        0    27979 2022-09-27 19:37:49.316949 sun2000_modbus-1.3.0/sun2000_modbus/registers.py
--rw-r--r--   0        0        0        0 2022-09-27 19:37:49.316949 sun2000_modbus-1.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1512 2022-09-27 19:37:49.316949 sun2000_modbus-1.3.0/tests/sun2000mock.py
--rw-r--r--   0        0        0    12502 2022-09-27 19:37:49.316949 sun2000_modbus-1.3.0/tests/test_sun2000_modbus.py
--rw-r--r--   0        0        0    31829 1970-01-01 00:00:00.000000 sun2000_modbus-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      231 2023-03-11 22:24:41.607193 sun2000_modbus-2.0.0/.editorconfig
+-rw-r--r--   0        0        0       21 2023-03-11 22:24:41.607193 sun2000_modbus-2.0.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      570 2023-03-11 22:24:41.607193 sun2000_modbus-2.0.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1136 2023-03-11 22:24:41.607193 sun2000_modbus-2.0.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      444 2023-03-11 22:24:41.607193 sun2000_modbus-2.0.0/.gitignore
+-rw-r--r--   0        0        0      385 2023-03-11 22:24:41.607193 sun2000_modbus-2.0.0/LEGAL
+-rw-r--r--   0        0        0     1073 2023-03-11 22:24:41.607193 sun2000_modbus-2.0.0/LICENSE
+-rw-r--r--   0        0        0    31234 2023-03-11 22:24:41.611193 sun2000_modbus-2.0.0/README.md
+-rw-r--r--   0        0        0      689 2023-03-11 22:24:41.611193 sun2000_modbus-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-03-11 22:24:41.611193 sun2000_modbus-2.0.0/requirements.txt
+-rw-r--r--   0        0        0       96 2023-03-11 22:24:41.979195 sun2000_modbus-2.0.0/sun2000_modbus/__init__.py
+-rw-r--r--   0        0        0     1144 2023-03-11 22:24:41.611193 sun2000_modbus-2.0.0/sun2000_modbus/datatypes.py
+-rw-r--r--   0        0        0     3695 2023-03-11 22:24:41.611193 sun2000_modbus-2.0.0/sun2000_modbus/inverter.py
+-rw-r--r--   0        0        0     2783 2023-03-11 22:24:41.611193 sun2000_modbus-2.0.0/sun2000_modbus/mappings.py
+-rw-r--r--   0        0        0    27950 2023-03-11 22:24:41.611193 sun2000_modbus-2.0.0/sun2000_modbus/registers.py
+-rw-r--r--   0        0        0        0 2023-03-11 22:24:41.611193 sun2000_modbus-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     1512 2023-03-11 22:24:41.611193 sun2000_modbus-2.0.0/tests/sun2000mock.py
+-rw-r--r--   0        0        0    14153 2023-03-11 22:24:41.611193 sun2000_modbus-2.0.0/tests/test_sun2000_modbus.py
+-rw-r--r--   0        0        0    31844 1970-01-01 00:00:00.000000 sun2000_modbus-2.0.0/PKG-INFO
```

### Comparing `sun2000_modbus-1.3.0/.github/workflows/build.yml` & `sun2000_modbus-2.0.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `sun2000_modbus-1.3.0/.github/workflows/publish.yml` & `sun2000_modbus-2.0.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `sun2000_modbus-1.3.0/LICENSE` & `sun2000_modbus-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sun2000_modbus-1.3.0/README.md` & `sun2000_modbus-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # sun2000_modbus
 
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/olivergregorius/sun2000_modbus/Python%20Build?label=Python%20Build&logo=github)](https://github.com/olivergregorius/sun2000_modbus/actions/workflows/build.yml)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/olivergregorius/sun2000_modbus/build.yml?branch=main&label=Python%20Build&logo=github)](https://github.com/olivergregorius/sun2000_modbus/actions/workflows/build.yml)
 [![Python Versions](https://img.shields.io/pypi/pyversions/sun2000_modbus?label=Python)](https://pypi.org/project/sun2000_modbus/)
 [![GitHub](https://img.shields.io/github/license/olivergregorius/sun2000_modbus?label=License)](https://github.com/olivergregorius/sun2000_modbus/blob/HEAD/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/sun2000_modbus?label=PyPI)](https://pypi.org/project/sun2000_modbus/)
 
 ## Introduction
 
 This library is intended for reading Huawei Sun2000 inverter metrics from registers via Modbus TCP. Access to the Modbus interface is established by connecting
@@ -76,16 +76,16 @@
 |-----------------------------------------|------------------------|------|------|------------------------------------|
 | Model                                   | String                 |      |      |                                    |
 | SN                                      | String                 |      |      |                                    |
 | PN                                      | String                 |      |      |                                    |
 | ModelID                                 | Number                 | 1    |      |                                    |
 | NumberOfPVStrings                       | Number                 | 1    |      |                                    |
 | NumberOfMPPTrackers                     | Number                 | 1    |      |                                    |
-| RatedPower                              | Number                 | 1000 | kW   |                                    |
-| MaximumActivePower                      | Number                 | 1000 | kW   |                                    |
+| RatedPower                              | Number                 | 1    | W    |                                    |
+| MaximumActivePower                      | Number                 | 1    | W    |                                    |
 | MaximumApparentPower                    | Number                 | 1000 | kVA  |                                    |
 | MaximumReactivePowerFedToTheGrid        | Number                 | 1000 | kvar |                                    |
 | MaximumReactivePowerAbsorbedFromTheGrid | Number                 | 1000 | kvar |                                    |
 | State1                                  | Binary String/Bitfield |      |      |                                    |
 | State2                                  | Binary String/Bitfield |      |      |                                    |
 | State3                                  | Binary String/Bitfield |      |      |                                    |
 | Alarm1                                  | Binary String/Bitfield |      |      |                                    |
@@ -95,26 +95,26 @@
 | PV1Current                              | Number                 | 100  | A    |                                    |
 | PV2Voltage                              | Number                 | 10   | V    |                                    |
 | PV2Current                              | Number                 | 100  | A    |                                    |
 | PV3Voltage                              | Number                 | 10   | V    |                                    |
 | PV3Current                              | Number                 | 100  | A    |                                    |
 | PV4Voltage                              | Number                 | 10   | V    |                                    |
 | PV4Current                              | Number                 | 100  | A    |                                    |
-| InputPower                              | Number                 | 1000 | kW   |                                    |
+| InputPower                              | Number                 | 1    | W    |                                    |
 | LineVoltageBetweenPhasesAAndB           | Number                 | 10   | V    |                                    |
 | LineVoltageBetweenPhasesBAndC           | Number                 | 10   | V    |                                    |
 | LineVoltageBetweenPhasesCAndA           | Number                 | 10   | V    |                                    |
 | PhaseAVoltage                           | Number                 | 10   | V    |                                    |
 | PhaseBVoltage                           | Number                 | 10   | V    |                                    |
 | PhaseCVoltage                           | Number                 | 10   | V    |                                    |
 | PhaseACurrent                           | Number                 | 1000 | A    |                                    |
 | PhaseBCurrent                           | Number                 | 1000 | A    |                                    |
 | PhaseCCurrent                           | Number                 | 1000 | A    |                                    |
-| PeakActivePowerOfCurrentDay             | Number                 | 1000 | kW   |                                    |
-| ActivePower                             | Number                 | 1000 | kW   |                                    |
+| PeakActivePowerOfCurrentDay             | Number                 | 1    | W    |                                    |
+| ActivePower                             | Number                 | 1    | W    |                                    |
 | ReactivePower                           | Number                 | 1000 | kvar |                                    |
 | PowerFactor                             | Number                 | 1000 |      |                                    |
 | GridFrequency                           | Number                 | 100  | Hz   |                                    |
 | Efficiency                              | Number                 | 100  | %    |                                    |
 | InternalTemperature                     | Number                 | 10   | °C   |                                    |
 | InsulationResistance                    | Number                 | 1000 | MOhm |                                    |
 | DeviceStatus                            | Number                 | 1    |      |                                    |
@@ -179,25 +179,25 @@
 | ChargingCutoffCapacity                 | Number     | 10   | %       |                                    |
 | DischargeCutoffCapacity                | Number     | 10   | %       |                                    |
 | ForcedChargingAndDischargingPeriod     | Number     | 1    | minutes |                                    |
 | ChargeFromGridFunction                 | Number     | 1    |         |                                    |
 | GridChargeCutoffSOC                    | Number     | 10   | %       |                                    |
 | ForcibleChargeDischarge                | Number     | 1    |         | Write only, not available for read |
 | FixedChargingAndDischargingPeriods     | Bytestring |      |         |                                    |
-| PowerOfChargeFromGrid                  | Number     | 100  | kW      |                                    |
-| MaximumPowerOfChargeFromGrid           | Number     | 100  | kW      |                                    |
+| PowerOfChargeFromGrid                  | Number     | 0.1  | W       |                                    |
+| MaximumPowerOfChargeFromGrid           | Number     | 0.1  | W       |                                    |
 | ForcibleChargeDischargeSettingMode     | Number     | 1    |         |                                    |
-| ForcibleChargePower                    | Number     | 100  | kW      |                                    |
-| ForcibleDischargePower                 | Number     | 100  | kW      |                                    |
+| ForcibleChargePower                    | Number     | 0.1  | W       |                                    |
+| ForcibleDischargePower                 | Number     | 0.1  | W       |                                    |
 | TimeOfUseChargingAndDischargingPeriods | Bytestring |      |         |                                    |
 | ExcessPVEnergyUseInTOU                 | Number     | 1    |         |                                    |
 | ActivePowerControlMode                 | Number     | 1    |         |                                    |
 | MaximumFeedGridPowerInKW               | Number     | 1000 | kW      |                                    |
 | MaximumFeedGridPowerInPercentage       | Number     | 10   | %       |                                    |
-| MaximumChargeFromGridPower             | Number     | 100  | kW      |                                    |
+| MaximumChargeFromGridPower             | Number     | 0.1  | W       |                                    |
 | SwitchToOffGrid                        | Number     | 1    |         |                                    |
 | VoltageInIndependentOperation          | Number     | 1    |         |                                    |
 | Unit1ProductModel                      | Number     | 1    |         |                                    |
 | Unit1SN                                | String     |      |         |                                    |
 | Unit1No                                | Number     | 1    |         |                                    |
 | Unit1SoftwareVersion                   | String     |      |         |                                    |
 | Unit1DCDCVersion                       | String     |      |         |                                    |
@@ -234,75 +234,75 @@
 | Unit1BatteryPack1SN                    | String     |      |         |                                    |
 | Unit1BatteryPack1No                    | Number     | 1    |         |                                    |
 | Unit1BatteryPack1FirmwareVersion       | String     |      |         |                                    |
 | Unit1BatteryPack1WorkingStatus         | Number     | 1    |         |                                    |
 | Unit1BatteryPack1Voltage               | Number     | 10   | V       |                                    |
 | Unit1BatteryPack1Current               | Number     | 10   | A       |                                    |
 | Unit1BatteryPack1SOC                   | Number     | 10   | %       |                                    |
-| Unit1BatteryPack1ChargeDischargePower  | Number     | 100  | kW      |                                    |
+| Unit1BatteryPack1ChargeDischargePower  | Number     | 0.1  | W       |                                    |
 | Unit1BatteryPack1TotalCharge           | Number     | 100  | kWh     |                                    |
 | Unit1BatteryPack1TotalDischarge        | Number     | 100  | kWh     |                                    |
 | Unit1BatteryPack1MinimumTemperature    | Number     | 10   | °C      |                                    |
 | Unit1BatteryPack1MaximumTemperature    | Number     | 10   | °C      |                                    |
 | Unit1BatteryPack2SN                    | String     |      |         |                                    |
 | Unit1BatteryPack2No                    | Number     | 1    |         |                                    |
 | Unit1BatteryPack2FirmwareVersion       | String     |      |         |                                    |
 | Unit1BatteryPack2WorkingStatus         | Number     | 1    |         |                                    |
 | Unit1BatteryPack2Voltage               | Number     | 10   | V       |                                    |
 | Unit1BatteryPack2Current               | Number     | 10   | A       |                                    |
 | Unit1BatteryPack2SOC                   | Number     | 10   | %       |                                    |
-| Unit1BatteryPack2ChargeDischargePower  | Number     | 100  | kW      |                                    |
+| Unit1BatteryPack2ChargeDischargePower  | Number     | 0.1  | W       |                                    |
 | Unit1BatteryPack2TotalCharge           | Number     | 100  | kWh     |                                    |
 | Unit1BatteryPack2TotalDischarge        | Number     | 100  | kWh     |                                    |
 | Unit1BatteryPack2MinimumTemperature    | Number     | 10   | °C      |                                    |
 | Unit1BatteryPack2MaximumTemperature    | Number     | 10   | °C      |                                    |
 | Unit1BatteryPack3SN                    | String     |      |         |                                    |
 | Unit1BatteryPack3No                    | Number     | 1    |         |                                    |
 | Unit1BatteryPack3FirmwareVersion       | String     |      |         |                                    |
 | Unit1BatteryPack3WorkingStatus         | Number     | 1    |         |                                    |
 | Unit1BatteryPack3Voltage               | Number     | 10   | V       |                                    |
 | Unit1BatteryPack3Current               | Number     | 10   | A       |                                    |
 | Unit1BatteryPack3SOC                   | Number     | 10   | %       |                                    |
-| Unit1BatteryPack3ChargeDischargeStatus | Number     | 100  | kW      |                                    |
+| Unit1BatteryPack3ChargeDischargeStatus | Number     | 0.1  | W       |                                    |
 | Unit1BatteryPack3TotalCharge           | Number     | 100  | kWh     |                                    |
 | Unit1BatteryPack3TotalDischarge        | Number     | 100  | kWh     |                                    |
 | Unit1BatteryPack3MinimumTemperature    | Number     | 10   | °C      |                                    |
 | Unit1BatteryPack3MaximumTemperature    | Number     | 10   | °C      |                                    |
 | Unit2BatteryPack1SN                    | String     |      |         |                                    |
 | Unit2BatteryPack1No                    | Number     | 1    |         |                                    |
 | Unit2BatteryPack1FirmwareVersion       | String     |      |         |                                    |
 | Unit2BatteryPack1WorkingStatus         | Number     | 1    |         |                                    |
 | Unit2BatteryPack1Voltage               | Number     | 10   | V       |                                    |
 | Unit2BatteryPack1Current               | Number     | 10   | A       |                                    |
 | Unit2BatteryPack1SOC                   | Number     | 10   | %       |                                    |
-| Unit2BatteryPack1ChargeDischargePower  | Number     | 100  | kW      |                                    |
+| Unit2BatteryPack1ChargeDischargePower  | Number     | 0.1  | W       |                                    |
 | Unit2BatteryPack1TotalCharge           | Number     | 100  | kWh     |                                    |
 | Unit2BatteryPack1TotalDischarge        | Number     | 100  | kWh     |                                    |
 | Unit2BatteryPack1MinimumTemperature    | Number     | 10   | °C      |                                    |
 | Unit2BatteryPack1MaximumTemperature    | Number     | 10   | °C      |                                    |
 | Unit2BatteryPack2SN                    | String     |      |         |                                    |
 | Unit2BatteryPack2No                    | Number     | 1    |         |                                    |
 | Unit2BatteryPack2FirmwareVersion       | String     |      |         |                                    |
 | Unit2BatteryPack2WorkingStatus         | Number     | 1    |         |                                    |
 | Unit2BatteryPack2Voltage               | Number     | 10   | V       |                                    |
 | Unit2BatteryPack2Current               | Number     | 10   | A       |                                    |
 | Unit2BatteryPack2SOC                   | Number     | 10   | %       |                                    |
-| Unit2BatteryPack2ChargeDischargePower  | Number     | 100  | kW      |                                    |
+| Unit2BatteryPack2ChargeDischargePower  | Number     | 0.1  | W       |                                    |
 | Unit2BatteryPack2TotalCharge           | Number     | 100  | kWh     |                                    |
 | Unit2BatteryPack2TotalDischarge        | Number     | 100  | kWh     |                                    |
 | Unit2BatteryPack2MinimumTemperature    | Number     | 10   | °C      |                                    |
 | Unit2BatteryPack2MaximumTemperature    | Number     | 10   | °C      |                                    |
 | Unit2BatteryPack3SN                    | String     |      |         |                                    |
 | Unit2BatteryPack3No                    | Number     | 1    |         |                                    |
 | Unit2BatteryPack3FirmwareVersion       | String     |      |         |                                    |
 | Unit2BatteryPack3WorkingStatus         | Number     | 1    |         |                                    |
 | Unit2BatteryPack3Voltage               | Number     | 10   | V       |                                    |
 | Unit2BatteryPack3Current               | Number     | 10   | A       |                                    |
 | Unit2BatteryPack3SOC                   | Number     | 10   | %       |                                    |
-| Unit2BatteryPack3ChargeDischargePower  | Number     | 100  | kW      |                                    |
+| Unit2BatteryPack3ChargeDischargePower  | Number     | 0.1  | W       |                                    |
 | Unit2BatteryPack3TotalCharge           | Number     | 100  | kWh     |                                    |
 | Unit2BatteryPack3TotalDischarge        | Number     | 100  | kWh     |                                    |
 | Unit2BatteryPack3MinimumTemperature    | Number     | 10   | °C      |                                    |
 | Unit2BatteryPack3MaximumTemperature    | Number     | 10   | °C      |                                    |
 
 ### MeterEquipmentRegister
```

### Comparing `sun2000_modbus-1.3.0/pyproject.toml` & `sun2000_modbus-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sun2000_modbus-1.3.0/sun2000_modbus/datatypes.py` & `sun2000_modbus-2.0.0/sun2000_modbus/datatypes.py`

 * *Files identical despite different names*

### Comparing `sun2000_modbus-1.3.0/sun2000_modbus/inverter.py` & `sun2000_modbus-2.0.0/sun2000_modbus/inverter.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,42 +6,52 @@
 
 from . import datatypes
 
 logging.basicConfig(level=logging.INFO)
 
 
 class Sun2000:
-    def __init__(self, host, port=502, timeout=5, wait=2, unit=0):
+    def __init__(self, host, port=502, timeout=5, wait=2, unit=0): # some models need unit=1
         self.wait = wait
-        self.connected = False
         self.unit = unit
         self.inverter = ModbusTcpClient(host, port, timeout=timeout)
 
     def connect(self):
-        if not self.connected:
-            self.connected = self.inverter.connect()
+        if not self.isConnected():
+            self.inverter.connect()
             time.sleep(self.wait)
-            if self.connected:
+            if self.isConnected():
                 logging.info('Successfully connected to inverter')
+                return True
             else:
                 logging.error('Connection to inverter failed')
+                return False
+
+    def disconnect(self):
+        """Close the underlying tcp socket"""
+        # Some Sun2000 models with the SDongle WLAN-FE require the TCP connection to be closed
+        # as soon as possible. Leaving the TCP connection open for an extended time may cause 
+        # dongle reboots and/or FusionSolar portal updates to be delayed or even paused. 
+        self.inverter.close()
+
+    def isConnected(self):
+        """Check if underlying tcp socket is open"""
+        return self.inverter.is_socket_open()
 
     def read_raw_value(self, register):
-        if not self.connected:
+        if not self.isConnected():
             raise ValueError('Inverter is not connected')
 
         try:
             register_value = self.inverter.read_holding_registers(register.value.address, register.value.quantity, unit=self.unit)
             if type(register_value) == ModbusIOException:
                 logging.error("Inverter unit did not respond")
-                self.connected = False
                 raise register_value
         except ConnectionException:
             logging.error("A connection error occurred")
-            self.connected = False
             raise
 
         return datatypes.decode(register_value.encode()[1:], register.value.data_type)
 
     def read(self, register):
         raw_value = self.read_raw_value(register)
 
@@ -64,25 +74,22 @@
         if quantity == 0 and end_address == 0:
             raise ValueError("Either parameter quantity or end_address is required and must be greater than 0")
         if quantity != 0 and end_address != 0:
             raise ValueError("Only one parameter quantity or end_address should be defined")
         if end_address != 0 and end_address <= start_address:
             raise ValueError("end_address must be greater than start_address")
 
-        if not self.connected:
-            self.connected = False
+        if not self.isConnected():
             raise ValueError('Inverter is not connected')
 
         if end_address != 0:
             quantity = end_address - start_address + 1
         try:
             register_range_value = self.inverter.read_holding_registers(start_address, quantity, unit=self.unit)
             if type(register_range_value) == ModbusIOException:
                 logging.error("Inverter unit did not respond")
-                self.connected = False
                 raise register_range_value
         except ConnectionException:
             logging.error("A connection error occurred")
-            self.connected = False
             raise
 
         return datatypes.decode(register_range_value.encode()[1:], datatypes.DataType.MULTIDATA)
```

### Comparing `sun2000_modbus-1.3.0/sun2000_modbus/mappings.py` & `sun2000_modbus-2.0.0/sun2000_modbus/mappings.py`

 * *Files identical despite different names*

### Comparing `sun2000_modbus-1.3.0/sun2000_modbus/registers.py` & `sun2000_modbus-2.0.0/sun2000_modbus/registers.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     WO = "wo"
 
 
 class Register:
     address: int
     quantity: int
     data_type: datatypes.DataType
-    gain: int
+    gain: float
     unit: str
     access_type: AccessType
     mapping: dict
 
     def __init__(self, address, quantity, data_type, gain, unit, access_type, mapping):
         self.address = address
         self.quantity = quantity
@@ -32,16 +32,16 @@
 class InverterEquipmentRegister(Enum):
     Model = Register(30000, 15, datatypes.DataType.STRING, None, None, AccessType.RO, None)
     SN = Register(30015, 10, datatypes.DataType.STRING, None, None, AccessType.RO, None)
     PN = Register(30025, 10, datatypes.DataType.STRING, None, None, AccessType.RO, None)
     ModelID = Register(30070, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RO, None)
     NumberOfPVStrings = Register(30071, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RO, None)
     NumberOfMPPTrackers = Register(30072, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RO, None)
-    RatedPower = Register(30073, 2, datatypes.DataType.UINT32_BE, 1000, "kW", AccessType.RO, None)
-    MaximumActivePower = Register(30075, 2, datatypes.DataType.UINT32_BE, 1000, "kW", AccessType.RO, None)
+    RatedPower = Register(30073, 2, datatypes.DataType.UINT32_BE, 1, "W", AccessType.RO, None)
+    MaximumActivePower = Register(30075, 2, datatypes.DataType.UINT32_BE, 1, "W", AccessType.RO, None)
     MaximumApparentPower = Register(30077, 2, datatypes.DataType.UINT32_BE, 1000, "kVA", AccessType.RO, None)
     MaximumReactivePowerFedToTheGrid = Register(30079, 2, datatypes.DataType.INT32_BE, 1000, "kvar", AccessType.RO, None)
     MaximumReactivePowerAbsorbedFromTheGrid = Register(30081, 2, datatypes.DataType.INT32_BE, 1000, "kvar", AccessType.RO, None)
     State1 = Register(32000, 1, datatypes.DataType.BITFIELD16, None, None, AccessType.RO, None)
     State2 = Register(32002, 1, datatypes.DataType.BITFIELD16, None, None, AccessType.RO, None)
     State3 = Register(32003, 2, datatypes.DataType.BITFIELD32, None, None, AccessType.RO, None)
     Alarm1 = Register(32008, 1, datatypes.DataType.BITFIELD16, None, None, AccessType.RO, None)
@@ -51,26 +51,26 @@
     PV1Current = Register(32017, 1, datatypes.DataType.INT16_BE, 100, "A", AccessType.RO, None)
     PV2Voltage = Register(32018, 1, datatypes.DataType.INT16_BE, 10, "V", AccessType.RO, None)
     PV2Current = Register(32019, 1, datatypes.DataType.INT16_BE, 100, "A", AccessType.RO, None)
     PV3Voltage = Register(32020, 1, datatypes.DataType.INT16_BE, 10, "V", AccessType.RO, None)
     PV3Current = Register(32021, 1, datatypes.DataType.INT16_BE, 100, "A", AccessType.RO, None)
     PV4Voltage = Register(32022, 1, datatypes.DataType.INT16_BE, 10, "V", AccessType.RO, None)
     PV4Current = Register(32023, 1, datatypes.DataType.INT16_BE, 100, "A", AccessType.RO, None)
-    InputPower = Register(32064, 2, datatypes.DataType.INT32_BE, 1000, "kW", AccessType.RO, None)
+    InputPower = Register(32064, 2, datatypes.DataType.INT32_BE, 1, "W", AccessType.RO, None)
     LineVoltageBetweenPhasesAAndB = Register(32066, 1, datatypes.DataType.UINT16_BE, 10, "V", AccessType.RO, None)
     LineVoltageBetweenPhasesBAndC = Register(32067, 1, datatypes.DataType.UINT16_BE, 10, "V", AccessType.RO, None)
     LineVoltageBetweenPhasesCAndA = Register(32068, 1, datatypes.DataType.UINT16_BE, 10, "V", AccessType.RO, None)
     PhaseAVoltage = Register(32069, 1, datatypes.DataType.UINT16_BE, 10, "V", AccessType.RO, None)
     PhaseBVoltage = Register(32070, 1, datatypes.DataType.UINT16_BE, 10, "V", AccessType.RO, None)
     PhaseCVoltage = Register(32071, 1, datatypes.DataType.UINT16_BE, 10, "V", AccessType.RO, None)
     PhaseACurrent = Register(32072, 2, datatypes.DataType.INT32_BE, 1000, "A", AccessType.RO, None)
     PhaseBCurrent = Register(32074, 2, datatypes.DataType.INT32_BE, 1000, "A", AccessType.RO, None)
     PhaseCCurrent = Register(32076, 2, datatypes.DataType.INT32_BE, 1000, "A", AccessType.RO, None)
-    PeakActivePowerOfCurrentDay = Register(32078, 2, datatypes.DataType.INT32_BE, 1000, "kW", AccessType.RO, None)
-    ActivePower = Register(32080, 2, datatypes.DataType.INT32_BE, 1000, "kW", AccessType.RO, None)
+    PeakActivePowerOfCurrentDay = Register(32078, 2, datatypes.DataType.INT32_BE, 1, "W", AccessType.RO, None)
+    ActivePower = Register(32080, 2, datatypes.DataType.INT32_BE, 1, "W", AccessType.RO, None)
     ReactivePower = Register(32082, 2, datatypes.DataType.INT32_BE, 1000, "kvar", AccessType.RO, None)
     PowerFactor = Register(32084, 1, datatypes.DataType.INT16_BE, 1000, None, AccessType.RO, None)
     GridFrequency = Register(32085, 1, datatypes.DataType.UINT16_BE, 100, "Hz", AccessType.RO, None)
     Efficiency = Register(32086, 1, datatypes.DataType.UINT16_BE, 100, "%", AccessType.RO, None)
     InternalTemperature = Register(32087, 1, datatypes.DataType.INT16_BE, 10, "°C", AccessType.RO, None)
     InsulationResistance = Register(32088, 1, datatypes.DataType.UINT16_BE, 1000, "MOhm", AccessType.RO, None)
     DeviceStatus = Register(32089, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RO, mappings.DeviceStatus)
@@ -134,25 +134,25 @@
     ChargingCutoffCapacity = Register(47081, 1, datatypes.DataType.UINT16_BE, 10, "%", AccessType.RW, None)
     DischargeCutoffCapacity = Register(47082, 1, datatypes.DataType.UINT16_BE, 10, "%", AccessType.RW, None)
     ForcedChargingAndDischargingPeriod = Register(47083, 1, datatypes.DataType.UINT16_BE, 1, "minutes", AccessType.RW, None)
     ChargeFromGridFunction = Register(47087, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RW, mappings.ChargeFromGridFunction)
     GridChargeCutoffSOC = Register(47088, 1, datatypes.DataType.UINT16_BE, 10, "%", AccessType.RW, None)
     # ForcibleChargeDischarge = Register(47100, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.WO, mappings.ForcibleChargeDischarge) # disabled because not readable (AccessType.WO)
     FixedChargingAndDischargingPeriods = Register(47200, 41, datatypes.DataType.MULTIDATA, None, None, AccessType.RW, None)
-    PowerOfChargeFromGrid = Register(47242, 2, datatypes.DataType.INT32_BE, 100, "kW", AccessType.RW, None)
-    MaximumPowerOfChargeFromGrid = Register(47244, 2, datatypes.DataType.INT32_BE, 100, "kW", AccessType.RW, None)
+    PowerOfChargeFromGrid = Register(47242, 2, datatypes.DataType.INT32_BE, 0.1, "W", AccessType.RW, None)
+    MaximumPowerOfChargeFromGrid = Register(47244, 2, datatypes.DataType.INT32_BE, 0.1, "W", AccessType.RW, None)
     ForcibleChargeDischargeSettingMode = Register(47246, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RW, mappings.ForcibleChargeDischargeSettingMode)
-    ForcibleChargePower = Register(47247, 2, datatypes.DataType.INT32_BE, 100, "kW", AccessType.RW, None)
-    ForcibleDischargePower = Register(47249, 2, datatypes.DataType.INT32_BE, 100, "kW", AccessType.RW, None)
+    ForcibleChargePower = Register(47247, 2, datatypes.DataType.INT32_BE, 0.1, "W", AccessType.RW, None)
+    ForcibleDischargePower = Register(47249, 2, datatypes.DataType.INT32_BE, 0.1, "W", AccessType.RW, None)
     TimeOfUseChargingAndDischargingPeriods = Register(47255, 43, datatypes.DataType.MULTIDATA, None, None, AccessType.RW, None)
     ExcessPVEnergyUseInTOU = Register(47299, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RW, mappings.ExcessPVEnergyUseInTOU)
     ActivePowerControlMode = Register(47415, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RW, mappings.ActivePowerControlMode)
     MaximumFeedGridPowerInKW = Register(47416, 2, datatypes.DataType.INT32_BE, 1000, "kW", AccessType.RW, None)
     MaximumFeedGridPowerInPercentage = Register(47418, 1, datatypes.DataType.INT16_BE, 10, "%", AccessType.RW, None)
-    MaximumChargeFromGridPower = Register(47590, 2, datatypes.DataType.INT32_BE, 100, "kW", AccessType.RW, None)
+    MaximumChargeFromGridPower = Register(47590, 2, datatypes.DataType.INT32_BE, 0.1, "W", AccessType.RW, None)
     SwitchToOffGrid = Register(47604, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RW, mappings.SwitchToOffGrid)
     VoltageInIndependentOperation = Register(47605, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RW, mappings.VoltageIndependentOperation)
 
     # Unit 1
     Unit1ProductModel = Register(47000, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RW, mappings.ProductModel)
     Unit1SN = Register(37052, 10, datatypes.DataType.STRING, None, None, AccessType.RO, None)
     Unit1No = Register(47107, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RW, None)
@@ -195,85 +195,85 @@
     Unit1BatteryPack1SN = Register(38200, 10, datatypes.DataType.STRING, None, None, AccessType.RO, None)
     Unit1BatteryPack1No = Register(47750, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RW, None)
     Unit1BatteryPack1FirmwareVersion = Register(38210, 15, datatypes.DataType.STRING, None, None, AccessType.RO, None)
     Unit1BatteryPack1WorkingStatus = Register(38228, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RO, None)
     Unit1BatteryPack1Voltage = Register(38235, 1, datatypes.DataType.UINT16_BE, 10, "V", AccessType.RO, None)
     Unit1BatteryPack1Current = Register(38236, 1, datatypes.DataType.INT16_BE, 10, "A", AccessType.RO, None)
     Unit1BatteryPack1SOC = Register(38229, 1, datatypes.DataType.UINT16_BE, 10, "%", AccessType.RO, None)
-    Unit1BatteryPack1ChargeDischargePower = Register(38233, 2, datatypes.DataType.INT32_BE, 100, "kW", AccessType.RO, None)
+    Unit1BatteryPack1ChargeDischargePower = Register(38233, 2, datatypes.DataType.INT32_BE, 0.1, "W", AccessType.RO, None)
     Unit1BatteryPack1TotalCharge = Register(38238, 2, datatypes.DataType.INT32_BE, 100, "kWh", AccessType.RO, None)
     Unit1BatteryPack1TotalDischarge = Register(38240, 2, datatypes.DataType.INT32_BE, 100, "kWh", AccessType.RO, None)
     Unit1BatteryPack1MinimumTemperature = Register(38453, 1, datatypes.DataType.INT16_BE, 10, "°C", AccessType.RO, None)
     Unit1BatteryPack1MaximumTemperature = Register(38452, 1, datatypes.DataType.INT16_BE, 10, "°C", AccessType.RO, None)
 
     # Unit 1 BatteryPack 2
     Unit1BatteryPack2SN = Register(38242, 10, datatypes.DataType.STRING, None, None, AccessType.RO, None)
     Unit1BatteryPack2No = Register(47751, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RW, None)
     Unit1BatteryPack2FirmwareVersion = Register(38252, 15, datatypes.DataType.STRING, None, None, AccessType.RO, None)
     Unit1BatteryPack2WorkingStatus = Register(38270, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RO, None)
     Unit1BatteryPack2Voltage = Register(38277, 1, datatypes.DataType.UINT16_BE, 10, "V", AccessType.RO, None)
     Unit1BatteryPack2Current = Register(38278, 1, datatypes.DataType.INT16_BE, 10, "A", AccessType.RO, None)
     Unit1BatteryPack2SOC = Register(38271, 1, datatypes.DataType.UINT16_BE, 10, "%", AccessType.RO, None)
-    Unit1BatteryPack2ChargeDischargePower = Register(38275, 2, datatypes.DataType.INT32_BE, 100, "kW", AccessType.RO, None)
+    Unit1BatteryPack2ChargeDischargePower = Register(38275, 2, datatypes.DataType.INT32_BE, 0.1, "W", AccessType.RO, None)
     Unit1BatteryPack2TotalCharge = Register(38280, 2, datatypes.DataType.INT32_BE, 100, "kWh", AccessType.RO, None)
     Unit1BatteryPack2TotalDischarge = Register(38282, 2, datatypes.DataType.INT32_BE, 100, "kWh", AccessType.RO, None)
     Unit1BatteryPack2MinimumTemperature = Register(38455, 1, datatypes.DataType.INT16_BE, 10, "°C", AccessType.RO, None)
     Unit1BatteryPack2MaximumTemperature = Register(38454, 1, datatypes.DataType.INT16_BE, 10, "°C", AccessType.RO, None)
 
     # Unit 1 BatteryPack 3
     Unit1BatteryPack3SN = Register(38284, 10, datatypes.DataType.STRING, None, None, AccessType.RO, None)
     Unit1BatteryPack3No = Register(47752, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RW, None)
     Unit1BatteryPack3FirmwareVersion = Register(38294, 15, datatypes.DataType.STRING, None, None, AccessType.RO, None)
     Unit1BatteryPack3WorkingStatus = Register(38312, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RO, None)
     Unit1BatteryPack3Voltage = Register(38319, 1, datatypes.DataType.UINT16_BE, 10, "V", AccessType.RO, None)
     Unit1BatteryPack3Current = Register(38320, 1, datatypes.DataType.INT16_BE, 10, "A", AccessType.RO, None)
     Unit1BatteryPack3SOC = Register(38313, 1, datatypes.DataType.UINT16_BE, 10, "%", AccessType.RO, None)
-    Unit1BatteryPack3ChargeDischargeStatus = Register(38317, 2, datatypes.DataType.INT32_BE, 100, "kW", AccessType.RO, None)
+    Unit1BatteryPack3ChargeDischargeStatus = Register(38317, 2, datatypes.DataType.INT32_BE, 0.1, "W", AccessType.RO, None)
     Unit1BatteryPack3TotalCharge = Register(38322, 2, datatypes.DataType.INT32_BE, 100, "kWh", AccessType.RO, None)
     Unit1BatteryPack3TotalDischarge = Register(38324, 2, datatypes.DataType.INT32_BE, 100, "kWh", AccessType.RO, None)
     Unit1BatteryPack3MinimumTemperature = Register(38457, 1, datatypes.DataType.INT16_BE, 10, "°C", AccessType.RO, None)
     Unit1BatteryPack3MaximumTemperature = Register(38456, 1, datatypes.DataType.INT16_BE, 10, "°C", AccessType.RO, None)
 
     # Unit 2 BatteryPack 1
     Unit2BatteryPack1SN = Register(38326, 10, datatypes.DataType.STRING, None, None, AccessType.RO, None)
     Unit2BatteryPack1No = Register(47753, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RW, None)
     Unit2BatteryPack1FirmwareVersion = Register(38336, 15, datatypes.DataType.STRING, None, None, AccessType.RO, None)
     Unit2BatteryPack1WorkingStatus = Register(38354, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RO, None)
     Unit2BatteryPack1Voltage = Register(38361, 1, datatypes.DataType.UINT16_BE, 10, "V", AccessType.RO, None)
     Unit2BatteryPack1Current = Register(38362, 1, datatypes.DataType.INT16_BE, 10, "A", AccessType.RO, None)
     Unit2BatteryPack1SOC = Register(38355, 1, datatypes.DataType.UINT16_BE, 10, "%", AccessType.RO, None)
-    Unit2BatteryPack1ChargeDischargePower = Register(38359, 2, datatypes.DataType.INT32_BE, 100, "kW", AccessType.RO, None)
+    Unit2BatteryPack1ChargeDischargePower = Register(38359, 2, datatypes.DataType.INT32_BE, 0.1, "W", AccessType.RO, None)
     Unit2BatteryPack1TotalCharge = Register(38364, 2, datatypes.DataType.INT32_BE, 100, "kWh", AccessType.RO, None)
     Unit2BatteryPack1TotalDischarge = Register(38366, 2, datatypes.DataType.INT32_BE, 100, "kWh", AccessType.RO, None)
     Unit2BatteryPack1MinimumTemperature = Register(38459, 1, datatypes.DataType.INT16_BE, 10, "°C", AccessType.RO, None)
     Unit2BatteryPack1MaximumTemperature = Register(38458, 1, datatypes.DataType.INT16_BE, 10, "°C", AccessType.RO, None)
 
     # Unit 2 BatteryPack 2
     Unit2BatteryPack2SN = Register(38368, 10, datatypes.DataType.STRING, None, None, AccessType.RO, None)
     Unit2BatteryPack2No = Register(47754, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RW, None)
     Unit2BatteryPack2FirmwareVersion = Register(38378, 15, datatypes.DataType.STRING, None, None, AccessType.RO, None)
     Unit2BatteryPack2WorkingStatus = Register(38396, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RO, None)
     Unit2BatteryPack2Voltage = Register(38403, 1, datatypes.DataType.UINT16_BE, 10, "V", AccessType.RO, None)
     Unit2BatteryPack2Current = Register(38404, 1, datatypes.DataType.INT16_BE, 10, "A", AccessType.RO, None)
     Unit2BatteryPack2SOC = Register(38397, 1, datatypes.DataType.UINT16_BE, 10, "%", AccessType.RO, None)
-    Unit2BatteryPack2ChargeDischargePower = Register(38401, 2, datatypes.DataType.INT32_BE, 100, "kW", AccessType.RO, None)
+    Unit2BatteryPack2ChargeDischargePower = Register(38401, 2, datatypes.DataType.INT32_BE, 0.1, "W", AccessType.RO, None)
     Unit2BatteryPack2TotalCharge = Register(38406, 2, datatypes.DataType.INT32_BE, 100, "kWh", AccessType.RO, None)
     Unit2BatteryPack2TotalDischarge = Register(38408, 2, datatypes.DataType.INT32_BE, 100, "kWh", AccessType.RO, None)
     Unit2BatteryPack2MinimumTemperature = Register(38461, 1, datatypes.DataType.INT16_BE, 10, "°C", AccessType.RO, None)
     Unit2BatteryPack2MaximumTemperature = Register(38460, 1, datatypes.DataType.INT16_BE, 10, "°C", AccessType.RO, None)
 
     # Unit 2 BatteryPack 3
     Unit2BatteryPack3SN = Register(38410, 10, datatypes.DataType.STRING, None, None, AccessType.RO, None)
     Unit2BatteryPack3No = Register(47755, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RW, None)
     Unit2BatteryPack3FirmwareVersion = Register(38420, 15, datatypes.DataType.STRING, None, None, AccessType.RO, None)
     Unit2BatteryPack3WorkingStatus = Register(38438, 1, datatypes.DataType.UINT16_BE, 1, None, AccessType.RO, None)
     Unit2BatteryPack3Voltage = Register(38445, 1, datatypes.DataType.UINT16_BE, 10, "V", AccessType.RO, None)
     Unit2BatteryPack3Current = Register(38446, 1, datatypes.DataType.INT16_BE, 10, "A", AccessType.RO, None)
     Unit2BatteryPack3SOC = Register(38439, 1, datatypes.DataType.UINT16_BE, 10, "%", AccessType.RO, None)
-    Unit2BatteryPack3ChargeDischargePower = Register(38443, 2, datatypes.DataType.INT32_BE, 100, "kW", AccessType.RO, None)
+    Unit2BatteryPack3ChargeDischargePower = Register(38443, 2, datatypes.DataType.INT32_BE, 0.1, "W", AccessType.RO, None)
     Unit2BatteryPack3TotalCharge = Register(38448, 2, datatypes.DataType.INT32_BE, 100, "kWh", AccessType.RO, None)
     Unit2BatteryPack3TotalDischarge = Register(38450, 2, datatypes.DataType.INT32_BE, 100, "kWh", AccessType.RO, None)
     Unit2BatteryPack3MinimumTemperature = Register(38463, 1, datatypes.DataType.INT16_BE, 10, "°C", AccessType.RO, None)
     Unit2BatteryPack3MaximumTemperature = Register(38462, 1, datatypes.DataType.INT16_BE, 10, "°C", AccessType.RO, None)
 
 
 class MeterEquipmentRegister(Enum):
```

### Comparing `sun2000_modbus-1.3.0/tests/sun2000mock.py` & `sun2000_modbus-2.0.0/tests/sun2000mock.py`

 * *Files identical despite different names*

### Comparing `sun2000_modbus-1.3.0/tests/test_sun2000_modbus.py` & `sun2000_modbus-2.0.0/tests/test_sun2000_modbus.py`

 * *Files 11% similar despite different names*

```diff
@@ -60,187 +60,230 @@
 
     def test_init(self):
         self.assertEqual(self.test_inverter.inverter.host, '192.168.8.1')
         self.assertEqual(self.test_inverter.inverter.port, 123)
         self.assertEqual(self.test_inverter.inverter.timeout, 3)
         self.assertEqual(self.test_inverter.wait, 0)
         self.assertEqual(self.test_inverter.unit, 1)
-        self.assertEqual(self.test_inverter.connected, False)
+        self.assertEqual(self.test_inverter.isConnected(), False)
 
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_success
     )
+    @patch(
+        'pymodbus.client.sync.ModbusTcpClient.is_socket_open', sun2000mock.connect_success
+    )
     def test_connect_success(self):
         self.test_inverter.connect()
-        self.assertTrue(self.test_inverter.connected)
+        self.assertTrue(self.test_inverter.isConnected())
 
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_fail
     )
     def test_connect_fail(self):
         self.test_inverter.connect()
-        self.assertFalse(self.test_inverter.connected)
+        self.assertFalse(self.test_inverter.isConnected())
 
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_fail
     )
     def test_read_raw_value_string_from_disconnected_unit(self):
         self.test_inverter.connect()
         self.assertRaises(ValueError, self.test_inverter.read_raw_value, InverterEquipmentRegister.Model)
 
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.read_holding_registers', sun2000mock.mock_read_holding_registers_ModbusIOException
     )
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_success
     )
+    @patch(
+        'pymodbus.client.sync.ModbusTcpClient.is_socket_open', sun2000mock.connect_success
+    )
     def test_read_raw_value_string_from_unavailable_unit(self):
         self.test_inverter.connect()
         self.assertRaises(ModbusIOException, self.test_inverter.read_raw_value, InverterEquipmentRegister.Model)
-        self.assertFalse(self.test_inverter.connected)
 
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.read_holding_registers', sun2000mock.mock_read_holding_registers_ConnectionException
     )
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_success
     )
+    @patch(
+        'pymodbus.client.sync.ModbusTcpClient.is_socket_open', sun2000mock.connect_success
+    )
     def test_read_raw_value_string_connection_unexpectedly_closed(self):
         self.test_inverter.connect()
         self.assertRaises(ConnectionException, self.test_inverter.read_raw_value, InverterEquipmentRegister.Model)
-        self.assertFalse(self.test_inverter.connected)
 
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.read_holding_registers', sun2000mock.mock_read_holding_registers
     )
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_success
     )
+    @patch(
+        'pymodbus.client.sync.ModbusTcpClient.is_socket_open', sun2000mock.connect_success
+    )
     def test_read_raw_value_string(self):
         self.test_inverter.connect()
         result = self.test_inverter.read_raw_value(InverterEquipmentRegister.Model)
         self.assertEqual(result, 'SUN2000')
 
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.read_holding_registers', sun2000mock.mock_read_holding_registers
     )
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_success
     )
+    @patch(
+        'pymodbus.client.sync.ModbusTcpClient.is_socket_open', sun2000mock.connect_success
+    )
     def test_read_raw_value_uint16be(self):
         self.test_inverter.connect()
         result = self.test_inverter.read_raw_value(InverterEquipmentRegister.ModelID)
         self.assertEqual(result, 429)
 
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.read_holding_registers', sun2000mock.mock_read_holding_registers
     )
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_success
     )
+    @patch(
+        'pymodbus.client.sync.ModbusTcpClient.is_socket_open', sun2000mock.connect_success
+    )
     def test_read_raw_value_uint32be(self):
         self.test_inverter.connect()
         result = self.test_inverter.read_raw_value(InverterEquipmentRegister.RatedPower)
         self.assertEqual(result, 10000)
 
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.read_holding_registers', sun2000mock.mock_read_holding_registers
     )
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_success
     )
+    @patch(
+        'pymodbus.client.sync.ModbusTcpClient.is_socket_open', sun2000mock.connect_success
+    )
     def test_read_uint32be(self):
         self.test_inverter.connect()
         result = self.test_inverter.read(InverterEquipmentRegister.RatedPower)
-        self.assertEqual(result, 10.0)
+        self.assertEqual(result, 10000.0)
 
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.read_holding_registers', sun2000mock.mock_read_holding_registers
     )
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_success
     )
+    @patch(
+        'pymodbus.client.sync.ModbusTcpClient.is_socket_open', sun2000mock.connect_success
+    )
     def test_read_formatted_uint32be(self):
         self.test_inverter.connect()
         result = self.test_inverter.read_formatted(InverterEquipmentRegister.RatedPower)
-        self.assertEqual(result, "10.0 kW")
+        self.assertEqual(result, "10000.0 W")
 
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.read_holding_registers', sun2000mock.mock_read_holding_registers
     )
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_success
     )
+    @patch(
+        'pymodbus.client.sync.ModbusTcpClient.is_socket_open', sun2000mock.connect_success
+    )
     def test_read_raw_value_bitfield16(self):
         self.test_inverter.connect()
         result = self.test_inverter.read_raw_value(InverterEquipmentRegister.State1)
         self.assertEqual(result, '0000000000000110')
 
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.read_holding_registers', sun2000mock.mock_read_holding_registers
     )
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_success
     )
+    @patch(
+        'pymodbus.client.sync.ModbusTcpClient.is_socket_open', sun2000mock.connect_success
+    )
     def test_read_bitfield16(self):
         self.test_inverter.connect()
         result = self.test_inverter.read(InverterEquipmentRegister.State1)
         self.assertEqual(result, '0000000000000110')
 
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.read_holding_registers', sun2000mock.mock_read_holding_registers
     )
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_success
     )
+    @patch(
+        'pymodbus.client.sync.ModbusTcpClient.is_socket_open', sun2000mock.connect_success
+    )
     def test_read_formatted_bitfield16(self):
         self.test_inverter.connect()
         result = self.test_inverter.read_formatted(InverterEquipmentRegister.State1)
         self.assertEqual(result, '0000000000000110')
 
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.read_holding_registers', sun2000mock.mock_read_holding_registers
     )
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_success
     )
+    @patch(
+        'pymodbus.client.sync.ModbusTcpClient.is_socket_open', sun2000mock.connect_success
+    )
     def test_read_raw_value_with_mapping(self):
         self.test_inverter.connect()
         result = self.test_inverter.read_raw_value(InverterEquipmentRegister.DeviceStatus)
         self.assertEqual(result, 512)
 
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.read_holding_registers', sun2000mock.mock_read_holding_registers
     )
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_success
     )
+    @patch(
+        'pymodbus.client.sync.ModbusTcpClient.is_socket_open', sun2000mock.connect_success
+    )
     def test_read_formatted_with_mapping(self):
         self.test_inverter.connect()
         result = self.test_inverter.read_formatted(InverterEquipmentRegister.DeviceStatus)
         self.assertEqual(result, 'On-grid')
 
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.read_holding_registers', sun2000mock.mock_read_holding_registers
     )
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_success
     )
+    @patch(
+        'pymodbus.client.sync.ModbusTcpClient.is_socket_open', sun2000mock.connect_success
+    )
     def test_read_returns_float(self):
         self.test_inverter.connect()
         result = self.test_inverter.read(MeterEquipmentRegister.ActivePower)
         self.assertEqual(result, 1000.0)
         self.assertTrue(isinstance(result, float))
 
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.read_holding_registers', sun2000mock.mock_read_holding_registers
     )
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_success
     )
+    @patch(
+        'pymodbus.client.sync.ModbusTcpClient.is_socket_open', sun2000mock.connect_success
+    )
     def test_read_range_returns_range_of_register_values(self):
         self.test_inverter.connect()
         result = self.test_inverter.read_range(30000, quantity=35)
         self.assertEqual(result, b'SUN2000-10KTL-M1\x00\x00\x00\x00SUN2000-12HV2220100135\x00\x00\x00\x00\x00\x00\x00\x0001074311-002\x00\x00\x00\x00\x00\x00\x00\x00')
 
         result = self.test_inverter.read_range(30000, end_address=30034)
         self.assertEqual(result, b'SUN2000-10KTL-M1\x00\x00\x00\x00SUN2000-12HV2220100135\x00\x00\x00\x00\x00\x00\x00\x0001074311-002\x00\x00\x00\x00\x00\x00\x00\x00')
@@ -278,27 +321,31 @@
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_fail
     )
     def test_read_range_from_disconnected_unit(self):
         self.test_inverter.connect()
         self.assertRaises(ValueError, self.test_inverter.read_range, 30000, quantity=35)
 
     @patch(
-        'pymodbus.client.sync.ModbusTcpClient.read_holding_registers', sun2000mock.mock_read_holding_registers_ModbusIOException
+        'pymodbus.client.sync.ModbusTcpClient.read_holding_registers', sun2000mock.mock_read_holding_registers_ConnectionException
     )
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_success
     )
+    @patch(
+        'pymodbus.client.sync.ModbusTcpClient.is_socket_open', sun2000mock.connect_success
+    )
     def test_read_range_from_unavailable_unit(self):
         self.test_inverter.connect()
-        self.assertRaises(ModbusIOException, self.test_inverter.read_range, 30000, quantity=35)
-        self.assertFalse(self.test_inverter.connected)
+        self.assertRaises(ConnectionException, self.test_inverter.read_range, 30000, quantity=35)
 
     @patch(
-        'pymodbus.client.sync.ModbusTcpClient.read_holding_registers', sun2000mock.mock_read_holding_registers_ConnectionException
+        'pymodbus.client.sync.ModbusTcpClient.read_holding_registers', sun2000mock.mock_read_holding_registers_ModbusIOException
     )
     @patch(
         'pymodbus.client.sync.ModbusTcpClient.connect', sun2000mock.connect_success
     )
-    def test_read_range_from_unavailable_unit(self):
+    @patch(
+        'pymodbus.client.sync.ModbusTcpClient.is_socket_open', sun2000mock.connect_success
+    )
+    def test_read_range_from_unavailable_unit2(self):
         self.test_inverter.connect()
-        self.assertRaises(ConnectionException, self.test_inverter.read_range, 30000, quantity=35)
-        self.assertFalse(self.test_inverter.connected)
+        self.assertRaises(ModbusIOException, self.test_inverter.read_range, 30000, quantity=35)
```

### Comparing `sun2000_modbus-1.3.0/PKG-INFO` & `sun2000_modbus-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: sun2000_modbus
-Version: 1.3.0
+Version: 2.0.0
 Summary: Library for reading Huawei Sun2000 inverter metrics via Modbus TCP
 Keywords: sun2000,modbus,photovoltaic
 Author-email: Oliver Gregorius <oliver@gregorius.dev>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: pymodbus==2.5.3
 Project-URL: Source, https://github.com/olivergregorius/sun2000_modbus
 
 # sun2000_modbus
 
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/olivergregorius/sun2000_modbus/Python%20Build?label=Python%20Build&logo=github)](https://github.com/olivergregorius/sun2000_modbus/actions/workflows/build.yml)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/olivergregorius/sun2000_modbus/build.yml?branch=main&label=Python%20Build&logo=github)](https://github.com/olivergregorius/sun2000_modbus/actions/workflows/build.yml)
 [![Python Versions](https://img.shields.io/pypi/pyversions/sun2000_modbus?label=Python)](https://pypi.org/project/sun2000_modbus/)
 [![GitHub](https://img.shields.io/github/license/olivergregorius/sun2000_modbus?label=License)](https://github.com/olivergregorius/sun2000_modbus/blob/HEAD/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/sun2000_modbus?label=PyPI)](https://pypi.org/project/sun2000_modbus/)
 
 ## Introduction
 
 This library is intended for reading Huawei Sun2000 inverter metrics from registers via Modbus TCP. Access to the Modbus interface is established by connecting
@@ -91,16 +91,16 @@
 |-----------------------------------------|------------------------|------|------|------------------------------------|
 | Model                                   | String                 |      |      |                                    |
 | SN                                      | String                 |      |      |                                    |
 | PN                                      | String                 |      |      |                                    |
 | ModelID                                 | Number                 | 1    |      |                                    |
 | NumberOfPVStrings                       | Number                 | 1    |      |                                    |
 | NumberOfMPPTrackers                     | Number                 | 1    |      |                                    |
-| RatedPower                              | Number                 | 1000 | kW   |                                    |
-| MaximumActivePower                      | Number                 | 1000 | kW   |                                    |
+| RatedPower                              | Number                 | 1    | W    |                                    |
+| MaximumActivePower                      | Number                 | 1    | W    |                                    |
 | MaximumApparentPower                    | Number                 | 1000 | kVA  |                                    |
 | MaximumReactivePowerFedToTheGrid        | Number                 | 1000 | kvar |                                    |
 | MaximumReactivePowerAbsorbedFromTheGrid | Number                 | 1000 | kvar |                                    |
 | State1                                  | Binary String/Bitfield |      |      |                                    |
 | State2                                  | Binary String/Bitfield |      |      |                                    |
 | State3                                  | Binary String/Bitfield |      |      |                                    |
 | Alarm1                                  | Binary String/Bitfield |      |      |                                    |
@@ -110,26 +110,26 @@
 | PV1Current                              | Number                 | 100  | A    |                                    |
 | PV2Voltage                              | Number                 | 10   | V    |                                    |
 | PV2Current                              | Number                 | 100  | A    |                                    |
 | PV3Voltage                              | Number                 | 10   | V    |                                    |
 | PV3Current                              | Number                 | 100  | A    |                                    |
 | PV4Voltage                              | Number                 | 10   | V    |                                    |
 | PV4Current                              | Number                 | 100  | A    |                                    |
-| InputPower                              | Number                 | 1000 | kW   |                                    |
+| InputPower                              | Number                 | 1    | W    |                                    |
 | LineVoltageBetweenPhasesAAndB           | Number                 | 10   | V    |                                    |
 | LineVoltageBetweenPhasesBAndC           | Number                 | 10   | V    |                                    |
 | LineVoltageBetweenPhasesCAndA           | Number                 | 10   | V    |                                    |
 | PhaseAVoltage                           | Number                 | 10   | V    |                                    |
 | PhaseBVoltage                           | Number                 | 10   | V    |                                    |
 | PhaseCVoltage                           | Number                 | 10   | V    |                                    |
 | PhaseACurrent                           | Number                 | 1000 | A    |                                    |
 | PhaseBCurrent                           | Number                 | 1000 | A    |                                    |
 | PhaseCCurrent                           | Number                 | 1000 | A    |                                    |
-| PeakActivePowerOfCurrentDay             | Number                 | 1000 | kW   |                                    |
-| ActivePower                             | Number                 | 1000 | kW   |                                    |
+| PeakActivePowerOfCurrentDay             | Number                 | 1    | W    |                                    |
+| ActivePower                             | Number                 | 1    | W    |                                    |
 | ReactivePower                           | Number                 | 1000 | kvar |                                    |
 | PowerFactor                             | Number                 | 1000 |      |                                    |
 | GridFrequency                           | Number                 | 100  | Hz   |                                    |
 | Efficiency                              | Number                 | 100  | %    |                                    |
 | InternalTemperature                     | Number                 | 10   | °C   |                                    |
 | InsulationResistance                    | Number                 | 1000 | MOhm |                                    |
 | DeviceStatus                            | Number                 | 1    |      |                                    |
@@ -194,25 +194,25 @@
 | ChargingCutoffCapacity                 | Number     | 10   | %       |                                    |
 | DischargeCutoffCapacity                | Number     | 10   | %       |                                    |
 | ForcedChargingAndDischargingPeriod     | Number     | 1    | minutes |                                    |
 | ChargeFromGridFunction                 | Number     | 1    |         |                                    |
 | GridChargeCutoffSOC                    | Number     | 10   | %       |                                    |
 | ForcibleChargeDischarge                | Number     | 1    |         | Write only, not available for read |
 | FixedChargingAndDischargingPeriods     | Bytestring |      |         |                                    |
-| PowerOfChargeFromGrid                  | Number     | 100  | kW      |                                    |
-| MaximumPowerOfChargeFromGrid           | Number     | 100  | kW      |                                    |
+| PowerOfChargeFromGrid                  | Number     | 0.1  | W       |                                    |
+| MaximumPowerOfChargeFromGrid           | Number     | 0.1  | W       |                                    |
 | ForcibleChargeDischargeSettingMode     | Number     | 1    |         |                                    |
-| ForcibleChargePower                    | Number     | 100  | kW      |                                    |
-| ForcibleDischargePower                 | Number     | 100  | kW      |                                    |
+| ForcibleChargePower                    | Number     | 0.1  | W       |                                    |
+| ForcibleDischargePower                 | Number     | 0.1  | W       |                                    |
 | TimeOfUseChargingAndDischargingPeriods | Bytestring |      |         |                                    |
 | ExcessPVEnergyUseInTOU                 | Number     | 1    |         |                                    |
 | ActivePowerControlMode                 | Number     | 1    |         |                                    |
 | MaximumFeedGridPowerInKW               | Number     | 1000 | kW      |                                    |
 | MaximumFeedGridPowerInPercentage       | Number     | 10   | %       |                                    |
-| MaximumChargeFromGridPower             | Number     | 100  | kW      |                                    |
+| MaximumChargeFromGridPower             | Number     | 0.1  | W       |                                    |
 | SwitchToOffGrid                        | Number     | 1    |         |                                    |
 | VoltageInIndependentOperation          | Number     | 1    |         |                                    |
 | Unit1ProductModel                      | Number     | 1    |         |                                    |
 | Unit1SN                                | String     |      |         |                                    |
 | Unit1No                                | Number     | 1    |         |                                    |
 | Unit1SoftwareVersion                   | String     |      |         |                                    |
 | Unit1DCDCVersion                       | String     |      |         |                                    |
@@ -249,75 +249,75 @@
 | Unit1BatteryPack1SN                    | String     |      |         |                                    |
 | Unit1BatteryPack1No                    | Number     | 1    |         |                                    |
 | Unit1BatteryPack1FirmwareVersion       | String     |      |         |                                    |
 | Unit1BatteryPack1WorkingStatus         | Number     | 1    |         |                                    |
 | Unit1BatteryPack1Voltage               | Number     | 10   | V       |                                    |
 | Unit1BatteryPack1Current               | Number     | 10   | A       |                                    |
 | Unit1BatteryPack1SOC                   | Number     | 10   | %       |                                    |
-| Unit1BatteryPack1ChargeDischargePower  | Number     | 100  | kW      |                                    |
+| Unit1BatteryPack1ChargeDischargePower  | Number     | 0.1  | W       |                                    |
 | Unit1BatteryPack1TotalCharge           | Number     | 100  | kWh     |                                    |
 | Unit1BatteryPack1TotalDischarge        | Number     | 100  | kWh     |                                    |
 | Unit1BatteryPack1MinimumTemperature    | Number     | 10   | °C      |                                    |
 | Unit1BatteryPack1MaximumTemperature    | Number     | 10   | °C      |                                    |
 | Unit1BatteryPack2SN                    | String     |      |         |                                    |
 | Unit1BatteryPack2No                    | Number     | 1    |         |                                    |
 | Unit1BatteryPack2FirmwareVersion       | String     |      |         |                                    |
 | Unit1BatteryPack2WorkingStatus         | Number     | 1    |         |                                    |
 | Unit1BatteryPack2Voltage               | Number     | 10   | V       |                                    |
 | Unit1BatteryPack2Current               | Number     | 10   | A       |                                    |
 | Unit1BatteryPack2SOC                   | Number     | 10   | %       |                                    |
-| Unit1BatteryPack2ChargeDischargePower  | Number     | 100  | kW      |                                    |
+| Unit1BatteryPack2ChargeDischargePower  | Number     | 0.1  | W       |                                    |
 | Unit1BatteryPack2TotalCharge           | Number     | 100  | kWh     |                                    |
 | Unit1BatteryPack2TotalDischarge        | Number     | 100  | kWh     |                                    |
 | Unit1BatteryPack2MinimumTemperature    | Number     | 10   | °C      |                                    |
 | Unit1BatteryPack2MaximumTemperature    | Number     | 10   | °C      |                                    |
 | Unit1BatteryPack3SN                    | String     |      |         |                                    |
 | Unit1BatteryPack3No                    | Number     | 1    |         |                                    |
 | Unit1BatteryPack3FirmwareVersion       | String     |      |         |                                    |
 | Unit1BatteryPack3WorkingStatus         | Number     | 1    |         |                                    |
 | Unit1BatteryPack3Voltage               | Number     | 10   | V       |                                    |
 | Unit1BatteryPack3Current               | Number     | 10   | A       |                                    |
 | Unit1BatteryPack3SOC                   | Number     | 10   | %       |                                    |
-| Unit1BatteryPack3ChargeDischargeStatus | Number     | 100  | kW      |                                    |
+| Unit1BatteryPack3ChargeDischargeStatus | Number     | 0.1  | W       |                                    |
 | Unit1BatteryPack3TotalCharge           | Number     | 100  | kWh     |                                    |
 | Unit1BatteryPack3TotalDischarge        | Number     | 100  | kWh     |                                    |
 | Unit1BatteryPack3MinimumTemperature    | Number     | 10   | °C      |                                    |
 | Unit1BatteryPack3MaximumTemperature    | Number     | 10   | °C      |                                    |
 | Unit2BatteryPack1SN                    | String     |      |         |                                    |
 | Unit2BatteryPack1No                    | Number     | 1    |         |                                    |
 | Unit2BatteryPack1FirmwareVersion       | String     |      |         |                                    |
 | Unit2BatteryPack1WorkingStatus         | Number     | 1    |         |                                    |
 | Unit2BatteryPack1Voltage               | Number     | 10   | V       |                                    |
 | Unit2BatteryPack1Current               | Number     | 10   | A       |                                    |
 | Unit2BatteryPack1SOC                   | Number     | 10   | %       |                                    |
-| Unit2BatteryPack1ChargeDischargePower  | Number     | 100  | kW      |                                    |
+| Unit2BatteryPack1ChargeDischargePower  | Number     | 0.1  | W       |                                    |
 | Unit2BatteryPack1TotalCharge           | Number     | 100  | kWh     |                                    |
 | Unit2BatteryPack1TotalDischarge        | Number     | 100  | kWh     |                                    |
 | Unit2BatteryPack1MinimumTemperature    | Number     | 10   | °C      |                                    |
 | Unit2BatteryPack1MaximumTemperature    | Number     | 10   | °C      |                                    |
 | Unit2BatteryPack2SN                    | String     |      |         |                                    |
 | Unit2BatteryPack2No                    | Number     | 1    |         |                                    |
 | Unit2BatteryPack2FirmwareVersion       | String     |      |         |                                    |
 | Unit2BatteryPack2WorkingStatus         | Number     | 1    |         |                                    |
 | Unit2BatteryPack2Voltage               | Number     | 10   | V       |                                    |
 | Unit2BatteryPack2Current               | Number     | 10   | A       |                                    |
 | Unit2BatteryPack2SOC                   | Number     | 10   | %       |                                    |
-| Unit2BatteryPack2ChargeDischargePower  | Number     | 100  | kW      |                                    |
+| Unit2BatteryPack2ChargeDischargePower  | Number     | 0.1  | W       |                                    |
 | Unit2BatteryPack2TotalCharge           | Number     | 100  | kWh     |                                    |
 | Unit2BatteryPack2TotalDischarge        | Number     | 100  | kWh     |                                    |
 | Unit2BatteryPack2MinimumTemperature    | Number     | 10   | °C      |                                    |
 | Unit2BatteryPack2MaximumTemperature    | Number     | 10   | °C      |                                    |
 | Unit2BatteryPack3SN                    | String     |      |         |                                    |
 | Unit2BatteryPack3No                    | Number     | 1    |         |                                    |
 | Unit2BatteryPack3FirmwareVersion       | String     |      |         |                                    |
 | Unit2BatteryPack3WorkingStatus         | Number     | 1    |         |                                    |
 | Unit2BatteryPack3Voltage               | Number     | 10   | V       |                                    |
 | Unit2BatteryPack3Current               | Number     | 10   | A       |                                    |
 | Unit2BatteryPack3SOC                   | Number     | 10   | %       |                                    |
-| Unit2BatteryPack3ChargeDischargePower  | Number     | 100  | kW      |                                    |
+| Unit2BatteryPack3ChargeDischargePower  | Number     | 0.1  | W       |                                    |
 | Unit2BatteryPack3TotalCharge           | Number     | 100  | kWh     |                                    |
 | Unit2BatteryPack3TotalDischarge        | Number     | 100  | kWh     |                                    |
 | Unit2BatteryPack3MinimumTemperature    | Number     | 10   | °C      |                                    |
 | Unit2BatteryPack3MaximumTemperature    | Number     | 10   | °C      |                                    |
 
 ### MeterEquipmentRegister
```

