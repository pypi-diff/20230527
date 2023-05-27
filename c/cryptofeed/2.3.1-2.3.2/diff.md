# Comparing `tmp/cryptofeed-2.3.1.tar.gz` & `tmp/cryptofeed-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptofeed-2.3.1.tar", last modified: Mon Oct 31 14:48:00 2022, max compression
+gzip compressed data, was "cryptofeed-2.3.2.tar", last modified: Sat May 27 19:27:02 2023, max compression
```

## Comparing `cryptofeed-2.3.1.tar` & `cryptofeed-2.3.2.tar`

### file list

```diff
@@ -1,118 +1,113 @@
-drwxr-xr-x   0 bryant     (501) staff       (20)        0 2022-10-31 14:48:00.744417 cryptofeed-2.3.1/
--rw-r--r--   0 bryant     (501) staff       (20)     1167 2022-04-10 19:37:09.000000 cryptofeed-2.3.1/AUTHORS.md
--rw-r--r--   0 bryant     (501) staff       (20)    41931 2022-10-31 14:46:03.000000 cryptofeed-2.3.1/CHANGES.md
--rw-r--r--   0 bryant     (501) staff       (20)     2396 2021-10-02 22:22:30.000000 cryptofeed-2.3.1/INSTALL.md
--rw-r--r--   0 bryant     (501) staff       (20)     2096 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/LICENSE
--rw-r--r--   0 bryant     (501) staff       (20)       85 2021-09-11 19:21:39.000000 cryptofeed-2.3.1/MANIFEST.in
--rw-r--r--   0 bryant     (501) staff       (20)    53718 2022-10-31 14:48:00.744116 cryptofeed-2.3.1/PKG-INFO
--rw-r--r--   0 bryant     (501) staff       (20)     8051 2022-04-15 00:03:44.000000 cryptofeed-2.3.1/README.md
-drwxr-xr-x   0 bryant     (501) staff       (20)        0 2022-10-31 14:48:00.678424 cryptofeed-2.3.1/cryptofeed/
--rw-r--r--   0 bryant     (501) staff       (20)      202 2022-01-16 21:05:34.000000 cryptofeed-2.3.1/cryptofeed/__init__.py
-drwxr-xr-x   0 bryant     (501) staff       (20)        0 2022-10-31 14:48:00.692473 cryptofeed-2.3.1/cryptofeed/backends/
--rw-r--r--   0 bryant     (501) staff       (20)        0 2021-12-19 14:46:21.000000 cryptofeed-2.3.1/cryptofeed/backends/__init__.py
--rw-r--r--   0 bryant     (501) staff       (20)     1287 2022-01-16 21:05:34.000000 cryptofeed-2.3.1/cryptofeed/backends/_util.py
--rw-r--r--   0 bryant     (501) staff       (20)     5831 2022-01-16 21:05:34.000000 cryptofeed-2.3.1/cryptofeed/backends/aggregate.py
--rw-r--r--   0 bryant     (501) staff       (20)     3120 2022-10-10 19:59:46.000000 cryptofeed-2.3.1/cryptofeed/backends/arctic.py
--rw-r--r--   0 bryant     (501) staff       (20)     4222 2022-04-15 00:03:44.000000 cryptofeed-2.3.1/cryptofeed/backends/backend.py
--rw-r--r--   0 bryant     (501) staff       (20)     5242 2022-08-23 23:08:14.000000 cryptofeed-2.3.1/cryptofeed/backends/gcppubsub.py
--rw-r--r--   0 bryant     (501) staff       (20)      885 2022-04-15 00:03:44.000000 cryptofeed-2.3.1/cryptofeed/backends/http.py
--rw-r--r--   0 bryant     (501) staff       (20)     5420 2022-08-21 20:56:07.000000 cryptofeed-2.3.1/cryptofeed/backends/influxdb.py
--rw-r--r--   0 bryant     (501) staff       (20)     3244 2022-08-21 20:56:07.000000 cryptofeed-2.3.1/cryptofeed/backends/kafka.py
--rw-r--r--   0 bryant     (501) staff       (20)     3161 2022-08-21 20:56:07.000000 cryptofeed-2.3.1/cryptofeed/backends/mongo.py
--rw-r--r--   0 bryant     (501) staff       (20)     9389 2022-04-15 00:03:44.000000 cryptofeed-2.3.1/cryptofeed/backends/postgres.py
--rw-r--r--   0 bryant     (501) staff       (20)     4680 2022-08-21 20:56:07.000000 cryptofeed-2.3.1/cryptofeed/backends/quest.py
--rw-r--r--   0 bryant     (501) staff       (20)     3664 2022-08-21 20:56:07.000000 cryptofeed-2.3.1/cryptofeed/backends/rabbitmq.py
--rw-r--r--   0 bryant     (501) staff       (20)     5602 2022-10-10 19:31:27.000000 cryptofeed-2.3.1/cryptofeed/backends/redis.py
--rw-r--r--   0 bryant     (501) staff       (20)     4741 2022-08-21 20:56:07.000000 cryptofeed-2.3.1/cryptofeed/backends/socket.py
--rw-r--r--   0 bryant     (501) staff       (20)     2531 2022-08-23 23:08:14.000000 cryptofeed-2.3.1/cryptofeed/backends/zmq.py
--rw-r--r--   0 bryant     (501) staff       (20)     1249 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/callback.py
--rw-r--r--   0 bryant     (501) staff       (20)     2646 2022-01-23 16:30:50.000000 cryptofeed-2.3.1/cryptofeed/config.py
--rw-r--r--   0 bryant     (501) staff       (20)    15224 2022-10-31 14:46:29.000000 cryptofeed-2.3.1/cryptofeed/connection.py
--rw-r--r--   0 bryant     (501) staff       (20)     5916 2022-02-27 22:57:27.000000 cryptofeed-2.3.1/cryptofeed/connection_handler.py
--rw-r--r--   0 bryant     (501) staff       (20)     5265 2022-09-04 17:23:19.000000 cryptofeed-2.3.1/cryptofeed/defines.py
--rw-r--r--   0 bryant     (501) staff       (20)      719 2022-01-16 21:05:34.000000 cryptofeed-2.3.1/cryptofeed/exceptions.py
--rw-r--r--   0 bryant     (501) staff       (20)    12341 2022-05-22 18:35:21.000000 cryptofeed-2.3.1/cryptofeed/exchange.py
-drwxr-xr-x   0 bryant     (501) staff       (20)        0 2022-10-31 14:48:00.728497 cryptofeed-2.3.1/cryptofeed/exchanges/
--rw-r--r--   0 bryant     (501) staff       (20)     2666 2022-05-17 11:41:30.000000 cryptofeed-2.3.1/cryptofeed/exchanges/__init__.py
--rw-r--r--   0 bryant     (501) staff       (20)     5591 2022-04-25 23:31:05.000000 cryptofeed-2.3.1/cryptofeed/exchanges/ascendex.py
--rw-r--r--   0 bryant     (501) staff       (20)     1980 2022-04-25 23:31:05.000000 cryptofeed-2.3.1/cryptofeed/exchanges/ascendex_futures.py
--rw-r--r--   0 bryant     (501) staff       (20)    16122 2022-02-19 16:34:14.000000 cryptofeed-2.3.1/cryptofeed/exchanges/bequant.py
--rw-r--r--   0 bryant     (501) staff       (20)    22733 2022-04-25 23:31:05.000000 cryptofeed-2.3.1/cryptofeed/exchanges/binance.py
--rw-r--r--   0 bryant     (501) staff       (20)     9902 2022-04-25 23:31:05.000000 cryptofeed-2.3.1/cryptofeed/exchanges/binance_delivery.py
--rw-r--r--   0 bryant     (501) staff       (20)    11806 2022-08-21 20:56:07.000000 cryptofeed-2.3.1/cryptofeed/exchanges/binance_futures.py
--rw-r--r--   0 bryant     (501) staff       (20)      739 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/binance_us.py
--rw-r--r--   0 bryant     (501) staff       (20)    22344 2022-05-22 18:17:57.000000 cryptofeed-2.3.1/cryptofeed/exchanges/bitdotcom.py
--rw-r--r--   0 bryant     (501) staff       (20)    16570 2022-05-22 18:17:57.000000 cryptofeed-2.3.1/cryptofeed/exchanges/bitfinex.py
--rw-r--r--   0 bryant     (501) staff       (20)     7993 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/bitflyer.py
--rw-r--r--   0 bryant     (501) staff       (20)    21491 2022-08-21 20:56:07.000000 cryptofeed-2.3.1/cryptofeed/exchanges/bitget.py
--rw-r--r--   0 bryant     (501) staff       (20)     5841 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/bithumb.py
--rw-r--r--   0 bryant     (501) staff       (20)    30788 2022-04-25 23:31:05.000000 cryptofeed-2.3.1/cryptofeed/exchanges/bitmex.py
--rw-r--r--   0 bryant     (501) staff       (20)     7321 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/bitstamp.py
--rw-r--r--   0 bryant     (501) staff       (20)    17154 2022-09-04 17:26:54.000000 cryptofeed-2.3.1/cryptofeed/exchanges/bittrex.py
--rw-r--r--   0 bryant     (501) staff       (20)     6956 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/blockchain.py
--rw-r--r--   0 bryant     (501) staff       (20)    22718 2022-08-21 20:56:07.000000 cryptofeed-2.3.1/cryptofeed/exchanges/bybit.py
--rw-r--r--   0 bryant     (501) staff       (20)    16245 2022-10-10 20:07:18.000000 cryptofeed-2.3.1/cryptofeed/exchanges/coinbase.py
--rw-r--r--   0 bryant     (501) staff       (20)     8786 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/cryptodotcom.py
--rw-r--r--   0 bryant     (501) staff       (20)     8017 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/delta.py
--rw-r--r--   0 bryant     (501) staff       (20)    24345 2022-09-04 17:22:43.000000 cryptofeed-2.3.1/cryptofeed/exchanges/deribit.py
--rw-r--r--   0 bryant     (501) staff       (20)     6483 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/dydx.py
--rw-r--r--   0 bryant     (501) staff       (20)     5505 2022-01-05 23:52:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/exx.py
--rw-r--r--   0 bryant     (501) staff       (20)     8193 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/fmfw.py
--rw-r--r--   0 bryant     (501) staff       (20)    17475 2022-08-21 20:56:07.000000 cryptofeed-2.3.1/cryptofeed/exchanges/ftx.py
--rw-r--r--   0 bryant     (501) staff       (20)      886 2022-05-17 11:41:30.000000 cryptofeed-2.3.1/cryptofeed/exchanges/ftx_tr.py
--rw-r--r--   0 bryant     (501) staff       (20)      880 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/ftx_us.py
--rw-r--r--   0 bryant     (501) staff       (20)    10407 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/gateio.py
--rw-r--r--   0 bryant     (501) staff       (20)     8372 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/gemini.py
--rw-r--r--   0 bryant     (501) staff       (20)     1378 2022-02-19 16:35:19.000000 cryptofeed-2.3.1/cryptofeed/exchanges/hitbtc.py
--rw-r--r--   0 bryant     (501) staff       (20)     7756 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/huobi.py
--rw-r--r--   0 bryant     (501) staff       (20)     5589 2022-02-20 22:33:45.000000 cryptofeed-2.3.1/cryptofeed/exchanges/huobi_dm.py
--rw-r--r--   0 bryant     (501) staff       (20)     4409 2022-02-19 16:37:29.000000 cryptofeed-2.3.1/cryptofeed/exchanges/huobi_swap.py
--rw-r--r--   0 bryant     (501) staff       (20)     9751 2022-04-10 19:37:09.000000 cryptofeed-2.3.1/cryptofeed/exchanges/independent_reserve.py
--rw-r--r--   0 bryant     (501) staff       (20)     9312 2022-05-22 18:17:57.000000 cryptofeed-2.3.1/cryptofeed/exchanges/kraken.py
--rw-r--r--   0 bryant     (501) staff       (20)     9243 2022-04-25 23:31:05.000000 cryptofeed-2.3.1/cryptofeed/exchanges/kraken_futures.py
--rw-r--r--   0 bryant     (501) staff       (20)    11683 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/kucoin.py
-drwxr-xr-x   0 bryant     (501) staff       (20)        0 2022-10-31 14:48:00.740109 cryptofeed-2.3.1/cryptofeed/exchanges/mixins/
--rw-r--r--   0 bryant     (501) staff       (20)        0 2021-12-08 22:54:58.000000 cryptofeed-2.3.1/cryptofeed/exchanges/mixins/__init__.py
--rw-r--r--   0 bryant     (501) staff       (20)     8671 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/mixins/binance_rest.py
--rw-r--r--   0 bryant     (501) staff       (20)    10240 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/mixins/bitfinex_rest.py
--rw-r--r--   0 bryant     (501) staff       (20)     4162 2022-02-20 18:32:11.000000 cryptofeed-2.3.1/cryptofeed/exchanges/mixins/bitmex_rest.py
--rw-r--r--   0 bryant     (501) staff       (20)     1813 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/mixins/bitstamp_rest.py
--rw-r--r--   0 bryant     (501) staff       (20)    14467 2022-04-10 19:37:09.000000 cryptofeed-2.3.1/cryptofeed/exchanges/mixins/coinbase_rest.py
--rw-r--r--   0 bryant     (501) staff       (20)     3096 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/mixins/deribit_rest.py
--rw-r--r--   0 bryant     (501) staff       (20)     2061 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/mixins/dydx_rest.py
--rw-r--r--   0 bryant     (501) staff       (20)     5352 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/mixins/ftx_rest.py
--rw-r--r--   0 bryant     (501) staff       (20)      713 2022-05-17 11:41:30.000000 cryptofeed-2.3.1/cryptofeed/exchanges/mixins/ftx_rest_tr.py
--rw-r--r--   0 bryant     (501) staff       (20)      710 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/mixins/ftx_rest_us.py
--rw-r--r--   0 bryant     (501) staff       (20)     7481 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/mixins/gemini_rest.py
--rw-r--r--   0 bryant     (501) staff       (20)    12055 2022-02-20 18:32:10.000000 cryptofeed-2.3.1/cryptofeed/exchanges/mixins/kraken_rest.py
--rw-r--r--   0 bryant     (501) staff       (20)     1880 2022-04-03 20:46:21.000000 cryptofeed-2.3.1/cryptofeed/exchanges/mixins/okx_rest.py
--rw-r--r--   0 bryant     (501) staff       (20)     3821 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/mixins/upbit_rest.py
--rw-r--r--   0 bryant     (501) staff       (20)     6963 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/okcoin.py
--rw-r--r--   0 bryant     (501) staff       (20)    21567 2022-10-22 22:06:48.000000 cryptofeed-2.3.1/cryptofeed/exchanges/okx.py
--rw-r--r--   0 bryant     (501) staff       (20)    26970 2022-10-22 20:52:47.000000 cryptofeed-2.3.1/cryptofeed/exchanges/phemex.py
--rw-r--r--   0 bryant     (501) staff       (20)     4877 2022-08-23 23:08:14.000000 cryptofeed-2.3.1/cryptofeed/exchanges/poloniex.py
--rw-r--r--   0 bryant     (501) staff       (20)     6680 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/probit.py
--rw-r--r--   0 bryant     (501) staff       (20)     7883 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/exchanges/upbit.py
--rw-r--r--   0 bryant     (501) staff       (20)    15191 2022-08-21 20:56:07.000000 cryptofeed-2.3.1/cryptofeed/feed.py
--rw-r--r--   0 bryant     (501) staff       (20)     7845 2022-01-16 21:05:34.000000 cryptofeed-2.3.1/cryptofeed/feedhandler.py
--rw-r--r--   0 bryant     (501) staff       (20)      701 2022-01-16 21:05:34.000000 cryptofeed-2.3.1/cryptofeed/log.py
--rw-r--r--   0 bryant     (501) staff       (20)     1728 2022-01-16 21:05:34.000000 cryptofeed-2.3.1/cryptofeed/nbbo.py
--rw-r--r--   0 bryant     (501) staff       (20)     7792 2022-08-23 23:08:14.000000 cryptofeed-2.3.1/cryptofeed/raw_data_collection.py
--rw-r--r--   0 bryant     (501) staff       (20)     5114 2022-09-04 17:16:39.000000 cryptofeed-2.3.1/cryptofeed/symbols.py
--rw-r--r--   0 bryant     (501) staff       (20)  2231593 2022-10-31 14:48:00.000000 cryptofeed-2.3.1/cryptofeed/types.c
--rw-r--r--   0 bryant     (501) staff       (20)    35344 2022-04-10 19:37:09.000000 cryptofeed-2.3.1/cryptofeed/types.pyx
-drwxr-xr-x   0 bryant     (501) staff       (20)        0 2022-10-31 14:48:00.743197 cryptofeed-2.3.1/cryptofeed/util/
--rw-r--r--   0 bryant     (501) staff       (20)        0 2021-12-08 22:54:58.000000 cryptofeed-2.3.1/cryptofeed/util/__init__.py
--rw-r--r--   0 bryant     (501) staff       (20)      922 2022-01-16 21:05:34.000000 cryptofeed-2.3.1/cryptofeed/util/book.py
--rw-r--r--   0 bryant     (501) staff       (20)     1372 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/util/perf.py
--rw-r--r--   0 bryant     (501) staff       (20)      712 2021-12-08 22:54:58.000000 cryptofeed-2.3.1/cryptofeed/util/split.py
--rw-r--r--   0 bryant     (501) staff       (20)      911 2022-01-16 21:05:35.000000 cryptofeed-2.3.1/cryptofeed/util/time.py
-drwxr-xr-x   0 bryant     (501) staff       (20)        0 2022-10-31 14:48:00.680600 cryptofeed-2.3.1/cryptofeed.egg-info/
--rw-r--r--   0 bryant     (501) staff       (20)    53718 2022-10-31 14:48:00.000000 cryptofeed-2.3.1/cryptofeed.egg-info/PKG-INFO
--rw-r--r--   0 bryant     (501) staff       (20)     3318 2022-10-31 14:48:00.000000 cryptofeed-2.3.1/cryptofeed.egg-info/SOURCES.txt
--rw-r--r--   0 bryant     (501) staff       (20)        1 2022-10-31 14:48:00.000000 cryptofeed-2.3.1/cryptofeed.egg-info/dependency_links.txt
--rw-r--r--   0 bryant     (501) staff       (20)      514 2022-10-31 14:48:00.000000 cryptofeed-2.3.1/cryptofeed.egg-info/requires.txt
--rw-r--r--   0 bryant     (501) staff       (20)       11 2022-10-31 14:48:00.000000 cryptofeed-2.3.1/cryptofeed.egg-info/top_level.txt
--rw-r--r--   0 bryant     (501) staff       (20)      667 2021-09-04 13:59:37.000000 cryptofeed-2.3.1/pyproject.toml
--rw-r--r--   0 bryant     (501) staff       (20)       38 2022-10-31 14:48:00.744530 cryptofeed-2.3.1/setup.cfg
--rw-r--r--   0 bryant     (501) staff       (20)     4050 2022-10-22 20:52:47.000000 cryptofeed-2.3.1/setup.py
+drwxr-xr-x   0 bryant     (501) staff       (20)        0 2023-05-27 19:27:02.749748 cryptofeed-2.3.2/
+-rw-r--r--   0 bryant     (501) staff       (20)     1167 2022-04-10 19:37:09.000000 cryptofeed-2.3.2/AUTHORS.md
+-rw-r--r--   0 bryant     (501) staff       (20)    42489 2023-05-27 19:14:33.000000 cryptofeed-2.3.2/CHANGES.md
+-rw-r--r--   0 bryant     (501) staff       (20)     2396 2021-10-02 22:22:30.000000 cryptofeed-2.3.2/INSTALL.md
+-rw-r--r--   0 bryant     (501) staff       (20)     2096 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/LICENSE
+-rw-r--r--   0 bryant     (501) staff       (20)       85 2021-09-11 19:21:39.000000 cryptofeed-2.3.2/MANIFEST.in
+-rw-r--r--   0 bryant     (501) staff       (20)    54211 2023-05-27 19:27:02.749186 cryptofeed-2.3.2/PKG-INFO
+-rw-r--r--   0 bryant     (501) staff       (20)     7997 2023-01-08 21:38:14.000000 cryptofeed-2.3.2/README.md
+drwxr-xr-x   0 bryant     (501) staff       (20)        0 2023-05-27 19:27:02.710443 cryptofeed-2.3.2/cryptofeed/
+-rw-r--r--   0 bryant     (501) staff       (20)      202 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/__init__.py
+drwxr-xr-x   0 bryant     (501) staff       (20)        0 2023-05-27 19:27:02.719449 cryptofeed-2.3.2/cryptofeed/backends/
+-rw-r--r--   0 bryant     (501) staff       (20)        0 2021-12-19 14:46:21.000000 cryptofeed-2.3.2/cryptofeed/backends/__init__.py
+-rw-r--r--   0 bryant     (501) staff       (20)     1287 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/backends/_util.py
+-rw-r--r--   0 bryant     (501) staff       (20)     6037 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/backends/aggregate.py
+-rw-r--r--   0 bryant     (501) staff       (20)     3120 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/backends/arctic.py
+-rw-r--r--   0 bryant     (501) staff       (20)     4222 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/backends/backend.py
+-rw-r--r--   0 bryant     (501) staff       (20)     5242 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/backends/gcppubsub.py
+-rw-r--r--   0 bryant     (501) staff       (20)      885 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/backends/http.py
+-rw-r--r--   0 bryant     (501) staff       (20)     5420 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/backends/influxdb.py
+-rw-r--r--   0 bryant     (501) staff       (20)     6304 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/backends/kafka.py
+-rw-r--r--   0 bryant     (501) staff       (20)     3161 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/backends/mongo.py
+-rw-r--r--   0 bryant     (501) staff       (20)     9389 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/backends/postgres.py
+-rw-r--r--   0 bryant     (501) staff       (20)     4680 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/backends/quest.py
+-rw-r--r--   0 bryant     (501) staff       (20)     3664 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/backends/rabbitmq.py
+-rw-r--r--   0 bryant     (501) staff       (20)     6469 2023-02-16 01:19:51.000000 cryptofeed-2.3.2/cryptofeed/backends/redis.py
+-rw-r--r--   0 bryant     (501) staff       (20)     4737 2023-05-27 19:14:02.000000 cryptofeed-2.3.2/cryptofeed/backends/socket.py
+-rw-r--r--   0 bryant     (501) staff       (20)     2531 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/backends/zmq.py
+-rw-r--r--   0 bryant     (501) staff       (20)     1249 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/callback.py
+-rw-r--r--   0 bryant     (501) staff       (20)     2646 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/config.py
+-rw-r--r--   0 bryant     (501) staff       (20)    15224 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/connection.py
+-rw-r--r--   0 bryant     (501) staff       (20)     5916 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/connection_handler.py
+-rw-r--r--   0 bryant     (501) staff       (20)     5243 2023-05-27 19:14:02.000000 cryptofeed-2.3.2/cryptofeed/defines.py
+-rw-r--r--   0 bryant     (501) staff       (20)      719 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exceptions.py
+-rw-r--r--   0 bryant     (501) staff       (20)    12341 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchange.py
+drwxr-xr-x   0 bryant     (501) staff       (20)        0 2023-05-27 19:27:02.740260 cryptofeed-2.3.2/cryptofeed/exchanges/
+-rw-r--r--   0 bryant     (501) staff       (20)     2582 2023-05-27 19:14:02.000000 cryptofeed-2.3.2/cryptofeed/exchanges/__init__.py
+-rw-r--r--   0 bryant     (501) staff       (20)     5591 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/ascendex.py
+-rw-r--r--   0 bryant     (501) staff       (20)     1980 2022-04-25 23:31:05.000000 cryptofeed-2.3.2/cryptofeed/exchanges/ascendex_futures.py
+-rw-r--r--   0 bryant     (501) staff       (20)    16122 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/bequant.py
+-rw-r--r--   0 bryant     (501) staff       (20)    22733 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/binance.py
+-rw-r--r--   0 bryant     (501) staff       (20)     9902 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/binance_delivery.py
+-rw-r--r--   0 bryant     (501) staff       (20)    11806 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/binance_futures.py
+-rw-r--r--   0 bryant     (501) staff       (20)      743 2023-05-27 19:14:02.000000 cryptofeed-2.3.2/cryptofeed/exchanges/binance_tr.py
+-rw-r--r--   0 bryant     (501) staff       (20)      739 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/binance_us.py
+-rw-r--r--   0 bryant     (501) staff       (20)    22344 2022-05-22 18:17:57.000000 cryptofeed-2.3.2/cryptofeed/exchanges/bitdotcom.py
+-rw-r--r--   0 bryant     (501) staff       (20)    16570 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/bitfinex.py
+-rw-r--r--   0 bryant     (501) staff       (20)     7993 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/bitflyer.py
+-rw-r--r--   0 bryant     (501) staff       (20)    21491 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/bitget.py
+-rw-r--r--   0 bryant     (501) staff       (20)     5841 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/bithumb.py
+-rw-r--r--   0 bryant     (501) staff       (20)    30788 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/bitmex.py
+-rw-r--r--   0 bryant     (501) staff       (20)     7321 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/bitstamp.py
+-rw-r--r--   0 bryant     (501) staff       (20)    17154 2022-09-04 17:26:54.000000 cryptofeed-2.3.2/cryptofeed/exchanges/bittrex.py
+-rw-r--r--   0 bryant     (501) staff       (20)     6956 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/blockchain.py
+-rw-r--r--   0 bryant     (501) staff       (20)    22718 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/bybit.py
+-rw-r--r--   0 bryant     (501) staff       (20)    16583 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/coinbase.py
+-rw-r--r--   0 bryant     (501) staff       (20)     8786 2023-05-27 19:14:02.000000 cryptofeed-2.3.2/cryptofeed/exchanges/cryptodotcom.py
+-rw-r--r--   0 bryant     (501) staff       (20)     8017 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/delta.py
+-rw-r--r--   0 bryant     (501) staff       (20)    24345 2022-09-04 17:22:43.000000 cryptofeed-2.3.2/cryptofeed/exchanges/deribit.py
+-rw-r--r--   0 bryant     (501) staff       (20)     6483 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/dydx.py
+-rw-r--r--   0 bryant     (501) staff       (20)     5505 2022-01-05 23:52:35.000000 cryptofeed-2.3.2/cryptofeed/exchanges/exx.py
+-rw-r--r--   0 bryant     (501) staff       (20)     8193 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/fmfw.py
+-rw-r--r--   0 bryant     (501) staff       (20)    10407 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/gateio.py
+-rw-r--r--   0 bryant     (501) staff       (20)     8372 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/gemini.py
+-rw-r--r--   0 bryant     (501) staff       (20)     1378 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/hitbtc.py
+-rw-r--r--   0 bryant     (501) staff       (20)     7756 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/huobi.py
+-rw-r--r--   0 bryant     (501) staff       (20)     5589 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/huobi_dm.py
+-rw-r--r--   0 bryant     (501) staff       (20)     4409 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/huobi_swap.py
+-rw-r--r--   0 bryant     (501) staff       (20)     9751 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/independent_reserve.py
+-rw-r--r--   0 bryant     (501) staff       (20)     9312 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/kraken.py
+-rw-r--r--   0 bryant     (501) staff       (20)     9258 2023-05-27 19:14:02.000000 cryptofeed-2.3.2/cryptofeed/exchanges/kraken_futures.py
+-rw-r--r--   0 bryant     (501) staff       (20)    11683 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/kucoin.py
+drwxr-xr-x   0 bryant     (501) staff       (20)        0 2023-05-27 19:27:02.746248 cryptofeed-2.3.2/cryptofeed/exchanges/mixins/
+-rw-r--r--   0 bryant     (501) staff       (20)        0 2021-12-08 22:54:58.000000 cryptofeed-2.3.2/cryptofeed/exchanges/mixins/__init__.py
+-rw-r--r--   0 bryant     (501) staff       (20)     8803 2023-05-27 19:14:02.000000 cryptofeed-2.3.2/cryptofeed/exchanges/mixins/binance_rest.py
+-rw-r--r--   0 bryant     (501) staff       (20)    10240 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/mixins/bitfinex_rest.py
+-rw-r--r--   0 bryant     (501) staff       (20)     4162 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/mixins/bitmex_rest.py
+-rw-r--r--   0 bryant     (501) staff       (20)     1813 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/mixins/bitstamp_rest.py
+-rw-r--r--   0 bryant     (501) staff       (20)    14467 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/mixins/coinbase_rest.py
+-rw-r--r--   0 bryant     (501) staff       (20)     3096 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/mixins/deribit_rest.py
+-rw-r--r--   0 bryant     (501) staff       (20)     2061 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/mixins/dydx_rest.py
+-rw-r--r--   0 bryant     (501) staff       (20)     7481 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/mixins/gemini_rest.py
+-rw-r--r--   0 bryant     (501) staff       (20)    12055 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/mixins/kraken_rest.py
+-rw-r--r--   0 bryant     (501) staff       (20)     1880 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/mixins/okx_rest.py
+-rw-r--r--   0 bryant     (501) staff       (20)     3821 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/mixins/upbit_rest.py
+-rw-r--r--   0 bryant     (501) staff       (20)     6963 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/okcoin.py
+-rw-r--r--   0 bryant     (501) staff       (20)    21567 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/okx.py
+-rw-r--r--   0 bryant     (501) staff       (20)    27078 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/phemex.py
+-rw-r--r--   0 bryant     (501) staff       (20)     4877 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/poloniex.py
+-rw-r--r--   0 bryant     (501) staff       (20)     6680 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/probit.py
+-rw-r--r--   0 bryant     (501) staff       (20)     7883 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/exchanges/upbit.py
+-rw-r--r--   0 bryant     (501) staff       (20)    15303 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/feed.py
+-rw-r--r--   0 bryant     (501) staff       (20)     7845 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/feedhandler.py
+-rw-r--r--   0 bryant     (501) staff       (20)      701 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/log.py
+-rw-r--r--   0 bryant     (501) staff       (20)     1728 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/nbbo.py
+-rw-r--r--   0 bryant     (501) staff       (20)     7792 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/raw_data_collection.py
+-rw-r--r--   0 bryant     (501) staff       (20)     5114 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/symbols.py
+-rw-r--r--   0 bryant     (501) staff       (20)  2231593 2023-05-27 19:27:02.000000 cryptofeed-2.3.2/cryptofeed/types.c
+-rw-r--r--   0 bryant     (501) staff       (20)    35344 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/types.pyx
+drwxr-xr-x   0 bryant     (501) staff       (20)        0 2023-05-27 19:27:02.748350 cryptofeed-2.3.2/cryptofeed/util/
+-rw-r--r--   0 bryant     (501) staff       (20)        0 2021-12-08 22:54:58.000000 cryptofeed-2.3.2/cryptofeed/util/__init__.py
+-rw-r--r--   0 bryant     (501) staff       (20)      922 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/util/book.py
+-rw-r--r--   0 bryant     (501) staff       (20)     1372 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/util/perf.py
+-rw-r--r--   0 bryant     (501) staff       (20)      712 2021-12-08 22:54:58.000000 cryptofeed-2.3.2/cryptofeed/util/split.py
+-rw-r--r--   0 bryant     (501) staff       (20)      911 2023-01-21 01:05:29.000000 cryptofeed-2.3.2/cryptofeed/util/time.py
+drwxr-xr-x   0 bryant     (501) staff       (20)        0 2023-05-27 19:27:02.712809 cryptofeed-2.3.2/cryptofeed.egg-info/
+-rw-r--r--   0 bryant     (501) staff       (20)    54211 2023-05-27 19:27:02.000000 cryptofeed-2.3.2/cryptofeed.egg-info/PKG-INFO
+-rw-r--r--   0 bryant     (501) staff       (20)     3137 2023-05-27 19:27:02.000000 cryptofeed-2.3.2/cryptofeed.egg-info/SOURCES.txt
+-rw-r--r--   0 bryant     (501) staff       (20)        1 2023-05-27 19:27:02.000000 cryptofeed-2.3.2/cryptofeed.egg-info/dependency_links.txt
+-rw-r--r--   0 bryant     (501) staff       (20)      499 2023-05-27 19:27:02.000000 cryptofeed-2.3.2/cryptofeed.egg-info/requires.txt
+-rw-r--r--   0 bryant     (501) staff       (20)       11 2023-05-27 19:27:02.000000 cryptofeed-2.3.2/cryptofeed.egg-info/top_level.txt
+-rw-r--r--   0 bryant     (501) staff       (20)      667 2021-09-04 13:59:37.000000 cryptofeed-2.3.2/pyproject.toml
+-rw-r--r--   0 bryant     (501) staff       (20)       38 2023-05-27 19:27:02.749899 cryptofeed-2.3.2/setup.cfg
+-rw-r--r--   0 bryant     (501) staff       (20)     3895 2023-05-27 19:26:24.000000 cryptofeed-2.3.2/setup.py
```

### Comparing `cryptofeed-2.3.1/AUTHORS.md` & `cryptofeed-2.3.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `cryptofeed-2.3.1/CHANGES.md` & `cryptofeed-2.3.2/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 ## Changelog
 
+### 2.3.2 (2023-05-27)
+ * Bugfix: Fix Socket backend
+ * Bugfix: Fix AUCTION symbol parsing on Coinbase
+ * Bugfix: Fix PERPETUAL symbol parsing on Phemex
+ * Bugfix: Fix PERPETUAL symbol parsing on Kraken Futures
+ * Feature: Access to all AIOKafka configuration options
+ * Feature: Use backend Queue for Kafka
+ * Feature: Add support for storing book snapshots in Redis as key-value
+ * Update: Switch from unmaintained aioredis to redis-py
+ * Bugfix: Correct value for Crypto.com Ask price
+ * Update: Remove cChardet dependency
+ * Feature: Binance TR support
+
 ### 2.3.1 (2022-10-31)
  * Bugfix: timestamp not reset correctly on reconnect
  * Bugfix: Arctic backend failing to write Trades when trade type was not present in data
  * Bugfix: Timestamp sometimes not present in Coinbase ticker updates
  * Bugfix: Phemex, symbols parsing
  * Bugfix: OKx - handle empty liquidations correctly
```

