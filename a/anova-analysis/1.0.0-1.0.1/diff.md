# Comparing `tmp/anova_analysis-1.0.0.tar.gz` & `tmp/anova_analysis-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anova_analysis-1.0.0.tar", last modified: Sat May 27 13:06:54 2023, max compression
+gzip compressed data, was "anova_analysis-1.0.1.tar", last modified: Sat May 27 13:20:56 2023, max compression
```

## Comparing `anova_analysis-1.0.0.tar` & `anova_analysis-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 13:06:54.079581 anova_analysis-1.0.0/
--rw-rw-rw-   0        0        0     2386 2023-05-27 13:06:54.078503 anova_analysis-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1839 2023-05-27 12:56:48.000000 anova_analysis-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 13:06:54.077504 anova_analysis-1.0.0/anova_analysis.egg-info/
--rw-rw-rw-   0        0        0     2386 2023-05-27 13:06:53.000000 anova_analysis-1.0.0/anova_analysis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-05-27 13:06:53.000000 anova_analysis-1.0.0/anova_analysis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 13:06:53.000000 anova_analysis-1.0.0/anova_analysis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-27 13:06:53.000000 anova_analysis-1.0.0/anova_analysis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 13:06:53.000000 anova_analysis-1.0.0/anova_analysis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 13:06:54.079581 anova_analysis-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1140 2023-05-27 12:56:43.000000 anova_analysis-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 13:20:56.840208 anova_analysis-1.0.1/
+-rw-rw-rw-   0        0        0     2348 2023-05-27 13:20:56.839199 anova_analysis-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1809 2023-05-27 13:20:41.000000 anova_analysis-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 13:20:56.836206 anova_analysis-1.0.1/anova_analysis.egg-info/
+-rw-rw-rw-   0        0        0     2348 2023-05-27 13:20:56.000000 anova_analysis-1.0.1/anova_analysis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-05-27 13:20:56.000000 anova_analysis-1.0.1/anova_analysis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 13:20:56.000000 anova_analysis-1.0.1/anova_analysis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-27 13:20:56.000000 anova_analysis-1.0.1/anova_analysis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 13:20:56.000000 anova_analysis-1.0.1/anova_analysis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 13:20:56.840208 anova_analysis-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1132 2023-05-27 13:20:13.000000 anova_analysis-1.0.1/setup.py
```

### Comparing `anova_analysis-1.0.0/PKG-INFO` & `anova_analysis-1.0.1/anova_analysis.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: anova_analysis
-Version: 1.0.0
+Name: anova-analysis
+Version: 1.0.1
 Summary: A package for performing ANOVA analysis by RBD
-Home-page: https://github.com/Insight-deviler/anova_analysis_package
+Home-page: https://github.com/Insight-deviler/anova_analysis
 Author: ['Sarath S', 'Saranyadevi S']
 Author-email: insightagri10@gmail.com
 License: MIT
 Keywords: python,ANOVA,RBD,analysis of variance
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,30 +19,30 @@
 Currently it can perform RBD analysis only
 
 ## Installation
 
 You can install the package using pip:
 
 ```
-pip install anova_analysis_package
+pip install anova_analysis
 ```
 ## Usage
 
 ```
-from anova_analysis_package.ANOVA_RBD import RBD
+import ANOVA_RBD
 
 #Set the replication, treatment, and file path
 
 replication = 4
 treatment = 23
 file_path = "path/to/excel/file.xlsx"
 
 # Perform ANOVA analysis
 
-RBD(replication, treatment, file_path)
+ANOVA_RBD.RBD(replication, treatment, file_path)
 ```
 ## Features
 
 - Calculates the correction factor, total sum of squares, replication sum of squares, treatment sum of squares, and error sum of squares.
 - Generates an ANOVA table with source, degrees of freedom, sum of squares, mean square, and F-values.
 - Saves the results in a text file for further analysis or reporting.
```

### Comparing `anova_analysis-1.0.0/README.md` & `anova_analysis-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 Currently it can perform RBD analysis only
 
 ## Installation
 
 You can install the package using pip:
 
 ```
-pip install anova_analysis_package
+pip install anova_analysis
 ```
 ## Usage
 
 ```
-from anova_analysis_package.ANOVA_RBD import RBD
+import ANOVA_RBD
 
 #Set the replication, treatment, and file path
 
 replication = 4
 treatment = 23
 file_path = "path/to/excel/file.xlsx"
 
 # Perform ANOVA analysis
 
-RBD(replication, treatment, file_path)
+ANOVA_RBD.RBD(replication, treatment, file_path)
 ```
 ## Features
 
 - Calculates the correction factor, total sum of squares, replication sum of squares, treatment sum of squares, and error sum of squares.
 - Generates an ANOVA table with source, degrees of freedom, sum of squares, mean square, and F-values.
 - Saves the results in a text file for further analysis or reporting.
```

### Comparing `anova_analysis-1.0.0/anova_analysis.egg-info/PKG-INFO` & `anova_analysis-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: anova-analysis
-Version: 1.0.0
+Name: anova_analysis
+Version: 1.0.1
 Summary: A package for performing ANOVA analysis by RBD
-Home-page: https://github.com/Insight-deviler/anova_analysis_package
+Home-page: https://github.com/Insight-deviler/anova_analysis
 Author: ['Sarath S', 'Saranyadevi S']
 Author-email: insightagri10@gmail.com
 License: MIT
 Keywords: python,ANOVA,RBD,analysis of variance
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,30 +19,30 @@
 Currently it can perform RBD analysis only
 
 ## Installation
 
 You can install the package using pip:
 
 ```
-pip install anova_analysis_package
+pip install anova_analysis
 ```
 ## Usage
 
 ```
-from anova_analysis_package.ANOVA_RBD import RBD
+import ANOVA_RBD
 
 #Set the replication, treatment, and file path
 
 replication = 4
 treatment = 23
 file_path = "path/to/excel/file.xlsx"
 
 # Perform ANOVA analysis
 
-RBD(replication, treatment, file_path)
+ANOVA_RBD.RBD(replication, treatment, file_path)
 ```
 ## Features
 
 - Calculates the correction factor, total sum of squares, replication sum of squares, treatment sum of squares, and error sum of squares.
 - Generates an ANOVA table with source, degrees of freedom, sum of squares, mean square, and F-values.
 - Saves the results in a text file for further analysis or reporting.
```

### Comparing `anova_analysis-1.0.0/setup.py` & `anova_analysis-1.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     LONG_DESCRIPTION = fh.read()
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="anova_analysis", 
-        version="1.0.0",
+        version="1.0.1",
         author=["Sarath S","Saranyadevi S"],
         author_email="insightagri10@gmail.com",
         description="A package for performing ANOVA analysis by RBD",
         license='MIT',
         long_description=LONG_DESCRIPTION,
         long_description_content_type="text/markdown",
         packages=find_packages(),
-        url="https://github.com/Insight-deviler/anova_analysis_package",
+        url="https://github.com/Insight-deviler/anova_analysis",
         install_requires=["tabulate", "pandas"], # add any additional packages that 
         # needs to be installed along with your package. Eg: 'caer'
         
         keywords=['python', 'ANOVA', 'RBD', 'analysis of variance'],
         classifiers= [
              "Programming Language :: Python :: 3",
              "License :: OSI Approved :: MIT License",
```

