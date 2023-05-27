# Comparing `tmp/pyCloudy-0.9.7.tar.gz` & `tmp/pyCloudy-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyCloudy-0.9.7.tar", last modified: Tue May 22 06:24:46 2018, max compression
+gzip compressed data, was "dist/pyCloudy-0.9.9.tar", last modified: Thu May 21 00:22:28 2020, max compression
```

## Comparing `pyCloudy-0.9.7.tar` & `pyCloudy-0.9.9.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwx------   0 christophemorisset   (501) staff       (20)        0 2018-05-22 06:24:46.000000 pyCloudy-0.9.7/
--rw-------   0 christophemorisset   (501) staff       (20)     2447 2018-05-22 06:24:46.000000 pyCloudy-0.9.7/PKG-INFO
-drwx------   0 christophemorisset   (501) staff       (20)        0 2018-05-22 06:24:46.000000 pyCloudy-0.9.7/pyCloudy/
--rw-------   0 christophemorisset   (501) staff       (20)      971 2017-04-16 01:56:18.000000 pyCloudy-0.9.7/pyCloudy/__init__.py
-drwx------   0 christophemorisset   (501) staff       (20)        0 2018-05-22 06:24:46.000000 pyCloudy-0.9.7/pyCloudy/c1d/
--rw-------   0 christophemorisset   (501) staff       (20)      164 2015-10-13 14:24:20.000000 pyCloudy-0.9.7/pyCloudy/c1d/__init__.py
--rw-r--r--   0 christophemorisset   (501) staff       (20)   104321 2018-05-22 06:15:37.000000 pyCloudy-0.9.7/pyCloudy/c1d/cloudy_model.py
-drwx------   0 christophemorisset   (501) staff       (20)        0 2018-05-22 06:24:46.000000 pyCloudy-0.9.7/pyCloudy/c3d/
--rw-------   0 christophemorisset   (501) staff       (20)      105 2015-10-13 14:24:20.000000 pyCloudy-0.9.7/pyCloudy/c3d/__init__.py
--rw-r--r--   0 christophemorisset   (501) staff       (20)    40221 2018-05-22 06:10:34.000000 pyCloudy-0.9.7/pyCloudy/c3d/model_3d.py
-drwx------   0 christophemorisset   (501) staff       (20)        0 2018-05-22 06:24:46.000000 pyCloudy-0.9.7/pyCloudy/db/
--rw-------   0 christophemorisset   (501) staff       (20)        1 2015-10-13 14:24:20.000000 pyCloudy-0.9.7/pyCloudy/db/__init__.py
--rw-------   0 christophemorisset   (501) staff       (20)    24671 2017-04-16 01:56:18.000000 pyCloudy-0.9.7/pyCloudy/db/initSQL.py
--rw-------   0 christophemorisset   (501) staff       (20)    18109 2017-06-29 14:25:15.000000 pyCloudy-0.9.7/pyCloudy/db/MdB.py
--rw-r--r--   0 christophemorisset   (501) staff       (20)    61896 2017-06-29 11:56:06.000000 pyCloudy-0.9.7/pyCloudy/db/use3MdB.py
-drwx------   0 christophemorisset   (501) staff       (20)        0 2018-05-22 06:24:46.000000 pyCloudy-0.9.7/pyCloudy/utils/
--rw-------   0 christophemorisset   (501) staff       (20)      135 2015-10-13 14:24:20.000000 pyCloudy-0.9.7/pyCloudy/utils/__init__.py
--rw-------   0 christophemorisset   (501) staff       (20)      470 2015-10-13 14:24:20.000000 pyCloudy-0.9.7/pyCloudy/utils/astro.py
--rw-r--r--   0 christophemorisset   (501) staff       (20)     6668 2017-06-02 22:31:51.000000 pyCloudy-0.9.7/pyCloudy/utils/Config.py
--rw-r--r--   0 christophemorisset   (501) staff       (20)     4391 2017-04-24 16:55:14.000000 pyCloudy-0.9.7/pyCloudy/utils/convert_c17_c13.txt
--rw-------   0 christophemorisset   (501) staff       (20)     4749 2017-04-30 23:17:14.000000 pyCloudy-0.9.7/pyCloudy/utils/convert_c17_c13_2.txt
--rw-------   0 christophemorisset   (501) staff       (20)     1186 2015-10-13 14:24:20.000000 pyCloudy-0.9.7/pyCloudy/utils/init.py
--rw-------   0 christophemorisset   (501) staff       (20)    11578 2017-05-29 17:12:23.000000 pyCloudy-0.9.7/pyCloudy/utils/Izotov2013_CR.txt
--rw-------   0 christophemorisset   (501) staff       (20)     6793 2017-04-16 01:56:18.000000 pyCloudy-0.9.7/pyCloudy/utils/logging.py
--rw-r--r--   0 christophemorisset   (501) staff       (20)    18723 2017-07-23 19:21:35.000000 pyCloudy-0.9.7/pyCloudy/utils/misc.py
--rw-r--r--   0 christophemorisset   (501) staff       (20)     8797 2017-05-29 17:14:23.000000 pyCloudy-0.9.7/pyCloudy/utils/physics.py
--rw-r--r--   0 christophemorisset   (501) staff       (20)     2636 2017-07-23 19:21:35.000000 pyCloudy-0.9.7/pyCloudy/utils/pyneb2cloudy.txt
--rw-------   0 christophemorisset   (501) staff       (20)    13511 2017-04-16 01:56:18.000000 pyCloudy-0.9.7/pyCloudy/utils/red_corr.py
--rw-r--r--   0 christophemorisset   (501) staff       (20)       70 2018-05-22 06:24:23.000000 pyCloudy-0.9.7/pyCloudy/version.py
-drwx------   0 christophemorisset   (501) staff       (20)        0 2018-05-22 06:24:46.000000 pyCloudy-0.9.7/pyCloudy.egg-info/
--rw-r--r--   0 christophemorisset   (501) staff       (20)        1 2018-05-22 06:24:46.000000 pyCloudy-0.9.7/pyCloudy.egg-info/dependency_links.txt
--rw-r--r--   0 christophemorisset   (501) staff       (20)     2447 2018-05-22 06:24:46.000000 pyCloudy-0.9.7/pyCloudy.egg-info/PKG-INFO
--rw-r--r--   0 christophemorisset   (501) staff       (20)      719 2018-05-22 06:24:46.000000 pyCloudy-0.9.7/pyCloudy.egg-info/SOURCES.txt
--rw-r--r--   0 christophemorisset   (501) staff       (20)        9 2018-05-22 06:24:46.000000 pyCloudy-0.9.7/pyCloudy.egg-info/top_level.txt
--rw-r--r--   0 christophemorisset   (501) staff       (20)     1324 2017-07-23 19:21:35.000000 pyCloudy-0.9.7/README.rst
--rw-------   0 christophemorisset   (501) staff       (20)       38 2018-05-22 06:24:46.000000 pyCloudy-0.9.7/setup.cfg
--rw-r--r--   0 christophemorisset   (501) staff       (20)     1476 2017-04-26 21:40:43.000000 pyCloudy-0.9.7/setup.py
+drwxr-xr-x   0 christophemorisset   (501) staff       (20)        0 2020-05-21 00:22:28.000000 pyCloudy-0.9.9/
+-rw-r--r--   0 christophemorisset   (501) staff       (20)     2447 2020-05-21 00:22:28.000000 pyCloudy-0.9.9/PKG-INFO
+-rw-r--r--   0 christophemorisset   (501) staff       (20)     1324 2017-07-23 19:21:35.000000 pyCloudy-0.9.9/README.rst
+drwxr-xr-x   0 christophemorisset   (501) staff       (20)        0 2020-05-21 00:22:28.000000 pyCloudy-0.9.9/pyCloudy/
+-rw-r--r--   0 christophemorisset   (501) staff       (20)      971 2017-04-16 01:56:18.000000 pyCloudy-0.9.9/pyCloudy/__init__.py
+drwxr-xr-x   0 christophemorisset   (501) staff       (20)        0 2020-05-21 00:22:28.000000 pyCloudy-0.9.9/pyCloudy/c1d/
+-rw-r--r--   0 christophemorisset   (501) staff       (20)      164 2015-10-13 14:24:20.000000 pyCloudy-0.9.9/pyCloudy/c1d/__init__.py
+-rw-r--r--   0 christophemorisset   (501) staff       (20)   108343 2020-05-06 15:56:13.000000 pyCloudy-0.9.9/pyCloudy/c1d/cloudy_model.py
+drwxr-xr-x   0 christophemorisset   (501) staff       (20)        0 2020-05-21 00:22:28.000000 pyCloudy-0.9.9/pyCloudy/c3d/
+-rw-r--r--   0 christophemorisset   (501) staff       (20)      105 2015-10-13 14:24:20.000000 pyCloudy-0.9.9/pyCloudy/c3d/__init__.py
+-rw-r--r--   0 christophemorisset   (501) staff       (20)    40368 2019-10-28 20:39:02.000000 pyCloudy-0.9.9/pyCloudy/c3d/model_3d.py
+drwxr-xr-x   0 christophemorisset   (501) staff       (20)        0 2020-05-21 00:22:28.000000 pyCloudy-0.9.9/pyCloudy/db/
+-rw-r--r--   0 christophemorisset   (501) staff       (20)    18417 2019-04-17 00:02:53.000000 pyCloudy-0.9.9/pyCloudy/db/MdB.py
+-rw-r--r--   0 christophemorisset   (501) staff       (20)        1 2015-10-13 14:24:20.000000 pyCloudy-0.9.9/pyCloudy/db/__init__.py
+-rw-r--r--   0 christophemorisset   (501) staff       (20)     7967 2019-11-30 02:48:07.000000 pyCloudy-0.9.9/pyCloudy/db/continuum_bands.ini
+-rw-r--r--   0 christophemorisset   (501) staff       (20)    42769 2020-02-20 10:23:05.000000 pyCloudy-0.9.9/pyCloudy/db/initSQL.py
+-rw-r--r--   0 christophemorisset   (501) staff       (20)    67491 2020-02-21 08:58:37.000000 pyCloudy-0.9.9/pyCloudy/db/use3MdB.py
+drwxr-xr-x   0 christophemorisset   (501) staff       (20)        0 2020-05-21 00:22:28.000000 pyCloudy-0.9.9/pyCloudy/utils/
+-rw-r--r--   0 christophemorisset   (501) staff       (20)     6751 2020-01-24 01:12:04.000000 pyCloudy-0.9.9/pyCloudy/utils/Config.py
+-rw-r--r--   0 christophemorisset   (501) staff       (20)    11578 2017-05-29 17:12:15.000000 pyCloudy-0.9.9/pyCloudy/utils/Izotov2013_CR.txt
+-rw-r--r--   0 christophemorisset   (501) staff       (20)      135 2015-10-13 14:24:20.000000 pyCloudy-0.9.9/pyCloudy/utils/__init__.py
+-rw-r--r--   0 christophemorisset   (501) staff       (20)      470 2015-10-13 14:24:20.000000 pyCloudy-0.9.9/pyCloudy/utils/astro.py
+-rw-r--r--   0 christophemorisset   (501) staff       (20)     4391 2017-04-24 16:55:14.000000 pyCloudy-0.9.9/pyCloudy/utils/convert_c17_c13.txt
+-rw-r--r--   0 christophemorisset   (501) staff       (20)     4749 2017-04-30 23:17:14.000000 pyCloudy-0.9.9/pyCloudy/utils/convert_c17_c13_2.txt
+-rw-r--r--   0 christophemorisset   (501) staff       (20)     1186 2015-10-13 14:24:20.000000 pyCloudy-0.9.9/pyCloudy/utils/init.py
+-rw-r--r--   0 christophemorisset   (501) staff       (20)     6793 2017-04-16 01:56:18.000000 pyCloudy-0.9.9/pyCloudy/utils/logging.py
+-rw-r--r--   0 christophemorisset   (501) staff       (20)    18723 2017-07-19 16:53:28.000000 pyCloudy-0.9.9/pyCloudy/utils/misc.py
+-rw-r--r--   0 christophemorisset   (501) staff       (20)    16442 2018-06-27 18:20:15.000000 pyCloudy-0.9.9/pyCloudy/utils/physics.py
+-rw-r--r--   0 christophemorisset   (501) staff       (20)     2636 2017-07-20 17:26:30.000000 pyCloudy-0.9.9/pyCloudy/utils/pyneb2cloudy.txt
+-rw-r--r--   0 christophemorisset   (501) staff       (20)    13511 2017-04-16 01:56:18.000000 pyCloudy-0.9.9/pyCloudy/utils/red_corr.py
+-rw-r--r--   0 christophemorisset   (501) staff       (20)       70 2020-05-20 23:39:33.000000 pyCloudy-0.9.9/pyCloudy/version.py
+drwxr-xr-x   0 christophemorisset   (501) staff       (20)        0 2020-05-21 00:22:28.000000 pyCloudy-0.9.9/pyCloudy.egg-info/
+-rw-r--r--   0 christophemorisset   (501) staff       (20)     2447 2020-05-21 00:22:28.000000 pyCloudy-0.9.9/pyCloudy.egg-info/PKG-INFO
+-rw-r--r--   0 christophemorisset   (501) staff       (20)      751 2020-05-21 00:22:28.000000 pyCloudy-0.9.9/pyCloudy.egg-info/SOURCES.txt
+-rw-r--r--   0 christophemorisset   (501) staff       (20)        1 2020-05-21 00:22:28.000000 pyCloudy-0.9.9/pyCloudy.egg-info/dependency_links.txt
+-rw-r--r--   0 christophemorisset   (501) staff       (20)        9 2020-05-21 00:22:28.000000 pyCloudy-0.9.9/pyCloudy.egg-info/top_level.txt
+-rw-r--r--   0 christophemorisset   (501) staff       (20)       38 2020-05-21 00:22:28.000000 pyCloudy-0.9.9/setup.cfg
+-rw-r--r--   0 christophemorisset   (501) staff       (20)     1522 2019-12-02 22:54:23.000000 pyCloudy-0.9.9/setup.py
```

### Comparing `pyCloudy-0.9.7/PKG-INFO` & `pyCloudy-0.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 1.2
 Name: pyCloudy
