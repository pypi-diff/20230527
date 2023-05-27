# Comparing `tmp/tsetmc_api-5.0.4.tar.gz` & `tmp/tsetmc_api-5.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsetmc_api-5.0.4.tar", max compression
+gzip compressed data, was "tsetmc_api-5.0.5.tar", max compression
```

## Comparing `tsetmc_api-5.0.4.tar` & `tsetmc_api-5.0.5.tar`

### file list

```diff
@@ -1,41 +1,40 @@
--rw-r--r--   0        0        0     1098 2022-12-09 11:30:04.936894 tsetmc_api-5.0.4/LICENSE
--rw-r--r--   0        0        0     1846 2022-12-09 11:30:04.936894 tsetmc_api-5.0.4/README.md
--rw-r--r--   0        0        0        0 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/__init__.py
--rw-r--r--   0        0        0       36 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/day_details/__init__.py
--rw-r--r--   0        0        0     7677 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/day_details/_core.py
--rw-r--r--   0        0        0     5717 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/day_details/day_details.py
--rw-r--r--   0        0        0      438 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/day_details/orderbook.py
--rw-r--r--   0        0        0      460 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/day_details/price.py
--rw-r--r--   0        0        0     1642 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/day_details/shareholder.py
--rw-r--r--   0        0        0      114 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/day_details/threshold.py
--rw-r--r--   0        0        0      215 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/day_details/trade.py
--rw-r--r--   0        0        0      368 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/day_details/traders_type.py
--rw-r--r--   0        0        0       36 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/group/__init__.py
--rw-r--r--   0        0        0      313 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/group/_core.py
--rw-r--r--   0        0        0      739 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/group/group.py
--rw-r--r--   0        0        0       36 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/market_map/__init__.py
--rw-r--r--   0        0        0     1213 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/market_map/_core.py
--rw-r--r--   0        0        0     1628 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/market_map/map.py
--rw-r--r--   0        0        0       31 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/market_watch/__init__.py
--rw-r--r--   0        0        0    17109 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/market_watch/_core.py
--rw-r--r--   0        0        0      224 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/market_watch/daily_history.py
--rw-r--r--   0        0        0      227 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/market_watch/orderbook.py
--rw-r--r--   0        0        0      514 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/market_watch/price.py
--rw-r--r--   0        0        0      321 2022-12-09 11:30:04.976899 tsetmc_api-5.0.4/lib/tsetmc_api/market_watch/traders_type.py
--rw-r--r--   0        0        0     5043 2022-12-09 11:30:04.980899 tsetmc_api-5.0.4/lib/tsetmc_api/market_watch/watch.py
--rw-r--r--   0        0        0       27 2022-12-09 11:30:04.980899 tsetmc_api-5.0.4/lib/tsetmc_api/symbol/__init__.py
--rw-r--r--   0        0        0    12312 2022-12-09 11:30:04.980899 tsetmc_api-5.0.4/lib/tsetmc_api/symbol/_core.py
--rw-r--r--   0        0        0      164 2022-12-09 11:30:04.980899 tsetmc_api-5.0.4/lib/tsetmc_api/symbol/group.py
--rw-r--r--   0        0        0      366 2022-12-09 11:30:04.980899 tsetmc_api-5.0.4/lib/tsetmc_api/symbol/identification.py
--rw-r--r--   0        0        0      219 2022-12-09 11:30:04.980899 tsetmc_api-5.0.4/lib/tsetmc_api/symbol/notification.py
--rw-r--r--   0        0        0      247 2022-12-09 11:30:04.980899 tsetmc_api-5.0.4/lib/tsetmc_api/symbol/orderbook.py
--rw-r--r--   0        0        0      920 2022-12-09 11:30:04.980899 tsetmc_api-5.0.4/lib/tsetmc_api/symbol/price.py
--rw-r--r--   0        0        0     1607 2022-12-09 11:30:04.980899 tsetmc_api-5.0.4/lib/tsetmc_api/symbol/shareholder.py
--rw-r--r--   0        0        0      221 2022-12-09 11:30:04.980899 tsetmc_api-5.0.4/lib/tsetmc_api/symbol/state_change.py
--rw-r--r--   0        0        0      240 2022-12-09 11:30:04.980899 tsetmc_api-5.0.4/lib/tsetmc_api/symbol/supervisor_message.py
--rw-r--r--   0        0        0     9532 2022-12-09 11:30:04.980899 tsetmc_api-5.0.4/lib/tsetmc_api/symbol/symbol.py
--rw-r--r--   0        0        0      343 2022-12-09 11:30:04.980899 tsetmc_api-5.0.4/lib/tsetmc_api/symbol/traders_type.py
--rw-r--r--   0        0        0      874 2022-12-09 11:30:04.980899 tsetmc_api-5.0.4/lib/tsetmc_api/utils.py
--rw-r--r--   0        0        0      745 2022-12-09 11:30:04.980899 tsetmc_api-5.0.4/pyproject.toml
--rw-r--r--   0        0        0     2977 1970-01-01 00:00:00.000000 tsetmc_api-5.0.4/setup.py
--rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 tsetmc_api-5.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-27 16:19:22.412208 tsetmc_api-5.0.5/LICENSE.md
+-rw-r--r--   0        0        0     2767 2023-05-27 16:19:22.412208 tsetmc_api-5.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/__init__.py
+-rw-r--r--   0        0        0       36 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/day_details/__init__.py
+-rw-r--r--   0        0        0     9279 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/day_details/_core.py
+-rw-r--r--   0        0        0     5877 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/day_details/day_details.py
+-rw-r--r--   0        0        0      438 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/day_details/orderbook.py
+-rw-r--r--   0        0        0      460 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/day_details/price.py
+-rw-r--r--   0        0        0     1842 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/day_details/shareholder.py
+-rw-r--r--   0        0        0      114 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/day_details/threshold.py
+-rw-r--r--   0        0        0      215 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/day_details/trade.py
+-rw-r--r--   0        0        0      368 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/day_details/traders_type.py
+-rw-r--r--   0        0        0       36 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/group/__init__.py
+-rw-r--r--   0        0        0      481 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/group/_core.py
+-rw-r--r--   0        0        0      739 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/group/group.py
+-rw-r--r--   0        0        0       36 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_map/__init__.py
+-rw-r--r--   0        0        0     1373 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_map/_core.py
+-rw-r--r--   0        0        0     1628 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_map/map.py
+-rw-r--r--   0        0        0       31 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/__init__.py
+-rw-r--r--   0        0        0    17109 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/_core.py
+-rw-r--r--   0        0        0      224 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/daily_history.py
+-rw-r--r--   0        0        0      227 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/orderbook.py
+-rw-r--r--   0        0        0      514 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/price.py
+-rw-r--r--   0        0        0      321 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/traders_type.py
+-rw-r--r--   0        0        0     5043 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/watch.py
+-rw-r--r--   0        0        0       27 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/__init__.py
+-rw-r--r--   0        0        0    12382 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/_core.py
+-rw-r--r--   0        0        0      164 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/group.py
+-rw-r--r--   0        0        0      366 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/identification.py
+-rw-r--r--   0        0        0      219 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/notification.py
+-rw-r--r--   0        0        0      247 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/orderbook.py
+-rw-r--r--   0        0        0      920 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/price.py
+-rw-r--r--   0        0        0     1887 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/shareholder.py
+-rw-r--r--   0        0        0      221 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/state_change.py
+-rw-r--r--   0        0        0      240 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/supervisor_message.py
+-rw-r--r--   0        0        0     9574 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/symbol.py
+-rw-r--r--   0        0        0      343 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/symbol/traders_type.py
+-rw-r--r--   0        0        0      874 2023-05-27 16:19:22.452208 tsetmc_api-5.0.5/lib/tsetmc_api/utils.py
+-rw-r--r--   0        0        0      745 2023-05-27 16:19:22.456208 tsetmc_api-5.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3725 1970-01-01 00:00:00.000000 tsetmc_api-5.0.5/PKG-INFO
```

### Comparing `tsetmc_api-5.0.4/LICENSE` & `tsetmc_api-5.0.5/LICENSE.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 (The MIT License)
 
