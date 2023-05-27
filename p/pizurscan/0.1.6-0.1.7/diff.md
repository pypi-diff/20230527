# Comparing `tmp/pizurscan-0.1.6.tar.gz` & `tmp/pizurscan-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pizurscan-0.1.6.tar", last modified: Fri May  5 08:06:54 2023, max compression
+gzip compressed data, was "pizurscan-0.1.7.tar", last modified: Sat May 27 15:20:31 2023, max compression
```

## Comparing `pizurscan-0.1.6.tar` & `pizurscan-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:06:54.553270 pizurscan-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-05-05 08:06:54.553270 pizurscan-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-05 08:06:46.000000 pizurscan-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:06:54.549270 pizurscan-0.1.6/pizurscan/
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-05-05 08:06:46.000000 pizurscan-0.1.6/pizurscan/InputProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-05-05 08:06:46.000000 pizurscan-0.1.6/pizurscan/InputValidator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-05 08:06:46.000000 pizurscan-0.1.6/pizurscan/OutputProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-05 08:06:46.000000 pizurscan-0.1.6/pizurscan/PI_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-05 08:06:46.000000 pizurscan-0.1.6/pizurscan/Scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:06:46.000000 pizurscan-0.1.6/pizurscan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:06:54.549270 pizurscan-0.1.6/pizurscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-05-05 08:06:54.000000 pizurscan-0.1.6/pizurscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-05 08:06:54.000000 pizurscan-0.1.6/pizurscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:06:54.000000 pizurscan-0.1.6/pizurscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 08:06:54.000000 pizurscan-0.1.6/pizurscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 08:06:54.000000 pizurscan-0.1.6/pizurscan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 08:06:54.553270 pizurscan-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-05 08:06:46.000000 pizurscan-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:06:54.553270 pizurscan-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    25984 2023-05-05 08:06:46.000000 pizurscan-0.1.6/tests/testclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 15:20:31.953004 pizurscan-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-05-27 15:20:31.953004 pizurscan-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-27 15:20:23.000000 pizurscan-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 15:20:31.953004 pizurscan-0.1.7/pizurscan/
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-27 15:20:23.000000 pizurscan-0.1.7/pizurscan/InputProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-27 15:20:23.000000 pizurscan-0.1.7/pizurscan/InputValidator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-27 15:20:23.000000 pizurscan-0.1.7/pizurscan/OutputProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-27 15:20:23.000000 pizurscan-0.1.7/pizurscan/PI_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-05-27 15:20:23.000000 pizurscan-0.1.7/pizurscan/Scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 15:20:23.000000 pizurscan-0.1.7/pizurscan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 15:20:31.953004 pizurscan-0.1.7/pizurscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-05-27 15:20:31.000000 pizurscan-0.1.7/pizurscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-27 15:20:31.000000 pizurscan-0.1.7/pizurscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 15:20:31.000000 pizurscan-0.1.7/pizurscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 15:20:31.000000 pizurscan-0.1.7/pizurscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 15:20:31.000000 pizurscan-0.1.7/pizurscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 15:20:31.953004 pizurscan-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-27 15:20:23.000000 pizurscan-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 15:20:31.953004 pizurscan-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    23748 2023-05-27 15:20:23.000000 pizurscan-0.1.7/tests/testclasses.py
```

### Comparing `pizurscan-0.1.6/PKG-INFO` & `pizurscan-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pizurscan
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library to interface PI controllers and Zurich lock-in
 Home-page: https://pizur-scanner.readthedocs.io/
 Author: Giacomo Rizzi
 Author-email: rizzigiacomo@pm.me
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pizurscan-0.1.6/README.md` & `pizurscan-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pizurscan-0.1.6/pizurscan/InputProcessor.py` & `pizurscan-0.1.7/pizurscan/InputProcessor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,156 +1,158 @@
 import numpy as np
 
-class InputProcessor():
-    """A class to process input scan parameters and provide the correct parameters to set
-    in the Zurich Lock-In API data acquisition."""
+def rows_columns_contiuous(delta, stepsize):
+    """
+    Calculate the number of rows and columns for a continuous scan with a PI controller and Zurich lock-in.
+
+    Parameters:
+    -----------
+    delta : float
+        The distance between the scan edges.
+    stepsize : float
+        The step size for the motion of the stepper.
+
+    Returns:
+    --------
+    N_rows : int
+        The number of rows for the data acquisition.
+    N_cols : int
+        The number of columns for the data acquisition.
+    """
+    N_rows = 1
+    N_cols = int(np.floor(delta / stepsize)) + 1
+    return N_rows, N_cols
+
+def rows_columns_discrete(delta, stepsize, sampl_freq):
+    """
+    Calculate the number of rows and columns for a discrete scan with a PI controller and Zurich lock-in.
     
-    def __init__(self,scan_pars):
-        """
-        Initialize an InputProcessor instance.
-
-        Parameters:
-        -----------
-        scan_pars : dict
-            A dictionary containing scan parameters, including:
-                - scan_edges : list of two floats
-                    The edges of the scan range.
-                - stepsize : float
-                    The step size for the scan.
-                - acceleration : float
-                    The acceleration of moving stage scans.
-                - velocity : float
-                    The velocity of the moving stage scans.
-                - sampling_frequency : float
-                    The sampling frequency used for discrete scans.
-                - type : str
-                    The type of scan, either 'continuous' or 'discrete'.
-        delta : float
-            a float containing the absolute value of the distance between the scan edges.
-        """
-        self.scan_edges = scan_pars["scan_edges"]
-        self.stepsize = scan_pars["stepsize"]
-        self.acc = scan_pars["acceleration"]
-        self.vel = scan_pars["velocity"]
-        self.sampl_freq = scan_pars["sampling_freq"]
-        self.type = scan_pars["type"]
-        self.delta = self.delta_calculator()
-
-    
-    def rows_columns_contiuous(self):
-            """
-            Process input data to find the number of rows and columns
-            for a continuous scan with PI controller and Zurich lock-in.
-
-            Returns:
-            --------
-            N_cols : int
+    Parameters:
+    -----------
+    delta : float
+        The distance between the scan edges.
+    stepsize : float
+        The step size for the motion of the stepper.
+    sampl_freq : float
+        The sampling frequency of the Zurich lock-in.
+
+    Returns:
+    --------
+    N_rows : int
+        The number of rows for the data acquisition.
+    N_cols : int
+        The number of columns for the data acquisition.
+    """
+    N_rows = int(np.floor(delta / stepsize)) + 1
+    N_cols = int(np.floor(0.05 * sampl_freq))
+    return N_rows, N_cols
+
+def evaluate_daq_pars(scan_pars):
+    """
+    Process input data for a 1D scan to return the complete DAQ parameters that suit the scan parameters.
+
+    Parameters:
+    -----------
+    scan_pars : dict
+        A dictionary containing scan parameters, including:
+            - stepsize : float
+                The step size for motin of the stepper
+            - acceleration : float
+                The acceleration of the stepper.
+            - velocity : float
+                The velocity of the stepper.
+            - sampling_freq : float
+                The sampling frequency of the Zurich lock-in
+            - type : str
+                The type of scan: 'continuous' or 'discrete'.
+            - scan_edges : list[float]
+                The edges of the scan range.
+
+    Returns:
+    --------
+    daq_pars : dict
+        A dictionary containing data acquisition parameters, including:
+            - daq_columns : int
                 The number of columns for the data acquisition.
-            N_rows : int
+            - daq_rows : int
                 The number of rows for the data acquisition.