-Version: 0.9.7
+Version: 0.9.9
 Summary: Tools to manage Astronomical Cloudy photoionization code
 Home-page: https://sites.google.com/site/pycloudy/
 Author: Christophe Morisset IA-UNAM
 Author-email: chris.morisset@gmail.com
 Maintainer: Christophe Morisset IA-UNAM
 Maintainer-email: chris.morisset@gmail.com
 License: GPL
-Download-URL: https://github.com/Morisset/pyCloudy/releases/tag/0.9.7
+Download-URL: https://github.com/Morisset/pyCloudy/releases/tag/0.9.9
 Description: PyCloudy is a Python library to deal with input and output files of Cloudy (Gary Ferland) photoionization code.
         Is also allows to generate 3D nebula from various runs of the 1D Cloudy code.
         
         Requirements
         ============
         
         You will need to have installed `Cloudy <http://nublado.org/>`_ .
```

### Comparing `pyCloudy-0.9.7/pyCloudy/__init__.py` & `pyCloudy-0.9.9/pyCloudy/__init__.py`

 * *Files identical despite different names*

### Comparing `pyCloudy-0.9.7/pyCloudy/c1d/cloudy_model.py` & `pyCloudy-0.9.9/pyCloudy/c1d/cloudy_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 from ..utils.init import LIST_ELEM, LIST_ALL_ELEM, SYM2ELEM
 from ..utils.misc import sextract, cloudy2pyneb, convert_c13_c17, convert_c17_c13, mytrapz
 from ..utils.physics import ATOMIC_MASS
 if pc.config.INSTALLED['PyNeb']:
     import pyneb
 if pc.config.INSTALLED['scipy']:
     from scipy.integrate import cumtrapz
+    from scipy.interpolate import interp1d
 if pc.config.INSTALLED['plt']:
     import matplotlib.pyplot as plt
-    
+
 ##
 # @bug There is a problem for plan parallel models (yes Will, you are right!) (when depth << radius) 
 # it can be that all the values in radius are the same, which gives pb to m_cut etc
 # Need to identify this situation and to deal with it without "try", but safetly.
 
 ## @include copyright.txt
 class CloudyModel(object):
@@ -87,14 +88,15 @@
     GPL Chris.Morisset@Gmail.com
     """
 
     ## Cloudy model object
     def __init__(self, model_name, verbose=None, 
                  read_all_ext = True, read_rad=True, read_phy=True, read_emis = True, read_grains = False, 
                  read_cont = True, read_heatcool = False, read_lin = False, read_opd = False, 
+                 read_pressure=False, read_abunds = False,
                  list_elem = LIST_ELEM, distance = None, line_is_log = False, 
                  emis_is_log = True, 
                  ionic_str_key = 'ele_'):
         """
         param:
             - model_name [str] The name of the model to be read.
             - verbose [int] level of verbosity as defined by pyCloudy.my_logging.
@@ -137,14 +139,18 @@
                 self._init_emis()
             if read_cont:
                 self._init_cont()
             if read_grains:
                 self._init_grains()
             if read_heatcool:
                 self._init_heatcool()
+            if read_pressure:
+                self._init_pressure()
+            if read_abunds:
+                self._init_abunds()
     ##            
     # @var distance
     # distance to the object (kpc)
     # @var model_name
     # name of the model [str]
     # @var log_
     # logging tool [my_logging object]
@@ -190,15 +196,17 @@
         self.gabund_labels = None
         self.n_gdgrat = 0
         self.gdgrat_full = None
         self.gdsize = None
         self.gdgrat_labels = None        
         self.plan_par = None
         self.Hbeta_full = None
-    
+        self.abunds_full = None
+        self.pressure_full = None
+        
     def _init_rad(self):
         key = 'rad'
         self._res[key] = self.read_outputs(key)
         if self._res[key] is not None:
             self.empty_model = False
             self.n_zones_full = self._res[key].size
             self.zones_full = np.arange(self.n_zones_full)
@@ -344,15 +352,23 @@
                 self.emis_labels_17 = np.array(self.emis_labels_17, dtype=str)
             self.n_emis = np.size(self.emis_labels)
             self.log_.message('Number of emissivities: {0.n_emis:d}'.format(self), calling = self.calling)
             self.emis_full = np.zeros((self.n_emis, np.size(emis)))
             for i, label in enumerate(self.emis_labels):
                 self.emis_full[i] = trans_emis(emis[label])
             if 'H__1__4861A' in self.emis_labels:
-                self.Hbeta_full = (self.get_emis('H__1__4861A') * self.dvff).cumsum()
+                self.Hbeta_label = 'H__1__4861A'
+            elif 'H__1_486133A' in self.emis_labels:
+                self.Hbeta_label = 'H__1_486133A'
+            elif 'H__1_486136A' in self.emis_labels:
+                self.Hbeta_label = 'H__1_486136A'
+            else:
+                self.Hbeta_label = None
+            if self.Hbeta_label is not None:
+                self.Hbeta_full = (self.get_emis(self.Hbeta_label) * self.dvff).cumsum()
                 self.__Hbeta_cut = self.Hbeta_full[-1]
 
     def _init_ionic(self, elem, str_key = 'ele_'):
         key = str_key + elem
         self._res[key] = self.read_outputs(key)
         if self._res[key] is not None:
             ionic_names = self._res[key].dtype.names[1:]
