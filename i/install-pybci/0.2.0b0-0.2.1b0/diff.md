# Comparing `tmp/install-pybci-0.2.0b0.tar.gz` & `tmp/install-pybci-0.2.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install-pybci-0.2.0b0.tar", last modified: Tue May 23 18:35:00 2023, max compression
+gzip compressed data, was "install-pybci-0.2.1b0.tar", last modified: Sat May 27 02:47:17 2023, max compression
```

## Comparing `install-pybci-0.2.0b0.tar` & `install-pybci-0.2.1b0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:35:00.313146 install-pybci-0.2.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-23 18:34:28.000000 install-pybci-0.2.0b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-23 18:34:28.000000 install-pybci-0.2.0b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-05-23 18:35:00.313146 install-pybci-0.2.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6762 2023-05-23 18:34:28.000000 install-pybci-0.2.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:35:00.309146 install-pybci-0.2.0b0/install_pybci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-05-23 18:35:00.000000 install-pybci-0.2.0b0/install_pybci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-23 18:35:00.000000 install-pybci-0.2.0b0/install_pybci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:35:00.000000 install-pybci-0.2.0b0/install_pybci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-23 18:35:00.000000 install-pybci-0.2.0b0/install_pybci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 18:35:00.000000 install-pybci-0.2.0b0/install_pybci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:35:00.309146 install-pybci-0.2.0b0/pybci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:35:00.309146 install-pybci-0.2.0b0/pybci/Configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-23 18:34:28.000000 install-pybci-0.2.0b0/pybci/Configuration/EpochSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-23 18:34:28.000000 install-pybci-0.2.0b0/pybci/Configuration/FeatureSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-23 18:34:28.000000 install-pybci-0.2.0b0/pybci/Configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:35:00.313146 install-pybci-0.2.0b0/pybci/ThreadClasses/
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/ThreadClasses/AsyncDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/ThreadClasses/ClassifierThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/ThreadClasses/DataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/ThreadClasses/FeatureProcessorThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/ThreadClasses/MarkerThread.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/ThreadClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:35:00.313146 install-pybci-0.2.0b0/pybci/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/Utils/Classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/Utils/FeatureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/Utils/LSLScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14751 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/pybci.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/pybci/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 18:35:00.313146 install-pybci-0.2.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-23 18:34:29.000000 install-pybci-0.2.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:47:17.976166 install-pybci-0.2.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-05-27 02:47:17.976166 install-pybci-0.2.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:47:17.972166 install-pybci-0.2.1b0/install_pybci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-05-27 02:47:17.000000 install-pybci-0.2.1b0/install_pybci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-27 02:47:17.000000 install-pybci-0.2.1b0/install_pybci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 02:47:17.000000 install-pybci-0.2.1b0/install_pybci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-27 02:47:17.000000 install-pybci-0.2.1b0/install_pybci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 02:47:17.000000 install-pybci-0.2.1b0/install_pybci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:47:17.972166 install-pybci-0.2.1b0/pybci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:47:17.972166 install-pybci-0.2.1b0/pybci/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/Configuration/EpochSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/Configuration/FeatureSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/Configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:47:17.976166 install-pybci-0.2.1b0/pybci/ThreadClasses/
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/ThreadClasses/AsyncDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6882 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/ThreadClasses/ClassifierThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/ThreadClasses/DataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/ThreadClasses/FeatureProcessorThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/ThreadClasses/MarkerThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/ThreadClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:47:17.976166 install-pybci-0.2.1b0/pybci/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/Utils/Classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/Utils/FeatureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/Utils/LSLScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15185 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/pybci.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/pybci/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 02:47:17.976166 install-pybci-0.2.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-27 02:46:41.000000 install-pybci-0.2.1b0/setup.py
```

### Comparing `install-pybci-0.2.0b0/LICENSE` & `install-pybci-0.2.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.0b0/PKG-INFO` & `install-pybci-0.2.1b0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,26 @@
-Metadata-Version: 2.1
-Name: install-pybci
-Version: 0.2.0b0
-Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
-Home-page: https://github.com/lmbooth/pybci
-Author: Liam Booth
-Author-email: liambooth123@hotmail.co.uk
-License: MIT
-Keywords: machine learning and data synchronisation on the Lab Streaming Layer
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: System :: Networking
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
 [![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
-A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
+A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
-The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
+The goal of PyBCI is to enable quick iteration when creating pipelines for testing human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
 
 (currently using install-pybci due to pybci having name too similar with another package on pypi)
 
 [ReadTheDocs available here!](https://pybci.readthedocs.io/en/latest/)      [Examples found here!](https://github.com/LMBooth/pybci/tree/main/pybci/Examples)
 
+[Examples of supported LSL hardware here!](https://labstreaminglayer.readthedocs.io/info/supported_devices.html)
+
 ## Basic implementation
 ```python
 import time
 from pybci import PyBCI
 bci = PyBCI() # set default epoch timing, looks for first available lsl stream and all data streams
 bci.TrainMode() # assume both marker and datastreams available to start training on received epochs
 accuracy = 0
@@ -71,10 +49,12 @@
 PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled physiological sensor data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count for more then one marker, example: a baseline marker may have one marker sent for a 60 second window, where as target actions may only be ~0.5s long, so to conform when testing the model and giving a standardised window length would be desirable to split the 60s window after the received baseline marker in to ~0.5s windows. By overlapping windows we try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the mdoel will begin to fit. Once fit classifier info can be queried with CurrentClassifierInfo, when a desired accuracy is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
-- Combine multiple data streams for multi modal bci!
+- ~~Combine multiple data streams for multi modal bci!~~
+- Add pytorch compatibility! 
+- Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.
 
 ## Curently in Beta, come back in a few days for updates!
```

### Comparing `install-pybci-0.2.0b0/README.md` & `install-pybci-0.2.1b0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,50 @@
+Metadata-Version: 2.1
+Name: install-pybci
+Version: 0.2.1b0
+Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
+Home-page: https://github.com/lmbooth/pybci
+Author: Liam Booth
+Author-email: liambooth123@hotmail.co.uk
+License: MIT
+Keywords: machine learning and data synchronisation on the Lab Streaming Layer
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: System :: Networking
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
 [![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
-A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
+A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
-The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
+The goal of PyBCI is to enable quick iteration when creating pipelines for testing human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
 
 (currently using install-pybci due to pybci having name too similar with another package on pypi)
 
 [ReadTheDocs available here!](https://pybci.readthedocs.io/en/latest/)      [Examples found here!](https://github.com/LMBooth/pybci/tree/main/pybci/Examples)
 
+[Examples of supported LSL hardware here!](https://labstreaminglayer.readthedocs.io/info/supported_devices.html)
+
 ## Basic implementation
 ```python
 import time
 from pybci import PyBCI
 bci = PyBCI() # set default epoch timing, looks for first available lsl stream and all data streams
 bci.TrainMode() # assume both marker and datastreams available to start training on received epochs
 accuracy = 0
@@ -47,10 +73,12 @@
 PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled physiological sensor data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count for more then one marker, example: a baseline marker may have one marker sent for a 60 second window, where as target actions may only be ~0.5s long, so to conform when testing the model and giving a standardised window length would be desirable to split the 60s window after the received baseline marker in to ~0.5s windows. By overlapping windows we try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the mdoel will begin to fit. Once fit classifier info can be queried with CurrentClassifierInfo, when a desired accuracy is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
-- Combine multiple data streams for multi modal bci!
+- ~~Combine multiple data streams for multi modal bci!~~
+- Add pytorch compatibility! 
+- Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.
 
 ## Curently in Beta, come back in a few days for updates!
```

### Comparing `install-pybci-0.2.0b0/install_pybci.egg-info/PKG-INFO` & `install-pybci-0.2.1b0/install_pybci.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.2.0b0
+Version: 0.2.1b0
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
@@ -22,27 +22,29 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
 [![pybci](https://raw.githubusercontent.com/LMBooth/pybci/main/docs/Images/pyBCITitle.svg)](https://github.com/LMBooth/pybci)
 
-A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
+A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [Pytorch](https://pytorch.org/), [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
-The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
+The goal of PyBCI is to enable quick iteration when creating pipelines for testing human machine and brain computer interfaces, namely testing applied data processing and feature extraction techniques on custom machine learning models. Training the BCI requires LSL enabled devices and an LSL marker stream for training stimuli. (The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware.)
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
 
 (currently using install-pybci due to pybci having name too similar with another package on pypi)
 
 [ReadTheDocs available here!](https://pybci.readthedocs.io/en/latest/)      [Examples found here!](https://github.com/LMBooth/pybci/tree/main/pybci/Examples)
 
+[Examples of supported LSL hardware here!](https://labstreaminglayer.readthedocs.io/info/supported_devices.html)
+
 ## Basic implementation
 ```python
 import time
 from pybci import PyBCI
 bci = PyBCI() # set default epoch timing, looks for first available lsl stream and all data streams
 bci.TrainMode() # assume both marker and datastreams available to start training on received epochs
 accuracy = 0
@@ -71,10 +73,12 @@
 PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled physiological sensor data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count for more then one marker, example: a baseline marker may have one marker sent for a 60 second window, where as target actions may only be ~0.5s long, so to conform when testing the model and giving a standardised window length would be desirable to split the 60s window after the received baseline marker in to ~0.5s windows. By overlapping windows we try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion. [See here for more information on epoch timing](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Epoch_Timing.html).
 
 Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, ideal for data stream types like "EEG" and "EMG". Since data analysis, preprocessing and feature extraction trechniques can vary greatly between device data inputs, a custom feature extraction class can be created for each data stream maker type. [See here for more information on feature extraction](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Feature_Selection.html).
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the mdoel will begin to fit. Once fit classifier info can be queried with CurrentClassifierInfo, when a desired accuracy is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state). [Review the examples for sklearn and model implementations](https://pybci.readthedocs.io/en/latest/BackgroundInformation/Examples.html).
 
 ## ToDo!
-- Combine multiple data streams for multi modal bci!
+- ~~Combine multiple data streams for multi modal bci!~~
+- Add pytorch compatibility! 
+- Run benchmark tests on DataReceiverThread.py and AsynDataReceiverThread.py, seeking potential optimisations.
 
 ## Curently in Beta, come back in a few days for updates!
```

### Comparing `install-pybci-0.2.0b0/install_pybci.egg-info/SOURCES.txt` & `install-pybci-0.2.1b0/install_pybci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.0b0/pybci/Configuration/EpochSettings.py` & `install-pybci-0.2.1b0/pybci/Configuration/EpochSettings.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.0b0/pybci/ThreadClasses/AsyncDataReceiverThread.py` & `install-pybci-0.2.1b0/pybci/ThreadClasses/AsyncDataReceiverThread.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import threading
+import threading, time
 from collections import deque
 import itertools
 from bisect import bisect_left
 def slice_fifo_by_time(fifo, start_time, end_time):
         """Find the slice of fifo between start_time and end_time using binary search."""
         # separate times and data for easier indexing
         times, data = zip(*fifo)
@@ -53,14 +53,16 @@
                     del sample[index] # remove the desired channels from the sample
                 for i,fifo in enumerate(dataFIFOs):
                     fifo.append((timestamp, sample[i]))
                 if self.trainTestEvent.is_set(): # We're training!
                     if self.startCounting: # we received a marker
                         posCount += 1
                         if posCount >= self.desiredCount:  # enough samples are in FIFO, chop up and put in dataqueue
+                            start = time.time()
+
                             if len(self.customEpochSettings.keys())>0: #  custom marker received
                                 if self.customEpochSettings[self.currentMarker].splitCheck: # slice epochs into overlapping time windows
                                     window_length = self.customEpochSettings[self.currentMarker].windowLength
                                     window_overlap = self.customEpochSettings[self.currentMarker].windowOverlap
                                     window_start_time = self.markerTimestamp + self.customEpochSettings[self.currentMarker].tmin
                                     window_end_time = window_start_time + window_length
                                     while window_end_time <= self.markerTimestamp + self.customEpochSettings[self.currentMarker].tmax:
@@ -87,14 +89,16 @@
                                     self.startCounting = False
                                 else: # don't slice just take tmin to tmax time
                                     start_time = self.markerTimestamp + self.globalEpochSettings.tmin
                                     end_time = self.markerTimestamp + self.globalEpochSettings.tmax
                                     sliceDataFIFOs = [slice_fifo_by_time(fifo, start_time, end_time) for fifo in dataFIFOs]
                                     self.dataQueueTrain.put([sliceDataFIFOs, self.currentMarker, self.sr, self.devCount])
                             # reset flags and counters
+                            end = time.time()
+                            print(f"Data slicing process time {end - start}")
                             posCount = 0
                             self.startCounting = False
                 else: # in Test mode
                     if self.globalEpochSettings.splitCheck:
                         window_length = self.globalEpochSettings.windowLength
                         window_overlap = self.globalEpochSettings.windowOverlap
                     else:
```

### Comparing `install-pybci-0.2.0b0/pybci/ThreadClasses/ClassifierThread.py` & `install-pybci-0.2.1b0/pybci/ThreadClasses/ClassifierThread.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from ..Utils.Classifier import Classifier 
-import queue,threading
+import queue,threading, time
 
 class ClassifierThread(threading.Thread):
     features = []
     targets = []
     mode = "train"
     guess = None
     epochCounts = {} 
     def __init__(self, closeEvent,trainTestEvent, featureQueueTest,featureQueueTrain, classifierInfoQueue, classifierInfoRetrieveEvent, 
-                 classifierGuessMarkerQueue, classifierGuessMarkerEvent, numStreamDevices = 1,
-                 minRequiredEpochs = 10, clf = None, model = None):
+                 classifierGuessMarkerQueue, classifierGuessMarkerEvent, printDebug = True, numStreamDevices = 1,
+                 minRequiredEpochs = 10, clf = None, model = None, torchModel = None):
         super().__init__()
         self.trainTestEvent = trainTestEvent # responsible for tolling between train and test mode
         self.closeEvent = closeEvent # responsible for cosing threads
         self.featureQueueTest = featureQueueTest # gets feature data from feature processing thread
         self.featureQueueTrain = featureQueueTrain # gets feature data from feature processing thread
-        self.classifier = Classifier(clf = clf, model = model) # sets classifier class, if clf and model passed, defaults to clf and sklearn
+        self.classifier = Classifier(clf = clf, model = model, torchModel = torchModel) # sets classifier class, if clf and model passed, defaults to clf and sklearn
         self.minRequiredEpochs = minRequiredEpochs # the minimum number of epochs required for classifier attempt
         self.classifierInfoRetrieveEvent = classifierInfoRetrieveEvent
         self.classifierInfoQueue = classifierInfoQueue
         self.classifierGuessMarkerQueue = classifierGuessMarkerQueue
         self.classifierGuessMarkerEvent = classifierGuessMarkerEvent
         self.numStreamDevices = numStreamDevices
+        self.printDebug = printDebug
 
     def run(self):
         if self.numStreamDevices > 1:
             tempdatatrain = {}
             tempdatatest = {}
         while not self.closeEvent.is_set():
             if self.trainTestEvent.is_set(): # We're training!
@@ -47,27 +48,35 @@
                         # need to check if all device data is captured, then flatten and append
                             if len(self.epochCounts) > 1: # check if there is more then one test condition
                                 minNumKeyEpochs = min([self.epochCounts[key][1] for key in self.epochCounts]) # check minimum viable number of training eochs have been obtained
                                 #print("minNumKeyEpochs"+str(minNumKeyEpochs))
                                 if minNumKeyEpochs < self.minRequiredEpochs:
                                     pass
                                 else: 
+                                    start = time.time()
                                     self.classifier.TrainModel(self.features, self.targets)
+                                    if (self.printDebug):
+                                        end = time.time()
+                                        print(f"PyBCI: Info - classifier training time {end - start}")
                             if self.classifierGuessMarkerEvent.is_set():
                                 self.classifierGuessMarkerQueue.put(None)
                     else:
                         self.targets.append(target)
                         self.features.append(featuresSingle)
                         if len(self.epochCounts) > 1: # check if there is more then one test condition
                             minNumKeyEpochs = min([self.epochCounts[key][1] for key in self.epochCounts]) # check minimum viable number of training eochs have been obtained
                             #print("minNumKeyEpochs"+str(minNumKeyEpochs))
                             if minNumKeyEpochs < self.minRequiredEpochs:
                                 pass
                             else: 
+                                start = time.time()
                                 self.classifier.TrainModel(self.features, self.targets)
+                                if (self.printDebug):
+                                    end = time.time()
+                                    print(f"PyBCI: Info - classifier training time {end - start}")
                         if self.classifierGuessMarkerEvent.is_set():
                             self.classifierGuessMarkerQueue.put(None)
                 except queue.Empty:
                     pass
             else: # We're testing!
                 try:
                     featuresSingle, devCount = self.featureQueueTest.get_nowait() #[dataFIFOs, self.currentMarker, self.sr, self.dataType]
@@ -75,18 +84,25 @@
                         tempdatatest[devCount] = featuresSingle
                         if len(tempdatatest) == self.numStreamDevices:
                             flattened_list = []
                             for value in tempdatatest.values():
                                 flattened_list.extend(value)
                             tempdatatest = {}
                             #self.features.append(flattened_list)
-
+                            start = time.time()
                             self.guess = self.classifier.TestModel(flattened_list)
+                            if (self.printDebug):
+                                end = time.time()
+                                print(f"PyBCI: Info - classifier testing time {end - start}")
                     else:
+                        start = time.time()
                         self.guess = self.classifier.TestModel(featuresSingle)
+                        if (self.printDebug):
+                            end = time.time()
+                            print(f"PyBCI: Info - classifier testing time {end - start}")
                     if self.classifierGuessMarkerEvent.is_set():
                         self.classifierGuessMarkerQueue.put(self.guess)
                 except queue.Empty:
                     pass
             if self.classifierInfoRetrieveEvent.is_set():
                 classdata = {
                     "clf":self.classifier.clf,
```

### Comparing `install-pybci-0.2.0b0/pybci/ThreadClasses/DataReceiverThread.py` & `install-pybci-0.2.1b0/pybci/ThreadClasses/DataReceiverThread.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import threading
+import time
 from collections import deque
 import itertools
 
 class DataReceiverThread(threading.Thread):
     """Responsible for receiving data from accepted LSL outlet, slices samples based on tmin+tmax basis, 
     starts counter for received samples after marker is received in ReceiveMarker.
     """
@@ -37,18 +38,18 @@
             sample, timestamp = self.dataStreamInlet.pull_sample(timeout = 1)
             if sample != None:
                 for index in sorted(self.streamChsDropDict, reverse=True):
                     del sample[index] # remove the desired channels from the sample
                 for i,fifo in enumerate(dataFIFOs):
                     fifo.append(sample[i])
                 if self.trainTestEvent.is_set(): # We're training!
-                    
                     if self.startCounting: # we received a marker
                         posCount+=1
                         if posCount >= self.desiredCount:  # enough samples are in FIFO, chop up and put in dataqueue
+                            #start = time.time()
                             if len(self.customEpochSettings.keys())>0: #  custom marker received
                                 if self.customEpochSettings[self.currentMarker].splitCheck: # slice epochs in to overlapping time windows
                                     window_samples =int(self.customEpochSettings[self.currentMarker].windowLength * self.sr) #number of samples in each window
                                     increment = int((1-self.customEpochSettings[self.currentMarker].windowOverlap)*window_samples) # if windows overlap each other by how many samples
                                     while posCount - window_samples > 0:
                                         sliceDataFIFOs = [list(itertools.islice(d, posCount - window_samples, posCount)) for d in dataFIFOs]
                                         self.dataQueueTrain.put([sliceDataFIFOs, self.currentMarker, self.sr,  self.devCount])
@@ -64,14 +65,16 @@
                                     while startCount - window_samples > 0:
                                         sliceDataFIFOs = [list(itertools.islice(d, startCount - window_samples, startCount)) for d in dataFIFOs]
                                         self.dataQueueTrain.put([sliceDataFIFOs, self.currentMarker, self.sr, self.devCount])
                                         startCount-=increment
                                 else: # don't slice just take tmin to tmax time
                                     sliceDataFIFOs = [list(itertools.islice(d, fifoLength - int((self.globalEpochSettings.tmin+self.globalEpochSettings.tmax) * self.sr), fifoLength)) for d in dataFIFOs]
                                     self.dataQueueTrain.put([sliceDataFIFOs, self.currentMarker, self.sr, self.devCount])
+                            #end = time.time()
+                            #print(f"Data slicing process time {end - start}")
                             # reset flags and counters
                             posCount = 0
                             self.startCounting = False
                 else: # in Test mode
                     posCount+=1
                     if self.globalEpochSettings.splitCheck:
                         window_samples = int(self.globalEpochSettings.windowLength * self.sr) #number of samples in each window
@@ -79,15 +82,14 @@
                         window_samples = int((self.globalEpochSettings.tmin+self.globalEpochSettings.tmax) * self.sr)
                     if posCount >= window_samples:
                         sliceDataFIFOs = [list(itertools.islice(d, fifoLength-window_samples, fifoLength)) for d in dataFIFOs]
                         if self.globalEpochSettings.splitCheck:
                             posCount = int((1-self.globalEpochSettings.windowOverlap)*window_samples) # offset poscoutn based on window overlap 
                         else:
                             posCount = 0
-                            
                         self.dataQueueTest.put([sliceDataFIFOs, self.sr, self.devCount])
             else:
                 pass
                 # add levels of debug 
                 # print("PyBCI: LSL pull_sample timed out, no data on stream...")
 
     def ReceiveMarker(self, marker, timestamp): # timestamp will be used for non sample rate specific devices (pupil-labs gazedata)
```

### Comparing `install-pybci-0.2.0b0/pybci/ThreadClasses/MarkerThread.py` & `install-pybci-0.2.1b0/pybci/ThreadClasses/MarkerThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.0b0/pybci/Utils/Classifier.py` & `install-pybci-0.2.1b0/pybci/Utils/Classifier.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,87 @@
 import sklearn
+from sklearn.preprocessing import StandardScaler
+from sklearn import svm
 import tensorflow
+import torch
+
 from sklearn.model_selection import train_test_split
 import numpy as np
-from sklearn import svm
 
 class Classifier():
     classifierLibrary = "sklearn" # current default, should be none or somthing different?
     clf = svm.SVC(kernel = "rbf")#C=c, kernel=k, degree=d, gamma=g, coef0=c0, tol=t, max_iter=i)
     accuracy = 0
     model = None
+    torchModel = None
 
-    def __init__(self, clf = None, model = None):
+    def __init__(self, clf = None, model = None, torchModel = None):
         super().__init__()
         if clf != None:
             self.clf = clf
         elif model != None:
             self.model = model
+        elif torchModel != None:
+            self.torchModel = model
         self.CheckClassifierLibrary()
 
     def CheckClassifierLibrary(self):
         if self.model != None: # maybe requires actual check for tensorflow model
             self.classifierLibrary = "tensor"
+        elif self.torchModel != None: # maybe requires actual check for sklearn clf
+            self.classifierLibrary = "pyTorch"
         elif self.clf != None: # maybe requires actual check for sklearn clf
             self.classifierLibrary = "sklearn"
 
+
     def TrainModel(self, features, targets):
-        # check for nans and infs in feature creation, not here
-        #if (len(np.array(features).shape) == 3):
-        #    features  = np.array(features).reshape(np.array(features).shape[0], -1)
-        #else:
-        #    features = np.array(features)
-        #features = np.where(np.isnan(features), 0, features)
-        #self.targets = targets
-        #print(features.shape)
         x_train, x_test, y_train, y_test = train_test_split(features, targets, shuffle = True, test_size=0.2)
-        #print("training model")
-        if self.classifierLibrary == "sklearn":
-            if all(item == y_train[0] for item in y_train):
-                pass
-            else:
+        self.scaler = StandardScaler() # normalise our data (everything is a 0 or a 1 if you think about it, cheers georgey boy boole)
+        self.scaler.fit(x_train)  # Compute the mean and standard deviation based on the training data
+        x_train = self.scaler.transform(x_train)  # Scale the training data
+        x_test = self.scaler.transform(x_test)  # Scale the test data
+        if all(item == y_train[0] for item in y_train):
+            pass
+        else:
+            #print(x_train, y_train)
+            if self.classifierLibrary == "pytorch":
+                self.accuracy, self.pymodel  = self.torchModel(x_train, x_test, y_train, y_test)
+            elif self.classifierLibrary == "sklearn":
                 self.clf.fit(x_train, y_train)
                 y_predictions = self.clf.predict(x_test)
-                #print(y_predictions)
                 self.accuracy = sklearn.metrics.accuracy_score(y_test, y_predictions)
-                #print("Classification accuracy (sklearn):" +str(self.accuracy))
-        elif self.classifierLibrary == "tensor":
-            if all(item == y_train[0] for item in y_train):
-                pass
-            else:
-                #print(np.array(x_train).shape)
-                #print(y_train)
-
-                self.model.fit(x_train, y_train) # epochs and batch_size should be customisable
+            elif self.classifierLibrary == "tensor":
+                self.model.fit(np.array(x_train), np.array(y_train)) # epochs and batch_size should be customisable
                 self.loss, self.accuracy = self.model.evaluate(np.array(x_test), np.array(y_test))
-                #print("Classification accuracy (tf):" +str(self.accuracy))
-        else:
-            # no classifier library selected, print debug?
-            pass
+            else:
+                # no classifier library selected, print debug?
+                pass
 
     def TestModel(self, x):
-        # needs check for nans and infs
-        #print(x)
-        #print(np.array(x).shape)
-        #if (len(np.array(x).shape) == 2):
-        #    #x = np.array(x).reshape(np.array(x).shape[0], -1)
-        #    x = np.array([x.flatten()])
-        #else:
-        #    x = np.array(x)
-        #print(x)
-        #print(x.shape)
+        x = self.scaler.transform([x])[0]  # Scale the test data
         if self.classifierLibrary == "sklearn":
             x = np.expand_dims(x, axis=0)
-            #print(x.shape)
             return self.clf.predict(x)
-            #print("we predict it's: "+str(self.y_pred))
         elif self.classifierLibrary == "tensor":
-            # Predict the class labels for the test data
-            #print(x)
             x = np.expand_dims(x, axis=0)
-            #print(x.shape)
             predictions = self.model.predict(x)
             if len (predictions[0]) == 1: # assume binary classification
                 return 1 if predictions[0] > 0.5 else 0
             else:    # assume multi-classification
                 return np.argmax(predictions[0])
-            #print("we predict it's: "+str(y_pred))
-            # Convert the predicted probabilities to class labels
-            #y_pred_classes = np.argmax(self.y_pred, axis=1)
-            #print("if class label: "+str(y_pred_classes))
+        elif self.classifierLibrary == "pyTorch":
+            x = torch.Tensor(np.expand_dims(x, axis=0))
+            self.pymodel.eval()
+            with torch.no_grad():
+                predictions = self.pymodel(x)
+                if len (predictions[0]) == 1: # assume binary classification
+                    return 1 if predictions[0] > 0.5 else 0
+                else:    # assume multi-classification
+                    return torch.argmax(predictions).item()
+
         else:
             print("no classifier library selected")
             # no classifier library selected, print debug?
             pass
 
 '''
     def UpdateModel(self, featuresSingle, target):
```

### Comparing `install-pybci-0.2.0b0/pybci/Utils/FeatureExtractor.py` & `install-pybci-0.2.1b0/pybci/Utils/FeatureExtractor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import antropy as ant
 import numpy as np
 from scipy.signal import welch
 from scipy.integrate import simps
 import warnings
 from ..Configuration.FeatureSettings import GeneralFeatureChoices
-# Filter out UserWarning messages from the scipy package, could be worth moving to init and applying printdebug print levels?
+# Filter out UserWarning messages from the scipy package, could be worth moving to init and applying printdebug print levels? (typically nans, 0 and infs causing errors)
 warnings.filterwarnings("ignore", category=UserWarning, module="scipy") # used to reduce print statements from constant signals being applied
 warnings.filterwarnings("ignore", category=UserWarning, module="antropy") # used to reduce print statements from constant signals being applied
 warnings.filterwarnings("ignore", category=RuntimeWarning, module="antropy") # used to reduce print statements from constant signals being applied
+warnings.filterwarnings("ignore", category=RuntimeWarning, module="numpy") # used to reduce print statements from constant signals being applied
 #warnings.filterwarnings("ignore", category=RuntimeWarning, module="pybci") # used to reduce print statements from constant signals being applied
 
 class GenericFeatureExtractor():
 
     def __init__(self, freqbands = [[1.0, 4.0], [4.0, 8.0], [8.0, 12.0], [12.0, 20.0]], featureChoices = GeneralFeatureChoices()):
         super().__init__()
         self.freqbands = freqbands
@@ -24,17 +25,17 @@
             self.featureChoices.svd_entropy,
             self.featureChoices.samp_entropy,
             self.featureChoices.rms,
             self.featureChoices.meanPSD,
             self.featureChoices.medianPSD,
             self.featureChoices.variance,
             self.featureChoices.meanAbs,
-            self.featureChoices.waveformLength,
-            self.featureChoices.zeroCross,
-            self.featureChoices.slopeSignChange]
+            #self.featureChoices.waveformLength,
+            self.featureChoices.zeroCross]
+            #self.featureChoices.slopeSignChange]
         )
         self.numFeatures = (len(self.freqbands)*self.featureChoices.psdBand)+selFeats
 
     def ProcessFeatures(self, epoch, sr, target):
         """Allows 2D time series data to be passed with given sample rate to get various time+frequency based features.
         Best for EEG, EMG, EOG, or other consistent data with a consistent sample rate (pupil labs does not)
         Which features are chosen is based on self.featureChoices with initialisation. self.freqbands sets the limits for
@@ -48,14 +49,15 @@
             target = same as input target
         NOTE: Any channels with a constant value will generate warnings in any frequency based features (constant level == no frequency components).
         """
         #print(np.array(epoch).shape)
         numchs = len(epoch)
         features = np.zeros(numchs * self.numFeatures)
         for k, ch in enumerate(epoch):
+            #ch = np.isnan(ch)
             if self.featureChoices.psdBand: # get custom average power within given frequency band from freqbands
                 freqs, psd = welch(ch, sr)
                 for l, band in enumerate(self.freqbands):
                     if len(freqs) > 0: # len(freqs) can be 0 if signal is all DC
                         idx_band = np.logical_and(freqs >= band[0], freqs <= band[1])
                         #if len(psd[idx_band]) == 1: # if freq band is only in one field just pass single value instead of calculating average
                         #print(ch)
@@ -97,26 +99,27 @@
                 features[(k* self.numFeatures)+l] = np.sqrt(np.mean(np.array(ch)**2))
             if self.featureChoices.variance: # variance
                 l += 1    
                 features[(k* self.numFeatures)+l] =  np.var(ch)
             if self.featureChoices.meanAbs: # Mean Absolute Value 
                 l += 1
                 features[(k* self.numFeatures)+l] = sum([np.linalg.norm(c) for c in ch])/len(ch)
-            if self.featureChoices.waveformLength: # waveformLength
-                l += 1
-                features[(k* self.numFeatures)+l] = sum([np.linalg.norm(c-ch[inum]) for inum, c in enumerate(ch[1:])])
+            #if self.featureChoices.waveformLength: # waveformLength
+            #    l += 1
+            #    features[(k* self.numFeatures)+l] = sum([np.linalg.norm(c-ch[inum]) for inum, c in enumerate(ch[1:])])
             if self.featureChoices.zeroCross: # zeroCross
                 l += 1
                 features[(k* self.numFeatures)+l] = sum([1 if c*ch[inum+1]<0 else 0 for inum, c in enumerate(ch[:-1])])
-            if self.featureChoices.slopeSignChange: # slopeSignChange
-                l += 1    
-                ssc = sum([1 if (c-ch[inum+1])*(c-ch[inum+1])>=0.1 else 0 for inum, c in enumerate(ch[:-1])])
-                features[(k* self.numFeatures)+l] = ssc
-        features[np.isnan(features)] = 0 # checks for nans
-        features[features == np.inf] = 0 # checks for infs
+            #if self.featureChoices.slopeSignChange: # slopeSignChange
+            #    l += 1    
+            #    ssc = sum([1 if (c-ch[inum+1])*(c-ch[inum+1])>=0.1 else 0 for inum, c in enumerate(ch[:-1])])
+            #    features[(k* self.numFeatures)+l] = ssc
+        #features[np.isnan(features)] = 0 # checks for nans
+        #features[features == np.inf] = 0 # checks for infs
+        #print(features)
         return features
     
 class GazeFeatureExtractor():
     def __init__(self):
         super().__init__()
 
 '''pupil channels in order
```

### Comparing `install-pybci-0.2.0b0/pybci/Utils/LSLScanner.py` & `install-pybci-0.2.1b0/pybci/Utils/LSLScanner.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.2.0b0/pybci/pybci.py` & `install-pybci-0.2.1b0/pybci/pybci.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from .ThreadClasses.AsyncDataReceiverThread import AsyncDataReceiverThread
 from .ThreadClasses.MarkerThread import MarkerThread
 from .ThreadClasses.ClassifierThread import ClassifierThread
 from .Configuration.EpochSettings import GlobalEpochSettings, IndividualEpochSetting
 from .Configuration.FeatureSettings import GeneralFeatureChoices
 import queue, threading, copy
 import tensorflow as tf
+import torch
+import torch.nn as nn
 tf.get_logger().setLevel('ERROR')
 
 class PyBCI:
     printDebug = True   # boolean, used to toggle print statements from LSLScanner class
     globalEpochSettings = GlobalEpochSettings()
     customEpochSettings = {}
     minimumEpochsRequired = 10
@@ -23,15 +25,15 @@
     connected = False
     epochCounts = {} # holds markers received, their target ids and number received of each
     classifierInformation = []
 
     def __init__(self, dataStreams = None, markerStream= None, streamTypes = None, markerTypes = None, printDebug = True,
                  globalEpochSettings = GlobalEpochSettings(), customEpochSettings = {}, streamChsDropDict = {},
                  streamCustomFeatureExtract = {},
-                 minimumEpochsRequired = 10, clf= None, model = None):
+                 minimumEpochsRequired = 10, clf= None, model = None, torchModel = None):
         """
         The PyBCI object stores data from available lsl time series data streams (EEG, pupilometry, EMG, etc.)
         and holds a configurable number of samples based on lsl marker strings.
         If no marker strings are available on the LSL the class will close and return an error.
         Parameters:
         dataStreams (List of strings): Allows user to set custom acceptable EEG stream definitions, if None defaults to streamTypes scan
         markerStream (List of strings): Allows user to set custom acceptable Marker stream definitions, if None defaults to markerTypes scan
@@ -49,15 +51,15 @@
         self.streamCustomFeatureExtract = streamCustomFeatureExtract
         self.globalEpochSettings = globalEpochSettings
         self.customEpochSettings = customEpochSettings
         self.streamChsDropDict = streamChsDropDict
         self.lslScanner = LSLScanner(self, dataStreams, markerStream,streamTypes, markerTypes)
         self.printDebug = printDebug
         #if self.printDebug == False:
-        self.ConfigureMachineLearning(minimumEpochsRequired,  clf, model) # configure first, connect second
+        self.ConfigureMachineLearning(minimumEpochsRequired,  clf, model, torchModel) # configure first, connect second
         self.Connect()
        
     def __enter__(self, dataStreams = None, markerStream= None, streamTypes = None, markerTypes = None, printDebug = True,
                  globalEpochSettings = GlobalEpochSettings(), customEpochSettings = {}, streamChsDropDict = {},
                  freqbands = [[1.0, 4.0], [4.0, 8.0], [8.0, 12.0], [12.0, 20.0]], featureChoices = GeneralFeatureChoices()): # with bci
         self.freqbands = freqbands
         self.featureChoices = featureChoices
@@ -180,16 +182,16 @@
             self.ft.start()
             self.featureThreads.append(dt)
         # marker thread requires data and feature threads to push new markers too
         self.markerThread = MarkerThread(self.closeEvent,self.trainTestEvent, self.markerStream,self.dataThreads, self.featureThreads)
         self.markerThread.start()
         self.classifierThread = ClassifierThread(self.closeEvent,self.trainTestEvent, self.featureQueueTest,self.featureQueueTrain,
                                                  self.classifierInfoQueue, self.classifierInfoRetrieveEvent,
-                                                 self.classifierGuessMarkerQueue, self.classifierGuessMarkerEvent, len(self.dataThreads),
-                                                self.minimumEpochsRequired, clf = self.clf, model = self.model)
+                                                 self.classifierGuessMarkerQueue, self.classifierGuessMarkerEvent, self.printDebug,len(self.dataThreads),
+                                                self.minimumEpochsRequired, clf = self.clf, model = self.model, torchModel = self.torchModel)
         self.classifierThread.start()
 
     def StopThreads(self):
         self.closeEvent.set()
         self.markerThread.join()
         # wait for all threads to finish processing, probably worth pulling out finalised classifier information stored for later use.
         for dt in self.dataThreads:
@@ -197,29 +199,36 @@
         for ft in self.featureThreads:
             ft.join()
         self.classifierThread.join()
         self.connected = False
         if self.printDebug:
             print("PyBCI: Threads stopped.")
 
-    def ConfigureMachineLearning(self, minimumEpochsRequired = 10, clf = None, model = None):
+    def ConfigureMachineLearning(self, minimumEpochsRequired = 10, clf = None, model = None, torchModel = None):
         from sklearn.base import ClassifierMixin
         self.minimumEpochsRequired = minimumEpochsRequired
         if isinstance(clf, ClassifierMixin):
             self.clf = clf
         else:
             self.clf = None
             if self.printDebug:
                 print("PyBCI: Error - Invalid sklearn classifier passed to clf, setting to SVM if no tensorflow model passed either.")
         if isinstance(model, tf.keras.Model):
             self.model = model
         else:
             self.model = None
             if self.printDebug:
                 print("PyBCI: Error - Invalid tensorflow model passed to model, setting to None.")
+        if callable(torchModel): # isinstance(torchModel, torch.nn.Module):
+            self.torchModel = model
+        else:
+            self.torchModel = None
+            if self.printDebug:
+                print("PyBCI: Error - Invalid PyTorch model passed to model, setting to None.")
+    
 
     # Could move all configures to a configuration class, might make options into more descriptive classes?
     def ConfigureEpochWindowSettings(self, globalEpochSettings = GlobalEpochSettings(), customEpochSettings = {}):
         """allows globalWindowSettings to be modified, customWindowSettings is a dict with value names for marker strings which will appear on avalable markerStreams """
         valid = False
         for key in customEpochSettings.keys():
             if isinstance(customEpochSettings[key], IndividualEpochSetting):
```

### Comparing `install-pybci-0.2.0b0/setup.py` & `install-pybci-0.2.1b0/setup.py`

 * *Files identical despite different names*

