# Comparing `tmp/dronecan-1.0.8.tar.gz` & `tmp/dronecan-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dronecan-1.0.8.tar", last modified: Tue Feb  8 03:56:42 2022, max compression
+gzip compressed data, was "dronecan-1.0.9.tar", last modified: Fri Feb 11 02:23:37 2022, max compression
```

## Comparing `dronecan-1.0.8.tar` & `dronecan-1.0.9.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.675799 dronecan-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-02-08 03:56:31.000000 dronecan-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-02-08 03:56:31.000000 dronecan-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-02-08 03:56:42.675799 dronecan-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-02-08 03:56:31.000000 dronecan-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.663798 dronecan-1.0.8/dronecan/
--rw-r--r--   0 runner    (1001) docker     (121)     8086 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.663798 dronecan-1.0.8/dronecan/app/
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9723 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/app/dynamic_node_id.py
--rw-r--r--   0 runner    (1001) docker     (121)     3694 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/app/file_server.py
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/app/log_message_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2405 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/app/message_collector.py
--rw-r--r--   0 runner    (1001) docker     (121)     8061 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/app/node_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.663798 dronecan-1.0.8/dronecan/driver/
--rw-r--r--   0 runner    (1001) docker     (121)     2070 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2438 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/driver/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     4705 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/driver/mavcan.py
--rw-r--r--   0 runner    (1001) docker     (121)     5808 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/driver/python_can.py
--rw-r--r--   0 runner    (1001) docker     (121)    32219 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/driver/slcan.py
--rw-r--r--   0 runner    (1001) docker     (121)     9765 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/driver/socketcan.py
--rw-r--r--   0 runner    (1001) docker     (121)    10116 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/driver/timestamp_estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.667798 dronecan-1.0.8/dronecan/dsdl/
--rw-r--r--   0 runner    (1001) docker     (121)      751 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/dsdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2560 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/dsdl/common.py
--rw-r--r--   0 runner    (1001) docker     (121)    35142 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/dsdl/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/dsdl/signature.py
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/dsdl/type_limits.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.659798 dronecan-1.0.8/dronecan/dsdl_specs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.659798 dronecan-1.0.8/dronecan/dsdl_specs/ardupilot/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.659798 dronecan-1.0.8/dronecan/dsdl_specs/ardupilot/equipment/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.667798 dronecan-1.0.8/dronecan/dsdl_specs/ardupilot/equipment/power/
--rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/ardupilot/equipment/power/20004.BatteryInfoAux.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.667798 dronecan-1.0.8/dronecan/dsdl_specs/ardupilot/equipment/trafficmonitor/
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/ardupilot/equipment/trafficmonitor/20790.TrafficReport.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.667798 dronecan-1.0.8/dronecan/dsdl_specs/ardupilot/gnss/
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/ardupilot/gnss/20002.Heading.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      464 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/ardupilot/gnss/20003.Status.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/ardupilot/gnss/20005.MovingBaselineData.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/ardupilot/gnss/20006.RelPosHeading.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.667798 dronecan-1.0.8/dronecan/dsdl_specs/ardupilot/indication/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/ardupilot/indication/20000.SafetyState.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/ardupilot/indication/20001.Button.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/ardupilot/indication/20007.NotifyState.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.659798 dronecan-1.0.8/dronecan/dsdl_specs/com/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.659798 dronecan-1.0.8/dronecan/dsdl_specs/com/hex/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.659798 dronecan-1.0.8/dronecan/dsdl_specs/com/hex/equipment/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.667798 dronecan-1.0.8/dronecan/dsdl_specs/com/hex/equipment/flow/
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/com/hex/equipment/flow/20200.Measurement.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.659798 dronecan-1.0.8/dronecan/dsdl_specs/cuav/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.659798 dronecan-1.0.8/dronecan/dsdl_specs/cuav/equipment/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.667798 dronecan-1.0.8/dronecan/dsdl_specs/cuav/equipment/power/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3008 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/cuav/equipment/power/20300.CBAT.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.659798 dronecan-1.0.8/dronecan/dsdl_specs/dronecan/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.659798 dronecan-1.0.8/dronecan/dsdl_specs/dronecan/sensors/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.667798 dronecan-1.0.8/dronecan/dsdl_specs/dronecan/sensors/hygrometer/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/dronecan/sensors/hygrometer/1032.Hygrometer.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.667798 dronecan-1.0.8/dronecan/dsdl_specs/mppt/
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/mppt/20020.Stream.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/mppt/240.OutputEnable.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.667798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/CoarseOrientation.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/Timestamp.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.659798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.667798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/actuator/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/actuator/1010.ArrayCommand.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/actuator/1011.Status.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      467 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/actuator/Command.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.667798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/ahrs/
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/ahrs/1000.Solution.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/ahrs/1001.MagneticFieldStrength.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/ahrs/1002.MagneticFieldStrength2.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/ahrs/1003.RawIMU.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.667798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/air_data/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/air_data/1020.TrueAirspeed.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/air_data/1021.IndicatedAirspeed.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/air_data/1025.AngleOfAttack.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/air_data/1026.Sideslip.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/air_data/1027.RawAirData.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/air_data/1028.StaticPressure.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/air_data/1029.StaticTemperature.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.667798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/camera_gimbal/
--rw-r--r--   0 runner    (1001) docker     (121)      543 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/camera_gimbal/1040.AngularCommand.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/camera_gimbal/1041.GEOPOICommand.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/camera_gimbal/1044.Status.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/camera_gimbal/Mode.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.667798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/device/
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/device/1110.Temperature.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.667798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/esc/
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/esc/1030.RawCommand.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/esc/1031.RPMCommand.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/esc/1034.Status.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.667798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/gnss/
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/gnss/1060.Fix.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/gnss/1061.Auxiliary.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/gnss/1062.RTCMStream.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)     3354 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/gnss/1063.Fix2.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/gnss/ECEFPositionVelocity.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.671798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/hardpoint/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/hardpoint/1070.Command.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/hardpoint/1071.Status.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.671798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/ice/
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/ice/1129.FuelTankStatus.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.671798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/ice/reciprocating/
--rw-r--r--   0 runner    (1001) docker     (121)     5446 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/ice/reciprocating/1120.Status.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/ice/reciprocating/CylinderStatus.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.671798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/indication/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/indication/1080.BeepCommand.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/indication/1081.LightsCommand.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/indication/RGB565.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)     1775 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/indication/SingleLightCommand.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.671798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/power/
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/power/1090.PrimaryPowerSupplyStatus.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/power/1091.CircuitStatus.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)     3219 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/power/1092.BatteryInfo.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.671798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/range_sensor/
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/range_sensor/1050.Measurement.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.671798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/safety/
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/safety/1100.ArmingStatus.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.671798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/navigation/
--rw-r--r--   0 runner    (1001) docker     (121)     2202 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/navigation/2000.GlobalNavigationSolution.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.671798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/1.GetNodeInfo.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/2.GetDataTypeInfo.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)     1986 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/341.NodeStatus.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/4.GetTransportStats.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/4.GlobalTimeSync.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/5.Panic.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/5.RestartNode.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)     2933 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/6.AccessCommandShell.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/CANIfaceStats.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/DataTypeKind.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      488 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/HardwareVersion.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/SoftwareVersion.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.671798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/debug/
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/debug/16370.KeyValue.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/debug/16383.LogMessage.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/debug/LogLevel.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.671798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/
--rw-r--r--   0 runner    (1001) docker     (121)     6997 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/1.Allocation.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.671798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/server/
--rw-r--r--   0 runner    (1001) docker     (121)     1383 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/server/30.AppendEntries.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/server/31.RequestVote.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/server/390.Discovery.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/server/Entry.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.671798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/enumeration/
--rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/enumeration/15.Begin.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/enumeration/380.Indication.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.671798 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/file/
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/file/40.BeginFirmwareUpdate.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/file/45.GetInfo.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/file/46.GetDirectoryEntryInfo.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/file/47.Delete.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/file/48.Read.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/file/49.Write.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/file/EntryType.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/file/Error.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/file/Path.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.675799 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/param/
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/param/10.ExecuteOpcode.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)     1462 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/param/11.GetSet.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/param/Empty.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/param/NumericValue.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/param/Value.uavcan
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.675799 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/tunnel/
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/tunnel/2010.Broadcast.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/tunnel/63.Call.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-02-08 03:56:32.000000 dronecan-1.0.8/dronecan/dsdl_specs/uavcan/tunnel/Protocol.uavcan
--rw-r--r--   0 runner    (1001) docker     (121)    14857 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/introspect.py
--rw-r--r--   0 runner    (1001) docker     (121)    21164 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/node.py
--rw-r--r--   0 runner    (1001) docker     (121)    32816 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/transport.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-02-08 03:56:31.000000 dronecan-1.0.8/dronecan/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.663798 dronecan-1.0.8/dronecan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-02-08 03:56:42.000000 dronecan-1.0.8/dronecan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12265 2022-02-08 03:56:42.000000 dronecan-1.0.8/dronecan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-08 03:56:42.000000 dronecan-1.0.8/dronecan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-02-08 03:56:42.000000 dronecan-1.0.8/dronecan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-08 03:56:42.675799 dronecan-1.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2014 2022-02-08 03:56:31.000000 dronecan-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-08 03:56:42.675799 dronecan-1.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-02-08 03:56:31.000000 dronecan-1.0.8/test/test_driver.py
--rw-r--r--   0 runner    (1001) docker     (121)     2511 2022-02-08 03:56:31.000000 dronecan-1.0.8/test/test_node.py
--rw-r--r--   0 runner    (1001) docker     (121)    22698 2022-02-08 03:56:31.000000 dronecan-1.0.8/test/test_transport.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.985826 dronecan-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-02-11 02:23:26.000000 dronecan-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-02-11 02:23:26.000000 dronecan-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      523 2022-02-11 02:23:37.985826 dronecan-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-02-11 02:23:26.000000 dronecan-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.969825 dronecan-1.0.9/dronecan/
+-rw-r--r--   0 runner    (1001) docker     (121)     8086 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.969825 dronecan-1.0.9/dronecan/app/
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9723 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/app/dynamic_node_id.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3694 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/app/file_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)      917 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/app/log_message_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2405 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/app/message_collector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8061 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/app/node_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.969825 dronecan-1.0.9/dronecan/driver/
+-rw-r--r--   0 runner    (1001) docker     (121)     2070 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3553 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/driver/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5150 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/driver/mavcan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5913 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/driver/python_can.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32402 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/driver/slcan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9862 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/driver/socketcan.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10116 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/driver/timestamp_estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.973825 dronecan-1.0.9/dronecan/dsdl/
+-rw-r--r--   0 runner    (1001) docker     (121)      751 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/dsdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2560 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/dsdl/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35142 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/dsdl/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/dsdl/signature.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/dsdl/type_limits.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.961825 dronecan-1.0.9/dronecan/dsdl_specs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.961825 dronecan-1.0.9/dronecan/dsdl_specs/ardupilot/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.961825 dronecan-1.0.9/dronecan/dsdl_specs/ardupilot/equipment/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.973825 dronecan-1.0.9/dronecan/dsdl_specs/ardupilot/equipment/power/
+-rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/ardupilot/equipment/power/20004.BatteryInfoAux.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.973825 dronecan-1.0.9/dronecan/dsdl_specs/ardupilot/equipment/trafficmonitor/
+-rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/ardupilot/equipment/trafficmonitor/20790.TrafficReport.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.973825 dronecan-1.0.9/dronecan/dsdl_specs/ardupilot/gnss/
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/ardupilot/gnss/20002.Heading.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      464 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/ardupilot/gnss/20003.Status.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/ardupilot/gnss/20005.MovingBaselineData.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/ardupilot/gnss/20006.RelPosHeading.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.973825 dronecan-1.0.9/dronecan/dsdl_specs/ardupilot/indication/
+-rw-r--r--   0 runner    (1001) docker     (121)      128 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/ardupilot/indication/20000.SafetyState.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      250 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/ardupilot/indication/20001.Button.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/ardupilot/indication/20007.NotifyState.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.961825 dronecan-1.0.9/dronecan/dsdl_specs/com/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.961825 dronecan-1.0.9/dronecan/dsdl_specs/com/hex/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.961825 dronecan-1.0.9/dronecan/dsdl_specs/com/hex/equipment/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.973825 dronecan-1.0.9/dronecan/dsdl_specs/com/hex/equipment/flow/
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/com/hex/equipment/flow/20200.Measurement.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.961825 dronecan-1.0.9/dronecan/dsdl_specs/cuav/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.961825 dronecan-1.0.9/dronecan/dsdl_specs/cuav/equipment/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.973825 dronecan-1.0.9/dronecan/dsdl_specs/cuav/equipment/power/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3008 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/cuav/equipment/power/20300.CBAT.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.961825 dronecan-1.0.9/dronecan/dsdl_specs/dronecan/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.961825 dronecan-1.0.9/dronecan/dsdl_specs/dronecan/sensors/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.973825 dronecan-1.0.9/dronecan/dsdl_specs/dronecan/sensors/hygrometer/
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/dronecan/sensors/hygrometer/1032.Hygrometer.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.973825 dronecan-1.0.9/dronecan/dsdl_specs/mppt/
+-rw-r--r--   0 runner    (1001) docker     (121)      421 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/mppt/20020.Stream.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      529 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/mppt/240.OutputEnable.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.973825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/CoarseOrientation.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/Timestamp.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.961825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.973825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/actuator/
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/actuator/1010.ArrayCommand.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/actuator/1011.Status.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/actuator/Command.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.973825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/ahrs/
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/ahrs/1000.Solution.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/ahrs/1001.MagneticFieldStrength.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      203 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/ahrs/1002.MagneticFieldStrength2.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)     1708 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/ahrs/1003.RawIMU.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.977825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/air_data/
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/air_data/1020.TrueAirspeed.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/air_data/1021.IndicatedAirspeed.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/air_data/1025.AngleOfAttack.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/air_data/1026.Sideslip.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/air_data/1027.RawAirData.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/air_data/1028.StaticPressure.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/air_data/1029.StaticTemperature.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.977825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/camera_gimbal/
+-rw-r--r--   0 runner    (1001) docker     (121)      543 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/camera_gimbal/1040.AngularCommand.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      515 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/camera_gimbal/1041.GEOPOICommand.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      320 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/camera_gimbal/1044.Status.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/camera_gimbal/Mode.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.977825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/device/
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/device/1110.Temperature.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.977825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/esc/
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/esc/1030.RawCommand.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      311 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/esc/1031.RPMCommand.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/esc/1034.Status.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.977825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/gnss/
+-rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/gnss/1060.Fix.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/gnss/1061.Auxiliary.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/gnss/1062.RTCMStream.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)     3354 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/gnss/1063.Fix2.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      953 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/gnss/ECEFPositionVelocity.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.977825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/hardpoint/
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/hardpoint/1070.Command.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/hardpoint/1071.Status.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.977825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/ice/
+-rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/ice/1129.FuelTankStatus.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.977825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/ice/reciprocating/
+-rw-r--r--   0 runner    (1001) docker     (121)     5446 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/ice/reciprocating/1120.Status.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      793 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/ice/reciprocating/CylinderStatus.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.977825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/indication/
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/indication/1080.BeepCommand.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/indication/1081.LightsCommand.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/indication/RGB565.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)     1775 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/indication/SingleLightCommand.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.977825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/power/
+-rw-r--r--   0 runner    (1001) docker     (121)      667 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/power/1090.PrimaryPowerSupplyStatus.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/power/1091.CircuitStatus.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)     3219 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/power/1092.BatteryInfo.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.977825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/range_sensor/
+-rw-r--r--   0 runner    (1001) docker     (121)      710 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/range_sensor/1050.Measurement.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.977825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/safety/
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/safety/1100.ArmingStatus.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.977825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/navigation/
+-rw-r--r--   0 runner    (1001) docker     (121)     2202 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/navigation/2000.GlobalNavigationSolution.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.981825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/
+-rw-r--r--   0 runner    (1001) docker     (121)      673 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/1.GetNodeInfo.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/2.GetDataTypeInfo.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)     1986 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/341.NodeStatus.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/4.GetTransportStats.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      778 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/4.GlobalTimeSync.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/5.Panic.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/5.RestartNode.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)     2933 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/6.AccessCommandShell.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/CANIfaceStats.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/DataTypeKind.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      488 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/HardwareVersion.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)     1549 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/SoftwareVersion.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.981825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/debug/
+-rw-r--r--   0 runner    (1001) docker     (121)      368 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/debug/16370.KeyValue.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/debug/16383.LogMessage.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/debug/LogLevel.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.981825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/
+-rw-r--r--   0 runner    (1001) docker     (121)     6997 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/1.Allocation.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.981825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/server/
+-rw-r--r--   0 runner    (1001) docker     (121)     1383 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/server/30.AppendEntries.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      335 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/server/31.RequestVote.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)     1054 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/server/390.Discovery.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/server/Entry.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.981825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/enumeration/
+-rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/enumeration/15.Begin.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      486 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/enumeration/380.Indication.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.981825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/file/
+-rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/file/40.BeginFirmwareUpdate.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/file/45.GetInfo.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      696 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/file/46.GetDirectoryEntryInfo.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/file/47.Delete.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      706 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/file/48.Read.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      953 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/file/49.Write.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      413 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/file/EntryType.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/file/Error.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/file/Path.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.981825 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/param/
+-rw-r--r--   0 runner    (1001) docker     (121)     1112 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/param/10.ExecuteOpcode.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)     1462 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/param/11.GetSet.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/param/Empty.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/param/NumericValue.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      756 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/param/Value.uavcan
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.985826 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/tunnel/
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/tunnel/2010.Broadcast.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      572 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/tunnel/63.Call.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-02-11 02:23:27.000000 dronecan-1.0.9/dronecan/dsdl_specs/uavcan/tunnel/Protocol.uavcan
+-rw-r--r--   0 runner    (1001) docker     (121)    14857 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/introspect.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21181 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/node.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33005 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/transport.py
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2022-02-11 02:23:26.000000 dronecan-1.0.9/dronecan/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.969825 dronecan-1.0.9/dronecan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      523 2022-02-11 02:23:37.000000 dronecan-1.0.9/dronecan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    12265 2022-02-11 02:23:37.000000 dronecan-1.0.9/dronecan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-11 02:23:37.000000 dronecan-1.0.9/dronecan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-02-11 02:23:37.000000 dronecan-1.0.9/dronecan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-11 02:23:37.985826 dronecan-1.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2014 2022-02-11 02:23:26.000000 dronecan-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-11 02:23:37.985826 dronecan-1.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      333 2022-02-11 02:23:26.000000 dronecan-1.0.9/test/test_driver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2511 2022-02-11 02:23:26.000000 dronecan-1.0.9/test/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22698 2022-02-11 02:23:26.000000 dronecan-1.0.9/test/test_transport.py
```

### Comparing `dronecan-1.0.8/LICENSE` & `dronecan-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/PKG-INFO` & `dronecan-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dronecan
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python implementation of the DroneCAN protocol stack
 Home-page: https://dronecan.github.io
 Author: Pavel Kirienko, Ben Dyer
 Author-email: uavcan@googlegroups.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dronecan-1.0.8/README.md` & `dronecan-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/__init__.py` & `dronecan-1.0.9/dronecan/__init__.py`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/app/dynamic_node_id.py` & `dronecan-1.0.9/dronecan/app/dynamic_node_id.py`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/app/file_server.py` & `dronecan-1.0.9/dronecan/app/file_server.py`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/app/log_message_monitor.py` & `dronecan-1.0.9/dronecan/app/log_message_monitor.py`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/app/message_collector.py` & `dronecan-1.0.9/dronecan/app/message_collector.py`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/app/node_monitor.py` & `dronecan-1.0.9/dronecan/app/node_monitor.py`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/driver/__init__.py` & `dronecan-1.0.9/dronecan/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/driver/mavcan.py` & `dronecan-1.0.9/dronecan/driver/mavcan.py`

 * *Files 13% similar despite different names*

```diff
@@ -78,36 +78,46 @@
             if frame.extended:
                 message_id |= 1<<31
             message = frame.data
             mlen = len(message)
             if mlen < 8:
                 message += bytearray([0]*(8-mlen))
             try:
-                conn.mav.can_frame_send(
-                    target_system,
-                    target_component,
-                    bus,
-                    mlen,
-                    message_id,
-                    message)
+                if frame.canfd:
+                    conn.mav.canfd_frame_send(
+                        target_system,
+                        target_component,
+                        bus,
+                        mlen,
+                        message_id,
+                        message)
+                else:
+                    conn.mav.can_frame_send(
+                        target_system,
+                        target_component,
+                        bus,
+                        mlen,
+                        message_id,
+                        message)
             except Exception as ex:
                 print(ex)
             if time.time() - last_enable > 1:
                 enable_can_forward()
 
         try:
-            m = conn.recv_match(type='CAN_FRAME',blocking=True,timeout=0.005)
+            m = conn.recv_match(type=['CAN_FRAME','CANFD_FRAME'],blocking=True,timeout=0.005)
         except Exception as ex:
             reconnect()
             continue
         if m is None:
             continue
         is_extended = (m.id & (1<<31)) != 0
+        is_canfd = m.get_type() == 'CANFD_FRAME'
         canid = m.id & 0x1FFFFFFF
-        frame = CANFrame(canid, m.data[:m.len], is_extended)
+        frame = CANFrame(canid, m.data[:m.len], is_extended, canfd=is_canfd)
         rx_queue.put_nowait(frame)
 
 
 # MAVLink CAN driver
 #
 class MAVCAN(AbstractDriver):
     """
@@ -142,16 +152,16 @@
                 self._rx_hook(frame)
                 return frame
             if timeout is not None:
                 timeout = max(timeout, 0.001)
                 if time.time() >= tstart + timeout:
                     return
 
-    def send(self, message_id, message, extended=False):
-        frame = CANFrame(message_id, message, extended)
+    def send(self, message_id, message, extended=False, canfd=False):
+        frame = CANFrame(message_id, message, extended, canfd=canfd)
         self._tx_hook(frame)
         self.tx_queue.put_nowait(frame)
 
     def is_mavlink_port(device_name):
         '''check if a device is sending mavlink'''
         os.environ['MAVLINK20'] = '1'
         conn = mavutil.mavlink_connection(device_name, source_system=250, source_component=mavutil.mavlink.MAV_COMP_ID_MAVCAN)
```

### Comparing `dronecan-1.0.8/dronecan/driver/python_can.py` & `dronecan-1.0.9/dronecan/driver/python_can.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,13 +148,15 @@
                         ts_real=ts_real,
                     )
                     self._rx_hook(frame)
                     return frame
             except Exception as ex:
                 logger.error("Receive exception", exc_info=True)
 
-        def send(self, message_id, message, extended=False):
+        def send(self, message_id, message, extended=False, canfd=False):
+            if canfd:
+                raise DriverError('CANFD not supported by PythonCAN')
             self._check_write_feedback()
             try:
                 self._write_queue.put_nowait(CANFrame(message_id, message, extended))
             except queue.Full:
                 raise TxQueueFullError()
```

### Comparing `dronecan-1.0.8/dronecan/driver/slcan.py` & `dronecan-1.0.9/dronecan/driver/slcan.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,31 +232,36 @@
     def _process_slcan_line(self, line, local_ts_mono, local_ts_real):
         line = line.strip().strip(NACK).strip(CLI_END_OF_TEXT)
         line_len = len(line)
 
         if line_len < 1:
             return
 
+        canfd = False
         # Checking the header, ignore all irrelevant lines
         if line[0] == b'T'[0]:
             id_len = 8
         elif line[0] == b't'[0]:
             id_len = 3
+        elif line[0] == b'D'[0]:
+            id_len = 8
+            canfd = True
         else:
             return
 
         # Parsing ID and DLC
         packet_id = int(line[1:1 + id_len], 16)
-        if self.PY2_COMPAT:
-            packet_len = int(line[1 + id_len])              # This version is horribly slow
-        else:
-            packet_len = line[1 + id_len] - 48              # Py3 version is faster
+        packet_len = CANFrame.dlc_to_datalength(int(chr(line[1 + id_len]), 16))
 
-        if packet_len > 8 or packet_len < 0:
-            raise DriverError('Invalid packet length')
+        if canfd:
+            if packet_len > 64 or packet_len < 0:
+                raise DriverError('Invalid packet length')
+        else:
+            if packet_len > 8 or packet_len < 0:
+                raise DriverError('Invalid packet length', packet_len, line[1 + id_len])
 
         # Parsing the payload, detecting timestamp
         # <type> <id> <dlc> <data>         [timestamp]
         # 1      3|8  1     packet_len * 2 [4]
         with_timestamp = line_len > (2 + id_len + packet_len * 2)
 
         packet_data = binascii.a2b_hex(line[2 + id_len:2 + id_len + packet_len * 2])
@@ -266,15 +271,15 @@
             ts_hardware = int(line[-4:], 16) * 1e-3
             ts_mono = self._ts_estimator_mono.update(ts_hardware, local_ts_mono)
             ts_real = self._ts_estimator_real.update(ts_hardware, local_ts_real)
         else:
             ts_mono = local_ts_mono
             ts_real = local_ts_real
 
-        frame = CANFrame(packet_id, packet_data, (id_len == 8), ts_monotonic=ts_mono, ts_real=ts_real)
+        frame = CANFrame(packet_id, packet_data, (id_len == 8), ts_monotonic=ts_mono, ts_real=ts_real, canfd=canfd)
         self._output_queue.put_nowait(frame)
 
     def _process_many_slcan_lines(self, lines, ts_mono, ts_real):
         for slc in lines:
             # noinspection PyBroadException
             try:
                 self._process_slcan_line(slc, local_ts_mono=ts_mono, local_ts_real=ts_real)
@@ -843,17 +848,17 @@
             # Termination condition
             if deadline == 0:
                 break
             elif deadline is not None:
                 if time.monotonic() >= deadline:
                     return
 
-    def send(self, message_id, message, extended=False):
+    def send(self, message_id, message, extended=False, canfd=False):
         self._check_alive()
-        frame = CANFrame(message_id, message, extended)
+        frame = CANFrame(message_id, message, extended, canfd=canfd)
         try:
             self._tx_queue.put_nowait(frame)
         except queue.Full:
             raise TxQueueFullError()
         self._tx_hook(frame)
 
     def execute_cli_command(self, command, callback, timeout=None):
```

### Comparing `dronecan-1.0.8/dronecan/driver/socketcan.py` & `dronecan-1.0.9/dronecan/driver/socketcan.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,13 +273,15 @@
                 ts_mono = self._convert_real_to_monotonic(ts_real)
 
             frame = CANFrame(can_id & CAN_EFF_MASK, can_data[0:can_dlc], bool(can_id & CAN_EFF_FLAG),
                              ts_monotonic=ts_mono, ts_real=ts_real)
             self._rx_hook(frame)
             return frame
 
-    def send(self, message_id, message, extended=False):
+    def send(self, message_id, message, extended=False, canfd=False):
+        if canfd:
+            raise DriverError('CANFD not supported by SocketCAN')
         self._check_write_feedback()
         try:
             self._write_queue.put_nowait(CANFrame(message_id, message, extended))
         except queue.Full:
             raise TxQueueFullError()
```

### Comparing `dronecan-1.0.8/dronecan/driver/timestamp_estimator.py` & `dronecan-1.0.9/dronecan/driver/timestamp_estimator.py`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl/__init__.py` & `dronecan-1.0.9/dronecan/dsdl/__init__.py`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl/common.py` & `dronecan-1.0.9/dronecan/dsdl/common.py`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl/parser.py` & `dronecan-1.0.9/dronecan/dsdl/parser.py`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl/signature.py` & `dronecan-1.0.9/dronecan/dsdl/signature.py`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl/type_limits.py` & `dronecan-1.0.9/dronecan/dsdl/type_limits.py`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/ardupilot/equipment/power/20004.BatteryInfoAux.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/ardupilot/equipment/power/20004.BatteryInfoAux.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/ardupilot/equipment/trafficmonitor/20790.TrafficReport.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/ardupilot/equipment/trafficmonitor/20790.TrafficReport.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/ardupilot/indication/20007.NotifyState.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/ardupilot/indication/20007.NotifyState.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/cuav/equipment/power/20300.CBAT.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/cuav/equipment/power/20300.CBAT.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/mppt/240.OutputEnable.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/mppt/240.OutputEnable.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/CoarseOrientation.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/CoarseOrientation.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/ahrs/1003.RawIMU.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/ahrs/1003.RawIMU.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/air_data/1027.RawAirData.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/air_data/1027.RawAirData.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/camera_gimbal/1040.AngularCommand.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/camera_gimbal/1040.AngularCommand.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/camera_gimbal/1041.GEOPOICommand.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/camera_gimbal/1041.GEOPOICommand.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/gnss/1060.Fix.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/gnss/1060.Fix.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/gnss/1063.Fix2.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/gnss/1063.Fix2.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/gnss/ECEFPositionVelocity.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/gnss/ECEFPositionVelocity.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/ice/1129.FuelTankStatus.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/ice/1129.FuelTankStatus.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/ice/reciprocating/1120.Status.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/ice/reciprocating/1120.Status.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/ice/reciprocating/CylinderStatus.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/ice/reciprocating/CylinderStatus.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/indication/SingleLightCommand.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/indication/SingleLightCommand.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/power/1090.PrimaryPowerSupplyStatus.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/power/1090.PrimaryPowerSupplyStatus.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/power/1092.BatteryInfo.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/power/1092.BatteryInfo.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/equipment/range_sensor/1050.Measurement.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/equipment/range_sensor/1050.Measurement.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/navigation/2000.GlobalNavigationSolution.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/navigation/2000.GlobalNavigationSolution.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/1.GetNodeInfo.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/1.GetNodeInfo.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/2.GetDataTypeInfo.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/2.GetDataTypeInfo.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/341.NodeStatus.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/341.NodeStatus.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/4.GlobalTimeSync.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/4.GlobalTimeSync.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/5.Panic.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/5.Panic.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/6.AccessCommandShell.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/6.AccessCommandShell.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/SoftwareVersion.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/SoftwareVersion.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/1.Allocation.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/1.Allocation.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/server/30.AppendEntries.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/server/30.AppendEntries.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/server/390.Discovery.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/dynamic_node_id/server/390.Discovery.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/enumeration/15.Begin.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/enumeration/15.Begin.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/file/40.BeginFirmwareUpdate.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/file/40.BeginFirmwareUpdate.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/file/46.GetDirectoryEntryInfo.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/file/46.GetDirectoryEntryInfo.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/file/48.Read.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/file/48.Read.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/file/49.Write.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/file/49.Write.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/param/10.ExecuteOpcode.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/param/10.ExecuteOpcode.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/param/11.GetSet.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/param/11.GetSet.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/protocol/param/Value.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/protocol/param/Value.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/dsdl_specs/uavcan/tunnel/63.Call.uavcan` & `dronecan-1.0.9/dronecan/dsdl_specs/uavcan/tunnel/63.Call.uavcan`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/introspect.py` & `dronecan-1.0.9/dronecan/introspect.py`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/dronecan/node.py` & `dronecan-1.0.9/dronecan/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,15 @@
     def can_driver(self):
         return self._can_driver
 
     def _recv_frame(self, raw_frame):
         if not raw_frame.extended:
             return
 
-        frame = transport.Frame(raw_frame.id, raw_frame.data, raw_frame.ts_monotonic, raw_frame.ts_real)
+        frame = transport.Frame(raw_frame.id, raw_frame.data, raw_frame.ts_monotonic, raw_frame.ts_real, raw_frame.canfd)
 
         transfer_frames = self._transfer_manager.receive_frame(frame)
         if not transfer_frames:
             return
 
         transfer = transport.Transfer()
         transfer.from_frames(transfer_frames)
```

### Comparing `dronecan-1.0.8/dronecan/transport.py` & `dronecan-1.0.9/dronecan/transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -620,19 +620,20 @@
             tag_len = union_tag_bits_from_num_elements(len(self._fields))
             return format(tag, '0' + str(tag_len) + 'b') + self._fields[field]._pack(tao)
         else:
             return ''.join(field._pack(tao and last) for _, last, field in enum_mark_last(self._fields.values()))
 
 
 class Frame(object):
-    def __init__(self, message_id, data, ts_monotonic=None, ts_real=None):  # @ReservedAssignment
+    def __init__(self, message_id, data, ts_monotonic=None, ts_real=None, canfd=False):  # @ReservedAssignment
         self.message_id = message_id
         self.bytes = bytearray(data)
         self.ts_monotonic = ts_monotonic
         self.ts_real = ts_real
+        self.canfd = canfd
 
     @property
     def transfer_key(self):
         # The transfer is uniquely identified by the message ID and the 5-bit
         # Transfer ID contained in the last byte of the frame payload.
         return self.message_id, (self.bytes[-1] & 0x1F) if self.bytes else None
 
@@ -818,17 +819,20 @@
         self.data_type_signature = datatype.get_data_type_signature()
         self.data_type_crc = datatype.base_crc
 
         if self.service_not_message:
             self.payload = datatype(_mode="request" if self.request_not_response else "response")
         else:
             self.payload = datatype()
-
+        tao = True
+        for frame in frames:
+            if frame.canfd:    # we are in CANFD world can't use tao
+                tao = False
         # noinspection PyProtectedMember
-        self.payload._unpack(bits_from_bytes(payload_bytes))
+        self.payload._unpack(bits_from_bytes(payload_bytes), tao)
 
     @property
     def key(self):
         return self.message_id, self.transfer_id
 
     def is_response_to(self, transfer):
         if (transfer.service_not_message and self.service_not_message and
```

### Comparing `dronecan-1.0.8/dronecan.egg-info/PKG-INFO` & `dronecan-1.0.9/dronecan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dronecan
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python implementation of the DroneCAN protocol stack
 Home-page: https://dronecan.github.io
 Author: Pavel Kirienko, Ben Dyer
 Author-email: uavcan@googlegroups.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dronecan-1.0.8/dronecan.egg-info/SOURCES.txt` & `dronecan-1.0.9/dronecan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/setup.py` & `dronecan-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/test/test_node.py` & `dronecan-1.0.9/test/test_node.py`

 * *Files identical despite different names*

### Comparing `dronecan-1.0.8/test/test_transport.py` & `dronecan-1.0.9/test/test_transport.py`

 * *Files identical despite different names*

