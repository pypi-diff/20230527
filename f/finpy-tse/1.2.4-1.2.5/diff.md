# Comparing `tmp/finpy_tse-1.2.4.tar.gz` & `tmp/finpy_tse-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finpy_tse-1.2.4.tar", last modified: Tue May 23 08:48:49 2023, max compression
+gzip compressed data, was "finpy_tse-1.2.5.tar", last modified: Sat May 27 05:30:03 2023, max compression
```

## Comparing `finpy_tse-1.2.4.tar` & `finpy_tse-1.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:48:49.395669 finpy_tse-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-23 08:48:33.000000 finpy_tse-1.2.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-05-23 08:48:49.395669 finpy_tse-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-05-23 08:48:33.000000 finpy_tse-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:48:49.391669 finpy_tse-1.2.4/finpy_tse/
--rw-r--r--   0 runner    (1001) docker     (123)   163610 2023-05-23 08:48:33.000000 finpy_tse-1.2.4/finpy_tse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:48:49.395669 finpy_tse-1.2.4/finpy_tse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-05-23 08:48:49.000000 finpy_tse-1.2.4/finpy_tse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-23 08:48:49.000000 finpy_tse-1.2.4/finpy_tse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:48:49.000000 finpy_tse-1.2.4/finpy_tse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-23 08:48:49.000000 finpy_tse-1.2.4/finpy_tse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-23 08:48:49.000000 finpy_tse-1.2.4/finpy_tse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 08:48:49.395669 finpy_tse-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-23 08:48:33.000000 finpy_tse-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:30:03.604768 finpy_tse-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-27 05:29:47.000000 finpy_tse-1.2.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-05-27 05:30:03.604768 finpy_tse-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11214 2023-05-27 05:29:47.000000 finpy_tse-1.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:30:03.604768 finpy_tse-1.2.5/finpy_tse/
+-rw-r--r--   0 runner    (1001) docker     (123)   182755 2023-05-27 05:29:47.000000 finpy_tse-1.2.5/finpy_tse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 05:30:03.604768 finpy_tse-1.2.5/finpy_tse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11107 2023-05-27 05:30:03.000000 finpy_tse-1.2.5/finpy_tse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-27 05:30:03.000000 finpy_tse-1.2.5/finpy_tse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 05:30:03.000000 finpy_tse-1.2.5/finpy_tse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-27 05:30:03.000000 finpy_tse-1.2.5/finpy_tse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 05:30:03.000000 finpy_tse-1.2.5/finpy_tse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 05:30:03.604768 finpy_tse-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-27 05:29:47.000000 finpy_tse-1.2.5/setup.py
```

### Comparing `finpy_tse-1.2.4/LICENSE.txt` & `finpy_tse-1.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finpy_tse-1.2.4/PKG-INFO` & `finpy_tse-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finpy_tse
-Version: 1.2.4
+Version: 1.2.5
 Summary: A Python Module to Access Tehran Stock Exchange Historical and Real-Time Data
 Author: ALI RAHIMI  AND  RASOOL GHAFOURI
 Author-email: a.rahimi.aut@gmail.com
 License: BSD (3-clause)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `finpy_tse-1.2.4/README.md` & `finpy_tse-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `finpy_tse-1.2.4/finpy_tse/__init__.py` & `finpy_tse-1.2.5/finpy_tse/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,89 @@
             print(f'Please enter valid {key_word} date')
             return
         else:
             print(f'Please enter valid {key_word} date in YYYY-MM-DD format')
             
 ################################################################################################################################################################################
 ################################################################################################################################################################################
+def get_tse_webid(stock:str = 'پترول') -> pd.DataFrame:
+    """
+    Takes ticker or firm's full name, does a live search in TSE new website and returns a multi-index Pandas dataframe that contains the following columns:
+    
+    Ticker: Symbol in the Tehran Stock Exchange.
+    Active: 1 shows the market in which the stock is currently trading. 
+    Name: firm's full name in the relevant market.
+    WebID: A numeric code that can be used for building request links and crawling the financial data of the given stock.
+    Market: Market name in Tehran Stock Exchange, markets the stock was traded in and is trading now (بورس، فرابورس، پایه زرد، پایه نارنجی، پایه قرمز).
+    
+    :param stock: (str) Ticker or firm's full name. 
+    :return: (pd.DataFrame) A dataframe that contains Ticker, Active, WebID, Name and Market columns for the requested stock.
+    """
+    
+    # basic search function: searches for and cleans the search results
+    def srch_req(srch_key):
+        srch_page = requests.get(f'http://cdn.tsetmc.com/api/Instrument/GetInstrumentSearch/{srch_key}', headers=headers)
+        srch_res = pd.DataFrame(srch_page.json()['instrumentSearch'])
+        srch_res = srch_res[['lVal18AFC','lVal30','insCode','lastDate','cgrValCot']]
+        srch_res.columns = ['Ticker','Name','WebID','Active','Market']
+        srch_res['Name'] = srch_res['Name'].apply(lambda x : characters.ar_to_fa(' '.join([i.strip() for i in x.split('\u200c')]).strip()))
+        srch_res['Ticker'] = srch_res['Ticker'].apply(lambda x : characters.ar_to_fa(''.join(x.split('\u200c')).strip()))
+        srch_res['NameSplit'] = srch_res['Name'].apply(lambda x : ''.join(x.split()).strip())
+        srch_res['SymbolSplit'] = srch_res['Ticker'].apply(lambda x : ''.join(x.split()).strip())
+        srch_res['Active'] = pd.to_numeric(srch_res['Active'])
+        srch_res = srch_res.sort_values('Ticker')
+        srch_res = pd.DataFrame(srch_res[['Name','WebID','NameSplit','SymbolSplit','Market']].values, columns=['Name','WebID',
+                                'NameSplit','SymbolSplit','Market'], index=pd.MultiIndex.from_frame(srch_res[['Ticker','Active']]))
+        return srch_res
+    
+    # checking function inputs
+    if type(stock) != str:
+        print('Please Enetr a Valid Ticker or Name!')
+        return False
+    
+    # special case that can not be found using ticker: convert ticker to full name!
+    if(stock=='آ س پ'):
+        stock = 'آ.س.پ'
+        
+    # generating search keys
+    stock = characters.ar_to_fa(''.join(stock.split('\u200c')).strip())
+    first_name = stock.split()[0]
+    stock = ''.join(stock.split())
+    
+    # start searching using keys, cleaning data, checking search results and handling special cases (ticker or full name)
+    data = srch_req(first_name)
+    df_symbol = data[data['SymbolSplit'] == stock]
+    df_name = data[data['NameSplit'] == stock]
+    
+    # matching search results with search key, cleaning the data and adding market data  
+    if len(df_symbol) > 0 :
+        df_symbol = df_symbol.sort_index(level=1,ascending=False).drop(['NameSplit','SymbolSplit'], axis=1)
+        df_symbol['Market'] = df_symbol['Market'].apply(lambda x: re.sub('[0-9]', '', x))
+        df_symbol['Market'] = df_symbol['Market'].map({'N':'بورس', 'Z':'فرابورس', 'D':'فرابورس', 'A':'پایه زرد', 'P':'پایه زرد', 'C':'پایه نارنجی', 'L':'پایه قرمز',
+                                                       'W':'کوچک و متوسط فرابورس', 'V':'کوچک و متوسط فرابورس',})
+        df_symbol['Market'] = df_symbol['Market'].fillna('نامعلوم')
+        return df_symbol
+    elif len(df_name) > 0 :
+        symbol = df_name.index[0][0]
+        data = srch_req(symbol)
+        symbol = characters.ar_to_fa(''.join(symbol.split('\u200c')).strip())
+        df_symbol = data[data.index.get_level_values('Ticker') == symbol]
+        if len(df_symbol) > 0 :
+            df_symbol = df_symbol.sort_index(level=1, ascending=False).drop(['NameSplit','SymbolSplit'], axis=1)
+            df_symbol['Market'] = df_symbol['Market'].apply(lambda x: re.sub('[0-9]', '', x))
+            df_symbol['Market'] = df_symbol['Market'].map({'N':'بورس', 'Z':'فرابورس', 'D':'فرابورس', 'A':'پایه زرد', 'P':'پایه زرد', 'C':'پایه نارنجی', 'L':'پایه قرمز',
+                                                           'W':'کوچک و متوسط فرابورس', 'V':'کوچک و متوسط فرابورس',})
+            df_symbol['Market'] = df_symbol['Market'].fillna('نامعلوم')
+            return df_symbol
+    
+    # invalid entry
+    print('Please Enetr a Valid Ticker or Name!')
+    
+    return False
+
 
 def __Get_TSE_WebID__(stock):
     # search TSE function ------------------------------------------------------------------------------------------------------------
     def request(name):
         page = requests.get(f'http://old.tsetmc.com/tsev2/data/search.aspx?skey={name}', headers=headers)
         data = []
         for i in page.text.split(';') :
