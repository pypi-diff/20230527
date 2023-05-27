# Comparing `tmp/act4e_mcdp-0.4.3-py3-none-any.whl.zip` & `tmp/act4e_mcdp-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 35412 bytes, number of entries: 14
--rw-r--r--  2.0 unx      347 b- defN 80-Jan-01 00:00 act4e_mcdp/__init__.py
+Zip file size: 37442 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      387 b- defN 80-Jan-01 00:00 act4e_mcdp/__init__.py
 -rw-r--r--  2.0 unx    67896 b- defN 80-Jan-01 00:00 act4e_mcdp/autogen_packed_test_data.py
 -rw-r--r--  2.0 unx      571 b- defN 80-Jan-01 00:00 act4e_mcdp/download.py
--rw-r--r--  2.0 unx    10217 b- defN 80-Jan-01 00:00 act4e_mcdp/loading.py
--rw-r--r--  2.0 unx     3363 b- defN 80-Jan-01 00:00 act4e_mcdp/main.py
--rw-r--r--  2.0 unx     4381 b- defN 80-Jan-01 00:00 act4e_mcdp/nameddps.py
+-rw-r--r--  2.0 unx    10246 b- defN 80-Jan-01 00:00 act4e_mcdp/loading.py
+-rw-r--r--  2.0 unx     3281 b- defN 80-Jan-01 00:00 act4e_mcdp/main_solve_dp.py
+-rw-r--r--  2.0 unx     3924 b- defN 80-Jan-01 00:00 act4e_mcdp/main_solve_mcdp.py
+-rw-r--r--  2.0 unx     4656 b- defN 80-Jan-01 00:00 act4e_mcdp/nameddps.py
 -rw-r--r--  2.0 unx     1790 b- defN 80-Jan-01 00:00 act4e_mcdp/posets.py
--rw-r--r--  2.0 unx    11777 b- defN 80-Jan-01 00:00 act4e_mcdp/primitivedps.py
+-rw-r--r--  2.0 unx    11916 b- defN 80-Jan-01 00:00 act4e_mcdp/primitivedps.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 act4e_mcdp/py.typed
--rw-r--r--  2.0 unx     3944 b- defN 80-Jan-01 00:00 act4e_mcdp/solution_interface.py
--rw-r--r--  2.0 unx      361 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.3.dist-info/WHEEL
--rw-r--r--  2.0 unx      109 b- defN 80-Jan-01 00:00 act4e_mcdp-0.4.3.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1121 b- defN 16-Jan-01 00:00 act4e_mcdp-0.4.3.dist-info/RECORD
-14 files, 105965 bytes uncompressed, 33560 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx     7934 b- defN 80-Jan-01 00:00 act4e_mcdp/solution_interface.py
+-rw-r--r--  2.0 unx      361 b- defN 80-Jan-01 00:00 act4e_mcdp-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 act4e_mcdp-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      164 b- defN 80-Jan-01 00:00 act4e_mcdp-0.5.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1216 b- defN 16-Jan-01 00:00 act4e_mcdp-0.5.0.dist-info/RECORD
+15 files, 114430 bytes uncompressed, 35438 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -6,15 +6,18 @@
 
 Filename: act4e_mcdp/download.py
 Comment: 
 
 Filename: act4e_mcdp/loading.py
 Comment: 
 
-Filename: act4e_mcdp/main.py
+Filename: act4e_mcdp/main_solve_dp.py
+Comment: 
+
+Filename: act4e_mcdp/main_solve_mcdp.py
 Comment: 
 
 Filename: act4e_mcdp/nameddps.py
 Comment: 
 
 Filename: act4e_mcdp/posets.py
 Comment: 
@@ -24,20 +27,20 @@
 
 Filename: act4e_mcdp/py.typed
 Comment: 
 
 Filename: act4e_mcdp/solution_interface.py
 Comment: 
 
-Filename: act4e_mcdp-0.4.3.dist-info/METADATA
+Filename: act4e_mcdp-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: act4e_mcdp-0.4.3.dist-info/WHEEL
+Filename: act4e_mcdp-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: act4e_mcdp-0.4.3.dist-info/entry_points.txt
+Filename: act4e_mcdp-0.5.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: act4e_mcdp-0.4.3.dist-info/RECORD
+Filename: act4e_mcdp-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## act4e_mcdp/__init__.py

```diff
@@ -6,13 +6,14 @@
 
 logger = getLogger(__name__)
 logger.setLevel(DEBUG)
 
 # __version__ = "0.2.1"
 
 from .loading import *
-from .main import *
+from .main_solve_mcdp import *
+from .main_solve_dp import *
 from .solution_interface import *
 from .nameddps import *
 from .primitivedps import *
 from .posets import *
 from .download import *
```

