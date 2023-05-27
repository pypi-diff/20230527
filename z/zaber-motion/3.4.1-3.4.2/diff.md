# Comparing `tmp/zaber_motion-3.4.1.tar.gz` & `tmp/zaber_motion-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zaber_motion-3.4.1.tar", last modified: Wed May 24 23:09:02 2023, max compression
+gzip compressed data, was "zaber_motion-3.4.2.tar", last modified: Fri May 26 22:59:02 2023, max compression
```

## Comparing `zaber_motion-3.4.1.tar` & `zaber_motion-3.4.2.tar`

### file list

```diff
@@ -1,187 +1,187 @@
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-24 23:09:02.097885 zaber_motion-3.4.1/
--rw-r--r--   0 zaber      (501) staff       (20)      218 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/DESCRIPTION.md
--rw-r--r--   0 zaber      (501) staff       (20)   109244 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/LICENSE.txt
--rw-r--r--   0 zaber      (501) staff       (20)       13 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/MANIFEST.in
--rw-r--r--   0 zaber      (501) staff       (20)      808 2023-05-24 23:09:02.097948 zaber_motion-3.4.1/PKG-INFO
--rw-r--r--   0 zaber      (501) staff       (20)      218 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/README.md
--rw-r--r--   0 zaber      (501) staff       (20)      134 2023-05-24 23:09:02.098187 zaber_motion-3.4.1/setup.cfg
--rw-r--r--   0 zaber      (501) staff       (20)     1371 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/setup.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-24 23:09:02.076913 zaber_motion-3.4.1/test/
--rw-r--r--   0 zaber      (501) staff       (20)     3544 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/test/test_integration.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-24 23:09:02.078971 zaber_motion-3.4.1/zaber_motion/
--rw-r--r--   0 zaber      (501) staff       (20)     6545 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/__init__.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-24 23:09:02.085046 zaber_motion-3.4.1/zaber_motion/ascii/
--rw-r--r--   0 zaber      (501) staff       (20)     2604 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     2185 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/alert_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     8708 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/all_axes.py
--rw-r--r--   0 zaber      (501) staff       (20)    40795 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/axis.py
--rw-r--r--   0 zaber      (501) staff       (20)     2259 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/axis_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)    12689 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/axis_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      272 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     1265 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/can_set_state_axis_response.py
--rw-r--r--   0 zaber      (501) staff       (20)     1530 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/can_set_state_device_response.py
--rw-r--r--   0 zaber      (501) staff       (20)    36081 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/connection.py
--rw-r--r--   0 zaber      (501) staff       (20)     1887 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/conversion_factor.py
--rw-r--r--   0 zaber      (501) staff       (20)    24838 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/device.py
--rw-r--r--   0 zaber      (501) staff       (20)     2801 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/device_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)    17751 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/device_io.py
--rw-r--r--   0 zaber      (501) staff       (20)     2077 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/device_io_info.py
--rw-r--r--   0 zaber      (501) staff       (20)    10347 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/device_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)    36231 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/lockstep.py
--rw-r--r--   0 zaber      (501) staff       (20)     1671 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/lockstep_axes.py
--rw-r--r--   0 zaber      (501) staff       (20)      386 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/message_type.py
--rw-r--r--   0 zaber      (501) staff       (20)    15804 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/oscilloscope.py
--rw-r--r--   0 zaber      (501) staff       (20)     1303 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/oscilloscope_capture_properties.py
--rw-r--r--   0 zaber      (501) staff       (20)     4860 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/oscilloscope_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1601 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/paramset_info.py
--rw-r--r--   0 zaber      (501) staff       (20)     2078 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/pid_tuning.py
--rw-r--r--   0 zaber      (501) staff       (20)     2094 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/pvt_axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)      256 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/pvt_axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3190 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/pvt_buffer.py
--rw-r--r--   0 zaber      (501) staff       (20)      247 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/pvt_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)    32301 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/pvt_sequence.py
--rw-r--r--   0 zaber      (501) staff       (20)     2896 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/response.py
--rw-r--r--   0 zaber      (501) staff       (20)    19220 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/servo_tuner.py
--rw-r--r--   0 zaber      (501) staff       (20)     1801 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/servo_tuning_param.py
--rw-r--r--   0 zaber      (501) staff       (20)      384 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/servo_tuning_paramset.py
--rw-r--r--   0 zaber      (501) staff       (20)    22658 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/setting_constants.py
--rw-r--r--   0 zaber      (501) staff       (20)     1893 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/simple_tuning_param_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)    26082 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/storage.py
--rw-r--r--   0 zaber      (501) staff       (20)    75822 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/stream.py
--rw-r--r--   0 zaber      (501) staff       (20)     2133 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/stream_axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)      253 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/stream_axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3084 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/stream_buffer.py
--rw-r--r--   0 zaber      (501) staff       (20)      273 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/stream_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)     5345 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/transport.py
--rw-r--r--   0 zaber      (501) staff       (20)     2966 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/unknown_response_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     2855 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/warning_flags.py
--rw-r--r--   0 zaber      (501) staff       (20)     5066 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/ascii/warnings.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-24 23:09:02.086580 zaber_motion-3.4.1/zaber_motion/binary/
--rw-r--r--   0 zaber      (501) staff       (20)      653 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/binary/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     1941 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/binary/binary_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)     3132 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/binary/command_code.py
--rw-r--r--   0 zaber      (501) staff       (20)    19348 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/binary/connection.py
--rw-r--r--   0 zaber      (501) staff       (20)    28560 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/binary/device.py
--rw-r--r--   0 zaber      (501) staff       (20)     3361 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/binary/device_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)     3346 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/binary/device_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      276 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/binary/device_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3116 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/binary/error_code.py
--rw-r--r--   0 zaber      (501) staff       (20)     1498 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/binary/message.py
--rw-r--r--   0 zaber      (501) staff       (20)      415 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/binary/reply_code.py
--rw-r--r--   0 zaber      (501) staff       (20)     1552 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/binary/reply_only_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     1588 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/binary/unknown_response_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     1153 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/bindings.py
--rw-r--r--   0 zaber      (501) staff       (20)     4196 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/call.py
--rw-r--r--   0 zaber      (501) staff       (20)     7349 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/convert_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      257 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/device_db_source_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     2200 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/events.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-24 23:09:02.095780 zaber_motion-3.4.1/zaber_motion/exceptions/
--rw-r--r--   0 zaber      (501) staff       (20)     7384 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     1121 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/binary_command_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      991 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/binary_command_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1045 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/command_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     3097 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/command_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/command_preempted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1129 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/command_too_long_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1971 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/command_too_long_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      304 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/connection_closed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      292 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/connection_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/conversion_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1158 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/device_address_conflict_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1126 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/device_address_conflict_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      314 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/device_busy_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1092 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/device_db_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      911 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/device_db_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      283 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/device_detection_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      335 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/device_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      317 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/device_not_identified_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1065 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/g_code_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1321 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/g_code_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1036 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/g_code_syntax_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1300 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/g_code_syntax_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      309 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/internal_error_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      295 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/invalid_argument_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      300 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/invalid_data_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      310 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/invalid_operation_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1058 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/invalid_packet_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1198 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/invalid_packet_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      282 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/invalid_park_state_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1140 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/invalid_pvt_point.py
--rw-r--r--   0 zaber      (501) staff       (20)     1091 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/invalid_response_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      928 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/invalid_response_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      342 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/io_channel_out_of_range_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      297 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/io_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      322 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/lockstep_enabled_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      329 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/lockstep_not_enabled_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      396 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/motion_lib_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1070 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1852 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1137 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1875 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      292 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/no_device_found_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      297 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/no_value_for_key_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/not_supported_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/os_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      317 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/out_of_request_ids_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      323 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/pvt_discontinuity_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1037 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/pvt_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1749 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/pvt_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      326 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/pvt_mode_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1102 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/pvt_movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1292 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/pvt_movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1169 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/pvt_movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1327 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      285 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/pvt_setup_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      300 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/request_timeout_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      349 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/serial_port_busy_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     3563 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/set_device_state_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1085 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/set_device_state_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     2372 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/set_peripheral_state_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1120 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/setting_not_found_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      320 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/stream_discontinuity_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1060 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/stream_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1232 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/stream_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      323 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/stream_mode_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1134 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/stream_movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1313 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/stream_movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1199 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/stream_movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1348 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      282 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/stream_setup_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      341 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/timeout_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      320 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/transport_already_used_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      335 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/exceptions/unknown_request_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     2106 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/firmware_version.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-24 23:09:02.096959 zaber_motion-3.4.1/zaber_motion/gcode/
--rw-r--r--   0 zaber      (501) staff       (20)      578 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/gcode/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     2269 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/gcode/axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)     1571 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/gcode/axis_mapping.py
--rw-r--r--   0 zaber      (501) staff       (20)     2170 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/gcode/axis_transformation.py
--rw-r--r--   0 zaber      (501) staff       (20)     2313 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/gcode/device_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)    12275 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/gcode/offline_translator.py
--rw-r--r--   0 zaber      (501) staff       (20)     1555 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/gcode/translate_message.py
--rw-r--r--   0 zaber      (501) staff       (20)     1401 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/gcode/translate_result.py
--rw-r--r--   0 zaber      (501) staff       (20)    12899 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/gcode/translator.py
--rw-r--r--   0 zaber      (501) staff       (20)     2225 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/gcode/translator_config.py
--rw-r--r--   0 zaber      (501) staff       (20)     2838 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/library.py
--rw-r--r--   0 zaber      (501) staff       (20)      279 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/log_output_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)     1519 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/measurement.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-24 23:09:02.097195 zaber_motion-3.4.1/zaber_motion/microscopy/
--rw-r--r--   0 zaber      (501) staff       (20)       68 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/microscopy/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     6181 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/microscopy/objective_changer.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-24 23:09:02.097653 zaber_motion-3.4.1/zaber_motion/protobufs/
--rw-r--r--   0 zaber      (501) staff       (20)        0 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/protobufs/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)    65838 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/protobufs/main_pb2.py
--rw-r--r--   0 zaber      (501) staff       (20)   200831 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/protobufs/main_pb2.pyi
--rw-r--r--   0 zaber      (501) staff       (20)        0 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/py.typed
--rw-r--r--   0 zaber      (501) staff       (20)      278 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/rotation_direction.py
--rw-r--r--   0 zaber      (501) staff       (20)      987 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/serialization.py
--rw-r--r--   0 zaber      (501) staff       (20)     2108 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/tools.py
--rw-r--r--   0 zaber      (501) staff       (20)     5744 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/units.py
--rw-r--r--   0 zaber      (501) staff       (20)       22 2023-05-24 23:08:14.000000 zaber_motion-3.4.1/zaber_motion/version.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-24 23:09:02.079534 zaber_motion-3.4.1/zaber_motion.egg-info/
--rw-r--r--   0 zaber      (501) staff       (20)      808 2023-05-24 23:09:02.000000 zaber_motion-3.4.1/zaber_motion.egg-info/PKG-INFO
--rw-r--r--   0 zaber      (501) staff       (20)     7588 2023-05-24 23:09:02.000000 zaber_motion-3.4.1/zaber_motion.egg-info/SOURCES.txt
--rw-r--r--   0 zaber      (501) staff       (20)        1 2023-05-24 23:09:02.000000 zaber_motion-3.4.1/zaber_motion.egg-info/dependency_links.txt
--rw-r--r--   0 zaber      (501) staff       (20)      239 2023-05-24 23:09:02.000000 zaber_motion-3.4.1/zaber_motion.egg-info/requires.txt
--rw-r--r--   0 zaber      (501) staff       (20)       13 2023-05-24 23:09:02.000000 zaber_motion-3.4.1/zaber_motion.egg-info/top_level.txt
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-26 22:59:02.165151 zaber_motion-3.4.2/
+-rw-r--r--   0 zaber      (501) staff       (20)      218 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/DESCRIPTION.md
+-rw-r--r--   0 zaber      (501) staff       (20)   109244 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/LICENSE.txt
+-rw-r--r--   0 zaber      (501) staff       (20)       13 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/MANIFEST.in
+-rw-r--r--   0 zaber      (501) staff       (20)      808 2023-05-26 22:59:02.165219 zaber_motion-3.4.2/PKG-INFO
+-rw-r--r--   0 zaber      (501) staff       (20)      218 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/README.md
+-rw-r--r--   0 zaber      (501) staff       (20)      134 2023-05-26 22:59:02.165476 zaber_motion-3.4.2/setup.cfg
+-rw-r--r--   0 zaber      (501) staff       (20)     1371 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/setup.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-26 22:59:02.143803 zaber_motion-3.4.2/test/
+-rw-r--r--   0 zaber      (501) staff       (20)     3544 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/test/test_integration.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-26 22:59:02.145672 zaber_motion-3.4.2/zaber_motion/
+-rw-r--r--   0 zaber      (501) staff       (20)     6583 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/__init__.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-26 22:59:02.152082 zaber_motion-3.4.2/zaber_motion/ascii/
+-rw-r--r--   0 zaber      (501) staff       (20)     2604 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2185 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/alert_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     8708 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/all_axes.py
+-rw-r--r--   0 zaber      (501) staff       (20)    41645 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/axis.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2259 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/axis_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12952 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/axis_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      272 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1265 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/can_set_state_axis_response.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1530 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/can_set_state_device_response.py
+-rw-r--r--   0 zaber      (501) staff       (20)    36081 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/connection.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1978 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/conversion_factor.py
+-rw-r--r--   0 zaber      (501) staff       (20)    24838 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/device.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2801 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/device_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)    17751 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/device_io.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2077 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/device_io_info.py
+-rw-r--r--   0 zaber      (501) staff       (20)    10610 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/device_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)    37243 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/lockstep.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1671 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/lockstep_axes.py
+-rw-r--r--   0 zaber      (501) staff       (20)      386 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/message_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)    16036 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/oscilloscope.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1303 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/oscilloscope_capture_properties.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5017 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/oscilloscope_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1601 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/paramset_info.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2078 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/pid_tuning.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2094 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/pvt_axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)      256 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/pvt_axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3190 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/pvt_buffer.py
+-rw-r--r--   0 zaber      (501) staff       (20)      247 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/pvt_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)    32301 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/pvt_sequence.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2896 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/response.py
+-rw-r--r--   0 zaber      (501) staff       (20)    19220 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/servo_tuner.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1801 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/servo_tuning_param.py
+-rw-r--r--   0 zaber      (501) staff       (20)      384 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/servo_tuning_paramset.py
+-rw-r--r--   0 zaber      (501) staff       (20)    22658 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/setting_constants.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1893 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/simple_tuning_param_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)    26082 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/storage.py
+-rw-r--r--   0 zaber      (501) staff       (20)    76318 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/stream.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2133 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/stream_axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)      253 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/stream_axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3084 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/stream_buffer.py
+-rw-r--r--   0 zaber      (501) staff       (20)      273 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/stream_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5345 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/transport.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2966 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/unknown_response_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2855 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/warning_flags.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5066 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/ascii/warnings.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-26 22:59:02.153754 zaber_motion-3.4.2/zaber_motion/binary/
+-rw-r--r--   0 zaber      (501) staff       (20)      653 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/binary/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1941 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/binary/binary_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3132 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/binary/command_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)    19348 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/binary/connection.py
+-rw-r--r--   0 zaber      (501) staff       (20)    29083 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/binary/device.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3361 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/binary/device_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3513 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/binary/device_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      276 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/binary/device_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3116 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/binary/error_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1498 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/binary/message.py
+-rw-r--r--   0 zaber      (501) staff       (20)      415 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/binary/reply_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1552 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/binary/reply_only_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1588 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/binary/unknown_response_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1153 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/bindings.py
+-rw-r--r--   0 zaber      (501) staff       (20)     4196 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/call.py
+-rw-r--r--   0 zaber      (501) staff       (20)     7349 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/convert_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      257 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/device_db_source_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2200 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/events.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-26 22:59:02.163086 zaber_motion-3.4.2/zaber_motion/exceptions/
+-rw-r--r--   0 zaber      (501) staff       (20)     7384 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1121 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/binary_command_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      991 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/binary_command_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1045 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/command_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3097 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/command_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/command_preempted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1129 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/command_too_long_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1971 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/command_too_long_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      304 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/connection_closed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/connection_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/conversion_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1158 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/device_address_conflict_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1126 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/device_address_conflict_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      314 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/device_busy_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1092 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/device_db_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      911 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/device_db_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      283 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/device_detection_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      335 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/device_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      317 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/device_not_identified_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1065 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/g_code_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1321 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/g_code_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1036 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/g_code_syntax_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1300 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/g_code_syntax_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      309 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/internal_error_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      295 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/invalid_argument_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      300 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/invalid_data_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      310 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/invalid_operation_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1058 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/invalid_packet_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1198 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/invalid_packet_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      282 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/invalid_park_state_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1140 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/invalid_pvt_point.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1091 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/invalid_response_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      928 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/invalid_response_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      342 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/io_channel_out_of_range_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      297 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/io_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      322 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/lockstep_enabled_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      329 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/lockstep_not_enabled_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      396 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/motion_lib_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1070 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1852 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1137 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1875 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/no_device_found_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      297 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/no_value_for_key_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/not_supported_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/os_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      317 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/out_of_request_ids_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      323 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/pvt_discontinuity_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1037 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/pvt_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1749 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/pvt_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      326 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/pvt_mode_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1102 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/pvt_movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1292 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/pvt_movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1169 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/pvt_movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1327 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      285 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/pvt_setup_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      300 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/request_timeout_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      349 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/serial_port_busy_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3563 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/set_device_state_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1085 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/set_device_state_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2372 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/set_peripheral_state_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1120 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/setting_not_found_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      320 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/stream_discontinuity_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1060 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/stream_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1232 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/stream_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      323 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/stream_mode_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1134 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/stream_movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1313 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/stream_movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1199 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/stream_movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1348 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      282 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/stream_setup_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      341 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/timeout_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      320 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/transport_already_used_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      335 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/exceptions/unknown_request_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2106 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/firmware_version.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-26 22:59:02.164294 zaber_motion-3.4.2/zaber_motion/gcode/
+-rw-r--r--   0 zaber      (501) staff       (20)      578 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/gcode/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2269 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/gcode/axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1571 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/gcode/axis_mapping.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2170 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/gcode/axis_transformation.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2313 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/gcode/device_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12481 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/gcode/offline_translator.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1555 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/gcode/translate_message.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1401 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/gcode/translate_result.py
+-rw-r--r--   0 zaber      (501) staff       (20)    13105 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/gcode/translator.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2225 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/gcode/translator_config.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2838 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/library.py
+-rw-r--r--   0 zaber      (501) staff       (20)      279 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/log_output_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1610 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/measurement.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-26 22:59:02.164531 zaber_motion-3.4.2/zaber_motion/microscopy/
+-rw-r--r--   0 zaber      (501) staff       (20)       68 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/microscopy/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     6181 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/microscopy/objective_changer.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-26 22:59:02.164911 zaber_motion-3.4.2/zaber_motion/protobufs/
+-rw-r--r--   0 zaber      (501) staff       (20)        0 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/protobufs/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)    65838 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/protobufs/main_pb2.py
+-rw-r--r--   0 zaber      (501) staff       (20)   200831 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/protobufs/main_pb2.pyi
+-rw-r--r--   0 zaber      (501) staff       (20)        0 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/py.typed
+-rw-r--r--   0 zaber      (501) staff       (20)      278 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/rotation_direction.py
+-rw-r--r--   0 zaber      (501) staff       (20)      987 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/serialization.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2108 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/tools.py
+-rw-r--r--   0 zaber      (501) staff       (20)     9021 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/units.py
+-rw-r--r--   0 zaber      (501) staff       (20)       22 2023-05-26 22:58:15.000000 zaber_motion-3.4.2/zaber_motion/version.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-05-26 22:59:02.146237 zaber_motion-3.4.2/zaber_motion.egg-info/
+-rw-r--r--   0 zaber      (501) staff       (20)      808 2023-05-26 22:59:02.000000 zaber_motion-3.4.2/zaber_motion.egg-info/PKG-INFO
+-rw-r--r--   0 zaber      (501) staff       (20)     7588 2023-05-26 22:59:02.000000 zaber_motion-3.4.2/zaber_motion.egg-info/SOURCES.txt
+-rw-r--r--   0 zaber      (501) staff       (20)        1 2023-05-26 22:59:02.000000 zaber_motion-3.4.2/zaber_motion.egg-info/dependency_links.txt
+-rw-r--r--   0 zaber      (501) staff       (20)      239 2023-05-26 22:59:02.000000 zaber_motion-3.4.2/zaber_motion.egg-info/requires.txt
+-rw-r--r--   0 zaber      (501) staff       (20)       13 2023-05-26 22:59:02.000000 zaber_motion-3.4.2/zaber_motion.egg-info/top_level.txt
```

### Comparing `zaber_motion-3.4.1/LICENSE.txt` & `zaber_motion-3.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/PKG-INFO` & `zaber_motion-3.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: zaber_motion
-Version: 3.4.1
+Version: 3.4.2
 Summary: A library for communicating with Zaber devices
 Home-page: https://gitlab.com/ZaberTech/zaber-motion-lib
 Author: Zaber Technologies Inc.
 Author-email: contact@zaber.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Zaber Motion Library
 
 Zaber Motion Library is a multi-platform library used to operate Zaber devices.