@@ -144,14 +219,161 @@
         else:
             print('Invalid sector name! Please try again with correct sector name!')
             return
     return sector_web_id   
 
 ################################################################################################################################################################################
 ################################################################################################################################################################################
+def get_price_history(stock:str = 'خودرو', 
+                      start_date:str = '1400-01-01', 
+                      end_date:str = '1401-01-01', 
+                      ignore_date:bool = False, 
+                      adjust_price:bool = False, 
+                      show_weekday:bool = False, 
+                      double_date:bool = False) -> pd.DataFrame:
+    
+    """
+    Takes ticker or firm's full name and returns a Pandas dataframe that contains the following columns:
+    
+    J-Date: Jalali date, as index
+    Date: Gregorian date
+    Weekday: Name of weekdays
+    Open: Opening price of day
+    High: Maximum price of day 
+    Low: Minimum price of day
+    Close: Closing price of day (آخرین قیمت)
+    Final: Weighted closing price of day (قیمت پایانی)
+    Volume: Traded volume of day
+    Value: Traded value of day in IRAN's Rial
+    No: Number of trades in a day
+    Ticker: Ticker/Symbol
+    Name: Firm's full name
+    Market: Market, the stock is traded in
+    Adj Open: Adjusted opening price of day for stock-splits and dividends
+    Adj High: Adjusted maximum price of day for stock-splits and dividends
+    Adj Low: Adjusted minimum price of day for stock-splits and dividends
+    Adj Close: Adjusted closing price of day for stock-splits and dividends
+    Adj Final: Adjusted weighted closing price of day for stock-splits and dividends
+    
+     * All data are taken from the new website of Tehran Stock Exchange.
+
+    :param stock: (str) Ticker or firm's full name. 
+    :param start_date: (str) Jalali date for starting day of historical price data in YYYY-MM-DD format.
+    :param end_date: (str) Jalali date for ending day of historical price data in YYYY-MM-DD format.
+    :param ignore_date: (bool) Ignores start_date and end_date and returns all available price history, if set to True.
+    :param adjust_price: (bool) Adjusts price for stock-splits and dividends, if set to True.
+    :param show_weekday: (bool) Shows weekdays in the output, if set to True.
+    :param double_date: (bool) Shows Gregorian date in the output, if set to True.
+    :return: (pd.DataFrame) A dataframe that contains J-Date as index and Date, Weekday, Open, High, Low, Close, Final, Volume, Value, No, Ticker, Name, Market, Adj Open, Adj High, Adj Low, Adj Close, Adj Final.
+    """
+
+    # basic request and data cleaning function for historical price data of a ticker for a given market 
+    def get_price_data(ticker_no, ticker, name, market):
+        r = requests.get(f'http://cdn.tsetmc.com/api/ClosingPrice/GetClosingPriceDailyList/{ticker_no}/0', headers=headers)
+        df_history = pd.DataFrame(r.json()['closingPriceDaily'])
+        columns=['Date','High','Low','Final','Close','Open','Y-Final','Value','Volume','No']
+        df_history = df_history[['dEven','priceMax','priceMin','pClosing','pDrCotVal','priceFirst','priceYesterday','qTotCap','qTotTran5J','zTotTran']]
+        df_history.columns = ['Date','High','Low','Final','Close','Open','Y-Final','Value','Volume','No']
+        df_history['Date'] = df_history['Date'].apply(lambda x: str(x))
+        df_history['Date'] = df_history['Date'].apply(lambda x: f'{x[:4]}-{x[4:6]}-{x[-2:]}')
+        df_history['Date']=pd.to_datetime(df_history['Date'])
+        df_history = df_history[df_history['No']!=0]
+        df_history['Ticker'] = ticker
+        df_history['Name'] = name
+        df_history['Market'] = market
+        df_history = df_history.set_index('Date')
+        return df_history
+    
+    # check to see if the entry start and end dates are valid or not
+    if(not ignore_date):
+        start_date = __Check_JDate_Validity__(start_date,key_word="'START'")
+        if(start_date==None):
+            return
+        end_date = __Check_JDate_Validity__(end_date,key_word="'END'")
+        if(end_date==None):
+            return
+        start = jdatetime.date(year=int(start_date.split('-')[0]), month=int(start_date.split('-')[1]), day=int(start_date.split('-')[2]))
+        end = jdatetime.date(year=int(end_date.split('-')[0]), month=int(end_date.split('-')[1]), day=int(end_date.split('-')[2]))
+        if(start>end):
+            print('Start date must be a day before end date!')
+            return
+    
+    # search for WebIDs
+    ticker_no_df = get_tse_webid(stock)
+    if(type(ticker_no_df)==bool):
+        return
+    
+    # create an empty dataframe:
+    df_history = pd.DataFrame({},columns=['Date','High','Low','Final','Close','Open','Y-Final','Value','Volume','No','Ticker','Name','Market']).set_index('Date')
+    
+    # loop to get data from different pages of a ticker:
+    for index, row in (ticker_no_df.reset_index()).iterrows():
+        try:
+            df_temp = get_price_data(ticker_no = row['WebID'],ticker = row['Ticker'],name = row['Name'],market = row['Market'])
+            df_history = pd.concat([df_history,df_temp])
+        except:
+            pass
+        
+    # sort based on dated index:
+    df_history = df_history.sort_index(ascending=True)
+    df_history = df_history.reset_index()
+    
+    # add weekdays and j-date columns:
+    df_history['Weekday']=df_history['Date'].dt.weekday
+    df_history['Weekday'] = df_history['Weekday'].apply(lambda x: calendar.day_name[x])
+    df_history['J-Date']=df_history['Date'].apply(lambda x: str(jdatetime.date.fromgregorian(date=x.date())))
+    df_history = df_history.set_index('J-Date')
+    
+    # rearrange columns and convert some columns to numeric
+    df_history=df_history[['Date','Weekday','Y-Final','Open','High','Low','Close','Final','Volume','Value','No','Ticker','Name','Market']]
+    cols = ['Y-Final','Open','High','Low','Close','Final','Volume','No','Value']
+    df_history[cols] = df_history[cols].apply(pd.to_numeric, axis=1)
+    
+
+    # find stock moves between markets and adjust for nominal price in the new market, if necessary
+    df_history['Final(+1)'] = df_history['Final'].shift(+1)          
+    df_history['Market(+1)'] = df_history['Market'].shift(+1)        
+    df_history['temp'] = df_history.apply(lambda x: x['Y-Final'] if((x['Y-Final']!=0)and(x['Y-Final']!=1000)) 
+                                          else (x['Y-Final'] if((x['Market(+1)']==x['Market'])or(pd.isnull(x['Final(+1)']))) 
+                                          else x['Final(+1)']),axis = 1)
+    df_history['Y-Final'] = df_history['temp']
+    df_history.drop(columns=['Final(+1)','temp','Market(+1)'],inplace=True)
+    
+    # convert numbers to int because we do not have less than Rial, just for clean outputs!
+    for col in cols:
+        df_history[col] = df_history[col].apply(lambda x: int(x))
+
+    # Adjust price data, if requested:
+    if(adjust_price):
+        df_history['COEF'] = (df_history['Y-Final'].shift(-1)/df_history['Final']).fillna(1.0)
+        df_history['ADJ-COEF']=df_history.iloc[::-1]['COEF'].cumprod().iloc[::-1]
+        df_history['Adj Open'] = (df_history['Open']*df_history['ADJ-COEF']).apply(lambda x: int(x))
+        df_history['Adj High'] = (df_history['High']*df_history['ADJ-COEF']).apply(lambda x: int(x))
+        df_history['Adj Low'] = (df_history['Low']*df_history['ADJ-COEF']).apply(lambda x: int(x))
+        df_history['Adj Close'] = (df_history['Close']*df_history['ADJ-COEF']).apply(lambda x: int(x))
+        df_history['Adj Final'] = (df_history['Final']*df_history['ADJ-COEF']).apply(lambda x: int(x))
+        df_history.drop(columns=['COEF','ADJ-COEF'],inplace=True)
+    
+    # drop weekdays if not requested
+    if(not show_weekday):
+        df_history.drop(columns=['Weekday'],inplace=True)
+    
+    # drop Gregorian date if not requested
+    if(not double_date):
+        df_history.drop(columns=['Date'],inplace=True)
+    
+    # drop yesterday's final price!
+    df_history.drop(columns=['Y-Final'],inplace=True)
+    
+    # slice requested time window, if requested:
+    if(not ignore_date):
+        df_history = df_history[start_date:end_date]
+        
+    return df_history
+
 
 def Get_Price_History(stock = 'خودرو', start_date = '1400-01-01', end_date='1401-01-01', ignore_date = False, adjust_price = False, show_weekday = False, double_date = False):
     """
     دریافت سابقه قیمت یک سهم در روزهای معاملاتی بین تاریخ شروع و پایان
     قابلیت دریافت همه سابقه قیمت بدون توجه به تاریخ شروع و پایان
     قابلیت تعدیل قیمت برای سود نقدی و افزایش سرمایه با احتساب آورده
     قابلیت ارائه تاریخ میلادی علاوه بر تاریخ شمسی، قابلیت نمایش روزهای هفته
@@ -244,14 +466,133 @@
     if(not ignore_date):
         df_history = df_history[start_date:end_date]
     return df_history
 
 
 ################################################################################################################################################################################
 ################################################################################################################################################################################
+def get_ri_history(stock:str = 'خودرو', 
+                   start_date:str = '1400-01-01', 
+                   end_date:str = '1401-01-01', 
+                   ignore_date:bool = False, 
+                   show_weekday:bool = False, 
+                   double_date:bool = False) -> pd.DataFrame:
+    
+    """
+    Takes ticker or firm's full name and returns a Pandas dataframe that contains the following columns:
+    
+    J-Date: Jalali date, as index
+    Date: Gregorian date
+    Weekday: Name of weekdays
+    No_Buy_R: Number of buy trades executed by retails 
+    No_Buy_I: Number of buy trades executed by institutionals 
+    No_Sell_R: Number of sell trades executed by retails 
+    No_Sell_I: Number of sell trades executed by institutionals
+    Vol_Buy_R: Total volume are bought by retails
+    Vol_Buy_I: Total volume are bought by institutionals
+    Vol_Sell_R: Total volume are sold by retails
+    Vol_Sell_I: Total volume are sold by institutionals
+    Val_Buy_R: Total value in IRAN's Rial that are bought by retails
+    Val_Buy_I: Total value in IRAN's Rial that are bought by institutionals
+    Val_Sell_R: Total value in IRAN's Rial that are sold by retails
+    Val_Sell_I: Total value in IRAN's Rial that are sold by institutionals
+    Ticker: Ticker/Symbol
+    Name: Firm's full name
+    Market: Market, the stock is traded in
+    
+    * All data are taken from the new website of Tehran Stock Exchange.
+    
+    :param stock: (str) Ticker or firm's full name. 
+    :param start_date: (str) Jalali date for starting day of historical retail-institutional data in YYYY-MM-DD format.
+    :param end_date: (str) Jalali date for ending day of historical retail-institutional data in YYYY-MM-DD format.
+    :param ignore_date: (bool) Ignores start_date and end_date and returns all available retail-institutional history, if set to True.
+    :param show_weekday: (bool) Shows weekdays in the output, if set to True.
+    :param double_date: (bool) Shows Gregorian date in the output, if set to True.
+    :return: (pd.DataFrame) A dataframe that contains J-Date as index and Date, Weekday, No_Buy_R, No_Buy_I, No_Sell_R, No_Sell_I, Vol_Buy_R, Vol_Buy_I, Vol_Sell_R, Vol_Sell_I, Val_Buy_R, Val_Buy_I, Val_Sell_R, Val_Sell_I, Ticker, Name, Market.
+    """
+    
+    # basic request and data cleaning function for historical retail-institutional data of a ticker for a given market:
+    def get_ri_data(ticker_no, ticker, name, market):
+        r = requests.get(f'http://cdn.tsetmc.com/api/ClientType/GetClientTypeHistory/{ticker_no}',headers=headers)
+        df_RI_tab = pd.DataFrame(r.json()['clientType'])
+        cols = ['Date','WebID','Vol_Buy_R','Vol_Buy_I','Val_Buy_R','Val_Buy_I','No_Buy_I','Vol_Sell_R','No_Buy_R','Vol_Sell_I','Val_Sell_R','Val_Sell_I','No_Sell_I','No_Sell_R']
+        df_RI_tab.columns = cols
+        df_RI_tab = df_RI_tab[['Date','No_Buy_R','No_Buy_I','No_Sell_R','No_Sell_I','Vol_Buy_R','Vol_Buy_I','Vol_Sell_R','Vol_Sell_I','Val_Buy_R','Val_Buy_I','Val_Sell_R','Val_Sell_I']]
+        df_RI_tab['Date'] = df_RI_tab['Date'].apply(lambda x: str(x))
+        cols = ['No_Buy_R','No_Buy_I','No_Sell_R','No_Sell_I','Vol_Buy_R','Vol_Buy_I','Vol_Sell_R','Vol_Sell_I','Val_Buy_R','Val_Buy_I','Val_Sell_R','Val_Sell_I']
+        df_RI_tab[cols] = df_RI_tab[cols].astype('int64')
+        df_RI_tab['Date']=pd.to_datetime(df_RI_tab['Date'])
+        df_RI_tab['Ticker'] = ticker
+        df_RI_tab['Name'] = name
+        df_RI_tab['Market'] = market
+        df_RI_tab = df_RI_tab.set_index('Date')
+        return df_RI_tab
+    
+    # check to see if the entry start and end dates are valid or not:
+    if(not ignore_date):
+        start_date = __Check_JDate_Validity__(start_date,key_word="'START'")
+        if(start_date==None):
+            return
+        end_date = __Check_JDate_Validity__(end_date,key_word="'END'")
+        if(end_date==None):
+            return
+        start = jdatetime.date(year=int(start_date.split('-')[0]), month=int(start_date.split('-')[1]), day=int(start_date.split('-')[2]))
+        end = jdatetime.date(year=int(end_date.split('-')[0]), month=int(end_date.split('-')[1]), day=int(end_date.split('-')[2]))
+        if(start>end):
+            print('Start date must be a day before end date!')
+            return
+
+    # search for WebIDs:
+    ticker_no_df = get_tse_webid(stock)
+    if(type(ticker_no_df)==bool):
+        return
+    
+    # create an empty dataframe:   
+    df_RI_tab = pd.DataFrame({},columns=['Date','No_Buy_R','No_Buy_I','No_Sell_R','No_Sell_I','Vol_Buy_R','Vol_Buy_I','Vol_Sell_R',
+                                         'Vol_Sell_I','Val_Buy_R','Val_Buy_I','Val_Sell_R','Val_Sell_I','Ticker','Name','Market']).set_index('Date')
+   
+    # loop to get data from different pages of a ticker:
+    for index, row in (ticker_no_df.reset_index()).iterrows():
+        try:
+            df_temp = get_ri_data(ticker_no = row['WebID'], ticker = row['Ticker'], name = row['Name'], market = row['Market'])
+            df_RI_tab = pd.concat([df_RI_tab,df_temp])
+        except:
+            pass
+        
+    # sort date index 
+    df_RI_tab = df_RI_tab.sort_index(ascending=True)
+    df_RI_tab = df_RI_tab.reset_index()
+    
+    # add weekdays and Jalali date:
+    df_RI_tab['Weekday']=df_RI_tab['Date'].dt.weekday
+    df_RI_tab['Weekday'] = df_RI_tab['Weekday'].apply(lambda x: calendar.day_name[x])
+    df_RI_tab['J-Date']=df_RI_tab['Date'].apply(lambda x: str(jdatetime.date.fromgregorian(date=x.date())))
+    df_RI_tab.set_index(df_RI_tab['J-Date'],inplace = True)
+    df_RI_tab = df_RI_tab.set_index('J-Date')
+    
+    # rearrange columns and convert some columns to numeric:
+    df_RI_tab=df_RI_tab[['Date','Weekday','No_Buy_R','No_Buy_I','No_Sell_R','No_Sell_I','Vol_Buy_R','Vol_Buy_I','Vol_Sell_R','Vol_Sell_I',
+                         'Val_Buy_R','Val_Buy_I','Val_Sell_R','Val_Sell_I','Ticker','Name','Market']]
+    cols = ['No_Buy_R','No_Buy_I','No_Sell_R','No_Sell_I','Vol_Buy_R','Vol_Buy_I','Vol_Sell_R','Vol_Sell_I','Val_Buy_R','Val_Buy_I','Val_Sell_R','Val_Sell_I']
+    df_RI_tab[cols] = df_RI_tab[cols].apply(pd.to_numeric, axis=1)
+    
+    # drop weekdays if not requested:
+    if(not show_weekday):
+        df_RI_tab.drop(columns=['Weekday'],inplace=True)
+        
+    # drop Gregorian date if not requested:
+    if(not double_date):
+        df_RI_tab.drop(columns=['Date'],inplace=True)
+        
+    # # slice requested time window, if requested:
+    if(not ignore_date):
+        df_RI_tab = df_RI_tab[start_date:end_date]
+        
+    return df_RI_tab
+
 
 def Get_RI_History(stock = 'خودرو', start_date = '1400-01-01', end_date='1401-01-01', ignore_date = False, show_weekday = False, double_date = False, alt = False):
     """
     دریافت سابقه اطلاعات حقیقی-حقوقی یک سهم در روزهای معاملاتی بین تاریخ شروع و پایان
     قابلیت دریافت همه سابقه حقیقی-حقوقی بدون توجه به تاریخ شروع و پایان
     قابلیت ارائه تاریخ میلادی علاوه بر تاریخ شمسی، قابلیت نمایش روزهای هفته
     """
@@ -486,15 +827,15 @@
     دریافت سابقه ریز معاملات یک سهم در روزهای معاملاتی بین تاریخ شروع و پایان
     اگر فقط به داده های یک روز مشخص نیاز دارید از تاریخ شروع و پایان یکسان استفاده کنید
     توجه داشته باشید که معاملات باطل شده نماد در خروجی این تابع نمایش داده نمی شود
     """
     # a function to get price data from a given page ----------------------------------------------------------------------------------
     failed_jdates = []
     def get_price_data_forintraday(ticker_no):
