# Comparing `tmp/carpet_concentrations-0.1.0.tar.gz` & `tmp/carpet_concentrations-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carpet_concentrations-0.1.0.tar", max compression
+gzip compressed data, was "carpet_concentrations-0.2.1.tar", max compression
```

## Comparing `carpet_concentrations-0.1.0.tar` & `carpet_concentrations-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,18 @@
--rw-r--r--   0        0        0     1524 2023-05-06 05:09:47.061875 carpet_concentrations-0.1.0/LICENSE
--rw-r--r--   0        0        0     1928 2023-05-27 02:21:43.498896 carpet_concentrations-0.1.0/README.rst
--rw-r--r--   0        0        0     2833 2023-05-27 02:21:43.505320 carpet_concentrations-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      408 2023-05-27 02:21:43.506945 carpet_concentrations-0.1.0/src/carpet_concentrations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 09:51:18.952420 carpet_concentrations-0.1.0/src/carpet_concentrations/py.typed
--rw-r--r--   0        0        0     1454 2023-05-27 02:21:43.507475 carpet_concentrations-0.1.0/src/carpet_concentrations/testing.py
--rw-r--r--   0        0        0     2999 2023-05-27 02:21:43.507737 carpet_concentrations-0.1.0/src/carpet_concentrations/time.py
--rw-r--r--   0        0        0     2670 1970-01-01 00:00:00.000000 carpet_concentrations-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1524 2023-05-22 05:41:30.506818 carpet_concentrations-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2096 2023-05-27 04:14:21.821420 carpet_concentrations-0.2.1/README.md
+-rw-r--r--   0        0        0     3768 2023-05-27 04:37:25.549441 carpet_concentrations-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      199 2023-05-27 02:26:43.018245 carpet_concentrations-0.2.1/src/carpet_concentrations/__init__.py
+-rw-r--r--   0        0        0     2975 2023-05-27 02:26:43.018245 carpet_concentrations-0.2.1/src/carpet_concentrations/attrs_utils.py
+-rw-r--r--   0        0        0     2812 2023-05-27 02:26:43.018245 carpet_concentrations-0.2.1/src/carpet_concentrations/exceptions.py
+-rw-r--r--   0        0        0      139 2023-05-27 02:26:43.018245 carpet_concentrations-0.2.1/src/carpet_concentrations/gridders/__init__.py
+-rw-r--r--   0        0        0     6629 2023-05-27 02:26:43.022245 carpet_concentrations-0.2.1/src/carpet_concentrations/gridders/latitude_seasonality_gridder.py
+-rw-r--r--   0        0        0       94 2023-05-27 02:26:43.022245 carpet_concentrations-0.2.1/src/carpet_concentrations/input4MIPs/__init__.py
+-rw-r--r--   0        0        0    18356 2023-05-27 02:26:43.022245 carpet_concentrations-0.2.1/src/carpet_concentrations/input4MIPs/dataset.py
+-rw-r--r--   0        0        0     1592 2023-05-27 02:26:43.022245 carpet_concentrations-0.2.1/src/carpet_concentrations/input4MIPs/metadata_options.py
+-rw-r--r--   0        0        0        0 2023-05-22 05:41:30.510818 carpet_concentrations-0.2.1/src/carpet_concentrations/py.typed
+-rw-r--r--   0        0        0     1429 2023-05-27 02:26:43.022245 carpet_concentrations-0.2.1/src/carpet_concentrations/testing.py
+-rw-r--r--   0        0        0     4948 2023-05-27 02:26:43.022245 carpet_concentrations-0.2.1/src/carpet_concentrations/time.py
+-rw-r--r--   0        0        0      335 2023-05-27 02:26:43.022245 carpet_concentrations-0.2.1/src/carpet_concentrations/unit_registry.py
+-rw-r--r--   0        0        0     1325 2023-05-27 04:25:46.035362 carpet_concentrations-0.2.1/src/carpet_concentrations/xarray_pint_utils.py
+-rw-r--r--   0        0        0     3591 2023-05-27 02:26:43.022245 carpet_concentrations-0.2.1/src/carpet_concentrations/xarray_utils.py
+-rw-r--r--   0        0        0     3368 1970-01-01 00:00:00.000000 carpet_concentrations-0.2.1/PKG-INFO
```

### Comparing `carpet_concentrations-0.1.0/LICENSE` & `carpet_concentrations-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `carpet_concentrations-0.1.0/README.rst` & `carpet_concentrations-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-.. sec-begin-description
+# Carpet - Concentrations
 
-Carpet - Concentrations
-=======================
+<!--- sec-begin-description -->
 
-[TODO badges here #1]
+[#1 badges here]
 
-Core tools for the development of greenhouse gas concentration input files (i.e.
-flying carpets).
+Core tools for the development of greenhouse gas concentration input files (i.e. flying carpets).
 
-Full documentation can be found at: [TODO read the docs link here #2]
+<!---
+Can use start-after and end-before directives in docs, see
+https://myst-parser.readthedocs.io/en/latest/syntax/organising_content.html#inserting-other-documents-directly-into-the-current-document
+-->
 
-.. sec-begin-links
+<!--- sec-end-description -->
 
-.. _issue tracker: https://gitlab.com/climate-resource/carpet-concentrations/-/issues
+Full documentation can be found at: [#2 read the docs link here]
 
-.. sec-end-links
+## Installation
 
-.. sec-end-description
+<!--- sec-begin-installation -->
 
-Installation
-------------
+Carpet - Concentrations can be installed with conda or pip:
 
-Carpet - concentrations can be installed with conda or pip:
-
-.. code:: bash
-
-    pip install carpet-concentrations
-    conda install -c conda-forge carpet-concentrations
+```bash
+pip install carpet-concentrations
+conda install -c conda-forge carpet-concentrations
+```
 
 Additional dependencies can be installed using
 
-.. code:: bash
+```bash
+# To add plotting dependencies
+pip install carpet-concentrations[plots]
+# To add notebook dependencies
+pip install carpet-concentrations[notebooks]
 
