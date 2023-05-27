# Comparing `tmp/PyQCAMS-1.0.0.tar.gz` & `tmp/PyQCAMS-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQCAMS-1.0.0.tar", last modified: Mon Apr  3 22:05:47 2023, max compression
+gzip compressed data, was "PyQCAMS-1.0.1.tar", last modified: Sat May 27 21:38:30 2023, max compression
```

## Comparing `PyQCAMS-1.0.0.tar` & `PyQCAMS-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0 roots     (1000) roots     (1000)        0 2023-04-03 22:05:47.048899 PyQCAMS-1.0.0/
--rwxrwxrwx   0 roots     (1000) roots     (1000)      250 2023-04-03 22:05:47.043980 PyQCAMS-1.0.0/PKG-INFO
-drwxrwxrwx   0 roots     (1000) roots     (1000)        0 2023-04-03 22:05:46.825750 PyQCAMS-1.0.0/PyQCAMS.egg-info/
--rwxrwxrwx   0 roots     (1000) roots     (1000)      250 2023-04-03 22:05:46.000000 PyQCAMS-1.0.0/PyQCAMS.egg-info/PKG-INFO
--rwxrwxrwx   0 roots     (1000) roots     (1000)      266 2023-04-03 22:05:46.000000 PyQCAMS-1.0.0/PyQCAMS.egg-info/SOURCES.txt
--rwxrwxrwx   0 roots     (1000) roots     (1000)        1 2023-04-03 22:05:46.000000 PyQCAMS-1.0.0/PyQCAMS.egg-info/dependency_links.txt
--rwxrwxrwx   0 roots     (1000) roots     (1000)       51 2023-04-03 22:05:46.000000 PyQCAMS-1.0.0/PyQCAMS.egg-info/requires.txt
--rwxrwxrwx   0 roots     (1000) roots     (1000)        8 2023-04-03 22:05:46.000000 PyQCAMS-1.0.0/PyQCAMS.egg-info/top_level.txt
--rwxrwxrwx   0 roots     (1000) roots     (1000)      381 2023-04-03 22:00:48.000000 PyQCAMS-1.0.0/README.md
-drwxrwxrwx   0 roots     (1000) roots     (1000)        0 2023-04-03 22:05:47.005528 PyQCAMS-1.0.0/pyqcams/
--rwxrwxrwx   0 roots     (1000) roots     (1000)       15 2023-04-03 15:05:00.000000 PyQCAMS-1.0.0/pyqcams/__init__.py
--rwxrwxrwx   0 roots     (1000) roots     (1000)      273 2023-03-30 15:34:08.000000 PyQCAMS-1.0.0/pyqcams/constants.py
--rwxrwxrwx   0 roots     (1000) roots     (1000)     4453 2023-04-03 16:28:07.000000 PyQCAMS-1.0.0/pyqcams/plotters.py
--rwxrwxrwx   0 roots     (1000) roots     (1000)    33321 2023-04-03 17:15:06.000000 PyQCAMS-1.0.0/pyqcams/pymar.py
--rwxrwxrwx   0 roots     (1000) roots     (1000)     5257 2023-04-03 21:05:10.000000 PyQCAMS-1.0.0/pyqcams/util.py
--rwxrwxrwx   0 roots     (1000) roots     (1000)       38 2023-04-03 22:05:47.050898 PyQCAMS-1.0.0/setup.cfg
--rwxrwxrwx   0 roots     (1000) roots     (1000)      543 2023-04-03 19:15:38.000000 PyQCAMS-1.0.0/setup.py
+drwxrwxrwx   0 roots     (1000) roots     (1000)        0 2023-05-27 21:38:30.076899 PyQCAMS-1.0.1/
+-rwxrwxrwx   0 roots     (1000) roots     (1000)     1063 2023-03-30 15:34:08.000000 PyQCAMS-1.0.1/LICENSE
+-rwxrwxrwx   0 roots     (1000) roots     (1000)     1416 2023-05-27 21:38:30.072898 PyQCAMS-1.0.1/PKG-INFO
+drwxrwxrwx   0 roots     (1000) roots     (1000)        0 2023-05-27 21:38:29.790670 PyQCAMS-1.0.1/PyQCAMS.egg-info/
+-rwxrwxrwx   0 roots     (1000) roots     (1000)     1416 2023-05-27 21:38:29.000000 PyQCAMS-1.0.1/PyQCAMS.egg-info/PKG-INFO
+-rwxrwxrwx   0 roots     (1000) roots     (1000)      307 2023-05-27 21:38:29.000000 PyQCAMS-1.0.1/PyQCAMS.egg-info/SOURCES.txt
+-rwxrwxrwx   0 roots     (1000) roots     (1000)        1 2023-05-27 21:38:29.000000 PyQCAMS-1.0.1/PyQCAMS.egg-info/dependency_links.txt
+-rwxrwxrwx   0 roots     (1000) roots     (1000)       96 2023-05-27 21:38:29.000000 PyQCAMS-1.0.1/PyQCAMS.egg-info/requires.txt
+-rwxrwxrwx   0 roots     (1000) roots     (1000)        8 2023-05-27 21:38:29.000000 PyQCAMS-1.0.1/PyQCAMS.egg-info/top_level.txt
+-rwxrwxrwx   0 roots     (1000) roots     (1000)      915 2023-05-27 21:12:06.000000 PyQCAMS-1.0.1/README.md
+drwxrwxrwx   0 roots     (1000) roots     (1000)        0 2023-05-27 21:38:30.033182 PyQCAMS-1.0.1/pyqcams/
+-rwxrwxrwx   0 roots     (1000) roots     (1000)       15 2023-04-03 15:05:00.000000 PyQCAMS-1.0.1/pyqcams/__init__.py
+-rwxrwxrwx   0 roots     (1000) roots     (1000)      273 2023-03-30 15:34:08.000000 PyQCAMS-1.0.1/pyqcams/constants.py
+-rwxrwxrwx   0 roots     (1000) roots     (1000)     2616 2023-05-22 15:19:49.000000 PyQCAMS-1.0.1/pyqcams/numv.py
+-rwxrwxrwx   0 roots     (1000) roots     (1000)     4528 2023-05-10 15:47:15.000000 PyQCAMS-1.0.1/pyqcams/plotters.py
+-rwxrwxrwx   0 roots     (1000) roots     (1000)     1986 2023-05-10 15:44:49.000000 PyQCAMS-1.0.1/pyqcams/psave.py
+-rwxrwxrwx   0 roots     (1000) roots     (1000)    33310 2023-05-27 21:05:23.000000 PyQCAMS-1.0.1/pyqcams/pymar.py
+-rwxrwxrwx   0 roots     (1000) roots     (1000)     5029 2023-05-27 21:05:26.000000 PyQCAMS-1.0.1/pyqcams/util.py
+-rwxrwxrwx   0 roots     (1000) roots     (1000)       38 2023-05-27 21:38:30.078899 PyQCAMS-1.0.1/setup.cfg
+-rwxrwxrwx   0 roots     (1000) roots     (1000)      839 2023-05-27 21:37:45.000000 PyQCAMS-1.0.1/setup.py
```

### Comparing `PyQCAMS-1.0.0/pyqcams/plotters.py` & `PyQCAMS-1.0.1/pyqcams/plotters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.animation as animation
 import mpl_toolkits.mplot3d.axes3d as p3
