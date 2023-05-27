# Comparing `tmp/compose-py-0.2.0.tar.gz` & `tmp/compose-py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compose-py-0.2.0.tar", last modified: Tue May 23 15:49:17 2023, max compression
+gzip compressed data, was "compose-py-0.3.0.tar", last modified: Sat May 27 06:16:25 2023, max compression
```

## Comparing `compose-py-0.2.0.tar` & `compose-py-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-05-23 15:49:17.957051 compose-py-0.2.0/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1070 2023-05-21 01:42:57.000000 compose-py-0.2.0/LICENSE
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3791 2023-05-23 15:49:17.957051 compose-py-0.2.0/PKG-INFO
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1946 2023-05-23 15:47:09.000000 compose-py-0.2.0/README.md
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-05-23 15:49:17.957051 compose-py-0.2.0/compose_py/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      170 2023-05-23 15:47:09.000000 compose-py-0.2.0/compose_py/__init__.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       79 2023-05-23 15:13:52.000000 compose-py-0.2.0/compose_py/_types.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       22 2023-05-23 15:49:03.000000 compose-py-0.2.0/compose_py/_version.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      733 2023-05-23 15:46:51.000000 compose-py-0.2.0/compose_py/_yaml.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3713 2023-05-23 15:47:09.000000 compose-py-0.2.0/compose_py/dumper.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2704 2023-05-23 15:47:09.000000 compose-py-0.2.0/compose_py/loader.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       99 2023-05-21 04:25:58.000000 compose-py-0.2.0/compose_py/model_type.py
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-05-23 15:49:17.957051 compose-py-0.2.0/compose_py/models_dataclasses/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1054 2023-05-21 08:33:20.000000 compose-py-0.2.0/compose_py/models_dataclasses/__init__.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    12265 2023-05-23 15:13:52.000000 compose-py-0.2.0/compose_py/models_dataclasses/_generated.py
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-05-23 15:49:17.957051 compose-py-0.2.0/compose_py/models_pydantic/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      972 2023-05-21 08:33:31.000000 compose-py-0.2.0/compose_py/models_pydantic/__init__.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    15492 2023-05-23 15:13:52.000000 compose-py-0.2.0/compose_py/models_pydantic/_generated.py
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2023-05-21 01:43:11.000000 compose-py-0.2.0/compose_py/py.typed
-drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-05-23 15:49:17.957051 compose-py-0.2.0/compose_py.egg-info/
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3791 2023-05-23 15:49:17.000000 compose-py-0.2.0/compose_py.egg-info/PKG-INFO
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      541 2023-05-23 15:49:17.000000 compose-py-0.2.0/compose_py.egg-info/SOURCES.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        1 2023-05-23 15:49:17.000000 compose-py-0.2.0/compose_py.egg-info/dependency_links.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      205 2023-05-23 15:49:17.000000 compose-py-0.2.0/compose_py.egg-info/requires.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       11 2023-05-23 15:49:17.000000 compose-py-0.2.0/compose_py.egg-info/top_level.txt
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1174 2023-05-23 15:13:52.000000 compose-py-0.2.0/pyproject.toml
--rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       38 2023-05-23 15:49:17.957051 compose-py-0.2.0/setup.cfg
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-05-27 06:16:25.741704 compose-py-0.3.0/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1070 2023-05-21 01:42:57.000000 compose-py-0.3.0/LICENSE
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3849 2023-05-27 06:16:25.741704 compose-py-0.3.0/PKG-INFO
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2004 2023-05-27 06:08:01.000000 compose-py-0.3.0/README.md
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-05-27 06:16:25.741704 compose-py-0.3.0/compose_py/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      170 2023-05-23 15:47:09.000000 compose-py-0.3.0/compose_py/__init__.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       79 2023-05-23 15:13:52.000000 compose-py-0.3.0/compose_py/_types.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       22 2023-05-27 06:15:57.000000 compose-py-0.3.0/compose_py/_version.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      733 2023-05-23 15:46:51.000000 compose-py-0.3.0/compose_py/_yaml.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3713 2023-05-23 15:47:09.000000 compose-py-0.3.0/compose_py/dumper.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2704 2023-05-23 15:47:09.000000 compose-py-0.3.0/compose_py/loader.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       99 2023-05-21 04:25:58.000000 compose-py-0.3.0/compose_py/model_type.py
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-05-27 06:16:25.741704 compose-py-0.3.0/compose_py/models_dataclasses/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1054 2023-05-21 08:33:20.000000 compose-py-0.3.0/compose_py/models_dataclasses/__init__.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    13084 2023-05-27 05:52:59.000000 compose-py-0.3.0/compose_py/models_dataclasses/_generated.py
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-05-27 06:16:25.741704 compose-py-0.3.0/compose_py/models_pydantic/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      972 2023-05-21 08:33:31.000000 compose-py-0.3.0/compose_py/models_pydantic/__init__.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    16287 2023-05-27 05:52:59.000000 compose-py-0.3.0/compose_py/models_pydantic/_generated.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2023-05-21 01:43:11.000000 compose-py-0.3.0/compose_py/py.typed
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-05-27 06:16:25.741704 compose-py-0.3.0/compose_py.egg-info/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3849 2023-05-27 06:16:25.000000 compose-py-0.3.0/compose_py.egg-info/PKG-INFO
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      541 2023-05-27 06:16:25.000000 compose-py-0.3.0/compose_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        1 2023-05-27 06:16:25.000000 compose-py-0.3.0/compose_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      205 2023-05-27 06:16:25.000000 compose-py-0.3.0/compose_py.egg-info/requires.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       11 2023-05-27 06:16:25.000000 compose-py-0.3.0/compose_py.egg-info/top_level.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1186 2023-05-27 06:08:01.000000 compose-py-0.3.0/pyproject.toml
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       38 2023-05-27 06:16:25.741704 compose-py-0.3.0/setup.cfg
```

### Comparing `compose-py-0.2.0/LICENSE` & `compose-py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `compose-py-0.2.0/PKG-INFO` & `compose-py-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compose-py
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python library for parsing and loading Compose files
 Author-email: Yuki Igarashi <me@bonprosoft.com>
 License: MIT License
         
         Copyright (c) 2023 Yuki Igarashi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -100,7 +100,11 @@
 print(compose_py.dump_yaml_str(obj))
 with open("docker-compose-modified.yml", "w") as f:
     compose_py.dump_yaml(obj, f, model=compose_py.ModelType.DATACLASSES)
 ```
 
 You can find more APIs under `compose_py.models_dataclasses` package.
 