@@ -392,14 +408,64 @@
             else:
                 self.opd_energy = None
                 self.log_.warn('No energy found in opd file', calling = self.calling)
             self.opd_total = self._res[key]['total']
             self.opd_absorp = self._res[key]['absorp']
             self.opd_scat = self._res[key]['scat']
             
+    def _init_abunds(self):
+        key = 'abunds'
+        self._res[key] = self.read_outputs(key)
+        self.abunds_full = self._res[key]  
+        names_translator = {'abund_H':'H',
+                            'HELI':'He',
+                            'LITH':'Li',
+                            'BERY':'Be',
+                            'BORO':'B',
+                            'CARB':'C',
+                            'NITR':'N',
+                            'OXYG':'O',
+                            'FLUO':'F',
+                            'NEON':'Ne',
+                            'SODI':'Na',
+                            'MAGN':'Mg',
+                            'ALUM':'Al',
+                            'SILI':'Si',
+                            'PHOS':'P',
+                            'SULP':'S',
+                            'CHLO':'Cl',
+                            'ARGO':'Ar',
+                            'POTA':'K',
+                            'CALC':'Ca',
+                            'SCAN':'Sc',
+                            'TITA':'Ti',
+                            'VANA':'V',
+                            'CHRO':'Cr',
+                            'MANG':'Mn',
+                            'IRON':'Fe',
+                            'COBA':'Co',
+                            'NICK':'Ni',
+                            'COPP':'Cu',
+                            'ZINC':'Zn'}
+        
+        ab_names = self.abunds_full.dtype.names
+        new_names = [names_translator[name] for name in ab_names]
+        self.abunds_full.dtype.names = new_names
+        for elem in self.abunds_full.dtype.names:
+            self.abunds_full[elem] -= np.log10(self.nH_full)
+    
+    def _init_pressure(self):
+        """
+        Pressure in dynes/cm2.
+        If P/k (in K.cm-3) is needed, divide by pc.CST.BOLTZMANN
+        """
+        key = 'pres'
+        self._res[key] = self.read_outputs(key)
+        self.pressure_full = self._res[key]['Pcurrent']
+        
     def _init_grains(self):
         key = 'gtemp'
         if int(self.cloudy_version_major) == 7:
             sk_header = 0
             sk_header2 = 1
         elif int(self.cloudy_version_major) < 16:
             """
@@ -482,21 +548,25 @@
                 self.out['###First'] = line
             elif line[0:4] == ' ###':
                 self.out['###Last'] = line
             elif 'Calculation stopped' in line:
                 self.out['stop'] = line
             elif 'Cloudy ends' in line:
                 self.out['Cloudy ends'] = line
+            elif 'something went wrong' in line:
+                self.out['wrong'] = line
             elif 'Gas Phase Chemical Composition' in line:
                 for i in range(4):
                     self.out['Chem' + str(i + 1)] = next(file_)
             elif 'Grain Chemical Composition' in line:
                 self.out['GrainChem'] = next(file_)
             elif 'Dust to gas ratio' in line:
                 self.out['D/G'] = line
+            elif "* grains" in line:
+                self.out['grains'] = line
             elif 'iterate' in line:
                 self.out['iterate'] = line
             elif 'Hi-Con' in line:
                 for i in range(7):
                     self.out['SED' + str(i + 1)] = next(file_)
             elif 'table star' in line:
                 self.out['table star'] = line
@@ -564,25 +634,25 @@
         self.Q = np.zeros(4)
         self.Phi = np.zeros(4)
         try:
             self.Q[0] = float(pc.sextract(self.out['SED2'], 'Q(1.0-1.8):', 'Q(1.8-4.0):'))
             self.Q[1] = float(pc.sextract(self.out['SED2'], 'Q(1.8-4.0):', 'Q(4.0-20):'))
             self.Q[2] = float(pc.sextract(self.out['SED2'], 'Q(4.0-20):', 'Q(20--):'))
             self.Q[3] = float(pc.sextract(self.out['SED2'], 'Q(20--):', 'Ion pht'))
-            self.Q = pow(10., self.Q)
+            self.Q = 10.**self.Q
             self.plan_par = False
         except:
             pass
         self.Q0 = self.Q.sum()
         try:
             self.Phi[0] = float(pc.sextract(self.out['SED2'], 'phi(1.0-1.8):', 'phi(1.8-4.0):'))
             self.Phi[1] = float(pc.sextract(self.out['SED2'], 'phi(1.8-4.0):', 'phi(4.0-20):'))
             self.Phi[2] = float(pc.sextract(self.out['SED2'], 'phi(4.0-20):', 'phi(20--):'))
             self.Phi[3] = float(pc.sextract(self.out['SED2'], 'phi(20--):', 'Ion pht'))
-            self.Phi = pow(10., self.Phi)
+            self.Phi = 10.**self.Phi
             self.plan_par = True
         except:
             pass
         self.Phi0 = self.Phi.sum()
         
         self.abund = {}
         try:
@@ -738,14 +808,20 @@
 
     ## te.ne.nH [float array] (K.cm^-6)
     @property
     def tenenH(self):
         """ array of Te.ne.nH (on r_range)"""
         return self._get_over_range(self.tenenH_full)
 
+    ## Abundances
+    @property
+    def abunds(self):
+        """ array of abundances (on r_range)"""
+        return self._get_over_range(self.abunds_full)
+
     ## filling factor [float array]
     @property
     def ff(self):
         """ array of filling factor (on r_range)"""
         return self._get_over_range(self.ff_full)
 
     ## cooling [float array]
@@ -1290,15 +1366,31 @@
         return to_return
 
     ## Return the continuum flux (stellar or nebular, depending on cont parameter
     def get_cont_y(self, cont='incid', unit='es', dist_norm='at_earth'):
         """
         param:
             cont : one of ['incid','trans','diffout','ntrans','reflec', 'total']
-            unit : one of ['esc', 'ec3','es','esA','esAc','esHzc','Jy','Q', 'Wcmu', 'WmHz', 'WmA', 'phs', 'phsmu', 'phsc', 'phsmuc']
+            unit : one of ['esc' for erg/s/cm2, 
+                           'ec3'for erg/s/cm2/C C : lightspeed,
+                           'es' for erg/s,
+                           'esA' for erg/s/AA,
+                           'esHz' for erg/s/Hz,
+                           'esAc' for erg/s/AA/cm2,
+                           'ec3A' for erg/s/AA/cm2/C C : lighspeed
+                           'esHzc' for erg/s/Hz/cm2,
+                           'Jy' for Jansky,
+                           'Q' for number of photons above the corresponding energy, 
+                           'Wcmu' for Watt/micron/cm2, 
+                           'WmHz' for Watt/Herz/m2, 
+                           'WmA' for Watt/Anstrom/m2, 
+                           'phs' for photons/s, 
+                           'phsmu' for photons/s/micron, 
+                           'phsc' for photons/s/cm2, 
+                           'phsmuc' for photons/s/micron/cm2]
             dist_norm : one of ['at_earth', 'r_out', a float for a distance in cm]
         return:
             continuum flux or intensity
         """
 
         """ First define which of the 6 continua will be return """
         if cont == 'incid':
@@ -1344,18 +1436,18 @@
         elif unit == 'esHz':
             """erg.s-1.Hz-1"""
             to_return = cont1 / self.get_cont_x(unit='Hz') * inner_surface
         elif unit == 'esc':
             """ erg.s-1.cm-2 """
             to_return = cont1 * dist_fact
         elif unit == 'ec3':
-            """ erg.cm-3 """
+            """ erg.s-1.cm-2.c-1 """
             to_return = cont1 * dist_fact / pc.CST.CLIGHT
         elif unit == 'ec3A':
-            """ erg.cm-3.A-1 """
+            """ erg.s-1.cm-2.A-1.c-1 """
             to_return = cont1 / self.get_cont_x(unit='Ang') * dist_fact / pc.CST.CLIGHT
         elif unit == 'esAc':
             """ erg.s-1.cm-2.A-1 """
             to_return = cont1 / self.get_cont_x(unit='Ang') * dist_fact
         elif unit == 'esHzc':
             """ erg.s-1.cm-2.Hz-1 """
             to_return = cont1 / self.get_cont_x(unit='Hz') * dist_fact
@@ -1399,16 +1491,17 @@
             self.log_.warn("unit must be one of: ['esc', 'ec3','es','esA','esAc','esHzc','WmHz','Wcmu','Jy','Q']",
                             calling = self.calling)
             to_return = None        
         return to_return
 
     def get_integ_spec(self, cont, lam_low, lam_high, unit='es'):
         """
-        Return the integral of the spectrum (in unit, see below) between lam_low and lam_high (in AA)
+        Return the integral of the spectrum (in unit, see below) between lam_low and lam_high
         unit : one of ['es', 'phs', 'esc', 'Wm', 'phsc']
