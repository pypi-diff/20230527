# Comparing `tmp/finpy_tse-1.2.5.tar.gz` & `tmp/finpy_tse-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finpy_tse-1.2.5.tar", last modified: Sat May 27 05:30:03 2023, max compression
+gzip compressed data, was "finpy_tse-1.2.6.tar", last modified: Sat May 27 20:07:51 2023, max compression
```

## Comparing `finpy_tse-1.2.5.tar` & `finpy_tse-1.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:30:03.604768 finpy_tse-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-27 05:29:47.000000 finpy_tse-1.2.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-05-27 05:30:03.604768 finpy_tse-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-05-27 05:29:47.000000 finpy_tse-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:30:03.604768 finpy_tse-1.2.5/finpy_tse/
--rw-r--r--   0 runner    (1001) docker     (123)   182755 2023-05-27 05:29:47.000000 finpy_tse-1.2.5/finpy_tse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:30:03.604768 finpy_tse-1.2.5/finpy_tse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-05-27 05:30:03.000000 finpy_tse-1.2.5/finpy_tse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-27 05:30:03.000000 finpy_tse-1.2.5/finpy_tse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 05:30:03.000000 finpy_tse-1.2.5/finpy_tse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-27 05:30:03.000000 finpy_tse-1.2.5/finpy_tse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 05:30:03.000000 finpy_tse-1.2.5/finpy_tse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 05:30:03.604768 finpy_tse-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-27 05:29:47.000000 finpy_tse-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:07:51.883015 finpy_tse-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-27 20:07:34.000000 finpy_tse-1.2.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-05-27 20:07:51.883015 finpy_tse-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-05-27 20:07:34.000000 finpy_tse-1.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:07:51.883015 finpy_tse-1.2.6/finpy_tse/
+-rw-r--r--   0 runner    (1001) docker     (123)   182906 2023-05-27 20:07:34.000000 finpy_tse-1.2.6/finpy_tse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:07:51.883015 finpy_tse-1.2.6/finpy_tse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-05-27 20:07:51.000000 finpy_tse-1.2.6/finpy_tse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-27 20:07:51.000000 finpy_tse-1.2.6/finpy_tse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 20:07:51.000000 finpy_tse-1.2.6/finpy_tse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-27 20:07:51.000000 finpy_tse-1.2.6/finpy_tse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 20:07:51.000000 finpy_tse-1.2.6/finpy_tse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 20:07:51.883015 finpy_tse-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-27 20:07:34.000000 finpy_tse-1.2.6/setup.py
```

### Comparing `finpy_tse-1.2.5/LICENSE.txt` & `finpy_tse-1.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finpy_tse-1.2.5/PKG-INFO` & `finpy_tse-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finpy_tse
-Version: 1.2.5
+Version: 1.2.6
 Summary: A Python Module to Access Tehran Stock Exchange Historical and Real-Time Data
 Author: ALI RAHIMI  AND  RASOOL GHAFOURI
 Author-email: a.rahimi.aut@gmail.com
 License: BSD (3-clause)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `finpy_tse-1.2.5/README.md` & `finpy_tse-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `finpy_tse-1.2.5/finpy_tse/__init__.py` & `finpy_tse-1.2.6/finpy_tse/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2281,15 +2281,15 @@
             return False
         tracemalloc.start()
         @unsync
         #تابعی برای سرچ کردن لیستی از نام ها و برگرداندن لیستی از دیتا فریم های تمیزشده  
         async def parallel_request(stock_list):
 
             async def get_data(session, stock):
-                url = f'http://www.tsetmc.com/tsev2/data/search.aspx?skey={stock}'
+                url = f'http://old.tsetmc.com/tsev2/data/search.aspx?skey={stock}'
                 #ارسال درخواست
                 async with session.get(url, headers=headers) as response:
                     data_id = await response.text()
 
                     #تبدیل به لیست کردن دیتای مورد نیاز
                     data = []
                     for i in data_id.split(';') :
@@ -2327,15 +2327,15 @@
 
         def request(stock_list) :
 
             view_counts = []
             for stock in stock_list :
                 while True :
                     try :
-                        data_id = requests.get(f'http://www.tsetmc.com/tsev2/data/search.aspx?skey={stock}', headers=headers).text
+                        data_id = requests.get(f'http://old.tsetmc.com/tsev2/data/search.aspx?skey={stock}', headers=headers).text
                         break
                     except :
                         print('nn')
                         pass
 
                 data = []
                 for i in data_id.split(';') :
@@ -2450,15 +2450,15 @@
     
         tracemalloc.start()
         @unsync
         #تابعی برای سرچ کردن لیستی از نام ها و برگرداندن لیستی از دیتا فریم های تمیزشده  
         async def parallel_request(list_code):
 
             async def get_data(session, code):
-                url = f'http://www.tsetmc.com/tsev2/data/InstTradeHistory.aspx?i={code}&Top=999999&A=0'
+                url = f'http://old.tsetmc.com/tsev2/data/InstTradeHistory.aspx?i={code}&Top=999999&A=0'
                 #ارسال درخواست
                 async with session.get(url, headers=headers) as response:
                     data_id = await response.text()
                     return [data_id,response.status]
 
             #مدیریت درخواست ها
             async with aiohttp.ClientSession() as session:
@@ -2686,15 +2686,15 @@
                     if (counter==1):
                         df_final = i.copy()
                     else:
                         df_final = pd.concat([df_final,i])
                     counter+=1
             return df_final
         async def get_session(session, code):
