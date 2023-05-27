# Comparing `tmp/mesh_sandbox-0.1.9-py3-none-any.whl.zip` & `tmp/mesh_sandbox-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,63 +1,78 @@
-Zip file size: 63971 bytes, number of entries: 61
+Zip file size: 78304 bytes, number of entries: 76
 -rw-r--r--  2.0 unx       22 b- defN 80-Jan-01 00:00 mesh_sandbox/__init__.py
--rw-r--r--  2.0 unx     3927 b- defN 80-Jan-01 00:00 mesh_sandbox/api.py
--rw-r--r--  2.0 unx     3071 b- defN 80-Jan-01 00:00 mesh_sandbox/common/__init__.py
+-rw-r--r--  2.0 unx     3925 b- defN 80-Jan-01 00:00 mesh_sandbox/api.py
+-rw-r--r--  2.0 unx     3403 b- defN 80-Jan-01 00:00 mesh_sandbox/common/__init__.py
 -rw-r--r--  2.0 unx     6504 b- defN 80-Jan-01 00:00 mesh_sandbox/common/constants.py
 -rw-r--r--  2.0 unx     1481 b- defN 80-Jan-01 00:00 mesh_sandbox/common/exceptions.py
 -rw-r--r--  2.0 unx      551 b- defN 80-Jan-01 00:00 mesh_sandbox/common/fernet.py
 -rw-r--r--  2.0 unx      392 b- defN 80-Jan-01 00:00 mesh_sandbox/common/handler_helpers.py
--rw-r--r--  2.0 unx     6065 b- defN 80-Jan-01 00:00 mesh_sandbox/common/mex_headers.py
--rw-r--r--  2.0 unx     2186 b- defN 80-Jan-01 00:00 mesh_sandbox/conftest.py
--rw-r--r--  2.0 unx     3264 b- defN 80-Jan-01 00:00 mesh_sandbox/dependencies.py
+-rw-r--r--  2.0 unx    14664 b- defN 80-Jan-01 00:00 mesh_sandbox/common/messaging.py
+-rw-r--r--  2.0 unx     6088 b- defN 80-Jan-01 00:00 mesh_sandbox/common/mex_headers.py
+-rw-r--r--  2.0 unx     2233 b- defN 80-Jan-01 00:00 mesh_sandbox/conftest.py
+-rw-r--r--  2.0 unx     4089 b- defN 80-Jan-01 00:00 mesh_sandbox/dependencies.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mesh_sandbox/handlers/__init__.py
+-rw-r--r--  2.0 unx     3783 b- defN 80-Jan-01 00:00 mesh_sandbox/handlers/admin.py
 -rw-r--r--  2.0 unx      605 b- defN 80-Jan-01 00:00 mesh_sandbox/handlers/handshake.py
--rw-r--r--  2.0 unx    14597 b- defN 80-Jan-01 00:00 mesh_sandbox/handlers/inbox.py
--rw-r--r--  2.0 unx     1471 b- defN 80-Jan-01 00:00 mesh_sandbox/handlers/lookup.py
--rw-r--r--  2.0 unx     9428 b- defN 80-Jan-01 00:00 mesh_sandbox/handlers/outbox.py
--rw-r--r--  2.0 unx     1918 b- defN 80-Jan-01 00:00 mesh_sandbox/handlers/tracking.py
+-rw-r--r--  2.0 unx    15450 b- defN 80-Jan-01 00:00 mesh_sandbox/handlers/inbox.py
+-rw-r--r--  2.0 unx     1392 b- defN 80-Jan-01 00:00 mesh_sandbox/handlers/lookup.py
+-rw-r--r--  2.0 unx    10045 b- defN 80-Jan-01 00:00 mesh_sandbox/handlers/outbox.py
+-rw-r--r--  2.0 unx     2356 b- defN 80-Jan-01 00:00 mesh_sandbox/handlers/tracking.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mesh_sandbox/models/__init__.py
 -rw-r--r--  2.0 unx      993 b- defN 80-Jan-01 00:00 mesh_sandbox/models/mailbox.py
--rw-r--r--  2.0 unx     4875 b- defN 80-Jan-01 00:00 mesh_sandbox/models/message.py
+-rw-r--r--  2.0 unx     4926 b- defN 80-Jan-01 00:00 mesh_sandbox/models/message.py
 -rw-r--r--  2.0 unx      518 b- defN 80-Jan-01 00:00 mesh_sandbox/models/workflow.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mesh_sandbox/plugins/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mesh_sandbox/routers/__init__.py
+-rw-r--r--  2.0 unx     3852 b- defN 80-Jan-01 00:00 mesh_sandbox/routers/admin.py
 -rw-r--r--  2.0 unx     2693 b- defN 80-Jan-01 00:00 mesh_sandbox/routers/handshake.py
--rw-r--r--  2.0 unx     8573 b- defN 80-Jan-01 00:00 mesh_sandbox/routers/inbox.py
--rw-r--r--  2.0 unx     1490 b- defN 80-Jan-01 00:00 mesh_sandbox/routers/inbox_count.py
+-rw-r--r--  2.0 unx     8898 b- defN 80-Jan-01 00:00 mesh_sandbox/routers/inbox.py
+-rw-r--r--  2.0 unx     1521 b- defN 80-Jan-01 00:00 mesh_sandbox/routers/inbox_count.py
 -rw-r--r--  2.0 unx     2115 b- defN 80-Jan-01 00:00 mesh_sandbox/routers/lookup.py
--rw-r--r--  2.0 unx     4736 b- defN 80-Jan-01 00:00 mesh_sandbox/routers/outbox.py
+-rw-r--r--  2.0 unx     4956 b- defN 80-Jan-01 00:00 mesh_sandbox/routers/outbox.py
 -rw-r--r--  2.0 unx     1439 b- defN 80-Jan-01 00:00 mesh_sandbox/routers/request_logging.py
--rw-r--r--  2.0 unx     1238 b- defN 80-Jan-01 00:00 mesh_sandbox/routers/simple.py
 -rw-r--r--  2.0 unx     2210 b- defN 80-Jan-01 00:00 mesh_sandbox/routers/tracking.py
 -rw-r--r--  2.0 unx      409 b- defN 80-Jan-01 00:00 mesh_sandbox/routers/update.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mesh_sandbox/store/__init__.py
--rw-r--r--  2.0 unx     5428 b- defN 80-Jan-01 00:00 mesh_sandbox/store/base.py
--rw-r--r--  2.0 unx     6894 b- defN 80-Jan-01 00:00 mesh_sandbox/store/canned_store.py
--rw-r--r--  2.0 unx     2612 b- defN 80-Jan-01 00:00 mesh_sandbox/store/data/chunks.jsonl
--rw-r--r--  2.0 unx      434 b- defN 80-Jan-01 00:00 mesh_sandbox/store/data/mailboxes.jsonl
--rw-r--r--  2.0 unx     2333 b- defN 80-Jan-01 00:00 mesh_sandbox/store/data/messages.jsonl
+-rw-r--r--  2.0 unx     1983 b- defN 80-Jan-01 00:00 mesh_sandbox/store/base.py
+-rw-r--r--  2.0 unx     9862 b- defN 80-Jan-01 00:00 mesh_sandbox/store/canned_store.py
+-rw-r--r--  2.0 unx      662 b- defN 80-Jan-01 00:00 mesh_sandbox/store/data/mailboxes/X26ABC1/in/SIMPLE_MESSAGE/1
+-rw-r--r--  2.0 unx      714 b- defN 80-Jan-01 00:00 mesh_sandbox/store/data/mailboxes/X26ABC1/in/SIMPLE_MESSAGE.json
+-rw-r--r--  2.0 unx      662 b- defN 80-Jan-01 00:00 mesh_sandbox/store/data/mailboxes/X26ABC1/in/UNDELIVERED_MESSAGE/1
+-rw-r--r--  2.0 unx      796 b- defN 80-Jan-01 00:00 mesh_sandbox/store/data/mailboxes/X26ABC1/in/UNDELIVERED_MESSAGE.json
+-rw-r--r--  2.0 unx      218 b- defN 80-Jan-01 00:00 mesh_sandbox/store/data/mailboxes/X26ABC2/in/CHUNKED_MESSAGE_GZ/1
+-rw-r--r--  2.0 unx      221 b- defN 80-Jan-01 00:00 mesh_sandbox/store/data/mailboxes/X26ABC2/in/CHUNKED_MESSAGE_GZ/2
+-rw-r--r--  2.0 unx      817 b- defN 80-Jan-01 00:00 mesh_sandbox/store/data/mailboxes/X26ABC2/in/CHUNKED_MESSAGE_GZ.json
+-rw-r--r--  2.0 unx      432 b- defN 80-Jan-01 00:00 mesh_sandbox/store/data/mailboxes.jsonl
 -rw-r--r--  2.0 unx      292 b- defN 80-Jan-01 00:00 mesh_sandbox/store/data/workflows.jsonl
--rw-r--r--  2.0 unx     1487 b- defN 80-Jan-01 00:00 mesh_sandbox/store/file_store.py
--rw-r--r--  2.0 unx     2208 b- defN 80-Jan-01 00:00 mesh_sandbox/store/memory_store.py
--rw-r--r--  2.0 unx     3585 b- defN 80-Jan-01 00:00 mesh_sandbox/store/serialisation.py
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/__init__.py
--rw-r--r--  2.0 unx     1292 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/docker_tests.py
+-rw-r--r--  2.0 unx     2400 b- defN 80-Jan-01 00:00 mesh_sandbox/store/file_store.py
+-rw-r--r--  2.0 unx     1643 b- defN 80-Jan-01 00:00 mesh_sandbox/store/memory_store.py
+-rw-r--r--  2.0 unx     3615 b- defN 80-Jan-01 00:00 mesh_sandbox/store/serialisation.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mesh_sandbox/test_plugin/__init__.py
+-rw-r--r--  2.0 unx      967 b- defN 80-Jan-01 00:00 mesh_sandbox/test_plugin/example_plugin.py
+-rw-r--r--  2.0 unx       24 b- defN 80-Jan-01 00:00 mesh_sandbox/test_plugin/example_plugin.txt
+-rw-r--r--  2.0 unx      106 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/__init__.py
+-rw-r--r--  2.0 unx    14549 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/admin.py
+-rw-r--r--  2.0 unx     1584 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/docker_tests.py
 -rw-r--r--  2.0 unx      740 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/exceptions.py
 -rw-r--r--  2.0 unx     6259 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/handshake.py
--rw-r--r--  2.0 unx     7909 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/helpers.py
--rw-r--r--  2.0 unx     8480 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/inbox.py
--rw-r--r--  2.0 unx     6546 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/java_client_tests.py
+-rw-r--r--  2.0 unx     6885 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/helpers.py
+-rw-r--r--  2.0 unx    10412 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/inbox.py
+-rw-r--r--  2.0 unx     6547 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/java_client_tests.py
 -rw-r--r--  2.0 unx     2768 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/lookup.py
--rw-r--r--  2.0 unx     2072 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/mesh_client_tests.py
--rw-r--r--  2.0 unx    18798 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/outbox.py
--rw-r--r--  2.0 unx      640 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/serialisation.py
+-rw-r--r--  2.0 unx     3901 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/mesh_api_helpers.py
+-rw-r--r--  2.0 unx     3947 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/mesh_client_tests.py
+-rw-r--r--  2.0 unx     5006 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/messaging_tests.py
+-rw-r--r--  2.0 unx    20061 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/outbox.py
+-rw-r--r--  2.0 unx      663 b- defN 80-Jan-01 00:00 mesh_sandbox/tests/serialisation.py
 -rw-r--r--  2.0 unx     1237 b- defN 80-Jan-01 00:00 mesh_sandbox/views/__init__.py
+-rw-r--r--  2.0 unx     1315 b- defN 80-Jan-01 00:00 mesh_sandbox/views/admin.py
 -rw-r--r--  2.0 unx     3885 b- defN 80-Jan-01 00:00 mesh_sandbox/views/error.py
 -rw-r--r--  2.0 unx     5662 b- defN 80-Jan-01 00:00 mesh_sandbox/views/inbox.py
 -rw-r--r--  2.0 unx     2775 b- defN 80-Jan-01 00:00 mesh_sandbox/views/lookup.py
--rw-r--r--  2.0 unx     4883 b- defN 80-Jan-01 00:00 mesh_sandbox/views/outbox.py
--rw-r--r--  2.0 unx     8827 b- defN 80-Jan-01 00:00 mesh_sandbox/views/tracking.py
--rw-r--r--  2.0 unx     2240 b- defN 80-Jan-01 00:00 mesh_sandbox-0.1.9.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mesh_sandbox-0.1.9.dist-info/WHEEL
--rw-r--r--  2.0 unx     1051 b- defN 80-Jan-01 00:00 mesh_sandbox-0.1.9.dist-info/LICENSE
-?rw-r--r--  2.0 unx     5329 b- defN 16-Jan-01 00:00 mesh_sandbox-0.1.9.dist-info/RECORD
-61 files, 203525 bytes uncompressed, 55447 bytes compressed:  72.8%
+-rw-r--r--  2.0 unx     4932 b- defN 80-Jan-01 00:00 mesh_sandbox/views/outbox.py
+-rw-r--r--  2.0 unx     8918 b- defN 80-Jan-01 00:00 mesh_sandbox/views/tracking.py
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mesh_sandbox-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1051 b- defN 80-Jan-01 00:00 mesh_sandbox-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2432 b- defN 80-Jan-01 00:00 mesh_sandbox-1.0.1.dist-info/METADATA
+?rw-r--r--  2.0 unx     6901 b- defN 16-Jan-01 00:00 mesh_sandbox-1.0.1.dist-info/RECORD
+76 files, 259445 bytes uncompressed, 67186 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -15,26 +15,32 @@
 
 Filename: mesh_sandbox/common/fernet.py
 Comment: 
 
 Filename: mesh_sandbox/common/handler_helpers.py
 Comment: 
 
+Filename: mesh_sandbox/common/messaging.py
+Comment: 
+
 Filename: mesh_sandbox/common/mex_headers.py
 Comment: 
 
 Filename: mesh_sandbox/conftest.py
 Comment: 
 
 Filename: mesh_sandbox/dependencies.py
 Comment: 
 
 Filename: mesh_sandbox/handlers/__init__.py
 Comment: 
 
+Filename: mesh_sandbox/handlers/admin.py
+Comment: 
+
 Filename: mesh_sandbox/handlers/handshake.py
 Comment: 
 
 Filename: mesh_sandbox/handlers/inbox.py
 Comment: 
 
 Filename: mesh_sandbox/handlers/lookup.py
@@ -54,17 +60,23 @@
 
 Filename: mesh_sandbox/models/message.py
 Comment: 
 
 Filename: mesh_sandbox/models/workflow.py
 Comment: 
 
+Filename: mesh_sandbox/plugins/__init__.py
+Comment: 
+
 Filename: mesh_sandbox/routers/__init__.py
 Comment: 
 
+Filename: mesh_sandbox/routers/admin.py
+Comment: 
+
 Filename: mesh_sandbox/routers/handshake.py
 Comment: 
 
 Filename: mesh_sandbox/routers/inbox.py
 Comment: 
 
 Filename: mesh_sandbox/routers/inbox_count.py
@@ -75,17 +87,14 @@
 
 Filename: mesh_sandbox/routers/outbox.py
 Comment: 
 
 Filename: mesh_sandbox/routers/request_logging.py
 Comment: 
 
-Filename: mesh_sandbox/routers/simple.py
-Comment: 
-
 Filename: mesh_sandbox/routers/tracking.py
 Comment: 
 
 Filename: mesh_sandbox/routers/update.py
 Comment: 
 
 Filename: mesh_sandbox/store/__init__.py
@@ -93,38 +102,65 @@
 
 Filename: mesh_sandbox/store/base.py
 Comment: 
 
 Filename: mesh_sandbox/store/canned_store.py
 Comment: 
 
-Filename: mesh_sandbox/store/data/chunks.jsonl
+Filename: mesh_sandbox/store/data/mailboxes/X26ABC1/in/SIMPLE_MESSAGE/1
 Comment: 
 
-Filename: mesh_sandbox/store/data/mailboxes.jsonl
+Filename: mesh_sandbox/store/data/mailboxes/X26ABC1/in/SIMPLE_MESSAGE.json
+Comment: 
+
+Filename: mesh_sandbox/store/data/mailboxes/X26ABC1/in/UNDELIVERED_MESSAGE/1
+Comment: 
+
+Filename: mesh_sandbox/store/data/mailboxes/X26ABC1/in/UNDELIVERED_MESSAGE.json
+Comment: 
+
+Filename: mesh_sandbox/store/data/mailboxes/X26ABC2/in/CHUNKED_MESSAGE_GZ/1
+Comment: 
+
+Filename: mesh_sandbox/store/data/mailboxes/X26ABC2/in/CHUNKED_MESSAGE_GZ/2
 Comment: 
 
-Filename: mesh_sandbox/store/data/messages.jsonl
+Filename: mesh_sandbox/store/data/mailboxes/X26ABC2/in/CHUNKED_MESSAGE_GZ.json
+Comment: 
+
+Filename: mesh_sandbox/store/data/mailboxes.jsonl
 Comment: 
 
 Filename: mesh_sandbox/store/data/workflows.jsonl
 Comment: 
 
 Filename: mesh_sandbox/store/file_store.py
 Comment: 
 
 Filename: mesh_sandbox/store/memory_store.py
 Comment: 
 
 Filename: mesh_sandbox/store/serialisation.py
 Comment: 
 
+Filename: mesh_sandbox/test_plugin/__init__.py
+Comment: 
+
+Filename: mesh_sandbox/test_plugin/example_plugin.py
+Comment: 
+
+Filename: mesh_sandbox/test_plugin/example_plugin.txt
+Comment: 
+
 Filename: mesh_sandbox/tests/__init__.py
 Comment: 
 
+Filename: mesh_sandbox/tests/admin.py
+Comment: 
+
 Filename: mesh_sandbox/tests/docker_tests.py
 Comment: 
 
 Filename: mesh_sandbox/tests/exceptions.py
 Comment: 
 
 Filename: mesh_sandbox/tests/handshake.py
@@ -138,26 +174,35 @@
 
 Filename: mesh_sandbox/tests/java_client_tests.py
 Comment: 
 
 Filename: mesh_sandbox/tests/lookup.py
 Comment: 
 
+Filename: mesh_sandbox/tests/mesh_api_helpers.py
+Comment: 
+
 Filename: mesh_sandbox/tests/mesh_client_tests.py
 Comment: 
 
+Filename: mesh_sandbox/tests/messaging_tests.py
+Comment: 
+
 Filename: mesh_sandbox/tests/outbox.py
 Comment: 
 
 Filename: mesh_sandbox/tests/serialisation.py
 Comment: 
 
 Filename: mesh_sandbox/views/__init__.py
 Comment: 
 
+Filename: mesh_sandbox/views/admin.py
+Comment: 
+
 Filename: mesh_sandbox/views/error.py
 Comment: 
 
 Filename: mesh_sandbox/views/inbox.py
 Comment: 
 
 Filename: mesh_sandbox/views/lookup.py
@@ -165,20 +210,20 @@
 
 Filename: mesh_sandbox/views/outbox.py
 Comment: 
 
 Filename: mesh_sandbox/views/tracking.py
 Comment: 
 