-from .constants import *
+from . import constants
 
 def traj_plt(traj, ax, title = True, legend = True):
     '''
     Plot trajectory of a QCT calculation.
 
     Input:
     traj, QCT object
     ax, axis labele
     '''
     r = traj.r
-    t = traj.t*ttos*10e12 # Convert a.u. to ns 
+    t = traj.t*constants.ttos*10e12 # Convert a.u. to ns 
     m1,m2,m3 = traj.m1, traj.m2, traj.m3
     mtot = m1 + m2 + m3
 
     r12 = np.sqrt(r[0]**2+r[1]**2+r[2]**2)
     r32 = np.sqrt((r[3] - m1*r[0]/(m1+m2))**2
                 + (r[4] - m1*r[1]/(m1+m2))**2 
                 + (r[5] - m1*r[2]/(m1+m2))**2)
@@ -28,15 +28,15 @@
     ax.plot(t, r32, label = 'r32')
     ax.plot(t, r31, label = 'r31')
     ax.set_xlabel('$t (ns)$')
     ax.set_ylabel('$r (a_0)$')
     if legend == True:
         ax.legend()
     if title == True:
-        ax.set_title(f'Energy: {traj.e0/cEK2H}K')
+        ax.set_title(f'Energy: {traj.e0/constants.cEK2H}K')
 
 def plot_e(traj, ax):
     ax.plot(traj.t,traj.E12,label = 'E12')
     # plt.hlines(bd12,traj.t[0],traj.t[-1], linestyle = 'dashed',label = 'bd12')
     ax.plot(traj.t,traj.E32,label = 'E32')
     # plt.hlines(bd32,traj.t[0],traj.t[-1], color = 'orange',linestyle = 'dashed', label = 'bd32')
     ax.plot(traj.t,traj.E31,label = 'E31')