-            """
-            N_rows = 1
-            N_cols = int(np.floor(self.delta/self.stepsize)) + 1
-            return N_rows, N_cols
-    
-    def rows_columns_discrete(self):
-        """
-        Process input data to find the number of rows and columns
-        for a discrete scan with Pi controller and Zurich lock-in
-
-        Returns:
-        --------
-        N_cols : int
-            The number of columns for the data acquisition.
-        N_rows : int
-            The number of rows for the data acquisition.
-        """
-        N_rows = int(np.floor(self.delta/self.stepsize)) + 1
-        N_cols = int(np.floor(0.05*self.sampl_freq))
-        return N_rows, N_cols
-
-    def evaluate_daq_pars(self):
-        """
-        Process input data for a 1D scan to return the complete DAQ parameters
-        that suit the scan parameters.
-
-        Returns:
-        --------
-        daq_pars : dict
-            A dictionary containing data acquisition parameters, including:
-                - daq_columns : int
-                    The number of columns for the data acquisition.
-                - daq_rows : int
-                    The number of rows for the data acquisition.
-                - duration : float
-                    The duration of the triggered data acquisition.
-                - mode : str
-                    The data acquisition mode; 'Exact (on-grid)' for discrete scan, 'Linear' for continuous
-                - trigger type : str
-                    The trigger type, always set to 'HW trigger'.
-                - trigger edge : str
-                    The trigger edge; 
-                - holdoff : float
-                    The holdoff time for the trigger
-        """
-
-        if self.type == "continuous":
-            duration = self.duration_calculator()
-            N_rows, N_cols = self.rows_columns_contiuous()
-            mode = "linear"
-            edge = "positive"
-        else:
-            duration = 0.05 # 50 milliseconds
-            N_rows, N_cols = self.rows_columns_discrete()
-            mode = "Exact (on-grid)"
-            edge = "negative"
-            
-        daq_pars =  {
-                    "daq_columns" : N_cols,
-                    "daq_rows" : N_rows,
-                    "duration" : duration,
-                    "mode" : mode,
-                    "trigger type" : "HW trigger",
-                    "trigger edge" : edge,
-                    "holdoff" : duration*(0.95),
-                    }
-        return daq_pars
-
-    def delta_calculator(self):
-        """
-        Calculate the absolute value of the distance between the scan edges.
-
-        Returns:
-        --------
-        delta : float
-            Absolute value of the distance between scan edges.
-        """
-        return abs(self.scan_edges[1]-self.scan_edges[0])
-
-    def duration_calculator(self):
-        """
-        Calculate the duration of the triggered data acquisition for a continuous scan.
-
-        Parameters:
-        -----------
-        acc : float
-            The acceleration of the moving stage scans.
-        delta : float
-            The distance between the scan edges.
-        vel : float
-            The velocity of the moving stage scans.
-
-        Returns:
-        --------
-        duration : float
-            The duration of the triggered data acquisition.
-        """
-        if (np.sqrt(self.acc*self.delta)>self.vel):
-            duration = self.vel/self.acc + self.delta/self.vel
-        else:
-            duration = 2*np.sqrt(self.delta/self.acc)
-        return duration
-
-            
-        
-
-    
+            - duration : float
+                The duration of the triggered data acquisition.
+            - mode : str
+                The data acquisition mode; 'Linear' for continuous scan, 'Exact (on-grid)' for discrete scan.
+            - trigger_type : str
+                The trigger type, always set to 'HW trigger'.
+            - trigger_edge : str
+                The trigger edge.
+            - holdoff : float
+                The holdoff time for the trigger.
+    """
+    stepsize = scan_pars["stepsize"]
+    acc = scan_pars["acceleration"]
+    vel = scan_pars["velocity"]
+    sampl_freq = scan_pars["sampling_freq"]
+    scan_type = scan_pars["type"]
+    scan_edges = scan_pars["scan_edges"]
+
+    delta = delta_calculator(scan_edges)
+
+    if scan_type == "continuous":
+        duration = duration_calculator(delta, vel, acc)
+        N_rows, N_cols = rows_columns_contiuous(delta, stepsize)
+        mode = "Linear"
+        edge = "positive"
+    else:
+        duration = 0.05  # 50 milliseconds
+        N_rows, N_cols = rows_columns_discrete(delta, stepsize, sampl_freq)
+        mode = "Exact (on-grid)"
+        edge = "negative"
+
+    daq_pars = {
+        "daq_columns": N_cols,
+        "daq_rows": N_rows,
+        "duration": duration,
+        "mode": mode,
+        "trigger_type": "HW trigger",
+        "trigger_edge": edge,
+        "holdoff": duration * 0.95,
+    }
+    return daq_pars
+
+def delta_calculator(scan_edges):
+    """
+    Calculate the absolute value of the distance between the scan edges.
+
+    Parameters:
+    -----------
+    scan_edges : list[float]
+        The edges of the scan range.
+
+    Returns:
+    --------
+    delta : float
+        Absolute value of the distance between scan edges.
+    """
+    return abs(scan_edges[1] - scan_edges[0])
+
+def duration_calculator(delta, vel, acc):
+    """
+    Calculate the duration of the triggered data acquisition for a continuous scan.
+
+    Parameters:
+    -----------
+    delta : float
+        The distance between the scan edges.
+    vel : float
+        The velocity of the stepper.
+    acc : float
+        The acceleration of the stepper.
+
+    Returns:
+    --------
+    duration : float
+        The duration of the triggered data acquisition.
+    """
+    if np.sqrt(acc * delta) > vel:
+        duration = vel / acc + delta / vel
+    else:
+        duration = 2 * np.sqrt(delta / acc)
+    return duration
```

### Comparing `pizurscan-0.1.6/pizurscan/PI_commands.py` & `pizurscan-0.1.7/pizurscan/PI_commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,26 +44,54 @@
         --------
         A list object with the indeces of the connected devices
         """
         return self.pidevice.EnumerateUSB(mask=self.controller_id)
     
     def connect_pidevice(self):
         """
-        Activates an I/O interface to select the device of interest among the plugged ones.
-        Accepts a user input with the index of the device to interest and connects to it.
+        Finds the plugged devices, activates the I/O interface to select the device of interest and 
+        eventually connects to the selected device.        
         """
         devices = self.usb_plugged_devices()
         if not devices:
             raise Exception("There are no plugged devices! Please connect at least one device.")
+
+        selected_device = self.select_device(devices)
+        self.startup_USB_device(selected_device)
+
+    def select_device(self, devices):
+        """
+        Displays the list of devices and prompts the user to select one.
+        
+        Parameters
+        ----------
+        devices : list
+            List object with the connected devices (as strings)
+        
+        Returns:
+        --------
+        A string object with the name of the pi device to be connected.
+        """            
+        print('Number ---- Device')
         for i, device in enumerate(devices):
-            print('Number ---- Device')
             print(f'{i}      ----  {device}')
-        # I/O for device selection
+
         item = int(input('Input the index of the device to connect: '))
-        self.pidevice.ConnectUSB(devices[item])
+        return devices[item]
+
+    def startup_USB_device(self, device):
+        """
+        Connects to the specified device.
+        
+        Parameters
+        ----------
+        device : str
+            A string object with the name of the pi device to be connected.
+        """
+        self.pidevice.ConnectUSB(device)
         pitools.startup(self.pidevice, self.axis_id)
         
     def move_stage_to_ref(self, refmode):
         """
         Moves the selected controller towards the reference position.
         
         Parameters
@@ -145,25 +173,38 @@
         ----------
         target : float
             Float defining the target position
         """
         self.pidevice.MOV(self.pidevice.axes,target)
         pitools.waitontarget(self.pidevice)
 
-    def configure_out_trigger(self, trigger_type):
-        """Configures and sets the output trigger for a given axis.
+    def enable_out_trigger(self, trigger_type):
+        """Configures and activate the output trigger for a given axis.
         
         Parameters
         ----------
         trigger_type : int
             Type of trigger to be output (6 == in Motion, 1 = Line trigger).
         """
         self.pidevice.CTO(1, 2, 1)
         self.pidevice.CTO(1, 3, trigger_type)
         # enable trigger output with the configuration defined above
         self.pidevice.TRO(1, True)
         
