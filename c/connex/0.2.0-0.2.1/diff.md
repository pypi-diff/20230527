# Comparing `tmp/connex-0.2.0.tar.gz` & `tmp/connex-0.2.1.tar.gz`

## Comparing `connex-0.2.0.tar` & `connex-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 connex-0.2.0/connex/__init__.py
--rw-r--r--   0        0        0    35120 2020-02-02 00:00:00.000000 connex-0.2.0/connex/_network.py
--rw-r--r--   0        0        0    44763 2020-02-02 00:00:00.000000 connex-0.2.0/connex/_plasticity.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 connex-0.2.0/connex/_utils.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 connex-0.2.0/connex/nn/__init__.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 connex-0.2.0/connex/nn/_dense_mlp.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 connex-0.2.0/connex/nn/_mlp.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 connex-0.2.0/connex/nn/_utils.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 connex-0.2.0/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 connex-0.2.0/LICENSE
--rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 connex-0.2.0/README.md
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 connex-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    17767 2020-02-02 00:00:00.000000 connex-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 connex-0.2.1/connex/__init__.py
+-rw-r--r--   0        0        0    35145 2020-02-02 00:00:00.000000 connex-0.2.1/connex/_network.py
+-rw-r--r--   0        0        0    46899 2020-02-02 00:00:00.000000 connex-0.2.1/connex/_plasticity.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 connex-0.2.1/connex/_utils.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 connex-0.2.1/connex/nn/__init__.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 connex-0.2.1/connex/nn/_dense_mlp.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 connex-0.2.1/connex/nn/_mlp.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 connex-0.2.1/connex/nn/_utils.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 connex-0.2.1/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 connex-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 connex-0.2.1/README.md
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 connex-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    17782 2020-02-02 00:00:00.000000 connex-0.2.1/PKG-INFO
```

### Comparing `connex-0.2.0/connex/_network.py` & `connex-0.2.1/connex/_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -740,15 +740,17 @@
         self._dropout_array = dropout_array
         self._dropout_dict = dropout_dict
 
     #####################################################
     ################## Public methods ###################  # noqa: E266
     #####################################################
 