-        r = requests.get(f'http://www.tsetmc.com/tsev2/data/InstTradeHistory.aspx?i={ticker_no}&Top=999999&A=0', headers=headers)
+        r = requests.get(f'http://old.tsetmc.com/tsev2/data/InstTradeHistory.aspx?i={ticker_no}&Top=999999&A=0', headers=headers)
         df_history=pd.DataFrame(r.text.split(';'))
         columns=['Date','High','Low','Final','Close','Open','Y-Final','Value','Volume','No']
         #split data into defined columns
         df_history[columns] = df_history[0].str.split("@",expand=True)
         # drop old column 0
         df_history.drop(columns=[0],inplace=True)
         df_history.dropna(inplace=True)
@@ -701,15 +1042,15 @@
 def Get_Queue_History(stock = 'وخارزم', start_date = '1400-09-15', end_date='1400-12-29', show_per_capita = True, show_weekday = False, double_date = False, show_progress = True):
     """
     دریافت ارزش صف خرید یا فروش یک سهم در زمان بسته شدن بازار، در روزهای معاملاتی بین تاریخ شروع و پایان
     اگر فقط به داده های یک روز مشخص نیاز دارید از تاریخ شروع و پایان یکسان استفاده کنید
     """
     # a function to get price data from a given page ----------------------------------------------------------------------------------
     def get_price_data_forintraday(ticker_no):
