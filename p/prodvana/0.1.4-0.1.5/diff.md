# Comparing `tmp/prodvana-0.1.4.tar.gz` & `tmp/prodvana-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodvana-0.1.4.tar", max compression
+gzip compressed data, was "prodvana-0.1.5.tar", max compression
```

## Comparing `prodvana-0.1.4.tar` & `prodvana-0.1.5.tar`

### file list

```diff
@@ -1,336 +1,332 @@
--rw-r--r--   0        0        0       81 2023-05-19 19:00:48.877495 prodvana-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.877495 prodvana-0.1.4/prodvana/__init__.py
--rw-r--r--   0        0        0     3529 2023-05-19 23:43:46.670463 prodvana-0.1.4/prodvana/client.py
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.480946 prodvana-0.1.4/prodvana/proto/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.480946 prodvana-0.1.4/prodvana/proto/prodvana/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.504946 prodvana-0.1.4/prodvana/proto/prodvana/agent/__init__.py
--rw-r--r--   0        0        0    19183 2023-05-20 13:57:37.164948 prodvana-0.1.4/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
--rw-r--r--   0        0        0    18983 2023-05-20 13:57:37.364947 prodvana-0.1.4/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
--rw-r--r--   0        0        0    22573 2023-05-20 13:57:37.164948 prodvana-0.1.4/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
--rw-r--r--   0        0        0     6760 2023-05-20 13:57:37.364947 prodvana-0.1.4/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.516946 prodvana-0.1.4/prodvana/proto/prodvana/application/__init__.py
--rw-r--r--   0        0        0     4200 2023-05-20 13:57:37.204948 prodvana-0.1.4/prodvana/proto/prodvana/application/application_config_pb2.py
--rw-r--r--   0        0        0     4693 2023-05-20 13:57:37.404946 prodvana-0.1.4/prodvana/proto/prodvana/application/application_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.208948 prodvana-0.1.4/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.404946 prodvana-0.1.4/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    24873 2023-05-20 13:57:37.208948 prodvana-0.1.4/prodvana/proto/prodvana/application/application_manager_pb2.py
--rw-r--r--   0        0        0    16394 2023-05-20 13:57:37.396947 prodvana-0.1.4/prodvana/proto/prodvana/application/application_manager_pb2.pyi
--rw-r--r--   0        0        0    22241 2023-05-20 13:57:37.204948 prodvana-0.1.4/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6755 2023-05-20 13:57:37.400946 prodvana-0.1.4/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2801 2023-05-20 13:57:37.208948 prodvana-0.1.4/prodvana/proto/prodvana/application/object_pb2.py
--rw-r--r--   0        0        0     2184 2023-05-20 13:57:37.400946 prodvana-0.1.4/prodvana/proto/prodvana/application/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.204948 prodvana-0.1.4/prodvana/proto/prodvana/application/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.400946 prodvana-0.1.4/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     2294 2023-05-20 13:57:37.212948 prodvana-0.1.4/prodvana/proto/prodvana/application/user_metadata_pb2.py
--rw-r--r--   0        0        0     1670 2023-05-20 13:57:37.396947 prodvana-0.1.4/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.200948 prodvana-0.1.4/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.404946 prodvana-0.1.4/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.516946 prodvana-0.1.4/prodvana/proto/prodvana/auth/__init__.py
--rw-r--r--   0        0        0    13908 2023-05-20 13:57:37.196948 prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_manager_pb2.py
--rw-r--r--   0        0        0    10206 2023-05-20 13:57:37.392947 prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
--rw-r--r--   0        0        0    18631 2023-05-20 13:57:37.200948 prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6767 2023-05-20 13:57:37.396947 prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     5071 2023-05-20 13:57:37.196948 prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_pb2.py
--rw-r--r--   0        0        0     5515 2023-05-20 13:57:37.392947 prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.196948 prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.392947 prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.484946 prodvana-0.1.4/prodvana/proto/prodvana/blobs/__init__.py
--rw-r--r--   0        0        0     2876 2023-05-20 13:57:37.092949 prodvana-0.1.4/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
--rw-r--r--   0        0        0     1129 2023-05-20 13:57:37.304947 prodvana-0.1.4/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
--rw-r--r--   0        0        0     2704 2023-05-20 13:57:37.092949 prodvana-0.1.4/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
--rw-r--r--   0        0        0      895 2023-05-20 13:57:37.308947 prodvana-0.1.4/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.504946 prodvana-0.1.4/prodvana/proto/prodvana/capability/__init__.py
--rw-r--r--   0        0        0     6823 2023-05-20 13:57:37.160948 prodvana-0.1.4/prodvana/proto/prodvana/capability/capability_pb2.py
--rw-r--r--   0        0        0     5455 2023-05-20 13:57:37.360947 prodvana-0.1.4/prodvana/proto/prodvana/capability/capability_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.160948 prodvana-0.1.4/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.364947 prodvana-0.1.4/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.520946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/__init__.py
--rw-r--r--   0        0        0     1595 2023-05-20 13:57:37.236948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
--rw-r--r--   0        0        0      869 2023-05-20 13:57:37.436946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.252947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.428946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
--rw-r--r--   0        0        0     2659 2023-05-20 13:57:37.232948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/env_pb2.py
--rw-r--r--   0        0        0     2017 2023-05-20 13:57:37.436946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/env_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.252947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.456946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
--rw-r--r--   0        0        0     3634 2023-05-20 13:57:37.240948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/external_config_pb2.py
--rw-r--r--   0        0        0     4163 2023-05-20 13:57:37.440946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/external_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.260948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/external_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.456946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/external_config_pb2_grpc.pyi
--rw-r--r--   0        0        0     5630 2023-05-20 13:57:37.252947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/helm_pb2.py
--rw-r--r--   0        0        0     5448 2023-05-20 13:57:37.440946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/helm_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.256947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.448946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
--rw-r--r--   0        0        0     1890 2023-05-20 13:57:37.268947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/links_pb2.py
--rw-r--r--   0        0        0      846 2023-05-20 13:57:37.432946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/links_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.248947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.444946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
--rw-r--r--   0        0        0     1384 2023-05-20 13:57:37.240948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/maturity_pb2.py
--rw-r--r--   0        0        0     1103 2023-05-20 13:57:37.424946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.236948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.440946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
--rw-r--r--   0        0        0     2541 2023-05-20 13:57:37.244948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/meta_pb2.py
--rw-r--r--   0        0        0     2531 2023-05-20 13:57:37.424946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.232948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.432946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0     2516 2023-05-20 13:57:37.256947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/notification_pb2.py
--rw-r--r--   0        0        0     1337 2023-05-20 13:57:37.428946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.228948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.448946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
--rw-r--r--   0        0        0    10776 2023-05-20 13:57:37.248947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/parameters_pb2.py
--rw-r--r--   0        0        0     8692 2023-05-20 13:57:37.448946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.260948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.456946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0    13928 2023-05-20 13:57:37.264948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/program_pb2.py
--rw-r--r--   0        0        0    15915 2023-05-20 13:57:37.452946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/program_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.264948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.428946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
--rw-r--r--   0        0        0     1837 2023-05-20 13:57:37.260948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/ref_pb2.py
--rw-r--r--   0        0        0      743 2023-05-20 13:57:37.432946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/ref_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.236948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/ref_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.436946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/ref_pb2_grpc.pyi
--rw-r--r--   0        0        0     3229 2023-05-20 13:57:37.240948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/retry_pb2.py
--rw-r--r--   0        0        0     2757 2023-05-20 13:57:37.444946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/retry_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.244948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.444946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
--rw-r--r--   0        0        0     2192 2023-05-20 13:57:37.248947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/task_pb2.py
--rw-r--r--   0        0        0     1490 2023-05-20 13:57:37.424946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.244948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.452946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
--rw-r--r--   0        0        0     1929 2023-05-20 13:57:37.264948 prodvana-0.1.4/prodvana/proto/prodvana/common_config/version_push_pb2.py
--rw-r--r--   0        0        0     1782 2023-05-20 13:57:37.452946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/version_push_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.256947 prodvana-0.1.4/prodvana/proto/prodvana/common_config/version_push_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.436946 prodvana-0.1.4/prodvana/proto/prodvana/common_config/version_push_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.492946 prodvana-0.1.4/prodvana/proto/prodvana/config_file/__init__.py
--rw-r--r--   0        0        0     3576 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/config_file/config_pb2.py
--rw-r--r--   0        0        0     4132 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/config_file/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.104948 prodvana-0.1.4/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.320947 prodvana-0.1.4/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.488946 prodvana-0.1.4/prodvana/proto/prodvana/config_writeback/__init__.py
--rw-r--r--   0        0        0     1648 2023-05-20 13:57:37.100948 prodvana-0.1.4/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
--rw-r--r--   0        0        0     1131 2023-05-20 13:57:37.312947 prodvana-0.1.4/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.100948 prodvana-0.1.4/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.316947 prodvana-0.1.4/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.524946 prodvana-0.1.4/prodvana/proto/prodvana/delivery/__init__.py
--rw-r--r--   0        0        0     2652 2023-05-20 13:57:37.272947 prodvana-0.1.4/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
--rw-r--r--   0        0        0     2294 2023-05-20 13:57:37.464946 prodvana-0.1.4/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.272947 prodvana-0.1.4/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.464946 prodvana-0.1.4/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/__init__.py
--rw-r--r--   0        0        0     6840 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/config_pb2.py
--rw-r--r--   0        0        0     6043 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/config_pb2_grpc.pyi
--rw-r--r--   0        0        0    11266 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/manager_pb2.py
--rw-r--r--   0        0        0     7072 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/manager_pb2.pyi
--rw-r--r--   0        0        0    10633 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3123 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2566 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/object_pb2.py
--rw-r--r--   0        0        0     1823 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 14:21:41.769423 prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/object_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.508946 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/__init__.py
--rw-r--r--   0        0        0    33432 2023-05-20 13:57:37.172948 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/manager_pb2.py
--rw-r--r--   0        0        0    28076 2023-05-20 13:57:37.372947 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
--rw-r--r--   0        0        0    18226 2023-05-20 13:57:37.176948 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
--rw-r--r--   0        0        0     5259 2023-05-20 13:57:37.372947 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.512946 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/__init__.py
--rw-r--r--   0        0        0    36441 2023-05-20 13:57:37.176948 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
--rw-r--r--   0        0        0    61690 2023-05-20 13:57:37.376947 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.180948 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.380947 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
--rw-r--r--   0        0        0     3895 2023-05-20 13:57:37.180948 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
--rw-r--r--   0        0        0     7903 2023-05-20 13:57:37.376947 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.180948 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.376947 prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.504946 prodvana-0.1.4/prodvana/proto/prodvana/environment/__init__.py
--rw-r--r--   0        0        0    17651 2023-05-20 13:57:37.168948 prodvana-0.1.4/prodvana/proto/prodvana/environment/clusters_pb2.py
--rw-r--r--   0        0        0    23424 2023-05-20 13:57:37.372947 prodvana-0.1.4/prodvana/proto/prodvana/environment/clusters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.168948 prodvana-0.1.4/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.368947 prodvana-0.1.4/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
--rw-r--r--   0        0        0    18211 2023-05-20 13:57:37.172948 prodvana-0.1.4/prodvana/proto/prodvana/environment/environment_manager_pb2.py
--rw-r--r--   0        0        0    14932 2023-05-20 13:57:37.368947 prodvana-0.1.4/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
--rw-r--r--   0        0        0    17792 2023-05-20 13:57:37.168948 prodvana-0.1.4/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
--rw-r--r--   0        0        0     5195 2023-05-20 13:57:37.368947 prodvana-0.1.4/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.496946 prodvana-0.1.4/prodvana/proto/prodvana/events/__init__.py
--rw-r--r--   0        0        0     6416 2023-05-20 13:57:37.116948 prodvana-0.1.4/prodvana/proto/prodvana/events/events_manager_pb2.py
--rw-r--r--   0        0        0     5547 2023-05-20 13:57:37.332947 prodvana-0.1.4/prodvana/proto/prodvana/events/events_manager_pb2.pyi
--rw-r--r--   0        0        0     2714 2023-05-20 13:57:37.120948 prodvana-0.1.4/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
--rw-r--r--   0        0        0      853 2023-05-20 13:57:37.332947 prodvana-0.1.4/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     3627 2023-05-20 13:57:37.120948 prodvana-0.1.4/prodvana/proto/prodvana/events/events_pb2.py
--rw-r--r--   0        0        0     4131 2023-05-20 13:57:37.328947 prodvana-0.1.4/prodvana/proto/prodvana/events/events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.116948 prodvana-0.1.4/prodvana/proto/prodvana/events/events_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.332947 prodvana-0.1.4/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
--rw-r--r--   0        0        0    15940 2023-05-20 13:57:37.116948 prodvana-0.1.4/prodvana/proto/prodvana/events/types_pb2.py
--rw-r--r--   0        0        0    30800 2023-05-20 13:57:37.328947 prodvana-0.1.4/prodvana/proto/prodvana/events/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.124948 prodvana-0.1.4/prodvana/proto/prodvana/events/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.328947 prodvana-0.1.4/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.512946 prodvana-0.1.4/prodvana/proto/prodvana/insights/__init__.py
--rw-r--r--   0        0        0     3041 2023-05-20 13:57:37.188948 prodvana-0.1.4/prodvana/proto/prodvana/insights/insights_pb2.py
--rw-r--r--   0        0        0     3508 2023-05-20 13:57:37.384947 prodvana-0.1.4/prodvana/proto/prodvana/insights/insights_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.188948 prodvana-0.1.4/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.388947 prodvana-0.1.4/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.520946 prodvana-0.1.4/prodvana/proto/prodvana/managed_resource/__init__.py
--rw-r--r--   0        0        0    14774 2023-05-20 13:57:37.228948 prodvana-0.1.4/prodvana/proto/prodvana/managed_resource/manager_pb2.py
--rw-r--r--   0        0        0    13338 2023-05-20 13:57:37.420946 prodvana-0.1.4/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
--rw-r--r--   0        0        0    12065 2023-05-20 13:57:37.228948 prodvana-0.1.4/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3657 2023-05-20 13:57:37.420946 prodvana-0.1.4/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.504946 prodvana-0.1.4/prodvana/proto/prodvana/metrics/__init__.py
--rw-r--r--   0        0        0     5507 2023-05-20 13:57:37.156948 prodvana-0.1.4/prodvana/proto/prodvana/metrics/metrics_pb2.py
--rw-r--r--   0        0        0     8746 2023-05-20 13:57:37.360947 prodvana-0.1.4/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.160948 prodvana-0.1.4/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.360947 prodvana-0.1.4/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.496946 prodvana-0.1.4/prodvana/proto/prodvana/object/__init__.py
--rw-r--r--   0        0        0     1844 2023-05-20 13:57:37.128948 prodvana-0.1.4/prodvana/proto/prodvana/object/meta_pb2.py
--rw-r--r--   0        0        0     1957 2023-05-20 13:57:37.336947 prodvana-0.1.4/prodvana/proto/prodvana/object/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.128948 prodvana-0.1.4/prodvana/proto/prodvana/object/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.340947 prodvana-0.1.4/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.512946 prodvana-0.1.4/prodvana/proto/prodvana/organization/__init__.py
--rw-r--r--   0        0        0    16162 2023-05-20 13:57:37.184948 prodvana-0.1.4/prodvana/proto/prodvana/organization/organization_manager_pb2.py
--rw-r--r--   0        0        0     9762 2023-05-20 13:57:37.384947 prodvana-0.1.4/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
--rw-r--r--   0        0        0    14668 2023-05-20 13:57:37.184948 prodvana-0.1.4/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
--rw-r--r--   0        0        0     4779 2023-05-20 13:57:37.380947 prodvana-0.1.4/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2859 2023-05-20 13:57:37.188948 prodvana-0.1.4/prodvana/proto/prodvana/organization/user_metadata_pb2.py
--rw-r--r--   0        0        0     1972 2023-05-20 13:57:37.380947 prodvana-0.1.4/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.184948 prodvana-0.1.4/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.384947 prodvana-0.1.4/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.500946 prodvana-0.1.4/prodvana/proto/prodvana/pipelines/__init__.py
--rw-r--r--   0        0        0     7494 2023-05-20 13:57:37.144948 prodvana-0.1.4/prodvana/proto/prodvana/pipelines/object_pb2.py
--rw-r--r--   0        0        0    10914 2023-05-20 13:57:37.348947 prodvana-0.1.4/prodvana/proto/prodvana/pipelines/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.140948 prodvana-0.1.4/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.344947 prodvana-0.1.4/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
--rw-r--r--   0        0        0    10003 2023-05-20 13:57:37.144948 prodvana-0.1.4/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
--rw-r--r--   0        0        0    11698 2023-05-20 13:57:37.348947 prodvana-0.1.4/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.136948 prodvana-0.1.4/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.348947 prodvana-0.1.4/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.484946 prodvana-0.1.4/prodvana/proto/prodvana/protection/__init__.py
--rw-r--r--   0        0        0     3412 2023-05-20 13:57:37.080949 prodvana-0.1.4/prodvana/proto/prodvana/protection/attachments_pb2.py
--rw-r--r--   0        0        0     2828 2023-05-20 13:57:37.292947 prodvana-0.1.4/prodvana/proto/prodvana/protection/attachments_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.068949 prodvana-0.1.4/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.296947 prodvana-0.1.4/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
--rw-r--r--   0        0        0     1859 2023-05-20 13:57:37.076949 prodvana-0.1.4/prodvana/proto/prodvana/protection/object_pb2.py
--rw-r--r--   0        0        0     1425 2023-05-20 13:57:37.296947 prodvana-0.1.4/prodvana/proto/prodvana/protection/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.072949 prodvana-0.1.4/prodvana/proto/prodvana/protection/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.288947 prodvana-0.1.4/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     8400 2023-05-20 13:57:37.068949 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_config_pb2.py
--rw-r--r--   0        0        0     8865 2023-05-20 13:57:37.300947 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.076949 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.296947 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    10471 2023-05-20 13:57:37.084949 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_manager_pb2.py
--rw-r--r--   0        0        0     6767 2023-05-20 13:57:37.292947 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
--rw-r--r--   0        0        0    10450 2023-05-20 13:57:37.072949 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
--rw-r--r--   0        0        0     3113 2023-05-20 13:57:37.296947 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     6255 2023-05-20 13:57:37.080949 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_reference_pb2.py
--rw-r--r--   0        0        0     4847 2023-05-20 13:57:37.292947 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.076949 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.288947 prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.500946 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/__init__.py
--rw-r--r--   0        0        0     3574 2023-05-20 13:57:37.152948 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/object_pb2.py
--rw-r--r--   0        0        0     3325 2023-05-20 13:57:37.356947 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.148948 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.352947 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
--rw-r--r--   0        0        0    12153 2023-05-20 13:57:37.156948 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
--rw-r--r--   0        0        0    12710 2023-05-20 13:57:37.356947 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.148948 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.352947 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    11989 2023-05-20 13:57:37.152948 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
--rw-r--r--   0        0        0     7509 2023-05-20 13:57:37.352947 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
--rw-r--r--   0        0        0    13099 2023-05-20 13:57:37.148948 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
--rw-r--r--   0        0        0     4150 2023-05-20 13:57:37.356947 prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.516946 prodvana-0.1.4/prodvana/proto/prodvana/repo/__init__.py
--rw-r--r--   0        0        0     2441 2023-05-20 13:57:37.192948 prodvana-0.1.4/prodvana/proto/prodvana/repo/repo_pb2.py
--rw-r--r--   0        0        0     2315 2023-05-20 13:57:37.388947 prodvana-0.1.4/prodvana/proto/prodvana/repo/repo_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.192948 prodvana-0.1.4/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.388947 prodvana-0.1.4/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.484946 prodvana-0.1.4/prodvana/proto/prodvana/runtimes/__init__.py
--rw-r--r--   0        0        0     1559 2023-05-20 13:57:37.084949 prodvana-0.1.4/prodvana/proto/prodvana/runtimes/extensions_pb2.py
--rw-r--r--   0        0        0     1360 2023-05-20 13:57:37.300947 prodvana-0.1.4/prodvana/proto/prodvana/runtimes/extensions_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.088949 prodvana-0.1.4/prodvana/proto/prodvana/runtimes/extensions_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.304947 prodvana-0.1.4/prodvana/proto/prodvana/runtimes/extensions_pb2_grpc.pyi
--rw-r--r--   0        0        0     7542 2023-05-20 13:57:37.088949 prodvana-0.1.4/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
--rw-r--r--   0        0        0     6671 2023-05-20 13:57:37.300947 prodvana-0.1.4/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.084949 prodvana-0.1.4/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.304947 prodvana-0.1.4/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.492946 prodvana-0.1.4/prodvana/proto/prodvana/scm/__init__.py
--rw-r--r--   0        0        0     1265 2023-05-20 13:57:37.108949 prodvana-0.1.4/prodvana/proto/prodvana/scm/types_pb2.py
--rw-r--r--   0        0        0      914 2023-05-20 13:57:37.324947 prodvana-0.1.4/prodvana/proto/prodvana/scm/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.108949 prodvana-0.1.4/prodvana/proto/prodvana/scm/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.320947 prodvana-0.1.4/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.488946 prodvana-0.1.4/prodvana/proto/prodvana/secrets/__init__.py
--rw-r--r--   0        0        0    10074 2023-05-20 13:57:37.100948 prodvana-0.1.4/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
--rw-r--r--   0        0        0     4586 2023-05-20 13:57:37.312947 prodvana-0.1.4/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
--rw-r--r--   0        0        0     9936 2023-05-20 13:57:37.096948 prodvana-0.1.4/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
--rw-r--r--   0        0        0     2847 2023-05-20 13:57:37.312947 prodvana-0.1.4/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.520946 prodvana-0.1.4/prodvana/proto/prodvana/service/__init__.py
--rw-r--r--   0        0        0     5498 2023-05-20 13:57:37.216948 prodvana-0.1.4/prodvana/proto/prodvana/service/object_pb2.py
--rw-r--r--   0        0        0     5760 2023-05-20 13:57:37.412947 prodvana-0.1.4/prodvana/proto/prodvana/service/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.216948 prodvana-0.1.4/prodvana/proto/prodvana/service/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.408946 prodvana-0.1.4/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     2655 2023-05-20 13:57:37.220948 prodvana-0.1.4/prodvana/proto/prodvana/service/parameters_pb2.py
--rw-r--r--   0        0        0     2424 2023-05-20 13:57:37.416947 prodvana-0.1.4/prodvana/proto/prodvana/service/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.224948 prodvana-0.1.4/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.420946 prodvana-0.1.4/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0    30923 2023-05-20 13:57:37.220948 prodvana-0.1.4/prodvana/proto/prodvana/service/service_config_pb2.py
--rw-r--r--   0        0        0    42140 2023-05-20 13:57:37.412947 prodvana-0.1.4/prodvana/proto/prodvana/service/service_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.220948 prodvana-0.1.4/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.416947 prodvana-0.1.4/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    47994 2023-05-20 13:57:37.216948 prodvana-0.1.4/prodvana/proto/prodvana/service/service_manager_pb2.py
--rw-r--r--   0        0        0    38013 2023-05-20 13:57:37.412947 prodvana-0.1.4/prodvana/proto/prodvana/service/service_manager_pb2.pyi
--rw-r--r--   0        0        0    33828 2023-05-20 13:57:37.224948 prodvana-0.1.4/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
--rw-r--r--   0        0        0     9674 2023-05-20 13:57:37.408946 prodvana-0.1.4/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2934 2023-05-20 13:57:37.224948 prodvana-0.1.4/prodvana/proto/prodvana/service/user_metadata_pb2.py
--rw-r--r--   0        0        0     2106 2023-05-20 13:57:37.408946 prodvana-0.1.4/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.212948 prodvana-0.1.4/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.416947 prodvana-0.1.4/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.492946 prodvana-0.1.4/prodvana/proto/prodvana/settings/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.492946 prodvana-0.1.4/prodvana/proto/prodvana/settings/organization/__init__.py
--rw-r--r--   0        0        0     8509 2023-05-20 13:57:37.104948 prodvana-0.1.4/prodvana/proto/prodvana/settings/organization/users_pb2.py
--rw-r--r--   0        0        0     5677 2023-05-20 13:57:37.316947 prodvana-0.1.4/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
--rw-r--r--   0        0        0     8214 2023-05-20 13:57:37.104948 prodvana-0.1.4/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
--rw-r--r--   0        0        0     2318 2023-05-20 13:57:37.316947 prodvana-0.1.4/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.496946 prodvana-0.1.4/prodvana/proto/prodvana/stat/__init__.py
--rw-r--r--   0        0        0     1530 2023-05-20 13:57:37.112949 prodvana-0.1.4/prodvana/proto/prodvana/stat/efficiency_pb2.py
--rw-r--r--   0        0        0     1156 2023-05-20 13:57:37.324947 prodvana-0.1.4/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.112949 prodvana-0.1.4/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.324947 prodvana-0.1.4/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.520946 prodvana-0.1.4/prodvana/proto/prodvana/template/__init__.py
--rw-r--r--   0        0        0     2429 2023-05-20 13:57:37.268947 prodvana-0.1.4/prodvana/proto/prodvana/template/service_pb2.py
--rw-r--r--   0        0        0     1768 2023-05-20 13:57:37.460946 prodvana-0.1.4/prodvana/proto/prodvana/template/service_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.268947 prodvana-0.1.4/prodvana/proto/prodvana/template/service_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.460946 prodvana-0.1.4/prodvana/proto/prodvana/template/service_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.484946 prodvana-0.1.4/prodvana/proto/prodvana/users/__init__.py
--rw-r--r--   0        0        0     1505 2023-05-20 13:57:37.068949 prodvana-0.1.4/prodvana/proto/prodvana/users/users_pb2.py
--rw-r--r--   0        0        0     1451 2023-05-20 13:57:37.284947 prodvana-0.1.4/prodvana/proto/prodvana/users/users_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.064949 prodvana-0.1.4/prodvana/proto/prodvana/users/users_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.288947 prodvana-0.1.4/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.496946 prodvana-0.1.4/prodvana/proto/prodvana/version/__init__.py
--rw-r--r--   0        0        0     2099 2023-05-20 13:57:37.124948 prodvana-0.1.4/prodvana/proto/prodvana/version/source_metadata_pb2.py
--rw-r--r--   0        0        0     2255 2023-05-20 13:57:37.336947 prodvana-0.1.4/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.124948 prodvana-0.1.4/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.336947 prodvana-0.1.4/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.488946 prodvana-0.1.4/prodvana/proto/prodvana/volumes/__init__.py
--rw-r--r--   0        0        0     4805 2023-05-20 13:57:37.092949 prodvana-0.1.4/prodvana/proto/prodvana/volumes/volumes_pb2.py
--rw-r--r--   0        0        0     4793 2023-05-20 13:57:37.308947 prodvana-0.1.4/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.096948 prodvana-0.1.4/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.308947 prodvana-0.1.4/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.500946 prodvana-0.1.4/prodvana/proto/prodvana/workflow/__init__.py
--rw-r--r--   0        0        0     5412 2023-05-20 13:57:37.132948 prodvana-0.1.4/prodvana/proto/prodvana/workflow/integration_config_pb2.py
--rw-r--r--   0        0        0     4328 2023-05-20 13:57:37.340947 prodvana-0.1.4/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.132948 prodvana-0.1.4/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.340947 prodvana-0.1.4/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    69010 2023-05-20 13:57:37.132948 prodvana-0.1.4/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
--rw-r--r--   0        0        0    50096 2023-05-20 13:57:37.344947 prodvana-0.1.4/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
--rw-r--r--   0        0        0    55859 2023-05-20 13:57:37.136948 prodvana-0.1.4/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
--rw-r--r--   0        0        0    16155 2023-05-20 13:57:37.344947 prodvana-0.1.4/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-20 13:57:37.524946 prodvana-0.1.4/prodvana/proto/validate/__init__.py
--rw-r--r--   0        0        0    21204 2023-05-20 13:57:37.284947 prodvana-0.1.4/prodvana/proto/validate/validate_pb2.py
--rw-r--r--   0        0        0    64630 2023-05-20 13:57:37.476946 prodvana-0.1.4/prodvana/proto/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-20 13:57:37.280947 prodvana-0.1.4/prodvana/proto/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-05-20 13:57:37.476946 prodvana-0.1.4/prodvana/proto/validate/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.901495 prodvana-0.1.4/prodvana/py.typed
--rw-r--r--   0        0        0        0 2023-05-19 19:00:48.901495 prodvana-0.1.4/prodvana/utils/__init__.py
--rw-r--r--   0        0        0      538 2023-05-19 19:00:48.901495 prodvana-0.1.4/prodvana/utils/desired_states.py
--rw-r--r--   0        0        0     4079 2023-05-20 03:23:03.669262 prodvana-0.1.4/prodvana/utils/service_config.py
--rw-r--r--   0        0        0     7140 2023-05-20 03:23:03.669262 prodvana-0.1.4/prodvana/utils/tests/test_service_config.py
--rw-r--r--   0        0        0      741 2023-05-20 03:23:03.669262 prodvana-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 prodvana-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       81 2023-05-19 19:00:48.877495 prodvana-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 19:00:48.877495 prodvana-0.1.5/prodvana/__init__.py
+-rw-r--r--   0        0        0     3529 2023-05-19 23:43:46.670463 prodvana-0.1.5/prodvana/client.py
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.883145 prodvana-0.1.5/prodvana/proto/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.883145 prodvana-0.1.5/prodvana/proto/prodvana/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.907145 prodvana-0.1.5/prodvana/proto/prodvana/agent/__init__.py
+-rw-r--r--   0        0        0    19183 2023-05-26 21:53:53.515147 prodvana-0.1.5/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
+-rw-r--r--   0        0        0    18983 2023-05-26 21:53:53.747146 prodvana-0.1.5/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
+-rw-r--r--   0        0        0    22573 2023-05-26 21:53:53.515147 prodvana-0.1.5/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
+-rw-r--r--   0        0        0     6760 2023-05-26 21:53:53.751146 prodvana-0.1.5/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.915145 prodvana-0.1.5/prodvana/proto/prodvana/application/__init__.py
+-rw-r--r--   0        0        0     4200 2023-05-26 21:53:53.555147 prodvana-0.1.5/prodvana/proto/prodvana/application/application_config_pb2.py
+-rw-r--r--   0        0        0     4693 2023-05-26 21:53:53.803146 prodvana-0.1.5/prodvana/proto/prodvana/application/application_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.559147 prodvana-0.1.5/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.799146 prodvana-0.1.5/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    24873 2023-05-26 21:53:53.559147 prodvana-0.1.5/prodvana/proto/prodvana/application/application_manager_pb2.py
+-rw-r--r--   0        0        0    16394 2023-05-26 21:53:53.791146 prodvana-0.1.5/prodvana/proto/prodvana/application/application_manager_pb2.pyi
+-rw-r--r--   0        0        0    22241 2023-05-26 21:53:53.551147 prodvana-0.1.5/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6755 2023-05-26 21:53:53.795146 prodvana-0.1.5/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2801 2023-05-26 21:53:53.559147 prodvana-0.1.5/prodvana/proto/prodvana/application/object_pb2.py
+-rw-r--r--   0        0        0     2184 2023-05-26 21:53:53.799146 prodvana-0.1.5/prodvana/proto/prodvana/application/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.555147 prodvana-0.1.5/prodvana/proto/prodvana/application/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.791146 prodvana-0.1.5/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2294 2023-05-26 21:53:53.563147 prodvana-0.1.5/prodvana/proto/prodvana/application/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1670 2023-05-26 21:53:53.787146 prodvana-0.1.5/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.551147 prodvana-0.1.5/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.803146 prodvana-0.1.5/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.911145 prodvana-0.1.5/prodvana/proto/prodvana/auth/__init__.py
+-rw-r--r--   0        0        0    13908 2023-05-26 21:53:53.547147 prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_manager_pb2.py
+-rw-r--r--   0        0        0    10206 2023-05-26 21:53:53.787146 prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
+-rw-r--r--   0        0        0    18631 2023-05-26 21:53:53.551147 prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6767 2023-05-26 21:53:53.787146 prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5071 2023-05-26 21:53:53.543147 prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_pb2.py
+-rw-r--r--   0        0        0     5515 2023-05-26 21:53:53.783146 prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.547147 prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.783146 prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.887145 prodvana-0.1.5/prodvana/proto/prodvana/blobs/__init__.py
+-rw-r--r--   0        0        0     2876 2023-05-26 21:53:53.443148 prodvana-0.1.5/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
+-rw-r--r--   0        0        0     1129 2023-05-26 21:53:53.675146 prodvana-0.1.5/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
+-rw-r--r--   0        0        0     2704 2023-05-26 21:53:53.443148 prodvana-0.1.5/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
+-rw-r--r--   0        0        0      895 2023-05-26 21:53:53.675146 prodvana-0.1.5/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.903145 prodvana-0.1.5/prodvana/proto/prodvana/capability/__init__.py
+-rw-r--r--   0        0        0     6823 2023-05-26 21:53:53.511147 prodvana-0.1.5/prodvana/proto/prodvana/capability/capability_pb2.py
+-rw-r--r--   0        0        0     5455 2023-05-26 21:53:53.743146 prodvana-0.1.5/prodvana/proto/prodvana/capability/capability_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.511147 prodvana-0.1.5/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.747146 prodvana-0.1.5/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.915145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/__init__.py
+-rw-r--r--   0        0        0     1595 2023-05-26 21:53:53.587147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
+-rw-r--r--   0        0        0      869 2023-05-26 21:53:53.839145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.611147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.835145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2659 2023-05-26 21:53:53.587147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/env_pb2.py
+-rw-r--r--   0        0        0     2017 2023-05-26 21:53:53.843145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/env_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.611147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.863145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5636 2023-05-26 21:53:53.611147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/helm_pb2.py
+-rw-r--r--   0        0        0     5454 2023-05-26 21:53:53.847145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/helm_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.615146 prodvana-0.1.5/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.855145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3658 2023-05-26 21:53:53.595147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py
+-rw-r--r--   0        0        0     4110 2023-05-26 21:53:53.847145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.603147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.843145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1890 2023-05-26 21:53:53.623147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/links_pb2.py
+-rw-r--r--   0        0        0      846 2023-05-26 21:53:53.835145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/links_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.607147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.851145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1384 2023-05-26 21:53:53.599147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/maturity_pb2.py
+-rw-r--r--   0        0        0     1103 2023-05-26 21:53:53.831145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.591147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.847145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2541 2023-05-26 21:53:53.599147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/meta_pb2.py
+-rw-r--r--   0        0        0     2531 2023-05-26 21:53:53.827145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.587147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.835145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2516 2023-05-26 21:53:53.615146 prodvana-0.1.5/prodvana/proto/prodvana/common_config/notification_pb2.py
+-rw-r--r--   0        0        0     1337 2023-05-26 21:53:53.831145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.583147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.859145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
+-rw-r--r--   0        0        0    12624 2023-05-26 21:53:53.607147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/parameters_pb2.py
+-rw-r--r--   0        0        0    10735 2023-05-26 21:53:53.855145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.619147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.863145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    13928 2023-05-26 21:53:53.623147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/program_pb2.py
+-rw-r--r--   0        0        0    15915 2023-05-26 21:53:53.859145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/program_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.623147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.831145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1837 2023-05-26 21:53:53.619147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/ref_pb2.py
+-rw-r--r--   0        0        0      743 2023-05-26 21:53:53.839145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/ref_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.591147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/ref_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.843145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/ref_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3229 2023-05-26 21:53:53.595147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/retry_pb2.py
+-rw-r--r--   0        0        0     2757 2023-05-26 21:53:53.851145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/retry_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.599147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.851145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2192 2023-05-26 21:53:53.607147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/task_pb2.py
+-rw-r--r--   0        0        0     1490 2023-05-26 21:53:53.827145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.603147 prodvana-0.1.5/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.859145 prodvana-0.1.5/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.895145 prodvana-0.1.5/prodvana/proto/prodvana/config_file/__init__.py
+-rw-r--r--   0        0        0     3597 2023-05-26 21:53:53.459148 prodvana-0.1.5/prodvana/proto/prodvana/config_file/config_pb2.py
+-rw-r--r--   0        0        0     4171 2023-05-26 21:53:53.691146 prodvana-0.1.5/prodvana/proto/prodvana/config_file/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.459148 prodvana-0.1.5/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.691146 prodvana-0.1.5/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.891145 prodvana-0.1.5/prodvana/proto/prodvana/config_writeback/__init__.py
+-rw-r--r--   0        0        0     1648 2023-05-26 21:53:53.451147 prodvana-0.1.5/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
+-rw-r--r--   0        0        0     1131 2023-05-26 21:53:53.683146 prodvana-0.1.5/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.451147 prodvana-0.1.5/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.687146 prodvana-0.1.5/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.919145 prodvana-0.1.5/prodvana/proto/prodvana/delivery/__init__.py
+-rw-r--r--   0        0        0     2652 2023-05-26 21:53:53.631147 prodvana-0.1.5/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
+-rw-r--r--   0        0        0     2294 2023-05-26 21:53:53.867145 prodvana-0.1.5/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.631147 prodvana-0.1.5/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.867145 prodvana-0.1.5/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.919145 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/__init__.py
+-rw-r--r--   0        0        0     7053 2023-05-26 21:53:53.639146 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/config_pb2.py
+-rw-r--r--   0        0        0     6102 2023-05-26 21:53:53.875145 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.635146 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.871145 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11893 2023-05-26 21:53:53.639146 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/manager_pb2.py
+-rw-r--r--   0        0        0     7309 2023-05-26 21:53:53.871145 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi
+-rw-r--r--   0        0        0    11002 2023-05-26 21:53:53.643146 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3288 2023-05-26 21:53:53.875145 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2686 2023-05-26 21:53:53.635146 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/object_pb2.py
+-rw-r--r--   0        0        0     1862 2023-05-26 21:53:53.875145 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.635146 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.871145 prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.907145 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/__init__.py
+-rw-r--r--   0        0        0    33432 2023-05-26 21:53:53.523147 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/manager_pb2.py
+-rw-r--r--   0        0        0    28076 2023-05-26 21:53:53.759146 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
+-rw-r--r--   0        0        0    18226 2023-05-26 21:53:53.523147 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     5259 2023-05-26 21:53:53.759146 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.907145 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/__init__.py
+-rw-r--r--   0        0        0    38158 2023-05-26 21:53:53.527147 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
+-rw-r--r--   0        0        0    64686 2023-05-26 21:53:53.767146 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.531147 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.767146 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3895 2023-05-26 21:53:53.527147 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
+-rw-r--r--   0        0        0     7903 2023-05-26 21:53:53.763146 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.531147 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.763146 prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.907145 prodvana-0.1.5/prodvana/proto/prodvana/environment/__init__.py
+-rw-r--r--   0        0        0    18876 2023-05-26 21:55:24.562636 prodvana-0.1.5/prodvana/proto/prodvana/environment/clusters_pb2.py
+-rw-r--r--   0        0        0    24612 2023-05-26 21:55:24.562636 prodvana-0.1.5/prodvana/proto/prodvana/environment/clusters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.519147 prodvana-0.1.5/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.755146 prodvana-0.1.5/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18211 2023-05-26 21:53:53.523147 prodvana-0.1.5/prodvana/proto/prodvana/environment/environment_manager_pb2.py
+-rw-r--r--   0        0        0    14932 2023-05-26 21:53:53.755146 prodvana-0.1.5/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
+-rw-r--r--   0        0        0    17792 2023-05-26 21:53:53.519147 prodvana-0.1.5/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     5195 2023-05-26 21:53:53.751146 prodvana-0.1.5/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.895145 prodvana-0.1.5/prodvana/proto/prodvana/events/__init__.py
+-rw-r--r--   0        0        0     6416 2023-05-26 21:53:53.471147 prodvana-0.1.5/prodvana/proto/prodvana/events/events_manager_pb2.py
+-rw-r--r--   0        0        0     5547 2023-05-26 21:53:53.711146 prodvana-0.1.5/prodvana/proto/prodvana/events/events_manager_pb2.pyi
+-rw-r--r--   0        0        0     2714 2023-05-26 21:53:53.471147 prodvana-0.1.5/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
+-rw-r--r--   0        0        0      853 2023-05-26 21:53:53.707146 prodvana-0.1.5/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3627 2023-05-26 21:53:53.471147 prodvana-0.1.5/prodvana/proto/prodvana/events/events_pb2.py
+-rw-r--r--   0        0        0     4131 2023-05-26 21:53:53.703146 prodvana-0.1.5/prodvana/proto/prodvana/events/events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.467147 prodvana-0.1.5/prodvana/proto/prodvana/events/events_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.707146 prodvana-0.1.5/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
+-rw-r--r--   0        0        0    15940 2023-05-26 21:53:53.467147 prodvana-0.1.5/prodvana/proto/prodvana/events/types_pb2.py
+-rw-r--r--   0        0        0    30800 2023-05-26 21:53:53.703146 prodvana-0.1.5/prodvana/proto/prodvana/events/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.475147 prodvana-0.1.5/prodvana/proto/prodvana/events/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.699146 prodvana-0.1.5/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.911145 prodvana-0.1.5/prodvana/proto/prodvana/insights/__init__.py
+-rw-r--r--   0        0        0     3041 2023-05-26 21:53:53.539147 prodvana-0.1.5/prodvana/proto/prodvana/insights/insights_pb2.py
+-rw-r--r--   0        0        0     3508 2023-05-26 21:53:53.775146 prodvana-0.1.5/prodvana/proto/prodvana/insights/insights_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.539147 prodvana-0.1.5/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.779146 prodvana-0.1.5/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.915145 prodvana-0.1.5/prodvana/proto/prodvana/managed_resource/__init__.py
+-rw-r--r--   0        0        0    14774 2023-05-26 21:53:53.579147 prodvana-0.1.5/prodvana/proto/prodvana/managed_resource/manager_pb2.py
+-rw-r--r--   0        0        0    13338 2023-05-26 21:53:53.823145 prodvana-0.1.5/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
+-rw-r--r--   0        0        0    12065 2023-05-26 21:53:53.583147 prodvana-0.1.5/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3657 2023-05-26 21:53:53.827145 prodvana-0.1.5/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.903145 prodvana-0.1.5/prodvana/proto/prodvana/metrics/__init__.py
+-rw-r--r--   0        0        0     5507 2023-05-26 21:53:53.507147 prodvana-0.1.5/prodvana/proto/prodvana/metrics/metrics_pb2.py
+-rw-r--r--   0        0        0     8746 2023-05-26 21:53:53.739146 prodvana-0.1.5/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.507147 prodvana-0.1.5/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.743146 prodvana-0.1.5/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.899145 prodvana-0.1.5/prodvana/proto/prodvana/object/__init__.py
+-rw-r--r--   0        0        0     1844 2023-05-26 21:53:53.479147 prodvana-0.1.5/prodvana/proto/prodvana/object/meta_pb2.py
+-rw-r--r--   0        0        0     1957 2023-05-26 21:53:53.715146 prodvana-0.1.5/prodvana/proto/prodvana/object/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.479147 prodvana-0.1.5/prodvana/proto/prodvana/object/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.715146 prodvana-0.1.5/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.911145 prodvana-0.1.5/prodvana/proto/prodvana/organization/__init__.py
+-rw-r--r--   0        0        0    16162 2023-05-26 21:53:53.535147 prodvana-0.1.5/prodvana/proto/prodvana/organization/organization_manager_pb2.py
+-rw-r--r--   0        0        0     9762 2023-05-26 21:53:53.775146 prodvana-0.1.5/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
+-rw-r--r--   0        0        0    14668 2023-05-26 21:53:53.535147 prodvana-0.1.5/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4779 2023-05-26 21:53:53.771146 prodvana-0.1.5/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2859 2023-05-26 21:53:53.539147 prodvana-0.1.5/prodvana/proto/prodvana/organization/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1972 2023-05-26 21:53:53.767146 prodvana-0.1.5/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.531147 prodvana-0.1.5/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.771146 prodvana-0.1.5/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.903145 prodvana-0.1.5/prodvana/proto/prodvana/pipelines/__init__.py
+-rw-r--r--   0        0        0     2598 2023-05-26 21:53:53.491147 prodvana-0.1.5/prodvana/proto/prodvana/pipelines/object_pb2.py
+-rw-r--r--   0        0        0     2595 2023-05-26 21:53:53.731146 prodvana-0.1.5/prodvana/proto/prodvana/pipelines/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.491147 prodvana-0.1.5/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.723146 prodvana-0.1.5/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10003 2023-05-26 21:53:53.491147 prodvana-0.1.5/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
+-rw-r--r--   0        0        0    11698 2023-05-26 21:53:53.727146 prodvana-0.1.5/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.487147 prodvana-0.1.5/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.727146 prodvana-0.1.5/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.887145 prodvana-0.1.5/prodvana/proto/prodvana/protection/__init__.py
+-rw-r--r--   0        0        0     3412 2023-05-26 21:53:53.431148 prodvana-0.1.5/prodvana/proto/prodvana/protection/attachments_pb2.py
+-rw-r--r--   0        0        0     2828 2023-05-26 21:53:53.659146 prodvana-0.1.5/prodvana/proto/prodvana/protection/attachments_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.391148 prodvana-0.1.5/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.659146 prodvana-0.1.5/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1907 2023-05-26 21:53:53.399148 prodvana-0.1.5/prodvana/proto/prodvana/protection/object_pb2.py
+-rw-r--r--   0        0        0     1545 2023-05-26 21:53:53.663146 prodvana-0.1.5/prodvana/proto/prodvana/protection/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.395148 prodvana-0.1.5/prodvana/proto/prodvana/protection/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.651147 prodvana-0.1.5/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8407 2023-05-26 21:53:53.395148 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_config_pb2.py
+-rw-r--r--   0        0        0     8891 2023-05-26 21:53:53.667146 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.427148 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.663146 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10471 2023-05-26 21:53:53.435148 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_manager_pb2.py
+-rw-r--r--   0        0        0     6767 2023-05-26 21:53:53.655146 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
+-rw-r--r--   0        0        0    10450 2023-05-26 21:53:53.395148 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3113 2023-05-26 21:53:53.667146 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6409 2023-05-26 21:53:53.431148 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_reference_pb2.py
+-rw-r--r--   0        0        0     4997 2023-05-26 21:53:53.659146 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.427148 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.655146 prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.903145 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/__init__.py
+-rw-r--r--   0        0        0     3574 2023-05-26 21:53:53.503147 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/object_pb2.py
+-rw-r--r--   0        0        0     3325 2023-05-26 21:53:53.735146 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.499147 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.731146 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0    12153 2023-05-26 21:53:53.507147 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
+-rw-r--r--   0        0        0    12710 2023-05-26 21:53:53.739146 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.495147 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.735146 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11989 2023-05-26 21:53:53.503147 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
+-rw-r--r--   0        0        0     7509 2023-05-26 21:53:53.731146 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
+-rw-r--r--   0        0        0    13099 2023-05-26 21:53:53.495147 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4150 2023-05-26 21:53:53.739146 prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.911145 prodvana-0.1.5/prodvana/proto/prodvana/repo/__init__.py
+-rw-r--r--   0        0        0     2441 2023-05-26 21:53:53.543147 prodvana-0.1.5/prodvana/proto/prodvana/repo/repo_pb2.py
+-rw-r--r--   0        0        0     2315 2023-05-26 21:53:53.779146 prodvana-0.1.5/prodvana/proto/prodvana/repo/repo_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.543147 prodvana-0.1.5/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.779146 prodvana-0.1.5/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.887145 prodvana-0.1.5/prodvana/proto/prodvana/runtimes/__init__.py
+-rw-r--r--   0        0        0     1559 2023-05-26 21:53:53.435148 prodvana-0.1.5/prodvana/proto/prodvana/runtimes/extensions_pb2.py
+-rw-r--r--   0        0        0     1360 2023-05-26 21:53:53.667146 prodvana-0.1.5/prodvana/proto/prodvana/runtimes/extensions_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.439148 prodvana-0.1.5/prodvana/proto/prodvana/runtimes/extensions_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.675146 prodvana-0.1.5/prodvana/proto/prodvana/runtimes/extensions_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7542 2023-05-26 21:53:53.439148 prodvana-0.1.5/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
+-rw-r--r--   0        0        0     6671 2023-05-26 21:53:53.671146 prodvana-0.1.5/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.435148 prodvana-0.1.5/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.671146 prodvana-0.1.5/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.895145 prodvana-0.1.5/prodvana/proto/prodvana/scm/__init__.py
+-rw-r--r--   0        0        0     1265 2023-05-26 21:53:53.459148 prodvana-0.1.5/prodvana/proto/prodvana/scm/types_pb2.py
+-rw-r--r--   0        0        0      914 2023-05-26 21:53:53.695146 prodvana-0.1.5/prodvana/proto/prodvana/scm/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.463147 prodvana-0.1.5/prodvana/proto/prodvana/scm/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.695146 prodvana-0.1.5/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.891145 prodvana-0.1.5/prodvana/proto/prodvana/secrets/__init__.py
+-rw-r--r--   0        0        0    10074 2023-05-26 21:53:53.451147 prodvana-0.1.5/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
+-rw-r--r--   0        0        0     4586 2023-05-26 21:53:53.683146 prodvana-0.1.5/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
+-rw-r--r--   0        0        0     9936 2023-05-26 21:53:53.447147 prodvana-0.1.5/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     2847 2023-05-26 21:53:53.683146 prodvana-0.1.5/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.915145 prodvana-0.1.5/prodvana/proto/prodvana/service/__init__.py
+-rw-r--r--   0        0        0     5498 2023-05-26 21:53:53.567147 prodvana-0.1.5/prodvana/proto/prodvana/service/object_pb2.py
+-rw-r--r--   0        0        0     5760 2023-05-26 21:53:53.815146 prodvana-0.1.5/prodvana/proto/prodvana/service/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.567147 prodvana-0.1.5/prodvana/proto/prodvana/service/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.807145 prodvana-0.1.5/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2655 2023-05-26 21:53:53.575147 prodvana-0.1.5/prodvana/proto/prodvana/service/parameters_pb2.py
+-rw-r--r--   0        0        0     2424 2023-05-26 21:53:53.819146 prodvana-0.1.5/prodvana/proto/prodvana/service/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.579147 prodvana-0.1.5/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.823145 prodvana-0.1.5/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    31313 2023-05-26 21:53:53.571147 prodvana-0.1.5/prodvana/proto/prodvana/service/service_config_pb2.py
+-rw-r--r--   0        0        0    44213 2023-05-26 21:53:53.815146 prodvana-0.1.5/prodvana/proto/prodvana/service/service_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.571147 prodvana-0.1.5/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.815146 prodvana-0.1.5/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    47994 2023-05-26 21:53:53.567147 prodvana-0.1.5/prodvana/proto/prodvana/service/service_manager_pb2.py
+-rw-r--r--   0        0        0    38013 2023-05-26 21:53:53.811146 prodvana-0.1.5/prodvana/proto/prodvana/service/service_manager_pb2.pyi
+-rw-r--r--   0        0        0    33828 2023-05-26 21:53:53.575147 prodvana-0.1.5/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     9674 2023-05-26 21:53:53.811146 prodvana-0.1.5/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2934 2023-05-26 21:53:53.575147 prodvana-0.1.5/prodvana/proto/prodvana/service/user_metadata_pb2.py
+-rw-r--r--   0        0        0     2106 2023-05-26 21:53:53.807145 prodvana-0.1.5/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.563147 prodvana-0.1.5/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.819146 prodvana-0.1.5/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.891145 prodvana-0.1.5/prodvana/proto/prodvana/settings/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.895145 prodvana-0.1.5/prodvana/proto/prodvana/settings/organization/__init__.py
+-rw-r--r--   0        0        0     8509 2023-05-26 21:53:53.455148 prodvana-0.1.5/prodvana/proto/prodvana/settings/organization/users_pb2.py
+-rw-r--r--   0        0        0     5677 2023-05-26 21:53:53.687146 prodvana-0.1.5/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
+-rw-r--r--   0        0        0     8214 2023-05-26 21:53:53.455148 prodvana-0.1.5/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
+-rw-r--r--   0        0        0     2318 2023-05-26 21:53:53.691146 prodvana-0.1.5/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.895145 prodvana-0.1.5/prodvana/proto/prodvana/stat/__init__.py
+-rw-r--r--   0        0        0     1530 2023-05-26 21:53:53.463147 prodvana-0.1.5/prodvana/proto/prodvana/stat/efficiency_pb2.py
+-rw-r--r--   0        0        0     1156 2023-05-26 21:53:53.699146 prodvana-0.1.5/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.467147 prodvana-0.1.5/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.699146 prodvana-0.1.5/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.919145 prodvana-0.1.5/prodvana/proto/prodvana/template/__init__.py
+-rw-r--r--   0        0        0     2429 2023-05-26 21:53:53.627147 prodvana-0.1.5/prodvana/proto/prodvana/template/service_pb2.py
+-rw-r--r--   0        0        0     1768 2023-05-26 21:53:53.863145 prodvana-0.1.5/prodvana/proto/prodvana/template/service_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.627147 prodvana-0.1.5/prodvana/proto/prodvana/template/service_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.867145 prodvana-0.1.5/prodvana/proto/prodvana/template/service_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.887145 prodvana-0.1.5/prodvana/proto/prodvana/users/__init__.py
+-rw-r--r--   0        0        0     1505 2023-05-26 21:53:53.391148 prodvana-0.1.5/prodvana/proto/prodvana/users/users_pb2.py
+-rw-r--r--   0        0        0     1451 2023-05-26 21:53:53.647146 prodvana-0.1.5/prodvana/proto/prodvana/users/users_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.387148 prodvana-0.1.5/prodvana/proto/prodvana/users/users_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.651147 prodvana-0.1.5/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.899145 prodvana-0.1.5/prodvana/proto/prodvana/version/__init__.py
+-rw-r--r--   0        0        0     2142 2023-05-26 21:53:53.479147 prodvana-0.1.5/prodvana/proto/prodvana/version/source_metadata_pb2.py
+-rw-r--r--   0        0        0     2646 2023-05-26 21:53:53.711146 prodvana-0.1.5/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.475147 prodvana-0.1.5/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.711146 prodvana-0.1.5/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.891145 prodvana-0.1.5/prodvana/proto/prodvana/volumes/__init__.py
+-rw-r--r--   0        0        0     4805 2023-05-26 21:53:53.443148 prodvana-0.1.5/prodvana/proto/prodvana/volumes/volumes_pb2.py
+-rw-r--r--   0        0        0     4793 2023-05-26 21:53:53.679146 prodvana-0.1.5/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.447147 prodvana-0.1.5/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.679146 prodvana-0.1.5/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.899145 prodvana-0.1.5/prodvana/proto/prodvana/workflow/__init__.py
+-rw-r--r--   0        0        0     5412 2023-05-26 21:53:53.483147 prodvana-0.1.5/prodvana/proto/prodvana/workflow/integration_config_pb2.py
+-rw-r--r--   0        0        0     4328 2023-05-26 21:53:53.719146 prodvana-0.1.5/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.483147 prodvana-0.1.5/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.719146 prodvana-0.1.5/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    69010 2023-05-26 21:53:53.487147 prodvana-0.1.5/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
+-rw-r--r--   0        0        0    50096 2023-05-26 21:53:53.723146 prodvana-0.1.5/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
+-rw-r--r--   0        0        0    55859 2023-05-26 21:53:53.487147 prodvana-0.1.5/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
+-rw-r--r--   0        0        0    16155 2023-05-26 21:53:53.719146 prodvana-0.1.5/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 21:53:53.923145 prodvana-0.1.5/prodvana/proto/validate/__init__.py
+-rw-r--r--   0        0        0    21204 2023-05-26 21:53:53.647146 prodvana-0.1.5/prodvana/proto/validate/validate_pb2.py
+-rw-r--r--   0        0        0    64630 2023-05-26 21:53:53.879145 prodvana-0.1.5/prodvana/proto/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-26 21:53:53.643146 prodvana-0.1.5/prodvana/proto/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-05-26 21:53:53.879145 prodvana-0.1.5/prodvana/proto/validate/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-19 19:00:48.901495 prodvana-0.1.5/prodvana/py.typed
+-rw-r--r--   0        0        0        0 2023-05-19 19:00:48.901495 prodvana-0.1.5/prodvana/utils/__init__.py
+-rw-r--r--   0        0        0      538 2023-05-19 19:00:48.901495 prodvana-0.1.5/prodvana/utils/desired_states.py
+-rw-r--r--   0        0        0     4079 2023-05-20 03:23:03.669262 prodvana-0.1.5/prodvana/utils/service_config.py
+-rw-r--r--   0        0        0     7140 2023-05-20 03:23:03.669262 prodvana-0.1.5/prodvana/utils/tests/test_service_config.py
+-rw-r--r--   0        0        0      746 2023-05-26 22:29:46.734902 prodvana-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 prodvana-0.1.5/PKG-INFO
```

### Comparing `prodvana-0.1.4/prodvana/client.py` & `prodvana-0.1.5/prodvana/client.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/agent/agent_interaction_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/agent/agent_interaction_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py` & `prodvana-0.1.5/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/application/application_config_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/application/application_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/application/application_config_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/application/application_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/application/application_manager_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/application/application_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/application/application_manager_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/application/application_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py` & `prodvana-0.1.5/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/application/object_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/application/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/application/object_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/application/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/application/user_metadata_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/application/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/application/user_metadata_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/application/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_manager_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py` & `prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/auth/auth_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/auth/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py` & `prodvana-0.1.5/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/capability/capability_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/capability/capability_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/capability/capability_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/capability/capability_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/env_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/env_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/env_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/env_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/external_config_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: prodvana/common_config/external_config.proto
+# source: prodvana/common_config/kubernetes_config.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,prodvana/common_config/external_config.proto\x12\x16prodvana.common_config\x1a\x17validate/validate.proto\"$\n\x0bLocalConfig\x12\x15\n\x04path\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\xa9\x03\n\x0e\x45xternalConfig\x12\x39\n\x04type\x18\x01 \x01(\x0e\x32+.prodvana.common_config.ExternalConfig.Type\x12\x1a\n\x07inlined\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01H\x00\x12\x34\n\x05local\x18\x03 \x01(\x0b\x32#.prodvana.common_config.LocalConfigH\x00\x12S\n\x12\x65nv_injection_mode\x18\x04 \x01(\x0e\x32\x37.prodvana.common_config.ExternalConfig.EnvInjectionMode\"<\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0e\n\nKUBERNETES\x10\x01\x12\r\n\tKUSTOMIZE\x10\x02\x12\x08\n\x04HELM\x10\x03\"b\n\x10\x45nvInjectionMode\x12\x16\n\x12\x45NV_INJECT_UNKNOWN\x10\x00\x12\x17\n\x13\x45NV_INJECT_DISABLED\x10\x01\x12\x1d\n\x19\x45NV_INJECT_NON_SECRET_ENV\x10\x02\x42\x13\n\x0csource_oneof\x12\x03\xf8\x42\x01\x42RZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.prodvana/common_config/kubernetes_config.proto\x12\x16prodvana.common_config\x1a\x17validate/validate.proto\"$\n\x0bLocalConfig\x12\x15\n\x04path\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"\xa5\x03\n\x10KubernetesConfig\x12;\n\x04type\x18\x01 \x01(\x0e\x32-.prodvana.common_config.KubernetesConfig.Type\x12\x1a\n\x07inlined\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01H\x00\x12\x34\n\x05local\x18\x03 \x01(\x0b\x32#.prodvana.common_config.LocalConfigH\x00\x12U\n\x12\x65nv_injection_mode\x18\x04 \x01(\x0e\x32\x39.prodvana.common_config.KubernetesConfig.EnvInjectionMode\"2\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0e\n\nKUBERNETES\x10\x01\x12\r\n\tKUSTOMIZE\x10\x02\"b\n\x10\x45nvInjectionMode\x12\x16\n\x12\x45NV_INJECT_UNKNOWN\x10\x00\x12\x17\n\x13\x45NV_INJECT_DISABLED\x10\x01\x12\x1d\n\x19\x45NV_INJECT_NON_SECRET_ENV\x10\x02\x42\x13\n\x0csource_oneof\x12\x03\xf8\x42\x01\x42RZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
 
 
 
 _LOCALCONFIG = DESCRIPTOR.message_types_by_name['LocalConfig']
-_EXTERNALCONFIG = DESCRIPTOR.message_types_by_name['ExternalConfig']
-_EXTERNALCONFIG_TYPE = _EXTERNALCONFIG.enum_types_by_name['Type']
-_EXTERNALCONFIG_ENVINJECTIONMODE = _EXTERNALCONFIG.enum_types_by_name['EnvInjectionMode']
+_KUBERNETESCONFIG = DESCRIPTOR.message_types_by_name['KubernetesConfig']
+_KUBERNETESCONFIG_TYPE = _KUBERNETESCONFIG.enum_types_by_name['Type']
+_KUBERNETESCONFIG_ENVINJECTIONMODE = _KUBERNETESCONFIG.enum_types_by_name['EnvInjectionMode']
 LocalConfig = _reflection.GeneratedProtocolMessageType('LocalConfig', (_message.Message,), {
   'DESCRIPTOR' : _LOCALCONFIG,
-  '__module__' : 'prodvana.common_config.external_config_pb2'
+  '__module__' : 'prodvana.common_config.kubernetes_config_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.common_config.LocalConfig)
   })
 _sym_db.RegisterMessage(LocalConfig)
 
-ExternalConfig = _reflection.GeneratedProtocolMessageType('ExternalConfig', (_message.Message,), {
-  'DESCRIPTOR' : _EXTERNALCONFIG,
-  '__module__' : 'prodvana.common_config.external_config_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.common_config.ExternalConfig)
+KubernetesConfig = _reflection.GeneratedProtocolMessageType('KubernetesConfig', (_message.Message,), {
+  'DESCRIPTOR' : _KUBERNETESCONFIG,
+  '__module__' : 'prodvana.common_config.kubernetes_config_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.common_config.KubernetesConfig)
   })
-_sym_db.RegisterMessage(ExternalConfig)
+_sym_db.RegisterMessage(KubernetesConfig)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_config'
   _LOCALCONFIG.fields_by_name['path']._options = None
   _LOCALCONFIG.fields_by_name['path']._serialized_options = b'\372B\004r\002\020\001'
-  _EXTERNALCONFIG.oneofs_by_name['source_oneof']._options = None
-  _EXTERNALCONFIG.oneofs_by_name['source_oneof']._serialized_options = b'\370B\001'
-  _EXTERNALCONFIG.fields_by_name['inlined']._options = None
-  _EXTERNALCONFIG.fields_by_name['inlined']._serialized_options = b'\372B\004r\002\020\001'
-  _LOCALCONFIG._serialized_start=97
-  _LOCALCONFIG._serialized_end=133
-  _EXTERNALCONFIG._serialized_start=136
-  _EXTERNALCONFIG._serialized_end=561
-  _EXTERNALCONFIG_TYPE._serialized_start=380
-  _EXTERNALCONFIG_TYPE._serialized_end=440
-  _EXTERNALCONFIG_ENVINJECTIONMODE._serialized_start=442
-  _EXTERNALCONFIG_ENVINJECTIONMODE._serialized_end=540
+  _KUBERNETESCONFIG.oneofs_by_name['source_oneof']._options = None
+  _KUBERNETESCONFIG.oneofs_by_name['source_oneof']._serialized_options = b'\370B\001'
+  _KUBERNETESCONFIG.fields_by_name['inlined']._options = None
+  _KUBERNETESCONFIG.fields_by_name['inlined']._serialized_options = b'\372B\004r\002\020\001'
+  _LOCALCONFIG._serialized_start=99
+  _LOCALCONFIG._serialized_end=135
+  _KUBERNETESCONFIG._serialized_start=138
+  _KUBERNETESCONFIG._serialized_end=559
+  _KUBERNETESCONFIG_TYPE._serialized_start=388
+  _KUBERNETESCONFIG_TYPE._serialized_end=438
+  _KUBERNETESCONFIG_ENVINJECTIONMODE._serialized_start=440
+  _KUBERNETESCONFIG_ENVINJECTIONMODE._serialized_end=538
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/external_config_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -26,69 +26,67 @@
         *,
         path: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["path", b"path"]) -> None: ...
 
 global___LocalConfig = LocalConfig
 
-class ExternalConfig(google.protobuf.message.Message):
+class KubernetesConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Type:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
-    class _TypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[ExternalConfig._Type.ValueType], builtins.type):  # noqa: F821
+    class _TypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[KubernetesConfig._Type.ValueType], builtins.type):  # noqa: F821
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
-        UNKNOWN: ExternalConfig._Type.ValueType  # 0
-        KUBERNETES: ExternalConfig._Type.ValueType  # 1
-        KUSTOMIZE: ExternalConfig._Type.ValueType  # 2
-        HELM: ExternalConfig._Type.ValueType  # 3
+        UNKNOWN: KubernetesConfig._Type.ValueType  # 0
+        KUBERNETES: KubernetesConfig._Type.ValueType  # 1
+        KUSTOMIZE: KubernetesConfig._Type.ValueType  # 2
 
     class Type(_Type, metaclass=_TypeEnumTypeWrapper): ...
-    UNKNOWN: ExternalConfig.Type.ValueType  # 0
-    KUBERNETES: ExternalConfig.Type.ValueType  # 1
-    KUSTOMIZE: ExternalConfig.Type.ValueType  # 2
-    HELM: ExternalConfig.Type.ValueType  # 3
+    UNKNOWN: KubernetesConfig.Type.ValueType  # 0
+    KUBERNETES: KubernetesConfig.Type.ValueType  # 1
+    KUSTOMIZE: KubernetesConfig.Type.ValueType  # 2
 
     class _EnvInjectionMode:
         ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
 
-    class _EnvInjectionModeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[ExternalConfig._EnvInjectionMode.ValueType], builtins.type):  # noqa: F821
+    class _EnvInjectionModeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[KubernetesConfig._EnvInjectionMode.ValueType], builtins.type):  # noqa: F821
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
-        ENV_INJECT_UNKNOWN: ExternalConfig._EnvInjectionMode.ValueType  # 0
-        ENV_INJECT_DISABLED: ExternalConfig._EnvInjectionMode.ValueType  # 1
+        ENV_INJECT_UNKNOWN: KubernetesConfig._EnvInjectionMode.ValueType  # 0
+        ENV_INJECT_DISABLED: KubernetesConfig._EnvInjectionMode.ValueType  # 1
         """disables env injection entirely"""
-        ENV_INJECT_NON_SECRET_ENV: ExternalConfig._EnvInjectionMode.ValueType  # 2
+        ENV_INJECT_NON_SECRET_ENV: KubernetesConfig._EnvInjectionMode.ValueType  # 2
         """inject non-secret env values from the Release Channel"""
 
     class EnvInjectionMode(_EnvInjectionMode, metaclass=_EnvInjectionModeEnumTypeWrapper): ...
-    ENV_INJECT_UNKNOWN: ExternalConfig.EnvInjectionMode.ValueType  # 0
-    ENV_INJECT_DISABLED: ExternalConfig.EnvInjectionMode.ValueType  # 1
+    ENV_INJECT_UNKNOWN: KubernetesConfig.EnvInjectionMode.ValueType  # 0
+    ENV_INJECT_DISABLED: KubernetesConfig.EnvInjectionMode.ValueType  # 1
     """disables env injection entirely"""
-    ENV_INJECT_NON_SECRET_ENV: ExternalConfig.EnvInjectionMode.ValueType  # 2
+    ENV_INJECT_NON_SECRET_ENV: KubernetesConfig.EnvInjectionMode.ValueType  # 2
     """inject non-secret env values from the Release Channel"""
 
     TYPE_FIELD_NUMBER: builtins.int
     INLINED_FIELD_NUMBER: builtins.int
     LOCAL_FIELD_NUMBER: builtins.int
     ENV_INJECTION_MODE_FIELD_NUMBER: builtins.int
-    type: global___ExternalConfig.Type.ValueType
+    type: global___KubernetesConfig.Type.ValueType
     inlined: builtins.str
     @property
     def local(self) -> global___LocalConfig: ...
-    env_injection_mode: global___ExternalConfig.EnvInjectionMode.ValueType
+    env_injection_mode: global___KubernetesConfig.EnvInjectionMode.ValueType
     """Defaults to ENV_INJECT_NON_SECRET_ENV"""
     def __init__(
         self,
         *,
-        type: global___ExternalConfig.Type.ValueType = ...,
+        type: global___KubernetesConfig.Type.ValueType = ...,
         inlined: builtins.str = ...,
         local: global___LocalConfig | None = ...,
-        env_injection_mode: global___ExternalConfig.EnvInjectionMode.ValueType = ...,
+        env_injection_mode: global___KubernetesConfig.EnvInjectionMode.ValueType = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["inlined", b"inlined", "local", b"local", "source_oneof", b"source_oneof"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["env_injection_mode", b"env_injection_mode", "inlined", b"inlined", "local", b"local", "source_oneof", b"source_oneof", "type", b"type"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["source_oneof", b"source_oneof"]) -> typing_extensions.Literal["inlined", "local"] | None: ...
 
-global___ExternalConfig = ExternalConfig
+global___KubernetesConfig = KubernetesConfig
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/helm_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/helm_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 from prodvana.proto.prodvana.common_config import env_pb2 as prodvana_dot_common__config_dot_env__pb2
-from prodvana.proto.prodvana.common_config import external_config_pb2 as prodvana_dot_common__config_dot_external__config__pb2
+from prodvana.proto.prodvana.common_config import kubernetes_config_pb2 as prodvana_dot_common__config_dot_kubernetes__config__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!prodvana/common_config/helm.proto\x12\x16prodvana.common_config\x1a\x17validate/validate.proto\x1a prodvana/common_config/env.proto\x1a,prodvana/common_config/external_config.proto\"l\n\x0fRemoteHelmChart\x12\x0e\n\x04repo\x18\x01 \x01(\tH\x00\x12\x16\n\x05\x63hart\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x1e\n\rchart_version\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x42\x11\n\nrepo_oneof\x12\x03\xf8\x42\x01\"\x94\x02\n\x13HelmValuesOverrides\x12\x1a\n\x07inlined\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01H\x00\x12\x34\n\x05local\x18\x02 \x01(\x0b\x32#.prodvana.common_config.LocalConfigH\x00\x12K\n\x03map\x18\x03 \x03(\x0b\x32\x34.prodvana.common_config.HelmValuesOverrides.MapEntryB\x08\xfa\x42\x05\x9a\x01\x02\x18\x01\x1aL\n\x08MapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42\x10\n\x0eoverride_oneof\"\xd4\x01\n\nHelmConfig\x12\x39\n\x06remote\x18\x01 \x01(\x0b\x32\'.prodvana.common_config.RemoteHelmChartH\x00\x12\x45\n\x10values_overrides\x18\x02 \x03(\x0b\x32+.prodvana.common_config.HelmValuesOverrides\x12\x14\n\x0crelease_name\x18\x03 \x01(\t\x12\x1a\n\tnamespace\x18\x04 \x01(\tB\x07\xfa\x42\x04r\x02\x18\x00\x42\x12\n\x0b\x63hart_oneof\x12\x03\xf8\x42\x01\x42RZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!prodvana/common_config/helm.proto\x12\x16prodvana.common_config\x1a\x17validate/validate.proto\x1a prodvana/common_config/env.proto\x1a.prodvana/common_config/kubernetes_config.proto\"l\n\x0fRemoteHelmChart\x12\x0e\n\x04repo\x18\x01 \x01(\tH\x00\x12\x16\n\x05\x63hart\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x1e\n\rchart_version\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x42\x11\n\nrepo_oneof\x12\x03\xf8\x42\x01\"\x94\x02\n\x13HelmValuesOverrides\x12\x1a\n\x07inlined\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01H\x00\x12\x34\n\x05local\x18\x02 \x01(\x0b\x32#.prodvana.common_config.LocalConfigH\x00\x12K\n\x03map\x18\x03 \x03(\x0b\x32\x34.prodvana.common_config.HelmValuesOverrides.MapEntryB\x08\xfa\x42\x05\x9a\x01\x02\x18\x01\x1aL\n\x08MapEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42\x10\n\x0eoverride_oneof\"\xd4\x01\n\nHelmConfig\x12\x39\n\x06remote\x18\x01 \x01(\x0b\x32\'.prodvana.common_config.RemoteHelmChartH\x00\x12\x45\n\x10values_overrides\x18\x02 \x03(\x0b\x32+.prodvana.common_config.HelmValuesOverrides\x12\x14\n\x0crelease_name\x18\x03 \x01(\t\x12\x1a\n\tnamespace\x18\x04 \x01(\tB\x07\xfa\x42\x04r\x02\x18\x00\x42\x12\n\x0b\x63hart_oneof\x12\x03\xf8\x42\x01\x42RZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
 
 
 
 _REMOTEHELMCHART = DESCRIPTOR.message_types_by_name['RemoteHelmChart']
 _HELMVALUESOVERRIDES = DESCRIPTOR.message_types_by_name['HelmValuesOverrides']
 _HELMVALUESOVERRIDES_MAPENTRY = _HELMVALUESOVERRIDES.nested_types_by_name['MapEntry']
 _HELMCONFIG = DESCRIPTOR.message_types_by_name['HelmConfig']
@@ -70,16 +70,16 @@
   _HELMVALUESOVERRIDES.fields_by_name['inlined']._serialized_options = b'\372B\004r\002\020\001'
   _HELMVALUESOVERRIDES.fields_by_name['map']._options = None
   _HELMVALUESOVERRIDES.fields_by_name['map']._serialized_options = b'\372B\005\232\001\002\030\001'
   _HELMCONFIG.oneofs_by_name['chart_oneof']._options = None
   _HELMCONFIG.oneofs_by_name['chart_oneof']._serialized_options = b'\370B\001'
   _HELMCONFIG.fields_by_name['namespace']._options = None
   _HELMCONFIG.fields_by_name['namespace']._serialized_options = b'\372B\004r\002\030\000'
-  _REMOTEHELMCHART._serialized_start=166
-  _REMOTEHELMCHART._serialized_end=274
-  _HELMVALUESOVERRIDES._serialized_start=277
-  _HELMVALUESOVERRIDES._serialized_end=553
-  _HELMVALUESOVERRIDES_MAPENTRY._serialized_start=459
-  _HELMVALUESOVERRIDES_MAPENTRY._serialized_end=535
-  _HELMCONFIG._serialized_start=556
-  _HELMCONFIG._serialized_end=768
+  _REMOTEHELMCHART._serialized_start=168
+  _REMOTEHELMCHART._serialized_end=276
+  _HELMVALUESOVERRIDES._serialized_start=279
+  _HELMVALUESOVERRIDES._serialized_end=555
+  _HELMVALUESOVERRIDES_MAPENTRY._serialized_start=461
+  _HELMVALUESOVERRIDES_MAPENTRY._serialized_end=537
+  _HELMCONFIG._serialized_start=558
+  _HELMCONFIG._serialized_end=770
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/helm_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/helm_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import prodvana.proto.prodvana.common_config.env_pb2
-import prodvana.proto.prodvana.common_config.external_config_pb2
+import prodvana.proto.prodvana.common_config.kubernetes_config_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
@@ -62,23 +62,23 @@
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     INLINED_FIELD_NUMBER: builtins.int
     LOCAL_FIELD_NUMBER: builtins.int
     MAP_FIELD_NUMBER: builtins.int
     inlined: builtins.str
     @property
-    def local(self) -> prodvana.proto.prodvana.common_config.external_config_pb2.LocalConfig: ...
+    def local(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.LocalConfig: ...
     @property
     def map(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue]:
         """treat this as part of the above oneof, even though proto does not allow us to"""
     def __init__(
         self,
         *,
         inlined: builtins.str = ...,
-        local: prodvana.proto.prodvana.common_config.external_config_pb2.LocalConfig | None = ...,
+        local: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.LocalConfig | None = ...,
         map: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["inlined", b"inlined", "local", b"local", "override_oneof", b"override_oneof"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["inlined", b"inlined", "local", b"local", "map", b"map", "override_oneof", b"override_oneof"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["override_oneof", b"override_oneof"]) -> typing_extensions.Literal["inlined", "local"] | None: ...
 
 global___HelmValuesOverrides = HelmValuesOverrides
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/links_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/links_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/links_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/maturity_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/maturity_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/maturity_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/maturity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/meta_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/meta_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/meta_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/notification_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/notification_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/parameters_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/parameters_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,29 +9,32 @@
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.prodvana.common_config import program_pb2 as prodvana_dot_common__config_dot_program__pb2
+from prodvana.proto.prodvana.common_config import env_pb2 as prodvana_dot_common__config_dot_env__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'prodvana/common_config/parameters.proto\x12\x16prodvana.common_config\x1a$prodvana/common_config/program.proto\x1a\x17validate/validate.proto\"&\n\rProgramChange\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"2\n\x19StringParameterDefinition\x12\x15\n\rdefault_value\x18\x01 \x01(\t\"\xc3\x02\n\x1e\x44ockerImageParameterDefinition\x12\x1c\n\x0b\x64\x65\x66\x61ult_tag\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12P\n\x13image_registry_info\x18\x02 \x01(\x0b\x32).prodvana.common_config.ImageRegistryInfoB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12^\n\x07\x63hanges\x18\x03 \x03(\x0b\x32>.prodvana.common_config.DockerImageParameterDefinition.ChangesB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x1aQ\n\x07\x43hanges\x12\x38\n\x07program\x18\x01 \x01(\x0b\x32%.prodvana.common_config.ProgramChangeH\x00\x42\x0c\n\x05oneof\x12\x03\xf8\x42\x01\"\x14\n\x12\x46ixedReplicaChange\"\xe5\x01\n\x16IntParameterDefinition\x12\x15\n\rdefault_value\x18\x01 \x01(\x03\x12V\n\x07\x63hanges\x18\x02 \x03(\x0b\x32\x36.prodvana.common_config.IntParameterDefinition.ChangesB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x1a\\\n\x07\x43hanges\x12\x43\n\rfixed_replica\x18\x01 \x01(\x0b\x32*.prodvana.common_config.FixedReplicaChangeH\x00\x42\x0c\n\x05oneof\x12\x03\xf8\x42\x01\"\xaa\x02\n\x13ParameterDefinition\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x43\n\x06string\x18\x03 \x01(\x0b\x32\x31.prodvana.common_config.StringParameterDefinitionH\x00\x12N\n\x0c\x64ocker_image\x18\x04 \x01(\x0b\x32\x36.prodvana.common_config.DockerImageParameterDefinitionH\x00\x12=\n\x03int\x18\x05 \x01(\x0b\x32..prodvana.common_config.IntParameterDefinitionH\x00\x42\x13\n\x0c\x63onfig_oneof\x12\x03\xf8\x42\x01\"\x8c\x01\n\x0eParameterValue\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x10\n\x06string\x18\x02 \x01(\tH\x00\x12\r\n\x03int\x18\x04 \x01(\x03H\x00\x12\x1a\n\x10\x64ocker_image_tag\x18\x05 \x01(\tH\x00\x42\x12\n\x0bvalue_oneof\x12\x03\xf8\x42\x01J\x04\x08\x03\x10\x04R\x0c\x64ocker_image\"b\n\x10ParametersConfig\x12N\n\nparameters\x18\x01 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x42RZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'prodvana/common_config/parameters.proto\x12\x16prodvana.common_config\x1a$prodvana/common_config/program.proto\x1a prodvana/common_config/env.proto\x1a\x17validate/validate.proto\"&\n\rProgramChange\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"2\n\x19StringParameterDefinition\x12\x15\n\rdefault_value\x18\x01 \x01(\t\"\xc3\x02\n\x1e\x44ockerImageParameterDefinition\x12\x1c\n\x0b\x64\x65\x66\x61ult_tag\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12P\n\x13image_registry_info\x18\x02 \x01(\x0b\x32).prodvana.common_config.ImageRegistryInfoB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12^\n\x07\x63hanges\x18\x03 \x03(\x0b\x32>.prodvana.common_config.DockerImageParameterDefinition.ChangesB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x1aQ\n\x07\x43hanges\x12\x38\n\x07program\x18\x01 \x01(\x0b\x32%.prodvana.common_config.ProgramChangeH\x00\x42\x0c\n\x05oneof\x12\x03\xf8\x42\x01\"\x14\n\x12\x46ixedReplicaChange\"\xe5\x01\n\x16IntParameterDefinition\x12\x15\n\rdefault_value\x18\x01 \x01(\x03\x12V\n\x07\x63hanges\x18\x02 \x03(\x0b\x32\x36.prodvana.common_config.IntParameterDefinition.ChangesB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x1a\\\n\x07\x43hanges\x12\x43\n\rfixed_replica\x18\x01 \x01(\x0b\x32*.prodvana.common_config.FixedReplicaChangeH\x00\x42\x0c\n\x05oneof\x12\x03\xf8\x42\x01\"\x1b\n\x19SecretParameterDefinition\"\x81\x03\n\x13ParameterDefinition\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x43\n\x06string\x18\x03 \x01(\x0b\x32\x31.prodvana.common_config.StringParameterDefinitionH\x00\x12N\n\x0c\x64ocker_image\x18\x04 \x01(\x0b\x32\x36.prodvana.common_config.DockerImageParameterDefinitionH\x00\x12=\n\x03int\x18\x05 \x01(\x0b\x32..prodvana.common_config.IntParameterDefinitionH\x00\x12\x43\n\x06secret\x18\x06 \x01(\x0b\x32\x31.prodvana.common_config.SecretParameterDefinitionH\x00\x12\x10\n\x08required\x18\x07 \x01(\x08\x42\x13\n\x0c\x63onfig_oneof\x12\x03\xf8\x42\x01\"w\n\x14SecretParameterValue\x12\x14\n\nraw_secret\x18\x01 \x01(\tH\x00\x12\x34\n\nsecret_ref\x18\x02 \x01(\x0b\x32\x1e.prodvana.common_config.SecretH\x00\x42\x13\n\x0csecret_oneof\x12\x03\xf8\x42\x01\"\xcc\x01\n\x0eParameterValue\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x10\n\x06string\x18\x02 \x01(\tH\x00\x12\r\n\x03int\x18\x04 \x01(\x03H\x00\x12\x1a\n\x10\x64ocker_image_tag\x18\x05 \x01(\tH\x00\x12>\n\x06secret\x18\x06 \x01(\x0b\x32,.prodvana.common_config.SecretParameterValueH\x00\x42\x12\n\x0bvalue_oneof\x12\x03\xf8\x42\x01J\x04\x08\x03\x10\x04R\x0c\x64ocker_image\"b\n\x10ParametersConfig\x12N\n\nparameters\x18\x01 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x42RZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
 
 
 
 _PROGRAMCHANGE = DESCRIPTOR.message_types_by_name['ProgramChange']
 _STRINGPARAMETERDEFINITION = DESCRIPTOR.message_types_by_name['StringParameterDefinition']
 _DOCKERIMAGEPARAMETERDEFINITION = DESCRIPTOR.message_types_by_name['DockerImageParameterDefinition']
 _DOCKERIMAGEPARAMETERDEFINITION_CHANGES = _DOCKERIMAGEPARAMETERDEFINITION.nested_types_by_name['Changes']
 _FIXEDREPLICACHANGE = DESCRIPTOR.message_types_by_name['FixedReplicaChange']
 _INTPARAMETERDEFINITION = DESCRIPTOR.message_types_by_name['IntParameterDefinition']
 _INTPARAMETERDEFINITION_CHANGES = _INTPARAMETERDEFINITION.nested_types_by_name['Changes']
+_SECRETPARAMETERDEFINITION = DESCRIPTOR.message_types_by_name['SecretParameterDefinition']
 _PARAMETERDEFINITION = DESCRIPTOR.message_types_by_name['ParameterDefinition']
+_SECRETPARAMETERVALUE = DESCRIPTOR.message_types_by_name['SecretParameterValue']
 _PARAMETERVALUE = DESCRIPTOR.message_types_by_name['ParameterValue']
 _PARAMETERSCONFIG = DESCRIPTOR.message_types_by_name['ParametersConfig']
 ProgramChange = _reflection.GeneratedProtocolMessageType('ProgramChange', (_message.Message,), {
   'DESCRIPTOR' : _PROGRAMCHANGE,
   '__module__' : 'prodvana.common_config.parameters_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.common_config.ProgramChange)
   })
@@ -77,21 +80,35 @@
   'DESCRIPTOR' : _INTPARAMETERDEFINITION,
   '__module__' : 'prodvana.common_config.parameters_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.common_config.IntParameterDefinition)
   })
 _sym_db.RegisterMessage(IntParameterDefinition)
 _sym_db.RegisterMessage(IntParameterDefinition.Changes)
 
+SecretParameterDefinition = _reflection.GeneratedProtocolMessageType('SecretParameterDefinition', (_message.Message,), {
+  'DESCRIPTOR' : _SECRETPARAMETERDEFINITION,
+  '__module__' : 'prodvana.common_config.parameters_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.common_config.SecretParameterDefinition)
+  })
+_sym_db.RegisterMessage(SecretParameterDefinition)
+
 ParameterDefinition = _reflection.GeneratedProtocolMessageType('ParameterDefinition', (_message.Message,), {
   'DESCRIPTOR' : _PARAMETERDEFINITION,
   '__module__' : 'prodvana.common_config.parameters_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.common_config.ParameterDefinition)
   })
 _sym_db.RegisterMessage(ParameterDefinition)
 
+SecretParameterValue = _reflection.GeneratedProtocolMessageType('SecretParameterValue', (_message.Message,), {
+  'DESCRIPTOR' : _SECRETPARAMETERVALUE,
+  '__module__' : 'prodvana.common_config.parameters_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.common_config.SecretParameterValue)
+  })
+_sym_db.RegisterMessage(SecretParameterValue)
+
 ParameterValue = _reflection.GeneratedProtocolMessageType('ParameterValue', (_message.Message,), {
   'DESCRIPTOR' : _PARAMETERVALUE,
   '__module__' : 'prodvana.common_config.parameters_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.common_config.ParameterValue)
   })
 _sym_db.RegisterMessage(ParameterValue)
 
@@ -120,34 +137,40 @@
   _INTPARAMETERDEFINITION_CHANGES.oneofs_by_name['oneof']._serialized_options = b'\370B\001'
   _INTPARAMETERDEFINITION.fields_by_name['changes']._options = None
   _INTPARAMETERDEFINITION.fields_by_name['changes']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
   _PARAMETERDEFINITION.oneofs_by_name['config_oneof']._options = None
   _PARAMETERDEFINITION.oneofs_by_name['config_oneof']._serialized_options = b'\370B\001'
   _PARAMETERDEFINITION.fields_by_name['name']._options = None
   _PARAMETERDEFINITION.fields_by_name['name']._serialized_options = b'\372B\004r\002\020\001'
+  _SECRETPARAMETERVALUE.oneofs_by_name['secret_oneof']._options = None
+  _SECRETPARAMETERVALUE.oneofs_by_name['secret_oneof']._serialized_options = b'\370B\001'
   _PARAMETERVALUE.oneofs_by_name['value_oneof']._options = None
   _PARAMETERVALUE.oneofs_by_name['value_oneof']._serialized_options = b'\370B\001'
   _PARAMETERVALUE.fields_by_name['name']._options = None
   _PARAMETERVALUE.fields_by_name['name']._serialized_options = b'\372B\004r\002\020\001'
   _PARAMETERSCONFIG.fields_by_name['parameters']._options = None
   _PARAMETERSCONFIG.fields_by_name['parameters']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
-  _PROGRAMCHANGE._serialized_start=130
-  _PROGRAMCHANGE._serialized_end=168
-  _STRINGPARAMETERDEFINITION._serialized_start=170
-  _STRINGPARAMETERDEFINITION._serialized_end=220
-  _DOCKERIMAGEPARAMETERDEFINITION._serialized_start=223
-  _DOCKERIMAGEPARAMETERDEFINITION._serialized_end=546
-  _DOCKERIMAGEPARAMETERDEFINITION_CHANGES._serialized_start=465
-  _DOCKERIMAGEPARAMETERDEFINITION_CHANGES._serialized_end=546
-  _FIXEDREPLICACHANGE._serialized_start=548
-  _FIXEDREPLICACHANGE._serialized_end=568
-  _INTPARAMETERDEFINITION._serialized_start=571
-  _INTPARAMETERDEFINITION._serialized_end=800
-  _INTPARAMETERDEFINITION_CHANGES._serialized_start=708
-  _INTPARAMETERDEFINITION_CHANGES._serialized_end=800
-  _PARAMETERDEFINITION._serialized_start=803
-  _PARAMETERDEFINITION._serialized_end=1101
-  _PARAMETERVALUE._serialized_start=1104
-  _PARAMETERVALUE._serialized_end=1244
-  _PARAMETERSCONFIG._serialized_start=1246
-  _PARAMETERSCONFIG._serialized_end=1344
+  _PROGRAMCHANGE._serialized_start=164
+  _PROGRAMCHANGE._serialized_end=202
+  _STRINGPARAMETERDEFINITION._serialized_start=204
+  _STRINGPARAMETERDEFINITION._serialized_end=254
+  _DOCKERIMAGEPARAMETERDEFINITION._serialized_start=257
+  _DOCKERIMAGEPARAMETERDEFINITION._serialized_end=580
+  _DOCKERIMAGEPARAMETERDEFINITION_CHANGES._serialized_start=499
+  _DOCKERIMAGEPARAMETERDEFINITION_CHANGES._serialized_end=580
+  _FIXEDREPLICACHANGE._serialized_start=582
+  _FIXEDREPLICACHANGE._serialized_end=602
+  _INTPARAMETERDEFINITION._serialized_start=605
+  _INTPARAMETERDEFINITION._serialized_end=834
+  _INTPARAMETERDEFINITION_CHANGES._serialized_start=742
+  _INTPARAMETERDEFINITION_CHANGES._serialized_end=834
+  _SECRETPARAMETERDEFINITION._serialized_start=836
+  _SECRETPARAMETERDEFINITION._serialized_end=863
+  _PARAMETERDEFINITION._serialized_start=866
+  _PARAMETERDEFINITION._serialized_end=1251
+  _SECRETPARAMETERVALUE._serialized_start=1253
+  _SECRETPARAMETERVALUE._serialized_end=1372
+  _PARAMETERVALUE._serialized_start=1375
+  _PARAMETERVALUE._serialized_end=1579
+  _PARAMETERSCONFIG._serialized_start=1581
+  _PARAMETERSCONFIG._serialized_end=1679
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/parameters_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,200 +1,245 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
+import google.protobuf.duration_pb2
 import google.protobuf.internal.containers
 import google.protobuf.message
-import prodvana.proto.prodvana.common_config.program_pb2
+import google.protobuf.timestamp_pb2
+import prodvana.proto.prodvana.config_writeback.writeback_pb2
+import prodvana.proto.prodvana.insights.insights_pb2
+import prodvana.proto.prodvana.metrics.metrics_pb2
+import prodvana.proto.prodvana.organization.user_metadata_pb2
+import prodvana.proto.prodvana.users.users_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class ProgramChange(google.protobuf.message.Message):
+class OrganizationInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    NAME_FIELD_NUMBER: builtins.int
-    name: builtins.str
+    ID_FIELD_NUMBER: builtins.int
+    DISPLAY_NAME_FIELD_NUMBER: builtins.int
+    WRITEBACK_CONFIG_FIELD_NUMBER: builtins.int
+    SLUG_FIELD_NUMBER: builtins.int
+    USER_METADATA_FIELD_NUMBER: builtins.int
+    id: builtins.str
+    display_name: builtins.str
+    @property
+    def writeback_config(self) -> prodvana.proto.prodvana.config_writeback.writeback_pb2.ConfigWritebackPath: ...
+    slug: builtins.str
+    @property
+    def user_metadata(self) -> prodvana.proto.prodvana.organization.user_metadata_pb2.OrganizationUserMetadata: ...
     def __init__(
         self,
         *,
-        name: builtins.str = ...,
+        id: builtins.str = ...,
+        display_name: builtins.str = ...,
+        writeback_config: prodvana.proto.prodvana.config_writeback.writeback_pb2.ConfigWritebackPath | None = ...,
+        slug: builtins.str = ...,
+        user_metadata: prodvana.proto.prodvana.organization.user_metadata_pb2.OrganizationUserMetadata | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["user_metadata", b"user_metadata", "writeback_config", b"writeback_config"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["display_name", b"display_name", "id", b"id", "slug", b"slug", "user_metadata", b"user_metadata", "writeback_config", b"writeback_config"]) -> None: ...
 
-global___ProgramChange = ProgramChange
+global___OrganizationInfo = OrganizationInfo
 
-class StringParameterDefinition(google.protobuf.message.Message):
+class GetOrganizationReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DEFAULT_VALUE_FIELD_NUMBER: builtins.int
-    default_value: builtins.str
     def __init__(
         self,
-        *,
-        default_value: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["default_value", b"default_value"]) -> None: ...
 
-global___StringParameterDefinition = StringParameterDefinition
+global___GetOrganizationReq = GetOrganizationReq
 
-class DockerImageParameterDefinition(google.protobuf.message.Message):
+class GetOrganizationResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    class Changes(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    ORGANIZATION_FIELD_NUMBER: builtins.int
+    @property
+    def organization(self) -> global___OrganizationInfo: ...
+    def __init__(
+        self,
+        *,
+        organization: global___OrganizationInfo | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["organization", b"organization"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["organization", b"organization"]) -> None: ...
+
+global___GetOrganizationResp = GetOrganizationResp
 
-        PROGRAM_FIELD_NUMBER: builtins.int
-        @property
-        def program(self) -> global___ProgramChange: ...
-        def __init__(
-            self,
-            *,
-            program: global___ProgramChange | None = ...,
-        ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["oneof", b"oneof", "program", b"program"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["oneof", b"oneof", "program", b"program"]) -> None: ...
-        def WhichOneof(self, oneof_group: typing_extensions.Literal["oneof", b"oneof"]) -> typing_extensions.Literal["program"] | None: ...
+class GetOrganizationMetricsReq(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DEFAULT_TAG_FIELD_NUMBER: builtins.int
-    IMAGE_REGISTRY_INFO_FIELD_NUMBER: builtins.int
-    CHANGES_FIELD_NUMBER: builtins.int
-    default_tag: builtins.str
-    """empty not a valid value"""
+    START_TIMESTAMP_FIELD_NUMBER: builtins.int
+    END_TIMESTAMP_FIELD_NUMBER: builtins.int
     @property
-    def image_registry_info(self) -> prodvana.proto.prodvana.common_config.program_pb2.ImageRegistryInfo: ...
+    def start_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
     @property
-    def changes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DockerImageParameterDefinition.Changes]: ...
+    def end_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
     def __init__(
         self,
         *,
-        default_tag: builtins.str = ...,
-        image_registry_info: prodvana.proto.prodvana.common_config.program_pb2.ImageRegistryInfo | None = ...,
-        changes: collections.abc.Iterable[global___DockerImageParameterDefinition.Changes] | None = ...,
+        start_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+        end_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["image_registry_info", b"image_registry_info"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["changes", b"changes", "default_tag", b"default_tag", "image_registry_info", b"image_registry_info"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["end_timestamp", b"end_timestamp", "start_timestamp", b"start_timestamp"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["end_timestamp", b"end_timestamp", "start_timestamp", b"start_timestamp"]) -> None: ...
 
-global___DockerImageParameterDefinition = DockerImageParameterDefinition
+global___GetOrganizationMetricsReq = GetOrganizationMetricsReq
 
-class FixedReplicaChange(google.protobuf.message.Message):
+class GetOrganizationMetricsResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    DEPLOYMENT_METRICS_FIELD_NUMBER: builtins.int
+    @property
+    def deployment_metrics(self) -> prodvana.proto.prodvana.metrics.metrics_pb2.DeploymentMetrics: ...
     def __init__(
         self,
+        *,
+        deployment_metrics: prodvana.proto.prodvana.metrics.metrics_pb2.DeploymentMetrics | None = ...,
     ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["deployment_metrics", b"deployment_metrics"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["deployment_metrics", b"deployment_metrics"]) -> None: ...
 
-global___FixedReplicaChange = FixedReplicaChange
+global___GetOrganizationMetricsResp = GetOrganizationMetricsResp
 
-class IntParameterDefinition(google.protobuf.message.Message):
+class GetOrganizationInsightsReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    class Changes(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    def __init__(
+        self,
+    ) -> None: ...
+
+global___GetOrganizationInsightsReq = GetOrganizationInsightsReq
 
-        FIXED_REPLICA_FIELD_NUMBER: builtins.int
-        @property
-        def fixed_replica(self) -> global___FixedReplicaChange: ...
-        def __init__(
-            self,
-            *,
-            fixed_replica: global___FixedReplicaChange | None = ...,
-        ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["fixed_replica", b"fixed_replica", "oneof", b"oneof"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["fixed_replica", b"fixed_replica", "oneof", b"oneof"]) -> None: ...
-        def WhichOneof(self, oneof_group: typing_extensions.Literal["oneof", b"oneof"]) -> typing_extensions.Literal["fixed_replica"] | None: ...
+class GetOrganizationInsightsResp(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DEFAULT_VALUE_FIELD_NUMBER: builtins.int
-    CHANGES_FIELD_NUMBER: builtins.int
-    default_value: builtins.int
+    INSIGHTS_FIELD_NUMBER: builtins.int
     @property
-    def changes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___IntParameterDefinition.Changes]: ...
+    def insights(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.insights.insights_pb2.Insight]: ...
     def __init__(
         self,
         *,
-        default_value: builtins.int = ...,
-        changes: collections.abc.Iterable[global___IntParameterDefinition.Changes] | None = ...,
+        insights: collections.abc.Iterable[prodvana.proto.prodvana.insights.insights_pb2.Insight] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["changes", b"changes", "default_value", b"default_value"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["insights", b"insights"]) -> None: ...
 
-global___IntParameterDefinition = IntParameterDefinition
+global___GetOrganizationInsightsResp = GetOrganizationInsightsResp
 
-class ParameterDefinition(google.protobuf.message.Message):
+class SnoozeOrganizationInsightReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    NAME_FIELD_NUMBER: builtins.int
-    DESCRIPTION_FIELD_NUMBER: builtins.int
-    STRING_FIELD_NUMBER: builtins.int
-    DOCKER_IMAGE_FIELD_NUMBER: builtins.int
-    INT_FIELD_NUMBER: builtins.int
-    name: builtins.str
-    """parameter name, used in substitutions"""
-    description: builtins.str
-    """optional description for display purposes"""
+    CLASS_FIELD_NUMBER: builtins.int
+    DURATION_FIELD_NUMBER: builtins.int
     @property
-    def string(self) -> global___StringParameterDefinition: ...
+    def duration(self) -> google.protobuf.duration_pb2.Duration: ...
+    def __init__(
+        self,
+        *,
+        duration: google.protobuf.duration_pb2.Duration | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["duration", b"duration"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["class", b"class", "duration", b"duration"]) -> None: ...
+
+global___SnoozeOrganizationInsightReq = SnoozeOrganizationInsightReq
+
+class SnoozeOrganizationInsightResp(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
+
+global___SnoozeOrganizationInsightResp = SnoozeOrganizationInsightResp
+
+class GetOrganizationMetadataReq(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
+    ) -> None: ...
+
+global___GetOrganizationMetadataReq = GetOrganizationMetadataReq
+
+class GetOrganizationMetadataResp(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    METADATA_FIELD_NUMBER: builtins.int
     @property
-    def docker_image(self) -> global___DockerImageParameterDefinition: ...
+    def metadata(self) -> prodvana.proto.prodvana.organization.user_metadata_pb2.OrganizationUserMetadata:
+        """metadata with no variables substitution, no modifications from parents"""
+    def __init__(
+        self,
+        *,
+        metadata: prodvana.proto.prodvana.organization.user_metadata_pb2.OrganizationUserMetadata | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["metadata", b"metadata"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["metadata", b"metadata"]) -> None: ...
+
+global___GetOrganizationMetadataResp = GetOrganizationMetadataResp
+
+class SetOrganizationMetadataReq(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    METADATA_FIELD_NUMBER: builtins.int
     @property
-    def int(self) -> global___IntParameterDefinition: ...
+    def metadata(self) -> prodvana.proto.prodvana.organization.user_metadata_pb2.OrganizationUserMetadata: ...
     def __init__(
         self,
         *,
-        name: builtins.str = ...,
-        description: builtins.str = ...,
-        string: global___StringParameterDefinition | None = ...,
-        docker_image: global___DockerImageParameterDefinition | None = ...,
-        int: global___IntParameterDefinition | None = ...,
+        metadata: prodvana.proto.prodvana.organization.user_metadata_pb2.OrganizationUserMetadata | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["metadata", b"metadata"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["metadata", b"metadata"]) -> None: ...
+
+global___SetOrganizationMetadataReq = SetOrganizationMetadataReq
+
+class SetOrganizationMetadataResp(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["config_oneof", b"config_oneof", "docker_image", b"docker_image", "int", b"int", "string", b"string"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["config_oneof", b"config_oneof", "description", b"description", "docker_image", b"docker_image", "int", b"int", "name", b"name", "string", b"string"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["string", "docker_image", "int"] | None: ...
 
-global___ParameterDefinition = ParameterDefinition
+global___SetOrganizationMetadataResp = SetOrganizationMetadataResp
 
-class ParameterValue(google.protobuf.message.Message):
+class GetUserReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    NAME_FIELD_NUMBER: builtins.int
-    STRING_FIELD_NUMBER: builtins.int
-    INT_FIELD_NUMBER: builtins.int
-    DOCKER_IMAGE_TAG_FIELD_NUMBER: builtins.int
-    name: builtins.str
-    string: builtins.str
-    int: builtins.int
-    docker_image_tag: builtins.str
+    USER_ID_FIELD_NUMBER: builtins.int
+    user_id: builtins.str
     def __init__(
         self,
         *,
-        name: builtins.str = ...,
-        string: builtins.str = ...,
-        int: builtins.int = ...,
-        docker_image_tag: builtins.str = ...,
+        user_id: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["docker_image_tag", b"docker_image_tag", "int", b"int", "string", b"string", "value_oneof", b"value_oneof"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["docker_image_tag", b"docker_image_tag", "int", b"int", "name", b"name", "string", b"string", "value_oneof", b"value_oneof"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["value_oneof", b"value_oneof"]) -> typing_extensions.Literal["string", "int", "docker_image_tag"] | None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["user_id", b"user_id"]) -> None: ...
 
-global___ParameterValue = ParameterValue
+global___GetUserReq = GetUserReq
 
-class ParametersConfig(google.protobuf.message.Message):
+class GetUserResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PARAMETERS_FIELD_NUMBER: builtins.int
+    USER_FIELD_NUMBER: builtins.int
     @property
-    def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ParameterDefinition]: ...
+    def user(self) -> prodvana.proto.prodvana.users.users_pb2.User: ...
     def __init__(
         self,
         *,
-        parameters: collections.abc.Iterable[global___ParameterDefinition] | None = ...,
+        user: prodvana.proto.prodvana.users.users_pb2.User | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["parameters", b"parameters"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["user", b"user"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["user", b"user"]) -> None: ...
 
-global___ParametersConfig = ParametersConfig
+global___GetUserResp = GetUserResp
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/program_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/program_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/program_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/program_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/ref_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/ref_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/ref_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/ref_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/retry_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/retry_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/retry_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/retry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/task_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/task_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/task_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/common_config/version_push_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/config_writeback/writeback_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: prodvana/common_config/version_push.proto
+# source: prodvana/config_writeback/writeback.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)prodvana/common_config/version_push.proto\x12\x16prodvana.common_config\"\x9a\x01\n\x11VersionPushOption\x12<\n\x04type\x18\x01 \x01(\x0e\x32..prodvana.common_config.VersionPushOption.Type\x12\x0f\n\x07version\x18\x02 \x01(\t\"6\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0f\n\x0bPUSH_LATEST\x10\x01\x12\x10\n\x0cPUSH_VERSION\x10\x02\x42RZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)prodvana/config_writeback/writeback.proto\x12\x19prodvana.config_writeback\"A\n\x13\x43onfigWritebackPath\x12\x14\n\x0c\x64isplay_name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_path\x18\x02 \x01(\tBUZSgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/config_writebackb\x06proto3')
 
 
 
-_VERSIONPUSHOPTION = DESCRIPTOR.message_types_by_name['VersionPushOption']
-_VERSIONPUSHOPTION_TYPE = _VERSIONPUSHOPTION.enum_types_by_name['Type']
-VersionPushOption = _reflection.GeneratedProtocolMessageType('VersionPushOption', (_message.Message,), {
-  'DESCRIPTOR' : _VERSIONPUSHOPTION,
-  '__module__' : 'prodvana.common_config.version_push_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.common_config.VersionPushOption)
+_CONFIGWRITEBACKPATH = DESCRIPTOR.message_types_by_name['ConfigWritebackPath']
+ConfigWritebackPath = _reflection.GeneratedProtocolMessageType('ConfigWritebackPath', (_message.Message,), {
+  'DESCRIPTOR' : _CONFIGWRITEBACKPATH,
+  '__module__' : 'prodvana.config_writeback.writeback_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.config_writeback.ConfigWritebackPath)
   })
-_sym_db.RegisterMessage(VersionPushOption)
+_sym_db.RegisterMessage(ConfigWritebackPath)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_config'
-  _VERSIONPUSHOPTION._serialized_start=70
-  _VERSIONPUSHOPTION._serialized_end=224
-  _VERSIONPUSHOPTION_TYPE._serialized_start=170
-  _VERSIONPUSHOPTION_TYPE._serialized_end=224
+  DESCRIPTOR._serialized_options = b'ZSgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/config_writeback'
+  _CONFIGWRITEBACKPATH._serialized_start=72
+  _CONFIGWRITEBACKPATH._serialized_end=137
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/config_file/config_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/config_file/config_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.prodvana.application import application_config_pb2 as prodvana_dot_application_dot_application__config__pb2
 from prodvana.proto.prodvana.application import user_metadata_pb2 as prodvana_dot_application_dot_user__metadata__pb2
 from prodvana.proto.prodvana.environment import clusters_pb2 as prodvana_dot_environment_dot_clusters__pb2
-from prodvana.proto.prodvana.delivery_module import config_pb2 as prodvana_dot_delivery__module_dot_config__pb2
+from prodvana.proto.prodvana.delivery_extension import config_pb2 as prodvana_dot_delivery__extension_dot_config__pb2
 from prodvana.proto.prodvana.protection import protection_config_pb2 as prodvana_dot_protection_dot_protection__config__pb2
 from prodvana.proto.prodvana.service import service_config_pb2 as prodvana_dot_service_dot_service__config__pb2
 from prodvana.proto.prodvana.service import user_metadata_pb2 as prodvana_dot_service_dot_user__metadata__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!prodvana/config_file/config.proto\x12\x14prodvana.config_file\x1a-prodvana/application/application_config.proto\x1a(prodvana/application/user_metadata.proto\x1a#prodvana/environment/clusters.proto\x1a%prodvana/delivery_module/config.proto\x1a+prodvana/protection/protection_config.proto\x1a%prodvana/service/service_config.proto\x1a$prodvana/service/user_metadata.proto\x1a\x17validate/validate.proto\"\xfd\x03\n\x0eProdvanaConfig\x12>\n\x0b\x61pplication\x18\x01 \x01(\x0b\x32\'.prodvana.application.ApplicationConfigH\x00\x12\x32\n\x07service\x18\x02 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfigH\x00\x12;\n\nprotection\x18\x03 \x01(\x0b\x32%.prodvana.protection.ProtectionConfigH\x00\x12\x36\n\x07runtime\x18\x04 \x01(\x0b\x32#.prodvana.environment.ClusterConfigH\x00\x12I\n\x0f\x64\x65livery_module\x18\x07 \x01(\x0b\x32..prodvana.delivery_module.DeliveryModuleConfigH\x00\x12M\n\x14\x61pplication_metadata\x18\x05 \x01(\x0b\x32-.prodvana.application.ApplicationUserMetadataH\x01\x12\x41\n\x10service_metadata\x18\x06 \x01(\x0b\x32%.prodvana.service.ServiceUserMetadataH\x01\x42\x13\n\x0c\x63onfig_oneof\x12\x03\xf8\x42\x01\x42\x10\n\x0emetadata_oneofBPZNgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/config_fileb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!prodvana/config_file/config.proto\x12\x14prodvana.config_file\x1a-prodvana/application/application_config.proto\x1a(prodvana/application/user_metadata.proto\x1a#prodvana/environment/clusters.proto\x1a(prodvana/delivery_extension/config.proto\x1a+prodvana/protection/protection_config.proto\x1a%prodvana/service/service_config.proto\x1a$prodvana/service/user_metadata.proto\x1a\x17validate/validate.proto\"\x86\x04\n\x0eProdvanaConfig\x12>\n\x0b\x61pplication\x18\x01 \x01(\x0b\x32\'.prodvana.application.ApplicationConfigH\x00\x12\x32\n\x07service\x18\x02 \x01(\x0b\x32\x1f.prodvana.service.ServiceConfigH\x00\x12;\n\nprotection\x18\x03 \x01(\x0b\x32%.prodvana.protection.ProtectionConfigH\x00\x12\x36\n\x07runtime\x18\x04 \x01(\x0b\x32#.prodvana.environment.ClusterConfigH\x00\x12R\n\x12\x64\x65livery_extension\x18\x07 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfigH\x00\x12M\n\x14\x61pplication_metadata\x18\x05 \x01(\x0b\x32-.prodvana.application.ApplicationUserMetadataH\x01\x12\x41\n\x10service_metadata\x18\x06 \x01(\x0b\x32%.prodvana.service.ServiceUserMetadataH\x01\x42\x13\n\x0c\x63onfig_oneof\x12\x03\xf8\x42\x01\x42\x10\n\x0emetadata_oneofBPZNgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/config_fileb\x06proto3')
 
 
 
 _PRODVANACONFIG = DESCRIPTOR.message_types_by_name['ProdvanaConfig']
 ProdvanaConfig = _reflection.GeneratedProtocolMessageType('ProdvanaConfig', (_message.Message,), {
   'DESCRIPTOR' : _PRODVANACONFIG,
   '__module__' : 'prodvana.config_file.config_pb2'
@@ -36,10 +36,10 @@
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZNgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/config_file'
   _PRODVANACONFIG.oneofs_by_name['config_oneof']._options = None
   _PRODVANACONFIG.oneofs_by_name['config_oneof']._serialized_options = b'\370B\001'
-  _PRODVANACONFIG._serialized_start=372
-  _PRODVANACONFIG._serialized_end=881
+  _PRODVANACONFIG._serialized_start=375
+  _PRODVANACONFIG._serialized_end=893
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/config_file/config_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/config_file/config_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 isort:skip_file
 """
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.message
 import prodvana.proto.prodvana.application.application_config_pb2
 import prodvana.proto.prodvana.application.user_metadata_pb2
-import prodvana.proto.prodvana.delivery_module.config_pb2
+import prodvana.proto.prodvana.delivery_extension.config_pb2
 import prodvana.proto.prodvana.environment.clusters_pb2
 import prodvana.proto.prodvana.protection.protection_config_pb2
 import prodvana.proto.prodvana.service.service_config_pb2
 import prodvana.proto.prodvana.service.user_metadata_pb2
 import sys
 import typing
 
@@ -27,43 +27,43 @@
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     APPLICATION_FIELD_NUMBER: builtins.int
     SERVICE_FIELD_NUMBER: builtins.int
     PROTECTION_FIELD_NUMBER: builtins.int
     RUNTIME_FIELD_NUMBER: builtins.int
-    DELIVERY_MODULE_FIELD_NUMBER: builtins.int
+    DELIVERY_EXTENSION_FIELD_NUMBER: builtins.int
     APPLICATION_METADATA_FIELD_NUMBER: builtins.int
     SERVICE_METADATA_FIELD_NUMBER: builtins.int
     @property
     def application(self) -> prodvana.proto.prodvana.application.application_config_pb2.ApplicationConfig: ...
     @property
     def service(self) -> prodvana.proto.prodvana.service.service_config_pb2.ServiceConfig: ...
     @property
     def protection(self) -> prodvana.proto.prodvana.protection.protection_config_pb2.ProtectionConfig: ...
     @property
     def runtime(self) -> prodvana.proto.prodvana.environment.clusters_pb2.ClusterConfig: ...
     @property
-    def delivery_module(self) -> prodvana.proto.prodvana.delivery_module.config_pb2.DeliveryModuleConfig: ...
+    def delivery_extension(self) -> prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig: ...
     @property
     def application_metadata(self) -> prodvana.proto.prodvana.application.user_metadata_pb2.ApplicationUserMetadata: ...
     @property
     def service_metadata(self) -> prodvana.proto.prodvana.service.user_metadata_pb2.ServiceUserMetadata: ...
     def __init__(
         self,
         *,
         application: prodvana.proto.prodvana.application.application_config_pb2.ApplicationConfig | None = ...,
         service: prodvana.proto.prodvana.service.service_config_pb2.ServiceConfig | None = ...,
         protection: prodvana.proto.prodvana.protection.protection_config_pb2.ProtectionConfig | None = ...,
         runtime: prodvana.proto.prodvana.environment.clusters_pb2.ClusterConfig | None = ...,
-        delivery_module: prodvana.proto.prodvana.delivery_module.config_pb2.DeliveryModuleConfig | None = ...,
+        delivery_extension: prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig | None = ...,
         application_metadata: prodvana.proto.prodvana.application.user_metadata_pb2.ApplicationUserMetadata | None = ...,
         service_metadata: prodvana.proto.prodvana.service.user_metadata_pb2.ServiceUserMetadata | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["application", b"application", "application_metadata", b"application_metadata", "config_oneof", b"config_oneof", "delivery_module", b"delivery_module", "metadata_oneof", b"metadata_oneof", "protection", b"protection", "runtime", b"runtime", "service", b"service", "service_metadata", b"service_metadata"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "application_metadata", b"application_metadata", "config_oneof", b"config_oneof", "delivery_module", b"delivery_module", "metadata_oneof", b"metadata_oneof", "protection", b"protection", "runtime", b"runtime", "service", b"service", "service_metadata", b"service_metadata"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["application", b"application", "application_metadata", b"application_metadata", "config_oneof", b"config_oneof", "delivery_extension", b"delivery_extension", "metadata_oneof", b"metadata_oneof", "protection", b"protection", "runtime", b"runtime", "service", b"service", "service_metadata", b"service_metadata"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "application_metadata", b"application_metadata", "config_oneof", b"config_oneof", "delivery_extension", b"delivery_extension", "metadata_oneof", b"metadata_oneof", "protection", b"protection", "runtime", b"runtime", "service", b"service", "service_metadata", b"service_metadata"]) -> None: ...
     @typing.overload
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["application", "service", "protection", "runtime", "delivery_module"] | None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["application", "service", "protection", "runtime", "delivery_extension"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["metadata_oneof", b"metadata_oneof"]) -> typing_extensions.Literal["application_metadata", "service_metadata"] | None: ...
 
 global___ProdvanaConfig = ProdvanaConfig
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/config_writeback/writeback_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/object/meta_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: prodvana/config_writeback/writeback.proto
+# source: prodvana/object/meta.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from prodvana.proto.prodvana.version import source_metadata_pb2 as prodvana_dot_version_dot_source__metadata__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)prodvana/config_writeback/writeback.proto\x12\x19prodvana.config_writeback\"A\n\x13\x43onfigWritebackPath\x12\x14\n\x0c\x64isplay_name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_path\x18\x02 \x01(\tBUZSgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/config_writebackb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aprodvana/object/meta.proto\x12\x0fprodvana.object\x1a&prodvana/version/source_metadata.proto\"\xb4\x01\n\nObjectMeta\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x16\n\x0e\x63onfig_version\x18\x04 \x01(\t\x12(\n\x06source\x18\x05 \x01(\x0e\x32\x18.prodvana.version.Source\x12\x39\n\x0fsource_metadata\x18\x06 \x01(\x0b\x32 .prodvana.version.SourceMetadataBKZIgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/objectb\x06proto3')
 
 
 
-_CONFIGWRITEBACKPATH = DESCRIPTOR.message_types_by_name['ConfigWritebackPath']
-ConfigWritebackPath = _reflection.GeneratedProtocolMessageType('ConfigWritebackPath', (_message.Message,), {
-  'DESCRIPTOR' : _CONFIGWRITEBACKPATH,
-  '__module__' : 'prodvana.config_writeback.writeback_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.config_writeback.ConfigWritebackPath)
+_OBJECTMETA = DESCRIPTOR.message_types_by_name['ObjectMeta']
+ObjectMeta = _reflection.GeneratedProtocolMessageType('ObjectMeta', (_message.Message,), {
+  'DESCRIPTOR' : _OBJECTMETA,
+  '__module__' : 'prodvana.object.meta_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.object.ObjectMeta)
   })
-_sym_db.RegisterMessage(ConfigWritebackPath)
+_sym_db.RegisterMessage(ObjectMeta)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZSgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/config_writeback'
-  _CONFIGWRITEBACKPATH._serialized_start=72
-  _CONFIGWRITEBACKPATH._serialized_end=137
+  DESCRIPTOR._serialized_options = b'ZIgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/object'
+  _OBJECTMETA._serialized_start=88
+  _OBJECTMETA._serialized_end=268
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/delivery/delivery_config_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/delivery/delivery_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/config_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/config_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,84 +1,84 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: prodvana/delivery_module/config.proto
+# source: prodvana/delivery_extension/config.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 from prodvana.proto.prodvana.common_config import task_pb2 as prodvana_dot_common__config_dot_task__pb2
 from prodvana.proto.prodvana.common_config import env_pb2 as prodvana_dot_common__config_dot_env__pb2
-from prodvana.proto.prodvana.common_config import external_config_pb2 as prodvana_dot_common__config_dot_external__config__pb2
+from prodvana.proto.prodvana.common_config import kubernetes_config_pb2 as prodvana_dot_common__config_dot_kubernetes__config__pb2
 from prodvana.proto.prodvana.common_config import parameters_pb2 as prodvana_dot_common__config_dot_parameters__pb2
 from prodvana.proto.prodvana.runtimes import runtimes_config_pb2 as prodvana_dot_runtimes_dot_runtimes__config__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%prodvana/delivery_module/config.proto\x12\x18prodvana.delivery_module\x1a\x17validate/validate.proto\x1a!prodvana/common_config/task.proto\x1a prodvana/common_config/env.proto\x1a,prodvana/common_config/external_config.proto\x1a\'prodvana/common_config/parameters.proto\x1a\'prodvana/runtimes/runtimes_config.proto\"\xb3\x02\n\x14\x44\x65liveryModuleConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\x39\n\x0btask_config\x18\x02 \x01(\x0b\x32\".prodvana.common_config.TaskConfigH\x00\x12\x41\n\x0f\x65xternal_config\x18\x03 \x01(\x0b\x32&.prodvana.common_config.ExternalConfigH\x00\x12N\n\nparameters\x18\x04 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x42\x12\n\x0b\x65xec_config\x12\x03\xf8\x42\x01\"\x95\x01\n\x1c\x44\x65liveryModuleInstanceConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12:\n\nparameters\x18\x03 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\"\xbf\x03\n$CompiledDeliveryModuleInstanceConfig\x12\x42\n\ndefinition\x18\x01 \x01(\x0b\x32..prodvana.delivery_module.DeliveryModuleConfig\x12\x44\n\x11runtime_execution\x18\x02 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12}\n\x03\x65nv\x18\x03 \x03(\x0b\x32G.prodvana.delivery_module.CompiledDeliveryModuleInstanceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x12@\n\x10parameter_values\x18\x04 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42TZRgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_moduleb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(prodvana/delivery_extension/config.proto\x12\x1bprodvana.delivery_extension\x1a\x17validate/validate.proto\x1a!prodvana/common_config/task.proto\x1a prodvana/common_config/env.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a\'prodvana/common_config/parameters.proto\x1a\'prodvana/runtimes/runtimes_config.proto\"\xba\x02\n\x17\x44\x65liveryExtensionConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\x39\n\x0btask_config\x18\x02 \x01(\x0b\x32\".prodvana.common_config.TaskConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x03 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12N\n\nparameters\x18\x04 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x42\x12\n\x0b\x65xec_config\x12\x03\xf8\x42\x01\"\x98\x01\n\x1f\x44\x65liveryExtensionInstanceConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12:\n\nparameters\x18\x03 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\"\xcf\x03\n\'CompiledDeliveryExtensionInstanceConfig\x12H\n\ndefinition\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfig\x12\x44\n\x11runtime_execution\x18\x02 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12\x83\x01\n\x03\x65nv\x18\x03 \x03(\x0b\x32M.prodvana.delivery_extension.CompiledDeliveryExtensionInstanceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x12@\n\x10parameter_values\x18\x04 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42WZUgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_extensionb\x06proto3')
 
 
 
-_DELIVERYMODULECONFIG = DESCRIPTOR.message_types_by_name['DeliveryModuleConfig']
-_DELIVERYMODULEINSTANCECONFIG = DESCRIPTOR.message_types_by_name['DeliveryModuleInstanceConfig']
-_COMPILEDDELIVERYMODULEINSTANCECONFIG = DESCRIPTOR.message_types_by_name['CompiledDeliveryModuleInstanceConfig']
-_COMPILEDDELIVERYMODULEINSTANCECONFIG_ENVENTRY = _COMPILEDDELIVERYMODULEINSTANCECONFIG.nested_types_by_name['EnvEntry']
-DeliveryModuleConfig = _reflection.GeneratedProtocolMessageType('DeliveryModuleConfig', (_message.Message,), {
-  'DESCRIPTOR' : _DELIVERYMODULECONFIG,
-  '__module__' : 'prodvana.delivery_module.config_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_module.DeliveryModuleConfig)
+_DELIVERYEXTENSIONCONFIG = DESCRIPTOR.message_types_by_name['DeliveryExtensionConfig']
+_DELIVERYEXTENSIONINSTANCECONFIG = DESCRIPTOR.message_types_by_name['DeliveryExtensionInstanceConfig']
+_COMPILEDDELIVERYEXTENSIONINSTANCECONFIG = DESCRIPTOR.message_types_by_name['CompiledDeliveryExtensionInstanceConfig']
+_COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY = _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG.nested_types_by_name['EnvEntry']
+DeliveryExtensionConfig = _reflection.GeneratedProtocolMessageType('DeliveryExtensionConfig', (_message.Message,), {
+  'DESCRIPTOR' : _DELIVERYEXTENSIONCONFIG,
+  '__module__' : 'prodvana.delivery_extension.config_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.DeliveryExtensionConfig)
   })
-_sym_db.RegisterMessage(DeliveryModuleConfig)
+_sym_db.RegisterMessage(DeliveryExtensionConfig)
 
-DeliveryModuleInstanceConfig = _reflection.GeneratedProtocolMessageType('DeliveryModuleInstanceConfig', (_message.Message,), {
-  'DESCRIPTOR' : _DELIVERYMODULEINSTANCECONFIG,
-  '__module__' : 'prodvana.delivery_module.config_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_module.DeliveryModuleInstanceConfig)
+DeliveryExtensionInstanceConfig = _reflection.GeneratedProtocolMessageType('DeliveryExtensionInstanceConfig', (_message.Message,), {
+  'DESCRIPTOR' : _DELIVERYEXTENSIONINSTANCECONFIG,
+  '__module__' : 'prodvana.delivery_extension.config_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.DeliveryExtensionInstanceConfig)
   })
-_sym_db.RegisterMessage(DeliveryModuleInstanceConfig)
+_sym_db.RegisterMessage(DeliveryExtensionInstanceConfig)
 
-CompiledDeliveryModuleInstanceConfig = _reflection.GeneratedProtocolMessageType('CompiledDeliveryModuleInstanceConfig', (_message.Message,), {
+CompiledDeliveryExtensionInstanceConfig = _reflection.GeneratedProtocolMessageType('CompiledDeliveryExtensionInstanceConfig', (_message.Message,), {
 
   'EnvEntry' : _reflection.GeneratedProtocolMessageType('EnvEntry', (_message.Message,), {
-    'DESCRIPTOR' : _COMPILEDDELIVERYMODULEINSTANCECONFIG_ENVENTRY,
-    '__module__' : 'prodvana.delivery_module.config_pb2'
-    # @@protoc_insertion_point(class_scope:prodvana.delivery_module.CompiledDeliveryModuleInstanceConfig.EnvEntry)
+    'DESCRIPTOR' : _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY,
+    '__module__' : 'prodvana.delivery_extension.config_pb2'
+    # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.CompiledDeliveryExtensionInstanceConfig.EnvEntry)
     })
   ,
-  'DESCRIPTOR' : _COMPILEDDELIVERYMODULEINSTANCECONFIG,
-  '__module__' : 'prodvana.delivery_module.config_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_module.CompiledDeliveryModuleInstanceConfig)
+  'DESCRIPTOR' : _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG,
+  '__module__' : 'prodvana.delivery_extension.config_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.CompiledDeliveryExtensionInstanceConfig)
   })
-_sym_db.RegisterMessage(CompiledDeliveryModuleInstanceConfig)
-_sym_db.RegisterMessage(CompiledDeliveryModuleInstanceConfig.EnvEntry)
+_sym_db.RegisterMessage(CompiledDeliveryExtensionInstanceConfig)
+_sym_db.RegisterMessage(CompiledDeliveryExtensionInstanceConfig.EnvEntry)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZRgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_module'
-  _DELIVERYMODULECONFIG.oneofs_by_name['exec_config']._options = None
-  _DELIVERYMODULECONFIG.oneofs_by_name['exec_config']._serialized_options = b'\370B\001'
-  _DELIVERYMODULECONFIG.fields_by_name['name']._options = None
-  _DELIVERYMODULECONFIG.fields_by_name['name']._serialized_options = b'\372B(r&\020\001\030?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$'
-  _DELIVERYMODULECONFIG.fields_by_name['parameters']._options = None
-  _DELIVERYMODULECONFIG.fields_by_name['parameters']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
-  _DELIVERYMODULEINSTANCECONFIG.fields_by_name['name']._options = None
-  _DELIVERYMODULEINSTANCECONFIG.fields_by_name['name']._serialized_options = b'\372B(r&\020\001\030?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$'
-  _COMPILEDDELIVERYMODULEINSTANCECONFIG_ENVENTRY._options = None
-  _COMPILEDDELIVERYMODULEINSTANCECONFIG_ENVENTRY._serialized_options = b'8\001'
-  _COMPILEDDELIVERYMODULEINSTANCECONFIG.fields_by_name['env']._options = None
-  _COMPILEDDELIVERYMODULEINSTANCECONFIG.fields_by_name['env']._serialized_options = b'\372B$\232\001!\030\001\"\035r\0332\031^[a-zA-Z_]+[a-zA-Z0-9_]*$'
-  _DELIVERYMODULECONFIG._serialized_start=290
-  _DELIVERYMODULECONFIG._serialized_end=597
-  _DELIVERYMODULEINSTANCECONFIG._serialized_start=600
-  _DELIVERYMODULEINSTANCECONFIG._serialized_end=749
-  _COMPILEDDELIVERYMODULEINSTANCECONFIG._serialized_start=752
-  _COMPILEDDELIVERYMODULEINSTANCECONFIG._serialized_end=1199
-  _COMPILEDDELIVERYMODULEINSTANCECONFIG_ENVENTRY._serialized_start=1123
-  _COMPILEDDELIVERYMODULEINSTANCECONFIG_ENVENTRY._serialized_end=1199
+  DESCRIPTOR._serialized_options = b'ZUgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_extension'
+  _DELIVERYEXTENSIONCONFIG.oneofs_by_name['exec_config']._options = None
+  _DELIVERYEXTENSIONCONFIG.oneofs_by_name['exec_config']._serialized_options = b'\370B\001'
+  _DELIVERYEXTENSIONCONFIG.fields_by_name['name']._options = None
+  _DELIVERYEXTENSIONCONFIG.fields_by_name['name']._serialized_options = b'\372B(r&\020\001\030?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$'
+  _DELIVERYEXTENSIONCONFIG.fields_by_name['parameters']._options = None
+  _DELIVERYEXTENSIONCONFIG.fields_by_name['parameters']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
+  _DELIVERYEXTENSIONINSTANCECONFIG.fields_by_name['name']._options = None
+  _DELIVERYEXTENSIONINSTANCECONFIG.fields_by_name['name']._serialized_options = b'\372B(r&\020\001\030?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$'
+  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY._options = None
+  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY._serialized_options = b'8\001'
+  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG.fields_by_name['env']._options = None
+  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG.fields_by_name['env']._serialized_options = b'\372B$\232\001!\030\001\"\035r\0332\031^[a-zA-Z_]+[a-zA-Z0-9_]*$'
+  _DELIVERYEXTENSIONCONFIG._serialized_start=298
+  _DELIVERYEXTENSIONCONFIG._serialized_end=612
+  _DELIVERYEXTENSIONINSTANCECONFIG._serialized_start=615
+  _DELIVERYEXTENSIONINSTANCECONFIG._serialized_end=767
+  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG._serialized_start=770
+  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG._serialized_end=1233
+  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY._serialized_start=1157
+  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY._serialized_end=1233
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/config_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -4,56 +4,56 @@
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import prodvana.proto.prodvana.common_config.env_pb2
-import prodvana.proto.prodvana.common_config.external_config_pb2
+import prodvana.proto.prodvana.common_config.kubernetes_config_pb2
 import prodvana.proto.prodvana.common_config.parameters_pb2
 import prodvana.proto.prodvana.common_config.task_pb2
 import prodvana.proto.prodvana.runtimes.runtimes_config_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class DeliveryModuleConfig(google.protobuf.message.Message):
+class DeliveryExtensionConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     TASK_CONFIG_FIELD_NUMBER: builtins.int
-    EXTERNAL_CONFIG_FIELD_NUMBER: builtins.int
+    KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
     name: builtins.str
     @property
     def task_config(self) -> prodvana.proto.prodvana.common_config.task_pb2.TaskConfig: ...
     @property
-    def external_config(self) -> prodvana.proto.prodvana.common_config.external_config_pb2.ExternalConfig: ...
+    def kubernetes_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig: ...
     @property
     def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition]: ...
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         task_config: prodvana.proto.prodvana.common_config.task_pb2.TaskConfig | None = ...,
-        external_config: prodvana.proto.prodvana.common_config.external_config_pb2.ExternalConfig | None = ...,
+        kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         parameters: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "external_config", b"external_config", "task_config", b"task_config"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "external_config", b"external_config", "name", b"name", "parameters", b"parameters", "task_config", b"task_config"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["exec_config", b"exec_config"]) -> typing_extensions.Literal["task_config", "external_config"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "kubernetes_config", b"kubernetes_config", "task_config", b"task_config"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "kubernetes_config", b"kubernetes_config", "name", b"name", "parameters", b"parameters", "task_config", b"task_config"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["exec_config", b"exec_config"]) -> typing_extensions.Literal["task_config", "kubernetes_config"] | None: ...
 
-global___DeliveryModuleConfig = DeliveryModuleConfig
+global___DeliveryExtensionConfig = DeliveryExtensionConfig
 
-class DeliveryModuleInstanceConfig(google.protobuf.message.Message):
+class DeliveryExtensionInstanceConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
     name: builtins.str
     @property
     def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue]: ...
@@ -61,17 +61,17 @@
         self,
         *,
         name: builtins.str = ...,
         parameters: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "parameters", b"parameters"]) -> None: ...
 
-global___DeliveryModuleInstanceConfig = DeliveryModuleInstanceConfig
+global___DeliveryExtensionInstanceConfig = DeliveryExtensionInstanceConfig
 
-class CompiledDeliveryModuleInstanceConfig(google.protobuf.message.Message):
+class CompiledDeliveryExtensionInstanceConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class EnvEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
@@ -88,31 +88,31 @@
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     DEFINITION_FIELD_NUMBER: builtins.int
     RUNTIME_EXECUTION_FIELD_NUMBER: builtins.int
     ENV_FIELD_NUMBER: builtins.int
     PARAMETER_VALUES_FIELD_NUMBER: builtins.int
     @property
-    def definition(self) -> global___DeliveryModuleConfig: ...
+    def definition(self) -> global___DeliveryExtensionConfig: ...
     @property
     def runtime_execution(self) -> prodvana.proto.prodvana.runtimes.runtimes_config_pb2.RuntimeExecutionConfig: ...
     @property
     def env(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue]:
         """The compiled environment for this attachment's context, e.g.  Release Channel."""
     @property
     def parameter_values(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue]:
         """TODO(naphat) custom task lifecycle
 
         compiled parameter values
         """
     def __init__(
         self,
         *,
-        definition: global___DeliveryModuleConfig | None = ...,
+        definition: global___DeliveryExtensionConfig | None = ...,
         runtime_execution: prodvana.proto.prodvana.runtimes.runtimes_config_pb2.RuntimeExecutionConfig | None = ...,
         env: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue] | None = ...,
         parameter_values: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["definition", b"definition", "runtime_execution", b"runtime_execution"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["definition", b"definition", "env", b"env", "parameter_values", b"parameter_values", "runtime_execution", b"runtime_execution"]) -> None: ...
 
-global___CompiledDeliveryModuleInstanceConfig = CompiledDeliveryModuleInstanceConfig
+global___CompiledDeliveryExtensionInstanceConfig = CompiledDeliveryExtensionInstanceConfig
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/manager_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/manager_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,139 +1,139 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: prodvana/delivery_module/manager.proto
+# source: prodvana/delivery_extension/manager.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
-from prodvana.proto.prodvana.delivery_module import object_pb2 as prodvana_dot_delivery__module_dot_object__pb2
-from prodvana.proto.prodvana.delivery_module import config_pb2 as prodvana_dot_delivery__module_dot_config__pb2
+from prodvana.proto.prodvana.delivery_extension import object_pb2 as prodvana_dot_delivery__extension_dot_object__pb2
+from prodvana.proto.prodvana.delivery_extension import config_pb2 as prodvana_dot_delivery__extension_dot_config__pb2
 from prodvana.proto.prodvana.version import source_metadata_pb2 as prodvana_dot_version_dot_source__metadata__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&prodvana/delivery_module/manager.proto\x12\x18prodvana.delivery_module\x1a\x1cgoogle/api/annotations.proto\x1a%prodvana/delivery_module/object.proto\x1a%prodvana/delivery_module/config.proto\x1a&prodvana/version/source_metadata.proto\x1a\x17validate/validate.proto\"\xdb\x01\n\x1a\x43onfigureDeliveryModuleReq\x12X\n\x16\x64\x65livery_module_config\x18\x01 \x01(\x0b\x32..prodvana.delivery_module.DeliveryModuleConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12(\n\x06source\x18\x02 \x01(\x0e\x32\x18.prodvana.version.Source\x12\x39\n\x0fsource_metadata\x18\x03 \x01(\x0b\x32 .prodvana.version.SourceMetadata\"J\n\x1b\x43onfigureDeliveryModuleResp\x12\x1a\n\x12\x64\x65livery_module_id\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"%\n#ValidateConfigureDeliveryModuleResp\"?\n\x16ListDeliveryModulesReq\x12\x12\n\npage_token\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\"v\n\x17ListDeliveryModulesResp\x12\x42\n\x10\x64\x65livery_modules\x18\x01 \x03(\x0b\x32(.prodvana.delivery_module.DeliveryModule\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"8\n\x14GetDeliveryModuleReq\x12 \n\x0f\x64\x65livery_module\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"Z\n\x15GetDeliveryModuleResp\x12\x41\n\x0f\x64\x65livery_module\x18\x01 \x01(\x0b\x32(.prodvana.delivery_module.DeliveryModule\"O\n\x1aGetDeliveryModuleConfigReq\x12 \n\x0f\x64\x65livery_module\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x0f\n\x07version\x18\x02 \x01(\t\"n\n\x1bGetDeliveryModuleConfigResp\x12>\n\x06\x63onfig\x18\x01 \x01(\x0b\x32..prodvana.delivery_module.DeliveryModuleConfig\x12\x0f\n\x07version\x18\x02 \x01(\t2\x9c\x07\n\x15\x44\x65liveryModuleManager\x12\xb1\x01\n\x17\x43onfigureDeliveryModule\x12\x34.prodvana.delivery_module.ConfigureDeliveryModuleReq\x1a\x35.prodvana.delivery_module.ConfigureDeliveryModuleResp\")\x82\xd3\xe4\x93\x02#\"\x1e/v1/delivery_modules/configure:\x01*\x12\xca\x01\n\x1fValidateConfigureDeliveryModule\x12\x34.prodvana.delivery_module.ConfigureDeliveryModuleReq\x1a=.prodvana.delivery_module.ValidateConfigureDeliveryModuleResp\"2\x82\xd3\xe4\x93\x02,\"\'/v1/delivery_modules/configure/validate:\x01*\x12\x98\x01\n\x13ListDeliveryModules\x12\x30.prodvana.delivery_module.ListDeliveryModulesReq\x1a\x31.prodvana.delivery_module.ListDeliveryModulesResp\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/v1/delivery_modules\x12\xa5\x01\n\x11GetDeliveryModule\x12..prodvana.delivery_module.GetDeliveryModuleReq\x1a/.prodvana.delivery_module.GetDeliveryModuleResp\"/\x82\xd3\xe4\x93\x02)\x12\'/v1/delivery_module/{delivery_module=*}\x12\xbe\x01\n\x17GetDeliveryModuleConfig\x12\x34.prodvana.delivery_module.GetDeliveryModuleConfigReq\x1a\x35.prodvana.delivery_module.GetDeliveryModuleConfigResp\"6\x82\xd3\xe4\x93\x02\x30\x12./v1/delivery_module/{delivery_module=*}/configBTZRgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_moduleb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)prodvana/delivery_extension/manager.proto\x12\x1bprodvana.delivery_extension\x1a\x1cgoogle/api/annotations.proto\x1a(prodvana/delivery_extension/object.proto\x1a(prodvana/delivery_extension/config.proto\x1a&prodvana/version/source_metadata.proto\x1a\x17validate/validate.proto\"\xe7\x01\n\x1d\x43onfigureDeliveryExtensionReq\x12\x61\n\x19\x64\x65livery_extension_config\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12(\n\x06source\x18\x02 \x01(\x0e\x32\x18.prodvana.version.Source\x12\x39\n\x0fsource_metadata\x18\x03 \x01(\x0b\x32 .prodvana.version.SourceMetadata\"P\n\x1e\x43onfigureDeliveryExtensionResp\x12\x1d\n\x15\x64\x65livery_extension_id\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"(\n&ValidateConfigureDeliveryExtensionResp\"B\n\x19ListDeliveryExtensionsReq\x12\x12\n\npage_token\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\"\x82\x01\n\x1aListDeliveryExtensionsResp\x12K\n\x13\x64\x65livery_extensions\x18\x01 \x03(\x0b\x32..prodvana.delivery_extension.DeliveryExtension\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\">\n\x17GetDeliveryExtensionReq\x12#\n\x12\x64\x65livery_extension\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"f\n\x18GetDeliveryExtensionResp\x12J\n\x12\x64\x65livery_extension\x18\x01 \x01(\x0b\x32..prodvana.delivery_extension.DeliveryExtension\"U\n\x1dGetDeliveryExtensionConfigReq\x12#\n\x12\x64\x65livery_extension\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x0f\n\x07version\x18\x02 \x01(\t\"w\n\x1eGetDeliveryExtensionConfigResp\x12\x44\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfig\x12\x0f\n\x07version\x18\x02 \x01(\t2\xff\x07\n\x18\x44\x65liveryExtensionManager\x12\xc3\x01\n\x1a\x43onfigureDeliveryExtension\x12:.prodvana.delivery_extension.ConfigureDeliveryExtensionReq\x1a;.prodvana.delivery_extension.ConfigureDeliveryExtensionResp\",\x82\xd3\xe4\x93\x02&\"!/v1/delivery_extensions/configure:\x01*\x12\xdc\x01\n\"ValidateConfigureDeliveryExtension\x12:.prodvana.delivery_extension.ConfigureDeliveryExtensionReq\x1a\x43.prodvana.delivery_extension.ValidateConfigureDeliveryExtensionResp\"5\x82\xd3\xe4\x93\x02/\"*/v1/delivery_extensions/configure/validate:\x01*\x12\xaa\x01\n\x16ListDeliveryExtensions\x12\x36.prodvana.delivery_extension.ListDeliveryExtensionsReq\x1a\x37.prodvana.delivery_extension.ListDeliveryExtensionsResp\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/v1/delivery_extensions\x12\xba\x01\n\x14GetDeliveryExtension\x12\x34.prodvana.delivery_extension.GetDeliveryExtensionReq\x1a\x35.prodvana.delivery_extension.GetDeliveryExtensionResp\"5\x82\xd3\xe4\x93\x02/\x12-/v1/delivery_extension/{delivery_extension=*}\x12\xd3\x01\n\x1aGetDeliveryExtensionConfig\x12:.prodvana.delivery_extension.GetDeliveryExtensionConfigReq\x1a;.prodvana.delivery_extension.GetDeliveryExtensionConfigResp\"<\x82\xd3\xe4\x93\x02\x36\x12\x34/v1/delivery_extension/{delivery_extension=*}/configBWZUgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_extensionb\x06proto3')
 
 
 
-_CONFIGUREDELIVERYMODULEREQ = DESCRIPTOR.message_types_by_name['ConfigureDeliveryModuleReq']
-_CONFIGUREDELIVERYMODULERESP = DESCRIPTOR.message_types_by_name['ConfigureDeliveryModuleResp']
-_VALIDATECONFIGUREDELIVERYMODULERESP = DESCRIPTOR.message_types_by_name['ValidateConfigureDeliveryModuleResp']
-_LISTDELIVERYMODULESREQ = DESCRIPTOR.message_types_by_name['ListDeliveryModulesReq']
-_LISTDELIVERYMODULESRESP = DESCRIPTOR.message_types_by_name['ListDeliveryModulesResp']
-_GETDELIVERYMODULEREQ = DESCRIPTOR.message_types_by_name['GetDeliveryModuleReq']
-_GETDELIVERYMODULERESP = DESCRIPTOR.message_types_by_name['GetDeliveryModuleResp']
-_GETDELIVERYMODULECONFIGREQ = DESCRIPTOR.message_types_by_name['GetDeliveryModuleConfigReq']
-_GETDELIVERYMODULECONFIGRESP = DESCRIPTOR.message_types_by_name['GetDeliveryModuleConfigResp']
-ConfigureDeliveryModuleReq = _reflection.GeneratedProtocolMessageType('ConfigureDeliveryModuleReq', (_message.Message,), {
-  'DESCRIPTOR' : _CONFIGUREDELIVERYMODULEREQ,
-  '__module__' : 'prodvana.delivery_module.manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_module.ConfigureDeliveryModuleReq)
+_CONFIGUREDELIVERYEXTENSIONREQ = DESCRIPTOR.message_types_by_name['ConfigureDeliveryExtensionReq']
+_CONFIGUREDELIVERYEXTENSIONRESP = DESCRIPTOR.message_types_by_name['ConfigureDeliveryExtensionResp']
+_VALIDATECONFIGUREDELIVERYEXTENSIONRESP = DESCRIPTOR.message_types_by_name['ValidateConfigureDeliveryExtensionResp']
+_LISTDELIVERYEXTENSIONSREQ = DESCRIPTOR.message_types_by_name['ListDeliveryExtensionsReq']
+_LISTDELIVERYEXTENSIONSRESP = DESCRIPTOR.message_types_by_name['ListDeliveryExtensionsResp']
+_GETDELIVERYEXTENSIONREQ = DESCRIPTOR.message_types_by_name['GetDeliveryExtensionReq']
+_GETDELIVERYEXTENSIONRESP = DESCRIPTOR.message_types_by_name['GetDeliveryExtensionResp']
+_GETDELIVERYEXTENSIONCONFIGREQ = DESCRIPTOR.message_types_by_name['GetDeliveryExtensionConfigReq']
+_GETDELIVERYEXTENSIONCONFIGRESP = DESCRIPTOR.message_types_by_name['GetDeliveryExtensionConfigResp']
+ConfigureDeliveryExtensionReq = _reflection.GeneratedProtocolMessageType('ConfigureDeliveryExtensionReq', (_message.Message,), {
+  'DESCRIPTOR' : _CONFIGUREDELIVERYEXTENSIONREQ,
+  '__module__' : 'prodvana.delivery_extension.manager_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.ConfigureDeliveryExtensionReq)
   })
-_sym_db.RegisterMessage(ConfigureDeliveryModuleReq)
+_sym_db.RegisterMessage(ConfigureDeliveryExtensionReq)
 
-ConfigureDeliveryModuleResp = _reflection.GeneratedProtocolMessageType('ConfigureDeliveryModuleResp', (_message.Message,), {
-  'DESCRIPTOR' : _CONFIGUREDELIVERYMODULERESP,
-  '__module__' : 'prodvana.delivery_module.manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_module.ConfigureDeliveryModuleResp)
+ConfigureDeliveryExtensionResp = _reflection.GeneratedProtocolMessageType('ConfigureDeliveryExtensionResp', (_message.Message,), {
+  'DESCRIPTOR' : _CONFIGUREDELIVERYEXTENSIONRESP,
+  '__module__' : 'prodvana.delivery_extension.manager_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.ConfigureDeliveryExtensionResp)
   })
-_sym_db.RegisterMessage(ConfigureDeliveryModuleResp)
+_sym_db.RegisterMessage(ConfigureDeliveryExtensionResp)
 
-ValidateConfigureDeliveryModuleResp = _reflection.GeneratedProtocolMessageType('ValidateConfigureDeliveryModuleResp', (_message.Message,), {
-  'DESCRIPTOR' : _VALIDATECONFIGUREDELIVERYMODULERESP,
-  '__module__' : 'prodvana.delivery_module.manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_module.ValidateConfigureDeliveryModuleResp)
+ValidateConfigureDeliveryExtensionResp = _reflection.GeneratedProtocolMessageType('ValidateConfigureDeliveryExtensionResp', (_message.Message,), {
+  'DESCRIPTOR' : _VALIDATECONFIGUREDELIVERYEXTENSIONRESP,
+  '__module__' : 'prodvana.delivery_extension.manager_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.ValidateConfigureDeliveryExtensionResp)
   })
-_sym_db.RegisterMessage(ValidateConfigureDeliveryModuleResp)
+_sym_db.RegisterMessage(ValidateConfigureDeliveryExtensionResp)
 
-ListDeliveryModulesReq = _reflection.GeneratedProtocolMessageType('ListDeliveryModulesReq', (_message.Message,), {
-  'DESCRIPTOR' : _LISTDELIVERYMODULESREQ,
-  '__module__' : 'prodvana.delivery_module.manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_module.ListDeliveryModulesReq)
+ListDeliveryExtensionsReq = _reflection.GeneratedProtocolMessageType('ListDeliveryExtensionsReq', (_message.Message,), {
+  'DESCRIPTOR' : _LISTDELIVERYEXTENSIONSREQ,
+  '__module__' : 'prodvana.delivery_extension.manager_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.ListDeliveryExtensionsReq)
   })
-_sym_db.RegisterMessage(ListDeliveryModulesReq)
+_sym_db.RegisterMessage(ListDeliveryExtensionsReq)
 
-ListDeliveryModulesResp = _reflection.GeneratedProtocolMessageType('ListDeliveryModulesResp', (_message.Message,), {
-  'DESCRIPTOR' : _LISTDELIVERYMODULESRESP,
-  '__module__' : 'prodvana.delivery_module.manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_module.ListDeliveryModulesResp)
+ListDeliveryExtensionsResp = _reflection.GeneratedProtocolMessageType('ListDeliveryExtensionsResp', (_message.Message,), {
+  'DESCRIPTOR' : _LISTDELIVERYEXTENSIONSRESP,
+  '__module__' : 'prodvana.delivery_extension.manager_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.ListDeliveryExtensionsResp)
   })
-_sym_db.RegisterMessage(ListDeliveryModulesResp)
+_sym_db.RegisterMessage(ListDeliveryExtensionsResp)
 
-GetDeliveryModuleReq = _reflection.GeneratedProtocolMessageType('GetDeliveryModuleReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETDELIVERYMODULEREQ,
-  '__module__' : 'prodvana.delivery_module.manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_module.GetDeliveryModuleReq)
+GetDeliveryExtensionReq = _reflection.GeneratedProtocolMessageType('GetDeliveryExtensionReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETDELIVERYEXTENSIONREQ,
+  '__module__' : 'prodvana.delivery_extension.manager_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.GetDeliveryExtensionReq)
   })
-_sym_db.RegisterMessage(GetDeliveryModuleReq)
+_sym_db.RegisterMessage(GetDeliveryExtensionReq)
 
-GetDeliveryModuleResp = _reflection.GeneratedProtocolMessageType('GetDeliveryModuleResp', (_message.Message,), {
-  'DESCRIPTOR' : _GETDELIVERYMODULERESP,
-  '__module__' : 'prodvana.delivery_module.manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_module.GetDeliveryModuleResp)
+GetDeliveryExtensionResp = _reflection.GeneratedProtocolMessageType('GetDeliveryExtensionResp', (_message.Message,), {
+  'DESCRIPTOR' : _GETDELIVERYEXTENSIONRESP,
+  '__module__' : 'prodvana.delivery_extension.manager_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.GetDeliveryExtensionResp)
   })
-_sym_db.RegisterMessage(GetDeliveryModuleResp)
+_sym_db.RegisterMessage(GetDeliveryExtensionResp)
 
-GetDeliveryModuleConfigReq = _reflection.GeneratedProtocolMessageType('GetDeliveryModuleConfigReq', (_message.Message,), {
-  'DESCRIPTOR' : _GETDELIVERYMODULECONFIGREQ,
-  '__module__' : 'prodvana.delivery_module.manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_module.GetDeliveryModuleConfigReq)
+GetDeliveryExtensionConfigReq = _reflection.GeneratedProtocolMessageType('GetDeliveryExtensionConfigReq', (_message.Message,), {
+  'DESCRIPTOR' : _GETDELIVERYEXTENSIONCONFIGREQ,
+  '__module__' : 'prodvana.delivery_extension.manager_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.GetDeliveryExtensionConfigReq)
   })
-_sym_db.RegisterMessage(GetDeliveryModuleConfigReq)
+_sym_db.RegisterMessage(GetDeliveryExtensionConfigReq)
 
-GetDeliveryModuleConfigResp = _reflection.GeneratedProtocolMessageType('GetDeliveryModuleConfigResp', (_message.Message,), {
-  'DESCRIPTOR' : _GETDELIVERYMODULECONFIGRESP,
-  '__module__' : 'prodvana.delivery_module.manager_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_module.GetDeliveryModuleConfigResp)
+GetDeliveryExtensionConfigResp = _reflection.GeneratedProtocolMessageType('GetDeliveryExtensionConfigResp', (_message.Message,), {
+  'DESCRIPTOR' : _GETDELIVERYEXTENSIONCONFIGRESP,
+  '__module__' : 'prodvana.delivery_extension.manager_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.GetDeliveryExtensionConfigResp)
   })
-_sym_db.RegisterMessage(GetDeliveryModuleConfigResp)
+_sym_db.RegisterMessage(GetDeliveryExtensionConfigResp)
 
-_DELIVERYMODULEMANAGER = DESCRIPTOR.services_by_name['DeliveryModuleManager']
+_DELIVERYEXTENSIONMANAGER = DESCRIPTOR.services_by_name['DeliveryExtensionManager']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZRgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_module'
-  _CONFIGUREDELIVERYMODULEREQ.fields_by_name['delivery_module_config']._options = None
-  _CONFIGUREDELIVERYMODULEREQ.fields_by_name['delivery_module_config']._serialized_options = b'\372B\005\212\001\002\020\001'
-  _GETDELIVERYMODULEREQ.fields_by_name['delivery_module']._options = None
-  _GETDELIVERYMODULEREQ.fields_by_name['delivery_module']._serialized_options = b'\372B\004r\002\020\001'
-  _GETDELIVERYMODULECONFIGREQ.fields_by_name['delivery_module']._options = None
-  _GETDELIVERYMODULECONFIGREQ.fields_by_name['delivery_module']._serialized_options = b'\372B\004r\002\020\001'
-  _DELIVERYMODULEMANAGER.methods_by_name['ConfigureDeliveryModule']._options = None
-  _DELIVERYMODULEMANAGER.methods_by_name['ConfigureDeliveryModule']._serialized_options = b'\202\323\344\223\002#\"\036/v1/delivery_modules/configure:\001*'
-  _DELIVERYMODULEMANAGER.methods_by_name['ValidateConfigureDeliveryModule']._options = None
-  _DELIVERYMODULEMANAGER.methods_by_name['ValidateConfigureDeliveryModule']._serialized_options = b'\202\323\344\223\002,\"\'/v1/delivery_modules/configure/validate:\001*'
-  _DELIVERYMODULEMANAGER.methods_by_name['ListDeliveryModules']._options = None
-  _DELIVERYMODULEMANAGER.methods_by_name['ListDeliveryModules']._serialized_options = b'\202\323\344\223\002\026\022\024/v1/delivery_modules'
-  _DELIVERYMODULEMANAGER.methods_by_name['GetDeliveryModule']._options = None
-  _DELIVERYMODULEMANAGER.methods_by_name['GetDeliveryModule']._serialized_options = b'\202\323\344\223\002)\022\'/v1/delivery_module/{delivery_module=*}'
-  _DELIVERYMODULEMANAGER.methods_by_name['GetDeliveryModuleConfig']._options = None
-  _DELIVERYMODULEMANAGER.methods_by_name['GetDeliveryModuleConfig']._serialized_options = b'\202\323\344\223\0020\022./v1/delivery_module/{delivery_module=*}/config'
-  _CONFIGUREDELIVERYMODULEREQ._serialized_start=242
-  _CONFIGUREDELIVERYMODULEREQ._serialized_end=461
-  _CONFIGUREDELIVERYMODULERESP._serialized_start=463
-  _CONFIGUREDELIVERYMODULERESP._serialized_end=537
-  _VALIDATECONFIGUREDELIVERYMODULERESP._serialized_start=539
-  _VALIDATECONFIGUREDELIVERYMODULERESP._serialized_end=576
-  _LISTDELIVERYMODULESREQ._serialized_start=578
-  _LISTDELIVERYMODULESREQ._serialized_end=641
-  _LISTDELIVERYMODULESRESP._serialized_start=643
-  _LISTDELIVERYMODULESRESP._serialized_end=761
-  _GETDELIVERYMODULEREQ._serialized_start=763
-  _GETDELIVERYMODULEREQ._serialized_end=819
-  _GETDELIVERYMODULERESP._serialized_start=821
-  _GETDELIVERYMODULERESP._serialized_end=911
-  _GETDELIVERYMODULECONFIGREQ._serialized_start=913
-  _GETDELIVERYMODULECONFIGREQ._serialized_end=992
-  _GETDELIVERYMODULECONFIGRESP._serialized_start=994
-  _GETDELIVERYMODULECONFIGRESP._serialized_end=1104
-  _DELIVERYMODULEMANAGER._serialized_start=1107
-  _DELIVERYMODULEMANAGER._serialized_end=2031
+  DESCRIPTOR._serialized_options = b'ZUgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_extension'
+  _CONFIGUREDELIVERYEXTENSIONREQ.fields_by_name['delivery_extension_config']._options = None
+  _CONFIGUREDELIVERYEXTENSIONREQ.fields_by_name['delivery_extension_config']._serialized_options = b'\372B\005\212\001\002\020\001'
+  _GETDELIVERYEXTENSIONREQ.fields_by_name['delivery_extension']._options = None
+  _GETDELIVERYEXTENSIONREQ.fields_by_name['delivery_extension']._serialized_options = b'\372B\004r\002\020\001'
+  _GETDELIVERYEXTENSIONCONFIGREQ.fields_by_name['delivery_extension']._options = None
+  _GETDELIVERYEXTENSIONCONFIGREQ.fields_by_name['delivery_extension']._serialized_options = b'\372B\004r\002\020\001'
+  _DELIVERYEXTENSIONMANAGER.methods_by_name['ConfigureDeliveryExtension']._options = None
+  _DELIVERYEXTENSIONMANAGER.methods_by_name['ConfigureDeliveryExtension']._serialized_options = b'\202\323\344\223\002&\"!/v1/delivery_extensions/configure:\001*'
+  _DELIVERYEXTENSIONMANAGER.methods_by_name['ValidateConfigureDeliveryExtension']._options = None
+  _DELIVERYEXTENSIONMANAGER.methods_by_name['ValidateConfigureDeliveryExtension']._serialized_options = b'\202\323\344\223\002/\"*/v1/delivery_extensions/configure/validate:\001*'
+  _DELIVERYEXTENSIONMANAGER.methods_by_name['ListDeliveryExtensions']._options = None
+  _DELIVERYEXTENSIONMANAGER.methods_by_name['ListDeliveryExtensions']._serialized_options = b'\202\323\344\223\002\031\022\027/v1/delivery_extensions'
+  _DELIVERYEXTENSIONMANAGER.methods_by_name['GetDeliveryExtension']._options = None
+  _DELIVERYEXTENSIONMANAGER.methods_by_name['GetDeliveryExtension']._serialized_options = b'\202\323\344\223\002/\022-/v1/delivery_extension/{delivery_extension=*}'
+  _DELIVERYEXTENSIONMANAGER.methods_by_name['GetDeliveryExtensionConfig']._options = None
+  _DELIVERYEXTENSIONMANAGER.methods_by_name['GetDeliveryExtensionConfig']._serialized_options = b'\202\323\344\223\0026\0224/v1/delivery_extension/{delivery_extension=*}/config'
+  _CONFIGUREDELIVERYEXTENSIONREQ._serialized_start=254
+  _CONFIGUREDELIVERYEXTENSIONREQ._serialized_end=485
+  _CONFIGUREDELIVERYEXTENSIONRESP._serialized_start=487
+  _CONFIGUREDELIVERYEXTENSIONRESP._serialized_end=567
+  _VALIDATECONFIGUREDELIVERYEXTENSIONRESP._serialized_start=569
+  _VALIDATECONFIGUREDELIVERYEXTENSIONRESP._serialized_end=609
+  _LISTDELIVERYEXTENSIONSREQ._serialized_start=611
+  _LISTDELIVERYEXTENSIONSREQ._serialized_end=677
+  _LISTDELIVERYEXTENSIONSRESP._serialized_start=680
+  _LISTDELIVERYEXTENSIONSRESP._serialized_end=810
+  _GETDELIVERYEXTENSIONREQ._serialized_start=812
+  _GETDELIVERYEXTENSIONREQ._serialized_end=874
+  _GETDELIVERYEXTENSIONRESP._serialized_start=876
+  _GETDELIVERYEXTENSIONRESP._serialized_end=978
+  _GETDELIVERYEXTENSIONCONFIGREQ._serialized_start=980
+  _GETDELIVERYEXTENSIONCONFIGREQ._serialized_end=1065
+  _GETDELIVERYEXTENSIONCONFIGRESP._serialized_start=1067
+  _GETDELIVERYEXTENSIONCONFIGRESP._serialized_end=1186
+  _DELIVERYEXTENSIONMANAGER._serialized_start=1189
+  _DELIVERYEXTENSIONMANAGER._serialized_end=2212
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/manager_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -3,169 +3,169 @@
 isort:skip_file
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import prodvana.proto.prodvana.delivery_module.config_pb2
-import prodvana.proto.prodvana.delivery_module.object_pb2
+import prodvana.proto.prodvana.delivery_extension.config_pb2
+import prodvana.proto.prodvana.delivery_extension.object_pb2
 import prodvana.proto.prodvana.version.source_metadata_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class ConfigureDeliveryModuleReq(google.protobuf.message.Message):
+class ConfigureDeliveryExtensionReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DELIVERY_MODULE_CONFIG_FIELD_NUMBER: builtins.int
+    DELIVERY_EXTENSION_CONFIG_FIELD_NUMBER: builtins.int
     SOURCE_FIELD_NUMBER: builtins.int
     SOURCE_METADATA_FIELD_NUMBER: builtins.int
     @property
-    def delivery_module_config(self) -> prodvana.proto.prodvana.delivery_module.config_pb2.DeliveryModuleConfig: ...
+    def delivery_extension_config(self) -> prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig: ...
     source: prodvana.proto.prodvana.version.source_metadata_pb2.Source.ValueType
     @property
     def source_metadata(self) -> prodvana.proto.prodvana.version.source_metadata_pb2.SourceMetadata: ...
     def __init__(
         self,
         *,
-        delivery_module_config: prodvana.proto.prodvana.delivery_module.config_pb2.DeliveryModuleConfig | None = ...,
+        delivery_extension_config: prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig | None = ...,
         source: prodvana.proto.prodvana.version.source_metadata_pb2.Source.ValueType = ...,
         source_metadata: prodvana.proto.prodvana.version.source_metadata_pb2.SourceMetadata | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["delivery_module_config", b"delivery_module_config", "source_metadata", b"source_metadata"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["delivery_module_config", b"delivery_module_config", "source", b"source", "source_metadata", b"source_metadata"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["delivery_extension_config", b"delivery_extension_config", "source_metadata", b"source_metadata"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["delivery_extension_config", b"delivery_extension_config", "source", b"source", "source_metadata", b"source_metadata"]) -> None: ...
 
-global___ConfigureDeliveryModuleReq = ConfigureDeliveryModuleReq
+global___ConfigureDeliveryExtensionReq = ConfigureDeliveryExtensionReq
 
-class ConfigureDeliveryModuleResp(google.protobuf.message.Message):
+class ConfigureDeliveryExtensionResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DELIVERY_MODULE_ID_FIELD_NUMBER: builtins.int
+    DELIVERY_EXTENSION_ID_FIELD_NUMBER: builtins.int
     VERSION_FIELD_NUMBER: builtins.int
-    delivery_module_id: builtins.str
+    delivery_extension_id: builtins.str
     version: builtins.str
     def __init__(
         self,
         *,
-        delivery_module_id: builtins.str = ...,
+        delivery_extension_id: builtins.str = ...,
         version: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["delivery_module_id", b"delivery_module_id", "version", b"version"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["delivery_extension_id", b"delivery_extension_id", "version", b"version"]) -> None: ...
 
-global___ConfigureDeliveryModuleResp = ConfigureDeliveryModuleResp
+global___ConfigureDeliveryExtensionResp = ConfigureDeliveryExtensionResp
 
-class ValidateConfigureDeliveryModuleResp(google.protobuf.message.Message):
+class ValidateConfigureDeliveryExtensionResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
-global___ValidateConfigureDeliveryModuleResp = ValidateConfigureDeliveryModuleResp
+global___ValidateConfigureDeliveryExtensionResp = ValidateConfigureDeliveryExtensionResp
 
-class ListDeliveryModulesReq(google.protobuf.message.Message):
+class ListDeliveryExtensionsReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     PAGE_TOKEN_FIELD_NUMBER: builtins.int
     PAGE_SIZE_FIELD_NUMBER: builtins.int
     page_token: builtins.str
     page_size: builtins.int
     def __init__(
         self,
         *,
         page_token: builtins.str = ...,
         page_size: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["page_size", b"page_size", "page_token", b"page_token"]) -> None: ...
 
-global___ListDeliveryModulesReq = ListDeliveryModulesReq
+global___ListDeliveryExtensionsReq = ListDeliveryExtensionsReq
 
-class ListDeliveryModulesResp(google.protobuf.message.Message):
+class ListDeliveryExtensionsResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DELIVERY_MODULES_FIELD_NUMBER: builtins.int
+    DELIVERY_EXTENSIONS_FIELD_NUMBER: builtins.int
     NEXT_PAGE_TOKEN_FIELD_NUMBER: builtins.int
     @property
-    def delivery_modules(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.delivery_module.object_pb2.DeliveryModule]: ...
+    def delivery_extensions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.delivery_extension.object_pb2.DeliveryExtension]: ...
     next_page_token: builtins.str
     def __init__(
         self,
         *,
-        delivery_modules: collections.abc.Iterable[prodvana.proto.prodvana.delivery_module.object_pb2.DeliveryModule] | None = ...,
+        delivery_extensions: collections.abc.Iterable[prodvana.proto.prodvana.delivery_extension.object_pb2.DeliveryExtension] | None = ...,
         next_page_token: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["delivery_modules", b"delivery_modules", "next_page_token", b"next_page_token"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["delivery_extensions", b"delivery_extensions", "next_page_token", b"next_page_token"]) -> None: ...
 
-global___ListDeliveryModulesResp = ListDeliveryModulesResp
+global___ListDeliveryExtensionsResp = ListDeliveryExtensionsResp
 
-class GetDeliveryModuleReq(google.protobuf.message.Message):
+class GetDeliveryExtensionReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DELIVERY_MODULE_FIELD_NUMBER: builtins.int
-    delivery_module: builtins.str
+    DELIVERY_EXTENSION_FIELD_NUMBER: builtins.int
+    delivery_extension: builtins.str
     def __init__(
         self,
         *,
-        delivery_module: builtins.str = ...,
+        delivery_extension: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["delivery_module", b"delivery_module"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["delivery_extension", b"delivery_extension"]) -> None: ...
 
-global___GetDeliveryModuleReq = GetDeliveryModuleReq
+global___GetDeliveryExtensionReq = GetDeliveryExtensionReq
 
-class GetDeliveryModuleResp(google.protobuf.message.Message):
+class GetDeliveryExtensionResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DELIVERY_MODULE_FIELD_NUMBER: builtins.int
+    DELIVERY_EXTENSION_FIELD_NUMBER: builtins.int
     @property
-    def delivery_module(self) -> prodvana.proto.prodvana.delivery_module.object_pb2.DeliveryModule: ...
+    def delivery_extension(self) -> prodvana.proto.prodvana.delivery_extension.object_pb2.DeliveryExtension: ...
     def __init__(
         self,
         *,
-        delivery_module: prodvana.proto.prodvana.delivery_module.object_pb2.DeliveryModule | None = ...,
+        delivery_extension: prodvana.proto.prodvana.delivery_extension.object_pb2.DeliveryExtension | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["delivery_module", b"delivery_module"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["delivery_module", b"delivery_module"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["delivery_extension", b"delivery_extension"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["delivery_extension", b"delivery_extension"]) -> None: ...
 
-global___GetDeliveryModuleResp = GetDeliveryModuleResp
+global___GetDeliveryExtensionResp = GetDeliveryExtensionResp
 
-class GetDeliveryModuleConfigReq(google.protobuf.message.Message):
+class GetDeliveryExtensionConfigReq(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DELIVERY_MODULE_FIELD_NUMBER: builtins.int
+    DELIVERY_EXTENSION_FIELD_NUMBER: builtins.int
     VERSION_FIELD_NUMBER: builtins.int
-    delivery_module: builtins.str
+    delivery_extension: builtins.str
     version: builtins.str
     """omit to get latest version"""
     def __init__(
         self,
         *,
-        delivery_module: builtins.str = ...,
+        delivery_extension: builtins.str = ...,
         version: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["delivery_module", b"delivery_module", "version", b"version"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["delivery_extension", b"delivery_extension", "version", b"version"]) -> None: ...
 
-global___GetDeliveryModuleConfigReq = GetDeliveryModuleConfigReq
+global___GetDeliveryExtensionConfigReq = GetDeliveryExtensionConfigReq
 
-class GetDeliveryModuleConfigResp(google.protobuf.message.Message):
+class GetDeliveryExtensionConfigResp(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CONFIG_FIELD_NUMBER: builtins.int
     VERSION_FIELD_NUMBER: builtins.int
     @property
-    def config(self) -> prodvana.proto.prodvana.delivery_module.config_pb2.DeliveryModuleConfig: ...
+    def config(self) -> prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig: ...
     version: builtins.str
     def __init__(
         self,
         *,
-        config: prodvana.proto.prodvana.delivery_module.config_pb2.DeliveryModuleConfig | None = ...,
+        config: prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig | None = ...,
         version: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["config", b"config"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["config", b"config", "version", b"version"]) -> None: ...
 
-global___GetDeliveryModuleConfigResp = GetDeliveryModuleConfigResp
+global___GetDeliveryExtensionConfigResp = GetDeliveryExtensionConfigResp
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/manager_pb2_grpc.py` & `prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,198 +1,198 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from prodvana.proto.prodvana.delivery_module import manager_pb2 as prodvana_dot_delivery__module_dot_manager__pb2
+from prodvana.proto.prodvana.delivery_extension import manager_pb2 as prodvana_dot_delivery__extension_dot_manager__pb2
 
 
-class DeliveryModuleManagerStub(object):
+class DeliveryExtensionManagerStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.ConfigureDeliveryModule = channel.unary_unary(
-                '/prodvana.delivery_module.DeliveryModuleManager/ConfigureDeliveryModule',
-                request_serializer=prodvana_dot_delivery__module_dot_manager__pb2.ConfigureDeliveryModuleReq.SerializeToString,
-                response_deserializer=prodvana_dot_delivery__module_dot_manager__pb2.ConfigureDeliveryModuleResp.FromString,
+        self.ConfigureDeliveryExtension = channel.unary_unary(
+                '/prodvana.delivery_extension.DeliveryExtensionManager/ConfigureDeliveryExtension',
+                request_serializer=prodvana_dot_delivery__extension_dot_manager__pb2.ConfigureDeliveryExtensionReq.SerializeToString,
+                response_deserializer=prodvana_dot_delivery__extension_dot_manager__pb2.ConfigureDeliveryExtensionResp.FromString,
                 )
-        self.ValidateConfigureDeliveryModule = channel.unary_unary(
-                '/prodvana.delivery_module.DeliveryModuleManager/ValidateConfigureDeliveryModule',
-                request_serializer=prodvana_dot_delivery__module_dot_manager__pb2.ConfigureDeliveryModuleReq.SerializeToString,
-                response_deserializer=prodvana_dot_delivery__module_dot_manager__pb2.ValidateConfigureDeliveryModuleResp.FromString,
+        self.ValidateConfigureDeliveryExtension = channel.unary_unary(
+                '/prodvana.delivery_extension.DeliveryExtensionManager/ValidateConfigureDeliveryExtension',
+                request_serializer=prodvana_dot_delivery__extension_dot_manager__pb2.ConfigureDeliveryExtensionReq.SerializeToString,
+                response_deserializer=prodvana_dot_delivery__extension_dot_manager__pb2.ValidateConfigureDeliveryExtensionResp.FromString,
                 )
-        self.ListDeliveryModules = channel.unary_unary(
-                '/prodvana.delivery_module.DeliveryModuleManager/ListDeliveryModules',
-                request_serializer=prodvana_dot_delivery__module_dot_manager__pb2.ListDeliveryModulesReq.SerializeToString,
-                response_deserializer=prodvana_dot_delivery__module_dot_manager__pb2.ListDeliveryModulesResp.FromString,
+        self.ListDeliveryExtensions = channel.unary_unary(
+                '/prodvana.delivery_extension.DeliveryExtensionManager/ListDeliveryExtensions',
+                request_serializer=prodvana_dot_delivery__extension_dot_manager__pb2.ListDeliveryExtensionsReq.SerializeToString,
+                response_deserializer=prodvana_dot_delivery__extension_dot_manager__pb2.ListDeliveryExtensionsResp.FromString,
                 )
-        self.GetDeliveryModule = channel.unary_unary(
-                '/prodvana.delivery_module.DeliveryModuleManager/GetDeliveryModule',
-                request_serializer=prodvana_dot_delivery__module_dot_manager__pb2.GetDeliveryModuleReq.SerializeToString,
-                response_deserializer=prodvana_dot_delivery__module_dot_manager__pb2.GetDeliveryModuleResp.FromString,
+        self.GetDeliveryExtension = channel.unary_unary(
+                '/prodvana.delivery_extension.DeliveryExtensionManager/GetDeliveryExtension',
+                request_serializer=prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionReq.SerializeToString,
+                response_deserializer=prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionResp.FromString,
                 )
-        self.GetDeliveryModuleConfig = channel.unary_unary(
-                '/prodvana.delivery_module.DeliveryModuleManager/GetDeliveryModuleConfig',
-                request_serializer=prodvana_dot_delivery__module_dot_manager__pb2.GetDeliveryModuleConfigReq.SerializeToString,
-                response_deserializer=prodvana_dot_delivery__module_dot_manager__pb2.GetDeliveryModuleConfigResp.FromString,
+        self.GetDeliveryExtensionConfig = channel.unary_unary(
+                '/prodvana.delivery_extension.DeliveryExtensionManager/GetDeliveryExtensionConfig',
+                request_serializer=prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionConfigReq.SerializeToString,
+                response_deserializer=prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionConfigResp.FromString,
                 )
 
 
-class DeliveryModuleManagerServicer(object):
+class DeliveryExtensionManagerServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def ConfigureDeliveryModule(self, request, context):
+    def ConfigureDeliveryExtension(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ValidateConfigureDeliveryModule(self, request, context):
+    def ValidateConfigureDeliveryExtension(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListDeliveryModules(self, request, context):
+    def ListDeliveryExtensions(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetDeliveryModule(self, request, context):
+    def GetDeliveryExtension(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetDeliveryModuleConfig(self, request, context):
+    def GetDeliveryExtensionConfig(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_DeliveryModuleManagerServicer_to_server(servicer, server):
+def add_DeliveryExtensionManagerServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'ConfigureDeliveryModule': grpc.unary_unary_rpc_method_handler(
-                    servicer.ConfigureDeliveryModule,
-                    request_deserializer=prodvana_dot_delivery__module_dot_manager__pb2.ConfigureDeliveryModuleReq.FromString,
-                    response_serializer=prodvana_dot_delivery__module_dot_manager__pb2.ConfigureDeliveryModuleResp.SerializeToString,
+            'ConfigureDeliveryExtension': grpc.unary_unary_rpc_method_handler(
+                    servicer.ConfigureDeliveryExtension,
+                    request_deserializer=prodvana_dot_delivery__extension_dot_manager__pb2.ConfigureDeliveryExtensionReq.FromString,
+                    response_serializer=prodvana_dot_delivery__extension_dot_manager__pb2.ConfigureDeliveryExtensionResp.SerializeToString,
             ),
-            'ValidateConfigureDeliveryModule': grpc.unary_unary_rpc_method_handler(
-                    servicer.ValidateConfigureDeliveryModule,
-                    request_deserializer=prodvana_dot_delivery__module_dot_manager__pb2.ConfigureDeliveryModuleReq.FromString,
-                    response_serializer=prodvana_dot_delivery__module_dot_manager__pb2.ValidateConfigureDeliveryModuleResp.SerializeToString,
+            'ValidateConfigureDeliveryExtension': grpc.unary_unary_rpc_method_handler(
+                    servicer.ValidateConfigureDeliveryExtension,
+                    request_deserializer=prodvana_dot_delivery__extension_dot_manager__pb2.ConfigureDeliveryExtensionReq.FromString,
+                    response_serializer=prodvana_dot_delivery__extension_dot_manager__pb2.ValidateConfigureDeliveryExtensionResp.SerializeToString,
             ),
-            'ListDeliveryModules': grpc.unary_unary_rpc_method_handler(
-                    servicer.ListDeliveryModules,
-                    request_deserializer=prodvana_dot_delivery__module_dot_manager__pb2.ListDeliveryModulesReq.FromString,
-                    response_serializer=prodvana_dot_delivery__module_dot_manager__pb2.ListDeliveryModulesResp.SerializeToString,
+            'ListDeliveryExtensions': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListDeliveryExtensions,
+                    request_deserializer=prodvana_dot_delivery__extension_dot_manager__pb2.ListDeliveryExtensionsReq.FromString,
+                    response_serializer=prodvana_dot_delivery__extension_dot_manager__pb2.ListDeliveryExtensionsResp.SerializeToString,
             ),
-            'GetDeliveryModule': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetDeliveryModule,
-                    request_deserializer=prodvana_dot_delivery__module_dot_manager__pb2.GetDeliveryModuleReq.FromString,
-                    response_serializer=prodvana_dot_delivery__module_dot_manager__pb2.GetDeliveryModuleResp.SerializeToString,
+            'GetDeliveryExtension': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetDeliveryExtension,
+                    request_deserializer=prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionReq.FromString,
+                    response_serializer=prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionResp.SerializeToString,
             ),
-            'GetDeliveryModuleConfig': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetDeliveryModuleConfig,
-                    request_deserializer=prodvana_dot_delivery__module_dot_manager__pb2.GetDeliveryModuleConfigReq.FromString,
-                    response_serializer=prodvana_dot_delivery__module_dot_manager__pb2.GetDeliveryModuleConfigResp.SerializeToString,
+            'GetDeliveryExtensionConfig': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetDeliveryExtensionConfig,
+                    request_deserializer=prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionConfigReq.FromString,
+                    response_serializer=prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionConfigResp.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'prodvana.delivery_module.DeliveryModuleManager', rpc_method_handlers)
+            'prodvana.delivery_extension.DeliveryExtensionManager', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class DeliveryModuleManager(object):
+class DeliveryExtensionManager(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def ConfigureDeliveryModule(request,
+    def ConfigureDeliveryExtension(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/prodvana.delivery_module.DeliveryModuleManager/ConfigureDeliveryModule',
-            prodvana_dot_delivery__module_dot_manager__pb2.ConfigureDeliveryModuleReq.SerializeToString,
-            prodvana_dot_delivery__module_dot_manager__pb2.ConfigureDeliveryModuleResp.FromString,
+        return grpc.experimental.unary_unary(request, target, '/prodvana.delivery_extension.DeliveryExtensionManager/ConfigureDeliveryExtension',
+            prodvana_dot_delivery__extension_dot_manager__pb2.ConfigureDeliveryExtensionReq.SerializeToString,
+            prodvana_dot_delivery__extension_dot_manager__pb2.ConfigureDeliveryExtensionResp.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ValidateConfigureDeliveryModule(request,
+    def ValidateConfigureDeliveryExtension(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/prodvana.delivery_module.DeliveryModuleManager/ValidateConfigureDeliveryModule',
-            prodvana_dot_delivery__module_dot_manager__pb2.ConfigureDeliveryModuleReq.SerializeToString,
-            prodvana_dot_delivery__module_dot_manager__pb2.ValidateConfigureDeliveryModuleResp.FromString,
+        return grpc.experimental.unary_unary(request, target, '/prodvana.delivery_extension.DeliveryExtensionManager/ValidateConfigureDeliveryExtension',
+            prodvana_dot_delivery__extension_dot_manager__pb2.ConfigureDeliveryExtensionReq.SerializeToString,
+            prodvana_dot_delivery__extension_dot_manager__pb2.ValidateConfigureDeliveryExtensionResp.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ListDeliveryModules(request,
+    def ListDeliveryExtensions(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/prodvana.delivery_module.DeliveryModuleManager/ListDeliveryModules',
-            prodvana_dot_delivery__module_dot_manager__pb2.ListDeliveryModulesReq.SerializeToString,
-            prodvana_dot_delivery__module_dot_manager__pb2.ListDeliveryModulesResp.FromString,
+        return grpc.experimental.unary_unary(request, target, '/prodvana.delivery_extension.DeliveryExtensionManager/ListDeliveryExtensions',
+            prodvana_dot_delivery__extension_dot_manager__pb2.ListDeliveryExtensionsReq.SerializeToString,
+            prodvana_dot_delivery__extension_dot_manager__pb2.ListDeliveryExtensionsResp.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetDeliveryModule(request,
+    def GetDeliveryExtension(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/prodvana.delivery_module.DeliveryModuleManager/GetDeliveryModule',
-            prodvana_dot_delivery__module_dot_manager__pb2.GetDeliveryModuleReq.SerializeToString,
-            prodvana_dot_delivery__module_dot_manager__pb2.GetDeliveryModuleResp.FromString,
+        return grpc.experimental.unary_unary(request, target, '/prodvana.delivery_extension.DeliveryExtensionManager/GetDeliveryExtension',
+            prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionReq.SerializeToString,
+            prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionResp.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetDeliveryModuleConfig(request,
+    def GetDeliveryExtensionConfig(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/prodvana.delivery_module.DeliveryModuleManager/GetDeliveryModuleConfig',
-            prodvana_dot_delivery__module_dot_manager__pb2.GetDeliveryModuleConfigReq.SerializeToString,
-            prodvana_dot_delivery__module_dot_manager__pb2.GetDeliveryModuleConfigResp.FromString,
+        return grpc.experimental.unary_unary(request, target, '/prodvana.delivery_extension.DeliveryExtensionManager/GetDeliveryExtensionConfig',
+            prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionConfigReq.SerializeToString,
+            prodvana_dot_delivery__extension_dot_manager__pb2.GetDeliveryExtensionConfigResp.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/object_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/object_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: prodvana/delivery_module/object.proto
+# source: prodvana/delivery_extension/object.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.prodvana.object import meta_pb2 as prodvana_dot_object_dot_meta__pb2
-from prodvana.proto.prodvana.delivery_module import config_pb2 as prodvana_dot_delivery__module_dot_config__pb2
+from prodvana.proto.prodvana.delivery_extension import config_pb2 as prodvana_dot_delivery__extension_dot_config__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%prodvana/delivery_module/object.proto\x12\x18prodvana.delivery_module\x1a\x1aprodvana/object/meta.proto\x1a%prodvana/delivery_module/config.proto\"\xb9\x01\n\x0e\x44\x65liveryModule\x12)\n\x04meta\x18\x01 \x01(\x0b\x32\x1b.prodvana.object.ObjectMeta\x12>\n\x06\x63onfig\x18\x02 \x01(\x0b\x32..prodvana.delivery_module.DeliveryModuleConfig\x12<\n\x05state\x18\x03 \x01(\x0b\x32-.prodvana.delivery_module.DeliveryModuleState\"\x15\n\x13\x44\x65liveryModuleStateBTZRgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_moduleb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(prodvana/delivery_extension/object.proto\x12\x1bprodvana.delivery_extension\x1a\x1aprodvana/object/meta.proto\x1a(prodvana/delivery_extension/config.proto\"\xc8\x01\n\x11\x44\x65liveryExtension\x12)\n\x04meta\x18\x01 \x01(\x0b\x32\x1b.prodvana.object.ObjectMeta\x12\x44\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfig\x12\x42\n\x05state\x18\x03 \x01(\x0b\x32\x33.prodvana.delivery_extension.DeliveryExtensionState\"\x18\n\x16\x44\x65liveryExtensionStateBWZUgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_extensionb\x06proto3')
 
 
 
-_DELIVERYMODULE = DESCRIPTOR.message_types_by_name['DeliveryModule']
-_DELIVERYMODULESTATE = DESCRIPTOR.message_types_by_name['DeliveryModuleState']
-DeliveryModule = _reflection.GeneratedProtocolMessageType('DeliveryModule', (_message.Message,), {
-  'DESCRIPTOR' : _DELIVERYMODULE,
-  '__module__' : 'prodvana.delivery_module.object_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_module.DeliveryModule)
+_DELIVERYEXTENSION = DESCRIPTOR.message_types_by_name['DeliveryExtension']
+_DELIVERYEXTENSIONSTATE = DESCRIPTOR.message_types_by_name['DeliveryExtensionState']
+DeliveryExtension = _reflection.GeneratedProtocolMessageType('DeliveryExtension', (_message.Message,), {
+  'DESCRIPTOR' : _DELIVERYEXTENSION,
+  '__module__' : 'prodvana.delivery_extension.object_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.DeliveryExtension)
   })
-_sym_db.RegisterMessage(DeliveryModule)
+_sym_db.RegisterMessage(DeliveryExtension)
 
-DeliveryModuleState = _reflection.GeneratedProtocolMessageType('DeliveryModuleState', (_message.Message,), {
-  'DESCRIPTOR' : _DELIVERYMODULESTATE,
-  '__module__' : 'prodvana.delivery_module.object_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.delivery_module.DeliveryModuleState)
+DeliveryExtensionState = _reflection.GeneratedProtocolMessageType('DeliveryExtensionState', (_message.Message,), {
+  'DESCRIPTOR' : _DELIVERYEXTENSIONSTATE,
+  '__module__' : 'prodvana.delivery_extension.object_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.delivery_extension.DeliveryExtensionState)
   })
-_sym_db.RegisterMessage(DeliveryModuleState)
+_sym_db.RegisterMessage(DeliveryExtensionState)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZRgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_module'
-  _DELIVERYMODULE._serialized_start=135
-  _DELIVERYMODULE._serialized_end=320
-  _DELIVERYMODULESTATE._serialized_start=322
-  _DELIVERYMODULESTATE._serialized_end=343
+  DESCRIPTOR._serialized_options = b'ZUgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_extension'
+  _DELIVERYEXTENSION._serialized_start=144
+  _DELIVERYEXTENSION._serialized_end=344
+  _DELIVERYEXTENSIONSTATE._serialized_start=346
+  _DELIVERYEXTENSIONSTATE._serialized_end=370
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/delivery_module/object_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.message
-import prodvana.proto.prodvana.delivery_module.config_pb2
+import prodvana.proto.prodvana.delivery_extension.config_pb2
 import prodvana.proto.prodvana.object.meta_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class DeliveryModule(google.protobuf.message.Message):
+class DeliveryExtension(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     META_FIELD_NUMBER: builtins.int
     CONFIG_FIELD_NUMBER: builtins.int
     STATE_FIELD_NUMBER: builtins.int
     @property
     def meta(self) -> prodvana.proto.prodvana.object.meta_pb2.ObjectMeta: ...
     @property
-    def config(self) -> prodvana.proto.prodvana.delivery_module.config_pb2.DeliveryModuleConfig: ...
+    def config(self) -> prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig: ...
     @property
-    def state(self) -> global___DeliveryModuleState: ...
+    def state(self) -> global___DeliveryExtensionState: ...
     def __init__(
         self,
         *,
         meta: prodvana.proto.prodvana.object.meta_pb2.ObjectMeta | None = ...,
-        config: prodvana.proto.prodvana.delivery_module.config_pb2.DeliveryModuleConfig | None = ...,
-        state: global___DeliveryModuleState | None = ...,
+        config: prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig | None = ...,
+        state: global___DeliveryExtensionState | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["config", b"config", "meta", b"meta", "state", b"state"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["config", b"config", "meta", b"meta", "state", b"state"]) -> None: ...
 
-global___DeliveryModule = DeliveryModule
+global___DeliveryExtension = DeliveryExtension
 
-class DeliveryModuleState(google.protobuf.message.Message):
+class DeliveryExtensionState(google.protobuf.message.Message):
     """TODO(naphat) list custom task instances?"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
-global___DeliveryModuleState = DeliveryModuleState
+global___DeliveryExtensionState = DeliveryExtensionState
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/desired_state/manager_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/desired_state/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/desired_state/manager_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/desired_state/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py` & `prodvana-0.1.5/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 from prodvana.proto.prodvana.common_config import program_pb2 as prodvana_dot_common__config_dot_program__pb2
 from prodvana.proto.prodvana.common_config import retry_pb2 as prodvana_dot_common__config_dot_retry__pb2
 from prodvana.proto.prodvana.protection import protection_reference_pb2 as prodvana_dot_protection_dot_protection__reference__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0prodvana/desired_state/model/desired_state.proto\x12\x1cprodvana.desired_state.model\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a$prodvana/common_config/program.proto\x1a\"prodvana/common_config/retry.proto\x1a.prodvana/protection/protection_reference.proto\"p\n\x0eProtectionLink\x12;\n\tlifecycle\x18\x03 \x01(\x0b\x32(.prodvana.protection.ProtectionLifecycle\x12\x15\n\rattachment_id\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\x93\x06\n\tCondition\x12X\n\x07rc_cond\x18\x01 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.ReleaseChannelStableConditionH\x00\x12Q\n\x0fmanual_approval\x18\x02 \x01(\x0b\x32\x36.prodvana.desired_state.model.Condition.ManualApprovalH\x00\x12\\\n\x0b\x63ustom_task\x18\x03 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.CustomTaskSuccessfulConditionH\x00\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x1a\xa7\x01\n\x1dReleaseChannelStableCondition\x12\x13\n\x0b\x61pplication\x18\x01 \x01(\t\x12\x0f\n\x07service\x18\x02 \x01(\t\x12\x12\n\nservice_id\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x05 \x01(\t\x12\x17\n\x0fservice_version\x18\x06 \x01(\t\x1a\x1f\n\x0eManualApproval\x12\r\n\x05topic\x18\x01 \x01(\t\x1a\x88\x02\n\x1d\x43ustomTaskSuccessfulCondition\x12\x18\n\x10\x63ustom_task_name\x18\x01 \x01(\t\x12\x66\n\nprotection\x18\x02 \x01(\x0b\x32P.prodvana.desired_state.model.Condition.CustomTaskSuccessfulCondition.ProtectionH\x00\x1a[\n\nProtection\x12\x0c\n\x04name\x18\x01 \x01(\t\x12?\n\ttask_type\x18\x03 \x01(\x0e\x32,.prodvana.desired_state.model.CustomTaskTypeB\x08\n\x06sourceB\x0b\n\tcondition\"L\n\nIdentifier\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32\".prodvana.desired_state.model.Type\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x89\x03\n\x08Metadata\x12>\n\rpreconditions\x18\x01 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12;\n\ninvariants\x18\x02 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12\x36\n\x04self\x18\x03 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x12\x1d\n\x15root_desired_state_id\x18\x05 \x01(\t\x12\x46\n\x10protection_links\x18\x06 \x03(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12G\n\x0bprotections\x18\x07 \x03(\x0b\x32\x32.prodvana.desired_state.model.ProtectionAttachment\"\xad\x01\n\x11StatusExplanation\x12\x39\n\x07subject\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12:\n\x06reason\x18\x02 \x01(\x0e\x32*.prodvana.desired_state.model.StatusReason\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x10\n\x08messages\x18\x04 \x03(\t\"\x8b\x01\n\x11\x41\x63tionExplanation\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12=\n\x0b\x61\x63tion_type\x18\x02 \x01(\x0e\x32(.prodvana.desired_state.model.ActionType\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xcf\x01\n\x07Version\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x10\n\x08replicas\x18\x02 \x01(\x05\x12\x1a\n\x12\x61vailable_replicas\x18\x08 \x01(\x05\x12\x32\n\x0epush_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12\x17\n\x0ftarget_replicas\x18\x06 \x01(\x05J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08R\tunhealthyR\x11unhealthy_reasons\"\x86\x03\n\x14ServiceInstanceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x12\n\nservice_id\x18\x08 \x01(\t\x12\x1a\n\x12release_channel_id\x18\t \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12?\n\x10rollback_version\x18\x06 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12\x10\n\x08rollback\x18\x07 \x01(\x08\x12=\n\x08\x64\x65livery\x18\n \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\"\x9d\x02\n\x0cServiceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x12\n\nservice_id\x18\x05 \x01(\t\x12L\n\x10release_channels\x18\x06 \x03(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceState\x12\x43\n\x0c\x63ustom_tasks\x18\x07 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateJ\x04\x08\x04\x10\x05J\x04\x08\x08\x10\t\"\xd2\x01\n\x11ServiceGroupState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12<\n\x08services\x18\x02 \x03(\x0b\x32*.prodvana.desired_state.model.ServiceState\x12\x43\n\x0c\x63ustom_tasks\x18\x03 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateJ\x04\x08\x04\x10\x05\"\xa8\x02\n\x13\x43\x61naryProgressState\x12H\n\x06status\x18\x01 \x01(\x0e\x32\x38.prodvana.desired_state.model.CanaryProgressState.Status\x12 \n\rcanary_weight\x18\x02 \x01(\x05\x42\t\xfa\x42\x06\x1a\x04\x18\x64(\x00\x12+\n\x08\x64uration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x39\n\x15pause_start_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"=\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\r\n\tCOMPLETED\x10\x03\"\x94\x03\n\rDeliveryState\x12\x18\n\x10\x64\x65sired_state_id\x18\x0c \x01(\t\x12\x42\n\x06status\x18\x08 \x01(\x0e\x32\x32.prodvana.desired_state.model.DeliveryState.Status\x12\x0f\n\x07message\x18\x06 \x01(\t\x12J\n\x0f\x63\x61nary_progress\x18\x0b \x03(\x0b\x32\x31.prodvana.desired_state.model.CanaryProgressState\x12\x11\n\tfirst_run\x18\r \x01(\x08\x12\x12\n\ngeneration\x18\x0e \x01(\t\"q\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_PROGRESSING\x10\x01\x12\x11\n\rSTATUS_PAUSED\x10\x02\x12\x12\n\x0eSTATUS_HEALTHY\x10\x03\x12\x14\n\x10STATUS_UNHEALTHY\x10\x04J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08J\x04\x08\t\x10\nJ\x04\x08\n\x10\x0b\"\xff\x03\n\rRuntimeObject\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0bobject_type\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x42\n\x06status\x18\x06 \x01(\x0e\x32\x32.prodvana.desired_state.model.RuntimeObject.Status\x12?\n\x10rollback_version\x18\x07 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12=\n\x08\x64\x65livery\x18\x08 \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\x12\x18\n\x10version_agnostic\x18\n \x01(\x08\x12\x12\n\nstate_hash\x18\x0b \x01(\x0c\x12\x0f\n\x07message\x18\x0c \x01(\t\"0\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\r\n\tSUCCEEDED\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02J\x04\x08\t\x10\nR\x0eunhealthy_pods\"O\n\x0e\x43onditionState\x12=\n\x06status\x18\x01 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\"\xde\x02\n\x0c\x43ontrolState\x12\x10\n\x08rollback\x18\x01 \x01(\x08\x12I\n\x13precondition_states\x18\x02 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x46\n\x10invariant_states\x18\x03 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x0e\n\x06paused\x18\x04 \x01(\x08\x12L\n\x13status_explanations\x18\x05 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12K\n\x12\x61\x63tion_explanation\x18\x06 \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation\"\x9e\x01\n\x13ManualApprovalState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.prodvana.desired_state.model.ManualApprovalStatus\x12\r\n\x05topic\x18\x03 \x01(\t\"\xed\x04\n\x05State\x12=\n\x07service\x18\x01 \x01(\x0b\x32*.prodvana.desired_state.model.ServiceStateH\x00\x12N\n\x10service_instance\x18\x02 \x01(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceStateH\x00\x12H\n\rservice_group\x18\x03 \x01(\x0b\x32/.prodvana.desired_state.model.ServiceGroupStateH\x00\x12\x45\n\x0eruntime_object\x18\x04 \x01(\x0b\x32+.prodvana.desired_state.model.RuntimeObjectH\x00\x12L\n\x0fmanual_approval\x18\x05 \x01(\x0b\x32\x31.prodvana.desired_state.model.ManualApprovalStateH\x00\x12\x44\n\x0b\x63ustom_task\x18\x06 \x01(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateH\x00\x12S\n\x15protection_attachment\x18\x07 \x01(\x0b\x32\x32.prodvana.desired_state.model.ProtectionAttachmentH\x00\x12L\n\x0fprotection_link\x18\x08 \x01(\x0b\x32\x31.prodvana.desired_state.model.ProtectionLinkStateH\x00\x42\r\n\x0bstate_oneof\"\x82\x01\n\x0b\x41nnotations\x12I\n\x0b\x61nnotations\x18\x01 \x03(\x0b\x32\x34.prodvana.desired_state.model.Annotations.Annotation\x1a(\n\nAnnotation\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xae\x01\n\x18\x43ustomTaskExecutionState\x12>\n\x06status\x18\x01 \x01(\x0e\x32..prodvana.desired_state.model.CustomTaskStatus\x12\x10\n\x08\x61ttempts\x18\x02 \x01(\x03\x12@\n\x1clatest_attempt_end_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xce\x03\n\x0f\x43ustomTaskState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x15\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x1c\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x13\n\x0b\x61pplication\x18\x04 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x05 \x01(\t\x12\x17\n\x0frelease_channel\x18\x06 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x07 \x01(\t\x12@\n\x07program\x18\t \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12J\n\ntask_state\x18\x0c \x01(\x0b\x32\x36.prodvana.desired_state.model.CustomTaskExecutionState\x12\x39\n\x0cretry_config\x18\r \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12\x13\n\x0bservice_ids\x18\x0e \x03(\tJ\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0c\"\xd4\x04\n\x13ProtectionLinkState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12=\n\x06status\x18\x02 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\x12:\n\x04link\x18\x03 \x01(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12\x35\n\x11started_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11stopped_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12T\n\x0estopped_reason\x18\x06 \x01(\x0e\x32<.prodvana.desired_state.model.ProtectionLinkState.StopReason\x12;\n\x17\x66irst_success_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x8a\x01\n\nStopReason\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x17\n\x13LIFECYCLE_COMPLETED\x10\x01\x12\x12\n\x0eSUCCEEDED_ONCE\x10\x02\x12\x1a\n\x16SUCCEEDED_FOR_DURATION\x10\x03\x12\r\n\tTIMED_OUT\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x12\x0b\n\x07\x44\x45LETED\x10\x06\"\x89\x04\n\x14ProtectionAttachment\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x46\n\x17last_completed_versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\x12\x15\n\rprotection_id\x18\x03 \x01(\t\x12\x15\n\rattachment_id\x18\x04 \x01(\t\"\xde\x01\n\x06Signal\x12\x36\n\x04type\x18\x01 \x01(\x0e\x32(.prodvana.desired_state.model.SignalType\x12Z\n\x12\x64\x65livery_promotion\x18\x02 \x01(\x0b\x32<.prodvana.desired_state.model.Signal.DeliveryPromotionConfigH\x00\x1a\x36\n\x17\x44\x65liveryPromotionConfig\x12\r\n\x05stage\x18\x01 \x01(\x03\x12\x0c\n\x04\x66ull\x18\x02 \x01(\x08\x42\x08\n\x06\x63onfig\"?\n\x08\x44\x65\x62ugLog\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0b\n\x03log\x18\x02 \x01(\t*\xb3\x01\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVICE\x10\x01\x12\x14\n\x10SERVICE_INSTANCE\x10\x02\x12\x11\n\rSERVICE_GROUP\x10\x03\x12\x12\n\x0eRUNTIME_OBJECT\x10\x04\x12\x13\n\x0fMANUAL_APPROVAL\x10\x05\x12\x0f\n\x0b\x43USTOM_TASK\x10\x06\x12\x19\n\x15PROTECTION_ATTACHMENT\x10\x07\x12\x13\n\x0fPROTECTION_LINK\x10\x08*w\n\tLifecycle\x12\x15\n\x11UNKNOWN_LIFECYCLE\x10\x00\x12\x15\n\x11\x43ONVERGENCE_START\x10\x01\x12\x10\n\x0cPRE_APPROVAL\x10\x02\x12\x11\n\rPOST_APPROVAL\x10\x03\x12\x08\n\x04PUSH\x10\x04\x12\r\n\tPOST_PUSH\x10\x05*\x8e\x01\n\x0e\x43ustomTaskType\x12\x1c\n\x18\x43USTOM_TASK_TYPE_UNKNOWN\x10\x00\x12\x15\n\x11PRE_APPROVAL_TASK\x10\x01\x12\x0c\n\x08\x41PPROVAL\x10\x02\x12\x16\n\x12POST_APPROVAL_TASK\x10\x03\x12\r\n\tPUSH_TASK\x10\x04\x12\x12\n\x0ePOST_PUSH_TASK\x10\x05*\xf0\x01\n\x06Status\x12\x12\n\x0eUNKNOWN_STATUS\x10\x00\x12\x0e\n\nCONVERGING\x10\x01\x12\r\n\tCONVERGED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x10\n\x0cROLLING_BACK\x10\x04\x12\x0f\n\x0bROLLED_BACK\x10\x05\x12\x13\n\x0f\x46\x41ILED_ROLLBACK\x10\x0c\x12\n\n\x06PAUSED\x10\x06\x12\x10\n\x0c\x43HILD_PAUSED\x10\x07\x12\x19\n\x15WAITING_PRECONDITIONS\x10\x08\x12\x0c\n\x08REPLACED\x10\t\x12\x1b\n\x17WAITING_MANUAL_APPROVAL\x10\n\x12\x0b\n\x07\x44\x45LETED\x10\x0b*R\n\x0cSimpleStatus\x12\x0e\n\nSS_UNKNOWN\x10\x00\x12\x11\n\rSS_CONVERGING\x10\x01\x12\x10\n\x0cSS_CONVERGED\x10\x02\x12\r\n\tSS_FAILED\x10\x03*\xec\x01\n\x0cStatusReason\x12\x12\n\x0eREASON_UNKNOWN\x10\x00\x12\x14\n\x10NO_CURRENT_STATE\x10\x01\x12\x10\n\x0c\x41PPLY_FAILED\x10\x02\x12\x12\n\x0eUNHEALTHY_PODS\x10\x03\x12\x11\n\rUPDATING_PODS\x10\x04\x12\x14\n\x10VERSION_MISMATCH\x10\x05\x12\x19\n\x15RUNTIME_OBJECT_FAILED\x10\x06\x12\x18\n\x14PRECONDITIONS_FAILED\x10\x07\x12\x1c\n\x18MANUAL_APPROVAL_REJECTED\x10\x08\x12\x10\n\x0cSTUCK_ENTITY\x10\t*r\n\nActionType\x12\x17\n\x13\x41\x43TION_TYPE_UNKNOWN\x10\x00\x12\x18\n\x14\x41\x43TION_TYPE_APPLYING\x10\x01\x12\x17\n\x13\x41\x43TION_TYPE_APPLIED\x10\x02\x12\x18\n\x14\x41\x43TION_TYPE_COMPLETE\x10\x03*\x96\x01\n\x0f\x43onditionStatus\x12\x1c\n\x18\x43ONDITION_UNKNOWN_STATUS\x10\x00\x12\x15\n\x11\x43ONDITION_PENDING\x10\x01\x12\x17\n\x13\x43ONDITION_SATISFIED\x10\x02\x12\x1f\n\x1b\x43ONDITION_MANUALLY_BYPASSED\x10\x03\x12\x14\n\x10\x43ONDITION_FAILED\x10\x04*?\n\x14ManualApprovalStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x41PPROVED\x10\x01\x12\x0c\n\x08REJECTED\x10\x02*\x85\x01\n\x10\x43ustomTaskStatus\x12\x17\n\x13\x43USTOM_TASK_PENDING\x10\x00\x12\x1a\n\x16\x43USTOM_TASK_SUCCESSFUL\x10\x01\x12!\n\x1d\x43USTOM_TASK_RETRIES_EXHAUSTED\x10\x02\x12\x19\n\x15\x43USTOM_TASK_TIMED_OUT\x10\x03*8\n\nSignalType\x12\x12\n\x0eSIGNAL_UNKNOWN\x10\x00\x12\x16\n\x12\x44\x45LIVERY_PROMOTION\x10\x01\x42XZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/modelb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0prodvana/desired_state/model/desired_state.proto\x12\x1cprodvana.desired_state.model\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a$prodvana/common_config/program.proto\x1a\"prodvana/common_config/retry.proto\x1a.prodvana/protection/protection_reference.proto\"p\n\x0eProtectionLink\x12;\n\tlifecycle\x18\x03 \x01(\x0b\x32(.prodvana.protection.ProtectionLifecycle\x12\x15\n\rattachment_id\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\x93\x06\n\tCondition\x12X\n\x07rc_cond\x18\x01 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.ReleaseChannelStableConditionH\x00\x12Q\n\x0fmanual_approval\x18\x02 \x01(\x0b\x32\x36.prodvana.desired_state.model.Condition.ManualApprovalH\x00\x12\\\n\x0b\x63ustom_task\x18\x03 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.CustomTaskSuccessfulConditionH\x00\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x1a\xa7\x01\n\x1dReleaseChannelStableCondition\x12\x13\n\x0b\x61pplication\x18\x01 \x01(\t\x12\x0f\n\x07service\x18\x02 \x01(\t\x12\x12\n\nservice_id\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x05 \x01(\t\x12\x17\n\x0fservice_version\x18\x06 \x01(\t\x1a\x1f\n\x0eManualApproval\x12\r\n\x05topic\x18\x01 \x01(\t\x1a\x88\x02\n\x1d\x43ustomTaskSuccessfulCondition\x12\x18\n\x10\x63ustom_task_name\x18\x01 \x01(\t\x12\x66\n\nprotection\x18\x02 \x01(\x0b\x32P.prodvana.desired_state.model.Condition.CustomTaskSuccessfulCondition.ProtectionH\x00\x1a[\n\nProtection\x12\x0c\n\x04name\x18\x01 \x01(\t\x12?\n\ttask_type\x18\x03 \x01(\x0e\x32,.prodvana.desired_state.model.CustomTaskTypeB\x08\n\x06sourceB\x0b\n\tcondition\"L\n\nIdentifier\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32\".prodvana.desired_state.model.Type\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xd3\x02\n\x08Metadata\x12>\n\rpreconditions\x18\x01 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12;\n\ninvariants\x18\x02 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12\x36\n\x04self\x18\x03 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x12\x1d\n\x15root_desired_state_id\x18\x05 \x01(\t\x12\x46\n\x10protection_links\x18\x06 \x03(\x0b\x32,.prodvana.desired_state.model.ProtectionLinkJ\x04\x08\x07\x10\x08R\x0bprotections\"\xad\x01\n\x11StatusExplanation\x12\x39\n\x07subject\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12:\n\x06reason\x18\x02 \x01(\x0e\x32*.prodvana.desired_state.model.StatusReason\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x10\n\x08messages\x18\x04 \x03(\t\"\x8b\x01\n\x11\x41\x63tionExplanation\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12=\n\x0b\x61\x63tion_type\x18\x02 \x01(\x0e\x32(.prodvana.desired_state.model.ActionType\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xcf\x01\n\x07Version\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x10\n\x08replicas\x18\x02 \x01(\x05\x12\x1a\n\x12\x61vailable_replicas\x18\x08 \x01(\x05\x12\x32\n\x0epush_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12\x17\n\x0ftarget_replicas\x18\x06 \x01(\x05J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08R\tunhealthyR\x11unhealthy_reasons\"\x86\x03\n\x14ServiceInstanceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x12\n\nservice_id\x18\x08 \x01(\t\x12\x1a\n\x12release_channel_id\x18\t \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12?\n\x10rollback_version\x18\x06 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12\x10\n\x08rollback\x18\x07 \x01(\x08\x12=\n\x08\x64\x65livery\x18\n \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\"\x9d\x02\n\x0cServiceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x12\n\nservice_id\x18\x05 \x01(\t\x12L\n\x10release_channels\x18\x06 \x03(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceState\x12\x43\n\x0c\x63ustom_tasks\x18\x07 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateJ\x04\x08\x04\x10\x05J\x04\x08\x08\x10\t\"\xd2\x01\n\x11ServiceGroupState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12<\n\x08services\x18\x02 \x03(\x0b\x32*.prodvana.desired_state.model.ServiceState\x12\x43\n\x0c\x63ustom_tasks\x18\x03 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateJ\x04\x08\x04\x10\x05\"\xa8\x02\n\x13\x43\x61naryProgressState\x12H\n\x06status\x18\x01 \x01(\x0e\x32\x38.prodvana.desired_state.model.CanaryProgressState.Status\x12 \n\rcanary_weight\x18\x02 \x01(\x05\x42\t\xfa\x42\x06\x1a\x04\x18\x64(\x00\x12+\n\x08\x64uration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x39\n\x15pause_start_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"=\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\r\n\tCOMPLETED\x10\x03\"\x94\x03\n\rDeliveryState\x12\x18\n\x10\x64\x65sired_state_id\x18\x0c \x01(\t\x12\x42\n\x06status\x18\x08 \x01(\x0e\x32\x32.prodvana.desired_state.model.DeliveryState.Status\x12\x0f\n\x07message\x18\x06 \x01(\t\x12J\n\x0f\x63\x61nary_progress\x18\x0b \x03(\x0b\x32\x31.prodvana.desired_state.model.CanaryProgressState\x12\x11\n\tfirst_run\x18\r \x01(\x08\x12\x12\n\ngeneration\x18\x0e \x01(\t\"q\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_PROGRESSING\x10\x01\x12\x11\n\rSTATUS_PAUSED\x10\x02\x12\x12\n\x0eSTATUS_HEALTHY\x10\x03\x12\x14\n\x10STATUS_UNHEALTHY\x10\x04J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08J\x04\x08\t\x10\nJ\x04\x08\n\x10\x0b\"\xff\x03\n\rRuntimeObject\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0bobject_type\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x42\n\x06status\x18\x06 \x01(\x0e\x32\x32.prodvana.desired_state.model.RuntimeObject.Status\x12?\n\x10rollback_version\x18\x07 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12=\n\x08\x64\x65livery\x18\x08 \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\x12\x18\n\x10version_agnostic\x18\n \x01(\x08\x12\x12\n\nstate_hash\x18\x0b \x01(\x0c\x12\x0f\n\x07message\x18\x0c \x01(\t\"0\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\r\n\tSUCCEEDED\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02J\x04\x08\t\x10\nR\x0eunhealthy_pods\"O\n\x0e\x43onditionState\x12=\n\x06status\x18\x01 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\"\xde\x02\n\x0c\x43ontrolState\x12\x10\n\x08rollback\x18\x01 \x01(\x08\x12I\n\x13precondition_states\x18\x02 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x46\n\x10invariant_states\x18\x03 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x0e\n\x06paused\x18\x04 \x01(\x08\x12L\n\x13status_explanations\x18\x05 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12K\n\x12\x61\x63tion_explanation\x18\x06 \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation\"\x9e\x01\n\x13ManualApprovalState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.prodvana.desired_state.model.ManualApprovalStatus\x12\r\n\x05topic\x18\x03 \x01(\t\"\xc1\x05\n\x05State\x12=\n\x07service\x18\x01 \x01(\x0b\x32*.prodvana.desired_state.model.ServiceStateH\x00\x12N\n\x10service_instance\x18\x02 \x01(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceStateH\x00\x12H\n\rservice_group\x18\x03 \x01(\x0b\x32/.prodvana.desired_state.model.ServiceGroupStateH\x00\x12\x45\n\x0eruntime_object\x18\x04 \x01(\x0b\x32+.prodvana.desired_state.model.RuntimeObjectH\x00\x12L\n\x0fmanual_approval\x18\x05 \x01(\x0b\x32\x31.prodvana.desired_state.model.ManualApprovalStateH\x00\x12\x44\n\x0b\x63ustom_task\x18\x06 \x01(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateH\x00\x12S\n\x15protection_attachment\x18\x07 \x01(\x0b\x32\x32.prodvana.desired_state.model.ProtectionAttachmentH\x00\x12L\n\x0fprotection_link\x18\x08 \x01(\x0b\x32\x31.prodvana.desired_state.model.ProtectionLinkStateH\x00\x12R\n\x12\x64\x65livery_extension\x18\t \x01(\x0b\x32\x34.prodvana.desired_state.model.DeliveryExtensionStateH\x00\x42\r\n\x0bstate_oneof\"\x82\x01\n\x0b\x41nnotations\x12I\n\x0b\x61nnotations\x18\x01 \x03(\x0b\x32\x34.prodvana.desired_state.model.Annotations.Annotation\x1a(\n\nAnnotation\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xae\x01\n\x18\x43ustomTaskExecutionState\x12>\n\x06status\x18\x01 \x01(\x0e\x32..prodvana.desired_state.model.CustomTaskStatus\x12\x10\n\x08\x61ttempts\x18\x02 \x01(\x03\x12@\n\x1clatest_attempt_end_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xce\x03\n\x0f\x43ustomTaskState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x15\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x1c\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x13\n\x0b\x61pplication\x18\x04 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x05 \x01(\t\x12\x17\n\x0frelease_channel\x18\x06 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x07 \x01(\t\x12@\n\x07program\x18\t \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12J\n\ntask_state\x18\x0c \x01(\x0b\x32\x36.prodvana.desired_state.model.CustomTaskExecutionState\x12\x39\n\x0cretry_config\x18\r \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12\x13\n\x0bservice_ids\x18\x0e \x03(\tJ\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0c\"\xd4\x04\n\x13ProtectionLinkState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12=\n\x06status\x18\x02 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\x12:\n\x04link\x18\x03 \x01(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12\x35\n\x11started_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11stopped_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12T\n\x0estopped_reason\x18\x06 \x01(\x0e\x32<.prodvana.desired_state.model.ProtectionLinkState.StopReason\x12;\n\x17\x66irst_success_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x8a\x01\n\nStopReason\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x17\n\x13LIFECYCLE_COMPLETED\x10\x01\x12\x12\n\x0eSUCCEEDED_ONCE\x10\x02\x12\x1a\n\x16SUCCEEDED_FOR_DURATION\x10\x03\x12\r\n\tTIMED_OUT\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x12\x0b\n\x07\x44\x45LETED\x10\x06\"\x89\x04\n\x14ProtectionAttachment\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x46\n\x17last_completed_versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\x12\x15\n\rprotection_id\x18\x03 \x01(\t\x12\x15\n\rattachment_id\x18\x04 \x01(\t\"\xa8\x04\n\x16\x44\x65liveryExtensionState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x14\n\x0c\x65xtension_id\x18\x03 \x01(\t\x12@\n\x07program\x18\x04 \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x39\n\x0cretry_config\x18\x05 \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\"\xde\x01\n\x06Signal\x12\x36\n\x04type\x18\x01 \x01(\x0e\x32(.prodvana.desired_state.model.SignalType\x12Z\n\x12\x64\x65livery_promotion\x18\x02 \x01(\x0b\x32<.prodvana.desired_state.model.Signal.DeliveryPromotionConfigH\x00\x1a\x36\n\x17\x44\x65liveryPromotionConfig\x12\r\n\x05stage\x18\x01 \x01(\x03\x12\x0c\n\x04\x66ull\x18\x02 \x01(\x08\x42\x08\n\x06\x63onfig\"?\n\x08\x44\x65\x62ugLog\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0b\n\x03log\x18\x02 \x01(\t*\xcb\x01\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVICE\x10\x01\x12\x14\n\x10SERVICE_INSTANCE\x10\x02\x12\x11\n\rSERVICE_GROUP\x10\x03\x12\x12\n\x0eRUNTIME_OBJECT\x10\x04\x12\x13\n\x0fMANUAL_APPROVAL\x10\x05\x12\x0f\n\x0b\x43USTOM_TASK\x10\x06\x12\x19\n\x15PROTECTION_ATTACHMENT\x10\x07\x12\x13\n\x0fPROTECTION_LINK\x10\x08\x12\x16\n\x12\x44\x45LIVERY_EXTENSION\x10\t*\x83\x01\n\tLifecycle\x12\x15\n\x11UNKNOWN_LIFECYCLE\x10\x00\x12\x15\n\x11\x43ONVERGENCE_START\x10\x01\x12\x10\n\x0cPRE_APPROVAL\x10\x02\x12\x11\n\rPOST_APPROVAL\x10\x03\x12\x0e\n\nDEPLOYMENT\x10\x04\x12\x13\n\x0fPOST_DEPLOYMENT\x10\x05*\x9a\x01\n\x0e\x43ustomTaskType\x12\x1c\n\x18\x43USTOM_TASK_TYPE_UNKNOWN\x10\x00\x12\x15\n\x11PRE_APPROVAL_TASK\x10\x01\x12\x0c\n\x08\x41PPROVAL\x10\x02\x12\x16\n\x12POST_APPROVAL_TASK\x10\x03\x12\x13\n\x0f\x44\x45PLOYMENT_TASK\x10\x04\x12\x18\n\x14POST_DEPLOYMENT_TASK\x10\x05*\xf0\x01\n\x06Status\x12\x12\n\x0eUNKNOWN_STATUS\x10\x00\x12\x0e\n\nCONVERGING\x10\x01\x12\r\n\tCONVERGED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x10\n\x0cROLLING_BACK\x10\x04\x12\x0f\n\x0bROLLED_BACK\x10\x05\x12\x13\n\x0f\x46\x41ILED_ROLLBACK\x10\x0c\x12\n\n\x06PAUSED\x10\x06\x12\x10\n\x0c\x43HILD_PAUSED\x10\x07\x12\x19\n\x15WAITING_PRECONDITIONS\x10\x08\x12\x0c\n\x08REPLACED\x10\t\x12\x1b\n\x17WAITING_MANUAL_APPROVAL\x10\n\x12\x0b\n\x07\x44\x45LETED\x10\x0b*R\n\x0cSimpleStatus\x12\x0e\n\nSS_UNKNOWN\x10\x00\x12\x11\n\rSS_CONVERGING\x10\x01\x12\x10\n\x0cSS_CONVERGED\x10\x02\x12\r\n\tSS_FAILED\x10\x03*\xec\x01\n\x0cStatusReason\x12\x12\n\x0eREASON_UNKNOWN\x10\x00\x12\x14\n\x10NO_CURRENT_STATE\x10\x01\x12\x10\n\x0c\x41PPLY_FAILED\x10\x02\x12\x12\n\x0eUNHEALTHY_PODS\x10\x03\x12\x11\n\rUPDATING_PODS\x10\x04\x12\x14\n\x10VERSION_MISMATCH\x10\x05\x12\x19\n\x15RUNTIME_OBJECT_FAILED\x10\x06\x12\x18\n\x14PRECONDITIONS_FAILED\x10\x07\x12\x1c\n\x18MANUAL_APPROVAL_REJECTED\x10\x08\x12\x10\n\x0cSTUCK_ENTITY\x10\t*r\n\nActionType\x12\x17\n\x13\x41\x43TION_TYPE_UNKNOWN\x10\x00\x12\x18\n\x14\x41\x43TION_TYPE_APPLYING\x10\x01\x12\x17\n\x13\x41\x43TION_TYPE_APPLIED\x10\x02\x12\x18\n\x14\x41\x43TION_TYPE_COMPLETE\x10\x03*\x96\x01\n\x0f\x43onditionStatus\x12\x1c\n\x18\x43ONDITION_UNKNOWN_STATUS\x10\x00\x12\x15\n\x11\x43ONDITION_PENDING\x10\x01\x12\x17\n\x13\x43ONDITION_SATISFIED\x10\x02\x12\x1f\n\x1b\x43ONDITION_MANUALLY_BYPASSED\x10\x03\x12\x14\n\x10\x43ONDITION_FAILED\x10\x04*?\n\x14ManualApprovalStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x41PPROVED\x10\x01\x12\x0c\n\x08REJECTED\x10\x02*\x85\x01\n\x10\x43ustomTaskStatus\x12\x17\n\x13\x43USTOM_TASK_PENDING\x10\x00\x12\x1a\n\x16\x43USTOM_TASK_SUCCESSFUL\x10\x01\x12!\n\x1d\x43USTOM_TASK_RETRIES_EXHAUSTED\x10\x02\x12\x19\n\x15\x43USTOM_TASK_TIMED_OUT\x10\x03*8\n\nSignalType\x12\x12\n\x0eSIGNAL_UNKNOWN\x10\x00\x12\x16\n\x12\x44\x45LIVERY_PROMOTION\x10\x01\x42XZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/modelb\x06proto3')
 
 _TYPE = DESCRIPTOR.enum_types_by_name['Type']
 Type = enum_type_wrapper.EnumTypeWrapper(_TYPE)
 _LIFECYCLE = DESCRIPTOR.enum_types_by_name['Lifecycle']
 Lifecycle = enum_type_wrapper.EnumTypeWrapper(_LIFECYCLE)
 _CUSTOMTASKTYPE = DESCRIPTOR.enum_types_by_name['CustomTaskType']
 CustomTaskType = enum_type_wrapper.EnumTypeWrapper(_CUSTOMTASKTYPE)
@@ -50,26 +50,27 @@
 SERVICE_INSTANCE = 2
 SERVICE_GROUP = 3
 RUNTIME_OBJECT = 4
 MANUAL_APPROVAL = 5
 CUSTOM_TASK = 6
 PROTECTION_ATTACHMENT = 7
 PROTECTION_LINK = 8
+DELIVERY_EXTENSION = 9
 UNKNOWN_LIFECYCLE = 0
 CONVERGENCE_START = 1
 PRE_APPROVAL = 2
 POST_APPROVAL = 3
-PUSH = 4
-POST_PUSH = 5
+DEPLOYMENT = 4
+POST_DEPLOYMENT = 5
 CUSTOM_TASK_TYPE_UNKNOWN = 0
 PRE_APPROVAL_TASK = 1
 APPROVAL = 2
 POST_APPROVAL_TASK = 3
-PUSH_TASK = 4
-POST_PUSH_TASK = 5
+DEPLOYMENT_TASK = 4
+POST_DEPLOYMENT_TASK = 5
 UNKNOWN_STATUS = 0
 CONVERGING = 1
 CONVERGED = 2
 FAILED = 3
 ROLLING_BACK = 4
 ROLLED_BACK = 5
 FAILED_ROLLBACK = 12
@@ -136,14 +137,15 @@
 _STATE = DESCRIPTOR.message_types_by_name['State']
 _ANNOTATIONS = DESCRIPTOR.message_types_by_name['Annotations']
 _ANNOTATIONS_ANNOTATION = _ANNOTATIONS.nested_types_by_name['Annotation']
 _CUSTOMTASKEXECUTIONSTATE = DESCRIPTOR.message_types_by_name['CustomTaskExecutionState']
 _CUSTOMTASKSTATE = DESCRIPTOR.message_types_by_name['CustomTaskState']
 _PROTECTIONLINKSTATE = DESCRIPTOR.message_types_by_name['ProtectionLinkState']
 _PROTECTIONATTACHMENT = DESCRIPTOR.message_types_by_name['ProtectionAttachment']
+_DELIVERYEXTENSIONSTATE = DESCRIPTOR.message_types_by_name['DeliveryExtensionState']
 _SIGNAL = DESCRIPTOR.message_types_by_name['Signal']
 _SIGNAL_DELIVERYPROMOTIONCONFIG = _SIGNAL.nested_types_by_name['DeliveryPromotionConfig']
 _DEBUGLOG = DESCRIPTOR.message_types_by_name['DebugLog']
 _CANARYPROGRESSSTATE_STATUS = _CANARYPROGRESSSTATE.enum_types_by_name['Status']
 _DELIVERYSTATE_STATUS = _DELIVERYSTATE.enum_types_by_name['Status']
 _RUNTIMEOBJECT_STATUS = _RUNTIMEOBJECT.enum_types_by_name['Status']
 _PROTECTIONLINKSTATE_STOPREASON = _PROTECTIONLINKSTATE.enum_types_by_name['StopReason']
@@ -337,14 +339,21 @@
 ProtectionAttachment = _reflection.GeneratedProtocolMessageType('ProtectionAttachment', (_message.Message,), {
   'DESCRIPTOR' : _PROTECTIONATTACHMENT,
   '__module__' : 'prodvana.desired_state.model.desired_state_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.desired_state.model.ProtectionAttachment)
   })
 _sym_db.RegisterMessage(ProtectionAttachment)
 
+DeliveryExtensionState = _reflection.GeneratedProtocolMessageType('DeliveryExtensionState', (_message.Message,), {
+  'DESCRIPTOR' : _DELIVERYEXTENSIONSTATE,
+  '__module__' : 'prodvana.desired_state.model.desired_state_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.desired_state.model.DeliveryExtensionState)
+  })
+_sym_db.RegisterMessage(DeliveryExtensionState)
+
 Signal = _reflection.GeneratedProtocolMessageType('Signal', (_message.Message,), {
 
   'DeliveryPromotionConfig' : _reflection.GeneratedProtocolMessageType('DeliveryPromotionConfig', (_message.Message,), {
     'DESCRIPTOR' : _SIGNAL_DELIVERYPROMOTIONCONFIG,
     '__module__' : 'prodvana.desired_state.model.desired_state_pb2'
     # @@protoc_insertion_point(class_scope:prodvana.desired_state.model.Signal.DeliveryPromotionConfig)
     })
@@ -371,36 +380,38 @@
   _CANARYPROGRESSSTATE.fields_by_name['canary_weight']._serialized_options = b'\372B\006\032\004\030d(\000'
   _CUSTOMTASKSTATE.fields_by_name['name']._options = None
   _CUSTOMTASKSTATE.fields_by_name['name']._serialized_options = b'\372B\004r\002\020\001'
   _CUSTOMTASKSTATE.fields_by_name['description']._options = None
   _CUSTOMTASKSTATE.fields_by_name['description']._serialized_options = b'\372B\004r\002\020\001'
   _CUSTOMTASKSTATE.fields_by_name['program']._options = None
   _CUSTOMTASKSTATE.fields_by_name['program']._serialized_options = b'\372B\005\212\001\002\020\001'
-  _TYPE._serialized_start=7722
-  _TYPE._serialized_end=7901
-  _LIFECYCLE._serialized_start=7903
-  _LIFECYCLE._serialized_end=8022
-  _CUSTOMTASKTYPE._serialized_start=8025
-  _CUSTOMTASKTYPE._serialized_end=8167
-  _STATUS._serialized_start=8170
-  _STATUS._serialized_end=8410
-  _SIMPLESTATUS._serialized_start=8412
-  _SIMPLESTATUS._serialized_end=8494
-  _STATUSREASON._serialized_start=8497
-  _STATUSREASON._serialized_end=8733
-  _ACTIONTYPE._serialized_start=8735
-  _ACTIONTYPE._serialized_end=8849
-  _CONDITIONSTATUS._serialized_start=8852
-  _CONDITIONSTATUS._serialized_end=9002
-  _MANUALAPPROVALSTATUS._serialized_start=9004
-  _MANUALAPPROVALSTATUS._serialized_end=9067
-  _CUSTOMTASKSTATUS._serialized_start=9070
-  _CUSTOMTASKSTATUS._serialized_end=9203
-  _SIGNALTYPE._serialized_start=9205
-  _SIGNALTYPE._serialized_end=9261
+  _DELIVERYEXTENSIONSTATE.fields_by_name['program']._options = None
+  _DELIVERYEXTENSIONSTATE.fields_by_name['program']._serialized_options = b'\372B\005\212\001\002\020\001'
+  _TYPE._serialized_start=8307
+  _TYPE._serialized_end=8510
+  _LIFECYCLE._serialized_start=8513
+  _LIFECYCLE._serialized_end=8644
+  _CUSTOMTASKTYPE._serialized_start=8647
+  _CUSTOMTASKTYPE._serialized_end=8801
+  _STATUS._serialized_start=8804
+  _STATUS._serialized_end=9044
+  _SIMPLESTATUS._serialized_start=9046
+  _SIMPLESTATUS._serialized_end=9128
+  _STATUSREASON._serialized_start=9131
+  _STATUSREASON._serialized_end=9367
+  _ACTIONTYPE._serialized_start=9369
+  _ACTIONTYPE._serialized_end=9483
+  _CONDITIONSTATUS._serialized_start=9486
+  _CONDITIONSTATUS._serialized_end=9636
+  _MANUALAPPROVALSTATUS._serialized_start=9638
+  _MANUALAPPROVALSTATUS._serialized_end=9701
+  _CUSTOMTASKSTATUS._serialized_start=9704
+  _CUSTOMTASKSTATUS._serialized_end=9837
+  _SIGNALTYPE._serialized_start=9839
+  _SIGNALTYPE._serialized_end=9895
   _PROTECTIONLINK._serialized_start=294
   _PROTECTIONLINK._serialized_end=406
   _CONDITION._serialized_start=409
   _CONDITION._serialized_end=1196
   _CONDITION_RELEASECHANNELSTABLECONDITION._serialized_start=716
   _CONDITION_RELEASECHANNELSTABLECONDITION._serialized_end=883
   _CONDITION_MANUALAPPROVAL._serialized_start=885
@@ -408,61 +419,63 @@
   _CONDITION_CUSTOMTASKSUCCESSFULCONDITION._serialized_start=919
   _CONDITION_CUSTOMTASKSUCCESSFULCONDITION._serialized_end=1183
   _CONDITION_CUSTOMTASKSUCCESSFULCONDITION_PROTECTION._serialized_start=1082
   _CONDITION_CUSTOMTASKSUCCESSFULCONDITION_PROTECTION._serialized_end=1173
   _IDENTIFIER._serialized_start=1198
   _IDENTIFIER._serialized_end=1274
   _METADATA._serialized_start=1277
-  _METADATA._serialized_end=1670
-  _STATUSEXPLANATION._serialized_start=1673
-  _STATUSEXPLANATION._serialized_end=1846
-  _ACTIONEXPLANATION._serialized_start=1849
-  _ACTIONEXPLANATION._serialized_end=1988
-  _VERSION._serialized_start=1991
-  _VERSION._serialized_end=2198
-  _SERVICEINSTANCESTATE._serialized_start=2201
-  _SERVICEINSTANCESTATE._serialized_end=2591
-  _SERVICESTATE._serialized_start=2594
-  _SERVICESTATE._serialized_end=2879
-  _SERVICEGROUPSTATE._serialized_start=2882
-  _SERVICEGROUPSTATE._serialized_end=3092
-  _CANARYPROGRESSSTATE._serialized_start=3095
-  _CANARYPROGRESSSTATE._serialized_end=3391
-  _CANARYPROGRESSSTATE_STATUS._serialized_start=3330
-  _CANARYPROGRESSSTATE_STATUS._serialized_end=3391
-  _DELIVERYSTATE._serialized_start=3394
-  _DELIVERYSTATE._serialized_end=3798
-  _DELIVERYSTATE_STATUS._serialized_start=3637
-  _DELIVERYSTATE_STATUS._serialized_end=3750
-  _RUNTIMEOBJECT._serialized_start=3801
-  _RUNTIMEOBJECT._serialized_end=4312
-  _RUNTIMEOBJECT_STATUS._serialized_start=4242
-  _RUNTIMEOBJECT_STATUS._serialized_end=4290
-  _CONDITIONSTATE._serialized_start=4314
-  _CONDITIONSTATE._serialized_end=4393
-  _CONTROLSTATE._serialized_start=4396
-  _CONTROLSTATE._serialized_end=4746
-  _MANUALAPPROVALSTATE._serialized_start=4749
-  _MANUALAPPROVALSTATE._serialized_end=4907
-  _STATE._serialized_start=4910
-  _STATE._serialized_end=5531
-  _ANNOTATIONS._serialized_start=5534
-  _ANNOTATIONS._serialized_end=5664
-  _ANNOTATIONS_ANNOTATION._serialized_start=5624
-  _ANNOTATIONS_ANNOTATION._serialized_end=5664
-  _CUSTOMTASKEXECUTIONSTATE._serialized_start=5667
-  _CUSTOMTASKEXECUTIONSTATE._serialized_end=5841
-  _CUSTOMTASKSTATE._serialized_start=5844
-  _CUSTOMTASKSTATE._serialized_end=6306
-  _PROTECTIONLINKSTATE._serialized_start=6309
-  _PROTECTIONLINKSTATE._serialized_end=6905
-  _PROTECTIONLINKSTATE_STOPREASON._serialized_start=6767
-  _PROTECTIONLINKSTATE_STOPREASON._serialized_end=6905
-  _PROTECTIONATTACHMENT._serialized_start=6908
-  _PROTECTIONATTACHMENT._serialized_end=7429
-  _SIGNAL._serialized_start=7432
-  _SIGNAL._serialized_end=7654
-  _SIGNAL_DELIVERYPROMOTIONCONFIG._serialized_start=7590
-  _SIGNAL_DELIVERYPROMOTIONCONFIG._serialized_end=7644
-  _DEBUGLOG._serialized_start=7656
-  _DEBUGLOG._serialized_end=7719
+  _METADATA._serialized_end=1616
+  _STATUSEXPLANATION._serialized_start=1619
+  _STATUSEXPLANATION._serialized_end=1792
+  _ACTIONEXPLANATION._serialized_start=1795
+  _ACTIONEXPLANATION._serialized_end=1934
+  _VERSION._serialized_start=1937
+  _VERSION._serialized_end=2144
+  _SERVICEINSTANCESTATE._serialized_start=2147
+  _SERVICEINSTANCESTATE._serialized_end=2537
+  _SERVICESTATE._serialized_start=2540
+  _SERVICESTATE._serialized_end=2825
+  _SERVICEGROUPSTATE._serialized_start=2828
+  _SERVICEGROUPSTATE._serialized_end=3038
+  _CANARYPROGRESSSTATE._serialized_start=3041
+  _CANARYPROGRESSSTATE._serialized_end=3337
+  _CANARYPROGRESSSTATE_STATUS._serialized_start=3276
+  _CANARYPROGRESSSTATE_STATUS._serialized_end=3337
+  _DELIVERYSTATE._serialized_start=3340
+  _DELIVERYSTATE._serialized_end=3744
+  _DELIVERYSTATE_STATUS._serialized_start=3583
+  _DELIVERYSTATE_STATUS._serialized_end=3696
+  _RUNTIMEOBJECT._serialized_start=3747
+  _RUNTIMEOBJECT._serialized_end=4258
+  _RUNTIMEOBJECT_STATUS._serialized_start=4188
+  _RUNTIMEOBJECT_STATUS._serialized_end=4236
+  _CONDITIONSTATE._serialized_start=4260
+  _CONDITIONSTATE._serialized_end=4339
+  _CONTROLSTATE._serialized_start=4342
+  _CONTROLSTATE._serialized_end=4692
+  _MANUALAPPROVALSTATE._serialized_start=4695
+  _MANUALAPPROVALSTATE._serialized_end=4853
+  _STATE._serialized_start=4856
+  _STATE._serialized_end=5561
+  _ANNOTATIONS._serialized_start=5564
+  _ANNOTATIONS._serialized_end=5694
+  _ANNOTATIONS_ANNOTATION._serialized_start=5654
+  _ANNOTATIONS_ANNOTATION._serialized_end=5694
+  _CUSTOMTASKEXECUTIONSTATE._serialized_start=5697
+  _CUSTOMTASKEXECUTIONSTATE._serialized_end=5871
+  _CUSTOMTASKSTATE._serialized_start=5874
+  _CUSTOMTASKSTATE._serialized_end=6336
+  _PROTECTIONLINKSTATE._serialized_start=6339
+  _PROTECTIONLINKSTATE._serialized_end=6935
+  _PROTECTIONLINKSTATE_STOPREASON._serialized_start=6797
+  _PROTECTIONLINKSTATE_STOPREASON._serialized_end=6935
+  _PROTECTIONATTACHMENT._serialized_start=6938
+  _PROTECTIONATTACHMENT._serialized_end=7459
+  _DELIVERYEXTENSIONSTATE._serialized_start=7462
+  _DELIVERYEXTENSIONSTATE._serialized_end=8014
+  _SIGNAL._serialized_start=8017
+  _SIGNAL._serialized_end=8239
+  _SIGNAL_DELIVERYPROMOTIONCONFIG._serialized_start=8175
+  _SIGNAL_DELIVERYPROMOTIONCONFIG._serialized_end=8229
+  _DEBUGLOG._serialized_start=8241
+  _DEBUGLOG._serialized_end=8304
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,49 +34,51 @@
     SERVICE_INSTANCE: _Type.ValueType  # 2
     SERVICE_GROUP: _Type.ValueType  # 3
     RUNTIME_OBJECT: _Type.ValueType  # 4
     MANUAL_APPROVAL: _Type.ValueType  # 5
     CUSTOM_TASK: _Type.ValueType  # 6
     PROTECTION_ATTACHMENT: _Type.ValueType  # 7
     PROTECTION_LINK: _Type.ValueType  # 8
+    DELIVERY_EXTENSION: _Type.ValueType  # 9
 
 class Type(_Type, metaclass=_TypeEnumTypeWrapper): ...
 
 UNKNOWN: Type.ValueType  # 0
 SERVICE: Type.ValueType  # 1
 SERVICE_INSTANCE: Type.ValueType  # 2
 SERVICE_GROUP: Type.ValueType  # 3
 RUNTIME_OBJECT: Type.ValueType  # 4
 MANUAL_APPROVAL: Type.ValueType  # 5
 CUSTOM_TASK: Type.ValueType  # 6
 PROTECTION_ATTACHMENT: Type.ValueType  # 7
 PROTECTION_LINK: Type.ValueType  # 8
+DELIVERY_EXTENSION: Type.ValueType  # 9
 global___Type = Type
 
 class _Lifecycle:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _LifecycleEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_Lifecycle.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     UNKNOWN_LIFECYCLE: _Lifecycle.ValueType  # 0
     CONVERGENCE_START: _Lifecycle.ValueType  # 1
     PRE_APPROVAL: _Lifecycle.ValueType  # 2
     POST_APPROVAL: _Lifecycle.ValueType  # 3
-    PUSH: _Lifecycle.ValueType  # 4
-    POST_PUSH: _Lifecycle.ValueType  # 5
+    DEPLOYMENT: _Lifecycle.ValueType  # 4
+    POST_DEPLOYMENT: _Lifecycle.ValueType  # 5
 
 class Lifecycle(_Lifecycle, metaclass=_LifecycleEnumTypeWrapper): ...
 
 UNKNOWN_LIFECYCLE: Lifecycle.ValueType  # 0
 CONVERGENCE_START: Lifecycle.ValueType  # 1
 PRE_APPROVAL: Lifecycle.ValueType  # 2
 POST_APPROVAL: Lifecycle.ValueType  # 3
-PUSH: Lifecycle.ValueType  # 4
-POST_PUSH: Lifecycle.ValueType  # 5
+DEPLOYMENT: Lifecycle.ValueType  # 4
+POST_DEPLOYMENT: Lifecycle.ValueType  # 5
 global___Lifecycle = Lifecycle
 
 class _CustomTaskType:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _CustomTaskTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_CustomTaskType.ValueType], builtins.type):  # noqa: F821
@@ -84,31 +86,31 @@
     CUSTOM_TASK_TYPE_UNKNOWN: _CustomTaskType.ValueType  # 0
     PRE_APPROVAL_TASK: _CustomTaskType.ValueType  # 1
     """Runs before everything else. May wait for any dependent RCs to be stable."""
     APPROVAL: _CustomTaskType.ValueType  # 2
     """Approval tasks, manual or automated. Must wait for all PRE_APPROVAL_TASK to be satisfied."""
     POST_APPROVAL_TASK: _CustomTaskType.ValueType  # 3
     """Runs after approval, just before service push."""
-    PUSH_TASK: _CustomTaskType.ValueType  # 4
+    DEPLOYMENT_TASK: _CustomTaskType.ValueType  # 4
     """Runs as long as service push is in progress."""
-    POST_PUSH_TASK: _CustomTaskType.ValueType  # 5
+    POST_DEPLOYMENT_TASK: _CustomTaskType.ValueType  # 5
     """Runs after service push succeeds (pods are replaced and healthy, ...), before declaring the service CONVERGED."""
 
 class CustomTaskType(_CustomTaskType, metaclass=_CustomTaskTypeEnumTypeWrapper): ...
 
 CUSTOM_TASK_TYPE_UNKNOWN: CustomTaskType.ValueType  # 0
 PRE_APPROVAL_TASK: CustomTaskType.ValueType  # 1
 """Runs before everything else. May wait for any dependent RCs to be stable."""
 APPROVAL: CustomTaskType.ValueType  # 2
 """Approval tasks, manual or automated. Must wait for all PRE_APPROVAL_TASK to be satisfied."""
 POST_APPROVAL_TASK: CustomTaskType.ValueType  # 3
 """Runs after approval, just before service push."""
-PUSH_TASK: CustomTaskType.ValueType  # 4
+DEPLOYMENT_TASK: CustomTaskType.ValueType  # 4
 """Runs as long as service push is in progress."""
-POST_PUSH_TASK: CustomTaskType.ValueType  # 5
+POST_DEPLOYMENT_TASK: CustomTaskType.ValueType  # 5
 """Runs after service push succeeds (pods are replaced and healthy, ...), before declaring the service CONVERGED."""
 global___CustomTaskType = CustomTaskType
 
 class _Status:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
@@ -467,41 +469,37 @@
 
     PRECONDITIONS_FIELD_NUMBER: builtins.int
     INVARIANTS_FIELD_NUMBER: builtins.int
     SELF_FIELD_NUMBER: builtins.int
     DESIRED_STATE_ID_FIELD_NUMBER: builtins.int
     ROOT_DESIRED_STATE_ID_FIELD_NUMBER: builtins.int
     PROTECTION_LINKS_FIELD_NUMBER: builtins.int
-    PROTECTIONS_FIELD_NUMBER: builtins.int
     @property
     def preconditions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Condition]: ...
     @property
     def invariants(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Condition]: ...
     @property
     def self(self) -> global___Identifier: ...
     desired_state_id: builtins.str
     root_desired_state_id: builtins.str
     @property
     def protection_links(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ProtectionLink]: ...
-    @property
-    def protections(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ProtectionAttachment]: ...
     def __init__(
         # pyright: reportSelfClsParameterName=false
         self_,
         *,
         preconditions: collections.abc.Iterable[global___Condition] | None = ...,
         invariants: collections.abc.Iterable[global___Condition] | None = ...,
         self: global___Identifier | None = ...,
         desired_state_id: builtins.str = ...,
         root_desired_state_id: builtins.str = ...,
         protection_links: collections.abc.Iterable[global___ProtectionLink] | None = ...,
-        protections: collections.abc.Iterable[global___ProtectionAttachment] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["self", b"self"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["desired_state_id", b"desired_state_id", "invariants", b"invariants", "preconditions", b"preconditions", "protection_links", b"protection_links", "protections", b"protections", "root_desired_state_id", b"root_desired_state_id", "self", b"self"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["desired_state_id", b"desired_state_id", "invariants", b"invariants", "preconditions", b"preconditions", "protection_links", b"protection_links", "root_desired_state_id", b"root_desired_state_id", "self", b"self"]) -> None: ...
 
 global___Metadata = Metadata
 
 class StatusExplanation(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SUBJECT_FIELD_NUMBER: builtins.int
@@ -952,14 +950,15 @@
     SERVICE_INSTANCE_FIELD_NUMBER: builtins.int
     SERVICE_GROUP_FIELD_NUMBER: builtins.int
     RUNTIME_OBJECT_FIELD_NUMBER: builtins.int
     MANUAL_APPROVAL_FIELD_NUMBER: builtins.int
     CUSTOM_TASK_FIELD_NUMBER: builtins.int
     PROTECTION_ATTACHMENT_FIELD_NUMBER: builtins.int
     PROTECTION_LINK_FIELD_NUMBER: builtins.int
+    DELIVERY_EXTENSION_FIELD_NUMBER: builtins.int
     @property
     def service(self) -> global___ServiceState: ...
     @property
     def service_instance(self) -> global___ServiceInstanceState: ...
     @property
     def service_group(self) -> global___ServiceGroupState: ...
     @property
@@ -968,29 +967,32 @@
     def manual_approval(self) -> global___ManualApprovalState: ...
     @property
     def custom_task(self) -> global___CustomTaskState: ...
     @property
     def protection_attachment(self) -> global___ProtectionAttachment: ...
     @property
     def protection_link(self) -> global___ProtectionLinkState: ...
+    @property
+    def delivery_extension(self) -> global___DeliveryExtensionState: ...
     def __init__(
         self,
         *,
         service: global___ServiceState | None = ...,
         service_instance: global___ServiceInstanceState | None = ...,
         service_group: global___ServiceGroupState | None = ...,
         runtime_object: global___RuntimeObject | None = ...,
         manual_approval: global___ManualApprovalState | None = ...,
         custom_task: global___CustomTaskState | None = ...,
         protection_attachment: global___ProtectionAttachment | None = ...,
         protection_link: global___ProtectionLinkState | None = ...,
+        delivery_extension: global___DeliveryExtensionState | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["custom_task", b"custom_task", "manual_approval", b"manual_approval", "protection_attachment", b"protection_attachment", "protection_link", b"protection_link", "runtime_object", b"runtime_object", "service", b"service", "service_group", b"service_group", "service_instance", b"service_instance", "state_oneof", b"state_oneof"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["custom_task", b"custom_task", "manual_approval", b"manual_approval", "protection_attachment", b"protection_attachment", "protection_link", b"protection_link", "runtime_object", b"runtime_object", "service", b"service", "service_group", b"service_group", "service_instance", b"service_instance", "state_oneof", b"state_oneof"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["state_oneof", b"state_oneof"]) -> typing_extensions.Literal["service", "service_instance", "service_group", "runtime_object", "manual_approval", "custom_task", "protection_attachment", "protection_link"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["custom_task", b"custom_task", "delivery_extension", b"delivery_extension", "manual_approval", b"manual_approval", "protection_attachment", b"protection_attachment", "protection_link", b"protection_link", "runtime_object", b"runtime_object", "service", b"service", "service_group", b"service_group", "service_instance", b"service_instance", "state_oneof", b"state_oneof"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["custom_task", b"custom_task", "delivery_extension", b"delivery_extension", "manual_approval", b"manual_approval", "protection_attachment", b"protection_attachment", "protection_link", b"protection_link", "runtime_object", b"runtime_object", "service", b"service", "service_group", b"service_group", "service_instance", b"service_instance", "state_oneof", b"state_oneof"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["state_oneof", b"state_oneof"]) -> typing_extensions.Literal["service", "service_instance", "service_group", "runtime_object", "manual_approval", "custom_task", "protection_attachment", "protection_link", "delivery_extension"] | None: ...
 
 global___State = State
 
 class Annotations(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class Annotation(google.protobuf.message.Message):
@@ -1201,14 +1203,59 @@
         attachment_id: builtins.str = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["last_completed_timestamp", b"last_completed_timestamp", "meta", b"meta"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["attachment_id", b"attachment_id", "last_completed_applied_version", b"last_completed_applied_version", "last_completed_status", b"last_completed_status", "last_completed_status_explanations", b"last_completed_status_explanations", "last_completed_timestamp", b"last_completed_timestamp", "last_completed_versions", b"last_completed_versions", "meta", b"meta", "protection_id", b"protection_id", "versions", b"versions"]) -> None: ...
 
 global___ProtectionAttachment = ProtectionAttachment
 
+class DeliveryExtensionState(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    META_FIELD_NUMBER: builtins.int
+    VERSIONS_FIELD_NUMBER: builtins.int
+    EXTENSION_ID_FIELD_NUMBER: builtins.int
+    PROGRAM_FIELD_NUMBER: builtins.int
+    RETRY_CONFIG_FIELD_NUMBER: builtins.int
+    LAST_COMPLETED_TIMESTAMP_FIELD_NUMBER: builtins.int
+    LAST_COMPLETED_STATUS_FIELD_NUMBER: builtins.int
+    LAST_COMPLETED_STATUS_EXPLANATIONS_FIELD_NUMBER: builtins.int
+    LAST_COMPLETED_APPLIED_VERSION_FIELD_NUMBER: builtins.int
+    @property
+    def meta(self) -> global___Metadata: ...
+    @property
+    def versions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Version]: ...
+    extension_id: builtins.str
+    @property
+    def program(self) -> prodvana.proto.prodvana.common_config.program_pb2.ProgramConfig: ...
+    @property
+    def retry_config(self) -> prodvana.proto.prodvana.common_config.retry_pb2.RetryConfig: ...
+    @property
+    def last_completed_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
+    last_completed_status: global___SimpleStatus.ValueType
+    @property
+    def last_completed_status_explanations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___StatusExplanation]: ...
+    last_completed_applied_version: builtins.str
+    def __init__(
+        self,
+        *,
+        meta: global___Metadata | None = ...,
+        versions: collections.abc.Iterable[global___Version] | None = ...,
+        extension_id: builtins.str = ...,
+        program: prodvana.proto.prodvana.common_config.program_pb2.ProgramConfig | None = ...,
+        retry_config: prodvana.proto.prodvana.common_config.retry_pb2.RetryConfig | None = ...,
+        last_completed_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+        last_completed_status: global___SimpleStatus.ValueType = ...,
+        last_completed_status_explanations: collections.abc.Iterable[global___StatusExplanation] | None = ...,
+        last_completed_applied_version: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["last_completed_timestamp", b"last_completed_timestamp", "meta", b"meta", "program", b"program", "retry_config", b"retry_config"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["extension_id", b"extension_id", "last_completed_applied_version", b"last_completed_applied_version", "last_completed_status", b"last_completed_status", "last_completed_status_explanations", b"last_completed_status_explanations", "last_completed_timestamp", b"last_completed_timestamp", "meta", b"meta", "program", b"program", "retry_config", b"retry_config", "versions", b"versions"]) -> None: ...
+
+global___DeliveryExtensionState = DeliveryExtensionState
+
 class Signal(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class DeliveryPromotionConfig(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         STAGE_FIELD_NUMBER: builtins.int
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/entity_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/environment/clusters_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/environment/clusters_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 from prodvana.proto.prodvana.common_config import task_pb2 as prodvana_dot_common__config_dot_task__pb2
+from prodvana.proto.prodvana.common_config import kubernetes_config_pb2 as prodvana_dot_common__config_dot_kubernetes__config__pb2
+from prodvana.proto.prodvana.common_config import parameters_pb2 as prodvana_dot_common__config_dot_parameters__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#prodvana/environment/clusters.proto\x12\x14prodvana.environment\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a!prodvana/common_config/task.proto\"\xe7\x04\n\x0b\x43lusterAuth\x12\x10\n\x08\x65ndpoint\x18\x01 \x01(\t\x12\x0f\n\x07\x63\x61_cert\x18\x02 \x01(\t\x12\r\n\x05token\x18\x03 \x01(\t\x12\x17\n\x0fservice_account\x18\x04 \x01(\t\x12\x38\n\x03\x65\x63s\x18\x05 \x01(\x0b\x32).prodvana.environment.ClusterAuth.ECSAuthH\x00\x12M\n\x0egeneric_docker\x18\x07 \x01(\x0b\x32\x33.prodvana.environment.ClusterAuth.GenericDockerAuthH\x00\x12\x38\n\x03k8s\x18\x08 \x01(\x0b\x32).prodvana.environment.ClusterAuth.K8sAuthH\x00\x12\x16\n\x0ek8s_agent_auth\x18\x06 \x01(\x08\x1ao\n\x07\x45\x43SAuth\x12\x12\n\naccess_key\x18\x01 \x01(\t\x12\x12\n\nsecret_key\x18\x02 \x01(\t\x12\x0e\n\x06region\x18\x03 \x01(\t\x12\x17\n\x0f\x61ssume_role_arn\x18\x04 \x01(\t\x12\x13\n\x0b\x63luster_arn\x18\x05 \x01(\t\x1a*\n\x11GenericDockerAuth\x12\x15\n\rproxy_runtime\x18\x01 \x01(\t\x1a\x86\x01\n\x07K8sAuth\x12J\n\tagent_env\x18\x01 \x03(\x0b\x32\x37.prodvana.environment.ClusterAuth.K8sAuth.AgentEnvEntry\x1a/\n\rAgentEnvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x0c\n\nauth_oneof\"\xe9\x02\n\x07\x43luster\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\ncluster_id\x18\x02 \x01(\t\x12\x34\n\x06origin\x18\x03 \x01(\x0e\x32$.prodvana.environment.Cluster.Origin\x12/\n\x04\x61uth\x18\x04 \x01(\x0b\x32!.prodvana.environment.ClusterAuth\x12/\n\x04type\x18\x05 \x01(\x0e\x32!.prodvana.environment.ClusterType\x12\x33\n\x06\x63onfig\x18\x06 \x01(\x0b\x32#.prodvana.environment.ClusterConfig\x12<\n\x18last_heartbeat_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"1\n\x06Origin\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08PRODVANA\x10\x01\x12\x0c\n\x08\x45XTERNAL\x10\x02\"\xc6\x01\n\x11\x46\x61keClusterConfig\x12Z\n\x11\x63rashing_programs\x18\x01 \x03(\x0b\x32?.prodvana.environment.FakeClusterConfig.CrashingProgramPatterns\x1aU\n\x17\x43rashingProgramPatterns\x12\x13\n\x0bimage_regex\x18\x01 \x01(\t\x12\x11\n\tcmd_regex\x18\x02 \x01(\t\x12\x12\n\nlog_output\x18\x03 \x01(\t\"H\n\x14GenericDockerCommand\x12\x30\n\x04task\x18\x01 \x01(\x0b\x32\".prodvana.common_config.TaskConfig\"\x9e\x01\n\x1aGenericDockerClusterConfig\x12\x39\n\x05\x61pply\x18\x01 \x01(\x0b\x32*.prodvana.environment.GenericDockerCommand\x12\x45\n\x11get_current_state\x18\x02 \x01(\x0b\x32*.prodvana.environment.GenericDockerCommand\"\xc9\x0c\n\rClusterConfig\x12\x0c\n\x04name\x18\x0e \x01(\t\x12\x17\n\x0f\x64isable_flagger\x18\x01 \x01(\x08\x12\x15\n\rdisable_istio\x18\x02 \x01(\x08\x12>\n\x08kubecost\x18\x03 \x01(\x0b\x32,.prodvana.environment.ClusterConfig.Kubecost\x12<\n\x07\x64\x61tadog\x18\x04 \x01(\x0b\x32+.prodvana.environment.ClusterConfig.Datadog\x12\x43\n\x0b\x61lb_ingress\x18\x06 \x01(\x0b\x32..prodvana.environment.ClusterConfig.ALBIngress\x12G\n\rargo_rollouts\x18\x07 \x01(\x0b\x32\x30.prodvana.environment.ClusterConfig.ArgoRollouts\x12\x43\n\x0bgke_ingress\x18\x08 \x01(\x0b\x32..prodvana.environment.ClusterConfig.GKEIngress\x12P\n\x18self_managed_gke_ingress\x18\x0b \x01(\x0b\x32..prodvana.environment.ClusterConfig.GKEIngress\x12I\n\x0e\x63loud_provider\x18\t \x01(\x0e\x32\x31.prodvana.environment.ClusterConfig.CloudProvider\x12\x37\n\x04\x66\x61ke\x18\n \x01(\x0b\x32\'.prodvana.environment.FakeClusterConfigH\x00\x12J\n\x0egeneric_docker\x18\x0c \x01(\x0b\x32\x30.prodvana.environment.GenericDockerClusterConfigH\x00\x1aH\n\x08Kubecost\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07managed\x18\x02 \x01(\x08\x12\x1a\n\x12kubecost_namespace\x18\x03 \x01(\t\x1a\x65\n\x07\x44\x61tadog\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07managed\x18\x02 \x01(\x08\x12\x19\n\x11\x64\x61tadog_namespace\x18\x03 \x01(\t\x12\x0f\n\x07\x61pi_key\x18\x04 \x01(\t\x12\x0c\n\x04site\x18\x05 \x01(\t\x1a\x62\n\nALBIngress\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1e\n\ringress_class\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12#\n\x1b\x64\x65\x66\x61ult_balancer_attributes\x18\x03 \x03(\t\x1a\xba\x03\n\x0c\x41rgoRollouts\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12T\n\ttemplates\x18\x02 \x03(\x0b\x32\x41.prodvana.environment.ClusterConfig.ArgoRollouts.AnalysisTemplate\x1a\xc2\x02\n\x10\x41nalysisTemplate\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x66\n\x0b\x61rg_mapping\x18\x02 \x03(\x0b\x32Q.prodvana.environment.ClusterConfig.ArgoRollouts.AnalysisTemplate.ArgMappingEntry\x1a}\n\x0f\x41rgMappingEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12Y\n\x05value\x18\x02 \x01(\x0e\x32J.prodvana.environment.ClusterConfig.ArgoRollouts.AnalysisTemplate.ArgValue:\x02\x38\x01\"9\n\x08\x41rgValue\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVICE\x10\x01\x12\x13\n\x0fRELEASE_CHANNEL\x10\x02\x1a\x37\n\nGKEIngress\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x18\n\x10\x63ontainer_native\x18\x02 \x01(\x08\"T\n\rCloudProvider\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03\x45KS\x10\x01\x12\x07\n\x03GKE\x10\x02\x12\x07\n\x03\x41KS\x10\x03\x12\n\n\x06ONPREM\x10\x04\x12\x0f\n\x0bOTHER_CLOUD\x10\x05\x42\x0f\n\rcluster_oneofJ\x04\x08\x05\x10\x06R\x0f\x61ws_alb_ingress*J\n\x0b\x43lusterType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03K8S\x10\x01\x12\x07\n\x03\x45\x43S\x10\x02\x12\x08\n\x04\x46\x41KE\x10\x03\x12\x12\n\x0eGENERIC_DOCKER\x10\x04\x42PZNgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/environmentb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#prodvana/environment/clusters.proto\x12\x14prodvana.environment\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a!prodvana/common_config/task.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a\'prodvana/common_config/parameters.proto\"\xe7\x04\n\x0b\x43lusterAuth\x12\x10\n\x08\x65ndpoint\x18\x01 \x01(\t\x12\x0f\n\x07\x63\x61_cert\x18\x02 \x01(\t\x12\r\n\x05token\x18\x03 \x01(\t\x12\x17\n\x0fservice_account\x18\x04 \x01(\t\x12\x38\n\x03\x65\x63s\x18\x05 \x01(\x0b\x32).prodvana.environment.ClusterAuth.ECSAuthH\x00\x12M\n\x0egeneric_docker\x18\x07 \x01(\x0b\x32\x33.prodvana.environment.ClusterAuth.GenericDockerAuthH\x00\x12\x38\n\x03k8s\x18\x08 \x01(\x0b\x32).prodvana.environment.ClusterAuth.K8sAuthH\x00\x12\x16\n\x0ek8s_agent_auth\x18\x06 \x01(\x08\x1ao\n\x07\x45\x43SAuth\x12\x12\n\naccess_key\x18\x01 \x01(\t\x12\x12\n\nsecret_key\x18\x02 \x01(\t\x12\x0e\n\x06region\x18\x03 \x01(\t\x12\x17\n\x0f\x61ssume_role_arn\x18\x04 \x01(\t\x12\x13\n\x0b\x63luster_arn\x18\x05 \x01(\t\x1a*\n\x11GenericDockerAuth\x12\x15\n\rproxy_runtime\x18\x01 \x01(\t\x1a\x86\x01\n\x07K8sAuth\x12J\n\tagent_env\x18\x01 \x03(\x0b\x32\x37.prodvana.environment.ClusterAuth.K8sAuth.AgentEnvEntry\x1a/\n\rAgentEnvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x0c\n\nauth_oneof\"\xe9\x02\n\x07\x43luster\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x12\n\ncluster_id\x18\x02 \x01(\t\x12\x34\n\x06origin\x18\x03 \x01(\x0e\x32$.prodvana.environment.Cluster.Origin\x12/\n\x04\x61uth\x18\x04 \x01(\x0b\x32!.prodvana.environment.ClusterAuth\x12/\n\x04type\x18\x05 \x01(\x0e\x32!.prodvana.environment.ClusterType\x12\x33\n\x06\x63onfig\x18\x06 \x01(\x0b\x32#.prodvana.environment.ClusterConfig\x12<\n\x18last_heartbeat_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"1\n\x06Origin\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08PRODVANA\x10\x01\x12\x0c\n\x08\x45XTERNAL\x10\x02\"\xc6\x01\n\x11\x46\x61keClusterConfig\x12Z\n\x11\x63rashing_programs\x18\x01 \x03(\x0b\x32?.prodvana.environment.FakeClusterConfig.CrashingProgramPatterns\x1aU\n\x17\x43rashingProgramPatterns\x12\x13\n\x0bimage_regex\x18\x01 \x01(\t\x12\x11\n\tcmd_regex\x18\x02 \x01(\t\x12\x12\n\nlog_output\x18\x03 \x01(\t\"\xac\x01\n\x14GenericDockerCommand\x12\x39\n\x0btask_config\x18\x01 \x01(\x0b\x32\".prodvana.common_config.TaskConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x02 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x42\x12\n\x0b\x65xec_config\x12\x03\xf8\x42\x01\"\xf8\x01\n\x1aGenericDockerClusterConfig\x12\x43\n\x05\x61pply\x18\x01 \x01(\x0b\x32*.prodvana.environment.GenericDockerCommandB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x45\n\x11get_current_state\x18\x02 \x01(\x0b\x32*.prodvana.environment.GenericDockerCommand\x12N\n\nparameters\x18\x03 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\"\xc9\x0c\n\rClusterConfig\x12\x0c\n\x04name\x18\x0e \x01(\t\x12\x17\n\x0f\x64isable_flagger\x18\x01 \x01(\x08\x12\x15\n\rdisable_istio\x18\x02 \x01(\x08\x12>\n\x08kubecost\x18\x03 \x01(\x0b\x32,.prodvana.environment.ClusterConfig.Kubecost\x12<\n\x07\x64\x61tadog\x18\x04 \x01(\x0b\x32+.prodvana.environment.ClusterConfig.Datadog\x12\x43\n\x0b\x61lb_ingress\x18\x06 \x01(\x0b\x32..prodvana.environment.ClusterConfig.ALBIngress\x12G\n\rargo_rollouts\x18\x07 \x01(\x0b\x32\x30.prodvana.environment.ClusterConfig.ArgoRollouts\x12\x43\n\x0bgke_ingress\x18\x08 \x01(\x0b\x32..prodvana.environment.ClusterConfig.GKEIngress\x12P\n\x18self_managed_gke_ingress\x18\x0b \x01(\x0b\x32..prodvana.environment.ClusterConfig.GKEIngress\x12I\n\x0e\x63loud_provider\x18\t \x01(\x0e\x32\x31.prodvana.environment.ClusterConfig.CloudProvider\x12\x37\n\x04\x66\x61ke\x18\n \x01(\x0b\x32\'.prodvana.environment.FakeClusterConfigH\x00\x12J\n\x0egeneric_docker\x18\x0c \x01(\x0b\x32\x30.prodvana.environment.GenericDockerClusterConfigH\x00\x1aH\n\x08Kubecost\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07managed\x18\x02 \x01(\x08\x12\x1a\n\x12kubecost_namespace\x18\x03 \x01(\t\x1a\x65\n\x07\x44\x61tadog\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07managed\x18\x02 \x01(\x08\x12\x19\n\x11\x64\x61tadog_namespace\x18\x03 \x01(\t\x12\x0f\n\x07\x61pi_key\x18\x04 \x01(\t\x12\x0c\n\x04site\x18\x05 \x01(\t\x1a\x62\n\nALBIngress\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1e\n\ringress_class\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12#\n\x1b\x64\x65\x66\x61ult_balancer_attributes\x18\x03 \x03(\t\x1a\xba\x03\n\x0c\x41rgoRollouts\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12T\n\ttemplates\x18\x02 \x03(\x0b\x32\x41.prodvana.environment.ClusterConfig.ArgoRollouts.AnalysisTemplate\x1a\xc2\x02\n\x10\x41nalysisTemplate\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x66\n\x0b\x61rg_mapping\x18\x02 \x03(\x0b\x32Q.prodvana.environment.ClusterConfig.ArgoRollouts.AnalysisTemplate.ArgMappingEntry\x1a}\n\x0f\x41rgMappingEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12Y\n\x05value\x18\x02 \x01(\x0e\x32J.prodvana.environment.ClusterConfig.ArgoRollouts.AnalysisTemplate.ArgValue:\x02\x38\x01\"9\n\x08\x41rgValue\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVICE\x10\x01\x12\x13\n\x0fRELEASE_CHANNEL\x10\x02\x1a\x37\n\nGKEIngress\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x18\n\x10\x63ontainer_native\x18\x02 \x01(\x08\"T\n\rCloudProvider\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03\x45KS\x10\x01\x12\x07\n\x03GKE\x10\x02\x12\x07\n\x03\x41KS\x10\x03\x12\n\n\x06ONPREM\x10\x04\x12\x0f\n\x0bOTHER_CLOUD\x10\x05\x42\x0f\n\rcluster_oneofJ\x04\x08\x05\x10\x06R\x0f\x61ws_alb_ingress*J\n\x0b\x43lusterType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x07\n\x03K8S\x10\x01\x12\x07\n\x03\x45\x43S\x10\x02\x12\x08\n\x04\x46\x41KE\x10\x03\x12\x12\n\x0eGENERIC_DOCKER\x10\x04\x42PZNgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/environmentb\x06proto3')
 
 _CLUSTERTYPE = DESCRIPTOR.enum_types_by_name['ClusterType']
 ClusterType = enum_type_wrapper.EnumTypeWrapper(_CLUSTERTYPE)
 UNKNOWN = 0
 K8S = 1
 ECS = 2
 FAKE = 3
@@ -190,56 +192,62 @@
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZNgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/environment'
   _CLUSTERAUTH_K8SAUTH_AGENTENVENTRY._options = None
   _CLUSTERAUTH_K8SAUTH_AGENTENVENTRY._serialized_options = b'8\001'
+  _GENERICDOCKERCOMMAND.oneofs_by_name['exec_config']._options = None
+  _GENERICDOCKERCOMMAND.oneofs_by_name['exec_config']._serialized_options = b'\370B\001'
+  _GENERICDOCKERCLUSTERCONFIG.fields_by_name['apply']._options = None
+  _GENERICDOCKERCLUSTERCONFIG.fields_by_name['apply']._serialized_options = b'\372B\005\212\001\002\020\001'
+  _GENERICDOCKERCLUSTERCONFIG.fields_by_name['parameters']._options = None
+  _GENERICDOCKERCLUSTERCONFIG.fields_by_name['parameters']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
   _CLUSTERCONFIG_ALBINGRESS.fields_by_name['ingress_class']._options = None
   _CLUSTERCONFIG_ALBINGRESS.fields_by_name['ingress_class']._serialized_options = b'\372B\004r\002\020\001'
   _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGMAPPINGENTRY._options = None
   _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGMAPPINGENTRY._serialized_options = b'8\001'
-  _CLUSTERTYPE._serialized_start=3184
-  _CLUSTERTYPE._serialized_end=3258
-  _CLUSTERAUTH._serialized_start=155
-  _CLUSTERAUTH._serialized_end=770
-  _CLUSTERAUTH_ECSAUTH._serialized_start=464
-  _CLUSTERAUTH_ECSAUTH._serialized_end=575
-  _CLUSTERAUTH_GENERICDOCKERAUTH._serialized_start=577
-  _CLUSTERAUTH_GENERICDOCKERAUTH._serialized_end=619
-  _CLUSTERAUTH_K8SAUTH._serialized_start=622
-  _CLUSTERAUTH_K8SAUTH._serialized_end=756
-  _CLUSTERAUTH_K8SAUTH_AGENTENVENTRY._serialized_start=709
-  _CLUSTERAUTH_K8SAUTH_AGENTENVENTRY._serialized_end=756
-  _CLUSTER._serialized_start=773
-  _CLUSTER._serialized_end=1134
-  _CLUSTER_ORIGIN._serialized_start=1085
-  _CLUSTER_ORIGIN._serialized_end=1134
-  _FAKECLUSTERCONFIG._serialized_start=1137
-  _FAKECLUSTERCONFIG._serialized_end=1335
-  _FAKECLUSTERCONFIG_CRASHINGPROGRAMPATTERNS._serialized_start=1250
-  _FAKECLUSTERCONFIG_CRASHINGPROGRAMPATTERNS._serialized_end=1335
-  _GENERICDOCKERCOMMAND._serialized_start=1337
-  _GENERICDOCKERCOMMAND._serialized_end=1409
-  _GENERICDOCKERCLUSTERCONFIG._serialized_start=1412
-  _GENERICDOCKERCLUSTERCONFIG._serialized_end=1570
-  _CLUSTERCONFIG._serialized_start=1573
-  _CLUSTERCONFIG._serialized_end=3182
-  _CLUSTERCONFIG_KUBECOST._serialized_start=2279
-  _CLUSTERCONFIG_KUBECOST._serialized_end=2351
-  _CLUSTERCONFIG_DATADOG._serialized_start=2353
-  _CLUSTERCONFIG_DATADOG._serialized_end=2454
-  _CLUSTERCONFIG_ALBINGRESS._serialized_start=2456
-  _CLUSTERCONFIG_ALBINGRESS._serialized_end=2554
-  _CLUSTERCONFIG_ARGOROLLOUTS._serialized_start=2557
-  _CLUSTERCONFIG_ARGOROLLOUTS._serialized_end=2999
-  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE._serialized_start=2677
-  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE._serialized_end=2999
-  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGMAPPINGENTRY._serialized_start=2815
-  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGMAPPINGENTRY._serialized_end=2940
-  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGVALUE._serialized_start=2942
-  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGVALUE._serialized_end=2999
-  _CLUSTERCONFIG_GKEINGRESS._serialized_start=3001
-  _CLUSTERCONFIG_GKEINGRESS._serialized_end=3056
-  _CLUSTERCONFIG_CLOUDPROVIDER._serialized_start=3058
-  _CLUSTERCONFIG_CLOUDPROVIDER._serialized_end=3142
+  _CLUSTERTYPE._serialized_start=3464
+  _CLUSTERTYPE._serialized_end=3538
+  _CLUSTERAUTH._serialized_start=244
+  _CLUSTERAUTH._serialized_end=859
+  _CLUSTERAUTH_ECSAUTH._serialized_start=553
+  _CLUSTERAUTH_ECSAUTH._serialized_end=664
+  _CLUSTERAUTH_GENERICDOCKERAUTH._serialized_start=666
+  _CLUSTERAUTH_GENERICDOCKERAUTH._serialized_end=708
+  _CLUSTERAUTH_K8SAUTH._serialized_start=711
+  _CLUSTERAUTH_K8SAUTH._serialized_end=845
+  _CLUSTERAUTH_K8SAUTH_AGENTENVENTRY._serialized_start=798
+  _CLUSTERAUTH_K8SAUTH_AGENTENVENTRY._serialized_end=845
+  _CLUSTER._serialized_start=862
+  _CLUSTER._serialized_end=1223
+  _CLUSTER_ORIGIN._serialized_start=1174
+  _CLUSTER_ORIGIN._serialized_end=1223
+  _FAKECLUSTERCONFIG._serialized_start=1226
+  _FAKECLUSTERCONFIG._serialized_end=1424
+  _FAKECLUSTERCONFIG_CRASHINGPROGRAMPATTERNS._serialized_start=1339
+  _FAKECLUSTERCONFIG_CRASHINGPROGRAMPATTERNS._serialized_end=1424
+  _GENERICDOCKERCOMMAND._serialized_start=1427
+  _GENERICDOCKERCOMMAND._serialized_end=1599
+  _GENERICDOCKERCLUSTERCONFIG._serialized_start=1602
+  _GENERICDOCKERCLUSTERCONFIG._serialized_end=1850
+  _CLUSTERCONFIG._serialized_start=1853
+  _CLUSTERCONFIG._serialized_end=3462
+  _CLUSTERCONFIG_KUBECOST._serialized_start=2559
+  _CLUSTERCONFIG_KUBECOST._serialized_end=2631
+  _CLUSTERCONFIG_DATADOG._serialized_start=2633
+  _CLUSTERCONFIG_DATADOG._serialized_end=2734
+  _CLUSTERCONFIG_ALBINGRESS._serialized_start=2736
+  _CLUSTERCONFIG_ALBINGRESS._serialized_end=2834
+  _CLUSTERCONFIG_ARGOROLLOUTS._serialized_start=2837
+  _CLUSTERCONFIG_ARGOROLLOUTS._serialized_end=3279
+  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE._serialized_start=2957
+  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE._serialized_end=3279
+  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGMAPPINGENTRY._serialized_start=3095
+  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGMAPPINGENTRY._serialized_end=3220
+  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGVALUE._serialized_start=3222
+  _CLUSTERCONFIG_ARGOROLLOUTS_ANALYSISTEMPLATE_ARGVALUE._serialized_end=3279
+  _CLUSTERCONFIG_GKEINGRESS._serialized_start=3281
+  _CLUSTERCONFIG_GKEINGRESS._serialized_end=3336
+  _CLUSTERCONFIG_CLOUDPROVIDER._serialized_start=3338
+  _CLUSTERCONFIG_CLOUDPROVIDER._serialized_end=3422
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/environment/clusters_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/environment/clusters_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import google.protobuf.timestamp_pb2
+import prodvana.proto.prodvana.common_config.kubernetes_config_pb2
+import prodvana.proto.prodvana.common_config.parameters_pb2
 import prodvana.proto.prodvana.common_config.task_pb2
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
@@ -234,44 +236,53 @@
     def ClearField(self, field_name: typing_extensions.Literal["crashing_programs", b"crashing_programs"]) -> None: ...
 
 global___FakeClusterConfig = FakeClusterConfig
 
 class GenericDockerCommand(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    TASK_FIELD_NUMBER: builtins.int
+    TASK_CONFIG_FIELD_NUMBER: builtins.int
+    KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
     @property
-    def task(self) -> prodvana.proto.prodvana.common_config.task_pb2.TaskConfig: ...
+    def task_config(self) -> prodvana.proto.prodvana.common_config.task_pb2.TaskConfig: ...
+    @property
+    def kubernetes_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig: ...
     def __init__(
         self,
         *,
-        task: prodvana.proto.prodvana.common_config.task_pb2.TaskConfig | None = ...,
+        task_config: prodvana.proto.prodvana.common_config.task_pb2.TaskConfig | None = ...,
+        kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["task", b"task"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["task", b"task"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "kubernetes_config", b"kubernetes_config", "task_config", b"task_config"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "kubernetes_config", b"kubernetes_config", "task_config", b"task_config"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["exec_config", b"exec_config"]) -> typing_extensions.Literal["task_config", "kubernetes_config"] | None: ...
 
 global___GenericDockerCommand = GenericDockerCommand
 
 class GenericDockerClusterConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     APPLY_FIELD_NUMBER: builtins.int
     GET_CURRENT_STATE_FIELD_NUMBER: builtins.int
+    PARAMETERS_FIELD_NUMBER: builtins.int
     @property
     def apply(self) -> global___GenericDockerCommand: ...
     @property
     def get_current_state(self) -> global___GenericDockerCommand: ...
+    @property
+    def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition]: ...
     def __init__(
         self,
         *,
         apply: global___GenericDockerCommand | None = ...,
         get_current_state: global___GenericDockerCommand | None = ...,
+        parameters: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["apply", b"apply", "get_current_state", b"get_current_state"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["apply", b"apply", "get_current_state", b"get_current_state"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["apply", b"apply", "get_current_state", b"get_current_state", "parameters", b"parameters"]) -> None: ...
 
 global___GenericDockerClusterConfig = GenericDockerClusterConfig
 
 class ClusterConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _CloudProvider:
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/environment/environment_manager_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/environment/environment_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py` & `prodvana-0.1.5/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/events/events_manager_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/events/events_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/events/events_manager_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/events/events_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py` & `prodvana-0.1.5/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/events/events_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/events/events_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/events/events_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/events/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/events/types_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/events/types_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/events/types_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/events/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/insights/insights_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/insights/insights_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/insights/insights_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/insights/insights_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/managed_resource/manager_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/managed_resource/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py` & `prodvana-0.1.5/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/metrics/metrics_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/metrics/metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/metrics/metrics_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/metrics/metrics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/object/meta_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/version/source_metadata_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: prodvana/object/meta.proto
+# source: prodvana/version/source_metadata.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from prodvana.proto.prodvana.version import source_metadata_pb2 as prodvana_dot_version_dot_source__metadata__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aprodvana/object/meta.proto\x12\x0fprodvana.object\x1a&prodvana/version/source_metadata.proto\"\xb4\x01\n\nObjectMeta\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x16\n\x0e\x63onfig_version\x18\x04 \x01(\t\x12(\n\x06source\x18\x05 \x01(\x0e\x32\x18.prodvana.version.Source\x12\x39\n\x0fsource_metadata\x18\x06 \x01(\x0b\x32 .prodvana.version.SourceMetadataBKZIgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/objectb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&prodvana/version/source_metadata.proto\x12\x10prodvana.version\"V\n\x0eSourceMetadata\x12\x10\n\x08repo_url\x18\x01 \x01(\t\x12\x11\n\tfile_path\x18\x02 \x01(\t\x12\x0e\n\x06\x63ommit\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t*m\n\x06Source\x12\x12\n\x0eUNKNOWN_SOURCE\x10\x00\x12\x07\n\x03WEB\x10\x01\x12\x16\n\x12INTERACTIVE_PVNCTL\x10\x02\x12\x0f\n\x0b\x43ONFIG_FILE\x10\x03\x12\x0f\n\x0bREPO_FOLLOW\x10\x04\x12\x0c\n\x08PRODVANA\x10\x05\x42LZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/versionb\x06proto3')
 
-
-
-_OBJECTMETA = DESCRIPTOR.message_types_by_name['ObjectMeta']
-ObjectMeta = _reflection.GeneratedProtocolMessageType('ObjectMeta', (_message.Message,), {
-  'DESCRIPTOR' : _OBJECTMETA,
-  '__module__' : 'prodvana.object.meta_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.object.ObjectMeta)
+_SOURCE = DESCRIPTOR.enum_types_by_name['Source']
+Source = enum_type_wrapper.EnumTypeWrapper(_SOURCE)
+UNKNOWN_SOURCE = 0
+WEB = 1
+INTERACTIVE_PVNCTL = 2
+CONFIG_FILE = 3
+REPO_FOLLOW = 4
+PRODVANA = 5
+
+
+_SOURCEMETADATA = DESCRIPTOR.message_types_by_name['SourceMetadata']
+SourceMetadata = _reflection.GeneratedProtocolMessageType('SourceMetadata', (_message.Message,), {
+  'DESCRIPTOR' : _SOURCEMETADATA,
+  '__module__' : 'prodvana.version.source_metadata_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.version.SourceMetadata)
   })
-_sym_db.RegisterMessage(ObjectMeta)
+_sym_db.RegisterMessage(SourceMetadata)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZIgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/object'
-  _OBJECTMETA._serialized_start=88
-  _OBJECTMETA._serialized_end=268
+  DESCRIPTOR._serialized_options = b'ZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/version'
+  _SOURCE._serialized_start=148
+  _SOURCE._serialized_end=257
+  _SOURCEMETADATA._serialized_start=60
+  _SOURCEMETADATA._serialized_end=146
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/object/meta_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/object/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/organization/organization_manager_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/organization/organization_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py` & `prodvana-0.1.5/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/organization/user_metadata_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/organization/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/pipelines/object_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_config_pb2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,105 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: prodvana/pipelines/object.proto
+# source: prodvana/protection/protection_config.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from prodvana.proto.prodvana.pipelines import pipelines_pb2 as prodvana_dot_pipelines_dot_pipelines__pb2
-from prodvana.proto.prodvana.common_config import meta_pb2 as prodvana_dot_common__config_dot_meta__pb2
-from prodvana.proto.prodvana.common_config import version_push_pb2 as prodvana_dot_common__config_dot_version__push__pb2
-from prodvana.proto.prodvana.object import meta_pb2 as prodvana_dot_object_dot_meta__pb2
-
-
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fprodvana/pipelines/object.proto\x12\x12prodvana.pipelines\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\"prodvana/pipelines/pipelines.proto\x1a!prodvana/common_config/meta.proto\x1a)prodvana/common_config/version_push.proto\x1a\x1aprodvana/object/meta.proto\"y\n\x10ServicePushParam\x12\x0f\n\x07service\x18\x01 \x01(\t\x12?\n\x0cversion_push\x18\x02 \x01(\x0b\x32).prodvana.common_config.VersionPushOption\x12\x13\n\x0b\x61pplication\x18\x03 \x01(\t\"\xb6\x01\n\x13ServiceInstancePush\x12\x35\n\x10\x61pplication_meta\x18\x01 \x01(\x0b\x32\x1b.prodvana.object.ObjectMeta\x12P\n\x15service_instance_meta\x18\x02 \x01(\x0b\x32\x31.prodvana.common_config.ServiceInstanceObjectMeta\x12\x16\n\x0etarget_version\x18\x03 \x01(\t\"\x9a\x01\n\nTaskStatus\x12\n\n\x02id\x18\x01 \x01(\x05\x12\r\n\x05state\x18\x02 \x01(\t\x12\x36\n\x12\x63reation_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x15last_update_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x0f\n\rPipelineState\"\x9b\x01\n\x08Pipeline\x12)\n\x04meta\x18\x01 \x01(\x0b\x32\x1b.prodvana.object.ObjectMeta\x12\x32\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\".prodvana.pipelines.PipelineConfig\x12\x30\n\x05state\x18\x03 \x01(\x0b\x32!.prodvana.pipelines.PipelineState\"\x9a\x02\n\x11PipelineRunConfig\x12;\n\x0fpipeline_config\x18\x01 \x01(\x0b\x32\".prodvana.pipelines.PipelineConfig\x12\x41\n\x13service_push_params\x18\x02 \x03(\x0b\x32$.prodvana.pipelines.ServicePushParam\x12 \n\x18skip_rollback_validation\x18\x03 \x01(\x08\x12H\n\x17service_instance_pushes\x18\x04 \x03(\x0b\x32\'.prodvana.pipelines.ServiceInstancePush\x12\x19\n\x11skip_alert_checks\x18\x05 \x01(\x08\"\xbb\x02\n\x10PipelineRunState\x12\x36\n\x12\x63reation_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x15last_update_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05state\x18\x03 \x01(\t\x12\x10\n\x08terminal\x18\x04 \x01(\x08\x12\x35\n\rtask_statuses\x18\x05 \x03(\x0b\x32\x1e.prodvana.pipelines.TaskStatus\x12\x11\n\tlastActor\x18\x06 \x01(\t\x12\x11\n\tinitiator\x18\x07 \x01(\t\x12\x0e\n\x06reason\x18\x08 \x01(\t\x12\x0f\n\x07message\x18\t \x01(\t\x12\x15\n\rexternal_link\x18\n \x01(\t\"\xb6\x01\n\x0bPipelineRun\x12;\n\x04meta\x18\x01 \x01(\x0b\x32-.prodvana.common_config.PipelineRunObjectMeta\x12\x35\n\x06\x63onfig\x18\x02 \x01(\x0b\x32%.prodvana.pipelines.PipelineRunConfig\x12\x33\n\x05state\x18\x03 \x01(\x0b\x32$.prodvana.pipelines.PipelineRunStateBNZLgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/pipelinesb\x06proto3')
+from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
+from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
+from prodvana.proto.prodvana.common_config import task_pb2 as prodvana_dot_common__config_dot_task__pb2
+from prodvana.proto.prodvana.common_config import env_pb2 as prodvana_dot_common__config_dot_env__pb2
+from prodvana.proto.prodvana.common_config import kubernetes_config_pb2 as prodvana_dot_common__config_dot_kubernetes__config__pb2
+from prodvana.proto.prodvana.common_config import parameters_pb2 as prodvana_dot_common__config_dot_parameters__pb2
+from prodvana.proto.prodvana.runtimes import runtimes_config_pb2 as prodvana_dot_runtimes_dot_runtimes__config__pb2
+
+
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+prodvana/protection/protection_config.proto\x12\x13prodvana.protection\x1a\x1egoogle/protobuf/duration.proto\x1a\x17validate/validate.proto\x1a!prodvana/common_config/task.proto\x1a prodvana/common_config/env.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a\'prodvana/common_config/parameters.proto\x1a\'prodvana/runtimes/runtimes_config.proto\"\x91\x03\n\x10ProtectionConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\x39\n\x0btask_config\x18\x02 \x01(\x0b\x32\".prodvana.common_config.TaskConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x03 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x30\n\rpoll_interval\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\x12*\n\x07timeout\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12N\n\nparameters\x18\x06 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x42\x12\n\x0b\x65xec_config\x12\x03\xf8\x42\x01\"\xe8\x03\n\"CompiledProtectionAttachmentConfig\x12\x35\n\x06\x63onfig\x18\x01 \x01(\x0b\x32%.prodvana.protection.ProtectionConfig\x12=\n\nattachment\x18\x02 \x01(\x0b\x32).prodvana.protection.ProtectionAttachment\x12\x44\n\x11runtime_execution\x18\x03 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12v\n\x03\x65nv\x18\x04 \x03(\x0b\x32@.prodvana.protection.CompiledProtectionAttachmentConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x12@\n\x10parameter_values\x18\x05 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\"Z\n\x19ServiceInstanceAttachment\x12\x0f\n\x07service\x18\x01 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x13\n\x0b\x61pplication\x18\x03 \x01(\t\"H\n\x18ReleaseChannelAttachment\x12\x13\n\x0b\x61pplication\x18\x01 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\"\xbf\x01\n\x14ProtectionAttachment\x12J\n\x10service_instance\x18\x01 \x01(\x0b\x32..prodvana.protection.ServiceInstanceAttachmentH\x00\x12H\n\x0frelease_channel\x18\x02 \x01(\x0b\x32-.prodvana.protection.ReleaseChannelAttachmentH\x00\x42\x11\n\nattachment\x12\x03\xf8\x42\x01\x42OZMgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/protectionb\x06proto3')
 
 
 
-_SERVICEPUSHPARAM = DESCRIPTOR.message_types_by_name['ServicePushParam']
-_SERVICEINSTANCEPUSH = DESCRIPTOR.message_types_by_name['ServiceInstancePush']
-_TASKSTATUS = DESCRIPTOR.message_types_by_name['TaskStatus']
-_PIPELINESTATE = DESCRIPTOR.message_types_by_name['PipelineState']
-_PIPELINE = DESCRIPTOR.message_types_by_name['Pipeline']
-_PIPELINERUNCONFIG = DESCRIPTOR.message_types_by_name['PipelineRunConfig']
-_PIPELINERUNSTATE = DESCRIPTOR.message_types_by_name['PipelineRunState']
-_PIPELINERUN = DESCRIPTOR.message_types_by_name['PipelineRun']
-ServicePushParam = _reflection.GeneratedProtocolMessageType('ServicePushParam', (_message.Message,), {
-  'DESCRIPTOR' : _SERVICEPUSHPARAM,
-  '__module__' : 'prodvana.pipelines.object_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.pipelines.ServicePushParam)
+_PROTECTIONCONFIG = DESCRIPTOR.message_types_by_name['ProtectionConfig']
+_COMPILEDPROTECTIONATTACHMENTCONFIG = DESCRIPTOR.message_types_by_name['CompiledProtectionAttachmentConfig']
+_COMPILEDPROTECTIONATTACHMENTCONFIG_ENVENTRY = _COMPILEDPROTECTIONATTACHMENTCONFIG.nested_types_by_name['EnvEntry']
+_SERVICEINSTANCEATTACHMENT = DESCRIPTOR.message_types_by_name['ServiceInstanceAttachment']
+_RELEASECHANNELATTACHMENT = DESCRIPTOR.message_types_by_name['ReleaseChannelAttachment']
+_PROTECTIONATTACHMENT = DESCRIPTOR.message_types_by_name['ProtectionAttachment']
+ProtectionConfig = _reflection.GeneratedProtocolMessageType('ProtectionConfig', (_message.Message,), {
+  'DESCRIPTOR' : _PROTECTIONCONFIG,
+  '__module__' : 'prodvana.protection.protection_config_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.protection.ProtectionConfig)
+  })
+_sym_db.RegisterMessage(ProtectionConfig)
+
+CompiledProtectionAttachmentConfig = _reflection.GeneratedProtocolMessageType('CompiledProtectionAttachmentConfig', (_message.Message,), {
+
+  'EnvEntry' : _reflection.GeneratedProtocolMessageType('EnvEntry', (_message.Message,), {
+    'DESCRIPTOR' : _COMPILEDPROTECTIONATTACHMENTCONFIG_ENVENTRY,
+    '__module__' : 'prodvana.protection.protection_config_pb2'
+    # @@protoc_insertion_point(class_scope:prodvana.protection.CompiledProtectionAttachmentConfig.EnvEntry)
+    })
+  ,
+  'DESCRIPTOR' : _COMPILEDPROTECTIONATTACHMENTCONFIG,
+  '__module__' : 'prodvana.protection.protection_config_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.protection.CompiledProtectionAttachmentConfig)
+  })
+_sym_db.RegisterMessage(CompiledProtectionAttachmentConfig)
+_sym_db.RegisterMessage(CompiledProtectionAttachmentConfig.EnvEntry)
+
+ServiceInstanceAttachment = _reflection.GeneratedProtocolMessageType('ServiceInstanceAttachment', (_message.Message,), {
+  'DESCRIPTOR' : _SERVICEINSTANCEATTACHMENT,
+  '__module__' : 'prodvana.protection.protection_config_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.protection.ServiceInstanceAttachment)
+  })
+_sym_db.RegisterMessage(ServiceInstanceAttachment)
+
+ReleaseChannelAttachment = _reflection.GeneratedProtocolMessageType('ReleaseChannelAttachment', (_message.Message,), {
+  'DESCRIPTOR' : _RELEASECHANNELATTACHMENT,
+  '__module__' : 'prodvana.protection.protection_config_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.protection.ReleaseChannelAttachment)
+  })
+_sym_db.RegisterMessage(ReleaseChannelAttachment)
+
+ProtectionAttachment = _reflection.GeneratedProtocolMessageType('ProtectionAttachment', (_message.Message,), {
+  'DESCRIPTOR' : _PROTECTIONATTACHMENT,
+  '__module__' : 'prodvana.protection.protection_config_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.protection.ProtectionAttachment)
   })
-_sym_db.RegisterMessage(ServicePushParam)
-
-ServiceInstancePush = _reflection.GeneratedProtocolMessageType('ServiceInstancePush', (_message.Message,), {
-  'DESCRIPTOR' : _SERVICEINSTANCEPUSH,
-  '__module__' : 'prodvana.pipelines.object_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.pipelines.ServiceInstancePush)
-  })
-_sym_db.RegisterMessage(ServiceInstancePush)
-
-TaskStatus = _reflection.GeneratedProtocolMessageType('TaskStatus', (_message.Message,), {
-  'DESCRIPTOR' : _TASKSTATUS,
-  '__module__' : 'prodvana.pipelines.object_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.pipelines.TaskStatus)
-  })
-_sym_db.RegisterMessage(TaskStatus)
-
-PipelineState = _reflection.GeneratedProtocolMessageType('PipelineState', (_message.Message,), {
-  'DESCRIPTOR' : _PIPELINESTATE,
-  '__module__' : 'prodvana.pipelines.object_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.pipelines.PipelineState)
-  })
-_sym_db.RegisterMessage(PipelineState)
-
-Pipeline = _reflection.GeneratedProtocolMessageType('Pipeline', (_message.Message,), {
-  'DESCRIPTOR' : _PIPELINE,
-  '__module__' : 'prodvana.pipelines.object_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.pipelines.Pipeline)
-  })
-_sym_db.RegisterMessage(Pipeline)
-
-PipelineRunConfig = _reflection.GeneratedProtocolMessageType('PipelineRunConfig', (_message.Message,), {
-  'DESCRIPTOR' : _PIPELINERUNCONFIG,
-  '__module__' : 'prodvana.pipelines.object_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.pipelines.PipelineRunConfig)
-  })
-_sym_db.RegisterMessage(PipelineRunConfig)
-
-PipelineRunState = _reflection.GeneratedProtocolMessageType('PipelineRunState', (_message.Message,), {
-  'DESCRIPTOR' : _PIPELINERUNSTATE,
-  '__module__' : 'prodvana.pipelines.object_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.pipelines.PipelineRunState)
-  })
-_sym_db.RegisterMessage(PipelineRunState)
-
-PipelineRun = _reflection.GeneratedProtocolMessageType('PipelineRun', (_message.Message,), {
-  'DESCRIPTOR' : _PIPELINERUN,
-  '__module__' : 'prodvana.pipelines.object_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.pipelines.PipelineRun)
-  })
-_sym_db.RegisterMessage(PipelineRun)
+_sym_db.RegisterMessage(ProtectionAttachment)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZLgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/pipelines'
-  _SERVICEPUSHPARAM._serialized_start=230
-  _SERVICEPUSHPARAM._serialized_end=351
-  _SERVICEINSTANCEPUSH._serialized_start=354
-  _SERVICEINSTANCEPUSH._serialized_end=536
-  _TASKSTATUS._serialized_start=539
-  _TASKSTATUS._serialized_end=693
-  _PIPELINESTATE._serialized_start=695
-  _PIPELINESTATE._serialized_end=710
-  _PIPELINE._serialized_start=713
-  _PIPELINE._serialized_end=868
-  _PIPELINERUNCONFIG._serialized_start=871
-  _PIPELINERUNCONFIG._serialized_end=1153
-  _PIPELINERUNSTATE._serialized_start=1156
-  _PIPELINERUNSTATE._serialized_end=1471
-  _PIPELINERUN._serialized_start=1474
-  _PIPELINERUN._serialized_end=1656
+  DESCRIPTOR._serialized_options = b'ZMgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/protection'
+  _PROTECTIONCONFIG.oneofs_by_name['exec_config']._options = None
+  _PROTECTIONCONFIG.oneofs_by_name['exec_config']._serialized_options = b'\370B\001'
+  _PROTECTIONCONFIG.fields_by_name['name']._options = None
+  _PROTECTIONCONFIG.fields_by_name['name']._serialized_options = b'\372B(r&\020\001\030?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$'
+  _PROTECTIONCONFIG.fields_by_name['parameters']._options = None
+  _PROTECTIONCONFIG.fields_by_name['parameters']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
+  _COMPILEDPROTECTIONATTACHMENTCONFIG_ENVENTRY._options = None
+  _COMPILEDPROTECTIONATTACHMENTCONFIG_ENVENTRY._serialized_options = b'8\001'
+  _COMPILEDPROTECTIONATTACHMENTCONFIG.fields_by_name['env']._options = None
+  _COMPILEDPROTECTIONATTACHMENTCONFIG.fields_by_name['env']._serialized_options = b'\372B$\232\001!\030\001\"\035r\0332\031^[a-zA-Z_]+[a-zA-Z0-9_]*$'
+  _PROTECTIONATTACHMENT.oneofs_by_name['attachment']._options = None
+  _PROTECTIONATTACHMENT.oneofs_by_name['attachment']._serialized_options = b'\370B\001'
+  _PROTECTIONCONFIG._serialized_start=325
+  _PROTECTIONCONFIG._serialized_end=726
+  _COMPILEDPROTECTIONATTACHMENTCONFIG._serialized_start=729
+  _COMPILEDPROTECTIONATTACHMENTCONFIG._serialized_end=1217
+  _COMPILEDPROTECTIONATTACHMENTCONFIG_ENVENTRY._serialized_start=1141
+  _COMPILEDPROTECTIONATTACHMENTCONFIG_ENVENTRY._serialized_end=1217
+  _SERVICEINSTANCEATTACHMENT._serialized_start=1219
+  _SERVICEINSTANCEATTACHMENT._serialized_end=1309
+  _RELEASECHANNELATTACHMENT._serialized_start=1311
+  _RELEASECHANNELATTACHMENT._serialized_end=1383
+  _PROTECTIONATTACHMENT._serialized_start=1386
+  _PROTECTIONATTACHMENT._serialized_end=1577
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/pipelines/object_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/common_config/parameters_pb2.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -3,231 +3,242 @@
 isort:skip_file
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
-import google.protobuf.timestamp_pb2
-import prodvana.proto.prodvana.common_config.meta_pb2
-import prodvana.proto.prodvana.common_config.version_push_pb2
-import prodvana.proto.prodvana.object.meta_pb2
-import prodvana.proto.prodvana.pipelines.pipelines_pb2
+import prodvana.proto.prodvana.common_config.env_pb2
+import prodvana.proto.prodvana.common_config.program_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class ServicePushParam(google.protobuf.message.Message):
+class ProgramChange(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    SERVICE_FIELD_NUMBER: builtins.int
-    VERSION_PUSH_FIELD_NUMBER: builtins.int
-    APPLICATION_FIELD_NUMBER: builtins.int
-    service: builtins.str
-    @property
-    def version_push(self) -> prodvana.proto.prodvana.common_config.version_push_pb2.VersionPushOption: ...
-    application: builtins.str
+    NAME_FIELD_NUMBER: builtins.int
+    name: builtins.str
     def __init__(
         self,
         *,
-        service: builtins.str = ...,
-        version_push: prodvana.proto.prodvana.common_config.version_push_pb2.VersionPushOption | None = ...,
-        application: builtins.str = ...,
+        name: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["version_push", b"version_push"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "service", b"service", "version_push", b"version_push"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["name", b"name"]) -> None: ...
 
-global___ServicePushParam = ServicePushParam
+global___ProgramChange = ProgramChange
 
-class ServiceInstancePush(google.protobuf.message.Message):
+class StringParameterDefinition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    APPLICATION_META_FIELD_NUMBER: builtins.int
-    SERVICE_INSTANCE_META_FIELD_NUMBER: builtins.int
-    TARGET_VERSION_FIELD_NUMBER: builtins.int
-    @property
-    def application_meta(self) -> prodvana.proto.prodvana.object.meta_pb2.ObjectMeta: ...
-    @property
-    def service_instance_meta(self) -> prodvana.proto.prodvana.common_config.meta_pb2.ServiceInstanceObjectMeta:
-        """service starting version stored in service_instance_meta"""
-    target_version: builtins.str
-    """TODO(naphat/rohit) store rollback target information here
-    string rollback_target_version = 4;
-    """
+    DEFAULT_VALUE_FIELD_NUMBER: builtins.int
+    default_value: builtins.str
     def __init__(
         self,
         *,
-        application_meta: prodvana.proto.prodvana.object.meta_pb2.ObjectMeta | None = ...,
-        service_instance_meta: prodvana.proto.prodvana.common_config.meta_pb2.ServiceInstanceObjectMeta | None = ...,
-        target_version: builtins.str = ...,
+        default_value: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["application_meta", b"application_meta", "service_instance_meta", b"service_instance_meta"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["application_meta", b"application_meta", "service_instance_meta", b"service_instance_meta", "target_version", b"target_version"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["default_value", b"default_value"]) -> None: ...
 
-global___ServiceInstancePush = ServiceInstancePush
+global___StringParameterDefinition = StringParameterDefinition
 
-class TaskStatus(google.protobuf.message.Message):
+class DockerImageParameterDefinition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ID_FIELD_NUMBER: builtins.int
-    STATE_FIELD_NUMBER: builtins.int
-    CREATION_TIMESTAMP_FIELD_NUMBER: builtins.int
-    LAST_UPDATE_TIMESTAMP_FIELD_NUMBER: builtins.int
-    id: builtins.int
-    state: builtins.str
+    class Changes(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        PROGRAM_FIELD_NUMBER: builtins.int
+        @property
+        def program(self) -> global___ProgramChange: ...
+        def __init__(
+            self,
+            *,
+            program: global___ProgramChange | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["oneof", b"oneof", "program", b"program"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["oneof", b"oneof", "program", b"program"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["oneof", b"oneof"]) -> typing_extensions.Literal["program"] | None: ...
+
+    DEFAULT_TAG_FIELD_NUMBER: builtins.int
+    IMAGE_REGISTRY_INFO_FIELD_NUMBER: builtins.int
+    CHANGES_FIELD_NUMBER: builtins.int
+    default_tag: builtins.str
+    """empty not a valid value"""
     @property
-    def creation_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
+    def image_registry_info(self) -> prodvana.proto.prodvana.common_config.program_pb2.ImageRegistryInfo: ...
     @property
-    def last_update_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
+    def changes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DockerImageParameterDefinition.Changes]: ...
     def __init__(
         self,
         *,
-        id: builtins.int = ...,
-        state: builtins.str = ...,
-        creation_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
-        last_update_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+        default_tag: builtins.str = ...,
+        image_registry_info: prodvana.proto.prodvana.common_config.program_pb2.ImageRegistryInfo | None = ...,
+        changes: collections.abc.Iterable[global___DockerImageParameterDefinition.Changes] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["creation_timestamp", b"creation_timestamp", "last_update_timestamp", b"last_update_timestamp"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["creation_timestamp", b"creation_timestamp", "id", b"id", "last_update_timestamp", b"last_update_timestamp", "state", b"state"]) -> None: ...
-
-global___TaskStatus = TaskStatus
+    def HasField(self, field_name: typing_extensions.Literal["image_registry_info", b"image_registry_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["changes", b"changes", "default_tag", b"default_tag", "image_registry_info", b"image_registry_info"]) -> None: ...
 
-class PipelineState(google.protobuf.message.Message):
-    """TODO(naphat) put stuff here"""
+global___DockerImageParameterDefinition = DockerImageParameterDefinition
 
+class FixedReplicaChange(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     def __init__(
         self,
     ) -> None: ...
 
-global___PipelineState = PipelineState
+global___FixedReplicaChange = FixedReplicaChange
 
-class Pipeline(google.protobuf.message.Message):
+class IntParameterDefinition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    META_FIELD_NUMBER: builtins.int
-    CONFIG_FIELD_NUMBER: builtins.int
-    STATE_FIELD_NUMBER: builtins.int
-    @property
-    def meta(self) -> prodvana.proto.prodvana.object.meta_pb2.ObjectMeta: ...
-    @property
-    def config(self) -> prodvana.proto.prodvana.pipelines.pipelines_pb2.PipelineConfig: ...
+    class Changes(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        FIXED_REPLICA_FIELD_NUMBER: builtins.int
+        @property
+        def fixed_replica(self) -> global___FixedReplicaChange: ...
+        def __init__(
+            self,
+            *,
+            fixed_replica: global___FixedReplicaChange | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["fixed_replica", b"fixed_replica", "oneof", b"oneof"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["fixed_replica", b"fixed_replica", "oneof", b"oneof"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["oneof", b"oneof"]) -> typing_extensions.Literal["fixed_replica"] | None: ...
+
+    DEFAULT_VALUE_FIELD_NUMBER: builtins.int
+    CHANGES_FIELD_NUMBER: builtins.int
+    default_value: builtins.int
     @property
-    def state(self) -> global___PipelineState: ...
+    def changes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___IntParameterDefinition.Changes]: ...
     def __init__(
         self,
         *,
-        meta: prodvana.proto.prodvana.object.meta_pb2.ObjectMeta | None = ...,
-        config: prodvana.proto.prodvana.pipelines.pipelines_pb2.PipelineConfig | None = ...,
-        state: global___PipelineState | None = ...,
+        default_value: builtins.int = ...,
+        changes: collections.abc.Iterable[global___IntParameterDefinition.Changes] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["config", b"config", "meta", b"meta", "state", b"state"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["config", b"config", "meta", b"meta", "state", b"state"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["changes", b"changes", "default_value", b"default_value"]) -> None: ...
 
-global___Pipeline = Pipeline
+global___IntParameterDefinition = IntParameterDefinition
 
-class PipelineRunConfig(google.protobuf.message.Message):
+class SecretParameterDefinition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PIPELINE_CONFIG_FIELD_NUMBER: builtins.int
-    SERVICE_PUSH_PARAMS_FIELD_NUMBER: builtins.int
-    SKIP_ROLLBACK_VALIDATION_FIELD_NUMBER: builtins.int
-    SERVICE_INSTANCE_PUSHES_FIELD_NUMBER: builtins.int
-    SKIP_ALERT_CHECKS_FIELD_NUMBER: builtins.int
+    def __init__(
+        self,
+    ) -> None: ...
+
+global___SecretParameterDefinition = SecretParameterDefinition
+
+class ParameterDefinition(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    NAME_FIELD_NUMBER: builtins.int
+    DESCRIPTION_FIELD_NUMBER: builtins.int
+    STRING_FIELD_NUMBER: builtins.int
+    DOCKER_IMAGE_FIELD_NUMBER: builtins.int
+    INT_FIELD_NUMBER: builtins.int
+    SECRET_FIELD_NUMBER: builtins.int
+    REQUIRED_FIELD_NUMBER: builtins.int
+    name: builtins.str
+    """parameter name, used in substitutions"""
+    description: builtins.str
+    """optional description for display purposes"""
     @property
-    def pipeline_config(self) -> prodvana.proto.prodvana.pipelines.pipelines_pb2.PipelineConfig: ...
+    def string(self) -> global___StringParameterDefinition: ...
     @property
-    def service_push_params(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ServicePushParam]: ...
-    skip_rollback_validation: builtins.bool
+    def docker_image(self) -> global___DockerImageParameterDefinition: ...
     @property
-    def service_instance_pushes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ServiceInstancePush]: ...
-    skip_alert_checks: builtins.bool
+    def int(self) -> global___IntParameterDefinition: ...
+    @property
+    def secret(self) -> global___SecretParameterDefinition: ...
+    required: builtins.bool
+    """next: 8"""
     def __init__(
         self,
         *,
-        pipeline_config: prodvana.proto.prodvana.pipelines.pipelines_pb2.PipelineConfig | None = ...,
-        service_push_params: collections.abc.Iterable[global___ServicePushParam] | None = ...,
-        skip_rollback_validation: builtins.bool = ...,
-        service_instance_pushes: collections.abc.Iterable[global___ServiceInstancePush] | None = ...,
-        skip_alert_checks: builtins.bool = ...,
+        name: builtins.str = ...,
+        description: builtins.str = ...,
+        string: global___StringParameterDefinition | None = ...,
+        docker_image: global___DockerImageParameterDefinition | None = ...,
+        int: global___IntParameterDefinition | None = ...,
+        secret: global___SecretParameterDefinition | None = ...,
+        required: builtins.bool = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["pipeline_config", b"pipeline_config"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["pipeline_config", b"pipeline_config", "service_instance_pushes", b"service_instance_pushes", "service_push_params", b"service_push_params", "skip_alert_checks", b"skip_alert_checks", "skip_rollback_validation", b"skip_rollback_validation"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["config_oneof", b"config_oneof", "docker_image", b"docker_image", "int", b"int", "secret", b"secret", "string", b"string"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["config_oneof", b"config_oneof", "description", b"description", "docker_image", b"docker_image", "int", b"int", "name", b"name", "required", b"required", "secret", b"secret", "string", b"string"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["string", "docker_image", "int", "secret"] | None: ...
 
-global___PipelineRunConfig = PipelineRunConfig
+global___ParameterDefinition = ParameterDefinition
 
-class PipelineRunState(google.protobuf.message.Message):
+class SecretParameterValue(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    CREATION_TIMESTAMP_FIELD_NUMBER: builtins.int
-    LAST_UPDATE_TIMESTAMP_FIELD_NUMBER: builtins.int
-    STATE_FIELD_NUMBER: builtins.int
-    TERMINAL_FIELD_NUMBER: builtins.int
-    TASK_STATUSES_FIELD_NUMBER: builtins.int
-    LASTACTOR_FIELD_NUMBER: builtins.int
-    INITIATOR_FIELD_NUMBER: builtins.int
-    REASON_FIELD_NUMBER: builtins.int
-    MESSAGE_FIELD_NUMBER: builtins.int
-    EXTERNAL_LINK_FIELD_NUMBER: builtins.int
-    @property
-    def creation_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
+    RAW_SECRET_FIELD_NUMBER: builtins.int
+    SECRET_REF_FIELD_NUMBER: builtins.int
+    raw_secret: builtins.str
+    """Raw secret value"""
     @property
-    def last_update_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
-    state: builtins.str
-    terminal: builtins.bool
-    """if pipeline run is in a terminal state"""
-    @property
-    def task_statuses(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TaskStatus]:
-        """This will only be set when querying specifically about this pipeline run"""
-    lastActor: builtins.str
-    initiator: builtins.str
-    reason: builtins.str
-    message: builtins.str
-    external_link: builtins.str
+    def secret_ref(self) -> prodvana.proto.prodvana.common_config.env_pb2.Secret:
+        """Existing secret reference."""
     def __init__(
         self,
         *,
-        creation_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
-        last_update_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
-        state: builtins.str = ...,
-        terminal: builtins.bool = ...,
-        task_statuses: collections.abc.Iterable[global___TaskStatus] | None = ...,
-        lastActor: builtins.str = ...,
-        initiator: builtins.str = ...,
-        reason: builtins.str = ...,
-        message: builtins.str = ...,
-        external_link: builtins.str = ...,
+        raw_secret: builtins.str = ...,
+        secret_ref: prodvana.proto.prodvana.common_config.env_pb2.Secret | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["creation_timestamp", b"creation_timestamp", "last_update_timestamp", b"last_update_timestamp"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["creation_timestamp", b"creation_timestamp", "external_link", b"external_link", "initiator", b"initiator", "lastActor", b"lastActor", "last_update_timestamp", b"last_update_timestamp", "message", b"message", "reason", b"reason", "state", b"state", "task_statuses", b"task_statuses", "terminal", b"terminal"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["raw_secret", b"raw_secret", "secret_oneof", b"secret_oneof", "secret_ref", b"secret_ref"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["raw_secret", b"raw_secret", "secret_oneof", b"secret_oneof", "secret_ref", b"secret_ref"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["secret_oneof", b"secret_oneof"]) -> typing_extensions.Literal["raw_secret", "secret_ref"] | None: ...
 
-global___PipelineRunState = PipelineRunState
+global___SecretParameterValue = SecretParameterValue
 
-class PipelineRun(google.protobuf.message.Message):
+class ParameterValue(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    META_FIELD_NUMBER: builtins.int
-    CONFIG_FIELD_NUMBER: builtins.int
-    STATE_FIELD_NUMBER: builtins.int
-    @property
-    def meta(self) -> prodvana.proto.prodvana.common_config.meta_pb2.PipelineRunObjectMeta: ...
+    NAME_FIELD_NUMBER: builtins.int
+    STRING_FIELD_NUMBER: builtins.int
+    INT_FIELD_NUMBER: builtins.int
+    DOCKER_IMAGE_TAG_FIELD_NUMBER: builtins.int
+    SECRET_FIELD_NUMBER: builtins.int
+    name: builtins.str
+    string: builtins.str
+    int: builtins.int
+    docker_image_tag: builtins.str
     @property
-    def config(self) -> global___PipelineRunConfig: ...
+    def secret(self) -> global___SecretParameterValue: ...
+    def __init__(
+        self,
+        *,
+        name: builtins.str = ...,
+        string: builtins.str = ...,
+        int: builtins.int = ...,
+        docker_image_tag: builtins.str = ...,
+        secret: global___SecretParameterValue | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["docker_image_tag", b"docker_image_tag", "int", b"int", "secret", b"secret", "string", b"string", "value_oneof", b"value_oneof"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["docker_image_tag", b"docker_image_tag", "int", b"int", "name", b"name", "secret", b"secret", "string", b"string", "value_oneof", b"value_oneof"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["value_oneof", b"value_oneof"]) -> typing_extensions.Literal["string", "int", "docker_image_tag", "secret"] | None: ...
+
+global___ParameterValue = ParameterValue
+
+class ParametersConfig(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    PARAMETERS_FIELD_NUMBER: builtins.int
     @property
-    def state(self) -> global___PipelineRunState: ...
+    def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ParameterDefinition]: ...
     def __init__(
         self,
         *,
-        meta: prodvana.proto.prodvana.common_config.meta_pb2.PipelineRunObjectMeta | None = ...,
-        config: global___PipelineRunConfig | None = ...,
-        state: global___PipelineRunState | None = ...,
+        parameters: collections.abc.Iterable[global___ParameterDefinition] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["config", b"config", "meta", b"meta", "state", b"state"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["config", b"config", "meta", b"meta", "state", b"state"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["parameters", b"parameters"]) -> None: ...
 
-global___PipelineRun = PipelineRun
+global___ParametersConfig = ParametersConfig
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/pipelines/pipelines_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/pipelines/pipelines_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/protection/attachments_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/protection/attachments_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/protection/attachments_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/protection/attachments_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/protection/object_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/protection/object_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from prodvana.proto.prodvana.object import meta_pb2 as prodvana_dot_object_dot_meta__pb2
 from prodvana.proto.prodvana.protection import protection_config_pb2 as prodvana_dot_protection_dot_protection__config__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n prodvana/protection/object.proto\x12\x13prodvana.protection\x1a\x1aprodvana/object/meta.proto\x1a+prodvana/protection/protection_config.proto\"n\n\nProtection\x12)\n\x04meta\x18\x01 \x01(\x0b\x32\x1b.prodvana.object.ObjectMeta\x12\x35\n\x06\x63onfig\x18\x02 \x01(\x0b\x32%.prodvana.protection.ProtectionConfigBOZMgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/protectionb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n prodvana/protection/object.proto\x12\x13prodvana.protection\x1a\x1aprodvana/object/meta.proto\x1a+prodvana/protection/protection_config.proto\"\x7f\n\nProtection\x12)\n\x04meta\x18\x01 \x01(\x0b\x32\x1b.prodvana.object.ObjectMeta\x12\x35\n\x06\x63onfig\x18\x02 \x01(\x0b\x32%.prodvana.protection.ProtectionConfig\x12\x0f\n\x07\x62uiltin\x18\x03 \x01(\x08\x42OZMgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/protectionb\x06proto3')
 
 
 
 _PROTECTION = DESCRIPTOR.message_types_by_name['Protection']
 Protection = _reflection.GeneratedProtocolMessageType('Protection', (_message.Message,), {
   'DESCRIPTOR' : _PROTECTION,
   '__module__' : 'prodvana.protection.object_pb2'
@@ -29,9 +29,9 @@
 _sym_db.RegisterMessage(Protection)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZMgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/protection'
   _PROTECTION._serialized_start=130
-  _PROTECTION._serialized_end=240
+  _PROTECTION._serialized_end=257
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/protection/object_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/protection/object_pb2.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -17,22 +17,25 @@
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class Protection(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     META_FIELD_NUMBER: builtins.int
     CONFIG_FIELD_NUMBER: builtins.int
+    BUILTIN_FIELD_NUMBER: builtins.int
     @property
     def meta(self) -> prodvana.proto.prodvana.object.meta_pb2.ObjectMeta: ...
     @property
-    def config(self) -> prodvana.proto.prodvana.protection.protection_config_pb2.ProtectionConfig:
-        """TODO: Add information about where this protection is currently used?"""
+    def config(self) -> prodvana.proto.prodvana.protection.protection_config_pb2.ProtectionConfig: ...
+    builtin: builtins.bool
+    """indicates this protection is provided by Prodvana by default."""
     def __init__(
         self,
         *,
         meta: prodvana.proto.prodvana.object.meta_pb2.ObjectMeta | None = ...,
         config: prodvana.proto.prodvana.protection.protection_config_pb2.ProtectionConfig | None = ...,
+        builtin: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["config", b"config", "meta", b"meta"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["config", b"config", "meta", b"meta"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["builtin", b"builtin", "config", b"config", "meta", b"meta"]) -> None: ...
 
 global___Protection = Protection
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_config_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_config_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.duration_pb2
 import google.protobuf.internal.containers
 import google.protobuf.message
 import prodvana.proto.prodvana.common_config.env_pb2
-import prodvana.proto.prodvana.common_config.external_config_pb2
+import prodvana.proto.prodvana.common_config.kubernetes_config_pb2
 import prodvana.proto.prodvana.common_config.parameters_pb2
 import prodvana.proto.prodvana.common_config.task_pb2
 import prodvana.proto.prodvana.runtimes.runtimes_config_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
@@ -23,24 +23,24 @@
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class ProtectionConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     TASK_CONFIG_FIELD_NUMBER: builtins.int
-    EXTERNAL_CONFIG_FIELD_NUMBER: builtins.int
+    KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
     POLL_INTERVAL_FIELD_NUMBER: builtins.int
     TIMEOUT_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
     name: builtins.str
     @property
     def task_config(self) -> prodvana.proto.prodvana.common_config.task_pb2.TaskConfig:
         """Inline task config with retry, template support."""
     @property
-    def external_config(self) -> prodvana.proto.prodvana.common_config.external_config_pb2.ExternalConfig: ...
+    def kubernetes_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig: ...
     @property
     def poll_interval(self) -> google.protobuf.duration_pb2.Duration:
         """customize intervals instead of using Prodvana default
         how often to run check even if it succeeds
         """
     @property
     def timeout(self) -> google.protobuf.duration_pb2.Duration:
@@ -48,22 +48,22 @@
     @property
     def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition]: ...
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         task_config: prodvana.proto.prodvana.common_config.task_pb2.TaskConfig | None = ...,
-        external_config: prodvana.proto.prodvana.common_config.external_config_pb2.ExternalConfig | None = ...,
+        kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         poll_interval: google.protobuf.duration_pb2.Duration | None = ...,
         timeout: google.protobuf.duration_pb2.Duration | None = ...,
         parameters: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "external_config", b"external_config", "poll_interval", b"poll_interval", "task_config", b"task_config", "timeout", b"timeout"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "external_config", b"external_config", "name", b"name", "parameters", b"parameters", "poll_interval", b"poll_interval", "task_config", b"task_config", "timeout", b"timeout"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["exec_config", b"exec_config"]) -> typing_extensions.Literal["task_config", "external_config"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "kubernetes_config", b"kubernetes_config", "poll_interval", b"poll_interval", "task_config", b"task_config", "timeout", b"timeout"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["exec_config", b"exec_config", "kubernetes_config", b"kubernetes_config", "name", b"name", "parameters", b"parameters", "poll_interval", b"poll_interval", "task_config", b"task_config", "timeout", b"timeout"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["exec_config", b"exec_config"]) -> typing_extensions.Literal["task_config", "kubernetes_config"] | None: ...
 
 global___ProtectionConfig = ProtectionConfig
 
 class CompiledProtectionAttachmentConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class EnvEntry(google.protobuf.message.Message):
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_manager_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py` & `prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_reference_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_reference_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,23 +13,23 @@
 
 
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 from prodvana.proto.prodvana.common_config import parameters_pb2 as prodvana_dot_common__config_dot_parameters__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.prodvana/protection/protection_reference.proto\x12\x13prodvana.protection\x1a\x1egoogle/protobuf/duration.proto\x1a\x17validate/validate.proto\x1a\'prodvana/common_config/parameters.proto\"\xf8\x03\n\x13ProtectionLifecycle\x12L\n\x0cpre_approval\x18\x01 \x01(\x0b\x32\x34.prodvana.protection.ProtectionLifecycle.PreApprovalH\x00\x12N\n\rpost_approval\x18\x03 \x01(\x0b\x32\x35.prodvana.protection.ProtectionLifecycle.PostApprovalH\x00\x12=\n\x04push\x18\x04 \x01(\x0b\x32-.prodvana.protection.ProtectionLifecycle.PushH\x00\x12\x46\n\tpost_push\x18\x05 \x01(\x0b\x32\x31.prodvana.protection.ProtectionLifecycle.PostPushH\x00\x1a\r\n\x0bPreApproval\x1a\x0e\n\x0cPostApproval\x1a\x06\n\x04Push\x1a\x82\x01\n\x08PostPush\x12\x37\n\x14\x64\x65lay_check_duration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x0e\x63heck_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\n\xfa\x42\x07\xaa\x01\x04\x08\x01*\x00\x42\x10\n\tlifecycle\x12\x03\xf8\x42\x01\"\x9c\x01\n\x13ProtectionReference\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12:\n\nparameters\x18\x03 \x03(\x0b\x32&.prodvana.common_config.ParameterValueJ\x04\x08\x02\x10\x03R\x08\x61ttachedBOZMgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/protectionb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.prodvana/protection/protection_reference.proto\x12\x13prodvana.protection\x1a\x1egoogle/protobuf/duration.proto\x1a\x17validate/validate.proto\x1a\'prodvana/common_config/parameters.proto\"\x9c\x04\n\x13ProtectionLifecycle\x12L\n\x0cpre_approval\x18\x01 \x01(\x0b\x32\x34.prodvana.protection.ProtectionLifecycle.PreApprovalH\x00\x12N\n\rpost_approval\x18\x03 \x01(\x0b\x32\x35.prodvana.protection.ProtectionLifecycle.PostApprovalH\x00\x12I\n\ndeployment\x18\x04 \x01(\x0b\x32\x33.prodvana.protection.ProtectionLifecycle.DeploymentH\x00\x12R\n\x0fpost_deployment\x18\x05 \x01(\x0b\x32\x37.prodvana.protection.ProtectionLifecycle.PostDeploymentH\x00\x1a\r\n\x0bPreApproval\x1a\x0e\n\x0cPostApproval\x1a\x0c\n\nDeployment\x1a\x88\x01\n\x0ePostDeployment\x12\x37\n\x14\x64\x65lay_check_duration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x0e\x63heck_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB\n\xfa\x42\x07\xaa\x01\x04\x08\x01*\x00\x42\x10\n\tlifecycle\x12\x03\xf8\x42\x01\"\x9c\x01\n\x13ProtectionReference\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12:\n\nparameters\x18\x03 \x03(\x0b\x32&.prodvana.common_config.ParameterValueJ\x04\x08\x02\x10\x03R\x08\x61ttachedBOZMgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/protectionb\x06proto3')
 
 
 
 _PROTECTIONLIFECYCLE = DESCRIPTOR.message_types_by_name['ProtectionLifecycle']
 _PROTECTIONLIFECYCLE_PREAPPROVAL = _PROTECTIONLIFECYCLE.nested_types_by_name['PreApproval']
 _PROTECTIONLIFECYCLE_POSTAPPROVAL = _PROTECTIONLIFECYCLE.nested_types_by_name['PostApproval']
-_PROTECTIONLIFECYCLE_PUSH = _PROTECTIONLIFECYCLE.nested_types_by_name['Push']
-_PROTECTIONLIFECYCLE_POSTPUSH = _PROTECTIONLIFECYCLE.nested_types_by_name['PostPush']
+_PROTECTIONLIFECYCLE_DEPLOYMENT = _PROTECTIONLIFECYCLE.nested_types_by_name['Deployment']
+_PROTECTIONLIFECYCLE_POSTDEPLOYMENT = _PROTECTIONLIFECYCLE.nested_types_by_name['PostDeployment']
 _PROTECTIONREFERENCE = DESCRIPTOR.message_types_by_name['ProtectionReference']
 ProtectionLifecycle = _reflection.GeneratedProtocolMessageType('ProtectionLifecycle', (_message.Message,), {
 
   'PreApproval' : _reflection.GeneratedProtocolMessageType('PreApproval', (_message.Message,), {
     'DESCRIPTOR' : _PROTECTIONLIFECYCLE_PREAPPROVAL,
     '__module__' : 'prodvana.protection.protection_reference_pb2'
     # @@protoc_insertion_point(class_scope:prodvana.protection.ProtectionLifecycle.PreApproval)
@@ -39,60 +39,60 @@
   'PostApproval' : _reflection.GeneratedProtocolMessageType('PostApproval', (_message.Message,), {
     'DESCRIPTOR' : _PROTECTIONLIFECYCLE_POSTAPPROVAL,
     '__module__' : 'prodvana.protection.protection_reference_pb2'
     # @@protoc_insertion_point(class_scope:prodvana.protection.ProtectionLifecycle.PostApproval)
     })
   ,
 
-  'Push' : _reflection.GeneratedProtocolMessageType('Push', (_message.Message,), {
-    'DESCRIPTOR' : _PROTECTIONLIFECYCLE_PUSH,
+  'Deployment' : _reflection.GeneratedProtocolMessageType('Deployment', (_message.Message,), {
+    'DESCRIPTOR' : _PROTECTIONLIFECYCLE_DEPLOYMENT,
     '__module__' : 'prodvana.protection.protection_reference_pb2'
-    # @@protoc_insertion_point(class_scope:prodvana.protection.ProtectionLifecycle.Push)
+    # @@protoc_insertion_point(class_scope:prodvana.protection.ProtectionLifecycle.Deployment)
     })
   ,
 
-  'PostPush' : _reflection.GeneratedProtocolMessageType('PostPush', (_message.Message,), {
-    'DESCRIPTOR' : _PROTECTIONLIFECYCLE_POSTPUSH,
+  'PostDeployment' : _reflection.GeneratedProtocolMessageType('PostDeployment', (_message.Message,), {
+    'DESCRIPTOR' : _PROTECTIONLIFECYCLE_POSTDEPLOYMENT,
     '__module__' : 'prodvana.protection.protection_reference_pb2'
-    # @@protoc_insertion_point(class_scope:prodvana.protection.ProtectionLifecycle.PostPush)
+    # @@protoc_insertion_point(class_scope:prodvana.protection.ProtectionLifecycle.PostDeployment)
     })
   ,
   'DESCRIPTOR' : _PROTECTIONLIFECYCLE,
   '__module__' : 'prodvana.protection.protection_reference_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.protection.ProtectionLifecycle)
   })
 _sym_db.RegisterMessage(ProtectionLifecycle)
 _sym_db.RegisterMessage(ProtectionLifecycle.PreApproval)
 _sym_db.RegisterMessage(ProtectionLifecycle.PostApproval)
-_sym_db.RegisterMessage(ProtectionLifecycle.Push)
-_sym_db.RegisterMessage(ProtectionLifecycle.PostPush)
+_sym_db.RegisterMessage(ProtectionLifecycle.Deployment)
+_sym_db.RegisterMessage(ProtectionLifecycle.PostDeployment)
 
 ProtectionReference = _reflection.GeneratedProtocolMessageType('ProtectionReference', (_message.Message,), {
   'DESCRIPTOR' : _PROTECTIONREFERENCE,
   '__module__' : 'prodvana.protection.protection_reference_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.protection.ProtectionReference)
   })
 _sym_db.RegisterMessage(ProtectionReference)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZMgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/protection'
-  _PROTECTIONLIFECYCLE_POSTPUSH.fields_by_name['check_duration']._options = None
-  _PROTECTIONLIFECYCLE_POSTPUSH.fields_by_name['check_duration']._serialized_options = b'\372B\007\252\001\004\010\001*\000'
+  _PROTECTIONLIFECYCLE_POSTDEPLOYMENT.fields_by_name['check_duration']._options = None
+  _PROTECTIONLIFECYCLE_POSTDEPLOYMENT.fields_by_name['check_duration']._serialized_options = b'\372B\007\252\001\004\010\001*\000'
   _PROTECTIONLIFECYCLE.oneofs_by_name['lifecycle']._options = None
   _PROTECTIONLIFECYCLE.oneofs_by_name['lifecycle']._serialized_options = b'\370B\001'
   _PROTECTIONREFERENCE.fields_by_name['name']._options = None
   _PROTECTIONREFERENCE.fields_by_name['name']._serialized_options = b'\372B(r&\020\001\030?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$'
   _PROTECTIONLIFECYCLE._serialized_start=170
-  _PROTECTIONLIFECYCLE._serialized_end=674
-  _PROTECTIONLIFECYCLE_PREAPPROVAL._serialized_start=486
-  _PROTECTIONLIFECYCLE_PREAPPROVAL._serialized_end=499
-  _PROTECTIONLIFECYCLE_POSTAPPROVAL._serialized_start=501
-  _PROTECTIONLIFECYCLE_POSTAPPROVAL._serialized_end=515
-  _PROTECTIONLIFECYCLE_PUSH._serialized_start=517
-  _PROTECTIONLIFECYCLE_PUSH._serialized_end=523
-  _PROTECTIONLIFECYCLE_POSTPUSH._serialized_start=526
-  _PROTECTIONLIFECYCLE_POSTPUSH._serialized_end=656
-  _PROTECTIONREFERENCE._serialized_start=677
-  _PROTECTIONREFERENCE._serialized_end=833
+  _PROTECTIONLIFECYCLE._serialized_end=710
+  _PROTECTIONLIFECYCLE_PREAPPROVAL._serialized_start=510
+  _PROTECTIONLIFECYCLE_PREAPPROVAL._serialized_end=523
+  _PROTECTIONLIFECYCLE_POSTAPPROVAL._serialized_start=525
+  _PROTECTIONLIFECYCLE_POSTAPPROVAL._serialized_end=539
+  _PROTECTIONLIFECYCLE_DEPLOYMENT._serialized_start=541
+  _PROTECTIONLIFECYCLE_DEPLOYMENT._serialized_end=553
+  _PROTECTIONLIFECYCLE_POSTDEPLOYMENT._serialized_start=556
+  _PROTECTIONLIFECYCLE_POSTDEPLOYMENT._serialized_end=692
+  _PROTECTIONREFERENCE._serialized_start=713
+  _PROTECTIONREFERENCE._serialized_end=869
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -35,30 +35,30 @@
 
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         def __init__(
             self,
         ) -> None: ...
 
-    class Push(google.protobuf.message.Message):
+    class Deployment(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         def __init__(
             self,
         ) -> None: ...
 
-    class PostPush(google.protobuf.message.Message):
+    class PostDeployment(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         DELAY_CHECK_DURATION_FIELD_NUMBER: builtins.int
         CHECK_DURATION_FIELD_NUMBER: builtins.int
         @property
         def delay_check_duration(self) -> google.protobuf.duration_pb2.Duration:
-            """How long after the push completes should we start checking status?
-            e.g, delay health checks X minutes after push (if push is noisy).
+            """How long after the deployment completes should we start checking status?
+            e.g, delay health checks X minutes after deployment (if deployment is noisy).
             """
         @property
         def check_duration(self) -> google.protobuf.duration_pb2.Duration:
             """How long after starting should we check for?"""
         def __init__(
             self,
             *,
@@ -66,37 +66,37 @@
             check_duration: google.protobuf.duration_pb2.Duration | None = ...,
         ) -> None: ...
         def HasField(self, field_name: typing_extensions.Literal["check_duration", b"check_duration", "delay_check_duration", b"delay_check_duration"]) -> builtins.bool: ...
         def ClearField(self, field_name: typing_extensions.Literal["check_duration", b"check_duration", "delay_check_duration", b"delay_check_duration"]) -> None: ...
 
     PRE_APPROVAL_FIELD_NUMBER: builtins.int
     POST_APPROVAL_FIELD_NUMBER: builtins.int
-    PUSH_FIELD_NUMBER: builtins.int
-    POST_PUSH_FIELD_NUMBER: builtins.int
+    DEPLOYMENT_FIELD_NUMBER: builtins.int
+    POST_DEPLOYMENT_FIELD_NUMBER: builtins.int
     @property
     def pre_approval(self) -> global___ProtectionLifecycle.PreApproval:
         """NOTE: Type here must match CustomTaskType"""
     @property
     def post_approval(self) -> global___ProtectionLifecycle.PostApproval:
         """Approval approval = 2;"""
     @property
-    def push(self) -> global___ProtectionLifecycle.Push: ...
+    def deployment(self) -> global___ProtectionLifecycle.Deployment: ...
     @property
-    def post_push(self) -> global___ProtectionLifecycle.PostPush: ...
+    def post_deployment(self) -> global___ProtectionLifecycle.PostDeployment: ...
     def __init__(
         self,
         *,
         pre_approval: global___ProtectionLifecycle.PreApproval | None = ...,
         post_approval: global___ProtectionLifecycle.PostApproval | None = ...,
-        push: global___ProtectionLifecycle.Push | None = ...,
-        post_push: global___ProtectionLifecycle.PostPush | None = ...,
+        deployment: global___ProtectionLifecycle.Deployment | None = ...,
+        post_deployment: global___ProtectionLifecycle.PostDeployment | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["lifecycle", b"lifecycle", "post_approval", b"post_approval", "post_push", b"post_push", "pre_approval", b"pre_approval", "push", b"push"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["lifecycle", b"lifecycle", "post_approval", b"post_approval", "post_push", b"post_push", "pre_approval", b"pre_approval", "push", b"push"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["lifecycle", b"lifecycle"]) -> typing_extensions.Literal["pre_approval", "post_approval", "push", "post_push"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["deployment", b"deployment", "lifecycle", b"lifecycle", "post_approval", b"post_approval", "post_deployment", b"post_deployment", "pre_approval", b"pre_approval"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["deployment", b"deployment", "lifecycle", b"lifecycle", "post_approval", b"post_approval", "post_deployment", b"post_deployment", "pre_approval", b"pre_approval"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["lifecycle", b"lifecycle"]) -> typing_extensions.Literal["pre_approval", "post_approval", "deployment", "post_deployment"] | None: ...
 
 global___ProtectionLifecycle = ProtectionLifecycle
 
 class ProtectionReference(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/release_channel/object_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/release_channel/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/release_channel/object_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/release_channel/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py` & `prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/repo/repo_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/repo/repo_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/repo/repo_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/repo/repo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/runtimes/extensions_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/runtimes/extensions_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/runtimes/extensions_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/runtimes/extensions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/scm/types_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/scm/types_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/scm/types_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/scm/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py` & `prodvana-0.1.5/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/service/object_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/service/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/service/object_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/service/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/service/parameters_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/service/parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/service/parameters_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/service/parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/service/service_config_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/service/service_config_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from prodvana.proto.prodvana.capability import capability_pb2 as prodvana_dot_capability_dot_capability__pb2
 from prodvana.proto.prodvana.common_config import env_pb2 as prodvana_dot_common__config_dot_env__pb2
-from prodvana.proto.prodvana.common_config import external_config_pb2 as prodvana_dot_common__config_dot_external__config__pb2
+from prodvana.proto.prodvana.common_config import kubernetes_config_pb2 as prodvana_dot_common__config_dot_kubernetes__config__pb2
 from prodvana.proto.prodvana.common_config import helm_pb2 as prodvana_dot_common__config_dot_helm__pb2
 from prodvana.proto.prodvana.common_config import maturity_pb2 as prodvana_dot_common__config_dot_maturity__pb2
 from prodvana.proto.prodvana.common_config import parameters_pb2 as prodvana_dot_common__config_dot_parameters__pb2
 from prodvana.proto.prodvana.common_config import program_pb2 as prodvana_dot_common__config_dot_program__pb2
 from prodvana.proto.prodvana.common_config import ref_pb2 as prodvana_dot_common__config_dot_ref__pb2
 from prodvana.proto.prodvana.common_config import retry_pb2 as prodvana_dot_common__config_dot_retry__pb2
 from prodvana.proto.prodvana.delivery import delivery_config_pb2 as prodvana_dot_delivery_dot_delivery__config__pb2
@@ -28,15 +28,15 @@
 from prodvana.proto.prodvana.runtimes import runtimes_config_pb2 as prodvana_dot_runtimes_dot_runtimes__config__pb2
 from prodvana.proto.prodvana.workflow import integration_config_pb2 as prodvana_dot_workflow_dot_integration__config__pb2
 from prodvana.proto.prodvana.service import parameters_pb2 as prodvana_dot_service_dot_parameters__pb2
 from prodvana.proto.prodvana.volumes import volumes_pb2 as prodvana_dot_volumes_dot_volumes__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%prodvana/service/service_config.proto\x12\x10prodvana.service\x1a\x1egoogle/protobuf/duration.proto\x1a$prodvana/capability/capability.proto\x1a prodvana/common_config/env.proto\x1a,prodvana/common_config/external_config.proto\x1a!prodvana/common_config/helm.proto\x1a%prodvana/common_config/maturity.proto\x1a\'prodvana/common_config/parameters.proto\x1a$prodvana/common_config/program.proto\x1a prodvana/common_config/ref.proto\x1a\"prodvana/common_config/retry.proto\x1a\'prodvana/delivery/delivery_config.proto\x1a.prodvana/protection/protection_reference.proto\x1a\x35prodvana/release_channel/release_channel_config.proto\x1a\'prodvana/runtimes/runtimes_config.proto\x1a*prodvana/workflow/integration_config.proto\x1a!prodvana/service/parameters.proto\x1a\x1eprodvana/volumes/volumes.proto\x1a\x17validate/validate.proto\"1\n\x0eReplicasConfig\x12\x0f\n\x05\x66ixed\x18\x01 \x01(\x05H\x00\x42\x0e\n\x0c\x63onfig_oneof\"\xaa\x02\n\x0eMetricAnalysis\x12J\n\x0csuccess_rate\x18\x02 \x01(\x0b\x32\x32.prodvana.service.MetricAnalysis.SuccessRateConfigH\x00\x12\x45\n\x0blatency_p95\x18\x03 \x01(\x0b\x32..prodvana.service.MetricAnalysis.LatencyConfigH\x00\x1a\x32\n\x11SuccessRateConfig\x12\x1d\n\x15min_threshold_percent\x18\x01 \x01(\x01\x1a?\n\rLatencyConfig\x12.\n\x0bmax_latency\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x10\n\x0e\x61nalysis_oneof\"\xb7\x02\n\x15ReleaseStrategyConfig\x12<\n\x19individual_stage_deadline\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x1a\x61utomated_testing_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12:\n\x10metrics_analysis\x18\x03 \x03(\x0b\x32 .prodvana.service.MetricAnalysis\x12\x17\n\x0fmanual_approval\x18\x04 \x01(\x08\x12\x31\n\x0e\x63heck_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x19\n\x11\x66\x61ilure_threshold\x18\x06 \x01(\x05\"f\n\tTLSSecret\x12\x14\n\nraw_secret\x18\x03 \x01(\tH\x00\x12\x30\n\x06secret\x18\x04 \x01(\x0b\x32\x1e.prodvana.common_config.SecretH\x00\x42\x11\n\ntls_secret\x12\x03\xf8\x42\x01\"\x81\x01\n\x0eTLSCertificate\x12\x37\n\x08tls_cert\x18\x01 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x36\n\x07tls_key\x18\x02 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\"j\n\x0b\x43\x65rtificate\x12/\n\x03tls\x18\x01 \x01(\x0b\x32 .prodvana.service.TLSCertificateH\x00\x12\x16\n\x0c\x61ws_acm_cert\x18\x02 \x01(\tH\x00\x42\x12\n\x0b\x63\x65rtificate\x12\x03\xf8\x42\x01\"\x84\x06\n\x17PerReleaseChannelConfig\x12 \n\x0frelease_channel\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12&\n\x10\x63ustom_hostnames\x18\x02 \x03(\tB\x0c\xfa\x42\t\x92\x01\x06\"\x04r\x02h\x01\x12W\n\x08programs\x18\x05 \x03(\x0b\x32\x36.prodvana.common_config.PerReleaseChannelProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12+\n\x04\x63\x65rt\x18\x06 \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12:\n\x0f\x64\x65livery_config\x18\x07 \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x08 \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\t \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x43\n\x0epre_push_tasks\x18\n \x03(\x0b\x32\x1c.prodvana.service.TaskConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x41\n\x10runtime_specific\x18\x0b \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x41\n\x0fgeneric_runtime\x18\r \x01(\x0b\x32&.prodvana.service.GenericRuntimeConfigH\x00\x12\x41\n\x0f\x65xternal_config\x18\x0e \x01(\x0b\x32&.prodvana.common_config.ExternalConfigH\x00\x12\x32\n\x04helm\x18\x0f \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x0c\x10\rR\x0bprotections\",\n\x13\x43\x61pabilityReference\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"U\n\x18\x43ompiledCapabilityConfig\x12\x39\n\ncapability\x18\x01 \x01(\x0b\x32%.prodvana.capability.CapabilityConfig\".\n\x10ProgramReference\x12\x0e\n\x04name\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"6\n\rTaskReference\x12\x19\n\x0frelease_channel\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"\xf1\x01\n\nTaskConfig\x12@\n\x07program\x18\x01 \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x38\n\x0c\x62\x61se_program\x18\x02 \x01(\x0b\x32\".prodvana.service.ProgramReference\x12\x39\n\x0cretry_config\x18\x03 \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12,\n\x03ref\x18\x04 \x01(\x0b\x32\x1f.prodvana.service.TaskReference\"\x9c\x02\n\x15RuntimeSpecificConfig\x12@\n\x03k8s\x18\x01 \x01(\x0b\x32\x31.prodvana.service.RuntimeSpecificConfig.K8SConfigH\x00\x1a\xae\x01\n\tK8SConfig\x12\x66\n\x13service_annotations\x18\x01 \x03(\x0b\x32I.prodvana.service.RuntimeSpecificConfig.K8SConfig.ServiceAnnotationsEntry\x1a\x39\n\x17ServiceAnnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x10\n\x0eruntime_config\"\x16\n\x14GenericRuntimeConfig\"&\n\x12\x41utoRollbackConfig\x12\x10\n\x08\x64isabled\x18\x01 \x01(\x08\"\xec\x01\n\x1fProtectionConvergenceAttachment\x12:\n\x04name\x18\x01 \x01(\tB,\xfa\x42)r\'\x10\x00\x18?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$\x12?\n\x03ref\x18\x02 \x01(\x0b\x32(.prodvana.protection.ProtectionReferenceB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12L\n\tlifecycle\x18\x03 \x03(\x0b\x32(.prodvana.protection.ProtectionLifecycleB\x0f\xfa\x42\x0c\x92\x01\t\x08\x01\"\x05\x8a\x01\x02\x10\x01\"\xfc\x0b\n\rServiceConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\x13\n\x0b\x61pplication\x18\x14 \x01(\t\x12\x46\n\x08programs\x18\x02 \x03(\x0b\x32%.prodvana.common_config.ProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x41\n\x10release_strategy\x18\x05 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12U\n\x13per_release_channel\x18\t \x03(\x0b\x32).prodvana.service.PerReleaseChannelConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12J\n\x0c\x63\x61pabilities\x18\n \x03(\x0b\x32%.prodvana.service.CapabilityReferenceB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12:\n\x0f\x64\x65livery_config\x18\x0b \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0c \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\r \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x41\n\rbase_template\x18\x0e \x01(\x0b\x32*.prodvana.common_config.ServiceTemplateRef\x12\x34\n\x0epre_push_tasks\x18\x0f \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x41\n\x10runtime_specific\x18\x10 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12N\n\nparameters\x18\x15 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x42\n\x10parameter_values\x18\x16 \x01(\x0b\x32(.prodvana.service.ServiceParameterValues\x12\x34\n\x11progress_deadline\x18\x18 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x41\n\x0fgeneric_runtime\x18\x12 \x01(\x0b\x32&.prodvana.service.GenericRuntimeConfigH\x00\x12\x41\n\x0f\x65xternal_config\x18\x13 \x01(\x0b\x32&.prodvana.common_config.ExternalConfigH\x00\x12\x32\n\x04helm\x18\x1a \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12M\n\x12parameters_autogen\x18\x17 \x01(\x0e\x32\x31.prodvana.service.ServiceConfig.ParametersAutogen\x12;\n\rauto_rollback\x18\x19 \x01(\x0b\x32$.prodvana.service.AutoRollbackConfig\"M\n\x11ParametersAutogen\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\t\n\x05IMAGE\x10\x02\x12\x16\n\x12IMAGE_AND_REPLICAS\x10\x03\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\x11\x10\x12R\x08\x65xternalR\x10image_repositoryR\x15\x63ontainer_registry_idR\x0bprotections\"\xc1\x0c\n\x1d\x43ompiledServiceInstanceConfig\x12\x0f\n\x07service\x18\x01 \x01(\t\x12\x13\n\x0b\x61pplication\x18\x12 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x32\n\x08maturity\x18\x05 \x01(\x0e\x32 .prodvana.common_config.Maturity\x12\x41\n\x10release_strategy\x18\x06 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12\x18\n\x10\x63ustom_hostnames\x18\x07 \x03(\t\x12+\n\x04\x63\x65rt\x18\n \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12\x46\n\x07runtime\x18\x0b \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x1b \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12@\n\x0c\x63\x61pabilities\x18\x0c \x03(\x0b\x32*.prodvana.service.CompiledCapabilityConfig\x12:\n\x0f\x64\x65livery_config\x18\r \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0e \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\x0f \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x41\n\rbase_template\x18\x10 \x01(\x0b\x32*.prodvana.common_config.ServiceTemplateRef\x12\x34\n\x0epre_push_tasks\x18\x11 \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x41\n\x10runtime_specific\x18\x13 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12?\n\nparameters\x18\x18 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinition\x12@\n\x10parameter_values\x18\x19 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x12\x34\n\x11progress_deadline\x18\x1a \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x41\n\x0fgeneric_runtime\x18\x16 \x01(\x0b\x32&.prodvana.service.GenericRuntimeConfigH\x00\x12\x41\n\x0f\x65xternal_config\x18\x17 \x01(\x0b\x32&.prodvana.common_config.ExternalConfigH\x00\x12\x32\n\x04helm\x18\x1d \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12n\n\x03\x65nv\x18\x1c \x03(\x0b\x32\x38.prodvana.service.CompiledServiceInstanceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\x14\x10\x15J\x04\x08\x15\x10\x16R\x0bprotectionsR\x0cruntime_type\"\x88\x02\n\x11\x43ompiledJobConfig\x12\x13\n\x0bname_prefix\x18\x01 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x46\n\x07runtime\x18\x04 \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x05 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfigBLZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/serviceb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%prodvana/service/service_config.proto\x12\x10prodvana.service\x1a\x1egoogle/protobuf/duration.proto\x1a$prodvana/capability/capability.proto\x1a prodvana/common_config/env.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a!prodvana/common_config/helm.proto\x1a%prodvana/common_config/maturity.proto\x1a\'prodvana/common_config/parameters.proto\x1a$prodvana/common_config/program.proto\x1a prodvana/common_config/ref.proto\x1a\"prodvana/common_config/retry.proto\x1a\'prodvana/delivery/delivery_config.proto\x1a.prodvana/protection/protection_reference.proto\x1a\x35prodvana/release_channel/release_channel_config.proto\x1a\'prodvana/runtimes/runtimes_config.proto\x1a*prodvana/workflow/integration_config.proto\x1a!prodvana/service/parameters.proto\x1a\x1eprodvana/volumes/volumes.proto\x1a\x17validate/validate.proto\"1\n\x0eReplicasConfig\x12\x0f\n\x05\x66ixed\x18\x01 \x01(\x05H\x00\x42\x0e\n\x0c\x63onfig_oneof\"\xaa\x02\n\x0eMetricAnalysis\x12J\n\x0csuccess_rate\x18\x02 \x01(\x0b\x32\x32.prodvana.service.MetricAnalysis.SuccessRateConfigH\x00\x12\x45\n\x0blatency_p95\x18\x03 \x01(\x0b\x32..prodvana.service.MetricAnalysis.LatencyConfigH\x00\x1a\x32\n\x11SuccessRateConfig\x12\x1d\n\x15min_threshold_percent\x18\x01 \x01(\x01\x1a?\n\rLatencyConfig\x12.\n\x0bmax_latency\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x10\n\x0e\x61nalysis_oneof\"\xb7\x02\n\x15ReleaseStrategyConfig\x12<\n\x19individual_stage_deadline\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x1a\x61utomated_testing_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12:\n\x10metrics_analysis\x18\x03 \x03(\x0b\x32 .prodvana.service.MetricAnalysis\x12\x17\n\x0fmanual_approval\x18\x04 \x01(\x08\x12\x31\n\x0e\x63heck_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x19\n\x11\x66\x61ilure_threshold\x18\x06 \x01(\x05\"f\n\tTLSSecret\x12\x14\n\nraw_secret\x18\x03 \x01(\tH\x00\x12\x30\n\x06secret\x18\x04 \x01(\x0b\x32\x1e.prodvana.common_config.SecretH\x00\x42\x11\n\ntls_secret\x12\x03\xf8\x42\x01\"\x81\x01\n\x0eTLSCertificate\x12\x37\n\x08tls_cert\x18\x01 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x36\n\x07tls_key\x18\x02 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\"j\n\x0b\x43\x65rtificate\x12/\n\x03tls\x18\x01 \x01(\x0b\x32 .prodvana.service.TLSCertificateH\x00\x12\x16\n\x0c\x61ws_acm_cert\x18\x02 \x01(\tH\x00\x42\x12\n\x0b\x63\x65rtificate\x12\x03\xf8\x42\x01\"\xe9\x06\n\x17PerReleaseChannelConfig\x12 \n\x0frelease_channel\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12&\n\x10\x63ustom_hostnames\x18\x02 \x03(\tB\x0c\xfa\x42\t\x92\x01\x06\"\x04r\x02h\x01\x12W\n\x08programs\x18\x05 \x03(\x0b\x32\x36.prodvana.common_config.PerReleaseChannelProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12+\n\x04\x63\x65rt\x18\x06 \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12:\n\x0f\x64\x65livery_config\x18\x07 \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x08 \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\t \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x43\n\x0epre_push_tasks\x18\n \x03(\x0b\x32\x1c.prodvana.service.TaskConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x41\n\x10runtime_specific\x18\x0b \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x11 \x01(\t\x12\x41\n\x0fgeneric_runtime\x18\r \x01(\x0b\x32&.prodvana.service.GenericRuntimeConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x0e \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x10 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x0f \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x0c\x10\rR\x0bprotections\",\n\x13\x43\x61pabilityReference\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"U\n\x18\x43ompiledCapabilityConfig\x12\x39\n\ncapability\x18\x01 \x01(\x0b\x32%.prodvana.capability.CapabilityConfig\".\n\x10ProgramReference\x12\x0e\n\x04name\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"6\n\rTaskReference\x12\x19\n\x0frelease_channel\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"\xf1\x01\n\nTaskConfig\x12@\n\x07program\x18\x01 \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x38\n\x0c\x62\x61se_program\x18\x02 \x01(\x0b\x32\".prodvana.service.ProgramReference\x12\x39\n\x0cretry_config\x18\x03 \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12,\n\x03ref\x18\x04 \x01(\x0b\x32\x1f.prodvana.service.TaskReference\"\x9c\x02\n\x15RuntimeSpecificConfig\x12@\n\x03k8s\x18\x01 \x01(\x0b\x32\x31.prodvana.service.RuntimeSpecificConfig.K8SConfigH\x00\x1a\xae\x01\n\tK8SConfig\x12\x66\n\x13service_annotations\x18\x01 \x03(\x0b\x32I.prodvana.service.RuntimeSpecificConfig.K8SConfig.ServiceAnnotationsEntry\x1a\x39\n\x17ServiceAnnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x10\n\x0eruntime_config\"X\n\x14GenericRuntimeConfig\x12@\n\x10parameter_values\x18\x01 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\"&\n\x12\x41utoRollbackConfig\x12\x10\n\x08\x64isabled\x18\x01 \x01(\x08\"\xec\x01\n\x1fProtectionConvergenceAttachment\x12:\n\x04name\x18\x01 \x01(\tB,\xfa\x42)r\'\x10\x00\x18?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$\x12?\n\x03ref\x18\x02 \x01(\x0b\x32(.prodvana.protection.ProtectionReferenceB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12L\n\tlifecycle\x18\x03 \x03(\x0b\x32(.prodvana.protection.ProtectionLifecycleB\x0f\xfa\x42\x0c\x92\x01\t\x08\x01\"\x05\x8a\x01\x02\x10\x01\"\xe1\x0c\n\rServiceConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\x13\n\x0b\x61pplication\x18\x14 \x01(\t\x12\x46\n\x08programs\x18\x02 \x03(\x0b\x32%.prodvana.common_config.ProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x41\n\x10release_strategy\x18\x05 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12U\n\x13per_release_channel\x18\t \x03(\x0b\x32).prodvana.service.PerReleaseChannelConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12J\n\x0c\x63\x61pabilities\x18\n \x03(\x0b\x32%.prodvana.service.CapabilityReferenceB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12:\n\x0f\x64\x65livery_config\x18\x0b \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0c \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\r \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x41\n\rbase_template\x18\x0e \x01(\x0b\x32*.prodvana.common_config.ServiceTemplateRef\x12\x34\n\x0epre_push_tasks\x18\x0f \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x41\n\x10runtime_specific\x18\x10 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x1c \x01(\t\x12N\n\nparameters\x18\x15 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x42\n\x10parameter_values\x18\x16 \x01(\x0b\x32(.prodvana.service.ServiceParameterValues\x12\x34\n\x11progress_deadline\x18\x18 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x41\n\x0fgeneric_runtime\x18\x12 \x01(\x0b\x32&.prodvana.service.GenericRuntimeConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x13 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x1b \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1a \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12M\n\x12parameters_autogen\x18\x17 \x01(\x0e\x32\x31.prodvana.service.ServiceConfig.ParametersAutogen\x12;\n\rauto_rollback\x18\x19 \x01(\x0b\x32$.prodvana.service.AutoRollbackConfig\"M\n\x11ParametersAutogen\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\t\n\x05IMAGE\x10\x02\x12\x16\n\x12IMAGE_AND_REPLICAS\x10\x03\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\x11\x10\x12R\x08\x65xternalR\x10image_repositoryR\x15\x63ontainer_registry_idR\x0bprotections\"\xc5\x0c\n\x1d\x43ompiledServiceInstanceConfig\x12\x0f\n\x07service\x18\x01 \x01(\t\x12\x13\n\x0b\x61pplication\x18\x12 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x32\n\x08maturity\x18\x05 \x01(\x0e\x32 .prodvana.common_config.Maturity\x12\x41\n\x10release_strategy\x18\x06 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12\x18\n\x10\x63ustom_hostnames\x18\x07 \x03(\t\x12+\n\x04\x63\x65rt\x18\n \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12\x46\n\x07runtime\x18\x0b \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x1b \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12@\n\x0c\x63\x61pabilities\x18\x0c \x03(\x0b\x32*.prodvana.service.CompiledCapabilityConfig\x12:\n\x0f\x64\x65livery_config\x18\r \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0e \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\x0f \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x41\n\rbase_template\x18\x10 \x01(\x0b\x32*.prodvana.common_config.ServiceTemplateRef\x12\x34\n\x0epre_push_tasks\x18\x11 \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x41\n\x10runtime_specific\x18\x13 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12?\n\nparameters\x18\x18 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinition\x12@\n\x10parameter_values\x18\x19 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x12\x34\n\x11progress_deadline\x18\x1a \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x41\n\x0fgeneric_runtime\x18\x16 \x01(\x0b\x32&.prodvana.service.GenericRuntimeConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x17 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1d \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12n\n\x03\x65nv\x18\x1c \x03(\x0b\x32\x38.prodvana.service.CompiledServiceInstanceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\x14\x10\x15J\x04\x08\x15\x10\x16R\x0bprotectionsR\x0cruntime_type\"\x88\x02\n\x11\x43ompiledJobConfig\x12\x13\n\x0bname_prefix\x18\x01 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x46\n\x07runtime\x18\x04 \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x05 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfigBLZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/serviceb\x06proto3')
 
 
 
 _REPLICASCONFIG = DESCRIPTOR.message_types_by_name['ReplicasConfig']
 _METRICANALYSIS = DESCRIPTOR.message_types_by_name['MetricAnalysis']
 _METRICANALYSIS_SUCCESSRATECONFIG = _METRICANALYSIS.nested_types_by_name['SuccessRateConfig']
 _METRICANALYSIS_LATENCYCONFIG = _METRICANALYSIS.nested_types_by_name['LatencyConfig']
@@ -286,58 +286,58 @@
   _SERVICECONFIG.fields_by_name['parameters']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
   _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._options = None
   _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._serialized_options = b'8\001'
   _COMPILEDSERVICEINSTANCECONFIG.fields_by_name['volumes']._options = None
   _COMPILEDSERVICEINSTANCECONFIG.fields_by_name['volumes']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
   _COMPILEDSERVICEINSTANCECONFIG.fields_by_name['env']._options = None
   _COMPILEDSERVICEINSTANCECONFIG.fields_by_name['env']._serialized_options = b'\372B$\232\001!\030\001\"\035r\0332\031^[a-zA-Z_]+[a-zA-Z0-9_]*$'
-  _REPLICASCONFIG._serialized_start=753
-  _REPLICASCONFIG._serialized_end=802
-  _METRICANALYSIS._serialized_start=805
-  _METRICANALYSIS._serialized_end=1103
-  _METRICANALYSIS_SUCCESSRATECONFIG._serialized_start=970
-  _METRICANALYSIS_SUCCESSRATECONFIG._serialized_end=1020
-  _METRICANALYSIS_LATENCYCONFIG._serialized_start=1022
-  _METRICANALYSIS_LATENCYCONFIG._serialized_end=1085
-  _RELEASESTRATEGYCONFIG._serialized_start=1106
-  _RELEASESTRATEGYCONFIG._serialized_end=1417
-  _TLSSECRET._serialized_start=1419
-  _TLSSECRET._serialized_end=1521
-  _TLSCERTIFICATE._serialized_start=1524
-  _TLSCERTIFICATE._serialized_end=1653
-  _CERTIFICATE._serialized_start=1655
-  _CERTIFICATE._serialized_end=1761
-  _PERRELEASECHANNELCONFIG._serialized_start=1764
-  _PERRELEASECHANNELCONFIG._serialized_end=2536
-  _CAPABILITYREFERENCE._serialized_start=2538
-  _CAPABILITYREFERENCE._serialized_end=2582
-  _COMPILEDCAPABILITYCONFIG._serialized_start=2584
-  _COMPILEDCAPABILITYCONFIG._serialized_end=2669
-  _PROGRAMREFERENCE._serialized_start=2671
-  _PROGRAMREFERENCE._serialized_end=2717
-  _TASKREFERENCE._serialized_start=2719
-  _TASKREFERENCE._serialized_end=2773
-  _TASKCONFIG._serialized_start=2776
-  _TASKCONFIG._serialized_end=3017
-  _RUNTIMESPECIFICCONFIG._serialized_start=3020
-  _RUNTIMESPECIFICCONFIG._serialized_end=3304
-  _RUNTIMESPECIFICCONFIG_K8SCONFIG._serialized_start=3112
-  _RUNTIMESPECIFICCONFIG_K8SCONFIG._serialized_end=3286
-  _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._serialized_start=3229
-  _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._serialized_end=3286
-  _GENERICRUNTIMECONFIG._serialized_start=3306
-  _GENERICRUNTIMECONFIG._serialized_end=3328
-  _AUTOROLLBACKCONFIG._serialized_start=3330
-  _AUTOROLLBACKCONFIG._serialized_end=3368
-  _PROTECTIONCONVERGENCEATTACHMENT._serialized_start=3371
-  _PROTECTIONCONVERGENCEATTACHMENT._serialized_end=3607
-  _SERVICECONFIG._serialized_start=3610
-  _SERVICECONFIG._serialized_end=5142
-  _SERVICECONFIG_PARAMETERSAUTOGEN._serialized_start=4961
-  _SERVICECONFIG_PARAMETERSAUTOGEN._serialized_end=5038
-  _COMPILEDSERVICEINSTANCECONFIG._serialized_start=5145
-  _COMPILEDSERVICEINSTANCECONFIG._serialized_end=6746
-  _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._serialized_start=6603
-  _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._serialized_end=6679
-  _COMPILEDJOBCONFIG._serialized_start=6749
-  _COMPILEDJOBCONFIG._serialized_end=7013
+  _REPLICASCONFIG._serialized_start=755
+  _REPLICASCONFIG._serialized_end=804
+  _METRICANALYSIS._serialized_start=807
+  _METRICANALYSIS._serialized_end=1105
+  _METRICANALYSIS_SUCCESSRATECONFIG._serialized_start=972
+  _METRICANALYSIS_SUCCESSRATECONFIG._serialized_end=1022
+  _METRICANALYSIS_LATENCYCONFIG._serialized_start=1024
+  _METRICANALYSIS_LATENCYCONFIG._serialized_end=1087
+  _RELEASESTRATEGYCONFIG._serialized_start=1108
+  _RELEASESTRATEGYCONFIG._serialized_end=1419
+  _TLSSECRET._serialized_start=1421
+  _TLSSECRET._serialized_end=1523
+  _TLSCERTIFICATE._serialized_start=1526
+  _TLSCERTIFICATE._serialized_end=1655
+  _CERTIFICATE._serialized_start=1657
+  _CERTIFICATE._serialized_end=1763
+  _PERRELEASECHANNELCONFIG._serialized_start=1766
+  _PERRELEASECHANNELCONFIG._serialized_end=2639
+  _CAPABILITYREFERENCE._serialized_start=2641
+  _CAPABILITYREFERENCE._serialized_end=2685
+  _COMPILEDCAPABILITYCONFIG._serialized_start=2687
+  _COMPILEDCAPABILITYCONFIG._serialized_end=2772
+  _PROGRAMREFERENCE._serialized_start=2774
+  _PROGRAMREFERENCE._serialized_end=2820
+  _TASKREFERENCE._serialized_start=2822
+  _TASKREFERENCE._serialized_end=2876
+  _TASKCONFIG._serialized_start=2879
+  _TASKCONFIG._serialized_end=3120
+  _RUNTIMESPECIFICCONFIG._serialized_start=3123
+  _RUNTIMESPECIFICCONFIG._serialized_end=3407
+  _RUNTIMESPECIFICCONFIG_K8SCONFIG._serialized_start=3215
+  _RUNTIMESPECIFICCONFIG_K8SCONFIG._serialized_end=3389
+  _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._serialized_start=3332
+  _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._serialized_end=3389
+  _GENERICRUNTIMECONFIG._serialized_start=3409
+  _GENERICRUNTIMECONFIG._serialized_end=3497
+  _AUTOROLLBACKCONFIG._serialized_start=3499
+  _AUTOROLLBACKCONFIG._serialized_end=3537
+  _PROTECTIONCONVERGENCEATTACHMENT._serialized_start=3540
+  _PROTECTIONCONVERGENCEATTACHMENT._serialized_end=3776
+  _SERVICECONFIG._serialized_start=3779
+  _SERVICECONFIG._serialized_end=5412
+  _SERVICECONFIG_PARAMETERSAUTOGEN._serialized_start=5231
+  _SERVICECONFIG_PARAMETERSAUTOGEN._serialized_end=5308
+  _COMPILEDSERVICEINSTANCECONFIG._serialized_start=5415
+  _COMPILEDSERVICEINSTANCECONFIG._serialized_end=7020
+  _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._serialized_start=6877
+  _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._serialized_end=6953
+  _COMPILEDJOBCONFIG._serialized_start=7023
+  _COMPILEDJOBCONFIG._serialized_end=7287
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/service/service_config_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/service/service_config_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import google.protobuf.descriptor
 import google.protobuf.duration_pb2
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import prodvana.proto.prodvana.capability.capability_pb2
 import prodvana.proto.prodvana.common_config.env_pb2
-import prodvana.proto.prodvana.common_config.external_config_pb2
 import prodvana.proto.prodvana.common_config.helm_pb2
+import prodvana.proto.prodvana.common_config.kubernetes_config_pb2
 import prodvana.proto.prodvana.common_config.maturity_pb2
 import prodvana.proto.prodvana.common_config.parameters_pb2
 import prodvana.proto.prodvana.common_config.program_pb2
 import prodvana.proto.prodvana.common_config.ref_pb2
 import prodvana.proto.prodvana.common_config.retry_pb2
 import prodvana.proto.prodvana.delivery.delivery_config_pb2
 import prodvana.proto.prodvana.protection.protection_reference_pb2
@@ -209,15 +209,17 @@
     PROGRAMS_FIELD_NUMBER: builtins.int
     CERT_FIELD_NUMBER: builtins.int
     DELIVERY_CONFIG_FIELD_NUMBER: builtins.int
     VOLUMES_FIELD_NUMBER: builtins.int
     REPLICAS_FIELD_NUMBER: builtins.int
     PRE_PUSH_TASKS_FIELD_NUMBER: builtins.int
     RUNTIME_SPECIFIC_FIELD_NUMBER: builtins.int
+    RUNTIME_CONNECTION_FIELD_NUMBER: builtins.int
     GENERIC_RUNTIME_FIELD_NUMBER: builtins.int
+    KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
     EXTERNAL_CONFIG_FIELD_NUMBER: builtins.int
     HELM_FIELD_NUMBER: builtins.int
     release_channel: builtins.str
     @property
     def custom_hostnames(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     @property
     def programs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.program_pb2.PerReleaseChannelProgramConfig]: ...
@@ -229,39 +231,48 @@
     def volumes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.volumes.volumes_pb2.Volume]: ...
     @property
     def replicas(self) -> global___ReplicasConfig: ...
     @property
     def pre_push_tasks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TaskConfig]: ...
     @property
     def runtime_specific(self) -> global___RuntimeSpecificConfig: ...
+    runtime_connection: builtins.str
+    """which runtime connection to use in each release channel.
+    optional if only one runtime makes sense for the service config.
+    """
     @property
     def generic_runtime(self) -> global___GenericRuntimeConfig: ...
     @property
-    def external_config(self) -> prodvana.proto.prodvana.common_config.external_config_pb2.ExternalConfig: ...
+    def kubernetes_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig: ...
+    @property
+    def external_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig:
+        """deprecated, pass this as kubernetes_config instead"""
     @property
     def helm(self) -> prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig: ...
     def __init__(
         self,
         *,
         release_channel: builtins.str = ...,
         custom_hostnames: collections.abc.Iterable[builtins.str] | None = ...,
         programs: collections.abc.Iterable[prodvana.proto.prodvana.common_config.program_pb2.PerReleaseChannelProgramConfig] | None = ...,
         cert: global___Certificate | None = ...,
         delivery_config: prodvana.proto.prodvana.delivery.delivery_config_pb2.DeliveryConfig | None = ...,
         volumes: collections.abc.Iterable[prodvana.proto.prodvana.volumes.volumes_pb2.Volume] | None = ...,
         replicas: global___ReplicasConfig | None = ...,
         pre_push_tasks: collections.abc.Iterable[global___TaskConfig] | None = ...,
         runtime_specific: global___RuntimeSpecificConfig | None = ...,
+        runtime_connection: builtins.str = ...,
         generic_runtime: global___GenericRuntimeConfig | None = ...,
-        external_config: prodvana.proto.prodvana.common_config.external_config_pb2.ExternalConfig | None = ...,
+        kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
+        external_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         helm: prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["cert", b"cert", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "external_config", b"external_config", "generic_runtime", b"generic_runtime", "helm", b"helm", "replicas", b"replicas", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cert", b"cert", "config_oneof", b"config_oneof", "custom_hostnames", b"custom_hostnames", "delivery_config", b"delivery_config", "external_config", b"external_config", "generic_runtime", b"generic_runtime", "helm", b"helm", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "release_channel", b"release_channel", "replicas", b"replicas", "runtime_specific", b"runtime_specific", "volumes", b"volumes"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["generic_runtime", "external_config", "helm"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["cert", b"cert", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "external_config", b"external_config", "generic_runtime", b"generic_runtime", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "replicas", b"replicas", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["cert", b"cert", "config_oneof", b"config_oneof", "custom_hostnames", b"custom_hostnames", "delivery_config", b"delivery_config", "external_config", b"external_config", "generic_runtime", b"generic_runtime", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "release_channel", b"release_channel", "replicas", b"replicas", "runtime_connection", b"runtime_connection", "runtime_specific", b"runtime_specific", "volumes", b"volumes"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["generic_runtime", "kubernetes_config", "external_config", "helm"] | None: ...
 
 global___PerReleaseChannelConfig = PerReleaseChannelConfig
 
 class CapabilityReference(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
@@ -408,21 +419,25 @@
     def HasField(self, field_name: typing_extensions.Literal["k8s", b"k8s", "runtime_config", b"runtime_config"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["k8s", b"k8s", "runtime_config", b"runtime_config"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["runtime_config", b"runtime_config"]) -> typing_extensions.Literal["k8s"] | None: ...
 
 global___RuntimeSpecificConfig = RuntimeSpecificConfig
 
 class GenericRuntimeConfig(google.protobuf.message.Message):
-    """TODO(naphat) put parameters here"""
-
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    PARAMETER_VALUES_FIELD_NUMBER: builtins.int
+    @property
+    def parameter_values(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue]: ...
     def __init__(
         self,
+        *,
+        parameter_values: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue] | None = ...,
     ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["parameter_values", b"parameter_values"]) -> None: ...
 
 global___GenericRuntimeConfig = GenericRuntimeConfig
 
 class AutoRollbackConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DISABLED_FIELD_NUMBER: builtins.int
@@ -495,18 +510,20 @@
     CAPABILITIES_FIELD_NUMBER: builtins.int
     DELIVERY_CONFIG_FIELD_NUMBER: builtins.int
     VOLUMES_FIELD_NUMBER: builtins.int
     DEPLOY_ANNOTATIONS_FIELD_NUMBER: builtins.int
     BASE_TEMPLATE_FIELD_NUMBER: builtins.int
     PRE_PUSH_TASKS_FIELD_NUMBER: builtins.int
     RUNTIME_SPECIFIC_FIELD_NUMBER: builtins.int
+    RUNTIME_CONNECTION_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
     PARAMETER_VALUES_FIELD_NUMBER: builtins.int
     PROGRESS_DEADLINE_FIELD_NUMBER: builtins.int
     GENERIC_RUNTIME_FIELD_NUMBER: builtins.int
+    KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
     EXTERNAL_CONFIG_FIELD_NUMBER: builtins.int
     HELM_FIELD_NUMBER: builtins.int
     PARAMETERS_AUTOGEN_FIELD_NUMBER: builtins.int
     AUTO_ROLLBACK_FIELD_NUMBER: builtins.int
     name: builtins.str
     application: builtins.str
     @property
@@ -527,26 +544,33 @@
     def deploy_annotations(self) -> prodvana.proto.prodvana.workflow.integration_config_pb2.AnnotationsConfig: ...
     @property
     def base_template(self) -> prodvana.proto.prodvana.common_config.ref_pb2.ServiceTemplateRef: ...
     @property
     def pre_push_tasks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TaskConfig]: ...
     @property
     def runtime_specific(self) -> global___RuntimeSpecificConfig: ...
+    runtime_connection: builtins.str
+    """which runtime connection to use in each release channel.
+    optional if only one runtime makes sense for the service config.
+    """
     @property
     def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition]: ...
     @property
     def parameter_values(self) -> prodvana.proto.prodvana.service.parameters_pb2.ServiceParameterValues:
         """only valid to set in compiled configs by Prodvana"""
     @property
     def progress_deadline(self) -> google.protobuf.duration_pb2.Duration:
         """how long to wait before marking deployment as failed"""
     @property
     def generic_runtime(self) -> global___GenericRuntimeConfig: ...
     @property
-    def external_config(self) -> prodvana.proto.prodvana.common_config.external_config_pb2.ExternalConfig: ...
+    def kubernetes_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig: ...
+    @property
+    def external_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig:
+        """deprecated, pass this as kubernetes_config instead"""
     @property
     def helm(self) -> prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig: ...
     parameters_autogen: global___ServiceConfig.ParametersAutogen.ValueType
     """How to autogenerate parameters, defaults to IMAGE"""
     @property
     def auto_rollback(self) -> global___AutoRollbackConfig: ...
     def __init__(
@@ -561,26 +585,28 @@
         capabilities: collections.abc.Iterable[global___CapabilityReference] | None = ...,
         delivery_config: prodvana.proto.prodvana.delivery.delivery_config_pb2.DeliveryConfig | None = ...,
         volumes: collections.abc.Iterable[prodvana.proto.prodvana.volumes.volumes_pb2.Volume] | None = ...,
         deploy_annotations: prodvana.proto.prodvana.workflow.integration_config_pb2.AnnotationsConfig | None = ...,
         base_template: prodvana.proto.prodvana.common_config.ref_pb2.ServiceTemplateRef | None = ...,
         pre_push_tasks: collections.abc.Iterable[global___TaskConfig] | None = ...,
         runtime_specific: global___RuntimeSpecificConfig | None = ...,
+        runtime_connection: builtins.str = ...,
         parameters: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition] | None = ...,
         parameter_values: prodvana.proto.prodvana.service.parameters_pb2.ServiceParameterValues | None = ...,
         progress_deadline: google.protobuf.duration_pb2.Duration | None = ...,
         generic_runtime: global___GenericRuntimeConfig | None = ...,
-        external_config: prodvana.proto.prodvana.common_config.external_config_pb2.ExternalConfig | None = ...,
+        kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
+        external_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         helm: prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig | None = ...,
         parameters_autogen: global___ServiceConfig.ParametersAutogen.ValueType = ...,
         auto_rollback: global___AutoRollbackConfig | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["auto_rollback", b"auto_rollback", "base_template", b"base_template", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "external_config", b"external_config", "generic_runtime", b"generic_runtime", "helm", b"helm", "parameter_values", b"parameter_values", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "auto_rollback", b"auto_rollback", "base_template", b"base_template", "capabilities", b"capabilities", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "external_config", b"external_config", "generic_runtime", b"generic_runtime", "helm", b"helm", "name", b"name", "parameter_values", b"parameter_values", "parameters", b"parameters", "parameters_autogen", b"parameters_autogen", "per_release_channel", b"per_release_channel", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime_specific", b"runtime_specific", "volumes", b"volumes"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["generic_runtime", "external_config", "helm"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["auto_rollback", b"auto_rollback", "base_template", b"base_template", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "external_config", b"external_config", "generic_runtime", b"generic_runtime", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "parameter_values", b"parameter_values", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "auto_rollback", b"auto_rollback", "base_template", b"base_template", "capabilities", b"capabilities", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "external_config", b"external_config", "generic_runtime", b"generic_runtime", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "name", b"name", "parameter_values", b"parameter_values", "parameters", b"parameters", "parameters_autogen", b"parameters_autogen", "per_release_channel", b"per_release_channel", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime_connection", b"runtime_connection", "runtime_specific", b"runtime_specific", "volumes", b"volumes"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["generic_runtime", "kubernetes_config", "external_config", "helm"] | None: ...
 
 global___ServiceConfig = ServiceConfig
 
 class CompiledServiceInstanceConfig(google.protobuf.message.Message):
     """a compiled version of ServiceConfig specific to a service instance, with release-channel configs applied"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
@@ -620,15 +646,15 @@
     BASE_TEMPLATE_FIELD_NUMBER: builtins.int
     PRE_PUSH_TASKS_FIELD_NUMBER: builtins.int
     RUNTIME_SPECIFIC_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
     PARAMETER_VALUES_FIELD_NUMBER: builtins.int
     PROGRESS_DEADLINE_FIELD_NUMBER: builtins.int
     GENERIC_RUNTIME_FIELD_NUMBER: builtins.int
-    EXTERNAL_CONFIG_FIELD_NUMBER: builtins.int
+    KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
     HELM_FIELD_NUMBER: builtins.int
     ENV_FIELD_NUMBER: builtins.int
     service: builtins.str
     application: builtins.str
     release_channel: builtins.str
     @property
     def programs(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.program_pb2.ProgramConfig]: ...
@@ -665,15 +691,15 @@
     def parameter_values(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue]: ...
     @property
     def progress_deadline(self) -> google.protobuf.duration_pb2.Duration:
         """how long to wait before marking deployment as failed"""
     @property
     def generic_runtime(self) -> global___GenericRuntimeConfig: ...
     @property
-    def external_config(self) -> prodvana.proto.prodvana.common_config.external_config_pb2.ExternalConfig: ...
+    def kubernetes_config(self) -> prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig: ...
     @property
     def helm(self) -> prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig: ...
     @property
     def env(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue]:
         """The compiled environment for this instance's context, e.g.  Release Channel.
         This is used to inject these values into external configs.
         """
@@ -698,21 +724,21 @@
         base_template: prodvana.proto.prodvana.common_config.ref_pb2.ServiceTemplateRef | None = ...,
         pre_push_tasks: collections.abc.Iterable[global___TaskConfig] | None = ...,
         runtime_specific: global___RuntimeSpecificConfig | None = ...,
         parameters: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition] | None = ...,
         parameter_values: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue] | None = ...,
         progress_deadline: google.protobuf.duration_pb2.Duration | None = ...,
         generic_runtime: global___GenericRuntimeConfig | None = ...,
-        external_config: prodvana.proto.prodvana.common_config.external_config_pb2.ExternalConfig | None = ...,
+        kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         helm: prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig | None = ...,
         env: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["base_template", b"base_template", "cert", b"cert", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "external_config", b"external_config", "generic_runtime", b"generic_runtime", "helm", b"helm", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime", b"runtime", "runtime_execution", b"runtime_execution", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "base_template", b"base_template", "capabilities", b"capabilities", "cert", b"cert", "config_oneof", b"config_oneof", "custom_hostnames", b"custom_hostnames", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "env", b"env", "external_config", b"external_config", "generic_runtime", b"generic_runtime", "helm", b"helm", "maturity", b"maturity", "parameter_values", b"parameter_values", "parameters", b"parameters", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "release_channel", b"release_channel", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime", b"runtime", "runtime_execution", b"runtime_execution", "runtime_specific", b"runtime_specific", "service", b"service", "volumes", b"volumes"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["generic_runtime", "external_config", "helm"] | None: ...
+    def HasField(self, field_name: typing_extensions.Literal["base_template", b"base_template", "cert", b"cert", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "generic_runtime", b"generic_runtime", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime", b"runtime", "runtime_execution", b"runtime_execution", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "base_template", b"base_template", "capabilities", b"capabilities", "cert", b"cert", "config_oneof", b"config_oneof", "custom_hostnames", b"custom_hostnames", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "env", b"env", "generic_runtime", b"generic_runtime", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "maturity", b"maturity", "parameter_values", b"parameter_values", "parameters", b"parameters", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "release_channel", b"release_channel", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime", b"runtime", "runtime_execution", b"runtime_execution", "runtime_specific", b"runtime_specific", "service", b"service", "volumes", b"volumes"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["generic_runtime", "kubernetes_config", "helm"] | None: ...
 
 global___CompiledServiceInstanceConfig = CompiledServiceInstanceConfig
 
 class CompiledJobConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_PREFIX_FIELD_NUMBER: builtins.int
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/service/service_manager_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/service/service_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/service/service_manager_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/service/service_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py` & `prodvana-0.1.5/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/service/user_metadata_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/service/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/service/user_metadata_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/service/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/settings/organization/users_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/settings/organization/users_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/settings/organization/users_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/settings/organization/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py` & `prodvana-0.1.5/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/stat/efficiency_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/stat/efficiency_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/stat/efficiency_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/stat/efficiency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/template/service_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/template/service_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/template/service_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/template/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/users/users_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/users/users_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/users/users_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/users/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/version/source_metadata_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/version/source_metadata_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -23,22 +23,30 @@
 class _SourceEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_Source.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     UNKNOWN_SOURCE: _Source.ValueType  # 0
     WEB: _Source.ValueType  # 1
     INTERACTIVE_PVNCTL: _Source.ValueType  # 2
     CONFIG_FILE: _Source.ValueType  # 3
     REPO_FOLLOW: _Source.ValueType  # 4
+    PRODVANA: _Source.ValueType  # 5
+    """this source indicates this version was provided by Prodvana
+    this is used for things like builtin Protections or other first party provided features
+    """
 
 class Source(_Source, metaclass=_SourceEnumTypeWrapper): ...
 
 UNKNOWN_SOURCE: Source.ValueType  # 0
 WEB: Source.ValueType  # 1
 INTERACTIVE_PVNCTL: Source.ValueType  # 2
 CONFIG_FILE: Source.ValueType  # 3
 REPO_FOLLOW: Source.ValueType  # 4
+PRODVANA: Source.ValueType  # 5
+"""this source indicates this version was provided by Prodvana
+this is used for things like builtin Protections or other first party provided features
+"""
 global___Source = Source
 
 class SourceMetadata(google.protobuf.message.Message):
     """all of these fields are optional and only set if it makes sense for a given source."""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/volumes/volumes_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/volumes/volumes_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/volumes/volumes_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/volumes/volumes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/workflow/integration_config_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/workflow/integration_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py` & `prodvana-0.1.5/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py` & `prodvana-0.1.5/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi` & `prodvana-0.1.5/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/validate/validate_pb2.py` & `prodvana-0.1.5/prodvana/proto/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/proto/validate/validate_pb2.pyi` & `prodvana-0.1.5/prodvana/proto/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/utils/desired_states.py` & `prodvana-0.1.5/prodvana/utils/desired_states.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/utils/service_config.py` & `prodvana-0.1.5/prodvana/utils/service_config.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/prodvana/utils/tests/test_service_config.py` & `prodvana-0.1.5/prodvana/utils/tests/test_service_config.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.4/pyproject.toml` & `prodvana-0.1.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prodvana"
-version = "0.1.4"
+version = "0.1.5"
 description = "Prodvana's client libraries"
 readme = "README.md"
 authors = []
 homepage = "https://prodvana.io"
 documentation = "https://docs.prodvana.io"
 repository = "https://github.com/prodvana/prodvana-public"
 exclude = ["examples"]
@@ -14,16 +14,16 @@
 protobuf = ">=4.21.0,<5.0"
 types-protobuf = ">=3.20.0,<5.0"
 grpcio = ">=1.48.0,<2.0"
 grpc-stubs = ">=1.24.0,<2.0"
 grpc-interceptor = "^0.15.0"
 google-api-python-client = ">=2.58.0,<3.0"
 
-[tool.poetry.dev-dependencies]
-mypy = "^0.961"
+[tool.poetry.group.dev.dependencies]
+mypy = "1.3.0"
 pytest = "^7.1.2"
 mock = "^4.0.3"
 types-mock = "^4.0.15"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `prodvana-0.1.4/PKG-INFO` & `prodvana-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodvana
-Version: 0.1.4
+Version: 0.1.5
 Summary: Prodvana's client libraries
 Home-page: https://prodvana.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: google-api-python-client (>=2.58.0,<3.0)
```

