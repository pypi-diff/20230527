# Comparing `tmp/nnx-0.0.2.tar.gz` & `tmp/nnx-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnx-0.0.2.tar", max compression
+gzip compressed data, was "nnx-0.0.3.tar", max compression
```

## Comparing `nnx-0.0.2.tar` & `nnx-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0     1072 2023-03-18 22:40:31.494888 nnx-0.0.2/LICENSE
--rw-r--r--   0        0        0    13864 2023-04-26 21:37:05.662113 nnx-0.0.2/README.md
--rw-r--r--   0        0        0      776 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/__init__.py
--rw-r--r--   0        0        0     2235 2023-04-08 23:38:12.700869 nnx-0.0.2/nnx/fields.py
--rw-r--r--   0        0        0     3789 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/filters.py
--rw-r--r--   0        0        0      140 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/nn/__init__.py
--rw-r--r--   0        0        0     1076 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/nn/activations.py
--rw-r--r--   0        0        0     2764 2023-04-08 19:11:50.337195 nnx-0.0.2/nnx/nn/dtypes.py
--rw-r--r--   0        0        0     1888 2023-04-08 18:42:49.425089 nnx-0.0.2/nnx/nn/initializers.py
--rw-r--r--   0        0        0    13270 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/nn/linear.py
--rw-r--r--   0        0        0     7341 2023-04-25 22:58:04.568349 nnx-0.0.2/nnx/nn/module.py
--rw-r--r--   0        0        0    10680 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/nn/normalization.py
--rw-r--r--   0        0        0     2250 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/nn/stochastic.py
--rw-r--r--   0        0        0     2431 2023-04-10 14:13:14.802122 nnx-0.0.2/nnx/partitioning.py
--rw-r--r--   0        0        0     2417 2023-03-30 22:50:08.758780 nnx-0.0.2/nnx/rng_stream.py
--rw-r--r--   0        0        0     5483 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/scope_lib.py
--rw-r--r--   0        0        0     6838 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/transforms.py
--rw-r--r--   0        0        0      563 2023-04-22 15:20:28.647804 nnx-0.0.2/nnx/utils.py
--rw-r--r--   0        0        0      751 2023-04-26 21:37:25.371790 nnx-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    14363 1970-01-01 00:00:00.000000 nnx-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-18 22:40:31.494888 nnx-0.0.3/LICENSE
+-rw-r--r--   0        0        0    11445 2023-05-27 00:26:17.305700 nnx-0.0.3/README.md
+-rw-r--r--   0        0        0     1525 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/__init__.py
+-rw-r--r--   0        0        0     5317 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/context.py
+-rw-r--r--   0        0        0     4133 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/dataclasses.py
+-rw-r--r--   0        0        0     2967 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/filters.py
+-rw-r--r--   0        0        0     6669 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/module.py
+-rw-r--r--   0        0        0        0 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/nn/__init__.py
+-rw-r--r--   0        0        0     1076 2023-04-22 15:20:28.647804 nnx-0.0.3/nnx/nn/activations.py
+-rw-r--r--   0        0        0     2764 2023-04-08 19:11:50.337195 nnx-0.0.3/nnx/nn/dtypes.py
+-rw-r--r--   0        0        0     1888 2023-04-08 18:42:49.425089 nnx-0.0.3/nnx/nn/initializers.py
+-rw-r--r--   0        0        0    16162 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/nn/linear.py
+-rw-r--r--   0        0        0    13710 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/nn/normalization.py
+-rw-r--r--   0        0        0     2283 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/nn/stochastic.py
+-rw-r--r--   0        0        0     5888 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/partitioning.py
+-rw-r--r--   0        0        0     8591 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/pytree.py
+-rw-r--r--   0        0        0     2807 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/ref_field.py
+-rw-r--r--   0        0        0    19755 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/reference.py
+-rw-r--r--   0        0        0     1185 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/tracers.py
+-rw-r--r--   0        0        0     6423 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/transforms.py
+-rw-r--r--   0        0        0      873 2023-05-27 00:26:17.305700 nnx-0.0.3/nnx/utils.py
+-rw-r--r--   0        0        0      682 2023-05-27 00:28:08.259906 nnx-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    11924 1970-01-01 00:00:00.000000 nnx-0.0.3/PKG-INFO
```

### Comparing `nnx-0.0.2/LICENSE` & `nnx-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nnx-0.0.2/README.md` & `nnx-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,105 +1,126 @@
+Metadata-Version: 2.1
+Name: nnx
+Version: 0.0.3
+Summary: 
+Author: Cristian Garcia
+Author-email: cgarcia.e88@gmail.com
+Requires-Python: >=3.8,<3.12
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: jax
+Requires-Dist: jaxlib
+Description-Content-Type: text/markdown
+
 # nnx
 
-_**N**erual **N**etworks for JA**X**_
+_**N**eural **N**etworks for JA**X**_
+
+`nnx` is a Neural Networks library for JAX that uses Pytree-based Modules and a novel 
+a **Ref**erence system to enable:
+
+* **Simplicity**: Provides an easy-to-understand mental model and implementation.
+* **Shared refereces**: Supports **safe** mutable shared state thanks to its **Ref**erence system.
+* **Leaf Metadata**: Enables semantic splitting a Module's state (similar to Flax collections) and adding [Axis Metadata](https://github.com/google/flax/blob/main/docs/flip/2434-general-metadata.md#flip-axis-metadata). 
+* **Stateful transformations**: Seamless integration with JAX's native transformation capabilities.
 
-`nnx` is a lightweight module system for JAX that provides the same power as `flax` but with a simpler mental model and implementation closer to `equinox`. It is built on top of `refx`, which enables shared state, tractable mutability, and semantic partitioning. `nnx` also supports stateful transformations, allowing you to train your models efficiently.
+NNX was designed to have the same capabilities as Flax with the simplicity of Equinox.
 
 ## Status
 
-`nnx` is currently a proof of concept, it is meant to explore the design space of a lightweight module system for JAX based on Refx.
+`nnx` is currently a proof of concept, aimed at exploring the design space of a lightweight module 
+system for JAX based on references. It is not intended for production use.
 
 ## Installation
 
 To get started with `nnx`, first install the package using pip:
 
 ```
 pip install nnx
 ```
+To get the latest version, install directly from GitHub:
+
+```
+pip install git+https://github.com/cgarciae/nnx
+```
 
 ## Usage
 
 ```python
 import nnx
 import jax
 
 class Linear(nnx.Module):
     w: jax.Array = nnx.param()
     b: jax.Array = nnx.param()
 
-    def __init__(self, din: int, dout: int):
-        key = self.make_rng("params")
+    def __init__(self, din: int, dout: int, *, ctx: nnx.Context):
+        key = ctx.make_rng("params")
         self.w = jax.random.uniform(key, (din, dout))
         self.b = jax.numpy.zeros((dout,))
 
     def __call__(self, x):
         return x @ self.w + self.b
 
-model = Linear.init(jax.random.PRNGKey(0))(din=12, dout=2)
+ctx = nnx.Context(params=jax.random.PRNGKey(0))
+model = Linear(din=12, dout=2, ctx=ctx)
 
 @nnx.jit
 def train_step(model, x, y):
     def loss_fn(model):
         y_pred = model(x)
         return jax.numpy.mean((y_pred - y) ** 2)
     
-    grad = nnx.grad(loss_fn, wrt="params")(model)
-    model["params"] = jax.tree_map(lambda w, g: w - 0.1 * g, model["params"], grad)
+    # compute gradient
+    grads = nnx.grad(loss_fn, wrt="params")(model)
+    # SGD update
+    model[:] = jax.tree_map(lambda w, g: w - 0.1 * g, model["params"], grads)
 
 # yes... there's no return :)
 train_step(model, x, y)
 ```
 
 ## Design
 
 ### Modules
 
-<!-- * Modules are Pytrees
-* `nnx.ref` and `nnx.param` mark ref fields, `params` is just a shorthand for `ref("params"), these are descriptor object (more info later)
-* `make_rng` is similar to flax's `make_rng`, distributes RNG keys through global state
-* the `init` and `apply` method lets you set the global state including RNG keys -->
-
-NNX `Module`s are [simple_pytree](https://github.com/cgarciae/simple-pytree) Pytrees with a few additional features to make them more easier to use with `refx` references. A custom Module can be created simply by
-subclassing `nnx.Module` and marking which fields are references with `nnx.ref` or `nnx.param`, as we will explain later, these are descriptors that store a `Ref` instance in a separate attribute and make using references transparent to the user.
+`nnx` has a simple and intuitive design with Modules at its core. These modules are built using [simple_pytree](https://github.com/cgarciae/simple-pytree) Pytrees. To create a custom module, simply subclass `nnx.Module` and mark the reference fields with `nnx.ref` or `nnx.param`. These are descriptors that store a `Ref` instance in a separate attribute, making references transparent to the user.
 
-Here is an example of a simple `Linear` module:
+Here's an example of a simple `Linear` module:
 
 ```python
 import nnx
 import jax
 
 class Linear(nnx.Module):
     w: jax.Array = nnx.ref("params")
     b: jax.Array = nnx.param() # shortcut for ref("params")
 
-    def __init__(self, din: int, dout: int):
-        key = self.make_rng("params") # request an RNG key
+    def __init__(self, din: int, dout: int, *, ctx: nnx.Context):
+        key = ctx.make_rng("params") # request an RNG key
         self.w = jax.random.uniform(key, (din, dout))
         self.b = jax.numpy.zeros((dout,))
 
     def __call__(self, x):
         return x @ self.w + self.b
-```
-NNX offers the same `make_rng` API as Flax to distribute RNG keys where they are needed, it does this by storing RNG keys in a global state and carefully handling them with context managers. You can set the state for the RNG keys and other flags via the `init` and `apply` methods, which are similar to Flax's `init` and `apply` methods but designed to be friendlier with static analysis tools.
 
-```python
-# global state ==>  .....................
-model = Linear.init(jax.random.PRNGKey(0))(din=12, dout=2)
-#                    constructor args ==> ^^^^^^^^^^^^^^^^
+ctx = nnx.Context(params=jax.random.PRNGKey(0))
+model = Linear(din=12, dout=2, ctx=ctx)
 ```
-If global state is not needed you can just use the constructor directly.
+
+`nnx` uses a `Context` object to propagate RNG and other forms of state throughout the model. `Context` provides a `make_rng` method that creates a new RNG key on demand for a given name (in this case, `"params"`).
 
 #### RefField Descriptor
-<!-- * `ref` and `params` create a `RefField` descriptor instances
-* `RefField` descriptors inherit from `dataclasses.Field` in order to be compatible with `dataclasses` when needed
-* `RefField` descriptors are descriptors that store a `Ref` instance in a separate `{name}__ref` attribute, this makes using references transparent to the user -->
 
-`nnx.ref` and `nnx.param` are descriptors that create `RefField` instances. `RefField` is a descriptor that stores a `Ref` instance in a separate `{attribute_name}__ref` attribute, and handle retrieving and setting the value of the reference automatically so that the user doesn't have to manipulate references directly. `RefField` inherits from `dataclasses.Field` in order to be compatible with `dataclasses` when needed.
+`nnx.ref` and `nnx.param` are descriptors that create `RefField` instances. A `RefField` is a descriptor that stores a `Ref` instance in a separate `{attribute_name}__ref` attribute. It handles retrieving and setting the value of the reference automatically, so the user doesn't have to manipulate references directly. Additionally, `RefField` inherits from `dataclasses.Field` to ensure compatibility with `nnx.dataclass` when needed.
 
-Here is a simplified version of how `RefField` is implemented:
+Here's a simplified version of the `RefField` implementation:
 
 ```python
 class RefField(dataclasses.Field):
     def __set_name__(self, cls, name):
         self.name = name
 
     def __get__(self, obj, objtype=None):