+## Examples
+
+See `examples/` directory to find examples.
+
```

### Comparing `compose-py-0.2.0/README.md` & `compose-py-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -61,7 +61,11 @@
 print(compose_py.dump_yaml_str(obj))
 with open("docker-compose-modified.yml", "w") as f:
     compose_py.dump_yaml(obj, f, model=compose_py.ModelType.DATACLASSES)
 ```
 
 You can find more APIs under `compose_py.models_dataclasses` package.
 
+## Examples
+
+See `examples/` directory to find examples.
+
```

### Comparing `compose-py-0.2.0/compose_py/_yaml.py` & `compose-py-0.3.0/compose_py/_yaml.py`

 * *Files identical despite different names*

### Comparing `compose-py-0.2.0/compose_py/dumper.py` & `compose-py-0.3.0/compose_py/dumper.py`

 * *Files identical despite different names*

### Comparing `compose-py-0.2.0/compose_py/loader.py` & `compose-py-0.3.0/compose_py/loader.py`

 * *Files identical despite different names*

### Comparing `compose-py-0.2.0/compose_py/models_dataclasses/__init__.py` & `compose-py-0.3.0/compose_py/models_dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `compose-py-0.2.0/compose_py/models_dataclasses/_generated.py` & `compose-py-0.3.0/compose_py/models_dataclasses/_generated.py`

 * *Files 8% similar despite different names*