## act4e_mcdp/loading.py

```diff
@@ -386,15 +386,15 @@
         raise ValueError(msg) from e
 
 
 def parse_yaml_value(poset: Poset, ob: object) -> object:
     match poset:
         case Numbers():
             if not isinstance(ob, (int, str, float, bool)):
-                msg = "Expected string, got %s" % type(ob)
+                msg = "For Poset of numbers, expected string or int, got %s" % type(ob)
                 raise ValueError(msg)
             return Decimal(ob)
         case FinitePoset():
             return ob
         case PosetProduct(subs):
             if not isinstance(ob, list):
                 msg = "Expected list, got %s" % type(ob)
```

## act4e_mcdp/nameddps.py

```diff
@@ -52,55 +52,59 @@
     dp: PrimitiveDP
 
 
 @dataclass
 class NodeResource:
     """
     A resource of a node.
+    Used by the [Connection][act4e_mcdp.nameddps.Connection] class.
 
     Attributes:
         node: the node name
         resource: the resource name
 
     """
 
     node: str
     resource: str
 
 
 @dataclass
 class NodeFunctionality:
     """
-    A functionality of a node
+    A functionality of a node.
+    Used by the [Connection][act4e_mcdp.nameddps.Connection] class.
 
     Attributes:
         node: the node name
         functionality: the functionality name
     """
 
     node: str
     functionality: str
 
 
 @dataclass
 class ModelFunctionality:
     """
-    A functionality of the entire diagram
+    A functionality of the entire diagram.
+    Used by the [Connection][act4e_mcdp.nameddps.Connection] class.
 
     Attributes:
         functionality: the functionality name
     """
 
     functionality: str
 
 
 @dataclass
 class ModelResource:
     """
-    A resource of the entire diagram
+    A resource of the entire diagram.
+    Used by the [Connection][act4e_mcdp.nameddps.Connection] class.
 
     Attributes:
         resource: the resource name
 
     """
 
     resource: str
```

## act4e_mcdp/primitivedps.py

```diff
@@ -526,14 +526,20 @@
     c: ValueFromPoset
 
 
 @dataclass
 class EntryInfo:
     r"""
     Describes $\fun^{\max}_{\imp}$ and $\res^{\min}_{\imp}$ for an implementation.
+
+
+    Attributes:
+        f_max: The maximum functionality $\fun^{\max}_{\imp}$
+        r_min: The minimum resources $\res^{\min}_{\imp}$
+
     """
     f_max: object
     r_min: object
 
 
 @dataclass
 class CatalogueDP(PrimitiveDP):
```

## act4e_mcdp/solution_interface.py