@@ -107,180 +128,155 @@
         return ref.value
 
     def __set__(self, obj, value):
         ref = getattr(obj, f"{self.name}__ref")
         ref.value = value
 ```
 
-The only thing to note here is that `Ref`s are created during the first call to `__set__` if the companion `{name}__ref` attribute doesn't exist yet. This should only happen during `__init__` or else `Module` will raise an error as `simple_pytree` Pytrees are frozen after initialization.
+It's important to note that `Ref` instances are created during the first call to `__set__` if the companion `{name}__ref` attribute doesn't exist yet. This should only happen inside the `__init__` method, otherwise, the `Module` will raise an error, as `simple_pytree` Pytrees are frozen after initialization.
 
-#### GetItem and SetItem syntactic sugar
-<!-- * `__getitem__` and `__setitem__` are syntactic sugar for `get_partition` and `update_refs`
-* they don't actually update the Module structure despite the appearance, they just update the references values -->
+#### GetItem and SetItem Syntactic Sugar
 
-`Module` implements `__getitem__` and `__setitem__` to provide syntactic sugar for creating and updating `Partition`s. Despite the appearance, `__setitem__` does not modify the Module's structure, it just updates the values of the references as can be seen in this simplified implementation:
+`Module` implements `__getitem__` and `__setitem__` to provide syntactic sugar for creating and updating `Partition`s. Although it may appear otherwise, `__setitem__` does not modify the Module's structure. Instead, it updates the values of the references, as demonstrated in this simplified implementation:
 
 ```python
-class Module(simple_pytree.Pytree):
+class Module(nnx.Pytree):
     ...
-    def __getitem__(self, collection: str) -> refx.Partition:
-        derefed_module = refx.deref(self)[0]
-        return nnx.get_partition(derefed_module, collection)
+    def __getitem__(self, collection: str) -> nnx.Partition:
+        return nnx.get_partition(self, collection)
 
-    def __setitem__(self, collection: str, updates: refx.Partition):
-        partition = nnx.get_partition(self, collection)
-        refx.update_refs(partition, updates)
+    def __setitem__(self, _: SetItemType, value: nnx.Partition):
+        nnx.update_refs(self, value)
 ```
 
-Sample usage could look something like this:
+Sample usage might look like this:
 
 ```python
-model["params"] = jax.tree_map(lambda w, g: w - 0.1 * g, model["params"], grad)
+# SGD update
+model[:] = jax.tree_map(lambda w, g: w - 0.1 * g, model["params"], grads)
 ```
 
-Here `model["params"]` is a `Partition` that contains all the references in the `params` collection, and `grad` is a `Partition` with the same structure as `model["params"]` but with gradients instead of parameters. `moduel["params"] = ...` updates the values of the references in `model["params"]` with the values of the `sdg` update.
+In this example, `model["params"]` returns a `Partition` that contains all the references in the `params` collection. `grads` is a `Partition` with the same structure as `model["params"]`, but with gradients instead of parameters. The statement `model[:] = ...` updates the values of the references in `model` with the values of the new parameters from stochastic gradient descent (SGD) update rule.
 
 ### Transformations
 
-<!-- * 3 types of transformations: stateful, filtered, and the partition API
-* a final API would probably have a mix of the 3 -->
-
-Currently NNX offers 3 types of transformations: stateful, filtered, and the partition API. At the moment its not clear which API is the best, the 3 will be kept for now.
+Currently, NNX offers three types of transformations: stateful, filtered, and the partition API. As it is unclear which API is the best, all three will be maintained for now.
 
 #### Stateful Transforms
 
-<!-- * stateful transformations take a pytree/Module of references as its first argument
-* use `deref` and `reref` to move the pytree/Module across the transformation
-* handle all relevant global state such as `nnx.scope` and Refx's trace state
-* their main feature is that they always update the state of the references of the input pytree/Module -->
-
-Stateful Transforms take a pytree of references (e.g. a Module) as their first argument, track changes in the state of the references that happen inside the transformation, and automatically propagate those changes to the input pytree outside the transformation. In general they have the following properties:
-
-* they behave as stateful functions w.r.t. the first argument
-* they can operate on collections and RNG streams according to the transformation's semantics, exactly like Flax's transformations
-* they take care of handling all relevant global state such as `nnx.scope` and Refx's trace state
-    
-Here is a diagram of how stateful transformations work:
+Stateful transforms take a Pytree of references (e.g., a Module) as their first argument, track changes in the state of the references that occur within the transformation, and automatically propagate those changes to the input Pytree outside the transformation. In general, they have the following properties:
 
-![stateful-transforms](https://raw.githubusercontent.com/cgarciae/nnx/main/docs/images/stateful-transforms.png)
+* They behave as stateful functions with respect to the first argument.
+* They can operate on collections and RNG streams according to the transformation's semantics, exactly like Flax's transformations.
+* They handle all relevant global state, such as `nnx.scope` and Refx's trace state.
+
+Here's a diagram illustrating how stateful transformations work:
 
-<!-- * `nnx.jit` and `nnx.grad` are stateful transformations -->
+![stateful-transforms](https://raw.githubusercontent.com/cgarciae/nnx/main/docs/images/stateful-transforms.png)
 
-Currently `nnx.jit` and `nnx.grad` are the only stateful transformations.
+Currently, `nnx.jit` and `nnx.grad` are the only stateful transformations.
 
-Here is how a `train_step` function could be implemented using `nnx.jit` and `nnx.grad`:
+The following example demonstrates how a `train_step` function can be implemented using `nnx.jit` and `nnx.grad`:
 
 ```python
 @nnx.jit
 def train_step(model, x, y):
 
     def loss_fn(model):
         y_pred = model(x)
         return jax.numpy.mean((y_pred - y) ** 2)
     
     # compute gradient
-    grad = nnx.grad(loss_fn, wrt="params")(model)
-    # sdg update
-    model["params"] = jax.tree_map(lambda w, g: w - 0.1 * g, model["params"], grad)
+    grads = nnx.grad(loss_fn, wrt="params")(model)
+    # SGD update
+    model[:] = jax.tree_map(lambda w, g: w - 0.1 * g, model["params"], grads)
 
-# stateful update, no return !!!
+# stateful update, no return needed
 train_step(model, x, y)
 ```
 
-<!-- * probably the most "interesting" part of the design is that code looks very imperative
-* state is automatically propagated in and out of the transformation -->
+The most interesting aspect of this design is that the code appears very imperative, as the state is automatically propagated in and out of the transformations. However, more consideration is needed to properly support `jit`'s `in_shardings` and `out_shardings` arguments.
 
-The most interesting part of the design is that the code looks very imperative since the state is automatically propagated in and out of the transformations. However, more thought is needed to see how to correctly support `jit`'s `in_shardings` and `out_shardings` arguments.
+Certainly! I've revised the text to improve clarity and readability. Here are the updated sections:
 
+---
 #### Filtered Transformations
 
-<!-- * filtered transformations `deref` and `reref` all their inputs and outputs to move the pytree/Modules across the transformation
-* they don't handle any global state, the must semantically behave as pure functions -->
-
-Filtered transformations are more flexible in that they can take pytrees of references in any of their arguments and also return pytrees of references. They just `deref` and `reref` all their inputs and outputs to move the pytrees across the transformation. In general they have the following properties:
+Filtered transformations offer more flexibility, as they can take Pytrees of references in any of their arguments and return Pytrees of references. They simply `deref` and `reref` all their inputs and outputs to transfer the Pytrees across the transformation. In general, they have the following properties:
 
-* they behave as pure functions
-* they don't handle any global state except for Refx's trace state
+* They behave as pure functions.
+* They don't handle any global state except for Refx's trace state.
 
 ![filtered-transforms](https://raw.githubusercontent.com/cgarciae/nnx/main/docs/images/filtered-transforms.png)
 
-<!-- * `nnx.jit_filter` is a filtered transformation, `nnx.grad` is a stateful transformation -->
-
-Currently `nnx.jit_filter` is the only filtered transformation.
+Currently, `nnx.jit_filter` is the only filtered transformation.
 
-Here is how a `train_step` function could be implemented using `nnx.jit_filter` and `nnx.grad`:
+Here's an example of how a `train_step` function can be implemented using `nnx.jit_filter` and `nnx.grad`:
 
 ```python
 @nnx.jit_filter
 def train_step(model, x, y):
 
     def loss_fn(model):
         y_pred = model(x)
         return jax.numpy.mean((y_pred - y) ** 2)
 
     # compute gradient
-    grad = nnx.grad(loss_fn, wrt="params")(model)
-    # sdg update                   |--------sdg-----------|
-    model["params"] = jax.tree_map(lambda w, g: w - 0.1 * g, model["params"], grad)
+    grads = nnx.grad(loss_fn, wrt="params")(model)
+    # SGD update
+    model[:] = jax.tree_map(lambda w, g: w - 0.1 * g, model["params"], grads)
     
     return model
 
 model = train_step(model, x, y)
 ```
 
-<!-- * filtered transformations must output any state that they want to propagate but have more flexibility in how they handle it -->
-
-Filtered transformations must output any state that they want to propagate but have more flexibility in how they handle it. Adding support for `jit`'s `in_shardings` and `out_shardings` arguments is probably more straightforward than with stateful transformations.
-
+Filtered transformations must output any state they want to propagate but have more flexibility in how they handle it. Adding support for `jit`'s `in_shardings` and `out_shardings` arguments is likely more straightforward than with stateful transformations.
 
 #### Partition API
 
-<!-- * the partition API mimicks Flax's `variables` + `apply` API
-* it splits a pytree/Module into all its `Partition`s + a `ModuleDef` object
-* each `Partition` is a flat dictionary so it works with regular JAX transformations -->
-
-The partition API mimicks Flax's `variables` plus `apply` API. It splits a pytree of references into all its `Partition`s and creates a `ModuleDef` object that knows how to reconstruct the original pytree from the `Partition`s. Since each `Partition` is a flat dictionary, this API works with regular JAX transformations.
- 
-Here is a diagram of how the partition API works:
+The partition API enables splitting a Module's state into sets of reference-less `Partition`s, this provides a general way of interacting with vanilla JAX transformations.
+
 
 ![partition-api](https://raw.githubusercontent.com/cgarciae/nnx/main/docs/images/partition-api.png)
 
-Here is an example of how to use the partition API:
+Here's an example of how a `train_step` function can be implemented using the partition API:
 
 ```python
-model: ModuleDef
-partitions, model = model.partition()
+modeldef: ModuleDef[Linear]
+partitions, modeldef = model.partition()
 params = partitions["params"]
 
 @jax.jit
 def train_step(params, x, y):
 
-    def loss_fn(params): #      |----merge----|
-        y_pred, updates = model.apply([params])(x)
+    def loss_fn(params):
+        model: Linear = modeldef.reref(params)
+        y_pred = model(x)
         return jax.numpy.mean((y_pred - y) ** 2)
 
     # compute gradient
-    grad = jax.grad(loss_fn)(params)
-    # sdg update          |--------sdg-----------|
-    params = jax.tree_map(lambda w, g: w - 0.1 * g, params, grad)
+    grads = jax.grad(loss_fn)(params)
+    # SGD update
+    params = jax.tree_map(lambda w, g: w - 0.1 * g, params, grads)
     
     return params
 
 params = train_step(params, x, y)
 ```
 
-The main benefit of the partition API is that its more compatible with other JAX tools as the training step can be written using regular JAX transformations. The main drawback is that it's more verbose and users have to manually keep track of all the partitions, this overhead is often what makes `flax` and `haiku` a bit harder to learn than other frameworks like `pytorch` and `keras`.
+The main benefit of the partition API is its compatibility with other JAX tools, as the training step can be written using regular JAX transformations. The main drawback is that it's more verbose.
 
 ### Case Studies
 
 #### Shared State
 
-In `nnx`, it's possible to create modules that share state between each other. This can be useful when designing complex neural network architectures, as it allows you to reuse certain layers and reduce the number of learnable parameters.
+In NNX, you can create modules that share state between them. This is useful when designing complex neural network architectures, as it allows you to reuse certain layers and reduce the number of learnable parameters.
 
-Here's an example of how to create a module with shared state:
+Here's an example of creating a module with shared state:
 
 ```python
 class Block(nnx.Module):
     def __init__(self, linear: nnx.Linear):
         self.linear = linear
         self.bn = nnx.BatchNorm(2)
 