-Copyright 2022 Mahdi Sadeghi <mahdi74sadeghi@gmail.com>
+Copyright 2023 Mahdi Sadeghi <mahdi74sadeghi@gmail.com>
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 'Software'), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `tsetmc_api-5.0.4/lib/tsetmc_api/day_details/_core.py` & `tsetmc_api-5.0.5/lib/tsetmc_api/day_details/_core.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 
 def get_day_details_price_overview(symbol_id: str, date: jdate) -> dict:
     t = date.togregorian().strftime('%Y%m%d')
     response = requests.get(
         url=f'http://cdn.tsetmc.com/api/ClosingPrice/GetClosingPriceDaily/{symbol_id}/{t}',
         params={},
+        headers={
+            'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
+        },
         verify=False,
         timeout=20,
     )
     response.raise_for_status()
     response = response.json()['closingPriceDaily']
 
     return {
@@ -33,14 +36,17 @@
 
 
 def get_day_details_price_data(symbol_id: str, date: jdate) -> list[dict]:
     t = date.togregorian().strftime('%Y%m%d')
     response = requests.get(
         url=f'http://cdn.tsetmc.com/api/ClosingPrice/GetClosingPriceHistory/{symbol_id}/{t}',
         params={},
+        headers={
+            'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
+        },
         verify=False,
         timeout=20,
     )
     response.raise_for_status()
     response = response.json()['closingPriceHistory']
 
     price_data = [{
@@ -56,14 +62,17 @@
 
 
 def get_day_details_orderbook_data(symbol_id: str, date: jdate) -> list[dict]:
     t = date.togregorian().strftime('%Y%m%d')
     response = requests.get(
         url=f'http://cdn.tsetmc.com/api/BestLimits/{symbol_id}/{t}',
         params={},
+        headers={
+            'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
+        },
         verify=False,
         timeout=20,
     )
     response.raise_for_status()
     response = response.json()['bestLimitsHistory']
     response = sorted(response, key=lambda x: (x['hEven'], x['number']))
 
@@ -110,14 +119,17 @@
 
 def get_day_details_trade_data(symbol_id: str, date: jdate, summarize: bool) -> list[dict]:
     t = date.togregorian().strftime('%Y%m%d')
     summarize_url_ph = 'true' if summarize else 'false'
     response = requests.get(
         url=f'http://cdn.tsetmc.com/api/Trade/GetTradeHistory/{symbol_id}/{t}/{summarize_url_ph}',
         params={},
+        headers={
+            'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
+        },
         verify=False,
         timeout=20,
     )
     response.raise_for_status()
     response = response.json()['tradeHistory']
 
     return [{
@@ -128,14 +140,17 @@
 
 
 def get_day_details_traders_type_data(symbol_id: str, date: jdate) -> dict:
     t = date.togregorian().strftime('%Y%m%d')
     response = requests.get(
         url=f'http://cdn.tsetmc.com/api/ClientType/GetClientTypeHistory/{symbol_id}/{t}',
         params={},
+        headers={
+            'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
+        },
         verify=False,
         timeout=20,
     )
     response.raise_for_status()
     response = response.json()['clientType']
 
     return {
@@ -167,14 +182,17 @@
 
 
 def get_day_details_thresholds_data(symbol_id: str, date: jdate) -> dict:
     t = date.togregorian().strftime('%Y%m%d')
     response = requests.get(
         url=f'http://cdn.tsetmc.com/api/MarketData/GetStaticThreshold/{symbol_id}/{t}',
         params={},
+        headers={
+            'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
+        },
         verify=False,
         timeout=20,
     )
     response.raise_for_status()
     response = response.json()['staticThreshold']
 
     return {
@@ -184,64 +202,75 @@
 
 
 def get_day_details_shareholders_data(symbol_id: str, date: jdate) -> tuple[list[dict], list[dict]]:
     t = date.togregorian().strftime('%Y%m%d')
     response = requests.get(
         url=f'http://cdn.tsetmc.com/api/Shareholder/{symbol_id}/{t}',
         params={},
+        headers={
+            'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
+        },
         verify=False,
         timeout=20,
     )
     response.raise_for_status()
     response = response.json()['shareShareholder']
 
     old_shareholders = []
     new_shareholders = []
     it = int(t)
     for row in response:
         sh_data = {
-            'id': str(row['shareHolderId']),
+            'id': str(row['shareHolderID']),
             'name': row['shareHolderName'],
-            'count': row['numberOfShares'],
-            'percentage': row['perOfShares'],
+            'shares_count': row['numberOfShares'],
+            'shares_percentage': row['perOfShares'],
         }
 
         if row['dEven'] < it:
             old_shareholders.append(sh_data)
         else:
             new_shareholders.append(sh_data)
 
     return old_shareholders, new_shareholders
 
 
 def get_shareholder_chart_data(symbol_id: str, shareholder_id: str, days: int) -> list[dict]:
     response = requests.get(
         url=f'http://cdn.tsetmc.com/api/Shareholder/GetShareHolderHistory/{symbol_id}/{shareholder_id}/{days}',
         params={},
+        headers={
+            'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
+        },
         verify=False,
         timeout=20,
     )
     response.raise_for_status()
     response = response.json()['shareHolder']
 
     return [{
         'date': convert_deven_to_jdate(deven=row['dEven']),
-        'count': row['numberOfShares'],
-        'percentage': row['perOfShares'],
+        'shares_count': row['numberOfShares'],
+        'shares_percentage': row['perOfShares'],
     } for row in response]
 
 
 def get_shareholder_portfolio(shareholder_id: str) -> list[dict]:
     response = requests.get(
         url=f'http://cdn.tsetmc.com/api/Shareholder/GetShareHolderCompanyList/{shareholder_id}',
         params={},
+        headers={
+            'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
+        },
         verify=False,
         timeout=20,
     )
     response.raise_for_status()
     response = response.json()['shareHolderShare']
 
     return [{
-        'symbol_id': row['insCodes'],
-        'short_name': row['lVal18AFC'],
-        'long_name': row['lVal30'],
+        'symbol_id': row['instrument']['insCode'],
+        'short_name': row['instrument']['lVal18AFC'],
+        'long_name': row['instrument']['lVal30'],
+        'shares_count': row['numberOfShares'],
+        'shares_percent': row['perOfShares'],
     } for row in response]
```