```

### Comparing `zaber_motion-3.4.1/setup.py` & `zaber_motion-3.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read_from_file(*filename):
     with open(path.join(*filename), 'r') as f:
         return f.read()
 
 
 setup(
     name='zaber_motion',
-    version='3.4.1',
+    version='3.4.2',
     packages=find_packages(exclude=["test*", "test_*", "*_test*"]),
     package_data={
         '': ['*.pyi', 'py.typed']
     },
     description='A library for communicating with Zaber devices',
     long_description=read_from_file('DESCRIPTION.md'),
     long_description_content_type="text/markdown",
@@ -28,16 +28,16 @@
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
     ],
     keywords='',
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=[
         'protobuf>=3.20.0,<4.22.0',
         'rx>=3.0.0',
-        'zaber_motion_bindings_windows==3.4.1;platform_system=="Windows"',
-        'zaber_motion_bindings_linux==3.4.1;platform_system=="Linux"',
-        'zaber_motion_bindings_darwin==3.4.1;platform_system=="Darwin"',
+        'zaber_motion_bindings_windows==3.4.2;platform_system=="Windows"',
+        'zaber_motion_bindings_linux==3.4.2;platform_system=="Linux"',
+        'zaber_motion_bindings_darwin==3.4.2;platform_system=="Darwin"',
     ],
 )
```

### Comparing `zaber_motion-3.4.1/test/test_integration.py` & `zaber_motion-3.4.2/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/__init__.py` & `zaber_motion-3.4.2/zaber_motion/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from .protobufs import main_pb2 as protobufs
-from .units import Units as Units
+from .units import UnitsAndLiterals as UnitsAndLiterals, Units as Units
 from .library import Library as Library
 from .log_output_mode import LogOutputMode as LogOutputMode
 from .tools import Tools as Tools
 from .device_db_source_type import DeviceDbSourceType as DeviceDbSourceType
 from .measurement import Measurement as Measurement
 from .convert_exception import convert_exception as convert_exception
 from .firmware_version import FirmwareVersion as FirmwareVersion
```

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/__init__.py` & `zaber_motion-3.4.2/zaber_motion/ascii/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/alert_event.py` & `zaber_motion-3.4.2/zaber_motion/ascii/alert_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/all_axes.py` & `zaber_motion-3.4.2/zaber_motion/ascii/all_axes.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/axis.py` & `zaber_motion-3.4.2/zaber_motion/ascii/axis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import TYPE_CHECKING, List
 from ..call import call, call_async, call_sync
 
 from ..protobufs import main_pb2
-from ..units import Units
+from ..units import Units, units_from_literals, LengthUnits, VelocityUnits, AccelerationUnits
 from .warnings import Warnings
 from .axis_settings import AxisSettings
 from .axis_identity import AxisIdentity
 from .storage import AxisStorage
 from .axis_type import AxisType
 from .response import Response
 from ..measurement import Measurement
@@ -355,20 +355,20 @@
         response = main_pb2.BoolResponse()
         await call_async("device/is_homed", request, response)
         return response.value
 
     def move_absolute(
             self,
             position: float,
-            unit: Units = Units.NATIVE,
+            unit: LengthUnits = Units.NATIVE,
             wait_until_idle: bool = True,
             velocity: float = 0,
-            velocity_unit: Units = Units.NATIVE,
+            velocity_unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Move axis to absolute position.
 
         Args:
             position: Absolute position.
             unit: Units of position.
@@ -384,31 +384,31 @@
         """
         request = main_pb2.DeviceMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.axis = self.axis_number
         request.type = main_pb2.DeviceMoveRequest.ABS
         request.arg = position
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.wait_until_idle = wait_until_idle
         request.velocity = velocity
-        request.velocity_unit = velocity_unit.value
+        request.velocity_unit = units_from_literals(velocity_unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         call("device/move", request)
 
     async def move_absolute_async(
             self,
             position: float,
-            unit: Units = Units.NATIVE,
+            unit: LengthUnits = Units.NATIVE,
             wait_until_idle: bool = True,
             velocity: float = 0,
-            velocity_unit: Units = Units.NATIVE,
+            velocity_unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Move axis to absolute position.
 
         Args:
             position: Absolute position.
             unit: Units of position.
@@ -424,29 +424,29 @@
         """
         request = main_pb2.DeviceMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.axis = self.axis_number
         request.type = main_pb2.DeviceMoveRequest.ABS
         request.arg = position
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.wait_until_idle = wait_until_idle
         request.velocity = velocity
-        request.velocity_unit = velocity_unit.value
+        request.velocity_unit = units_from_literals(velocity_unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         await call_async("device/move", request)
 
     def move_max(
             self,
             wait_until_idle: bool = True,
             velocity: float = 0,
-            velocity_unit: Units = Units.NATIVE,
+            velocity_unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Moves the axis to the maximum position as specified by limit.max.
 
         Args:
             wait_until_idle: Determines whether function should return after the movement is finished or just started.
             velocity: Movement velocity.
@@ -461,26 +461,26 @@
         request = main_pb2.DeviceMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.axis = self.axis_number
         request.type = main_pb2.DeviceMoveRequest.MAX
         request.wait_until_idle = wait_until_idle
         request.velocity = velocity
-        request.velocity_unit = velocity_unit.value
+        request.velocity_unit = units_from_literals(velocity_unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         call("device/move", request)
 
     async def move_max_async(
             self,
             wait_until_idle: bool = True,
             velocity: float = 0,
-            velocity_unit: Units = Units.NATIVE,
+            velocity_unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Moves the axis to the maximum position as specified by limit.max.
 
         Args:
             wait_until_idle: Determines whether function should return after the movement is finished or just started.
             velocity: Movement velocity.
@@ -495,26 +495,26 @@
         request = main_pb2.DeviceMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.axis = self.axis_number
         request.type = main_pb2.DeviceMoveRequest.MAX
         request.wait_until_idle = wait_until_idle
         request.velocity = velocity
-        request.velocity_unit = velocity_unit.value
+        request.velocity_unit = units_from_literals(velocity_unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         await call_async("device/move", request)
 
     def move_min(
             self,
             wait_until_idle: bool = True,
             velocity: float = 0,
-            velocity_unit: Units = Units.NATIVE,
+            velocity_unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Moves the axis to the minimum position as specified by limit.min.
 
         Args:
             wait_until_idle: Determines whether function should return after the movement is finished or just started.
             velocity: Movement velocity.
@@ -529,26 +529,26 @@
         request = main_pb2.DeviceMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.axis = self.axis_number
         request.type = main_pb2.DeviceMoveRequest.MIN
         request.wait_until_idle = wait_until_idle
         request.velocity = velocity
-        request.velocity_unit = velocity_unit.value
+        request.velocity_unit = units_from_literals(velocity_unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         call("device/move", request)
 
     async def move_min_async(
             self,
             wait_until_idle: bool = True,
             velocity: float = 0,
-            velocity_unit: Units = Units.NATIVE,
+            velocity_unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Moves the axis to the minimum position as specified by limit.min.
 
         Args:
             wait_until_idle: Determines whether function should return after the movement is finished or just started.
             velocity: Movement velocity.
@@ -563,28 +563,28 @@
         request = main_pb2.DeviceMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.axis = self.axis_number
         request.type = main_pb2.DeviceMoveRequest.MIN
         request.wait_until_idle = wait_until_idle
         request.velocity = velocity
-        request.velocity_unit = velocity_unit.value
+        request.velocity_unit = units_from_literals(velocity_unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         await call_async("device/move", request)
 
     def move_relative(
             self,
             position: float,
-            unit: Units = Units.NATIVE,
+            unit: LengthUnits = Units.NATIVE,
             wait_until_idle: bool = True,
             velocity: float = 0,
-            velocity_unit: Units = Units.NATIVE,
+            velocity_unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Move axis to position relative to current position.
 
         Args:
             position: Relative position.
             unit: Units of position.
@@ -600,31 +600,31 @@
         """
         request = main_pb2.DeviceMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.axis = self.axis_number
         request.type = main_pb2.DeviceMoveRequest.REL
         request.arg = position
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.wait_until_idle = wait_until_idle
         request.velocity = velocity
-        request.velocity_unit = velocity_unit.value
+        request.velocity_unit = units_from_literals(velocity_unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         call("device/move", request)
 
     async def move_relative_async(
             self,
             position: float,
-            unit: Units = Units.NATIVE,
+            unit: LengthUnits = Units.NATIVE,
             wait_until_idle: bool = True,
             velocity: float = 0,
-            velocity_unit: Units = Units.NATIVE,
+            velocity_unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Move axis to position relative to current position.
 
         Args:
             position: Relative position.
             unit: Units of position.
@@ -640,28 +640,28 @@
         """
         request = main_pb2.DeviceMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.axis = self.axis_number
         request.type = main_pb2.DeviceMoveRequest.REL
         request.arg = position
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.wait_until_idle = wait_until_idle
         request.velocity = velocity
-        request.velocity_unit = velocity_unit.value
+        request.velocity_unit = units_from_literals(velocity_unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         await call_async("device/move", request)
 
     def move_velocity(
             self,
             velocity: float,
-            unit: Units = Units.NATIVE,
+            unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Begins to move axis at specified speed.
 
         Args:
             velocity: Movement velocity.
             unit: Units of velocity.
@@ -672,25 +672,25 @@
         """
         request = main_pb2.DeviceMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.axis = self.axis_number
         request.type = main_pb2.DeviceMoveRequest.VEL
         request.arg = velocity
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         call("device/move", request)
 
     async def move_velocity_async(
             self,
             velocity: float,
-            unit: Units = Units.NATIVE,
+            unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Begins to move axis at specified speed.
 
         Args:
             velocity: Movement velocity.
             unit: Units of velocity.
@@ -701,22 +701,22 @@
         """
         request = main_pb2.DeviceMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.axis = self.axis_number
         request.type = main_pb2.DeviceMoveRequest.VEL
         request.arg = velocity
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         await call_async("device/move", request)
 
     def get_position(
             self,
-            unit: Units = Units.NATIVE
+            unit: LengthUnits = Units.NATIVE
     ) -> float:
         """
         Returns current axis position.
 
         Args:
             unit: Units of position.
 
@@ -724,22 +724,22 @@
             Axis position.
         """
         request = main_pb2.DeviceGetSettingRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.axis = self.axis_number
         request.setting = "pos"
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call("device/get_setting", request, response)
         return response.value
 
     async def get_position_async(
             self,
-            unit: Units = Units.NATIVE
+            unit: LengthUnits = Units.NATIVE
     ) -> float:
         """
         Returns current axis position.
 
         Args:
             unit: Units of position.
 
@@ -747,15 +747,15 @@
             Axis position.
         """
         request = main_pb2.DeviceGetSettingRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.axis = self.axis_number
         request.setting = "pos"
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         await call_async("device/get_setting", request, response)
         return response.value
 
     def generic_command(
             self,
             command: str,
```

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/axis_identity.py` & `zaber_motion-3.4.2/zaber_motion/ascii/axis_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/axis_settings.py` & `zaber_motion-3.4.2/zaber_motion/ascii/axis_settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import TYPE_CHECKING, List
 from ..call import call, call_async, call_sync
 
 from ..protobufs import main_pb2