@@ -295,18 +291,19 @@
 
     def __call__(self, x):
         x = self.block1(x)
         x = self.block2(x)
         return x
 ```
 
-In this example, the `Model` module contains two instances of the `Block` module, each of which shares the same `nnx.Linear` module. To run the model you can use the `apply` method to set the `use_running_average` flag for all `BatchNorm` modules.
+In this example, the `Model` module contains two instances of the `Block` module. Each instance shares the same `nnx.Linear` module. To run the model, you can use the `apply` method to set the `use_running_average` flag for all `BatchNorm` modules.
 
-Here's an example of how to compute the loss for a `Model` instance:
+Here's an example of computing the loss for a `Model` instance:
 
 ```python
 def loss_fn(model: Model, x: jax.Array, y: jax.Array):
     y_pred = model.apply(use_running_average=False)(x)
     return jnp.mean((y - y_pred) ** 2)
 ```
 
-It's worth noting that the state for the shared `nnx.Linear` module will be kept in sync at all times on both `Block` instances, including during gradient updates.
+It's important to note that the state for the shared `nnx.Linear` module will be kept in sync at all times on both `Block` instances, including during gradient updates.
+
```

### Comparing `nnx-0.0.2/nnx/nn/activations.py` & `nnx-0.0.3/nnx/nn/activations.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.2/nnx/nn/dtypes.py` & `nnx-0.0.3/nnx/nn/dtypes.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.2/nnx/nn/initializers.py` & `nnx-0.0.3/nnx/nn/initializers.py`

 * *Files identical despite different names*

### Comparing `nnx-0.0.2/nnx/nn/linear.py` & `nnx-0.0.3/nnx/nn/linear.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import dataclasses
 import typing as tp
 
 import jax
 from jax import lax
 import jax.numpy as jnp
 import numpy as np
+from nnx import context
 
-from nnx.nn.module import Module
+from nnx.module import Module
 from nnx.nn import initializers