+        unit for lam_low and lam_high: Angstrom, except if unit in ('phs', 'phsc'): micron
         example: get_integ_spec('diffout', 5000, 6000)
         """
         if unit == 'es':
             unitx = 'Ang'
             unity = 'esA'
         elif unit == 'phs':
             unitx = 'mu'
@@ -1423,14 +1516,26 @@
             unitx = 'mu'
             unity = 'phsmuc'
         else:
             self.log_.error("unit must be one of: ['es', 'phs', 'esc', 'Wm', 'phsc']", calling = self.calling)
         integ = mytrapz(self.get_cont_y(cont=cont, unit=unity), self.get_cont_x(unitx), lam_low, lam_high)        
         return integ
             
+    def get_interp_cont(self, cont='incid', unit='es', dist_norm='at_earth',
+                        x_value=4686.0, x_unit='Ang'):
+        """
+        Return the value of the continuum at a given wavelength/energy value
+        """
+        
+        cont_x = self.get_cont_x(unit=x_unit)
+        cont_y = self.get_cont_y(cont=cont, unit=unit, dist_norm=dist_norm)
+        interp_cont = interp1d(cont_x, cont_y)
+        return interp_cont(x_value)
+        
+    
     ## get_G0 = integral(f_lambda . dlambda) Between lam_min and lam_max (Ang), normalized by norm, in unit of W.m-2 or erg.cm-3
     def get_G0(self, lam_min = 913, lam_max = 1e8, dist_norm = 'r_out', norm = 1.6e-6, unit = 'Wm'):
         """
         Normalisation from Habing 1968: 1.6e-6 erg.cm-2.s-1
         """
         lam = self.get_cont_x(unit = 'Ang')
         lam_range = (lam > lam_min) & (lam < lam_max)
@@ -1549,15 +1654,15 @@
             return None
         
     ## Hbeta = \f$ \int Hbeta.n_H.ff.dV\f$ [solar mass]                
     @property        
     def Hbeta(self):
         """Return the intensity of Hbeta"""
         try:
-            return self.get_emis_vol('H__1__4861A')
+            return self.get_emis_vol(self.Hbeta_label)
         except:
             self.log_.warn('H beta not available', calling = self.calling)
             return None
         
     
     ## Mean Temperature \f$T0=\frac{\int T_e.n_e.n_H.ff.dV}{\int n_e.n_H.ff.dV}\f$
     @property        
@@ -1579,20 +1684,16 @@
 
     ## Hb_SB = I\f$_\beta / (Rout^2 * pi * 206265.^2)\f$
     def get_Hb_SB(self):
         """
         Hbeta surface brightness:
         Returns Ibeta / (Rout**2 * pi * 206265.**2)
         """
-        if 'H__1__4861A' in self.emis_labels:
-            return self.get_emis_vol('H__1__4861A') / (self.r_out_cut**2 * np.pi * 206265.**2)
-        elif 'H__1_486136A' in self.emis_labels:
-            return self.get_emis_vol('H__1_486136A') / (self.r_out_cut**2 * np.pi * 206265.**2)
-        elif 'H__1_486133A' in self.emis_labels:
-            return self.get_emis_vol('H__1_486133A') / (self.r_out_cut**2 * np.pi * 206265.**2)
+        if self.Hbeta_label is not None:
+            return self.get_emis_vol(self.Hbeta_label) / (self.r_out_cut**2 * np.pi * 206265.**2)
         else:
             self.log_.warn('Hbeta emissivity not in emis file', calling = self.calling + '.get_Hb_SB')
     
     def get_EW(self, label, lam0, lam_inf, lam_sup):
         """
         Equivalent Width:
         Returns -lam0 * I(label) / continuum(lam0)
@@ -1647,20 +1748,15 @@
     def get_Hb_EW(self):
         """
         Hbeta Equivalent Width:
         Returns -4861 * I(H__1__4861A) / continuum(4860)
         where continuum(4860) is estimated by looking for the minimum of the net transmited continuum between
         4560 and 4860 on one side, and 4860 and 5160 on the other side, and meaning them.
         """
-        if 'H__1__4861A' in self.emis_labels:
-            return self.get_EW('H__1__4861A', 4861, 4560, 5160)
-        elif 'H__1_486136A' in self.emis_labels:
-            return self.get_EW('H__1_486136A', 4861, 4560, 5160)
-        elif 'H__1_486133A' in self.emis_labels:
-            return self.get_EW('H__1_486133A', 4861, 4560, 5160)
+        return self.get_EW(self.Hbeta_label, 4861, 4560, 5160)
 
     ## Ha_EW = -\f$\lambda_\alpha$ x I$_\alpha^{line}$ / $\lambda.F_\alpha^{cont}\f$
     def get_Ha_EW(self):
         """
         Halpha Equivalent Width:
         Returns -6563 * I(H__1__6563A) / continuum(6563)
         where continuum(6563) is estimated by looking for the minimum of the net transmited continuum between
@@ -1743,33 +1839,37 @@
         
         new_emis_full = np.zeros((len(self.emis_labels)+1, self.n_zones_full))
         new_emis_full[:-1, :] = self.emis_full
         if type(pyneb_atom) is pyneb.RecAtom:
             spec = pyneb_atom.spec
         else:
             spec = pyneb_atom.spec - 1
-        
+        if self.abunds_full is None:
+            abunds = self.abund
+        else:
+            abunds = self.abunds_full
+            
+        self.log_.message('Doing atom {} {} {}'.format(pyneb_atom, wave, label))
         if wave is not None:
+            
             new_emis_full[-1, :] = pyneb_atom.getEmissivity(self.te_full, self.ne_full, wave = wave, product = False) * \
                                    self.ionic_full[pyneb_atom.elem][spec] * self.ne_full * \
-                                   self.nH_full * 10**self.abund[pyneb_atom.elem]
+                                   self.nH_full * 10**abunds[pyneb_atom.elem]
         else:
             new_emis_full[-1, :] = pyneb_atom.getEmissivity(self.te_full, self.ne_full, label = label, product = False) * \
                                    self.ionic_full[pyneb_atom.elem][spec] * self.ne_full * \
-                                   self.nH_full * 10**self.abund[pyneb_atom.elem]
-        new_emis_labels = np.zeros(len(self.emis_labels)+1, dtype=self.emis_labels.dtype)
-        new_emis_labels[:-1] = self.emis_labels
-        new_emis_labels[-1] = new_label
+                                   self.nH_full * 10**abunds[pyneb_atom.elem]
+                                           
+        self.emis_full = new_emis_full        
+        self.emis_labels = np.append(self.emis_labels, new_label)
         
-        self.emis_full = new_emis_full
-        self.emis_labels = new_emis_labels
         if self.cloudy_version_major > 16:
-            self.emis_labels_17 = new_emis_labels
+            self.emis_labels_17 = self.emis_labels 
         else:
-            self.emis_labels_13 = new_emis_labels
+            self.emis_labels_13 = self.emis_labels 
     
     def plot_spectrum(self, xunit='eV', cont='ntrans', yunit='es', ax=None, 
                       xlog=True, ylog=True, **kargv):
         """
         plot the spectrum of the model.
         parameters:
             - xunit ['eV']. See get_cont_y for details
@@ -2019,26 +2119,30 @@
                 params_str += ' {1}'
             else:
                 params_str += ' {1:f}'
             shape = params_str.format(SED, SED_params)
             lumi = '{0} = {1:.3f}'.format(lumi_unit, lumi_value)
             self._SEDs.append((shape, lumi))
         
-    def set_cste_density(self, dens = None, ff = None):
+    def set_cste_density(self, dens = None, ff = None, others = None):
         """
         Set the density of the model to a constant value
         Parameters:
             - dens:    the density (in log(cm-3))
             - ff:    filling factor (unused if None, default value)
+            - others: any string to be added to hden command
         """
         if dens is None:
             self._density = None
             self._filling_factor = None
             return None
-        self._density = 'hden = {0:.3f}'.format(dens)
+        if others is None:
+            self._density = 'hden = {0:.3f}'.format(dens)
+        else:
+            self._density = 'hden = {0:.3f}, {1}'.format(dens, others)
         if ff is not None:
             if type(ff) == type(()) or type(ff) == type([]):
                 self._filling_factor = 'filling factor = {0[0]:f} {0[1]:f}'.format(ff)
             else:
                 self._filling_factor = 'filling factor = {0:f}'.format(ff)
         else:
             self._filling_factor = 'filling factor = 1.0'
@@ -2132,15 +2236,15 @@
         else:
             if type(stop_criter) == type(()) or type(stop_criter) == type([]): 
                 for criter in stop_criter:
                     self._stop.append(criter)
             else:
                 self._stop.append(stop_criter)
     
-    def read_emis_file(self, emis_file, N_char=12):
+    def read_emis_file(self, emis_file, N_char=14):
         """
         Define the name of the file containing the labels for the list of emissivities to output
             in the .emis file
         """
         self._emis_tab = []
         try:
             with open(emis_file, 'r') as f:
```

### Comparing `pyCloudy-0.9.7/pyCloudy/c3d/model_3d.py` & `pyCloudy-0.9.9/pyCloudy/c3d/model_3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -950,15 +950,18 @@
                     plt.plot(prof, c = color)
                     plt.ylim((0., 1.05))
                     ax.xaxis.set_ticks_position("none")
                     ax.yaxis.set_ticks_position("none")
                     ax.xaxis.set_ticklabels([])
                     ax.yaxis.set_ticklabels([])
                     if transp:
-                        ax.axesPatch.set_alpha(0.0)
+                        try:
+                            ax.axesPatch.set_alpha(0.0)
+                        except:
+                            ax.patch.set_alpha(0.0)
     
     def _calc_profile(self, ref, axis):
         """
         Mihalas,1969,p250,p339 corrected from 3D to 1D (sqrt(3):
         zeta_0 = sqrt(2)*sigma to have gaus=exp(-(v/zeta)^2)
         sigma_therm_lambda = lambda_0 * sqrt(kT/mc2)
         then zeta_0_velo(km/s) = sqrt(2*k*1d4/M_H) * sqrt(M_H/m*T4) *1d-5
@@ -972,23 +975,23 @@
         zeta_0 = np.sqrt(self.v_turb**2 + coeff1**2. * self.te / 1e4 / atomic_mass(elem))
         if not self.cub_coord.vel_defined:
             self.log_.warn('Velocity not defined', calling = self.calling)
             return None
         if axis == 'x' or axis == 0:
             sum_axis = 0
             vel = self.cub_coord.vel_x
-            res = np.zeros((self.size_spectrum,self.cub_coord.dim_y,self.cub_coord.dim_z))
+            res = np.zeros((self.size_spectrum,self.cub_coord.dim_y,self.cub_coord.dim_z)).squeeze()
         elif axis == 'y' or axis == 1:
             sum_axis = 1
             vel = self.cub_coord.vel_y
-            res = np.zeros((self.size_spectrum,self.cub_coord.dim_x,self.cub_coord.dim_z))
+            res = np.zeros((self.size_spectrum,self.cub_coord.dim_x,self.cub_coord.dim_z)).squeeze()
         elif axis == 'z' or axis == 2:
             sum_axis = 2
             vel = self.cub_coord.vel_z
-            res = np.zeros((self.size_spectrum,self.cub_coord.dim_x,self.cub_coord.dim_y))
+            res = np.zeros((self.size_spectrum,self.cub_coord.dim_x,self.cub_coord.dim_y)).squeeze()
         for i in np.arange(self.size_spectrum):
             delta_v = vel + self.vel_tab[i]
             try:
                 res[i] = (emis * self.profile_function(x = delta_v, zeta_0 = zeta_0)).sum(axis=sum_axis)
             except:
                 self.log_.error('Error using the profile function', calling = self.calling)
         self.log_.message('line {0} : profile computed on axis {1}'.format(l_ref, axis), calling = self.calling)
```

### Comparing `pyCloudy-0.9.7/pyCloudy/db/MdB.py` & `pyCloudy-0.9.9/pyCloudy/db/MdB.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 import subprocess
 import numpy as np
 from getpass import getpass
 import pyCloudy as pc
 from pyCloudy.utils.init import LIST_ELEM
 from pyCloudy.utils.logging import my_logging
 if pc.config.INSTALLED['pandas']:
@@ -109,16 +110,20 @@
         if self.connected:
             self.close_dB()
 
     def connect_dB(self):
         if self.connected:
             self.log_.warn('Already connected', calling = self.calling)
             return None
-        try:
-            self._dB = self.SQLdb.connect(host = self.host, user = self.user_name, passwd = self.user_passwd, 
+        try:            
+            if self.unix_socket is None or sys.version_info[0] >= 3:
+                self._dB = self.SQLdb.connect(host = self.host, user = self.user_name, passwd = self.user_passwd, 
+                                        db = self.base_name, port = self.port)
+            else:
+                self._dB = self.SQLdb.connect(host = self.host, user = self.user_name, passwd = self.user_passwd, 
                                         db = self.base_name, port = self.port, unix_socket = self.unix_socket)
             self.connected = True
             self.log_.message('Connected to {0}'.format(self.host), calling = self.calling)
         except:
             self.log_.warn('Connection to {0} failed'.format(self.host), calling = self.calling)
         try:
             self._cursor = self._dB.cursor(self.SQLdb.cursors.DictCursor)
```

### Comparing `pyCloudy-0.9.7/pyCloudy/db/use3MdB.py` & `pyCloudy-0.9.9/pyCloudy/db/use3MdB.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 import glob
 import time
 import threading
 import numpy as np
 import datetime
 import pyCloudy as pc
 from random import randint
@@ -294,14 +295,16 @@
         else:
             com_str = 'com{0}'.format(i_com+1)
             self.insert_in_dic(com_str, comments)
             
     def set_C_version(self, version=None):
         if version in pc.config.cloudy_dict:
             self.insert_in_dic('C_version', version)
+        else:
+            self.log_.error('Unknown Cloudy version {}'.format(version))
 
     def insert_model(self, verbose_only=False, status=None):
         
         if not self.MdB.connected:
             self.log_.error('Not connected to the database')
             return None
         
@@ -357,49 +360,60 @@
     command = 'INSERT INTO {0} ({1}) VALUES ({2});'.format(seds_table, fields_str, values_str)
     MdB.exec_dB(command)
         
         
 class writeTab(object):
     
     def __init__(self, MdB=None, OVN_dic=None, models_dir = './', do_update_status=True):
-        
+        """
+        This object is in charge of filling the tab database table with the 
+        results of the model.
+        """
         self.log_ = pc.log_
         if MdB is None:
             MdB = pc.MdB(OVN_dic=OVN_dic)
         else:
             OVN_dic = MdB.OVN_dic
         if not isinstance(MdB, pc.MdB):
             self.log_.error('The first argument must be a MdB object')    
         self.MdB = MdB
         if not self.MdB.connected:
             self.MdB.connect_dB()
         self.OVN_dic = OVN_dic
         self.table = OVN_dic['master_table']
         self.pending_table = OVN_dic['pending_table']
+        self.lines_table = OVN_dic['lines_table']
         self.models_dir = models_dir
         self.fields = self.MdB.get_fields(from_ = self.table)
         self.pending_fields = self.MdB.get_fields(from_ = self.pending_table)
         self._dic = {}
         self.selectedN = None
         self.do_update_status = do_update_status
-         
+        self.RecDic = {'O_2R': pn.RecAtom('O', 2),
+                       'N_2R': pn.RecAtom('N', 2)}
+        self.host = os.getenv('HOST')
+        if self.host is None:
+            self.host = os.getenv('HOSTNAME')
+        if self.host is None:
+            self.host = 'localhost'
+        
     def insert_in_dic(self, key, value):
         
         if value is not None and np.isreal(value):
             if not np.isfinite(value):
                 value = None
                 
         if value is None:
             if key in self._dic:
                 del self._dic[key]
         else:
             if key in self.fields:
                 self._dic[key] = value
             else:
-                self.log_.error('Not a valid field {0}'.format(key))
+                self.log_.warn('Not a valid field {0}'.format(key), calling='insert_in_dic')
     
     def update_status(self, status):
         
         if not self.do_update_status:
             return
         if status in status_dic and self.selectedN is not None:
             command = 'UPDATE {0} SET `status`={1} WHERE N = {2}'.format(self.pending_table, 
@@ -426,15 +440,18 @@
             name = self.pending['file']
         self.update_status('Read model')
         try:
             self.CloudyModel = pc.CloudyModel('{0}/{1}/{2}'.format(self.models_dir, self.pending['dir'], name), 
                                               read_cont=True, list_elem = LIST_ALL_ELEM)
             if not self.CloudyModel.aborted:
                 self.update_status('Model read')
-                status = True
+                if 'wrong' in self.CloudyModel.out:
+                    status = False
+                else:
+                    status = True
             else:
                 self.update_status('Model not read')
                 status = False
         except:
             self.update_status('Model not read')
             status = False
             self.log_.warn('Model {0} not read in {1}/{2}/{3}'.format(name, self.models_dir, self.pending['dir'], name))
@@ -460,68 +477,126 @@
         self.insert_in_dic('logQ2', np.log10(self.CloudyModel.Q[2]))
         self.insert_in_dic('logQ3', np.log10(self.CloudyModel.Q[3]))
         self.insert_in_dic('logPhi', np.log10(self.CloudyModel.Phi0))
         self.insert_in_dic('logPhi0', np.log10(self.CloudyModel.Phi[0]))
         self.insert_in_dic('logPhi1', np.log10(self.CloudyModel.Phi[1]))
         self.insert_in_dic('logPhi2', np.log10(self.CloudyModel.Phi[2]))
         self.insert_in_dic('logPhi3', np.log10(self.CloudyModel.Phi[3]))
+            
         self.insert_in_dic('Cloudy_version', self.CloudyModel.cloudy_version)
+        if 'Cloudy ends' in self.CloudyModel.out:
+            self.insert_in_dic('CloudyEnds', self.CloudyModel.out['Cloudy ends'])
+        if '###First' in self.CloudyModel.out:
+            self.insert_in_dic('FirstZone', self.CloudyModel.out['###First'])
+        if '###Last' in self.CloudyModel.out:
+            self.insert_in_dic('LastZone', self.CloudyModel.out['###Last'])
+        if 'stop' in self.CloudyModel.out:
+            self.insert_in_dic('CalculStop', self.CloudyModel.out['stop'])
+        self.insert_in_dic('t2_H1', self.CloudyModel.get_t2_ion_vol_ne('H',1))
+        self.insert_in_dic('t2_O1', self.CloudyModel.get_t2_ion_vol_ne('O',1))
+        self.insert_in_dic('t2_O2', self.CloudyModel.get_t2_ion_vol_ne('O',2))
+        self.insert_in_dic('t2_O3', self.CloudyModel.get_t2_ion_vol_ne('O',3))
+        self.insert_in_dic('ne_H1', self.CloudyModel.get_ne_ion_vol_ne('H',1))
+        self.insert_in_dic('ne_O1', self.CloudyModel.get_ne_ion_vol_ne('O',1))
+        self.insert_in_dic('ne_O2', self.CloudyModel.get_ne_ion_vol_ne('O',2))
+        self.insert_in_dic('ne_O3', self.CloudyModel.get_ne_ion_vol_ne('O',3))
+        self.insert_in_dic('H_mass', self.CloudyModel.H_mass)
+        self.insert_in_dic('H1_mass', self.CloudyModel.Hp_mass)
+        self.insert_in_dic('nH_mean', self.CloudyModel.nH_mean)
+        self.insert_in_dic('Hb_SB', self.CloudyModel.get_Hb_SB())
+        self.insert_in_dic('Hb_EW', self.CloudyModel.get_Hb_EW())
+        self.insert_in_dic('Ha_EW', self.CloudyModel.get_Ha_EW())
         if self.CloudyModel.n_zones > 1:
+            for E in ('11.26', '35.12', '40.73', '47.45', '77.41', '113.90', 
+                      '138.12', '151.06', '233.60', '262.10', '361.00'):
+                Eev = float(E)
+                logQE = np.log10(self.CloudyModel.get_interp_cont(x_value=Eev,
+                                                                             x_unit='eV',
+                                                                             unit='Q'))
+                logPhiE = logQE - np.log10(4 * np.pi * self.CloudyModel.radius[0]**2)
+            
+                self.insert_in_dic('logQ{}'.format(E), logQE)
+                self.insert_in_dic('logPhi{}'.format(E), logPhiE)
             self.insert_in_dic('DepthFrac', self.CloudyModel.depth[-1] / self.CloudyModel.depth_full[-1])
             self.insert_in_dic('MassFrac', self.CloudyModel.H_mass / self.CloudyModel.H_mass_full[-1])
             self.insert_in_dic('HbFrac', self.CloudyModel.Hbeta / self.CloudyModel.Hbeta_full[-1])
-            if 'Cloudy ends' in self.CloudyModel.out:
-                self.insert_in_dic('CloudyEnds', self.CloudyModel.out['Cloudy ends'])
-            if '###First' in self.CloudyModel.out:
-                self.insert_in_dic('FirstZone', self.CloudyModel.out['###First'])
-            if '###Last' in self.CloudyModel.out:
-                self.insert_in_dic('LastZone', self.CloudyModel.out['###Last'])
-            if 'stop' in self.CloudyModel.out:
-                self.insert_in_dic('CalculStop', self.CloudyModel.out['stop'])
             self.insert_in_dic('logU_in', self.CloudyModel.log_U[0])
             self.insert_in_dic('logU_out', self.CloudyModel.log_U[-1])
             self.insert_in_dic('logU_mean', self.CloudyModel.log_U_mean_ne)
-            self.insert_in_dic('t2_H1', self.CloudyModel.get_t2_ion_vol_ne('H',1))
-            self.insert_in_dic('t2_O1', self.CloudyModel.get_t2_ion_vol_ne('O',1))
-            self.insert_in_dic('t2_O2', self.CloudyModel.get_t2_ion_vol_ne('O',2))
-            self.insert_in_dic('t2_O3', self.CloudyModel.get_t2_ion_vol_ne('O',3))
-            self.insert_in_dic('ne_H1', self.CloudyModel.get_ne_ion_vol_ne('H',1))
-            self.insert_in_dic('ne_O1', self.CloudyModel.get_ne_ion_vol_ne('O',1))
-            self.insert_in_dic('ne_O2', self.CloudyModel.get_ne_ion_vol_ne('O',2))
-            self.insert_in_dic('ne_O3', self.CloudyModel.get_ne_ion_vol_ne('O',3))
-            self.insert_in_dic('H_mass', self.CloudyModel.H_mass)
-            self.insert_in_dic('H1_mass', self.CloudyModel.Hp_mass)
-            self.insert_in_dic('nH_mean', self.CloudyModel.nH_mean)
+            self.insert_in_dic('THp', self.CloudyModel.get_T0_ion_vol_ne(elem='H', ion=1))
             self.insert_in_dic('nH_in', self.CloudyModel.nH[0])
             self.insert_in_dic('nH_out', self.CloudyModel.nH[-1])
-            self.insert_in_dic('Hb_SB', self.CloudyModel.get_Hb_SB())
-            self.insert_in_dic('Hb_EW', self.CloudyModel.get_Hb_EW())
-            self.insert_in_dic('Ha_EW', self.CloudyModel.get_Ha_EW())
-                 
+            try:
+                Radio = self.CloudyModel.get_interp_cont(unit='WmHz', x_unit='GHz', x_value=2.5)
+                self.insert_in_dic('Radio_2.5GHz', Radio)
+            except:
+                self.insert_in_dic('Radio_2.5GHz', -40)
+            try:
+                Radio = self.CloudyModel.get_interp_cont(unit='WmHz', x_unit='GHz', x_value=4.9)
+                self.insert_in_dic('Radio_4.9GHz', Radio)
+            except:
+                self.insert_in_dic('Radio_4.9GHz', -40)
+            try:
+                Radio = self.CloudyModel.get_interp_cont(unit='WmHz', x_unit='GHz', x_value=12.)
+                self.insert_in_dic('Radio_12GHz', Radio)
+            except:
+                self.insert_in_dic('Radio_12GHz', -40)
+            try:
+                Radio = self.CloudyModel.get_interp_cont(unit='WmHz', x_unit='GHz', x_value=20.)
+                self.insert_in_dic('Radio_20GHz', Radio)
+            except:
+                self.insert_in_dic('Radio_20GHz', -40)
+        else:
+            for E in ('11.26', '35.12', '40.73', '47.45', '77.41', '113.90', 
+                      '138.12', '151.06', '233.60', '262.10', '361.00'):
+                Eev = float(E)
+                logQE = np.log10(self.CloudyModel.get_interp_cont(x_value=Eev,
+                                                                             x_unit='eV',
+                                                                             unit='Q'))
+                logPhiE = logQE - np.log10(4 * np.pi * self.CloudyModel.radius**2)
+            
+                self.insert_in_dic('logQ{}'.format(E), logQE)
+                self.insert_in_dic('logPhi{}'.format(E), logPhiE)
+            self.insert_in_dic('logU_in', self.CloudyModel.log_U)
+            self.insert_in_dic('logU_out', self.CloudyModel.log_U)
+            self.insert_in_dic('logU_mean', self.CloudyModel.log_U_mean_ne)
+            self.insert_in_dic('nH_in', self.CloudyModel.nH)
+            self.insert_in_dic('nH_out', self.CloudyModel.nH)
+                
     def lines2dic(self):
         
         if self.CloudyModel.n_zones > 1:
+            # Adding some recombination lines from PyNeb
+            self.lines, N_lines = self.MdB.select_dB(select_='id, lambda, label, name', from_=self.OVN_dic['lines_table'], 
+                                                where_='used = 1', limit_=None, format_='numpy', 
+                                                dtype_=[('id', 'U20'), ('lambda', '<f8'), ('label', 'U15'), ('name', 'U40')])
+            for line in self.lines:
+                label = line['label']
+                if label[-2:] == 'PN' and label not in self.CloudyModel.emis_labels:
+                    atom = self.RecDic[label[0:4]]
+                    self.CloudyModel.add_emis_from_pyneb(label, atom, line['name'].split()[2][:-1])
+                    
             for clabel in self.CloudyModel.emis_labels:
                 self.insert_in_dic(clabel, self.CloudyModel.get_emis_vol(clabel))
                 self.insert_in_dic(clabel+'_rad', self.CloudyModel.get_emis_rad(clabel))
-                  
+
     def insert_model(self, add2dic=None):
         if not self.MdB.connected:
             self.log_.error('Not connected')
             return None
 
         self.pending2dic()
         self.model2dic()
         self.lines2dic()
         if add2dic is not None:
             for key in add2dic:
                 self.insert_in_dic(key, add2dic[key])
         
-        fields_str = '`datetime`, '
-        values_str = 'now(), '
+        fields_str = '`datetime`, `host`, '
+        values_str = "now(), '{}', ".format(self.host)
         
         for key in self._dic:
             if self._dic[key] is not None:
                 if key in self.fields:
                     fields_str += '`{0}`, '.format(key)
                     if type(self._dic[key]) == type(''):
                         values_str += "'{0}', ".format(self._dic[key])
@@ -584,15 +659,19 @@
          
         if self.CloudyModel.n_zones > 1:
             fields_str = '`N`, `ref`,'
             values_tem_str = "{0}, '{1}',".format(self.last_N,  self._dic['ref'])
             for clabel in self.CloudyModel.emis_labels:
                 try:
                     fields_str += '`T_{0}`, '.format(clabel)
-                    values_tem_str += '{0}, '.format(self.CloudyModel.get_T0_emis(clabel))
+                    t_emis = self.CloudyModel.get_T0_emis(clabel)
+                    if np.isfinite(t_emis):
+                        values_tem_str += '{0}, '.format(t_emis)
+                    else:
+                        values_tem_str += '0.0,'
                 except:
                     pass
             fields_str = fields_str[:-2]
             values_tem_str = values_tem_str[:-2]
             command = 'INSERT INTO {0} ({1}) VALUES ({2});'.format(self.OVN_dic['temis_table'], fields_str, values_tem_str)
             self.MdB.exec_dB(command)
         self.update_status('Temis inserted') #17
@@ -624,35 +703,40 @@
             self.MdB.connect_dB()
         self.table = self.OVN_dic['master_table']
         self.pending_table = self.OVN_dic['pending_table']
         self.proc_name = proc_name
         self.models_dir = models_dir
         self.do_update_status = do_update_status        
         self.lines, N_lines = MdB.select_dB(select_='id, lambda, label, name', from_=self.OVN_dic['lines_table'], 
-                                           where_='used = 1', limit_=None, format_='numpy')
+                                           where_='used = 1', limit_=None, format_='numpy', 
+                                           dtype_=[('id', 'U20'), ('lambda', '<f8'), ('label', 'U15'), ('name', 'U40')])
        
         if register:
             self.get_ID()
         self.init_CloudyInput()
     
     def get_emis_table(self):
         emis_tab = []
         for line in self.lines:
             ide = line['id']
-            lambda_ = line['lambda']
-            unit = line['label'][-1]
-            if lambda_ > 1000:
-                lambda_str = '{0:5.0f}'.format(lambda_)
-            elif lambda_ > 100:
-                lambda_str = '{0:5.1f}'.format(lambda_)
-            elif lambda_ > 10:
-                lambda_str = '{0:5.2f}'.format(lambda_)
-            else:
-                lambda_str = '{0:5.3f}'.format(lambda_)
-            emis_tab.append('{0} {1}{2}'.format(ide, lambda_str, unit))
+            label = line['label']
+            if label[-2:] != 'PN':
+                lambda_ = line['lambda']
+                if lambda_ > 1000:
+                    lambda_str = '{0:5.2f}'.format(lambda_)
+                elif lambda_ > 100:
+                    lambda_str = '{0:5.3f}'.format(lambda_)
+                elif lambda_ > 10:
+                    lambda_str = '{0:5.4f}'.format(lambda_)
+                else:
+                    lambda_str = '{0:5.5f}'.format(lambda_)
+                unit = line['label'][-1]
+                if unit == 'C':
+                    unit = 'M'
+                emis_tab.append('{0} {1}{2}'.format(ide, lambda_str, unit))
         return emis_tab
     
     def init_CloudyInput(self):
         self.CloudyInput = pc.CloudyInput()
         self.CloudyInput.save_list = [['radius', '.rad'], 
                                       ['physical conditions', '.phy'],
                                       ['continuum', '.cont']]
@@ -662,15 +746,20 @@
     def get_ID(self):
         table=self.OVN_dic['procIDs_table']
         if not self.MdB.connected:
             self.log_.error('Not connected')
             return None
         
         host = os.getenv('HOST')
+        if host is None:
+            host = os.getenv('HOSTNAME')
+        if host is None:
+            host = 'localhost'
         user = os.getenv('USER')
+        print(table, self.proc_name, user, host)
         command = 'INSERT INTO {0} (`proc_name`, `datetime`, `user`, `host`) VALUES ("{1:s}", now(), "{2:s}", "{3:s}");'.format(table, self.proc_name, user, host)
         self.MdB.exec_dB(command)
         res, N = self.MdB.select_dB(select_='last_insert_id()', from_=table)
         self.procID = res[0]['last_insert_id()']
         
     def select_pending(self):
 
@@ -908,27 +997,28 @@
     rc = runCloudy(MdB = MdB, do_update_status=False, register=False, models_dir='./')
     rc.fill_CloudyInput(N, dir=dir, parameters=parameters, read_tab=read_tab)
     if close_after:
         MdB.close_dB()
 
 class runCloudyByThread(threading.Thread):
 
-    def __init__(self, OVN_dic, models_dir, norun=False, noinput=False):
+    def __init__(self, OVN_dic, models_dir, norun=False, noinput=False, clean=True):
         
         self.log_ = pc.log_
         threading.Thread.__init__(self)
         self._stop = threading.Event()
         self.models_dir = models_dir
         self.norun = norun
         self.noinput = noinput
         self.MdB = None
         self.sleep_time = 10.
         self.setDaemon(True)
         self.OVN_dic = OVN_dic
         self.calling = 'runCloudyByThread'
+        self.clean = clean
     
     def run(self):
         
         self.MdB = pc.MdB(self.OVN_dic)
         tname = threading.currentThread().getName()
         rC = runCloudy(self.MdB, OVN_dic = self.OVN_dic, models_dir = self.models_dir, proc_name=tname)
         
@@ -971,15 +1061,16 @@
                                 master_N.append(wT.last_N)
                         Ncuts = rC.pending['N_Hb_cut']
                         for Hbeta_cut in np.linspace(0, 1, Ncuts + 2)[1:-1]:
                             if wT.CloudyModel.n_zones > 1:
                                 wT.CloudyModel.Hbeta_cut = Hbeta_cut * wT.CloudyModel.Hbeta_full[-1]
                                 wT.insert_model()
                                 master_N.append(wT.last_N)
-                    wT.clean_files()
+                    if self.clean:
+                        wT.clean_files()
                     self.log_.message('model {0} finished, inserted into {1}.'.format(self.selectedN, master_N), 
                                  calling=self.calling)
             else:
                 time.sleep(self.sleep_time)
             
         self.MdB.close_dB()
 
@@ -1198,23 +1289,27 @@
                     self.obs.addLine(EL)
                 else:
                     if EL.corrIntens.size == n_lines:
                         self.obs.addLine(EL)
 
 class manage3MdB(object):
     
-    def __init__(self, OVN_dic, models_dir='/DATA/MdB', Nprocs=pn.config.Nprocs):
+    def __init__(self, OVN_dic, models_dir='/DATA/MdB', Nprocs=pn.config.Nprocs,
+                 clean=True):
         self.OVN_dic = OVN_dic
         self.models_dir = models_dir
         self.Nprocs = Nprocs
+        self.clean = clean
                 
-    def start(self, norun=False, noinput=False):
+    def start(self, norun=False, noinput=False, clean=True):
         self.all_threads = []
         for i in range(self.Nprocs):
-            self.all_threads.append(runCloudyByThread(self.OVN_dic, self.models_dir, norun=norun, noinput=noinput))
+            self.all_threads.append(runCloudyByThread(self.OVN_dic, self.models_dir, 
+                                                      norun=norun, noinput=noinput,
+                                                      clean=self.clean))
         for t in self.all_threads:
             t.start()
             
     def restart(self):
         for t in self.all_threads:
             t.start()        
     
@@ -1227,15 +1322,15 @@
     Print all the references from the master table, with the number of entries for each.
     """
     if MdB is None:
         MdB = pc.MdB(OVN_dic=OVN_dic)
     else:
         OVN_dic = MdB.OVN_dic
     if not isinstance(MdB, pc.MdB):
