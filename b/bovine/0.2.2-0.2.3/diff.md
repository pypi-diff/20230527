# Comparing `tmp/bovine-0.2.2.tar.gz` & `tmp/bovine-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine-0.2.2.tar", max compression
+gzip compressed data, was "bovine-0.2.3.tar", max compression
```

## Comparing `bovine-0.2.2.tar` & `bovine-0.2.3.tar`

### file list

```diff
@@ -1,63 +1,112 @@
--rw-r--r--   0        0        0     1363 2023-05-25 18:44:02.786690 bovine-0.2.2/README.md
--rw-r--r--   0        0        0     9265 2023-05-25 09:12:12.412301 bovine-0.2.2/bovine/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 06:22:46.640327 bovine-0.2.2/bovine/activitypub/__init__.py
--rw-r--r--   0        0        0     3505 2023-05-25 18:44:02.786690 bovine-0.2.2/bovine/activitypub/authorization_wrapper.py
--rw-r--r--   0        0        0     2837 2023-05-22 14:17:04.626842 bovine-0.2.2/bovine/activitypub/collection_helper.py
--rw-r--r--   0        0        0      434 2023-05-22 14:17:04.626842 bovine-0.2.2/bovine/activitypub/collection_iterator.py
--rw-r--r--   0        0        0     2757 2023-05-22 14:17:04.626842 bovine-0.2.2/bovine/activitypub/test_actor.py
--rw-r--r--   0        0        0      498 2023-05-22 14:17:04.626842 bovine-0.2.2/bovine/activitypub/test_collection_helper.py
--rw-r--r--   0        0        0     4957 2023-05-22 14:17:04.626842 bovine-0.2.2/bovine/activitystreams/__init__.py
--rw-r--r--   0        0        0     4203 2023-05-22 14:17:04.626842 bovine-0.2.2/bovine/activitystreams/activity_factory.py
--rw-r--r--   0        0        0     4178 2023-05-22 14:17:04.626842 bovine-0.2.2/bovine/activitystreams/object_factory.py
--rw-r--r--   0        0        0     2195 2023-05-22 14:17:04.626842 bovine-0.2.2/bovine/activitystreams/test_activity_factory.py
--rw-r--r--   0        0        0     1442 2023-05-22 14:17:04.626842 bovine-0.2.2/bovine/activitystreams/test_actor.py
--rw-r--r--   0        0        0     1257 2023-05-22 14:17:04.626842 bovine-0.2.2/bovine/activitystreams/test_object_factory.py
--rw-r--r--   0        0        0     1034 2023-05-22 14:17:04.626842 bovine-0.2.2/bovine/activitystreams/test_ordered_collection_builder.py
--rw-r--r--   0        0        0      817 2023-05-22 14:17:04.626842 bovine-0.2.2/bovine/activitystreams/test_ordered_collection_page.py
--rw-r--r--   0        0        0     2354 2023-05-22 14:17:04.630842 bovine-0.2.2/bovine/activitystreams/utils/__init__.py
--rw-r--r--   0        0        0      787 2023-03-30 06:22:46.644327 bovine-0.2.2/bovine/activitystreams/utils/print.py
--rw-r--r--   0        0        0     2266 2023-05-25 09:12:12.360301 bovine-0.2.2/bovine/activitystreams/utils/test_utils.py
--rw-r--r--   0        0        0     3826 2023-05-22 14:17:04.630842 bovine-0.2.2/bovine/clients/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-22 14:17:04.630842 bovine-0.2.2/bovine/clients/bearer.py
--rw-r--r--   0        0        0       91 2023-05-22 14:17:04.630842 bovine-0.2.2/bovine/clients/consts.py
--rw-r--r--   0        0        0     1520 2023-05-22 14:17:04.630842 bovine-0.2.2/bovine/clients/event_source.py
--rw-r--r--   0        0        0      868 2023-05-22 14:17:04.630842 bovine-0.2.2/bovine/clients/lookup_account.py
--rw-r--r--   0        0        0     3001 2023-05-22 14:17:04.630842 bovine-0.2.2/bovine/clients/moo_auth.py
--rw-r--r--   0        0        0      948 2023-05-22 14:17:04.630842 bovine-0.2.2/bovine/clients/nodeinfo.py
--rw-r--r--   0        0        0     1150 2023-05-22 14:17:04.630842 bovine-0.2.2/bovine/clients/signed_http.py
--rw-r--r--   0        0        0     3278 2023-05-22 14:17:04.630842 bovine-0.2.2/bovine/clients/signed_http_methods.py
--rw-r--r--   0        0        0      651 2023-05-25 18:44:02.786690 bovine-0.2.2/bovine/clients/test_event_source.py
--rw-r--r--   0        0        0     1149 2023-05-25 09:12:12.320301 bovine-0.2.2/bovine/clients/test_lookup_account.py
--rw-r--r--   0        0        0      319 2023-05-22 14:17:04.630842 bovine-0.2.2/bovine/clients/test_nodeinfo.py
--rw-r--r--   0        0        0     1153 2023-05-22 14:17:04.630842 bovine-0.2.2/bovine/clients/test_signed_http.py
--rw-r--r--   0        0        0      522 2023-05-22 14:17:04.630842 bovine-0.2.2/bovine/clients/test_signed_http_client.py
--rw-r--r--   0        0        0     4141 2023-05-25 09:12:12.368301 bovine-0.2.2/bovine/crypto/__init__.py
--rw-r--r--   0        0        0     2664 2023-05-25 09:12:12.348301 bovine-0.2.2/bovine/crypto/helper.py
--rw-r--r--   0        0        0     2112 2023-05-22 14:17:04.634842 bovine-0.2.2/bovine/crypto/http_signature.py
--rw-r--r--   0        0        0     2942 2023-05-22 14:17:04.634842 bovine-0.2.2/bovine/crypto/signature_checker.py
--rw-r--r--   0        0        0     1266 2023-05-22 14:17:04.634842 bovine-0.2.2/bovine/crypto/signature_parser.py
--rw-r--r--   0        0        0     2199 2023-05-22 14:17:04.634842 bovine-0.2.2/bovine/crypto/test.py
--rw-r--r--   0        0        0     4995 2023-05-25 09:12:12.372301 bovine-0.2.2/bovine/crypto/test_crypto.py
--rw-r--r--   0        0        0      896 2023-05-25 09:12:12.316301 bovine-0.2.2/bovine/crypto/test_helper.py
--rw-r--r--   0        0        0     5081 2023-05-22 14:17:04.634842 bovine-0.2.2/bovine/crypto/test_http_signature.py
--rw-r--r--   0        0        0     1207 2023-05-22 14:17:04.634842 bovine-0.2.2/bovine/crypto/test_signature_parser.py
--rw-r--r--   0        0        0      302 2023-05-22 14:17:04.634842 bovine-0.2.2/bovine/ed25519_key.py
--rw-r--r--   0        0        0     3342 2023-05-22 14:17:04.634842 bovine-0.2.2/bovine/jsonld.py
--rw-r--r--   0        0        0      864 2023-05-22 14:17:04.634842 bovine-0.2.2/bovine/msg.py
--rw-r--r--   0        0        0     1670 2023-05-25 18:44:02.786690 bovine-0.2.2/bovine/repl.py
--rw-r--r--   0        0        0      178 2023-03-30 06:22:46.648327 bovine-0.2.2/bovine/test_bovine_client.py
--rw-r--r--   0        0        0     5250 2023-05-22 14:17:04.634842 bovine-0.2.2/bovine/test_jsonld.py
--rw-r--r--   0        0        0      282 2023-03-30 06:22:46.648327 bovine-0.2.2/bovine/test_types.py
--rw-r--r--   0        0        0     2397 2023-05-22 14:17:04.634842 bovine-0.2.2/bovine/types.py
--rw-r--r--   0        0        0      856 2023-05-22 14:17:04.634842 bovine-0.2.2/bovine/utils/__init__.py
--rw-r--r--   0        0        0      519 2023-03-30 06:22:46.648327 bovine-0.2.2/bovine/utils/date.py
--rw-r--r--   0        0        0     1313 2023-05-22 14:17:04.634842 bovine-0.2.2/bovine/utils/msg/__init__.py
--rw-r--r--   0        0        0      599 2023-05-22 14:17:04.634842 bovine-0.2.2/bovine/utils/msg/test_validation.py
--rw-r--r--   0        0        0      261 2023-05-22 14:17:04.634842 bovine-0.2.2/bovine/utils/msg/validation.py
--rw-r--r--   0        0        0     4736 2023-05-22 14:17:04.634842 bovine-0.2.2/bovine/utils/pyld_requests.py
--rw-r--r--   0        0        0      761 2023-05-22 14:17:04.634842 bovine-0.2.2/bovine/utils/test_date.py
--rw-r--r--   0        0        0      452 2023-05-22 14:17:04.634842 bovine-0.2.2/bovine/utils/test_parse.py
--rw-r--r--   0        0        0      368 2023-05-22 14:17:04.634842 bovine-0.2.2/bovine/utils/test_webfinger.py
--rw-r--r--   0        0        0     1291 2023-05-25 18:44:02.786690 bovine-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2485 1970-01-01 00:00:00.000000 bovine-0.2.2/setup.py
--rw-r--r--   0        0        0     2425 1970-01-01 00:00:00.000000 bovine-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1363 2023-05-27 18:25:16.679233 bovine-0.2.3/README.md
+-rw-r--r--   0        0        0     9485 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 18:25:16.807235 bovine-0.2.3/bovine/activitypub/__init__.py
+-rw-r--r--   0        0        0      173 2023-05-27 18:26:22.763913 bovine-0.2.3/bovine/activitypub/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3741 2023-05-27 18:26:22.763913 bovine-0.2.3/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc
+-rw-r--r--   0        0        0     2475 2023-05-27 18:26:23.275918 bovine-0.2.3/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc
+-rw-r--r--   0        0        0      922 2023-05-27 18:26:23.399919 bovine-0.2.3/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc
+-rw-r--r--   0        0        0     3638 2023-05-27 18:26:23.731922 bovine-0.2.3/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1212 2023-05-27 18:26:23.751923 bovine-0.2.3/bovine/activitypub/__pycache__/test_collection_helper.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3505 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitypub/authorization_wrapper.py
+-rw-r--r--   0        0        0     2542 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitypub/collection_helper.py
+-rw-r--r--   0        0        0      434 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitypub/collection_iterator.py
+-rw-r--r--   0        0        0     2757 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitypub/test_actor.py
+-rw-r--r--   0        0        0      498 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitypub/test_collection_helper.py
+-rw-r--r--   0        0        0     4957 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/__init__.py
+-rw-r--r--   0        0        0     4645 2023-05-27 18:26:23.391919 bovine-0.2.3/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4269 2023-05-27 18:26:23.395919 bovine-0.2.3/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc
+-rw-r--r--   0        0        0     4028 2023-05-27 18:26:23.395919 bovine-0.2.3/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc
+-rw-r--r--   0        0        0     4584 2023-05-27 18:26:23.759923 bovine-0.2.3/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3327 2023-05-27 18:26:23.767923 bovine-0.2.3/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3113 2023-05-27 18:26:23.775923 bovine-0.2.3/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1951 2023-05-27 18:26:23.779923 bovine-0.2.3/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1386 2023-05-27 18:26:23.779923 bovine-0.2.3/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     4203 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/activity_factory.py
+-rw-r--r--   0        0        0     4178 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/object_factory.py
+-rw-r--r--   0        0        0     2195 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/test_activity_factory.py
+-rw-r--r--   0        0        0     1442 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/test_actor.py
+-rw-r--r--   0        0        0     1257 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/test_object_factory.py
+-rw-r--r--   0        0        0     1034 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/test_ordered_collection_builder.py
+-rw-r--r--   0        0        0      817 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/test_ordered_collection_page.py
+-rw-r--r--   0        0        0     2354 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/utils/__init__.py
+-rw-r--r--   0        0        0     2836 2023-05-27 18:26:23.395919 bovine-0.2.3/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      972 2023-05-27 18:26:23.399919 bovine-0.2.3/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc
+-rw-r--r--   0        0        0     4763 2023-05-27 18:26:23.791923 bovine-0.2.3/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      865 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/utils/print.py
+-rw-r--r--   0        0        0     2266 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/activitystreams/utils/test_utils.py
+-rw-r--r--   0        0        0     3968 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/__init__.py
+-rw-r--r--   0        0        0     4002 2023-05-27 18:26:23.055916 bovine-0.2.3/bovine/clients/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1916 2023-05-27 18:26:23.059916 bovine-0.2.3/bovine/clients/__pycache__/bearer.cpython-310.pyc
+-rw-r--r--   0        0        0      268 2023-05-27 18:26:23.055916 bovine-0.2.3/bovine/clients/__pycache__/consts.cpython-310.pyc
+-rw-r--r--   0        0        0     1719 2023-05-27 18:26:23.107916 bovine-0.2.3/bovine/clients/__pycache__/event_source.cpython-310.pyc
+-rw-r--r--   0        0        0     1084 2023-05-27 18:26:23.055916 bovine-0.2.3/bovine/clients/__pycache__/lookup_account.cpython-310.pyc
+-rw-r--r--   0        0        0     2534 2023-05-27 18:26:23.111916 bovine-0.2.3/bovine/clients/__pycache__/moo_auth.cpython-310.pyc
+-rw-r--r--   0        0        0     1237 2023-05-27 18:26:23.059916 bovine-0.2.3/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc
+-rw-r--r--   0        0        0     1529 2023-05-27 18:26:23.275918 bovine-0.2.3/bovine/clients/__pycache__/signed_http.cpython-310.pyc
+-rw-r--r--   0        0        0     2479 2023-05-27 18:26:23.275918 bovine-0.2.3/bovine/clients/__pycache__/signed_http_methods.cpython-310.pyc
+-rw-r--r--   0        0        0     1507 2023-05-27 18:26:23.795923 bovine-0.2.3/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2844 2023-05-27 18:26:23.799923 bovine-0.2.3/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1217 2023-05-27 18:26:23.803923 bovine-0.2.3/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2102 2023-05-27 18:26:23.807923 bovine-0.2.3/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      814 2023-05-27 18:26:23.807923 bovine-0.2.3/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1794 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/bearer.py
+-rw-r--r--   0        0        0       91 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/consts.py
+-rw-r--r--   0        0        0     1520 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/event_source.py
+-rw-r--r--   0        0        0      868 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/lookup_account.py
+-rw-r--r--   0        0        0     3001 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/moo_auth.py
+-rw-r--r--   0        0        0      948 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/nodeinfo.py
+-rw-r--r--   0        0        0     1150 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/signed_http.py
+-rw-r--r--   0        0        0     3278 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/signed_http_methods.py
+-rw-r--r--   0        0        0      651 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/test_event_source.py
+-rw-r--r--   0        0        0     1505 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/test_lookup_account.py
+-rw-r--r--   0        0        0      319 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/test_nodeinfo.py
+-rw-r--r--   0        0        0     1153 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/test_signed_http.py
+-rw-r--r--   0        0        0      522 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/clients/test_signed_http_client.py
+-rw-r--r--   0        0        0     4141 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/__init__.py
+-rw-r--r--   0        0        0     3749 2023-05-27 18:26:23.111916 bovine-0.2.3/bovine/crypto/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2863 2023-05-27 18:26:23.271918 bovine-0.2.3/bovine/crypto/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     2909 2023-05-27 18:26:23.271918 bovine-0.2.3/bovine/crypto/__pycache__/http_signature.cpython-310.pyc
+-rw-r--r--   0        0        0     2257 2023-05-27 18:26:23.271918 bovine-0.2.3/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc
+-rw-r--r--   0        0        0     1784 2023-05-27 18:26:23.271918 bovine-0.2.3/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc
+-rw-r--r--   0        0        0     2363 2023-05-27 18:26:23.747923 bovine-0.2.3/bovine/crypto/__pycache__/test.cpython-310.pyc
+-rw-r--r--   0        0        0     5821 2023-05-27 18:26:23.815923 bovine-0.2.3/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2742 2023-05-27 18:26:23.819923 bovine-0.2.3/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     7454 2023-05-27 18:26:23.831924 bovine-0.2.3/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2674 2023-05-27 18:26:23.839924 bovine-0.2.3/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2664 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/helper.py
+-rw-r--r--   0        0        0     2112 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/http_signature.py
+-rw-r--r--   0        0        0     2942 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/signature_checker.py
+-rw-r--r--   0        0        0     1266 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/signature_parser.py
+-rw-r--r--   0        0        0     2199 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/test.py
+-rw-r--r--   0        0        0     4995 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/test_crypto.py
+-rw-r--r--   0        0        0      896 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/test_helper.py
+-rw-r--r--   0        0        0     5081 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/test_http_signature.py
+-rw-r--r--   0        0        0     1207 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/crypto/test_signature_parser.py
+-rw-r--r--   0        0        0      302 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/ed25519_key.py
+-rw-r--r--   0        0        0     3342 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/jsonld.py
+-rw-r--r--   0        0        0      864 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/msg.py
+-rw-r--r--   0        0        0     3256 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/repl.py
+-rw-r--r--   0        0        0      178 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/test_bovine_client.py
+-rw-r--r--   0        0        0     5250 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/test_jsonld.py
+-rw-r--r--   0        0        0      282 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/test_types.py
+-rw-r--r--   0        0        0     2397 2023-05-27 18:25:16.679233 bovine-0.2.3/bovine/types.py
+-rw-r--r--   0        0        0      856 2023-05-27 18:25:16.683233 bovine-0.2.3/bovine/utils/__init__.py
+-rw-r--r--   0        0        0     1120 2023-05-27 18:26:23.055916 bovine-0.2.3/bovine/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      877 2023-05-27 18:26:23.059916 bovine-0.2.3/bovine/utils/__pycache__/date.cpython-310.pyc
+-rw-r--r--   0        0        0     3240 2023-05-27 18:26:23.715922 bovine-0.2.3/bovine/utils/__pycache__/pyld_requests.cpython-310.pyc
+-rw-r--r--   0        0        0     3465 2023-05-27 18:26:23.847924 bovine-0.2.3/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1662 2023-05-27 18:26:23.851924 bovine-0.2.3/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1625 2023-05-27 18:26:23.851924 bovine-0.2.3/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      519 2023-05-27 18:25:16.683233 bovine-0.2.3/bovine/utils/date.py
+-rw-r--r--   0        0        0     1432 2023-05-27 18:25:16.683233 bovine-0.2.3/bovine/utils/msg/__init__.py
+-rw-r--r--   0        0        0     1934 2023-05-27 18:26:23.855924 bovine-0.2.3/bovine/utils/msg/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1967 2023-05-27 18:26:23.859924 bovine-0.2.3/bovine/utils/msg/__pycache__/test_validation.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      659 2023-05-27 18:26:23.855924 bovine-0.2.3/bovine/utils/msg/__pycache__/validation.cpython-310.pyc
+-rw-r--r--   0        0        0      599 2023-05-27 18:25:16.683233 bovine-0.2.3/bovine/utils/msg/test_validation.py
+-rw-r--r--   0        0        0      261 2023-05-27 18:25:16.683233 bovine-0.2.3/bovine/utils/msg/validation.py
+-rw-r--r--   0        0        0     4736 2023-05-27 18:25:16.683233 bovine-0.2.3/bovine/utils/pyld_requests.py
+-rw-r--r--   0        0        0      761 2023-05-27 18:25:16.683233 bovine-0.2.3/bovine/utils/test_date.py
+-rw-r--r--   0        0        0      452 2023-05-27 18:25:16.683233 bovine-0.2.3/bovine/utils/test_parse.py
+-rw-r--r--   0        0        0      368 2023-05-27 18:25:16.683233 bovine-0.2.3/bovine/utils/test_webfinger.py
+-rw-r--r--   0        0        0     1405 2023-05-27 18:25:16.683233 bovine-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2524 1970-01-01 00:00:00.000000 bovine-0.2.3/PKG-INFO
```

### Comparing `bovine-0.2.2/README.md` & `bovine-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/__init__.py` & `bovine-0.2.3/bovine/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,20 @@
     def __init__(self, config):
         super().__init__()
 
         self.actor_id = None
         self.information: Optional[dict] = None
         self._activity_factory = None
         self._object_factory = None