-from ..units import Units
+from ..units import UnitsAndLiterals, Units, units_from_literals
 from .conversion_factor import ConversionFactor
 
 if TYPE_CHECKING:
     from .axis import Axis
 
 
 class AxisSettings:
@@ -19,15 +19,15 @@
 
     def __init__(self, axis: 'Axis'):
         self._axis = axis
 
     def get(
             self,
             setting: str,
-            unit: Units = Units.NATIVE
+            unit: UnitsAndLiterals = Units.NATIVE
     ) -> float:
         """
         Returns any axis setting or property.
         For more information refer to the [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_settings).
 
         Args:
             setting: Name of the setting.
@@ -37,23 +37,23 @@
             Setting value.
         """
         request = main_pb2.DeviceGetSettingRequest()
         request.interface_id = self._axis.device.connection.interface_id
         request.device = self._axis.device.device_address
         request.axis = self._axis.axis_number
         request.setting = setting
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call("device/get_setting", request, response)
         return response.value
 
     async def get_async(
             self,
             setting: str,
-            unit: Units = Units.NATIVE
+            unit: UnitsAndLiterals = Units.NATIVE
     ) -> float:
         """
         Returns any axis setting or property.
         For more information refer to the [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_settings).
 
         Args:
             setting: Name of the setting.
@@ -63,24 +63,24 @@
             Setting value.
         """
         request = main_pb2.DeviceGetSettingRequest()
         request.interface_id = self._axis.device.connection.interface_id
         request.device = self._axis.device.device_address
         request.axis = self._axis.axis_number
         request.setting = setting
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         await call_async("device/get_setting", request, response)
         return response.value
 
     def set(
             self,
             setting: str,
             value: float,
-            unit: Units = Units.NATIVE
+            unit: UnitsAndLiterals = Units.NATIVE
     ) -> None:
         """
         Sets any axis setting.
         For more information refer to the [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_settings).
 
         Args:
             setting: Name of the setting.
@@ -89,22 +89,22 @@
         """
         request = main_pb2.DeviceSetSettingRequest()
         request.interface_id = self._axis.device.connection.interface_id
         request.device = self._axis.device.device_address
         request.axis = self._axis.axis_number
         request.setting = setting
         request.value = value
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         call("device/set_setting", request)
 
     async def set_async(
             self,
             setting: str,
             value: float,
-            unit: Units = Units.NATIVE
+            unit: UnitsAndLiterals = Units.NATIVE
     ) -> None:
         """
         Sets any axis setting.
         For more information refer to the [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_settings).
 
         Args:
             setting: Name of the setting.
@@ -113,15 +113,15 @@
         """
         request = main_pb2.DeviceSetSettingRequest()
         request.interface_id = self._axis.device.connection.interface_id
         request.device = self._axis.device.device_address
         request.axis = self._axis.axis_number
         request.setting = setting
         request.value = value
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         await call_async("device/set_setting", request)
 
     def get_string(
             self,
             setting: str
     ) -> str:
         """
@@ -208,15 +208,15 @@
         request.value = value
         await call_async("device/set_setting_str", request)
 
     def convert_to_native_units(
             self,
             setting: str,
             value: float,
-            unit: Units
+            unit: UnitsAndLiterals
     ) -> float:
         """
         Convert arbitrary setting value to Zaber native units.
 
         Args:
             setting: Name of the setting.
             value: Value of the setting in units specified by following argument.
@@ -227,24 +227,24 @@
         """
         request = main_pb2.DeviceConvertSettingRequest()
         request.interface_id = self._axis.device.connection.interface_id
         request.device = self._axis.device.device_address
         request.axis = self._axis.axis_number
         request.setting = setting
         request.value = value
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call_sync("device/convert_setting", request, response)
         return response.value
 
     def convert_from_native_units(
             self,
             setting: str,
             value: float,
-            unit: Units
+            unit: UnitsAndLiterals
     ) -> float:
         """
         Convert arbitrary setting value from Zaber native units.
 
         Args:
             setting: Name of the setting.
             value: Value of the setting in Zaber native units.
