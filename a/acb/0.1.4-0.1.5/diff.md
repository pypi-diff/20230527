# Comparing `tmp/acb-0.1.4.tar.gz` & `tmp/acb-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acb-0.1.4.tar", last modified: Wed Apr 26 17:25:41 2023, max compression
+gzip compressed data, was "acb-0.1.5.tar", last modified: Sat May 27 21:19:36 2023, max compression
```

## Comparing `acb-0.1.4.tar` & `acb-0.1.5.tar`

### file list

```diff
@@ -1,45 +1,30 @@
--rw-r--r--   0        0        0      694 2023-04-26 10:42:56.638728 acb-0.1.4/README.md
--rw-r--r--   0        0        0      126 2023-04-26 02:25:22.898091 acb-0.1.4/acb/__init__.py
--rw-r--r--   0        0        0      124 2023-04-22 16:43:07.429717 acb-0.1.4/acb/actions/__init__.py
--rw-r--r--   0        0        0    12869 2023-04-26 10:43:29.503944 acb-0.1.4/acb/actions/backup.py
--rw-r--r--   0        0        0     2026 2023-04-26 17:21:57.123274 acb-0.1.4/acb/actions/debug.py
--rw-r--r--   0        0        0     2944 2023-04-26 10:43:25.703934 acb-0.1.4/acb/actions/encode.py
--rw-r--r--   0        0        0     1260 2023-04-26 16:49:42.039701 acb-0.1.4/acb/actions/hash.py
--rw-r--r--   0        0        0     5597 2023-04-26 10:43:30.248567 acb-0.1.4/acb/actions/mail.py
--rw-r--r--   0        0        0      158 2023-04-26 14:59:45.938340 acb-0.1.4/acb/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 01:47:22.926037 acb-0.1.4/acb/adapters/analytic/__init__.py
--rw-r--r--   0        0        0      841 2023-04-22 16:43:13.241412 acb-0.1.4/acb/adapters/analytic/google.py
--rw-r--r--   0        0        0        0 2023-04-26 10:42:56.660227 acb-0.1.4/acb/adapters/auth/__init__.py
--rw-r--r--   0        0        0     6739 2023-04-26 10:43:27.144404 acb-0.1.4/acb/adapters/auth/firebase.py
--rw-r--r--   0        0        0        0 2023-04-20 12:04:32.606819 acb-0.1.4/acb/adapters/cache/__init__.py
--rw-r--r--   0        0        0    11625 2023-04-26 10:43:33.424885 acb-0.1.4/acb/adapters/cache/redis.py
--rw-r--r--   0        0        0        0 2023-04-26 01:28:40.559756 acb-0.1.4/acb/adapters/database/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 01:48:03.525185 acb-0.1.4/acb/adapters/database/redis.py
--rw-r--r--   0        0        0     3737 2023-04-26 10:43:27.141502 acb-0.1.4/acb/adapters/database/sqlalchemy.py
--rw-r--r--   0        0        0     4258 2023-04-26 10:43:30.602745 acb-0.1.4/acb/adapters/dns/google.py
--rw-r--r--   0        0        0        0 2023-04-26 16:20:06.240641 acb-0.1.4/acb/adapters/logging/__init__.py
--rw-r--r--   0        0        0      705 2023-04-26 17:21:56.350830 acb-0.1.4/acb/adapters/logging/handlers.py
--rw-r--r--   0        0        0        0 2023-04-26 17:01:50.567413 acb-0.1.4/acb/adapters/logging/loggers/__init__.py
--rw-r--r--   0        0        0     1496 2023-04-26 17:21:54.266676 acb-0.1.4/acb/adapters/logging/loggers/loguru.py
--rw-r--r--   0        0        0        0 2023-04-26 17:02:04.985966 acb-0.1.4/acb/adapters/logging/loggers/picologger.py
--rw-r--r--   0        0        0      250 2023-04-26 17:21:23.313242 acb-0.1.4/acb/adapters/logging/loggers/sentry.py
--rw-r--r--   0        0        0        0 2023-04-26 01:36:40.098734 acb-0.1.4/acb/adapters/mail/__init__.py
--rw-r--r--   0        0        0     9958 2023-04-26 17:21:23.538631 acb-0.1.4/acb/adapters/mail/mailgun.py
--rw-r--r--   0        0        0     2437 2023-04-26 10:43:31.462644 acb-0.1.4/acb/adapters/recaptcha/google.py
--rw-r--r--   0        0        0        0 2023-04-26 01:43:28.269577 acb-0.1.4/acb/adapters/secret/__init__.py
--rw-r--r--   0        0        0     7171 2023-04-26 10:43:33.604151 acb-0.1.4/acb/adapters/secret/google.py
--rw-r--r--   0        0        0        0 2023-04-26 01:31:02.544210 acb-0.1.4/acb/adapters/storage/__init__.py
--rw-r--r--   0        0        0     4764 2023-04-26 17:21:23.441799 acb-0.1.4/acb/adapters/storage/google.py
--rw-r--r--   0        0        0     6392 2023-04-26 17:21:57.767534 acb-0.1.4/acb/adapters/storage/universal.py
--rw-r--r--   0        0        0      407 2023-04-26 02:25:26.622784 acb-0.1.4/acb/adapters/template/jinja/__init__.py
--rw-r--r--   0        0        0     1314 2023-04-26 10:43:25.386904 acb-0.1.4/acb/adapters/template/jinja/bccache.py
--rw-r--r--   0        0        0     5079 2023-04-16 01:42:22.123633 acb-0.1.4/acb/adapters/template/jinja/compiler.py
--rw-r--r--   0        0        0     1786 2023-04-26 10:43:29.925170 acb-0.1.4/acb/adapters/template/jinja/environment.py
--rw-r--r--   0        0        0    17799 2023-04-26 16:03:44.559195 acb-0.1.4/acb/adapters/template/jinja/loaders.py
--rw-r--r--   0        0        0      599 2023-04-26 17:21:22.076448 acb-0.1.4/acb/adapters/theme/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 17:09:08.379335 acb-0.1.4/acb/adapters/theme/bulma.py
--rw-r--r--   0        0        0        0 2023-04-26 17:09:24.644513 acb-0.1.4/acb/adapters/theme/tailwind.py
--rw-r--r--   0        0        0        0 2023-04-26 16:49:26.854107 acb-0.1.4/acb/config/__init__.py
--rw-r--r--   0        0        0     7457 2023-04-26 17:21:57.616592 acb-0.1.4/acb/config/settings.py
--rw-r--r--   0        0        0     1585 2023-04-26 17:25:41.010442 acb-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1923 1970-01-01 00:00:00.000000 acb-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1001 2023-05-27 13:27:12.641564 acb-0.1.5/README.md
+-rw-r--r--   0        0        0      140 2023-05-27 20:21:40.115629 acb-0.1.5/acb/__init__.py
+-rw-r--r--   0        0        0      124 2023-04-22 16:43:07.429717 acb-0.1.5/acb/actions/__init__.py
+-rw-r--r--   0        0        0     1387 2023-05-27 21:16:17.114056 acb-0.1.5/acb/actions/debug.py
+-rw-r--r--   0        0        0     3249 2023-05-27 21:05:57.372642 acb-0.1.5/acb/actions/encode.py
+-rw-r--r--   0        0        0      877 2023-05-07 15:46:56.099014 acb-0.1.5/acb/actions/hash.py
+-rw-r--r--   0        0        0       77 2023-05-26 17:34:58.552486 acb-0.1.5/acb/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:04:32.606819 acb-0.1.5/acb/adapters/cache/__init__.py
+-rw-r--r--   0        0        0     1571 2023-05-27 19:19:32.332620 acb-0.1.5/acb/adapters/cache/redis.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:28:40.559756 acb-0.1.5/acb/adapters/database/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-27 21:16:18.244974 acb-0.1.5/acb/adapters/database/redis_om.py
+-rw-r--r--   0        0        0    16459 2023-05-26 14:44:49.878690 acb-0.1.5/acb/adapters/database/sqlalchemy.py
+-rw-r--r--   0        0        0     1848 2023-05-27 13:27:44.420088 acb-0.1.5/acb/adapters/database/sqlmodel.py
+-rw-r--r--   0        0        0        0 2023-05-27 19:13:35.056779 acb-0.1.5/acb/adapters/debug/__init__.py
+-rw-r--r--   0        0        0      471 2023-05-27 21:16:52.557919 acb-0.1.5/acb/adapters/debug/sentry.py
+-rw-r--r--   0        0        0     4770 2023-05-27 21:01:37.006314 acb-0.1.5/acb/adapters/dns/cloud_dns.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:36:40.098734 acb-0.1.5/acb/adapters/mail/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 20:21:31.954823 acb-0.1.5/acb/adapters/mail/gmail.py
+-rw-r--r--   0        0        0     9799 2023-05-27 21:01:36.998525 acb-0.1.5/acb/adapters/mail/mailgun.py
+-rw-r--r--   0        0        0        0 2023-05-27 13:39:02.267034 acb-0.1.5/acb/adapters/requests/__init__.py
+-rw-r--r--   0        0        0      687 2023-05-27 21:16:18.575095 acb-0.1.5/acb/adapters/requests/httpx.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:43:28.269577 acb-0.1.5/acb/adapters/secret/__init__.py
+-rw-r--r--   0        0        0     7078 2023-05-27 13:27:14.023615 acb-0.1.5/acb/adapters/secret/google.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:31:02.544210 acb-0.1.5/acb/adapters/storage/__init__.py
+-rw-r--r--   0        0        0     4675 2023-04-29 15:06:51.116866 acb-0.1.5/acb/adapters/storage/google.py
+-rw-r--r--   0        0        0     6392 2023-04-26 17:21:57.767534 acb-0.1.5/acb/adapters/storage/universal.py
+-rw-r--r--   0        0        0     3836 2023-05-27 21:15:49.356733 acb-0.1.5/acb/config.py
+-rw-r--r--   0        0        0     3434 2023-05-27 21:16:13.327412 acb-0.1.5/acb/logger.py
+-rw-r--r--   0        0        0     1839 2023-05-27 21:19:36.544613 acb-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2567 1970-01-01 00:00:00.000000 acb-0.1.5/PKG-INFO
```

### Comparing `acb-0.1.4/README.md` & `acb-0.1.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,15 @@
-# Asynchronous Component Base
+<p align="center">
+<img src="https://drive.google.com/uc?id=1pMUqyvgMkhGYoLz3jBibZDl3J63HEcCC">
+</p>
+
+# <u>A</u>synchronous <u>C</u>omponent <u>B</u>ase
+
+[![Code style: crackerjack](https://img.shields.io/badge/code%20style-crackerjack-000042)](https://github.com/lesleslie/crackerjack)
+
 
 Asynchronous Component Base, or 'acb', is a collection of modular
 components (actions / adapters) that provide the building blocks for rapid,
 asynchronous, application development.
 This codebase should be considered alpha right now as it is under
 heavy development. A majority of the components though should be
 immediately usable as they are added.
@@ -39,7 +46,15 @@
 from acb.configure import (
     AppConfig,
     AppSettings,
 )
 ```
 
 ## Adapters
+
+
+## Acknowledgements
+
+
+## License
+
+BSD-3-Clause
```

### Comparing `acb-0.1.4/acb/actions/backup.py` & `acb-0.1.5/acb/adapters/database/sqlalchemy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,152 @@
-import asyncio
+import typing as t
 from calendar import isleap
 from calendar import monthrange
 from concurrent.futures import as_completed
 from concurrent.futures import ThreadPoolExecutor
+from contextlib import asynccontextmanager
 from contextlib import suppress
 from datetime import date
 from datetime import datetime
 from datetime import timedelta
+from functools import lru_cache
 from itertools import chain
 from pathlib import Path
 from re import search
 from typing import Any
 
-# from actions.load import load
-from adapters.database import async_session
+# from sqlalchemy.orm.exc import UnmappedInstanceError
+from storage import stor
+
+import arrow
 
 # from re import sub
 # from adapters.database_ import async_session
-from adapters.database import db_engine
-from config import ac
-from config import debug
-from models import AppModelBase
-from resize import clear_resized_images
+from acb.adapters.database.sqlmodel import AppBaseModel
+from acb import ac
+from acb import AppSettings
+from acb import logger
+from acb.actions.debug import apformat
+from aioconsole import ainput
+from aioconsole import aprint
+
+# from plugins import plugin_source
+from pydantic import BaseModel
+from sqlalchemy import inspect
+from sqlalchemy import text
+from sqlalchemy.engine import URL
+from sqlalchemy.ext.asyncio import create_async_engine
 
 # from sqlalchemy.exc import IntegrityError
 # from sqlalchemy.exc import InvalidRequestError
 from sqlalchemy.ext.serializer import dumps as sdumps
 from sqlalchemy.ext.serializer import loads as sloads
+from sqlalchemy.pool import NullPool
+from sqlalchemy_utils import create_database
+from sqlalchemy_utils import database_exists
+from sqlalchemy_utils import drop_database
 from sqlmodel import select
 from sqlmodel import SQLModel
+from sqlmodel.ext.asyncio.session import AsyncSession
 
-# from sqlalchemy.orm.exc import UnmappedInstanceError
-from storage import stor
 
-import arrow
+# from actions.load import load
+# from resize import clear_resized_images
 
-# from plugins import plugin_source
-from pydantic import BaseModel
 
-logger = asyncio.run(get_app_logger(__file__))(debug)
+class DatabaseSettings(AppSettings):
+    host: str = ac.secrets.database_host if ac.deployed else "127.0.0.1"
+    user: str = ac.secrets.database_user
+    port = 3306
+    async_url: t.Optional[URL]
+    url: t.Optional[URL]
+    engine_kwargs = dict(poolclass=NullPool, pool_pre_ping=True)
+
+    def __init__(self, **data: t.Any) -> None:
+        super().__init__(**data)
+        self.async_url_kwargs = dict(
+            drivername="mysql+asyncmy",
+            username=ac.secrets.database_user,
+            password=ac.secrets.database_password,
+            port=self.port,
+            host=self.host,
+            database=ac.app.name,
+        )
+        self.async_url = URL.create(**self.async_url_kwargs)
+        self.url_kwargs = dict(drivername="mysql+mysqldb")
+        self.url = URL.create(**{**self.async_url_kwargs, **self.url_kwargs})
+
+
+class Database:
+    engine: t.Any = None
+    # session: t.Any = None
+
+    async def create(self, demo: bool = False) -> None:
+        exists = database_exists(ac.db.url)
+        if exists:
+            logger.debug("Database exists.")
+
+        if (
+            (ac.debug.database or ac.debug.models)
+            and not (ac.app.is_deployed or ac.debug.production)
+            and exists
+        ):
+            msg = (
+                "\n\nRESETTING THE DATABASE WILL CAUSE ALL OF YOUR"
+                " CURRENT DATA TO BE LOST!\n"
+            )
+            if demo:
+                msg = (
+                    "\nBy running this module,\n\nYOUR DATABASE WILL BE DELETED AND "
+                    "REPLACED WITH DEMO DATA.\nALL OF YOUR CURRENT DATA WILL BE LOST!\n"
+                )
+            await aprint(msg)
+            delete_db = await ainput("Would you like to reset the database? (Y/N) ")
+            if delete_db:
+                drop_database(ac.db.url)
+                logger.warning("Database dropped.")
+                exists = database_exists(ac.db.url)
+
+        if not exists:
+            create_database(ac.db.url)
+            logger.info("Database created.")
+
+    @lru_cache
+    async def get_async_session(self):
+        return AsyncSession(self.engine, expire_on_commit=False)
+
+    @asynccontextmanager
+    async def session(self) -> AsyncSession:
+        async with self.get_async_session() as sess:
+            yield sess
+
+    @staticmethod
+    def get_table_names(conn):
+        inspector = inspect(conn)
+        return inspector.get_table_names()
+
+    async def init(self, demo: bool = False) -> None:
+        self.engine = create_async_engine(ac.db.async_url, **ac.db.engine_kwargs)
+
+        # print(debug.database)
+        # print(type(debug.database))
+        await self.create(demo)
+        async with self.engine.connect() as conn:
+            if ac.debug.database:
+                sql = text("DROP TABLE IF EXISTS alembic_version")
+                await conn.execute(sql)
+            logger.info("Creating database tables...")
+            await conn.run_sync(SQLModel.metadata.create_all)
+            if ac.debug.models:
+                table_names = await conn.run_sync(self.get_table_names)
+                await apformat(table_names)
+            logger.info("Database initialized.")
+
+
+db = Database()
 
 sure_delete = False
 
 
 class BackupDbUtils(BaseModel):
     @staticmethod
     def get_timestamp(name: str):
@@ -87,15 +191,15 @@
         return self.backup_path
 
 
 class BackupDbDates(BaseModel):
     today = arrow.utcnow()
     white_list = []
     black_list = []
-    dates = list()
+    dates = []
 
     def __init__(self, dates=None, **data: Any) -> None:
         super().__init__(**data)
         self.dates = sorted(dates, reverse=True) if dates else []
         self.run()  # feed self.white_list & self.black_list
 
     def get_last_month_length(self):
@@ -109,21 +213,21 @@
     def filter_dates(self, dates, period):
         reference = self.today.int_timestamp
         method_mapping = {
             "week": lambda obj: getattr(obj, "isocalendar")()[1],
             "month": lambda obj: getattr(obj, "month"),
             "year": lambda obj: getattr(obj, "year"),
         }
-        for date in dates:
-            comp_date = datetime.fromtimestamp(int(date))
+        for dt in dates:
+            comp_date = datetime.fromtimestamp(int(dt))
             comparison = method_mapping.get(period)(comp_date)
             ref_date = datetime.fromtimestamp(int(reference))
             if comparison != method_mapping.get(period)(ref_date):
-                reference = date
-                yield date
+                reference = dt
+                yield dt
 
     def run(self) -> None:
         last_w = self.today.shift(days=-7).int_timestamp
         last_m = self.today.shift(days=-(self.get_last_month_length())).int_timestamp
         last_y = self.today.shift(days=-(self.get_last_year_length())).int_timestamp
         backups_week = []
         backups_month = []
@@ -154,44 +258,44 @@
     do_not_backup = list()
     models = list()
 
     def show(self):
         return [
             m
             for m in SQLModel.metadata.schema
-            if isinstance(m, type) and issubclass(m, AppModelBase)
+            if isinstance(m, type) and issubclass(m, AppBaseModel)
         ]
 
     def get_mapped_classes(self):
-        self.add_subclasses(AppModelBase)
+        self.add_subclasses(AppBaseModel)
         return self.models
 
     def add_subclasses(self, model) -> None:
         if model.__subclasses__():
             for submodel in model.__subclasses__():
                 self.add_subclasses(submodel)
         else:
             self.models.append(model)
 
     def get_data(self):
         data = dict()
-        async with async_session() as session:
+        async with db.session() as session:
             for model in self.get_mapped_classes():
                 query = select(model)
                 results = session.exec(query)
                 data[model.__name__] = sdumps(results)
         return data
 
     def parse_data(self, contents):
         with suppress(AttributeError):
             contents = sloads(
                 contents,
                 metadata=SQLModel.metadata,
-                engine=db_engine,
-                scoped_session=async_session(),
+                engine=db.engine,
+                scoped_session=db.session(),
             )
         return contents
 
     async def backup(self, class_name: str, data, now) -> None:
         path = self.get_path(class_name, now)
         await stor.db.save(data, path)
 
@@ -306,46 +410,43 @@
             logger.debug("==> No backup to be deleted.")
             return True
 
         logger.debug(f"==> {len(white_list)} backups will be kept:")
         for timestamp in white_list:
             date_formatted = arrow.Arrow.fromtimestamp(timestamp).humanize()
             logger.debug(f"ID: {timestamp} (from {date_formatted})")
-            if debug.database:
+            if ac.debug.database:
                 for f in self.by_timestamp(timestamp):
                     logger.debug(f)
 
         delete_list = list()
         logger.debug(f"==> {len(black_list)} backups will be deleted:")
         for timestamp in black_list:
             date_formatted = arrow.Arrow.fromtimestamp(timestamp).humanize()
             logger.debug(f"ID: {timestamp} (from {date_formatted})")
             for f in self.by_timestamp(timestamp):
-                if debug.database:
+                if ac.debug.database:
                     logger.debug(f)
                 delete_list.append(f)
 
         self.delete_backups(delete_list)
         return "cleandb"
 
     def run(self) -> None:
         if not ac.app.is_deployed:
             last_backup = self.get_last_backup()
-            if debug.database and sure_delete:
+            if ac.debug.database and sure_delete:
                 blobs = [b.name for b in stor.db.list()]
                 for b in blobs:
                     stor.db.delete(b)
-                clear_resized_images()
+                # clear_resized_images()
                 last_backup = None
             if not last_backup:
                 self.save()
-            elif last_backup and debug.database and not sure_delete:
+            elif last_backup and ac.debug.database and not sure_delete:
                 logger.info(f"Restoring last backup - {last_backup}")
                 self.restore_backup(last_backup)
             self.clean()
             logger.info("Backups complete.")
 
 
 backup_db = BackupDb()
-
-if __name__ == "__main__":
-    backup_db.run()
```

### Comparing `acb-0.1.4/acb/actions/encode.py` & `acb-0.1.5/acb/actions/encode.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import linecache
-import pickle
 import sys
 import tomllib
-from pathlib import Path
+from os import PathLike
 from re import search
+from warnings import warn
 
+import dill as pickle
 import msgspec
 import tomlkit
-from addict import Dict as adict
 from aiopath import AsyncPath
+from blake3 import blake3  # type: ignore
 from itsdangerous import Serializer as SecureSerializer
-from pathy import Path as PathyPath
 
 
 class AcbEncoder:
     def __init__(self) -> None:
-        self.serializers = adict(
+        self.serializers = dict(
             json=msgspec.json,
             yaml=msgspec.yaml,
             msgpack=msgspec.msgpack,
             pickle=pickle,
             toml=tomllib,
         )
         pickle.encode = pickle.dumps
@@ -27,58 +27,73 @@
         tomllib.encode = tomlkit.dumps
         tomllib.dumps = tomlkit.dumps
         tomllib.decode = tomllib.loads
         for s in self.serializers.keys():
             setattr(self, s, self.__call__)
 
     async def process(
-        self, obj, path, action, serializer, sort_keys, use_list, **kwargs
-    ) -> adict | bytes:
+        self,
+        obj: bytes | str | AsyncPath,
+        path: AsyncPath,
+        action,
+        serializer,
+        sort_keys,
+        use_list,
+        **kwargs,
+    ) -> int | bytes:
         if action in ("load", "decode"):
             if serializer is msgspec.msgpack:
                 kwargs.use_list = use_list
             if isinstance(obj, AsyncPath):
                 obj = await obj.read_text()
-            return adict(serializer.decode(obj, **kwargs))
+            return serializer.decode(obj, **kwargs)
         elif action in ("dump", "encode"):
             if serializer is msgspec.yaml:
                 kwargs.sort_keys = sort_keys
             data = serializer.encode(obj, **kwargs)
             if isinstance(path, AsyncPath):
                 return await path.write_text(data)
-            elif isinstance(path, PathyPath):
-                return path.write_text(data)
             return data
 
     def get_vars(self, frame):
         code_context = linecache.getline(frame.f_code.co_filename, frame.f_lineno)
         calling_method = search("await\s(\w+)\.(\w+)\(", code_context)
         return calling_method.group(1), self.serializers[calling_method.group(2)]
 
     def get_serializer(self, serializer, secret_key, secure_salt):
         secure = secret_key and secure_salt
         return (
-            SecureSerializer(secret_key, secure_salt, serializer=serializer)
+            SecureSerializer(
+                secret_key,
+                salt=secure_salt,
+                serializer=serializer,
+                signer_kwargs=dict(digest_method=blake3),
+            )
             if secure
             else serializer
         )
 
     async def __call__(
         self,
-        obj: str | Path | AsyncPath | Path | bytes | dict | adict = None,
-        path: AsyncPath | Path | PathyPath | str | None = None,
+        obj: str | PathLike | dict,
+        path: AsyncPath | str | None = None,
         sort_keys: bool = True,
         use_list: bool = False,
         secret_key: str = None,
         secure_salt: str = None,
         **kwargs,
-    ) -> adict | bytes:
-        obj = obj if not isinstance(obj, Path | AsyncPath) else AsyncPath(obj)
-        path = AsyncPath(path) if isinstance(path, Path | str) else path
+    ) -> dict | bytes:
+        # obj = obj if not isinstance(obj, AsyncPath) else AsyncPath(obj)
+        # path = AsyncPath(path) if isinstance(path, Path | str) else path
         action, serializer = self.get_vars(sys._getframe(1))
+        if (secret_key and not secure_salt) or (secure_salt and not secret_key):
+            warn(
+                f"{serializer} serializer won't sign objects unless both "
+                f"secret_key and secure_salt are set"
+            )
         serializer = self.get_serializer(serializer, secret_key, secure_salt)
         return await self.process(
             obj, path, action, serializer, sort_keys, use_list, **kwargs
         )
 
 
 dump = load = encode = decode = AcbEncoder()
```

### Comparing `acb-0.1.4/acb/actions/hash.py` & `acb-0.1.5/acb/actions/hash.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,30 @@
-from hashlib import blake2b
-from pathlib import Path
 from os import PathLike
 
 import arrow
 from aiopath import AsyncPath
-from google_crc32c import value
-from pydantic import BaseModel
+from blake3 import blake3 as hash_blake3
+from google_crc32c import value as hash_crc32c
 
 
-class Hash(BaseModel):
+class Hash:
     @staticmethod
-    async def blake2b(obj: PathLike | list | bytes | str) -> str:
-        hash_obj = blake2b(digest_size=20)
+    async def blake3(obj: PathLike | list | bytes | str) -> str:
         if not obj:
             timestamp = arrow.utcnow().float_timestamp
             obj = str(timestamp)
         elif isinstance(obj, PathLike):
-            obj = AsyncPath(obj) if isinstance(obj, Path) else obj
-            obj = await obj.read_bytes()
+            obj = await AsyncPath(obj).read_bytes()
         elif isinstance(obj, list):
             obj = "".join([str(a) for a in obj])
         if not isinstance(obj, bytes):
             obj = obj.encode()
-        hash_obj.update(obj)
-        return hash_obj.hexdigest()
+        return hash_blake3(obj).hexdigest()
 
     @staticmethod
-    def crc32c(obj: Path | bytes | str) -> bytes:
-        if isinstance(obj, Path):
-            obj = obj.read_text()
-        return value(obj.encode())
-
-    @staticmethod
-    async def acrc32c(obj: PathLike | bytes | str) -> bytes:
+    async def crc32c(obj: PathLike | bytes | str) -> bytes:
         if isinstance(obj, PathLike):
-            obj = AsyncPath(obj) if isinstance(obj, Path) else obj
-            obj = await obj.read_text()
-        return value(obj.encode())
+            obj = await AsyncPath(obj).read_text()
+        return hash_crc32c(obj.encode())
 
 
 hash = Hash()
```

### Comparing `acb-0.1.4/acb/adapters/dns/google.py` & `acb-0.1.5/acb/adapters/dns/cloud_dns.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,130 +1,132 @@
 from contextlib import suppress
 from time import sleep
-from typing import List
 from warnings import catch_warnings
 from warnings import filterwarnings
 
-from config import *
-from validators import domain
-from validators import ValidationFailure
-
+from acb import ac
+from acb.logger import apformat
 from google.api_core.exceptions import BadRequest
 from google.api_core.exceptions import Conflict
 from google.cloud.dns import Client as DnsClient
+from pydantic import BaseModel
+from validators import domain
+from validators import ValidationFailure
 
 with catch_warnings():
     filterwarnings("ignore", category=Warning)
     dns_client = DnsClient(project=ac.project)
 
 dns_zone = dns_client.zone(ac.app_name, f"{ac.raw_domain}.")
 splashstand_zone = dns_client.zone("sstand", "splashstand.com.")
 
 
-@dataclass
-class DnsRecord:
+class DnsRecord(BaseModel):
     name: str = ac.mail_domain
     type: str = "TXT"
     ttl: int = 300
-    rrdata: str = ""
+    rrdata: str | list = ""
 
 
-def create_dns_zone() -> None:
-    if not dns_zone.exists():
-        print(f"Creating gdns zone '{ac.app_name}...")
-        dns_zone.create()
-        print(f"Zone '{dns_zone.name}' successfully created.")
-    else:
-        print(f"Zone for '{dns_zone.name}' exists.")
-
-
-def list_dns_records(zone: DnsClient.zone = dns_zone):
-    records = zone.list_resource_record_sets()
-    records = [
-        DnsRecord(
-            name=record.name,
-            type=record.record_type,
-            ttl=record.ttl,
-            rrdata=record.rrdatas,
-        )
-        for record in records
-    ]
-    if debug.dns or debug.mail:
-        pprint(records)
-    return records
-
-
-def create_dns_records(
-    records: Union[List, DnsRecord], zone: DnsClient.zone = dns_zone
-):
-    if type(records) == DnsRecord:
-        records = [records]
-    changes = zone.changes()
-    current_record_sets = []
-    new_record_sets = []
-    for record in records:
-        if not record.name.endswith("."):
-            record.name = f"{record.name}."
-        record.rrdata = (
-            [record.rrdata] if type(record.rrdata) != list else record.rrdata
-        )
-        for i, r in enumerate(record.rrdata):
-            with suppress(ValidationFailure):
-                if type(r) == str and domain(r) and not r.endswith("."):
-                    r = f"{r}."
-                    record.rrdata[i] = r
-                if record.type == "TXT":
-                    record.rrdata[i] = f'"{r}"'
-        current_record = [
-            r
-            for r in list_dns_records()
-            if r.name == record.name and r.type == record.type
+class GoogleDNS:
+    @staticmethod
+    def create_dns_zone() -> None:
+        if not dns_zone.exists():
+            print(f"Creating gdns zone '{ac.app_name}...")
+            dns_zone.create()
+            print(f"Zone '{dns_zone.name}' successfully created.")
+        else:
+            print(f"Zone for '{dns_zone.name}' exists.")
+
+    async def list_dns_records(zone: DnsClient.zone = dns_zone):
+        records = zone.list_resource_record_sets()
+        records = [
+            DnsRecord(
+                name=record.name,
+                type=record.record_type,
+                ttl=record.ttl,
+                rrdata=record.rrdatas,
+            )
+            for record in records
         ]
-        if len(current_record) == 1:
-            # print(current_record[0])
-            current_record = current_record[0]
-            if current_record.__dict__ == record.__dict__:
-                continue
-            current_record_set = zone.resource_record_set(
-                name=current_record.name,
-                record_type=current_record.type,
-                ttl=current_record.ttl,
-                rrdatas=current_record.rrdata,
+        if ac.debug.dns or ac.debug.mail:
+            await apformat(records)
+        return records
+
+    def create_dns_records(
+        self, records: list | DnsRecord, zone: DnsClient.zone = dns_zone
+    ):
+        if type(records) == DnsRecord:
+            records = [records]
+        changes = zone.changes()
+        current_record_sets = []
+        new_record_sets = []
+        for record in records:
+            if not record.name.endswith("."):
+                record.name = f"{record.name}."
+            record.rrdata = (
+                [record.rrdata] if type(record.rrdata) != list else record.rrdata
+            )
+            for i, r in enumerate(record.rrdata):
+                with suppress(ValidationFailure):
+                    if type(r) == str and domain(r) and not r.endswith("."):
+                        r = f"{r}."
+                        record.rrdata[i] = r
+                    if record.type == "TXT":
+                        record.rrdata[i] = f'"{r}"'
+            current_record = [
+                r
+                for r in await self.list_dns_records()
+                if r.name == record.name and r.type == record.type
+            ]
+            if len(current_record) == 1:
+                # print(current_record[0])
+                current_record = current_record[0]
+                if current_record.__dict__ == record.__dict__:
+                    continue
+                current_record_set = zone.resource_record_set(
+                    name=current_record.name,
+                    record_type=current_record.type,
+                    ttl=current_record.ttl,
+                    rrdatas=current_record.rrdata,
+                )
+                current_record_sets.append(current_record_set)
+                print(f"Deleting - {current_record}")
+            record_set = zone.resource_record_set(
+                name=record.name,
+                record_type=record.type,
+                ttl=record.ttl,
+                rrdatas=record.rrdata,
             )
-            current_record_sets.append(current_record_set)
-            print(f"Deleting - {current_record}")
-        record_set = zone.resource_record_set(
-            name=record.name,
-            record_type=record.type,
-            ttl=record.ttl,
-            rrdatas=record.rrdata,
-        )
-        new_record_sets.append(record_set)
-        print(f"Creating - {record}")
-    if len(current_record_sets):
-        for set in current_record_sets:
-            changes.delete_record_set(set)
-        changes.create()  # API request
-        print("Deleting record sets", end="")
-        while changes.status != "done":
-            print(".", end="")
-            sleep(5)
-            changes.reload()  # API request
-        print("")
-    changes = zone.changes()
-    if len(new_record_sets):
-        for set in new_record_sets:
-            changes.add_record_set(set)
-        try:
+            new_record_sets.append(record_set)
+            print(f"Creating - {record}")
+        if len(current_record_sets):
+            for set in current_record_sets:
+                changes.delete_record_set(set)
             changes.create()  # API request
-            print("Creating record sets", end="")
+            print("Deleting record sets", end="")
             while changes.status != "done":
                 print(".", end="")
                 sleep(5)
                 changes.reload()  # API request
             print("")
-        except (Conflict, BadRequest) as err:
-            if not changes.additions[0].name.split(".")[1] == "splashstand":
-                raise err
-            print("SplashStand development domain detected. No changes made.")
-    else:
-        print("No DNS changes detected.")
+        changes = zone.changes()
+        if len(new_record_sets):
+            for set in new_record_sets:
+                changes.add_record_set(set)
+            try:
+                changes.create()  # API request
+                print("Creating record sets", end="")
+                while changes.status != "done":
+                    print(".", end="")
+                    sleep(5)
+                    changes.reload()  # API request
+                print("")
+            except (Conflict, BadRequest) as err:
+                if not changes.additions[0].name.split(".")[1] == "splashstand":
+                    raise err
+                print("SplashStand development domain detected. No changes made.")
+        else:
+            print("No DNS changes detected.")
+
+
+gdns = GoogleDNS()
```

### Comparing `acb-0.1.4/acb/adapters/mail/mailgun.py` & `acb-0.1.5/acb/adapters/mail/mailgun.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+import typing as t
 from asyncio import gather
-from pathlib import Path
 from pprint import pformat
 from pprint import pprint
 from re import search
-from typing import Any
-from loguru import logger
-
-from acb.actions.encode import load
-from acb.adapters.dns.google import create_dns_records
-from acb.adapters.dns.google import DnsRecord
-from acb.config.settings import AppSettings
 
+from acb import ac
+from acb import AppSettings
+from acb.actions import load
+from acb.adapters.dns.cloud_dns import DnsRecord
+from acb.adapters.dns.cloud_dns import gdns
+from acb.config import inspect_
+from aiopath import AsyncPath
 from httpx import AsyncClient
+from loguru import logger
 from pydantic import BaseModel
 
 
 class MailSettings(AppSettings):
     # MAIL_USERNAME: str
     # MAIL_PASSWORD: str
     # MAIL_PORT: int = 465
@@ -26,86 +27,83 @@
     # MAIL_FROM: EmailStr
     # MAIL_FROM_NAME: Optional[str] = None
     # TEMPLATE_FOLDER: Optional[DirectoryAsyncPath] = None
     # SUPPRESS_SEND: conint(gt=-1, lt=2) = 0  # type: ignore
     # USE_CREDENTIALS: bool = True
     # VALIDATE_CERTS: bool = True
 
-    debug = debug.mail
+    enabled = (not ac.app.mail_provider == "gmail",)
+    debug = ac.debug.mail
     domain = f"mail@{ac.app.domain}"
     server = "smpt.mailgun.com"
     port = "587"
     username = f"postmaster@{ac.app.domain}"
     password = ac.secrets.app_mail_password
+    api_url = ("https://api.mailgun.net/v3/domains",)
+    api_key = (ac.secrets.mailgun_api_key,)
     default_from = f"info@{ac.app.domain}"
     default_from_name = ac.app.title
     test_receiver = "email@splashstand.org"
     tls = True
     ssl = False
-    template_folder: Optional[AsyncPath]
-    gmail = adict(
+    template_folder: t.Optional[AsyncPath]
+    gmail = dict(
         enabled=ac.app.mail_provider == "gmail",
         mx_servers=[
             "1 aspmx.l.google.com.",
             "5 alt1.aspmx.l.google.com.",
             "5 alt2.aspmx.l.google.com.",
             "10 alt3.aspmx.l.google.com.",
             "10 alt4.aspmx.l.google.com.",
         ],
     )
-    mailgun = adict(
-        enabled=not ac.app.mail_provider == "gmail",
-        server="smtp.mailgun.org",
-        api_url="https://api.mailgun.net/v3/domains",
-        api_key=ac.secrets.mailgun_api_key,
-    )
 
 
 class Mailgun(BaseModel):
-    def __init__(self, **data: Any) -> None:
+    def __init__(self, **data: t.Any) -> None:
         super().__init__(**data)
 
     # conf = ConnectionConfig(
     #     MAIL_SERVER="smtp.ac.mail.mailgun.org",
     #     MAIL_PORT=587,
     #     MAIL_USERNAME=f"postmaster@{app.domain}",
     #     MAIL_PASSWORD=secrets.app_mail_password,
     #     MAIL_FROM="info@{app.domain}",
     #     MAIL_TLS=True,
     #     MAIL_SSL=False,
     #     TEMPLATE_FOLDER=theme.path / "utility" / "mail",
     # )
 
-    def get_response(self, req_type: str, domain=None, data=None, params=None) -> None:
-        pass
-
-    #     caller = inspect_.calling_function()
-    #     match caller:
-    #         case search(caller, "domain"):
-    #             caller = "domain"
-    #         case search(caller, "route"):
-    #             caller = "route"
-    #     url = "/".join([ac.mailgun.api_url, caller, domain])
-    #     data = dict(auth=("api", ac.mailgun.api_key), params=params, data=data)
-    #     resp = None
-    #     async with AsyncClient() as client:
-    #         match req_type:
-    #             case "get":
-    #                 resp = await client.get(url)
-    #             case "put":
-    #                 url = "".join([url, "/connection"])
-    #                 resp = await client.put(url, data=data)
-    #             case "post":
-    #                 url = "".join([url, "/connection"])
-    #                 resp = await client.post(url, data=data)
-    #             case "delete":
-    #                 resp = await client.delete(url)
-    #     if debug.mail:
-    #         print(resp)
-    #     return load.json(resp.json())
+    async def get_response(
+        self, req_type: str, domain=None, data=None, params=None
+    ) -> dict:
+        caller = inspect_.calling_function()
+        match caller:
+            case search(caller, "domain"):
+                caller = "domain"
+            case search(caller, "route"):
+                caller = "route"
+        url = "/".join([ac.mailgun.api_url, caller, domain])
+        data = dict(auth=("api", ac.mailgun.api_key), params=params, data=data)
+        resp = None
+        async with AsyncClient() as client:
+            match req_type:
+                case "get":
+                    resp = await client.get(url)
+                case "put":
+                    url = "".join([url, "/connection"])
+                    resp = await client.put(url, data=data)
+                case "post":
+                    url = "".join([url, "/connection"])
+                    resp = await client.post(url, data=data)
+                case "delete":
+                    resp = await client.delete(url)
+        if ac.debug.mail:
+            print(resp)
+        return load.json(resp.json())
 
     async def list_domains(self):
         resp = await self.get_response("get", params={"skip": 0, "limit": 1000})
         domains = [d["name"] for d in resp["items"]]
         return domains
 
     async def get_domain(self, domain):
@@ -116,15 +114,15 @@
             "post",
             data={
                 "name": domain,
                 "smtp_password": ac.mail.password,
                 "web_scheme": "https",
             },
         )
-        if debug.mail:
+        if ac.debug.mail:
             logger.debug(resp)
         resp = await self.get_response(
             "put", data={"require_tls": True, "skip_verification": True}
         )
         return resp
 
     async def delete_domain(self, domain):
@@ -166,24 +164,24 @@
         if ac.mail.mailgun.gmail.enabled:
             await self.delete_domain(ac.mail.mailgun.domain)
             rrdata = ac.mail.gmail.mx_servers
             record = DnsRecord(name=ac.mail.mailgun.domain, type="MX", rrdata=rrdata)
             records.append(record)
         else:
             await self.delete_domain(ac.mail.mailgun.domain)
-        if debug.mail:
+        if ac.debug.mail:
             pprint(records)
-        await create_dns_records(records)
+        await gdns.create_dns_records(records)
 
     async def list_routes(self):
         resp = await self.get_response("get", params={"skip": 0, "limit": 1000})
         domain_routes = [
             r for r in resp["items"] if ac.mail.mailgun.domain in r["expression"]
         ]
-        if debug.mail:
+        if ac.debug.mail:
             logger.debug(pformat(resp["items"]))
             logger.debug(len(resp["items"]))
             logger.debug(pformat(domain_routes))
             logger.debug(len(domain_routes))
 
         return domain_routes
 
@@ -195,43 +193,43 @@
 
     @staticmethod
     def get_name(address: str):
         name = search("'(.+)@.+", address)
         return name.group(1) if name else ""
 
     async def delete_routes(self, delete_all: bool = False) -> None:
-        forwards = await load.yaml(Path("mail.yml")).keys()
+        forwards = await load.yaml(AsyncPath("mail.yml")).keys()
         routes = await self.list_routes()
         deletes = []
         deletes.extend(
             [r for r in routes if self.get_name(r["expression"]) not in forwards]
         )
-        if debug.mail:
+        if ac.debug.mail:
             pprint(deletes)
         for f in forwards:
             fs = [r for r in routes if self.get_name(r["expression"]) == f]
             deletes.extend(fs[1:])
         if delete_all or ac.mail.mailgun.gmail.enabled:
             deletes = [r for r in routes if len(self.get_name(r["expression"]))]
-        if debug.mail:
+        if ac.debug.mail:
             pprint(deletes)
             print(len(deletes))
         else:
             for d in deletes:
                 await self.delete_route(d)
 
     async def create_route(self, domain_address, forwarding_addresses):
         domain_address = f"{domain_address}@{ac.mail.mailgun.domain}"
         if not isinstance(forwarding_addresses, list):
             forwarding_addresses = [forwarding_addresses]
         actions = ["stop(self)"]
 
         for addr in forwarding_addresses:
             actions.insert(0, f"forward('{addr}')")
-        if debug.mail:
+        if ac.debug.mail:
             print(actions)
         route = {
             "priority": 0,
             "description": domain_address,
             "expression": f"match_recipient('{domain_address}')",
             "action": actions,
         }
@@ -253,29 +251,29 @@
         resp = await self.get_response("post", data=route)
         logger.info(
             f"Created route for {domain_address}  ==> "
             f" {', '.join(forwarding_addresses)}"
         )
         return resp
 
-    async def create_routes(self, ordered: bool = True) -> None:
-        if ac.mail.mailgun.gmail.enabled:
-            logger.info("Using gmail mx servers. No routes created.")
-            return
-        else:
-            forwards = await load.yaml(Path("mail.yml"), ordered=ordered)
-            async for k, v in forwards.items():
-                await self.create_route(k, v)
-
-    def setup_mail(self) -> bool:
-        self.create_dns_records()
-        if not (Path("mail.yml").exists()):
-            logger.info("No mail routes to configre - mail.yml not found.")
-            return False
-        self.delete_routes(delete_all=False)
-        self.create_routes()
 
+async def create_routes(self, ordered: bool = True) -> None:
+    if ac.mail.mailgun.gmail.enabled:
+        logger.info("Using gmail mx servers. No routes created.")
+        return
+    else:
+        forwards = await load.yaml(AsyncPath("mail.yml"), ordered=ordered)
+        async for k, v in forwards.items():
+            await self.create_route(k, v)
+
+
+def setup_mail(self) -> bool:
+    self.create_dns_records()
+
+    if not (AsyncPath("mail.yml").exists()):
+        logger.info("No mail routes to configre - mail.yml not found.")
+        return False
+    self.delete_routes(delete_all=False)
+    self.create_routes()
 
-mailgun = Mailgun()
 
-# if __name__ == "__main__":
-#     ac.mail.mailgun.setup_mail()
+mailgun = Mailgun()
```

### Comparing `acb-0.1.4/acb/adapters/secret/google.py` & `acb-0.1.5/acb/adapters/secret/google.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 from contextlib import suppress
-from logging import getLogger
 from pathlib import Path
 from random import choice
 from secrets import compare_digest
 from secrets import token_bytes
 from secrets import token_urlsafe
 from string import ascii_letters
 from string import digits
 from string import punctuation
 from typing import Any
 from typing import Optional
 from warnings import catch_warnings
 from warnings import filterwarnings
 
-from addict import Dict as adict
+from acb.config import ac
+from acb.adapters.logging.loguru import logger
 from aiopath import AsyncPath
 from google.api_core.exceptions import AlreadyExists
 from google.auth import default
 from google.auth.transport.requests import AuthorizedSession
 from google.auth.transport.requests import Request
 from google.cloud.secretmanager import SecretManagerServiceClient
 from google.oauth2.credentials import Credentials
-from msgspec import yaml
 from pydantic import BaseSettings
 
 secret_dir = "tmp/secrets"
 deployed = False
 
-logger = getLogger()
 
-basedir = Path().cwd()
-
-settings = adict(yaml.decode((basedir / "settings" / "app.yml").read_bytes()))
-debug = adict(yaml.decode((basedir / "settings" / "debug.yml").read_bytes()))
+# settings = yaml.decode((basedir / "settings" / "app.yml").read_bytes())
+# debug = yaml.decode((basedir / "settings" / "debug.yml").read_bytes())
 
 
 def gen_password(size: int) -> str:
     chars = ascii_letters + digits + punctuation
-    return "".join(choice(chars) for i in range(size))
+    return "".join(choice(chars) for _ in range(size))
 
 
 class AppSecrets(BaseSettings):
     database_host: Optional[str]
     database_user: Optional[str]
     database_password: Optional[str]
     database_connection: Optional[str]
@@ -70,21 +66,21 @@
         extra = "forbid"
 
 
 class SecretManager:
     client: Optional[SecretManagerServiceClient]
     authed_session: Optional[AuthorizedSession]
     creds: Optional[Credentials]
-    target_audience: Optional[str]
-    projects: Optional[list]
-    project: Optional[str] = settings.project
-    domain: Optional[str] = settings.domain
-    prefix: Optional[str] = settings.name
-    parent: Optional[str] = f"projects/{settings.project}"
-    secret_dir: str = secret_dir
+    # target_audience: Optional[str]
+    # projects: Optional[list]
+    project: Optional[str] = ac.app.project
+    # domain: Optional[str] = settings.domain
+    prefix: Optional[str] = ac.app.name
+    parent: Optional[str] = f"projects/{ac.app.project}"
+    secret_dir: str = ac.tmp / "secrets"
 
     class Config:
         arbitrary_types_allowed = True
 
     @staticmethod
     def extract_secret_name(secret: str) -> str:
         return Path(secret).parts[-1]
@@ -95,30 +91,30 @@
             if name.startswith("app_")
             else f"000_{name}"
         )
         return name
 
     async def get_access_token(self) -> str:
         self.creds.refresh(Request())
-        if debug.secret_manager:
+        if ac.debug.secret_manager:
             logger.debug(f"Secrets access token:\n{self.creds.token}")
         return self.creds.token
 
     async def verify_access_token(self, token: str) -> bool:
         verified = compare_digest(self.creds.token, token)
-        if debug.secret_manager:
+        if ac.debug.secret_manager:
             logger.debug(f"Secrets access token verified - {verified}")
         return verified
 
     async def list(self):
         secrets = self.client.list_secrets(request={"parent": self.parent})
         secrets = [self.extract_secret_name(secret.name) for secret in secrets]
-        secrets = [s for s in secrets if s.split("_")[0] in [settings.name, "000"]]
+        secrets = [s for s in secrets if s.split("_")[0] in [ac.app.name, "000"]]
         # if not deployed and debug.secret_manager:
-        #     await pf(secrets)
+        #     await apformat(secrets)
         return secrets
 
     async def get(self, name: str) -> str:
         name = self.get_name(name)
         path = f"projects/{self.project}/secrets/{name}/versions/latest"
         version = self.client.access_secret_version(request={"name": path})
         payload = str(version.payload.data.decode())
@@ -136,72 +132,72 @@
                     "secret_id": name,
                     "secret": {"replication": {"automatic": {}}},
                 }
             )
             self.client.add_secret_version(
                 request={
                     "parent": version.name,
-                    "payload": {"data": bytes(str.encode(f"{value}"))},
+                    "payload": {"data": f"{value}".encode()},
                 }
             )
             if not deployed:
                 logger.debug(f"Created secret - {name}")
 
     async def update(self, name: str, value: str) -> None:
         name = self.get_name(name)
         secret = self.client.secret_path(self.project, name)
         self.client.add_secret_version(
             request={
                 "parent": secret,
-                "payload": {"data": bytes(str.encode(f"{value}"))},
+                "payload": {"data": f"{value}".encode()},
             }
         )
         if not deployed:
             logger.debug(f"Updated secret - {name}")
 
     async def delete(self, name: str) -> None:
         name = self.get_name(name)
         secret = self.client.secret_path(self.project, name)
         self.client.delete_secret(request={"name": secret})
         if not deployed:
             logger.debug(f"Deleted secret - {secret}")
 