+    def disable_out_trigger(self, trigger_type):
+        """Configures and disable the output trigger for a given axis.
+        
+        Parameters
+        ----------
+        trigger_type : int
+            Type of trigger to be output (6 == in Motion, 1 = Line trigger).
+        """
+        self.pidevice.CTO(1, 2, 1)
+        self.pidevice.CTO(1, 3, trigger_type)
+        # disable trigger output with the configuration defined above
+        self.pidevice.TRO(1, False)
+        
     def close_connection(self):
         """
         Close the connection and reset the axis property
         """
         self.pidevice.CloseConnection()
```

### Comparing `pizurscan-0.1.6/pizurscan/Scanner.py` & `pizurscan-0.1.7/pizurscan/Scanner.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,36 +4,38 @@
 class Scanner:
     """
     A class for performing a 1D scan using a PI device.
 
     Attributes:
         PI (dict): Dictionary of PI device information.
         scan_pars (dict): Dictionary of scan parameters.
-        scan_edges (tuple): Tuple of start and end positions of the scan.
+        scan_edges (list): List containing the two edges of the scan. Axis will move from the leftward to the rightward.
         stepsize (float): Step size of the scan.
         targets (numpy.ndarray): Array of target positions for the scan.
         stepper (Stepper): Stepper object for controlling the PI device.
 
     Methods:
         __init__(self, InPars):
-            Initializes Scan1D object with input parameters.
+            Initializes Scanner object with input parameters.
+        __enter__(self):
+            Context manager enter method.
+        __exit__(self, exc_type, exc_value, traceback):
+            Context manager exit method.
+        __connect_stepper(self):
+            Connects to the PI device through a user-interface I/O.
+        __reference_stepper(self):
+            Setup the 1D scan in four steps.
         evaluate_target_positions(self):
             Evaluates the partition of the target points for a 1D scan.
-            Returns:
-                numpy.ndarray: Array of target positions.
-        connect_stepper(self):
-            Connects to the PI device through a user-interface I/O.
         setup_motion_stepper(self):
-            Stores input velocity and acceleration in the ROM of the device.
-        init_stepper_scan(self):
-            Sets up the 1D scan in four steps.
+            Stores input velocity, acceleration, and trigger type in the ROM of the device.
+        init_scan(self):
+            Disables the trigger and moves to the first target of the scan.
         execute_discrete_scan(self):
             Executes the 1D discrete scan by moving the axis on all the target positions.
-            Returns:
-                list: List of current positions.
         execute_continuous_scan(self):
             Executes the continuous scan by moving the axis to the last position.
     """
 
     def __init__(self, InPars):
         """ Initializes Scanner object with input parameters.
         
@@ -60,70 +62,105 @@
         self.PI = InPars["pi"]
         self.scan_pars = InPars["scan_pars"]
         self.scan_edges = self.scan_pars["scan_edges"]
         self.stepsize = self.scan_pars["stepsize"]
         self.targets = self.evaluate_target_positions()
         self.stepper = Stepper(self.PI["ID"], self.PI["stage_ID"])
 
+
+    def __enter__(self):
+        """
+        Context manager enter method.
+        Establishes the connection with the pidevice as soon as a context manager is opened
+        and references the axis to either the positive or the negative edge.
+        
+        Returns:
+        -------
+            Scanner: Scanner object connected to the pidevice and referenced
+        """
+        self.__connect_stepper()  
+        self.__reference_stepper()
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        """
+        Context manager exit method that closes the connection with the pidevice.
+
+        Parameters:
+        ----------
+        - exc_type : type
+            The type of the exception raised, if any. None if no exception occurred.
+        - exc_value : Exception
+            The exception instance raised, if any. None if no exception occurred.
+        - traceback : traceback
+            The traceback object related to the exception, if any. None if no exception occurred.
+        """
+        self.stepper.close_connection()  # Close the connection with the pidevice
+
+
+    def __connect_stepper(self):
+        """
+        Connects to the PI device through a user-interface I/O.
+        """
+        self.stepper.connect_pidevice()
+
+    def __reference_stepper(self):
+        """
+        Moves stepper to the required reference position at the maximum velocity
+        and acceleration. 
+        """
+        # Set high default values to obtain quick referencing
+        max_vel = 10    # mm/s
+        max_acc = 20    # mm/s^2
+        self.stepper.set_velocity(max_vel)
+        self.stepper.set_acceleration(max_acc)
+        self.stepper.move_stage_to_ref(self.PI["refmode"])
+        
     def evaluate_target_positions(self):
         """
         Evaluates the partition of the target points for a 1D scan.
 
         Returns:
         --------
         numpy.ndarray: Array of target positions.
         """
         Npoints = int(abs(self.scan_edges[1] - self.scan_edges[0]) / self.stepsize) + 1
         return np.linspace(self.scan_edges[0], self.scan_edges[1], Npoints, endpoint=True)
 
-    def connect_stepper(self):
-        """
-        Connects to the PI device through a user-interface I/O.
-        """
-        self.stepper.connect_pidevice()
-
     def setup_motion_stepper(self):
         """
-        Stores input velocity and acceleration in the ROM of the device.
+        Stores input velocity, acceleration, and trigger type in the ROM of the device.
         """
+        self.stepper.enable_out_trigger(trigger_type=self.PI["trig_type"])
         self.stepper.set_velocity(self.scan_pars["velocity"])
         self.stepper.set_acceleration(self.scan_pars["acceleration"])
         
-    def init_stepper_scan(self):
-        """Setup the 1D scan in four steps: (1) acceleration and velocity are set to
-        default values for quick refering and motion. (2) Stage is moved to reference,
-        either positive or negative depending on the input refmode. (3) stage is moved 
-        to the first target point output trigger is selected and activated
-        """
-        # high default values to obtain a quick referencing 
-        self.stepper.set_velocity(10)
-        self.stepper.set_acceleration(20)
-        self.stepper.move_stage_to_ref(self.PI["refmode"])
+    def init_scan(self):
+        """
+        Disables the trigger that was previously set and moves to the first target of the scan.
+        """
+        self.stepper.disable_out_trigger(trigger_type=self.PI["trig_type"])
         self.stepper.move_stage_to_target(self.targets[0])
-        trigtype = self.PI["trig_type"]
-        self.stepper.configure_out_trigger(trigger_type=trigtype)
-
+        self.setup_motion_stepper()
+        
     def execute_discrete_scan(self):
         """
-        Execute the 1D discrete scan by moving the axis on all the target positions.
+        Executes the 1D discrete scan by moving the axis to all the target positions.
 
         Returns:
         --------
-        list : List of current positions.
+        scan_pos : List of scanned positions.
         """
-        cur_pos = []
+        self.init_scan()
+        scan_pos = []
         for target in self.targets:
             self.stepper.move_stage_to_target(target)        
-            print("Position: ", target)
-            cur_pos.append(self.stepper.get_curr_pos())
-        self.stepper.close_connection()
-        return cur_pos
+            cur_pos = self.stepper.get_curr_pos()
+            scan_pos.append(cur_pos)
+        return scan_pos
 
-    
     def execute_continuous_scan(self):
         """