-        r = requests.get(f'http://www.tsetmc.com/tsev2/data/InstTradeHistory.aspx?i={ticker_no}&Top=999999&A=0', headers=headers)
+        r = requests.get(f'http://old.tsetmc.com/tsev2/data/InstTradeHistory.aspx?i={ticker_no}&Top=999999&A=0', headers=headers)
         df_history=pd.DataFrame(r.text.split(';'))
         columns=['Date','High','Low','Final','Close','Open','Y-Final','Value','Volume','No']
         #split data into defined columns
         df_history[columns] = df_history[0].str.split("@",expand=True)
         # drop old column 0
         df_history.drop(columns=[0],inplace=True)
         df_history.dropna(inplace=True)
@@ -823,15 +1164,15 @@
 def Get_IntradayOB_History(stock = 'کرمان', start_date = '1400-08-01', end_date='1400-08-01', jalali_date = True, combined_datatime = False, show_progress = True):
     """
     دریافت اطلاعات عرضه تقاضای اردر بوک برای یک سهم، در روزهای معاملاتی بین تاریخ شروع و پایان
     اگر فقط به داده های یک روز مشخص نیاز دارید از تاریخ شروع و پایان یکسان استفاده کنید
     """
 # a function to get price data from a given page ----------------------------------------------------------------------------------
     def get_price_data_forintraday(ticker_no):
-        r = requests.get(f'http://www.tsetmc.com/tsev2/data/InstTradeHistory.aspx?i={ticker_no}&Top=999999&A=0', headers=headers)
+        r = requests.get(f'http://old.tsetmc.com/tsev2/data/InstTradeHistory.aspx?i={ticker_no}&Top=999999&A=0', headers=headers)
         df_history=pd.DataFrame(r.text.split(';'))
         columns=['Date','High','Low','Final','Close','Open','Y-Final','Value','Volume','No']
         #split data into defined columns
         df_history[columns] = df_history[0].str.split("@",expand=True)
         # drop old column 0
         df_history.drop(columns=[0],inplace=True)
         df_history.dropna(inplace=True)
@@ -945,29 +1286,28 @@
     try:
         sector_web_id = __Get_TSE_Sector_WebID__(sector_name = sector)
     except:
         print('Please Enter a Valid Name for Sector Index!')
         return
     if(sector_web_id == None):
         return
