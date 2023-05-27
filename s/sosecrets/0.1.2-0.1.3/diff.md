# Comparing `tmp/sosecrets-0.1.2.tar.gz` & `tmp/sosecrets-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosecrets-0.1.2.tar", max compression
+gzip compressed data, was "sosecrets-0.1.3.tar", max compression
```

## Comparing `sosecrets-0.1.2.tar` & `sosecrets-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      955 2023-05-27 17:34:45.087611 sosecrets-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5244 2023-05-27 17:34:45.090608 sosecrets-0.1.2/README.md
--rw-r--r--   0        0        0      161 2023-05-27 17:34:45.088610 sosecrets-0.1.2/src/sosecrets/__init__.py
--rw-r--r--   0        0        0       42 2023-05-27 15:09:04.656926 sosecrets-0.1.2/src/sosecrets/__init__.pyi
--rw-r--r--   0        0        0      482 2023-05-25 16:38:42.002355 sosecrets-0.1.2/src/sosecrets/exceptions.py
--rw-r--r--   0        0        0     7542 2023-05-27 17:00:43.333186 sosecrets-0.1.2/src/sosecrets/secretdicts.py
--rw-r--r--   0        0        0     3264 2023-05-27 15:11:09.184173 sosecrets-0.1.2/src/sosecrets/secrets.py
--rw-r--r--   0        0        0     1392 2023-05-27 15:30:13.527848 sosecrets-0.1.2/src/sosecrets/sosecrets.pyi
--rw-r--r--   0        0        0     5850 1970-01-01 00:00:00.000000 sosecrets-0.1.2/setup.py
--rw-r--r--   0        0        0     5662 1970-01-01 00:00:00.000000 sosecrets-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      955 2023-05-27 18:04:53.017918 sosecrets-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5306 2023-05-27 18:04:53.021945 sosecrets-0.1.3/README.md
+-rw-r--r--   0        0        0      161 2023-05-27 18:04:53.019916 sosecrets-0.1.3/src/sosecrets/__init__.py
+-rw-r--r--   0        0        0       42 2023-05-27 15:09:04.656926 sosecrets-0.1.3/src/sosecrets/__init__.pyi
+-rw-r--r--   0        0        0      482 2023-05-25 16:38:42.002355 sosecrets-0.1.3/src/sosecrets/exceptions.py
+-rw-r--r--   0        0        0     7671 2023-05-27 17:53:28.379809 sosecrets-0.1.3/src/sosecrets/secretdicts.py
+-rw-r--r--   0        0        0     3264 2023-05-27 15:11:09.184173 sosecrets-0.1.3/src/sosecrets/secrets.py
+-rw-r--r--   0        0        0     1392 2023-05-27 15:30:13.527848 sosecrets-0.1.3/src/sosecrets/sosecrets.pyi
+-rw-r--r--   0        0        0     5912 1970-01-01 00:00:00.000000 sosecrets-0.1.3/setup.py
+-rw-r--r--   0        0        0     5723 1970-01-01 00:00:00.000000 sosecrets-0.1.3/PKG-INFO
```

### Comparing `sosecrets-0.1.2/pyproject.toml` & `sosecrets-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sosecrets"
-version = "0.1.2"
+version = "0.1.3"
 description = "Simple wrapper to secure your secrets."
 authors = ["Jim Chng <jimchng@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["secrets", "security"]
 
 [tool.poetry.dependencies]
@@ -19,15 +19,15 @@
 python-dotenv = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "0.1.2"
+current_version = "0.1.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `sosecrets-0.1.2/README.md` & `sosecrets-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # sosecrets
 
 `sosecrets` is a Python module that provides a secure way to handle sensitive data by encapsulating it and only exposing it through a controlled interface.
 
-Version: 0.1.2
+Version: 0.1.3
+[Documentation](https://sosecrets.readthedocs.io/en/latest/)
 
 ## Installation
 
 To install `sosecrets`, you can use pip:
 
 ```bash
 pip install sosecrets
```

### Comparing `sosecrets-0.1.2/src/sosecrets/secretdicts.py` & `sosecrets-0.1.3/src/sosecrets/secretdicts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,120 +1,118 @@
-from src.sosecrets.secrets import Secret, Dict, Any, Optional
+from src.sosecrets.secrets import Secret, Dict, Any, Optional, Callable, Generic, T, Tuple
 
 
 class ImmutableSecretMapping(dict, Dict[Any, Secret]):
     """
     A dictionary-like object that stores secret values and prevents changes to the dictionary.
     """
-    def __new__(cls, mapping: Dict[Any, Any]):
+    def __new__(cls, mapping: Dict[Any, Any]) -> 'ImmutableSecretMapping':
         """
-        Initialize the ImmutableSecretMapping object.
+        Initialize a new ImmutableSecretMapping object.
 
-        Parameters:
-        - mapping (Dict[Any, Any]): A dictionary with `Any` keys and secret values.
+        Args:
+            mapping (Dict[Any, Any]): A dictionary with `Any` keys and `Any` values.
 
-       Raises:
-        - Exception: If the mapping argument is empty or if any of the values in the mapping are not of type Secret.
+        Raises:
+            ValueError: If the mapping argument is empty.
         """
         if not mapping:
             raise ValueError("Mapping argument is empty.")
-        new_mapping = {}
+        new_mapping: Dict[Any, Any] = {}
         for k, v in mapping.items():
             if not isinstance(v, Secret):
                 new_mapping[k] = Secret(v)
             else:
                 new_mapping[k] = v
         return super().__new__(cls, new_mapping)
 
     def __setitem__(self, key: Any, value: Any) -> None:
         """
         Raise an exception when attempting to set a new key-value pair in the `ImmutableSecretMapping` object.
 
         Parameters:
-        - key (Any): The key to set.
-        - value (Any): The value to set.
+            key (Any): The key to set.
+            value (Any): The value to set.
 
         Raises:
-        - Exception: When attempting to set a new key-value pair.
+            Exception: When attempting to set a new key-value pair.
         """
         raise TypeError(
             "ImmutableSecretMapping object does not support item assignment.")
 
     @classmethod
     def from_func(
             cls,
-            func,
-            *func_args,
-            **func_kwargs) -> 'ImmutableSecretMapping':
-        """
-        Create a new ImmutableSecretMapping object from the result of a function.
-
-        Parameters:
-        - func (callable): A function that returns a dictionary with Anying keys and secret values.
-        - *func_args (Any): Positional arguments to pass to the function.
-        - **func_kwargs (Any): Keyword arguments to pass to the function.
+            func: Callable[[Any], Dict[Any, Any]],
+            *func_args: Tuple[Any],
+            **func_kwargs: Dict[Any, Any]) -> 'ImmutableSecretMapping':
+        """Create a new ImmutableSecretMapping object from the result of a function.
+
+        Args:
+            func (callable): A function that returns a dictionary with `Any` keys and secret values.
+            *func_args (Any): Positional arguments to pass to the function.
+            **func_kwargs (Any): Keyword arguments to pass to the function.
 
         Returns:
-        - ImmutableSecretMapping: A new ImmutableSecretMapping object.
+            ImmutableSecretMapping: A new ImmutableSecretMapping object.
 
-       Raises:
-        - ValueError: If the result of the function is empty or if any of the values in the result are not of type Secret.
+        Raises:
+            ValueError: If the result of the function is empty.
+            TypeError: If any of the values in the result are not of type Secret.
         """
         mapping = func(*func_args, **func_kwargs)
         if not mapping:
             raise ValueError("Result of the function is empty.")
         new_mapping = {}
         for k, v in mapping.items():
             if not isinstance(v, Secret):
                 new_mapping[k] = Secret(v)
             else:
                 new_mapping[k] = v
         return cls(new_mapping)
 
     def get_exposed(self, key: Any, default: Optional[Any] = None) -> Any:
-        """
-        Get the exposed value of a key in the ImmutableSecretMapping object.
+        """Get the exposed value of a key in the ImmutableSecretMapping object.
 
-        Parameters:
-        - key (Any): The key to get.
-        - default (Optional[Any]): The default value to return if the key is not found.
+        Args:
+            key (Any): The key to get.
+            default (Optional[Any]): The default value to return if the key is not found.
 
         Returns:
-        - Any: The exposed value of the key, or the default value if the key is not found.
-        """
+            Any: The exposed value of the key, or the default value if the key is not found."""
         value = super().get(key, default)
         if value == default:
             return value
         return value.expose_secret()
 
     def expose_dict(self) -> Dict[Any, Any]:
         """
         Return a new dictionary that exposes non-sensitive information.
 
         This method returns a new dictionary with the same keys as the original dictionary, but with values that have been converted to non-sensitive information using their `expose_secret()` method. The `expose_secret()` method is expected to return a non-sensitive version of the value, so that the dictionary can be safely exported or displayed without exposing sensitive information.
 
         Returns:
-            A new dictionary with non-sensitive values.
+            Dict[Any, Any]: A new dictionary with non-sensitive values.
         """
         return {k: v.expose_secret() for k, v in super().items()}
 
 
 class MutableSecretMapping(dict):
     """
     A dictionary-like object that stores secret values and allows changes to the dictionary.
     """
     def __new__(cls, mapping: Dict[Any, Any]):
         """
-        Initialize the MutableSecretMapping object.
+        Initialize a new MutableSecretMapping object.
 
-        Parameters:
-        - mapping (Dict[Any, Any]): A dictionary with Any keys and secret values.
+        Args:
+            mapping (Dict[Any, Any]): A dictionary with `Any` keys and `Any` values.
 
         Raises:
-        - ValueError: If the mapping argument is empty or if any of the values in the mapping are not of type Secret.
+            ValueError: If the mapping argument is empty.
         """
         if not mapping:
             raise ValueError("Mapping argument is empty.")
         new_mapping = {}
         for k, v in mapping.items():
             if not isinstance(v, Secret):
                 new_mapping[k] = Secret(v)
@@ -123,43 +121,43 @@
         return super().__new__(cls, new_mapping)
 
     def __setitem__(self, key: Any, value: Any) -> None:
         """
         Set a new key-value pair in the MutableSecretMapping object.
 
         Parameters:
-        - key (Any): The key to set.
-        - value (Any): The value to set.
+            key (Any): The key to set.
+            value (Any): The value to set.
 
         Raises:
-        - ValueError: If the value is not of type Secret.
+            ValueError: If the value is not of type Secret.
         """
         if not isinstance(value, Secret):
             raise ValueError("Value must be of type Secret.")
         super().__setitem__(key, value)
 
     @classmethod
     def from_func(
             cls,
-            func,
-            *func_args,
-            **func_kwargs) -> 'MutableSecretMapping':
-        """
-        Create a new MutableSecretMapping object from the result of a function.
-
-        Parameters:
-        - func (callable): A function that returns a dictionary with `Any` keys and secret values.
-        - *func_args (Any): Positional arguments to pass to the function.
-        - **func_kwargs (Any): Keyword arguments to pass to the function.
+            func: Callable[[Any], Dict[Any, Any]],
+            *func_args: Tuple[Any],
+            **func_kwargs: Dict[Any, Any]) -> 'MutableSecretMapping':
+        """Create a new MutableSecretMapping object from the result of a function.
+
+        Args:
+            func (callable): A function that returns a dictionary with `Any` keys and secret values.
+            *func_args (Any): Positional arguments to pass to the function.
+            **func_kwargs (Any): Keyword arguments to pass to the function.
 
         Returns:
-        - MutableSecretMapping: A new MutableSecretMapping object.
+            MutableSecretMapping: A new MutableSecretMapping object.
 
         Raises:
-        - ValueError: If the result of the function is empty or if any of the values in the result are not of type Secret.
+            ValueError: If the result of the function is empty.
+            TypeError: If any of the values in the result are not of type Secret.
         """
         mapping = func(*func_args, **func_kwargs)
         if not mapping:
             raise ValueError("Result of the function is empty.")
         new_mapping = {}
         for k, v in mapping.items():
             if not isinstance(v, Secret):
@@ -168,26 +166,26 @@
                 new_mapping[k] = v
         return cls(new_mapping)
 
     def get_exposed(self, key: Any, default: Optional[Any] = None) -> Any:
         """
         Get the exposed value of a key in the MutableSecretMapping object.
 
-        Parameters:
-        - key (Any): The key to get.
-        - default (Optional[Any]): The default value to return if the key is not found.
+        Args:
+            key (Any): The key to get.
+            default (Optional[Any]): The default value to return if the key is not found.
 
         Returns:
-        - Any: The exposed value of the key, or the default value if the key is not found.
+            Any: The exposed value of the key, or the default value if the key is not found.
         """
         return super().get(key, default).expose_secret()
 
     def expose_dict(self) -> Dict[Any, Any]:
         """
         Return a new dictionary that exposes non-sensitive information.
 
         This method returns a new dictionary with the same keys as the original dictionary, but with values that have been converted to non-sensitive information using their `expose_secret()` method. The `expose_secret()` method is expected to return a non-sensitive version of the value, so that the dictionary can be safely exported or displayed without exposing sensitive information.
 
         Returns:
-            A new dictionary with non-sensitive values.
+            Dict[Any, Any]: A new dictionary with non-sensitive values.
         """
         return {k: v.expose_secret() for k, v in super().items()}
```

### Comparing `sosecrets-0.1.2/src/sosecrets/secrets.py` & `sosecrets-0.1.3/src/sosecrets/secrets.py`

 * *Files identical despite different names*

### Comparing `sosecrets-0.1.2/src/sosecrets/sosecrets.pyi` & `sosecrets-0.1.3/src/sosecrets/sosecrets.pyi`

 * *Files identical despite different names*

### Comparing `sosecrets-0.1.2/setup.py` & `sosecrets-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 ['sosecrets']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'sosecrets',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Simple wrapper to secure your secrets.',
-    'long_description': '# sosecrets\n\n`sosecrets` is a Python module that provides a secure way to handle sensitive data by encapsulating it and only exposing it through a controlled interface.\n\nVersion: 0.1.2\n\n## Installation\n\nTo install `sosecrets`, you can use pip:\n\n```bash\npip install sosecrets\n```\n\n## Usage\n\nHere\'s are the examples of how to use `sosecrets`:\n\n### Secret\n\nHere\'s an example of how to use `Secret`:\n\n```python\nfrom sosecrets import Secret\n\n# Create a secret value\nsecret_value = Secret("my secret value")\n\n# Use the secret value while keeping it encapsulated\nresult = secret_value.apply(len)\nprint(result)  # Output: 14\n\n# Get the value of the secret\nvalue = secret_value.expose_secret()\nprint(value)  # Output: "my secret value"\n```\n\nIn this example, we create a `Secret` object with the value "my secret value". We then use the `apply` method to apply the `len` function to the secret value while keeping it encapsulated. Finally, we use the `expose_secret` method to retrieve the value of the secret.\n\n### ImmutableSecretMapping\n\nHere\'s an example of how to use `ImmutableSecretMapping`:\n\n```python\nfrom pathlib import Path\nfrom sosecrets import ImmutableSecretMapping\nfrom dotenv import dotenv_values\n\n# Define the path to the `.env` file\nTHIS_SCRIPT_FILE_PATH = Path(__file__)\nEXAMPLES = THIS_SCRIPT_FILE_PATH.parent / \'.env\'\n\n# Load the environment variables and store them securely\nsecret_env_dict = ImmutableSecretMapping.from_func(dotenv_values, dotenv_path=EXAMPLES)\n\n# Get a dictionary of the exposed values of the secret variables\nexposed_dict = secret_env_dict.expose_dict()\nprint("exposed_dict: ", exposed_dict)\n\n# Print the `ImmutableSecretMapping` object itself\nprint("secret_env_dict: ", secret_env_dict)\n\n# Get the value associated with a key using the `get()` method\nvalue0 = secret_env_dict.get(\'value0\')\nprint("value0: ", value0)\n\n# Get the exposed value of a key using the `get_exposed()` method\nvalue1 = secret_env_dict.get_exposed(\'value1\')\nprint("value1: ", value1)\n```\n\nThe example code does the following:\n\n1. Imports the necessary packages: `Path` from `pathlib`, `src` from the `sosecrets` module, `ImmutableSecretMapping` from `secretdicts` in the `sosecrets` module, and `dotenv_values` from the `dotenv` package.\n2. Defines the path to a `.env` file that contains environment variables to be loaded.\n3. Uses `ImmutableSecretMapping.from_func(dotenv_values, dotenv_path=EXAMPLES)` to load the environment variables from the `.env` file and store them in an instance of `ImmutableSecretMapping`.\n4. Prints the exposed dictionary of the `ImmutableSecretMapping` object using the `expose_dict()` method.\n5. Prints the `ImmutableSecretMapping` object itself.\n6. Gets a value from the `ImmutableSecretMapping` object using the `get()` method and prints it.\n7. Gets the exposed value of a key using the `get_exposed()` method## The Output\n\n### MutableSecretMapping\n\nSimilar to `ImmutableSecretMapping`.\n\n## Use Cases\nsosecrets can be used in a variety of scenarios where sensitive data needs to be securely handled. Here are some common use cases:\n\nStoring API keys, passwords, and other credentials: sosecrets can be used to securely store sensitive information such as API keys, passwords, and other credentials that are required for authentication or authorization in an application.\n\nHandling personal identifiable information (PII): sosecrets can be used to protect personal identifiable information (PII) such as names, addresses, social security numbers, and other sensitive data that needs to be kept confidential.\n\n## API Reference\n\n### `Secret`\n\nThe `Secret` class encapsulates a secret value and only exposes it through a controlled interface.\n\n```\nSecret(value: Optional[T] = None, func: Optional[Callable[[Any], T]] = None, func_args: Tuple[Any] = tuple(), func_kwargs: Dict[str, Any] = dict()) -> SecretType\n```\n\n- `value`: The secret value to encapsulate.\n- `func`: A function to generate the secret value.\n- `func_args`: The positional arguments to pass to the `func` function.\n- `func_kwargs`: The keyword arguments to pass to the `func` function.\n\n#### `apply`\n\nThe `apply` method applies a function to the secret value while keeping it encapsulated.\n\n```python\napply(self, func: Callable[[Any], Any], *args: Tuple[Any], **kwargs: Dict[str, Any]) -> SecretType:\n```\n\n- `func`: The function to apply to the secret value.\n- `args`: The positional arguments to pass to the `func` function.\n- `kwargs`: The keyword arguments to pass to the `func` function.\n\n#### `expose_secret`\n\nThe `expose_secret` method returns the value of the secret.\n\n```python\ndef expose_secret(self) -> T:\n```\n\n### Exceptions\n\n`sosecrets` defines the following exceptions:\n\n#### `CannotInstantiateExposeSecret`\n\nRaised when attempting to instantiate the `__expose_secret__` class.\n\n#### `CannotInheritFromSecret`\n\nRaised when attempting to subclass the `Secret` class.\n\n#### `FuncAndValueCannotBeBothPassed`\n\nRaised when both `value` and `func` arguments are passed to the `Secret` constructor.\n\n## Contributing\n\nContributions are welcome! Let me know if you need help with anything else.',
+    'long_description': '# sosecrets\n\n`sosecrets` is a Python module that provides a secure way to handle sensitive data by encapsulating it and only exposing it through a controlled interface.\n\nVersion: 0.1.3\n[Documentation](https://sosecrets.readthedocs.io/en/latest/)\n\n## Installation\n\nTo install `sosecrets`, you can use pip:\n\n```bash\npip install sosecrets\n```\n\n## Usage\n\nHere\'s are the examples of how to use `sosecrets`:\n\n### Secret\n\nHere\'s an example of how to use `Secret`:\n\n```python\nfrom sosecrets import Secret\n\n# Create a secret value\nsecret_value = Secret("my secret value")\n\n# Use the secret value while keeping it encapsulated\nresult = secret_value.apply(len)\nprint(result)  # Output: 14\n\n# Get the value of the secret\nvalue = secret_value.expose_secret()\nprint(value)  # Output: "my secret value"\n```\n\nIn this example, we create a `Secret` object with the value "my secret value". We then use the `apply` method to apply the `len` function to the secret value while keeping it encapsulated. Finally, we use the `expose_secret` method to retrieve the value of the secret.\n\n### ImmutableSecretMapping\n\nHere\'s an example of how to use `ImmutableSecretMapping`:\n\n```python\nfrom pathlib import Path\nfrom sosecrets import ImmutableSecretMapping\nfrom dotenv import dotenv_values\n\n# Define the path to the `.env` file\nTHIS_SCRIPT_FILE_PATH = Path(__file__)\nEXAMPLES = THIS_SCRIPT_FILE_PATH.parent / \'.env\'\n\n# Load the environment variables and store them securely\nsecret_env_dict = ImmutableSecretMapping.from_func(dotenv_values, dotenv_path=EXAMPLES)\n\n# Get a dictionary of the exposed values of the secret variables\nexposed_dict = secret_env_dict.expose_dict()\nprint("exposed_dict: ", exposed_dict)\n\n# Print the `ImmutableSecretMapping` object itself\nprint("secret_env_dict: ", secret_env_dict)\n\n# Get the value associated with a key using the `get()` method\nvalue0 = secret_env_dict.get(\'value0\')\nprint("value0: ", value0)\n\n# Get the exposed value of a key using the `get_exposed()` method\nvalue1 = secret_env_dict.get_exposed(\'value1\')\nprint("value1: ", value1)\n```\n\nThe example code does the following:\n\n1. Imports the necessary packages: `Path` from `pathlib`, `src` from the `sosecrets` module, `ImmutableSecretMapping` from `secretdicts` in the `sosecrets` module, and `dotenv_values` from the `dotenv` package.\n2. Defines the path to a `.env` file that contains environment variables to be loaded.\n3. Uses `ImmutableSecretMapping.from_func(dotenv_values, dotenv_path=EXAMPLES)` to load the environment variables from the `.env` file and store them in an instance of `ImmutableSecretMapping`.\n4. Prints the exposed dictionary of the `ImmutableSecretMapping` object using the `expose_dict()` method.\n5. Prints the `ImmutableSecretMapping` object itself.\n6. Gets a value from the `ImmutableSecretMapping` object using the `get()` method and prints it.\n7. Gets the exposed value of a key using the `get_exposed()` method## The Output\n\n### MutableSecretMapping\n\nSimilar to `ImmutableSecretMapping`.\n\n## Use Cases\nsosecrets can be used in a variety of scenarios where sensitive data needs to be securely handled. Here are some common use cases:\n\nStoring API keys, passwords, and other credentials: sosecrets can be used to securely store sensitive information such as API keys, passwords, and other credentials that are required for authentication or authorization in an application.\n\nHandling personal identifiable information (PII): sosecrets can be used to protect personal identifiable information (PII) such as names, addresses, social security numbers, and other sensitive data that needs to be kept confidential.\n\n## API Reference\n\n### `Secret`\n\nThe `Secret` class encapsulates a secret value and only exposes it through a controlled interface.\n\n```\nSecret(value: Optional[T] = None, func: Optional[Callable[[Any], T]] = None, func_args: Tuple[Any] = tuple(), func_kwargs: Dict[str, Any] = dict()) -> SecretType\n```\n\n- `value`: The secret value to encapsulate.\n- `func`: A function to generate the secret value.\n- `func_args`: The positional arguments to pass to the `func` function.\n- `func_kwargs`: The keyword arguments to pass to the `func` function.\n\n#### `apply`\n\nThe `apply` method applies a function to the secret value while keeping it encapsulated.\n\n```python\napply(self, func: Callable[[Any], Any], *args: Tuple[Any], **kwargs: Dict[str, Any]) -> SecretType:\n```\n\n- `func`: The function to apply to the secret value.\n- `args`: The positional arguments to pass to the `func` function.\n- `kwargs`: The keyword arguments to pass to the `func` function.\n\n#### `expose_secret`\n\nThe `expose_secret` method returns the value of the secret.\n\n```python\ndef expose_secret(self) -> T:\n```\n\n### Exceptions\n\n`sosecrets` defines the following exceptions:\n\n#### `CannotInstantiateExposeSecret`\n\nRaised when attempting to instantiate the `__expose_secret__` class.\n\n#### `CannotInheritFromSecret`\n\nRaised when attempting to subclass the `Secret` class.\n\n#### `FuncAndValueCannotBeBothPassed`\n\nRaised when both `value` and `func` arguments are passed to the `Secret` constructor.\n\n## Contributing\n\nContributions are welcome! Let me know if you need help with anything else.',
     'author': 'Jim Chng',
     'author_email': 'jimchng@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `sosecrets-0.1.2/PKG-INFO` & `sosecrets-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosecrets
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple wrapper to secure your secrets.
 License: MIT
 Keywords: secrets,security
 Author: Jim Chng
 Author-email: jimchng@outlook.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # sosecrets
 
 `sosecrets` is a Python module that provides a secure way to handle sensitive data by encapsulating it and only exposing it through a controlled interface.
 
-Version: 0.1.2
+Version: 0.1.3
+[Documentation](https://sosecrets.readthedocs.io/en/latest/)
 
 ## Installation
 
 To install `sosecrets`, you can use pip:
 
 ```bash
 pip install sosecrets
```