-        Execute the continuous scan by moving the axis to the last position.
+        Executes the continuous scan by moving the axis to the last position.
         """
-        self.stepper.move_stage_to_target(self.targets[-1])    
-        self.stepper.close_connection()
-    
-        
+        self.init_scan()
+        self.stepper.move_stage_to_target(self.targets[-1])
```

### Comparing `pizurscan-0.1.6/pizurscan.egg-info/PKG-INFO` & `pizurscan-0.1.7/pizurscan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pizurscan
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library to interface PI controllers and Zurich lock-in
 Home-page: https://pizur-scanner.readthedocs.io/
 Author: Giacomo Rizzi
 Author-email: rizzigiacomo@pm.me
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pizurscan-0.1.6/setup.py` & `pizurscan-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="pizurscan",
-    version="0.1.6",
+    version="0.1.7",
     description="Library to interface PI controllers and Zurich lock-in",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pizur-scanner.readthedocs.io/",
     author="Giacomo Rizzi",
     author_email="rizzigiacomo@pm.me",
     license="MIT",
```

### Comparing `pizurscan-0.1.6/tests/testclasses.py` & `pizurscan-0.1.7/tests/testclasses.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,64 @@
 from pizurscan.PI_commands import Stepper
 from pizurscan.Scanner import Scanner
-from pizurscan.InputProcessor import InputProcessor
+from pizurscan.InputProcessor import *
 from pipython import pitools,GCS2Commands,GCSDevice
-from pizurscan.OutputProcessor import OutputProcessor
-from pizurscan.InputValidator import InputValidator
+from pizurscan.OutputProcessor import *
+from pizurscan.InputValidator import *
 import pytest as pytest
 from math import isclose
 import numpy as np 
 
 class TestStepper:
-    stepper = Stepper('C-663', 'L-406.40SD00')
-    
-    def test_initialization_pidevice(self):
-        """Tests that when a Stepper object is initialiazed through 
-        the __init__ method, the instantiation of the GCSDevice is corrected."""
-        assert isinstance(self.stepper.pidevice, GCSDevice)
+    def setup_method(self, method):
+        """Setup any state tied to the execution of the given method in a class.
+        `setup_method` is invoked for every test method of a class.
+        in the Setup, an instance of the stepper class is created and a PI_device is connected
+        """
+        self.stepper = Stepper('C-663', 'L-406.40SD00')
+        self.stepper.connect_pidevice()
     
+    def teardown_method(self, method):
+        """teardown any state that was previously setup with a setup_method
+        call. In particular, it calls close_connection.
+        """
+        self.stepper.close_connection()
+        self.stepper = None
+        
     def test_initialization_controller_axis(self):
         """Tests that when a Stepper object is initialized through
         the __init__ method, the attributes controller_id and axis_id are
         properly assigned."""
         controller = 'C-663'
         axis = 'L-406.40SD00'
         # make id of controller and axis attributes
         assert self.stepper.controller_id == controller
         assert self.stepper.axis_id == axis
             
-    def test_usb_return_list(self):
-        """
-        Tests that when a Stepper object is passed to 
-        usb_plugged_devices the returned object is a list.
-        """
-        assert isinstance(self.stepper.usb_plugged_devices(), list)
-    
     def test_usb_return_notempty_list(self):
         """Test that when a Stepper object is passed to 
         usb_plugged_devices, the returned list is not empty."""
         assert self.stepper.usb_plugged_devices() != []
         
+    def test_select_device(self):
+        """Test that when select device is called on a list of devices,
+        the one selected with the input is correct."""
+        random_devs = ["Device1", "Device2", "Device3"]
+        device = self.stepper.select_device(devices = random_devs)
+        assert device in random_devs
+    
+    #######################
+    def test_startup_USB_device(self): 
+        """Tests that when the PI device with the known name is connected
+        with ConnectUSB and startup, a connection is established."""    
+        self.stepper.close_connection()
+        dev_name = "###########"
+        self.stepper.startup_USB_device()
+        assert self.stepper.pidevice.IsConnected()
+        
     def test_connection_is_established(self):
         """
         Tests that when a Stepper object is passed to connect_pidevice,
         a connection to the controller is successfully established.
         """
         self.stepper.connect_pidevice()
         assert self.stepper.pidevice.IsConnected()
@@ -49,479 +66,438 @@
     def test_connected_axis(self):
         """
         Tests that when a Stepper object is connected, the connected axis 
         is one ('1'). C663 controller supports connection with only 
         axis at a time. 
         """
         assert pitools.getaxeslist(self.stepper.pidevice, axes=None) == ['1']
-        
-    def test_pos_is_float(self):
-        """Tests that when the current position of a connected Stepper object is probed, 
-        the position returned by get_curr_pos is a float number."""
-        pos = self.stepper.get_curr_pos()['1']
-        assert isinstance(pos, float)
-    
-    def test_pos_is_in_range(self):
-        """Tests that when the current position of a connected Stepper object is probed, 
-        the position returned by get_curr_pos is comprised in the available range (0,102)"""
-        pos = self.stepper.get_curr_pos()['1']
-        assert pos >= 0.
-        assert pos <= 102.
-        
+                
     def test_negative_reference(self):
         """Tests that when a connected Stepper object is referenced to the
         negative edge of the axis through move_stage_to_ref, the final position
         is indeed the negative edge (0)."""
         self.stepper.move_stage_to_ref('FNL')
         assert isclose(self.stepper.get_curr_pos()['1'],0,rel_tol=1e-8)
 
     def test_positive_reference(self):
         """Tests that when a connected Stepper object is referenced to the
         positive edge of the axis through move_stage_to_ref, the final position
         is indeed the positive edge (102)."""
         self.stepper.move_stage_to_ref('FPL')
         assert isclose(self.stepper.get_curr_pos()['1'],102,rel_tol=1e-8)
-        
-    def test_get_velocity(self):
-        """Tests that when the Stepper object is connected, the method get_velocity
-        returns the correct value of velocity"""
-        velocity = self.stepper.get_velocity()
-        assert isclose(GCS2Commands.qVEL(self.stepper.pidevice)['1'],velocity, rel_tol = 1e-8)
-    
-    def test_get_acceleration(self):
-        """Tests that when the Stepper object is connected, the method get_acceleration
-        returns the correct value of acceleration"""
-        acceleration = self.stepper.get_acceleration()
-        assert isclose(GCS2Commands.qACC(self.stepper.pidevice)['1'],acceleration, rel_tol = 1e-8)
-    
+           
     def test_velocity_is_set(self):
         """Tests that when the velocity of a connected Stepper object is set through set_velocity, 
         the velocity stored in the controller's ROM is indeed the set one."""
-        self.stepper.set_velocity(15.44)
-        assert isclose(self.stepper.get_velocity(),15.44,rel_tol=1e-8)
+        self.stepper.set_velocity(5)
+        assert isclose(self.stepper.get_velocity(),5,rel_tol=1e-8)
     
     def test_acceleration_is_set(self):
         """Tests that when the acceleration of a connected Stepper object is set through set_acceleration, 
         the acceleration stored in the controller's ROM is indeed the set one."""
-        self.stepper.set_acceleration(12.69)
-        assert isclose(self.stepper.get_acceleration(),12.69,rel_tol=1e-8)
+        self.stepper.set_acceleration(5)
+        assert isclose(self.stepper.get_acceleration(),5,rel_tol=1e-8)
        
     def test_target_is_reached(self):
         """Tests that when the connected Stepper object is moved to a certain target through 
         move_stage_to_target, the position when the motion is completed is equal to the target."""
+        self.stepper.move_stage_to_ref('FNL')
         self.stepper.move_stage_to_target(10)
         assert isclose(self.stepper.get_curr_pos()['1'],10,rel_tol=1e-8)
     
-    def test_trigger_is_set(self):
+    def test_trigger_is_enabled(self):
         """Tests that when the trigger of the connected Stepper object is set through 
         configure out_trigger, the type of trigger stored in the ROM is the selected one."""
-        self.stepper.configure_out_trigger(6)
+        self.stepper.enable_out_trigger(6)
         assert self.stepper.pidevice.qCTO(1, 3)[1][3] == '6'