-    r_cl = requests.get(f'http://tsetmc.com/tsev2/chart/data/Index.aspx?i={sector_web_id}&t=value', headers=headers)
-    df_sector_cl = pd.DataFrame(r_cl.text.split(';'))
-    columns=['J-Date','Adj Close']
-    df_sector_cl[columns] = df_sector_cl[0].str.split(",",expand=True)
-    df_sector_cl.drop(columns=[0],inplace=True)
-    df_sector_cl['J-Date'] = df_sector_cl['J-Date'].apply(lambda x: str(jdatetime.date(int(x.split('/')[0]),int(x.split('/')[1]),int(x.split('/')[2]))))
-    df_sector_cl['Date'] = df_sector_cl['J-Date'].apply(lambda x: jdatetime.date(int(x[:4]),int(x[5:7]),int(x[8:])).togregorian())  
-    df_sector_cl['Date'] = pd.to_datetime(df_sector_cl['Date'])
+    r_cl = requests.get(f'http://cdn.tsetmc.com/api/Index/GetIndexB2History/{sector_web_id}', headers=headers)
+    df_sector_cl = pd.DataFrame(r_cl.json()['indexB2'])[['dEven','xNivInuClMresIbs']]
+    df_sector_cl['dEven'] = df_sector_cl['dEven'].apply(lambda x: str(x))
+    df_sector_cl['dEven'] = df_sector_cl['dEven'].apply(lambda x: x[:4]+'-'+x[4:6]+'-'+x[-2:])
+    df_sector_cl['dEven'] = pd.to_datetime(df_sector_cl['dEven'])
+    df_sector_cl.rename(columns={"dEven": "Date", "xNivInuClMresIbs":"Adj Close"}, inplace=True)
+    df_sector_cl['J-Date']=df_sector_cl['Date'].apply(lambda x: str(jdatetime.date.fromgregorian(date=x.date())))
     df_sector_cl['Weekday']=df_sector_cl['Date'].dt.weekday
     df_sector_cl['Weekday'] = df_sector_cl['Weekday'].apply(lambda x: calendar.day_name[x])
     df_sector_cl = df_sector_cl.set_index('J-Date')
     df_sector_cl = df_sector_cl[['Date','Weekday','Adj Close']]
     df_sector_cl['Adj Close'] = pd.to_numeric(df_sector_cl['Adj Close'])
     if(not just_adj_close):
-        r = requests.get(f'http://www.tsetmc.com/tsev2/chart/data/IndexFinancial.aspx?i={sector_web_id}&t=ph', headers=headers)
+        r = requests.get(f'http://old.tsetmc.com/tsev2/chart/data/IndexFinancial.aspx?i={sector_web_id}&t=ph', headers=headers)
         df_sector = pd.DataFrame(r.text.split(';'))
         columns=['Date','High','Low','Open','Close','Volume','D']
         # split data into defined columns
         df_sector[columns] = df_sector[0].str.split(",",expand=True)
         df_sector.drop(columns=[0,'D'],inplace=True)
         df_sector['Date']=pd.to_datetime(df_sector['Date'])
         df_sector['J-Date']=df_sector['Date'].apply(lambda x: str(jdatetime.date.fromgregorian(date=x.date())))
@@ -1011,30 +1351,28 @@
         start = jdatetime.date(year=int(start_date.split('-')[0]), month=int(start_date.split('-')[1]), day=int(start_date.split('-')[2]))
         end = jdatetime.date(year=int(end_date.split('-')[0]), month=int(end_date.split('-')[1]), day=int(end_date.split('-')[2]))
         if(start>end):
             print('Start date must be a day before end date!')
             return
     # get sector web-id ---------------------------------------------------------------------------------------------------------------------
     sector_web_id = 5798407779416661
-    # get only close chart data for sector index:
-    r_cl = requests.get(f'http://tsetmc.com/tsev2/chart/data/Index.aspx?i={sector_web_id}&t=value', headers=headers)
-    df_sector_cl = pd.DataFrame(r_cl.text.split(';'))
-    columns=['J-Date','Adj Close']
-    df_sector_cl[columns] = df_sector_cl[0].str.split(",",expand=True)
-    df_sector_cl.drop(columns=[0],inplace=True)
-    df_sector_cl['J-Date'] = df_sector_cl['J-Date'].apply(lambda x: str(jdatetime.date(int(x.split('/')[0]),int(x.split('/')[1]),int(x.split('/')[2]))))
-    df_sector_cl['Date'] = df_sector_cl['J-Date'].apply(lambda x: jdatetime.date(int(x[:4]),int(x[5:7]),int(x[8:])).togregorian())  
-    df_sector_cl['Date'] = pd.to_datetime(df_sector_cl['Date'])
+    r_cl = requests.get(f'http://cdn.tsetmc.com/api/Index/GetIndexB2History/{sector_web_id}', headers=headers)
+    df_sector_cl = pd.DataFrame(r_cl.json()['indexB2'])[['dEven','xNivInuClMresIbs']]
+    df_sector_cl['dEven'] = df_sector_cl['dEven'].apply(lambda x: str(x))
+    df_sector_cl['dEven'] = df_sector_cl['dEven'].apply(lambda x: x[:4]+'-'+x[4:6]+'-'+x[-2:])
+    df_sector_cl['dEven'] = pd.to_datetime(df_sector_cl['dEven'])
+    df_sector_cl.rename(columns={"dEven": "Date", "xNivInuClMresIbs":"Adj Close"}, inplace=True)
+    df_sector_cl['J-Date']=df_sector_cl['Date'].apply(lambda x: str(jdatetime.date.fromgregorian(date=x.date())))
     df_sector_cl['Weekday']=df_sector_cl['Date'].dt.weekday
     df_sector_cl['Weekday'] = df_sector_cl['Weekday'].apply(lambda x: calendar.day_name[x])
     df_sector_cl = df_sector_cl.set_index('J-Date')
     df_sector_cl = df_sector_cl[['Date','Weekday','Adj Close']]
     df_sector_cl['Adj Close'] = pd.to_numeric(df_sector_cl['Adj Close'])
     if(not just_adj_close):
-        r = requests.get(f'http://www.tsetmc.com/tsev2/chart/data/IndexFinancial.aspx?i={sector_web_id}&t=ph', headers=headers)
+        r = requests.get(f'http://old.tsetmc.com/tsev2/chart/data/IndexFinancial.aspx?i={sector_web_id}&t=ph', headers=headers)
         df_sector = pd.DataFrame(r.text.split(';'))
         columns=['Date','High','Low','Open','Close','Volume','D']
         # split data into defined columns
         df_sector[columns] = df_sector[0].str.split(",",expand=True)
         df_sector.drop(columns=[0,'D'],inplace=True)
         df_sector['Date']=pd.to_datetime(df_sector['Date'])
         df_sector['J-Date']=df_sector['Date'].apply(lambda x: str(jdatetime.date.fromgregorian(date=x.date())))
@@ -1143,30 +1481,28 @@
         start = jdatetime.date(year=int(start_date.split('-')[0]), month=int(start_date.split('-')[1]), day=int(start_date.split('-')[2]))
         end = jdatetime.date(year=int(end_date.split('-')[0]), month=int(end_date.split('-')[1]), day=int(end_date.split('-')[2]))
         if(start>end):
             print('Start date must be a day before end date!')
             return
     # get sector web-id ---------------------------------------------------------------------------------------------------------------------
     sector_web_id = 49579049405614711