-    async def load(self, name: str, secrets, cls_dict):
+    async def load(self, name: str, secrets, cls_dict) -> str:
         if name not in secrets:
             await self.create(name, cls_dict[name])
         secret = await self.get(name)
         return secret
 
     async def load_all(self, cls_dict):
         secrets = await self.list()
-        data = adict()
+        data = {}
         secret_dir = AsyncPath(self.secret_dir)
         await secret_dir.mkdir()
         for name in cls_dict.keys():
             secret = await self.load(name, secrets, cls_dict)
             data[name] = secret
             secret_path = secret_dir / name
             await secret_path.write_text(secret)
         return data
 
     async def init(self):
-        if not await AsyncPath(secret_manager.secret_dir).exists():
-            return await secret_manager.load_all(AppSecrets().dict())
+        if not await AsyncPath(self.secret_dir).exists():
+            return await self.load_all(AppSecrets().dict())
         else:
-            return AppSecrets(_secrets_dir=secret_manager.secret_dir)
+            return AppSecrets(_secrets_dir=self.secret_dir)
 
     def __init__(self) -> None:
         super().__init__()
         self.debug = None
-        self.target_audience = f"https://{self.domain}"
+        # self.target_audience = f"https://{self.domain}"
         with catch_warnings():
             filterwarnings("ignore", category=Warning)
             creds, projects = default()
         self.creds = creds
         self.projects = projects
         self.client = SecretManagerServiceClient(credentials=self.creds)
         self.authed_session = AuthorizedSession(self.creds)
