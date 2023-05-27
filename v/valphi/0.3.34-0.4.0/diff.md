# Comparing `tmp/valphi-0.3.34.tar.gz` & `tmp/valphi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valphi-0.3.34.tar", max compression
+gzip compressed data, was "valphi-0.4.0.tar", max compression
```

## Comparing `valphi-0.3.34.tar` & `valphi-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2022-09-22 13:08:25.021598 valphi-0.3.34/LICENSE
--rw-r--r--   0        0        0      427 2023-05-26 18:18:04.224918 valphi-0.3.34/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-22 13:13:37.919365 valphi-0.3.34/valphi/__init__.py
--rwxr-xr-x   0        0        0       97 2022-09-22 16:30:02.808202 valphi-0.3.34/valphi/__main__.py
--rw-r--r--   0        0        0    10620 2023-05-26 18:14:44.616560 valphi-0.3.34/valphi/cli.py
--rw-r--r--   0        0        0     2266 2023-01-17 17:02:20.445653 valphi-0.3.34/valphi/contexts.py
--rw-r--r--   0        0        0    17029 2023-01-19 09:06:20.915594 valphi-0.3.34/valphi/controllers.py
--rw-r--r--   0        0        0     1899 2023-01-17 17:07:21.715958 valphi-0.3.34/valphi/models.py
--rw-r--r--   0        0        0    14909 2023-01-17 17:02:20.461653 valphi-0.3.34/valphi/networks.py
--rw-r--r--   0        0        0     5570 2023-01-17 17:02:20.453652 valphi-0.3.34/valphi/propagators.py
--rw-r--r--   0        0        0      102 2023-01-13 07:23:53.009969 valphi-0.3.34/valphi/utils.py
--rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 valphi-0.3.34/setup.py
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 valphi-0.3.34/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-09-22 13:08:25.021598 valphi-0.4.0/LICENSE
+-rw-r--r--   0        0        0      426 2023-05-27 07:42:09.517912 valphi-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-22 13:13:37.919365 valphi-0.4.0/valphi/__init__.py
+-rwxr-xr-x   0        0        0       97 2022-09-22 16:30:02.808202 valphi-0.4.0/valphi/__main__.py
+-rw-r--r--   0        0        0    10775 2023-05-27 06:50:25.868917 valphi-0.4.0/valphi/cli.py
+-rw-r--r--   0        0        0     2266 2023-01-17 17:02:20.445653 valphi-0.4.0/valphi/contexts.py
+-rw-r--r--   0        0        0    17336 2023-05-27 07:26:58.452592 valphi-0.4.0/valphi/controllers.py
+-rw-r--r--   0        0        0     1899 2023-01-17 17:07:21.715958 valphi-0.4.0/valphi/models.py
+-rw-r--r--   0        0        0    16153 2023-05-27 07:42:09.529912 valphi-0.4.0/valphi/networks.py
+-rw-r--r--   0        0        0     5570 2023-01-17 17:02:20.453652 valphi-0.4.0/valphi/propagators.py
+-rw-r--r--   0        0        0      102 2023-01-13 07:23:53.009969 valphi-0.4.0/valphi/utils.py
+-rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 valphi-0.4.0/setup.py
+-rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 valphi-0.4.0/PKG-INFO
```

### Comparing `valphi-0.3.34/LICENSE` & `valphi-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `valphi-0.3.34/valphi/cli.py` & `valphi-0.4.0/valphi/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,15 +60,19 @@
         ),
         filenames: List[Path] = typer.Option(
             [],
             "--filename",
             "-f",
             help="One or more files to parse",
         ),
-        weight_constraints: bool = typer.Option(False, help="Use weight constraints instead of ad-hoc propagator"),
+        weight_constraints: Optional[int] = typer.Option(
+            None,
+            help="Use weight constraints instead of ad-hoc propagator. "
+                 "It also requires a multiplier to approximate real numbers."
+        ),
         ordered: bool = typer.Option(False, help="Add ordered encoding for eval/3"),
         debug: bool = typer.Option(False, "--debug", help="Show stacktrace and debug info"),
 ):
     """
     Neural Network evaluation under fuzzy semantics.
 
     Use --help after a command for the list of arguments and options of that command.
@@ -178,22 +182,25 @@
     with console.status("Running..."):
         res = app_options.controller.find_solutions(number_of_solutions)
     if not res:
         console.print('NO SOLUTIONS')
     for index, values in enumerate(res, start=1):
         console.print(network_values_to_table(values, title=f"Solution {index}"))
     if show_in_asp_chef:
-        for index, values in enumerate(res, start=1):
-            url = "https://asp-chef.alviano.net/open#"
-            # url = "http://localhost:5188/open#"
-            graph = app_options.controller.network.network_facts.filter(when=lambda atom: atom.predicate_name == "attack").as_facts
-            evaluation = '\n'.join(f"eval({node},{','.join(value.split('/'))})." for node, value in values.items())
-            url += compress_object_for_url({"input": graph + '\n' + evaluation}, suffix="")
-            url += ";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%21"
-            webbrowser.open(url, new=0, autoraise=True)
+        url = "https://asp-chef.alviano.net/open#"
+        # url = "http://localhost:5188/open#"
+        graph = app_options.controller.network.network_facts.filter(when=lambda atom: atom.predicate_name == "attack").as_facts
+        models = []
+        for values in res:
+            models.append(graph)
+            models.append('\n'.join(f"eval({node},{','.join(value.split('/'))})." for node, value in values.items()))
+            models.append('§')
+        url += compress_object_for_url({"input": '\n'.join(models[:-1])}, suffix="")
+        url += ";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%21"
+        webbrowser.open(url, new=0, autoraise=True)
 
 
 @app.command(name="query")
 def command_query(
         query: Optional[str] = typer.Argument(
             None,
             help=f"A string representing the query as an alternative to --query-filename",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `valphi-0.3.34/valphi/contexts.py` & `valphi-0.4.0/valphi/contexts.py`

 * *Files identical despite different names*

### Comparing `valphi-0.3.34/valphi/controllers.py` & `valphi-0.4.0/valphi/controllers.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 @typeguard.typechecked
 @dataclasses.dataclass(frozen=True)
 class Controller:
     network: NetworkInterface
     val_phi: List[float] = dataclasses.field(default_factory=lambda: Controller.default_val_phi())
     raw_code: str = dataclasses.field(default="")