-    # To add plotting dependencies
-    pip install carpet-concentrations[plots]
-    # To run the notebooks
-    pip install carpet-concentrations[notebooks, plots]
-    # If you are installing with conda, we recommend
-    # installing the extras by hand because there is no stable
-    # solution yet (issue here: https://github.com/conda/conda/issues/7502)
+# If you are installing with conda, we recommend
+# installing the extras by hand because there is no stable
+# solution yet (issue here: https://github.com/conda/conda/issues/7502)
+```
 
-.. sec-end-installation
+<!--- sec-end-installation -->
 
-.. sec-begin-installation-dev
+### For developers
 
-For developers
-~~~~~~~~~~~~~~
+<!--- sec-begin-installation-dev -->
 
-For development, we rely on `poetry <https://python-poetry.org>`_ for all our
+For development, we rely on [poetry](https://python-poetry.org) for all our
 dependency management. To get started, you will need to make sure that poetry
 is installed
-(https://python-poetry.org/docs/#installing-with-the-official-installer, we
-found that pipx and pip worked better to install on a Mac).
+([instructions here](https://python-poetry.org/docs/#installing-with-the-official-installer),
+we found that pipx and pip worked better to install on a Mac).
 
-For all of work, we use our ``Makefile``.
+For all of work, we use our `Makefile`.
 You can read the instructions out and run the commands by hand if you wish,
-but we generally discourage this because it can be error prone and doesn't
-update if dependencies change (e.g. the environment is updated).
-In order to create your environment, run ``make virtual-environment``.
-
-If there are any issues, the messages from the ``Makefile`` should guide you
-through. If not, please raise an issue in the
-`issue tracker`_.
+but we generally discourage this because it can be error prone.
+In order to create your environment, run `make virtual-environment`.
+
+If there are any issues, the messages from the `Makefile` should guide you
+through. If not, please raise an issue in the [issue tracker][issue_tracker].
+
+For the rest of our developer docs, please see {ref}`development-reference`.
+
+[issue_tracker]: https://gitlab.com/climate-resource/carpet-concentrations/issues
 
-.. sec-end-installation-dev
+<!--- sec-end-installation-dev -->
```

### Comparing `carpet_concentrations-0.1.0/src/carpet_concentrations/testing.py` & `carpet_concentrations-0.2.1/src/carpet_concentrations/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 Testing related functions
 """
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from typing import Any, Dict, Optional, Tuple
+    from typing import Any
 
 
 def get_call_kwargs(
-    paras: Tuple[Tuple[str, Any]],
-    extra_kwargs: Optional[Dict[str, Any]] = None,
-) -> Dict[str, Any]:
+    paras: tuple[tuple[str, Any]],
+    extra_kwargs: dict[str, Any] | None = None,
+) -> dict[str, Any]:
     """
-    Get kwargs used to call a callable
+    Get kwargs used to call a callable.
 
     Useful when you want to test the default values of a function
 
     Parameters
     ----------
     paras
         Input parameters to test. Each element is the parameter's name and its
```

### Comparing `carpet_concentrations-0.1.0/src/carpet_concentrations/time.py` & `carpet_concentrations-0.2.1/src/carpet_concentrations/time.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,23 +2,61 @@
 Time handling
 """
 from __future__ import annotations
 
 from functools import partial
 from typing import TYPE_CHECKING, Protocol
 
-import cftime  # type: ignore[import]
+import cftime
 import numpy as np
 
 if TYPE_CHECKING:
-    from typing import Any, Tuple, Union
+    from collections.abc import Iterable
+    from typing import Any
 
     import xarray as xr
 
 
+MONTHS_PER_YEAR: int = 12
+"""Months per year"""
+
+
+class NonUniqueYearMonths(ValueError):
+    """
+    Raised when the user tries to convert to year-month with non-unique values
+
+    This happens when the datetime values lead to year-month values that are
+    not unique
+    """
+
+    def __init__(
+        self, unique_vals: Iterable[tuple[int, int]], counts: Iterable[int]
+    ) -> None:
+        """
+        Initialise the error
+
+        Parameters
+        ----------
+        unique_vals
+            Unique values. In each tuple, the first value is the year and the
+            second is the month.
+
+        counts
+            Counts of the number of time each unique value appeared in the
+            original array
+        """
+        non_unique = list((v, c) for v, c in zip(unique_vals, counts) if c > 1)
+
+        error_msg = (
+            "Your year-month axis is not unique. "
+            f"Year-month values with a count > 1: {non_unique}"
+        )
+        super().__init__(error_msg)
+
+
 def convert_year_month_to_time(
     inp: xr.Dataset,
     day: int = 1,
     **kwargs: Any,
 ) -> xr.Dataset:
     """
     Convert year and month co-ordinates into a time axis
@@ -48,26 +86,26 @@
 
 
 class CftimeConverter(Protocol):  # pylint: disable=too-few-public-methods
     """
     Callable that supports converting stacked time co-ordinates to :obj:`cftime.datetime`
     """
 
-    def __call__(  # type: ignore[no-any-unimported]
+    def __call__(
         self,
-        *args: Union[np.float_, np.int_],
+        *args: np.float_ | np.int_,
     ) -> cftime.datetime:
         """
         Convert input values to an :obj:`cftime.datetime`
         """
 
 
 def convert_to_time(
     inp: xr.Dataset,
-    time_coords: Tuple[str, ...],
+    time_coords: tuple[str, ...],
     cftime_converter: CftimeConverter,
 ) -> xr.Dataset:
     """
     Convert some co-ordinates representing time into a time axis
 
     Parameters
     ----------
@@ -82,51 +120,105 @@
         :obj:`cftime.datetime`
 
     Returns
     -------
         Data with time axis
     """
     inp = inp.stack(time=time_coords)
-    times = inp["time"].values
+    times = inp["time"].to_numpy()
 
-    inp = inp.drop_vars(("time",) + time_coords).assign_coords(
+    inp = inp.drop_vars(("time", *time_coords)).assign_coords(
         {"time": [cftime_converter(*t) for t in times]}
     )
 
     return inp
 
 
-def convert_time_to_year_month(
+def split_time_to_year_month(
     inp: xr.Dataset,
     time_axis: str = "time",
 ) -> xr.Dataset:
     """
-    Convert the time dimension to year and month co-ordinates
+    Convert the time dimension to year and month without stacking
+
+    This means there is still a single time dimension in the output, but there
+    is now also accompanying year and month information
 
     Parameters
     ----------
     inp
         Data to convert
 
     Returns
     -------
-        Data with year and month co-ordinates
+        Data with year and month information for the time axis
+
+    Raises
+    ------
+    NonUniqueYearMonths
+        The years and months are not unique
     """
     out = inp.assign_coords(
         {
             "month": inp[time_axis].dt.month,
             "year": inp[time_axis].dt.year,
         }
     ).set_index({time_axis: ("year", "month")})
 
     # Could be updated when https://github.com/pydata/xarray/issues/7104 is
     # closed
     unique_vals, counts = np.unique(out[time_axis].values, return_counts=True)
 
     if (counts > 1).any():
-        non_unique = list((v, c) for v, c in zip(unique_vals, counts) if c > 1)
-        raise ValueError(
-            "Your year-month axis is not unique. "
-            f"Year-month values with a count > 1: {non_unique}"
-        )
+        raise NonUniqueYearMonths(unique_vals, counts)
+
+    return out
+
 
-    return out.unstack(time_axis)
+def convert_time_to_year_month(
+    inp: xr.Dataset,
+    time_axis: str = "time",
+) -> xr.Dataset:
+    """
+    Convert the time dimension to year and month co-ordinates
+
+    Parameters
+    ----------
+    inp
+        Data to convert
+
+    Returns
+    -------
+        Data with year and month co-ordinates
+    """
+    return split_time_to_year_month(
+        inp=inp,
+        time_axis=time_axis,
+    ).unstack(time_axis)
+
+
+def get_start_of_next_month(y: int, m: int) -> cftime.datetime:
+    """
+    Get start of next month
+
+    Parameters
+    ----------
+    y
+        Year
+
+    m
+        Month
+
+    Returns
+    -------
+        Start of next month
+    """
+    if m == MONTHS_PER_YEAR:
+        m_out = 1
+        y_out = y + 1
+    else:
+        m_out = m + 1
+        y_out = y
+
+    # This may need to be refactored to allow the cftime_converter to be
+    # injected, same idea as `convert_to_time`
+    return cftime.datetime(y_out, m_out, 1)
```

### Comparing `carpet_concentrations-0.1.0/PKG-INFO` & `carpet_concentrations-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,97 @@
 Metadata-Version: 2.1
 Name: carpet-concentrations
-Version: 0.1.0
-Summary: 
+Version: 0.2.1
+Summary: Core tools for the development of greenhouse gas concentration input files (i.e. flying carpets).
 Author: Zebedee Nicholls
 Author-email: zebedee.nicholls@climate-resource.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: cfxarray
+Provides-Extra: netcdf
 Provides-Extra: notebooks
 Provides-Extra: plots
+Requires-Dist: attrs (>=23.1.0,<24.0.0)
+Requires-Dist: cf-xarray (>=0.8.1,<0.9.0) ; extra == "cfxarray"
 Requires-Dist: cftime (>=1.6.2,<2.0.0)
 Requires-Dist: ipywidgets (>=8.0.6,<9.0.0) ; extra == "notebooks"
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: netcdf4 (>=1.6.3,<2.0.0) ; extra == "netcdf"
 Requires-Dist: notebook (>=6.5.3,<7.0.0) ; extra == "notebooks"
+Requires-Dist: openscm-units (>=0.5.2,<0.6.0)
+Requires-Dist: pint (>=0.19)
+Requires-Dist: pint-xarray (>=0.3,<0.4)
+Requires-Dist: pooch (>=1.7.0,<2.0.0) ; extra == "cfxarray"
 Requires-Dist: seaborn (>=0.12.2,<0.13.0) ; extra == "plots"
 Requires-Dist: xarray (>=2023.4.2,<2024.0.0)
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 
-.. sec-begin-description
+# Carpet - Concentrations
 
-Carpet - Concentrations
-=======================
+<!--- sec-begin-description -->
 
-[TODO badges here #1]
+[#1 badges here]
 
-Core tools for the development of greenhouse gas concentration input files (i.e.
-flying carpets).
+Core tools for the development of greenhouse gas concentration input files (i.e. flying carpets).
 
-Full documentation can be found at: [TODO read the docs link here #2]
+<!---
+Can use start-after and end-before directives in docs, see
+https://myst-parser.readthedocs.io/en/latest/syntax/organising_content.html#inserting-other-documents-directly-into-the-current-document
+-->
 
-.. sec-begin-links
+<!--- sec-end-description -->
 
-.. _issue tracker: https://gitlab.com/climate-resource/carpet-concentrations/-/issues
+Full documentation can be found at: [#2 read the docs link here]
 
-.. sec-end-links
+## Installation
 
-.. sec-end-description
+<!--- sec-begin-installation -->
 
-Installation
-------------
+Carpet - Concentrations can be installed with conda or pip:
 
-Carpet - concentrations can be installed with conda or pip:
-
-.. code:: bash
-
-    pip install carpet-concentrations
-    conda install -c conda-forge carpet-concentrations
+```bash
+pip install carpet-concentrations
+conda install -c conda-forge carpet-concentrations
+```
 
 Additional dependencies can be installed using
 
-.. code:: bash
+```bash
+# To add plotting dependencies
+pip install carpet-concentrations[plots]
+# To add notebook dependencies
+pip install carpet-concentrations[notebooks]
 
-    # To add plotting dependencies
-    pip install carpet-concentrations[plots]
-    # To run the notebooks
-    pip install carpet-concentrations[notebooks, plots]
-    # If you are installing with conda, we recommend
-    # installing the extras by hand because there is no stable
-    # solution yet (issue here: https://github.com/conda/conda/issues/7502)
+# If you are installing with conda, we recommend
+# installing the extras by hand because there is no stable
+# solution yet (issue here: https://github.com/conda/conda/issues/7502)
+```
 
-.. sec-end-installation
+<!--- sec-end-installation -->
 
-.. sec-begin-installation-dev
+### For developers
 
-For developers
-~~~~~~~~~~~~~~
+<!--- sec-begin-installation-dev -->
 
-For development, we rely on `poetry <https://python-poetry.org>`_ for all our
+For development, we rely on [poetry](https://python-poetry.org) for all our
 dependency management. To get started, you will need to make sure that poetry
 is installed
-(https://python-poetry.org/docs/#installing-with-the-official-installer, we
-found that pipx and pip worked better to install on a Mac).
+([instructions here](https://python-poetry.org/docs/#installing-with-the-official-installer),
+we found that pipx and pip worked better to install on a Mac).
 
-For all of work, we use our ``Makefile``.
+For all of work, we use our `Makefile`.
 You can read the instructions out and run the commands by hand if you wish,
-but we generally discourage this because it can be error prone and doesn't
-update if dependencies change (e.g. the environment is updated).
-In order to create your environment, run ``make virtual-environment``.
-
-If there are any issues, the messages from the ``Makefile`` should guide you
-through. If not, please raise an issue in the
-`issue tracker`_.
+but we generally discourage this because it can be error prone.
+In order to create your environment, run `make virtual-environment`.
+
+If there are any issues, the messages from the `Makefile` should guide you
+through. If not, please raise an issue in the [issue tracker][issue_tracker].
+
+For the rest of our developer docs, please see {ref}`development-reference`.
+
+[issue_tracker]: https://gitlab.com/climate-resource/carpet-concentrations/issues
 
-.. sec-end-installation-dev
+<!--- sec-end-installation-dev -->
```