### Comparing `tsetmc_api-5.0.4/lib/tsetmc_api/day_details/day_details.py` & `tsetmc_api-5.0.5/lib/tsetmc_api/day_details/day_details.py`

 * *Files 8% similar despite different names*

```diff
@@ -134,19 +134,23 @@
 
         raw_old_shareholders, raw_new_shareholders = _core.get_day_details_shareholders_data(
             symbol_id=self.symbol_id,
             date=self.date,
         )
 
         old_shareholders = [DayDetailsShareHolderDataRow(
+            symbol_id=self.symbol_id,
+            date=self.date,
             shareholder=DayDetailsShareHolder(id=row['id'], name=row['name']),
             count=row['count'],
             percentage=row['percentage'],
         ) for row in raw_old_shareholders]
 
         new_shareholders = [DayDetailsShareHolderDataRow(
+            symbol_id=self.symbol_id,
+            date=self.date,
             shareholder=DayDetailsShareHolder(id=row['id'], name=row['name']),
-            count=row['count'],
-            percentage=row['percentage'],
+            shares_count=row['shares_count'],
+            shares_percentage=row['shares_percentage'],
         ) for row in raw_new_shareholders]
 
         return old_shareholders, new_shareholders
```

### Comparing `tsetmc_api-5.0.4/lib/tsetmc_api/day_details/shareholder.py` & `tsetmc_api-5.0.5/lib/tsetmc_api/symbol/shareholder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,65 +1,70 @@
+from typing import Any
+
 from jdatetime import date as jdate
