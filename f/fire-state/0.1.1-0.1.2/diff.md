# Comparing `tmp/fire-state-0.1.1.tar.gz` & `tmp/fire_state-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fire-state-0.1.1.tar", max compression
+gzip compressed data, was "fire_state-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fire-state-0.1.1.tar` & `fire_state-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,11 @@
--rw-r--r--   0        0        0     1063 2022-07-01 11:53:38.989660 fire-state-0.1.1/LICENSE
--rw-r--r--   0        0        0     3678 2022-07-01 11:53:38.989660 fire-state-0.1.1/README.md
--rw-r--r--   0        0        0      118 2022-07-01 11:53:38.989660 fire-state-0.1.1/fire_state/__init__.py
--rw-r--r--   0        0        0     3932 2022-07-01 11:53:38.989660 fire-state-0.1.1/fire_state/state.py
--rw-r--r--   0        0        0      578 2022-07-01 11:53:38.989660 fire-state-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4464 2022-07-01 11:57:24.531668 fire-state-0.1.1/setup.py
--rw-r--r--   0        0        0     4332 2022-07-01 11:57:24.532003 fire-state-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      662 2023-05-27 03:16:41.542686 fire_state-0.1.2/.github/workflows/build.yaml
+-rw-r--r--   0        0        0      463 2023-05-27 03:16:41.542686 fire_state-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1063 2023-05-27 03:16:41.542686 fire_state-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3678 2023-05-27 03:16:41.546686 fire_state-0.1.2/README.md
+-rw-r--r--   0        0        0     1234 2023-05-27 03:16:41.546686 fire_state-0.1.2/demo/Home.py
+-rw-r--r--   0        0        0      327 2023-05-27 03:16:41.546686 fire_state-0.1.2/demo/pages/increment_button.py
+-rw-r--r--   0        0        0      866 2023-05-27 03:16:41.546686 fire_state-0.1.2/demo/pages/stateless_page.py
+-rw-r--r--   0        0        0      175 2023-05-27 03:16:41.546686 fire_state-0.1.2/fire_state/__init__.py
+-rw-r--r--   0        0        0     4056 2023-05-27 03:16:41.546686 fire_state-0.1.2/fire_state/state.py
+-rw-r--r--   0        0        0      523 2023-05-27 03:16:41.546686 fire_state-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4066 1970-01-01 00:00:00.000000 fire_state-0.1.2/PKG-INFO
```

### Comparing `fire-state-0.1.1/LICENSE` & `fire_state-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fire-state-0.1.1/README.md` & `fire_state-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fire-state-0.1.1/fire_state/state.py` & `fire_state-0.1.2/fire_state/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from typing import List, Tuple, Any
 
 import streamlit as st
-from streamlit.scriptrunner import get_script_run_ctx
+try:
+    from streamlit.scriptrunner import get_script_run_ctx
+except ImportError:
+    from streamlit.runtime.scriptrunner.script_run_context import \
+        get_script_run_ctx
 
 
 class Storage:
 
     def __init__(self):
         self._store = dict()
         self._slot_keys = dict()
```

### Comparing `fire-state-0.1.1/setup.py` & `fire_state-0.1.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,164 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: fire-state
+Version: 0.1.2
+Summary: Persist state across multiple pages in streamlit.
+Author-email: Mr-Milk <yb97643@um.edu.mo>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Developers
+Requires-Dist: streamlit
 
-packages = \
-['fire_state']
+# Streamlit fire state
 