-    # get only close chart data for sector index:
-    r_cl = requests.get(f'http://tsetmc.com/tsev2/chart/data/Index.aspx?i={sector_web_id}&t=value', headers=headers)
-    df_sector_cl = pd.DataFrame(r_cl.text.split(';'))
-    columns=['J-Date','Adj Close']
-    df_sector_cl[columns] = df_sector_cl[0].str.split(",",expand=True)
-    df_sector_cl.drop(columns=[0],inplace=True)
-    df_sector_cl['J-Date'] = df_sector_cl['J-Date'].apply(lambda x: str(jdatetime.date(int(x.split('/')[0]),int(x.split('/')[1]),int(x.split('/')[2]))))
-    df_sector_cl['Date'] = df_sector_cl['J-Date'].apply(lambda x: jdatetime.date(int(x[:4]),int(x[5:7]),int(x[8:])).togregorian())  
-    df_sector_cl['Date'] = pd.to_datetime(df_sector_cl['Date'])
+    r_cl = requests.get(f'http://cdn.tsetmc.com/api/Index/GetIndexB2History/{sector_web_id}', headers=headers)
+    df_sector_cl = pd.DataFrame(r_cl.json()['indexB2'])[['dEven','xNivInuClMresIbs']]
+    df_sector_cl['dEven'] = df_sector_cl['dEven'].apply(lambda x: str(x))
+    df_sector_cl['dEven'] = df_sector_cl['dEven'].apply(lambda x: x[:4]+'-'+x[4:6]+'-'+x[-2:])
+    df_sector_cl['dEven'] = pd.to_datetime(df_sector_cl['dEven'])
+    df_sector_cl.rename(columns={"dEven": "Date", "xNivInuClMresIbs":"Adj Close"}, inplace=True)
+    df_sector_cl['J-Date']=df_sector_cl['Date'].apply(lambda x: str(jdatetime.date.fromgregorian(date=x.date())))
     df_sector_cl['Weekday']=df_sector_cl['Date'].dt.weekday
     df_sector_cl['Weekday'] = df_sector_cl['Weekday'].apply(lambda x: calendar.day_name[x])
     df_sector_cl = df_sector_cl.set_index('J-Date')
     df_sector_cl = df_sector_cl[['Date','Weekday','Adj Close']]
     df_sector_cl['Adj Close'] = pd.to_numeric(df_sector_cl['Adj Close'])
     if(not just_adj_close):
-        r = requests.get(f'http://www.tsetmc.com/tsev2/chart/data/IndexFinancial.aspx?i={sector_web_id}&t=ph', headers=headers)
+        r = requests.get(f'http://old.tsetmc.com/tsev2/chart/data/IndexFinancial.aspx?i={sector_web_id}&t=ph', headers=headers)
         df_sector = pd.DataFrame(r.text.split(';'))
         columns=['Date','High','Low','Open','Close','Volume','D']
         # split data into defined columns
         df_sector[columns] = df_sector[0].str.split(",",expand=True)
         df_sector.drop(columns=[0,'D'],inplace=True)
         df_sector['Date']=pd.to_datetime(df_sector['Date'])
         df_sector['J-Date']=df_sector['Date'].apply(lambda x: str(jdatetime.date.fromgregorian(date=x.date())))
@@ -1209,30 +1545,28 @@
         start = jdatetime.date(year=int(start_date.split('-')[0]), month=int(start_date.split('-')[1]), day=int(start_date.split('-')[2]))
         end = jdatetime.date(year=int(end_date.split('-')[0]), month=int(end_date.split('-')[1]), day=int(end_date.split('-')[2]))
         if(start>end):
             print('Start date must be a day before end date!')
             return
     # get sector web-id ---------------------------------------------------------------------------------------------------------------------
     sector_web_id = 62752761908615603
-    # get only close chart data for sector index:
-    r_cl = requests.get(f'http://tsetmc.com/tsev2/chart/data/Index.aspx?i={sector_web_id}&t=value', headers=headers)
-    df_sector_cl = pd.DataFrame(r_cl.text.split(';'))
-    columns=['J-Date','Adj Close']
-    df_sector_cl[columns] = df_sector_cl[0].str.split(",",expand=True)
-    df_sector_cl.drop(columns=[0],inplace=True)
-    df_sector_cl['J-Date'] = df_sector_cl['J-Date'].apply(lambda x: str(jdatetime.date(int(x.split('/')[0]),int(x.split('/')[1]),int(x.split('/')[2]))))
-    df_sector_cl['Date'] = df_sector_cl['J-Date'].apply(lambda x: jdatetime.date(int(x[:4]),int(x[5:7]),int(x[8:])).togregorian())  
-    df_sector_cl['Date'] = pd.to_datetime(df_sector_cl['Date'])
+    r_cl = requests.get(f'http://cdn.tsetmc.com/api/Index/GetIndexB2History/{sector_web_id}', headers=headers)
+    df_sector_cl = pd.DataFrame(r_cl.json()['indexB2'])[['dEven','xNivInuClMresIbs']]
+    df_sector_cl['dEven'] = df_sector_cl['dEven'].apply(lambda x: str(x))
+    df_sector_cl['dEven'] = df_sector_cl['dEven'].apply(lambda x: x[:4]+'-'+x[4:6]+'-'+x[-2:])
+    df_sector_cl['dEven'] = pd.to_datetime(df_sector_cl['dEven'])
+    df_sector_cl.rename(columns={"dEven": "Date", "xNivInuClMresIbs":"Adj Close"}, inplace=True)
+    df_sector_cl['J-Date']=df_sector_cl['Date'].apply(lambda x: str(jdatetime.date.fromgregorian(date=x.date())))
     df_sector_cl['Weekday']=df_sector_cl['Date'].dt.weekday
     df_sector_cl['Weekday'] = df_sector_cl['Weekday'].apply(lambda x: calendar.day_name[x])
     df_sector_cl = df_sector_cl.set_index('J-Date')
     df_sector_cl = df_sector_cl[['Date','Weekday','Adj Close']]
     df_sector_cl['Adj Close'] = pd.to_numeric(df_sector_cl['Adj Close'])
     if(not just_adj_close):
-        r = requests.get(f'http://www.tsetmc.com/tsev2/chart/data/IndexFinancial.aspx?i={sector_web_id}&t=ph', headers=headers)
+        r = requests.get(f'http://old.tsetmc.com/tsev2/chart/data/IndexFinancial.aspx?i={sector_web_id}&t=ph', headers=headers)
         df_sector = pd.DataFrame(r.text.split(';'))
         columns=['Date','High','Low','Open','Close','Volume','D']
         # split data into defined columns
         df_sector[columns] = df_sector[0].str.split(",",expand=True)
         df_sector.drop(columns=[0,'D'],inplace=True)
         df_sector['Date']=pd.to_datetime(df_sector['Date'])
         df_sector['J-Date']=df_sector['Date'].apply(lambda x: str(jdatetime.date.fromgregorian(date=x.date())))
@@ -1276,29 +1610,28 @@
         end = jdatetime.date(year=int(end_date.split('-')[0]), month=int(end_date.split('-')[1]), day=int(end_date.split('-')[2]))
         if(start>end):
             print('Start date must be a day before end date!')
             return
     # get sector web-id ---------------------------------------------------------------------------------------------------------------------
     sector_web_id = 71704845530629737
     # get only close chart data for sector index:
-    r_cl = requests.get(f'http://tsetmc.com/tsev2/chart/data/Index.aspx?i={sector_web_id}&t=value', headers=headers)
-    df_sector_cl = pd.DataFrame(r_cl.text.split(';'))
-    columns=['J-Date','Adj Close']
-    df_sector_cl[columns] = df_sector_cl[0].str.split(",",expand=True)
-    df_sector_cl.drop(columns=[0],inplace=True)
-    df_sector_cl['J-Date'] = df_sector_cl['J-Date'].apply(lambda x: str(jdatetime.date(int(x.split('/')[0]),int(x.split('/')[1]),int(x.split('/')[2]))))
-    df_sector_cl['Date'] = df_sector_cl['J-Date'].apply(lambda x: jdatetime.date(int(x[:4]),int(x[5:7]),int(x[8:])).togregorian())  
-    df_sector_cl['Date'] = pd.to_datetime(df_sector_cl['Date'])
+    r_cl = requests.get(f'http://cdn.tsetmc.com/api/Index/GetIndexB2History/{sector_web_id}', headers=headers)
+    df_sector_cl = pd.DataFrame(r_cl.json()['indexB2'])[['dEven','xNivInuClMresIbs']]
+    df_sector_cl['dEven'] = df_sector_cl['dEven'].apply(lambda x: str(x))
+    df_sector_cl['dEven'] = df_sector_cl['dEven'].apply(lambda x: x[:4]+'-'+x[4:6]+'-'+x[-2:])
+    df_sector_cl['dEven'] = pd.to_datetime(df_sector_cl['dEven'])
+    df_sector_cl.rename(columns={"dEven": "Date", "xNivInuClMresIbs":"Adj Close"}, inplace=True)
+    df_sector_cl['J-Date']=df_sector_cl['Date'].apply(lambda x: str(jdatetime.date.fromgregorian(date=x.date())))
     df_sector_cl['Weekday']=df_sector_cl['Date'].dt.weekday
     df_sector_cl['Weekday'] = df_sector_cl['Weekday'].apply(lambda x: calendar.day_name[x])
     df_sector_cl = df_sector_cl.set_index('J-Date')
     df_sector_cl = df_sector_cl[['Date','Weekday','Adj Close']]
     df_sector_cl['Adj Close'] = pd.to_numeric(df_sector_cl['Adj Close'])
     if(not just_adj_close):
-        r = requests.get(f'http://www.tsetmc.com/tsev2/chart/data/IndexFinancial.aspx?i={sector_web_id}&t=ph', headers=headers)
+        r = requests.get(f'http://old.tsetmc.com/tsev2/chart/data/IndexFinancial.aspx?i={sector_web_id}&t=ph', headers=headers)
         df_sector = pd.DataFrame(r.text.split(';'))
         columns=['Date','High','Low','Open','Close','Volume','D']
         # split data into defined columns
         df_sector[columns] = df_sector[0].str.split(",",expand=True)
         df_sector.drop(columns=[0,'D'],inplace=True)
         df_sector['Date']=pd.to_datetime(df_sector['Date'])
         df_sector['J-Date']=df_sector['Date'].apply(lambda x: str(jdatetime.date.fromgregorian(date=x.date())))
@@ -1342,29 +1675,28 @@
         end = jdatetime.date(year=int(end_date.split('-')[0]), month=int(end_date.split('-')[1]), day=int(end_date.split('-')[2]))
         if(start>end):
             print('Start date must be a day before end date!')
             return
     # get sector web-id ---------------------------------------------------------------------------------------------------------------------
     sector_web_id = 43754960038275285
     # get only close chart data for sector index:
-    r_cl = requests.get(f'http://tsetmc.com/tsev2/chart/data/Index.aspx?i={sector_web_id}&t=value', headers=headers)
-    df_sector_cl = pd.DataFrame(r_cl.text.split(';'))
-    columns=['J-Date','Adj Close']
-    df_sector_cl[columns] = df_sector_cl[0].str.split(",",expand=True)
-    df_sector_cl.drop(columns=[0],inplace=True)
-    df_sector_cl['J-Date'] = df_sector_cl['J-Date'].apply(lambda x: str(jdatetime.date(int(x.split('/')[0]),int(x.split('/')[1]),int(x.split('/')[2]))))
-    df_sector_cl['Date'] = df_sector_cl['J-Date'].apply(lambda x: jdatetime.date(int(x[:4]),int(x[5:7]),int(x[8:])).togregorian())  
-    df_sector_cl['Date'] = pd.to_datetime(df_sector_cl['Date'])
+    r_cl = requests.get(f'http://cdn.tsetmc.com/api/Index/GetIndexB2History/{sector_web_id}', headers=headers)
+    df_sector_cl = pd.DataFrame(r_cl.json()['indexB2'])[['dEven','xNivInuClMresIbs']]
+    df_sector_cl['dEven'] = df_sector_cl['dEven'].apply(lambda x: str(x))
+    df_sector_cl['dEven'] = df_sector_cl['dEven'].apply(lambda x: x[:4]+'-'+x[4:6]+'-'+x[-2:])
+    df_sector_cl['dEven'] = pd.to_datetime(df_sector_cl['dEven'])
+    df_sector_cl.rename(columns={"dEven": "Date", "xNivInuClMresIbs":"Adj Close"}, inplace=True)
+    df_sector_cl['J-Date']=df_sector_cl['Date'].apply(lambda x: str(jdatetime.date.fromgregorian(date=x.date())))
     df_sector_cl['Weekday']=df_sector_cl['Date'].dt.weekday
     df_sector_cl['Weekday'] = df_sector_cl['Weekday'].apply(lambda x: calendar.day_name[x])
     df_sector_cl = df_sector_cl.set_index('J-Date')
     df_sector_cl = df_sector_cl[['Date','Weekday','Adj Close']]
     df_sector_cl['Adj Close'] = pd.to_numeric(df_sector_cl['Adj Close'])
     if(not just_adj_close):
-        r = requests.get(f'http://www.tsetmc.com/tsev2/chart/data/IndexFinancial.aspx?i={sector_web_id}&t=ph', headers=headers)
+        r = requests.get(f'http://old.tsetmc.com/tsev2/chart/data/IndexFinancial.aspx?i={sector_web_id}&t=ph', headers=headers)
         df_sector = pd.DataFrame(r.text.split(';'))
         columns=['Date','High','Low','Open','Close','Volume','D']
         # split data into defined columns
         df_sector[columns] = df_sector[0].str.split(",",expand=True)
         df_sector.drop(columns=[0,'D'],inplace=True)
         df_sector['Date']=pd.to_datetime(df_sector['Date'])
         df_sector['J-Date']=df_sector['Date'].apply(lambda x: str(jdatetime.date.fromgregorian(date=x.date())))
@@ -1408,29 +1740,28 @@
         end = jdatetime.date(year=int(end_date.split('-')[0]), month=int(end_date.split('-')[1]), day=int(end_date.split('-')[2]))
         if(start>end):
             print('Start date must be a day before end date!')
             return
     # get sector web-id ---------------------------------------------------------------------------------------------------------------------
     sector_web_id = 10523825119011581
     # get only close chart data for sector index:
-    r_cl = requests.get(f'http://tsetmc.com/tsev2/chart/data/Index.aspx?i={sector_web_id}&t=value', headers=headers)
-    df_sector_cl = pd.DataFrame(r_cl.text.split(';'))
-    columns=['J-Date','Adj Close']
-    df_sector_cl[columns] = df_sector_cl[0].str.split(",",expand=True)
-    df_sector_cl.drop(columns=[0],inplace=True)
-    df_sector_cl['J-Date'] = df_sector_cl['J-Date'].apply(lambda x: str(jdatetime.date(int(x.split('/')[0]),int(x.split('/')[1]),int(x.split('/')[2]))))
-    df_sector_cl['Date'] = df_sector_cl['J-Date'].apply(lambda x: jdatetime.date(int(x[:4]),int(x[5:7]),int(x[8:])).togregorian())  
-    df_sector_cl['Date'] = pd.to_datetime(df_sector_cl['Date'])
+    r_cl = requests.get(f'http://cdn.tsetmc.com/api/Index/GetIndexB2History/{sector_web_id}', headers=headers)
+    df_sector_cl = pd.DataFrame(r_cl.json()['indexB2'])[['dEven','xNivInuClMresIbs']]
+    df_sector_cl['dEven'] = df_sector_cl['dEven'].apply(lambda x: str(x))
+    df_sector_cl['dEven'] = df_sector_cl['dEven'].apply(lambda x: x[:4]+'-'+x[4:6]+'-'+x[-2:])
+    df_sector_cl['dEven'] = pd.to_datetime(df_sector_cl['dEven'])
+    df_sector_cl.rename(columns={"dEven": "Date", "xNivInuClMresIbs":"Adj Close"}, inplace=True)
+    df_sector_cl['J-Date']=df_sector_cl['Date'].apply(lambda x: str(jdatetime.date.fromgregorian(date=x.date())))
     df_sector_cl['Weekday']=df_sector_cl['Date'].dt.weekday
     df_sector_cl['Weekday'] = df_sector_cl['Weekday'].apply(lambda x: calendar.day_name[x])
     df_sector_cl = df_sector_cl.set_index('J-Date')
     df_sector_cl = df_sector_cl[['Date','Weekday','Adj Close']]
     df_sector_cl['Adj Close'] = pd.to_numeric(df_sector_cl['Adj Close'])
     if(not just_adj_close):