-from pydantic import BaseModel
+from pydantic import BaseModel, PrivateAttr
 
 from . import _core
 
 
-class DayDetailsShareHolderPortfolioRow(BaseModel):
+class SymbolShareHolderPortfolioRow(BaseModel):
     symbol_id: str
-    short_name: str
     long_name: str
+    shares_count: int
+    shares_percentage: float
 
 
-class DayDetailsShareHolder(BaseModel):
+class SymbolShareHolder(BaseModel):
+    _company_isin: str = PrivateAttr()
     id: str
     name: str
 
-    def get_portfolio_data(self) -> list[DayDetailsShareHolderPortfolioRow]:
+    def __init__(self, _company_isin: str, **data: Any):
+        super().__init__(**data)
+        self._company_isin = _company_isin
+
+    def get_portfolio_data(self) -> list[SymbolShareHolderPortfolioRow]:
         """
         returns list of companies owned by this shareholder
         """
 
-        raw_data = _core.get_shareholder_portfolio(shareholder_id=self.id)
+        raw_data = _core.get_symbol_shareholder_details(
+            shareholder_id=self.id,
+            company_isin=self._company_isin,
+        )['portfolio']
 
-        return [DayDetailsShareHolderPortfolioRow(
+        return [SymbolShareHolderPortfolioRow(
             symbol_id=row['symbol_id'],
-            short_name=row['short_name'],
             long_name=row['long_name'],
+            shares_count=row['shares_count'],
+            shares_percentage=row['shares_percentage'],
         ) for row in raw_data]
 
 
-class DayDetailsShareHolderChartRow(BaseModel):
+class SymbolShareHolderChartRow(BaseModel):
     date: jdate
-    count: int
-    percentage: float
+    shares_count: int
 
     class Config:
         arbitrary_types_allowed = True
 
 
-class DayDetailsShareHolderDataRow(BaseModel):
-    symbol_id: str
-    date: jdate
-    shareholder: DayDetailsShareHolder
-    count: int
-    percentage: float
+class SymbolShareHolderDataRow(BaseModel):
+    shareholder: SymbolShareHolder
+    shares_count: int
+    shares_percentage: float
+    shares_change: int
 
-    def get_chart_data(self, days: int = 90) -> list[DayDetailsShareHolderChartRow]:
+    def get_chart_data(self) -> list[SymbolShareHolderChartRow]:
         """
         returns list of changes to shareholders share count in history of this symbol
         """
 
-        raw_data = _core.get_shareholder_chart_data(
-            symbol_id=self.symbol_id,
+        raw_data = _core.get_symbol_shareholder_details(
             shareholder_id=self.shareholder.id,
-            days=days,
-        )
+            company_isin=self.shareholder._company_isin,
+        )['chart']
 
-        return [DayDetailsShareHolderChartRow(
+        return [SymbolShareHolderChartRow(
             date=row['date'],
-            count=row['count'],
-            percentage=row['percentage'],
+            shares_count=row['shares_count'],
         ) for row in raw_data]
-
-    class Config:
-        arbitrary_types_allowed = True
```

### Comparing `tsetmc_api-5.0.4/lib/tsetmc_api/group/group.py` & `tsetmc_api-5.0.5/lib/tsetmc_api/group/group.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.0.4/lib/tsetmc_api/market_map/map.py` & `tsetmc_api-5.0.5/lib/tsetmc_api/market_map/map.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.0.4/lib/tsetmc_api/market_watch/_core.py` & `tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     88: 'total_sell_average_count_rank_3_month',  # رتبه تعداد فروشندگان در 3 ماه گذشته
     89: 'total_sell_average_count_rank_12_month',  # رتبه تعداد فروشندگان در 12 ماه گذشته
 }
 
 
 def get_watch_price_data(refid: int = 0, heven: int = 0) -> tuple[dict, int, int]:
     response = requests.get(
-        url='http://www.tsetmc.com/tsev2/data/MarketWatchPlus.aspx',
+        url='http://old.tsetmc.com/tsev2/data/MarketWatchPlus.aspx',
         params={
             'h': heven,
             'r': refid,
         },
         verify=False,
         timeout=20,
     )
@@ -214,15 +214,15 @@
     refid = int(sections[4])
 
     return watch_data, refid, max_heven
 
 
 def get_watch_traders_type_data() -> dict:
     response = requests.get(
-        url='http://www.tsetmc.com/tsev2/data/ClientTypeAll.aspx',
+        url='http://old.tsetmc.com/tsev2/data/ClientTypeAll.aspx',
         params={},
         verify=False,
         timeout=20,
     )
     response.raise_for_status()
     response = response.text
 
@@ -304,15 +304,15 @@
         })
 
     return watch_data
 
 
 def get_watch_raw_stats_data() -> dict:
     response = requests.get(
-        url='http://www.tsetmc.com/tsev2/data/InstValue.aspx?t=a',
+        url='http://old.tsetmc.com/tsev2/data/InstValue.aspx?t=a',
         params={},
         verify=False,
         timeout=20,
     )
     response.raise_for_status()
     response = response.text
```

### Comparing `tsetmc_api-5.0.4/lib/tsetmc_api/market_watch/price.py` & `tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/price.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.0.4/lib/tsetmc_api/market_watch/watch.py` & `tsetmc_api-5.0.5/lib/tsetmc_api/market_watch/watch.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.0.4/lib/tsetmc_api/symbol/_core.py` & `tsetmc_api-5.0.5/lib/tsetmc_api/symbol/_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from jdatetime import time as jtime, date as jdate, datetime as jdatetime
 
 from ..utils import convert_deven_to_jdate
 
 
 def get_symbol_intraday_price_chart(symbol_id: str) -> list[dict]:
     response = requests.get(
-        url='http://www.tsetmc.com/tsev2/chart/data/IntraDayPrice.aspx',
+        url='http://old.tsetmc.com/tsev2/chart/data/IntraDayPrice.aspx',
         params={'i': symbol_id},
         verify=False,
         timeout=20,
     )
     response.raise_for_status()
     response = response.text
 
@@ -34,15 +34,15 @@
         })
 
     return result
 
 
 def get_symbol_price_overview(symbol_id: str) -> dict:
     response = requests.get(
-        url='http://www.tsetmc.com/tsev2/data/instinfodata.aspx',
+        url='http://old.tsetmc.com/tsev2/data/instinfodata.aspx',
         params={
             'i': symbol_id,
             'c': 27,
         },
         verify=False,
         timeout=20,
     )
