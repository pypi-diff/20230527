# Comparing `tmp/ExPSO-0.1.1.tar.gz` & `tmp/ExPSO-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ExPSO-0.1.1.tar", last modified: Sat May 27 07:35:15 2023, max compression
+gzip compressed data, was "ExPSO-0.1.2.tar", last modified: Sat May 27 08:31:50 2023, max compression
```

## Comparing `ExPSO-0.1.1.tar` & `ExPSO-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 07:35:15.337696 ExPSO-0.1.1/
--rw-rw-rw-   0        0        0    35560 2023-05-07 11:50:19.000000 ExPSO-0.1.1/LICENSE
--rw-rw-rw-   0        0        0    16539 2023-05-27 07:35:15.335695 ExPSO-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0    15676 2023-05-27 07:32:24.000000 ExPSO-0.1.1/README.md
--rw-rw-rw-   0        0        0     1041 2023-05-27 07:32:07.000000 ExPSO-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 07:35:15.337696 ExPSO-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 07:35:15.274618 ExPSO-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 07:35:15.317681 ExPSO-0.1.1/src/ExPSO/
--rw-rw-rw-   0        0        0     9942 2023-05-27 07:08:41.000000 ExPSO-0.1.1/src/ExPSO/ExPSOClass.py
--rw-rw-rw-   0        0        0      124 2023-05-07 10:18:51.000000 ExPSO-0.1.1/src/ExPSO/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 07:35:15.331693 ExPSO-0.1.1/src/ExPSO.egg-info/
--rw-rw-rw-   0        0        0    16539 2023-05-27 07:35:15.000000 ExPSO-0.1.1/src/ExPSO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-05-27 07:35:15.000000 ExPSO-0.1.1/src/ExPSO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 07:35:15.000000 ExPSO-0.1.1/src/ExPSO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-27 07:35:15.000000 ExPSO-0.1.1/src/ExPSO.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-27 08:31:50.475324 ExPSO-0.1.2/
+-rw-rw-rw-   0        0        0    35560 2023-05-07 11:50:19.000000 ExPSO-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0    16972 2023-05-27 08:31:50.471318 ExPSO-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0    16109 2023-05-27 08:27:33.000000 ExPSO-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1041 2023-05-27 08:27:20.000000 ExPSO-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 08:31:50.479328 ExPSO-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 08:31:50.338223 ExPSO-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-27 08:31:50.373248 ExPSO-0.1.2/src/ExPSO/
+-rw-rw-rw-   0        0        0     9942 2023-05-27 07:08:41.000000 ExPSO-0.1.2/src/ExPSO/ExPSOClass.py
+-rw-rw-rw-   0        0        0      124 2023-05-07 10:18:51.000000 ExPSO-0.1.2/src/ExPSO/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 08:31:50.459310 ExPSO-0.1.2/src/ExPSO.egg-info/
+-rw-rw-rw-   0        0        0    16972 2023-05-27 08:31:50.000000 ExPSO-0.1.2/src/ExPSO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-05-27 08:31:50.000000 ExPSO-0.1.2/src/ExPSO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 08:31:50.000000 ExPSO-0.1.2/src/ExPSO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-27 08:31:50.000000 ExPSO-0.1.2/src/ExPSO.egg-info/top_level.txt
```

### Comparing `ExPSO-0.1.1/LICENSE` & `ExPSO-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ExPSO-0.1.1/PKG-INFO` & `ExPSO-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,53 @@
 Metadata-Version: 2.1
 Name: ExPSO
-Version: 0.1.1
+Version: 0.1.2
 Summary: The Exponential Particle Swarm Optimization (ExPSO) is a Python library that implements an extended variant of the Particle Swarm Optimization (PSO) algorithm. 
 Author-email: Insaf Kraidia <insaf.kraidia@univ-constantine2.dz>, Khelil Kassoul <khelil.kassoul@etu.unige.ch>, Samir Brahim Belhaouari <sbelhaouari@hbku.edu.qa>, Naoufel Cheikhrouhou <naoufel.cheikhrouhou@hesge.ch>, Nicolas Zufferey <nicolas.zufferey.1@ulaval.ca>
 Project-URL: Homepage, https://github.com/insafkraidia/ExPSO.git
 Project-URL: Bug Tracker, https://github.com/insafkraidia/ExPSO.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Welcome to pspso's documentation!
-
 # Exponential Particle Swarm Optimization for Global Optimization (ExPSO)
 