```diff
@@ -171,17 +171,14 @@
 
 
 @dataclass
 class GenericResource:
     discrete_resource_spec: Optional[DiscreteResourceSpec] = None
 
 
-GenericResources = List[GenericResource]
-
-
 @dataclass
 class ConfigItem:
     subnet: Optional[str] = None
     ip_range: Optional[str] = None
     gateway: Optional[str] = None
     aux_addresses: Optional[Dict[str, str]] = None
 
@@ -194,23 +191,14 @@
 
 
 @dataclass
 class External:
     name: Optional[str] = None
 
 
-Command = Optional[Union[str, List[str]]]
-
-
-ListOfStrings = List[str]
-
-
-ListOrDict = Union[Dict[str, Optional[Union[str, float, bool]]], List[str]]
-
-
 @dataclass
 class BlkioLimit:
     path: Optional[str] = None
     rate: Optional[Union[int, str]] = None
 
 
 @dataclass
@@ -224,40 +212,45 @@
     source: Optional[str] = None
     target: Optional[str] = None
     uid: Optional[str] = None
     gid: Optional[str] = None
     mode: Optional[float] = None
 
 
-ServiceConfigOrSecret = List[Union[str, ServiceConfigOrSecretItem]]
-
-
 Constraints = Any
 
 
 @dataclass
 class BuildItem:
     context: Optional[str] = None
     dockerfile: Optional[str] = None
     dockerfile_inline: Optional[str] = None
-    args: Optional[ListOrDict] = None
-    ssh: Optional[ListOrDict] = None
-    labels: Optional[ListOrDict] = None
+    args: Optional[
+        Union[Dict[str, Optional[Union[str, float, bool]]], List[str]]
+    ] = None
+    ssh: Optional[Union[Dict[str, Optional[Union[str, float, bool]]], List[str]]] = None
+    labels: Optional[
+        Union[Dict[str, Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     cache_from: Optional[List[str]] = None
     cache_to: Optional[List[str]] = None
     no_cache: Optional[bool] = None
-    additional_contexts: Optional[ListOrDict] = None
+    additional_contexts: Optional[
+        Union[Dict[str, Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     network: Optional[str] = None
     pull: Optional[bool] = None
     target: Optional[str] = None
     shm_size: Optional[Union[int, str]] = None
-    extra_hosts: Optional[ListOrDict] = None
+    extra_hosts: Optional[
+        Union[Dict[str, Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     isolation: Optional[str] = None
     privileged: Optional[bool] = None
-    secrets: Optional[ServiceConfigOrSecret] = None
+    secrets: Optional[List[Union[str, ServiceConfigOrSecretItem]]] = None
     tags: Optional[List[str]] = None
     platforms: Optional[List[str]] = None
 
 
 @dataclass
 class BlkioConfig:
     device_read_bps: Optional[List[BlkioLimit]] = None
@@ -266,182 +259,198 @@
     device_write_iops: Optional[List[BlkioLimit]] = None
     weight: Optional[int] = None
     weight_device: Optional[List[BlkioWeight]] = None
 
 
 @dataclass
 class Network1:
-    aliases: Optional[ListOfStrings] = None
+    aliases: Optional[List[str]] = None
     ipv4_address: Optional[str] = None
     ipv6_address: Optional[str] = None
-    link_local_ips: Optional[ListOfStrings] = None
+    link_local_ips: Optional[List[str]] = None
     priority: Optional[float] = None
 
 
 @dataclass
 class Device:
-    capabilities: Optional[ListOfStrings] = None
+    capabilities: Optional[List[str]] = None
     count: Optional[Union[str, int]] = None
-    device_ids: Optional[ListOfStrings] = None
+    device_ids: Optional[List[str]] = None
     driver: Optional[str] = None
-    options: Optional[ListOrDict] = None
-
-
-Devices = List[Device]
+    options: Optional[
+        Union[Dict[str, Optional[Union[str, float, bool]]], List[str]]
+    ] = None
 
 
 @dataclass
 class Network:
     name: Optional[str] = None
     driver: Optional[str] = None
     driver_opts: Optional[Dict[str, Union[str, float]]] = None
     ipam: Optional[Ipam] = None
     external: Optional[External] = None
     internal: Optional[bool] = None
     enable_ipv6: Optional[bool] = None
     attachable: Optional[bool] = None
-    labels: Optional[ListOrDict] = None
+    labels: Optional[
+        Union[Dict[str, Optional[Union[str, float, bool]]], List[str]]
+    ] = None
 
 
 @dataclass
 class Volume:
     name: Optional[str] = None
     driver: Optional[str] = None
     driver_opts: Optional[Dict[str, Union[str, float]]] = None
     external: Optional[External] = None
-    labels: Optional[ListOrDict] = None
+    labels: Optional[
+        Union[Dict[str, Optional[Union[str, float, bool]]], List[str]]
+    ] = None
 
 
 @dataclass
 class Secret:
     name: Optional[str] = None
     environment: Optional[str] = None
     file: Optional[str] = None
     external: Optional[External] = None
-    labels: Optional[ListOrDict] = None
+    labels: Optional[
+        Union[Dict[str, Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     driver: Optional[str] = None
     driver_opts: Optional[Dict[str, Union[str, float]]] = None
     template_driver: Optional[str] = None
 
 
 @dataclass
 class Config:
     name: Optional[str] = None
     file: Optional[str] = None
     external: Optional[External] = None
-    labels: Optional[ListOrDict] = None
+    labels: Optional[
+        Union[Dict[str, Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     template_driver: Optional[str] = None
 
 
-StringOrList = Union[str, ListOfStrings]
-
-
 @dataclass
 class Reservations:
     cpus: Optional[Union[float, str]] = None
     memory: Optional[str] = None
-    generic_resources: Optional[GenericResources] = None
-    devices: Optional[Devices] = None
+    generic_resources: Optional[List[GenericResource]] = None
+    devices: Optional[List[Device]] = None
 
 
 @dataclass
 class Resources:
     limits: Optional[Limits] = None
     reservations: Optional[Reservations] = None
 
 
 @dataclass
 class Deployment:
     mode: Optional[str] = None
     endpoint_mode: Optional[str] = None
     replicas: Optional[int] = None
-    labels: Optional[ListOrDict] = None
+    labels: Optional[
+        Union[Dict[str, Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     rollback_config: Optional[RollbackConfig] = None
     update_config: Optional[UpdateConfig] = None
     resources: Optional[Resources] = None
     restart_policy: Optional[RestartPolicy] = None
     placement: Optional[Placement] = None
 
 
 @dataclass
 class Service:
     deploy: Optional[Deployment] = None
-    annotations: Optional[ListOrDict] = None
+    annotations: Optional[
+        Union[Dict[str, Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     build: Optional[Union[str, BuildItem]] = None
     blkio_config: Optional[BlkioConfig] = None
     cap_add: Optional[List[str]] = None
     cap_drop: Optional[List[str]] = None
     cgroup: Optional[Cgroup] = None
     cgroup_parent: Optional[str] = None
-    command: Optional[Command] = None
-    configs: Optional[ServiceConfigOrSecret] = None
+    command: Optional[Union[str, List[str]]] = None
+    configs: Optional[List[Union[str, ServiceConfigOrSecretItem]]] = None
     container_name: Optional[str] = None
     cpu_count: Optional[int] = None
     cpu_percent: Optional[int] = None
     cpu_shares: Optional[Union[float, str]] = None
     cpu_quota: Optional[Union[float, str]] = None
     cpu_period: Optional[Union[float, str]] = None
     cpu_rt_period: Optional[Union[float, str]] = None
     cpu_rt_runtime: Optional[Union[float, str]] = None
     cpus: Optional[Union[float, str]] = None
     cpuset: Optional[str] = None
     credential_spec: Optional[CredentialSpec] = None
-    depends_on: Optional[Union[ListOfStrings, Dict[str, DependsOn]]] = None
-    device_cgroup_rules: Optional[ListOfStrings] = None
+    depends_on: Optional[Union[Dict[str, DependsOn], List[str]]] = None
+    device_cgroup_rules: Optional[List[str]] = None
     devices: Optional[List[str]] = None
-    dns: Optional[StringOrList] = None
+    dns: Optional[Union[str, List[str]]] = None
     dns_opt: Optional[List[str]] = None
-    dns_search: Optional[StringOrList] = None
+    dns_search: Optional[Union[str, List[str]]] = None
     domainname: Optional[str] = None
-    entrypoint: Optional[Command] = None
-    env_file: Optional[StringOrList] = None
-    environment: Optional[ListOrDict] = None
+    entrypoint: Optional[Union[str, List[str]]] = None
+    env_file: Optional[Union[str, List[str]]] = None
+    environment: Optional[
+        Union[Dict[str, Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     expose: Optional[List[Union[str, float]]] = None
     extends: Optional[Union[str, Extend]] = None
     external_links: Optional[List[str]] = None
-    extra_hosts: Optional[ListOrDict] = None
+    extra_hosts: Optional[
+        Union[Dict[str, Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     group_add: Optional[List[Union[str, float]]] = None
     healthcheck: Optional[Healthcheck] = None
     hostname: Optional[str] = None
     image: Optional[str] = None
     init: Optional[bool] = None
     ipc: Optional[str] = None
     isolation: Optional[str] = None
-    labels: Optional[ListOrDict] = None
+    labels: Optional[
+        Union[Dict[str, Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     links: Optional[List[str]] = None
     logging: Optional[Logging] = None
     mac_address: Optional[str] = None
     mem_limit: Optional[Union[float, str]] = None
     mem_reservation: Optional[Union[str, int]] = None
     mem_swappiness: Optional[int] = None
     memswap_limit: Optional[Union[float, str]] = None
     network_mode: Optional[str] = None
-    networks: Optional[Union[ListOfStrings, Dict[str, Optional[Network1]]]] = None
+    networks: Optional[Union[Dict[str, Optional[Network1]], List[str]]] = None
     oom_kill_disable: Optional[bool] = None
     oom_score_adj: Optional[int] = None
     pid: Optional[str] = None
     pids_limit: Optional[Union[float, str]] = None
     platform: Optional[str] = None
     ports: Optional[List[Union[float, str, Port]]] = None
     privileged: Optional[bool] = None
-    profiles: Optional[ListOfStrings] = None
+    profiles: Optional[List[str]] = None
     pull_policy: Optional[PullPolicy] = None
     read_only: Optional[bool] = None
     restart: Optional[str] = None
     runtime: Optional[str] = None
     scale: Optional[int] = None
     security_opt: Optional[List[str]] = None
     shm_size: Optional[Union[float, str]] = None
-    secrets: Optional[ServiceConfigOrSecret] = None
-    sysctls: Optional[ListOrDict] = None
+    secrets: Optional[List[Union[str, ServiceConfigOrSecretItem]]] = None
+    sysctls: Optional[
+        Union[Dict[str, Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     stdin_open: Optional[bool] = None
     stop_grace_period: Optional[str] = None
     stop_signal: Optional[str] = None
     storage_opt: Optional[Dict[str, Any]] = None
-    tmpfs: Optional[StringOrList] = None
+    tmpfs: Optional[Union[str, List[str]]] = None
     tty: Optional[bool] = None
     ulimits: Optional[Dict[str, Union[int, Ulimit]]] = None
     user: Optional[str] = None
     uts: Optional[str] = None
     userns_mode: Optional[str] = None
     volumes: Optional[List[Union[str, Volume1]]] = None
     volumes_from: Optional[List[str]] = None
```