@@ -142,15 +142,15 @@
         'traders_type_data': traders_type,
         'group_data': group_data,
     }
 
 
 def get_symbol_supervisor_messages(symbol_id: str) -> list[dict]:
     response = requests.get(
-        url=' http://tsetmc.ir/Loader.aspx',
+        url='http://old.tsetmc.com/Loader.aspx',
         params={
             'i': symbol_id,
             'Partree': '15131W',
         },
         verify=False,
         timeout=20,
     )
@@ -177,15 +177,15 @@
             last_item = None
 
     return messages
 
 
 def get_symbol_daily_ticks_history(symbol_id: str) -> list[dict]:
     response = requests.get(
-        url='http://www.tsetmc.com/tsev2/data/InstTradeHistory.aspx',
+        url='http://old.tsetmc.com/tsev2/data/InstTradeHistory.aspx',
         params={
             'i': symbol_id,
             'Top': 999999,
             'A': 0,
         },
         verify=False,
         timeout=20,
@@ -218,15 +218,15 @@
         })
 
     return ticks
 
 
 def get_symbol_notifications(symbol_id: str) -> list[dict]:
     response = requests.get(
-        url='http://tsetmc.ir/tsev2/data/CodalTopNew.aspx',
+        url='http://old.tsetmc.com/tsev2/data/CodalTopNew.aspx',
         params={
             'i': symbol_id,
         },
         verify=False,
         timeout=20,
     )
     response.raise_for_status()