-from nnx import fields
+from nnx.dataclasses import dataclass, param
 from nnx.nn import dtypes
 
 Array = jax.Array
 PRNGKey = tp.Any
 Shape = tp.Tuple[int, ...]
 Dtype = tp.Any  # this could be a real type?
 PrecisionLike = tp.Union[
@@ -55,57 +57,64 @@
     ndim = len(input_shape)
     lhs_spec = (0, ndim - 1) + tuple(range(1, ndim - 1))
     rhs_spec = (ndim - 1, ndim - 2) + tuple(range(0, ndim - 2))
     out_spec = lhs_spec
     return lax.ConvDimensionNumbers(lhs_spec, rhs_spec, out_spec)
 
 
-@fields.dataclass
 class Linear(Module):
     """A linear transformation applied over the last dimension of the input.
 
     Attributes:
       features: the number of output features.
       use_bias: whether to add a bias to the output (default: True).
       dtype: the dtype of the computation (default: infer from input and params).
       param_dtype: the dtype passed to parameter initializers (default: float32).
       precision: numerical precision of the computation see `jax.lax.Precision`
         for details.
       kernel_init: initializer function for the weight matrix.
       bias_init: initializer function for the bias.
     """
 
-    in_features: int = fields.static_field()
-    out_features: int = fields.static_field()
-    use_bias: bool = fields.static_field(default=True)
-    dtype: tp.Optional[Dtype] = fields.static_field(default=None)
-    param_dtype: Dtype = fields.static_field(default=jnp.float32)
-    precision: PrecisionLike = fields.static_field(default=None)
-    kernel_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = fields.static_field(
-        default=default_kernel_init
-    )
-    bias_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = fields.static_field(
-        default=initializers.zeros()
-    )
-    dot_general: DotGeneralT = fields.static_field(default=lax.dot_general)
     # ref fields
-    kernel: Array = fields.param(init=False)
-    bias: tp.Optional[Array] = fields.param(init=False)
+    kernel: Array = param()
+    bias: tp.Optional[Array] = param()
 
-    def __post_init__(self):
-        kernel_key = self.make_rng("params")
-        self.kernel = self.kernel_init(
-            kernel_key, (self.in_features, self.out_features), self.param_dtype
-        )
-        if self.use_bias:
-            bias_key = self.make_rng("params")
-            self.bias = self.bias_init(bias_key, (self.out_features,), self.param_dtype)
+    def __init__(
+        self,
+        in_features: int,
+        out_features: int,
+        *,
+        use_bias: bool = True,
+        dtype: tp.Optional[Dtype] = None,
+        param_dtype: Dtype = jnp.float32,
+        precision: PrecisionLike = None,
+        kernel_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = default_kernel_init,
+        bias_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = initializers.zeros(),
+        dot_general: DotGeneralT = lax.dot_general,
+        ctx: context.Context,
+    ):
+        kernel_key = ctx.make_rng("params")
+        self.kernel = kernel_init(kernel_key, (in_features, out_features), param_dtype)
+        if use_bias:
+            bias_key = ctx.make_rng("params")
+            self.bias = bias_init(bias_key, (out_features,), param_dtype)
         else:
             self.bias = None
 
+        self.in_features = in_features
+        self.out_features = out_features
+        self.use_bias = use_bias
+        self.dtype = dtype
+        self.param_dtype = param_dtype
+        self.precision = precision
+        self.kernel_init = kernel_init
+        self.bias_init = bias_init
+        self.dot_general = dot_general
+
     def __call__(self, inputs: Array) -> Array:
         """Applies a linear transformation to the inputs along the last dimension.
 
         Args:
           inputs: The nd-array to be transformed.
 
         Returns:
@@ -124,15 +133,14 @@
             precision=self.precision,
         )
         if bias is not None:
             y += jnp.reshape(bias, (1,) * (y.ndim - 1) + (-1,))
         return y
 
 
-@fields.dataclass
 class Conv(Module):
     """Convolution Module wrapping `lax.conv_general_dilated[_local]`.
 
     Attributes:
       features: number of convolution filters.
       kernel_size: shape of the convolutional kernel. For 1D convolution,
         the kernel size can be passed as an integer. For all other cases, it must
@@ -163,70 +171,78 @@
       param_dtype: the dtype passed to parameter initializers (default: float32).
       precision: numerical precision of the computation see `jax.lax.Precision`
         for details.
       kernel_init: initializer for the convolutional kernel.
       bias_init: initializer for the bias.
     """
 
-    in_features: int = fields.static_field()
-    out_features: int = fields.static_field()
-    kernel_size: tp.Sequence[int] = fields.static_field()
-    strides: tp.Union[None, int, tp.Sequence[int]] = fields.static_field(default=1)
-    padding: PaddingLike = fields.static_field(default="SAME")
-    input_dilation: tp.Union[None, int, tp.Sequence[int]] = fields.static_field(
-        default=1
-    )
-    kernel_dilation: tp.Union[None, int, tp.Sequence[int]] = fields.static_field(
-        default=1
-    )
-    feature_group_count: int = fields.static_field(default=1)
-    use_bias: bool = fields.static_field(default=True)
-    mask_fn: tp.Optional[tp.Callable[[Array], Array]] = fields.static_field(
-        default=None
-    )
-    dtype: tp.Optional[Dtype] = fields.static_field(default=None)
-    param_dtype: Dtype = fields.static_field(default=jnp.float32)
-    precision: PrecisionLike = fields.static_field(default=None)
-    kernel_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = fields.static_field(
-        default=default_kernel_init
-    )
-    bias_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = fields.static_field(
-        default=initializers.zeros()
-    )
-    conv_general_dilated: ConvGeneralDilatedT = fields.static_field(
-        default=lax.conv_general_dilated
-    )
-    # ref fields
-    kernel: Array = fields.param(init=False)
-    bias: tp.Optional[Array] = fields.param(init=False)
+    kernel: Array = param()
+    bias: tp.Optional[Array] = param()
 
-    def __post_init__(self):
-        if isinstance(self.kernel_size, int):
+    def __init__(
+        self,
+        in_features: int,
+        out_features: int,
+        kernel_size: tp.Sequence[int],
+        strides: tp.Union[None, int, tp.Sequence[int]] = 1,
+        *,
+        padding: PaddingLike = "SAME",
+        input_dilation: tp.Union[None, int, tp.Sequence[int]] = 1,
+        kernel_dilation: tp.Union[None, int, tp.Sequence[int]] = 1,
+        feature_group_count: int = 1,
+        use_bias: bool = True,
+        mask_fn: tp.Optional[tp.Callable[[Array], Array]] = None,
+        dtype: tp.Optional[Dtype] = None,
+        param_dtype: Dtype = jnp.float32,
+        precision: PrecisionLike = None,
+        kernel_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = default_kernel_init,
+        bias_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = initializers.zeros(),
+        conv_general_dilated: ConvGeneralDilatedT = lax.conv_general_dilated,
+        ctx: context.Context,
+    ):
+        if isinstance(kernel_size, int):
             raise TypeError(
                 "Expected Conv kernel_size to be a"
                 " tuple/list of integers (eg.: [3, 3]) but got"
-                f" {self.kernel_size}."
+                f" {kernel_size}."
             )
         else:
-            self.kernel_size = tuple(self.kernel_size)
+            kernel_size = tuple(kernel_size)
 
-        kernel_shape = self.kernel_size + (
-            self.in_features // self.feature_group_count,
-            self.out_features,
+        kernel_shape = kernel_size + (
+            in_features // feature_group_count,
+            out_features,
         )
-        kernel_key = self.make_rng("params")
-        self.kernel = self.kernel_init(kernel_key, kernel_shape, self.param_dtype)
+        kernel_key = ctx.make_rng("params")
+        self.kernel = kernel_init(kernel_key, kernel_shape, param_dtype)
 
-        if self.use_bias:
-            bias_shape = (self.out_features,)
-            bias_key = self.make_rng("params")
-            self.bias = self.bias_init(bias_key, bias_shape, self.param_dtype)
+        if use_bias:
+            bias_shape = (out_features,)
+            bias_key = ctx.make_rng("params")
+            self.bias = bias_init(bias_key, bias_shape, param_dtype)
         else:
             self.bias = None
 
+        self.in_features = in_features
+        self.out_features = out_features
+        self.kernel_size = kernel_size
+        self.strides = strides
+        self.padding = padding
+        self.input_dilation = input_dilation
+        self.kernel_dilation = kernel_dilation
+        self.feature_group_count = feature_group_count
+        self.use_bias = use_bias
+        self.mask_fn = mask_fn
+        self.dtype = dtype
+        self.param_dtype = param_dtype
+        self.precision = precision
+        self.kernel_init = kernel_init
+        self.bias_init = bias_init
+        self.conv_general_dilated = conv_general_dilated
+
     def __call__(self, inputs: Array) -> Array:
         """Applies a (potentially unshared) convolution to the inputs.
 
         Args:
           inputs: input data with dimensions (*batch_dims, spatial_dims...,
             features). This is the channels-last convention, i.e. NHWC for a 2d
             convolution and NDHWC for a 3D convolution. Note: this is different from
@@ -325,7 +341,84 @@
             bias = bias.reshape((1,) * (y.ndim - bias.ndim) + bias.shape)
             y += bias
 
         if num_batch_dimensions != 1:
             output_shape = input_batch_shape + y.shape[1:]
             y = jnp.reshape(y, output_shape)
         return y
+
+
+default_embed_init = initializers.variance_scaling(1.0, "fan_in", "normal", out_axis=0)
+
+
+class Embed(Module):
+    """Embedding Module.
+
+    A parameterized function from integers [0, n) to d-dimensional vectors.
+
+    Attributes:
+      num_embeddings: number of embeddings.
+      features: number of feature dimensions for each embedding.
+      dtype: the dtype of the embedding vectors (default: same as embedding).
+      param_dtype: the dtype passed to parameter initializers (default: float32).
+      embedding_init: embedding initializer.
+    """
+
+    embedding: Array = param()
+
+    def __init__(
+        self,
+        num_embeddings: int,
+        features: int,
+        *,
+        dtype: tp.Optional[Dtype] = None,
+        param_dtype: Dtype = jnp.float32,
+        embedding_init: tp.Callable[
+            [PRNGKey, Shape, Dtype], Array
+        ] = default_embed_init,
+        ctx: context.Context,
+    ):
+        self.embedding = embedding_init(
+            ctx.make_rng("params"),
+            (num_embeddings, features),
+            param_dtype,
+        )
+
+        self.num_embeddings = num_embeddings
+        self.features = features
+        self.dtype = dtype or self.embedding.dtype
+        self.param_dtype = param_dtype
+        self.embedding_init = embedding_init
+
+    def __call__(self, inputs: Array) -> Array:
+        """Embeds the inputs along the last dimension.
+
+        Args:
+          inputs: input data, all dimensions are considered batch dimensions.
+
+        Returns:
+          Output which is embedded input data.  The output shape follows the input,
+          with an additional `features` dimension appended.
+        """
+        if not jnp.issubdtype(inputs.dtype, jnp.integer):
+            raise ValueError("Input type must be an integer or unsigned integer.")
+        # Use take because fancy indexing numpy arrays with JAX indices does not
+        # work correctly.
+        (embedding,) = dtypes.promote_dtype(
+            self.embedding, dtype=self.dtype, inexact=False
+        )
+        return jnp.take(embedding, inputs, axis=0)
+
+    def attend(self, query: Array) -> Array:
+        """Attend over the embedding using a query array.
+
+        Args:
+          query: array with last dimension equal the feature depth `features` of the
+            embedding.
+        Returns:
+          An array with final dim `num_embeddings` corresponding to the batched
+          inner-product of the array of query vectors against each embedding.
+          Commonly used for weight-sharing between embeddings and logit transform
+          in NLP models.
+        """
+        query, embedding = dtypes.promote_dtype(query, self.embedding, dtype=self.dtype)
+        return jnp.dot(query, embedding.T)
```

### Comparing `nnx-0.0.2/nnx/nn/module.py` & `nnx-0.0.3/nnx/module.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,92 @@
 import dataclasses
-import jax
-from simple_pytree import Pytree
+from nnx.pytree import Pytree
 from nnx import partitioning
-from nnx import scope_lib
-import refx
+from nnx.reference import (
+    NOTHING,
+    P,
+    DagDef,
+    Derefed,
+    Partition,
+    Referential,
+    clone,
+    deref,
+    reref,
+    update_refs,
+    _to_str_path,
+    _merge_partitions,
+)
 import typing as tp
 import jax.tree_util as jtu
+import builtins
 
+
+A = tp.TypeVar("A")
 M = tp.TypeVar("M", bound="Module")
 
 
+class ApplyCaller(tp.Protocol):
+    def __getattr__(self, __name) -> "ApplyCaller":
+        ...
+
+    def __call__(self, *args, **kwargs) -> tp.Tuple[tp.Any, tp.Dict[str, Partition]]:
+        ...
+
+
+class ModuleDef(DagDef[M]):
+    def apply(
+        self,
+        partitions: tp.Union[
+            Partition, tp.Tuple[Partition, ...], tp.Dict[str, Partition]
+        ],
+    ) -> ApplyCaller:
+        module: M = self.reref(partitions)
+
+        def _context(fn, *args, **kwargs) -> tp.Tuple[tp.Any, tp.Dict[str, Partition]]:
+            out = fn(*args, **kwargs)
+            updates, _ = module.partition()
+            return out, updates
+
+        return CallableProxy(_context, module)  # type: ignore
+
+
+class DerefedMod(tp.Tuple[P, ModuleDef[M]]):
+    @property
+    def partitions(self) -> P:
+        return self[0]
+
+    @property
+    def moduledef(self) -> ModuleDef[M]:
+        return self[1]
+
+    def reref(self) -> M:
+        return reref(self.partitions, self.moduledef)
+
+    @property
+    def apply(self) -> ApplyCaller:
+        return self.moduledef.apply(self.partitions)
+
+
+def _flatten_bounded(bounded: DerefedMod[P, M]):
+    return tuple(bounded), None
+
+
+def _unflatten_bounded(_, values):
+    return DerefedMod(values)
+
+
+jtu.register_pytree_node(DerefedMod, _flatten_bounded, _unflatten_bounded)
+
+
+if tp.TYPE_CHECKING:
+    SetItemType = tp.Union[builtins.ellipsis, builtins.slice]
+else:
+    SetItemType = tp.Any
+
+
 class _ProxyContext(tp.Protocol):
     def __call__(self, __fn: tp.Callable[..., tp.Any], *args, **kwargs) -> tp.Any:
         ...
 
 
 @dataclasses.dataclass
 class CallableProxy:
@@ -24,218 +97,148 @@
         return self._proxy_context(self._proxy_callable, *args, **kwargs)
 
     def __getattr__(self, name) -> "CallableProxy":
         return CallableProxy(self._proxy_context, getattr(self._proxy_callable, name))
 
 
 class Module(Pytree):
-    def deref(self: M) -> tp.Tuple[M, refx.DagDef]:
-        return refx.deref(self)
-
-    def reref(self: M, dagdef: refx.DagDef) -> M:
-        return refx.reref(self, dagdef)
+    def deref(self: M) -> DerefedMod[Partition, M]:
+        partition, dagdef = deref(self)
+        return DerefedMod((partition, ModuleDef.from_value(dagdef)))
 
     def clone(self: M) -> M:
-        return refx.clone(self)
+        return clone(self)
 
-    def make_rng(self, collection: str) -> jax.random.KeyArray:
-        return scope_lib.make_rng(collection)
+    @tp.overload
+    def __getitem__(self, collections: str) -> Partition:
+        ...
+
+    @tp.overload
+    def __getitem__(self, collections: tp.Tuple[str, ...]) -> tp.Tuple[Partition, ...]:
+        ...
 
-    def get_flag(self, name: str, default: tp.Any = dataclasses.MISSING) -> tp.Any:
-        return scope_lib.get_flag(name, default)
+    @tp.overload
+    def __getitem__(
+        self, collections: tp.Union[str, tp.Tuple[str, ...]]
+    ) -> tp.Union[Partition, tp.Tuple[Partition, ...]]:
+        ...
 
-    def __getitem__(self, collection: str) -> refx.Partition:
-        return partitioning.get_partition(self.deref()[0], collection)
+    def __getitem__(
+        self, collections: tp.Union[str, tp.Tuple[str, ...]]
+    ) -> tp.Union[Partition, tp.Tuple[Partition, ...]]:
+        if len(collections) < 1:
+            raise ValueError("Must specify at least one collection")
 
-    def __setitem__(self, collection: str, value: refx.Partition):
-        refx.update_refs(partitioning.get_partition(self, collection), value)
+        if isinstance(collections, str):
+            collections = (collections,)
 
-    def collections(self) -> tp.FrozenSet[str]:
-        return frozenset(
+        return partitioning.get_partition(self, *collections)
+
+    def __setitem__(
+        self,
+        _: SetItemType,
+        value: tp.Union[Partition, tp.Tuple[Partition, ...], tp.Dict[str, Partition]],
+    ):
+        update_refs(self, value)
+
+    def collections(self) -> tp.Set[str]:
+        return {
             x.collection
-            for x in jtu.tree_leaves(
-                self, is_leaf=lambda x: isinstance(x, refx.Referential)
-            )
-            if isinstance(x, refx.Referential)
-            if isinstance(x.collection, str)
-        )
+            for x in jtu.tree_leaves(self, is_leaf=lambda x: isinstance(x, Referential))
+            if isinstance(x, Referential)
+        }
 
     @tp.overload
     def partition(
         self: M,
+        collection: None = None,
+        second: None = None,
+        /,
         *,
         is_leaf: tp.Optional[partitioning.LeafPredicate] = None,
-    ) -> tp.Tuple[tp.Dict[str, refx.Partition], "ModuleDef[M]"]:
+    ) -> DerefedMod[tp.Dict[str, Partition], M]:
         ...
 
     @tp.overload
     def partition(
         self: M,
         collection: str,
+        second: None = None,
+        /,
+        *,
         is_leaf: tp.Optional[partitioning.LeafPredicate] = None,
-    ) -> tp.Tuple[refx.Partition, "ModuleDef[M]",]:
+    ) -> DerefedMod[Partition, M]:
         ...
 
     @tp.overload
     def partition(
         self: M,
         collection: str,
-        *extract_colelctions: str,
+        second: str,
+        /,
+        *collections: str,
         is_leaf: tp.Optional[partitioning.LeafPredicate] = None,
-    ) -> tp.Tuple[tp.Tuple[refx.Partition, ...], "ModuleDef[M]",]:
+    ) -> DerefedMod[tp.Tuple[Partition, ...], M]:
         ...
 
     def partition(
         self: M,
-        *extract_collections: str,
+        collection: tp.Optional[str] = None,
+        second: tp.Optional[str] = None,
+        /,
+        *collections: str,
         is_leaf: tp.Optional[partitioning.LeafPredicate] = None,
-    ) -> tp.Tuple[
-        tp.Union[
-            tp.Dict[str, refx.Partition], tp.Tuple[refx.Partition, ...], refx.Partition
-        ],
-        "ModuleDef[M]",
+    ) -> tp.Union[
+        DerefedMod[Partition, M],
+        DerefedMod[tp.Tuple[Partition, ...], M],
+        DerefedMod[tp.Dict[str, Partition], M],
     ]:
-        collections = list(self.collections())
-        module, dagdef = self.deref()
-        partitions, treedef = partitioning.tree_partition(
-            module, *collections, is_leaf=is_leaf
-        )
-        moduledef = ModuleDef(dagdef, treedef)
-
-        if all(x is refx.NOTHING for x in partitions[-1].values()):
-            partitions = partitions[:-1]
-        else:
-            # add "rest" as a reserved name for the rest of the tree
-            collections.append("rest")
+        if second is not None:
+            collections = (second, *collections)
 
-        partitions = dict(zip(collections, partitions))
+        if collection is not None:
+            collections = (collection, *collections)
 
-        if extract_collections:
-            if set(extract_collections) != set(collections):
-                raise ValueError(
-                    f"extract_colelctions contain all collections: "
-                    f"{extract_collections} != {collections}"
-                )
-
-            if len(extract_collections) == 1:
-                partitions = partitions[extract_collections[0]]
-            else:
-                partitions = tuple(partitions[x] for x in extract_collections)
-
-        return partitions, moduledef
-
-    @classmethod
-    def init(
-        cls: tp.Type[M],
-        rngs: tp.Union[
-            tp.Dict[str, jax.random.KeyArray], jax.random.KeyArray, None
-        ] = None,
-        **flags: tp.Hashable,
-    ) -> tp.Type[M]:
-        if rngs is None:
-            rngs = {}
-        elif isinstance(rngs, jax.Array):
-            rngs = {"params": rngs}
-
-        scope = scope_lib.Scope.from_keys_and_flags(rngs, flags)
-
-        def _context(fn, *args, **kwargs):
-            with scope_lib.scope(scope):
-                return fn(*args, **kwargs)
-
-        return CallableProxy(_context, cls)  # type: ignore
-
-    def apply(
-        self: M,
-        *,
-        rngs: tp.Optional[tp.Dict[str, jax.random.KeyArray]] = None,
-        **flags: tp.Hashable,
-    ) -> M:
-        if rngs is None:
-            rngs = {}
-
-        scope = scope_lib.Scope.from_keys_and_flags(rngs, flags)
-
-        def _context(fn, *args, **kwargs):
-            with scope_lib.scope(scope):
-                return fn(*args, **kwargs)
+        if len(collections) == 0:
+            partitions, dagdef = partitioning.collection_partition(
+                self, is_leaf=is_leaf
+            )
+        elif len(collections) == 1:
+            partitions, dagdef = partitioning.collection_partition(
+                self, collections[0], is_leaf=is_leaf
+            )
+        else:
+            partitions, dagdef = partitioning.collection_partition(
+                self, collections[0], collections[1], *collections[2:], is_leaf=is_leaf
+            )
 