@@ -45,14 +45,17 @@
     ax.set_xlabel('time (a.u)')
     ax.set_ylabel('$E_(E_H)$')
     ax.legend()
     ax.set_title('Energy vs t')
 
 
 def traj_3d(traj):
+    '''
+    Make a 3-d trace of the trajectory.
+    '''
     r = traj.r
     m1,m2,m3 = traj.m1, traj.m2, traj.m3
     mtot = m1 + m2 + m3
     c1 = m1/(m1+m2)
     c2 = m2/(m1+m2)
     r1 = np.array([-c2*r[i] - m3/mtot*r[i+3] for i in range(0,3)]) #x,y,z for particle 1
     r2 = np.array([c1*r[i]-m3/mtot*r[i+3] for i in range(0,3)])
```

### Comparing `PyQCAMS-1.0.0/pyqcams/pymar.py` & `PyQCAMS-1.0.1/pyqcams/pymar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from scipy.integrate import solve_ivp, quad
 from scipy.optimize import root_scalar, fsolve
-from scipy import constants
 import warnings
-from . import util, constants
+from pyqcams import util, constants
 import json
 
 
 class Energy(object):
     '''DVR with sine function basis for non-periodic functions over
         [xmin,xmax] interval.
     
@@ -69,40 +68,41 @@
         bv = np.asarray(bv)
         bv *= self.j*(self.j+1)
         evj = evals + bv
         return evj
     
     def turningPts(self, V, re, v=0):
         ''' Setter function for turning points, period, & n of energy level of a given (v,j)
-        Evj, list
-            energy spectrum
         V, function
             potential
-        mu, float
-            reduced mass
         re, float
             equilibrium length of molecule
         v, int
             vibrational quantum number
-        b, function
-            buckingham potentential 
-            (if V is piecewise, root_scalar doesn't work.
-            However, DVR must still be done on the piecewise function.)
         '''
         self.v = v # Assign the molecules vibrational number
         self.evj = self.eDVR(V) 
         vbrot = lambda r: -self.j*(self.j+1)/2/self.mu/(r**2)- V(r)+ self.evj[self.v]
-        # x = np.linspace(.5,10,1000)
-        # plt.plot(x,V(x))
-        # plt.hlines(evj[0], 0, 5)
-        # plt.show()
-        # print(self.xmin)
-        rm = root_scalar(vbrot,bracket = [self.xmin,re]).root
-        rp = root_scalar(vbrot,bracket = [re,self.xmax]).root
-        
+        x = np.linspace(self.xmin,self.xmax,1000)
+        try:
+            rm = root_scalar(vbrot,bracket = [self.xmin,re]).root
+            rp = root_scalar(vbrot,bracket = [re,self.xmax]).root
+        except:
+            print('Root solver failed. Try adjusting your guess equilibrium point.\n'
+                  'It should fall between the classical turning points.')
+            fig = input('Would you like to see a plot of your potential? '
+                        'Type "y" for yes, or "n" for no: \n')
+            if fig == 'y':
+                # Show re guess compared with elev
+                plt.plot(x,V(x))
+                plt.plot(re,V(re), marker = 'o')
+                plt.hlines(self.evj[self.v], 0, 5)
+                plt.ylim(self.evj[self.v]*3, V(re)*3) # zoom in
+                plt.show()
+            quit()
         # Integrate to solve for tau, n_vib
         tau = quad(lambda x: 1/np.sqrt(vbrot(x)),rm,rp)[0]
         vib = quad(lambda x: np.sqrt(vbrot(x)),rm,rp)[0]
         tau *= np.sqrt(2*self.mu)
         n_vib = np.round(-0.5 + vib*np.sqrt(2*self.mu)/np.pi)
         self.n_vib = n_vib
         self.tau = tau
@@ -682,38 +682,34 @@
         np.set_printoptions(suppress = True) # Remove sci notation
         self.count = [n12,n32,n31,nd,comp]
         self.f_state = [vt, w, j_eff]
         self.f_p = [p1x[-1], p1y[-1], p1z[-1],
                     p2x[-1], p2y[-1], p2z[-1]]
         self.delta_e = En[-1]-En[0]
         self.delta_p = Ln[-1] - Ln[0]
-        # return count, r, t
-        # return count
         return
 
 class Potential(object):
     """
     Potential functions.
     """
-    def morse(self, de = 1.,alpha = 1.,re = 1., we = .1):
+    def morse(self, de = 1.,alpha = 1.,re = 1.):
         '''Usage:
                 V = morse(**kwargs)
         
         Return a one-dimensional morse potential:
         V(r) = De*(1-exp(-a*(r-re)))^2 - De
 
         Keyword arguments:
         de, float
             dissociation energy (depth)
         alpha, float
             returned from eVib function
         re, float
             equilibrium length