@@ -240,15 +240,15 @@
     } for row in data]
 
     return notifications
 
 
 def get_symbol_state_changes(symbol_id: str) -> list[dict]:
     response = requests.get(
-        url=' http://tsetmc.ir/Loader.aspx',
+        url='http://old.tsetmc.com/Loader.aspx',
         params={
             'i': symbol_id,
             'Partree': '15131L',
         },
         verify=False,
         timeout=20,
     )
@@ -267,15 +267,15 @@
         })
 
     return state_changes
 
 
 def get_symbol_id_details(symbol_id: str) -> dict:
     response = requests.get(
-        url='http://tsetmc.ir/Loader.aspx',
+        url='http://old.tsetmc.com/Loader.aspx',
         params={
             'i': symbol_id,
             'Partree': '15131M',
         },
         verify=False,
         timeout=20,
     )
@@ -312,15 +312,15 @@
     }
 
     return result
 
 
 def get_symbol_traders_type_history(symbol_id: str) -> list[dict]:
     response = requests.get(
-        url='http://tsetmc.ir/tsev2/data/clienttype.aspx',
+        url='http://old.tsetmc.com/tsev2/data/clienttype.aspx',
         params={
             'i': symbol_id,
         },
         verify=False,
         timeout=20,
     )
     response.raise_for_status()