### Comparing `compose-py-0.2.0/compose_py/models_pydantic/__init__.py` & `compose-py-0.3.0/compose_py/models_pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `compose-py-0.2.0/compose_py/models_pydantic/_generated.py` & `compose-py-0.3.0/compose_py/models_pydantic/_generated.py`

 * *Files 5% similar despite different names*

```diff
@@ -210,18 +210,14 @@
 class GenericResource(BaseModel):
     class Config:
         extra = Extra.forbid
 
     discrete_resource_spec: Optional[DiscreteResourceSpec] = None
 
 
-class GenericResources(BaseModel):
-    __root__: List[GenericResource]
-
-
 class ConfigItem(BaseModel):
     class Config:
         extra = Extra.forbid
 
     subnet: Optional[str] = None
     ip_range: Optional[str] = None
     gateway: Optional[str] = None
@@ -244,28 +240,14 @@
     name: Optional[str] = None
 
 
 class External2(BaseModel):
     name: Optional[str] = None
 
 
-class Command(BaseModel):
-    __root__: Optional[Union[str, List[str]]]
-
-
-class ListOfStrings(BaseModel):
-    __root__: List[str] = Field(..., unique_items=True)
-
-
-class ListOrDict(BaseModel):
-    __root__: Union[
-        Dict[constr(regex=r'.+'), Optional[Union[str, float, bool]]], List[str]
-    ]
-
-
 class BlkioLimit(BaseModel):
     class Config:
         extra = Extra.forbid
 
     path: Optional[str] = None
     rate: Optional[Union[int, str]] = None
 
@@ -285,44 +267,50 @@
     source: Optional[str] = None
     target: Optional[str] = None
     uid: Optional[str] = None
     gid: Optional[str] = None
     mode: Optional[float] = None
 
 
-class ServiceConfigOrSecret(BaseModel):
-    __root__: List[Union[str, ServiceConfigOrSecretItem]]
-
-
 class Constraints(BaseModel):
     __root__: Any
 
 
 class BuildItem(BaseModel):
     class Config:
         extra = Extra.forbid
 
     context: Optional[str] = None
     dockerfile: Optional[str] = None
     dockerfile_inline: Optional[str] = None
-    args: Optional[ListOrDict] = None
-    ssh: Optional[ListOrDict] = None
-    labels: Optional[ListOrDict] = None
+    args: Optional[
+        Union[Dict[constr(regex=r'.+'), Optional[Union[str, float, bool]]], List[str]]
+    ] = None
+    ssh: Optional[
+        Union[Dict[constr(regex=r'.+'), Optional[Union[str, float, bool]]], List[str]]
+    ] = None
+    labels: Optional[
+        Union[Dict[constr(regex=r'.+'), Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     cache_from: Optional[List[str]] = None
     cache_to: Optional[List[str]] = None
     no_cache: Optional[bool] = None
-    additional_contexts: Optional[ListOrDict] = None
+    additional_contexts: Optional[
+        Union[Dict[constr(regex=r'.+'), Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     network: Optional[str] = None
     pull: Optional[bool] = None
     target: Optional[str] = None
     shm_size: Optional[Union[int, str]] = None
-    extra_hosts: Optional[ListOrDict] = None
+    extra_hosts: Optional[
+        Union[Dict[constr(regex=r'.+'), Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     isolation: Optional[str] = None
     privileged: Optional[bool] = None
-    secrets: Optional[ServiceConfigOrSecret] = None
+    secrets: Optional[List[Union[str, ServiceConfigOrSecretItem]]] = None
     tags: Optional[List[str]] = None
     platforms: Optional[List[str]] = None
 
 
 class BlkioConfig(BaseModel):
     class Config:
         extra = Extra.forbid
@@ -335,99 +323,101 @@
     weight_device: Optional[List[BlkioWeight]] = None
 
 
 class Network1(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    aliases: Optional[ListOfStrings] = None
+    aliases: Optional[List[str]] = None
     ipv4_address: Optional[str] = None
     ipv6_address: Optional[str] = None
-    link_local_ips: Optional[ListOfStrings] = None
+    link_local_ips: Optional[List[str]] = None
     priority: Optional[float] = None
 
 
 class Device(BaseModel):
     class Config:
         extra = Extra.forbid
 
-    capabilities: Optional[ListOfStrings] = None
+    capabilities: Optional[List[str]] = None
     count: Optional[Union[str, int]] = None
-    device_ids: Optional[ListOfStrings] = None
+    device_ids: Optional[List[str]] = None
     driver: Optional[str] = None
-    options: Optional[ListOrDict] = None
-
-
-class Devices(BaseModel):
-    __root__: List[Device]
+    options: Optional[
+        Union[Dict[constr(regex=r'.+'), Optional[Union[str, float, bool]]], List[str]]
+    ] = None
 
 
 class Network(BaseModel):
     class Config:
         extra = Extra.forbid
 
     name: Optional[str] = None
     driver: Optional[str] = None
     driver_opts: Optional[Dict[constr(regex=r'^.+$'), Union[str, float]]] = None
     ipam: Optional[Ipam] = None
     external: Optional[External] = None
     internal: Optional[bool] = None
     enable_ipv6: Optional[bool] = None
     attachable: Optional[bool] = None
-    labels: Optional[ListOrDict] = None
+    labels: Optional[
+        Union[Dict[constr(regex=r'.+'), Optional[Union[str, float, bool]]], List[str]]
+    ] = None
 
 
 class Volume(BaseModel):
     class Config:
         extra = Extra.forbid
 
     name: Optional[str] = None
     driver: Optional[str] = None
     driver_opts: Optional[Dict[constr(regex=r'^.+$'), Union[str, float]]] = None
     external: Optional[External] = None
-    labels: Optional[ListOrDict] = None
+    labels: Optional[
+        Union[Dict[constr(regex=r'.+'), Optional[Union[str, float, bool]]], List[str]]
+    ] = None
 
 
 class Secret(BaseModel):
     class Config:
         extra = Extra.forbid
 
     name: Optional[str] = None
     environment: Optional[str] = None
     file: Optional[str] = None
     external: Optional[External2] = None
-    labels: Optional[ListOrDict] = None
+    labels: Optional[
+        Union[Dict[constr(regex=r'.+'), Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     driver: Optional[str] = None
     driver_opts: Optional[Dict[constr(regex=r'^.+$'), Union[str, float]]] = None
     template_driver: Optional[str] = None
 
 
 class Config(BaseModel):
     class Config:
         extra = Extra.forbid
 
     name: Optional[str] = None
     file: Optional[str] = None
     external: Optional[External2] = None
-    labels: Optional[ListOrDict] = None
+    labels: Optional[
+        Union[Dict[constr(regex=r'.+'), Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     template_driver: Optional[str] = None
 
 
-class StringOrList(BaseModel):
-    __root__: Union[str, ListOfStrings]
-
-
 class Reservations(BaseModel):
     class Config:
         extra = Extra.forbid
 
     cpus: Optional[Union[float, str]] = None
     memory: Optional[str] = None
-    generic_resources: Optional[GenericResources] = None
-    devices: Optional[Devices] = None
+    generic_resources: Optional[List[GenericResource]] = None
+    devices: Optional[List[Device]] = None
 
 
 class Resources(BaseModel):
     class Config:
         extra = Extra.forbid
 
     limits: Optional[Limits] = None
@@ -437,106 +427,116 @@
 class Deployment(BaseModel):
     class Config:
         extra = Extra.forbid
 
     mode: Optional[str] = None
     endpoint_mode: Optional[str] = None
     replicas: Optional[int] = None
-    labels: Optional[ListOrDict] = None
+    labels: Optional[
+        Union[Dict[constr(regex=r'.+'), Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     rollback_config: Optional[RollbackConfig] = None
     update_config: Optional[UpdateConfig] = None
     resources: Optional[Resources] = None
     restart_policy: Optional[RestartPolicy] = None
     placement: Optional[Placement] = None
 
 
 class Service(BaseModel):
     class Config:
         extra = Extra.forbid
 
     deploy: Optional[Deployment] = None
-    annotations: Optional[ListOrDict] = None
+    annotations: Optional[
+        Union[Dict[constr(regex=r'.+'), Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     build: Optional[Union[str, BuildItem]] = None
     blkio_config: Optional[BlkioConfig] = None
     cap_add: Optional[List[str]] = Field(None, unique_items=True)
     cap_drop: Optional[List[str]] = Field(None, unique_items=True)
     cgroup: Optional[Cgroup] = None
     cgroup_parent: Optional[str] = None
-    command: Optional[Command] = None
-    configs: Optional[ServiceConfigOrSecret] = None
+    command: Optional[Union[str, List[str]]] = None
+    configs: Optional[List[Union[str, ServiceConfigOrSecretItem]]] = None
     container_name: Optional[str] = None
     cpu_count: Optional[conint(ge=0)] = None
     cpu_percent: Optional[conint(ge=0, le=100)] = None
     cpu_shares: Optional[Union[float, str]] = None
     cpu_quota: Optional[Union[float, str]] = None
     cpu_period: Optional[Union[float, str]] = None
     cpu_rt_period: Optional[Union[float, str]] = None
     cpu_rt_runtime: Optional[Union[float, str]] = None
     cpus: Optional[Union[float, str]] = None
     cpuset: Optional[str] = None
     credential_spec: Optional[CredentialSpec] = None
     depends_on: Optional[
-        Union[ListOfStrings, Dict[constr(regex=r'^[a-zA-Z0-9._-]+$'), DependsOn]]
+        Union[Dict[constr(regex=r'^[a-zA-Z0-9._-]+$'), DependsOn], List[str]]
     ] = None
-    device_cgroup_rules: Optional[ListOfStrings] = None
+    device_cgroup_rules: Optional[List[str]] = None
     devices: Optional[List[str]] = Field(None, unique_items=True)
-    dns: Optional[StringOrList] = None
+    dns: Optional[Union[str, List[str]]] = None
     dns_opt: Optional[List[str]] = Field(None, unique_items=True)
-    dns_search: Optional[StringOrList] = None
+    dns_search: Optional[Union[str, List[str]]] = None
     domainname: Optional[str] = None
-    entrypoint: Optional[Command] = None
-    env_file: Optional[StringOrList] = None
-    environment: Optional[ListOrDict] = None
+    entrypoint: Optional[Union[str, List[str]]] = None
+    env_file: Optional[Union[str, List[str]]] = None
+    environment: Optional[
+        Union[Dict[constr(regex=r'.+'), Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     expose: Optional[List[Union[str, float]]] = Field(None, unique_items=True)
     extends: Optional[Union[str, Extend]] = None
     external_links: Optional[List[str]] = Field(None, unique_items=True)
-    extra_hosts: Optional[ListOrDict] = None
+    extra_hosts: Optional[
+        Union[Dict[constr(regex=r'.+'), Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     group_add: Optional[List[Union[str, float]]] = Field(None, unique_items=True)
     healthcheck: Optional[Healthcheck] = None
     hostname: Optional[str] = None
     image: Optional[str] = None
     init: Optional[bool] = None
     ipc: Optional[str] = None
     isolation: Optional[str] = None
-    labels: Optional[ListOrDict] = None
+    labels: Optional[
+        Union[Dict[constr(regex=r'.+'), Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     links: Optional[List[str]] = Field(None, unique_items=True)
     logging: Optional[Logging] = None
     mac_address: Optional[str] = None
     mem_limit: Optional[Union[float, str]] = None
     mem_reservation: Optional[Union[str, int]] = None
     mem_swappiness: Optional[int] = None
     memswap_limit: Optional[Union[float, str]] = None
     network_mode: Optional[str] = None
     networks: Optional[
-        Union[
-            ListOfStrings, Dict[constr(regex=r'^[a-zA-Z0-9._-]+$'), Optional[Network1]]
-        ]
+        Union[Dict[constr(regex=r'^[a-zA-Z0-9._-]+$'), Optional[Network1]], List[str]]
     ] = None
     oom_kill_disable: Optional[bool] = None
     oom_score_adj: Optional[conint(ge=-1000, le=1000)] = None
     pid: Optional[str] = None
     pids_limit: Optional[Union[float, str]] = None
     platform: Optional[str] = None
     ports: Optional[List[Union[float, str, Port]]] = Field(None, unique_items=True)
     privileged: Optional[bool] = None
-    profiles: Optional[ListOfStrings] = None
+    profiles: Optional[List[str]] = None
     pull_policy: Optional[PullPolicy] = None
     read_only: Optional[bool] = None
     restart: Optional[str] = None
     runtime: Optional[str] = None
     scale: Optional[int] = None
     security_opt: Optional[List[str]] = Field(None, unique_items=True)
     shm_size: Optional[Union[float, str]] = None
-    secrets: Optional[ServiceConfigOrSecret] = None
-    sysctls: Optional[ListOrDict] = None
+    secrets: Optional[List[Union[str, ServiceConfigOrSecretItem]]] = None
+    sysctls: Optional[
+        Union[Dict[constr(regex=r'.+'), Optional[Union[str, float, bool]]], List[str]]
+    ] = None
     stdin_open: Optional[bool] = None
     stop_grace_period: Optional[str] = None
     stop_signal: Optional[str] = None
     storage_opt: Optional[Dict[str, Any]] = None
-    tmpfs: Optional[StringOrList] = None
+    tmpfs: Optional[Union[str, List[str]]] = None
     tty: Optional[bool] = None
     ulimits: Optional[Dict[constr(regex=r'^[a-z]+$'), Union[int, Ulimit]]] = None
     user: Optional[str] = None
     uts: Optional[str] = None
     userns_mode: Optional[str] = None
     volumes: Optional[List[Union[str, Volume1]]] = Field(None, unique_items=True)
     volumes_from: Optional[List[str]] = Field(None, unique_items=True)
```