```diff
@@ -1,14 +1,21 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Any, Generic, Mapping, TypeVar
 
 from .nameddps import NamedDP
+from .primitivedps import PrimitiveDP
 
-__all__ = ["LowerSet", "SolverInterface", "UpperSet"]
+__all__ = [
+    "DPSolverInterface",
+    "Interval",
+    "LowerSet",
+    "MCDPSolverInterface",
+    "UpperSet",
+]
 
 X = TypeVar("X")
 
 
 @dataclass
 class UpperSet(Generic[X]):
     """
@@ -31,24 +38,140 @@
         maxima: A list of elements of type X, which are the minimal elements of the set.
 
     """
 
     maxima: list[X]
 
 
-class SolverInterface(ABC):
+@dataclass(kw_only=True)
+class Interval(Generic[X]):
     """
-    An abstract class that describes the interface of a solver.
+    Describes an optimistic-pessimistic interval for a quantity of type X.
 
+    The two values can be the same if there is no uncertainty.
+
+    Attributes:
+        pessimistic: The pessimistic value
+        optimistic: The optimistic value
+
+    """
+
+    pessimistic: X
+    optimistic: X
+
+
+class DPSolverInterface(ABC):
     """
+    An abstract class that describes the interface of a solver for DPs.
+
+    """
+
+    @abstractmethod
+    def solve_dp_FixFunMinRes(
+        self,
+        dp: PrimitiveDP,
+        functionality_needed: object,
+        /,
+        resolution_optimistic: int = 0,
+        resolution_pessimistic: int = 0,
+    ) -> Interval[UpperSet[object]]:
+        """
+
+        Solves the problem of finding the minimal resources needed to satisfy a given functional requirement.
+
+        The problem is defined by a DP and a query. The model is a DP, and the query is an
+        object that belongs to the poset $\F$ of the functionalities of the DP.
+
+        The solution is an interval of upper sets (of objects of $\R$).
+
+
+        For example, this is what we expect from a solver for an empty catalogue:
+
+        ```python
+
+            solver: SolverInterface = ...
+
+            P = FinitePoset({'a', 'b'}, {('a', 'b')})
+
+            empty_catalogue = CatalogueDP(F=P, R=P, entries={})
+
+            result = solver.solve_dp_FixFunMinRes(empty, 'a')
+
+            assert result.pessimistic == result.optimistic == UpperSet([])
+
+        ```
+        For example, for the identity:
+
+
+        ```python
+
+            solver: SolverInterface = ...
+
+            P = FinitePoset({'a', 'b'}, {('a', 'b')})
+
+            empty_catalogue = IdentityDP(F=P, R=P)
+
+            result = solver.solve_dp_FixFunMinRes(empty, 'a')
+
+            assert result.pessimistic == result.optimistic == UpperSet(['a'])
+
+        ```
+
+        Parameters:
+            dp: A design problem.
+            functionality_needed: The functionality needed.
+            resolution_optimistic: An integer returning the resolution of the optimistic answer, to be used
+            in the case of DPs that are not computable.
+            resolution_pessimistic: Same thing, for the pessimistic answer.
+
+        Returns:
+
+            An interval of upper sets.
+        """
+        raise NotImplementedError
 
     @abstractmethod
-    def solve_FixFunMinRes(
-        self, model: NamedDP, functionality_needed: Mapping[str, Any], /
-    ) -> UpperSet[Mapping[str, Any]]:
+    def solve_dp_FixResMaxFun(
+        self,
+        dp: PrimitiveDP,
+        resource_budget: object,
+        /,
+        resolution_optimistic: int = 0,
+        resolution_pessimistic: int = 0,
+    ) -> Interval[LowerSet[object]]:
+        """
+        Solves the problem of finding the maximal functionality that can be provided with a given budget of
+        resources.
+        It is the dual of solve_dp_FixFunMinRes.
+
+        Parameters:
+            dp: A design problem.
+            resource_budget: The resources available.
+            resolution_optimistic: An integer returning the resolution of the optimistic answer, to be used
+            in the case of DPs that are not computable.
+            resolution_pessimistic: Same thing, for the pessimistic answer.
+
+        Returns:
+
+            An interval of lower sets.
+        """
+
+
+class MCDPSolverInterface(ABC):
+    """An abstract class that describes the interface of a solver for NamedDPs."""
+
+    @abstractmethod
+    def solve_mcdp_FixFunMinRes(
+        self,
+        graph: NamedDP,
+        functionality_needed: Mapping[str, Any],
+        /,
+        resolution_optimistic: int = 0,
+        resolution_pessimistic: int = 0,
+    ) -> Interval[UpperSet[Mapping[str, Any]]]:
         """
 
         Solves the problem of finding the minimal resources needed to satisfy a given functional requirement.
 
         The problem is defined by a model and a query. The model is a NamedDP, and the query is a mapping from
         the names of the resources to the values of the resources.
 
@@ -95,27 +218,36 @@
             # We expect that the result is a list containing only one element
 
             assert list(result.minima) == [{'r1': 'a'}]
         ```
 
 
         Parameters:
-            model: The model of the problem.
+            graph: The model of the problem.
             functionality_needed: The functionality needed (key-value dictionary).
+            resolution_optimistic: An integer returning the resolution of the optimistic answer, to be used
+            in the case of DPs that are not computable.
+            resolution_pessimistic: Same thing, for the pessimistic answer.
 
         Returns:
 
-            A finitely-supported upper set of resources.
+            An interval of upper sets.
+
         """
         raise NotImplementedError
 
     @abstractmethod
-    def solve_FixResMaxFun(
-        self, model: NamedDP, resources_budget: Mapping[str, Any], /
-    ) -> LowerSet[Mapping[str, Any]]:
+    def solve_mcdp_FixResMaxFun(
+        self,
+        graph: NamedDP,
+        resources_budget: Mapping[str, Any],
+        /,
+        resolution_optimistic: int = 0,
+        resolution_pessimistic: int = 0,
+    ) -> Interval[LowerSet[Mapping[str, Any]]]:
         """
         This is the dual of solve_FixFunMinRes. It solves the problem of finding the maximal functionality
         that can be provided with a given budget of resources.
 
 
         For example, this is what we expect from a solver for the empty model:
 
@@ -130,17 +262,20 @@
             # We expect that the result is a list containing the empty dictionary
 
             assert list(result.maxima) == [{}]
 
         ```
 
         Parameters:
-            model: The model of the problem.
+            graph: The model of the problem.
             resources_budget: The maximum budget that we have (key-value dictionary).
+            resolution_optimistic: An integer returning the resolution of the optimistic answer, to be used
+            in the case of DPs that are not computable.
+            resolution_pessimistic: Same thing, for the pessimistic answer.
 
         Returns:
 
-            A finitely-supported upper set of resources.
+             An interval of lower sets.
 
 
         """
         raise NotImplementedError
```