@@ -368,15 +368,15 @@
         })
 
     return traders_type_history
 
 
 def get_symbol_shareholders(company_isin: str) -> list[dict]:
     response = requests.get(
-        url='http://tsetmc.ir/Loader.aspx',
+        url='http://old.tsetmc.com/Loader.aspx',
         params={
             'c': company_isin,
             'Partree': '15131T',
         },
         verify=False,
         timeout=20,
     )
@@ -396,25 +396,25 @@
         count = int(tds[1].div['title'].replace(',', ''))
         percentage = float(tds[2].text)
         change = locale.atoi(tds[3].text.strip())
 
         shareholders.append({
             'id': shareholder_id,
             'name': name,
-            'count': count,
-            'percentage': percentage,
-            'change': change,
+            'shares_count': count,
+            'shares_percentage': percentage,
+            'shares_change': change,
         })
 
     return shareholders
 
 
 def get_symbol_shareholder_details(shareholder_id: str, company_isin: str):
     response = requests.get(
-        url=f'http://www.tsetmc.com/tsev2/data/ShareHolder.aspx?i={shareholder_id}%2C{company_isin}',
+        url=f'http://old.tsetmc.com/tsev2/data/ShareHolder.aspx?i={shareholder_id}%2C{company_isin}',
         params={
             'i': f'{shareholder_id}%C{company_isin}',
         },
         verify=False,
         timeout=20,
     )
     response.raise_for_status()
@@ -425,21 +425,21 @@
     chart = []
     portfolio = []
     for row in response:
         row = row.split(',')
         if len(row) == 2:
             chart.append({
                 'date': convert_deven_to_jdate(deven=int(row[0])),
-                'count': int(row[1]),
+                'shares_count': int(row[1]),
             })
         elif len(row) == 4:
             portfolio.append({
                 'symbol_id': row[0][1:] if '#' in row[0] else row[0],
                 'long_name': row[1],
-                'count': int(row[2]),
-                'percentage': float(row[3]),
+                'shares_count': int(row[2]),
+                'shares_percentage': float(row[3]),
             })
 
     return {
         'chart': chart,
         'portfolio': portfolio,
     }
```

### Comparing `tsetmc_api-5.0.4/lib/tsetmc_api/symbol/price.py` & `tsetmc_api-5.0.5/lib/tsetmc_api/symbol/price.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.0.4/lib/tsetmc_api/symbol/shareholder.py` & `tsetmc_api-5.0.5/lib/tsetmc_api/day_details/shareholder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,69 @@
 from jdatetime import date as jdate
 from pydantic import BaseModel
 
 from . import _core
 
 
-class SymbolShareHolderPortfolioRow(BaseModel):
+class DayDetailsShareHolderPortfolioRow(BaseModel):
     symbol_id: str
+    short_name: str
     long_name: str