-Filename: mesh_sandbox-0.1.9.dist-info/METADATA
+Filename: mesh_sandbox-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: mesh_sandbox-0.1.9.dist-info/WHEEL
+Filename: mesh_sandbox-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: mesh_sandbox-0.1.9.dist-info/LICENSE
+Filename: mesh_sandbox-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: mesh_sandbox-0.1.9.dist-info/RECORD
+Filename: mesh_sandbox-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mesh_sandbox/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.9"
+__version__ = "1.0.1"
```

## mesh_sandbox/api.py

```diff
@@ -3,20 +3,20 @@
 from fastapi import FastAPI, HTTPException, Request, status
 from fastapi.exceptions import RequestValidationError
 
 from .common import logger
 from .common.exceptions import MessagingException
 from .dependencies import get_env_config
 from .routers import (
+    admin,
     handshake,
     inbox,
     inbox_count,
     lookup,
     outbox,
-    simple,
     tracking,
     update,
 )
 from .views.error import get_error_response, get_validation_error_response
 
 app = FastAPI(
     title="MESH Sandbox",
@@ -68,15 +68,15 @@
 
 
 @app.exception_handler(RequestValidationError)
 async def validation_exception_handler(request: Request, exc: RequestValidationError):
     return get_validation_error_response(request, exc)
 
 
-app.include_router(simple.router)
+app.include_router(admin.router)
 
 
 app.include_router(
     handshake.router,
     prefix="/messageexchange/{mailbox_id}",
     tags=["Handshake"],
     responses={
```

## mesh_sandbox/common/__init__.py

```diff
@@ -49,23 +49,27 @@
 class EnvConfig:
 
     env: str = field(default="local")
     build_label: str = field(default="latest")
     auth_mode: str = field(default="no_auth")
     store_mode: str = field(default="canned")
     shared_key: str = field(default="Banana")
-    file_store_dir: str = field(default="/tmp/mesh_store")
+    mailboxes_dir: str = field(default="/tmp/mesh_store")
+    message_expiry_days: int = field(default=30)
+    inbox_expiry_days: int = field(default=5)
 
     def __post_init__(self):
         self.env = os.environ.get("ENV", self.env)
         self.build_label = os.environ.get("BUILD_LABEL", self.build_label)
         self.auth_mode = os.environ.get("AUTH_MODE", self.auth_mode)
         self.store_mode = os.environ.get("STORE_MODE", self.store_mode)
         self.shared_key = os.environ.get("SHARED_KEY", self.shared_key)
-        self.file_store_dir = os.environ.get("FILE_STORE_DIR", self.file_store_dir)
+        self.mailboxes_dir = os.environ.get("MAILBOXES_DATA_DIR", os.environ.get("FILE_STORE_DIR", self.mailboxes_dir))
+        self.message_expiry_days = int(os.environ.get("MESSAGE_EXPIRY_DAYS", self.message_expiry_days))
+        self.inbox_expiry_days = int(os.environ.get("INBOX_EXPIRY_DAYS", self.inbox_expiry_days))
 
 
 T = TypeVar("T")
 
 
 def index_of(items: list[T], find: Callable[[T], bool]) -> int:
```

## mesh_sandbox/common/mex_headers.py

```diff
@@ -44,26 +44,26 @@
             return self
         updated = self._asdict()  # pylint: disable=no-member
         updated.update(kwargs)
         return MexHeaders(*[updated[f] for f in self._fields])  # pylint: disable=no-member
 
     @classmethod
     def from_message(cls, message: Message, chunk_range: Optional[str], **kwargs):
-        create: dict[str, Any] = dict(
-            mex_to=message.recipient.mailbox_id,
-            mex_workflow_id=message.workflow_id,
-            mex_chunk_range=chunk_range,
-            mex_subject=message.metadata.subject,
-            mex_localid=message.metadata.local_id,
-            mex_partnerid=message.metadata.partner_id,
-            mex_filename=message.metadata.file_name,
-            mex_content_encrypted=message.metadata.encrypted,
-            mex_content_compressed=message.metadata.is_compressed,
-            mex_content_checksum=message.metadata.checksum,
-        )
+        create: dict[str, Any] = {
+            "mex_to": message.recipient.mailbox_id,
+            "mex_workflow_id": message.workflow_id,
+            "mex_chunk_range": chunk_range,
+            "mex_subject": message.metadata.subject,
+            "mex_localid": message.metadata.local_id,
+            "mex_partnerid": message.metadata.partner_id,
+            "mex_filename": message.metadata.file_name,
+            "mex_content_encrypted": message.metadata.encrypted,
+            "mex_content_compressed": message.metadata.compressed,
+            "mex_content_checksum": message.metadata.checksum,
+        }
 
         if kwargs:
             create.update(kwargs)
         return MexHeaders(*[create[f] for f in cls._fields])  # pylint: disable=no-member
 
 
 def validate_content_checksum(content_checksum: Optional[str]):
```

## mesh_sandbox/conftest.py

```diff
@@ -7,23 +7,24 @@
 import httpx
 import pytest
 from fastapi import status
 from fastapi.testclient import TestClient
 from uvicorn import Config, Server  # type: ignore[import]
 
 from .api import app
-from .dependencies import get_env_config, get_store
+from .dependencies import get_env_config, get_messaging, get_store
 from .tests.helpers import temp_env_vars
 
 
 @pytest.fixture(scope="function", autouse=True)
 def setup():
 
     get_store.cache_clear()
     get_env_config.cache_clear()
+    get_messaging.cache_clear()
 
     with temp_env_vars(
         ENV="local",
         BUILD_LABEL="test",
         AUTH_MODE="full",
         STORE_MODE="memory",
         SHARED_KEY="TestKey",
```

## mesh_sandbox/dependencies.py

```diff
@@ -1,25 +1,27 @@
+import logging
 import re
 from functools import lru_cache
 from typing import Optional
 
 from fastapi import Depends, Header, HTTPException, Path, Query, Request
 
 from .common import EnvConfig
 from .common.constants import Headers
 from .common.fernet import FernetHelper
+from .common.messaging import Messaging
 from .store.base import Store
 from .store.canned_store import CannedStore
 from .store.file_store import FileStore
 from .store.memory_store import MemoryStore
 
 _ACCEPTABLE_ACCEPTS = re.compile(r"^application/vnd\.mesh\.v(\d+)\+json$")
 
 
-def parse_accept_header(accept: str) -> Optional[int]:
+def parse_accept_header(accept: Optional[str]) -> Optional[int]:
 
     if not accept:
         return 1
 
     for accepts in accept.split(";"):
         accepts = accepts.strip()
         if not accepts or "vnd.mesh" not in accepts:
@@ -82,36 +84,65 @@
         example="20210311101813838554_1B8F53",
         min_length=1,
     ),
 ):
     return message_id.upper()
 
 
+async def normalise_content_encoding(
+    content_encoding: str = Header(
+        title=Headers.Content_Encoding, description="content encoding", example="gzip", default=""
+    ),
+):
+    return (content_encoding or "").strip().lower()
+
+
+async def normalise_content_type(
+    content_type: str = Header(
+        title=Headers.Content_Type,
+        description="content type of the message when decoded",
+        example="text/csv",
+        default="",
+    ),
+):
+    return (content_type or "").strip().lower()
+
+
 @lru_cache()
 def get_env_config() -> EnvConfig:
     return EnvConfig()
 
 
 @lru_cache()
-def get_store() -> Store:
+def get_logger() -> logging.Logger:
+    return logging.getLogger("mesh-sandbox")
+
 
+@lru_cache()
+def get_store() -> Store:
+    logger = get_logger()
     config = get_env_config()
     if config.store_mode == "canned":
-        return CannedStore(config)
+        return CannedStore(config, logger)
 
     if config.store_mode == "memory":
-        return MemoryStore(config)
+        return MemoryStore(config, logger)
 
     if config.store_mode == "file":
-        return FileStore(config)
+        return FileStore(config, logger)
 
     raise ValueError(f"unrecognised store mode {config.store_mode}")
 
 
 @lru_cache()
+def get_messaging() -> Messaging:
+    return Messaging(store=get_store())
+
+
+@lru_cache()
 def get_fernet() -> FernetHelper:
     return FernetHelper()
 
 
 async def authorised_mailbox(
     request: Request,
     mailbox_id: str = Depends(normalise_mailbox_id_path),
@@ -120,11 +151,10 @@
         description="Authorisation header",
         example=(
             "authorization: NHSMESH TEST:2c001608-5f09-4840-9611-bea43e666a30:"
             "1:201511201038:3cded68a9e0f9b83f2c5de1b79fc4dac45004523e6658d46145156fa6a03eced"
         ),
         default="",
     ),
-    store: Store = Depends(get_store),
+    messaging: Messaging = Depends(get_messaging),
 ):
-
-    request.state.authorised_mailbox = await store.authorise_mailbox(mailbox_id, authorization)
+    request.state.authorised_mailbox = await messaging.authorise_mailbox(mailbox_id, authorization)
```

## mesh_sandbox/handlers/inbox.py

```diff
@@ -1,31 +1,25 @@
 import gzip
 from datetime import datetime, tzinfo
 from typing import Any, Callable, Optional, cast
 
 from dateutil.parser import isoparse
 from dateutil.relativedelta import relativedelta
 from dateutil.tz import tzutc
-from fastapi import Depends, HTTPException, Response, status
+from fastapi import BackgroundTasks, Depends, HTTPException, Response, status
 from starlette.responses import JSONResponse
 
-from ..common import (
-    MESH_MEDIA_TYPES,
-    EnvConfig,
-    constants,
-    exclude_none_json_encoder,
-    index_of,
-)
+from ..common import MESH_MEDIA_TYPES, constants, exclude_none_json_encoder, index_of
 from ..common.constants import Headers
 from ..common.fernet import FernetHelper
 from ..common.handler_helpers import get_handler_uri
-from ..dependencies import get_env_config, get_fernet, get_store
+from ..common.messaging import Messaging
+from ..dependencies import get_fernet, get_messaging
 from ..models.mailbox import Mailbox
 from ..models.message import Message, MessageDeliveryStatus, MessageStatus, MessageType
-from ..store.base import Store
 from ..views.inbox import InboxV1, InboxV2, get_rich_inbox_view
 
 HTTP_DATETIME_FORMAT = "%a, %d %b %Y %H:%M:%S %Z"
 DEFAULT_MAX_RESULTS = 500
 
 
 def to_http_datetime(maybe_naive_dt: datetime, as_timezone: Optional[tzinfo] = None) -> str:
@@ -35,20 +29,19 @@
     maybe_naive_dt = maybe_naive_dt.astimezone(tz=as_timezone)
     return maybe_naive_dt.strftime(HTTP_DATETIME_FORMAT)
 
 
 class InboxHandler:
     def __init__(
         self,
-        config: EnvConfig = Depends(get_env_config),
-        store: Store = Depends(get_store),
+        messaging: Messaging = Depends(get_messaging),
         fernet: FernetHelper = Depends(get_fernet),
     ):
-        self.config = config
-        self.store = store
+        self.messaging = messaging
+
         self.fernet = fernet
 
     @staticmethod
     def _get_status_headers(message: Message) -> dict[str, Optional[str]]:
 
         status_timestamp = (
             message.status_timestamp(MessageStatus.ACCEPTED, MessageStatus.ERROR) or datetime.utcnow()
@@ -95,30 +88,31 @@
             Headers.Mex_FileName: message.metadata.file_name or f"{message.message_id}.dat",
             Headers.Mex_Subject: message.metadata.subject,
             Headers.Mex_Version: "1.0",
             Headers.Mex_MessageType: message.message_type,
             Headers.Mex_MessageID: message.message_id,
             Headers.Content_Encoding: message.metadata.content_encoding,
             **InboxHandler._get_status_headers(message),
-            Headers.Mex_Content_Compressed: "Y" if message.metadata.is_compressed else None,
+            Headers.Mex_Content_Compressed: "Y" if message.metadata.compressed else None,
             Headers.Mex_Content_Encrypted: "Y" if message.metadata.encrypted else None,
+            Headers.Mex_Content_Checksum: message.metadata.checksum,
         }
 
         if message.message_type == MessageType.REPORT:
             headers.pop(Headers.Content_Encoding)
 
         if message.last_event and message.last_event.timestamp:
             headers[Headers.Last_Modified] = to_http_datetime(message.last_event.timestamp)
 
         # filter empty headers ( as per existing API )
         return {h: v for h, v in headers.items() if v}
 
     async def head_message(self, mailbox: Mailbox, message_id: str):
 
-        message = await self.store.get_message(message_id)
+        message = await self.messaging.get_message(message_id)
 
         if not message:
             raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=constants.ERROR_MESSAGE_DOES_NOT_EXIST)
 
         is_recipient_query = message.recipient.mailbox_id == mailbox.mailbox_id
         is_sender_query = message.sender and message.sender.mailbox_id == mailbox.mailbox_id
         allow_access = is_recipient_query or is_sender_query
@@ -132,28 +126,44 @@
 
         if message.status not in allowed_statuses:
             raise HTTPException(status_code=status.HTTP_410_GONE, detail=constants.ERROR_MESSAGE_GONE)
 
         headers = self._get_response_headers(message, 1)
         return Response(headers=headers)
 
-    async def retrieve_message(self, mailbox: Mailbox, message_id: str, accept_encoding: str):
+    async def retrieve_message(
+        self, mailbox: Mailbox, message_id: str, accept_encoding: str, accepts_api_version: int = 1
+    ):
         return await self._retrieve_message_or_chunk(
-            mailbox=mailbox, message_id=message_id, accept_encoding=accept_encoding
+            mailbox=mailbox,
+            message_id=message_id,
+            accept_encoding=accept_encoding,
+            accepts_api_version=accepts_api_version,
         )
 
-    async def retrieve_chunk(self, mailbox: Mailbox, message_id: str, accept_encoding: str, chunk_number: int):
+    async def retrieve_chunk(
+        self, mailbox: Mailbox, message_id: str, accept_encoding: str, chunk_number: int, accepts_api_version: int = 1
+    ):
         return await self._retrieve_message_or_chunk(
-            mailbox=mailbox, message_id=message_id, accept_encoding=accept_encoding, chunk_number=chunk_number
+            mailbox=mailbox,
+            message_id=message_id,
+            accept_encoding=accept_encoding,
+            chunk_number=chunk_number,
+            accepts_api_version=accepts_api_version,
         )
 
     async def _retrieve_message_or_chunk(
-        self, mailbox: Mailbox, message_id: str, accept_encoding: str, chunk_number: int = 1
+        self,
+        mailbox: Mailbox,
+        message_id: str,
+        accept_encoding: str,
+        chunk_number: int = 1,
+        accepts_api_version: int = 1,
     ):
-        message = await self.store.get_message(message_id)
+        message = await self.messaging.get_message(message_id)
 
         if not message:
             raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=constants.ERROR_MESSAGE_DOES_NOT_EXIST)
 
         if message.recipient.mailbox_id != mailbox.mailbox_id:
             raise HTTPException(status_code=status.HTTP_403_FORBIDDEN)
 
@@ -166,67 +176,79 @@
             return Response(headers=headers, content="")
 
         if chunk_number < 1 or chunk_number > message.total_chunks:
             raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=constants.ERROR_MESSAGE_DOES_NOT_EXIST)
 
         status_code = status.HTTP_200_OK if chunk_number >= message.total_chunks else status.HTTP_206_PARTIAL_CONTENT
 
-        chunk = await self.store.retrieve_chunk(message, chunk_number)
+        chunk = await self.messaging.get_chunk(message, chunk_number)
 
         if chunk is None:
             raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=constants.ERROR_MESSAGE_DOES_NOT_EXIST)
 
         headers[Headers.Content_Length] = str(len(chunk))
         content_encoding = headers.get(Headers.Content_Encoding, "")
         if content_encoding == "gzip" and "gzip" not in accept_encoding:
             headers.pop(Headers.Content_Encoding)
-            headers.pop(Headers.Content_Length)
             chunk = gzip.decompress(chunk)
 
+        if accepts_api_version > 1 and not content_encoding and "gzip" in accept_encoding:
+            headers[Headers.Content_Encoding] = "gzip"
+            chunk = gzip.compress(chunk)
+
+        headers[Headers.Content_Length] = str(len(chunk))
+
         if headers.get(Headers.Content_Encoding) == "gzip":
             headers[Headers.Mex_Content_Compressed] = "Y"
 
         return Response(
             status_code=status_code,
             content=chunk,
             headers=headers,
             media_type="application/octet-stream",
         )
 
-    async def acknowledge_message(self, mailbox: Mailbox, message_id: str, accepts_api_version: int = 1):
+    async def acknowledge_message(
+        self, background_tasks: BackgroundTasks, mailbox: Mailbox, message_id: str, accepts_api_version: int = 1
+    ):
 
-        message = await self.store.get_message(message_id)
+        message = await self.messaging.get_message(message_id)
         if not message:
             raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=constants.ERROR_MESSAGE_DOES_NOT_EXIST)
 
         if message.recipient.mailbox_id != mailbox.mailbox_id:
             raise HTTPException(status_code=status.HTTP_403_FORBIDDEN)
 
         def response():
             if accepts_api_version < 2:
                 # current format compatibility
-                return {"messageId": message.message_id}
+                return {"messageId": message.message_id}  # type: ignore[union-attr]
             return Response()
 
         if message.status != MessageStatus.ACCEPTED:
             return response()
 
-        await self.store.acknowledge_message(message)
+        await self.messaging.acknowledge_message(message=message, background_tasks=background_tasks)
 
         return response()
 
     async def _get_inbox_messages(
         self,
         mailbox: Mailbox,
         max_results: int = DEFAULT_MAX_RESULTS,
         last_key: Optional[dict] = None,
         message_filter: Optional[Callable[[Message], bool]] = None,
+        rich: bool = False,
     ) -> tuple[list[Message], Optional[dict]]:
 
-        messages = await self.store.get_inbox(mailbox.mailbox_id)
+        messages = (
+            await self.messaging.get_inbox_messages(mailbox.mailbox_id)
+            if rich
+            else await self.messaging.get_accepted_inbox_messages(mailbox.mailbox_id)
+        )
 
         if message_filter:
             messages = list(filter(message_filter, messages))
 
         if last_key:
             last_message_id = last_key["message_id"]
             ix = index_of(messages, lambda msg: bool(msg.message_id == last_message_id))
@@ -234,15 +256,15 @@
                 messages = messages[ix + 1 :]
 
         last_key = None
 
         if len(messages) > max_results:
             messages = messages[:max_results]
             if messages:
-                last_key = dict(message_id=messages[-1].message_id)
+                last_key = {"message_id": messages[-1].message_id}
 
         return messages, last_key
 
     @staticmethod
     def _get_workflow_filter(workflow_filter: Optional[str]) -> Optional[Callable[[Message], bool]]:
 
         workflow_id_filter = (workflow_filter or "").strip()
@@ -306,15 +328,15 @@
         workflow_filter: Optional[str] = None,
     ) -> Response:
 
         last_key: Optional[dict] = None
 
         if continue_from:
             if accepts_api_version < 2:
-                last_key = dict(message_id=continue_from)
+                last_key = {"message_id": continue_from}
             else:
                 last_key = self.fernet.decode_dict(continue_from)
 
         message_filter = self._get_workflow_filter(workflow_filter)
 
         messages, last_key = await self._get_inbox_messages(mailbox, max_results, last_key, message_filter)
 
@@ -327,19 +349,21 @@
         response = {"messages": [msg.message_id for msg in messages]}
 
         uri_query_args = {
             "max_results": max_results if max_results != DEFAULT_MAX_RESULTS else None,
             "workflow_filter": workflow_filter,
         }
 
-        links: dict[str, str] = dict(self=get_handler_uri([mailbox.mailbox_id], "{0}/inbox", **uri_query_args))
+        links: dict[str, str] = {"self": get_handler_uri([mailbox.mailbox_id], "{0}/inbox", **uri_query_args)}
 
-        result: dict[str, Any] = dict(
-            messages=cast(list[str], response.get("messages", [])), approx_inbox_count=mailbox.inbox_count, links=links
-        )
+        result: dict[str, Any] = {
+            "messages": cast(list[str], response.get("messages", [])),
+            "approx_inbox_count": mailbox.inbox_count,
+            "links": links,
+        }
 
         if last_key:
             uri_query_args["continue_from"] = self.fernet.encode_dict(last_key)
             links["next"] = get_handler_uri([mailbox.mailbox_id], "{0}/inbox", **uri_query_args)
 
         return JSONResponse(content=exclude_none_json_encoder(InboxV2(**result)), media_type=MESH_MEDIA_TYPES[2])
 
@@ -356,22 +380,22 @@
             last_key = self.fernet.decode_dict(continue_from)
 
         from_date = datetime.utcnow() + relativedelta(days=-30) if start_time is None else isoparse(start_time)
 
         def message_filter(message: Message) -> bool:
             return message.created_timestamp > from_date
 
-        messages, last_key = await self._get_inbox_messages(mailbox, max_results, last_key, message_filter)
+        messages, last_key = await self._get_inbox_messages(mailbox, max_results, last_key, message_filter, rich=True)
 
         url_template = "{0}/inbox/rich"
