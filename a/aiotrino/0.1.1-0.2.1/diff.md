# Comparing `tmp/aiotrino-0.1.1.tar.gz` & `tmp/aiotrino-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\aiotrino-0.1.1.tar", last modified: Tue May 10 18:34:22 2022, max compression
+gzip compressed data, was "aiotrino-0.2.1.tar", last modified: Sat May 27 18:37:27 2023, max compression
```

## Comparing `aiotrino-0.1.1.tar` & `aiotrino-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-05-10 18:34:22.000000 aiotrino-0.1.1/
--rw-rw-rw-   0        0        0    11358 2021-01-09 04:33:37.000000 aiotrino-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     7358 2022-05-10 18:34:22.000000 aiotrino-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5974 2021-04-17 03:06:48.000000 aiotrino-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-05-10 18:34:22.000000 aiotrino-0.1.1/aiotrino/
--rw-rw-rw-   0        0        0      634 2022-05-10 18:26:30.000000 aiotrino-0.1.1/aiotrino/__init__.py
--rw-rw-rw-   0        0        0     4068 2021-01-15 18:18:36.000000 aiotrino-0.1.1/aiotrino/auth.py
--rw-rw-rw-   0        0        0    23291 2022-05-10 18:23:59.000000 aiotrino-0.1.1/aiotrino/client.py
--rw-rw-rw-   0        0        0     2089 2021-01-15 19:14:42.000000 aiotrino-0.1.1/aiotrino/constants.py
--rw-rw-rw-   0        0        0    17444 2022-05-10 18:24:13.000000 aiotrino-0.1.1/aiotrino/dbapi.py
--rw-rw-rw-   0        0        0     5198 2021-04-16 21:12:09.000000 aiotrino-0.1.1/aiotrino/exceptions.py
--rw-rw-rw-   0        0        0      765 2021-01-15 18:18:37.000000 aiotrino-0.1.1/aiotrino/logging.py
--rw-rw-rw-   0        0        0     3580 2021-04-17 03:00:32.000000 aiotrino-0.1.1/aiotrino/transaction.py
--rw-rw-rw-   0        0        0      431 2021-04-16 23:55:45.000000 aiotrino-0.1.1/aiotrino/utils.py
-drwxrwxrwx   0        0        0        0 2022-05-10 18:34:22.000000 aiotrino-0.1.1/aiotrino.egg-info/
--rw-rw-rw-   0        0        0     7358 2022-05-10 18:34:22.000000 aiotrino-0.1.1/aiotrino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2022-05-10 18:34:22.000000 aiotrino-0.1.1/aiotrino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-10 18:34:22.000000 aiotrino-0.1.1/aiotrino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      170 2022-05-10 18:34:22.000000 aiotrino-0.1.1/aiotrino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-05-10 18:34:22.000000 aiotrino-0.1.1/aiotrino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      128 2022-05-10 18:34:22.000000 aiotrino-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2463 2022-05-10 18:24:42.000000 aiotrino-0.1.1/setup.py
+drwxrwxr-x   0 michiel   (1000) michiel   (1000)        0 2023-05-27 18:37:27.218042 aiotrino-0.2.1/
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)    11358 2023-05-27 16:11:32.000000 aiotrino-0.2.1/LICENSE
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)     8397 2023-05-27 18:37:27.222042 aiotrino-0.2.1/PKG-INFO
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)     7178 2023-05-27 18:37:26.000000 aiotrino-0.2.1/README.md
+drwxrwxr-x   0 michiel   (1000) michiel   (1000)        0 2023-05-27 18:37:27.218042 aiotrino-0.2.1/aiotrino/
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)      634 2023-05-27 18:35:33.000000 aiotrino-0.2.1/aiotrino/__init__.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)     4705 2023-05-27 16:11:32.000000 aiotrino-0.2.1/aiotrino/auth.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)    23291 2023-05-27 16:11:32.000000 aiotrino-0.2.1/aiotrino/client.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)     2089 2023-05-27 16:11:32.000000 aiotrino-0.2.1/aiotrino/constants.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)    17444 2023-05-27 16:11:32.000000 aiotrino-0.2.1/aiotrino/dbapi.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)     5198 2023-05-27 16:11:32.000000 aiotrino-0.2.1/aiotrino/exceptions.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)      765 2023-05-27 16:11:32.000000 aiotrino-0.2.1/aiotrino/logging.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)     3580 2023-05-27 16:11:32.000000 aiotrino-0.2.1/aiotrino/transaction.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)      431 2023-05-27 16:11:32.000000 aiotrino-0.2.1/aiotrino/utils.py
+drwxrwxr-x   0 michiel   (1000) michiel   (1000)        0 2023-05-27 18:37:27.218042 aiotrino-0.2.1/aiotrino.egg-info/
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)     8397 2023-05-27 18:37:27.000000 aiotrino-0.2.1/aiotrino.egg-info/PKG-INFO
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)      442 2023-05-27 18:37:27.000000 aiotrino-0.2.1/aiotrino.egg-info/SOURCES.txt
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)        1 2023-05-27 18:37:27.000000 aiotrino-0.2.1/aiotrino.egg-info/dependency_links.txt
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)      170 2023-05-27 18:37:27.000000 aiotrino-0.2.1/aiotrino.egg-info/requires.txt
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)        9 2023-05-27 18:37:27.000000 aiotrino-0.2.1/aiotrino.egg-info/top_level.txt
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)      150 2023-05-27 18:37:27.222042 aiotrino-0.2.1/setup.cfg
+-rwxrwxr-x   0 michiel   (1000) michiel   (1000)     2547 2023-05-27 16:48:52.000000 aiotrino-0.2.1/setup.py
+drwxrwxr-x   0 michiel   (1000) michiel   (1000)        0 2023-05-27 18:37:27.218042 aiotrino-0.2.1/tests/
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)    24153 2023-05-27 16:11:32.000000 aiotrino-0.2.1/tests/test_client.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)     2136 2023-05-27 16:11:32.000000 aiotrino-0.2.1/tests/test_exceptions.py
+-rw-rw-r--   0 michiel   (1000) michiel   (1000)     1067 2023-05-27 16:11:32.000000 aiotrino-0.2.1/tests/test_http.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aiotrino-0.1.1/LICENSE` & `aiotrino-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotrino-0.1.1/PKG-INFO` & `aiotrino-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,231 +1,289 @@
-Metadata-Version: 2.1
-Name: aiotrino
-Version: 0.1.1
-Summary: ASyncIO Client for the Trino distributed SQL Engine
-Home-page: https://github.com/mvanderlee/trino-python-client/tree/py3-async
-Author: Michiel Van Der Lee, Trino Team
-Author-email: jmt.vanderlee@gmail.com
-License: Apache 2.0
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Database :: Front-Ends
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: kerberos
-Provides-Extra: tests
-License-File: LICENSE
-
-[![Build Status](https://github.com/mvanderlee/trino-python-client/workflows/ci/badge.svg)](https://github.com/mvanderlee/trino-python-client/actions?query=workflow%3Aci+event%3Apush+branch%3Apy3-async)
-[![Trino Slack](https://img.shields.io/static/v1?logo=slack&logoColor=959DA5&label=Slack&labelColor=333a41&message=join%20conversation&color=3AC358)](https://trino.io/slack.html)
-[![Presto: The Definitive Guide book download](https://img.shields.io/badge/Presto%3A%20The%20Definitive%20Guide-download-brightgreen)](https://www.starburstdata.com/oreilly-presto-guide-download/)
-
-# Introduction
-
-This package provides a asyncio client interface to query [Trino](https://trino.io/)
-a distributed SQL engine. It supports Python 3.6, 3.7, and pypy.
-# Installation
-
-```
-$ pip install aiotrino
-```
-
-# Quick Start
-
-Use the DBAPI interface to query Trino:
-
-```python
-import aiotrino
-conn = aiotrino.dbapi.connect(
-    host='localhost',
-    port=8080,
-    user='the-user',
-    catalog='the-catalog',
-    schema='the-schema',
-)
-await cur = conn.cursor()
-await cur.execute('SELECT * FROM system.runtime.nodes')
-rows = await cur.fetchall()
-await conn.close()
-```
-Or with context manager 
-```python
-import aiotrino
-async with aiotrino.dbapi.connect(
-    host='localhost',
-    port=8080,
-    user='the-user',
-    catalog='the-catalog',
-    schema='the-schema',
-) as conn:
-    await cur = conn.cursor()
-    await cur.execute('SELECT * FROM system.runtime.nodes')
-    rows = await cur.fetchall()
-```
-
-This will query the `system.runtime.nodes` system tables that shows the nodes
-in the Trino cluster.
-
-The DBAPI implementation in `aiotrino.dbapi` provides methods to retrieve fewer
-rows for example `Cursorfetchone()` or `Cursor.fetchmany()`. By default
-`Cursor.fetchmany()` fetches one row. Please set
-`trino.dbapi.Cursor.arraysize` accordingly.
-
-For backwards compatibility with PrestoSQL, override the headers at the start of your application
-```python
-import aiotrino
-aiotrino.constants.HEADERS = aiotrino.constants.PrestoHeaders
-```
-
-# Basic Authentication
-The `BasicAuthentication` class can be used to connect to a LDAP-configured Trino
-cluster:
-```python
-import aiotrino
-conn = aiotrino.dbapi.connect(
-    host='coordinator url',
-    port=8443,
-    user='the-user',
-    catalog='the-catalog',
-    schema='the-schema',
-    http_scheme='https',
-    auth=aiotrino.auth.BasicAuthentication("principal id", "password"),
-)
-cur = await conn.cursor()
-await cur.execute('SELECT * FROM system.runtime.nodes')
-rows = await cur.fetchall()
-await conn.close()
-```
-
-# Transactions
-The client runs by default in *autocommit* mode. To enable transactions, set
-*isolation_level* to a value different than `IsolationLevel.AUTOCOMMIT`:
-
-```python
-import aiotrino
-from aiotrino import transaction
-async with aiotrino.dbapi.connect(
-    host='localhost',
-    port=8080,
-    user='the-user',
-    catalog='the-catalog',
-    schema='the-schema',
-    isolation_level=transaction.IsolationLevel.REPEATABLE_READ,
-) as conn:
-  cur = await conn.cursor()
-  await cur.execute('INSERT INTO sometable VALUES (1, 2, 3)')
-  await cur.fetchone()
-  await cur.execute('INSERT INTO sometable VALUES (4, 5, 6)')
-  await cur.fetchone()
-```
-
-The transaction is created when the first SQL statement is executed.
-`trino.dbapi.Connection.commit()` will be automatically called when the code
-exits the *with* context and the queries succeed, otherwise
-`trino.dbapi.Connection.rollback()' will be called.
-
-# Development
-
-## Getting Started With Development
-
-Start by forking the repository and then modify the code in your fork.
-
-Clone the repository and go inside the code directory. Then you can get the
-version with `./setup.py --version`.
-
-We recommend that you use `virtualenv` for development:
-
-```
-$ virtualenv .venv
-$ . .venv/bin/activate
-# TODO add requirements.txt: pip install -r requirements.txt
-$ pip install .
-```
-
-For development purpose, pip can reference the code you are modifying in a
-*virtualenv*:
-
-```
-$ pip install -e .[tests]
-```
-
-That way, you do not need to run `pip install` again to make your changes
-applied to the *virtualenv*.
-
-When the code is ready, submit a Pull Request.
-
-## Code Style
-
-- For Python code, adhere to PEP 8.
-- Prefer code that is readable over one that is "clever".
-- When writing a Git commit message, follow these [guidelines](https://chris.beams.io/posts/git-commit/).
-
-## Running Tests
-
-There is a helper scripts, `run`, that provides commands to run tests.
-Type `./run tests` to run both unit and integration tests.
-
-`trino-python-client` uses [pytest](https://pytest.org/) for its tests. To run
-only unit tests, type:
-
-```
-$ pytest tests
-```
-
-Then you can pass options like `--pdb` or anything supported by `pytest --help`.
-
-To run the tests with different versions of Python in managed *virtualenvs*,
-use `tox` (see the configuration in `tox.ini`):
-
-```
-$ tox
-```
-
-To run integration tests:
-
-```
-$ pytest integration_tests
-```
-
-They pull a Docker image and then run a container with a Trino server:
-- the image is named `trinodb/trino:${TRINO_VERSION}`
-- the container is named `trino-python-client-tests-{uuid4()[:7]}`
-
-## Releasing
-
-- [Set up your development environment](#Getting-Started-With-Development).
-- Change version in `trino/__init__.py`.
-- Commit and create an annotated tag (`git tag -m '' current_version`)
-- Run the following:
-  ```bash
-  . .venv/bin/activate &&
-  pip install twine &&
-  rm -rf dist/ &&
-  ./setup.py sdist bdist_wheel &&
-  twine upload dist/* &&
-  open https://pypi.org/project/trino/ &&
-  echo "Released!"
-  ```
-- Push the branch and the tag (`git push upstream master current_version`)
-- Send release announcement.
-
-# Need Help?
-
-Feel free to create an issue as it make your request visible to other users and contributors.
-
-If an interactive discussion would be better or if you just want to hangout and chat about
-the Trino Python client, you can join us on the *#python-client* channel on
-[Trino Slack](https://trino.io/slack.html).
-
-
+Metadata-Version: 2.1
+Name: aiotrino
+Version: 0.2.1
+Summary: ASyncIO Client for the Trino distributed SQL Engine
+Home-page: https://github.com/mvanderlee/aiotrino/tree/main
+Author: Michiel Van Der Lee, Trino Team
+Author-email: jmt.vanderlee@gmail.com
+License: Apache 2.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Database :: Front-Ends
+Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: kerberos
+Provides-Extra: tests
+License-File: LICENSE
+
+[![Build Status](https://github.com/mvanderlee/trino-python-client/workflows/ci/badge.svg)](https://github.com/mvanderlee/trino-python-client/actions?query=workflow%3Aci+event%3Apush+branch%3Apy3-async)
+[![Trino Slack](https://img.shields.io/static/v1?logo=slack&logoColor=959DA5&label=Slack&labelColor=333a41&message=join%20conversation&color=3AC358)](https://trino.io/slack.html)
+[![Presto: The Definitive Guide book download](https://img.shields.io/badge/Presto%3A%20The%20Definitive%20Guide-download-brightgreen)](https://www.starburstdata.com/oreilly-presto-guide-download/)
+
+# Introduction
+
+This package provides a asyncio client interface to query [Trino](https://trino.io/)
+a distributed SQL engine. It supports Python 3.7, 3.8, 3.9, 3.10, 3.11.
+# Installation
+
+```
+$ pip install aiotrino
+```
+
+# Quick Start
+
+Use the DBAPI interface to query Trino:
+
+```python
+import aiotrino
+conn = aiotrino.dbapi.connect(
+    host='localhost',
+    port=8080,
+    user='the-user',
+    catalog='the-catalog',
+    schema='the-schema',
+)
+await cur = conn.cursor()
+await cur.execute('SELECT * FROM system.runtime.nodes')
+rows = await cur.fetchall()
+await conn.close()
+```
+Or with context manager 
+```python
+import aiotrino
+async with aiotrino.dbapi.connect(
+    host='localhost',
+    port=8080,
+    user='the-user',
+    catalog='the-catalog',
+    schema='the-schema',
+) as conn:
+    await cur = conn.cursor()
+    await cur.execute('SELECT * FROM system.runtime.nodes')
+    rows = await cur.fetchall()
+```
+
+This will query the `system.runtime.nodes` system tables that shows the nodes
+in the Trino cluster.
+
+The DBAPI implementation in `aiotrino.dbapi` provides methods to retrieve fewer
+rows for example `Cursorfetchone()` or `Cursor.fetchmany()`. By default
+`Cursor.fetchmany()` fetches one row. Please set
+`trino.dbapi.Cursor.arraysize` accordingly.
+
+For backwards compatibility with PrestoSQL, override the headers at the start of your application
+```python
+import aiotrino
+aiotrino.constants.HEADERS = aiotrino.constants.PrestoHeaders
+```
+
+# Basic Authentication
+The `BasicAuthentication` class can be used to connect to a LDAP-configured Trino
+cluster:
+```python
+import aiotrino
+conn = aiotrino.dbapi.connect(
+    host='coordinator url',
+    port=8443,
+    user='the-user',
+    catalog='the-catalog',
+    schema='the-schema',
+    http_scheme='https',
+    auth=aiotrino.auth.BasicAuthentication("principal id", "password"),
+)
+cur = await conn.cursor()
+await cur.execute('SELECT * FROM system.runtime.nodes')
+rows = await cur.fetchall()
+await conn.close()
+```
+
+# JWT Token Authentication
+The `JWTAuthentication` class can be used to connect to a configured Trino cluster:
+```python
+import aiotrino
+conn = aiotrino.dbapi.connect(
+    host='coordinator url',
+    port=8443,
+    catalog='the-catalog',
+    schema='the-schema',
+    http_scheme='https',
+    auth=aiotrino.auth.JWTAuthentication(token="jwt-token"),
+)
+cur = await conn.cursor()
+await cur.execute('SELECT * FROM system.runtime.nodes')
+rows = await cur.fetchall()
+await conn.close()
+```
+
+# Transactions
+The client runs by default in *autocommit* mode. To enable transactions, set
+*isolation_level* to a value different than `IsolationLevel.AUTOCOMMIT`:
+
+```python
+import aiotrino
+from aiotrino import transaction
+async with aiotrino.dbapi.connect(
+    host='localhost',
+    port=8080,
+    user='the-user',
+    catalog='the-catalog',
+    schema='the-schema',
+    isolation_level=transaction.IsolationLevel.REPEATABLE_READ,
+) as conn:
+  cur = await conn.cursor()
+  await cur.execute('INSERT INTO sometable VALUES (1, 2, 3)')
+  await cur.fetchone()
+  await cur.execute('INSERT INTO sometable VALUES (4, 5, 6)')
+  await cur.fetchone()
+```
+
+The transaction is created when the first SQL statement is executed.
+`trino.dbapi.Connection.commit()` will be automatically called when the code
+exits the *with* context and the queries succeed, otherwise
+`trino.dbapi.Connection.rollback()' will be called.
+
+# Development
+
+## Getting Started With Development
+
+Start by forking the repository and then modify the code in your fork.
+
+Clone the repository and go inside the code directory. Then you can get the
+version with `./setup.py --version`.
+
+We recommend that you use `virtualenv` for development:
+
+```
+$ virtualenv .venv
+$ . .venv/bin/activate
+# TODO add requirements.txt: pip install -r requirements.txt
+$ pip install .
+```
+
+For development purpose, pip can reference the code you are modifying in a
+*virtualenv*:
+
+```
+$ pip install -e .[tests]
+```
+
+That way, you do not need to run `pip install` again to make your changes
+applied to the *virtualenv*.
+
+When the code is ready, submit a Pull Request.
+
+## Code Style
+
+- For Python code, adhere to PEP 8.
+- Prefer code that is readable over one that is "clever".
+- When writing a Git commit message, follow these [guidelines](https://chris.beams.io/posts/git-commit/).
+
+## Running Tests
+
+There is a helper scripts, `run`, that provides commands to run tests.
+Type `./run tests` to run both unit and integration tests.
+
+`trino-python-client` uses [pytest](https://pytest.org/) for its tests. To run
+only unit tests, type:
+
+```
+$ pytest tests
+```
+
+Then you can pass options like `--pdb` or anything supported by `pytest --help`.
+
+To run the tests with different versions of Python in managed *virtualenvs*,
+use `tox` (see the configuration in `tox.ini`):
+
+```
+$ tox
+```
+
+To run integration tests:
+
+```
+$ pytest integration_tests
+```
+
+They pull a Docker image and then run a container with a Trino server:
+- the image is named `trinodb/trino:${TRINO_VERSION}`
+- the container is named `trino-python-client-tests-{uuid4()[:7]}`
+
+
+### Test setup
+
+Supported OS Ubuntu 22.04
+
+1. Install [pyenv](https://github.com/pyenv/pyenv#automatic-installer)
+
+    ```shell
+    curl https://pyenv.run | bash
+    ```
+
+2. Install required python versions
+
+    ```shell
+    # Install the latest of all supported versions
+    pyenv install 3.7, 3.8, 3.9, 3.10, 3.11
+    ```
+
+3. Set the installed versions as default for the shell. This allows `tox` to find them.
+
+    List installed versions and update the following command as needed.
+    ```shell
+    pyenv versions
+    ```
+
+    ```shell
+    pyenv shell 3.11.3 3.10.11 3.9.16 3.8.16 3.7.16
+    ```
+
+4. Install `tox`
+
+    ```shell
+    pip install tox
+    ```
+
+5. Run `tox`
+
+    ```shell
+    tox
+    ```
+
+## Releasing
+
+- [Set up your development environment](#Getting-Started-With-Development).
+- Change version in `trino/__init__.py`.
+- Commit and create an annotated tag (`git tag -m '' current_version`)
+- Run the following:
+  ```bash
+  . .venv/bin/activate &&
+  pip install twine wheel &&
+  rm -rf dist/ &&
+  ./setup.py sdist bdist_wheel &&
+  twine upload dist/* &&
+  open https://pypi.org/project/trino/ &&
+  echo "Released!"
+  ```
+- Push the branch and the tag (`git push upstream master current_version`)
+- Send release announcement.
+
+# Need Help?
+
+Feel free to create an issue as it make your request visible to other users and contributors.
+
+If an interactive discussion would be better or if you just want to hangout and chat about
+the Trino Python client, you can join us on the *#python-client* channel on
+[Trino Slack](https://trino.io/slack.html).
```

### Comparing `aiotrino-0.1.1/README.md` & `aiotrino-0.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [![Build Status](https://github.com/mvanderlee/trino-python-client/workflows/ci/badge.svg)](https://github.com/mvanderlee/trino-python-client/actions?query=workflow%3Aci+event%3Apush+branch%3Apy3-async)
 [![Trino Slack](https://img.shields.io/static/v1?logo=slack&logoColor=959DA5&label=Slack&labelColor=333a41&message=join%20conversation&color=3AC358)](https://trino.io/slack.html)
 [![Presto: The Definitive Guide book download](https://img.shields.io/badge/Presto%3A%20The%20Definitive%20Guide-download-brightgreen)](https://www.starburstdata.com/oreilly-presto-guide-download/)
 
 # Introduction
 
 This package provides a asyncio client interface to query [Trino](https://trino.io/)
-a distributed SQL engine. It supports Python 3.6, 3.7, and pypy.
+a distributed SQL engine. It supports Python 3.7, 3.8, 3.9, 3.10, 3.11.
 # Installation
 
 ```
 $ pip install aiotrino
 ```
 
 # Quick Start
@@ -75,14 +75,32 @@
 )
 cur = await conn.cursor()
 await cur.execute('SELECT * FROM system.runtime.nodes')
 rows = await cur.fetchall()
 await conn.close()
 ```
 
+# JWT Token Authentication
+The `JWTAuthentication` class can be used to connect to a configured Trino cluster:
+```python
+import aiotrino
+conn = aiotrino.dbapi.connect(
+    host='coordinator url',
+    port=8443,
+    catalog='the-catalog',
+    schema='the-schema',
+    http_scheme='https',
+    auth=aiotrino.auth.JWTAuthentication(token="jwt-token"),
+)
+cur = await conn.cursor()
+await cur.execute('SELECT * FROM system.runtime.nodes')
+rows = await cur.fetchall()
+await conn.close()
+```
+
 # Transactions
 The client runs by default in *autocommit* mode. To enable transactions, set
 *isolation_level* to a value different than `IsolationLevel.AUTOCOMMIT`:
 
 ```python
 import aiotrino
 from aiotrino import transaction
@@ -169,23 +187,64 @@
 $ pytest integration_tests
 ```
 
 They pull a Docker image and then run a container with a Trino server:
 - the image is named `trinodb/trino:${TRINO_VERSION}`
 - the container is named `trino-python-client-tests-{uuid4()[:7]}`
 
+
+### Test setup
+
+Supported OS Ubuntu 22.04
+
+1. Install [pyenv](https://github.com/pyenv/pyenv#automatic-installer)
+
+    ```shell
+    curl https://pyenv.run | bash
+    ```
+
+2. Install required python versions
+
+    ```shell
+    # Install the latest of all supported versions
+    pyenv install 3.7, 3.8, 3.9, 3.10, 3.11
+    ```
+
+3. Set the installed versions as default for the shell. This allows `tox` to find them.
+
+    List installed versions and update the following command as needed.
+    ```shell
+    pyenv versions
+    ```
+
+    ```shell
+    pyenv shell 3.11.3 3.10.11 3.9.16 3.8.16 3.7.16
+    ```
+
+4. Install `tox`
+
+    ```shell
+    pip install tox
+    ```
+
+5. Run `tox`
+
+    ```shell
+    tox
+    ```
+
 ## Releasing
 
 - [Set up your development environment](#Getting-Started-With-Development).
 - Change version in `trino/__init__.py`.
 - Commit and create an annotated tag (`git tag -m '' current_version`)
 - Run the following:
   ```bash
   . .venv/bin/activate &&
-  pip install twine &&
+  pip install twine wheel &&
   rm -rf dist/ &&
   ./setup.py sdist bdist_wheel &&
   twine upload dist/* &&
   open https://pypi.org/project/trino/ &&
   echo "Released!"
   ```
 - Push the branch and the tag (`git push upstream master current_version`)
```

### Comparing `aiotrino-0.1.1/aiotrino/__init__.py` & `aiotrino-0.2.1/aiotrino/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from . import auth, client, constants, dbapi, exceptions, logging
 
-__version__ = "0.1.1"
+__version__ = "0.2.1"
```

### Comparing `aiotrino-0.1.1/aiotrino/auth.py` & `aiotrino-0.2.1/aiotrino/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import abc
 
 import aiohttp
-
+from typing import Tuple, Any
+# from requests.auth import AuthBase, extract_cookies_to_jar
 
 class Authentication(abc.ABC):  # type: ignore
     @abc.abstractmethod
     def set_http_session(self, http_session):
         pass
 
     @abc.abstractmethod
@@ -117,7 +118,27 @@
         self.set_http_session(trino_client.http_session)
 
     def get_exceptions(self):
         return ()
 
     def handle_error(self, handle_error):
         pass
+    
+
+class JWTAuthentication(Authentication):
+
+    def __init__(self, token: str):
+        self.token = token
+
+    def setup(self, trino_client):
+        self.set_client_session(trino_client.client_session)
+        self.set_http_session(trino_client.http_session)
+
+    def set_http_session(self, http_session):
+        http_session.headers["Authorization"] = "Bearer " + self.token
+        return http_session
+    
+    def set_client_session(self, client_session):
+        pass
+
+    def get_exceptions(self) -> Tuple[Any, ...]:
+        return ()
```

### Comparing `aiotrino-0.1.1/aiotrino/client.py` & `aiotrino-0.2.1/aiotrino/client.py`

 * *Files identical despite different names*

### Comparing `aiotrino-0.1.1/aiotrino/constants.py` & `aiotrino-0.2.1/aiotrino/constants.py`

 * *Files identical despite different names*

### Comparing `aiotrino-0.1.1/aiotrino/dbapi.py` & `aiotrino-0.2.1/aiotrino/dbapi.py`

 * *Files identical despite different names*

### Comparing `aiotrino-0.1.1/aiotrino/exceptions.py` & `aiotrino-0.2.1/aiotrino/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiotrino-0.1.1/aiotrino/logging.py` & `aiotrino-0.2.1/aiotrino/logging.py`

 * *Files identical despite different names*

### Comparing `aiotrino-0.1.1/aiotrino/transaction.py` & `aiotrino-0.2.1/aiotrino/transaction.py`

 * *Files identical despite different names*

### Comparing `aiotrino-0.1.1/aiotrino.egg-info/PKG-INFO` & `aiotrino-0.2.1/aiotrino.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,231 +1,289 @@
-Metadata-Version: 2.1
-Name: aiotrino
-Version: 0.1.1
-Summary: ASyncIO Client for the Trino distributed SQL Engine
-Home-page: https://github.com/mvanderlee/trino-python-client/tree/py3-async
-Author: Michiel Van Der Lee, Trino Team
-Author-email: jmt.vanderlee@gmail.com
-License: Apache 2.0
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Database :: Front-Ends
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: kerberos
-Provides-Extra: tests
-License-File: LICENSE
-
-[![Build Status](https://github.com/mvanderlee/trino-python-client/workflows/ci/badge.svg)](https://github.com/mvanderlee/trino-python-client/actions?query=workflow%3Aci+event%3Apush+branch%3Apy3-async)
-[![Trino Slack](https://img.shields.io/static/v1?logo=slack&logoColor=959DA5&label=Slack&labelColor=333a41&message=join%20conversation&color=3AC358)](https://trino.io/slack.html)
-[![Presto: The Definitive Guide book download](https://img.shields.io/badge/Presto%3A%20The%20Definitive%20Guide-download-brightgreen)](https://www.starburstdata.com/oreilly-presto-guide-download/)
-
-# Introduction
-
-This package provides a asyncio client interface to query [Trino](https://trino.io/)
-a distributed SQL engine. It supports Python 3.6, 3.7, and pypy.
-# Installation
-
-```
-$ pip install aiotrino
-```
-
-# Quick Start
-
-Use the DBAPI interface to query Trino:
-
-```python
-import aiotrino
-conn = aiotrino.dbapi.connect(
-    host='localhost',
-    port=8080,
-    user='the-user',
-    catalog='the-catalog',
-    schema='the-schema',
-)
-await cur = conn.cursor()
-await cur.execute('SELECT * FROM system.runtime.nodes')
-rows = await cur.fetchall()
-await conn.close()
-```
-Or with context manager 
-```python
-import aiotrino
-async with aiotrino.dbapi.connect(
-    host='localhost',
-    port=8080,
-    user='the-user',
-    catalog='the-catalog',
-    schema='the-schema',
-) as conn:
-    await cur = conn.cursor()
-    await cur.execute('SELECT * FROM system.runtime.nodes')
-    rows = await cur.fetchall()
-```
-
-This will query the `system.runtime.nodes` system tables that shows the nodes
-in the Trino cluster.
-
-The DBAPI implementation in `aiotrino.dbapi` provides methods to retrieve fewer
-rows for example `Cursorfetchone()` or `Cursor.fetchmany()`. By default
-`Cursor.fetchmany()` fetches one row. Please set
-`trino.dbapi.Cursor.arraysize` accordingly.
-
-For backwards compatibility with PrestoSQL, override the headers at the start of your application
-```python
-import aiotrino
-aiotrino.constants.HEADERS = aiotrino.constants.PrestoHeaders
-```
-
-# Basic Authentication
-The `BasicAuthentication` class can be used to connect to a LDAP-configured Trino
-cluster:
-```python
-import aiotrino
-conn = aiotrino.dbapi.connect(
-    host='coordinator url',
-    port=8443,
-    user='the-user',
-    catalog='the-catalog',
-    schema='the-schema',
-    http_scheme='https',
-    auth=aiotrino.auth.BasicAuthentication("principal id", "password"),
-)
-cur = await conn.cursor()
-await cur.execute('SELECT * FROM system.runtime.nodes')
-rows = await cur.fetchall()
-await conn.close()
-```
-
-# Transactions
-The client runs by default in *autocommit* mode. To enable transactions, set
-*isolation_level* to a value different than `IsolationLevel.AUTOCOMMIT`:
-
-```python
-import aiotrino
-from aiotrino import transaction
-async with aiotrino.dbapi.connect(
-    host='localhost',
-    port=8080,
-    user='the-user',
-    catalog='the-catalog',
-    schema='the-schema',
-    isolation_level=transaction.IsolationLevel.REPEATABLE_READ,
-) as conn:
-  cur = await conn.cursor()
-  await cur.execute('INSERT INTO sometable VALUES (1, 2, 3)')
-  await cur.fetchone()
-  await cur.execute('INSERT INTO sometable VALUES (4, 5, 6)')
-  await cur.fetchone()
-```
-
-The transaction is created when the first SQL statement is executed.
-`trino.dbapi.Connection.commit()` will be automatically called when the code
-exits the *with* context and the queries succeed, otherwise
-`trino.dbapi.Connection.rollback()' will be called.
-
-# Development
-
-## Getting Started With Development
-
-Start by forking the repository and then modify the code in your fork.
-
-Clone the repository and go inside the code directory. Then you can get the
-version with `./setup.py --version`.
-
-We recommend that you use `virtualenv` for development:
-
-```
-$ virtualenv .venv
-$ . .venv/bin/activate
-# TODO add requirements.txt: pip install -r requirements.txt
-$ pip install .
-```
-
-For development purpose, pip can reference the code you are modifying in a
-*virtualenv*:
-
-```
-$ pip install -e .[tests]
-```
-
-That way, you do not need to run `pip install` again to make your changes
-applied to the *virtualenv*.
-
-When the code is ready, submit a Pull Request.
-
-## Code Style
-
-- For Python code, adhere to PEP 8.
-- Prefer code that is readable over one that is "clever".
-- When writing a Git commit message, follow these [guidelines](https://chris.beams.io/posts/git-commit/).
-
-## Running Tests
-
-There is a helper scripts, `run`, that provides commands to run tests.
-Type `./run tests` to run both unit and integration tests.
-
-`trino-python-client` uses [pytest](https://pytest.org/) for its tests. To run
-only unit tests, type:
-
-```
-$ pytest tests
-```
-
-Then you can pass options like `--pdb` or anything supported by `pytest --help`.
-
-To run the tests with different versions of Python in managed *virtualenvs*,
-use `tox` (see the configuration in `tox.ini`):
-
-```
-$ tox
-```
-
-To run integration tests:
-
-```
-$ pytest integration_tests
-```
-
-They pull a Docker image and then run a container with a Trino server:
-- the image is named `trinodb/trino:${TRINO_VERSION}`
-- the container is named `trino-python-client-tests-{uuid4()[:7]}`
-
-## Releasing
-
-- [Set up your development environment](#Getting-Started-With-Development).
-- Change version in `trino/__init__.py`.
-- Commit and create an annotated tag (`git tag -m '' current_version`)
-- Run the following:
-  ```bash
-  . .venv/bin/activate &&
-  pip install twine &&
-  rm -rf dist/ &&
-  ./setup.py sdist bdist_wheel &&
-  twine upload dist/* &&
-  open https://pypi.org/project/trino/ &&
-  echo "Released!"
-  ```
-- Push the branch and the tag (`git push upstream master current_version`)
-- Send release announcement.
-
-# Need Help?
-
-Feel free to create an issue as it make your request visible to other users and contributors.
-
-If an interactive discussion would be better or if you just want to hangout and chat about
-the Trino Python client, you can join us on the *#python-client* channel on
-[Trino Slack](https://trino.io/slack.html).
-
-
+Metadata-Version: 2.1
+Name: aiotrino
+Version: 0.2.1
+Summary: ASyncIO Client for the Trino distributed SQL Engine
+Home-page: https://github.com/mvanderlee/aiotrino/tree/main
+Author: Michiel Van Der Lee, Trino Team
+Author-email: jmt.vanderlee@gmail.com
+License: Apache 2.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Database :: Front-Ends
+Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: kerberos
+Provides-Extra: tests
+License-File: LICENSE
+
+[![Build Status](https://github.com/mvanderlee/trino-python-client/workflows/ci/badge.svg)](https://github.com/mvanderlee/trino-python-client/actions?query=workflow%3Aci+event%3Apush+branch%3Apy3-async)
+[![Trino Slack](https://img.shields.io/static/v1?logo=slack&logoColor=959DA5&label=Slack&labelColor=333a41&message=join%20conversation&color=3AC358)](https://trino.io/slack.html)
+[![Presto: The Definitive Guide book download](https://img.shields.io/badge/Presto%3A%20The%20Definitive%20Guide-download-brightgreen)](https://www.starburstdata.com/oreilly-presto-guide-download/)
+
+# Introduction
+
+This package provides a asyncio client interface to query [Trino](https://trino.io/)
+a distributed SQL engine. It supports Python 3.7, 3.8, 3.9, 3.10, 3.11.
+# Installation
+
+```
+$ pip install aiotrino
+```
+
+# Quick Start
+
+Use the DBAPI interface to query Trino:
+
+```python
+import aiotrino
+conn = aiotrino.dbapi.connect(
+    host='localhost',
+    port=8080,
+    user='the-user',
+    catalog='the-catalog',
+    schema='the-schema',
+)
+await cur = conn.cursor()
+await cur.execute('SELECT * FROM system.runtime.nodes')
+rows = await cur.fetchall()
+await conn.close()
+```
+Or with context manager 
+```python
+import aiotrino
+async with aiotrino.dbapi.connect(
+    host='localhost',
+    port=8080,
+    user='the-user',
+    catalog='the-catalog',
+    schema='the-schema',
+) as conn:
+    await cur = conn.cursor()
+    await cur.execute('SELECT * FROM system.runtime.nodes')
+    rows = await cur.fetchall()
+```
+
+This will query the `system.runtime.nodes` system tables that shows the nodes
+in the Trino cluster.
+
+The DBAPI implementation in `aiotrino.dbapi` provides methods to retrieve fewer
+rows for example `Cursorfetchone()` or `Cursor.fetchmany()`. By default
+`Cursor.fetchmany()` fetches one row. Please set
+`trino.dbapi.Cursor.arraysize` accordingly.
+
+For backwards compatibility with PrestoSQL, override the headers at the start of your application
+```python
+import aiotrino
+aiotrino.constants.HEADERS = aiotrino.constants.PrestoHeaders
+```
+
+# Basic Authentication
+The `BasicAuthentication` class can be used to connect to a LDAP-configured Trino
+cluster:
+```python
+import aiotrino
+conn = aiotrino.dbapi.connect(
+    host='coordinator url',
+    port=8443,
+    user='the-user',
+    catalog='the-catalog',
+    schema='the-schema',
+    http_scheme='https',
+    auth=aiotrino.auth.BasicAuthentication("principal id", "password"),
+)
+cur = await conn.cursor()
+await cur.execute('SELECT * FROM system.runtime.nodes')
+rows = await cur.fetchall()
+await conn.close()
+```
+
+# JWT Token Authentication
+The `JWTAuthentication` class can be used to connect to a configured Trino cluster:
+```python
+import aiotrino
+conn = aiotrino.dbapi.connect(
+    host='coordinator url',
+    port=8443,
+    catalog='the-catalog',
+    schema='the-schema',
+    http_scheme='https',
+    auth=aiotrino.auth.JWTAuthentication(token="jwt-token"),
+)
+cur = await conn.cursor()
+await cur.execute('SELECT * FROM system.runtime.nodes')
+rows = await cur.fetchall()
+await conn.close()
+```
+
+# Transactions
+The client runs by default in *autocommit* mode. To enable transactions, set
+*isolation_level* to a value different than `IsolationLevel.AUTOCOMMIT`:
+
+```python
+import aiotrino
+from aiotrino import transaction
+async with aiotrino.dbapi.connect(
+    host='localhost',
+    port=8080,
+    user='the-user',
+    catalog='the-catalog',
+    schema='the-schema',
+    isolation_level=transaction.IsolationLevel.REPEATABLE_READ,
+) as conn:
+  cur = await conn.cursor()
+  await cur.execute('INSERT INTO sometable VALUES (1, 2, 3)')
+  await cur.fetchone()
+  await cur.execute('INSERT INTO sometable VALUES (4, 5, 6)')
+  await cur.fetchone()
+```
+
+The transaction is created when the first SQL statement is executed.
+`trino.dbapi.Connection.commit()` will be automatically called when the code
+exits the *with* context and the queries succeed, otherwise
+`trino.dbapi.Connection.rollback()' will be called.
+
+# Development
+
+## Getting Started With Development
+
+Start by forking the repository and then modify the code in your fork.
+
+Clone the repository and go inside the code directory. Then you can get the
+version with `./setup.py --version`.
+
+We recommend that you use `virtualenv` for development:
+
+```
+$ virtualenv .venv
+$ . .venv/bin/activate
+# TODO add requirements.txt: pip install -r requirements.txt
+$ pip install .
+```
+
+For development purpose, pip can reference the code you are modifying in a
+*virtualenv*:
+
+```
+$ pip install -e .[tests]
+```
+
+That way, you do not need to run `pip install` again to make your changes
+applied to the *virtualenv*.
+
+When the code is ready, submit a Pull Request.
+
+## Code Style
+
+- For Python code, adhere to PEP 8.
+- Prefer code that is readable over one that is "clever".
+- When writing a Git commit message, follow these [guidelines](https://chris.beams.io/posts/git-commit/).
+
+## Running Tests
+
+There is a helper scripts, `run`, that provides commands to run tests.
+Type `./run tests` to run both unit and integration tests.
+
+`trino-python-client` uses [pytest](https://pytest.org/) for its tests. To run
+only unit tests, type:
+
+```
+$ pytest tests
+```
+
+Then you can pass options like `--pdb` or anything supported by `pytest --help`.
+
+To run the tests with different versions of Python in managed *virtualenvs*,
+use `tox` (see the configuration in `tox.ini`):
+
+```
+$ tox
+```
+
+To run integration tests:
+
+```
+$ pytest integration_tests
+```
+
+They pull a Docker image and then run a container with a Trino server:
+- the image is named `trinodb/trino:${TRINO_VERSION}`
+- the container is named `trino-python-client-tests-{uuid4()[:7]}`
+
+
+### Test setup
+
+Supported OS Ubuntu 22.04
+
+1. Install [pyenv](https://github.com/pyenv/pyenv#automatic-installer)
+
+    ```shell
+    curl https://pyenv.run | bash
+    ```
+
+2. Install required python versions
+
+    ```shell
+    # Install the latest of all supported versions
+    pyenv install 3.7, 3.8, 3.9, 3.10, 3.11
+    ```
+
+3. Set the installed versions as default for the shell. This allows `tox` to find them.
+
+    List installed versions and update the following command as needed.
+    ```shell
+    pyenv versions
+    ```
+
+    ```shell
+    pyenv shell 3.11.3 3.10.11 3.9.16 3.8.16 3.7.16
+    ```
+
+4. Install `tox`
+
+    ```shell
+    pip install tox
+    ```
+
+5. Run `tox`
+
+    ```shell
+    tox
+    ```
+
+## Releasing
+
+- [Set up your development environment](#Getting-Started-With-Development).
+- Change version in `trino/__init__.py`.
+- Commit and create an annotated tag (`git tag -m '' current_version`)
+- Run the following:
+  ```bash
+  . .venv/bin/activate &&
+  pip install twine wheel &&
+  rm -rf dist/ &&
+  ./setup.py sdist bdist_wheel &&
+  twine upload dist/* &&
+  open https://pypi.org/project/trino/ &&
+  echo "Released!"
+  ```
+- Push the branch and the tag (`git push upstream master current_version`)
+- Send release announcement.
+
+# Need Help?
+
+Feel free to create an issue as it make your request visible to other users and contributors.
+
+If an interactive discussion would be better or if you just want to hangout and chat about
+the Trino Python client, you can join us on the *#python-client* channel on
+[Trino Slack](https://trino.io/slack.html).
```

### Comparing `aiotrino-0.1.1/setup.py` & `aiotrino-0.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 tests_require = all_require + ["pytest", "pytest-aiohttp", "pytest-asyncio", "pytest-runner", "aioresponses", "click", "mock", "pytz"]
 
 setup(
     name="aiotrino",
     author="Michiel Van Der Lee, Trino Team",
     author_email="jmt.vanderlee@gmail.com",
     version=version,
-    url="https://github.com/mvanderlee/trino-python-client/tree/py3-async",
+    url="https://github.com/mvanderlee/aiotrino/tree/main",
     packages=["aiotrino"],
     package_data={"": ["LICENSE", "README.md"]},
     description="ASyncIO Client for the Trino distributed SQL Engine",
     long_description=README,
     long_description_content_type="text/markdown",
     license="Apache 2.0",
     classifiers=[
@@ -52,17 +52,19 @@
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Database :: Front-Ends",
     ],
     install_requires=["aiohttp"],
     extras_require={
         "all": all_require,
```