## Comparing `act4e_mcdp/main.py` & `act4e_mcdp/main_solve_dp.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,51 +2,56 @@
 import os
 import sys
 from importlib import import_module
 
 import yaml
 
 from . import logger
+from .primitivedps import PrimitiveDP
 from .loading import load_repr1, parse_yaml_value
-from .solution_interface import SolverInterface
 from .nameddps import NamedDP
+from .solution_interface import DPSolverInterface
 
 
 def import_from_string(dot_path: str) -> object:
     module_path, _, name = dot_path.rpartition(".")
     module = import_module(module_path)
     return getattr(module, name)
 
 
-__all__ = ["solve_main"]
+__all__ = ["solve_dp_main"]
 
 
-def solve_main() -> None:
+def solve_dp_main() -> None:
     queries = ["FixFunMinRes", "FixResMaxFun"]
     parser = argparse.ArgumentParser()
-    parser.add_argument("--model", help="Model source (file or URL)", required=True)
+    parser.add_argument("--model", help="DP Model source (file or URL)", required=True)
     parser.add_argument("--query", help="query", default="FixFunMinRes", required=False)
     parser.add_argument("--data", help="data (YAML Format)", required=True)
     parser.add_argument("--solver", help="Model source (file or URL)", required=True)
 
     args = parser.parse_args()
 
     model_source = args.model
     try:
         solver0 = import_from_string(args.solver)
     except Exception as e:
         logger.error("Could not import solver %r", args.solver, exc_info=e)
         sys.exit(1)
 
-    solver: SolverInterface
+    solver: DPSolverInterface
 
-    if isinstance(solver0, SolverInterface):
+    if isinstance(solver0, DPSolverInterface):
         solver = solver0
     else:
+        # noinspection PyCallingNonCallable
         solver = solver0()  # type: ignore
+    if not isinstance(solver, DPSolverInterface):
+        msg = f"Expected a DPSolverInterface, got {solver!r}"
+        raise ValueError(msg)
 
     query = args.query
 
     if query not in queries:
         logger.error("Unknown query %r. Known: %r", query, queries)
         sys.exit(1)
 
@@ -65,50 +70,39 @@
         if os.path.exists(model_source):
             model_source = open(model_source).read()
             data = yaml.load(model_source, Loader=yaml.SafeLoader)
         else:
             logger.error("Cannot open file: %r", model_source)
             sys.exit(1)
 
-    model = load_repr1(data, NamedDP)
+    model = load_repr1(data, PrimitiveDP)
+    if not isinstance(model, PrimitiveDP):
+        if isinstance(model, NamedDP):
+            msg = f"Expected a PrimitiveDP, not a NamedDP. Did you mean to use 'act4e-mcdp-solve-mcdp'?"
+            raise ValueError(msg)
+
+        msg = f"Expected a NamedDP, got {model!r}"
+        raise ValueError(msg)
     logger.info("model: %s", model)
 
     yaml_query = yaml.load(query_data, Loader=yaml.SafeLoader)
-    if not isinstance(yaml_query, dict):
-        raise ValueError(f"Expected dict, got {yaml_query!r}")
 
     if query == "FixFunMinRes":
-        found = set(yaml_query)
-        expected = set(model.functionalities)
-        if found != expected:
-            msg = f"Expected {expected}, got {found}"
-            raise ValueError(msg)
-
-        value = {}
-        for k, v in model.functionalities.items():
-            value[k] = parse_yaml_value(v, yaml_query[k])
+        value = parse_yaml_value(model.F, yaml_query)
 
         logger.info("query: %s", value)
 
-        solution = solver.solve_FixFunMinRes(model, value)
+        solution = solver.solve_dp_FixFunMinRes(model, value)
 
         logger.info("solution: %s", solution)
 
     elif query == "FixResMaxFun":
-        found = set(yaml_query)
-        expected = set(model.resources)
-        if found != expected:
-            msg = f"Expected {expected}, got {found}"
-            raise ValueError(msg)
-
-        value = {}
-        for k, v in model.resources.items():
-            value[k] = parse_yaml_value(v, yaml_query[k])
+        value = parse_yaml_value(model.R, yaml_query)
 
         logger.info("query: %s", value)
 
-        solution = solver.solve_FixResMaxFun(model, value)
+        solution = solver.solve_dp_FixFunMinRes(model, value)
 
         logger.info("solution: %s", solution)
 
     else:
         raise ValueError(f"Unknown query {query}")
```