-        self.log_.error('The first argument must be a MdB object')    
+        pc.log_.error('The first argument must be a MdB object')    
     res, N_ref = MdB.select_dB(select_ = 'distinct(ref), count(*)', from_ = OVN_dic['master_table'], 
                                group_ = 'ref', limit_ = None)
     for row in res:
         print(('The ref "{0:15}" counts {1:8d} entries.'.format(row['ref'], row['count(*)'])))
     print(('Number of distinct references = {0}'.format(N_ref)))
     
 def print_all_lines(MdB = None, OVN_dic=None, limit_=None):
@@ -1244,30 +1339,30 @@
     A limit can be given
     """
     if MdB is None:
         MdB = pc.MdB(OVN_dic=OVN_dic)
     else:
         OVN_dic = MdB.OVN_dic
     if not isinstance(MdB, pc.MdB):
-        self.log_.error('The first argument must be a MdB object')    
+        pc.log_.error('The first argument must be a MdB object')    
     lines, N_lines = MdB.select_dB(select_ = '*', from_ = OVN_dic['lines_table'], limit_ = limit_)
     for line in lines:
         print(('Nl = {0[Nl]:3} id = {0[id]:4} label = {0[label]:5} wavelength = {0[lambda]:6} full name = {0[name]}'.format(line)))
 
 def print_status_stats(MdB = None, OVN_dic=None, ref_=None):
     """
     Print the number of pending models for each status.
     A reference can be given. 
     """
     if MdB is None:
         MdB = pc.MdB(OVN_dic=OVN_dic)
     else:
         OVN_dic = MdB.OVN_dic
     if not isinstance(MdB, pc.MdB):
-        self.log_.error('The first argument must be a MdB object')
+        pc.log_.error('The first argument must be a MdB object')
     if ref_ is not None:
         where_ = 'ref = "{0}"'.format(ref_)
     else:
         where_ = None
     res, N_res = MdB.select_dB(select_='status, count(*) as ct',from_=OVN_dic['pending_table'],
                                where_=where_, group_='status', limit_=None, commit=True)
     for status in res: 
@@ -1279,15 +1374,15 @@
     A reference can be given
     """
     if MdB is None:
         MdB = pc.MdB(OVN_dic=OVN_dic)
     else:
         OVN_dic = MdB.OVN_dic
     if not isinstance(MdB, pc.MdB):