-        return CallableProxy(_context, self)  # type: ignore
+        moduledef = ModuleDef.from_value(dagdef)
 
+        return DerefedMod((partitions, moduledef))
 
-class ApplyCaller(tp.Protocol):
-    def __getattr__(self, __name) -> "ApplyCaller":
+    @tp.overload
+    def ref_dict(self) -> tp.Tuple[tp.Dict[tp.Tuple[str, ...], tp.Any], jtu.PyTreeDef]:
         ...
 
-    def __call__(
-        self, *args, **kwargs
-    ) -> tp.Tuple[tp.Any, tp.Dict[str, refx.Partition]]:
+    @tp.overload
+    def ref_dict(self, sep: str) -> tp.Tuple[tp.Dict[str, tp.Any], jtu.PyTreeDef]:
         ...
 
-
-class ModuleDefValue(tp.NamedTuple):
-    reref_dagdef: refx.DagDef
-    partition_treedef: jtu.PyTreeDef
-
-
-class ModuleDef(tp.Generic[M]):
-    __slots__ = ("_reref_dagdef", "_partition_treedef")
-
-    def __init__(self, reref_dagdef: refx.DagDef, partition_treedef: jtu.PyTreeDef):
-        self._reref_dagdef = reref_dagdef
-        self._partition_treedef = partition_treedef
-
-    @property
-    def reref_dagdef(self) -> refx.DagDef:
-        return self._reref_dagdef
-
-    @property
-    def partition_treedef(self) -> jtu.PyTreeDef:
-        return self._partition_treedef
-
-    def apply(
-        self,
-        partitions: tp.Union[tp.Sequence[refx.Partition], tp.Dict[str, refx.Partition]],
-        *,
-        rngs: tp.Optional[tp.Dict[str, jax.random.KeyArray]] = None,
-        flags: tp.Optional[tp.Dict[str, tp.Hashable]] = None,
-    ) -> ApplyCaller:
-        if flags is None:
-            flags = {}
-        if rngs is None:
-            rngs = {}
-        if isinstance(partitions, dict):
-            partitions = tuple(partitions.values())
-        module: M = self.merge(partitions)
-        scope = scope_lib.Scope.from_keys_and_flags(rngs, flags)
-
-        def _context(fn, *args, **kwargs):
-            with scope_lib.scope(scope):
-                out = fn(*args, **kwargs)
-                partitions, _ = module.partition()
-                return out, partitions
-
-        return CallableProxy(_context, module)  # type: ignore
-
-    def merge(
-        self,
-        partitions: tp.Union[tp.Sequence[refx.Partition], tp.Dict[str, refx.Partition]],
-    ) -> M:
-        if isinstance(partitions, dict):
-            partitions = tuple(partitions.values())
-        module: M = partitioning.merge_partitions(partitions, self.partition_treedef)
-        return module.reref(self.reref_dagdef)
-
-
-def _moduledef_flatten(
-    x: ModuleDef[M],
-) -> tp.Tuple[tp.Tuple[()], tp.Tuple[refx.DagDef, jtu.PyTreeDef]]:
-    return (), (x.reref_dagdef, x.partition_treedef)
-
-
-def _moduledef_unflatten(
-    aux_data: tp.Tuple[refx.DagDef, jtu.PyTreeDef], _: tp.Tuple[()]
-) -> ModuleDef[M]:
-    return ModuleDef(*aux_data)
-
-
-jtu.register_pytree_node(ModuleDef, _moduledef_flatten, _moduledef_unflatten)
+    def ref_dict(
+        self, sep: tp.Optional[str] = None
+    ) -> tp.Tuple[
+        tp.Union[tp.Dict[tp.Tuple[str, ...], tp.Any], tp.Dict[str, tp.Any]],
+        jtu.PyTreeDef,
+    ]:
+        path_leaves, treedef = jtu.tree_flatten_with_path(self)
+        partition = ((_to_str_path(path), leaf) for path, leaf in path_leaves)
+        partition = (
+            (path[-1][:-5] if path[-1].endswith("__ref") else path, leaf)
+            for path, leaf in partition
+        )
+        if sep is None:
+            partition = {_to_str_path(path): leaf for path, leaf in path_leaves}
+        else:
+            partition = {
+                sep.join(_to_str_path(path)): leaf for path, leaf in path_leaves
+            }
+        return partition, treedef
```

### Comparing `nnx-0.0.2/nnx/nn/normalization.py` & `nnx-0.0.3/nnx/nn/normalization.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import typing as tp
 
 import jax
 import jax.numpy as jnp
 from jax import lax
 
-from nnx.nn.module import Module
+from nnx.module import Module
 from nnx.nn import initializers, dtypes
-from nnx import fields, utils
+from nnx import context, utils
+from nnx.dataclasses import param, ref
 
 PRNGKey = jax.Array
 Array = jax.Array
 Shape = tp.Tuple[int, ...]
 Dtype = tp.Any  # this could be a real type?
 
 Axes = tp.Union[int, tp.Any]
@@ -143,45 +144,17 @@
         bias = bias.reshape(feature_shape)
         y += bias
         args.append(bias)
     dtype = dtypes.canonicalize_dtype(*args, dtype=dtype)
     return jnp.asarray(y, dtype)
 
 
-@fields.dataclass
 class BatchNorm(Module):
     """BatchNorm Module.
 
-    Usage Note:
-    If we define a model with BatchNorm, for example::
-
-      BN = nn.BatchNorm(use_running_average=False, momentum=0.9, epsilon=1e-5,
-                        dtype=jnp.float32)
-
-    The initialized variables dict will contain in addition to a 'params'
-    collection a separate 'batch_stats' collection that will contain all the
-    running statistics for all the BatchNorm layers in a model::
-
-      vars_initialized = BN.init(key, x)  # {'params': ..., 'batch_stats': ...}
-
-    We then update the batch_stats during training by specifying that the
-    `batch_stats` collection is mutable in the `apply` method for our module.::
-
-      vars_in = {'params': params, 'batch_stats': old_batch_stats}
-      y, mutated_vars = BN.apply(vars_in, x, mutable=['batch_stats'])
-      new_batch_stats = mutated_vars['batch_stats']
-
-    During eval we would define BN with `use_running_average=True` and use the
-    batch_stats collection from training to set the statistics.  In this case
-    we are not mutating the batch statistics collection, and needn't mark it
-    mutable::
-
-      vars_in = {'params': params, 'batch_stats': training_batch_stats}
-      y = BN.apply(vars_in, x)
-
     Attributes:
       use_running_average: if True, the statistics stored in batch_stats
         will be used instead of computing the batch statistics on the input.
       axis: the feature or non-batch axis of the input.
       momentum: decay rate for the exponential moving average of
         the batch statistics.
       epsilon: a small float added to variance to avoid dividing by zero.
@@ -198,70 +171,89 @@
       axis_index_groups: groups of axis indices within that named axis
         representing subsets of devices to reduce over (default: None). For
         example, `[[0, 1], [2, 3]]` would independently batch-normalize over
         the examples on the first two and last two devices. See `jax.lax.psum`
         for more details.
     """
 
-    num_features: int = fields.static_field()
-    use_running_average: tp.Optional[bool] = fields.static_field(default=None)
-    axis: int = fields.static_field(default=-1)
-    momentum: float = fields.static_field(default=0.99)
-    epsilon: float = fields.static_field(default=1e-5)
-    dtype: tp.Optional[Dtype] = fields.static_field(default=None)
-    param_dtype: Dtype = fields.static_field(default=jnp.float32)
-    use_bias: bool = fields.static_field(default=True)
-    use_scale: bool = fields.static_field(default=True)
-    bias_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = fields.static_field(
-        default=initializers.zeros()
-    )
-    scale_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = fields.static_field(
-        default=initializers.ones()
-    )
-    axis_name: tp.Optional[str] = fields.static_field(default=None)
-    axis_index_groups: tp.Any = fields.static_field(default=None)
-    # refs
-    mean: Array = fields.ref("batch_stats", init=False)
-    var: Array = fields.ref("batch_stats", init=False)
-    scale: tp.Optional[Array] = fields.param(init=False)
-    bias: tp.Optional[Array] = fields.param(init=False)
-
-    def __post_init__(self):
-        feature_shape = (self.num_features,)
+    mean: Array = ref("batch_stats", init=False)
+    var: Array = ref("batch_stats", init=False)
+    scale: tp.Optional[Array] = param(init=False)
+    bias: tp.Optional[Array] = param(init=False)
+
+    def __init__(
+        self,
+        num_features: int,
+        *,
+        use_running_average: tp.Optional[bool] = None,
+        axis: int = -1,
+        momentum: float = 0.99,
+        epsilon: float = 1e-5,
+        dtype: tp.Optional[Dtype] = None,
+        param_dtype: Dtype = jnp.float32,
+        use_bias: bool = True,
+        use_scale: bool = True,
+        bias_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = initializers.zeros(),
+        scale_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = initializers.ones(),
+        axis_name: tp.Optional[str] = None,
+        axis_index_groups: tp.Any = None,
+        ctx: context.Context,
+    ):
+        feature_shape = (num_features,)
         self.mean = jnp.zeros(feature_shape, jnp.float32)
         self.var = jnp.ones(feature_shape, jnp.float32)
 
-        if self.use_scale:
-            key = self.make_rng("params")
-            self.scale = self.scale_init(key, feature_shape, self.param_dtype)
+        if use_scale:
+            key = ctx.make_rng("params")
+            self.scale = scale_init(key, feature_shape, param_dtype)
         else:
             self.scale = None
 
-        if self.use_bias:
-            key = self.make_rng("params")
-            self.bias = self.bias_init(key, feature_shape, self.param_dtype)
+        if use_bias:
+            key = ctx.make_rng("params")
+            self.bias = bias_init(key, feature_shape, param_dtype)
         else:
             self.bias = None
 
-    def __call__(self, x, use_running_average: tp.Optional[bool] = None):
+        self.num_features = num_features
+        self.use_running_average = use_running_average
+        self.axis = axis
+        self.momentum = momentum
+        self.epsilon = epsilon
+        self.dtype = dtype
+        self.param_dtype = param_dtype
+        self.use_bias = use_bias
+        self.use_scale = use_scale
+        self.bias_init = bias_init
+        self.scale_init = scale_init
+        self.axis_name = axis_name
+        self.axis_index_groups = axis_index_groups
+
+    def __call__(
+        self,
+        x,
+        use_running_average: tp.Optional[bool] = None,
+        *,
+        ctx: tp.Optional[context.Context] = None,
+    ):
         """Normalizes the input using batch statistics.
 
         Args:
           x: the input to be normalized.
           use_running_average: if true, the statistics stored in batch_stats
             will be used instead of computing the batch statistics on the input.
 
         Returns:
           Normalized inputs (the same shape as inputs).
         """
 
         use_running_average = utils.first_from(
             use_running_average,
             self.use_running_average,
-            self.get_flag("use_running_average", None),
+            ctx and ctx.get_flag("use_running_average"),
         )
         feature_axes = _canonicalize_axes(x.ndim, self.axis)
         reduction_axes = tuple(i for i in range(x.ndim) if i not in feature_axes)
 
         if use_running_average:
             mean, var = self.mean, self.var
         else:
@@ -283,7 +275,114 @@
             self.scale,
             self.bias,
             reduction_axes,
             feature_axes,
             self.dtype,
             self.epsilon,
         )