### Comparing `cryptofeed-2.3.1/INSTALL.md` & `cryptofeed-2.3.2/INSTALL.md`

 * *Files identical despite different names*

### Comparing `cryptofeed-2.3.1/LICENSE` & `cryptofeed-2.3.2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to
  deal in the Software without restriction, including without limitation the
  rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
  sell copies of the Software, and to permit persons to whom the Software is
  furnished to do so, subject to the following conditions:
```

### Comparing `cryptofeed-2.3.1/PKG-INFO` & `cryptofeed-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cryptofeed
-Version: 2.3.1
+Version: 2.3.2
 Summary: Cryptocurrency Exchange Websocket Data Feed Handler
 Home-page: https://github.com/bmoscon/cryptofeed
 Author: Bryant Moscon
 Author-email: bmoscon@gmail.com
 License: XFree86
-Keywords: cryptocurrency,bitcoin,btc,feed handler,market feed,market data,crypto assets,Trades,Tickers,BBO,Funding,Open Interest,Liquidation,Order book,Bid,Ask,fmfw.io,Bitfinex,bitFlyer,AscendEX,Bitstamp,Bittrex,Blockchain.com,Bybit,Binance,Binance Delivery,Binance Futures,Binance US,BitMEX,Coinbase,Deribit,EXX,FTX,FTX US,Gate.io,Gemini,HitBTC,Huobi,Huobi DM,Huobi Swap,Kraken,Kraken Futures,OKCoin,OKX,Poloniex,ProBit,Upbit
+Keywords: cryptocurrency,bitcoin,btc,feed handler,market feed,market data,crypto assets,Trades,Tickers,BBO,Funding,Open Interest,Liquidation,Order book,Bid,Ask,fmfw.io,Bitfinex,bitFlyer,AscendEX,Bitstamp,Bittrex,Blockchain.com,Bybit,Binance,Binance Delivery,Binance Futures,Binance US,BitMEX,Coinbase,Deribit,EXX,Gate.io,Gemini,HitBTC,Huobi,Huobi DM,Huobi Swap,Kraken,Kraken Futures,OKCoin,OKX,Poloniex,ProBit,Upbit
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -59,16 +59,14 @@
 * [Coinbase](https://www.coinbase.com/)
 * [Crypto.com](https://www.crypto.com)
 * [Delta](https://www.delta.exchange/)
 * [Deribit](https://www.deribit.com/)
 * [dYdX](https://dydx.exchange/)
 * [FMFW.io](https://www.fmfw.io/)
 * [EXX](https://www.exx.com/)
-* [FTX](https://ftx.com/)
-* [FTX US](https://ftx.us/)
 * [Gate.io](https://www.gate.io/)
 * [Gemini](https://gemini.com/)
 * [HitBTC](https://hitbtc.com/)
 * [Huobi](https://www.hbg.com/)
 * [Huobi DM](https://www.huobi.com/en-us/markets/hb_dm/)
 * Huobi Swap (Coin-M and USDT-M)
 * [Independent Reserve](https://www.independentreserve.com/) 
@@ -296,14 +294,27 @@
 Your Pull Requests are also welcome, even for minor changes.
 
 
 ----
 
 ## Changelog
 
+### 2.3.2 (2023-05-27)
+ * Bugfix: Fix Socket backend
+ * Bugfix: Fix AUCTION symbol parsing on Coinbase
+ * Bugfix: Fix PERPETUAL symbol parsing on Phemex
+ * Bugfix: Fix PERPETUAL symbol parsing on Kraken Futures
+ * Feature: Access to all AIOKafka configuration options
+ * Feature: Use backend Queue for Kafka
+ * Feature: Add support for storing book snapshots in Redis as key-value
+ * Update: Switch from unmaintained aioredis to redis-py
+ * Bugfix: Correct value for Crypto.com Ask price
+ * Update: Remove cChardet dependency
+ * Feature: Binance TR support
+
 ### 2.3.1 (2022-10-31)
  * Bugfix: timestamp not reset correctly on reconnect
  * Bugfix: Arctic backend failing to write Trades when trade type was not present in data
  * Bugfix: Timestamp sometimes not present in Coinbase ticker updates
  * Bugfix: Phemex, symbols parsing
  * Bugfix: OKx - handle empty liquidations correctly
```

### Comparing `cryptofeed-2.3.1/README.md` & `cryptofeed-2.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,14 @@
 * [Coinbase](https://www.coinbase.com/)
 * [Crypto.com](https://www.crypto.com)
 * [Delta](https://www.delta.exchange/)
 * [Deribit](https://www.deribit.com/)
 * [dYdX](https://dydx.exchange/)
 * [FMFW.io](https://www.fmfw.io/)
 * [EXX](https://www.exx.com/)
-* [FTX](https://ftx.com/)
-* [FTX US](https://ftx.us/)
 * [Gate.io](https://www.gate.io/)
 * [Gemini](https://gemini.com/)
 * [HitBTC](https://hitbtc.com/)
 * [Huobi](https://www.hbg.com/)
 * [Huobi DM](https://www.huobi.com/en-us/markets/hb_dm/)
 * Huobi Swap (Coin-M and USDT-M)
 * [Independent Reserve](https://www.independentreserve.com/)
```

### Comparing `cryptofeed-2.3.1/cryptofeed/backends/_util.py` & `cryptofeed-2.3.2/cryptofeed/backends/_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from typing import Any, Dict, List, Union
 
 from cryptofeed.defines import BID, ASK
```

### Comparing `cryptofeed-2.3.1/cryptofeed/backends/aggregate.py` & `cryptofeed-2.3.2/cryptofeed/backends/aggregate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import time
 from decimal import Decimal
 
 import numpy as np
 
 
 class AggregateCallback:
     def __init__(self, handler):
         self.handler = handler
+        if hasattr(self.handler, '__class__'):
+            setattr(self, 'start', self.handler.start)
+            setattr(self, 'stop', self.handler.stop)
+            self.__name__ = self.handler.__class__
 
 
 class Throttle(AggregateCallback):
     """
     Wraps a callback and throttles updates based on `window`. Will allow
     1 update per `window` interval; all others are dropped
     """
```

### Comparing `cryptofeed-2.3.1/cryptofeed/backends/arctic.py` & `cryptofeed-2.3.2/cryptofeed/backends/arctic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 
 Book backends are intentionally left out here - Arctic cannot handle high throughput
 data like book data. Arctic is best used for writing large datasets in batches.
 '''
```

### Comparing `cryptofeed-2.3.1/cryptofeed/backends/backend.py` & `cryptofeed-2.3.2/cryptofeed/backends/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 from asyncio.queues import Queue
 from multiprocessing import Pipe, Process
```

### Comparing `cryptofeed-2.3.1/cryptofeed/backends/gcppubsub.py` & `cryptofeed-2.3.2/cryptofeed/backends/gcppubsub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from collections import defaultdict
 import os
 import io
```

### Comparing `cryptofeed-2.3.1/cryptofeed/backends/http.py` & `cryptofeed-2.3.2/cryptofeed/backends/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import logging
 
 import aiohttp
```

### Comparing `cryptofeed-2.3.1/cryptofeed/backends/influxdb.py` & `cryptofeed-2.3.2/cryptofeed/backends/influxdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from collections import defaultdict
 import logging
```

### Comparing `cryptofeed-2.3.1/cryptofeed/backends/kafka.py` & `cryptofeed-2.3.2/cryptofeed/backends/mongo.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,106 +1,88 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from collections import defaultdict
-import asyncio
-from typing import Optional
+from datetime import timezone, datetime as dt
 
-from aiokafka import AIOKafkaProducer
-from yapic import json
+import bson
+import motor.motor_asyncio
 
-from cryptofeed.backends.backend import BackendBookCallback, BackendCallback
+from cryptofeed.backends.backend import BackendBookCallback, BackendCallback, BackendQueue
 
 
-class KafkaCallback:
-    def __init__(self, bootstrap='127.0.0.1', port=9092, key=None, numeric_type=float, none_to=None, acks=0, client_id='cryptofeed', **kwargs):
-        """
-        bootstrap: str, list
-            if a list, should be a list of strings in the format: ip/host:port, i.e.
-                192.1.1.1:9092
-                192.1.1.2:9092
-                etc
-            if a string, should be ip/port only
-        """
-        self.bootstrap = bootstrap
+class MongoCallback(BackendQueue):
+    def __init__(self, db, host='127.0.0.1', port=27017, key=None, none_to=None, numeric_type=str, **kwargs):
+        self.host = host
         self.port = port
-        self.producer = None
-        self.key = key if key else self.default_key
+        self.db = db
         self.numeric_type = numeric_type
         self.none_to = none_to
-        self.acks = acks
-        self.client_id = client_id
+        self.collection = key if key else self.default_key
+        self.running = True
 
-    async def __connect(self):
-        if not self.producer:
-            loop = asyncio.get_event_loop()
-            self.producer = AIOKafkaProducer(acks=self.acks,
-                                             loop=loop,
-                                             bootstrap_servers=f'{self.bootstrap}:{self.port}' if isinstance(self.bootstrap, str) else self.bootstrap,
-                                             client_id=self.client_id)
-            await self.producer.start()
+    async def writer(self):
+        conn = motor.motor_asyncio.AsyncIOMotorClient(self.host, self.port)
+        db = conn[self.db]
+        while self.running:
+            async with self.read_queue() as updates:
+                for index in range(len(updates)):
+                    updates[index]['timestamp'] = dt.fromtimestamp(updates[index]['timestamp'], tz=timezone.utc) if updates[index]['timestamp'] else None
+                    updates[index]['receipt_timestamp'] = dt.fromtimestamp(updates[index]['receipt_timestamp'], tz=timezone.utc) if updates[index]['receipt_timestamp'] else None
 
-    def topic(self, data: dict) -> str:
-        return f"{self.key}-{data['exchange']}-{data['symbol']}"
+                    if 'book' in updates[index]:
+                        updates[index] = {'exchange': updates[index]['exchange'], 'symbol': updates[index]['symbol'], 'timestamp': updates[index]['timestamp'], 'receipt_timestamp': updates[index]['receipt_timestamp'], 'delta': 'delta' in updates[index], 'bid': bson.BSON.encode(updates[index]['book']['bid'] if 'delta' not in updates[index] else updates[index]['delta']['bid']), 'ask': bson.BSON.encode(updates[index]['book']['ask'] if 'delta' not in updates[index] else updates[index]['delta']['ask'])}
 
-    def partition_key(self, data: dict) -> Optional[bytes]:
-        return None
+                await db[self.collection].insert_many(updates)
 
-    def partition(self, data: dict) -> Optional[int]:
-        return None
 
-    async def write(self, data: dict):
-        await self.__connect()
-        await self.producer.send_and_wait(self.topic(data), json.dumps(data).encode('utf-8'), self.partition_key(data), self.partition(data))
-
-
-class TradeKafka(KafkaCallback, BackendCallback):
+class TradeMongo(MongoCallback, BackendCallback):
     default_key = 'trades'
 
 
-class FundingKafka(KafkaCallback, BackendCallback):
+class FundingMongo(MongoCallback, BackendCallback):
     default_key = 'funding'
 
 
-class BookKafka(KafkaCallback, BackendBookCallback):
+class BookMongo(MongoCallback, BackendBookCallback):
     default_key = 'book'
 
     def __init__(self, *args, snapshots_only=False, snapshot_interval=1000, **kwargs):
         self.snapshots_only = snapshots_only
         self.snapshot_interval = snapshot_interval
         self.snapshot_count = defaultdict(int)
         super().__init__(*args, **kwargs)
 
 
-class TickerKafka(KafkaCallback, BackendCallback):
+class TickerMongo(MongoCallback, BackendCallback):
     default_key = 'ticker'
 
 
-class OpenInterestKafka(KafkaCallback, BackendCallback):
+class OpenInterestMongo(MongoCallback, BackendCallback):
     default_key = 'open_interest'
 
 
-class LiquidationsKafka(KafkaCallback, BackendCallback):
+class LiquidationsMongo(MongoCallback, BackendCallback):
     default_key = 'liquidations'
 
 
-class CandlesKafka(KafkaCallback, BackendCallback):
+class CandlesMongo(MongoCallback, BackendCallback):
     default_key = 'candles'
 
 
-class OrderInfoKafka(KafkaCallback, BackendCallback):
+class OrderInfoMongo(MongoCallback, BackendCallback):
     default_key = 'order_info'
 
 
-class TransactionsKafka(KafkaCallback, BackendCallback):
+class TransactionsMongo(MongoCallback, BackendCallback):
     default_key = 'transactions'
 
 
-class BalancesKafka(KafkaCallback, BackendCallback):
+class BalancesMongo(MongoCallback, BackendCallback):
     default_key = 'balances'
 
 
-class FillsKafka(KafkaCallback, BackendCallback):
+class FillsMongo(MongoCallback, BackendCallback):
     default_key = 'fills'
```

### Comparing `cryptofeed-2.3.1/cryptofeed/backends/mongo.py` & `cryptofeed-2.3.2/cryptofeed/backends/zmq.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,90 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from collections import defaultdict
-from datetime import timezone, datetime as dt
 
-import bson
-import motor.motor_asyncio
+import zmq
+import zmq.asyncio
+from yapic import json
 
-from cryptofeed.backends.backend import BackendBookCallback, BackendCallback, BackendQueue
+from cryptofeed.backends.backend import BackendQueue, BackendBookCallback, BackendCallback
 
 
-class MongoCallback(BackendQueue):
-    def __init__(self, db, host='127.0.0.1', port=27017, key=None, none_to=None, numeric_type=str, **kwargs):
-        self.host = host
-        self.port = port
-        self.db = db
+class ZMQCallback(BackendQueue):
+    def __init__(self, host='127.0.0.1', port=5555, none_to=None, numeric_type=float, key=None, dynamic_key=True, **kwargs):
+        self.url = "tcp://{}:{}".format(host, port)
+        self.key = key if key else self.default_key
         self.numeric_type = numeric_type
         self.none_to = none_to
-        self.collection = key if key else self.default_key
+        self.dynamic_key = dynamic_key
         self.running = True
 
     async def writer(self):
-        conn = motor.motor_asyncio.AsyncIOMotorClient(self.host, self.port)
-        db = conn[self.db]
+        ctx = zmq.asyncio.Context.instance()
+        con = ctx.socket(zmq.PUB)
+        con.connect(self.url)
         while self.running:
             async with self.read_queue() as updates:
-                for index in range(len(updates)):
-                    updates[index]['timestamp'] = dt.fromtimestamp(updates[index]['timestamp'], tz=timezone.utc) if updates[index]['timestamp'] else None
-                    updates[index]['receipt_timestamp'] = dt.fromtimestamp(updates[index]['receipt_timestamp'], tz=timezone.utc) if updates[index]['receipt_timestamp'] else None
+                for update in updates:
+                    if self.dynamic_key:
+                        update = f'{update["exchange"]}-{self.key}-{update["symbol"]} {json.dumps(update)}'
+                    else:
+                        update = f'{self.key} {json.dumps(update)}'
+                    await con.send_string(update)
 
-                    if 'book' in updates[index]:
-                        updates[index] = {'exchange': updates[index]['exchange'], 'symbol': updates[index]['symbol'], 'timestamp': updates[index]['timestamp'], 'receipt_timestamp': updates[index]['receipt_timestamp'], 'delta': 'delta' in updates[index], 'bid': bson.BSON.encode(updates[index]['book']['bid'] if 'delta' not in updates[index] else updates[index]['delta']['bid']), 'ask': bson.BSON.encode(updates[index]['book']['ask'] if 'delta' not in updates[index] else updates[index]['delta']['ask'])}
 
-                await db[self.collection].insert_many(updates)
+class TradeZMQ(ZMQCallback, BackendCallback):
+    default_key = 'trades'
 
 
-class TradeMongo(MongoCallback, BackendCallback):
-    default_key = 'trades'
+class TickerZMQ(ZMQCallback, BackendCallback):
+    default_key = 'ticker'
 
 
-class FundingMongo(MongoCallback, BackendCallback):
+class FundingZMQ(ZMQCallback, BackendCallback):
     default_key = 'funding'
 
 
-class BookMongo(MongoCallback, BackendBookCallback):
+class BookZMQ(ZMQCallback, BackendBookCallback):
     default_key = 'book'
 
     def __init__(self, *args, snapshots_only=False, snapshot_interval=1000, **kwargs):
         self.snapshots_only = snapshots_only
         self.snapshot_interval = snapshot_interval
         self.snapshot_count = defaultdict(int)
         super().__init__(*args, **kwargs)
 
 
-class TickerMongo(MongoCallback, BackendCallback):
-    default_key = 'ticker'
-
-
-class OpenInterestMongo(MongoCallback, BackendCallback):
+class OpenInterestZMQ(ZMQCallback, BackendCallback):
     default_key = 'open_interest'
 
 
-class LiquidationsMongo(MongoCallback, BackendCallback):
+class LiquidationsZMQ(ZMQCallback, BackendCallback):
     default_key = 'liquidations'
 
 
-class CandlesMongo(MongoCallback, BackendCallback):
+class CandlesZMQ(ZMQCallback, BackendCallback):
     default_key = 'candles'
 
 
-class OrderInfoMongo(MongoCallback, BackendCallback):
-    default_key = 'order_info'
+class BalancesZMQ(ZMQCallback, BackendCallback):
+    default_key = 'balances'
 
 
-class TransactionsMongo(MongoCallback, BackendCallback):
-    default_key = 'transactions'
+class PositionsZMQ(ZMQCallback, BackendCallback):
+    default_key = 'positions'
 
 
-class BalancesMongo(MongoCallback, BackendCallback):
-    default_key = 'balances'
+class OrderInfoZMQ(ZMQCallback, BackendCallback):
+    default_key = 'order_info'
 
 
-class FillsMongo(MongoCallback, BackendCallback):
+class FillsZMQ(ZMQCallback, BackendCallback):
     default_key = 'fills'
+
+
+class TransactionsZMQ(ZMQCallback, BackendCallback):
+    default_key = 'transactions'
```

### Comparing `cryptofeed-2.3.1/cryptofeed/backends/postgres.py` & `cryptofeed-2.3.2/cryptofeed/backends/postgres.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from collections import defaultdict
 from datetime import datetime as dt
 from typing import Tuple
```

### Comparing `cryptofeed-2.3.1/cryptofeed/backends/quest.py` & `cryptofeed-2.3.2/cryptofeed/backends/quest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import logging
 
 from cryptofeed.backends.backend import BackendCallback
```

### Comparing `cryptofeed-2.3.1/cryptofeed/backends/rabbitmq.py` & `cryptofeed-2.3.2/cryptofeed/backends/rabbitmq.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 from collections import defaultdict
```

### Comparing `cryptofeed-2.3.1/cryptofeed/backends/redis.py` & `cryptofeed-2.3.2/cryptofeed/backends/redis.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from collections import defaultdict
 
-import aioredis
+from redis import asyncio as aioredis
 from yapic import json
 
 from cryptofeed.backends.backend import BackendBookCallback, BackendCallback, BackendQueue
 
 
 class RedisCallback(BackendQueue):
     def __init__(self, host='127.0.0.1', port=6379, socket=None, key=None, none_to='None', numeric_type=float, **kwargs):
@@ -74,14 +74,29 @@
                         pipe = pipe.xadd(f"{self.key}-{update['exchange']}-{update['symbol']}", update)
                     await pipe.execute()
 
         await conn.close()
         await conn.connection_pool.disconnect()
 
 
+class RedisKeyCallback(RedisCallback):
+
+    async def writer(self):
+        conn = aioredis.from_url(self.redis)
+
+        while self.running:
+            async with self.read_queue() as updates:
+                update = list(updates)[-1]
+                if update:
+                    await conn.set(f"{self.key}-{update['exchange']}-{update['symbol']}", json.dumps(update))
+
+        await conn.close()
+        await conn.connection_pool.disconnect()
+
+
 class TradeRedis(RedisZSetCallback, BackendCallback):
     default_key = 'trades'
 
 
 class TradeStream(RedisStreamCallback, BackendCallback):
     default_key = 'trades'
 
@@ -110,14 +125,24 @@
     def __init__(self, *args, snapshots_only=False, snapshot_interval=1000, **kwargs):
         self.snapshots_only = snapshots_only
         self.snapshot_interval = snapshot_interval
         self.snapshot_count = defaultdict(int)
         super().__init__(*args, **kwargs)
 
 
+class BookSnapshotRedisKey(RedisKeyCallback, BackendBookCallback):
+    default_key = 'book'
+
+    def __init__(self, *args, snapshot_interval=1000, score_key='receipt_timestamp', **kwargs):
+        kwargs['snapshots_only'] = True
+        self.snapshot_interval = snapshot_interval
+        self.snapshot_count = defaultdict(int)
+        super().__init__(*args, score_key=score_key, **kwargs)
+
+
 class TickerRedis(RedisZSetCallback, BackendCallback):
     default_key = 'ticker'
 
 
 class TickerStream(RedisStreamCallback, BackendCallback):
     default_key = 'ticker'
```

### Comparing `cryptofeed-2.3.1/cryptofeed/backends/socket.py` & `cryptofeed-2.3.2/cryptofeed/backends/socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from collections import defaultdict
 import asyncio
 import logging
@@ -81,17 +81,17 @@
                     if self.conn_type == 'udp://':
                         if len(update) > self.mtu:
                             chunks = wrap(update, self.mtu)
                             for chunk in chunks:
                                 msg = json.dumps({'type': 'chunked', 'chunks': len(chunks), 'data': chunk}).encode()
                                 self.conn.sendto(msg)
                         else:
-                            self.conn.sendto(update.encode())
+                            self.conn.sendto(data.encode())
                     else:
-                        self.conn.write(update.encode())
+                        self.conn.write(data.encode())
 
     async def connect(self):
         if not self.conn:
             if self.conn_type == 'udp://':
                 loop = asyncio.get_event_loop()
                 self.conn, self.protocol = await loop.create_datagram_endpoint(
                     lambda: UDPProtocol(loop), remote_addr=(self.addr, self.port))
```

### Comparing `cryptofeed-2.3.1/cryptofeed/callback.py` & `cryptofeed-2.3.2/cryptofeed/callback.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 import inspect
```

### Comparing `cryptofeed-2.3.1/cryptofeed/config.py` & `cryptofeed-2.3.2/cryptofeed/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import os
 
 import yaml
```

### Comparing `cryptofeed-2.3.1/cryptofeed/connection.py` & `cryptofeed-2.3.2/cryptofeed/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import logging
 import time
 import asyncio
```

### Comparing `cryptofeed-2.3.1/cryptofeed/connection_handler.py` & `cryptofeed-2.3.2/cryptofeed/connection_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 import logging
 import random
```

### Comparing `cryptofeed-2.3.1/cryptofeed/defines.py` & `cryptofeed-2.3.2/cryptofeed/defines.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 
 
 Defines contains all constant string definitions for Cryptofeed,
 as well as some documentation (in comment form) regarding
@@ -13,14 +13,15 @@
 ASCENDEX_FUTURES = 'ASCENDEX_FUTURES'
 BEQUANT = 'BEQUANT'
 BITFINEX = 'BITFINEX'
 BITHUMB = 'BITHUMB'
 BITMEX = 'BITMEX'
 BINANCE = 'BINANCE'
 BINANCE_US = 'BINANCE_US'
+BINANCE_TR = 'BINANCE_TR'
 BINANCE_FUTURES = 'BINANCE_FUTURES'
 BINANCE_DELIVERY = 'BINANCE_DELIVERY'
 BITDOTCOM = 'BIT.COM'
 BITFLYER = 'BITFLYER'
 BITGET = 'BITGET'
 BITSTAMP = 'BITSTAMP'
 BITTREX = 'BITTREX'
@@ -28,17 +29,14 @@
 BYBIT = 'BYBIT'
 COINBASE = 'COINBASE'
 CRYPTODOTCOM = "CRYPTO.COM"
 DELTA = 'DELTA'
 DERIBIT = 'DERIBIT'
 DYDX = 'DYDX'
 EXX = 'EXX'
-FTX = 'FTX'
-FTX_US = 'FTX_US'
-FTX_TR = 'FTX_TR'
 FMFW = 'FMFW'
 GATEIO = 'GATEIO'
 GEMINI = 'GEMINI'
 HITBTC = 'HITBTC'
 HUOBI = 'HUOBI'
 HUOBI_DM = 'HUOBI_DM'
 HUOBI_SWAP = 'HUOBI_SWAP'
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exceptions.py` & `cryptofeed-2.3.2/cryptofeed/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 
 
 class MissingSequenceNumber(Exception):
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchange.py` & `cryptofeed-2.3.2/cryptofeed/exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 from decimal import Decimal
 import logging
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/__init__.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from cryptofeed.defines import *
-from cryptofeed.defines import FTX as FTX_str, EXX as EXX_str, FMFW as FMFW_str, OKX as OKX_str
+from cryptofeed.defines import EXX as EXX_str, FMFW as FMFW_str, OKX as OKX_str
 from .bitdotcom import BitDotCom
 from .phemex import Phemex
 from .ascendex import AscendEX
 from .ascendex_futures import AscendEXFutures
 from .bequant import Bequant
 from .binance import Binance
 from .binance_delivery import BinanceDelivery
 from .binance_futures import BinanceFutures
 from .binance_us import BinanceUS
+from .binance_tr import BinanceTR
 from .fmfw import FMFW
 from .bitfinex import Bitfinex
 from .bitflyer import Bitflyer
 from .bitget import Bitget
 from .bithumb import Bithumb
 from .bitmex import Bitmex
 from .bitstamp import Bitstamp
@@ -27,17 +28,14 @@
 from .bybit import Bybit
 from .coinbase import Coinbase
 from .cryptodotcom import CryptoDotCom
 from .delta import Delta
 from .deribit import Deribit
 from .dydx import dYdX
 from .exx import EXX
-from .ftx import FTX
-from .ftx_us import FTXUS
-from .ftx_tr import FTXTR
 from .gateio import Gateio
 from .gemini import Gemini
 from .hitbtc import HitBTC
 from .huobi import Huobi
 from .huobi_dm import HuobiDM
 from .huobi_swap import HuobiSwap
 from .independent_reserve import IndependentReserve
@@ -54,14 +52,15 @@
 EXCHANGE_MAP = {
     ASCENDEX: AscendEX,
     ASCENDEX_FUTURES: AscendEXFutures,
     BEQUANT: Bequant,
     BINANCE_DELIVERY: BinanceDelivery,
     BINANCE_FUTURES: BinanceFutures,
     BINANCE_US: BinanceUS,
+    BINANCE_TR: BinanceTR,
     BINANCE: Binance,
     FMFW_str: FMFW,
     BITDOTCOM: BitDotCom,
     BITFINEX: Bitfinex,
     BITFLYER: Bitflyer,
     BITGET: Bitget,
     BITHUMB: Bithumb,
@@ -72,17 +71,14 @@
     BYBIT: Bybit,
     COINBASE: Coinbase,
     CRYPTODOTCOM: CryptoDotCom,
     DERIBIT: Deribit,
     DELTA: Delta,
     DYDX: dYdX,
     EXX_str: EXX,
-    FTX_str: FTX,
-    FTX_US: FTXUS,
-    FTX_TR: FTXTR,
     GATEIO: Gateio,
     GEMINI: Gemini,
     HITBTC: HitBTC,
     HUOBI_DM: HuobiDM,
     HUOBI_SWAP: HuobiSwap,
     HUOBI: Huobi,
     INDEPENDENT_RESERVE: IndependentReserve,
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/ascendex.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/ascendex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from collections import defaultdict
 from typing import Dict, Tuple
 from cryptofeed.connection import AsyncConnection, RestEndpoint, Routes, WebsocketEndpoint
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/ascendex_futures.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/ascendex_futures.py`

 * *Files identical despite different names*

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/bequant.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/bequant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import hashlib
 import hmac
 import random
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/binance.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/binance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import logging
 from asyncio import create_task, sleep
 from collections import defaultdict
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/binance_delivery.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/binance_delivery.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from decimal import Decimal
 import logging
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/binance_futures.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/binance_futures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from decimal import Decimal
 import logging
 from typing import Tuple, Dict
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/binance_us.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/binance_us.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import logging
 
 from cryptofeed.connection import RestEndpoint, WebsocketEndpoint, Routes
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/bitdotcom.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/bitdotcom.py`

 * *Files identical despite different names*

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/bitfinex.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/bitfinex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from collections import defaultdict
 from decimal import Decimal
 from functools import partial
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/bitflyer.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/bitflyer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2018-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2018-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from collections import defaultdict
 import logging
 from decimal import Decimal
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/bitget.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/bitget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import base64
 import hmac
 import logging
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/bithumb.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/bithumb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import logging
 from decimal import Decimal
 from typing import Tuple, Dict
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/bitmex.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/bitmex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from typing import Dict, Tuple
 import hashlib
 import hmac
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/bitstamp.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/bitstamp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 from cryptofeed.symbols import Symbol
 import logging
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/bittrex.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/bittrex.py`

 * *Files identical despite different names*

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/blockchain.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/blockchain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import logging
 from decimal import Decimal
 from typing import Dict, Tuple
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/bybit.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/bybit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2018-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2018-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import hmac
 import time
 from collections import defaultdict
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/coinbase.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/coinbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 import logging
 import time
@@ -39,15 +39,16 @@
 
     @classmethod
     def _parse_symbol_data(cls, data: list) -> Tuple[Dict, Dict]:
         ret = {}
         info = defaultdict(dict)
 
         for entry in data:
-            sym = Symbol(entry['base_currency'], entry['quote_currency'])
+            base, quote = entry['id'].split("-")
+            sym = Symbol(base, quote)
             info['tick_size'][sym.normalized] = entry['quote_increment']
             info['instrument_type'][sym.normalized] = sym.type
             ret[sym.normalized] = entry['id']
         return ret, info
 
     def __init__(self, callbacks=None, **kwargs):
         super().__init__(callbacks=callbacks, **kwargs)
@@ -299,14 +300,16 @@
     async def _change(self, msg: dict, timestamp: float):
         """
         Like done, these updates can be sent for orders that are not in the book. Per the docs:
 
         Not all done or change messages will result in changing the order book. These messages will
         be sent for received orders which are not yet on the order book. Do not alter
         the order book for such messages, otherwise your order book will be incorrect.
+
+        {'price': '16556.88', 'old_size': '0.24076471', 'new_size': '0.04076471', 'order_id': '9675d63e-0432-413d-a3f3-f30d7df39614', 'reason': 'STP', 'type': 'change', 'side': 'buy', 'product_id': 'BTC-USD', 'time': datetime.datetime(2022, 11, 24, 0, 35, 28, 904847, tzinfo=datetime.timezone.utc), 'sequence': 50703787284}
         """
         if not self.keep_l3_book:
             return
 
         delta = {BID: [], ASK: []}
 
         if 'price' not in msg or not msg['price']:
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/cryptodotcom.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/cryptodotcom.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 import logging
 from decimal import Decimal
@@ -105,15 +105,15 @@
                     'l': Decimal('55313.95'),
                     'c': Decimal('1311.15')
                 }
             ]
         }
         '''
         for entry in msg['data']:
-            await self.callback(TICKER, Ticker(self.id, self.exchange_symbol_to_std_symbol(entry['i']), entry['b'], entry['a'], self.timestamp_normalize(entry['t']), raw=entry), timestamp)
+            await self.callback(TICKER, Ticker(self.id, self.exchange_symbol_to_std_symbol(entry['i']), entry['b'], entry['k'], self.timestamp_normalize(entry['t']), raw=entry), timestamp)
 
     async def _candle(self, msg: dict, timestamp: float):
         '''
         {
             'instrument_name': 'BTC_USDT',
             'subscription': 'candlestick.14D.BTC_USDT',
             'channel': 'candlestick',
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/delta.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/delta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import logging
 from decimal import Decimal
 from typing import Dict, Tuple
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/deribit.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/deribit.py`

 * *Files identical despite different names*

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/dydx.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/dydx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from collections import defaultdict
 from cryptofeed.symbols import Symbol
 import logging
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/exx.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/exx.py`

 * *Files identical despite different names*

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/fmfw.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/fmfw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from collections import defaultdict
 from decimal import Decimal
 import logging
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/ftx.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/okx.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,437 +1,509 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
-
-import asyncio
 from collections import defaultdict
-import logging
 from decimal import Decimal
-import hmac
-from time import time
-from typing import Dict, Iterable, Tuple
-
+from typing import Dict, Tuple
 from yapic import json
+import asyncio
+import base64
+import hmac
+import logging
+import requests
+import time
 
 from cryptofeed.connection import AsyncConnection, RestEndpoint, Routes, WebsocketEndpoint
-from cryptofeed.defines import BID, ASK, BUY, CLOSED, FUTURES, LIMIT, MAKER, MARKET, OPEN, ORDER_INFO, PERPETUAL, SPOT, SUBMITTING, FILLS, TAKER
-from cryptofeed.defines import FTX as FTX_id
-from cryptofeed.defines import FUNDING, L2_BOOK, LIQUIDATIONS, OPEN_INTEREST, SELL, TICKER, TRADES, FILLED
-from cryptofeed.exceptions import BadChecksum
+from cryptofeed.defines import CALL, CANCELLED, FILL_OR_KILL, FUTURES, IMMEDIATE_OR_CANCEL, MAKER_OR_CANCEL, MARKET, OKX as OKX_str, LIQUIDATIONS, BUY, OPEN, OPTION, PARTIAL, PERPETUAL, PUT, SELL, FILLED, ASK, BID, FUNDING, L2_BOOK, OPEN_INTEREST, TICKER, TRADES, ORDER_INFO, CANDLES, SPOT, UNFILLED, LIMIT
+from cryptofeed.exchanges.mixins.okx_rest import OKXRestMixin
 from cryptofeed.feed import Feed
+from cryptofeed.exceptions import BadChecksum
 from cryptofeed.symbols import Symbol
-from cryptofeed.exchanges.mixins.ftx_rest import FTXRestMixin
-from cryptofeed.types import OrderBook, Trade, Ticker, Funding, OpenInterest, Liquidation, OrderInfo, Fill
+from cryptofeed.types import OrderBook, Trade, Ticker, Funding, OpenInterest, Liquidation, OrderInfo, Candle
 
 
-LOG = logging.getLogger('feedhandler')
+LOG = logging.getLogger("feedhandler")
 
 
-class FTX(Feed, FTXRestMixin):
-    id = FTX_id
-    allow_empty_subscriptions = True
-    websocket_endpoints = [WebsocketEndpoint('wss://ftx.com/ws/', options={'compression': None})]
-    rest_endpoints = [RestEndpoint('https://ftx.com', routes=Routes('/api/markets', open_interest='/api/futures/{}/stats', funding='/api/funding_rates?future={}', stats='/api/futures/{}/stats'))]
-
+class OKX(Feed, OKXRestMixin):
+    id = OKX_str
+    valid_candle_intervals = {'1M', '1W', '1D', '12H', '6H', '4H', '2H', '1H', '30m', '15m', '5m', '3m', '1m'}
+    candle_interval_map = {'1M': 2630000, '1W': 604800, '1D': 86400, '12H': 43200, '6H': 21600, '4H': 14400, '2H': 7200, '1H': 3600, '30m': 1800, '15m': 900, '5m': 300, '3m': 180, '1m': 60}
     websocket_channels = {
-        L2_BOOK: 'orderbook',
+        L2_BOOK: 'books',
         TRADES: 'trades',
-        TICKER: 'ticker',
-        FUNDING: 'funding',
-        OPEN_INTEREST: 'open_interest',
-        LIQUIDATIONS: 'trades',
+        TICKER: 'tickers',
+        FUNDING: 'funding-rate',
+        OPEN_INTEREST: 'open-interest',
+        LIQUIDATIONS: LIQUIDATIONS,
         ORDER_INFO: 'orders',
-        FILLS: 'fills',
+        CANDLES: 'candle'
     }
-    request_limit = 30
+    websocket_endpoints = [
+        WebsocketEndpoint('wss://ws.okx.com:8443/ws/v5/public', channel_filter=(websocket_channels[L2_BOOK], websocket_channels[TRADES], websocket_channels[TICKER], websocket_channels[FUNDING], websocket_channels[OPEN_INTEREST], websocket_channels[LIQUIDATIONS], websocket_channels[CANDLES]), options={'compression': None}),
+        WebsocketEndpoint('wss://ws.okx.com:8443/ws/v5/private', channel_filter=(websocket_channels[ORDER_INFO],), options={'compression': None}),
+    ]
+    rest_endpoints = [RestEndpoint('https://www.okx.com', routes=Routes(['/api/v5/public/instruments?instType=SPOT', '/api/v5/public/instruments?instType=SWAP', '/api/v5/public/instruments?instType=FUTURES', '/api/v5/public/instruments?instType=OPTION&uly=BTC-USD', '/api/v5/public/instruments?instType=OPTION&uly=ETH-USD'], liquidations='/api/v5/public/liquidation-orders?instType={}&limit=100&state={}&uly={}'))]
+    request_limit = 20
 
     @classmethod
-    def _parse_symbol_data(cls, data: dict) -> Tuple[Dict, Dict]:
+    def timestamp_normalize(cls, ts: float) -> float:
+        return ts / 1000.0
+
+    @classmethod
+    def _parse_symbol_data(cls, data: list) -> Tuple[Dict, Dict]:
         ret = {}
         info = defaultdict(dict)
 
-        for d in data['result']:
-            if not d['enabled']:
-                continue
-            expiry = None
-            stype = SPOT
-            # FTX Futures contracts are stable coin settled, but
-            # prices quoted are in USD, see https://help.ftx.com/hc/en-us/articles/360024780791-What-Are-Futures
-            if "-MOVE-" in d['name']:
-                stype = FUTURES
-                base, expiry = d['name'].rsplit("-", maxsplit=1)
-                quote = 'USD'
-                if 'Q' in expiry:
-                    year, quarter = expiry.split("Q")
-                    year = year[2:]
-                    date = ["0325", "0624", "0924", "1231"]
-                    expiry = year + date[int(quarter) - 1]
-            elif "-" in d['name']:
-                base, expiry = d['name'].split("-")
-                quote = 'USD'
-                stype = FUTURES
-                if expiry == 'PERP':
-                    expiry = None
+        for entry in data:
+            for e in entry['data']:
+                expiry = None
+                otype = None
+                stype = e['instType'].lower()
+                strike = None
+
+                if stype == SPOT:
+                    base = e['baseCcy']
+                    quote = e['quoteCcy']
+                elif stype == FUTURES:
+                    base, quote, expiry = e['instId'].split("-")
+                elif stype == OPTION:
+                    base, quote, expiry, strike, otype = e['instId'].split("-")
+                    otype = PUT if otype == 'P' else CALL
+                elif stype == 'swap':
+                    # this is a perpetual swap (aka perpetual futures contract), not a real swap
                     stype = PERPETUAL
-            elif d['type'] == SPOT:
-                base, quote = d['baseCurrency'], d['quoteCurrency']
-            else:
-                # not enough info to construct a symbol - this is usually caused
-                # by non crypto futures, i.e. TRUMP2024 or other contracts involving
-                # betting on world events
-                continue
-
-            s = Symbol(base, quote, type=stype, expiry_date=expiry)
-            ret[s.normalized] = d['name']
-            info['tick_size'][s.normalized] = d['priceIncrement']
-            info['quantity_step'][s.normalized] = d['sizeIncrement']
-            info['instrument_type'][s.normalized] = s.type
-        return ret, info
+                    base, quote, _ = e['instId'].split("-")
 
-    def __reset(self):
-        self._l2_book = {}
-        self._funding_cache = {}
-        self._open_interest_cache = {}
+                s = Symbol(base, quote, expiry_date=expiry, type=stype, option_type=otype, strike_price=strike)
+                ret[s.normalized] = e['instId']
+                info['tick_size'][s.normalized] = e['tickSz']
+                info['instrument_type'][s.normalized] = stype
 
-    async def generate_token(self, conn: AsyncConnection):
-        ts = int(time() * 1000)
-        msg = {
-            'op': 'login',
-            'args':
-            {
-                'key': self.key_id,
-                'sign': hmac.new(self.key_secret.encode(), f'{ts}websocket_login'.encode(), 'sha256').hexdigest(),
-                'time': ts,
-            }
-        }
-        if self.subaccount:
-            msg['args']['subaccount'] = self.subaccount
-        await conn.write(json.dumps(msg))
-
-    async def authenticate(self, conn: AsyncConnection):
-        if self.requires_authentication:
-            await self.generate_token(conn)
-
-    async def subscribe(self, conn: AsyncConnection):
-        self.__reset()
-        for chan in self.subscription:
-            symbols = self.subscription[chan]
-            if chan == FUNDING:
-                asyncio.create_task(self._funding(symbols))
-                continue
-            if chan == OPEN_INTEREST:
-                asyncio.create_task(self._open_interest(symbols))
-                continue
-            if self.is_authenticated_channel(self.exchange_channel_to_std(chan)):
-                await conn.write(json.dumps(
-                    {
-                        "channel": chan,
-                        "op": "subscribe"
-                    }
-                ))
-                continue
-            for pair in symbols:
-                await conn.write(json.dumps(
-                    {
-                        "channel": chan,
-                        "market": pair,
-                        "op": "subscribe"
-                    }
-                ))
+        return ret, info
 
-    async def _open_interest(self, pairs: Iterable):
+    async def _liquidations(self, pairs: list):
+        last_update = defaultdict(dict)
         """
-            {
-              "success": true,
-              "result": {
-                "volume": 1000.23,
-                "nextFundingRate": 0.00025,
-                "nextFundingTime": "2019-03-29T03:00:00+00:00",
-                "expirationPrice": 3992.1,
-                "predictedExpirationPrice": 3993.6,
-                "strikePrice": 8182.35,
-                "openInterest": 21124.583
-              }
-            }
+        for PERP liquidations, the following arguments are required: uly, state
+        for FUTURES liquidations, the following arguments are required: uly, state, alias
+        FUTURES, MARGIN and OPTION liquidation request not currently supported by the below
         """
+
         while True:
             for pair in pairs:
-                # OI only for perp and futures, so check for / in pair name indicating spot
-                if '/' in pair:
+                if 'SWAP' in pair:
+                    instrument_type = 'SWAP'
+                    uly = pair.split("-")[0] + "-" + pair.split("-")[1]
+                else:
                     continue
-                data = await self.http_conn.read(self.rest_endpoints[0].route('open_interest', sandbox=self.sandbox).format(pair))
-                received = time()
-                data = json.loads(data, parse_float=Decimal)
-                if 'result' in data:
-                    oi = data['result']['openInterest']
-                    if oi != self._open_interest_cache.get(pair, None):
-                        o = OpenInterest(
+
+                for status in (FILLED, UNFILLED):
+                    data = await self.http_conn.read(self.rest_endpoints[0].route('liquidations', sandbox=self.sandbox).format(instrument_type, status, uly))
+                    data = json.loads(data, parse_float=Decimal)
+                    timestamp = time.time()
+                    if not data['data']:
+                        LOG.info('%s: no liquidation data received for %s @ %s', self.id, pair, self.rest_endpoints[0].route('liquidations', sandbox=self.sandbox).format(instrument_type, status, uly))
+                        continue
+                    if len(data['data'][0]['details']) == 0 or (len(data['data'][0]['details']) > 0 and last_update.get(pair) == data['data'][0]['details'][0]):
+                        continue
+                    for entry in data['data'][0]['details']:
+                        if pair in last_update:
+                            if entry == last_update[pair].get(status):
+                                break
+
+                        liq = Liquidation(
                             self.id,
-                            self.exchange_symbol_to_std_symbol(pair),
-                            oi,
+                            pair,
+                            BUY if entry['side'] == 'buy' else SELL,
+                            Decimal(entry['sz']),
+                            Decimal(entry['bkPx']),
                             None,
+                            status,
+                            self.timestamp_normalize(int(entry['ts'])),
                             raw=data
                         )
-                        await self.callback(OPEN_INTEREST, o, received)
-                        self._open_interest_cache[pair] = oi
-                        await asyncio.sleep(1)
+                        await self.callback(LIQUIDATIONS, liq, timestamp)
+                    last_update[pair][status] = data['data'][0]['details'][0]
+                await asyncio.sleep(0.1)
             await asyncio.sleep(60)
 
-    async def _funding(self, pairs: Iterable):
+    def __reset(self):
+        self._l2_book = {}
+
+    @classmethod
+    def instrument_type(cls, symbol: str):
+        return cls.info()['instrument_type'][symbol]
+
+    async def _candle(self, msg: dict, timestamp: float):
+        '''
+        {
+            "arg": {
+                "channel": "candle1D",
+                "instId": "BTC-USD-191227"
+            },
+            "data": [
+                [
+                    "1597026383085",     // ts
+                    "8533.02",           // open
+                    "8553.74",           // high
+                    "8527.17",           // low
+                    "8548.26",           // close
+                    "45247",             // contracts, spot/margin -> amount of base ccy, derivatives -> contracts,
+                    "529.5858061"        // currency, spot/margin -> amount of quote ccy, derivatives -> amount of base ccy
+                ]
+            ]
+        }
+        '''
+        symbol = self.exchange_symbol_to_std_symbol(msg['arg']['instId'])
+        ts = int(msg['data'][0][0]) / 1_000
+
+        for entry in msg['data']:
+            candle = Candle(
+                self.id,
+                symbol,
+                ts,
+                ts + self.candle_interval_map[self.candle_interval],
+                self.candle_interval,
+                None,
+                Decimal(entry[1]),
+                Decimal(entry[4]),
+                Decimal(entry[2]),
+                Decimal(entry[3]),
+                Decimal(entry[5]),
+                Decimal(entry[6]),
+                timestamp,
+                raw=msg
+            )
+            await self.callback(CANDLES, candle, timestamp)
+
+    async def _ticker(self, msg: dict, timestamp: float):
         """
-            {
-              "success": true,
-              "result": [
+        {"arg": {"channel": "tickers", "instId": "LTC-USD-200327"}, "data": [{"instType": "SWAP","instId": "LTC-USD-SWAP","last": "9999.99","lastSz": "0.1","askPx": "9999.99","askSz": "11","bidPx": "8888.88","bidSz": "5","open24h": "9000","high24h": "10000","low24h": "8888.88","volCcy24h": "2222","vol24h": "2222","sodUtc0": "2222","sodUtc8": "2222","ts": "1597026383085"}]}
+        """
+        pair = self.exchange_symbol_to_std_symbol(msg['arg']['instId'])
+        for update in msg['data']:
+            update_timestamp = self.timestamp_normalize(int(update['ts']))
+            t = Ticker(
+                self.id,
+                pair,
+                Decimal(update['bidPx']) if update['bidPx'] else Decimal(0),
+                Decimal(update['askPx']) if update['askPx'] else Decimal(0),
+                update_timestamp,
+                raw=update
+            )
+            await self.callback(TICKER, t, timestamp)
+
+    async def _open_interest(self, msg: dict, timestamp: float):
+        """
+        {
+            'arg': {
+                'channel': 'open-interest',
+                'instId': 'BTC-USDT-SWAP
+            },
+            'data': [
                 {
-                  "future": "BTC-PERP",
-                  "rate": 0.0025,
-                  "time": "2019-06-02T08:00:00+00:00"
+                    'instId': 'BTC-USDT-SWAP',
+                    'instType': 'SWAP',
+                    'oi':'565474',
+                    'oiCcy': '5654.74',
+                    'ts': '1630338003010'
                 }
-              ]
-            }
+            ]
+        }
         """
-        while True:
-            for pair in pairs:
-                if '-PERP' not in pair:
-                    continue
-                data = await self.http_conn.read(self.rest_endpoints[0].route('funding', sandbox=self.sandbox).format(pair))
-                data = json.loads(data, parse_float=Decimal)
-                data2 = await self.http_conn.read(self.rest_endpoints[0].route('stats', sandbox=self.sandbox).format(pair))
-                data2 = json.loads(data2, parse_float=Decimal)
-                received = time()
-                data['predicted_rate'] = Decimal(data2['result']['nextFundingRate'])
-
-                last_update = self._funding_cache.get(pair, None)
-                update = str(data['result'][0]['rate']) + str(data['result'][0]['time']) + str(data['predicted_rate'])
-                if last_update and last_update == update:
-                    continue
-                else:
-                    self._funding_cache[pair] = update
-
-                f = Funding(
-                    self.id,
-                    self.exchange_symbol_to_std_symbol(data['result'][0]['future']),
-                    None,
-                    data['result'][0]['rate'],
-                    self.timestamp_normalize(data2['result']['nextFundingTime']),
-                    self.timestamp_normalize(data['result'][0]['time']),
-                    predicted_rate=data['predicted_rate'],
-                    raw=[data, data2]
-                )
-                await self.callback(FUNDING, f, received)
-                await asyncio.sleep(0.1)
-            await asyncio.sleep(60)
+        symbol = self.exchange_symbol_to_std_symbol(msg['arg']['instId'])
+        for update in msg['data']:
+            oi = OpenInterest(
+                self.id,
+                symbol,
+                Decimal(update['oi']),
+                self.timestamp_normalize(int(update['ts'])),
+                raw=update
+            )
+            await self.callback(OPEN_INTEREST, oi, timestamp)
 
     async def _trade(self, msg: dict, timestamp: float):
         """
-        example message:
-
-        {"channel": "trades", "market": "BTC-PERP", "type": "update", "data": [{"id": null, "price": 10738.75,
-        "size": 0.3616, "side": "buy", "liquidation": false, "time": "2019-08-03T12:20:19.170586+00:00"}]}
+        {
+            "arg": {
+                "channel": "trades",
+                "instId": "BTC-USD-191227"
+            },
+            "data": [
+                {
+                    "instId": "BTC-USD-191227",
+                    "tradeId": "9",
+                    "px": "0.016",
+                    "sz": "50",
+                    "side": "buy",
+                    "ts": "1597026383085"
+                }
+            ]
+        }
         """
         for trade in msg['data']:
             t = Trade(
                 self.id,
-                self.exchange_symbol_to_std_symbol(msg['market']),
+                self.exchange_symbol_to_std_symbol(trade['instId']),
                 BUY if trade['side'] == 'buy' else SELL,
-                Decimal(trade['size']),
-                Decimal(trade['price']),
-                float(self.timestamp_normalize(trade['time'])),
-                id=str(trade['id']),
+                Decimal(trade['sz']),
+                Decimal(trade['px']),
+                self.timestamp_normalize(int(trade['ts'])),
+                id=trade['tradeId'],
                 raw=trade
             )
             await self.callback(TRADES, t, timestamp)
-            if bool(trade['liquidation']):
-                liq = Liquidation(
-                    self.id,
-                    self.exchange_symbol_to_std_symbol(msg['market']),
-                    BUY if trade['side'] == 'buy' else SELL,
-                    Decimal(trade['size']),
-                    Decimal(trade['price']),
-                    str(trade['id']),
-                    FILLED,
-                    float(self.timestamp_normalize(trade['time'])),
-                    raw=trade
-                )
-                await self.callback(LIQUIDATIONS, liq, timestamp)
-
-    async def _ticker(self, msg: dict, timestamp: float):
-        """
-        example message:
 
-        {"channel": "ticker", "market": "BTC/USD", "type": "update", "data": {"bid": 10717.5, "ask": 10719.0,
-        "last": 10719.0, "time": 1564834587.1299787}}
-        """
-        t = Ticker(
-            self.id,
-            self.exchange_symbol_to_std_symbol(msg['market']),
-            Decimal(msg['data']['bid'] if msg['data']['bid'] else 0.0),
-            Decimal(msg['data']['ask'] if msg['data']['ask'] else 0.0),
-            float(msg['data']['time']),
-            raw=msg
-        )
-        await self.callback(TICKER, t, timestamp)
+    async def _funding(self, msg: dict, timestamp: float):
+        for update in msg['data']:
+            f = Funding(
+                self.id,
+                self.exchange_symbol_to_std_symbol(update['instId']),
+                None,
+                Decimal(update['fundingRate']),
+                None,
+                self.timestamp_normalize(int(update['fundingTime'])),
+                predicted_rate=Decimal(update['nextFundingRate']),
+                raw=update
+            )
+            await self.callback(FUNDING, f, timestamp)
 
     async def _book(self, msg: dict, timestamp: float):
-        """
-        example messages:
-
-        snapshot:
-        {"channel": "orderbook", "market": "BTC/USD", "type": "partial", "data": {"time": 1564834586.3382702,
-        "checksum": 427503966, "bids": [[10717.5, 4.092], ...], "asks": [[10720.5, 15.3458], ...], "action": "partial"}}
-
-        update:
-        {"channel": "orderbook", "market": "BTC/USD", "type": "update", "data": {"time": 1564834587.1299787,
-        "checksum": 3115602423, "bids": [], "asks": [[10719.0, 14.7461]], "action": "update"}}
-        """
-        check = msg['data']['checksum']
-        if msg['type'] == 'partial':
+        if msg['action'] == 'snapshot':
             # snapshot
-            pair = self.exchange_symbol_to_std_symbol(msg['market'])
-            self._l2_book[pair] = OrderBook(self.id, pair, max_depth=self.max_depth, checksum_format='FTX')
-            self._l2_book[pair].book.bids = {Decimal(price): Decimal(amount) for price, amount in msg['data']['bids']}
-            self._l2_book[pair].book.asks = {Decimal(price): Decimal(amount) for price, amount in msg['data']['asks']}
-
-            if self.checksum_validation and self._l2_book[pair].book.checksum() != check:
-                raise BadChecksum
-            await self.book_callback(L2_BOOK, self._l2_book[pair], timestamp, timestamp=float(msg['data']['time']), raw=msg, checksum=check)
+            pair = self.exchange_symbol_to_std_symbol(msg['arg']['instId'])
+            for update in msg['data']:
+                bids = {Decimal(price): Decimal(amount) for price, amount, *_ in update['bids']}
+                asks = {Decimal(price): Decimal(amount) for price, amount, *_ in update['asks']}
+                self._l2_book[pair] = OrderBook(self.id, pair, max_depth=self.max_depth, checksum_format=self.id, bids=bids, asks=asks)
+
+                if self.checksum_validation and self._l2_book[pair].book.checksum() != (update['checksum'] & 0xFFFFFFFF):
+                    raise BadChecksum
+                await self.book_callback(L2_BOOK, self._l2_book[pair], timestamp, timestamp=self.timestamp_normalize(int(update['ts'])), checksum=update['checksum'] & 0xFFFFFFFF, raw=msg)
         else:
             # update
-            delta = {BID: [], ASK: []}
-            pair = self.exchange_symbol_to_std_symbol(msg['market'])
-            for side in ('bids', 'asks'):
-                s = BID if side == 'bids' else ASK
-                for price, amount in msg['data'][side]:
-                    price = Decimal(price)
-                    amount = Decimal(amount)
-                    if amount == 0:
-                        delta[s].append((price, 0))
-                        del self._l2_book[pair].book[s][price]
-                    else:
-                        delta[s].append((price, amount))
-                        self._l2_book[pair].book[s][price] = amount
-            if self.checksum_validation and self._l2_book[pair].book.checksum() != check:
-                raise BadChecksum
-            await self.book_callback(L2_BOOK, self._l2_book[pair], timestamp, timestamp=float(msg['data']['time']), raw=msg, checksum=check, delta=delta)
-
-    async def _fill(self, msg: dict, timestamp: float):
-        """
-        example message:
-        {
-            "channel": "fills",
-            "data": {
-                "fee": 78.05799225,
-                "feeRate": 0.0014,
-                "future": "BTC-PERP",
-                "id": 7828307,
-                "liquidity": "taker",
-                "market": "BTC-PERP",
-                "orderId": 38065410,
-                "tradeId": 19129310,
-                "price": 3723.75,
-                "side": "buy",
-                "size": 14.973,
-                "time": "2019-05-07T16:40:58.358438+00:00",
-                "type": "order"
-            },
-            "type": "update"
-        }
-        """
-        fill = msg['data']
-        f = Fill(
-            self.id,
-            self.exchange_symbol_to_std_symbol(fill['market']),
-            BUY if fill['side'] == 'buy' else SELL,
-            Decimal(fill['size']),
-            Decimal(fill['price']),
-            Decimal(fill['fee']),
-            str(fill['tradeId']),
-            str(fill['orderId']),
-            None,
-            TAKER if fill['liquidity'] == 'taker' else MAKER,
-            fill['time'].timestamp(),
-            account=self.subaccount,
-            raw=msg
-        )
-        await self.callback(FILLS, f, timestamp)
+            pair = self.exchange_symbol_to_std_symbol(msg['arg']['instId'])
+            for update in msg['data']:
+                delta = {BID: [], ASK: []}
+
+                for side in ('bids', 'asks'):
+                    s = BID if side == 'bids' else ASK
+                    for price, amount, *_ in update[side]:
+                        price = Decimal(price)
+                        amount = Decimal(amount)
+                        if amount == 0:
+                            if price in self._l2_book[pair].book[s]:
+                                delta[s].append((price, 0))
+                                del self._l2_book[pair].book[s][price]
+                        else:
+                            delta[s].append((price, amount))
+                            self._l2_book[pair].book[s][price] = amount
+                if self.checksum_validation and self._l2_book[pair].book.checksum() != (update['checksum'] & 0xFFFFFFFF):
+                    raise BadChecksum
+                await self.book_callback(L2_BOOK, self._l2_book[pair], timestamp, timestamp=self.timestamp_normalize(int(update['ts'])), raw=msg, delta=delta, checksum=update['checksum'] & 0xFFFFFFFF)
 
     async def _order(self, msg: dict, timestamp: float):
-        """
-        example message:
+        '''
         {
+          "arg": {
             "channel": "orders",
-            "data": {
-                "id": 24852229,
-                "clientId": null,
-                "market": "XRP-PERP",
-                "type": "limit",
-                "side": "buy",
-                "size": 42353.0,
-                "price": 0.2977,
-                "reduceOnly": false,
-                "ioc": false,
-                "postOnly": false,
-                "status": "closed",
-                "filledSize": 0.0,
-                "remainingSize": 0.0,
-                "avgFillPrice": 0.2978
-            },
-            "type": "update"
+            "instType": "FUTURES",
+            "instId": "BTC-USD-200329"
+          },
+          "data": [
+            {
+              "instType": "FUTURES",
+              "instId": "BTC-USD-200329",
+              "ccy": "BTC",
+              "ordId": "312269865356374016",
+              "clOrdId": "b1",
+              "tag": "",
+              "px": "999",
+              "sz": "333",
+              "notionalUsd": "",
+              "ordType": "limit",
+              "side": "buy",
+              "posSide": "long",
+              "tdMode": "cross",
+              "tgtCcy": "",
+              "fillSz": "0",
+              "fillPx": "long",
+              "tradeId": "0",
+              "accFillSz": "323",
+              "fillNotionalUsd": "",
+              "fillTime": "0",
+              "fillFee": "0.0001",
+              "fillFeeCcy": "BTC",
+              "execType": "T",
+              "state": "canceled",
+              "avgPx": "0",
+              "lever": "20",
+              "tpTriggerPx": "0",
+              "tpOrdPx": "20",
+              "slTriggerPx": "0",
+              "slOrdPx": "20",
+              "feeCcy": "",
+              "fee": "",
+              "rebateCcy": "",
+              "rebate": "",
+              "tgtCcy":"",
+              "pnl": "",
+              "category": "",
+              "uTime": "1597026383085",
+              "cTime": "1597026383085",
+              "reqId": "",
+              "amendResult": "",
+              "code": "0",
+              "msg": ""
+            }
+          ]
         }
-        """
-        order = msg['data']
-        status = order['status']
-        if status == 'new':
-            status = SUBMITTING
-        elif status == 'open':
-            status = OPEN
-        elif status == 'closed':
-            status = CLOSED
+        '''
+        status = msg['data'][0]['state']
+        if status == 'canceled':
+            status == CANCELLED
+        elif status == 'live':
+            status == OPEN
+        elif status == 'partially-filled':
+            status = PARTIAL
+        elif status == 'filled':
+            status = FILLED
+
+        o_type = msg['data'][0]['ordType']
+        if o_type == 'market':
+            o_type = MARKET
+        elif o_type == 'post_only':
+            o_type = MAKER_OR_CANCEL
+        elif o_type == 'fok':
+            o_type = FILL_OR_KILL
+        elif o_type == 'ioc':
+            o_type = IMMEDIATE_OR_CANCEL
+        elif o_type == 'limit':
+            o_type = LIMIT
 
         oi = OrderInfo(
             self.id,
-            self.exchange_symbol_to_std_symbol(order['market']),
-            str(order['id']),
-            BUY if order['side'].lower() == 'buy' else SELL,
+            self.exchange_symbol_to_std_symbol(msg['data'][0]['instId'].upper()),
+            msg['data'][0]['ordId'],
+            BUY if msg['data'][0]['side'].lower() == 'buy' else SELL,
             status,
-            LIMIT if order['type'] == 'limit' else MARKET,
-            Decimal(order['price']) if order['price'] else None,
-            Decimal(order['filledSize']),
-            Decimal(order['remainingSize']),
-            timestamp=str(order['createdAt']),
-            client_order_id=str(order['clientId']),
-            account=self.subaccount,
+            o_type,
+            Decimal(msg['data'][0]['px']) if msg['data'][0]['px'] else Decimal(msg['data'][0]['avgPx']),
+            Decimal(msg['data'][0]['sz']),
+            Decimal(msg['data'][0]['sz']) - Decimal(msg['data'][0]['accFillSz']) if msg['data'][0]['accFillSz'] else Decimal(msg['data'][0]['sz']),
+            self.timestamp_normalize(int(msg['data'][0]['uTime'])),
             raw=msg
         )
         await self.callback(ORDER_INFO, oi, timestamp)
 
+    async def _login(self, msg: dict, timestamp: float):
+        LOG.debug('%s: Websocket logged in? %s', self.id, msg['code'])
+
     async def message_handler(self, msg: str, conn, timestamp: float):
+        # DEFLATE compression, no header
+        # msg = zlib.decompress(msg, -15)
+        # not required, as websocket now set to "Per-Message Deflate"
         msg = json.loads(msg, parse_float=Decimal)
-        if 'type' in msg:
-            if msg['type'] == 'subscribed':
-                if 'market' in msg:
-                    LOG.info('%s: Subscribed to %s channel for %s', self.id, msg['channel'], msg['market'])
-                else:
-                    LOG.info('%s: Subscribed to %s channel', self.id, msg['channel'])
-            elif msg['type'] == 'error':
-                LOG.error('%s: Received error message %s', self.id, msg)
-                raise Exception('Error from %s: %s', self.id, msg)
-            elif 'channel' in msg:
-                if msg['channel'] == 'orderbook':
-                    await self._book(msg, timestamp)
-                elif msg['channel'] == 'trades':
-                    await self._trade(msg, timestamp)
-                elif msg['channel'] == 'ticker':
-                    await self._ticker(msg, timestamp)
-                elif msg['channel'] == 'fills':
-                    await self._fill(msg, timestamp)
-                elif msg['channel'] == 'orders':
-                    await self._order(msg, timestamp)
-                else:
-                    LOG.warning("%s: Invalid message type %s", self.id, msg)
+
+        if 'event' in msg:
+            if msg['event'] == 'error':
+                LOG.error("%s: Error: %s", self.id, msg)
+            elif msg['event'] == 'subscribe':
+                pass
+            elif msg['event'] == 'login':
+                await self._login(msg, timestamp)
             else:
-                LOG.warning("%s: Invalid message type %s", self.id, msg)
+                LOG.warning("%s: Unhandled event %s", self.id, msg)
+        elif 'arg' in msg:
+            if self.websocket_channels[L2_BOOK] in msg['arg']['channel']:
+                await self._book(msg, timestamp)
+            elif self.websocket_channels[TICKER] in msg['arg']['channel']:
+                await self._ticker(msg, timestamp)
+            elif self.websocket_channels[TRADES] in msg['arg']['channel']:
+                await self._trade(msg, timestamp)
+            elif self.websocket_channels[FUNDING] in msg['arg']['channel']:
+                await self._funding(msg, timestamp)
+            elif self.websocket_channels[ORDER_INFO] in msg['arg']['channel']:
+                await self._order(msg, timestamp)
+            elif self.websocket_channels[OPEN_INTEREST] in msg['arg']['channel']:
+                await self._open_interest(msg, timestamp)
+            elif self.websocket_channels[CANDLES] in msg['arg']['channel']:
+                await self._candle(msg, timestamp)
         else:
-            LOG.warning("%s: Invalid message type %s", self.id, msg)
+            LOG.warning("%s: Unhandled message %s", self.id, msg)
+
+    async def subscribe(self, connection: AsyncConnection):
+        channels = []
+        for chan in self.subscription:
+            if chan == LIQUIDATIONS:
+                asyncio.create_task(self._liquidations(self.subscription[chan]))
+                continue
+            for pair in self.subscription[chan]:
+                channels.append(self.build_subscription(chan, pair))
+
+            msg = {"op": "subscribe", "args": channels}
+            await connection.write(json.dumps(msg))
+
+    async def authenticate(self, conn: AsyncConnection):
+        if self.requires_authentication:
+            if any([self.is_authenticated_channel(self.exchange_channel_to_std(chan)) for chan in conn.subscription]):
+                auth = self._auth(self.key_id, self.key_secret)
+                LOG.debug(f"{conn.uuid}: Authenticating with message: {auth}")
+                await conn.write(json.dumps(auth))
+                await asyncio.sleep(1)
+
+    def _auth(self, key_id, key_secret) -> str:
+        timestamp, sign = self._generate_token(key_id, key_secret)
+        login_param = {"op": "login", "args": [{"apiKey": self.key_id, "passphrase": self.key_passphrase, "timestamp": timestamp, "sign": sign.decode("utf-8")}]}
+        return login_param
+
+    def build_subscription(self, channel: str, ticker: str) -> dict:
+        if channel in ['positions', 'orders']:
+            subscription_dict = {"channel": channel,
+                                 "instType": self.inst_type_to_okx_type(ticker),
+                                 "instId": ticker}
+        elif channel in ['candle']:
+            subscription_dict = {"channel": f"{channel}{self.candle_interval}",
+                                 "instId": ticker}
+        else:
+            subscription_dict = {"channel": channel,
+                                 "instId": ticker}
+        return subscription_dict
+
+    def inst_type_to_okx_type(self, ticker):
+        sym = self.exchange_symbol_to_std_symbol(ticker)
+        instrument_type = self.instrument_type(sym)
+        instrument_type_map = {
+            'perpetual': 'SWAP',
+            'spot': 'MARGIN',
+            'futures': 'FUTURES',
+            'option': 'OPTION'
+        }
+        return instrument_type_map.get(instrument_type, 'MARGIN')
+
+    def _get_server_time(self):
+        endpoint = "public/time"
+        response = requests.get(self.api + endpoint)
+        if response.status_code == 200:
+            return response.json()['data'][0]['ts']
+        else:
+            return ""
+
+    def _server_timestamp(self):
+        server_time = self._get_server_time()
+        return int(server_time) / 1000
+
+    def _create_sign(self, timestamp: str, key_secret: str):
+        message = timestamp + 'GET' + '/users/self/verify'
+        mac = hmac.new(bytes(key_secret, encoding='utf8'), bytes(message, encoding='utf-8'), digestmod='sha256')
+        d = mac.digest()
+        sign = base64.b64encode(d)
+        return sign
+
+    def _generate_token(self, key_id: str, key_secret: str) -> dict:
+        timestamp = str(self._server_timestamp())
+        sign = self._create_sign(timestamp, key_secret)
+        return timestamp, sign
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/gateio.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/gateio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from collections import defaultdict
 import logging
 from decimal import Decimal
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/gemini.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/gemini.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from collections import defaultdict
 import logging
 from decimal import Decimal
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/hitbtc.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/hitbtc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import logging
 from cryptofeed.connection import RestEndpoint, Routes, WebsocketEndpoint
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/huobi.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/huobi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from cryptofeed.symbols import Symbol
 from cryptofeed.util.time import timedelta_str_to_sec
 import logging
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/huobi_dm.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/huobi_dm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from collections import defaultdict
 from cryptofeed.symbols import Symbol
 import logging
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/huobi_swap.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/huobi_swap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 from collections import defaultdict
 from cryptofeed.symbols import Symbol, str_to_symbol
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/independent_reserve.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/independent_reserve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 from decimal import Decimal
 import logging
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/kraken.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/kraken.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from decimal import Decimal
 from collections import defaultdict
 import logging
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/kraken_futures.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/kraken_futures.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from collections import defaultdict
 from cryptofeed.symbols import Symbol
 import logging
@@ -59,15 +59,15 @@
             ftype, symbol = entry['symbol'].upper().split("_", maxsplit=1)
             stype = PERPETUAL
             expiry = None
             if "_" in symbol:
                 stype = FUTURES
                 symbol, expiry = symbol.split("_")
             symbol = symbol.replace('XBT', 'BTC')
-            base, quote = symbol[:3], symbol[3:]
+            base, quote = symbol[:len(symbol) - 3], symbol[-3:]
 
             s = Symbol(base, quote, type=stype, expiry_date=expiry)
 
             info['tick_size'][s.normalized] = entry['tickSize']
             info['contract_size'][s.normalized] = entry['contractSize']
             info['underlying'][s.normalized] = entry.get('underlying')
             info['product_type'][s.normalized] = _kraken_futures_product_type[ftype]
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/kucoin.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/kucoin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from decimal import Decimal
 import logging
 import time
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/mixins/binance_rest.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/mixins/binance_rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 from decimal import Decimal
 import hashlib
@@ -216,7 +216,14 @@
 
 
 class BinanceUSRestMixin(BinanceRestMixin):
     api = 'https://api.binance.us/api/v3/'
     rest_channels = (
         TRADES
     )
+
+
+class BinanceTRRestMixin(BinanceRestMixin):
+    api = 'https://api.binance.me/api/v3/'
+    rest_channels = (
+        TRADES
+    )
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/mixins/bitfinex_rest.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/mixins/bitfinex_rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 import hashlib
 import hmac
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/mixins/bitmex_rest.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/mixins/bitmex_rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import decimal
 import hashlib
 import hmac
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/mixins/bitstamp_rest.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/mixins/bitstamp_rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 from decimal import Decimal
 import logging
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/mixins/coinbase_rest.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/mixins/coinbase_rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 import base64
 from cryptofeed.util.time import timedelta_str_to_sec
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/mixins/deribit_rest.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/mixins/deribit_rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 from decimal import Decimal
 import logging
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/mixins/dydx_rest.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/mixins/dydx_rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from decimal import Decimal
 import logging
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/mixins/gemini_rest.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/mixins/gemini_rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 from decimal import Decimal
 import logging
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/mixins/kraken_rest.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/mixins/kraken_rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 import base64
 import hashlib
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/mixins/okx_rest.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/mixins/okx_rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 from decimal import Decimal
 import logging
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/mixins/upbit_rest.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/mixins/upbit_rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 from decimal import Decimal
 import logging
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/okcoin.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/okcoin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from collections import defaultdict
 from decimal import Decimal
 import logging
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/phemex.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/phemex.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import hmac
 import time
 from collections import defaultdict
@@ -11,15 +11,15 @@
 import logging
 from decimal import Decimal
 from typing import Dict, Tuple
 
 from yapic import json
 
 from cryptofeed.connection import AsyncConnection, RestEndpoint, Routes, WebsocketEndpoint
-from cryptofeed.defines import BALANCES, BID, ASK, BUY, CANDLES, PHEMEX, L2_BOOK, SELL, TRADES
+from cryptofeed.defines import BALANCES, BID, ASK, BUY, CANDLES, PHEMEX, L2_BOOK, SELL, TRADES, PERPETUAL
 from cryptofeed.feed import Feed
 from cryptofeed.types import OrderBook, Trade, Candle, Balance
 
 LOG = logging.getLogger('feedhandler')
 
 
 class Phemex(Feed):
@@ -46,14 +46,16 @@
         ret = {}
         info = defaultdict(dict)
 
         for entry in data['data']['products']:
             if entry['status'] != 'Listed':
                 continue
             stype = entry['type'].lower()
+            if "perpetual" in stype:    # can be "perpetualv2"
+                stype = PERPETUAL
             base, quote = entry['displaySymbol'].split("/")
             s = Symbol(base.strip(), quote.strip(), type=stype)
             ret[s.normalized] = entry['symbol']
             info['tick_size'][s.normalized] = entry['tickSize'] if 'tickSize' in entry else entry['quoteTickSize']
             info['instrument_type'][s.normalized] = stype
             # the price scale for spot symbols is not reported via the API but it is documented
             # here in the API docs: https://github.com/phemex/phemex-api-docs/blob/master/Public-Spot-API-en.md#spot-currency-and-symbols
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/poloniex.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/poloniex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import logging
 from decimal import Decimal
 from typing import Dict, Tuple
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/probit.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/probit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import logging
 from decimal import Decimal
 from typing import Dict, Tuple
```

### Comparing `cryptofeed-2.3.1/cryptofeed/exchanges/upbit.py` & `cryptofeed-2.3.2/cryptofeed/exchanges/upbit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import logging
 from decimal import Decimal
 from typing import Dict, Tuple
```

### Comparing `cryptofeed-2.3.1/cryptofeed/feed.py` & `cryptofeed-2.3.2/cryptofeed/feed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 from collections import defaultdict
 import logging
@@ -269,16 +269,15 @@
     async def shutdown(self):
         LOG.info('%s: feed shutdown starting...', self.id)
         await self.http_conn.close()
 
         for callbacks in self.callbacks.values():
             for callback in callbacks:
                 if hasattr(callback, 'stop'):
-                    cb_name = callback.__class__.__name__ if hasattr(callback, '__class__') else callback.__name__
-                    LOG.info('%s: stopping backend %s', self.id, cb_name)
+                    LOG.info('%s: stopping backend %s', self.id, self.backend_name(callback))
                     await callback.stop()
         for c in self.connection_handlers:
             await c.conn.close()
         LOG.info('%s: feed shutdown completed', self.id)
 
     def stop(self):
         for c in self.connection_handlers:
@@ -291,11 +290,17 @@
         for conn, sub, handler, auth in self.connect():
             self.connection_handlers.append(ConnectionHandler(conn, sub, handler, auth, self.retries, timeout=self.timeout, timeout_interval=self.timeout_interval, exceptions=self.exceptions, log_on_error=self.log_on_error, start_delay=self.start_delay))
             self.connection_handlers[-1].start(loop)
 
         for callbacks in self.callbacks.values():
             for callback in callbacks:
                 if hasattr(callback, 'start'):
-                    cb_name = callback.__class__.__name__ if hasattr(callback, '__class__') else callback.__name__
-                    LOG.info('%s: starting backend task %s with multiprocessing=%s', self.id, cb_name, 'True' if self.config.backend_multiprocessing else 'False')
+                    LOG.info('%s: starting backend task %s with multiprocessing=%s', self.id, self.backend_name(callback), 'True' if self.config.backend_multiprocessing else 'False')
                     # Backends start tasks to write messages
                     callback.start(loop, multiprocess=self.config.backend_multiprocessing)
+
+    def backend_name(self, callback):
+        if hasattr(callback, '__class__'):
+            if hasattr(callback, 'handler'):
+                return callback.handler.__class__.__name__ + "+" + callback.__class__.__name__
+            return callback.__class__.__name__
+        return callback.__name__
```

### Comparing `cryptofeed-2.3.1/cryptofeed/feedhandler.py` & `cryptofeed-2.3.2/cryptofeed/feedhandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 from cryptofeed.connection import Connection
 import logging
```

### Comparing `cryptofeed-2.3.1/cryptofeed/log.py` & `cryptofeed-2.3.2/cryptofeed/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import logging
 from logging.handlers import RotatingFileHandler
```

### Comparing `cryptofeed-2.3.1/cryptofeed/nbbo.py` & `cryptofeed-2.3.2/cryptofeed/nbbo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 
 from cryptofeed.callback import Callback
```

### Comparing `cryptofeed-2.3.1/cryptofeed/raw_data_collection.py` & `cryptofeed-2.3.2/cryptofeed/raw_data_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import asyncio
 import atexit
 from collections import defaultdict
```

### Comparing `cryptofeed-2.3.1/cryptofeed/symbols.py` & `cryptofeed-2.3.2/cryptofeed/symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from datetime import datetime as dt, timezone
 from typing import Dict, Tuple, Union
```

### Comparing `cryptofeed-2.3.1/cryptofeed/types.c` & `cryptofeed-2.3.2/cryptofeed/types.c`

 * *Files 0% similar despite different names*

```diff
@@ -2393,15 +2393,15 @@
 static const char __pyx_k_to_dict_locals_helper[] = "to_dict.<locals>.helper";
 static const char __pyx_k_pyx_unpickle_OrderBook[] = "__pyx_unpickle_OrderBook";
 static const char __pyx_k_pyx_unpickle_OrderInfo[] = "__pyx_unpickle_OrderInfo";
 static const char __pyx_k_COMPILED_WITH_ASSERTIONS[] = "COMPILED_WITH_ASSERTIONS";
 static const char __pyx_k_pyx_unpickle_Liquidation[] = "__pyx_unpickle_Liquidation";
 static const char __pyx_k_pyx_unpickle_Transaction[] = "__pyx_unpickle_Transaction";
 static const char __pyx_k_pyx_unpickle_OpenInterest[] = "__pyx_unpickle_OpenInterest";
-static const char __pyx_k_Copyright_C_2017_2022_Bryant_Mo[] = "\nCopyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com\n\nPlease see the LICENSE file for the terms and conditions\nassociated with this software.\n";
+static const char __pyx_k_Copyright_C_2017_2023_Bryant_Mo[] = "\nCopyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com\n\nPlease see the LICENSE file for the terms and conditions\nassociated with this software.\n";
 static const char __pyx_k_Incompatible_checksums_s_vs_0x11[] = "Incompatible checksums (%s vs 0x115d197 = (amount, currency, exchange, raw, status, timestamp, type))";
 static const char __pyx_k_Incompatible_checksums_s_vs_0x28[] = "Incompatible checksums (%s vs 0x28c632c = (close, closed, exchange, high, interval, low, open, raw, start, stop, symbol, timestamp, trades, volume))";
 static const char __pyx_k_Incompatible_checksums_s_vs_0x39[] = "Incompatible checksums (%s vs 0x394a8c9 = (amount, exchange, id, price, raw, side, symbol, timestamp, type))";
 static const char __pyx_k_Incompatible_checksums_s_vs_0x3b[] = "Incompatible checksums (%s vs 0x3b08dc7 = (account, amount, client_order_id, exchange, id, price, raw, remaining, side, status, symbol, timestamp, type))";
 static const char __pyx_k_Incompatible_checksums_s_vs_0x3f[] = "Incompatible checksums (%s vs 0x3f6b4bc = (balance, currency, exchange, raw, reserved))";
 static const char __pyx_k_Incompatible_checksums_s_vs_0x4f[] = "Incompatible checksums (%s vs 0x4f31878 = (exchange, id, price, quantity, raw, side, status, symbol, timestamp))";
 static const char __pyx_k_Incompatible_checksums_s_vs_0x5b[] = "Incompatible checksums (%s vs 0x5b8ec65 = (exchange, mark_price, next_funding_time, predicted_rate, rate, raw, symbol, timestamp))";
@@ -45338,15 +45338,15 @@
   {0, NULL}
 };
 #endif
 
 static struct PyModuleDef __pyx_moduledef = {
     PyModuleDef_HEAD_INIT,
     "types",
-    __pyx_k_Copyright_C_2017_2022_Bryant_Mo, /* m_doc */
+    __pyx_k_Copyright_C_2017_2023_Bryant_Mo, /* m_doc */
   #if CYTHON_PEP489_MULTI_PHASE_INIT
     0, /* m_size */
   #else
     -1, /* m_size */
   #endif
     __pyx_methods /* m_methods */,
   #if CYTHON_PEP489_MULTI_PHASE_INIT
@@ -46250,15 +46250,15 @@
   #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("types", __pyx_methods, __pyx_k_Copyright_C_2017_2022_Bryant_Mo, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  __pyx_m = Py_InitModule4("types", __pyx_methods, __pyx_k_Copyright_C_2017_2023_Bryant_Mo, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   #endif
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
@@ -46776,15 +46776,15 @@
   __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_10cryptofeed_5types_29__pyx_unpickle_Position, NULL, __pyx_n_s_cryptofeed_types); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_Position, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "cryptofeed/types.pyx":1
  * '''             # <<<<<<<<<<<<<<
- * Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+ * Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
  * 
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
```

### Comparing `cryptofeed-2.3.1/cryptofeed/types.pyx` & `cryptofeed-2.3.2/cryptofeed/types.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 cimport cython
 from decimal import Decimal
```

### Comparing `cryptofeed-2.3.1/cryptofeed/util/book.py` & `cryptofeed-2.3.2/cryptofeed/util/book.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 from cryptofeed.defines import BID, ASK, L2_BOOK
```

### Comparing `cryptofeed-2.3.1/cryptofeed/util/perf.py` & `cryptofeed-2.3.2/cryptofeed/util/perf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 
 
 This file contains helper functions for performance instrumentation
 '''
```

### Comparing `cryptofeed-2.3.1/cryptofeed/util/split.py` & `cryptofeed-2.3.2/cryptofeed/util/split.py`

 * *Files identical despite different names*

### Comparing `cryptofeed-2.3.1/cryptofeed/util/time.py` & `cryptofeed-2.3.2/cryptofeed/util/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 
 
 def timedelta_str_to_sec(td: str):
```

### Comparing `cryptofeed-2.3.1/cryptofeed.egg-info/PKG-INFO` & `cryptofeed-2.3.2/cryptofeed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cryptofeed
-Version: 2.3.1
+Version: 2.3.2
 Summary: Cryptocurrency Exchange Websocket Data Feed Handler
 Home-page: https://github.com/bmoscon/cryptofeed
 Author: Bryant Moscon
 Author-email: bmoscon@gmail.com
 License: XFree86
-Keywords: cryptocurrency,bitcoin,btc,feed handler,market feed,market data,crypto assets,Trades,Tickers,BBO,Funding,Open Interest,Liquidation,Order book,Bid,Ask,fmfw.io,Bitfinex,bitFlyer,AscendEX,Bitstamp,Bittrex,Blockchain.com,Bybit,Binance,Binance Delivery,Binance Futures,Binance US,BitMEX,Coinbase,Deribit,EXX,FTX,FTX US,Gate.io,Gemini,HitBTC,Huobi,Huobi DM,Huobi Swap,Kraken,Kraken Futures,OKCoin,OKX,Poloniex,ProBit,Upbit
+Keywords: cryptocurrency,bitcoin,btc,feed handler,market feed,market data,crypto assets,Trades,Tickers,BBO,Funding,Open Interest,Liquidation,Order book,Bid,Ask,fmfw.io,Bitfinex,bitFlyer,AscendEX,Bitstamp,Bittrex,Blockchain.com,Bybit,Binance,Binance Delivery,Binance Futures,Binance US,BitMEX,Coinbase,Deribit,EXX,Gate.io,Gemini,HitBTC,Huobi,Huobi DM,Huobi Swap,Kraken,Kraken Futures,OKCoin,OKX,Poloniex,ProBit,Upbit
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -59,16 +59,14 @@
 * [Coinbase](https://www.coinbase.com/)
 * [Crypto.com](https://www.crypto.com)
 * [Delta](https://www.delta.exchange/)
 * [Deribit](https://www.deribit.com/)
 * [dYdX](https://dydx.exchange/)
 * [FMFW.io](https://www.fmfw.io/)
 * [EXX](https://www.exx.com/)
-* [FTX](https://ftx.com/)
-* [FTX US](https://ftx.us/)
 * [Gate.io](https://www.gate.io/)
 * [Gemini](https://gemini.com/)
 * [HitBTC](https://hitbtc.com/)
 * [Huobi](https://www.hbg.com/)
 * [Huobi DM](https://www.huobi.com/en-us/markets/hb_dm/)
 * Huobi Swap (Coin-M and USDT-M)
 * [Independent Reserve](https://www.independentreserve.com/) 
@@ -296,14 +294,27 @@
 Your Pull Requests are also welcome, even for minor changes.
 
 
 ----
 
 ## Changelog
 
+### 2.3.2 (2023-05-27)
+ * Bugfix: Fix Socket backend
+ * Bugfix: Fix AUCTION symbol parsing on Coinbase
+ * Bugfix: Fix PERPETUAL symbol parsing on Phemex
+ * Bugfix: Fix PERPETUAL symbol parsing on Kraken Futures
+ * Feature: Access to all AIOKafka configuration options
+ * Feature: Use backend Queue for Kafka
+ * Feature: Add support for storing book snapshots in Redis as key-value
+ * Update: Switch from unmaintained aioredis to redis-py
+ * Bugfix: Correct value for Crypto.com Ask price
+ * Update: Remove cChardet dependency
+ * Feature: Binance TR support
+
 ### 2.3.1 (2022-10-31)
  * Bugfix: timestamp not reset correctly on reconnect
  * Bugfix: Arctic backend failing to write Trades when trade type was not present in data
  * Bugfix: Timestamp sometimes not present in Coinbase ticker updates
  * Bugfix: Phemex, symbols parsing
  * Bugfix: OKx - handle empty liquidations correctly
```

### Comparing `cryptofeed-2.3.1/cryptofeed.egg-info/SOURCES.txt` & `cryptofeed-2.3.2/cryptofeed.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 cryptofeed/exchanges/__init__.py
 cryptofeed/exchanges/ascendex.py
 cryptofeed/exchanges/ascendex_futures.py
 cryptofeed/exchanges/bequant.py
 cryptofeed/exchanges/binance.py
 cryptofeed/exchanges/binance_delivery.py
 cryptofeed/exchanges/binance_futures.py
+cryptofeed/exchanges/binance_tr.py
 cryptofeed/exchanges/binance_us.py
 cryptofeed/exchanges/bitdotcom.py
 cryptofeed/exchanges/bitfinex.py
 cryptofeed/exchanges/bitflyer.py
 cryptofeed/exchanges/bitget.py
 cryptofeed/exchanges/bithumb.py
 cryptofeed/exchanges/bitmex.py
@@ -64,17 +65,14 @@
 cryptofeed/exchanges/coinbase.py
 cryptofeed/exchanges/cryptodotcom.py
 cryptofeed/exchanges/delta.py
 cryptofeed/exchanges/deribit.py
 cryptofeed/exchanges/dydx.py
 cryptofeed/exchanges/exx.py
 cryptofeed/exchanges/fmfw.py
-cryptofeed/exchanges/ftx.py
-cryptofeed/exchanges/ftx_tr.py
-cryptofeed/exchanges/ftx_us.py
 cryptofeed/exchanges/gateio.py
 cryptofeed/exchanges/gemini.py
 cryptofeed/exchanges/hitbtc.py
 cryptofeed/exchanges/huobi.py
 cryptofeed/exchanges/huobi_dm.py
 cryptofeed/exchanges/huobi_swap.py
 cryptofeed/exchanges/independent_reserve.py
@@ -91,17 +89,14 @@
 cryptofeed/exchanges/mixins/binance_rest.py
 cryptofeed/exchanges/mixins/bitfinex_rest.py
 cryptofeed/exchanges/mixins/bitmex_rest.py
 cryptofeed/exchanges/mixins/bitstamp_rest.py
 cryptofeed/exchanges/mixins/coinbase_rest.py
 cryptofeed/exchanges/mixins/deribit_rest.py
 cryptofeed/exchanges/mixins/dydx_rest.py
-cryptofeed/exchanges/mixins/ftx_rest.py
-cryptofeed/exchanges/mixins/ftx_rest_tr.py
-cryptofeed/exchanges/mixins/ftx_rest_us.py
 cryptofeed/exchanges/mixins/gemini_rest.py
 cryptofeed/exchanges/mixins/kraken_rest.py
 cryptofeed/exchanges/mixins/okx_rest.py
 cryptofeed/exchanges/mixins/upbit_rest.py
 cryptofeed/util/__init__.py
 cryptofeed/util/book.py
 cryptofeed/util/perf.py
```

### Comparing `cryptofeed-2.3.1/pyproject.toml` & `cryptofeed-2.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cryptofeed-2.3.1/setup.py` & `cryptofeed-2.3.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-Copyright (C) 2017-2022 Bryant Moscon - bmoscon@gmail.com
+Copyright (C) 2017-2023 Bryant Moscon - bmoscon@gmail.com
 
 Please see the LICENSE file for the terms and conditions
 associated with this software.
 '''
 import os
 import sys
 
@@ -42,26 +42,26 @@
 extension = Extension("cryptofeed.types", ["cryptofeed/types.pyx"],
                       extra_compile_args=extra_compile_args,
                       define_macros=define_macros)
 
 setup(
     name="cryptofeed",
     ext_modules=cythonize([extension], language_level=3, force=True),
-    version="2.3.1",
+    version="2.3.2",
     author="Bryant Moscon",
     author_email="bmoscon@gmail.com",
     description="Cryptocurrency Exchange Websocket Data Feed Handler",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     license="XFree86",
     keywords=["cryptocurrency", "bitcoin", "btc", "feed handler", "market feed", "market data", "crypto assets",
               "Trades", "Tickers", "BBO", "Funding", "Open Interest", "Liquidation", "Order book", "Bid", "Ask",
               "fmfw.io", "Bitfinex", "bitFlyer", "AscendEX", "Bitstamp", "Bittrex", "Blockchain.com", "Bybit",
               "Binance", "Binance Delivery", "Binance Futures", "Binance US", "BitMEX", "Coinbase", "Deribit", "EXX",
-              "FTX", "FTX US", "Gate.io", "Gemini", "HitBTC", "Huobi", "Huobi DM", "Huobi Swap", "Kraken",
+              "Gate.io", "Gemini", "HitBTC", "Huobi", "Huobi DM", "Huobi Swap", "Kraken",
               "Kraken Futures", "OKCoin", "OKX", "Poloniex", "ProBit", "Upbit"],
     url="https://github.com/bmoscon/cryptofeed",
     packages=find_packages(exclude=['tests*']),
     cmdclass={'test': Test},
     python_requires='>=3.8',
     classifiers=[
         "Intended Audience :: Developers",
@@ -73,40 +73,38 @@
         "Framework :: AsyncIO",
     ],
     tests_require=["pytest"],
     install_requires=[
         "requests>=2.18.4",
         "websockets>=10.0",
         "pyyaml",
-        "aiohttp==3.8.3",
+        "aiohttp==3.8.4",
         "aiofile>=2.0.0",
         "yapic.json>=1.6.3",
         'uvloop ; platform_system!="Windows"',
-        # Two (optional) dependencies that speed up Cryptofeed:
-        "aiodns>=1.1",  # aiodns speeds up DNS resolving
-        "cchardet",  # cchardet is a faster replacement for chardet
-        "order_book>=0.6.0"
+        "order_book>=0.6.0",
+        "aiodns>=1.1"  # aiodns speeds up DNS resolving
     ],
     extras_require={
         "arctic": ["arctic", "pandas"],
         "gcp_pubsub": ["google_cloud_pubsub>=2.4.1", "gcloud_aio_pubsub"],
         "kafka": ["aiokafka>=0.7.0"],
         "mongo": ["motor"],
         "postgres": ["asyncpg"],
         "rabbit": ["aio_pika", "pika"],
-        "redis": ["hiredis", "aioredis>=2.0.0"],
+        "redis": ["hiredis", "redis>=4.5.1"],
         "zmq": ["pyzmq"],
         "all": [
             "arctic",
             "google_cloud_pubsub>=2.4.1",
             "gcloud_aio_pubsub",
             "aiokafka>=0.7.0",
             "motor",
             "asyncpg",
             "aio_pika",
             "pika",
             "hiredis",
-            "aioredis>=2.0.0",
+            "redis>=4.5.1",
             "pyzmq",
         ],
     },
 )
```