-        links: dict[str, str] = dict(
-            self=get_handler_uri(
+        links: dict[str, str] = {
+            "self": get_handler_uri(
                 [mailbox.mailbox_id], url_template=url_template, start_time=from_date, max_results=max_results
             )
-        )
+        }
         if last_key:
             links["next"] = get_handler_uri(
                 [mailbox.mailbox_id],
                 url_template=url_template,
                 start_time=from_date,
                 max_results=max_results,
                 continue_from=self.fernet.encode_dict(last_key),
```

## mesh_sandbox/handlers/lookup.py

```diff
@@ -1,33 +1,31 @@
 from fastapi import Depends, HTTPException, status
 
-from ..common import EnvConfig
-from ..dependencies import get_env_config, get_store
-from ..store.base import Store
+from ..common.messaging import Messaging
+from ..dependencies import get_messaging
 from ..views.lookup import endpoint_lookup_response, workflow_search_response
 
 
 class LookupHandler:
-    def __init__(self, config: EnvConfig = Depends(get_env_config), store: Store = Depends(get_store)):
-        self.config = config
-        self.store = store
+    def __init__(self, messaging: Messaging = Depends(get_messaging)):
+        self.messaging = messaging
 
     async def lookup_by_ods_code_and_workflow(self, ods_code: str, workflow_id: str, accepts_api_version: int = 1):
 
         if not ods_code or (ods_code and not ods_code.strip()):
             raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="ods code missing")
 
         if not workflow_id or (workflow_id and not workflow_id.strip()):
             raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="workflow id missing")
 
-        mailboxes = await self.store.lookup_by_ods_code_and_workflow_id(ods_code, workflow_id)
+        mailboxes = await self.messaging.lookup_by_ods_code_and_workflow_id(ods_code, workflow_id)
 
         return endpoint_lookup_response(mailboxes, accepts_api_version)
 
     async def lookup_by_workflow_id(self, workflow_id: str, accepts_api_version: int = 1):
 
         if not workflow_id or (workflow_id and not workflow_id.strip()):
             raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="workflow id missing")
 
-        mailboxes = await self.store.lookup_by_workflow_id(workflow_id)
+        mailboxes = await self.messaging.lookup_by_workflow_id(workflow_id)
 
         return workflow_search_response(mailboxes, accepts_api_version)
```

## mesh_sandbox/handlers/outbox.py

```diff
@@ -1,34 +1,34 @@
+import logging
 from datetime import datetime
 from typing import Optional, cast
 from uuid import uuid4
 
 from dateutil.parser import isoparse
 from dateutil.relativedelta import relativedelta
-from fastapi import Depends, HTTPException, Request
+from fastapi import BackgroundTasks, Depends, HTTPException, Request
 from fastapi import status as http_status
 from fastapi.responses import JSONResponse
 
-from ..common import EnvConfig, constants, index_of, strtobool
-from ..common.constants import Headers
+from ..common import constants, index_of, strtobool
 from ..common.exceptions import MessagingException
 from ..common.fernet import FernetHelper
 from ..common.handler_helpers import get_handler_uri
+from ..common.messaging import Messaging
 from ..common.mex_headers import MexHeaders
-from ..dependencies import get_env_config, get_fernet, get_store
+from ..dependencies import get_fernet, get_logger, get_messaging
 from ..models.mailbox import Mailbox
 from ..models.message import (
     Message,
     MessageEvent,
     MessageMetadata,
     MessageParty,
     MessageStatus,
     MessageType,
 )
-from ..store.base import Store
 from ..views.outbox import (
     get_rich_outbox_view,
     send_message_response,
     upload_chunk_response,
 )
 
 
@@ -56,28 +56,30 @@
     return None, chunk_no, total_chunks
 
 
 class OutboxHandler:
     # pylint: disable=too-many-arguments
     def __init__(
         self,
-        config: EnvConfig = Depends(get_env_config),
-        store: Store = Depends(get_store),
+        messaging: Messaging = Depends(get_messaging),
         fernet: FernetHelper = Depends(get_fernet),
+        logger: logging.Logger = Depends(get_logger),
     ):
-        self.config = config
-        self.store = store
+        self.messaging = messaging
         self.fernet = fernet
+        self.logger = logger
 
     async def send_message(
         self,
+        background_tasks: BackgroundTasks,
         request: Request,
         sender_mailbox: Mailbox,
         mex_headers: MexHeaders,
         content_encoding: str,
+        content_type: str,
         accepts_api_version: int = 1,
     ):  # pylint: disable=too-many-locals
 
         if not mex_headers.mex_to:
             raise HTTPException(status_code=http_status.HTTP_400_BAD_REQUEST, detail=constants.ERROR_MISSING_TO_ADDRESS)
 
         if content_encoding and content_encoding != "gzip":
@@ -88,15 +90,15 @@
         chunk_error, chunk_no, total_chunks = get_chunk_range(cast(str, mex_headers.mex_chunk_range), 1)
 
         if chunk_error or chunk_no > 1:
             raise HTTPException(
                 status_code=http_status.HTTP_417_EXPECTATION_FAILED, detail=constants.ERROR_INVALID_HEADER_CHUNKS
             )
 
-        recipient = await self.store.get_mailbox(mex_headers.mex_to)
+        recipient = await self.messaging.get_mailbox(mex_headers.mex_to)
         if not recipient:
             raise HTTPException(
                 status_code=http_status.HTTP_417_EXPECTATION_FAILED, detail=constants.ERROR_UNREGISTERED_RECIPIENT
             )
 
         status = MessageStatus.ACCEPTED if total_chunks < 2 else MessageStatus.UPLOADING
 
@@ -122,37 +124,44 @@
                 billing_entity=recipient.billing_entity,
             ),
             total_chunks=total_chunks,
             message_type=MessageType.DATA,
             workflow_id=mex_headers.mex_workflow_id,
             metadata=MessageMetadata(
                 subject=mex_headers.mex_subject,
-                content_encoding=request.headers.get(Headers.Content_Encoding, ""),
+                content_type=content_type,
+                content_encoding=content_encoding,
                 file_name=mex_headers.mex_filename or f"{message_id}.dat",
                 local_id=mex_headers.mex_localid,
                 partner_id=mex_headers.mex_partnerid,
                 checksum=mex_headers.mex_content_checksum,
                 encrypted=strtobool(mex_headers.mex_content_encrypted),
-                is_compressed=strtobool(mex_headers.mex_content_compressed),
+                compressed=strtobool(mex_headers.mex_content_compressed),
             ),
         )
 
         body = await request.body()
         if len(body) == 0:
             raise HTTPException(status_code=http_status.HTTP_417_EXPECTATION_FAILED, detail="MissingDataFile")
 
-        if message.status == MessageStatus.ACCEPTED:
-            message.file_size = len(body)
+        await self.messaging.send_message(message=message, body=body, background_tasks=background_tasks)
 
-        await self.store.send_message(message, body)
+        self.logger.info(
+            (
+                f"created message: message_id={message.message_id} "
+                f"from={message.sender.mailbox_id} to={message.recipient.mailbox_id} "
+                f"workflow={message.workflow_id or ''}"
+            )
+        )
 
         return send_message_response(message, accepts_api_version)
 
     async def send_chunk(  # pylint: disable=too-many-locals
         self,
+        background_tasks: BackgroundTasks,
         request: Request,
         sender_mailbox: Mailbox,
         message_id: str,
         chunk_number: int,
         mex_chunk_range: str,
         content_encoding: str,
         accepts_api_version: int = 1,
@@ -169,15 +178,15 @@
         error, _, _ = get_chunk_range(chunk_range, chunk_number)
         if error:
             raise MessagingException(
                 status_code=http_status.HTTP_417_EXPECTATION_FAILED,
                 detail=constants.ERROR_INVALID_HEADER_CHUNKS,
                 message_id=message_id,
             )
-        message: Optional[Message] = await self.store.get_message(message_id)
+        message: Optional[Message] = await self.messaging.get_message(message_id)
 
         if not message:
             raise HTTPException(status_code=http_status.HTTP_404_NOT_FOUND)
 
         if not sender_mailbox or sender_mailbox.mailbox_id != message.sender.mailbox_id:
             raise HTTPException(status_code=http_status.HTTP_403_FORBIDDEN)
 
@@ -190,20 +199,26 @@
         if (content_encoding or "").strip() != message.metadata.content_encoding:
             raise MessagingException(
                 status_code=http_status.HTTP_417_EXPECTATION_FAILED,
                 detail=constants.ERROR_CONTENT_ENCODING_CHANGED,
                 message_id=message_id,
             )
 
-        await self.store.receive_chunk(message, chunk_number, await request.body())
+        chunk = await request.body()
+
+        await self.messaging.save_chunk(
+            message=message, chunk_number=chunk_number, chunk=chunk, background_tasks=background_tasks
+        )
 
         if chunk_number < message.total_chunks:
             return upload_chunk_response(message, chunk_number, accepts_api_version)
 
-        await self.store.accept_message(message)
+        file_size = await self.messaging.get_file_size(message)
+
+        await self.messaging.accept_message(message=message, file_size=file_size, background_tasks=background_tasks)
 
         return upload_chunk_response(message, chunk_number, accepts_api_version)
 
     async def rich_outbox(
         self,
         mailbox: Mailbox,
         start_time: Optional[str],
@@ -213,15 +228,15 @@
         max_results = max(min(max_results, 100), 0)
         from_date = datetime.utcnow() + relativedelta(days=-30) if start_time is None else isoparse(start_time)
 
         last_key: Optional[dict] = None
         if continue_from:
             last_key = self.fernet.decode_dict(continue_from)
 
-        messages: list[Message] = cast(list[Message], await self.store.get_outbox(mailbox.mailbox_id))
+        messages: list[Message] = cast(list[Message], await self.messaging.get_outbox(mailbox.mailbox_id))
 
         def message_filter(message: Message) -> bool:
             return message.created_timestamp > from_date
 
         messages = list(filter(message_filter, messages))
 
         if last_key:
@@ -231,22 +246,22 @@
                 messages = messages[ix + 1 :]
 
         last_key = None
 
         if len(messages) > max_results:
             messages = messages[:max_results]
             if messages:
-                last_key = dict(message_id=messages[-1].message_id)
+                last_key = {"message_id": messages[-1].message_id}
 
         url_template = "{0}/outbox/rich"
-        links: dict[str, str] = dict(
-            self=get_handler_uri(
+        links: dict[str, str] = {
+            "self": get_handler_uri(
                 [mailbox.mailbox_id], url_template=url_template, start_time=from_date, max_results=max_results
             )
-        )
+        }
         if last_key:
             links["next"] = get_handler_uri(
                 [mailbox.mailbox_id],
                 url_template=url_template,
                 start_time=from_date,
                 max_results=max_results,
                 continue_from=self.fernet.encode_dict(last_key),
```

## mesh_sandbox/handlers/tracking.py

```diff
@@ -1,46 +1,54 @@
 from typing import Optional
 
 from fastapi import Depends, HTTPException
 from fastapi import status as http_status
 from starlette.responses import JSONResponse
 
-from ..common import MESH_MEDIA_TYPES, EnvConfig, exclude_none_json_encoder
-from ..dependencies import get_env_config, get_store
+from ..common import MESH_MEDIA_TYPES, exclude_none_json_encoder
+from ..common.messaging import Messaging
+from ..dependencies import get_messaging
 from ..models.mailbox import Mailbox
 from ..models.message import Message
-from ..store.base import Store
 from ..views.tracking import create_tracking_response
 
 
 class TrackingHandler:
-    def __init__(self, config: EnvConfig = Depends(get_env_config), store: Store = Depends(get_store)):
-        self.config = config
-        self.store = store
+    def __init__(self, messaging: Messaging = Depends(get_messaging)):
+        self.messaging = messaging
 
     async def tracking_by_message_id(self, sender_mailbox: Mailbox, message_id: str, accepts_api_version: int = 1):
 
-        message: Optional[Message] = await self.store.get_message(message_id)
+        message: Optional[Message] = await self.messaging.get_message(message_id)
 
         if not message:
             raise HTTPException(status_code=http_status.HTTP_404_NOT_FOUND)
 
         if sender_mailbox.mailbox_id != message.sender.mailbox_id or not sender_mailbox.mailbox_id:
             # intentionally not a 403 (matching spine)
             raise HTTPException(status_code=http_status.HTTP_404_NOT_FOUND)
 
+        sender_outbox = await self.messaging.get_outbox(sender_mailbox.mailbox_id)
+        if message.message_id not in [message.message_id for message in sender_outbox]:
+            raise HTTPException(status_code=http_status.HTTP_404_NOT_FOUND)
+
         model = create_tracking_response(message, accepts_api_version)
         return JSONResponse(content=exclude_none_json_encoder(model), media_type=MESH_MEDIA_TYPES[accepts_api_version])
 
     async def tracking_by_local_id(self, sender_mailbox: Mailbox, local_id: str):
 
-        messages: list[Message] = await self.store.get_by_local_id(sender_mailbox.mailbox_id, local_id)
+        messages: list[Message] = await self.messaging.get_by_local_id(sender_mailbox.mailbox_id, local_id)
 
         if len(messages) == 0:
             raise HTTPException(status_code=http_status.HTTP_404_NOT_FOUND)
 
         if len(messages) > 1:
             raise HTTPException(status_code=http_status.HTTP_300_MULTIPLE_CHOICES)
 
         message = messages[0]
+
+        sender_outbox = await self.messaging.get_outbox(sender_mailbox.mailbox_id)
+        if message.message_id not in [message.message_id for message in sender_outbox]:
+            raise HTTPException(status_code=http_status.HTTP_404_NOT_FOUND)
+
         model = create_tracking_response(message, 1)
         return JSONResponse(content=exclude_none_json_encoder(model))
```

## mesh_sandbox/models/message.py

```diff
@@ -29,21 +29,22 @@
     ERROR = "ERROR"
 
 
 @dataclass
 class MessageMetadata:
 
     subject: Optional[str] = field(default=None)
+    content_type: Optional[str] = field(default=None)
     content_encoding: Optional[str] = field(default=None)
     file_name: Optional[str] = field(default=None)
     local_id: Optional[str] = field(default=None)
     partner_id: Optional[str] = field(default=None)
     checksum: Optional[str] = field(default=None)
     encrypted: Optional[bool] = field(default=None)
-    is_compressed: Optional[bool] = field(default=None)
+    compressed: Optional[bool] = field(default=None)
     etag: Optional[str] = field(default=None)
     last_modified: Optional[str] = field(default=None)
 
 
 @dataclass
 class MessageParty:
     """This will be either a sender or a recipient."""
```

## mesh_sandbox/routers/inbox.py

```diff
@@ -1,10 +1,19 @@
 from typing import Optional, cast
 
-from fastapi import APIRouter, Depends, Header, Path, Query, Request, Response
+from fastapi import (
+    APIRouter,
+    BackgroundTasks,
+    Depends,
+    Header,
+    Path,
+    Query,
+    Request,
+    Response,
+)
 from starlette import status
 
 from ..common import MESH_MEDIA_TYPES
 from ..dependencies import (
     authorised_mailbox,
     get_accepts_api_version,
     normalise_message_id_path,
@@ -94,21 +103,22 @@
         status.HTTP_200_OK: {"content": None},
         status.HTTP_403_FORBIDDEN: {"description": "Authentication failed", "content": None},
     },
     response_model_exclude_none=True,
     openapi_extra={"spec_order": 220},
 )
 async def acknowledge_message(
+    background_tasks: BackgroundTasks,
     request: Request,
     message_id: str = Depends(normalise_message_id_path),
     accepts_api_version: int = Depends(get_accepts_api_version),
     handler: InboxHandler = Depends(InboxHandler),
 ):
     return await handler.acknowledge_message(
-        cast(Mailbox, request.state.authorised_mailbox), message_id, accepts_api_version
+        background_tasks, cast(Mailbox, request.state.authorised_mailbox), message_id, accepts_api_version
     )
 
 
 @router.head(
     "/{message_id}",
     summary="Head Message",
     responses={
@@ -210,17 +220,20 @@
     request: Request,
     message_id: str = Depends(normalise_message_id_path),
     accept_encoding: str = Header(
         title="Accept-Encoding",
         default="",
         example="gzip",
     ),
+    accepts_api_version: int = Depends(get_accepts_api_version),
     handler: InboxHandler = Depends(InboxHandler),
 ):
-    return await handler.retrieve_message(cast(Mailbox, request.state.authorised_mailbox), message_id, accept_encoding)
+    return await handler.retrieve_message(
+        cast(Mailbox, request.state.authorised_mailbox), message_id, accept_encoding, accepts_api_version
+    )
 
 
 @router.get(
     "/{message_id}/{chunk_number}",
     summary="Download message chunk",
     response_class=Response,
     responses={
@@ -244,15 +257,17 @@
     message_id: str = Depends(normalise_message_id_path),
     chunk_number: int = Path(..., title="chunk_number", description="The index number of the chunk", example="1", ge=1),
     accept_encoding: str = Header(
         title="Accept-Encoding",
         default="",
         example="gzip",
     ),
+    accepts_api_version: int = Depends(get_accepts_api_version),
     handler: InboxHandler = Depends(InboxHandler),
 ):
     return await handler.retrieve_chunk(
         cast(Mailbox, request.state.authorised_mailbox),
         message_id,
         accept_encoding,
         chunk_number=chunk_number,
+        accepts_api_version=accepts_api_version,
     )
```

## mesh_sandbox/routers/inbox_count.py

```diff
@@ -28,23 +28,26 @@
                 },
                 MESH_MEDIA_TYPES[1]: {
                     "schema": InboxCountV1.schema(),
                 },
             }
         }
     },
+    deprecated=True,
     response_model_exclude_none=True,
     openapi_extra={"spec_order": 290},
 )
 async def count_messages_in_inbox(
     request: Request,
     accepts_api_version: int = Depends(get_accepts_api_version),
 ):
     mailbox = cast(Mailbox, request.state.authorised_mailbox)
 
+    count = mailbox.inbox_count or 0
+
     response = (
-        InboxCountV1(count=mailbox.inbox_count, internalID=uuid4().hex, allResultsIncluded=True)
+        InboxCountV1(count=count, internalID=uuid4().hex, allResultsIncluded=True)
         if accepts_api_version < 2
-        else InboxCountV2(count=mailbox.inbox_count)
+        else InboxCountV2(count=count)
     )
 
     return JSONResponse(content=exclude_none_json_encoder(response))
```

## mesh_sandbox/routers/outbox.py

```diff
@@ -1,17 +1,29 @@
 from typing import Optional, cast
 
-from fastapi import APIRouter, Depends, Header, Path, Query, Request, Response, status
+from fastapi import (
+    APIRouter,
+    BackgroundTasks,
+    Depends,
+    Header,
+    Path,
+    Query,
+    Request,
+    Response,
+    status,
+)
 
 from ..common import MESH_MEDIA_TYPES
 from ..common.constants import Headers
 from ..common.mex_headers import MexHeaders, send_message_mex_headers
 from ..dependencies import (
     authorised_mailbox,
     get_accepts_api_version,
+    normalise_content_encoding,
+    normalise_content_type,
     normalise_message_id_path,
 )
 from ..handlers.outbox import OutboxHandler
 from ..models.mailbox import Mailbox
 from ..views.outbox import RichOutboxView, SendMessageV1, SendMessageV2
 from .request_logging import RequestLoggingRoute
 