-<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/05.png?raw=true"> </p>
+<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/06.png?raw=true"> </p>
 
 The ExPSO package is a Python library that includes an algorithm designed to optimize machine and deep learning parameters/hyperparameters. The algorithm divides the swarm population into three subpopulations and utilizes a search strategy based on an exponential function, allowing particles to make large leaps in the search space. It also adapts the control of the velocity range of each particle to balance the exploration and exploitation search phases. The leaping strategy is integrated into the velocity equation, and a new linearly decreasing cognitive parameter is included in the proposed method, along with a dynamic inertia weight strategy. The algorithm is designed to make large jumps at the beginning of the search and then small jumps for further improvements in specific regions of the solution search space. To obtain further information, we recommend referring to the journal paper available at [Exponential Particle Swarm Optimization for Global Optimization (ExPSO)](https://ieeexplore.ieee.org/document/9837898/).
 
 ## Table of content
 
-| Section                                | Description                                                            |
-| -------------------------------------- | ---------------------------------------------------------------------- |
-| [Installation](#installation)          | Installing the dependencies and ExPSO                                  |
-| [Getting started](#requirements)       | Packages necessary to work with ExPSO                                  |
-| [Available parameters](#parameters)    | Modifiable parameters in API with their possible values                |
-| [Usage](#usage)                        | Usage example data                                                     |
-| [Examples with public data](#examples) | Different examples for API                                             |
-| [Results](#results)                    | Comparative study between ExPSO and PSO for CNN,LSTM, XLNET,MLP models |
-| [References](#reference)               | References to cite                                                     |
-| [License](#license)                    | Package license                                                        |
+| Section                                | Description                                                                              |
+| -------------------------------------- | ---------------------------------------------------------------------------------------- |
+| [Installation](#installation)          | Installing the dependencies and ExPSO                                                    |
+| [Getting started](#requirements)       | Packages necessary to work with ExPSO                                                    |
+| [Available parameters](#parameters)    | Modifiable parameters in API with their possible values                                  |
+| [Usage](#usage)                        | Usage example data                                                                       |
+| [Examples with public data](#examples) | Different examples for API                                                               |
+| [Results](#results)                    | Comparative study between ExPSO and other variants of PSO for CNN,LSTM, XLNET,MLP models |
+| [References](#reference)               | References to cite                                                                       |
+| [License](#license)                    | Package license                                                                          |
 
 ## Flowchart of the proposed ExPSO
 
 <p align="center" style="max-width: 100%;height: 900px;width: 600px;"> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/01.png?raw=true"> </p>
 
 ## Installation
 
 ExPSO can be installed using [pip](https://pip.pypa.io/en/stable/), a tool
 for installing Python packages. To do it, run the following command:
 
 ```
 pip install ExPSO
 ```
 
-**Current version:** 0.1.1
-
 ## Requirements
 
 ExPSO requires Python >= 3.6.1 or later to run. For other Python
 dependencies, please check the `pyproject.toml` file included
 on this repository.
 
 Note that you should have also the following packages installed in your system:
@@ -61,28 +57,28 @@
 - math
 - tensorflow
 - keras
 - scikit-learn
 
 ## Parameters
 
-| Parameter name                    | Parameter description                                                                                                                                                                                                                    | Possible values |
-| --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------- |
-| Objective function(ObjFunction)   | This is the function that the algorithm will attempt to optimize. It is the main goal of the algorithm and is determined by the user based on the problem they are trying to solve.                                                      | List of floats  |
-| Dimensions (D)                    | This parameter refers to the number of variables or features that are present in the objective function. It is important to correctly specify the dimension in order to achieve accurate optimization.                                   | Integer         |
-| Number of particles (nPop)        | This refers to the number of agents or particles that will be used to search the solution space. Increasing the number of particles can help to find better solutions, but it also increases the computational cost.                     | Integer         |
-| Maximum iteration numbers (MaxIt) | This parameter specifies the maximum number of iterations that the algorithm will perform before terminating. The number of iterations can help to obtain a more accurate solution and reduce the risk of finding a suboptimal solution. | Integer         |
-| Upper and lower bounds (ub,lb)    | These are the maximum and the lowest value in the search space                                                                                                                                                                           | Float           |
-| Number of runs (runs)             | This parameter refers to the number of times the algorithm will be run with the same parameters.                                                                                                                                         | Integer         |
+| Parameter name                    | Parameter description                                                                                                                                                                                                                    | Possible values                        |
+| --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------- |
+| Objective function (ObjFunction)  | This is the function that the algorithm will attempt to optimize. It is the main goal of the algorithm and is determined by the user based on the problem they are trying to solve.                                                      | Function with list of floats as inputs |
+| Dimensions (D)                    | This parameter refers to the number of variables or features that are present in the objective function. It is important to correctly specify the dimension in order to achieve accurate optimization.                                   | Integer                                |
+| Number of particles (nPop)        | This refers to the number of agents or particles that will be used to search the solution space. Increasing the number of particles can help to find better solutions, but it also increases the computational cost.                     | Integer                                |
+| Maximum iteration numbers (MaxIt) | This parameter specifies the maximum number of iterations that the algorithm will perform before terminating. The number of iterations can help to obtain a more accurate solution and reduce the risk of finding a suboptimal solution. | Integer                                |
+| Upper and lower bounds (ub,lb)    | These are the maximum and the lowest value in the search space                                                                                                                                                                           | Float                                  |
+| Number of runs (runs)             | This parameter refers to the number of times the algorithm will be run with the same parameters.                                                                                                                                         | Integer                                |
 
 ## Usage
 
-Below is an example for using the ExPSO package.
+Here is a sample guide outlining the procedure for utilizing the ExPSO package:
 
-1. Import the ExPSO class
+1. Import the ExPSO class.
 
 ```
 from ExPSO import ExPSOClass
 ```
 
 2. Define the objective function.
 
@@ -94,21 +90,30 @@
 
 3. Create an instance of the ExPSO class from the ExPSO package with specified parameters, including the objective function, dimensionality (D), population size (nPop), maximum iterations (MaxIt), lower bounds (lb), upper bounds (ub), and number of runs (runs).
 
 ```
 expso = ExPSOClass.ExponentialParticleSwarmOptimizer(ObjFunction, D=D, nPop=nPop, MaxIt=MaxIt, lb=lb, ub=ub, runs=runs)
 ```
 
-4. The ExPSO algorithm is then used to optimize the objective function
+4. Execute the optimization process by employing the optimize() function.
 
 ```
 best_solution = expso.optimize()
 ```
 
-<a name="item1"></a>
+Note: The result of this function is an object that can be accessed by the user, containing multiple items arranged in the following manner.
+
+- GlobalBestCost: It represents the optimal or near-optimal value achieved by the ExPSO algorithm.
+- GlobalBestPosition: It represents the optimal or near-optimal solution obtained by the ExPSO algorithm in the search space.
+- MEAN: It represents the average value of the best cost found across multiple optimization runs.
+- WorstSol: It refers to the highest value of the best cost found during the optimization process. It helps evaluate the quality of the obtained solutions and identify the worst-performing solution.
+- BestSol: It refers to the lowest value of the best cost found during the optimization process.
+- STD (Standard Deviation): It refers to the standard deviation, which is often used to assess the diversity or convergence of the obtained solutions.
+- Avg_FES (Average Function Evaluations): It represents the average number of function evaluations performed during the optimization process.
+  <a name="item1"></a>
 
 ## Examples
 
 ### Experiment 1. ExPSO with rosenbrock function
 
 <p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/10.png?raw=true"> </p>
 
@@ -139,22 +144,14 @@
         -3.16572820e+00, -1.23867646e+01, -2.06098389e+01,
          1.86093654e+00,  1.71640639e+01,  1.89470347e+01,
          .................................................]]),
 'Metrics': {'ExPSO': array([0., 0., 0., ..., 0., 0., 0.]),
  'MEAN': 0.0, 'WorstSol': 0.0, 'BestSol': 0.0, 'STD': 0.0, 'Avg_FES': 0.033296337402885685}}
 ```
 
-- GlobalBestCost: It represents the optimal or near-optimal value achieved by the ExPSO algorithm.
-- GlobalBestPosition: It represents the optimal or near-optimal solution obtained by the ExPSO algorithm in the search space.
-- MEAN: It represents the average value of the best cost found across multiple optimization runs.
-- WorstSol: It refers to the highest value of the best cost found during the optimization process. It helps evaluate the quality of the obtained solutions and identify the worst-performing solution.
-- BestSol: It refers to the lowest value of the best cost found during the optimization process.
-- STD (Standard Deviation): It refers to the standard deviation, which is often used to assess the diversity or convergence of the obtained solutions.
-- Avg_FES (Average Function Evaluations): It represents the average number of function evaluations performed during the optimization process.
-
 ### Experiment 2. ExPSO with ackley function
 
 <p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/08.png?raw=true"> </p>
 
 The following example demonstrates the optimization process of ExPSO using the ackley function:
 
 ```
@@ -270,16 +267,15 @@
 def ObjFunction(particles):
     allLosses = mlp(particleDimensions=particles, x_train=x_train, x_test=x_test,
                         y_train=y_train, y_test=y_test)
 
     return allLosses
 
 def main():
-    opt = -4.189829e+05
-    thrshold = 1
+
     nPop = 30
     runs = 10
     lb = 1
     ub = 500
     D = 2
     MaxIt = 100
     # create an instance of the ExPSOClass class with the specified parameters
```

### Comparing `ExPSO-0.1.1/README.md` & `ExPSO-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,39 @@
-# Welcome to pspso's documentation!
-
 # Exponential Particle Swarm Optimization for Global Optimization (ExPSO)
 
-<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/05.png?raw=true"> </p>
+<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/06.png?raw=true"> </p>
 
 The ExPSO package is a Python library that includes an algorithm designed to optimize machine and deep learning parameters/hyperparameters. The algorithm divides the swarm population into three subpopulations and utilizes a search strategy based on an exponential function, allowing particles to make large leaps in the search space. It also adapts the control of the velocity range of each particle to balance the exploration and exploitation search phases. The leaping strategy is integrated into the velocity equation, and a new linearly decreasing cognitive parameter is included in the proposed method, along with a dynamic inertia weight strategy. The algorithm is designed to make large jumps at the beginning of the search and then small jumps for further improvements in specific regions of the solution search space. To obtain further information, we recommend referring to the journal paper available at [Exponential Particle Swarm Optimization for Global Optimization (ExPSO)](https://ieeexplore.ieee.org/document/9837898/).
 
 ## Table of content
 
-| Section                                | Description                                                            |
-| -------------------------------------- | ---------------------------------------------------------------------- |
-| [Installation](#installation)          | Installing the dependencies and ExPSO                                  |
-| [Getting started](#requirements)       | Packages necessary to work with ExPSO                                  |
-| [Available parameters](#parameters)    | Modifiable parameters in API with their possible values                |
-| [Usage](#usage)                        | Usage example data                                                     |
-| [Examples with public data](#examples) | Different examples for API                                             |
-| [Results](#results)                    | Comparative study between ExPSO and PSO for CNN,LSTM, XLNET,MLP models |
-| [References](#reference)               | References to cite                                                     |
-| [License](#license)                    | Package license                                                        |
+| Section                                | Description                                                                              |
+| -------------------------------------- | ---------------------------------------------------------------------------------------- |
+| [Installation](#installation)          | Installing the dependencies and ExPSO                                                    |
+| [Getting started](#requirements)       | Packages necessary to work with ExPSO                                                    |
+| [Available parameters](#parameters)    | Modifiable parameters in API with their possible values                                  |
+| [Usage](#usage)                        | Usage example data                                                                       |
+| [Examples with public data](#examples) | Different examples for API                                                               |
+| [Results](#results)                    | Comparative study between ExPSO and other variants of PSO for CNN,LSTM, XLNET,MLP models |
+| [References](#reference)               | References to cite                                                                       |
+| [License](#license)                    | Package license                                                                          |
 
 ## Flowchart of the proposed ExPSO
 
 <p align="center" style="max-width: 100%;height: 900px;width: 600px;"> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/01.png?raw=true"> </p>
 
 ## Installation
 
 ExPSO can be installed using [pip](https://pip.pypa.io/en/stable/), a tool
 for installing Python packages. To do it, run the following command:
 
 ```
 pip install ExPSO
 ```
 
-**Current version:** 0.1.1
-
 ## Requirements
 
 ExPSO requires Python >= 3.6.1 or later to run. For other Python
 dependencies, please check the `pyproject.toml` file included
 on this repository.
 
 Note that you should have also the following packages installed in your system:
@@ -47,28 +43,28 @@
 - math
 - tensorflow
 - keras
 - scikit-learn
 
 ## Parameters
 
-| Parameter name                    | Parameter description                                                                                                                                                                                                                    | Possible values |
-| --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------- |
-| Objective function(ObjFunction)   | This is the function that the algorithm will attempt to optimize. It is the main goal of the algorithm and is determined by the user based on the problem they are trying to solve.                                                      | List of floats  |
-| Dimensions (D)                    | This parameter refers to the number of variables or features that are present in the objective function. It is important to correctly specify the dimension in order to achieve accurate optimization.                                   | Integer         |
-| Number of particles (nPop)        | This refers to the number of agents or particles that will be used to search the solution space. Increasing the number of particles can help to find better solutions, but it also increases the computational cost.                     | Integer         |
-| Maximum iteration numbers (MaxIt) | This parameter specifies the maximum number of iterations that the algorithm will perform before terminating. The number of iterations can help to obtain a more accurate solution and reduce the risk of finding a suboptimal solution. | Integer         |
-| Upper and lower bounds (ub,lb)    | These are the maximum and the lowest value in the search space                                                                                                                                                                           | Float           |
-| Number of runs (runs)             | This parameter refers to the number of times the algorithm will be run with the same parameters.                                                                                                                                         | Integer         |
+| Parameter name                    | Parameter description                                                                                                                                                                                                                    | Possible values                        |
+| --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------- |
+| Objective function (ObjFunction)  | This is the function that the algorithm will attempt to optimize. It is the main goal of the algorithm and is determined by the user based on the problem they are trying to solve.                                                      | Function with list of floats as inputs |
+| Dimensions (D)                    | This parameter refers to the number of variables or features that are present in the objective function. It is important to correctly specify the dimension in order to achieve accurate optimization.                                   | Integer                                |
+| Number of particles (nPop)        | This refers to the number of agents or particles that will be used to search the solution space. Increasing the number of particles can help to find better solutions, but it also increases the computational cost.                     | Integer                                |
+| Maximum iteration numbers (MaxIt) | This parameter specifies the maximum number of iterations that the algorithm will perform before terminating. The number of iterations can help to obtain a more accurate solution and reduce the risk of finding a suboptimal solution. | Integer                                |
+| Upper and lower bounds (ub,lb)    | These are the maximum and the lowest value in the search space                                                                                                                                                                           | Float                                  |
+| Number of runs (runs)             | This parameter refers to the number of times the algorithm will be run with the same parameters.                                                                                                                                         | Integer                                |
 
 ## Usage
 
-Below is an example for using the ExPSO package.
+Here is a sample guide outlining the procedure for utilizing the ExPSO package:
 
-1. Import the ExPSO class
+1. Import the ExPSO class.
 
 ```
 from ExPSO import ExPSOClass
 ```
 
 2. Define the objective function.
 
@@ -80,21 +76,30 @@
 
 3. Create an instance of the ExPSO class from the ExPSO package with specified parameters, including the objective function, dimensionality (D), population size (nPop), maximum iterations (MaxIt), lower bounds (lb), upper bounds (ub), and number of runs (runs).
 
 ```
 expso = ExPSOClass.ExponentialParticleSwarmOptimizer(ObjFunction, D=D, nPop=nPop, MaxIt=MaxIt, lb=lb, ub=ub, runs=runs)
 ```
 
-4. The ExPSO algorithm is then used to optimize the objective function
+4. Execute the optimization process by employing the optimize() function.
 
 ```
 best_solution = expso.optimize()
 ```
 
-<a name="item1"></a>
+Note: The result of this function is an object that can be accessed by the user, containing multiple items arranged in the following manner.
+
+- GlobalBestCost: It represents the optimal or near-optimal value achieved by the ExPSO algorithm.
+- GlobalBestPosition: It represents the optimal or near-optimal solution obtained by the ExPSO algorithm in the search space.
+- MEAN: It represents the average value of the best cost found across multiple optimization runs.
+- WorstSol: It refers to the highest value of the best cost found during the optimization process. It helps evaluate the quality of the obtained solutions and identify the worst-performing solution.
+- BestSol: It refers to the lowest value of the best cost found during the optimization process.
+- STD (Standard Deviation): It refers to the standard deviation, which is often used to assess the diversity or convergence of the obtained solutions.
+- Avg_FES (Average Function Evaluations): It represents the average number of function evaluations performed during the optimization process.
+  <a name="item1"></a>
 
 ## Examples
 
 ### Experiment 1. ExPSO with rosenbrock function
 
 <p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/10.png?raw=true"> </p>
 
@@ -125,22 +130,14 @@
         -3.16572820e+00, -1.23867646e+01, -2.06098389e+01,
          1.86093654e+00,  1.71640639e+01,  1.89470347e+01,
          .................................................]]),
 'Metrics': {'ExPSO': array([0., 0., 0., ..., 0., 0., 0.]),
  'MEAN': 0.0, 'WorstSol': 0.0, 'BestSol': 0.0, 'STD': 0.0, 'Avg_FES': 0.033296337402885685}}
 ```
 
-- GlobalBestCost: It represents the optimal or near-optimal value achieved by the ExPSO algorithm.
-- GlobalBestPosition: It represents the optimal or near-optimal solution obtained by the ExPSO algorithm in the search space.
-- MEAN: It represents the average value of the best cost found across multiple optimization runs.
-- WorstSol: It refers to the highest value of the best cost found during the optimization process. It helps evaluate the quality of the obtained solutions and identify the worst-performing solution.
-- BestSol: It refers to the lowest value of the best cost found during the optimization process.
-- STD (Standard Deviation): It refers to the standard deviation, which is often used to assess the diversity or convergence of the obtained solutions.
-- Avg_FES (Average Function Evaluations): It represents the average number of function evaluations performed during the optimization process.
-
 ### Experiment 2. ExPSO with ackley function
 
 <p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/08.png?raw=true"> </p>
 
 The following example demonstrates the optimization process of ExPSO using the ackley function:
 
 ```
@@ -256,16 +253,15 @@
 def ObjFunction(particles):
     allLosses = mlp(particleDimensions=particles, x_train=x_train, x_test=x_test,
                         y_train=y_train, y_test=y_test)
 
     return allLosses
 
 def main():
-    opt = -4.189829e+05
-    thrshold = 1
+
     nPop = 30
     runs = 10
     lb = 1
     ub = 500
     D = 2
     MaxIt = 100
     # create an instance of the ExPSOClass class with the specified parameters
```

### Comparing `ExPSO-0.1.1/pyproject.toml` & `ExPSO-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   "scikit-learn"
 ]
 
 
 
 [project]
 name = "ExPSO"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Insaf Kraidia", email="insaf.kraidia@univ-constantine2.dz" },
   { name="Khelil Kassoul", email="khelil.kassoul@etu.unige.ch" },
   { name="Samir Brahim Belhaouari", email="sbelhaouari@hbku.edu.qa" },
   { name="Naoufel Cheikhrouhou",email="naoufel.cheikhrouhou@hesge.ch"},
   { name="Nicolas Zufferey",email="nicolas.zufferey.1@ulaval.ca"}
```

### Comparing `ExPSO-0.1.1/src/ExPSO/ExPSOClass.py` & `ExPSO-0.1.2/src/ExPSO/ExPSOClass.py`

 * *Files identical despite different names*

### Comparing `ExPSO-0.1.1/src/ExPSO.egg-info/PKG-INFO` & `ExPSO-0.1.2/src/ExPSO.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,53 @@
 Metadata-Version: 2.1
 Name: ExPSO
-Version: 0.1.1
+Version: 0.1.2
 Summary: The Exponential Particle Swarm Optimization (ExPSO) is a Python library that implements an extended variant of the Particle Swarm Optimization (PSO) algorithm. 
 Author-email: Insaf Kraidia <insaf.kraidia@univ-constantine2.dz>, Khelil Kassoul <khelil.kassoul@etu.unige.ch>, Samir Brahim Belhaouari <sbelhaouari@hbku.edu.qa>, Naoufel Cheikhrouhou <naoufel.cheikhrouhou@hesge.ch>, Nicolas Zufferey <nicolas.zufferey.1@ulaval.ca>
 Project-URL: Homepage, https://github.com/insafkraidia/ExPSO.git
 Project-URL: Bug Tracker, https://github.com/insafkraidia/ExPSO.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Welcome to pspso's documentation!
-
 # Exponential Particle Swarm Optimization for Global Optimization (ExPSO)
 
-<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/05.png?raw=true"> </p>
+<p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/06.png?raw=true"> </p>
 
 The ExPSO package is a Python library that includes an algorithm designed to optimize machine and deep learning parameters/hyperparameters. The algorithm divides the swarm population into three subpopulations and utilizes a search strategy based on an exponential function, allowing particles to make large leaps in the search space. It also adapts the control of the velocity range of each particle to balance the exploration and exploitation search phases. The leaping strategy is integrated into the velocity equation, and a new linearly decreasing cognitive parameter is included in the proposed method, along with a dynamic inertia weight strategy. The algorithm is designed to make large jumps at the beginning of the search and then small jumps for further improvements in specific regions of the solution search space. To obtain further information, we recommend referring to the journal paper available at [Exponential Particle Swarm Optimization for Global Optimization (ExPSO)](https://ieeexplore.ieee.org/document/9837898/).
 
 ## Table of content
 
-| Section                                | Description                                                            |
-| -------------------------------------- | ---------------------------------------------------------------------- |
-| [Installation](#installation)          | Installing the dependencies and ExPSO                                  |
-| [Getting started](#requirements)       | Packages necessary to work with ExPSO                                  |
-| [Available parameters](#parameters)    | Modifiable parameters in API with their possible values                |
-| [Usage](#usage)                        | Usage example data                                                     |
-| [Examples with public data](#examples) | Different examples for API                                             |
-| [Results](#results)                    | Comparative study between ExPSO and PSO for CNN,LSTM, XLNET,MLP models |
-| [References](#reference)               | References to cite                                                     |
-| [License](#license)                    | Package license                                                        |
+| Section                                | Description                                                                              |
+| -------------------------------------- | ---------------------------------------------------------------------------------------- |
+| [Installation](#installation)          | Installing the dependencies and ExPSO                                                    |
+| [Getting started](#requirements)       | Packages necessary to work with ExPSO                                                    |
+| [Available parameters](#parameters)    | Modifiable parameters in API with their possible values                                  |
+| [Usage](#usage)                        | Usage example data                                                                       |
+| [Examples with public data](#examples) | Different examples for API                                                               |
+| [Results](#results)                    | Comparative study between ExPSO and other variants of PSO for CNN,LSTM, XLNET,MLP models |
+| [References](#reference)               | References to cite                                                                       |
+| [License](#license)                    | Package license                                                                          |
 
 ## Flowchart of the proposed ExPSO
 
 <p align="center" style="max-width: 100%;height: 900px;width: 600px;"> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/01.png?raw=true"> </p>
 
 ## Installation
 
 ExPSO can be installed using [pip](https://pip.pypa.io/en/stable/), a tool
 for installing Python packages. To do it, run the following command:
 
 ```
 pip install ExPSO
 ```
 
-**Current version:** 0.1.1
-
 ## Requirements
 
 ExPSO requires Python >= 3.6.1 or later to run. For other Python
 dependencies, please check the `pyproject.toml` file included
 on this repository.
 
 Note that you should have also the following packages installed in your system:
@@ -61,28 +57,28 @@
 - math
 - tensorflow
 - keras
 - scikit-learn
 
 ## Parameters
 
-| Parameter name                    | Parameter description                                                                                                                                                                                                                    | Possible values |
-| --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------- |
-| Objective function(ObjFunction)   | This is the function that the algorithm will attempt to optimize. It is the main goal of the algorithm and is determined by the user based on the problem they are trying to solve.                                                      | List of floats  |
-| Dimensions (D)                    | This parameter refers to the number of variables or features that are present in the objective function. It is important to correctly specify the dimension in order to achieve accurate optimization.                                   | Integer         |
-| Number of particles (nPop)        | This refers to the number of agents or particles that will be used to search the solution space. Increasing the number of particles can help to find better solutions, but it also increases the computational cost.                     | Integer         |
-| Maximum iteration numbers (MaxIt) | This parameter specifies the maximum number of iterations that the algorithm will perform before terminating. The number of iterations can help to obtain a more accurate solution and reduce the risk of finding a suboptimal solution. | Integer         |
-| Upper and lower bounds (ub,lb)    | These are the maximum and the lowest value in the search space                                                                                                                                                                           | Float           |
-| Number of runs (runs)             | This parameter refers to the number of times the algorithm will be run with the same parameters.                                                                                                                                         | Integer         |
+| Parameter name                    | Parameter description                                                                                                                                                                                                                    | Possible values                        |
+| --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------- |
+| Objective function (ObjFunction)  | This is the function that the algorithm will attempt to optimize. It is the main goal of the algorithm and is determined by the user based on the problem they are trying to solve.                                                      | Function with list of floats as inputs |
+| Dimensions (D)                    | This parameter refers to the number of variables or features that are present in the objective function. It is important to correctly specify the dimension in order to achieve accurate optimization.                                   | Integer                                |
+| Number of particles (nPop)        | This refers to the number of agents or particles that will be used to search the solution space. Increasing the number of particles can help to find better solutions, but it also increases the computational cost.                     | Integer                                |
+| Maximum iteration numbers (MaxIt) | This parameter specifies the maximum number of iterations that the algorithm will perform before terminating. The number of iterations can help to obtain a more accurate solution and reduce the risk of finding a suboptimal solution. | Integer                                |
+| Upper and lower bounds (ub,lb)    | These are the maximum and the lowest value in the search space                                                                                                                                                                           | Float                                  |
+| Number of runs (runs)             | This parameter refers to the number of times the algorithm will be run with the same parameters.                                                                                                                                         | Integer                                |
 
 ## Usage
 
-Below is an example for using the ExPSO package.
+Here is a sample guide outlining the procedure for utilizing the ExPSO package:
 
-1. Import the ExPSO class
+1. Import the ExPSO class.
 
 ```
 from ExPSO import ExPSOClass
 ```
 
 2. Define the objective function.
 
@@ -94,21 +90,30 @@
 
 3. Create an instance of the ExPSO class from the ExPSO package with specified parameters, including the objective function, dimensionality (D), population size (nPop), maximum iterations (MaxIt), lower bounds (lb), upper bounds (ub), and number of runs (runs).
 
 ```
 expso = ExPSOClass.ExponentialParticleSwarmOptimizer(ObjFunction, D=D, nPop=nPop, MaxIt=MaxIt, lb=lb, ub=ub, runs=runs)
 ```
 
-4. The ExPSO algorithm is then used to optimize the objective function
+4. Execute the optimization process by employing the optimize() function.
 
 ```
 best_solution = expso.optimize()
 ```
 
-<a name="item1"></a>
+Note: The result of this function is an object that can be accessed by the user, containing multiple items arranged in the following manner.
+
+- GlobalBestCost: It represents the optimal or near-optimal value achieved by the ExPSO algorithm.
+- GlobalBestPosition: It represents the optimal or near-optimal solution obtained by the ExPSO algorithm in the search space.
+- MEAN: It represents the average value of the best cost found across multiple optimization runs.
+- WorstSol: It refers to the highest value of the best cost found during the optimization process. It helps evaluate the quality of the obtained solutions and identify the worst-performing solution.
+- BestSol: It refers to the lowest value of the best cost found during the optimization process.
+- STD (Standard Deviation): It refers to the standard deviation, which is often used to assess the diversity or convergence of the obtained solutions.
+- Avg_FES (Average Function Evaluations): It represents the average number of function evaluations performed during the optimization process.
+  <a name="item1"></a>
 
 ## Examples
 
 ### Experiment 1. ExPSO with rosenbrock function
 
 <p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/10.png?raw=true"> </p>
 
@@ -139,22 +144,14 @@
         -3.16572820e+00, -1.23867646e+01, -2.06098389e+01,
          1.86093654e+00,  1.71640639e+01,  1.89470347e+01,
          .................................................]]),
 'Metrics': {'ExPSO': array([0., 0., 0., ..., 0., 0., 0.]),
  'MEAN': 0.0, 'WorstSol': 0.0, 'BestSol': 0.0, 'STD': 0.0, 'Avg_FES': 0.033296337402885685}}
 ```
 
-- GlobalBestCost: It represents the optimal or near-optimal value achieved by the ExPSO algorithm.
-- GlobalBestPosition: It represents the optimal or near-optimal solution obtained by the ExPSO algorithm in the search space.
-- MEAN: It represents the average value of the best cost found across multiple optimization runs.
-- WorstSol: It refers to the highest value of the best cost found during the optimization process. It helps evaluate the quality of the obtained solutions and identify the worst-performing solution.
-- BestSol: It refers to the lowest value of the best cost found during the optimization process.
-- STD (Standard Deviation): It refers to the standard deviation, which is often used to assess the diversity or convergence of the obtained solutions.
-- Avg_FES (Average Function Evaluations): It represents the average number of function evaluations performed during the optimization process.
-
 ### Experiment 2. ExPSO with ackley function
 
 <p align="center" style=""> <img src="https://github.com/insafkraidia/ExPSO/blob/62b69fe475f026dcbab2d5339d8a05ce36b257a9/src/08.png?raw=true"> </p>
 
 The following example demonstrates the optimization process of ExPSO using the ackley function:
 
 ```
@@ -270,16 +267,15 @@
 def ObjFunction(particles):
     allLosses = mlp(particleDimensions=particles, x_train=x_train, x_test=x_test,
                         y_train=y_train, y_test=y_test)
 
     return allLosses
 
 def main():
-    opt = -4.189829e+05
-    thrshold = 1
+
     nPop = 30
     runs = 10
     lb = 1
     ub = 500
     D = 2
     MaxIt = 100
     # create an instance of the ExPSOClass class with the specified parameters
```