+
+        if "domain" in config and "host" not in config:
+            config["host"] = config["domain"]
+        if "secret" in config and "private_key" not in config:
+            config["private_key"] = config["secret"]
+
         self.config = config
 
     async def get(self, target):
         assert self.client
 
         response = await self.client.get(target)
         response.raise_for_status()
```

### Comparing `bovine-0.2.2/bovine/activitypub/authorization_wrapper.py` & `bovine-0.2.3/bovine/activitypub/authorization_wrapper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/activitypub/collection_helper.py` & `bovine-0.2.3/bovine/activitypub/collection_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,22 +56,14 @@
 
         response = await self.actor.get(self.basic_information["first"])
 
         self.items = response["orderedItems"]
         self.next_items = response["next"]
         self.item_index = 0
 
-    async def summary(self):
-        print()
-        print(f"Items loaded {len(self.items)}")
-        print()
-        for idx, item in enumerate(self.items):
-            obj = await self.get_element(item)
-            print(f"{idx:4}: {obj.get('type'):10}: {short_version_of_object(obj)[:80]}")
-
     async def get_element(self, element):
         if not isinstance(element, str):
             return element
 
         if element in self.element_cache:
             return self.element_cache[element]
```

### Comparing `bovine-0.2.2/bovine/activitypub/test_actor.py` & `bovine-0.2.3/bovine/activitypub/test_actor.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/activitystreams/__init__.py` & `bovine-0.2.3/bovine/activitystreams/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/activitystreams/activity_factory.py` & `bovine-0.2.3/bovine/activitystreams/activity_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/activitystreams/object_factory.py` & `bovine-0.2.3/bovine/activitystreams/object_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/activitystreams/test_activity_factory.py` & `bovine-0.2.3/bovine/activitystreams/test_activity_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/activitystreams/test_actor.py` & `bovine-0.2.3/bovine/activitystreams/test_actor.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/activitystreams/test_object_factory.py` & `bovine-0.2.3/bovine/activitystreams/test_object_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/activitystreams/test_ordered_collection_builder.py` & `bovine-0.2.3/bovine/activitystreams/test_ordered_collection_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/activitystreams/test_ordered_collection_page.py` & `bovine-0.2.3/bovine/activitystreams/test_ordered_collection_page.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/activitystreams/utils/__init__.py` & `bovine-0.2.3/bovine/activitystreams/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/activitystreams/utils/print.py` & `bovine-0.2.3/bovine/activitystreams/utils/print.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,27 +5,27 @@
     if "type" in activity:
         print(f"Type: {activity['type']:10}, Id: {activity.get('id')}")
         print()
 
     if "object" in activity and isinstance(activity["object"], dict):
         obj = activity["object"]
 