-        self.log_.error('The first argument must be a MdB object')
+        pc.log_.error('The first argument must be a MdB object')
     if ref_ is not None:
         where_ = 'ref = "{0}"'.format(ref_)
     else:
         where_ = None
     res, N_res = MdB.select_dB(select_='avg(substring_index(CloudyEnds,"ExecTime(s)", -1)) as MRT, '\
                                'min(substring_index(CloudyEnds,"ExecTime(s)", -1)) as MN, '\
                                'max(substring_index(CloudyEnds,"ExecTime(s)", -1)) as MX',
@@ -1300,30 +1395,30 @@
     A reference can be given
     """
     if MdB is None:
         MdB = pc.MdB(OVN_dic=OVN_dic)
     else:
         OVN_dic = MdB.OVN_dic
     if not isinstance(MdB, pc.MdB):
-        self.log_.error('The first argument must be a MdB object')
+        pc.log_.error('The first argument must be a MdB object')
     if ref_ is not None:
         where_ = 'ref = "{0}"'.format(ref_)
     else:
         where_ = None
     res, N_res = MdB.select_dB(select_='time_to_sec(timediff(max(datetime),min(datetime))) as ET',
                                from_=OVN_dic['master_table'], where_=where_, limit_=None)
     print(('Models running during = {0}'.format(datetime.timedelta(seconds=res[0]['ET']))))
     
 def print_ETA(MdB= None, OVN_dic=None, ref_=None):
     if MdB is None:
         MdB = pc.MdB(OVN_dic=OVN_dic)
     else:
         OVN_dic = MdB.OVN_dic
     if not isinstance(MdB, pc.MdB):
-        self.log_.error('The first argument must be a MdB object')
+        pc.log_.error('The first argument must be a MdB object')
     if ref_ is not None:
         where_ = 'ref = "{0}"'.format(ref_)
     else:
         where_ = ''
     res, N_res = MdB.select_dB(select_='count(*)',from_=OVN_dic['pending_table'],
                                where_=where_ + ' AND status=0', limit_=None, commit=True)
     N_pending = res[0]['count(*)']
@@ -1339,15 +1434,15 @@
 
 def print_efficiency(MdB= None, OVN_dic=None, ref_=None):
     if MdB is None:
         MdB = pc.MdB(OVN_dic=OVN_dic)
     else:
         OVN_dic = MdB.OVN_dic
     if not isinstance(MdB, pc.MdB):
-        self.log_.error('The first argument must be a MdB object')
+        pc.log_.error('The first argument must be a MdB object')
     if ref_ is not None:
         where_ = 'ref = "{0}"'.format(ref_)
     else:
         where_ = ''
     res, N_res = MdB.select_dB(select_='count(*)',from_=OVN_dic['pending_table'],
                                where_=where_ + 'AND status=50', limit_=None, commit=True)
     N_run = res[0]['count(*)']
@@ -1364,39 +1459,60 @@
     
 def print_infos(MdB= None, OVN_dic=None, ref_=None, where_=None, Nprocs=32):
     if MdB is None:
         MdB = pc.MdB(OVN_dic=OVN_dic)
     else:
         OVN_dic = MdB.OVN_dic
     if not isinstance(MdB, pc.MdB):
-        self.log_.error('The first argument must be a MdB object')
-    if ref_ is not None:
-        this_where_ = 'ref = "{0}"'.format(ref_)
+        pc.log_.error('The first argument must be a MdB object')
+        
+    if ref_ is None:
+        where_ref = ''
     else:
-        this_where_ = ''
-    if where_ is not None:
-        this_where_ += ' AND {}'.format(where_)
+        where_ref = 'ref = "{0}"'.format(ref_)
+    
+    if where_ is None:
+        where_where = ''
+    else:
+        where_where = where_
+    this_where = ' AND '.join([i for i in (where_ref,where_where,'status=0') if i != ''])
+    if this_where == '':
+        this_where = None
+        
     res, N_res = MdB.select_dB(select_='count(*)',from_=OVN_dic['pending_table'],
-                               where_=this_where_ + ' AND status=0', limit_=None, commit=True)
+                               where_=this_where, 
+                               limit_=None, commit=True)
     N_pending = res[0]['count(*)']
+    this_where = ' AND '.join([i for i in (where_ref,where_where,'status=50') if i != ''])
+    if this_where == '':
+        this_where = None
     res, N_res = MdB.select_dB(select_='count(*)',from_=OVN_dic['pending_table'],
-                               where_=this_where_ + ' AND status=50', limit_=None, commit=True)
+                               where_=this_where, 
+                               limit_=None, commit=True)
     N_run = res[0]['count(*)']
     if N_run == 0 and N_pending == 0:
         print('No entry')
         return
+    this_where = ' AND '.join([i for i in (where_ref,where_where) if i != ''])
+    if this_where == '':
+        this_where = None
+    
     res_et, N_res = MdB.select_dB(select_='time_to_sec(timediff(max(datetime),min(datetime))) as ET',
-                               from_=OVN_dic['master_table'], where_=this_where_, limit_=None)
+                               from_=OVN_dic['master_table'], 
+                               where_=this_where, 
+                               limit_=None)
     ET = res_et[0]['ET']
     
     eta = datetime.datetime.today() + datetime.timedelta(seconds=ET/float(N_run)*N_pending)
     res, N_res = MdB.select_dB(select_='avg(cast(substring_index(CloudyEnds,"ExecTime(s)", -1) as decimal)) as MRT, '\
                                'min(cast(substring_index(CloudyEnds,"ExecTime(s)", -1) as decimal)) as MN, '\
                                'max(cast(substring_index(CloudyEnds,"ExecTime(s)", -1) as decimal)) as MX',
-                              from_=OVN_dic['master_table'], where_=this_where_, limit_=None)
+                              from_=OVN_dic['master_table'], 
+                              where_=this_where, 
+                              limit_=None)
     MRT = float(res[0]['MRT'])
     MN = float(res[0]['MN'])
     MX = float(res[0]['MX'])
     Mean_eff = np.float(N_run)*MRT/ET
     eta2 = datetime.datetime.today() + datetime.timedelta(seconds=MRT*N_pending/float(Nprocs))
     print(('{} pending, {} run'.format(N_pending, N_run)))
     print(('Mean running time = {0:.0f}s, min = {1:.0f}s, max = {2:.0f}s'.format(MRT, MN, MX)))
```

### Comparing `pyCloudy-0.9.7/pyCloudy/utils/Config.py` & `pyCloudy-0.9.9/pyCloudy/utils/Config.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,16 @@
         if 'CLOUDY_EXE' in os.environ:
             self.cloudy_exe = os.environ['CLOUDY_EXE']
         else:
             self.cloudy_exe = 'cloudy.exe'
         
         self.cloudy_dict = {'10.00': '/usr/local/Cloudy/c10.00/cloudy.exe',
                             '13.03': '/usr/local/Cloudy/c13.03/source/cloudy.exe',
-                            '17.00': '/usr/local/Cloudy/c17.00/source/cloudy.exe'}
+                            '17.00': '/usr/local/Cloudy/c17.00/source/cloudy.exe',
+                            '17.01': '/usr/local/Cloudy/c17.01/source/cloudy.exe'}
             
         self.INSTALLED ={}
         try:
             try:
                 from matplotlib.tri.triangulation import Triangulation
             except:
                 from matplotlib.delaunay import Triangulation
```

### Comparing `pyCloudy-0.9.7/pyCloudy/utils/convert_c17_c13.txt` & `pyCloudy-0.9.9/pyCloudy/utils/convert_c17_c13.txt`

 * *Files identical despite different names*

### Comparing `pyCloudy-0.9.7/pyCloudy/utils/convert_c17_c13_2.txt` & `pyCloudy-0.9.9/pyCloudy/utils/convert_c17_c13_2.txt`

 * *Files identical despite different names*

### Comparing `pyCloudy-0.9.7/pyCloudy/utils/init.py` & `pyCloudy-0.9.9/pyCloudy/utils/init.py`

 * *Files identical despite different names*

### Comparing `pyCloudy-0.9.7/pyCloudy/utils/Izotov2013_CR.txt` & `pyCloudy-0.9.9/pyCloudy/utils/Izotov2013_CR.txt`

 * *Files identical despite different names*

### Comparing `pyCloudy-0.9.7/pyCloudy/utils/logging.py` & `pyCloudy-0.9.9/pyCloudy/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pyCloudy-0.9.7/pyCloudy/utils/misc.py` & `pyCloudy-0.9.9/pyCloudy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `pyCloudy-0.9.7/pyCloudy/utils/pyneb2cloudy.txt` & `pyCloudy-0.9.9/pyCloudy/utils/pyneb2cloudy.txt`

 * *Files identical despite different names*

### Comparing `pyCloudy-0.9.7/pyCloudy/utils/red_corr.py` & `pyCloudy-0.9.9/pyCloudy/utils/red_corr.py`

 * *Files identical despite different names*

### Comparing `pyCloudy-0.9.7/pyCloudy.egg-info/PKG-INFO` & `pyCloudy-0.9.9/pyCloudy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 1.2
 Name: pyCloudy
-Version: 0.9.7
+Version: 0.9.9
 Summary: Tools to manage Astronomical Cloudy photoionization code
 Home-page: https://sites.google.com/site/pycloudy/
 Author: Christophe Morisset IA-UNAM
 Author-email: chris.morisset@gmail.com
 Maintainer: Christophe Morisset IA-UNAM
 Maintainer-email: chris.morisset@gmail.com
 License: GPL
-Download-URL: https://github.com/Morisset/pyCloudy/releases/tag/0.9.7
+Download-URL: https://github.com/Morisset/pyCloudy/releases/tag/0.9.9
 Description: PyCloudy is a Python library to deal with input and output files of Cloudy (Gary Ferland) photoionization code.
         Is also allows to generate 3D nebula from various runs of the 1D Cloudy code.
         
         Requirements
         ============
         
         You will need to have installed `Cloudy <http://nublado.org/>`_ .
```

### Comparing `pyCloudy-0.9.7/pyCloudy.egg-info/SOURCES.txt` & `pyCloudy-0.9.9/pyCloudy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 pyCloudy.egg-info/top_level.txt
 pyCloudy/c1d/__init__.py
 pyCloudy/c1d/cloudy_model.py
 pyCloudy/c3d/__init__.py
 pyCloudy/c3d/model_3d.py
 pyCloudy/db/MdB.py
 pyCloudy/db/__init__.py
+pyCloudy/db/continuum_bands.ini
 pyCloudy/db/initSQL.py
 pyCloudy/db/use3MdB.py
 pyCloudy/utils/Config.py
 pyCloudy/utils/Izotov2013_CR.txt
 pyCloudy/utils/__init__.py
 pyCloudy/utils/astro.py
 pyCloudy/utils/convert_c17_c13.txt
```

### Comparing `pyCloudy-0.9.7/README.rst` & `pyCloudy-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyCloudy-0.9.7/setup.py` & `pyCloudy-0.9.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,16 @@
       author='Christophe Morisset IA-UNAM',
       author_email='chris.morisset@gmail.com',
       maintainer='Christophe Morisset IA-UNAM',
       maintainer_email='chris.morisset@gmail.com',
       url='https://sites.google.com/site/pycloudy/',
       download_url = 'https://github.com/Morisset/pyCloudy/releases/tag/{}'.format(__version__),
       packages=['pyCloudy','pyCloudy.c1d','pyCloudy.c3d','pyCloudy.utils', 'pyCloudy.db'],
-      package_data={'pyCloudy.utils':['*txt']},
+      package_data={'pyCloudy.utils':['*txt'],
+                    'pyCloudy.db': ['*.ini']},
       classifiers=['Development Status :: 5 - Production/Stable',
                    'Intended Audience :: Science/Research',
                    'License :: Free for non-commercial use',
                    'Programming Language :: Python :: 2',
                    'Topic :: Scientific/Engineering :: Astronomy'
                    ],
       license='GPL',
```