+    
+    ########################################
+    def test_trigger_is_disabled(self):
+        """Tests that when the trigger of the connected Stepper object is set through 
+        configure out_trigger, the type of trigger stored in the ROM is the selected one."""
+        self.stepper.disable_out_trigger(6)
+        assert not self.stepper.pidevice.qTRO(1, 3)[1][3] 
 
     def test_connection_is_closed(self):
         """Tests that the connection of the Stepper object with controller is indeed closed 
         with close_connection."""
         self.stepper.close_connection()
         assert not self.stepper.pidevice.IsConnected()
 
-
 class TestInputProcessor:
-    scanPars = {		
+    def setup_method(self, method):
+        """Setup any state tied to the execution of the given method in a class.
+        `setup_method` is invoked for every test method of a class.
+        """
+        self.scanPars = {		
 			    "type": "discrete",
 			    "scan_edges": [0,1],
                 "stepsize" : 0.1,
 			    "velocity" : 1,
 		    	"acceleration" : 1,
 			    "sampling_freq" : 100
 		        }
-
-    inputprocess = InputProcessor(scanPars)
-
-    def test_initialization(self):
-        """Tests that when an instance of InputProcessor is created, the inizialitation of the 
-        object's attributes through __init__ method is correct."""
-        assert self.inputprocess.type == "discrete"
-        assert isclose(self.inputprocess.scan_edges[0],0,rel_tol = 1e-8)
-        assert isclose(self.inputprocess.scan_edges[1],1,rel_tol = 1e-8)
-        assert isclose(self.inputprocess.stepsize,0.1,rel_tol= 1e-8)
-        assert isclose(self.inputprocess.vel,1,rel_tol=1e-8)
-        assert isclose(self.inputprocess.acc,1,rel_tol=1e-8)
-        assert isclose(self.inputprocess.sampl_freq,100,rel_tol=1e-8)
+    
+    def teardown_method(self, method):
+        """teardown any state that was previously setup with a setup_method
+        call. 
+        """
+        self.scanPars = None
 
     def test_delta_calculation(self):
-        """Tests that when an InputProcessor object is instantiated, the attribute delta 
-        is correctly evaluated through delta_calculator given the input scan_edges."""
-        assert isclose(self.inputprocess.delta,1,rel_tol = 1e-8)
+        """Tests that when the function delta_calculator is called, it correctly evaluates
+        the delta value given the input scan_edges."""
+        expected_delta = 1
+        calculated_delta = delta_calculator(self.scanPars["scan_edges"])
+        assert isclose(calculated_delta,expected_delta,rel_tol = 1e-8)
     
     def test_delta_traslation_invariant(self):
-        """Tests that when an InputProcessor object is instantiated, the attribute delta 
-        is invariant under rigid traslation of the scan_edges coordinates."""
+        """Tests that when the both the scan_edges values are shifted by a constant number, 
+        the delta values before and after translation calculated with delta_calculator are the same."""
         # assumes that scan_edges[1] + 10 < 102
-        self.inputprocess.scan_edges[0] += 10
-        self.inputprocess.scan_edges[1] += 10
-        assert isclose(self.inputprocess.delta,self.inputprocess.delta_calculator(),rel_tol=1e-8)
-        
-    def test_duration_positive(self):
-        """ Tests that when the InputProcessor object is instantiated, the computation 
-        of the duration always results in a positive (>=0, if no motion is desired) number.       
-        """
-        assert self.inputprocess.duration_calculator() >= 0
-       
+        delta_before_traslation = delta_calculator(self.scanPars["scan_edges"])
+        scan_edges = self.scanPars["scan_edges"]
+        scan_edges[0] += 10
+        scan_edges[1] += 10
+        delta_after_translation = delta_calculator(scan_edges)
+        assert isclose(delta_before_traslation,delta_after_translation,rel_tol=1e-8)
+        
     def test_duration_velocity_not_constant(self):
-        """Tests that when the InputProcessor object is instantiated, the computation 
-        of the duration of the motion through duration_calculator is corrected. 
-        Here is covered the case in which a constant velocity is never reached, i.e, sqrt(acc*delta)<=vel         
+        """Tests that when a constant velocity of the stepper is never reached, the computation 
+        of the duration of the motion through duration_calculator is corrected.          
         """
-        assert isclose(self.inputprocess.duration_calculator(),2,rel_tol = 1e-8)
+        delta = delta_calculator(self.scanPars["scan_edges"])
+        vel, acc = self.scanPars["velocity"], self.scanPars["acceleration"]
+        duration = duration_calculator(delta,vel,acc)
+        assert isclose(duration,2,rel_tol = 1e-8)
     
     def test_duration_velocity_constant(self):
-        """Tests that when the InputProcessor object is instantiated, the computation 
-        of the duration of the motion through duration_calculator is corrected. 
-        Here is covered the case in which a constant velocity is reached, i.e, sqrt(acc*delta)>vel         
+        """Tests that when a constant velocity of the stepper is reached, the computation 
+        of the duration of the motion through duration_calculator is corrected.          
         """
-        self.inputprocess.acc = 0.5
-        assert isclose(self.inputprocess.duration_calculator(),2*np.sqrt(2),rel_tol=1e-8)
+        delta = delta_calculator(self.scanPars["scan_edges"])
+        vel, acc = self.scanPars["velocity"], 2
+        duration = duration_calculator(delta,vel,acc)
+        assert isclose(duration,2*np.sqrt(2),rel_tol=1e-8)
 
     def test_rows_continous_values(self):
-        """Tests that when an InputProcessor objected is instantiated and the scan mode is set
-        to continuous, the number of rows of the DAQ must be set to 1"""
-        N_rows , _ = self.inputprocess.rows_columns_contiuous()
+        """Tests that when the type of scan is set to continuous, the number of rows
+        that are calculated with rows_columns_continuous is correct. 
+        """
+        delta = delta_calculator(self.scanPars["scan_edges"])
+        stepsize = self.scanPars["stepsize"]
+        N_rows , _ = rows_columns_contiuous(delta,stepsize)
         assert N_rows == 1
         
-    def test_rows_equal_cols(self):
-        """Tests that when an InputProcessor object is intantiated, the number of columns obtained in 
-        continuous mode is equal to the number of rows obtained in discrete mode."""
-        _ , N_cols = self.inputprocess.rows_columns_contiuous()
-        N_rows, _ = self.inputprocess.rows_columns_discrete()
-        assert isclose(N_rows,N_cols,rel_tol = 1e-8)
-        
     def test_cols_continuous_values(self):
-        """Tests that when an InputProcessor objected in instantiated and the scan mode is set
-        to continuous, the number of columns is given by the floor of the ratio of delta over stepsize."""
-        _ , N_cols = self.inputprocess.rows_columns_contiuous()
+        """Tests that when the type of scan is set to continuous, the number of columns
+        that are calculated with rows_columns_continuous is correct. 
+        """
+        delta = delta_calculator(self.scanPars["scan_edges"])
+        stepsize = self.scanPars["stepsize"]
+        _ , N_cols = rows_columns_contiuous(delta,stepsize)
         assert N_cols == 11
+        
+    def test_rows_discrete_values(self):
+        """Tests that when the type of scan is set to discrete, the number of rows
+        that are calculated with rows_columns_discrete is correct. 
+        """
+        delta = delta_calculator(self.scanPars["scan_edges"])
+        stepsize = self.scanPars["stepsize"]
+        sampl_freq = self.scanPars["samp_freq"]
+        N_rows, _ = rows_columns_discrete(delta,stepsize,sampl_freq)
+        assert N_rows == 11
     
     def test_cols_discrete_values(self):
-        """Tests that when an InputProcessor objected in instantiated and the scan mode is set
-        to discrete, the number of columns of the DAQ must be set to the floor of the product
-        of the sampling frequency with the characteristic time of 50 ms."""
-        _ , N_cols = self.inputprocess.rows_columns_discrete()
-        assert isclose(N_cols,5,1e-8)
+        """Tests that when the type of scan is set to discrete, the number of columns
+        that are calculated with rows_columns_discrete is correct. 
+        """
+        delta = delta_calculator(self.scanPars["scan_edges"])
+        stepsize = self.scanPars["stepsize"]
+        sampl_freq = self.scanPars["samp_freq"]
+        _ , N_cols = rows_columns_discrete(delta,stepsize,sampl_freq)
+        assert N_cols == 5
         
     def test_rows_cols_types(self):
-        """Tests that when an InputProcessor object is instantiated the types of the number of rows
-        and the number of columns (calculated either in continuous or discrete mode) are integer."""
-        N_rows_cont, N_cols_cont = self.inputprocess.rows_columns_contiuous()
-        N_rows_disc, N_cols_disc = self.inputprocess.rows_columns_discrete()
+        """Tests that when rows and columns are calculated in discrete and continuous mode through 
+        rows_columns_continuous and rows_columns_discrete, respectively, the outputted numbers are integer.""""
+        delta = delta_calculator(self.scanPars["scan_edges"])
+        stepsize = self.scanPars["stepsize"]
+        sampl_freq = self.scanPars["samp_freq"]
+        N_rows_cont, N_cols_cont = rows_columns_contiuous(delta,stepsize)
+        N_rows_disc, N_cols_disc = rows_columns_discrete(delta,stepsize,sampl_freq)
         tup = (N_rows_cont,N_cols_cont,N_rows_disc,N_cols_disc)
         assert all(isinstance(i, int) for i in tup)
-
-    def test_daq_pars_is_dict(self):
-        """Tests that when an InputProcessor object is instantiated, the daq_pars object 
-        that is constructed with the values of the DAQ is a dictionary."""
-        daq_pars = self.inputprocess.evaluate_daq_pars()
-        assert isinstance(daq_pars,dict)
     
     def test_daq_pars_continuous(self):
-        """Tests that when an InputProcessor object is instantiated, the scan mode is set 
-        to continuous and the daq_pars dictionary is built-up, the values associated
-        with the keys are corrected. """
-        self.inputprocess.type = "continuous"
-        daq_pars = self.inputprocess.evaluate_daq_pars()
-        N_rows, N_cols = self.inputprocess.rows_columns_contiuous()
-        duration = self.inputprocess.duration_calculator()
-        assert daq_pars["daq_columns"] == N_cols
-        assert daq_pars["daq_rows"] == N_rows
-        assert daq_pars["duration"] == duration
+        """ Tests that when the type of scan is set to continuous, the values of the dictionary "daq_pars" 
+        calculated with the function evaluate_daq_pars are correct.
+        """
+        self.scanPars["type"] == "continuous"
+        daq_pars = evaluate_daq_pars(self.scanPars)
+    
+        assert daq_pars["daq_columns"] == 11
+        assert daq_pars["daq_rows"] == 1
+        assert daq_pars["duration"] == 2
         assert daq_pars["mode"] == "linear"
         assert daq_pars["trigger type"] == "HW trigger"
         assert daq_pars["trigger edge"] == "positive"
-        assert isclose(daq_pars["holdoff"],duration*0.95,rel_tol = 1e-8)
+        assert isclose(daq_pars["holdoff"],2*0.95,rel_tol = 1e-8)
 
     def test_daq_pars_discrete(self):
-        """Tests that when an InputProcessor object is instantiated, the scan mode is set 
-        to discrete and the daq_pars dictionary is built-up, the values associated
-        with the keys are corrected. """
-        self.inputprocess.type = "discrete"
-        daq_pars = self.inputprocess.evaluate_daq_pars()
-        N_rows, N_cols = self.inputprocess.rows_columns_discrete()
+        """ Tests that when the type of scan is set to discrete, the values of the dictionary "daq_pars" 
+        calculated with the function evaluate_daq_pars are correct.
+        """
+        daq_pars = evaluate_daq_pars(self.scanPars)
         duration = 0.05
-        assert daq_pars["daq_columns"] == N_cols
-        assert daq_pars["daq_rows"] == N_rows
-        assert daq_pars["duration"] == duration
+        assert daq_pars["daq_columns"] == 5
+        assert daq_pars["daq_rows"] == 11
+        assert isclose(daq_pars["duration"],duration,rel_tol=1e-8)
         assert daq_pars["mode"] == "Exact (on-grid)"
         assert daq_pars["trigger type"] == "HW trigger"
         assert daq_pars["trigger edge"] == "negative"
         assert isclose(daq_pars["holdoff"],duration*0.95,rel_tol = 1e-8)
 
-
 class TestScanners:
-    inPars = {
-        "scan_pars" : {		
-            "type": "discrete",
-            "scan_edges": [0,1],
-            "stepsize" : 0.1,
-            "velocity" : 1,
-            "acceleration" : 1,
-            "sampling_freq" : 100
-            },
-        "pi" : 	{	
-            "ID":"C-663",
-            "stage_ID": "L-406.40SD00",
-            "refmode": "FNL",
-            "trig_type":6
-		    }
-            }
-    
-    scanner = Scanner(inPars)
-    
+    def setup_method(self, method):
+        """Setup any state tied to the execution of the given method in a class.
+        `setup_method` is invoked for every test method of a class.
+        """
+        self.inPars = {
+            "scan_pars" : {		
+                "type": "discrete",
+                "scan_edges": [0,1],
+                "stepsize" : 0.1,
+                "velocity" : 1,
+                "acceleration" : 1,
+                "sampling_freq" : 100
+                },
+            "pi" : 	{	
+                "ID":"C-663",
+                "stage_ID": "L-406.40SD00",
+                "refmode": "FNL",
+                "trig_type":6
+                }
+                }
+        self.scanner = Scanner(self.inPars)
+
+    
+    def teardown_method(self, method):
+        """teardown any state that was previously setup with a setup_method
+        call.
+        """
+        self.scanner = None
+        self.inPars = None
+                
     def test_initialization_pars(self):
-        """Tests that when an instance of Scan1D is created, the inizialitation of the 
+        """Tests that when an instance of scanner is created, the inizialitation of the 
         object's attributes through __init__ method is correct."""
         assert self.scanner.PI["ID"] == "C-663"
         assert self.scanner.PI["stage_ID"] == "L-406.40SD00"
         assert self.scanner.PI["refmode"] == "FNL"
         assert self.scanner.PI["trig_type"] == 6
         assert self.scanner.scan_pars["type"] == "discrete"
         assert isclose(self.scanner.scan_pars["scan_edges"][0],0,rel_tol = 1e-8)
         assert isclose(self.scanner.scan_pars["scan_edges"][1],1,rel_tol = 1e-8)
         assert isclose(self.scanner.scan_pars["stepsize"],0.1,rel_tol = 1e-8)
-        assert isclose(self.scanner.scan_pars["velocity"],1,rel_tol= 1e-8)
-        assert isclose(self.scanner.scan_pars["acceleration"],1,rel_tol= 1e-8)
-        assert isclose(self.scanner.scan_pars["sampling_freq"],100,rel_tol= 1e-8)
-    
+        
     def test_dimension_target_positions(self):
-        """Tests that when an instance of Scan1D is created,the dimension of the 
+        """Tests that when an instance of scanner is created,the dimension of the 
         targets array is correct." 
         """
         N_targets = 11
         assert len(self.scanner.targets) == N_targets
         
     def test_values_target_positions(self):
-        """Tests that when an instance of Scan1D is created, the first and the final 
-        point of targets is correct."""
+        """Tests that when an instance of scanner is created, the first and the final 
+        point of targets are correct."""
         assert isclose(self.scanner.targets[0],self.scanner.scan_edges[0],rel_tol = 1e-8)
         assert isclose(self.scanner.targets[-1],self.scanner.scan_edges[1],rel_tol = 1e-8)  # by induction is right because of linspace
     
     def test_stepper_is_instantiated(self):
-        """Tests that when an instance of Scan1D is created, the instance of Stepper
+        """Tests that when an instance of scanner is created, the instance of Stepper
         is properly instantiated throught the __init__ method."""
         assert isinstance(self.scanner.stepper,Stepper)
     
-    def test_stepper_is_connected(self):
-        """Tests that when an instance of Scan1D is created and connected_master is called, 
-        master is properly connected to the PI controller"""
-        self.scanner.connect_stepper()
-        assert self.scanner.stepper.pidevice.isConnected()
-
-    def test_vel_acc_stepper(self):
-        """Tests that when an instance of Scan1D is created and stepper is connected, 
-        velocity and acceleration are properly set through the method setup_motion_stepper"""
-        self.scanner.setup_motion_stepper(self)
-        assert isclose(self.scanner.stepper.get_velocity(),1,rel_tol = 1e-8)
-        assert isclose(self.scanner.stepper.get_acceleration(),1,rel_tol = 1e-8)
-        
-    def test_initial_scan_position(self):
-        """Tests that when an instance of Scan1D is created and init_stepper_scan is called,
-        the axis is moved to the first target position."""
-        self.scanner.init_stepper_scan()
-        cur_pos = self.scanner.stepper.get_curr_pos()
-        assert isclose(cur_pos,self.scanner.targets[0])
-
-    def test_trigger_is_configured(self):
-        """Tests that when an instance of Scan1D is created and init_1D_scan is called, 
-        the output trigger is set and activated.
-        """
-        trig_type = self.inPars ["pi"]["trig_type"]
-        assert self.scanner.stepper.pidevice.qCTO(1, 3)[1][3] == str(trig_type)
-        
+    def test_context_manager_enter(self):
+        """Tests that when an instance of scanner is created and the context manager is opened, 
+        the stepper object connects to the controller and gets referenced to negative edge."""
+        with self.scanner as scan:
+            assert scan.stepper.pidevice.isConnected()
+            assert isclose(scan.stepper.get_curr_pos()['1'],0,rel_tol=1e-8)
+
+    def test_context_manager_exit(self):
+        """Tests that when an instance of scanner is created and the context manager is opened and closed, 
+        the connection is also closed"""
+        with self.scanner as scan:
+            pass
+        assert not self.scanner.stepper.pidevice.isConnected()
+
     def test_discrete_scan(self):
         """Tests that when an instance of Scan1D is created and execute_discrete_scan
            is performed, the covered positions are the targeted ones."""
-        self.scanner.init_stepper_scan()
-        cur_pos = self.scanner.execute_discrete_scan()
+        with self.scanner as scan:
+            cur_pos = scan.execute_discrete_scan()
         assert all(abs(pos - target) <= 0.5e-3 for pos, target in zip(cur_pos, self.scanner.targets))
-    
-    def test_continuous_1D_scan(self):
-        """Tests that when an instance of Scan1D is created and execute_continuous_scan
-        is performed, the position of the stage is equal to the last target point.
-        """
-        self.scanner.init_stepper_scan()
-        self.scanner.execute_continuous_scan()
-        cur_pos = self.scanner.stepper.get_curr_pos()
-        assert isclose(cur_pos,self.scanner.targets[-1])
-        
+
 class TestOutputProcessor:
-    scan_pars = {		
-            "type": "discrete",
-            "scan_edges": [0.3,0.],
-            "stepsize" : 0.001,
-            "velocity" : 1,
-            "acceleration" : 1,
-            "sampling_freq" : 100
-            }
-    daq_pars = {
-                "daq_columns" : 100,
-                "daq_rows" : 300,
-                "duration" : 0.05,
-                "mode" : "Exact (on-grid)",
-                "trigger type" : "HW trigger",
-                "trigger edge" : "negative",
-                "holdoff" : 0.05*(0.95),
-            }     
-    
-    filename = "dev4910_demods_0_sample_r_avg_00000.csv"
-    outputprocess = OutputProcessor(filename,scan_pars,daq_pars)
-    
-    def test_initialization_scan_pars(self):
-        """Tests that when an OutputProcessor object is instantiated, the attributes inizialization
-        through the __init__ method is correct"""
-        assert self.scan_pars == self.outputprocess.scan_pars
-        assert self.filename == self.outputprocess.filename
-        assert self.daq_pars["daq_columns"] == self.outputprocess.N_cols
-        assert self.daq_pars["daq_rows"] == self.outputprocess.N_rows
-        
-    def test_raw_data_shape(self):
-        """Tests that when an OutProcessor object is instantiated and get_raw_data is called,
-        the returned NumPy has the correct number of rows"""
-        raw_data = np.genfromtxt(self.filename,skip_header = 1, delimiter = ";")
-        returned_column = self.outputprocess.get_raw_data()
-        assert raw_data.shape[0] == returned_column.shape[0]
+    def setup_method(self, method):
+        """Setup any state tied to the execution of the given method in a class.
+        `setup_method` is invoked for every test method of a class.
+        """
+        
+        self.scan_pars = {		
+                        "type": "discrete",
+                        "scan_edges": [0.3,0.],
+                        "stepsize" : 0.001,
+                        "velocity" : 1,
+                        "acceleration" : 1,
+                        "sampling_freq" : 100
+                        }
+        self.daq_pars = {
+                        "daq_columns" : 100,
+                        "daq_rows" : 300,
+                        "duration" : 0.05,
+                        "mode" : "Exact (on-grid)",
+                        "trigger type" : "HW trigger",
+                        "trigger edge" : "negative",
+                        "holdoff" : 0.05*(0.95),
+                        }   
+        self.filename =  "input/dev4910_demods_0_sample_r_avg_00000.csv"  
+                    
+    def teardown_method(self, method):
+        """teardown any state that was previously setup with a setup_method
+        call.
+        """
+        self.scan_pars = None
+        self.daq_pars = None
 
     def test_raw_data_values(self):
-        """Tests that when an OutProcessor object is instantiated and get_raw_data is called,
-        the returned NumPy has the same values of the original one."""
+        """Tests that when when the data outputted by the Zurich lock-in are read through get_raw_data,
+        the returned NumPy has the same values of the original one.
+        """
         # find raw data column directly, select only non nan values
         raw_data = np.genfromtxt(self.filename,skip_header = 1, delimiter = ";")
         raw_column = raw_data[:,2]
         raw_column_not_nan = raw_column[~np.isnan(raw_column)]
         # find raw data through get_raw_data, select only non nan values
-        returned_column = self.outputprocess.get_raw_data()
+        returned_column = get_raw_data(self.filename)
         returned_column_not_nan = returned_column[~np.isnan(returned_column)]
         assert all(abs(raw - returned)/raw <= 1e-8 for raw, returned in zip(raw_column_not_nan,returned_column_not_nan))
     
     def test_dimension_averaged_subintervals_is_rows(self):
-        """Tests tat when an OutputProcessor object is instantiated and evaluate_averaged_data is called, 
+        """Tests tat when raw data are read with get_raw_data and evaluate_averaged_data is called, 
         the dimension of the returned array (with averaged subintervals) is equal to the 
         number of rows"""
-        returned_column = self.outputprocess.get_raw_data()
-        avg_returned_column = self.outputprocess.evaluate_averaged_data(returned_column)
+        returned_column = get_raw_data(self.filename)
+        avg_returned_column = evaluate_averaged_data(returned_column)
         N_rows_avg = len(avg_returned_column)
         assert self.daq_pars["daq_rows"] == N_rows_avg
         
-    
     def test_average_data(self):
-        """Tests that when an OutputProcessor object is instantiated and evaluate_average_data
+        """Tests that when raw data are read by get_raw_data and evaluate_average_data
         is called, the average of the averaged subintervals (of N_cols dimensions) is equal to the
-        average of the overall raw_data. This is justified by subintervals of equal dimension"""
+        average of the overall raw_data. This is justified by subintervals of equal dimension
+        """
         # find raw data column directly, select only non nan values
         raw_data = np.genfromtxt(self.filename,skip_header = 1, delimiter = ";")
         raw_column = raw_data[:,2]
         raw_column_not_nan = raw_column[~np.isnan(raw_column)]
+        avg_raw= np.mean(raw_column_not_nan)
         # find raw data through get_raw_data, select only non nan values
-        returned_column = self.outputprocess.get_raw_data()
+        returned_column = get_raw_data(self.filename)
         returned_column_not_nan = returned_column[~np.isnan(returned_column)]        
         # average subintervals of returned_column_not_nan
-        avg_returned_column = self.outputprocess.evaluate_averaged_data(returned_column_not_nan)
-        avg_raw= np.mean(raw_column_not_nan)
-
+        avg_returned_column = evaluate_averaged_data(returned_column_not_nan)
         # average averaged subintervals of returned_column_not_nan
         avg_avg_returned = np.mean(avg_returned_column)
-          
-        assert isclose(avg_avg_returned,avg_raw,rel_tol = 1e-12)
+        assert isclose(avg_avg_returned,avg_raw,rel_tol = 1e-8)
         
     def test_dimension_target_positions(self):
-        """Tests that when an instance of OutputProcessor is created and evaluate_target_position is called,
+        """Tests that when target positions are evaluated through evaluate_target_position,
         the dimension of the targets array is correct."""
         scanedges = self.scan_pars["scan_edges"]
         stepsize = self.scan_pars["stepsize"]
-        targets = self.outputprocess.evaluate_target_positions(scanedges,stepsize)
+        targets = evaluate_target_positions(scanedges,stepsize)
         N_targets = 301
         assert N_targets == len(targets)
         
     def test_values_target_positions(self):
-        """Tests that when an instance of OutputProcessor is created and evasluate_target_position is called,
+        """Tests that when target positions are evaluated through evaluate_target_position,
         the first and the last point of the target array is corrected"""
         scanedges = self.scan_pars["scan_edges"]
         stepsize = self.scan_pars["stepsize"]
-        targets = self.outputprocess.evaluate_target_positions(scanedges,stepsize)
-
+        targets = evaluate_target_positions(scanedges,stepsize)
         assert isclose(scanedges[0],targets[0],rel_tol = 1e-8)
         assert isclose(scanedges[1],targets[-1],rel_tol = 1e-8)  # by induction is right because of linspace
 
-    
     def test_save_data_file(self):
-        """Tests that when an instance of OutputProcessor is created and save_data_file  is called, 
-        an output file named "cleaned_1D_data.txt" is indeed saved in the current folder"""
+        """Tests that when processed data are saved through save_data_file,
+        an output file named "cleaned_1D_data.txt" with the correct values is stored in the output folder.
+        """
         # create fictitious targets 
         targets  = np.array([1,2,3,4,5],dtype=float)
         # create fictitious signal values
         avg_val = np.random.random(size = len(targets))
         # save file to "cleaned_1D_data.txt"
-        self.outputprocess.save_data_file(targets,avg_val)
+        save_data_file(targets,avg_val)
         # expected output
         expected_output = ''
         for i in range(len(targets)):
             expected_output += '\b'+str(targets[i])+', '+'{:.6f}'.format(avg_val[i])+'\n'
-
         # Read the file contents and compare with expected output
-        with open("cleaned_1D_data.txt", "rb") as f:
+        with open("output/cleaned_1D_data.txt", "rb") as f:
             assert f.read(),expected_output
             
         
 class TestInputValidator:
     """ A class to test that when invalid input scan parameters are inserted, an exeption is raised and the code stops the execution. 
      Although a lower-level control is already present in the internal PI subroutines, it takes time to be activated. 
      Therefore, this additional entrance control find out invalid inputs without the need of connecting to the PI instrument. 
     """
-
-    scanPars = {		
-        "type": "discrete",
-        "scan_edges": [0,1],
-        "stepsize" : 0.1,
-        "velocity" : 1,
-        "acceleration" : 1,
-        "sampling_freq" : 100
-        }
-    
-    
-    inputval = InputValidator(scan_pars=scanPars)
-      
-    def test_valid_input(self):
-        """Tests that when an InputValidator class is instantiated and corrected values of scan parameters
-        are provided, the validate method does not raise any error and return True."""
-        assert self.inputval.validate() == True
-
     def test_invalid_type(self):
-        """Tests that when an InputValidator class is instantiated and an invalid value of 'type' is passed 
-        to the validate_type function, an exception is raised."""
-        self.inputval.type = "invalid"
+        """Tests that when an invalid value of 'type' is passed to the validate_type function,
+        an exception (ValueError) is raised."""
+        type = "invalid"
         with pytest.raises(ValueError):
-            self.inputval.validate_type()
+            validate_type(type)
 
     def test_invalid_scan_edges(self):
-        """ Tests that when an InputValidator class is instantiated an invalid value of 'scan_edges' is passed 
-        to the validate_scan_edges function, an exception is raised """
-        self.inputval.scan_edges = [-10, 110]
+        """ Tests that when an invalid value of 'scan_edges' is passed to the validate_scan_edges function,
+        an exception (ValueError) is raised """
+        scan_edges = [-10, 110]
         with pytest.raises(ValueError):
-            self.inputval.validate_scan_edges()
+            validate_scan_edges(scan_edges)
     
     def test_invalid_stepsize(self):
-        """ Tests that when an InputValidator class is instantiated an invalid value of 'stepsize' is passed 
-        to the validate_stepsize function, an exception is raised """
-        self.inputval.stepsize = 200
+        """ Tests that an invalid value of 'stepsize' is passed to the validate_stepsize function,
+        an exception (ValueError) is raised """
+        stepsize = 200
         with pytest.raises(ValueError):
-            self.inputval.validate_stepsize()
+            validate_stepsize(stepsize)
 
     def test_invalid_velocity(self):
-        """ Tests that when an InputValidator class is instantiated an invalid value of 'velocity' is passed 
-        to the validate_velocity function, an exception is raised """
-        self.inputval.velocity = -5
+        """ Tests that when an invalid value of 'velocity' is passed to the validate_velocity function, 
+        an exception (valueError) is raised """
+        velocity = -5
         with pytest.raises(ValueError):
-            self.inputval.validate_velocity()
+            validate_velocity(velocity)
 
     def test_invalid_acceleration(self):
-        """ Tests that when an InputValidator class is instantiated an invalid value of 'acceleration' is passed 
-        to the validate_velocity function, an exception is raised """
-        self.inputval.acceleration = 30
+        """ Tests that when an invalid value of 'acceleration' is passed to the validate_velocity function,
+        an exception (ValueError) is raised """
+        acceleration = 30
         with pytest.raises(ValueError):
-            self.inputval.validate_acceleration()
+            validate_acceleration(acceleration)
+
+def test_valid_input(self):
+        """Tests that when corrected values of scan parameters are provided, all the input validations 
+        are successfull."""
+        scanPars = {		
+                "type": "discrete",
+                "scan_edges": [0,1],
+                "stepsize" : 0.1,
+                "velocity" : 1,
+                "acceleration" : 1,
+                "sampling_freq" : 100
+                }
+        assert validate(scanPars)
```