-        print_object(obj)
+        print_object(obj, indent="    ")
 
 
-def print_object(obj):
+def print_object(obj, indent=""):
     if "type" in obj:
-        print(f"Type: {obj['type']}")
+        print(f"{indent}Type: {obj['type']}")
         print()
 
     if "name" in obj and obj["name"]:
-        print(f"Name: {obj['name']}")
+        print(f"{indent}Name: {obj['name']}")
         print()
     if "summary" in obj and obj["summary"]:
-        print("Summary")
-        print(bleach.clean(obj["summary"], tags=[], strip=True))
+        print(f"{indent}Summary")
+        print(indent + bleach.clean(obj["summary"], tags=[], strip=True))
         print()
 
     if "content" in obj and obj["content"]:
-        print("Content")
-        print(bleach.clean(obj["content"], tags=[], strip=True))
+        print(f"{indent}Content")
+        print(indent + bleach.clean(obj["content"], tags=[], strip=True))
         print()
```

### Comparing `bovine-0.2.2/bovine/activitystreams/utils/test_utils.py` & `bovine-0.2.3/bovine/activitystreams/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/clients/__init__.py` & `bovine-0.2.3/bovine/clients/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,15 +62,18 @@
     """
     if domain is None:
         if uri.startswith("acct:"):
             _, domain = parse_fediverse_handle(uri.removeprefix("acct:"))
         else:
             raise ValueError(f"For the uri {uri} a domain must be specified")
 
-    webfinger_url = f"https://{domain}/.well-known/webfinger"
+    if domain.startswith("http://") or domain.startswith("https://"):
+        webfinger_url = f"{domain}/.well-known/webfinger"
+    else:
+        webfinger_url = f"https://{domain}/.well-known/webfinger"
     params = {"resource": uri}
 
     result = await lookup_with_webfinger(session, webfinger_url, params)
 
     return result, not uri.startswith("acct:")
```

### Comparing `bovine-0.2.2/bovine/clients/bearer.py` & `bovine-0.2.3/bovine/clients/bearer.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/clients/event_source.py` & `bovine-0.2.3/bovine/clients/event_source.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/clients/lookup_account.py` & `bovine-0.2.3/bovine/clients/lookup_account.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/clients/moo_auth.py` & `bovine-0.2.3/bovine/clients/moo_auth.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/clients/nodeinfo.py` & `bovine-0.2.3/bovine/clients/nodeinfo.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/clients/signed_http.py` & `bovine-0.2.3/bovine/clients/signed_http.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/clients/signed_http_methods.py` & `bovine-0.2.3/bovine/clients/signed_http_methods.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/clients/test_event_source.py` & `bovine-0.2.3/bovine/clients/test_event_source.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/clients/test_lookup_account.py` & `bovine-0.2.3/bovine/clients/test_lookup_account.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,14 +14,24 @@
     did_helge = "did:key:z6MkujdZ216eYz55vz8X5HetqeJXj9ddn5ZHZUsBpRX4wfnL"
     async with aiohttp.ClientSession() as session:
         result = await lookup_did_with_webfinger(session, "mymath.rocks", did_helge)
 
     assert result.startswith("https://mymath.rocks/")
 
 
+async def test_lookup_did_with_webfinger_with_protocol():
+    did_helge = "did:key:z6MkujdZ216eYz55vz8X5HetqeJXj9ddn5ZHZUsBpRX4wfnL"
+    async with aiohttp.ClientSession() as session:
+        result = await lookup_did_with_webfinger(
+            session, "https://mymath.rocks", did_helge
+        )
+
+    assert result.startswith("https://mymath.rocks/")
+
+
 async def test_lookup_with_dns():
     domain = "mymath.rocks"
 
     async with aiohttp.ClientSession() as session:
         result = await lookup_with_dns(session, domain)
 
     assert (
```

### Comparing `bovine-0.2.2/bovine/clients/test_signed_http.py` & `bovine-0.2.3/bovine/clients/test_signed_http.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/clients/test_signed_http_client.py` & `bovine-0.2.3/bovine/clients/test_signed_http_client.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/crypto/__init__.py` & `bovine-0.2.3/bovine/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/crypto/helper.py` & `bovine-0.2.3/bovine/crypto/helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/crypto/http_signature.py` & `bovine-0.2.3/bovine/crypto/http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/crypto/signature_checker.py` & `bovine-0.2.3/bovine/crypto/signature_checker.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/crypto/signature_parser.py` & `bovine-0.2.3/bovine/crypto/signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/crypto/test.py` & `bovine-0.2.3/bovine/crypto/test.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/crypto/test_crypto.py` & `bovine-0.2.3/bovine/crypto/test_crypto.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/crypto/test_helper.py` & `bovine-0.2.3/bovine/crypto/test_helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/crypto/test_http_signature.py` & `bovine-0.2.3/bovine/crypto/test_http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/crypto/test_signature_parser.py` & `bovine-0.2.3/bovine/crypto/test_signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/jsonld.py` & `bovine-0.2.3/bovine/jsonld.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/msg.py` & `bovine-0.2.3/bovine/msg.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/test_jsonld.py` & `bovine-0.2.3/bovine/test_jsonld.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/types.py` & `bovine-0.2.3/bovine/types.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/utils/__init__.py` & `bovine-0.2.3/bovine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/utils/date.py` & `bovine-0.2.3/bovine/utils/date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/utils/msg/__init__.py` & `bovine-0.2.3/bovine/utils/msg/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,20 @@
     if "@" in to:
         return await lookup_account_with_webfinger(session, to)
 
     return to
 
 
 async def process(args):
-    async with BovineClient({"host": args.host, "private_key": args.secret}) as client:
+    if args.host and args.secret:
+        client = BovineClient({"host": args.host, "private_key": args.secret})
+    else:
+        client = BovineClient.from_file("bovine_user.toml")
+
+    async with client:
         recipients = [await resolve(client.session, to) for to in args.to]
 
         mentions = [
             await client.object_factory.mention_for_actor_uri(recipient)
             for recipient in recipients
         ]
         mentions = [m.build() for m in mentions]
```

### Comparing `bovine-0.2.2/bovine/utils/msg/test_validation.py` & `bovine-0.2.3/bovine/utils/msg/test_validation.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/utils/pyld_requests.py` & `bovine-0.2.3/bovine/utils/pyld_requests.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/bovine/utils/test_date.py` & `bovine-0.2.3/bovine/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.2/pyproject.toml` & `bovine-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bovine"
-version = "0.2.2"
+version = "0.2.3"
 description = "Core functionality of bovine needed to build fediverse applications"
 authors = ["Helge <helge.krueger@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bovine" }]
 repository = "https://codeberg.org/bovine/bovine"
 documentation = "https://bovine.readthedocs.io/en/latest/"
@@ -12,32 +12,36 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "^3.8.3"
 cryptography = "^39.0.0"
 python-dateutil = "^2.8.2"
 tomli = "^2.0.1"
 multiformats = "^0.2.1"
-bleach = "^6.0.0"
 aiodns = "^3.0.0"
 requests-cache = "^0.9.8"
 requests = "^2.30.0"
 pyld = "^2.0.3"
+ptpython = { version = "^3.0.23", optional = true }
+bleach = { version = "^6.0.0", optional = true}
+
+[tool.poetry.extras]
+
+repl = ["ptpython", "bleach"]
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "^4.0.0"
 behave = "^1.2.6"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 mypy = "^0.991"
 types-python-dateutil = "^2.8.19.6"
 black = "*"
-ptpython = "^3.0.23"
 rich = "^13.3.2"
 types-bleach = "^6.0.0.2"
 reload = "^0.9"
 quart = "^0.18.3"
 rdflib = "^6.3.2"
 ruff = "^0.0.261"
```

### Comparing `bovine-0.2.2/PKG-INFO` & `bovine-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: bovine
-Version: 0.2.2
+Version: 0.2.3
 Summary: Core functionality of bovine needed to build fediverse applications
 Home-page: https://codeberg.org/bovine/bovine
 License: MIT
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: repl
 Requires-Dist: aiodns (>=3.0.0,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
-Requires-Dist: bleach (>=6.0.0,<7.0.0)
+Requires-Dist: bleach (>=6.0.0,<7.0.0) ; extra == "repl"
 Requires-Dist: cryptography (>=39.0.0,<40.0.0)
 Requires-Dist: multiformats (>=0.2.1,<0.3.0)
+Requires-Dist: ptpython (>=3.0.23,<4.0.0) ; extra == "repl"
 Requires-Dist: pyld (>=2.0.3,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Requires-Dist: requests-cache (>=0.9.8,<0.10.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Project-URL: Documentation, https://bovine.readthedocs.io/en/latest/
 Project-URL: Repository, https://codeberg.org/bovine/bovine
```