-        if debug.secret:
+        if ac.debug.secret:
             Path(secret_dir).rmdir()
 
 
-secret_manager = SecretManager()
+# secret_manager = SecretManager()
```

### Comparing `acb-0.1.4/acb/adapters/storage/google.py` & `acb-0.1.5/acb/adapters/storage/google.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import typing as t
 from pathlib import Path
 
-from acb.actions.debug import ic
 from acb.actions.log import logger
 
+from acb.actions.debug import ic
+from acb.config import AppSettings
+
 # from aiologger import Logger
 from acb.config import tmp
-
-from acb.config import AppSettings
 from aiopath import AsyncPath
 from google.cloud.exceptions import NotFound
 from pathy import Pathy
 from pathy import set_client_params
 from pathy import use_fs_cache
 from pydantic import BaseModel
 from pydantic import BaseSettings
@@ -70,30 +70,32 @@
     pf: t.Any = None
 
     class Config:
         arbitrary_types_allowed = True
 
     def __init__(self, bucket: str, prefix: str = None, **data: t.Any) -> None:
         super().__init__(**data)
-        self.prefix = prefix if prefix else self.prefix
-        self.bucket = (
-            f"splashstand-{bucket}"
-            if bucket not in [ac.storage.bucket.media, ac.storage.bucket.upload]
-            else bucket
-        )
-        self.path = Pathy(f"gs://{self.bucket}/{self.prefix}/")
+
+    self.prefix = prefix if prefix else self.prefix
+    self.bucket = (
+        f"splashstand-{bucket}"
+        if bucket not in [ac.storage.bucket.media, ac.storage.bucket.upload]
+        else bucket
+    )
+    self.path = Pathy(f"gs://{self.bucket}/{self.prefix}/")
 
     def save(self, obj_path: AsyncPath, data: t.Any) -> None:
-        stor_path = self.get_path(obj_path)
-        logger.debug(f"Saving {stor_path}...")
-        if isinstance(data, bytes):
-            stor_path.write_bytes(data)
-        else:
-            stor_path.write_text(data)
-        logger.debug(f"Saved - {stor_path}")
+        self.get_path(obj_path)
+
+    logger.debug(f"Saving {stor_path}...")
+    if isinstance(data, bytes):
+        stor_path.write_bytes(data)
+    else:
+        stor_path.write_text(data)
+    logger.debug(f"Saved - {stor_path}")
 
     def get(self, obj_path: AsyncPath):
         stor_path = self.get_path(obj_path)
         logger.debug(f"Getting {stor_path}...")
         try:
             data = stor_path.read_text()
         except NotFound:
@@ -129,22 +131,23 @@
     settings = CloudStorageBucket("settings")
     plugins = CloudStorageBucket("plugins")
     migrations = CloudStorageBucket("migrations")
     theme = CloudStorageBucket("theme")
 
     async def init(self) -> None:
         set_client_params("gs", project=ac.app.project)
-        use_fs_cache(root=tmp / "storage")
 
-        for bucket in [
-            b for b in self.__dict__.values() if isinstance(b, CloudStorageBucket)
-        ]:
-            ic(type(bucket))
-            logger.debug(f"{bucket.__name__.title()} initialized.")
-        logger.info("Storage initialized.")
+    use_fs_cache(root=tmp / "storage")
+
+    for bucket in [
+        b for b in self.__dict__.values() if isinstance(b, CloudStorageBucket)
+    ]:
+        ic(type(bucket))
+        logger.debug(f"{bucket.__name__.title()} initialized.")
+    logger.info("Storage initialized.")
 
 
 stor = AppStorage()
 
 # return blob(f"{url_pre}/{url_path.name}").public_url
 # return f"https://storage.cloud.google.com/{stor.media.name}/{ac.app_name}/{path}"