@@ -256,23 +256,23 @@
         request = main_pb2.DeviceConvertSettingRequest()
         request.interface_id = self._axis.device.connection.interface_id
         request.device = self._axis.device.device_address
         request.axis = self._axis.axis_number
         request.from_native = True
         request.setting = setting
         request.value = value
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call_sync("device/convert_setting", request, response)
         return response.value
 
     def get_default(
             self,
             setting: str,
-            unit: Units = Units.NATIVE
+            unit: UnitsAndLiterals = Units.NATIVE
     ) -> float:
         """
         Returns the default value of a setting.
 
         Args:
             setting: Name of the setting.
             unit: Units of setting.
@@ -281,15 +281,15 @@
             Default setting value.
         """
         request = main_pb2.DeviceGetSettingRequest()
         request.interface_id = self._axis.device.connection.interface_id
         request.device = self._axis.device.device_address
         request.axis = self._axis.axis_number
         request.setting = setting
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call_sync("device/get_setting_default", request, response)
         return response.value
 
     def get_default_string(
             self,
             setting: str
```

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/can_set_state_axis_response.py` & `zaber_motion-3.4.2/zaber_motion/ascii/can_set_state_axis_response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/can_set_state_device_response.py` & `zaber_motion-3.4.2/zaber_motion/ascii/can_set_state_device_response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/connection.py` & `zaber_motion-3.4.2/zaber_motion/ascii/connection.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/conversion_factor.py` & `zaber_motion-3.4.2/zaber_motion/ascii/conversion_factor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 # pylint: disable=W0201
 
 from typing import Optional  # pylint: disable=unused-import
 from ..protobufs import main_pb2
-from ..units import Units
+from ..units import UnitsAndLiterals, Units, units_from_literals
 
 
 class ConversionFactor:
     """
     Represents unit conversion factor for a single dimension.
     """
 
     def __init__(
             self: 'ConversionFactor',
             setting: str,
             value: float,
-            unit: Units
+            unit: UnitsAndLiterals
     ) -> None:
         self._setting = setting
         self._value = value
         self._unit = unit
 
     @property
     def setting(self) -> str:
@@ -43,23 +43,23 @@
         return self._value
 
     @value.setter
     def value(self, value: float) -> None:
         self._value = value
 
     @property
-    def unit(self) -> Units:
+    def unit(self) -> UnitsAndLiterals:
         """
         Units of the value.
         """
 
         return self._unit
 
     @unit.setter
-    def unit(self, value: Units) -> None:
+    def unit(self, value: UnitsAndLiterals) -> None:
         self._unit = value
 
     def __repr__(self) -> str:
         return str(self.__dict__)
 
     @staticmethod
     def to_protobuf(source: 'Optional[ConversionFactor]') -> main_pb2.ConversionFactor:
@@ -68,9 +68,9 @@
 
         if not isinstance(source, ConversionFactor):
             raise TypeError("Provided value is not ConversionFactor.")
 
         pb_data = main_pb2.ConversionFactor()
         pb_data.setting = source.setting
         pb_data.value = source.value
-        pb_data.unit = (source.unit or Units.NATIVE).value
+        pb_data.unit = units_from_literals(source.unit or Units.NATIVE).value
         return pb_data
```

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/device.py` & `zaber_motion-3.4.2/zaber_motion/ascii/device.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/device_identity.py` & `zaber_motion-3.4.2/zaber_motion/ascii/device_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/device_io.py` & `zaber_motion-3.4.2/zaber_motion/ascii/device_io.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/device_io_info.py` & `zaber_motion-3.4.2/zaber_motion/ascii/device_io_info.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/device_settings.py` & `zaber_motion-3.4.2/zaber_motion/ascii/device_settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import TYPE_CHECKING
 from ..call import call, call_async, call_sync
 
 from ..protobufs import main_pb2
-from ..units import Units
+from ..units import UnitsAndLiterals, Units, units_from_literals
 
 if TYPE_CHECKING:
     from .device import Device
 
 
 class DeviceSettings:
     """
@@ -18,15 +18,15 @@
 
     def __init__(self, device: 'Device'):
         self._device = device
 
     def get(
             self,
             setting: str,
-            unit: Units = Units.NATIVE
+            unit: UnitsAndLiterals = Units.NATIVE
     ) -> float:
         """
         Returns any device setting or property.
         For more information refer to the [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_settings).
 
         Args:
             setting: Name of the setting.
@@ -35,23 +35,23 @@
         Returns:
             Setting value.
         """
         request = main_pb2.DeviceGetSettingRequest()
         request.interface_id = self._device.connection.interface_id
         request.device = self._device.device_address
         request.setting = setting
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call("device/get_setting", request, response)
         return response.value
 
     async def get_async(
             self,
             setting: str,
-            unit: Units = Units.NATIVE
+            unit: UnitsAndLiterals = Units.NATIVE
     ) -> float:
         """
         Returns any device setting or property.
         For more information refer to the [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_settings).
 
         Args:
             setting: Name of the setting.
@@ -60,24 +60,24 @@
         Returns:
             Setting value.
         """
         request = main_pb2.DeviceGetSettingRequest()
         request.interface_id = self._device.connection.interface_id
         request.device = self._device.device_address
         request.setting = setting
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         await call_async("device/get_setting", request, response)
         return response.value
 
     def set(
             self,
             setting: str,
             value: float,
-            unit: Units = Units.NATIVE
+            unit: UnitsAndLiterals = Units.NATIVE
     ) -> None:
         """
         Sets any device setting.
         For more information refer to the [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_settings).
 
         Args:
             setting: Name of the setting.
@@ -85,22 +85,22 @@
             unit: Units of setting.
         """
         request = main_pb2.DeviceSetSettingRequest()
         request.interface_id = self._device.connection.interface_id
         request.device = self._device.device_address
         request.setting = setting
         request.value = value
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         call("device/set_setting", request)
 
     async def set_async(
             self,
             setting: str,
             value: float,
-            unit: Units = Units.NATIVE
+            unit: UnitsAndLiterals = Units.NATIVE
     ) -> None:
         """
         Sets any device setting.
         For more information refer to the [ASCII Protocol Manual](https://www.zaber.com/protocol-manual#topic_settings).
 
         Args:
             setting: Name of the setting.
@@ -108,15 +108,15 @@
             unit: Units of setting.
         """
         request = main_pb2.DeviceSetSettingRequest()
         request.interface_id = self._device.connection.interface_id
         request.device = self._device.device_address
         request.setting = setting
         request.value = value
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         await call_async("device/set_setting", request)
 
     def get_string(
             self,
             setting: str
     ) -> str:
         """
@@ -199,15 +199,15 @@
         request.value = value
         await call_async("device/set_setting_str", request)
 
     def convert_to_native_units(
             self,
             setting: str,
             value: float,
-            unit: Units
+            unit: UnitsAndLiterals
     ) -> float:
         """
         Convert arbitrary setting value to Zaber native units.
 
         Args:
             setting: Name of the setting.
             value: Value of the setting in units specified by following argument.
@@ -217,24 +217,24 @@
             Setting value.
         """
         request = main_pb2.DeviceConvertSettingRequest()
         request.interface_id = self._device.connection.interface_id
         request.device = self._device.device_address
         request.setting = setting
         request.value = value
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call_sync("device/convert_setting", request, response)
         return response.value
 
     def convert_from_native_units(
             self,
             setting: str,
             value: float,
-            unit: Units
+            unit: UnitsAndLiterals
     ) -> float:
         """
         Convert arbitrary setting value from Zaber native units.
 
         Args:
             setting: Name of the setting.
             value: Value of the setting in Zaber native units.
@@ -245,23 +245,23 @@
         """
         request = main_pb2.DeviceConvertSettingRequest()
         request.interface_id = self._device.connection.interface_id
         request.device = self._device.device_address
         request.from_native = True
         request.setting = setting
         request.value = value
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call_sync("device/convert_setting", request, response)
         return response.value
 
     def get_default(
             self,
             setting: str,
-            unit: Units = Units.NATIVE
+            unit: UnitsAndLiterals = Units.NATIVE
     ) -> float:
         """
         Returns the default value of a setting.
 
         Args:
             setting: Name of the setting.
             unit: Units of setting.
@@ -269,15 +269,15 @@
         Returns:
             Default setting value.
         """
         request = main_pb2.DeviceGetSettingRequest()
         request.interface_id = self._device.connection.interface_id
         request.device = self._device.device_address
         request.setting = setting
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call_sync("device/get_setting_default", request, response)
         return response.value
 
     def get_default_string(
             self,
             setting: str
```

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/lockstep.py` & `zaber_motion-3.4.2/zaber_motion/ascii/lockstep.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 from typing import TYPE_CHECKING, List
 from ..protobufs import main_pb2
-from ..units import Units
+from ..units import Units, units_from_literals, LengthUnits, VelocityUnits, AccelerationUnits
 from ..call import call, call_async, call_sync
 from .lockstep_axes import LockstepAxes
 
 if TYPE_CHECKING:
     from .device import Device
 
 
@@ -160,20 +160,20 @@
         request.lockstep_group_id = self.lockstep_group_id
         request.wait_until_idle = wait_until_idle
         await call_async("device/lockstep_home", request)
 
     def move_absolute(
             self,
             position: float,
-            unit: Units = Units.NATIVE,
+            unit: LengthUnits = Units.NATIVE,
             wait_until_idle: bool = True,
             velocity: float = 0,
-            velocity_unit: Units = Units.NATIVE,
+            velocity_unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Move the first axis of the lockstep group to an absolute position.
         The other axes in the lockstep group maintain their offsets throughout movement.
 
         Args:
             position: Absolute position.
@@ -190,31 +190,31 @@
         """
         request = main_pb2.LockstepMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
         request.type = main_pb2.LockstepMoveRequest.ABS
         request.arg = position
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.wait_until_idle = wait_until_idle
         request.velocity = velocity
-        request.velocity_unit = velocity_unit.value
+        request.velocity_unit = units_from_literals(velocity_unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         call("device/lockstep_move", request)
 
     async def move_absolute_async(
             self,
             position: float,
-            unit: Units = Units.NATIVE,
+            unit: LengthUnits = Units.NATIVE,
             wait_until_idle: bool = True,
             velocity: float = 0,
-            velocity_unit: Units = Units.NATIVE,
+            velocity_unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Move the first axis of the lockstep group to an absolute position.
         The other axes in the lockstep group maintain their offsets throughout movement.
 
         Args:
             position: Absolute position.
@@ -231,31 +231,31 @@
         """
         request = main_pb2.LockstepMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
         request.type = main_pb2.LockstepMoveRequest.ABS
         request.arg = position
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.wait_until_idle = wait_until_idle
         request.velocity = velocity
-        request.velocity_unit = velocity_unit.value
+        request.velocity_unit = units_from_literals(velocity_unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         await call_async("device/lockstep_move", request)
 
     def move_relative(
             self,
             position: float,
-            unit: Units = Units.NATIVE,
+            unit: LengthUnits = Units.NATIVE,
             wait_until_idle: bool = True,
             velocity: float = 0,
-            velocity_unit: Units = Units.NATIVE,
+            velocity_unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Move the first axis of the lockstep group to a position relative to its current position.
         The other axes in the lockstep group maintain their offsets throughout movement.
 
         Args:
             position: Relative position.
@@ -272,31 +272,31 @@
         """
         request = main_pb2.LockstepMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
         request.type = main_pb2.LockstepMoveRequest.REL
         request.arg = position
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.wait_until_idle = wait_until_idle
         request.velocity = velocity
-        request.velocity_unit = velocity_unit.value
+        request.velocity_unit = units_from_literals(velocity_unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         call("device/lockstep_move", request)
 
     async def move_relative_async(
             self,
             position: float,
-            unit: Units = Units.NATIVE,
+            unit: LengthUnits = Units.NATIVE,
             wait_until_idle: bool = True,
             velocity: float = 0,
-            velocity_unit: Units = Units.NATIVE,
+            velocity_unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Move the first axis of the lockstep group to a position relative to its current position.
         The other axes in the lockstep group maintain their offsets throughout movement.
 
         Args:
             position: Relative position.
@@ -313,28 +313,28 @@
         """
         request = main_pb2.LockstepMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
         request.type = main_pb2.LockstepMoveRequest.REL
         request.arg = position
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.wait_until_idle = wait_until_idle
         request.velocity = velocity
-        request.velocity_unit = velocity_unit.value
+        request.velocity_unit = units_from_literals(velocity_unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         await call_async("device/lockstep_move", request)
 
     def move_velocity(
             self,
             velocity: float,
-            unit: Units = Units.NATIVE,
+            unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Moves the first axis of the lockstep group at the specified speed.
         The other axes in the lockstep group maintain their offsets throughout movement.
 
         Args:
             velocity: Movement velocity.
@@ -346,25 +346,25 @@
         """
         request = main_pb2.LockstepMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
         request.type = main_pb2.LockstepMoveRequest.VEL
         request.arg = velocity
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         call("device/lockstep_move", request)
 
     async def move_velocity_async(
             self,
             velocity: float,
-            unit: Units = Units.NATIVE,
+            unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Moves the first axis of the lockstep group at the specified speed.
         The other axes in the lockstep group maintain their offsets throughout movement.
 
         Args:
             velocity: Movement velocity.
@@ -376,26 +376,26 @@
         """
         request = main_pb2.LockstepMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
         request.type = main_pb2.LockstepMoveRequest.VEL
         request.arg = velocity
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         await call_async("device/lockstep_move", request)
 
     def move_max(
             self,
             wait_until_idle: bool = True,
             velocity: float = 0,
-            velocity_unit: Units = Units.NATIVE,
+            velocity_unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Moves the axes to the maximum valid position.
         The axes in the lockstep group maintain their offsets throughout movement.
         Respects lim.max for all axes in the group.
 
         Args:
@@ -412,26 +412,26 @@
         request = main_pb2.LockstepMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
         request.type = main_pb2.LockstepMoveRequest.MAX
         request.wait_until_idle = wait_until_idle
         request.velocity = velocity
-        request.velocity_unit = velocity_unit.value
+        request.velocity_unit = units_from_literals(velocity_unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         call("device/lockstep_move", request)
 
     async def move_max_async(
             self,
             wait_until_idle: bool = True,
             velocity: float = 0,
-            velocity_unit: Units = Units.NATIVE,
+            velocity_unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Moves the axes to the maximum valid position.
         The axes in the lockstep group maintain their offsets throughout movement.
         Respects lim.max for all axes in the group.
 
         Args:
@@ -448,26 +448,26 @@
         request = main_pb2.LockstepMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
         request.type = main_pb2.LockstepMoveRequest.MAX
         request.wait_until_idle = wait_until_idle
         request.velocity = velocity
-        request.velocity_unit = velocity_unit.value
+        request.velocity_unit = units_from_literals(velocity_unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         await call_async("device/lockstep_move", request)
 
     def move_min(
             self,
             wait_until_idle: bool = True,
             velocity: float = 0,
-            velocity_unit: Units = Units.NATIVE,
+            velocity_unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Moves the axes to the minimum valid position.
         The axes in the lockstep group maintain their offsets throughout movement.
         Respects lim.min for all axes in the group.
 
         Args:
@@ -484,26 +484,26 @@
         request = main_pb2.LockstepMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
         request.type = main_pb2.LockstepMoveRequest.MIN
         request.wait_until_idle = wait_until_idle
         request.velocity = velocity
-        request.velocity_unit = velocity_unit.value
+        request.velocity_unit = units_from_literals(velocity_unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         call("device/lockstep_move", request)
 
     async def move_min_async(
             self,
             wait_until_idle: bool = True,
             velocity: float = 0,
-            velocity_unit: Units = Units.NATIVE,
+            velocity_unit: VelocityUnits = Units.NATIVE,
             acceleration: float = 0,
-            acceleration_unit: Units = Units.NATIVE
+            acceleration_unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Moves the axes to the minimum valid position.
         The axes in the lockstep group maintain their offsets throughout movement.
         Respects lim.min for all axes in the group.
 
         Args:
@@ -520,17 +520,17 @@
         request = main_pb2.LockstepMoveRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
         request.type = main_pb2.LockstepMoveRequest.MIN
         request.wait_until_idle = wait_until_idle
         request.velocity = velocity
-        request.velocity_unit = velocity_unit.value
+        request.velocity_unit = units_from_literals(velocity_unit).value
         request.acceleration = acceleration
-        request.acceleration_unit = acceleration_unit.value
+        request.acceleration_unit = units_from_literals(acceleration_unit).value
         await call_async("device/lockstep_move", request)
 
     def wait_until_idle(
             self,
             throw_error_on_fault: bool = True
     ) -> None:
         """
@@ -667,15 +667,15 @@
         request.lockstep_group_id = self.lockstep_group_id
         response = main_pb2.LockstepGetAxisNumbersResponse()
         await call_async("device/lockstep_get_axis_numbers", request, response)
         return list(response.axes)
 
     def get_offsets(
             self,
-            unit: Units = Units.NATIVE
+            unit: LengthUnits = Units.NATIVE
     ) -> List[float]:
         """
         Gets the initial offsets of secondary axes of an enabled lockstep group.
 
         Args:
             unit: Units of position.
                 Uses primary axis unit conversion.
@@ -683,22 +683,22 @@
         Returns:
             Initial offset for each axis of the lockstep group.
         """
         request = main_pb2.LockstepGetRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleArrayResponse()
         call("device/lockstep_get_offsets", request, response)
         return list(response.values)
 
     async def get_offsets_async(
             self,
-            unit: Units = Units.NATIVE
+            unit: LengthUnits = Units.NATIVE
     ) -> List[float]:
         """
         Gets the initial offsets of secondary axes of an enabled lockstep group.
 
         Args:
             unit: Units of position.
                 Uses primary axis unit conversion.
@@ -706,22 +706,22 @@
         Returns:
             Initial offset for each axis of the lockstep group.
         """
         request = main_pb2.LockstepGetRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleArrayResponse()
         await call_async("device/lockstep_get_offsets", request, response)
         return list(response.values)
 
     def get_twists(
             self,
-            unit: Units = Units.NATIVE
+            unit: LengthUnits = Units.NATIVE
     ) -> List[float]:
         """
         Gets the twists of secondary axes of an enabled lockstep group.
 
         Args:
             unit: Units of position.
                 Uses primary axis unit conversion.
@@ -729,22 +729,22 @@
         Returns:
             Difference between the initial offset and the actual offset for each axis of the lockstep group.
         """
         request = main_pb2.LockstepGetRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleArrayResponse()
         call("device/lockstep_get_twists", request, response)
         return list(response.values)
 
     async def get_twists_async(
             self,
-            unit: Units = Units.NATIVE
+            unit: LengthUnits = Units.NATIVE
     ) -> List[float]:
         """
         Gets the twists of secondary axes of an enabled lockstep group.
 
         Args:
             unit: Units of position.
                 Uses primary axis unit conversion.
@@ -752,67 +752,67 @@
         Returns:
             Difference between the initial offset and the actual offset for each axis of the lockstep group.
         """
         request = main_pb2.LockstepGetRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleArrayResponse()
         await call_async("device/lockstep_get_twists", request, response)
         return list(response.values)
 
     def get_position(
             self,
-            unit: Units = Units.NATIVE
+            unit: LengthUnits = Units.NATIVE
     ) -> float:
         """
         Returns current position of the primary axis.
 
         Args:
             unit: Units of the position.
 
         Returns:
             Primary axis position.
         """
         request = main_pb2.LockstepGetRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call("device/lockstep_get_pos", request, response)
         return response.value
 
     async def get_position_async(
             self,
-            unit: Units = Units.NATIVE
+            unit: LengthUnits = Units.NATIVE
     ) -> float:
         """
         Returns current position of the primary axis.
 
         Args:
             unit: Units of the position.
 
         Returns:
             Primary axis position.
         """
         request = main_pb2.LockstepGetRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         await call_async("device/lockstep_get_pos", request, response)
         return response.value
 
     def set_tolerance(
             self,
             tolerance: float,
-            unit: Units = Units.NATIVE,
+            unit: LengthUnits = Units.NATIVE,
             axis_index: int = 0
     ) -> None:
         """
         Sets lockstep twist tolerance.
         Twist tolerances that do not match the system configuration can reduce performance or damage the system.
 
         Args:
@@ -824,22 +824,22 @@
                 If left empty or set to 0, the tolerance is set to all the secondary axes.
         """
         request = main_pb2.LockstepSetRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
         request.value = tolerance
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.axis_index = axis_index
         call("device/lockstep_set_tolerance", request)
 
     async def set_tolerance_async(
             self,
             tolerance: float,
-            unit: Units = Units.NATIVE,
+            unit: LengthUnits = Units.NATIVE,
             axis_index: int = 0
     ) -> None:
         """
         Sets lockstep twist tolerance.
         Twist tolerances that do not match the system configuration can reduce performance or damage the system.
 
         Args:
@@ -851,15 +851,15 @@
                 If left empty or set to 0, the tolerance is set to all the secondary axes.
         """
         request = main_pb2.LockstepSetRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.lockstep_group_id = self.lockstep_group_id
         request.value = tolerance
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.axis_index = axis_index
         await call_async("device/lockstep_set_tolerance", request)
 
     def is_enabled(
             self
     ) -> bool:
         """
```

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/lockstep_axes.py` & `zaber_motion-3.4.2/zaber_motion/ascii/lockstep_axes.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/oscilloscope.py` & `zaber_motion-3.4.2/zaber_motion/ascii/oscilloscope.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 from typing import TYPE_CHECKING, List
 from ..protobufs import main_pb2
-from ..units import Units
+from ..units import Units, units_from_literals, TimeUnits
 from ..call import call, call_async
 from .oscilloscope_data import OscilloscopeData
 
 if TYPE_CHECKING:
     from .device import Device
 
 
@@ -85,178 +85,178 @@
         request = main_pb2.DeviceEmptyRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         await call_async("oscilloscope/clear_channels", request)
 
     def get_timebase(
             self,
-            unit: Units = Units.NATIVE
+            unit: TimeUnits = Units.NATIVE
     ) -> float:
         """
         Get the current sampling interval.
 
         Args:
             unit: Unit of measure to represent the timebase in.
 
         Returns:
             The current sampling interval in the selected time units.
         """
         request = main_pb2.DeviceGetSettingRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.setting = "scope.timebase"
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call("device/get_setting", request, response)
         return response.value
 
     async def get_timebase_async(
             self,
-            unit: Units = Units.NATIVE
+            unit: TimeUnits = Units.NATIVE
     ) -> float:
         """
         Get the current sampling interval.
 
         Args:
             unit: Unit of measure to represent the timebase in.
 
         Returns:
             The current sampling interval in the selected time units.
         """
         request = main_pb2.DeviceGetSettingRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.setting = "scope.timebase"
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         await call_async("device/get_setting", request, response)
         return response.value
 
     def set_timebase(
             self,
             interval: float,
-            unit: Units = Units.NATIVE
+            unit: TimeUnits = Units.NATIVE
     ) -> None:
         """
         Set the sampling interval.
 
         Args:
             interval: Sample interval for the next oscilloscope recording. Minimum value is 100µs.
             unit: Unit of measure the timebase is represented in.
         """
         request = main_pb2.DeviceSetSettingRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.setting = "scope.timebase"
         request.value = interval
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         call("device/set_setting", request)
 
     async def set_timebase_async(
             self,
             interval: float,
-            unit: Units = Units.NATIVE
+            unit: TimeUnits = Units.NATIVE
     ) -> None:
         """
         Set the sampling interval.
 
         Args:
             interval: Sample interval for the next oscilloscope recording. Minimum value is 100µs.
             unit: Unit of measure the timebase is represented in.
         """
         request = main_pb2.DeviceSetSettingRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.setting = "scope.timebase"
         request.value = interval
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         await call_async("device/set_setting", request)
 
     def get_delay(
             self,
-            unit: Units = Units.NATIVE
+            unit: TimeUnits = Units.NATIVE
     ) -> float:
         """
         Get the delay before oscilloscope recording starts.
 
         Args:
             unit: Unit of measure to represent the delay in.
 
         Returns:
             The current start delay in the selected time units.
         """
         request = main_pb2.DeviceGetSettingRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.setting = "scope.delay"
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call("device/get_setting", request, response)
         return response.value
 
     async def get_delay_async(
             self,
-            unit: Units = Units.NATIVE
+            unit: TimeUnits = Units.NATIVE
     ) -> float:
         """
         Get the delay before oscilloscope recording starts.
 
         Args:
             unit: Unit of measure to represent the delay in.
 
         Returns:
             The current start delay in the selected time units.
         """
         request = main_pb2.DeviceGetSettingRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.setting = "scope.delay"
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         await call_async("device/get_setting", request, response)
         return response.value
 
     def set_delay(
             self,
             interval: float,
-            unit: Units = Units.NATIVE
+            unit: TimeUnits = Units.NATIVE
     ) -> None:
         """
         Set the sampling start delay.
 
         Args:
             interval: Delay time between triggering a recording and the first data point being recorded.
             unit: Unit of measure the delay is represented in.
         """
         request = main_pb2.DeviceSetSettingRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.setting = "scope.delay"
         request.value = interval
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         call("device/set_setting", request)
 
     async def set_delay_async(
             self,
             interval: float,
-            unit: Units = Units.NATIVE
+            unit: TimeUnits = Units.NATIVE
     ) -> None:
         """
         Set the sampling start delay.
 
         Args:
             interval: Delay time between triggering a recording and the first data point being recorded.
             unit: Unit of measure the delay is represented in.
         """
         request = main_pb2.DeviceSetSettingRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.setting = "scope.delay"
         request.value = interval
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         await call_async("device/set_setting", request)
 
     def get_max_channels(
             self
     ) -> int:
         """
         Get the maximum number of channels that can be recorded.
```

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/oscilloscope_capture_properties.py` & `zaber_motion-3.4.2/zaber_motion/ascii/oscilloscope_capture_properties.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/oscilloscope_data.py` & `zaber_motion-3.4.2/zaber_motion/ascii/oscilloscope_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 from typing import List
 from ..protobufs import main_pb2
 from ..call import call_sync
-from ..units import Units
+from ..units import UnitsAndLiterals, Units, units_from_literals, TimeUnits
 from .oscilloscope_capture_properties import OscilloscopeCaptureProperties
 
 
 class OscilloscopeData:
     """
     Contains a block of contiguous recorded data for one channel of the device's oscilloscope.
     """
@@ -34,92 +34,92 @@
         return self.__retrieve_properties().axis_number
 
     def __init__(self, data_id: int):
         self._data_id = data_id
 
     def get_timebase(
             self,
-            unit: Units = Units.NATIVE
+            unit: TimeUnits = Units.NATIVE
     ) -> float:
         """
         Get the sample interval that this data was recorded with.
 
         Args:
             unit: Unit of measure to represent the timebase in.
 
         Returns:
             The timebase setting at the time the data was recorded.
         """
         request = main_pb2.OscilloscopeDataGetRequest()
         request.data_id = self.data_id
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call_sync("oscilloscopedata/get_timebase", request, response)
         return response.value
 
     def get_delay(
             self,
-            unit: Units = Units.NATIVE
+            unit: TimeUnits = Units.NATIVE
     ) -> float:
         """
         Get the user-specified time period between receipt of the start command and the first data point.
         Under some circumstances, the actual delay may be different - call GetSampleTime(0) to get the effective delay.
 
         Args:
             unit: Unit of measure to represent the delay in.
 
         Returns:
             The delay setting at the time the data was recorded.
         """
         request = main_pb2.OscilloscopeDataGetRequest()
         request.data_id = self.data_id
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call_sync("oscilloscopedata/get_delay", request, response)
         return response.value
 
     def get_sample_time(
             self,
             index: int,
-            unit: Units = Units.NATIVE
+            unit: TimeUnits = Units.NATIVE
     ) -> float:
         """
         Calculate the time a sample was recorded, relative to when the recording was triggered.
 
         Args:
             index: 0-based index of the sample to calculate the time of.
             unit: Unit of measure to represent the calculated time in.
 
         Returns:
             The calculated time offset of the data sample at the given index.
         """
         request = main_pb2.OscilloscopeDataGetSampleTimeRequest()
         request.data_id = self.data_id
         request.index = index
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call_sync("oscilloscopedata/get_sample_time", request, response)
         return response.value
 
     def get_data(
             self,
-            unit: Units = Units.NATIVE
+            unit: UnitsAndLiterals = Units.NATIVE
     ) -> List[float]:
         """
         Get the recorded data as an array of doubles.
 
         Args:
             unit: Unit of measure to convert the data to.
 
         Returns:
             The recorded data for one oscilloscope channel, converted to the units specified.
         """
         request = main_pb2.OscilloscopeDataGetRequest()
         request.data_id = self.data_id
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.OscilloscopeDataGetSamplesResponse()
         call_sync("oscilloscopedata/get_samples", request, response)
         return list(response.data)
 
     @staticmethod
     def __free(
             data_id: int
```

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/paramset_info.py` & `zaber_motion-3.4.2/zaber_motion/ascii/paramset_info.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/pid_tuning.py` & `zaber_motion-3.4.2/zaber_motion/ascii/pid_tuning.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/pvt_axis_definition.py` & `zaber_motion-3.4.2/zaber_motion/ascii/pvt_axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/pvt_buffer.py` & `zaber_motion-3.4.2/zaber_motion/ascii/pvt_buffer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/pvt_sequence.py` & `zaber_motion-3.4.2/zaber_motion/ascii/pvt_sequence.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/response.py` & `zaber_motion-3.4.2/zaber_motion/ascii/response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/servo_tuner.py` & `zaber_motion-3.4.2/zaber_motion/ascii/servo_tuner.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/servo_tuning_param.py` & `zaber_motion-3.4.2/zaber_motion/ascii/servo_tuning_param.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/setting_constants.py` & `zaber_motion-3.4.2/zaber_motion/ascii/setting_constants.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/simple_tuning_param_definition.py` & `zaber_motion-3.4.2/zaber_motion/ascii/simple_tuning_param_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/storage.py` & `zaber_motion-3.4.2/zaber_motion/ascii/storage.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/stream.py` & `zaber_motion-3.4.2/zaber_motion/ascii/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ﻿# pylint: disable=too-many-arguments, too-many-lines
 
 # ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 from typing import TYPE_CHECKING, List
 from ..protobufs import main_pb2
-from ..units import Units
+from ..units import Units, units_from_literals, VelocityUnits, AccelerationUnits, TimeUnits
 from ..call import call, call_async, call_sync
 from ..measurement import Measurement
 from ..rotation_direction import RotationDirection
 from .stream_buffer import StreamBuffer
 from .stream_mode import StreamMode
 from .stream_axis_definition import StreamAxisDefinition
 
@@ -1226,49 +1226,49 @@
         request.stream_id = self.stream_id
         request.values.extend(values)
         await call_async("device/stream_set_all_analog_outputs", request)
 
     def wait(
             self,
             time: float,
-            unit: Units = Units.NATIVE
+            unit: TimeUnits = Units.NATIVE
     ) -> None:
         """
         Wait a specified time.
 
         Args:
             time: Amount of time to wait.
             unit: Units of time.
         """
         request = main_pb2.StreamWaitRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.time = time
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         call("device/stream_wait", request)
 
     async def wait_async(
             self,
             time: float,
-            unit: Units = Units.NATIVE
+            unit: TimeUnits = Units.NATIVE
     ) -> None:
         """
         Wait a specified time.
 
         Args:
             time: Amount of time to wait.
             unit: Units of time.
         """
         request = main_pb2.StreamWaitRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.time = time
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         await call_async("device/stream_wait", request)
 
     def wait_until_idle(
             self,
             throw_error_on_fault: bool = True
     ) -> None:
         """
@@ -1389,15 +1389,15 @@
         request.stream_id = self.stream_id
         response = main_pb2.BoolResponse()
         await call_async("device/stream_is_busy", request, response)
         return response.value
 
     def get_max_speed(
             self,
-            unit: Units = Units.NATIVE
+            unit: VelocityUnits = Units.NATIVE
     ) -> float:
         """
         Gets the maximum speed of the live stream.
         Converts the units using the first axis of the stream.
 
         Args:
             unit: Units of velocity.
@@ -1405,22 +1405,22 @@
         Returns:
             The maximum speed of the stream.
         """
         request = main_pb2.StreamGetMaxSpeedRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call("device/stream_get_max_speed", request, response)
         return response.value
 
     async def get_max_speed_async(
             self,
-            unit: Units = Units.NATIVE
+            unit: VelocityUnits = Units.NATIVE
     ) -> float:
         """
         Gets the maximum speed of the live stream.
         Converts the units using the first axis of the stream.
 
         Args:
             unit: Units of velocity.
@@ -1428,64 +1428,64 @@
         Returns:
             The maximum speed of the stream.
         """
         request = main_pb2.StreamGetMaxSpeedRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         await call_async("device/stream_get_max_speed", request, response)
         return response.value
 
     def set_max_speed(
             self,
             max_speed: float,
-            unit: Units = Units.NATIVE
+            unit: VelocityUnits = Units.NATIVE
     ) -> None:
         """
         Sets the maximum speed of the live stream.
         Converts the units using the first axis of the stream.
 
         Args:
             max_speed: Maximum speed at which any stream action is executed.
             unit: Units of velocity.
         """
         request = main_pb2.StreamSetMaxSpeedRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.max_speed = max_speed
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         call("device/stream_set_max_speed", request)
 
     async def set_max_speed_async(
             self,
             max_speed: float,
-            unit: Units = Units.NATIVE
+            unit: VelocityUnits = Units.NATIVE
     ) -> None:
         """
         Sets the maximum speed of the live stream.
         Converts the units using the first axis of the stream.
 
         Args:
             max_speed: Maximum speed at which any stream action is executed.
             unit: Units of velocity.
         """
         request = main_pb2.StreamSetMaxSpeedRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.max_speed = max_speed
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         await call_async("device/stream_set_max_speed", request)
 
     def get_max_tangential_acceleration(
             self,
-            unit: Units = Units.NATIVE
+            unit: AccelerationUnits = Units.NATIVE
     ) -> float:
         """
         Gets the maximum tangential acceleration of the live stream.
         Converts the units using the first axis of the stream.
 
         Args:
             unit: Units of acceleration.
@@ -1493,22 +1493,22 @@
         Returns:
             The maximum tangential acceleration of the live stream.
         """
         request = main_pb2.StreamGetMaxTangentialAccelerationRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call("device/stream_get_max_tangential_acceleration", request, response)
         return response.value
 
     async def get_max_tangential_acceleration_async(
             self,
-            unit: Units = Units.NATIVE
+            unit: AccelerationUnits = Units.NATIVE
     ) -> float:
         """
         Gets the maximum tangential acceleration of the live stream.
         Converts the units using the first axis of the stream.
 
         Args:
             unit: Units of acceleration.
@@ -1516,64 +1516,64 @@
         Returns:
             The maximum tangential acceleration of the live stream.
         """
         request = main_pb2.StreamGetMaxTangentialAccelerationRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         await call_async("device/stream_get_max_tangential_acceleration", request, response)
         return response.value
 
     def set_max_tangential_acceleration(
             self,
             max_tangential_acceleration: float,
-            unit: Units = Units.NATIVE
+            unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Sets the maximum tangential acceleration of the live stream.
         Converts the units using the first axis of the stream.
 
         Args:
             max_tangential_acceleration: Maximum tangential acceleration at which any stream action is executed.
             unit: Units of acceleration.
         """
         request = main_pb2.StreamSetMaxTangentialAccelerationRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.max_tangential_acceleration = max_tangential_acceleration
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         call("device/stream_set_max_tangential_acceleration", request)
 
     async def set_max_tangential_acceleration_async(
             self,
             max_tangential_acceleration: float,
-            unit: Units = Units.NATIVE
+            unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Sets the maximum tangential acceleration of the live stream.
         Converts the units using the first axis of the stream.
 
         Args:
             max_tangential_acceleration: Maximum tangential acceleration at which any stream action is executed.
             unit: Units of acceleration.
         """
         request = main_pb2.StreamSetMaxTangentialAccelerationRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.max_tangential_acceleration = max_tangential_acceleration
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         await call_async("device/stream_set_max_tangential_acceleration", request)
 
     def get_max_centripetal_acceleration(
             self,
-            unit: Units = Units.NATIVE
+            unit: AccelerationUnits = Units.NATIVE
     ) -> float:
         """
         Gets the maximum centripetal acceleration of the live stream.
         Converts the units using the first axis of the stream.
 
         Args:
             unit: Units of acceleration.
@@ -1581,22 +1581,22 @@
         Returns:
             The maximum centripetal acceleration of the live stream.
         """
         request = main_pb2.StreamGetMaxCentripetalAccelerationRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call("device/stream_get_max_centripetal_acceleration", request, response)
         return response.value
 
     async def get_max_centripetal_acceleration_async(
             self,
-            unit: Units = Units.NATIVE
+            unit: AccelerationUnits = Units.NATIVE
     ) -> float:
         """
         Gets the maximum centripetal acceleration of the live stream.
         Converts the units using the first axis of the stream.
 
         Args:
             unit: Units of acceleration.
@@ -1604,59 +1604,59 @@
         Returns:
             The maximum centripetal acceleration of the live stream.
         """
         request = main_pb2.StreamGetMaxCentripetalAccelerationRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         await call_async("device/stream_get_max_centripetal_acceleration", request, response)
         return response.value
 
     def set_max_centripetal_acceleration(
             self,
             max_centripetal_acceleration: float,
-            unit: Units = Units.NATIVE
+            unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Sets the maximum centripetal acceleration of the live stream.
         Converts the units using the first axis of the stream.
 
         Args:
             max_centripetal_acceleration: Maximum centripetal acceleration at which any stream action is executed.
             unit: Units of acceleration.
         """
         request = main_pb2.StreamSetMaxCentripetalAccelerationRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.max_centripetal_acceleration = max_centripetal_acceleration
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         call("device/stream_set_max_centripetal_acceleration", request)
 
     async def set_max_centripetal_acceleration_async(
             self,
             max_centripetal_acceleration: float,
-            unit: Units = Units.NATIVE
+            unit: AccelerationUnits = Units.NATIVE
     ) -> None:
         """
         Sets the maximum centripetal acceleration of the live stream.
         Converts the units using the first axis of the stream.
 
         Args:
             max_centripetal_acceleration: Maximum centripetal acceleration at which any stream action is executed.
             unit: Units of acceleration.
         """
         request = main_pb2.StreamSetMaxCentripetalAccelerationRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
         request.stream_id = self.stream_id
         request.max_centripetal_acceleration = max_centripetal_acceleration
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         await call_async("device/stream_set_max_centripetal_acceleration", request)
 
     def __repr__(
             self
     ) -> str:
         """
         Returns a string which represents the stream.
```

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/stream_axis_definition.py` & `zaber_motion-3.4.2/zaber_motion/ascii/stream_axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/stream_buffer.py` & `zaber_motion-3.4.2/zaber_motion/ascii/stream_buffer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/transport.py` & `zaber_motion-3.4.2/zaber_motion/ascii/transport.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/unknown_response_event.py` & `zaber_motion-3.4.2/zaber_motion/ascii/unknown_response_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/warning_flags.py` & `zaber_motion-3.4.2/zaber_motion/ascii/warning_flags.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/ascii/warnings.py` & `zaber_motion-3.4.2/zaber_motion/ascii/warnings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/binary/__init__.py` & `zaber_motion-3.4.2/zaber_motion/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/binary/binary_settings.py` & `zaber_motion-3.4.2/zaber_motion/binary/binary_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/binary/command_code.py` & `zaber_motion-3.4.2/zaber_motion/binary/command_code.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/binary/connection.py` & `zaber_motion-3.4.2/zaber_motion/binary/connection.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/binary/device.py` & `zaber_motion-3.4.2/zaber_motion/binary/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from ..protobufs import main_pb2
 from .binary_settings import BinarySettings
 from .device_identity import DeviceIdentity
 from .device_settings import DeviceSettings
 from .command_code import CommandCode
 from .message import Message
-from ..units import Units
+from ..units import UnitsAndLiterals, Units, units_from_literals, LengthUnits, VelocityUnits
 from .device_type import DeviceType
 from ..firmware_version import FirmwareVersion
 
 if TYPE_CHECKING:
     from .connection import Connection
 
 
@@ -234,16 +234,16 @@
         request.data = data
         await call_async("binary/interface/generic_command_no_response", request)
 
     def generic_command_with_units(
             self,
             command: CommandCode,
             data: float = 0,
-            from_unit: Units = Units.NATIVE,
-            to_unit: Units = Units.NATIVE,
+            from_unit: UnitsAndLiterals = Units.NATIVE,
+            to_unit: UnitsAndLiterals = Units.NATIVE,
             timeout: float = 0.0
     ) -> float:
         """
         Sends a generic Binary command to this device with unit conversions for both sent data and retrieved data.
 
         Args:
             command: Command to send.
@@ -256,27 +256,27 @@
             Data that has been converted to the provided unit.
         """
         request = main_pb2.BinaryGenericWithUnitsRequest()
         request.interface_id = self.connection.interface_id
         request.device = self.device_address
         request.command = command.value
         request.data = data
-        request.from_unit = from_unit.value
-        request.to_unit = to_unit.value
+        request.from_unit = units_from_literals(from_unit).value
+        request.to_unit = units_from_literals(to_unit).value
         request.timeout = timeout
         response = main_pb2.DoubleResponse()
         call("binary/device/generic_command_with_units", request, response)
         return response.value
 
     async def generic_command_with_units_async(
             self,
             command: CommandCode,
             data: float = 0,
-            from_unit: Units = Units.NATIVE,
-            to_unit: Units = Units.NATIVE,
+            from_unit: UnitsAndLiterals = Units.NATIVE,
+            to_unit: UnitsAndLiterals = Units.NATIVE,
             timeout: float = 0.0
     ) -> float:
         """
         Sends a generic Binary command to this device with unit conversions for both sent data and retrieved data.
 
         Args:
             command: Command to send.
@@ -289,24 +289,24 @@
             Data that has been converted to the provided unit.
         """
         request = main_pb2.BinaryGenericWithUnitsRequest()
         request.interface_id = self.connection.interface_id
         request.device = self.device_address
         request.command = command.value
         request.data = data
-        request.from_unit = from_unit.value
-        request.to_unit = to_unit.value
+        request.from_unit = units_from_literals(from_unit).value
+        request.to_unit = units_from_literals(to_unit).value
         request.timeout = timeout
         response = main_pb2.DoubleResponse()
         await call_async("binary/device/generic_command_with_units", request, response)
         return response.value
 
     def home(
             self,
-            unit: Units = Units.NATIVE,
+            unit: LengthUnits = Units.NATIVE,
             timeout: float = DEFAULT_MOVEMENT_TIMEOUT
     ) -> float:
         """
         Homes device. Device returns to its homing position.
 
         Args:
             unit: Unit to convert returned position to.
@@ -314,23 +314,23 @@
 
         Returns:
             Current position that has been converted to the provided unit.
         """
         request = main_pb2.BinaryDeviceHomeRequest()
         request.interface_id = self.connection.interface_id
         request.device = self.device_address
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.timeout = timeout
         response = main_pb2.DoubleResponse()
         call("binary/device/home", request, response)
         return response.value
 
     async def home_async(
             self,
-            unit: Units = Units.NATIVE,
+            unit: LengthUnits = Units.NATIVE,
             timeout: float = DEFAULT_MOVEMENT_TIMEOUT
     ) -> float:
         """
         Homes device. Device returns to its homing position.
 
         Args:
             unit: Unit to convert returned position to.
@@ -338,23 +338,23 @@
 
         Returns:
             Current position that has been converted to the provided unit.
         """
         request = main_pb2.BinaryDeviceHomeRequest()
         request.interface_id = self.connection.interface_id
         request.device = self.device_address
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.timeout = timeout
         response = main_pb2.DoubleResponse()
         await call_async("binary/device/home", request, response)
         return response.value
 
     def stop(
             self,
-            unit: Units = Units.NATIVE,
+            unit: LengthUnits = Units.NATIVE,
             timeout: float = DEFAULT_MOVEMENT_TIMEOUT
     ) -> float:
         """
         Stops ongoing device movement. Decelerates until zero speed.
 
         Args:
             unit: Unit to convert returned position to.
@@ -362,23 +362,23 @@
 
         Returns:
             Current position that has been converted to the provided unit.
         """
         request = main_pb2.BinaryDeviceStopRequest()
         request.interface_id = self.connection.interface_id
         request.device = self.device_address
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.timeout = timeout
         response = main_pb2.DoubleResponse()
         call("binary/device/stop", request, response)
         return response.value
 
     async def stop_async(
             self,
-            unit: Units = Units.NATIVE,
+            unit: LengthUnits = Units.NATIVE,
             timeout: float = DEFAULT_MOVEMENT_TIMEOUT
     ) -> float:
         """
         Stops ongoing device movement. Decelerates until zero speed.
 
         Args:
             unit: Unit to convert returned position to.
@@ -386,24 +386,24 @@
 
         Returns:
             Current position that has been converted to the provided unit.
         """
         request = main_pb2.BinaryDeviceStopRequest()
         request.interface_id = self.connection.interface_id
         request.device = self.device_address
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.timeout = timeout
         response = main_pb2.DoubleResponse()
         await call_async("binary/device/stop", request, response)
         return response.value
 
     def move_absolute(
             self,
             position: float,
-            unit: Units = Units.NATIVE,
+            unit: LengthUnits = Units.NATIVE,
             timeout: float = DEFAULT_MOVEMENT_TIMEOUT
     ) -> float:
         """
         Move device to absolute position.
 
         Args:
             position: Absolute position.
@@ -414,24 +414,24 @@
             Current position that has been converted to the provided unit.
         """
         request = main_pb2.BinaryDeviceMoveRequest()
         request.interface_id = self.connection.interface_id
         request.device = self.device_address
         request.type = main_pb2.BinaryDeviceMoveRequest.ABS
         request.arg = position
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.timeout = timeout
         response = main_pb2.DoubleResponse()
         call("binary/device/move", request, response)
         return response.value
 
     async def move_absolute_async(
             self,
             position: float,
-            unit: Units = Units.NATIVE,
+            unit: LengthUnits = Units.NATIVE,
             timeout: float = DEFAULT_MOVEMENT_TIMEOUT
     ) -> float:
         """
         Move device to absolute position.
 
         Args:
             position: Absolute position.
@@ -442,24 +442,24 @@
             Current position that has been converted to the provided unit.
         """
         request = main_pb2.BinaryDeviceMoveRequest()
         request.interface_id = self.connection.interface_id
         request.device = self.device_address
         request.type = main_pb2.BinaryDeviceMoveRequest.ABS
         request.arg = position
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.timeout = timeout
         response = main_pb2.DoubleResponse()
         await call_async("binary/device/move", request, response)
         return response.value
 
     def move_relative(
             self,
             position: float,
-            unit: Units = Units.NATIVE,
+            unit: LengthUnits = Units.NATIVE,
             timeout: float = DEFAULT_MOVEMENT_TIMEOUT
     ) -> float:
         """
         Move device to position relative to current position.
 
         Args:
             position: Relative position.
@@ -470,24 +470,24 @@
             Current position that has been converted to the provided unit.
         """
         request = main_pb2.BinaryDeviceMoveRequest()
         request.interface_id = self.connection.interface_id
         request.device = self.device_address
         request.type = main_pb2.BinaryDeviceMoveRequest.REL
         request.arg = position
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.timeout = timeout
         response = main_pb2.DoubleResponse()
         call("binary/device/move", request, response)
         return response.value
 
     async def move_relative_async(
             self,
             position: float,
-            unit: Units = Units.NATIVE,
+            unit: LengthUnits = Units.NATIVE,
             timeout: float = DEFAULT_MOVEMENT_TIMEOUT
     ) -> float:
         """
         Move device to position relative to current position.
 
         Args:
             position: Relative position.
@@ -498,24 +498,24 @@
             Current position that has been converted to the provided unit.
         """
         request = main_pb2.BinaryDeviceMoveRequest()
         request.interface_id = self.connection.interface_id
         request.device = self.device_address
         request.type = main_pb2.BinaryDeviceMoveRequest.REL
         request.arg = position
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         request.timeout = timeout
         response = main_pb2.DoubleResponse()
         await call_async("binary/device/move", request, response)
         return response.value
 
     def move_velocity(
             self,
             velocity: float,
-            unit: Units = Units.NATIVE
+            unit: VelocityUnits = Units.NATIVE
     ) -> float:
         """
         Begins to move device at specified speed.
 
         Args:
             velocity: Movement velocity.
             unit: Unit to convert returned velocity to.
@@ -524,23 +524,23 @@
             Device velocity that has been converted to the provided unit.
         """
         request = main_pb2.BinaryDeviceMoveRequest()
         request.interface_id = self.connection.interface_id
         request.device = self.device_address
         request.type = main_pb2.BinaryDeviceMoveRequest.VEL
         request.arg = velocity
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call("binary/device/move", request, response)
         return response.value
 
     async def move_velocity_async(
             self,
             velocity: float,
-            unit: Units = Units.NATIVE
+            unit: VelocityUnits = Units.NATIVE
     ) -> float:
         """
         Begins to move device at specified speed.
 
         Args:
             velocity: Movement velocity.
             unit: Unit to convert returned velocity to.
@@ -549,15 +549,15 @@
             Device velocity that has been converted to the provided unit.
         """
         request = main_pb2.BinaryDeviceMoveRequest()
         request.interface_id = self.connection.interface_id
         request.device = self.device_address
         request.type = main_pb2.BinaryDeviceMoveRequest.VEL
         request.arg = velocity
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         await call_async("binary/device/move", request, response)
         return response.value
 
     def wait_until_idle(
             self
     ) -> None:
@@ -732,52 +732,52 @@
         request.device = self.device_address
         response = main_pb2.BoolResponse()
         await call_async("binary/device/is_parked", request, response)
         return response.value
 
     def get_position(
             self,
-            unit: Units = Units.NATIVE
+            unit: LengthUnits = Units.NATIVE
     ) -> float:
         """
         Returns current device position.
 
         Args:
             unit: Units of position.
 
         Returns:
             Axis position.
         """
         request = main_pb2.BinaryDeviceGetSettingRequest()
         request.interface_id = self.connection.interface_id
         request.device = self.device_address
         request.setting = BinarySettings.CURRENT_POSITION.value
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call("binary/device/get_setting", request, response)
         return response.value
 
     async def get_position_async(
             self,
-            unit: Units = Units.NATIVE
+            unit: LengthUnits = Units.NATIVE
     ) -> float:
         """
         Returns current device position.
 
         Args:
             unit: Units of position.
 
         Returns:
             Axis position.
         """
         request = main_pb2.BinaryDeviceGetSettingRequest()
         request.interface_id = self.connection.interface_id
         request.device = self.device_address
         request.setting = BinarySettings.CURRENT_POSITION.value
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         await call_async("binary/device/get_setting", request, response)
         return response.value
 
     def __repr__(
             self
     ) -> str:
```

### Comparing `zaber_motion-3.4.1/zaber_motion/binary/device_identity.py` & `zaber_motion-3.4.2/zaber_motion/binary/device_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/binary/device_settings.py` & `zaber_motion-3.4.2/zaber_motion/binary/device_settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import TYPE_CHECKING
 from ..call import call, call_async
 
 from ..protobufs import main_pb2
-from ..units import Units
+from ..units import UnitsAndLiterals, Units, units_from_literals
 from .binary_settings import BinarySettings
 
 if TYPE_CHECKING:
     from .device import Device
 
 
 class DeviceSettings:
@@ -19,15 +19,15 @@
 
     def __init__(self, device: 'Device'):
         self._device = device
 
     def get(
             self,
             setting: BinarySettings,
-            unit: Units = Units.NATIVE
+            unit: UnitsAndLiterals = Units.NATIVE
     ) -> float:
         """
         Returns any device setting or property.
 
         Args:
             setting: Setting to get.
             unit: Units of setting.
@@ -35,23 +35,23 @@
         Returns:
             Setting value.
         """
         request = main_pb2.BinaryDeviceGetSettingRequest()
         request.interface_id = self._device.connection.interface_id
         request.device = self._device.device_address
         request.setting = setting.value
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call("binary/device/get_setting", request, response)
         return response.value
 
     async def get_async(
             self,
             setting: BinarySettings,
-            unit: Units = Units.NATIVE
+            unit: UnitsAndLiterals = Units.NATIVE
     ) -> float:
         """
         Returns any device setting or property.
 
         Args:
             setting: Setting to get.
             unit: Units of setting.
@@ -59,55 +59,55 @@
         Returns:
             Setting value.
         """
         request = main_pb2.BinaryDeviceGetSettingRequest()
         request.interface_id = self._device.connection.interface_id
         request.device = self._device.device_address
         request.setting = setting.value
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         await call_async("binary/device/get_setting", request, response)
         return response.value
 
     def set(
             self,
             setting: BinarySettings,
             value: float,
-            unit: Units = Units.NATIVE
+            unit: UnitsAndLiterals = Units.NATIVE
     ) -> None:
         """
         Sets any device setting.
 
         Args:
             setting: Setting to set.
             value: Value of the setting.
             unit: Units of setting.
         """
         request = main_pb2.BinaryDeviceSetSettingRequest()
         request.interface_id = self._device.connection.interface_id
         request.device = self._device.device_address
         request.setting = setting.value
         request.value = value
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         call("binary/device/set_setting", request)
 
     async def set_async(
             self,
             setting: BinarySettings,
             value: float,
-            unit: Units = Units.NATIVE
+            unit: UnitsAndLiterals = Units.NATIVE
     ) -> None:
         """
         Sets any device setting.
 
         Args:
             setting: Setting to set.
             value: Value of the setting.
             unit: Units of setting.
         """
         request = main_pb2.BinaryDeviceSetSettingRequest()
         request.interface_id = self._device.connection.interface_id
         request.device = self._device.device_address
         request.setting = setting.value
         request.value = value
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         await call_async("binary/device/set_setting", request)
```

### Comparing `zaber_motion-3.4.1/zaber_motion/binary/error_code.py` & `zaber_motion-3.4.2/zaber_motion/binary/error_code.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/binary/message.py` & `zaber_motion-3.4.2/zaber_motion/binary/message.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/binary/reply_only_event.py` & `zaber_motion-3.4.2/zaber_motion/binary/reply_only_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/binary/unknown_response_event.py` & `zaber_motion-3.4.2/zaber_motion/binary/unknown_response_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/bindings.py` & `zaber_motion-3.4.2/zaber_motion/bindings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/call.py` & `zaber_motion-3.4.2/zaber_motion/call.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/convert_exception.py` & `zaber_motion-3.4.2/zaber_motion/convert_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/events.py` & `zaber_motion-3.4.2/zaber_motion/events.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/__init__.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/binary_command_failed_exception.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/binary_command_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/binary_command_failed_exception_data.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/binary_command_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/command_failed_exception.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/command_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/command_failed_exception_data.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/command_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/command_too_long_exception.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/command_too_long_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/command_too_long_exception_data.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/command_too_long_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/device_address_conflict_exception.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/device_address_conflict_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/device_address_conflict_exception_data.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/device_address_conflict_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/device_db_failed_exception.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/device_db_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/device_db_failed_exception_data.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/device_db_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/g_code_execution_exception.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/g_code_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/g_code_execution_exception_data.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/g_code_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/g_code_syntax_exception.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/g_code_syntax_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/g_code_syntax_exception_data.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/g_code_syntax_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/invalid_packet_exception.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/invalid_packet_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/invalid_packet_exception_data.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/invalid_packet_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/invalid_pvt_point.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/invalid_pvt_point.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/invalid_response_exception.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/invalid_response_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/invalid_response_exception_data.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/invalid_response_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/movement_failed_exception.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/movement_failed_exception_data.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/movement_interrupted_exception.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/movement_interrupted_exception_data.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/pvt_execution_exception.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/pvt_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/pvt_execution_exception_data.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/pvt_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/pvt_movement_failed_exception.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/pvt_movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/pvt_movement_failed_exception_data.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/pvt_movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/pvt_movement_interrupted_exception.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/pvt_movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/set_device_state_exception_data.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/set_device_state_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/set_device_state_failed_exception.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/set_device_state_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/set_peripheral_state_exception_data.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/set_peripheral_state_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/set_peripheral_state_failed_exception.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/set_peripheral_state_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/stream_execution_exception.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/stream_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/stream_execution_exception_data.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/stream_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/stream_movement_failed_exception.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/stream_movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/stream_movement_failed_exception_data.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/stream_movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/stream_movement_interrupted_exception.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/stream_movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py` & `zaber_motion-3.4.2/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/firmware_version.py` & `zaber_motion-3.4.2/zaber_motion/firmware_version.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/gcode/__init__.py` & `zaber_motion-3.4.2/zaber_motion/gcode/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/gcode/axis_definition.py` & `zaber_motion-3.4.2/zaber_motion/gcode/axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/gcode/axis_mapping.py` & `zaber_motion-3.4.2/zaber_motion/gcode/axis_mapping.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/gcode/axis_transformation.py` & `zaber_motion-3.4.2/zaber_motion/gcode/axis_transformation.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/gcode/device_definition.py` & `zaber_motion-3.4.2/zaber_motion/gcode/device_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/gcode/offline_translator.py` & `zaber_motion-3.4.2/zaber_motion/gcode/translator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import List, Optional
 from ..call import call, call_async, call_sync
 
 from ..protobufs import main_pb2
-from ..units import Units
-from ..ascii import Device
-from .device_definition import DeviceDefinition
+from ..units import units_from_literals, LengthUnits, VelocityUnits
+from ..ascii import Stream
 from .translator_config import TranslatorConfig
 from .translate_result import TranslateResult
 
 
-class OfflineTranslator:
+class Translator:
     """
-    Represents an offline G-Code translator.
-    It allows to translate G-Code blocks to Zaber ASCII protocol stream commands.
-    This translator does not need a connected device to perform translation.
+    Represents a live G-Code translator.
+    It allows to stream G-Code blocks to a connected device.
+    It requires a stream to be setup on the device.
     Requires at least Firmware 7.11.
     """
 
     @property
     def translator_id(self) -> int:
         """
         The ID of the translator that serves to identify native resources.
@@ -35,171 +34,193 @@
         return self.__get_current_coordinate_system()
 
     def __init__(self, translator_id: int):
         self._translator_id = translator_id
 
     @staticmethod
     def setup(
-            definition: DeviceDefinition,
+            stream: Stream,
             config: Optional[TranslatorConfig] = None
-    ) -> 'OfflineTranslator':
+    ) -> 'Translator':
         """
-        Sets up translator from provided device definition and configuration.
+        Sets up the translator on top of a provided stream.
 
         Args:
-            definition: Definition of device and its peripherals.
-                The definition must match a device that later performs the commands.
+            stream: The stream to setup the translator on.
+                The stream must be already setup in a live or a store mode.
             config: Configuration of the translator.
 
         Returns:
             New instance of translator.
         """
-        request = main_pb2.TranslatorCreateRequest()
-        request.definition.CopyFrom(DeviceDefinition.to_protobuf(definition))
+        request = main_pb2.TranslatorCreateLiveRequest()
+        request.device = stream.device.device_address
+        request.interface_id = stream.device.connection.interface_id
+        request.stream_id = stream.stream_id
         request.config.CopyFrom(TranslatorConfig.to_protobuf(config))
         response = main_pb2.TranslatorCreateResponse()
-        call("gcode/create", request, response)
-        return OfflineTranslator(response.translator_id)
+        call("gcode/create_live", request, response)
+        return Translator(response.translator_id)
 
     @staticmethod
     async def setup_async(
-            definition: DeviceDefinition,
+            stream: Stream,
             config: Optional[TranslatorConfig] = None
-    ) -> 'OfflineTranslator':
+    ) -> 'Translator':
         """
-        Sets up translator from provided device definition and configuration.
+        Sets up the translator on top of a provided stream.
 
         Args:
-            definition: Definition of device and its peripherals.
-                The definition must match a device that later performs the commands.
+            stream: The stream to setup the translator on.
+                The stream must be already setup in a live or a store mode.
             config: Configuration of the translator.
 
         Returns:
             New instance of translator.
         """
-        request = main_pb2.TranslatorCreateRequest()
-        request.definition.CopyFrom(DeviceDefinition.to_protobuf(definition))
+        request = main_pb2.TranslatorCreateLiveRequest()
+        request.device = stream.device.device_address
+        request.interface_id = stream.device.connection.interface_id
+        request.stream_id = stream.stream_id
         request.config.CopyFrom(TranslatorConfig.to_protobuf(config))
         response = main_pb2.TranslatorCreateResponse()
-        await call_async("gcode/create", request, response)
-        return OfflineTranslator(response.translator_id)
+        await call_async("gcode/create_live", request, response)
+        return Translator(response.translator_id)
 
-    @staticmethod
-    def setup_from_device(
-            device: Device,
-            axes: List[int],
-            config: Optional[TranslatorConfig] = None
-    ) -> 'OfflineTranslator':
-        """
-        Sets up an offline translator from provided device, axes, and configuration.
-
-        Args:
-            device: Device that later performs the command streaming.
-            axes: Axis numbers that are later used to setup the stream.
-                For a lockstep group specify only the first axis of the group.
-            config: Configuration of the translator.
-
-        Returns:
-            New instance of translator.
-        """
-        request = main_pb2.TranslatorCreateFromDeviceRequest()
-        request.interface_id = device.connection.interface_id
-        request.device = device.device_address
-        request.axes.extend(axes)
-        request.config.CopyFrom(TranslatorConfig.to_protobuf(config))
-        response = main_pb2.TranslatorCreateResponse()
-        call("gcode/create_from_device", request, response)
-        return OfflineTranslator(response.translator_id)
-
-    @staticmethod
-    async def setup_from_device_async(
-            device: Device,
-            axes: List[int],
-            config: Optional[TranslatorConfig] = None
-    ) -> 'OfflineTranslator':
+    def translate(
+            self,
+            block: str
+    ) -> TranslateResult:
         """
-        Sets up an offline translator from provided device, axes, and configuration.
+        Translates a single block (line) of G-code.
+        The commands are queued in the underlying stream to ensure smooth continues movement.
+        Returning of this method indicates that the commands are queued (not necessarily executed).
 
         Args:
-            device: Device that later performs the command streaming.
-            axes: Axis numbers that are later used to setup the stream.
-                For a lockstep group specify only the first axis of the group.
-            config: Configuration of the translator.
+            block: Block (line) of G-code.
 
         Returns:
-            New instance of translator.
+            Result of translation containing the commands sent to the device.
         """
-        request = main_pb2.TranslatorCreateFromDeviceRequest()
-        request.interface_id = device.connection.interface_id
-        request.device = device.device_address
-        request.axes.extend(axes)
-        request.config.CopyFrom(TranslatorConfig.to_protobuf(config))
-        response = main_pb2.TranslatorCreateResponse()
-        await call_async("gcode/create_from_device", request, response)
-        return OfflineTranslator(response.translator_id)
+        request = main_pb2.TranslatorTranslateRequest()
+        request.translator_id = self.translator_id
+        request.block = block
+        response = main_pb2.TranslatorTranslateResponse()
+        call("gcode/translate_live", request, response)
+        return TranslateResult.from_protobuf(response)
 
-    def translate(
+    async def translate_async(
             self,
             block: str
     ) -> TranslateResult:
         """
         Translates a single block (line) of G-code.
+        The commands are queued in the underlying stream to ensure smooth continues movement.
+        Returning of this method indicates that the commands are queued (not necessarily executed).
 
         Args:
             block: Block (line) of G-code.
 
         Returns:
-            Result of translation containing the stream commands.
+            Result of translation containing the commands sent to the device.
         """
         request = main_pb2.TranslatorTranslateRequest()
         request.translator_id = self.translator_id
         request.block = block
         response = main_pb2.TranslatorTranslateResponse()
-        call_sync("gcode/translate", request, response)
+        await call_async("gcode/translate_live", request, response)
         return TranslateResult.from_protobuf(response)
 
     def flush(
-            self
+            self,
+            wait_until_idle: bool = True
     ) -> List[str]:
         """
-        Flushes the remaining stream commands waiting in optimization buffer.
+        Flushes the remaining stream commands waiting in optimization buffer into the underlying stream.
         The flush is also performed by M2 and M30 codes.
 
+        Args:
+            wait_until_idle: Determines whether to wait for the stream to finish all the movements.
+
         Returns:
             The remaining stream commands.
         """
-        request = main_pb2.TranslatorEmptyRequest()
+        request = main_pb2.TranslatorFlushLiveRequest()
+        request.translator_id = self.translator_id
+        request.wait_until_idle = wait_until_idle
+        response = main_pb2.TranslatorFlushResponse()
+        call("gcode/flush_live", request, response)
+        return list(response.commands)
+
+    async def flush_async(
+            self,
+            wait_until_idle: bool = True
+    ) -> List[str]:
+        """
+        Flushes the remaining stream commands waiting in optimization buffer into the underlying stream.
+        The flush is also performed by M2 and M30 codes.
+
+        Args:
+            wait_until_idle: Determines whether to wait for the stream to finish all the movements.
+
+        Returns:
+            The remaining stream commands.
+        """
+        request = main_pb2.TranslatorFlushLiveRequest()
         request.translator_id = self.translator_id
+        request.wait_until_idle = wait_until_idle
         response = main_pb2.TranslatorFlushResponse()
-        call_sync("gcode/flush", request, response)
+        await call_async("gcode/flush_live", request, response)
         return list(response.commands)
 
+    def reset_position(
+            self
+    ) -> None:
+        """
+        Resets position of the translator from the underlying stream.
+        Call this method after performing a movement outside of translator.
+        """
+        request = main_pb2.TranslatorEmptyRequest()
+        request.translator_id = self.translator_id
+        call("gcode/reset_position_from_stream", request)
+
+    async def reset_position_async(
+            self
+    ) -> None:
+        """
+        Resets position of the translator from the underlying stream.
+        Call this method after performing a movement outside of translator.
+        """
+        request = main_pb2.TranslatorEmptyRequest()
+        request.translator_id = self.translator_id
+        await call_async("gcode/reset_position_from_stream", request)
+
     def set_traverse_rate(
             self,
             traverse_rate: float,
-            unit: Units
+            unit: VelocityUnits
     ) -> None:
         """
         Sets the speed at which the device moves when traversing (G0).
 
         Args:
             traverse_rate: The traverse rate.
             unit: Units of the traverse rate.
         """
         request = main_pb2.TranslatorSetTraverseRateRequest()
         request.translator_id = self.translator_id
         request.traverse_rate = traverse_rate
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         call_sync("gcode/set_traverse_rate", request)
 
     def set_axis_position(
             self,
             axis: str,
             position: float,
-            unit: Units
+            unit: LengthUnits
     ) -> None:
         """
         Sets position of translator's axis.
         Use this method to set position after performing movement outside of the translator.
         This method does not cause any movement.
 
         Args:
@@ -207,21 +228,21 @@
             position: The position.
             unit: Units of position.
         """
         request = main_pb2.TranslatorSetAxisPositionRequest()
         request.translator_id = self.translator_id
         request.axis = axis
         request.position = position
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         call_sync("gcode/set_axis_position", request)
 
     def get_axis_position(
             self,
             axis: str,
-            unit: Units
+            unit: LengthUnits
     ) -> float:
         """
         Gets position of translator's axis.
         This method does not query device but returns value from translator's state.
 
         Args:
             axis: Letter of the axis.
@@ -229,68 +250,68 @@
 
         Returns:
             Position of translator's axis.
         """
         request = main_pb2.TranslatorGetAxisPositionRequest()
         request.translator_id = self.translator_id
         request.axis = axis
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call_sync("gcode/get_axis_position", request, response)
         return response.value
 
     def set_axis_home_position(
             self,
             axis: str,
             position: float,
-            unit: Units
+            unit: LengthUnits
     ) -> None:
         """
         Sets the home position of translator's axis.
         This position is used by G28.
 
         Args:
             axis: Letter of the axis.
             position: The home position.
             unit: Units of position.
         """
         request = main_pb2.TranslatorSetAxisPositionRequest()
         request.translator_id = self.translator_id
         request.axis = axis
         request.position = position
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         call_sync("gcode/set_axis_home", request)
 
     def set_axis_secondary_home_position(
             self,
             axis: str,
             position: float,
-            unit: Units
+            unit: LengthUnits
     ) -> None:
         """
         Sets the secondary home position of translator's axis.
         This position is used by G30.
 
         Args:
             axis: Letter of the axis.
             position: The home position.
             unit: Units of position.
         """
         request = main_pb2.TranslatorSetAxisPositionRequest()
         request.translator_id = self.translator_id
         request.axis = axis
         request.position = position
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         call_sync("gcode/set_axis_secondary_home", request)
 
     def get_axis_coordinate_system_offset(
             self,
             coordinate_system: str,
             axis: str,
-            unit: Units
+            unit: LengthUnits
     ) -> float:
         """
         Gets offset of an axis in a given coordinate system.
 
         Args:
             coordinate_system: Coordinate system (e.g. G54).
             axis: Letter of the axis.
@@ -299,15 +320,15 @@
         Returns:
             Offset in translator units of the axis.
         """
         request = main_pb2.TranslatorGetAxisOffsetRequest()
         request.translator_id = self.translator_id
         request.coordinate_system = coordinate_system
         request.axis = axis
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call_sync("gcode/get_axis_offset", request, response)
         return response.value
 
     def reset_after_stream_error(
             self
     ) -> None:
@@ -360,8 +381,8 @@
         request = main_pb2.TranslatorEmptyRequest()
         request.translator_id = self.translator_id
         response = main_pb2.StringResponse()
         call_sync("gcode/get_current_coordinate_system", request, response)
         return response.value
 
     def __del__(self) -> None:
-        OfflineTranslator.__free(self.translator_id)
+        Translator.__free(self.translator_id)
```

### Comparing `zaber_motion-3.4.1/zaber_motion/gcode/translate_message.py` & `zaber_motion-3.4.2/zaber_motion/gcode/translate_message.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/gcode/translate_result.py` & `zaber_motion-3.4.2/zaber_motion/gcode/translate_result.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/gcode/translator.py` & `zaber_motion-3.4.2/zaber_motion/gcode/offline_translator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 
 from typing import List, Optional
 from ..call import call, call_async, call_sync
 
 from ..protobufs import main_pb2
-from ..units import Units
-from ..ascii import Stream
+from ..units import units_from_literals, LengthUnits, VelocityUnits
+from ..ascii import Device
+from .device_definition import DeviceDefinition
 from .translator_config import TranslatorConfig
 from .translate_result import TranslateResult
 
 
-class Translator:
+class OfflineTranslator:
     """
-    Represents a live G-Code translator.
-    It allows to stream G-Code blocks to a connected device.
-    It requires a stream to be setup on the device.
+    Represents an offline G-Code translator.
+    It allows to translate G-Code blocks to Zaber ASCII protocol stream commands.
+    This translator does not need a connected device to perform translation.
     Requires at least Firmware 7.11.
     """
 
     @property
     def translator_id(self) -> int:
         """
         The ID of the translator that serves to identify native resources.
@@ -34,193 +35,171 @@
         return self.__get_current_coordinate_system()
 
     def __init__(self, translator_id: int):
         self._translator_id = translator_id
 
     @staticmethod
     def setup(
-            stream: Stream,
+            definition: DeviceDefinition,
             config: Optional[TranslatorConfig] = None
-    ) -> 'Translator':
+    ) -> 'OfflineTranslator':
         """
-        Sets up the translator on top of a provided stream.
+        Sets up translator from provided device definition and configuration.
 
         Args:
-            stream: The stream to setup the translator on.
-                The stream must be already setup in a live or a store mode.
+            definition: Definition of device and its peripherals.
+                The definition must match a device that later performs the commands.
             config: Configuration of the translator.
 
         Returns:
             New instance of translator.
         """
-        request = main_pb2.TranslatorCreateLiveRequest()
-        request.device = stream.device.device_address
-        request.interface_id = stream.device.connection.interface_id
-        request.stream_id = stream.stream_id
+        request = main_pb2.TranslatorCreateRequest()
+        request.definition.CopyFrom(DeviceDefinition.to_protobuf(definition))
         request.config.CopyFrom(TranslatorConfig.to_protobuf(config))
         response = main_pb2.TranslatorCreateResponse()
-        call("gcode/create_live", request, response)
-        return Translator(response.translator_id)
+        call("gcode/create", request, response)
+        return OfflineTranslator(response.translator_id)
 
     @staticmethod
     async def setup_async(
-            stream: Stream,
+            definition: DeviceDefinition,
             config: Optional[TranslatorConfig] = None
-    ) -> 'Translator':
+    ) -> 'OfflineTranslator':
         """
-        Sets up the translator on top of a provided stream.
+        Sets up translator from provided device definition and configuration.
 
         Args:
-            stream: The stream to setup the translator on.
-                The stream must be already setup in a live or a store mode.
+            definition: Definition of device and its peripherals.
+                The definition must match a device that later performs the commands.
             config: Configuration of the translator.
 
         Returns:
             New instance of translator.
         """
-        request = main_pb2.TranslatorCreateLiveRequest()
-        request.device = stream.device.device_address
-        request.interface_id = stream.device.connection.interface_id
-        request.stream_id = stream.stream_id
+        request = main_pb2.TranslatorCreateRequest()
+        request.definition.CopyFrom(DeviceDefinition.to_protobuf(definition))
         request.config.CopyFrom(TranslatorConfig.to_protobuf(config))
         response = main_pb2.TranslatorCreateResponse()
-        await call_async("gcode/create_live", request, response)
-        return Translator(response.translator_id)
+        await call_async("gcode/create", request, response)
+        return OfflineTranslator(response.translator_id)
 
-    def translate(
-            self,
-            block: str
-    ) -> TranslateResult:
+    @staticmethod
+    def setup_from_device(
+            device: Device,
+            axes: List[int],
+            config: Optional[TranslatorConfig] = None
+    ) -> 'OfflineTranslator':
         """
-        Translates a single block (line) of G-code.
-        The commands are queued in the underlying stream to ensure smooth continues movement.
-        Returning of this method indicates that the commands are queued (not necessarily executed).
+        Sets up an offline translator from provided device, axes, and configuration.
 
         Args:
-            block: Block (line) of G-code.
+            device: Device that later performs the command streaming.
+            axes: Axis numbers that are later used to setup the stream.
+                For a lockstep group specify only the first axis of the group.
+            config: Configuration of the translator.
 
         Returns:
-            Result of translation containing the commands sent to the device.
+            New instance of translator.
         """
-        request = main_pb2.TranslatorTranslateRequest()
-        request.translator_id = self.translator_id
-        request.block = block
-        response = main_pb2.TranslatorTranslateResponse()
-        call("gcode/translate_live", request, response)
-        return TranslateResult.from_protobuf(response)
+        request = main_pb2.TranslatorCreateFromDeviceRequest()
+        request.interface_id = device.connection.interface_id
+        request.device = device.device_address
+        request.axes.extend(axes)
+        request.config.CopyFrom(TranslatorConfig.to_protobuf(config))
+        response = main_pb2.TranslatorCreateResponse()
+        call("gcode/create_from_device", request, response)
+        return OfflineTranslator(response.translator_id)
+
+    @staticmethod
+    async def setup_from_device_async(
+            device: Device,
+            axes: List[int],
+            config: Optional[TranslatorConfig] = None
+    ) -> 'OfflineTranslator':
+        """
+        Sets up an offline translator from provided device, axes, and configuration.
+
+        Args:
+            device: Device that later performs the command streaming.
+            axes: Axis numbers that are later used to setup the stream.
+                For a lockstep group specify only the first axis of the group.
+            config: Configuration of the translator.
 
-    async def translate_async(
+        Returns:
+            New instance of translator.
+        """
+        request = main_pb2.TranslatorCreateFromDeviceRequest()
+        request.interface_id = device.connection.interface_id
+        request.device = device.device_address
+        request.axes.extend(axes)
+        request.config.CopyFrom(TranslatorConfig.to_protobuf(config))
+        response = main_pb2.TranslatorCreateResponse()
+        await call_async("gcode/create_from_device", request, response)
+        return OfflineTranslator(response.translator_id)
+
+    def translate(
             self,
             block: str
     ) -> TranslateResult:
         """
         Translates a single block (line) of G-code.
-        The commands are queued in the underlying stream to ensure smooth continues movement.
-        Returning of this method indicates that the commands are queued (not necessarily executed).
 
         Args:
             block: Block (line) of G-code.
 
         Returns:
-            Result of translation containing the commands sent to the device.
+            Result of translation containing the stream commands.
         """
         request = main_pb2.TranslatorTranslateRequest()
         request.translator_id = self.translator_id
         request.block = block
         response = main_pb2.TranslatorTranslateResponse()
-        await call_async("gcode/translate_live", request, response)
+        call_sync("gcode/translate", request, response)
         return TranslateResult.from_protobuf(response)
 
     def flush(
-            self,
-            wait_until_idle: bool = True
-    ) -> List[str]:
-        """
-        Flushes the remaining stream commands waiting in optimization buffer into the underlying stream.
-        The flush is also performed by M2 and M30 codes.
-
-        Args:
-            wait_until_idle: Determines whether to wait for the stream to finish all the movements.
-
-        Returns:
-            The remaining stream commands.
-        """
-        request = main_pb2.TranslatorFlushLiveRequest()
-        request.translator_id = self.translator_id
-        request.wait_until_idle = wait_until_idle
-        response = main_pb2.TranslatorFlushResponse()
-        call("gcode/flush_live", request, response)
-        return list(response.commands)
-
-    async def flush_async(
-            self,
-            wait_until_idle: bool = True
+            self
     ) -> List[str]:
         """
-        Flushes the remaining stream commands waiting in optimization buffer into the underlying stream.
+        Flushes the remaining stream commands waiting in optimization buffer.
         The flush is also performed by M2 and M30 codes.
 
-        Args:
-            wait_until_idle: Determines whether to wait for the stream to finish all the movements.
-
         Returns:
             The remaining stream commands.
         """
-        request = main_pb2.TranslatorFlushLiveRequest()
+        request = main_pb2.TranslatorEmptyRequest()
         request.translator_id = self.translator_id
-        request.wait_until_idle = wait_until_idle
         response = main_pb2.TranslatorFlushResponse()
-        await call_async("gcode/flush_live", request, response)
+        call_sync("gcode/flush", request, response)
         return list(response.commands)
 
-    def reset_position(
-            self
-    ) -> None:
-        """
-        Resets position of the translator from the underlying stream.
-        Call this method after performing a movement outside of translator.
-        """
-        request = main_pb2.TranslatorEmptyRequest()
-        request.translator_id = self.translator_id
-        call("gcode/reset_position_from_stream", request)
-
-    async def reset_position_async(
-            self
-    ) -> None:
-        """
-        Resets position of the translator from the underlying stream.
-        Call this method after performing a movement outside of translator.
-        """
-        request = main_pb2.TranslatorEmptyRequest()
-        request.translator_id = self.translator_id
-        await call_async("gcode/reset_position_from_stream", request)
-
     def set_traverse_rate(
             self,
             traverse_rate: float,
-            unit: Units
+            unit: VelocityUnits
     ) -> None:
         """
         Sets the speed at which the device moves when traversing (G0).
 
         Args:
             traverse_rate: The traverse rate.
             unit: Units of the traverse rate.
         """
         request = main_pb2.TranslatorSetTraverseRateRequest()
         request.translator_id = self.translator_id
         request.traverse_rate = traverse_rate
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         call_sync("gcode/set_traverse_rate", request)
 
     def set_axis_position(
             self,
             axis: str,
             position: float,
-            unit: Units
+            unit: LengthUnits
     ) -> None:
         """
         Sets position of translator's axis.
         Use this method to set position after performing movement outside of the translator.
         This method does not cause any movement.
 
         Args:
@@ -228,21 +207,21 @@
             position: The position.
             unit: Units of position.
         """
         request = main_pb2.TranslatorSetAxisPositionRequest()
         request.translator_id = self.translator_id
         request.axis = axis
         request.position = position
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         call_sync("gcode/set_axis_position", request)
 
     def get_axis_position(
             self,
             axis: str,
-            unit: Units
+            unit: LengthUnits
     ) -> float:
         """
         Gets position of translator's axis.
         This method does not query device but returns value from translator's state.
 
         Args:
             axis: Letter of the axis.
@@ -250,68 +229,68 @@
 
         Returns:
             Position of translator's axis.
         """
         request = main_pb2.TranslatorGetAxisPositionRequest()
         request.translator_id = self.translator_id
         request.axis = axis
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call_sync("gcode/get_axis_position", request, response)
         return response.value
 
     def set_axis_home_position(
             self,
             axis: str,
             position: float,
-            unit: Units
+            unit: LengthUnits
     ) -> None:
         """
         Sets the home position of translator's axis.
         This position is used by G28.
 
         Args:
             axis: Letter of the axis.
             position: The home position.
             unit: Units of position.
         """
         request = main_pb2.TranslatorSetAxisPositionRequest()
         request.translator_id = self.translator_id
         request.axis = axis
         request.position = position
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         call_sync("gcode/set_axis_home", request)
 
     def set_axis_secondary_home_position(
             self,
             axis: str,
             position: float,
-            unit: Units
+            unit: LengthUnits
     ) -> None:
         """
         Sets the secondary home position of translator's axis.
         This position is used by G30.
 
         Args:
             axis: Letter of the axis.
             position: The home position.
             unit: Units of position.
         """
         request = main_pb2.TranslatorSetAxisPositionRequest()
         request.translator_id = self.translator_id
         request.axis = axis
         request.position = position
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         call_sync("gcode/set_axis_secondary_home", request)
 
     def get_axis_coordinate_system_offset(
             self,
             coordinate_system: str,
             axis: str,
-            unit: Units
+            unit: LengthUnits
     ) -> float:
         """
         Gets offset of an axis in a given coordinate system.
 
         Args:
             coordinate_system: Coordinate system (e.g. G54).
             axis: Letter of the axis.
@@ -320,15 +299,15 @@
         Returns:
             Offset in translator units of the axis.
         """
         request = main_pb2.TranslatorGetAxisOffsetRequest()
         request.translator_id = self.translator_id
         request.coordinate_system = coordinate_system
         request.axis = axis
-        request.unit = unit.value
+        request.unit = units_from_literals(unit).value
         response = main_pb2.DoubleResponse()
         call_sync("gcode/get_axis_offset", request, response)
         return response.value
 
     def reset_after_stream_error(
             self
     ) -> None:
@@ -381,8 +360,8 @@
         request = main_pb2.TranslatorEmptyRequest()
         request.translator_id = self.translator_id
         response = main_pb2.StringResponse()
         call_sync("gcode/get_current_coordinate_system", request, response)
         return response.value
 
     def __del__(self) -> None:
-        Translator.__free(self.translator_id)
+        OfflineTranslator.__free(self.translator_id)
```

### Comparing `zaber_motion-3.4.1/zaber_motion/gcode/translator_config.py` & `zaber_motion-3.4.2/zaber_motion/gcode/translator_config.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/library.py` & `zaber_motion-3.4.2/zaber_motion/library.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/measurement.py` & `zaber_motion-3.4.2/zaber_motion/measurement.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ﻿# ===== THIS FILE IS GENERATED FROM A TEMPLATE ===== #
 # ============== DO NOT EDIT DIRECTLY ============== #
 # pylint: disable=W0201
 
 from typing import Optional  # pylint: disable=unused-import
 from .protobufs import main_pb2
-from .units import Units
+from .units import UnitsAndLiterals, Units, units_from_literals
 
 
 class Measurement:
     """
     Represents a numerical value with optional units specified.
     """
 
     def __init__(
             self: 'Measurement',
             value: float,
-            unit: Optional[Units] = None
+            unit: Optional[UnitsAndLiterals] = None
     ) -> None:
         self._value = value
         self._unit = unit
 
     @property
     def value(self) -> float:
         """
@@ -29,23 +29,23 @@
         return self._value
 
     @value.setter
     def value(self, value: float) -> None:
         self._value = value
 
     @property
-    def unit(self) -> Optional[Units]:
+    def unit(self) -> Optional[UnitsAndLiterals]:
         """
         Optional units of the measurement.
         """
 
         return self._unit
 
     @unit.setter
-    def unit(self, value: Optional[Units]) -> None:
+    def unit(self, value: Optional[UnitsAndLiterals]) -> None:
         self._unit = value
 
     def __repr__(self) -> str:
         return str(self.__dict__)
 
     @staticmethod
     def to_protobuf(source: 'Optional[Measurement]') -> main_pb2.Measurement:
@@ -53,9 +53,9 @@
             return main_pb2.Measurement()
 
         if not isinstance(source, Measurement):
             raise TypeError("Provided value is not Measurement.")
 
         pb_data = main_pb2.Measurement()
         pb_data.value = source.value
-        pb_data.unit = (source.unit or Units.NATIVE).value
+        pb_data.unit = units_from_literals(source.unit or Units.NATIVE).value
         return pb_data
```

### Comparing `zaber_motion-3.4.1/zaber_motion/microscopy/objective_changer.py` & `zaber_motion-3.4.2/zaber_motion/microscopy/objective_changer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/protobufs/main_pb2.py` & `zaber_motion-3.4.2/zaber_motion/protobufs/main_pb2.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/protobufs/main_pb2.pyi` & `zaber_motion-3.4.2/zaber_motion/protobufs/main_pb2.pyi`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/serialization.py` & `zaber_motion-3.4.2/zaber_motion/serialization.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion/tools.py` & `zaber_motion-3.4.2/zaber_motion/tools.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-3.4.1/zaber_motion.egg-info/PKG-INFO` & `zaber_motion-3.4.2/zaber_motion.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: zaber-motion
-Version: 3.4.1
+Version: 3.4.2
 Summary: A library for communicating with Zaber devices
 Home-page: https://gitlab.com/ZaberTech/zaber-motion-lib
 Author: Zaber Technologies Inc.
 Author-email: contact@zaber.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Zaber Motion Library
 
 Zaber Motion Library is a multi-platform library used to operate Zaber devices.
```

### Comparing `zaber_motion-3.4.1/zaber_motion.egg-info/SOURCES.txt` & `zaber_motion-3.4.2/zaber_motion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