-    use_wc: bool = dataclasses.field(default=False)
+    use_wc: Optional[int] = dataclasses.field(default=None)
     use_ordered_encoding: bool = dataclasses.field(default=False)
 
     @typeguard.typechecked
     @dataclasses.dataclass(frozen=True)
     class QueryResult:
         key: InitVar[PrivateKey]
         true: bool
@@ -73,44 +73,48 @@
                 consistent_knowledge_base=False,
                 left_concept_value=None,
             )
 
     def __post_init__(self):
         validate("max_value", self.max_value, min_value=1, max_value=1000)
         validate("val_phi", self.val_phi, equals=sorted(self.val_phi))
-        validate("val-phi must be integer", all(type(value) is int or value.is_integer() for value in self.val_phi),
-                 equals=True, help_msg="Weight-constraints requires an integer val-phi")
+        if self.use_wc is not None:
+            validate("use_wc", self.use_wc, min_value=1, max_value=1_000_000)
+        # if self.use_wc:
+        #     validate("val-phi must be integer", all(type(value) is int or value.is_integer() for value in self.val_phi),
+        #              equals=True, help_msg="Weight-constraints requires an integer val-phi")
         if type(self.network) is MaxSAT:
             validate("", self.val_phi, equals=self.network.val_phi)
 
     @staticmethod
     def default_val_phi() -> List[float]:
-        return [-10987, -4237, 0, 4236, 10986]
+        return [-10.987, -4.237, 0, 4.236, 10.986]
 
     @property
     def max_value(self) -> int:
         return len(self.val_phi)
 
     def __setup_control(self, query: Optional[str] = None):
+        network = self.network if self.use_wc is None else self.network.approximate(self.use_wc)
         # control = clingo.Control(["--opt-strategy=usc,k,4", "--opt-usc-shrink=rgs"] if query else [])
         control = clingo.Control()
         # control.configuration.solve.models = self.max_stable_models if query is None else 0
         control.add("base", ["max_value"], BASE_PROGRAM
                     + (QUERY_ENCODING if query and not self.use_ordered_encoding else "")
                     + (QUERY_ORDERED_ENCODING if query and self.use_ordered_encoding else "")
                     + (ORDERED_ENCODING if self.use_ordered_encoding else "")
-                    + self.network.network_facts.as_facts
+                    + network.network_facts.as_facts
                     + self.raw_code + ("" if query is None else f"query({query})."))
         control.ground([("base", [Number(self.max_value)])], context=Context())
         if self.use_wc:
             constraints = self.__generate_wc()
             control.add("base", ["max_value"], '\n'.join(constraints))
             control.ground([("base", [Number(self.max_value)])], context=Context())
         else:
-            self.network.register_propagators(control, self.val_phi)
+            network.register_propagators(control, self.val_phi)
         return control
 
     def __read_eval(self, model) -> frozendict:
         res = {}
         for symbol in model:
             if symbol.predicate_name == "eval":
                 concept, individual, value = symbol.arguments
@@ -140,15 +144,15 @@
             raise ValueError("Use 'query even' for MaxSAT")
         control = self.__setup_control()
         control.configuration.solve.models = max_number_of_solutions
         model_collect = ModelCollect()
         control.solve(on_model=model_collect)
         return [self.__read_eval(model) for model in model_collect]
 
-    def answer_query(self, query: str) -> QueryResult:
+    def answer_query(self, query: str) -> "Controller.QueryResult":
         if type(self.network) is MaxSAT:
             validate("query", query, equals="even")
             query = self.network.query
         validate("query", query, custom=[pattern(r"[^#]+#[^#]+#(<|<=|>=|>)#(1|1.0|0\.\d+)")],
                  help_msg=f'The query "{query}" is not in the expected format. Is it a filename?')
         left, right, comparator, threshold = query.split('#')
         control = self.__setup_control(f'{left},{right},"{comparator}","{threshold}"')
@@ -168,18 +172,19 @@
         return factory_method(
             left_concept_value=left_concept_value / self.max_value,
             assignment=eval_values,
             witness=witness,
         )
 
     def __generate_wc(self):
-        res = [f"val_phi(0,#inf,{int(self.val_phi[0])})."]
-        for value in range(len(self.val_phi) - 1):
-            res.append(f"val_phi({value + 1},{int(self.val_phi[value])},{int(self.val_phi[value + 1])}).")
-        res.append(f"val_phi({len(self.val_phi)},{int(self.val_phi[-1])},#sup).")
+        val_phi = [round(value * self.use_wc) for value in self.val_phi]
+        res = [f"val_phi(0,#inf,{int(val_phi[0])})."]
+        for value in range(len(val_phi) - 1):
+            res.append(f"val_phi({value + 1},{int(val_phi[value])},{int(val_phi[value + 1])}).")
+        res.append(f"val_phi({len(val_phi)},{int(val_phi[-1])},#sup).")
         if self.use_ordered_encoding:
             res.append(WC_ORDERED_ENCODING)
         else:
             res.append(WC_ENCODING)
         return res
```

### Comparing `valphi-0.3.34/valphi/models.py` & `valphi-0.4.0/valphi/models.py`

 * *Files identical despite different names*

### Comparing `valphi-0.3.34/valphi/networks.py` & `valphi-0.4.0/valphi/networks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import dataclasses
+from copy import deepcopy
 from typing import List, Tuple, Optional, Union, Any, Set, FrozenSet
 
 import clingo
 import typeguard
 from distlib.util import cached_property
 from dumbo_utils.validation import validate
 
@@ -16,17 +17,17 @@
     __complete: List[bool] = dataclasses.field(default_factory=lambda: [False], init=False)
 
     __parse_key = object()
 
     @staticmethod
     def parse(s: Union[str, List[str]]) -> 'NetworkInterface':
         if type(s) == str:
-            lines = [x.strip() for x in s.strip().split('\n')]
+            lines = [x.strip().replace('\t', ' ') for x in s.strip().split('\n')]
         else:
-            lines = [x.strip() for x in s]
+            lines = [x.strip().replace('\t', ' ') for x in s]
         res = MaxSAT.parse_implementation(lines, NetworkInterface.__parse_key)
         if res is None:
             res = ArgumentationGraph.parse_implementation(lines, NetworkInterface.__parse_key)
         if res is None:
             res = NetworkTopology.parse_implementation(lines, NetworkInterface.__parse_key)
         return res
 
@@ -60,27 +61,37 @@
     def _register_propagators(self, control: clingo.Control, val_phi: List[float]) -> None:
         raise NotImplemented
 
     @cached_property
     def val_phi(self):
         raise NotImplemented
 