@@ -38,51 +50,53 @@
         status.HTTP_417_EXPECTATION_FAILED: {"content": None},
     },
     status_code=status.HTTP_202_ACCEPTED,
     response_model_exclude_none=True,
     openapi_extra={"spec_order": 300},
 )
 async def send_message(
+    background_tasks: BackgroundTasks,
     request: Request,
     mex_headers: MexHeaders = Depends(send_message_mex_headers),
-    content_encoding: str = Header(
-        title=Headers.Content_Encoding, description="content encoding", example="gzip", default=""
-    ),
+    content_type: str = Depends(normalise_content_type),
+    content_encoding: str = Depends(normalise_content_encoding),
     accepts_api_version: int = Depends(get_accepts_api_version),
     handler: OutboxHandler = Depends(OutboxHandler),
 ):
     return await handler.send_message(
+        background_tasks=background_tasks,
         request=request,
         sender_mailbox=cast(Mailbox, request.state.authorised_mailbox),
         mex_headers=mex_headers,
         content_encoding=content_encoding,
+        content_type=content_type,
         accepts_api_version=accepts_api_version,
     )
 
 
 @router.post(
     "/{message_id}/{chunk_number}",
     summary="Send chunked message",
     responses={202: {"content": None}},
     status_code=status.HTTP_202_ACCEPTED,
     response_model_exclude_none=True,
     openapi_extra={"spec_order": 310},
 )
 async def send_chunk(
+    background_tasks: BackgroundTasks,
     request: Request,
     message_id: str = Depends(normalise_message_id_path),
     mex_chunk_range: str = Header(title=Headers.Mex_Chunk_Range, default="", example="1:2", max_length=20),
-    content_encoding: str = Header(
-        title=Headers.Content_Encoding, description="content encoding", example="gzip", default=""
-    ),
+    content_encoding: str = Depends(normalise_content_encoding),
     chunk_number: int = Path(..., title="chunk_number", description="The index number of the chunk", example="1"),
     accepts_api_version: int = Depends(get_accepts_api_version),
     handler: OutboxHandler = Depends(OutboxHandler),
 ):
     return await handler.send_chunk(
+        background_tasks=background_tasks,
         request=request,
         sender_mailbox=cast(Mailbox, request.state.authorised_mailbox),
         message_id=message_id,
         chunk_number=chunk_number,
         mex_chunk_range=mex_chunk_range,
         content_encoding=content_encoding,
         accepts_api_version=accepts_api_version,
```

## mesh_sandbox/store/base.py

```diff
@@ -1,172 +1,76 @@
+import logging
 from abc import ABC, abstractmethod
-from typing import NamedTuple, Optional
+from typing import Callable, Optional
 
-from fastapi import HTTPException, status
-
-from ..common import EnvConfig, constants, generate_cipher_text
+from ..common import EnvConfig
 from ..models.mailbox import Mailbox
 from ..models.message import Message
 
 
-class AuthoriseHeaderParts(NamedTuple):
-    scheme: str
-    mailbox_id: str
-    nonce: str
-    nonce_count: str
-    timestamp: str
-    cipher_text: str
-    parts: int
-
-    def get_reasons_invalid(self) -> list[str]:
-        reasons = []
-        if self.parts != 5:
-            reasons.append(f"invalid num header parts: {self.parts}")
-
-        if not self.nonce_count.isdigit():
-            reasons.append("nonce count is not digits")
-
-        if self.scheme not in (MESH_AUTH_SCHEME, ""):
-            reasons.append("invalid auth scheme or mailbox_id contains a space")
-
-        if " " in self.mailbox_id:
-            reasons.append("mailbox_id contains a space")
-
-        return reasons
-
-
-_DEFAULT_PARTS_IF_MISSING = ["" for _ in range(5)]
-MESH_AUTH_SCHEME = "NHSMESH"
-
-
-def try_parse_authorisation_token(auth_token: str) -> Optional[AuthoriseHeaderParts]:
-
-    if not auth_token:
-        return None
-
-    auth_token = auth_token.strip()
-
-    scheme = MESH_AUTH_SCHEME if auth_token.upper().startswith(MESH_AUTH_SCHEME) else ""
-
-    if scheme:
-        auth_token = auth_token[len(MESH_AUTH_SCHEME) + 1 :]
-
-    auth_token_parts = auth_token.split(":")
-
-    num_parts = len(auth_token_parts)
-    auth_token_parts = auth_token_parts + _DEFAULT_PARTS_IF_MISSING
-
-    header_parts = AuthoriseHeaderParts(
-        scheme=scheme,
-        mailbox_id=auth_token_parts[0],
-        nonce=auth_token_parts[1],
-        nonce_count=auth_token_parts[2],
-        timestamp=auth_token_parts[3],
-        cipher_text=auth_token_parts[4],
-        parts=num_parts,
-    )
-
-    return header_parts
+class Store(ABC):
 
+    readonly = True
 
-class Store(ABC):
-    def __init__(self, config: EnvConfig):
+    def __init__(self, config: EnvConfig, logger: logging.Logger):
         self.config = config
+        self.logger = logger
 
     @abstractmethod
     async def get_mailbox(self, mailbox_id: str, accessed: bool = False) -> Optional[Mailbox]:
         pass
 
-    async def _validate_auth_token(self, mailbox_id: str, authorization: str) -> Optional[Mailbox]:
-
-        if self.config.auth_mode == "none":
-            return await self.get_mailbox(mailbox_id, accessed=True)
-
-        authorization = (authorization or "").strip()
-        if not authorization:
-            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=constants.ERROR_READING_AUTH_HEADER)
-
-        header_parts = try_parse_authorisation_token(authorization)
-        if not header_parts:
-            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=constants.ERROR_READING_AUTH_HEADER)
-
-        if header_parts.mailbox_id != mailbox_id:
-            raise HTTPException(status_code=status.HTTP_403_FORBIDDEN, detail=constants.ERROR_MAILBOX_TOKEN_MISMATCH)
-
-        if self.config.auth_mode == "canned":
-
-            if header_parts.nonce.upper() != "VALID":
-                raise HTTPException(status_code=status.HTTP_403_FORBIDDEN, detail=constants.ERROR_INVALID_AUTH_TOKEN)
-            return await self.get_mailbox(mailbox_id, accessed=True)
-
-        if header_parts.get_reasons_invalid():
-            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=constants.ERROR_INVALID_AUTH_TOKEN)
-
-        mailbox = await self.get_mailbox(mailbox_id, accessed=True)
-
-        if not mailbox:
-            return None
-
-        cypher_text = generate_cipher_text(
-            self.config.shared_key,
-            header_parts.mailbox_id,
-            mailbox.password,
-            header_parts.timestamp,
-            header_parts.nonce,
-            header_parts.nonce_count,
-        )
-
-        if header_parts.cipher_text != cypher_text:
-            raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail=constants.ERROR_INVALID_AUTH_TOKEN)
-
-        return mailbox
-
-    async def authorise_mailbox(self, mailbox_id: str, authorization: str) -> Optional[Mailbox]:
-
-        mailbox = await self._validate_auth_token(mailbox_id, authorization)
+    @abstractmethod
+    async def get_message(self, message_id: str) -> Optional[Message]:
+        pass
 
-        if not mailbox:
-            raise HTTPException(status_code=status.HTTP_403_FORBIDDEN, detail=constants.ERROR_NO_MAILBOX_MATCHES)
+    @abstractmethod
+    async def save_message(self, message: Message):
+        pass
 
-        return mailbox
+    @abstractmethod
+    async def get_chunk(self, message: Message, chunk_number: int) -> Optional[bytes]:
+        pass
 
     @abstractmethod
-    async def send_message(self, message: Message, body: bytes):
+    async def save_chunk(self, message: Message, chunk_number: int, chunk: bytes):
         pass
 
     @abstractmethod
-    async def receive_chunk(self, message: Message, chunk_number: int, chunk: bytes):
+    async def add_to_outbox(self, message: Message):
         pass
 
     @abstractmethod
-    async def accept_message(self, message: Message):
+    async def add_to_inbox(self, message: Message):
         pass
 
     @abstractmethod
-    async def acknowledge_message(self, message: Message):
+    async def get_file_size(self, message: Message) -> int:
         pass
 
     @abstractmethod
-    async def get_message(self, message_id: str) -> Optional[Message]:
+    async def reset(self):
         pass
 
     @abstractmethod
-    async def get_inbox(self, mailbox_id: str) -> list[Message]:
+    async def reset_mailbox(self, mailbox_id: str):
         pass
 
     @abstractmethod
-    async def get_outbox(self, mailbox_id: str) -> list[Message]:
+    async def get_inbox_messages(
+        self, mailbox_id: str, predicate: Optional[Callable[[Message], bool]] = None
+    ) -> list[Message]:
         pass
 
     @abstractmethod
-    async def get_by_local_id(self, mailbox_id: str, local_id: str) -> list[Message]:
+    async def get_outbox(self, mailbox_id: str) -> list[Message]:
         pass
 
     @abstractmethod
-    async def retrieve_chunk(self, message: Message, chunk_number: int) -> Optional[bytes]:
+    async def get_by_local_id(self, mailbox_id: str, local_id: str) -> list[Message]:
         pass
 
     @abstractmethod
     async def lookup_by_ods_code_and_workflow_id(self, ods_code: str, workflow_id: str) -> list[Mailbox]:
         pass
 
     @abstractmethod
```

## mesh_sandbox/store/canned_store.py

```diff
@@ -1,83 +1,100 @@
-import asyncio
-import base64
 import json
+import logging
 import os
-import threading
 from collections import defaultdict
 from datetime import datetime
-from typing import Optional, cast
+from json import JSONDecodeError
+from typing import Callable, Optional, cast
+from weakref import WeakValueDictionary
+
+from dateutil.relativedelta import relativedelta
 
 from ..common import EnvConfig
 from ..models.mailbox import Mailbox
-from ..models.message import Message, MessageStatus
+from ..models.message import Message, MessageStatus, MessageType
 from ..models.workflow import Workflow
 from .base import Store
 from .serialisation import deserialise_model
 
 
+def _accepted_messages(msg: Message) -> bool:
+    return msg.status == MessageStatus.ACCEPTED
+
+
 class CannedStore(Store):
     """
     pre canned messages or mailboxes not editable
     """
 
-    def __init__(self, config: EnvConfig, load_messages: bool = True):
-        super().__init__(config)
-        self._sync_lock = threading.Lock()
-        self._lock = None
+    load_messages = True
+
+    def __init__(self, config: EnvConfig, logger: logging.Logger, filter_expired: bool = False):
+        self._config = config
+        self._canned_data_dir = os.path.join(os.path.dirname(__file__), "data")
+        self._mailboxes_data_dir = self.get_mailboxes_data_dir()
+        self._filter_expired = filter_expired
+        super().__init__(self._config, logger)
+
+        self.initialise()
+
+    def get_mailboxes_data_dir(self) -> str:
+        return os.path.join(self._canned_data_dir, "mailboxes")
+
+    def initialise(self):
         self.mailboxes = self._load_mailboxes()
         self.endpoints = self._load_endpoints()
-        self.chunks = self._load_chunks() if load_messages else {}
-        self.messages = self._load_messages() if load_messages else {}
+        self.messages = self._load_messages() if self.load_messages else {}
+        self.chunks = self._load_chunks() if self.load_messages else defaultdict(list)
         self.inboxes: dict[str, list[Message]] = {mailbox.mailbox_id: [] for mailbox in self.mailboxes.values()}
         self.outboxes: dict[str, list[Message]] = {mailbox.mailbox_id: [] for mailbox in self.mailboxes.values()}
         self.local_ids: dict[str, dict[str, list[Message]]] = {
             mailbox.mailbox_id: defaultdict(list) for mailbox in self.mailboxes.values()
         }
         self._fill_boxes()
-
-    @property
-    def lock(self):
-
-        if self._lock is not None:
-            return self._lock
-
-        with self._sync_lock:
-            if self._lock is not None:
-                return self._lock
-            self._lock = asyncio.Lock()
-            return self._lock
+        self.messages = cast(dict[str, Message], WeakValueDictionary(self.messages))
 
     def _fill_boxes(self):
         for message in self.messages.values():
             if message.sender.mailbox_id and message.sender.mailbox_id in self.mailboxes:
                 self.outboxes[message.sender.mailbox_id].append(message)
 
-            if message.status != MessageStatus.ACCEPTED or message.recipient.mailbox_id not in self.mailboxes:
+            if message.recipient.mailbox_id not in self.mailboxes:
                 continue
 
             self.inboxes[message.recipient.mailbox_id].append(message)
 
         for inbox in self.inboxes.values():
             inbox.sort(key=lambda msg: msg.created_timestamp)
 
         for mailbox_id, outbox in self.outboxes.items():
             outbox.sort(reverse=True, key=lambda msg: msg.created_timestamp)
             for message in outbox:
                 if not message.metadata.local_id:
                     continue
                 self.local_ids[mailbox_id][message.metadata.local_id].append(message)
 
+        for mailbox in self.mailboxes.values():
+            mailbox.inbox_count = sum(
+                1 for message in self.inboxes[mailbox.mailbox_id] if message.status == MessageStatus.ACCEPTED
+            )
+
     def _load_endpoints(self) -> dict[str, list[Mailbox]]:
 
-        with open(os.path.join(os.path.dirname(__file__), "data/workflows.jsonl"), "r", encoding="utf-8") as f:
+        canned_workflows = os.path.join(self._canned_data_dir, "workflows.jsonl")
+        endpoints: dict[str, list[Mailbox]] = defaultdict(list)
+
+        if not os.path.exists(canned_workflows):
+            return endpoints
+
+        with open(canned_workflows, "r", encoding="utf-8") as f:
             workflows = list(
                 cast(Workflow, deserialise_model(json.loads(line), Workflow)) for line in f.readlines() if line.strip()
             )
-            endpoints = defaultdict(list)
+
             for workflow in workflows:
 
                 receivers = workflow.receivers
                 for receiver in receivers:
                     receiver = (receiver or "").strip().upper()
                     mailbox = self.mailboxes.get(receiver)
                     if not mailbox:
@@ -87,98 +104,146 @@
                     ods_code = (mailbox.ods_code or "").strip().upper()
                     if not ods_code:
                         continue
                     endpoints[f"{ods_code}/{workflow.workflow_id}"].append(mailbox)
 
             return endpoints
 
-    @staticmethod
-    def _load_mailboxes() -> dict[str, Mailbox]:
+    def _load_mailboxes(self) -> dict[str, Mailbox]:
+
+        canned_mailboxes = os.path.join(self._canned_data_dir, "mailboxes.jsonl")
 
-        with open(os.path.join(os.path.dirname(__file__), "data/mailboxes.jsonl"), "r", encoding="utf-8") as f:
+        if not os.path.exists(canned_mailboxes):
+            return {}
+
+        with open(canned_mailboxes, "r", encoding="utf-8") as f:
             return {
                 mailbox.mailbox_id: mailbox
                 for mailbox in (
                     cast(Mailbox, deserialise_model(json.loads(line), Mailbox))
                     for line in f.readlines()
                     if line.strip()
                 )
             }
 
-    @staticmethod
-    def _load_messages() -> dict[str, Message]:
-        with open(os.path.join(os.path.dirname(__file__), "data/messages.jsonl"), "r", encoding="utf-8") as f:
-            return {
-                message.message_id: message
-                for message in (
-                    cast(Message, deserialise_model(json.loads(line), Message))
-                    for line in f.readlines()
-                    if line.strip()
-                )
-            }
+    def _load_messages(self) -> dict[str, Message]:
 
-    @staticmethod
-    def _load_chunks() -> dict[str, list[bytes]]:
+        messages: dict[str, Message] = {}
 
-        chunks = defaultdict(list)
+        if not os.path.exists(self._mailboxes_data_dir):
+            return messages
 
-        with open(os.path.join(os.path.dirname(__file__), "data/chunks.jsonl"), "r", encoding="utf-8") as f:
+        for mailbox_path in os.scandir(self._mailboxes_data_dir):
+            if not mailbox_path.is_dir():
+                continue
+            mailbox_id = mailbox_path.name.upper().strip()
+            if mailbox_id != mailbox_path.name:
+                raise ValueError("mailbox directory names should be upper case")
+
+            if mailbox_id not in self.mailboxes:
+                self.mailboxes[mailbox_id] = Mailbox(mailbox_id=mailbox_id, mailbox_name="Unknown", password="password")
 
-            for line in f.readlines():
-                line = line.strip()
-                if not line:
+            inbox_dir = os.path.join(self._mailboxes_data_dir, mailbox_id, "in")
+            if not os.path.exists(inbox_dir):
+                continue
+
+            for message_path in os.scandir(inbox_dir):
+
+                if not message_path.is_file() or not message_path.name.endswith(".json"):
                     continue
-                loaded = json.loads(line)
-                chunks[loaded["message_id"]].append(loaded)
 
-        for message_chunks in chunks.values():
-            message_chunks.sort(key=lambda x: cast(int, x["chunk_no"]))
+                try:
+                    with open(message_path.path, "r", encoding="utf-8") as f:
+                        message = deserialise_model(json.load(f), Message)
+                        assert message
+                        message_expiry_date = message.created_timestamp + relativedelta(
+                            days=self.config.message_expiry_days
+                        )
+                        if self._filter_expired and message_expiry_date <= datetime.utcnow():
+                            continue
+                        messages[message.message_id] = message
+                except JSONDecodeError as e:
+                    print(f"failed to load message json {message_path.path}")
+                    print(e)
 
-        parsed_chunks = {k: [base64.b64decode(chunk["data"]) for chunk in v] for k, v in chunks.items()}
+        return messages
 
-        return parsed_chunks
+    def _load_chunks(self) -> dict[str, list[Optional[bytes]]]:
+
+        chunks: dict[str, list[Optional[bytes]]] = defaultdict(list)
+
+        for message in self.messages.values():
+            if not message.recipient.mailbox_id or message.message_type != MessageType.DATA or message.total_chunks < 1:
+                continue
+
+            chunks_dir = os.path.join(self._mailboxes_data_dir, message.recipient.mailbox_id, "in", message.message_id)
+            message_chunks: list[Optional[bytes]] = [None for _ in range(message.total_chunks)]
+            for chunk_no in range(message.total_chunks):
+                chunk_path = os.path.join(chunks_dir, str(chunk_no + 1))
+                if not os.path.exists(chunk_path):
+                    continue
+                with open(chunk_path, "rb") as f:
+                    message_chunks[chunk_no] = f.read()
+            chunks[message.message_id] = message_chunks
+
+        return chunks
 
     async def get_mailbox(self, mailbox_id: str, accessed: bool = False) -> Optional[Mailbox]:
         mailbox = self.mailboxes.get(mailbox_id)
         if not mailbox:
             return None
 
-        mailbox.inbox_count = len(self.inboxes[mailbox_id])
+        mailbox.inbox_count = len(await self.get_inbox_messages(mailbox_id, _accepted_messages))
         if accessed:
             mailbox.last_accessed = datetime.utcnow()
         return mailbox
 
-    async def send_message(self, message: Message, body: bytes):
-        pass
+    async def get_message(self, message_id: str) -> Optional[Message]:
+        return self.messages.get(message_id)
 
-    async def accept_message(self, message: Message):
-        pass
+    async def get_file_size(self, message: Message) -> int:
+        return sum(len(chunk or b"") for chunk in self.chunks.get(message.message_id, []))
 
-    async def acknowledge_message(self, message: Message):
-        pass
+    async def add_to_outbox(self, message: Message):
+        """does nothing on this readonly store..."""
 
-    async def receive_chunk(self, message: Message, chunk_number: int, chunk: bytes):
-        pass
+    async def add_to_inbox(self, message: Message):
+        """does nothing on this readonly store..."""
 
-    async def get_message(self, message_id: str) -> Optional[Message]:
-        return self.messages.get(message_id)
+    async def save_message(self, message: Message):
+        raise NotImplementedError()
 
-    async def get_inbox(self, mailbox_id: str) -> list[Message]:
-        return self.inboxes[mailbox_id]
+    async def get_chunk(self, message: Message, chunk_number: int) -> Optional[bytes]:
+        parts = self.chunks.get(message.message_id, [])
+        if not parts or len(parts) < chunk_number:
+            return None
+        return parts[chunk_number - 1]
+
+    async def save_chunk(self, message: Message, chunk_number: int, chunk: bytes):
+        raise NotImplementedError()
+
+    async def reset(self):
+        raise NotImplementedError()
+
+    async def reset_mailbox(self, mailbox_id: str):
+        raise NotImplementedError()
+
+    async def get_inbox_messages(
+        self, mailbox_id: str, predicate: Optional[Callable[[Message], bool]] = None
+    ) -> list[Message]:
+        inbox = self.inboxes[mailbox_id]
+        if not predicate:
+            return inbox
+
+        return [m for m in inbox if predicate(m)]
 
     async def get_outbox(self, mailbox_id: str) -> list[Message]:
         return self.outboxes[mailbox_id]
 
     async def get_by_local_id(self, mailbox_id: str, local_id: str) -> list[Message]:
         return self.local_ids.get(mailbox_id, {}).get(local_id, [])
 
-    async def retrieve_chunk(self, message: Message, chunk_number: int) -> Optional[bytes]:
-        parts: list[bytes] = self.chunks.get(message.message_id, [])
-        if not parts or len(parts) < chunk_number:
-            return None
-        return parts[chunk_number - 1]
-
     async def lookup_by_ods_code_and_workflow_id(self, ods_code: str, workflow_id: str) -> list[Mailbox]:
         return self.endpoints.get(f"{ods_code}/{workflow_id}", [])
 
     async def lookup_by_workflow_id(self, workflow_id: str) -> list[Mailbox]:
         return self.endpoints.get(workflow_id, [])