-        we, float
-            vibrational frequency
         '''
         V = lambda r: de*(1-np.exp(-alpha*(r-re)))**2 - de
         dV = lambda r: 2*alpha*de*(1-np.exp(-alpha*(r-re)))*np.exp(-alpha*(r-re))
         return V, dV
     
     def lj(self, m=12, n = 6, cm = 1., cn=1., **kwargs):
         '''Usage:
@@ -787,61 +783,64 @@
         directory to JSON input file
     '''
     with open(f'{input_file}') as f:
         data = json.load(f)
     potential_AB = data['potential_AB'] # which potential
     potential_BC = data['potential_BC']
     potential_CA = data['potential_CA']
-    mol1 = data['potential_params']["AB"][f"{potential_AB}"]  # potential parameters
-    mol2 = data['potential_params']["BC"][f"{potential_BC}"]
-    mol3 = data['potential_params']["CA"][f"{potential_CA}"]
-    xmin = data['potential_params']["AB"]['xmin'] 
-    xmax = data['potential_params']["AB"]['xmax']
+    vList = ['morse','buck','lj']
+    vF = Potential()
     m1,m2,m3 = data['masses'].values() # masses
     m12 = m1*m2/(m1+m2)
-    m23 = m2*m3/(m2+m3)
-    m31 = m1*m3/(m1+m3)
-    vF = Potential()
-    # Create energy object according to chosen potential
-    if potential_AB == 'morse':
-        mol1['alpha'] = mol1['we']*np.sqrt(m12/2/mol1['de'])
-        mol1_V, mol1_dV = vF.morse(**mol1)
-    elif potential_AB == 'lj':
-        mol1_V, mol1_dV = vF.lj(**mol1)
-    elif potential_AB == 'buck':
-        mol1_V, mol1_dV, xmin= vF.buckingham(**mol1)
 
+    if potential_AB in vList:
+        mol1 = data['potential_params']["AB"][f"{potential_AB}"]  # potential parameters
+        if potential_AB == 'morse':
+                mol1_V, mol1_dV = vF.morse(**mol1)
+        elif potential_AB == 'lj':
+            mol1_V, mol1_dV = vF.lj(**mol1)
+        elif potential_AB == 'buck':
+            mol1_V, mol1_dV, xmin= vF.buckingham(**mol1)
+        if xmin == None:
+            xmin = data['potential_params']["AB"]['xmin'] 
+        xmax = data['potential_params']["AB"]['xmax']
+    else: # numerical
+        mol1 = {}
+        xvals, mol1_V, mol1_dV, mol1['re'] = util.numToV(f'{potential_AB}') # Find V, dV via spline
+        xmin = min(xvals)
+        xmax = max(xvals)
+
+    # Create energy object according to chosen potential
     AB = Energy(mu=m12, npts=data['potential_params']["AB"]['npts'], xmin = xmin,
                 xmax = xmax, j = data['ji'])
     AB.turningPts(mol1_V,mol1['re'], v= data['vi']) # Assign attributies evals, rm, rp
-    # else:
-    #     print('This potential is not available: \
-    #           Choose from morse, lj, buck.')
-
-    if potential_BC == 'morse':
-        mol2['alpha'] = mol2['we']*np.sqrt(m23/2/mol2['de'])
-        mol2_V, mol2_dV = vF.morse(**mol2)
-    elif potential_BC == 'lj':
-        mol2_V, mol2_dV = vF.lj(**mol2)
-    elif potential_BC == 'buck':
-        mol2_V, mol2_dV, _ = vF.buckingham(**mol2)
+        
+    if potential_BC in vList:
+        mol2 = data['potential_params']["BC"][f"{potential_BC}"]
+        if potential_BC == 'morse':
+            mol2_V, mol2_dV = vF.morse(**mol2)
+        elif potential_BC == 'lj':
+            mol2_V, mol2_dV = vF.lj(**mol2)
+        elif potential_BC == 'buck':
+            mol2_V, mol2_dV, _ = vF.buckingham(**mol2)
     else:
-        print('This potential is not available: \
-              Choose from morse, lj, buck.')
+        mol2 = {}
+        _, mol2_V, mol2_dV, mol2['re'] = util.numToV(f'{potential_BC}')
 
-    if potential_CA == 'morse':
-        mol3['alpha'] = mol3['we']*np.sqrt(m31/2/mol3['de'])
-        mol3_V, mol3_dV = vF.morse(**mol3)
-    elif potential_CA == 'lj':
-        mol3_V, mol3_dV = vF.lj(**mol3)
-    elif potential_CA == 'buck':
-        mol3_V, mol3_dV, _ = vF.buckingham(**mol3)
+    if potential_CA in vList:
+        mol3 = data['potential_params']["CA"][f"{potential_CA}"]
+        if potential_CA == 'morse':
+            mol3_V, mol3_dV = vF.morse(**mol3)
+        elif potential_CA == 'lj':
+            mol3_V, mol3_dV = vF.lj(**mol3)
+        elif potential_CA == 'buck':
+            mol3_V, mol3_dV, _ = vF.buckingham(**mol3)
     else:
-        print('This potential is not available: \
-              Choose from morse, lj, buck.')
+        mol3 = {}
+        _, mol3_V, mol3_dV, mol3['re'] = util.numToV(f'{potential_CA}')
 
     # Calculate relevant attributes
     inputs = {'m1' : m1, 'm2': m2, 'm3': m3, 
          'd0' : data['r0'], 'e0' : data['Ec (K)']*constants.cEK2H,
          'b': data['b'],'mol': AB, 'v1' : mol1_V, 'v2' : mol2_V, 'v3':mol3_V,
          'dv1' : mol1_dV,'dv2': mol2_dV, 'dv3': mol3_dV,
          're1' : mol1['re'], 're2': mol2['re'], 're3': mol3['re'],
@@ -853,15 +852,9 @@
     a = QCT(**kwargs)
     a.runT(doplot = plot)
     # result = {'d_e': a.delta_e}
     # return result
     return util.get_results(a)
 
 if __name__ == '__main__':
-    # inputs = start('inputs.json')
-    # # for i in range(10):
-    # #     a = QCT(**inputs)
-    # #     a.runT()
-    # #     with open('e_cons.csv','a') as f:
-    # #         f.write(f'{a.delta_e}\n')
-    # print(main(plot = True, **inputs))
-    print(constants.angstrom/constants.physical_constants['Bohr radius'][0])
+    calc = start('example/h2_ca/inputs.json')
+    print(main(plot = True, **calc))
```

### Comparing `PyQCAMS-1.0.0/pyqcams/util.py` & `PyQCAMS-1.0.1/pyqcams/util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import numpy as np
+import os
 import warnings
+import numpy as np
 from scipy.optimize import fsolve
-import matplotlib.pyplot as plt
-import multiprocess as mp 
+from scipy.interpolate import InterpolatedUnivariateSpline
 import pandas as pd
-from . import pymar
-from .constants import *
-import os 
+from pyqcams import constants
 
 def gaus(vp , vt, s=0.1):
             ''' Gaussian function used for Gaussian Binning of final vibrational states.
             Inputs:
             vp, float
                 vPrime output, some number between integers
             vt, int