-        r = requests.get(f'http://www.tsetmc.com/tsev2/chart/data/IndexFinancial.aspx?i={sector_web_id}&t=ph', headers=headers)
+        r = requests.get(f'http://old.tsetmc.com/tsev2/chart/data/IndexFinancial.aspx?i={sector_web_id}&t=ph', headers=headers)
         df_sector = pd.DataFrame(r.text.split(';'))
         columns=['Date','High','Low','Open','Close','Volume','D']
         # split data into defined columns
         df_sector[columns] = df_sector[0].str.split(",",expand=True)
         df_sector.drop(columns=[0,'D'],inplace=True)
         df_sector['Date']=pd.to_datetime(df_sector['Date'])
         df_sector['J-Date']=df_sector['Date'].apply(lambda x: str(jdatetime.date.fromgregorian(date=x.date())))
@@ -1474,29 +1805,28 @@
         end = jdatetime.date(year=int(end_date.split('-')[0]), month=int(end_date.split('-')[1]), day=int(end_date.split('-')[2]))
         if(start>end):
             print('Start date must be a day before end date!')
             return
     # get sector web-id ---------------------------------------------------------------------------------------------------------------------
     sector_web_id = 46342955726788357
     # get only close chart data for sector index:
-    r_cl = requests.get(f'http://tsetmc.com/tsev2/chart/data/Index.aspx?i={sector_web_id}&t=value', headers=headers)
-    df_sector_cl = pd.DataFrame(r_cl.text.split(';'))
-    columns=['J-Date','Adj Close']
-    df_sector_cl[columns] = df_sector_cl[0].str.split(",",expand=True)
-    df_sector_cl.drop(columns=[0],inplace=True)
-    df_sector_cl['J-Date'] = df_sector_cl['J-Date'].apply(lambda x: str(jdatetime.date(int(x.split('/')[0]),int(x.split('/')[1]),int(x.split('/')[2]))))
-    df_sector_cl['Date'] = df_sector_cl['J-Date'].apply(lambda x: jdatetime.date(int(x[:4]),int(x[5:7]),int(x[8:])).togregorian())  
-    df_sector_cl['Date'] = pd.to_datetime(df_sector_cl['Date'])
+    r_cl = requests.get(f'http://cdn.tsetmc.com/api/Index/GetIndexB2History/{sector_web_id}', headers=headers)
+    df_sector_cl = pd.DataFrame(r_cl.json()['indexB2'])[['dEven','xNivInuClMresIbs']]
+    df_sector_cl['dEven'] = df_sector_cl['dEven'].apply(lambda x: str(x))
+    df_sector_cl['dEven'] = df_sector_cl['dEven'].apply(lambda x: x[:4]+'-'+x[4:6]+'-'+x[-2:])
+    df_sector_cl['dEven'] = pd.to_datetime(df_sector_cl['dEven'])
+    df_sector_cl.rename(columns={"dEven": "Date", "xNivInuClMresIbs":"Adj Close"}, inplace=True)
+    df_sector_cl['J-Date']=df_sector_cl['Date'].apply(lambda x: str(jdatetime.date.fromgregorian(date=x.date())))
     df_sector_cl['Weekday']=df_sector_cl['Date'].dt.weekday
     df_sector_cl['Weekday'] = df_sector_cl['Weekday'].apply(lambda x: calendar.day_name[x])
     df_sector_cl = df_sector_cl.set_index('J-Date')
     df_sector_cl = df_sector_cl[['Date','Weekday','Adj Close']]
     df_sector_cl['Adj Close'] = pd.to_numeric(df_sector_cl['Adj Close'])
     if(not just_adj_close):
-        r = requests.get(f'http://www.tsetmc.com/tsev2/chart/data/IndexFinancial.aspx?i={sector_web_id}&t=ph', headers=headers)
+        r = requests.get(f'http://old.tsetmc.com/tsev2/chart/data/IndexFinancial.aspx?i={sector_web_id}&t=ph', headers=headers)
         df_sector = pd.DataFrame(r.text.split(';'))
         columns=['Date','High','Low','Open','Close','Volume','D']
         # split data into defined columns
         df_sector[columns] = df_sector[0].str.split(",",expand=True)
         df_sector.drop(columns=[0,'D'],inplace=True)
         df_sector['Date']=pd.to_datetime(df_sector['Date'])
         df_sector['J-Date']=df_sector['Date'].apply(lambda x: str(jdatetime.date.fromgregorian(date=x.date())))
@@ -2543,19 +2873,19 @@
         return
     ticker_no_df.reset_index(inplace=True)
     ticker_no_df = ticker_no_df[ticker_no_df['Active']==1]
     wid = ticker_no_df['WEB-ID'].values[0]
     market = ticker_no_df['Market'].values[0]
 
     # get isin id
-    r = requests.get(f'http://www.tsetmc.com/Loader.aspx?Partree=15131M&i={wid}', headers=headers)
+    r = requests.get(f'http://old.tsetmc.com/Loader.aspx?Partree=15131M&i={wid}', headers=headers)
     isin_id = pd.read_html(r.text)[0].iloc[7,1]
 
     # get shareholders data
-    r = requests.get(f'http://www.tsetmc.com/Loader.aspx?Partree=15131T&c={isin_id}', headers=headers)
+    r = requests.get(f'http://old.tsetmc.com/Loader.aspx?Partree=15131T&c={isin_id}', headers=headers)
     soup = BeautifulSoup(r.text, 'html.parser')
     table = soup.findAll("table", {"class": "table1"})[0].findAll("tr", {"class": "sh"})
 
     # extarct data and create dataframe
     name_list = []
     out_list = []
     per_list = []
```

### Comparing `finpy_tse-1.2.4/finpy_tse.egg-info/PKG-INFO` & `finpy_tse-1.2.5/finpy_tse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finpy-tse
-Version: 1.2.4
+Version: 1.2.5
 Summary: A Python Module to Access Tehran Stock Exchange Historical and Real-Time Data
 Author: ALI RAHIMI  AND  RASOOL GHAFOURI
 Author-email: a.rahimi.aut@gmail.com
 License: BSD (3-clause)
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `finpy_tse-1.2.4/setup.py` & `finpy_tse-1.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name='finpy_tse',                           # should match the package folder
     packages=['finpy_tse'],                     # should match the package folder
-    version='1.2.4',                            # important for updates
+    version='1.2.5',                            # important for updates
     license='BSD (3-clause)',                                  # should match your chosen license
     description='A Python Module to Access Tehran Stock Exchange Historical and Real-Time Data',
     long_description=long_description,              # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='ALI RAHIMI  AND  RASOOL GHAFOURI',
     author_email='a.rahimi.aut@gmail.com',
     install_requires=['requests','jdatetime','pandas','numpy','requests','bs4','asyncio','urllib3','aiohttp','unsync','IPython','persiantools','datetime','XlsxWriter','lxml'],                  # list all packages that your package uses
```