-package_data = \
-{'': ['*']}
+[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://mr-milk-streamlit-state-demohome-mqsp3p.streamlitapp.com/)
+![pypi version](https://img.shields.io/pypi/v/fire-state?color=black&logo=python&logoColor=white&style=flat)
 
-install_requires = \
-['streamlit>=1.10.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'fire-state',
-    'version': '0.1.1',
-    'description': '',
-    'long_description': '# Streamlit fire state\n\n[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://mr-milk-streamlit-state-demohome-mqsp3p.streamlitapp.com/)\n![pypi version](https://img.shields.io/pypi/v/fire-state?color=black&logo=python&logoColor=white&style=flat)\n\nIn a multipage streamlit app, one of the most headache issues \nis that your state is not preserved if you switch between pages.\n\nThat\'s why fire-state is here for you.\n\n## Installation\n\n```shell\npip install fire-state\n```\n\n## Quick Start\n\n### Persist state in Form\n\n```python\nimport streamlit as st\nfrom fire_state import create_store, form_update\n\n# Register state with initiate values in a slot\nslot = "home_page"\nkey1, key2 = create_store(slot, [\n    ("state1", 5),\n    ("state2", 12),\n])\n\n# Now create a form using the generated keys\nwith st.form("my form"):\n    st.slider("State 1", 1, 10, step=1, key=key1)\n    st.slider("State 1", 10, 20, step=1, key=key2)\n    st.form_submit_button(label="Submit", on_click=form_update, args=(slot,))\n\n```\n\nWhen you switch between pages, the states are preserved.\n\n### Persist state in any place\n\nYou need to control the state by yourself, using the `set_state` function.\n\n```python\nimport streamlit as st\nfrom fire_state import create_store, get_state, set_state\n\n\nslot = "home_page"\ncreate_store(slot, [\n    ("state1", 0),\n])\n\ndef increment():\n    prev = get_state(slot, "state1")\n    set_state(slot, ("state1", prev + 1))\n\n\nst.button("+1", on_click=increment)\nst.text(f"Value: {get_state(slot, \'state1\')}")\n```\n\n## Advanced Usage\n\n### Persist state after form submission\n\nIn this example, we have a form to control \nhow the line chart is drawn.\n\nLet\'s do some setup first\n\n```python\nimport numpy as np\nimport pandas as pd\nimport streamlit as st\n\nnp.random.seed(0)\n\n@st.cache\ndef chart_data(line_count, data_size):\n    return pd.DataFrame(\n        np.random.randn(data_size, line_count),\n        columns=np.random.choice(list(\'abcdefghijlkmn\'), line_count))\n\n```\n\nNow we can use fire state to record the user action.\n\nThe idea is that the first time user opens the page, they never click the run button,\nso the number of times they click a button is 0. When it no longer is 0, which means user clicked it. \nTherefore, the plot is rendered or updated (if chart data is changed).\n\n\n```python\nfrom fire_state import create_store, get_state, set_state, form_update\n\nPAGE_SLOT = "Home_Page"\nkey1, key2, key3 = create_store(PAGE_SLOT, [\n    ("line_count", 2),\n    ("data_size", 13),\n    ("run", 0)\n])\n\nwith st.form(key="a form"):\n    line_count = st.slider("Line Count", 1, 10, step=1, key=key1)\n    data_size = st.slider("Data Size", 10, 20, step=1, key=key2)\n    run = st.form_submit_button(label="Run", on_click=form_update, args=(PAGE_SLOT,))\n\nprev_run_state = get_state(PAGE_SLOT, \'run\')\nif (prev_run_state != 0) or run:\n    data = chart_data(line_count, data_size)\n    st.line_chart(data)\n    # increase by 1 every time user click it\n    set_state(PAGE_SLOT, ("run", prev_run_state + 1))\n```\n\n\n### Reset the state\n\nUse the `set_store` function to update states in a batch:\n\n```python\nimport streamlit as st\nfrom fire_state import create_store, \\\n    get_store, set_store, \\\n    get_state, set_state\n\nslot = "page"\ninit_state = [\n    ("state1", 1),\n    ("state2", 2),\n    ("state3", 3),\n]\ncreate_store(slot, init_state)\n\ndef reset():\n    set_store(slot, init_state)\n\nst.button("Reset", on_click=reset)\n```\n\nThe `set_store` and `get_store` functions allow you to\nmodify and get your state in a batch.\n\n\n## The Life Cycle of State\n\nThe state persists if you don\'t close or refresh the page. The state instance\nis only destroyed if you stop your app.\n',
-    'author': 'Mr-Milk',
-    'author_email': 'yb97643@um.edu.mo',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/Mr-Milk/streamlit-state',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+In a multipage streamlit app, one of the most headache issues 
+is that your state is not preserved if you switch between pages.
 
+That's why fire-state is here for you.
+
+## Installation
+
+```shell
+pip install fire-state
+```
+
+## Quick Start
+
+### Persist state in Form
+
+```python
+import streamlit as st
+from fire_state import create_store, form_update
+
+# Register state with initiate values in a slot
+slot = "home_page"
+key1, key2 = create_store(slot, [
+    ("state1", 5),
+    ("state2", 12),
+])
+
+# Now create a form using the generated keys
+with st.form("my form"):
+    st.slider("State 1", 1, 10, step=1, key=key1)
+    st.slider("State 1", 10, 20, step=1, key=key2)
+    st.form_submit_button(label="Submit", on_click=form_update, args=(slot,))
+
+```
+
+When you switch between pages, the states are preserved.
+
+### Persist state in any place
+
+You need to control the state by yourself, using the `set_state` function.
+
+```python
+import streamlit as st
+from fire_state import create_store, get_state, set_state
+
+
+slot = "home_page"
+create_store(slot, [
+    ("state1", 0),
+])
+
+def increment():
+    prev = get_state(slot, "state1")
+    set_state(slot, ("state1", prev + 1))
+
+
+st.button("+1", on_click=increment)
+st.text(f"Value: {get_state(slot, 'state1')}")
+```
+
+## Advanced Usage
+
+### Persist state after form submission
+
+In this example, we have a form to control 
+how the line chart is drawn.
+
+Let's do some setup first
+
+```python
+import numpy as np
+import pandas as pd
+import streamlit as st
+
+np.random.seed(0)
+
+@st.cache
+def chart_data(line_count, data_size):
+    return pd.DataFrame(
+        np.random.randn(data_size, line_count),
+        columns=np.random.choice(list('abcdefghijlkmn'), line_count))
+
+```
+
+Now we can use fire state to record the user action.
+
+The idea is that the first time user opens the page, they never click the run button,
+so the number of times they click a button is 0. When it no longer is 0, which means user clicked it. 
+Therefore, the plot is rendered or updated (if chart data is changed).
+
+
+```python
+from fire_state import create_store, get_state, set_state, form_update
+
+PAGE_SLOT = "Home_Page"
+key1, key2, key3 = create_store(PAGE_SLOT, [
+    ("line_count", 2),
+    ("data_size", 13),
+    ("run", 0)
+])
+
+with st.form(key="a form"):
+    line_count = st.slider("Line Count", 1, 10, step=1, key=key1)
+    data_size = st.slider("Data Size", 10, 20, step=1, key=key2)
+    run = st.form_submit_button(label="Run", on_click=form_update, args=(PAGE_SLOT,))
+
+prev_run_state = get_state(PAGE_SLOT, 'run')
+if (prev_run_state != 0) or run:
+    data = chart_data(line_count, data_size)
+    st.line_chart(data)
+    # increase by 1 every time user click it
+    set_state(PAGE_SLOT, ("run", prev_run_state + 1))
+```
+
+
+### Reset the state
+
+Use the `set_store` function to update states in a batch:
+
+```python
+import streamlit as st
+from fire_state import create_store, \
+    get_store, set_store, \
+    get_state, set_state
+
+slot = "page"
+init_state = [
+    ("state1", 1),
+    ("state2", 2),
+    ("state3", 3),
+]
+create_store(slot, init_state)
+
+def reset():
+    set_store(slot, init_state)
+
+st.button("Reset", on_click=reset)
+```
+
+The `set_store` and `get_store` functions allow you to
+modify and get your state in a batch.
+
+
+## The Life Cycle of State
+
+The state persists if you don't close or refresh the page. The state instance
+is only destroyed if you stop your app.
 
-setup(**setup_kwargs)
```