+    def approximate(self, multiplier: int) -> "NetworkInterface":
+        validate("multiplier", multiplier, min_value=1, max_value=1_000_000)
+        return self._approximate(multiplier)
+
+    def _approximate(self, multiplier: int) -> "NetworkInterface":
+        raise NotImplemented
+
 
 @typeguard.typechecked
 @dataclasses.dataclass(frozen=True)
 class EmptyNetwork(NetworkInterface):
     def __post_init__(self):
         self.complete()
 
     def _network_facts(self) -> Model:
         return Model.empty()
 
     def _register_propagators(self, control: clingo.Control, val_phi: List[float]) -> None:
         pass
 
+    def _approximate(self, multiplier: int) -> "NetworkInterface":
+        return self
+
 
 @typeguard.typechecked
 @dataclasses.dataclass(frozen=True)
 class NetworkTopology(NetworkInterface):
     __layers: List[List[List[float]]] = dataclasses.field(default_factory=list, init=False)
     __crisp_layers: set[int] = dataclasses.field(default_factory=set, init=False)
     __exactly_one: List[List[int]] = dataclasses.field(default_factory=list, init=False)
@@ -200,14 +211,27 @@
 
     def _register_propagators(self, control: clingo.Control, val_phi: List[float]) -> None:
         for layer_index, _ in enumerate(range(1, self.number_of_layers()), start=2):
             for node_index, _ in enumerate(range(self.number_of_nodes(layer=layer_index)), start=1):
                 propagator = ValPhiPropagator(self.term(layer_index, node_index), val_phi=val_phi)
                 control.register_propagator(propagator)
 
+    def _approximate(self, multiplier: int) -> "NetworkInterface":
+        res = NetworkTopology()
+        res.__layers.extend(
+            [
+                [round(weight * multiplier) for weight in node]
+                for node in layer
+            ]
+            for layer in self.__layers
+        )
+        res.__exactly_one.extend(deepcopy(self.__exactly_one))
+        res.__crisp_layers.update(self.__crisp_layers)
+        return res.complete()
+
 
 @typeguard.typechecked
 @dataclasses.dataclass(frozen=True)
 class ArgumentationGraph(NetworkInterface):
     __attacks: Set[Tuple[Any, Any, float]] = dataclasses.field(default_factory=set, init=False)
 
     @staticmethod
@@ -261,14 +285,21 @@
             for (attacker, attacked, weight) in self.__attacks
         ])
 
     def _register_propagators(self, control: clingo.Control, val_phi: List[float]) -> None:
         for attacked in self.attacked:
             control.register_propagator(ValPhiPropagator(self.term(attacked), val_phi=val_phi))
 
+    def _approximate(self, multiplier: int) -> "ArgumentationGraph":
+        res = ArgumentationGraph()
+        res.__attacks.update(
+            (value[0], value[1], round(value[2] * multiplier)) for value in self.__attacks
+        )
+        return res.complete()
+
 
 @typeguard.typechecked
 @dataclasses.dataclass(frozen=True)
 class MaxSAT(NetworkInterface):
     __clauses: List[Tuple[int]] = dataclasses.field(default_factory=list, init=False)
 
     @staticmethod
@@ -374,7 +405,10 @@
     def _register_propagators(self, control: clingo.Control, val_phi: List[float]) -> None:
         output_nodes = Model.of_program(self.network_facts.as_facts, """
 #show.
 #show Node : weighted_typicality_inclusion(Node,_,_).
         """)
         for node in output_nodes:
             control.register_propagator(ValPhiPropagator(str(node), val_phi=val_phi))
+
+    def _approximate(self, multiplier: int) -> "NetworkInterface":
+        return self
```

### Comparing `valphi-0.3.34/valphi/propagators.py` & `valphi-0.4.0/valphi/propagators.py`

 * *Files identical despite different names*

### Comparing `valphi-0.3.34/setup.py` & `valphi-0.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['distlib>=0.3.6,<0.4.0', 'dumbo-asp>=0.0.37,<0.0.38', 'pydot>=1.4.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'valphi',
-    'version': '0.3.34',
+    'version': '0.4.0',
     'description': 'Logic programs ralying on ValPhi semantics',
     'long_description': 'None',
     'author': 'Mario Alviano',
     'author_email': 'mario.alviano@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