### Comparing `compose-py-0.2.0/compose_py.egg-info/PKG-INFO` & `compose-py-0.3.0/compose_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compose-py
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python library for parsing and loading Compose files
 Author-email: Yuki Igarashi <me@bonprosoft.com>
 License: MIT License
         
         Copyright (c) 2023 Yuki Igarashi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -100,7 +100,11 @@
 print(compose_py.dump_yaml_str(obj))
 with open("docker-compose-modified.yml", "w") as f:
     compose_py.dump_yaml(obj, f, model=compose_py.ModelType.DATACLASSES)
 ```
 
 You can find more APIs under `compose_py.models_dataclasses` package.
 
+## Examples
+
+See `examples/` directory to find examples.
+
```

### Comparing `compose-py-0.2.0/compose_py.egg-info/SOURCES.txt` & `compose-py-0.3.0/compose_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compose-py-0.2.0/pyproject.toml` & `compose-py-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,15 @@
   "mypy==1.3.0",
   "pysen==0.10.4",
   "pytest==7.3.1",
   "types-PyYAML==6.0.12.9",
 ]
 
 [tool.setuptools.packages.find]
-exclude = ["build", "tests"]
+exclude = ["build", "examples", "tests"]
 namespaces = false
 
 [tool.setuptools.package-data]
 "compose_py" = ["py.typed"]
 
 [tool.setuptools.dynamic]
 version = {attr = "compose_py._version.__version__"}
```