```

## mesh_sandbox/store/data/mailboxes.jsonl

```diff
@@ -1,3 +1,3 @@
 {"mailbox_id":  "X26ABC1", "mailbox_name": "TESTMB1", "billing_entity": "England", "ods_code": "X26", "org_code": "X26", "password": "password"}
-{"mailbox_id":  "X26ABC2", "mailbox_name": "TESTMB2", "billing_entity": "England", "ods_code": "X26", "org_code": "X26", "password": "password"}
+{"mailbox_id":  "X26ABC2", "mailbox_name": "TESTMB2", "billing_entity": "Wales", "ods_code": "X26", "org_code": "X26", "password": "password"}
 {"mailbox_id":  "X26ABC3", "mailbox_name": "TESTMB3", "billing_entity": "England", "ods_code": "X27", "org_code": "X27", "password": "password"}
```

## mesh_sandbox/store/file_store.py

```diff
@@ -1,41 +1,69 @@
+import json
 import os.path
+from collections import defaultdict
 from typing import Optional
 
-from ..common import EnvConfig
 from ..models.message import Message
 from .memory_store import MemoryStore
+from .serialisation import serialise_model
 
 
 class FileStore(MemoryStore):
 
     """file based store, will store the message payloads in the filesystem"""
 
-    def __init__(self, config: EnvConfig):
-        super().__init__(config)
-        self._base_dir = config.file_store_dir
+    load_messages = True
 
-    async def _get_file_size(self, message: Message) -> int:
-        size = 0
-        message_dir = os.path.join(self._base_dir, f"{message.recipient.mailbox_id}/in/{message.message_id}")
-        for file in os.listdir(message_dir):
-            stat = os.stat(f"{message_dir}/{file}")
-            size += stat.st_size
-        return size
+    def get_mailboxes_data_dir(self) -> str:
+        return self._config.mailboxes_dir
+
+    def message_path(self, message: Message) -> str:
+        return os.path.join(self._mailboxes_data_dir, message.recipient.mailbox_id, "in", message.message_id)
 
     def chunk_path(self, message: Message, chunk_number: int) -> str:
-        return os.path.join(self._base_dir, f"{message.recipient.mailbox_id}/in/{message.message_id}/{chunk_number}")
+        return os.path.join(
+            self._mailboxes_data_dir, message.recipient.mailbox_id, "in", message.message_id, str(chunk_number)
+        )
+
+    def _load_chunks(self) -> dict[str, list[Optional[bytes]]]:
+        """overrides canned store default data load"""
+        return defaultdict(list)
+
+    async def save_message(self, message: Message):
+        await super().save_message(message)
+        message_json_path = f"{self.message_path(message)}.json"
+        os.makedirs(os.path.dirname(message_json_path), exist_ok=True)
+        with open(message_json_path, "w+", encoding="utf-8") as f:
+            json.dump(serialise_model(message), f)
 
-    async def receive_chunk(self, message: Message, chunk_number: int, chunk: bytes):
+    async def save_chunk(self, message: Message, chunk_number: int, chunk: Optional[bytes]):
         chunk_path = self.chunk_path(message, chunk_number)
+        if chunk is None:
+            if not os.path.exists(chunk_path):
+                return
+            os.remove(chunk_path)
+            return
+
         os.makedirs(os.path.dirname(chunk_path), exist_ok=True)
         with open(chunk_path, "wb+") as f:
             f.write(chunk)
 
-    async def retrieve_chunk(self, message: Message, chunk_number: int) -> Optional[bytes]:
+    async def get_chunk(self, message: Message, chunk_number: int) -> Optional[bytes]:
 
         chunk_path = self.chunk_path(message, chunk_number)
         if not os.path.exists(chunk_path):
             return None
 
-        with open(chunk_path, "rb+") as f:
+        with open(chunk_path, "rb") as f:
             return f.read()
+
+    async def get_file_size(self, message: Message) -> int:
+        size = 0
+        if message.total_chunks < 1:
+            return 0
+
+        message_dir = self.message_path(message)
+        for chunk_no in range(message.total_chunks):
+            stat = os.stat(f"{message_dir}/{chunk_no+1}")
+            size += stat.st_size
+        return size
```

## mesh_sandbox/store/memory_store.py

```diff
@@ -1,57 +1,49 @@
-from typing import cast
+import logging
+from collections import defaultdict
+from typing import Optional
 
 from ..common import EnvConfig
-from ..models.message import Message, MessageEvent, MessageStatus
+from ..models.message import Message
 from .canned_store import CannedStore
 
 
 class MemoryStore(CannedStore):
     """
     in memory store, good for 'in-process' testing or small messages
     """
 
-    def __init__(self, config: EnvConfig):
-        super().__init__(config, load_messages=False)
+    readonly = False
+    load_messages = False
 
-    async def send_message(self, message: Message, body: bytes):
+    def __init__(self, config: EnvConfig, logger: logging.Logger):
+        super().__init__(config, logger, filter_expired=True)
 
-        async with self.lock:
-            parts: list[bytes] = cast(list[bytes], [None for _ in range(message.total_chunks)])
+    async def reset(self):
+        super().initialise()
 
-            self.messages[message.message_id] = message
-            self.chunks[message.message_id] = parts
+    async def reset_mailbox(self, mailbox_id: str):
+        self.inboxes[mailbox_id] = []
+        self.outboxes[mailbox_id] = []
+        self.local_ids[mailbox_id] = defaultdict(list)
+        self.mailboxes[mailbox_id].inbox_count = 0
 
-            await self.receive_chunk(message, 1, body)
+    async def add_to_outbox(self, message: Message):
+        if not message.sender.mailbox_id:
+            return
 
-            if message.sender.mailbox_id:
-                self.outboxes[message.sender.mailbox_id].insert(0, message)
-                if message.metadata.local_id:
-                    self.local_ids[message.sender.mailbox_id][message.metadata.local_id].insert(0, message)
+        self.outboxes[message.sender.mailbox_id].insert(0, message)
+        if not message.metadata.local_id:
+            return
 
-            if message.status != MessageStatus.ACCEPTED:
-                return
+        self.local_ids[message.sender.mailbox_id][message.metadata.local_id].insert(0, message)
 
-            self.inboxes[message.recipient.mailbox_id].append(message)
+    async def add_to_inbox(self, message: Message):
+        self.inboxes[message.recipient.mailbox_id].append(message)
 
-    async def receive_chunk(self, message: Message, chunk_number: int, chunk: bytes):
-        self.chunks[message.message_id][chunk_number - 1] = chunk
-
-    async def _get_file_size(self, message: Message) -> int:
-        return sum(len(chunk) for chunk in self.chunks.get(message.message_id, []))
+    async def save_message(self, message: Message):
+        self.messages[message.message_id] = message
 
-    async def accept_message(self, message: Message):
-        async with self.lock:
-            message.events.insert(0, MessageEvent(status=MessageStatus.ACCEPTED))
-            message.file_size = await self._get_file_size(message)
-            self.inboxes[message.recipient.mailbox_id].append(message)
-
-    async def acknowledge_message(self, message: Message):
-        async with self.lock:
-            message.events.insert(0, MessageEvent(status=MessageStatus.ACKNOWLEDGED))
-            inbox = self.inboxes[message.recipient.mailbox_id]
-
-            for ix, inbox_message in enumerate(inbox):
-                if inbox_message.message_id != message.message_id:
-                    continue
-                inbox.pop(ix)
-                break
+    async def save_chunk(self, message: Message, chunk_number: int, chunk: Optional[bytes]):
+        if message.message_id not in self.chunks:
+            self.chunks[message.message_id] = [None for _ in range(message.total_chunks)]
+        self.chunks[message.message_id][chunk_number - 1] = chunk
```

## mesh_sandbox/store/serialisation.py

```diff
@@ -129,8 +129,8 @@
     for field in model_fields:
         value = model_dict.get(field.name)
         if value is None:
             continue
 
         deserialised[field.name] = _deserialise_value(field.type, value)
 
-    return model_type(**deserialised)
+    return model_type(**deserialised)  # type: ignore[return-value]
```

## mesh_sandbox/tests/__init__.py

```diff
@@ -0,0 +1,7 @@
+00000000: 5f43 414e 4e45 445f 4d41 494c 424f 5831  _CANNED_MAILBOX1
+00000010: 203d 2022 5832 3641 4243 3122 0a5f 4341   = "X26ABC1"._CA
+00000020: 4e4e 4544 5f4d 4149 4c42 4f58 3220 3d20  NNED_MAILBOX2 = 
+00000030: 2258 3236 4142 4332 220a 5f53 4841 5245  "X26ABC2"._SHARE
+00000040: 445f 4b45 5920 3d20 6222 5465 7374 4b65  D_KEY = b"TestKe
+00000050: 7922 0a5f 5041 5353 574f 5244 203d 2022  y"._PASSWORD = "
+00000060: 7061 7373 776f 7264 220a                 password".
```

## mesh_sandbox/tests/docker_tests.py

```diff
@@ -10,23 +10,28 @@
 
 def test_send_receive_chunked_message():
 
     sender_mailbox_id = _CANNED_MAILBOX1
     recipient_mailbox_id = _CANNED_MAILBOX2
     workflow_id = uuid4().hex
 
-    base_uri = "http://localhost:8700"
+    base_uri = "https://localhost:8700"
 
     with MeshClient(
-        url=base_uri, mailbox=sender_mailbox_id, password=_PASSWORD, shared_key=_SHARED_KEY, max_chunk_size=100
+        url=base_uri,
+        mailbox=sender_mailbox_id,
+        password=_PASSWORD,
+        shared_key=_SHARED_KEY,
+        max_chunk_size=100,
+        verify=False,
     ) as sender:
 
         sent_payload = b"a" * 1000
 
-        message_id = sender.send_message(_CANNED_MAILBOX2, sent_payload, workflow_id=workflow_id)
+        message_id = sender.send_message(_CANNED_MAILBOX2, sent_payload, workflow_id=workflow_id, subject="change me")
 
         assert message_id
 
         with MeshClient(
             url=base_uri, mailbox=recipient_mailbox_id, password=_PASSWORD, shared_key=_SHARED_KEY
         ) as recipient:
             message_ids = recipient.list_messages()
@@ -35,7 +40,10 @@
             assert message.workflow_id == workflow_id  # pylint: disable=no-member
             received_payload = message.read()
             assert received_payload == sent_payload
 
             message.acknowledge()
             message_ids = recipient.list_messages()
             assert message_ids == []
+
+            # test that plugin is loaded and is able to edit the message ( though this wouldn't be saved in file mode )
+            assert message.subject == "plugin message from file"  # pylint: disable=no-member
```

## mesh_sandbox/tests/helpers.py

```diff
@@ -4,19 +4,17 @@
 import shutil
 import subprocess
 from datetime import datetime
 from typing import Optional
 from uuid import uuid4
 
 import httpx
-from fastapi.testclient import TestClient
 from OpenSSL import crypto
 
 from ..common import MESH_AUTH_SCHEME, generate_cipher_text