@@ -47,119 +45,98 @@
 
 
 def get_results(a):
     '''Get long output from trajectory
     a, object
         trajectory object containing relevant attributes
     '''
-    results = {'e': a.e0/cEK2H,
-            'b': a.b,
-            'q': a.count[0],
-            'r1': a.count[1],
-            'r2': a.count[2],
-            'diss': a.count[3],
-            'comp': a.count[4],
-            'v': a.f_state[0],
-            'w': a.f_state[1],
-            'j': a.f_state[2],
-            'd_i': a.d,
-            'theta': a.ang[0], 
+    results = {'e': a.e0/constants.cEK2H, # energy
+            'b': a.b, # impact param   
+            'q': a.count[0], # quench
+            'r1': a.count[1], # reaction 1
+            'r2': a.count[2], # reaction 2
+            'diss': a.count[3],  # dissociation
+            'comp': a.count[4], # complex
+            'v': a.f_state[0], # final vib num
+            'w': a.f_state[1], # weight
+            'j': a.f_state[2], # final j
+            'd_i': a.d, # initial distance
+            'theta': a.ang[0], # initial angles
             'phi': a.ang[1], 
             'eta': a.ang[2], 
-            'n_i': a.n_vib,
-            'j_i': a.j,
-            'rho1x': a.r[0][-1],
+            'n_i': a.n_vib, # initial vib num
+            'j_i': a.j, # initial j 
+            'rho1x': a.r[0][-1], # final positions
             'rho1y': a.r[1][-1],
             'rho1z': a.r[2][-1],
             'rho2x': a.r[0][-1],
             'rho2y': a.r[1][-1],
             'rho2z': a.r[2][-1],
-            'p1x': a.f_p[0],
+            'p1x': a.f_p[0], # final momentum 
             'p1y': a.f_p[1],
             'p1z': a.f_p[2],
-            'tf': a.t[-1]}
+            'p2x': a.f_p[3],
+            'p2y': a.f_p[4],
+            'p2z': a.f_p[5],
+            'tf': a.t[-1]} # final time
     
     return results
 