-    def set_dropout_p(self, dropout_p: Union[float, Mapping[Any, float]]) -> None:
+    def set_dropout_p(
+        self, dropout_p: Union[float, Mapping[Any, float]]
+    ) -> "NeuralNetwork":
         """Set the per-neuron dropout probabilities.
 
         **Arguments:**
 
         - `dropout_p`: Either a float or mapping from neuron (`Any`) to float. If a
             single float, all hidden neurons will have that dropout probability, and
             all input and output neurons will have dropout probability 0 by default.
```

### Comparing `connex-0.2.0/connex/_plasticity.py` & `connex-0.2.1/connex/_plasticity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1165,7 +1165,61 @@
             new_weights_and_biases,
             new_attention_params_neuron,
             new_attention_params_topo,
             new_topo_norm_params,
             new_adaptive_activation_params,
         ),
     )
+
+
+def set_dropout_p(
+    network: NeuralNetwork, dropout_p: Union[float, Mapping[Any, float]]
+) -> NeuralNetwork:
+    """Set the per-neuron dropout probabilities.
+
+    **Arguments:**
+
+    - `network`: The `NeuralNetwork` whose dropout probabilities will be modified.
+    - `dropout_p`: Either a float or mapping from neuron (`Any`) to float. If a
+        single float, all hidden neurons will have that dropout probability, and
+        all input and output neurons will have dropout probability 0 by default.
+        If a `Mapping`, it is assumed that `dropout_p` maps a neuron to its dropout
+        probability, and all unspecified neurons will retain their current dropout
+        probability.
+
+    **Returns:**
+
+    A copy of the network with dropout probabilities as specified.
+    The original network (including unspecified dropout probabilities) is left
+    unchanged.
+    """
+
+    def update_dropout_probabilities():
+        if isinstance(dropout_p, float):
+            hidden_dropout = {neuron: dropout_p for neuron in network._hidden_neurons}
+            input_output_dropout = {
+                neuron: 0.0
+                for neuron in network._input_neurons + network._output_neurons
+            }
+            return {**hidden_dropout, **input_output_dropout}
+        else:
+            assert isinstance(dropout_p, Mapping)
+            for n, d in dropout_p.items():
+                if n not in network._graph.nodes:
+                    raise ValueError(f"'{n}' is not present in the network.")
+                if not isinstance(d, float):
+                    raise TypeError(f"Invalid dropout value of {d} for neuron {n}.")
+                return {**network._dropout_dict, **dropout_p}
+
+    dropout_dict = update_dropout_probabilities()
+    dropout_array = jnp.array(
+        [dropout_dict[neuron] for neuron in network._topo_sort], dtype=float
+    )
+
+    assert jnp.all(jnp.greater_equal(dropout_array, 0))
+    assert jnp.all(jnp.less_equal(dropout_array, 1))
+
+    return eqx.tree_at(
+        lambda network: (network._dropout_dict, network._dropout_array),
+        network,
+        (dropout_dict, dropout_array),
+    )
```

### Comparing `connex-0.2.0/connex/_utils.py` & `connex-0.2.1/connex/_utils.py`

 * *Files identical despite different names*

### Comparing `connex-0.2.0/connex/nn/_dense_mlp.py` & `connex-0.2.1/connex/nn/_dense_mlp.py`

 * *Files identical despite different names*

### Comparing `connex-0.2.0/connex/nn/_mlp.py` & `connex-0.2.1/connex/nn/_mlp.py`

 * *Files identical despite different names*

### Comparing `connex-0.2.0/LICENSE` & `connex-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `connex-0.2.0/README.md` & `connex-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 # Add connections
 network = cnx.add_connections(network, [(1, 6), (2, 11)])
 
 # Remove neuron
 network = cnx.remove_neurons(network, [9])
 
 # Set dropout probability
-network.set_dropout_p(0.1)
+network = cnx.set_dropout_p(network, 0.1)
 ```
 
 That's all there is to it.  The new connections have been initialized with untrained parameters, and the neurons in the original network that have not been removed (along with their respective incoming and outgoing connections) have retained their trained parameters. Furthermore, since a `connex.NeuralNetwork` is an `equinox.Module`, it can seamlessly be used as a submodule inside other Equinox Modules.
 
 For more information about manipulating connectivity structure and the `NeuralNetwork` base class, please see the API section of the documentation. For examples of subclassing `NeuralNetwork`, please see `connex.nn`.
 
 ## Citation
```

### Comparing `connex-0.2.0/pyproject.toml` & `connex-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "connex"
-version = "0.2.0"
+version = "0.2.1"
 description = "Making neural networks more neural."
 readme = "README.md"
 requires-python ="~=3.8"
 license = {file = "LICENSE"}
 authors = [
   {name = "Leonard Gleyzer", email = "lenny@lenn.ai"},
 ]
```

### Comparing `connex-0.2.0/PKG-INFO` & `connex-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connex
-Version: 0.2.0
+Version: 0.2.1
 Summary: Making neural networks more neural.
 Project-URL: repository, https://github.com/leonard-gleyzer/connex
 Author-email: Leonard Gleyzer <lenny@lenn.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -327,15 +327,15 @@
 # Add connections
 network = cnx.add_connections(network, [(1, 6), (2, 11)])
 
 # Remove neuron
 network = cnx.remove_neurons(network, [9])
 
 # Set dropout probability
-network.set_dropout_p(0.1)
+network = cnx.set_dropout_p(network, 0.1)
 ```
 
 That's all there is to it.  The new connections have been initialized with untrained parameters, and the neurons in the original network that have not been removed (along with their respective incoming and outgoing connections) have retained their trained parameters. Furthermore, since a `connex.NeuralNetwork` is an `equinox.Module`, it can seamlessly be used as a submodule inside other Equinox Modules.
 
 For more information about manipulating connectivity structure and the `NeuralNetwork` base class, please see the API section of the documentation. For examples of subclassing `NeuralNetwork`, please see `connex.nn`.
 
 ## Citation
```