```

### Comparing `acb-0.1.4/acb/adapters/storage/universal.py` & `acb-0.1.5/acb/adapters/storage/universal.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.4/pyproject.toml` & `acb-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=7.3.0",
     "icecream>=2.1.3",
     "pre-commit>=3.2.2",
-    "crackerjack>=0.1.6",
+    "crackerjack>=0.2.0",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py311"
 fix = true
 show-fixes = true
@@ -24,39 +24,45 @@
 
 [tool.black]
 target-version = [
     "py311",
 ]
 
 [tool.mypy]
-strict = true
+strict = false
 pretty = true
+ignore_missing_imports = false
+plugins = [
+    "pydantic.mypy",
+]
 
 [tool.refurb]
 enable_all = true
 
 [tool.pytype]
 inputs = [
     "package_name",
 ]
 
 [project]
 name = "acb"
-version = "0.1.4"
+version = "0.1.5"
 description = "Asynchronus Code Base"
 dependencies = [
     "pydantic>=1.10.7",
     "itsdangerous>=2.1.2",
     "msgspec>=0.14.1",
-    "addict>=2.4.0",
     "aiopath>=0.6.11",
     "arrow>=1.2.3",
     "google-crc32c>=1.5.0",
     "icecream>=2.1.3",
     "pathy>=0.10.1",
+    "dill>=0.3.6",
+    "blake3>=0.3.3",
+    "python-ulid>=1.1.0",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 
@@ -68,31 +74,37 @@
 Documentation = "https://github.com/lesleslie/acb"
 Repository = "https://github.com/lesleslie/acb"
 
 [project.optional-dependencies]
 cache = [
     "cashews[redis]>=6.0.2",
 ]
-auth = [
-    "firebase-admin>=6.1.0",
-]
 storage = [
     "google-cloud-storage>=2.8.0",
 ]
 secret = [
     "google-cloud-secret-manager>=2.16.1",
 ]
 dns = [
     "google-cloud-dns>=0.34.1",
-]
-template = [
-    "jinja2>=3.1.2",
+    "validators>=0.20.0",
 ]
 logging = [
     "loguru>=0.7.0",
 ]
+database = [
+    "sqlmodel>=0.0.8",
+    "sqlalchemy>=1.4.41",
+    "sqlalchemy-utils>=0.41.1",
+    "redis-om>=0.1.2",
+]
+requests = [
+    "httpx>=0.24.1",
+    "httpx-cache>=0.10.0",
+]
+mail = []
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `acb-0.1.4/PKG-INFO` & `acb-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,57 @@
 Metadata-Version: 2.1
 Name: acb
-Version: 0.1.4
+Version: 0.1.5
 Summary: Asynchronus Code Base
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/lesleslie/acb
 Project-URL: Documentation, https://github.com/lesleslie/acb
 Project-URL: Repository, https://github.com/lesleslie/acb
 Requires-Python: >=3.11
 Requires-Dist: pydantic>=1.10.7
 Requires-Dist: itsdangerous>=2.1.2
 Requires-Dist: msgspec>=0.14.1
-Requires-Dist: addict>=2.4.0
 Requires-Dist: aiopath>=0.6.11
 Requires-Dist: arrow>=1.2.3
 Requires-Dist: google-crc32c>=1.5.0
 Requires-Dist: icecream>=2.1.3
 Requires-Dist: pathy>=0.10.1
+Requires-Dist: dill>=0.3.6
+Requires-Dist: blake3>=0.3.3
+Requires-Dist: python-ulid>=1.1.0
 Requires-Dist: cashews[redis]>=6.0.2; extra == "cache"
-Requires-Dist: firebase-admin>=6.1.0; extra == "auth"
 Requires-Dist: google-cloud-storage>=2.8.0; extra == "storage"
 Requires-Dist: google-cloud-secret-manager>=2.16.1; extra == "secret"
 Requires-Dist: google-cloud-dns>=0.34.1; extra == "dns"
-Requires-Dist: jinja2>=3.1.2; extra == "template"
+Requires-Dist: validators>=0.20.0; extra == "dns"
 Requires-Dist: loguru>=0.7.0; extra == "logging"
+Requires-Dist: sqlmodel>=0.0.8; extra == "database"
+Requires-Dist: sqlalchemy>=1.4.41; extra == "database"
+Requires-Dist: sqlalchemy-utils>=0.41.1; extra == "database"
+Requires-Dist: redis-om>=0.1.2; extra == "database"
+Requires-Dist: httpx>=0.24.1; extra == "requests"
+Requires-Dist: httpx-cache>=0.10.0; extra == "requests"
 Provides-Extra: cache
-Provides-Extra: auth
 Provides-Extra: storage
 Provides-Extra: secret
 Provides-Extra: dns
-Provides-Extra: template
 Provides-Extra: logging
+Provides-Extra: database
+Provides-Extra: requests
 Description-Content-Type: text/markdown
 
-# Asynchronous Component Base
+<p align="center">
+<img src="https://drive.google.com/uc?id=1pMUqyvgMkhGYoLz3jBibZDl3J63HEcCC">
+</p>
+
+# <u>A</u>synchronous <u>C</u>omponent <u>B</u>ase
+
+[![Code style: crackerjack](https://img.shields.io/badge/code%20style-crackerjack-000042)](https://github.com/lesleslie/crackerjack)
+
 
 Asynchronous Component Base, or 'acb', is a collection of modular
 components (actions / adapters) that provide the building blocks for rapid,
 asynchronous, application development.
 This codebase should be considered alpha right now as it is under
 heavy development. A majority of the components though should be
 immediately usable as they are added.
@@ -74,7 +88,15 @@
 from acb.configure import (
     AppConfig,
     AppSettings,
 )
 ```
 
 ## Adapters
+
+
+## Acknowledgements
+
+
+## License
+
+BSD-3-Clause
```