+
+
+class LayerNorm(Module):
+    """Layer normalization (https://arxiv.org/abs/1607.06450).
+
+    LayerNorm normalizes the activations of the layer for each given example in a
+    batch independently, rather than across a batch like Batch Normalization.
+    i.e. applies a transformation that maintains the mean activation within
+    each example close to 0 and the activation standard deviation close to 1.
+
+    Attributes:
+        epsilon: A small float added to variance to avoid dividing by zero.
+        dtype: the dtype of the result (default: infer from input and params).
+        param_dtype: the dtype passed to parameter initializers (default: float32).
+        use_bias:  If True, bias (beta) is added.
+        use_scale: If True, multiply by scale (gamma). When the next layer is linear
+            (also e.g. nn.relu), this can be disabled since the scaling will be done
+            by the next layer.
+        bias_init: Initializer for bias, by default, zero.
+        scale_init: Initializer for scale, by default, one.
+        reduction_axes: Axes for computing normalization statistics.
+        feature_axes: Feature axes for learned bias and scaling.
+        axis_name: the axis name used to combine batch statistics from multiple
+            devices. See `jax.pmap` for a description of axis names (default: None).
+            This is only needed if the model is subdivided across devices, i.e. the
+            array being normalized is sharded across devices within a pmap.
+        axis_index_groups: groups of axis indices within that named axis
+            representing subsets of devices to reduce over (default: None). For
+            example, `[[0, 1], [2, 3]]` would independently batch-normalize over
+            the examples on the first two and last two devices. See `jax.lax.psum`
+            for more details.
+    """
+
+    scale: tp.Optional[Array] = param(init=False)
+    bias: tp.Optional[Array] = param(init=False)
+
+    def __init__(
+        self,
+        num_features: int,
+        *,
+        epsilon: float = 1e-6,
+        dtype: tp.Optional[Dtype] = None,
+        param_dtype: Dtype = jnp.float32,
+        use_bias: bool = True,
+        use_scale: bool = True,
+        bias_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = initializers.zeros(),
+        scale_init: tp.Callable[[PRNGKey, Shape, Dtype], Array] = initializers.ones(),
+        reduction_axes: Axes = -1,
+        feature_axes: Axes = -1,
+        axis_name: tp.Optional[str] = None,
+        axis_index_groups: tp.Any = None,
+        ctx: context.Context,
+    ):
+        feature_shape = (num_features,)
+
+        if use_scale:
+            key = ctx.make_rng("params")
+            self.scale = scale_init(key, feature_shape, param_dtype)
+        else:
+            self.scale = None
+
+        if use_bias:
+            key = ctx.make_rng("params")
+            self.bias = bias_init(key, feature_shape, param_dtype)
+        else:
+            self.bias = None
+
+        self.num_features = num_features
+        self.epsilon = epsilon
+        self.dtype = dtype
+        self.param_dtype = param_dtype
+        self.use_bias = use_bias
+        self.use_scale = use_scale
+        self.bias_init = bias_init
+        self.scale_init = scale_init
+        self.reduction_axes = reduction_axes
+        self.feature_axes = feature_axes
+        self.axis_name = axis_name
+        self.axis_index_groups = axis_index_groups
+
+    def __call__(self, x):
+        """Applies layer normalization on the input.
+
+        Args:
+          x: the inputs
+
+        Returns:
+          Normalized inputs (the same shape as inputs).
+        """
+        mean, var = _compute_stats(
+            x, self.reduction_axes, self.dtype, self.axis_name, self.axis_index_groups
+        )
+
+        return _normalize(
+            x,
+            mean,
+            var,
+            self.scale,
+            self.bias,
+            self.reduction_axes,
+            self.feature_axes,
+            self.dtype,
+            self.epsilon,
+        )
+
+
+
```

### Comparing `nnx-0.0.2/nnx/nn/stochastic.py` & `nnx-0.0.3/nnx/nn/stochastic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,65 +1,72 @@
 from typing import Optional, Sequence
 
 import jax.numpy as jnp
 from jax import lax, random
 
-from nnx.nn.module import Module
-from nnx import fields, utils
+from nnx.module import Module
+from nnx import context, utils
+from nnx.dataclasses import dataclass
 
 
-@fields.dataclass
+@dataclass
 class Dropout(Module):
     """Create a dropout layer.
 
-    Note: When using :meth:`Module.apply() <flax.linen.Module.apply>`, make sure
-    to include an RNG seed named `'dropout'`. For example::
-
-      model.apply({'params': params}, inputs=inputs, train=True, rngs={'dropout': dropout_rng})`
-
     Attributes:
       rate: the dropout probability.  (_not_ the keep rate!)
       broadcast_dims: dimensions that will share the same dropout mask
       deterministic: if false the inputs are scaled by `1 / (1 - rate)` and
         masked, whereas if true, no mask is applied and the inputs are returned
         as is.
       rng_collection: the rng collection name to use when requesting an rng key.
     """
 
     rate: float
     broadcast_dims: Sequence[int] = ()
     deterministic: Optional[bool] = None
     rng_collection: str = "dropout"
 
-    def __call__(self, inputs, deterministic: Optional[bool] = None):
+    def __call__(
+        self,
+        inputs,
+        *,
+        deterministic: Optional[bool] = None,
+        ctx: Optional[context.Context] = None,
+    ):
         """Applies a random dropout mask to the input.
 
         Args:
           inputs: the inputs that should be randomly masked.
           deterministic: if false the inputs are scaled by `1 / (1 - rate)` and
             masked, whereas if true, no mask is applied and the inputs are returned
             as is.
 
         Returns:
           The masked inputs reweighted to preserve mean.
         """
         deterministic = utils.first_from(
             deterministic,
             self.deterministic,
-            self.get_flag("deterministic", None),
+            ctx and ctx.get_flag("deterministic"),
         )
 
         if (self.rate == 0.0) or deterministic:
             return inputs
 
         # Prevent gradient NaNs in 1.0 edge-case.
         if self.rate == 1.0:
             return jnp.zeros_like(inputs)
 
+        if ctx is None:
+            raise ValueError(
+                "Dropout needs to generate a random mask but no 'ctx' were provided."
+            )
+
         keep_prob = 1.0 - self.rate
-        rng = self.make_rng(self.rng_collection)
+        rng = ctx.make_rng(self.rng_collection)
         broadcast_shape = list(inputs.shape)
         for dim in self.broadcast_dims:
             broadcast_shape[dim] = 1
         mask = random.bernoulli(rng, p=keep_prob, shape=broadcast_shape)
         mask = jnp.broadcast_to(mask, inputs.shape)
         return lax.select(mask, inputs / keep_prob, jnp.zeros_like(inputs))
```

### Comparing `nnx-0.0.2/nnx/transforms.py` & `nnx-0.0.3/nnx/transforms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import functools
 import typing as tp
 
 import jax
 import jax.stages
-import refx
-import refx.tracers
-from jax._src import sharding_impls
-from refx.partitioning import Partition
+from nnx.reference import DagDef, Partition, deref, reref, update_refs
 import jax.tree_util as jtu
+from nnx import context
 
 import nnx
-from nnx import partitioning, scope_lib
+from nnx import partitioning
 
 A = tp.TypeVar("A")
 F = tp.TypeVar("F", bound=tp.Callable[..., tp.Any])
 G = tp.TypeVar("G", bound=tp.Callable[..., tp.Any])
 
 AxisName = tp.Hashable
 Leaf = tp.Any
@@ -26,50 +24,57 @@
         self,
         fun: tp.Callable[..., tp.Any],
         stateful: bool,
         **jit_kwargs,
     ):
         @functools.partial(jax.jit, **jit_kwargs)
         def jitted_fn(
-            pytree, scope: nnx.Scope, *args, _nnx__dagdef: refx.DagDef, **kwargs
+            partition: Partition,
+            *args,
+            _nnx__dagdef: DagDef[tp.Any],
+            **kwargs,
         ):
-            top_trace = refx.tracers.current_jax_trace()
-            with scope_lib.scope(scope.fork(), trace=top_trace):
-                pytree = refx.reref(pytree, _nnx__dagdef)
-                out = fun(pytree, *args, **kwargs)
-                if self.stateful:
-                    out = (refx.deref(pytree), out)
-                return out
+            pytree = reref(partition, _nnx__dagdef)
+            out = fun(pytree, *args, **kwargs)
+            if self.stateful:
+                out = (deref(pytree), out)
+            return out
 
         self.jitted_fn = jitted_fn
         self.stateful = stateful
 
     def __call__(self, pytree, *args, **kwargs):
         pytree_in = pytree
-        pytree, dagdef = refx.deref(pytree_in)
-        scope = nnx.current_scope()
-        out = self.jitted_fn(pytree, scope, *args, _nnx__dagdef=dagdef, **kwargs)
+
+        if "ctx" in kwargs and isinstance(kwargs["ctx"], context.Context):
+            kwargs["ctx"] = kwargs["ctx"].fork()
+
+        partition, dagdef = deref(pytree_in)
+        out = self.jitted_fn(partition, *args, _nnx__dagdef=dagdef, **kwargs)
         if self.stateful:
-            (pytree_out, _), out = out
-            refx.update_refs(pytree_in, pytree_out)
+            (partition_out, _), out = out
+            update_refs(pytree_in, partition_out)
         return out
 
     def __repr__(self):
         return f"JitTransform({self.jitted_fn})"
 
     def lower(self, *args, **kwargs):
         return self.jitted_fn.lower(*args, **kwargs)
 
 