-    count: int
-    percentage: float
+    shares_count: int
+    shares_percent: float
 
 
-class SymbolShareHolder(BaseModel):
-    _company_isin: str
+class DayDetailsShareHolder(BaseModel):
     id: str
     name: str
 
-    def get_portfolio_data(self) -> list[SymbolShareHolderPortfolioRow]:
+    def get_portfolio_data(self) -> list[DayDetailsShareHolderPortfolioRow]:
         """
         returns list of companies owned by this shareholder
         """
 
-        raw_data = _core.get_symbol_shareholder_details(
-            shareholder_id=self.id,
-            company_isin=self._company_isin,
-        )['portfolio']
+        raw_data = _core.get_shareholder_portfolio(shareholder_id=self.id)
 
-        return [SymbolShareHolderPortfolioRow(
+        return [DayDetailsShareHolderPortfolioRow(
             symbol_id=row['symbol_id'],
+            short_name=row['short_name'],
             long_name=row['long_name'],
-            count=row['count'],
-            percentage=row['percentage'],
+            shares_count=row['shares_count'],
+            shares_percent=row['shares_percent'],
         ) for row in raw_data]
 
 
-class SymbolShareHolderChartRow(BaseModel):
+class DayDetailsShareHolderChartRow(BaseModel):
     date: jdate
-    count: int
+    shares_count: int
+    shares_percentage: float
 
     class Config:
         arbitrary_types_allowed = True
 
 
-class SymbolShareHolderDataRow(BaseModel):
-    shareholder: SymbolShareHolder
-    count: int
-    percentage: float
-    change: int
+class DayDetailsShareHolderDataRow(BaseModel):
+    symbol_id: str
+    date: jdate
+    shareholder: DayDetailsShareHolder
+    shares_count: int
+    shares_percentage: float
 
-    def get_chart_data(self) -> list[SymbolShareHolderChartRow]:
+    def get_chart_data(self, days: int = 90) -> list[DayDetailsShareHolderChartRow]:
         """
         returns list of changes to shareholders share count in history of this symbol
         """
 
-        raw_data = _core.get_symbol_shareholder_details(
+        raw_data = _core.get_shareholder_chart_data(
+            symbol_id=self.symbol_id,
             shareholder_id=self.shareholder.id,
-            company_isin=self.shareholder._company_isin,
+            days=days,
         )
 
-        return [SymbolShareHolderChartRow(
+        return [DayDetailsShareHolderChartRow(
             date=row['date'],
-            count=row['count'],
+            shares_count=row['shares_count'],
+            shares_percentage=row['shares_percentage'],
         ) for row in raw_data]
+
+    class Config:
+        arbitrary_types_allowed = True
```

### Comparing `tsetmc_api-5.0.4/lib/tsetmc_api/symbol/symbol.py` & `tsetmc_api-5.0.5/lib/tsetmc_api/symbol/symbol.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,13 +250,13 @@
 
         shareholders = [SymbolShareHolderDataRow(
             shareholder=SymbolShareHolder(
                 _company_isin=company_isin,
                 id=row['id'],
                 name=row['name'],
             ),
-            count=row['count'],
-            percentage=row['percentage'],
-            change=row['change'],
+            shares_count=row['shares_count'],
+            shares_percentage=row['shares_percentage'],
+            shares_change=row['shares_change'],
         ) for row in raw_data]
 
         return shareholders
```

### Comparing `tsetmc_api-5.0.4/lib/tsetmc_api/utils.py` & `tsetmc_api-5.0.5/lib/tsetmc_api/utils.py`

 * *Files identical despite different names*

### Comparing `tsetmc_api-5.0.4/pyproject.toml` & `tsetmc_api-5.0.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tsetmc-api"
-version = "5.0.4"
+version = "5.0.5"
 description = "simple package to communicate and crawl data from tsetmc.com (Tehran Stock Exchange Website)"
 license = "MIT"
 repository = "https://github.com/mahs4d/tsetmc-api"
 authors = ["Mahdi Sadeghi <mahdi74sadeghi@gmail.com>"]
 packages = [
     { include = "tsetmc_api", from = "lib" },
 ]
```