-from ..common.constants import Headers
 
 
 def generate_auth_token(
     mailbox_id: str,
     mailbox_password: str = "password",
     secret_key: str = "TestKey",
     timestamp: Optional[datetime] = None,
@@ -45,45 +43,14 @@
     try:
         yield
     finally:
         os.environ.clear()
         os.environ.update(old_environ)
 
 
-def send_message(
-    app: TestClient,
-    sender_mailbox_id: str,
-    recipient_mailbox_id: str,
-    workflow_id: Optional[str] = None,
-    message_data: Optional[bytes] = None,
-    extra_headers: Optional[dict] = None,
-    test_empty_payload: bool = False,
-    file_name: Optional[str] = None,
-):
-
-    if not test_empty_payload:
-        message_data = message_data or f"Hello World!\n{uuid4().hex}".encode("utf-8")
-
-    headers = {
-        Headers.Mex_From: sender_mailbox_id,
-        Headers.Mex_To: recipient_mailbox_id,
-        Headers.Mex_WorkflowID: workflow_id or "TEST_WORKFLOW",
-        Headers.Authorization: generate_auth_token(sender_mailbox_id),
-    }
-    if file_name:
-        headers[Headers.Mex_FileName] = file_name
-
-    if extra_headers:
-        headers.update(extra_headers)
-
-    response = app.post(f"/messageexchange/{sender_mailbox_id}/outbox", headers=headers, data=message_data)
-
-    return response
-
-
 def ensure_client_installed(java_path: str, base_dir: str, version: str):  # pylint: disable=too-many-locals
 
     install_dir = os.path.join(base_dir, version)
 
     client_dir = os.path.join(install_dir, "client")
 
     if os.path.exists(os.path.join(client_dir, "meshClient.jar")):
@@ -98,15 +65,15 @@
     os.makedirs(data_dir, exist_ok=True)
 
     installer_rar = os.path.join(installer_dir, "installer.rar")
     if not os.path.exists(installer_rar):
         version_dash = version.replace(".", "-")
 
         installer_uri = (
-            "https://nhs-prod.global.ssl.fastly.net/binaries/content/assets/website-assets/services"
+            "https://digital.nhs.uk/binaries/content/assets/website-assets/services"
             f"/message-exchange-for-social-care-and-health-mesh/mesh-installation-pack-client-{version_dash}.rar"
         )
 
         with httpx.Client() as client:
             res = client.get(installer_uri)
             with open(installer_rar, "wb+") as f:
                 f.write(res.read())
```

## mesh_sandbox/tests/inbox.py

```diff
@@ -1,17 +1,19 @@
 from uuid import uuid4
 
 import pytest
 from fastapi import status
 from fastapi.testclient import TestClient
 
+from mesh_sandbox.tests.mesh_api_helpers import mesh_api_send_message
+
 from ..common import APP_V1_JSON, APP_V2_JSON
 from ..common.constants import Headers
 from ..models.message import MessageStatus
-from .helpers import generate_auth_token, send_message, temp_env_vars
+from .helpers import generate_auth_token, temp_env_vars
 
 _CANNED_MAILBOX1 = "X26ABC1"
 _CANNED_MAILBOX2 = "X26ABC2"
 
 
 @pytest.mark.parametrize("accept", [APP_V1_JSON, APP_V2_JSON])
 def test_inbox_count(app: TestClient, accept: str):
@@ -35,20 +37,20 @@
     assert res.json()["count"] == 0
 
     local_id = uuid4().hex
     workflow_id = "TEST_MATT_WORKFLOW"
 
     message_body = f"test{uuid4().hex}".encode()
 
-    resp = send_message(
+    resp = mesh_api_send_message(
         app,
         sender_mailbox_id=sender,
         recipient_mailbox_id=recipient,
-        workflow_id=workflow_id,
         message_data=message_body,
+        workflow_id=workflow_id,
         extra_headers={Headers.Accept: accept, Headers.Mex_LocalID: local_id},
     )
 
     assert resp.status_code == status.HTTP_202_ACCEPTED
 
     res = app.get(
         f"/messageexchange/{recipient}/count",
@@ -74,15 +76,15 @@
     assert response["messages"] == []
 
     page_size = 10
 
     message_ids = []
     for _ in range(page_size * 3):
 
-        resp = send_message(
+        resp = mesh_api_send_message(
             app,
             sender_mailbox_id=sender,
             recipient_mailbox_id=recipient,
             extra_headers={Headers.Accept: accept},
         )
 
         assert resp.status_code == status.HTTP_202_ACCEPTED
@@ -255,7 +257,64 @@
             headers={Headers.Accept: accept, Headers.Authorization: generate_auth_token(sender)},
         )
 
         assert res.status_code == status.HTTP_200_OK
         result = res.json()
         expected = MessageStatus.UNDELIVERABLE.title() if accept == APP_V1_JSON else MessageStatus.UNDELIVERABLE
         assert result["status"] == expected
+
+
+def test_rich_inbox_includes_acknowledged_messages(app: TestClient):
+
+    sender = _CANNED_MAILBOX1
+    recipient = _CANNED_MAILBOX2
+
+    res = app.get(
+        f"/messageexchange/{recipient}/inbox",
+        headers={Headers.Authorization: generate_auth_token(recipient)},
+    )
+    assert res.json()["messages"] == []
+
+    acknowledged_message_id = ""
+    message_ids = []
+    for index in range(5):
+
+        resp = mesh_api_send_message(
+            app,
+            sender_mailbox_id=sender,
+            recipient_mailbox_id=recipient,
+        )
+
+        assert resp.status_code == status.HTTP_202_ACCEPTED
+        result = resp.json()
+        message_id = result["messageID"]
+        assert message_id
+        message_ids.append(message_id)
+
+        if index == 2:
+            ack_response = app.put(
+                f"/messageexchange/{recipient}/inbox/{message_id}/status/acknowledged",
+                headers={Headers.Authorization: generate_auth_token(recipient)},
+            )
+            assert ack_response.status_code == status.HTTP_200_OK
+            assert message_id in ack_response.text
+            acknowledged_message_id = message_id
+
+    # inbox
+    res = app.get(
+        f"/messageexchange/{recipient}/inbox",
+        headers={Headers.Authorization: generate_auth_token(recipient)},
+    )
+    assert res.status_code == status.HTTP_200_OK
+    messages = res.json().get("messages", [])
+    assert len(messages) == 4
+    assert acknowledged_message_id not in messages
+
+    # rich inbox
+    res = app.get(
+        f"/messageexchange/{recipient}/inbox/rich",
+        headers={Headers.Authorization: generate_auth_token(recipient)},
+    )
+    assert res.status_code == status.HTTP_200_OK
+    messages = res.json().get("messages", [])
+    assert len(messages) == 5
+    assert acknowledged_message_id in [m["message_id"] for m in messages]
```

## mesh_sandbox/tests/java_client_tests.py

```diff
@@ -16,15 +16,15 @@
 
 def configure_client(base_uri: str, version: str):
 
     base_dir = ensure_java_client(version)
 
     java_client_config_path = f"{base_dir}/client/meshclient.cfg"
     java_client_jar_path = f"{base_dir}/client/meshClient.jar"
-    java_client_log_config = f"-Dlog4j.configuration=file:{base_dir}/client/log4j.xml"
+    java_client_log_config = f"-Dlog4j2.configurationFile={base_dir}/client/log4j2.xml"
 
     assert os.path.exists(java_client_jar_path), "Could not find java mesh client installation"
 
     # clean the log for this scenario
     pathlib.Path(f"{base_dir}/client/log/mesh.log").unlink(missing_ok=True)
 
     client_config = etree.parse(java_client_config_path)
```

## mesh_sandbox/tests/mesh_client_tests.py

```diff
@@ -2,66 +2,110 @@
 
 import httpx
 import pytest
 from fastapi import status
 from mesh_client import MeshClient
 from requests.models import HTTPError
 
+from mesh_sandbox.tests.docker_tests import (
+    _CANNED_MAILBOX1,
+    _CANNED_MAILBOX2,
+    _PASSWORD,
+    _SHARED_KEY,
+)
+
+
+def _mesh_client_send_message(
+    base_uri: str,
+    sender_mailbox_id: str,
+    recipient_mailbox_id: str,
+    workflow_id: str,
+    payload: bytes,
+):
+    with MeshClient(
+        url=base_uri, mailbox=sender_mailbox_id, password=_PASSWORD, shared_key=_SHARED_KEY, max_chunk_size=100
+    ) as sender:
+        message_id = sender.send_message(recipient_mailbox_id, payload, workflow_id=workflow_id)
+        assert message_id
+        return message_id
+
+
+def _mesh_client_get_inbox_count(base_uri: str, recipient_mailbox_id: str):
+    with MeshClient(
+        url=base_uri, mailbox=recipient_mailbox_id, password=_PASSWORD, shared_key=_SHARED_KEY
+    ) as recipient:
+        message_ids = recipient.list_messages()
+        return len(message_ids)
+
+
+def _mesh_client_track_message_by_message_id(base_uri: str, sender_mailbox_id: str, message_id: str):
+    with MeshClient(
+        url=base_uri, mailbox=sender_mailbox_id, password=_PASSWORD, shared_key=_SHARED_KEY, max_chunk_size=100
+    ) as sender:
+        tracking = sender.track_by_message_id(message_id)
+        assert tracking
+        return tracking
+
 
 def test_app_health(base_uri: str):
 
     with httpx.Client(base_url=base_uri) as client:
         res = client.get("/health")
         assert res.status_code == status.HTTP_200_OK
 
 
-_CANNED_MAILBOX1 = "X26ABC1"
-_CANNED_MAILBOX2 = "X26ABC2"
-_SHARED_KEY = b"TestKey"
-_PASSWORD = "password"
-
-
 def test_handshake(base_uri: str):
 
     with MeshClient(url=base_uri, mailbox=_CANNED_MAILBOX1, password=_PASSWORD, shared_key=_SHARED_KEY) as client:
         res = client.handshake()
         assert res == b"hello"
 
 
 def test_handshake_bad_password(base_uri: str):
 
     with MeshClient(url=base_uri, mailbox=_CANNED_MAILBOX1, password="BAD", shared_key=_SHARED_KEY) as client:
 
         with pytest.raises(HTTPError) as err:
             client.handshake()
-        assert err.value.response.status_code == status.HTTP_400_BAD_REQUEST
+        assert err.value.response.status_code == status.HTTP_403_FORBIDDEN
 
 
 def test_send_receive_chunked_message(base_uri: str):
 
-    sender_mailbox_id = _CANNED_MAILBOX1
-    recipient_mailbox_id = _CANNED_MAILBOX2
     workflow_id = uuid4().hex
+    sent_payload = b"a" * 1000
+    message_id = _mesh_client_send_message(base_uri, _CANNED_MAILBOX1, _CANNED_MAILBOX2, workflow_id, sent_payload)
+    assert _mesh_client_get_inbox_count(base_uri, _CANNED_MAILBOX2) == 1
+
+    with MeshClient(url=base_uri, mailbox=_CANNED_MAILBOX2, password=_PASSWORD, shared_key=_SHARED_KEY) as recipient:
+        message_ids = recipient.list_messages()
+        assert message_ids == [message_id]
+        message = recipient.retrieve_message(message_id)
+        assert message.workflow_id == workflow_id  # pylint: disable=no-member
+        received_payload = message.read()
+        assert received_payload == sent_payload
+
+        message.acknowledge()
+        message_ids = recipient.list_messages()
+        assert message_ids == []
 
-    with MeshClient(
-        url=base_uri, mailbox=sender_mailbox_id, password=_PASSWORD, shared_key=_SHARED_KEY, max_chunk_size=100
-    ) as sender:
-
-        sent_payload = b"a" * 1000
 
-        message_id = sender.send_message(_CANNED_MAILBOX2, sent_payload, workflow_id=workflow_id)
+def test_track_message_by_message_id(base_uri: str):
 
-        assert message_id
-
-        with MeshClient(
-            url=base_uri, mailbox=recipient_mailbox_id, password=_PASSWORD, shared_key=_SHARED_KEY
-        ) as recipient:
-            message_ids = recipient.list_messages()
-            assert message_ids == [message_id]
-            message = recipient.retrieve_message(message_id)
-            assert message.workflow_id == workflow_id  # pylint: disable=no-member
-            received_payload = message.read()
-            assert received_payload == sent_payload
-
-            message.acknowledge()
-            message_ids = recipient.list_messages()
-            assert message_ids == []
+    workflow_id = uuid4().hex
+    sent_payload = b"a" * 1000
+    message_id = _mesh_client_send_message(base_uri, _CANNED_MAILBOX1, _CANNED_MAILBOX2, workflow_id, sent_payload)
+    assert _mesh_client_get_inbox_count(base_uri, _CANNED_MAILBOX2) == 1
+
+    tracking = _mesh_client_track_message_by_message_id(base_uri, _CANNED_MAILBOX1, message_id)
+    assert tracking["messageId"] == message_id
+    assert tracking["status"] == "Accepted"
+    assert tracking["sender"] == _CANNED_MAILBOX1
+    assert tracking["recipient"] == _CANNED_MAILBOX2
+
+    with MeshClient(url=base_uri, mailbox=_CANNED_MAILBOX2, password=_PASSWORD, shared_key=_SHARED_KEY) as recipient:
+        message = recipient.retrieve_message(message_id)
+        message.acknowledge()
+
+    tracking = _mesh_client_track_message_by_message_id(base_uri, _CANNED_MAILBOX1, message_id)
+    assert tracking["messageId"] == message_id
+    assert tracking["status"] == "Acknowledged"
```

## mesh_sandbox/tests/outbox.py

```diff
@@ -1,18 +1,20 @@
 import os.path
 from uuid import uuid4
 
 import pytest
 from fastapi import status
 from fastapi.testclient import TestClient
 
+from mesh_sandbox.tests.mesh_api_helpers import mesh_api_send_message
+
 from ..common import APP_V1_JSON, APP_V2_JSON
 from ..common.constants import Headers
 from ..models.message import MessageStatus
-from .helpers import generate_auth_token, send_message, temp_env_vars
+from .helpers import generate_auth_token, temp_env_vars
 
 _CANNED_MAILBOX1 = "X26ABC1"
 _CANNED_MAILBOX2 = "X26ABC2"
 
 
 @pytest.mark.parametrize("accept", [APP_V1_JSON, APP_V2_JSON])
 def test_memory_send_message_with_local_id(app: TestClient, accept: str):
@@ -29,20 +31,20 @@
     assert list_inbox_response["messages"] == []
 
     local_id = uuid4().hex
     workflow_id = "TEST_MATT_WORKFLOW"
 
     message_body = f"test{uuid4().hex}".encode()
 
-    resp = send_message(
+    resp = mesh_api_send_message(
         app,
         sender_mailbox_id=sender,
         recipient_mailbox_id=recipient,
-        workflow_id=workflow_id,
         message_data=message_body,
+        workflow_id=workflow_id,
         extra_headers={Headers.Accept: accept, Headers.Mex_LocalID: local_id},
     )
 
     assert resp.status_code == status.HTTP_202_ACCEPTED
     result = resp.json()
     message_id = result["messageID"] if accept == APP_V1_JSON else result["message_id"]
     assert message_id
@@ -128,34 +130,34 @@
 
 @pytest.mark.parametrize("accept", [APP_V1_JSON, APP_V2_JSON])
 def test_file_send_message_with_local_id(app: TestClient, accept: str, tmp_path: str):
 
     sender = _CANNED_MAILBOX1
     recipient = _CANNED_MAILBOX2
 
-    with temp_env_vars(STORE_MODE="file", FILE_STORE_DIR=tmp_path):
+    with temp_env_vars(STORE_MODE="file", MAILBOXES_DATA_DIR=tmp_path):
 
         res = app.get(
             f"/messageexchange/{recipient}/inbox",
             headers={Headers.Authorization: generate_auth_token(recipient), Headers.Accept: accept},
         )
 
         list_inbox_response = res.json()
         assert list_inbox_response["messages"] == []
 
         workflow_id = "TEST_MATT_WORKFLOW"
 
         message_body = f"test{uuid4().hex}".encode()
 
-        resp = send_message(
+        resp = mesh_api_send_message(
             app,
             sender_mailbox_id=sender,
             recipient_mailbox_id=recipient,
-            workflow_id=workflow_id,
             message_data=message_body,
+            workflow_id=workflow_id,
             extra_headers={Headers.Accept: accept},
         )
 
         assert resp.status_code == status.HTTP_202_ACCEPTED
         result = resp.json()
         message_id = result["messageID"] if accept == APP_V1_JSON else result["message_id"]
         assert message_id
@@ -204,20 +206,20 @@
     assert list_inbox_response["messages"] == []
 
     chunk_1 = f"test{uuid4().hex}".encode()
     chunk_2 = f"test{uuid4().hex}".encode()
 
     workflow_id = "TEST_WORKFLOW"
 
-    resp = send_message(
+    resp = mesh_api_send_message(
         app,
         sender_mailbox_id=sender,
         recipient_mailbox_id=recipient,
-        workflow_id=workflow_id,
         message_data=chunk_1,
+        workflow_id=workflow_id,
         extra_headers={Headers.Accept: accept, Headers.Mex_Chunk_Range: "1:2"},
     )
 
     assert resp.status_code == status.HTTP_202_ACCEPTED
     result = resp.json()
     message_id = result["messageID"] if accept == APP_V1_JSON else result["message_id"]
     assert message_id
@@ -241,15 +243,15 @@
     res = app.post(
         f"/messageexchange/{sender}/outbox/{message_id}/2",
         headers={
             Headers.Authorization: generate_auth_token(sender),
             Headers.Accept: accept,
             Headers.Mex_Chunk_Range: "2:2",
         },
-        data=chunk_2,
+        content=chunk_2,
     )
     assert res.status_code == status.HTTP_202_ACCEPTED, res.text
 
     res = app.head(
         f"/messageexchange/{recipient}/inbox/{message_id}",
         headers={Headers.Authorization: generate_auth_token(recipient), Headers.Accept: accept},
     )
@@ -311,35 +313,35 @@
 
 @pytest.mark.parametrize("accept", [APP_V1_JSON, APP_V2_JSON])
 def test_file_send_chunked_message(app: TestClient, accept: str, tmp_path: str):  # pylint: disable=too-many-statements
 
     sender = _CANNED_MAILBOX1
     recipient = _CANNED_MAILBOX2
 
-    with temp_env_vars(STORE_MODE="file", FILE_STORE_DIR=tmp_path):
+    with temp_env_vars(STORE_MODE="file", MAILBOXES_DATA_DIR=tmp_path):
 
         res = app.get(
             f"/messageexchange/{recipient}/inbox",
             headers={Headers.Authorization: generate_auth_token(recipient), Headers.Accept: accept},
         )
 
         list_inbox_response = res.json()
         assert list_inbox_response["messages"] == []
 
         chunk_1 = f"test{uuid4().hex}".encode()
         chunk_2 = f"test{uuid4().hex}".encode()
 
         workflow_id = "TEST_WORKFLOW"
 
-        resp = send_message(
+        resp = mesh_api_send_message(
             app,
             sender_mailbox_id=sender,
             recipient_mailbox_id=recipient,
-            workflow_id=workflow_id,
             message_data=chunk_1,
+            workflow_id=workflow_id,
             extra_headers={Headers.Accept: accept, Headers.Mex_Chunk_Range: "1:2"},
         )
 
         assert resp.status_code == status.HTTP_202_ACCEPTED
         result = resp.json()
         message_id = result["messageID"] if accept == APP_V1_JSON else result["message_id"]
         assert message_id
@@ -363,15 +365,15 @@
         res = app.post(
             f"/messageexchange/{sender}/outbox/{message_id}/2",
             headers={
                 Headers.Authorization: generate_auth_token(sender),
                 Headers.Accept: accept,
                 Headers.Mex_Chunk_Range: "2:2",
             },
-            data=chunk_2,
+            content=chunk_2,
         )
         assert res.status_code == status.HTTP_202_ACCEPTED, res.text
 
         res = app.head(
             f"/messageexchange/{recipient}/inbox/{message_id}",
             headers={Headers.Authorization: generate_auth_token(recipient), Headers.Accept: accept},
         )
@@ -460,15 +462,15 @@
     ],
 )
 def test_mex_content_compress_validation(app: TestClient, value: str):
 
     sender = _CANNED_MAILBOX1
     recipient = _CANNED_MAILBOX2
 
-    response = send_message(app, sender, recipient, extra_headers={Headers.Mex_Content_Compress: value})
+    response = mesh_api_send_message(app, sender, recipient, extra_headers={Headers.Mex_Content_Compress: value})
 
     assert response.status_code == status.HTTP_202_ACCEPTED
 
 
 @pytest.mark.parametrize(
     "value",
     [
@@ -498,15 +500,15 @@
     ],
 )
 def test_mex_content_encrypted_validation(app: TestClient, value: str):
 
     sender = _CANNED_MAILBOX1
     recipient = _CANNED_MAILBOX2
 
-    response = send_message(app, sender, recipient, extra_headers={Headers.Mex_Content_Encrypted: value})
+    response = mesh_api_send_message(app, sender, recipient, extra_headers={Headers.Mex_Content_Encrypted: value})
 
     assert response.status_code == status.HTTP_202_ACCEPTED
 
 
 @pytest.mark.parametrize(
     "value",
     [
@@ -536,15 +538,15 @@
     ],
 )
 def test_mex_content_compressed_validation(app: TestClient, value: str):
 
     sender = _CANNED_MAILBOX1
     recipient = _CANNED_MAILBOX2
 
-    response = send_message(app, sender, recipient, extra_headers={Headers.Mex_Content_Compressed: value})
+    response = mesh_api_send_message(app, sender, recipient, extra_headers={Headers.Mex_Content_Compressed: value})
     assert response.status_code == status.HTTP_202_ACCEPTED
 
 
 @pytest.mark.parametrize(
     "mex_content_checksum, expected_response_status",
     [
         ("", status.HTTP_202_ACCEPTED),
@@ -557,22 +559,55 @@
     ],
 )
 def test_mex_content_checksum_validation(app: TestClient, mex_content_checksum: str, expected_response_status: int):
 
     sender = _CANNED_MAILBOX1
     recipient = _CANNED_MAILBOX2
 
-    response = send_message(app, sender, recipient, extra_headers={Headers.Mex_Content_Checksum: mex_content_checksum})
+    response = mesh_api_send_message(
+        app, sender, recipient, extra_headers={Headers.Mex_Content_Checksum: mex_content_checksum}
+    )
 
     assert response.status_code == expected_response_status
 
 
 def test_mex_local_id_validation(app: TestClient):
 
     sender = _CANNED_MAILBOX1
     recipient = _CANNED_MAILBOX2
 
-    response = send_message(
+    response = mesh_api_send_message(
         app, sender, recipient, extra_headers={Headers.Mex_LocalID: "test#TEST", Headers.Mex_WorkflowID: "test TEST"}
     )
 
     assert response.status_code == status.HTTP_202_ACCEPTED
+
+
+@pytest.mark.parametrize("accept", [APP_V1_JSON, APP_V2_JSON])
+def test_checksum_is_returned(app: TestClient, accept: str):
+
+    sender = _CANNED_MAILBOX1
+    recipient = _CANNED_MAILBOX2
+    checksum = uuid4().hex
+
+    send_response = mesh_api_send_message(
+        app,
+        sender,
+        recipient,
+        extra_headers={
+            Headers.Mex_LocalID: "test#TEST",
+            Headers.Mex_WorkflowID: "test TEST",
+            Headers.Accept: accept,
+            Headers.Mex_Content_Checksum: checksum,
+        },
+    )
+    assert send_response.status_code == status.HTTP_202_ACCEPTED
+    send_result = send_response.json()
+    message_id = send_result["messageID"] if accept == APP_V1_JSON else send_result["message_id"]
+    assert message_id
+
+    download_response = app.head(
+        f"/messageexchange/{recipient}/inbox/{message_id}",
+        headers={Headers.Authorization: generate_auth_token(recipient), Headers.Accept: accept},
+    )
+    assert download_response.status_code == status.HTTP_200_OK
+    assert download_response.headers[Headers.Mex_Content_Checksum] == checksum
```

## mesh_sandbox/tests/serialisation.py

```diff
@@ -15,9 +15,9 @@
     )
 
     serialised = serialise_model(message)
 
     assert serialised
 
     deserialised = deserialise_model(serialised, Message)
-
+    assert deserialised
     assert asdict(deserialised) == asdict(message)
```

## mesh_sandbox/views/outbox.py

```diff
@@ -23,15 +23,15 @@
     class Config:
         title = "send_message"
         schema_extra = {"example": {"message_id": "20220228174323222_ABCDEF"}}
 
 
 class UploadChunkV1(BaseModel):
     messageID: str = Field(default=None, description="message identifier, as supplied in the request url")
-    blockID: str = Field(default=None, description="chunk number, as supplied in the request url")
+    blockID: int = Field(default=None, description="chunk number, as supplied in the request url")
 
     class Config:
         title = "upload_chunk"
         schema_extra = {"example": {"messageID": "20220228174323222_ABCDEF", "blockID": 3}}
 
 
 class OutboxMessageV1(RichMessageV1):
@@ -94,14 +94,15 @@
                 message_type=msg.message_type,
                 recipient=msg.recipient.mailbox_id,
                 recipient_name=msg.recipient.mailbox_name,
                 sender=msg.sender.mailbox_id,
                 sender_name=msg.sender.mailbox_name,
                 sent_date=msg.created_timestamp,
                 status=msg.status,
+                status_code=msg.last_event.code,
                 workflow_id=msg.workflow_id,
             ),
             messages,
         )
     )
```

## mesh_sandbox/views/tracking.py

```diff
@@ -40,16 +40,16 @@
 
     sender: Optional[str] = Field(description="sender mailbox identifier")
     senderName: Optional[str] = Field(description="sender mailbox name")
     senderOdsCode: Optional[str] = Field(description="sender ods code")
     senderOrgCode: Optional[str] = Field(description="sender organisation code")
     senderOrgName: Optional[str] = Field(description="sender organisation name")
     senderSmtp: Optional[str] = _EMPTY
-    status: Optional[str] = Field(description="message status e.g. 'accepted' 'acknowledged'")
 
+    status: Optional[str] = Field(description="message status e.g. 'accepted' 'acknowledged'")
     statusCode: Optional[str] = Field(description="status code")
     statusDescription: Optional[str] = Field(description="status description")
     statusEvent: Optional[str] = Field(description="status event")
     statusSuccess: Optional[str] = Field(description="SUCCESS or ERROR if the message accepted")
     statusTimestamp: Optional[str] = Field(description="timestamp of the status change")
 
     subject: Optional[str] = Field(description="message subject")
@@ -105,41 +105,43 @@
 
     failure_date = None
     failure_description = None
     status_code = None
     status_description = None
     status_event = None
     status_timestamp = None
+    status_timestamp_string = None
 
     if error_event:
         if message.message_type == MessageType.DATA:
             failure_date = _format_timestamp(error_event.timestamp)
             failure_description = error_event.description
         else:
             status_code = error_event.code
             status_description = error_event.description
             status_event = error_event.event
-            status_timestamp = _format_timestamp(error_event.timestamp)
+            status_timestamp = error_event.timestamp
+            status_timestamp_string = _format_timestamp(status_timestamp)
 
     if model_version < 2:
 
         return TrackingV1(
             checksum=message.metadata.checksum or _EMPTY,
             chunkCount=message.total_chunks,
-            compressFlag="Y" if message.metadata.is_compressed else _EMPTY,
+            compressFlag="Y" if message.metadata.compressed else _EMPTY,
             contentEncoding=message.metadata.content_encoding,
             downloadTimestamp=_format_timestamp(message.status_timestamp(MessageStatus.ACKNOWLEDGED)),
             dtsId=message.message_id,
             encryptedFlag="Y" if message.metadata.encrypted else _EMPTY,
             expiryTime=_format_timestamp(message.inbox_expiry_timestamp),
             failureDate=failure_date,
             failureDiagnostic=failure_description,
             fileName=message.metadata.file_name or f"{message.message_id}.dat",
             fileSize=message.file_size,
-            isCompressed="Y" if message.metadata.is_compressed else _EMPTY,
+            isCompressed="Y" if message.metadata.compressed else _EMPTY,
             linkedMsgId=error_event.linked_message_id if error_event else None,
             localId=message.metadata.local_id,
             meshRecipientOdsCode=message.recipient.ods_code,
             messageId=message.message_id,
             messageType=(message.message_type or _EMPTY).title(),
             partnerId=message.metadata.partner_id or _EMPTY,
             recipient=message.recipient.mailbox_id,
@@ -152,15 +154,15 @@
             senderOrgCode=message.sender.org_code,
             senderOrgName=message.sender.org_name,
             status=message.status.title(),
             statusCode=status_code,
             statusDescription=status_description,
             statusEvent=status_event,
             statusSuccess=MessageDeliveryStatus.SUCCESS if successful else MessageDeliveryStatus.ERROR,
-            statusTimestamp=status_timestamp,
+            statusTimestamp=status_timestamp_string,
             subject=message.metadata.subject,
             uploadTimestamp=_format_timestamp(message.created_timestamp),
             workflowId=message.workflow_id,
         )
 
     return TrackingV2(
         message_id=message.message_id,
```

## Comparing `mesh_sandbox/store/data/messages.jsonl` & `mesh_sandbox/store/data/mailboxes/X26ABC1/in/UNDELIVERED_MESSAGE.json`

 * *Files 19% similar despite different names*

```diff
@@ -1,146 +1,50 @@
 00000000: 7b22 6d65 7373 6167 655f 6964 223a 2022  {"message_id": "
-00000010: 4348 554e 4b45 445f 4d45 5353 4147 455f  CHUNKED_MESSAGE_
-00000020: 475a 222c 2022 7265 6369 7069 656e 7422  GZ", "recipient"
-00000030: 3a20 7b22 6d61 696c 626f 785f 6964 223a  : {"mailbox_id":
-00000040: 2022 5832 3641 4243 3222 2c20 226d 6169   "X26ABC2", "mai
-00000050: 6c62 6f78 5f6e 616d 6522 3a20 2254 4553  lbox_name": "TES
-00000060: 544d 4232 222c 2022 6f72 675f 636f 6465  TMB2", "org_code
-00000070: 223a 2022 5832 3622 2c20 226f 6473 5f63  ": "X26", "ods_c
-00000080: 6f64 6522 3a20 2258 3236 222c 2022 6269  ode": "X26", "bi
-00000090: 6c6c 696e 675f 656e 7469 7479 223a 2022  lling_entity": "
-000000a0: 456e 676c 616e 6422 7d2c 2022 7365 6e64  England"}, "send
-000000b0: 6572 223a 207b 226d 6169 6c62 6f78 5f69  er": {"mailbox_i
-000000c0: 6422 3a20 2258 3236 4142 4331 222c 2022  d": "X26ABC1", "
-000000d0: 6d61 696c 626f 785f 6e61 6d65 223a 2022  mailbox_name": "
-000000e0: 5445 5354 4d42 3122 2c20 226f 7267 5f63  TESTMB1", "org_c
-000000f0: 6f64 6522 3a20 2258 3236 222c 2022 6f64  ode": "X26", "od
-00000100: 735f 636f 6465 223a 2022 5832 3622 2c20  s_code": "X26", 
-00000110: 2262 696c 6c69 6e67 5f65 6e74 6974 7922  "billing_entity"
-00000120: 3a20 2245 6e67 6c61 6e64 227d 2c20 2265  : "England"}, "e
-00000130: 7665 6e74 7322 3a20 5b7b 2273 7461 7475  vents": [{"statu
-00000140: 7322 3a20 2261 6363 6570 7465 6422 2c20  s": "accepted", 
-00000150: 2274 696d 6573 7461 6d70 223a 2022 3230  "timestamp": "20
-00000160: 3232 2d31 312d 3230 5431 343a 3530 3a31  22-11-20T14:50:1
-00000170: 322e 3932 3332 3039 227d 2c7b 2273 7461  2.923209"},{"sta
-00000180: 7475 7322 3a20 2275 706c 6f61 6469 6e67  tus": "uploading
-00000190: 222c 2022 7469 6d65 7374 616d 7022 3a20  ", "timestamp": 
-000001a0: 2232 3032 322d 3131 2d32 3054 3134 3a35  "2022-11-20T14:5
-000001b0: 303a 3137 2e39 3233 3230 3922 7d5d 2c20  0:17.923209"}], 
-000001c0: 226d 6574 6164 6174 6122 3a20 7b22 636f  "metadata": {"co
-000001d0: 6e74 656e 745f 656e 636f 6469 6e67 223a  ntent_encoding":
-000001e0: 2022 677a 6970 222c 2022 6669 6c65 5f6e   "gzip", "file_n
-000001f0: 616d 6522 3a20 2243 4855 4e4b 4544 5f4d  ame": "CHUNKED_M
-00000200: 4553 5341 4745 5f47 5a2e 6461 7422 2c20  ESSAGE_GZ.dat", 
-00000210: 2265 6e63 7279 7074 6564 223a 2066 616c  "encrypted": fal
-00000220: 7365 2c20 2269 735f 636f 6d70 7265 7373  se, "is_compress
-00000230: 6564 223a 2074 7275 657d 2c20 2277 6f72  ed": true}, "wor
-00000240: 6b66 6c6f 775f 6964 223a 2022 5445 5354  kflow_id": "TEST
-00000250: 5f57 4f52 4b46 4c4f 5722 2c20 226d 6573  _WORKFLOW", "mes
-00000260: 7361 6765 5f74 7970 6522 3a20 2244 4154  sage_type": "DAT
-00000270: 4122 2c20 2274 6f74 616c 5f63 6875 6e6b  A", "total_chunk
-00000280: 7322 3a20 322c 2022 6669 6c65 5f73 697a  s": 2, "file_siz
-00000290: 6522 3a20 3433 392c 2022 696e 626f 785f  e": 439, "inbox_
-000002a0: 6578 7069 7279 5f74 696d 6573 7461 6d70  expiry_timestamp
-000002b0: 223a 2022 3230 3232 2d31 312d 3235 5431  ": "2022-11-25T1
-000002c0: 343a 3530 3a31 372e 3932 3332 3433 222c  4:50:17.923243",
-000002d0: 2022 6c61 7374 5f6d 6f64 6966 6965 6422   "last_modified"
-000002e0: 3a20 2232 3032 322d 3131 2d32 3054 3134  : "2022-11-20T14
-000002f0: 3a35 303a 3137 2e39 3233 3238 3822 2c20  :50:17.923288", 
-00000300: 2263 7265 6174 6564 5f74 696d 6573 7461  "created_timesta
-00000310: 6d70 223a 2022 3230 3232 2d31 312d 3230  mp": "2022-11-20
-00000320: 5431 343a 3530 3a31 372e 3932 3332 3838  T14:50:17.923288
-00000330: 227d 0a7b 226d 6573 7361 6765 5f69 6422  "}.{"message_id"
-00000340: 3a20 2253 494d 504c 455f 4d45 5353 4147  : "SIMPLE_MESSAG
-00000350: 4522 2c20 2272 6563 6970 6965 6e74 223a  E", "recipient":
-00000360: 207b 226d 6169 6c62 6f78 5f69 6422 3a20   {"mailbox_id": 
-00000370: 2258 3236 4142 4331 222c 2022 6d61 696c  "X26ABC1", "mail
-00000380: 626f 785f 6e61 6d65 223a 2022 5445 5354  box_name": "TEST
-00000390: 4d42 3122 2c20 226f 7267 5f63 6f64 6522  MB1", "org_code"
-000003a0: 3a20 2258 3236 222c 2022 6f64 735f 636f  : "X26", "ods_co
-000003b0: 6465 223a 2022 5832 3622 2c20 2262 696c  de": "X26", "bil
-000003c0: 6c69 6e67 5f65 6e74 6974 7922 3a20 2245  ling_entity": "E
-000003d0: 6e67 6c61 6e64 227d 2c20 2273 656e 6465  ngland"}, "sende
-000003e0: 7222 3a20 7b22 6d61 696c 626f 785f 6964  r": {"mailbox_id
-000003f0: 223a 2022 5832 3641 4243 3222 2c20 226d  ": "X26ABC2", "m
-00000400: 6169 6c62 6f78 5f6e 616d 6522 3a20 2254  ailbox_name": "T
-00000410: 4553 544d 4232 222c 2022 6f72 675f 636f  ESTMB2", "org_co
-00000420: 6465 223a 2022 5832 3622 2c20 226f 6473  de": "X26", "ods
-00000430: 5f63 6f64 6522 3a20 2258 3236 222c 2022  _code": "X26", "
-00000440: 6269 6c6c 696e 675f 656e 7469 7479 223a  billing_entity":
-00000450: 2022 456e 676c 616e 6422 7d2c 2022 6576   "England"}, "ev
-00000460: 656e 7473 223a 205b 7b22 7374 6174 7573  ents": [{"status
-00000470: 223a 2022 6163 6365 7074 6564 222c 2022  ": "accepted", "
-00000480: 7469 6d65 7374 616d 7022 3a20 2232 3032  timestamp": "202
-00000490: 322d 3131 2d32 3054 3134 3a35 303a 3132  2-11-20T14:50:12
-000004a0: 2e39 3233 3230 3922 7d5d 2c20 226d 6574  .923209"}], "met
-000004b0: 6164 6174 6122 3a20 7b22 6669 6c65 5f6e  adata": {"file_n
-000004c0: 616d 6522 3a20 2253 494d 504c 455f 4d45  ame": "SIMPLE_ME
-000004d0: 5353 4147 452e 6461 7422 2c20 2265 6e63  SSAGE.dat", "enc
-000004e0: 7279 7074 6564 223a 2066 616c 7365 2c20  rypted": false, 
-000004f0: 2269 735f 636f 6d70 7265 7373 6564 223a  "is_compressed":
-00000500: 2066 616c 7365 7d2c 2022 776f 726b 666c   false}, "workfl
-00000510: 6f77 5f69 6422 3a20 2254 4553 545f 574f  ow_id": "TEST_WO
-00000520: 524b 464c 4f57 222c 2022 6d65 7373 6167  RKFLOW", "messag
-00000530: 655f 7479 7065 223a 2022 4441 5441 222c  e_type": "DATA",
-00000540: 2022 746f 7461 6c5f 6368 756e 6b73 223a   "total_chunks":
-00000550: 2031 2c20 2266 696c 655f 7369 7a65 223a   1, "file_size":
-00000560: 2036 3632 2c20 2269 6e62 6f78 5f65 7870   662, "inbox_exp
-00000570: 6972 795f 7469 6d65 7374 616d 7022 3a20  iry_timestamp": 
-00000580: 2232 3032 322d 3131 2d32 3554 3134 3a35  "2022-11-25T14:5
-00000590: 303a 3137 2e39 3233 3234 3322 2c20 226c  0:17.923243", "l
-000005a0: 6173 745f 6d6f 6469 6669 6564 223a 2022  ast_modified": "
-000005b0: 3230 3232 2d31 312d 3230 5431 343a 3530  2022-11-20T14:50
-000005c0: 3a31 372e 3932 3332 3838 222c 2022 6372  :17.923288", "cr
-000005d0: 6561 7465 645f 7469 6d65 7374 616d 7022  eated_timestamp"
-000005e0: 3a20 2232 3032 322d 3131 2d32 3054 3134  : "2022-11-20T14
-000005f0: 3a35 303a 3137 2e39 3233 3238 3822 7d0a  :50:17.923288"}.
-00000600: 7b22 6d65 7373 6167 655f 6964 223a 2022  {"message_id": "
-00000610: 554e 4445 4c49 5645 5245 445f 4d45 5353  UNDELIVERED_MESS
-00000620: 4147 4522 2c20 2272 6563 6970 6965 6e74  AGE", "recipient
-00000630: 223a 207b 226d 6169 6c62 6f78 5f69 6422  ": {"mailbox_id"
-00000640: 3a20 2258 3236 4142 4331 222c 2022 6d61  : "X26ABC1", "ma
-00000650: 696c 626f 785f 6e61 6d65 223a 2022 5445  ilbox_name": "TE
-00000660: 5354 4d42 3122 2c20 226f 7267 5f63 6f64  STMB1", "org_cod
-00000670: 6522 3a20 2258 3236 222c 2022 6f64 735f  e": "X26", "ods_
-00000680: 636f 6465 223a 2022 5832 3622 2c20 2262  code": "X26", "b
-00000690: 696c 6c69 6e67 5f65 6e74 6974 7922 3a20  illing_entity": 
-000006a0: 2245 6e67 6c61 6e64 227d 2c20 2273 656e  "England"}, "sen
-000006b0: 6465 7222 3a20 7b22 6d61 696c 626f 785f  der": {"mailbox_
-000006c0: 6964 223a 2022 5832 3641 4243 3222 2c20  id": "X26ABC2", 
-000006d0: 226d 6169 6c62 6f78 5f6e 616d 6522 3a20  "mailbox_name": 
-000006e0: 2254 4553 544d 4232 222c 2022 6f72 675f  "TESTMB2", "org_
-000006f0: 636f 6465 223a 2022 5832 3622 2c20 226f  code": "X26", "o
-00000700: 6473 5f63 6f64 6522 3a20 2258 3236 222c  ds_code": "X26",
-00000710: 2022 6269 6c6c 696e 675f 656e 7469 7479   "billing_entity
-00000720: 223a 2022 456e 676c 616e 6422 7d2c 2022  ": "England"}, "
-00000730: 6576 656e 7473 223a 205b 7b22 7374 6174  events": [{"stat
-00000740: 7573 223a 2022 756e 6465 6c69 7665 7261  us": "undelivera
-00000750: 626c 6522 2c20 2274 696d 6573 7461 6d70  ble", "timestamp
-00000760: 223a 2022 3230 3232 2d31 312d 3230 5431  ": "2022-11-20T1
-00000770: 343a 3530 3a31 322e 3932 3332 3039 227d  4:50:12.923209"}
-00000780: 2c7b 2273 7461 7475 7322 3a20 2261 6363  ,{"status": "acc
-00000790: 6570 7465 6422 2c20 2274 696d 6573 7461  epted", "timesta
-000007a0: 6d70 223a 2022 3230 3232 2d31 312d 3135  mp": "2022-11-15
-000007b0: 5431 343a 3530 3a31 322e 3932 3332 3039  T14:50:12.923209
-000007c0: 227d 5d2c 2022 6d65 7461 6461 7461 223a  "}], "metadata":
-000007d0: 207b 2266 696c 655f 6e61 6d65 223a 2022   {"file_name": "
-000007e0: 554e 4445 4c49 5645 5245 445f 4d45 5353  UNDELIVERED_MESS
-000007f0: 4147 452e 6461 7422 2c20 2265 6e63 7279  AGE.dat", "encry
-00000800: 7074 6564 223a 2066 616c 7365 2c20 2269  pted": false, "i
-00000810: 735f 636f 6d70 7265 7373 6564 223a 2066  s_compressed": f
-00000820: 616c 7365 7d2c 2022 776f 726b 666c 6f77  alse}, "workflow
-00000830: 5f69 6422 3a20 2254 4553 545f 574f 524b  _id": "TEST_WORK
-00000840: 464c 4f57 222c 2022 6d65 7373 6167 655f  FLOW", "message_
-00000850: 7479 7065 223a 2022 4441 5441 222c 2022  type": "DATA", "
-00000860: 746f 7461 6c5f 6368 756e 6b73 223a 2031  total_chunks": 1
-00000870: 2c20 2266 696c 655f 7369 7a65 223a 2036  , "file_size": 6
-00000880: 3632 2c20 2269 6e62 6f78 5f65 7870 6972  62, "inbox_expir
-00000890: 795f 7469 6d65 7374 616d 7022 3a20 2232  y_timestamp": "2
-000008a0: 3032 322d 3131 2d32 3054 3134 3a35 303a  022-11-20T14:50:
-000008b0: 3137 2e39 3233 3234 3322 2c20 226c 6173  17.923243", "las
-000008c0: 745f 6d6f 6469 6669 6564 223a 2022 3230  t_modified": "20
-000008d0: 3232 2d31 312d 3135 5431 343a 3530 3a31  22-11-15T14:50:1
-000008e0: 372e 3932 3332 3838 222c 2022 6372 6561  7.923288", "crea
-000008f0: 7465 645f 7469 6d65 7374 616d 7022 3a20  ted_timestamp": 
-00000900: 2232 3032 322d 3131 2d31 3554 3134 3a35  "2022-11-15T14:5
-00000910: 303a 3137 2e39 3233 3238 3822 7d         0:17.923288"}
+00000010: 554e 4445 4c49 5645 5245 445f 4d45 5353  UNDELIVERED_MESS
+00000020: 4147 4522 2c20 2272 6563 6970 6965 6e74  AGE", "recipient
+00000030: 223a 207b 226d 6169 6c62 6f78 5f69 6422  ": {"mailbox_id"
+00000040: 3a20 2258 3236 4142 4331 222c 2022 6d61  : "X26ABC1", "ma
+00000050: 696c 626f 785f 6e61 6d65 223a 2022 5445  ilbox_name": "TE
+00000060: 5354 4d42 3122 2c20 226f 7267 5f63 6f64  STMB1", "org_cod
+00000070: 6522 3a20 2258 3236 222c 2022 6f64 735f  e": "X26", "ods_
+00000080: 636f 6465 223a 2022 5832 3622 2c20 2262  code": "X26", "b
+00000090: 696c 6c69 6e67 5f65 6e74 6974 7922 3a20  illing_entity": 
+000000a0: 2245 6e67 6c61 6e64 227d 2c20 2273 656e  "England"}, "sen
+000000b0: 6465 7222 3a20 7b22 6d61 696c 626f 785f  der": {"mailbox_
+000000c0: 6964 223a 2022 5832 3641 4243 3222 2c20  id": "X26ABC2", 
+000000d0: 226d 6169 6c62 6f78 5f6e 616d 6522 3a20  "mailbox_name": 
+000000e0: 2254 4553 544d 4232 222c 2022 6f72 675f  "TESTMB2", "org_
+000000f0: 636f 6465 223a 2022 5832 3622 2c20 226f  code": "X26", "o
+00000100: 6473 5f63 6f64 6522 3a20 2258 3236 222c  ds_code": "X26",
+00000110: 2022 6269 6c6c 696e 675f 656e 7469 7479   "billing_entity
+00000120: 223a 2022 5761 6c65 7322 7d2c 2022 6576  ": "Wales"}, "ev
+00000130: 656e 7473 223a 205b 7b22 7374 6174 7573  ents": [{"status
+00000140: 223a 2022 756e 6465 6c69 7665 7261 626c  ": "undeliverabl
+00000150: 6522 2c20 2274 696d 6573 7461 6d70 223a  e", "timestamp":
+00000160: 2022 3230 3232 2d31 312d 3230 5431 343a   "2022-11-20T14:
+00000170: 3530 3a31 322e 3932 3332 3039 227d 2c20  50:12.923209"}, 
+00000180: 7b22 7374 6174 7573 223a 2022 6163 6365  {"status": "acce
+00000190: 7074 6564 222c 2022 7469 6d65 7374 616d  pted", "timestam
+000001a0: 7022 3a20 2232 3032 322d 3131 2d31 3554  p": "2022-11-15T
+000001b0: 3134 3a35 303a 3132 2e39 3233 3230 3922  14:50:12.923209"
+000001c0: 7d5d 2c20 226d 6574 6164 6174 6122 3a20  }], "metadata": 
+000001d0: 7b22 6669 6c65 5f6e 616d 6522 3a20 2255  {"file_name": "U
+000001e0: 4e44 454c 4956 4552 4544 5f4d 4553 5341  NDELIVERED_MESSA
+000001f0: 4745 2e64 6174 222c 2022 656e 6372 7970  GE.dat", "encryp
+00000200: 7465 6422 3a20 6661 6c73 652c 2022 6973  ted": false, "is
+00000210: 5f63 6f6d 7072 6573 7365 6422 3a20 6661  _compressed": fa
+00000220: 6c73 657d 2c20 2277 6f72 6b66 6c6f 775f  lse}, "workflow_
+00000230: 6964 223a 2022 5445 5354 5f57 4f52 4b46  id": "TEST_WORKF
+00000240: 4c4f 5722 2c20 226d 6573 7361 6765 5f74  LOW", "message_t
+00000250: 7970 6522 3a20 2244 4154 4122 2c20 2274  ype": "DATA", "t
+00000260: 6f74 616c 5f63 6875 6e6b 7322 3a20 312c  otal_chunks": 1,
+00000270: 2022 6669 6c65 5f73 697a 6522 3a20 3636   "file_size": 66
+00000280: 322c 2022 696e 626f 785f 6578 7069 7279  2, "inbox_expiry
+00000290: 5f74 696d 6573 7461 6d70 223a 2022 3230  _timestamp": "20
+000002a0: 3232 2d31 312d 3230 5431 343a 3530 3a31  22-11-20T14:50:1
+000002b0: 372e 3932 3332 3433 222c 2022 6c61 7374  7.923243", "last
+000002c0: 5f6d 6f64 6966 6965 6422 3a20 2232 3032  _modified": "202
+000002d0: 322d 3131 2d31 3554 3134 3a35 303a 3137  2-11-15T14:50:17
+000002e0: 2e39 3233 3238 3822 2c20 2263 7265 6174  .923288", "creat
+000002f0: 6564 5f74 696d 6573 7461 6d70 223a 2022  ed_timestamp": "
+00000300: 3230 3232 2d31 312d 3135 5431 343a 3530  2022-11-15T14:50
+00000310: 3a31 372e 3932 3332 3838 227d            :17.923288"}
```

## Comparing `mesh_sandbox-0.1.9.dist-info/METADATA` & `mesh_sandbox-1.0.1.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 Metadata-Version: 2.1
 Name: mesh-sandbox
-Version: 0.1.9
+Version: 1.0.1
 Summary: NHSDigital mesh sandbox, a locally testable version of the MESH api
 License: MIT
 Author: spinecore
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cryptography (>=38.0.3,<39.0.0)
-Requires-Dist: fastapi (>=0.75.0,<0.76.0)
+Requires-Dist: cryptography (>=39.0.1,<40.0.0)
+Requires-Dist: fastapi (>=0.94,<0.96)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
+Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: types-python-dateutil (>=2.8.9,<3.0.0)
-Requires-Dist: uvicorn (>=0.15.0,<0.16.0)
+Requires-Dist: uvicorn (>=0.21.0,<0.22.0)
 Description-Content-Type: text/markdown
 
 MESH Sandbox
 ===========
 
 MESH sandbox for local testing of [NHS Digital's MESH API](https://digital.nhs.uk/developer/api-catalogue/message-exchange-for-social-care-and-health-api).
 
 Installation
 ------------
 
-
 Example use
 -----------
 
 pip
 ---
+
 ```bash
 pip install mesh-sandbox
-STORE_MODE=file FILE_STORE_DIR=/tmp/mesh uvicorn mesh_sandbox.api:app --reload --port 8700 --workers=1
+STORE_MODE=file MAILBOXES_DATA_DIR=/tmp/mesh uvicorn mesh_sandbox.api:app --reload --port 8700 --workers=1
 curl http://localhost:8700/health
 ```
 
 docker compose
 --------------
+
 ```yaml
 version: '3.9'
 
 
 services:
 
   mesh_sandbox:
@@ -60,39 +62,47 @@
       interval: 3s
       timeout: 10s
     environment:
       - SHARED_KEY=TestKey
     volumes:
       # mount a different mailboxes.jsonl to pre created mailboxes
       - ./src/mesh_sandbox/store/data/mailboxes.jsonl:/app/mesh_sandbox/store/data/mailboxes.jsonl:ro
+      # the mesh sandbox supports injecting a plugin to support test hooks 
+      # - ./my_test_plugin.py:/app/mesh_sandbox/plugin/my_test_plygin.py:ro
 
 ```
 
 Guidance for contributors
 -------------------------
+
 this project uses
+
 - python 3.9
 - java coretto11
 - poetry > 1.2
 
 Setup
 -----
+
 using asdf
 [install asdf](https://asdf-vm.com/guide/getting-started.html#_3-install-asdf)
 
 get the required plugins
+
 ```bash
 asdf plugin add python
 asdf plugin add java
 asdf plugin add poetry
 ```
 
 install the tools
+
 ```bash
-cd <project_dir>
 asdf install
 ```
 
 install the dependencies
+
 ```bash
 make install
 ```
+
```

## Comparing `mesh_sandbox-0.1.9.dist-info/LICENSE` & `mesh_sandbox-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mesh_sandbox-0.1.9.dist-info/RECORD` & `mesh_sandbox-1.0.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,76 @@
-mesh_sandbox/__init__.py,sha256=XIaxbMbyiP-L3kguR1GhxirFblTXiHR1lMfDVITvHUI,22
-mesh_sandbox/api.py,sha256=Aj_qE5eIXEmLCqvUJdAiuhONgGH_khnooH3JbAhNJoI,3927
-mesh_sandbox/common/__init__.py,sha256=B0eGgN6SGCvNIsalhQOXhFJvxZaE4wJS_ratFOMMwvI,3071
+mesh_sandbox/__init__.py,sha256=d4QHYmS_30j0hPN8NmNPnQ_Z0TphDRbu4MtQj9cT9e8,22
+mesh_sandbox/api.py,sha256=F2KUKENAsSe6NAGG0wzHA2jebGF6mWFgta1q55oqacU,3925
+mesh_sandbox/common/__init__.py,sha256=MwKS4FixADUGgN49MQJI7vW0Wx6mnf9SBOPbgE4RddM,3403
 mesh_sandbox/common/constants.py,sha256=_hnaHDkAQGHWLF7n_WfC5ZHIY5D-fUbOdpSqLusUMNY,6504
 mesh_sandbox/common/exceptions.py,sha256=YQII8w6DQQoKuW0cukEr6PIE9j0rwrqDpCn5lapgmkQ,1481
 mesh_sandbox/common/fernet.py,sha256=f8yygkVnK1cmQLBgcPifoB4PwGpgiOrG8Yk-6OMDy8o,551
 mesh_sandbox/common/handler_helpers.py,sha256=Eg00Tide2mL87EoMFw83fDuxiTL5DgIwxHs2RaJasgE,392
-mesh_sandbox/common/mex_headers.py,sha256=QG4yLmp4b4PyhjDhcKOuE0JJejBbJctmeQj9vXiQ9pE,6065
-mesh_sandbox/conftest.py,sha256=Bd-soyJTgtNAhC_LOH0vFNuE5bK9mPW1uYPglxL2Ox4,2186
-mesh_sandbox/dependencies.py,sha256=f23B71zqz4gAyQHdlw-9bFpWrQk373BG9zZrHY2wnd4,3264
+mesh_sandbox/common/messaging.py,sha256=xZbNpWQLhfjI4wiBG3PpIkEy2WbvwxqaWSR90sSb4hk,14664
+mesh_sandbox/common/mex_headers.py,sha256=Eu-ixdVml2obROXggYyUyiS4QZHUA1JUgF7gO4YYkyg,6088
+mesh_sandbox/conftest.py,sha256=IXrb8Y8Hi4-0ZxDNfTDFI0L1uG1Iz9FBQdNBZtPMsEw,2233
+mesh_sandbox/dependencies.py,sha256=Crl7yEUED-XYl_odMenpvMJoYeIVDROWfvcrfvV85fc,4089
 mesh_sandbox/handlers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mesh_sandbox/handlers/admin.py,sha256=JwPqeN3LHpau0pk7QOEFVrKZ9DV_896j0L_eSZxHIX4,3783
 mesh_sandbox/handlers/handshake.py,sha256=p3_NveSscNBgCdIIJhBza34b0WreqgBxZwI2sw7ZMTk,605
-mesh_sandbox/handlers/inbox.py,sha256=_MBaf5ENou1TsufFknZOIRwJgrwtkhDamPKhCFE2ndY,14597
-mesh_sandbox/handlers/lookup.py,sha256=hqZBjp-Bwg4Jrx71BfKE3ET2AO6x8XXsbl81tLYoshM,1471
-mesh_sandbox/handlers/outbox.py,sha256=FV9BEGqxBkl-cPUUDBDKnZPXAYYBVQwiEy12YYpkqXg,9428
-mesh_sandbox/handlers/tracking.py,sha256=ZSrFVcs7J-aLz8TLCF7JpVZ6ZBBFjQZOmofg2MUolbQ,1918
+mesh_sandbox/handlers/inbox.py,sha256=J20JUX1dHlS2We2UIDQa1MMoVN_QsRoP0tC-3zKAlD8,15450
+mesh_sandbox/handlers/lookup.py,sha256=p_xmnCJi6BoNqRaQjRAGeQthL5EohQfZ_LA1h0QU36Q,1392
+mesh_sandbox/handlers/outbox.py,sha256=XrLOGhw0QqMTfMFevrh-_Z-EyFSEAQLO1BcmbL1bR0Y,10045
+mesh_sandbox/handlers/tracking.py,sha256=nmn5JexFhAvzFmj9C5l0w4sq8sNz3x-mMd3CsGVrEM4,2356
 mesh_sandbox/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mesh_sandbox/models/mailbox.py,sha256=W1b1R1XjhyiCp30LvTLtQVlxagfxXH8eb0XnNj3D4Dw,993
-mesh_sandbox/models/message.py,sha256=br4U7jxJ8Dxkibal9IA9FAK-Yv1sEtkXVQzPDAFXT08,4875
+mesh_sandbox/models/message.py,sha256=ze-IPbCg6XlKZtOL1RWQvMnu04AzrGppwdk2mTyVAfU,4926
 mesh_sandbox/models/workflow.py,sha256=T8A1Q729TOUaz1MOa1Ly8oZs_G4769xMZpTYGF0TlO8,518
+mesh_sandbox/plugins/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mesh_sandbox/routers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mesh_sandbox/routers/admin.py,sha256=pJ9rPF-JDWs1dbVbQVqW8uKQrX3yh4oUxswBOnO5zR8,3852
 mesh_sandbox/routers/handshake.py,sha256=5TVyQ5OrHIe6W3UVpbap-hc5ia669Of6w6F1vgcYjm4,2693
-mesh_sandbox/routers/inbox.py,sha256=Q9HjbM5xuEUaJXrHNBVFdWQfXf26F9sgQMXOPvb2fZg,8573
-mesh_sandbox/routers/inbox_count.py,sha256=_hnBuJJaO-g9F_ddmA6WLaNcYHEAsvyF9TimRVaRBH0,1490
+mesh_sandbox/routers/inbox.py,sha256=EkOmL9pxE6pYPBTzGU1CZJLu80ZR2EnKg9fe7DDMLLQ,8898
+mesh_sandbox/routers/inbox_count.py,sha256=hY88h7dBa6asnvYEP9mmx6CEBw5ZyRO7gz6lHg4Yj3c,1521
 mesh_sandbox/routers/lookup.py,sha256=ViYK80gp9m9nkiZuQf-nimuuIo_nmYKdUBHEuNcKCLY,2115
-mesh_sandbox/routers/outbox.py,sha256=kuMrJPW9XiwLisquAs2rNqaUG0c9VauCudWPLu43inc,4736
+mesh_sandbox/routers/outbox.py,sha256=TtPiPR1zlc3ydnAPTBrTpN_-BIkyr04Km6qkTbwyhsI,4956
 mesh_sandbox/routers/request_logging.py,sha256=gZaOJ_Mp3QPsmrpxXQ0pOzVGNPKd_RAEjpT3Iz1ImVM,1439
-mesh_sandbox/routers/simple.py,sha256=E_95Ae7KGTEz0lAY7ECeyJUJo4AqlJB-qXfRp_GRNnY,1238
 mesh_sandbox/routers/tracking.py,sha256=UVIRkMBGD5pI7vgp8l6cnP5VX8OFRDPNb2JHs9q5w58,2210
 mesh_sandbox/routers/update.py,sha256=a9ttmk3levdDcu-ZF7a5EniR35zRMhty8pG2EyzB1po,409
 mesh_sandbox/store/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mesh_sandbox/store/base.py,sha256=_sS9Q-NKPLpr6Ubr5WpFp7nlZFlt7cv9OV09K40PBKg,5428
-mesh_sandbox/store/canned_store.py,sha256=BNtKpBm1LtgEwZ7A4wme0Uc1_0r3O8M8WVtbShsn0q0,6894
-mesh_sandbox/store/data/chunks.jsonl,sha256=sQ6ZfrCGLMRxeukgbdUYC03ScPg3ofgppG7USNu20ek,2612
-mesh_sandbox/store/data/mailboxes.jsonl,sha256=Gar9pfGb3f3v0Tp8ighV31ZQVy5uKtjofSb8NURgGzs,434
-mesh_sandbox/store/data/messages.jsonl,sha256=MtwyUVows8-nrk4uR88cw7uz_CjjxI7wyD7qc0ppBAg,2333
+mesh_sandbox/store/base.py,sha256=FV93oTeg40ikOaIqcRmDGnigbOEpYexYNqcLyvCaLnA,1983
+mesh_sandbox/store/canned_store.py,sha256=DG5v7Aqy29mCCF9nupqoLIW4m2puLl6iGs2JiNtYnyw,9862
+mesh_sandbox/store/data/mailboxes/X26ABC1/in/SIMPLE_MESSAGE/1,sha256=aqaFLD9HL0hqn0sLIsv-qQqMVyaBmnHx17fu-lgVR9A,662
+mesh_sandbox/store/data/mailboxes/X26ABC1/in/SIMPLE_MESSAGE.json,sha256=lb_vaAXr9hJefOdQ1WXvrBXlIRtzPKzUXt3NT_-b_qA,714
+mesh_sandbox/store/data/mailboxes/X26ABC1/in/UNDELIVERED_MESSAGE/1,sha256=aqaFLD9HL0hqn0sLIsv-qQqMVyaBmnHx17fu-lgVR9A,662
+mesh_sandbox/store/data/mailboxes/X26ABC1/in/UNDELIVERED_MESSAGE.json,sha256=6ipTOkjGUTQyYYny68rI4oTImN07M1KwxKnAy5aZjOc,796
+mesh_sandbox/store/data/mailboxes/X26ABC2/in/CHUNKED_MESSAGE_GZ/1,sha256=osRQ398mz3XvAHSg_V_WSng_4U1WHZ7u4BkehV3-lmo,218
+mesh_sandbox/store/data/mailboxes/X26ABC2/in/CHUNKED_MESSAGE_GZ/2,sha256=uelYjD261gYqGvq1D_wzUs7QcrLlWeIT8nrs-m2u2Yo,221
+mesh_sandbox/store/data/mailboxes/X26ABC2/in/CHUNKED_MESSAGE_GZ.json,sha256=N9T-V-nTrwnJeSefL5aIjXLLlBkjdO86iUmKyxjee0k,817
+mesh_sandbox/store/data/mailboxes.jsonl,sha256=ADXpImNo9UH6rY6T9bqgI-BvnbziFaGwcf_XeJW1bW4,432
 mesh_sandbox/store/data/workflows.jsonl,sha256=RFvycuqVmEkImeXlFD2wjuJFjt6dw581D_raPWstxpU,292
-mesh_sandbox/store/file_store.py,sha256=_sK863McLwLig8cvLnKAjvfEmrboGezhGisRKG1FSo4,1487
-mesh_sandbox/store/memory_store.py,sha256=nPE8l74PcFC7SebZVk6QF3XROndUNhPz7My3MNUad5k,2208
-mesh_sandbox/store/serialisation.py,sha256=nzBMxGkrHOEQ3Q-zmV0W5bwNhs_Q1JlvLsbqONDAtzo,3585
-mesh_sandbox/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mesh_sandbox/tests/docker_tests.py,sha256=nxErB5EDDvewgrgI-YqofsOqo52uYWCPTsk-ggK5axQ,1292
+mesh_sandbox/store/file_store.py,sha256=a4GAhDLjEj2S-zvQxpbMkyDKhC69POCFZln0abH6sUw,2400
+mesh_sandbox/store/memory_store.py,sha256=VJTsPAnwvPAVFTEo-mO2A__lcc7jMnyqiq0JerYmrKY,1643
+mesh_sandbox/store/serialisation.py,sha256=pMYZ704GP74aCDRX9Nu1r4B1XA4BPJXYY-RKLFJJfUg,3615
+mesh_sandbox/test_plugin/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mesh_sandbox/test_plugin/example_plugin.py,sha256=MnNpyyWKziqvOr89LeIxOwqskwHcrSsh_te67SeNJr4,967
+mesh_sandbox/test_plugin/example_plugin.txt,sha256=aUePU6UUVhpxeP37Pdz5Zxyn_nxI6HCY3qtQBo1iUEI,24
+mesh_sandbox/tests/__init__.py,sha256=wPjH0Ka1334a0OR9VMUfeYxsr03JqWjHTBnAH_1SB7I,106
+mesh_sandbox/tests/admin.py,sha256=Y_nzBhqSGPCTjG3EczSHClA-mVALGNBd-iOShoYh8WU,14549
+mesh_sandbox/tests/docker_tests.py,sha256=SJuuquoQA7_fP49--89mrIZmY_4KRO7fiFkOcZeR4AU,1584
 mesh_sandbox/tests/exceptions.py,sha256=j_jKskVzLAYpyu4qNAEY5ahkbk8Uh2Nc_CGpnpdXjnI,740
 mesh_sandbox/tests/handshake.py,sha256=X-fCbwaEAc8cAvvnniCvt4W4DAV9ItPq7tpIpZkfj6M,6259
-mesh_sandbox/tests/helpers.py,sha256=7wMi4YhStWrJhAlsGUjc5kmOQjMDtOZBhnTNyZIQ-o0,7909
-mesh_sandbox/tests/inbox.py,sha256=UdDlhqpCjRurrgexm5S9dnfyaiKnIFyG27jrXnBeU6M,8480
-mesh_sandbox/tests/java_client_tests.py,sha256=oeg1dG83ZBrgy3rb3-lQ26myAxRu-z-u7T-wigIwAhE,6546
+mesh_sandbox/tests/helpers.py,sha256=wRC1t8mj4FKChebvwfcJWpxqK_nmE1NBUHgfCA2rBsk,6885
+mesh_sandbox/tests/inbox.py,sha256=GLqOC6qlivKpp7qEtcGqv_nECkf2MhP4XwRWbIPC_ks,10412
+mesh_sandbox/tests/java_client_tests.py,sha256=NYvNH1LxJc0SmHQ3q6mSvEd6Wuv2r_xMqAXW28sT2Pw,6547
 mesh_sandbox/tests/lookup.py,sha256=wY8x0F415y2um48Lw5kyD4ugMo1vBGKB7cqPdHEaVO4,2768
-mesh_sandbox/tests/mesh_client_tests.py,sha256=7FIsTfKmkEa76DaMleURHL8D0MQr0Ly-drPkMy148dU,2072
-mesh_sandbox/tests/outbox.py,sha256=aFZLKUHxK1fYlBY65r6k45fItn2uo-izJlC9pqT_X5M,18798
-mesh_sandbox/tests/serialisation.py,sha256=zCoP_fAaTCzZ68HpdKQVZLzUJGpbcHTYjHPM2uTtNWQ,640
+mesh_sandbox/tests/mesh_api_helpers.py,sha256=ZedDWMHO88j4Zxw3hsK5vmvivy3UhdzbzHle0g9GJXA,3901
+mesh_sandbox/tests/mesh_client_tests.py,sha256=WL7ht-tT4QLMw73pIbcFMZg7Ehpn5Mi4jcZg5qgEgyw,3947
+mesh_sandbox/tests/messaging_tests.py,sha256=Bup6aJsiJ0xdtg0Ab37ME0VHI6HFJA-0ATmfS88giBI,5006
+mesh_sandbox/tests/outbox.py,sha256=AbQR8vgRy8KAG0RMCU0jYFUXSCPQMrLRJMJTU3PGQhI,20061
+mesh_sandbox/tests/serialisation.py,sha256=kRSMZLDHlX6oRK6c2OCZL0XQoUCKQxqcYXrJWbc9VkA,663
 mesh_sandbox/views/__init__.py,sha256=nZkb6_1S8jz8Xl_AayfwjgEZG0JD2dfulfGxjJ5W9Ec,1237
+mesh_sandbox/views/admin.py,sha256=2YGslfDyC0QKoq3WTGXBicqrOMR9UmQYocP3R0qTbAY,1315
 mesh_sandbox/views/error.py,sha256=9lnUr3P93Vm-nOrBTEuAD6nrSBUvpI6-XqXzILWjgGk,3885
 mesh_sandbox/views/inbox.py,sha256=gnaD9Csx5BqilVRefQQ_tXmeq80lwcLJfepW005GrkU,5662
 mesh_sandbox/views/lookup.py,sha256=HHUqZ-Iy22ysC3qaO8Bl5GBQqf_7IiBbe5acyxqS78M,2775
-mesh_sandbox/views/outbox.py,sha256=gd32ClmFn-_sROCBnsPos9SPrkTn9GpY1e4tQ_jWf1g,4883
-mesh_sandbox/views/tracking.py,sha256=UDEHd0DI_iCS5di8r134nh5lY0c9gClb7mdhXA5nMo4,8827
-mesh_sandbox-0.1.9.dist-info/METADATA,sha256=GlUonPrblasO-yXbNVL6JR6z9ywfngf-hIvnPcrT_zU,2240
-mesh_sandbox-0.1.9.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-mesh_sandbox-0.1.9.dist-info/LICENSE,sha256=usgzIvDUpVX5pYZepJTRXQJqIaz0mdd32GuS5a3PFlY,1051
-mesh_sandbox-0.1.9.dist-info/RECORD,,
+mesh_sandbox/views/outbox.py,sha256=jxYiHylEdpljZ6Wl45Ke3aaH5rEKb-kzUuCNEKDS3So,4932
+mesh_sandbox/views/tracking.py,sha256=1H7Ghcvqkmx__KS1Y-lm105EVx_Z1eJo3oMDh8pzRMQ,8918
+mesh_sandbox-1.0.1.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+mesh_sandbox-1.0.1.dist-info/LICENSE,sha256=usgzIvDUpVX5pYZepJTRXQJqIaz0mdd32GuS5a3PFlY,1051
+mesh_sandbox-1.0.1.dist-info/METADATA,sha256=UUnhdGz3llub6OOLmTV7d2zGBkawfaUyyUzhSR1zMuE,2432
+mesh_sandbox-1.0.1.dist-info/RECORD,,
```