-def save_long(n_traj,cpus,calc,out_file):
-    '''
-    Runs parallel trajectories.
-    Saves a long version of the data; one line per trajectory.
-    Stores all input & output data.
-
-    n_traj, int
-        number of trajectories
-    cpus, int
-        number of cpus for parallel calculation
-    calc, dict
-        output from pymar.start() function
-    out_file, string
-        output file name
-    '''
-    with mp.Pool(processes = cpus) as p:
-        event = [p.apply_async(pymar.main, kwds = (calc)) for i in range(n_traj)]
-        for res in event:
-            df = pd.DataFrame([res.get()])
-            df.to_csv(out_file, mode = 'a', index = False, 
-                    header = os.path.isfile(out_file) == False or os.path.getsize(out_file) == 0)
-    return
-
-def save_short(n_traj,cpus,calc,out_file):
-    '''
-    Runs parallel trajectories.
-    Saves a short version of the data; sums up the counts so one line per (E,b) set.
-    Use this if input data & distributions are not needed.
-
-    Set cpus = 1 for serial calculation.
-
-    n_traj, int
-        number of trajectories
-    cpus, int
-        number of cpus for parallel calculation
-    calc, dict
-        output from pymar.start() function
-    out_file, string
-        output file name
+def numToV(file):
     '''
-    result = []
-    with mp.Pool(processes = cpus) as p:
-        event = [p.apply_async(pymar.main, kwds = (calc)) for i in range(n_traj)]
-        for res in event:
-            result.append(res.get())
-    df = pd.DataFrame(result)
-    counts = df.loc[:,:'comp'].groupby(['e','b']).sum() # sum counts
-    counts.to_csv(out_file, mode = 'a', 
-                  header = os.path.isfile(out_file) == False or os.path.getsize(out_file) == 0)
-    return
+    Convert pdf table to potential function and first derivative.
+    Assumes positions in column 0, energy in column 1.
 
+    Inputs:
 
