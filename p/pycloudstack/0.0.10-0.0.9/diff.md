# Comparing `tmp/pycloudstack-0.0.10.tar.gz` & `tmp/pycloudstack-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycloudstack-0.0.10.tar", last modified: Sat May 27 12:47:12 2023, max compression
+gzip compressed data, was "pycloudstack-0.0.9.tar", last modified: Fri Feb 24 14:14:57 2023, max compression
```

## Comparing `pycloudstack-0.0.10.tar` & `pycloudstack-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 cpio      (1001) cpio      (1001)        0 2023-05-27 12:47:12.987546 pycloudstack-0.0.10/
--rw-r--r--   0 cpio      (1001) cpio      (1001)     3816 2023-05-27 12:47:12.987546 pycloudstack-0.0.10/PKG-INFO
--rw-r--r--   0 cpio      (1001) cpio      (1001)     3175 2023-04-19 11:33:32.000000 pycloudstack-0.0.10/README.md
-drwxr-xr-x   0 cpio      (1001) cpio      (1001)        0 2023-05-27 12:47:12.987546 pycloudstack-0.0.10/pycloudstack/
--rw-rw-r--   0 cpio      (1001) cpio      (1001)        0 2023-02-28 12:52:36.000000 pycloudstack-0.0.10/pycloudstack/__init__.py
--rw-rw-r--   0 cpio      (1001) cpio      (1001)    10924 2023-02-28 12:52:36.000000 pycloudstack-0.0.10/pycloudstack/artifacts.py
--rw-rw-r--   0 cpio      (1001) cpio      (1001)    14983 2023-02-28 12:52:36.000000 pycloudstack-0.0.10/pycloudstack/cluster.py
--rw-rw-r--   0 cpio      (1001) cpio      (1001)     4063 2023-02-28 12:52:36.000000 pycloudstack-0.0.10/pycloudstack/cmdrunner.py
--rw-rw-r--   0 cpio      (1001) cpio      (1001)     3637 2023-02-28 12:52:36.000000 pycloudstack-0.0.10/pycloudstack/dut.py
--rw-rw-r--   0 cpio      (1001) cpio      (1001)     2893 2023-02-28 12:52:36.000000 pycloudstack-0.0.10/pycloudstack/msr.py
--rw-rw-r--   0 cpio      (1001) cpio      (1001)     2454 2023-02-28 12:52:36.000000 pycloudstack-0.0.10/pycloudstack/registry.py
-drwxr-xr-x   0 cpio      (1001) cpio      (1001)        0 2023-05-27 12:47:12.987546 pycloudstack-0.0.10/pycloudstack/templates/
--rw-rw-r--   0 cpio      (1001) cpio      (1001)     2291 2023-02-28 12:52:36.000000 pycloudstack-0.0.10/pycloudstack/templates/legacy-base-perf.xml
--rw-rw-r--   0 cpio      (1001) cpio      (1001)     1768 2023-02-28 12:52:36.000000 pycloudstack-0.0.10/pycloudstack/templates/legacy-base.xml
--rw-rw-r--   0 cpio      (1001) cpio      (1001)     2294 2023-02-28 12:52:36.000000 pycloudstack-0.0.10/pycloudstack/templates/ovmf-base-perf.xml
--rw-rw-r--   0 cpio      (1001) cpio      (1001)     1771 2023-02-28 12:52:36.000000 pycloudstack-0.0.10/pycloudstack/templates/ovmf-base.xml
--rw-rw-r--   0 cpio      (1001) cpio      (1001)     1542 2023-02-28 12:52:36.000000 pycloudstack-0.0.10/pycloudstack/templates/sgx-base.xml
--rw-r--r--   0 cpio      (1001) cpio      (1001)     2326 2023-05-27 12:45:47.000000 pycloudstack-0.0.10/pycloudstack/templates/tdx-base-perf.xml
--rw-r--r--   0 cpio      (1001) cpio      (1001)     1803 2023-05-27 12:45:47.000000 pycloudstack-0.0.10/pycloudstack/templates/tdx-base.xml
--rw-r--r--   0 cpio      (1001) cpio      (1001)    24701 2023-05-05 09:53:03.000000 pycloudstack-0.0.10/pycloudstack/virtxml.py
--rw-r--r--   0 cpio      (1001) cpio      (1001)    13594 2023-05-27 12:45:47.000000 pycloudstack-0.0.10/pycloudstack/vmguest.py
--rw-rw-r--   0 cpio      (1001) cpio      (1001)     3634 2023-02-28 12:52:36.000000 pycloudstack-0.0.10/pycloudstack/vmimg.py
--rw-r--r--   0 cpio      (1001) cpio      (1001)    15817 2023-05-15 02:39:55.000000 pycloudstack-0.0.10/pycloudstack/vmm.py
--rw-r--r--   0 cpio      (1001) cpio      (1001)     5671 2023-05-27 12:45:47.000000 pycloudstack-0.0.10/pycloudstack/vmparam.py
-drwxr-xr-x   0 cpio      (1001) cpio      (1001)        0 2023-05-27 12:47:12.987546 pycloudstack-0.0.10/pycloudstack.egg-info/
--rw-r--r--   0 cpio      (1001) cpio      (1001)     3816 2023-05-27 12:47:12.000000 pycloudstack-0.0.10/pycloudstack.egg-info/PKG-INFO
--rw-r--r--   0 cpio      (1001) cpio      (1001)      758 2023-05-27 12:47:12.000000 pycloudstack-0.0.10/pycloudstack.egg-info/SOURCES.txt
--rw-r--r--   0 cpio      (1001) cpio      (1001)        1 2023-05-27 12:47:12.000000 pycloudstack-0.0.10/pycloudstack.egg-info/dependency_links.txt
--rw-r--r--   0 cpio      (1001) cpio      (1001)       87 2023-05-27 12:47:12.000000 pycloudstack-0.0.10/pycloudstack.egg-info/requires.txt
--rw-r--r--   0 cpio      (1001) cpio      (1001)       13 2023-05-27 12:47:12.000000 pycloudstack-0.0.10/pycloudstack.egg-info/top_level.txt
--rw-r--r--   0 cpio      (1001) cpio      (1001)      956 2023-05-27 12:45:47.000000 pycloudstack-0.0.10/pyproject.toml
--rw-r--r--   0 cpio      (1001) cpio      (1001)       38 2023-05-27 12:47:12.987546 pycloudstack-0.0.10/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:14:57.483751 pycloudstack-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-02-24 14:14:57.483751 pycloudstack-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:14:57.483751 pycloudstack-0.0.9/pycloudstack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pycloudstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pycloudstack/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14983 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pycloudstack/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pycloudstack/cmdrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pycloudstack/dut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pycloudstack/msr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pycloudstack/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:14:57.483751 pycloudstack-0.0.9/pycloudstack/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pycloudstack/templates/legacy-base-perf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pycloudstack/templates/legacy-base.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pycloudstack/templates/ovmf-base-perf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pycloudstack/templates/ovmf-base.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pycloudstack/templates/sgx-base.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pycloudstack/templates/tdx-base-perf.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pycloudstack/templates/tdx-base.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    24225 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pycloudstack/virtxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13515 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pycloudstack/vmguest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pycloudstack/vmimg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15767 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pycloudstack/vmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pycloudstack/vmparam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:14:57.483751 pycloudstack-0.0.9/pycloudstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-02-24 14:14:57.000000 pycloudstack-0.0.9/pycloudstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-02-24 14:14:57.000000 pycloudstack-0.0.9/pycloudstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 14:14:57.000000 pycloudstack-0.0.9/pycloudstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-24 14:14:57.000000 pycloudstack-0.0.9/pycloudstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-24 14:14:57.000000 pycloudstack-0.0.9/pycloudstack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-02-24 14:14:44.000000 pycloudstack-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 14:14:57.483751 pycloudstack-0.0.9/setup.cfg
```

### Comparing `pycloudstack-0.0.10/PKG-INFO` & `pycloudstack-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycloudstack
-Version: 0.0.10
+Version: 0.0.9
 Summary: Python package to manage hypervisor/docker/kubernetes stacks
 Author-email: Lu Ken <ken.lu@intel.com>, "Hao, Ruomeng" <ruomeng.hao@intel.com>
 License: Apache Software License
 Project-URL: Homepage, https://github.com/intel/tdx-tools
 Project-URL: Bug Tracker, https://github.com/intel/tdx-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,28 +16,28 @@
 
 # PyCloudStack (Unified Cloud Stack Operator Framework)
 
 ## 1. Overview
 
 PyCloudStack abstracts the common objects/operations/resources for diverse cloud
 architectures like hypervisor stack based on libvirt or direct qemu command,