+UNSPECIFIED = object()
+
+
 def jit(
     fun: tp.Callable[..., tp.Any],
     *,
     stateful: bool = True,
-    in_shardings: tp.Any = sharding_impls.UNSPECIFIED,
-    out_shardings: tp.Any = sharding_impls.UNSPECIFIED,
+    in_shardings: tp.Any = UNSPECIFIED,
+    out_shardings: tp.Any = UNSPECIFIED,
     static_argnums: tp.Union[int, tp.Sequence[int], None] = None,
     static_argnames: tp.Union[str, tp.Iterable[str], None] = None,
     donate_argnums: tp.Union[int, tp.Sequence[int]] = (),
     keep_unused: bool = False,
     device: tp.Optional[jax.Device] = None,
     backend: tp.Optional[str] = None,
     inline: bool = False,
@@ -82,28 +87,35 @@
     elif isinstance(static_argnames, str):
         static_argnames = [static_argnames]
     else:
         static_argnames = list(static_argnames)
 
     static_argnames.append("_nnx__dagdef")
 
-    ref_jit = JitTransform(
-        fun,
-        stateful,
-        in_shardings=in_shardings,
-        out_shardings=out_shardings,
+    jit_kwargs = dict(
         static_argnums=static_argnums,
         static_argnames=static_argnames,
         donate_argnums=donate_argnums,
         keep_unused=keep_unused,
         device=device,
         backend=backend,
         inline=inline,
         abstracted_axes=abstracted_axes,
     )
+
+    if in_shardings is not UNSPECIFIED:
+        jit_kwargs["in_shardings"] = in_shardings
+    if out_shardings is not UNSPECIFIED:
+        jit_kwargs["out_shardings"] = out_shardings
+
+    ref_jit = JitTransform(
+        fun,
+        stateful,
+        **jit_kwargs,
+    )
     ref_jit = functools.wraps(fun)(ref_jit)
     # _update_decorator_fields(ref_jit, fun)
     return ref_jit
 
 
 class GradTransform:
     def __init__(
@@ -123,58 +135,52 @@
             holomorphic=holomorphic,
             allow_int=allow_int,
             reduce_axes=reduce_axes,
         )
         def grad_fn(
             diff: Partition,
             non_diff: Partition,
-            dagdef: refx.DagDef,
-            treedef: jtu.PyTreeDef,
+            dagdef: DagDef[tp.Any],
             *args,
         ):
-            diff_trace = refx.tracers.get_top_trace(diff)
-            scope = scope_lib.current_scope()
-            with scope_lib.scope(scope.fork(), trace=diff_trace):
-                pytree = refx.merge_partitions((diff, non_diff), treedef)
-                pytree = refx.reref(pytree, dagdef)
-                out = fun(pytree, *args)
+            pytree = dagdef.reref((diff, non_diff))
+            out = fun(pytree, *args)
 
-                pytree = refx.deref(pytree)
-                if self.has_aux and self.stateful:
+            if self.stateful:
+                updates = deref(pytree)[0]
+                if self.has_aux:
                     loss, aux = out
-                    out = (loss, (pytree, aux))
-                elif self.stateful:
-                    out = (out, pytree)
+                    out = (loss, (updates, aux))
+                else:
+                    out = (out, updates)
 
-                return out
+            return out
 
         self.grad_fn = grad_fn
         self.predicate = predicate
         self.has_aux = has_aux
         self.stateful = stateful
 
     def __call__(self, pytree, *args):
         pytree_in = pytree
-        pytree, dagdef = refx.deref(pytree)
-        (diff, nondiff), treedef = refx.tree_partition(pytree, self.predicate)
-        # diff, nondiff = refx.deref((diff, nondiff))
-        grads = self.grad_fn(diff, nondiff, dagdef, treedef, *args)
-
-        if self.has_aux and self.stateful:
-            grad, (pytree_dagdef, aux) = grads
-            pytree_out = refx.reref(*pytree_dagdef)
-            refx.update_refs(pytree_in, pytree_out)
-            return grad, aux
-        elif self.stateful:
-            grad, pytree_dagdef = grads
-            pytree_out = refx.reref(*pytree_dagdef)
-            refx.update_refs(pytree_in, pytree_out)
-            return grad
+        (diff, nondiff), dagdef = partitioning.tree_partition(pytree, self.predicate)
+        grads = self.grad_fn(diff, nondiff, dagdef, *args)
+
+        if self.stateful:
+            updates: Partition
+            if self.has_aux:
+                grads, (updates, aux) = grads
+                out = grads, aux
+            else:
+                out, updates = grads
+            update_refs(pytree_in, updates)
         else:
-            return grads
+            out = grads
+
+        return out
 
     def __repr__(self):
         return f"GradTransform({self.grad_fn})"
 
 
 @tp.overload
 def grad(
```

### Comparing `nnx-0.0.2/pyproject.toml` & `nnx-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [tool.poetry]
 name = "nnx"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["Cristian Garcia <cgarcia.e88@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-# refx = { path = "../refx", develop = true }
-refx = "*"
 jax = "*"
 jaxlib = "*"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
+flax = "^0.6.10"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 ipykernel = "^6.22.0"
 
 [tool.poetry.group.examples.dependencies]
 matplotlib = "^3.7.1"
-ciclo = { path = "../ciclo", develop = true }
+optax = "^0.1.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.report]
 exclude_lines = [
```

### Comparing `nnx-0.0.2/PKG-INFO` & `nnx-0.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,122 +1,110 @@
-Metadata-Version: 2.1
-Name: nnx
-Version: 0.0.2
-Summary: 
-Author: Cristian Garcia
-Author-email: cgarcia.e88@gmail.com
-Requires-Python: >=3.8,<3.12
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: jax
-Requires-Dist: jaxlib
-Requires-Dist: refx
-Description-Content-Type: text/markdown
-
 # nnx
 
-_**N**erual **N**etworks for JA**X**_
+_**N**eural **N**etworks for JA**X**_
+
+`nnx` is a Neural Networks library for JAX that uses Pytree-based Modules and a novel 
+a **Ref**erence system to enable:
+
+* **Simplicity**: Provides an easy-to-understand mental model and implementation.
+* **Shared refereces**: Supports **safe** mutable shared state thanks to its **Ref**erence system.
+* **Leaf Metadata**: Enables semantic splitting a Module's state (similar to Flax collections) and adding [Axis Metadata](https://github.com/google/flax/blob/main/docs/flip/2434-general-metadata.md#flip-axis-metadata). 
+* **Stateful transformations**: Seamless integration with JAX's native transformation capabilities.
 
-`nnx` is a lightweight module system for JAX that provides the same power as `flax` but with a simpler mental model and implementation closer to `equinox`. It is built on top of `refx`, which enables shared state, tractable mutability, and semantic partitioning. `nnx` also supports stateful transformations, allowing you to train your models efficiently.
+NNX was designed to have the same capabilities as Flax with the simplicity of Equinox.
 
 ## Status
 
-`nnx` is currently a proof of concept, it is meant to explore the design space of a lightweight module system for JAX based on Refx.
+`nnx` is currently a proof of concept, aimed at exploring the design space of a lightweight module 
+system for JAX based on references. It is not intended for production use.
 
 ## Installation
 
 To get started with `nnx`, first install the package using pip:
 
 ```
 pip install nnx
 ```
+To get the latest version, install directly from GitHub:
+
+```
+pip install git+https://github.com/cgarciae/nnx
+```
 
 ## Usage
 
 ```python
 import nnx
 import jax
 
 class Linear(nnx.Module):
     w: jax.Array = nnx.param()
     b: jax.Array = nnx.param()
 
-    def __init__(self, din: int, dout: int):
-        key = self.make_rng("params")
+    def __init__(self, din: int, dout: int, *, ctx: nnx.Context):
+        key = ctx.make_rng("params")
         self.w = jax.random.uniform(key, (din, dout))
         self.b = jax.numpy.zeros((dout,))
 
     def __call__(self, x):
         return x @ self.w + self.b
 
-model = Linear.init(jax.random.PRNGKey(0))(din=12, dout=2)
+ctx = nnx.Context(params=jax.random.PRNGKey(0))
+model = Linear(din=12, dout=2, ctx=ctx)
 
 @nnx.jit
 def train_step(model, x, y):
     def loss_fn(model):
         y_pred = model(x)
         return jax.numpy.mean((y_pred - y) ** 2)
     
-    grad = nnx.grad(loss_fn, wrt="params")(model)
-    model["params"] = jax.tree_map(lambda w, g: w - 0.1 * g, model["params"], grad)
+    # compute gradient
+    grads = nnx.grad(loss_fn, wrt="params")(model)
+    # SGD update
+    model[:] = jax.tree_map(lambda w, g: w - 0.1 * g, model["params"], grads)
 
 # yes... there's no return :)
 train_step(model, x, y)
 ```
 
 ## Design
 
 ### Modules
 
-<!-- * Modules are Pytrees
-* `nnx.ref` and `nnx.param` mark ref fields, `params` is just a shorthand for `ref("params"), these are descriptor object (more info later)
-* `make_rng` is similar to flax's `make_rng`, distributes RNG keys through global state
-* the `init` and `apply` method lets you set the global state including RNG keys -->
-
-NNX `Module`s are [simple_pytree](https://github.com/cgarciae/simple-pytree) Pytrees with a few additional features to make them more easier to use with `refx` references. A custom Module can be created simply by
-subclassing `nnx.Module` and marking which fields are references with `nnx.ref` or `nnx.param`, as we will explain later, these are descriptors that store a `Ref` instance in a separate attribute and make using references transparent to the user.
+`nnx` has a simple and intuitive design with Modules at its core. These modules are built using [simple_pytree](https://github.com/cgarciae/simple-pytree) Pytrees. To create a custom module, simply subclass `nnx.Module` and mark the reference fields with `nnx.ref` or `nnx.param`. These are descriptors that store a `Ref` instance in a separate attribute, making references transparent to the user.
 
-Here is an example of a simple `Linear` module:
+Here's an example of a simple `Linear` module:
 
 ```python
 import nnx
 import jax
 
 class Linear(nnx.Module):
     w: jax.Array = nnx.ref("params")
     b: jax.Array = nnx.param() # shortcut for ref("params")
 
-    def __init__(self, din: int, dout: int):
-        key = self.make_rng("params") # request an RNG key
+    def __init__(self, din: int, dout: int, *, ctx: nnx.Context):
+        key = ctx.make_rng("params") # request an RNG key
         self.w = jax.random.uniform(key, (din, dout))
         self.b = jax.numpy.zeros((dout,))
 
     def __call__(self, x):
         return x @ self.w + self.b
-```
-NNX offers the same `make_rng` API as Flax to distribute RNG keys where they are needed, it does this by storing RNG keys in a global state and carefully handling them with context managers. You can set the state for the RNG keys and other flags via the `init` and `apply` methods, which are similar to Flax's `init` and `apply` methods but designed to be friendlier with static analysis tools.
 
-```python
-# global state ==>  .....................
-model = Linear.init(jax.random.PRNGKey(0))(din=12, dout=2)
-#                    constructor args ==> ^^^^^^^^^^^^^^^^
+ctx = nnx.Context(params=jax.random.PRNGKey(0))
+model = Linear(din=12, dout=2, ctx=ctx)
 ```
-If global state is not needed you can just use the constructor directly.
+
+`nnx` uses a `Context` object to propagate RNG and other forms of state throughout the model. `Context` provides a `make_rng` method that creates a new RNG key on demand for a given name (in this case, `"params"`).
 
 #### RefField Descriptor
-<!-- * `ref` and `params` create a `RefField` descriptor instances
-* `RefField` descriptors inherit from `dataclasses.Field` in order to be compatible with `dataclasses` when needed
-* `RefField` descriptors are descriptors that store a `Ref` instance in a separate `{name}__ref` attribute, this makes using references transparent to the user -->
 
-`nnx.ref` and `nnx.param` are descriptors that create `RefField` instances. `RefField` is a descriptor that stores a `Ref` instance in a separate `{attribute_name}__ref` attribute, and handle retrieving and setting the value of the reference automatically so that the user doesn't have to manipulate references directly. `RefField` inherits from `dataclasses.Field` in order to be compatible with `dataclasses` when needed.
+`nnx.ref` and `nnx.param` are descriptors that create `RefField` instances. A `RefField` is a descriptor that stores a `Ref` instance in a separate `{attribute_name}__ref` attribute. It handles retrieving and setting the value of the reference automatically, so the user doesn't have to manipulate references directly. Additionally, `RefField` inherits from `dataclasses.Field` to ensure compatibility with `nnx.dataclass` when needed.
 
-Here is a simplified version of how `RefField` is implemented:
+Here's a simplified version of the `RefField` implementation:
 
 ```python
 class RefField(dataclasses.Field):
     def __set_name__(self, cls, name):
         self.name = name
 
     def __get__(self, obj, objtype=None):
@@ -124,180 +112,155 @@
         return ref.value
 
     def __set__(self, obj, value):
         ref = getattr(obj, f"{self.name}__ref")
         ref.value = value
 ```
 
-The only thing to note here is that `Ref`s are created during the first call to `__set__` if the companion `{name}__ref` attribute doesn't exist yet. This should only happen during `__init__` or else `Module` will raise an error as `simple_pytree` Pytrees are frozen after initialization.
+It's important to note that `Ref` instances are created during the first call to `__set__` if the companion `{name}__ref` attribute doesn't exist yet. This should only happen inside the `__init__` method, otherwise, the `Module` will raise an error, as `simple_pytree` Pytrees are frozen after initialization.
 
-#### GetItem and SetItem syntactic sugar
-<!-- * `__getitem__` and `__setitem__` are syntactic sugar for `get_partition` and `update_refs`
-* they don't actually update the Module structure despite the appearance, they just update the references values -->
+#### GetItem and SetItem Syntactic Sugar
 
-`Module` implements `__getitem__` and `__setitem__` to provide syntactic sugar for creating and updating `Partition`s. Despite the appearance, `__setitem__` does not modify the Module's structure, it just updates the values of the references as can be seen in this simplified implementation:
+`Module` implements `__getitem__` and `__setitem__` to provide syntactic sugar for creating and updating `Partition`s. Although it may appear otherwise, `__setitem__` does not modify the Module's structure. Instead, it updates the values of the references, as demonstrated in this simplified implementation:
 
 ```python
-class Module(simple_pytree.Pytree):
+class Module(nnx.Pytree):
     ...
-    def __getitem__(self, collection: str) -> refx.Partition:
-        derefed_module = refx.deref(self)[0]
-        return nnx.get_partition(derefed_module, collection)
+    def __getitem__(self, collection: str) -> nnx.Partition:
+        return nnx.get_partition(self, collection)
 
-    def __setitem__(self, collection: str, updates: refx.Partition):
-        partition = nnx.get_partition(self, collection)
-        refx.update_refs(partition, updates)
+    def __setitem__(self, _: SetItemType, value: nnx.Partition):
+        nnx.update_refs(self, value)
 ```
 
-Sample usage could look something like this:
+Sample usage might look like this:
 
 ```python
-model["params"] = jax.tree_map(lambda w, g: w - 0.1 * g, model["params"], grad)
+# SGD update
+model[:] = jax.tree_map(lambda w, g: w - 0.1 * g, model["params"], grads)
 ```
 
-Here `model["params"]` is a `Partition` that contains all the references in the `params` collection, and `grad` is a `Partition` with the same structure as `model["params"]` but with gradients instead of parameters. `moduel["params"] = ...` updates the values of the references in `model["params"]` with the values of the `sdg` update.
+In this example, `model["params"]` returns a `Partition` that contains all the references in the `params` collection. `grads` is a `Partition` with the same structure as `model["params"]`, but with gradients instead of parameters. The statement `model[:] = ...` updates the values of the references in `model` with the values of the new parameters from stochastic gradient descent (SGD) update rule.
 
 ### Transformations
 
-<!-- * 3 types of transformations: stateful, filtered, and the partition API
-* a final API would probably have a mix of the 3 -->
-
-Currently NNX offers 3 types of transformations: stateful, filtered, and the partition API. At the moment its not clear which API is the best, the 3 will be kept for now.
+Currently, NNX offers three types of transformations: stateful, filtered, and the partition API. As it is unclear which API is the best, all three will be maintained for now.
 
 #### Stateful Transforms
 
-<!-- * stateful transformations take a pytree/Module of references as its first argument
-* use `deref` and `reref` to move the pytree/Module across the transformation
-* handle all relevant global state such as `nnx.scope` and Refx's trace state
-* their main feature is that they always update the state of the references of the input pytree/Module -->
-
-Stateful Transforms take a pytree of references (e.g. a Module) as their first argument, track changes in the state of the references that happen inside the transformation, and automatically propagate those changes to the input pytree outside the transformation. In general they have the following properties:
-
-* they behave as stateful functions w.r.t. the first argument
-* they can operate on collections and RNG streams according to the transformation's semantics, exactly like Flax's transformations
-* they take care of handling all relevant global state such as `nnx.scope` and Refx's trace state
-    
-Here is a diagram of how stateful transformations work:
+Stateful transforms take a Pytree of references (e.g., a Module) as their first argument, track changes in the state of the references that occur within the transformation, and automatically propagate those changes to the input Pytree outside the transformation. In general, they have the following properties:
 
-![stateful-transforms](https://raw.githubusercontent.com/cgarciae/nnx/main/docs/images/stateful-transforms.png)
+* They behave as stateful functions with respect to the first argument.
+* They can operate on collections and RNG streams according to the transformation's semantics, exactly like Flax's transformations.
+* They handle all relevant global state, such as `nnx.scope` and Refx's trace state.
+
+Here's a diagram illustrating how stateful transformations work:
 
-<!-- * `nnx.jit` and `nnx.grad` are stateful transformations -->
+![stateful-transforms](https://raw.githubusercontent.com/cgarciae/nnx/main/docs/images/stateful-transforms.png)
 
-Currently `nnx.jit` and `nnx.grad` are the only stateful transformations.
+Currently, `nnx.jit` and `nnx.grad` are the only stateful transformations.
 
-Here is how a `train_step` function could be implemented using `nnx.jit` and `nnx.grad`:
+The following example demonstrates how a `train_step` function can be implemented using `nnx.jit` and `nnx.grad`:
 
 ```python
 @nnx.jit
 def train_step(model, x, y):
 
     def loss_fn(model):
         y_pred = model(x)
         return jax.numpy.mean((y_pred - y) ** 2)
     
     # compute gradient
-    grad = nnx.grad(loss_fn, wrt="params")(model)
-    # sdg update
-    model["params"] = jax.tree_map(lambda w, g: w - 0.1 * g, model["params"], grad)
+    grads = nnx.grad(loss_fn, wrt="params")(model)
+    # SGD update
+    model[:] = jax.tree_map(lambda w, g: w - 0.1 * g, model["params"], grads)
 
-# stateful update, no return !!!
+# stateful update, no return needed
 train_step(model, x, y)
 ```
 
-<!-- * probably the most "interesting" part of the design is that code looks very imperative
-* state is automatically propagated in and out of the transformation -->
+The most interesting aspect of this design is that the code appears very imperative, as the state is automatically propagated in and out of the transformations. However, more consideration is needed to properly support `jit`'s `in_shardings` and `out_shardings` arguments.
 
-The most interesting part of the design is that the code looks very imperative since the state is automatically propagated in and out of the transformations. However, more thought is needed to see how to correctly support `jit`'s `in_shardings` and `out_shardings` arguments.
+Certainly! I've revised the text to improve clarity and readability. Here are the updated sections:
 
+---
 #### Filtered Transformations
 
-<!-- * filtered transformations `deref` and `reref` all their inputs and outputs to move the pytree/Modules across the transformation
-* they don't handle any global state, the must semantically behave as pure functions -->
-
-Filtered transformations are more flexible in that they can take pytrees of references in any of their arguments and also return pytrees of references. They just `deref` and `reref` all their inputs and outputs to move the pytrees across the transformation. In general they have the following properties:
+Filtered transformations offer more flexibility, as they can take Pytrees of references in any of their arguments and return Pytrees of references. They simply `deref` and `reref` all their inputs and outputs to transfer the Pytrees across the transformation. In general, they have the following properties:
 
-* they behave as pure functions
-* they don't handle any global state except for Refx's trace state
+* They behave as pure functions.
+* They don't handle any global state except for Refx's trace state.
 
 ![filtered-transforms](https://raw.githubusercontent.com/cgarciae/nnx/main/docs/images/filtered-transforms.png)
 
-<!-- * `nnx.jit_filter` is a filtered transformation, `nnx.grad` is a stateful transformation -->
-
-Currently `nnx.jit_filter` is the only filtered transformation.
+Currently, `nnx.jit_filter` is the only filtered transformation.
 
-Here is how a `train_step` function could be implemented using `nnx.jit_filter` and `nnx.grad`:
+Here's an example of how a `train_step` function can be implemented using `nnx.jit_filter` and `nnx.grad`:
 
 ```python
 @nnx.jit_filter
 def train_step(model, x, y):
 
     def loss_fn(model):
         y_pred = model(x)
         return jax.numpy.mean((y_pred - y) ** 2)
 
     # compute gradient
-    grad = nnx.grad(loss_fn, wrt="params")(model)
-    # sdg update                   |--------sdg-----------|
-    model["params"] = jax.tree_map(lambda w, g: w - 0.1 * g, model["params"], grad)
+    grads = nnx.grad(loss_fn, wrt="params")(model)
+    # SGD update
+    model[:] = jax.tree_map(lambda w, g: w - 0.1 * g, model["params"], grads)
     
     return model
 
 model = train_step(model, x, y)
 ```
 
-<!-- * filtered transformations must output any state that they want to propagate but have more flexibility in how they handle it -->
-
-Filtered transformations must output any state that they want to propagate but have more flexibility in how they handle it. Adding support for `jit`'s `in_shardings` and `out_shardings` arguments is probably more straightforward than with stateful transformations.
-
+Filtered transformations must output any state they want to propagate but have more flexibility in how they handle it. Adding support for `jit`'s `in_shardings` and `out_shardings` arguments is likely more straightforward than with stateful transformations.
 
 #### Partition API
 
-<!-- * the partition API mimicks Flax's `variables` + `apply` API
-* it splits a pytree/Module into all its `Partition`s + a `ModuleDef` object
-* each `Partition` is a flat dictionary so it works with regular JAX transformations -->
-
-The partition API mimicks Flax's `variables` plus `apply` API. It splits a pytree of references into all its `Partition`s and creates a `ModuleDef` object that knows how to reconstruct the original pytree from the `Partition`s. Since each `Partition` is a flat dictionary, this API works with regular JAX transformations.
- 
-Here is a diagram of how the partition API works:
+The partition API enables splitting a Module's state into sets of reference-less `Partition`s, this provides a general way of interacting with vanilla JAX transformations.
+
 
 ![partition-api](https://raw.githubusercontent.com/cgarciae/nnx/main/docs/images/partition-api.png)
 
-Here is an example of how to use the partition API:
+Here's an example of how a `train_step` function can be implemented using the partition API:
 
 ```python
-model: ModuleDef
-partitions, model = model.partition()
+modeldef: ModuleDef[Linear]
+partitions, modeldef = model.partition()
 params = partitions["params"]
 
 @jax.jit
 def train_step(params, x, y):
 
-    def loss_fn(params): #      |----merge----|
-        y_pred, updates = model.apply([params])(x)
+    def loss_fn(params):
+        model: Linear = modeldef.reref(params)
+        y_pred = model(x)
         return jax.numpy.mean((y_pred - y) ** 2)
 
     # compute gradient
-    grad = jax.grad(loss_fn)(params)
-    # sdg update          |--------sdg-----------|
-    params = jax.tree_map(lambda w, g: w - 0.1 * g, params, grad)
+    grads = jax.grad(loss_fn)(params)
+    # SGD update
+    params = jax.tree_map(lambda w, g: w - 0.1 * g, params, grads)
     
     return params
 
 params = train_step(params, x, y)
 ```
 
-The main benefit of the partition API is that its more compatible with other JAX tools as the training step can be written using regular JAX transformations. The main drawback is that it's more verbose and users have to manually keep track of all the partitions, this overhead is often what makes `flax` and `haiku` a bit harder to learn than other frameworks like `pytorch` and `keras`.
+The main benefit of the partition API is its compatibility with other JAX tools, as the training step can be written using regular JAX transformations. The main drawback is that it's more verbose.
 
 ### Case Studies
 
 #### Shared State
 
-In `nnx`, it's possible to create modules that share state between each other. This can be useful when designing complex neural network architectures, as it allows you to reuse certain layers and reduce the number of learnable parameters.
+In NNX, you can create modules that share state between them. This is useful when designing complex neural network architectures, as it allows you to reuse certain layers and reduce the number of learnable parameters.
 
-Here's an example of how to create a module with shared state:
+Here's an example of creating a module with shared state:
 
 ```python
 class Block(nnx.Module):
     def __init__(self, linear: nnx.Linear):
         self.linear = linear
         self.bn = nnx.BatchNorm(2)
 
@@ -312,19 +275,18 @@
 
     def __call__(self, x):
         x = self.block1(x)
         x = self.block2(x)
         return x
 ```
 
-In this example, the `Model` module contains two instances of the `Block` module, each of which shares the same `nnx.Linear` module. To run the model you can use the `apply` method to set the `use_running_average` flag for all `BatchNorm` modules.
+In this example, the `Model` module contains two instances of the `Block` module. Each instance shares the same `nnx.Linear` module. To run the model, you can use the `apply` method to set the `use_running_average` flag for all `BatchNorm` modules.
 
-Here's an example of how to compute the loss for a `Model` instance:
+Here's an example of computing the loss for a `Model` instance:
 
 ```python
 def loss_fn(model: Model, x: jax.Array, y: jax.Array):
     y_pred = model.apply(use_running_average=False)(x)
     return jnp.mean((y - y_pred) ** 2)
 ```
 
-It's worth noting that the state for the shared `nnx.Linear` module will be kept in sync at all times on both `Block` instances, including during gradient updates.
-
+It's important to note that the state for the shared `nnx.Linear` module will be kept in sync at all times on both `Block` instances, including during gradient updates.
```