-def trace(a):
-    '''
-    Make 3-d trace of the trajectory
-    '''
-    # Coordinate transformation
-    m1,m2,m3 = a.m1, a.m2, a.m3
-    r = a.r
-
-    mtot = m1 + m2 + m3
-    c1 = m1/(m1+m2)
-    c2 = m2/(m1+m2)
-    r1 = np.array([-c2*r[i] - m3/mtot*r[i+3] for i in range(0,3)]) #x,y,z for particle 1
-    r2 = np.array([c1*r[i]-m3/mtot*r[i+3] for i in range(0,3)])
-    r3 = np.array([(m1+m2)/mtot*r[i+3] for i in range(0,3)])
-
-
-    ax = plt.axes(projection='3d')
-    ax.plot3D(r1[0], r1[1], r1[2], 'g')
-    ax.plot3D(r2[0], r2[1], r2[2], 'orange')
-    ax.plot3D(r3[0], r3[1], r3[2], 'r')
-    ax.scatter3D(r1[0][0], r1[1][0], r1[2][0],marker = 'o',color = 'g')
-    ax.scatter3D(r2[0][0], r2[1][0], r2[2][0],marker = 'o',color = 'orange')
-    ax.scatter3D(r3[0][0], r3[1][0], r3[2][0],marker = 'o',color = 'r')
-    ax.scatter3D(r1[0][-1], r1[1][-1], r1[2][-1],marker = '^',color = 'g')
-    ax.scatter3D(r2[0][-1], r2[1][-1], r2[2][-1],marker = '^',color = 'orange')
-    ax.scatter3D(r3[0][-1], r3[1][-1], r3[2][-1],marker = '^',color = 'r')
-    ax.set_xlabel('X')
-    ax.set_ylabel('Y')
-    ax.set_zlabel('Z')
-    plt.show()
-    return 
+    file, str
+        path to pdf file
+
+    Outputs:
+    num_x, list
+        x values of potential
+    num_V, function
+        interpolated potential
+    num_dV, function
+        interpolated potential derivative
+    num_re, float
+        equilibrium point (min of potential)
+    '''
+    types = ['.csv','.txt','.dat']
+    split = os.path.splitext(f'{file}')
+    filetype = split[1]
+    if filetype in types:
+        try:
+            # comma separated
+            df = pd.read_csv(f'{file}',header = None)
+            num_x = np.array([float(i) for i in df[0][:].values.tolist()])
+            num_y = np.array([float(i) for i in df[1][:].values.tolist()])
+        except:
+            try:
+                # tab separated
+                df = pd.read_csv(f'{file}',header = None, sep = '\s+')
+                num_x = np.array([float(i) for i in df[0][:].values.tolist()])
+                num_y = np.array([float(i) for i in df[1][:].values.tolist()])
+            except:
+                print('Please use either comma or tab separated data.')
+                quit()
+    else: 
+        print('Please specify filetype. Choose from "csv", "dat", or "txt".')
+    num_y -= num_y[-1] # Shift values to make curve approach 0 by setting final point to 0
+    num_V = InterpolatedUnivariateSpline(num_x,num_y, k = 4, ext = 'raise') # Use k = 4 to find roots of derivative
+    num_dV = num_V.derivative()
+    cr_pts = num_dV.roots()
+    cr_pts = np.append(cr_pts, (num_x[0], num_x[-1]))  # also check the endpoints of the interval
+    cr_vals = num_V(cr_pts)
+    min_index = np.argmin(cr_vals)
+    num_re = cr_pts[min_index] # Equilibrium distance
+    return num_x, num_V, num_dV, num_re
+
+if __name__ == '__main__':
+    import matplotlib.pyplot as plt
+    # num_x, num_V, num_dV, num_re = numToV(r"C:\Users\Rian\Documents\research\jesusgroup\cah_pec\cah_au.txt")
+    num_x, num_V, num_dV, num_re = numToV(r"C:\Users\Rian\Documents\research\jesusgroup\cah_pec\h2_pec.dat")
+    x = np.linspace(min(num_x),max(num_x),500)
+    # plt.scatter(num_x, num_y)
+    plt.plot(x, num_V(x))
+    plt.plot(num_re, num_V(num_re), marker = 'o')
+    plt.show()
```