-container stack orchestrated by Kubernetes or direct docker command, and the running
+container stack orchestrated by kubernetes or direct docker command, and the running
 or remote IaaS host.
 
 It can be used to create advance deployment CI/CD operator via python plugin for
 ansible, end-to-end validation framework with customized the components/configurations
 in full vertical stack.
 
 The architecture diagram is as follows:
 
 ![](https://github.com/intel/tdx-tools/blob/main/doc/pycloudstack.png)
 
 ## 2. Getting Start
 
-### Install from PyPI
+### Install from pypi
 
 ```
 pip3 install pycloudstack
 ```
 
 ### Install from source
 ```
@@ -79,15 +79,15 @@
 
 vm_factory = VMGuestFactory(vm_image, vm_kernel)
 inst = vm_factory.new_vm(vm_instance_type, vm_class=VMMQemu,
                          auto_start=True)
 inst.wait_for_ssh_ready()
 ```
 
-## Example 3: Operate Kubernetes Cluster
+## Example 3: Operate Kubenetes Cluster
 
 ```
 from pycloudstack.cluster import SGXCluster
 
 DEPLOYMENT_TEMPLATE='''
 apiVersion: apps/v1
 kind: Deployment
```

### Comparing `pycloudstack-0.0.10/README.md` & `pycloudstack-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 
 # PyCloudStack (Unified Cloud Stack Operator Framework)
 
 ## 1. Overview
 
 PyCloudStack abstracts the common objects/operations/resources for diverse cloud
 architectures like hypervisor stack based on libvirt or direct qemu command,
-container stack orchestrated by Kubernetes or direct docker command, and the running
+container stack orchestrated by kubernetes or direct docker command, and the running
 or remote IaaS host.
 
 It can be used to create advance deployment CI/CD operator via python plugin for
 ansible, end-to-end validation framework with customized the components/configurations
 in full vertical stack.
 
 The architecture diagram is as follows:
 
 ![](https://github.com/intel/tdx-tools/blob/main/doc/pycloudstack.png)
 
 ## 2. Getting Start
 
-### Install from PyPI
+### Install from pypi
 
 ```
 pip3 install pycloudstack
 ```
 
 ### Install from source
 ```
@@ -64,15 +64,15 @@
 
 vm_factory = VMGuestFactory(vm_image, vm_kernel)
 inst = vm_factory.new_vm(vm_instance_type, vm_class=VMMQemu,
                          auto_start=True)
 inst.wait_for_ssh_ready()
 ```
 
-## Example 3: Operate Kubernetes Cluster
+## Example 3: Operate Kubenetes Cluster
 
 ```
 from pycloudstack.cluster import SGXCluster
 
 DEPLOYMENT_TEMPLATE='''
 apiVersion: apps/v1
 kind: Deployment
@@ -125,8 +125,8 @@
 cluster_instance.create_service(
         svc_name,
         yaml.safe_load(SERVICE_TEMPLATE % {"name":svc_name}),
         TEST_NAMESPACE)
 cluster_instance.delete_service(svc_name, TEST_NAMESPACE)
 cluster_instance.delete_deployment(deploy_name, TEST_NAMESPACE)
 
-```
+```
```

### Comparing `pycloudstack-0.0.10/pycloudstack/artifacts.py` & `pycloudstack-0.0.9/pycloudstack/artifacts.py`

 * *Files identical despite different names*

### Comparing `pycloudstack-0.0.10/pycloudstack/cluster.py` & `pycloudstack-0.0.9/pycloudstack/cluster.py`

 * *Files identical despite different names*

### Comparing `pycloudstack-0.0.10/pycloudstack/cmdrunner.py` & `pycloudstack-0.0.9/pycloudstack/cmdrunner.py`

 * *Files identical despite different names*

### Comparing `pycloudstack-0.0.10/pycloudstack/dut.py` & `pycloudstack-0.0.9/pycloudstack/dut.py`

 * *Files identical despite different names*

### Comparing `pycloudstack-0.0.10/pycloudstack/msr.py` & `pycloudstack-0.0.9/pycloudstack/msr.py`

 * *Files identical despite different names*

### Comparing `pycloudstack-0.0.10/pycloudstack/registry.py` & `pycloudstack-0.0.9/pycloudstack/registry.py`

 * *Files identical despite different names*

### Comparing `pycloudstack-0.0.10/pycloudstack/templates/legacy-base-perf.xml` & `pycloudstack-0.0.9/pycloudstack/templates/legacy-base-perf.xml`

 * *Files identical despite different names*

### Comparing `pycloudstack-0.0.10/pycloudstack/templates/legacy-base.xml` & `pycloudstack-0.0.9/pycloudstack/templates/legacy-base.xml`

 * *Files identical despite different names*

### Comparing `pycloudstack-0.0.10/pycloudstack/templates/ovmf-base-perf.xml` & `pycloudstack-0.0.9/pycloudstack/templates/ovmf-base-perf.xml`

 * *Files identical despite different names*

### Comparing `pycloudstack-0.0.10/pycloudstack/templates/ovmf-base.xml` & `pycloudstack-0.0.9/pycloudstack/templates/ovmf-base.xml`

 * *Files identical despite different names*

### Comparing `pycloudstack-0.0.10/pycloudstack/templates/sgx-base.xml` & `pycloudstack-0.0.9/pycloudstack/templates/sgx-base.xml`

 * *Files identical despite different names*

### Comparing `pycloudstack-0.0.10/pycloudstack/templates/tdx-base-perf.xml` & `pycloudstack-0.0.9/pycloudstack/templates/tdx-base-perf.xml`

 * *Files identical despite different names*

### Comparing `pycloudstack-0.0.10/pycloudstack/templates/tdx-base.xml` & `pycloudstack-0.0.9/pycloudstack/templates/tdx-base.xml`

 * *Files identical despite different names*

### Comparing `pycloudstack-0.0.10/pycloudstack/virtxml.py` & `pycloudstack-0.0.9/pycloudstack/virtxml.py`

 * *Files 1% similar despite different names*

```diff
@@ -636,28 +636,14 @@
             allow_multi_same_leaf=True)
         self._add_new_element(
             [f"{QEMUS_NS}commandline", f"{QEMUS_NS}arg"],
             {"value": f"{cpu_param}"},
             allow_multi_same_leaf=True)
         self.save()
 
-    def set_overcommit_params(self, overcommit_param):
-        """
-        Set overcommit parameters
-        """
-        self._add_new_element(
-            [f"{QEMUS_NS}commandline", f"{QEMUS_NS}arg"],
-            {"value": "-overcommit"},
-            allow_multi_same_leaf=True)
-        self._add_new_element(
-            [f"{QEMUS_NS}commandline", f"{QEMUS_NS}arg"],
-            {"value": f"{overcommit_param}"},
-            allow_multi_same_leaf=True)
-        self.save()
-
     def bind_cpuids(self, cpu_ids):
         """
         bind available cpuids
         """
         # set iothread
         self._add_new_element(["cputune", "iothreadpin"],
                               {"iothread": "1", "cpuset": f"{cpu_ids.pop(0)}"}, True)
```

### Comparing `pycloudstack-0.0.10/pycloudstack/vmguest.py` & `pycloudstack-0.0.9/pycloudstack/vmguest.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 __author__ = 'cpio'
 
 LOG = logging.getLogger(__name__)
 
 LOOPBACK = "127.0.0.1"
 DEFAULT_SSH_PORT = 22
-DEFAULT_CHECK_INTERVAL = 1
 
 
 class VMGuest:
 
     """
     VM Guest instance with VM customization.
 
@@ -148,15 +147,15 @@
                   "-o", "PreferredAuthentications=publickey",
                   "-i", ssh_id_key,
                   "-r", f"root@{self.get_ip()}:{source}", target]
         runner = NativeCmdRunner(cmdarr)
         runner.runwait()
         return runner
 
-    def wait_for_ssh_ready(self, timeout=BOOT_TIMEOUT, check_interval=DEFAULT_CHECK_INTERVAL):
+    def wait_for_ssh_ready(self, timeout=BOOT_TIMEOUT):
         """
         Wait for the port of forwarded SSH ready until timeout
         @return True is ready, False is timeout
         """
 
         tstart = time.time()
         tnow = time.time()
@@ -187,15 +186,15 @@
             # Open SSH socket
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             sock.settimeout(timeout)
             retcode = sock.connect_ex((ssh_ip, ssh_port))
             if retcode != 0:
                 LOG.error("Fail to connect SSH for guest %s, connect error: %d", self.name, retcode)
                 sock.close()
-                time.sleep(check_interval)
+                time.sleep(1)
                 tnow = time.time()
                 continue
 
             # Recev SSH packet
             try:
                 data = sock.recv(4096)
             except socket.timeout:
```

### Comparing `pycloudstack-0.0.10/pycloudstack/vmimg.py` & `pycloudstack-0.0.9/pycloudstack/vmimg.py`

 * *Files identical despite different names*

### Comparing `pycloudstack-0.0.10/pycloudstack/vmm.py` & `pycloudstack-0.0.9/pycloudstack/vmm.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 """
 import os
 import re
 import logging
 import time
 import json
+import tempfile
+import shutil
 import libvirt
 import libvirt_qemu
 from .cmdrunner import NativeCmdRunner
 from .dut import DUT
 from .virtxml import VirtXml
 from .vmparam import VM_TYPE_LEGACY, VM_TYPE_EFI, VM_TYPE_TD, VM_TYPE_SGX, \
     VM_STATE_SHUTDOWN, VM_STATE_RUNNING, VM_STATE_PAUSE, \
@@ -170,17 +172,14 @@
             xmlobj.set_vsock(self.vminst.vsock_cid)
 
         if self.vminst.diskfile_path:
             xmlobj.set_disk(self.vminst.diskfile_path)
 
         self.set_cpu_params_xml(xmlobj)
 
-        if self.vminst.mwait is not None:
-            xmlobj.set_overcommit_params(f"cpu-pm={self.vminst.mwait}")
-
         if self.vminst.boot == BOOT_TYPE_GRUB:
             xmlobj.kernel = None
             xmlobj.cmdline = None
         else:
             xmlobj.kernel = self.vminst.kernel
             xmlobj.cmdline = str(self.vminst.cmdline)
 
@@ -194,42 +193,39 @@
         if "ubuntu" in distro:
             bios_legacy = BIOS_BINARY_LEGACY_UBUNTU
             xmlobj.qemu_exec = QEMU_EXEC_UBUNTU
         else:
             bios_legacy = BIOS_BINARY_LEGACY_CENTOS
             xmlobj.qemu_exec = QEMU_EXEC_CENTOS
 
+        loader_filename = "OVMF-" + xmlobj.uuid + ".fd"
+        loader_fullpath = os.path.join(tempfile.gettempdir(), loader_filename)
+        assert os.path.exists(BIOS_OVMF)
+        shutil.copy(BIOS_OVMF, loader_fullpath)
+
         if self.vminst.vmtype in [VM_TYPE_LEGACY, VM_TYPE_LEGACY_PERF]:
             xmlobj.loader = bios_legacy
             xmlobj.set_cpu_params("host,-kvm-steal-time,pmu=off")
         elif self.vminst.vmtype in [VM_TYPE_EFI, VM_TYPE_EFI_PERF]:
-            xmlobj.loader = BIOS_OVMF
+            xmlobj.loader = loader_fullpath
             xmlobj.set_cpu_params("host,-kvm-steal-time,pmu=off")
         elif self.vminst.vmtype == VM_TYPE_SGX:
             xmlobj.loader = bios_legacy
             xmlobj.set_cpu_params(
                 "host,host-phys-bits,+sgx,+sgx-debug,+sgx-exinfo,"
                 "+sgx-kss,+sgx-mode64,+sgx-provisionkey,+sgx-tokenkey,+sgx1,+sgx2,+sgxlc")
             xmlobj.set_epc_params(self.vminst.vmspec.epc)
         elif self.vminst.vmtype in [VM_TYPE_TD, VM_TYPE_TD_PERF]:
-            xmlobj.loader = BIOS_OVMF
+            xmlobj.loader = loader_fullpath
 
-            param_cpu = ""
             if DUT.get_cpu_base_freq() < 1000000:
-                param_cpu = "host,-shstk,-kvm-steal-time,pmu=off,tsc-freq=1000000000"
+                xmlobj.set_cpu_params(
+                    "host,-shstk,-kvm-steal-time,pmu=off,tsc-freq=1000000000")
             else:
-                param_cpu = "host,-shstk,-kvm-steal-time,pmu=off"
-
-            if self.vminst.tsx is False:
-                param_cpu += ",-hle,-rtm"
-            if self.vminst.tsc is False:
-                param_cpu += ",-tsc-deadline"
-
-            xmlobj.set_cpu_params(param_cpu)
-
+                xmlobj.set_cpu_params("host,-shstk,-kvm-steal-time,pmu=off")
 
     def _connect_virt(self):
         LOG.debug("Create libvirt connection")
         try:
             self._virt_conn = libvirt.open("qemu:///system")
             return self._virt_conn
         except libvirt.libvirtError:
```

### Comparing `pycloudstack-0.0.10/pycloudstack/vmparam.py` & `pycloudstack-0.0.9/pycloudstack/vmparam.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 VM_TYPE_TD_PERF = "td_perf"
 VM_TYPE_EFI_PERF = "efi_perf"
 VM_TYPE_LEGACY_PERF = "legacy_perf"
 
 BOOT_TYPE_DIRECT = "direct"
 BOOT_TYPE_GRUB = "grub"
 
-# Note:
-#   1.  hvc0 is the default console for TD VM, ttyS0 will be filtered
-#   due to security concern.
+#
+# hvc0 is the default console for TD VM, ttyS0 will be filtered
+# due to security concern.
 
 DEFAULT_CMDLINE = "rw selinux=0 console=hvc0 earlyprintk console=tty0"
 
 QEMU_EXEC_CENTOS = "/usr/libexec/qemu-kvm"
 QEMU_EXEC_UBUNTU = "/usr/bin/qemu-system-x86_64"
 
 BIOS_BINARY_LEGACY_CENTOS = "/usr/share/qemu-kvm/bios.bin"
```

### Comparing `pycloudstack-0.0.10/pycloudstack.egg-info/PKG-INFO` & `pycloudstack-0.0.9/pycloudstack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycloudstack
-Version: 0.0.10
+Version: 0.0.9
 Summary: Python package to manage hypervisor/docker/kubernetes stacks
 Author-email: Lu Ken <ken.lu@intel.com>, "Hao, Ruomeng" <ruomeng.hao@intel.com>
 License: Apache Software License
 Project-URL: Homepage, https://github.com/intel/tdx-tools
 Project-URL: Bug Tracker, https://github.com/intel/tdx-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,28 +16,28 @@
 
 # PyCloudStack (Unified Cloud Stack Operator Framework)
 
 ## 1. Overview
 
 PyCloudStack abstracts the common objects/operations/resources for diverse cloud
 architectures like hypervisor stack based on libvirt or direct qemu command,
-container stack orchestrated by Kubernetes or direct docker command, and the running
+container stack orchestrated by kubernetes or direct docker command, and the running
 or remote IaaS host.
 
 It can be used to create advance deployment CI/CD operator via python plugin for
 ansible, end-to-end validation framework with customized the components/configurations
 in full vertical stack.
 
 The architecture diagram is as follows:
 
 ![](https://github.com/intel/tdx-tools/blob/main/doc/pycloudstack.png)
 
 ## 2. Getting Start
 
-### Install from PyPI
+### Install from pypi
 
 ```
 pip3 install pycloudstack
 ```
 
 ### Install from source
 ```
@@ -79,15 +79,15 @@
 
 vm_factory = VMGuestFactory(vm_image, vm_kernel)
 inst = vm_factory.new_vm(vm_instance_type, vm_class=VMMQemu,
                          auto_start=True)
 inst.wait_for_ssh_ready()
 ```
 
-## Example 3: Operate Kubernetes Cluster
+## Example 3: Operate Kubenetes Cluster
 
 ```
 from pycloudstack.cluster import SGXCluster
 
 DEPLOYMENT_TEMPLATE='''
 apiVersion: apps/v1
 kind: Deployment
```

### Comparing `pycloudstack-0.0.10/pycloudstack.egg-info/SOURCES.txt` & `pycloudstack-0.0.9/pycloudstack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycloudstack-0.0.10/pyproject.toml` & `pycloudstack-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pycloudstack"
-version = "0.0.10"
+version = "0.0.9"
 authors = [
   { name="Lu Ken", email="ken.lu@intel.com" },
   { name="Hao, Ruomeng", email="ruomeng.hao@intel.com" },
 ]
 description = "Python package to manage hypervisor/docker/kubernetes stacks"
 readme = "README.md"
 license = { text="Apache Software License" }
```