-            url = f'http://www.tsetmc.com/Loader.aspx?Partree=15131M&i={code}'
+            url = f'http://old.tsetmc.com/Loader.aspx?Partree=15131M&i={code}'
             async with session.get(url, headers=headers) as response:
                 try:
                     data_text = await response.text()
                     soup = BeautifulSoup(data_text, 'html.parser')
                     table = soup.findAll("table", {"class": "table1"})
                     df_id = pd.read_html(str(table[0]))[0]
                     ticker = (df_id.iloc[5,1].split('-')[0]).strip()
@@ -2708,15 +2708,15 @@
     #---------------------------------------------------------------------------------
     start_time = time.time()
     if(show_progress):
         clear_output(wait=True)
         print(f'STEP 1/4: Gathering historical price data of last 60 trading days ...')
     # send request:
     headers = {'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'}
-    r = requests.get('http://www.tsetmc.com/tsev2/data/ClosingPriceAll.aspx', headers=headers)
+    r = requests.get('http://old.tsetmc.com/tsev2/data/ClosingPriceAll.aspx', headers=headers)
 
     # clean the data:
     hist_60_days = pd.DataFrame(r.text.split(';'))
     hist_60_days.columns = ['Data']
     hist_60_days['WEB-ID'] = hist_60_days['Data'].apply(lambda x: x.split(',')[0] if(x.count(',')==10) else None)
     hist_60_days['Data'] = hist_60_days['Data'].apply(lambda x: x.replace(x.split(',')[0]+',','') if(x.count(',')==10) else x)
     temp_data_df = hist_60_days['Data'].str.split(",",expand=True)
@@ -2730,29 +2730,31 @@
     hist_60_days = hist_60_days.apply(pd.to_numeric)
     hist_60_days = hist_60_days.sort_values(by=['n','WEB-ID'], ascending=[True,True])
 
     # find trading days j-dates and join:
     if(show_progress):
         clear_output(wait=True)
         print(f'STEP 2/4: Adding J-date to the historical data ...')
-    r_trading_days = requests.get(f'http://tsetmc.com/tsev2/chart/data/Index.aspx?i=32097828799138957&t=value', headers=headers)
-    df_trading_days = pd.DataFrame(r_trading_days.text.split(';'))
-    df_trading_days[['J-Date','Adj Close']] = df_trading_days[0].str.split(",",expand=True)
-    df_trading_days['J-Date'] = df_trading_days['J-Date'].apply(lambda x: str(jdatetime.date(int(x.split('/')[0]),int(x.split('/')[1]),int(x.split('/')[2]))))
+    r_trading_days = requests.get(f'http://cdn.tsetmc.com/api/Index/GetIndexB2History/32097828799138957', headers=headers)
+    df_trading_days = pd.DataFrame(r_trading_days.json()['indexB2'])[['dEven','xNivInuClMresIbs']]
+    df_trading_days['dEven'] = df_trading_days['dEven'].apply(lambda x: str(x))
+    df_trading_days['dEven'] = df_trading_days['dEven'].apply(lambda x: x[:4]+'-'+x[4:6]+'-'+x[-2:])
+    df_trading_days['dEven'] = pd.to_datetime(df_trading_days['dEven'])
+    df_trading_days['J-Date']=df_trading_days['dEven'].apply(lambda x: str(jdatetime.date.fromgregorian(date=x.date())))
     df_trading_days = df_trading_days.set_index('J-Date')[::-1].reset_index()[['J-Date']]
     df_trading_days = df_trading_days[:60]
     df_trading_days.index.name = 'n'
     df_trading_days = df_trading_days.reset_index()
     hist_60_days = pd.merge(hist_60_days, df_trading_days, on='n')
 
     if(show_progress):
         clear_output(wait=True)
         print(f'STEP 3/4: Adding ticker names from market watch ...')
     # adding ticker names:
-    r = requests.get('http://www.tsetmc.com/tsev2/data/MarketWatchPlus.aspx', headers=headers)
+    r = requests.get('http://old.tsetmc.com/tsev2/data/MarketWatchPlus.aspx', headers=headers)
     main_text = r.text
     Mkt_df = pd.DataFrame((main_text.split('@')[2]).split(';'))
     Mkt_df = Mkt_df[0].str.split(",",expand=True)
     Mkt_df = Mkt_df.iloc[:,:23]
     Mkt_df.columns = ['WEB-ID','Ticker-Code','Ticker','Name','Time','Open','Final','Close','No','Volume','Value',
                       'Low','High','Y-Final','EPS','Base-Vol','Unknown1','Unknown2','Sector','Day_UL','Day_LL','Share-No','Mkt-ID']
     Mkt_df = Mkt_df[['WEB-ID','Ticker']]
```

### Comparing `finpy_tse-1.2.5/finpy_tse.egg-info/PKG-INFO` & `finpy_tse-1.2.6/finpy_tse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finpy-tse
-Version: 1.2.5
+Version: 1.2.6
 Summary: A Python Module to Access Tehran Stock Exchange Historical and Real-Time Data
 Author: ALI RAHIMI  AND  RASOOL GHAFOURI
 Author-email: a.rahimi.aut@gmail.com
 License: BSD (3-clause)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `finpy_tse-1.2.5/setup.py` & `finpy_tse-1.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='finpy_tse',                           # should match the package folder
     packages=['finpy_tse'],                     # should match the package folder
-    version='1.2.5',                            # important for updates
+    version='1.2.6',                            # important for updates
     license='BSD (3-clause)',                                  # should match your chosen license
     description='A Python Module to Access Tehran Stock Exchange Historical and Real-Time Data',
     long_description=long_description,              # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='ALI RAHIMI  AND  RASOOL GHAFOURI',
     author_email='a.rahimi.aut@gmail.com',
     install_requires=['requests','jdatetime','pandas','numpy','requests','bs4','asyncio','urllib3','aiohttp','unsync','IPython','persiantools','datetime','XlsxWriter','lxml'],                  # list all packages that your package uses
```

