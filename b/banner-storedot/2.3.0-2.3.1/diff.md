# Comparing `tmp/banner-storedot-2.3.0.tar.gz` & `tmp/banner-storedot-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "banner-storedot-2.3.0.tar", last modified: Tue May 16 12:13:57 2023, max compression
+gzip compressed data, was "banner-storedot-2.3.1.tar", last modified: Sat May 27 10:46:29 2023, max compression
```

## Comparing `banner-storedot-2.3.0.tar` & `banner-storedot-2.3.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-05-16 12:13:57.677067 banner-storedot-2.3.0/
--rw-rwSr--   0 gil       (1008) developers  (1234)     1073 2021-08-19 08:44:05.000000 banner-storedot-2.3.0/LICENSE
--rw-r--r--   0 gil       (1008) developers  (1234)     8235 2023-05-16 12:13:57.677067 banner-storedot-2.3.0/PKG-INFO
--rw-rwSr--   0 gil       (1008) developers  (1234)     7782 2022-07-18 10:09:00.000000 banner-storedot-2.3.0/README.md
--rw-rwSr--   0 gil       (1008) developers  (1234)      122 2021-08-19 10:21:45.000000 banner-storedot-2.3.0/pyproject.toml
--rw-rwSr--   0 gil       (1008) developers  (1234)      672 2023-05-16 12:13:57.677067 banner-storedot-2.3.0/setup.cfg
-drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-05-16 12:13:57.669067 banner-storedot-2.3.0/src/
-drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-05-16 12:13:57.673067 banner-storedot-2.3.0/src/banner/
--rw-rwSr--   0 gil       (1008) developers  (1234)      161 2022-11-08 14:34:28.000000 banner-storedot-2.3.0/src/banner/__init__.py
--rw-rwSr--   0 gil       (1008) developers  (1234)    27556 2023-05-16 12:12:09.000000 banner-storedot-2.3.0/src/banner/connection.py
--rw-rwSr--   0 gil       (1008) developers  (1234)     6164 2023-03-20 12:23:23.000000 banner-storedot-2.3.0/src/banner/pandas_decorator.py
--rw-rwSr--   0 gil       (1008) developers  (1234)     2121 2022-01-09 16:04:35.000000 banner-storedot-2.3.0/src/banner/pandas_wrap.py
--rw-rwSr--   0 gil       (1008) developers  (1234)    52211 2023-05-16 12:12:15.000000 banner-storedot-2.3.0/src/banner/queries.py
-drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-05-16 12:13:57.673067 banner-storedot-2.3.0/src/banner/utils/
--rw-rwSr--   0 gil       (1008) developers  (1234)        0 2021-08-19 11:04:29.000000 banner-storedot-2.3.0/src/banner/utils/__init__.py
--rw-rwSr--   0 gil       (1008) developers  (1234)     3798 2022-12-22 09:12:51.000000 banner-storedot-2.3.0/src/banner/utils/const.py
--rw-rwSr--   0 gil       (1008) developers  (1234)     1923 2023-03-23 08:47:01.000000 banner-storedot-2.3.0/src/banner/utils/misc.py
--rw-rwSr--   0 gil       (1008) developers  (1234)    10202 2023-05-09 07:24:41.000000 banner-storedot-2.3.0/src/banner/utils/neware.py
--rw-rwSr--   0 gil       (1008) developers  (1234)     1952 2022-08-17 11:13:16.000000 banner-storedot-2.3.0/src/banner/utils/pandas.py
--rw-rwSr--   0 gil       (1008) developers  (1234)   182089 2023-05-09 12:41:23.000000 banner-storedot-2.3.0/src/banner/utils/web2py.py
-drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-05-16 12:13:57.677067 banner-storedot-2.3.0/src/banner_storedot.egg-info/
--rw-rwSr--   0 gil       (1008) developers  (1234)     8235 2023-05-16 12:13:57.000000 banner-storedot-2.3.0/src/banner_storedot.egg-info/PKG-INFO
--rw-rwSr--   0 gil       (1008) developers  (1234)      544 2023-05-16 12:13:57.000000 banner-storedot-2.3.0/src/banner_storedot.egg-info/SOURCES.txt
--rw-rwSr--   0 gil       (1008) developers  (1234)        1 2023-05-16 12:13:57.000000 banner-storedot-2.3.0/src/banner_storedot.egg-info/dependency_links.txt
--rw-rwSr--   0 gil       (1008) developers  (1234)       75 2023-05-16 12:13:57.000000 banner-storedot-2.3.0/src/banner_storedot.egg-info/requires.txt
--rw-rwSr--   0 gil       (1008) developers  (1234)        7 2023-05-16 12:13:57.000000 banner-storedot-2.3.0/src/banner_storedot.egg-info/top_level.txt
+drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-05-27 10:46:29.556936 banner-storedot-2.3.1/
+-rw-rwSr--   0 gil       (1008) developers  (1234)     1073 2021-08-19 08:44:05.000000 banner-storedot-2.3.1/LICENSE
+-rw-r--r--   0 gil       (1008) developers  (1234)     8235 2023-05-27 10:46:29.556936 banner-storedot-2.3.1/PKG-INFO
+-rw-rwSr--   0 gil       (1008) developers  (1234)     7782 2022-07-18 10:09:00.000000 banner-storedot-2.3.1/README.md
+-rw-rwSr--   0 gil       (1008) developers  (1234)      122 2021-08-19 10:21:45.000000 banner-storedot-2.3.1/pyproject.toml
+-rw-r--r--   0 gil       (1008) developers  (1234)      672 2023-05-27 10:46:29.556936 banner-storedot-2.3.1/setup.cfg
+drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-05-27 10:46:29.552936 banner-storedot-2.3.1/src/
+drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-05-27 10:46:29.552936 banner-storedot-2.3.1/src/banner/
+-rw-rwSr--   0 gil       (1008) developers  (1234)      161 2022-11-08 14:34:28.000000 banner-storedot-2.3.1/src/banner/__init__.py
+-rw-r--r--   0 gil       (1008) developers  (1234)    30331 2023-05-27 10:45:17.000000 banner-storedot-2.3.1/src/banner/connection.py
+-rw-r--r--   0 gil       (1008) developers  (1234)     6632 2023-05-27 10:45:17.000000 banner-storedot-2.3.1/src/banner/pandas_decorator.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)     2121 2022-01-09 16:04:35.000000 banner-storedot-2.3.1/src/banner/pandas_wrap.py
+-rw-r--r--   0 gil       (1008) developers  (1234)    52804 2023-05-27 10:45:17.000000 banner-storedot-2.3.1/src/banner/queries.py
+drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-05-27 10:46:29.556936 banner-storedot-2.3.1/src/banner/utils/
+-rw-rwSr--   0 gil       (1008) developers  (1234)        0 2021-08-19 11:04:29.000000 banner-storedot-2.3.1/src/banner/utils/__init__.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)     3798 2022-12-22 09:12:51.000000 banner-storedot-2.3.1/src/banner/utils/const.py
+-rw-r--r--   0 gil       (1008) developers  (1234)     2042 2023-05-27 10:45:17.000000 banner-storedot-2.3.1/src/banner/utils/misc.py
+-rw-r--r--   0 gil       (1008) developers  (1234)    10250 2023-05-27 10:45:17.000000 banner-storedot-2.3.1/src/banner/utils/neware.py
+-rw-rwSr--   0 gil       (1008) developers  (1234)     1952 2022-08-17 11:13:16.000000 banner-storedot-2.3.1/src/banner/utils/pandas.py
+-rw-r--r--   0 gil       (1008) developers  (1234)   182362 2023-05-27 10:45:17.000000 banner-storedot-2.3.1/src/banner/utils/web2py.py
+drwxr-sr-x   0 gil       (1008) developers  (1234)        0 2023-05-27 10:46:29.556936 banner-storedot-2.3.1/src/banner_storedot.egg-info/
+-rw-rwSr--   0 gil       (1008) developers  (1234)     8235 2023-05-27 10:46:29.000000 banner-storedot-2.3.1/src/banner_storedot.egg-info/PKG-INFO
+-rw-rwSr--   0 gil       (1008) developers  (1234)      544 2023-05-27 10:46:29.000000 banner-storedot-2.3.1/src/banner_storedot.egg-info/SOURCES.txt
+-rw-rwSr--   0 gil       (1008) developers  (1234)        1 2023-05-27 10:46:29.000000 banner-storedot-2.3.1/src/banner_storedot.egg-info/dependency_links.txt
+-rw-rwSr--   0 gil       (1008) developers  (1234)       75 2023-05-27 10:46:29.000000 banner-storedot-2.3.1/src/banner_storedot.egg-info/requires.txt
+-rw-rwSr--   0 gil       (1008) developers  (1234)        7 2023-05-27 10:46:29.000000 banner-storedot-2.3.1/src/banner_storedot.egg-info/top_level.txt
```

### Comparing `banner-storedot-2.3.0/LICENSE` & `banner-storedot-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.3.0/PKG-INFO` & `banner-storedot-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banner-storedot
-Version: 2.3.0
+Version: 2.3.1
 Summary: light dal package
 Home-page: https://https://github.com/storedot/banner
 Author: GB
 Author-email: gilb@store-dot.com
 Project-URL: Bug Tracker, https://https://github.com/storedot/banner/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `banner-storedot-2.3.0/README.md` & `banner-storedot-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.3.0/setup.cfg` & `banner-storedot-2.3.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = banner-storedot
-version = 2.3.0
+version = 2.3.1
 author = GB
 author_email = gilb@store-dot.com
 description = light dal package
 long_description = file: README.md
 url = https://https://github.com/storedot/banner
 project_urls = 
 	Bug Tracker = https://https://github.com/storedot/banner/issues
```

### Comparing `banner-storedot-2.3.0/src/banner/connection.py` & `banner-storedot-2.3.1/src/banner/connection.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,20 +28,21 @@
 
 from banner.utils.const import TTL_KWARG, NW_CACHE_COLUMNS
 from banner.utils.misc import digested_key #Banner
 from banner.utils.pandas import parse_mysql_to_pandas_query
 from banner.utils.web2py import LABEL_TO_COLUMN
 
 class ConnectionType(Enum):
+    ''' What connection types are supported by ConnectionFactory'''
     mysql = 'mysql'
     redis = 'redis'
     postgres = 'postgres'
 
 class ConnectionFactory(object):
-    ''' Connection Factory'''
+    ''' Create and return a Connection based on given data, defaults to MySqlConnection'''
     def __new__(self, con_type: Union[ConnectionType, str] = ConnectionType.mysql, **kwargs):
         try:
             con_type = ConnectionType[con_type]
 
         except KeyError:
             pass
             
@@ -50,157 +51,176 @@
         
         if con_type is ConnectionType.redis:
             return RedisConnection(**kwargs)
             
         return MySqlConnection(**kwargs)        
 
 class Connection(ABC):
+    ''' Abstract Connection, Defines Connection required methods '''
     @abstractmethod
     def retrieve(self):
         pass
 
     @abstractmethod
     def store(self):
         pass
 
 class RelationalConnection(Connection):
+    ''' A Relcational Connection'''
     @abstractmethod
     def describe(self, table: str = ''):
         pass
 
 class Storage(Connection):
+    ''' A Key/Value Connection'''
     @abstractmethod
     def keys(self, query):
         pass
 
 class PrintableConnection(Connection):
+    ''' print mixin'''
     @abstractmethod
     def name(self):
         pass
     
     @abstractmethod
     def __str__(self):
         pass
 
 class RedisConnection(Storage, PrintableConnection):
+    ''' Connection with Redis db which is a printable Storage(Connection) '''
     HOUR = 3600
 
     def __init__(self, host, port=6379, passwd=None, db=0, ssl_key=None, ssl_cert=None, ssl_ca_cert=None, name=None, ttl=HOUR):
         self.data = dict(
             host=host,
             port=port,
             password=passwd,
             db=db,
             ssl_keyfile=ssl_key,
             ssl_certfile=ssl_cert,
             ssl_ca_certs=ssl_ca_cert,
             ssl=any([ssl_key, ssl_cert, ssl_ca_cert])
-        )
+        ) # all args and kwargs are stored in here
 
-        self.__ttl = ttl or RedisConnection.HOUR
-        self.__name = name
+        self.__ttl = ttl or RedisConnection.HOUR # default ttl used
+        self.__name = name # connection name
 
         # Redis manages opening/closing by itself, it is safe to init it here
         self.instance = redis.Redis(
             **self.data, 
             decode_responses=True
-        )
+        ) # The actual instance of redis
     
     def keys(self, query: str):
         '''
             Retrieve Keys from Storage
         '''
         return self.instance.keys(pattern=f'{str(query)}')
 
     def retrieve(self, func: callable, *args, **kwargs):
         '''
-            Retrieve Value from Storage
+            Retrieve Value from Storage for a callable
         '''
-        controller = QUERY_TO_STORAGE_CONTROL.get(func.__name__, DefaultStorageController)
+        controller = QUERY_TO_STORAGE_CONTROL.get(
+            func.__name__, DefaultStorageController
+        ) # Try get storage controller based on func, otherwise DefaultStorageController
 
         return controller.retrieve(
             self.instance, func, *args, **kwargs
-        )
+        ) # Use the controller to get value from db
         
     def store(self, value, func: callable, *args, ttl=None, nx=True, **kwargs):
         '''
             Set Value Into Storage
         '''
-        ttl = ttl if ttl else self.__ttl
+        ttl = ttl if ttl else self.__ttl # determine ttl
 
-        controller = QUERY_TO_STORAGE_CONTROL.get(func.__name__, DefaultStorageController)
+        controller = QUERY_TO_STORAGE_CONTROL.get(
+            func.__name__, DefaultStorageController
+        ) # Try get storage controller based on func, otherwise DefaultStorageController
         
         return controller.store(
             self.instance, value, func, *args, ttl=ttl, nx=nx, **kwargs
-        )
+        ) # Use the controller to store value in db
 
     def retrieve_by(self, keys: Union[str, list]): #TODO support json
+        ''' retrieve an str or a list of strs '''
         if isinstance(keys, str):
             return self.instance.get(keys)
         
         return self.instance.mget(keys)
         
     def store_by(self, key: str, value, ttl=None, nx=True):
+        ''' 
+            store value under key, for ttl 
+            force update if nx=False
+        '''
         ttl = ttl if ttl else self.__ttl
 
         resp = self.instance.set(
             key, value, ex=ttl, nx=nx
         )
 
         if resp is True:
             return key
 
         raise KeyError(f'{key} Exists')
         
     @property
-    def name(self):
+    def name(self): # name of the connection
         return self.__name or str(self.data)
 
-    def __str__(self):
+    def __str__(self): 
         return self.name
             
 class MySqlConnection(RelationalConnection, PrintableConnection):
+    ''' Connection with Mysql db which is a printable RelationalConnection(Connection) '''
     def __init__(self, host, user, port=3306, passwd=None, db=None, ssl_key=None, ssl_cert=None, charset='utf8', use_unicode=True, name=None):
         self.data = dict(
             host=host,
             user=user,
             port=port,
             passwd=passwd,
             db=db,
             ssl=dict(key=ssl_key, cert=ssl_cert),
             charset=charset,
             use_unicode=use_unicode,
             cursorclass=DictCursor 
-        )
+        )  # all args and kwargs are stored in here
 
         self.__name = name
 
     def retrieve(self, query: str):
+        ''' 
+            get value(df) for mysql query(str) 
+        '''
         try:
             instance = self.__connect()
             
             cursor = instance.cursor()
             
-            cursor.execute(query)
+            cursor.execute(query) # the actualy query
 
             records = cursor.fetchall()
 
             cursor.close()
         
             records = DataFrame(records).convert_dtypes()
             
         except MySQLError as e:
             raise e
         
         finally:
-            self.__close(instance)        
+            self.__close(instance) # handle closing the connection       
 
         return records
 
     def store(self, statement: str, *args, unique_checks=True, foreign_key_checks=True):
+        ''' execute mysql statement for updating db data '''
         prefix, suffix = list(), list()
 
         if not unique_checks:
             prefix.append('SET unique_checks=0;')
             suffix.insert(0, 'SET unique_checks=1;')
 
         if not foreign_key_checks:
@@ -211,33 +231,34 @@
             instance = self.__connect()
             
             cursor = instance.cursor()
             
             for q in prefix:
                 cursor.execute(q)
 
-            cursor.execute(statement, *args)
+            cursor.execute(statement, *args) # the actualy query
             
             for q in suffix:
                 cursor.execute(q)
             
             instance.commit()
             
             cursor.close()
             
         except MySQLError as e:
-            instance.rollback()
+            instance.rollback() # if an error occures, rollback
             raise e
         
         finally:
-            self.__close(instance)
+            self.__close(instance) # handle closing the connection
         
-        return cursor.rowcount
+        return cursor.rowcount # return number of updated rows
 
     def describe(self, table: str = ''):
+        ''' Describe table or whole schema '''
         _query = f"SELECT table_name FROM information_schema.tables WHERE table_schema = '{self.data.get('db')}'"
 
         if table:
             _query = f'DESCRIBE {table}'
 
         return self.retrieve(_query)
 
@@ -261,14 +282,15 @@
     def name(self):
         return self.__name or str(self.data)
 
     def __str__(self):
         return self.name
 
 class PostgresSqlConnection(RelationalConnection, PrintableConnection):
+    ''' Connection with Postgressql db which is a printable RelationalConnection(Connection) '''
     def __init__(self, host, user, port=5432, passwd=None, db=None, ssl_key=None, ssl_cert=None, charset='utf8', name=None):
         self.data = dict(
             host=host,
             port=port,
             user=user,
             password=passwd,
             dbname=db,
@@ -276,32 +298,35 @@
             sslcert=ssl_cert
         )
 
         self.__name = name
         self.__charset = charset
         
     def retrieve(self, query: str):
+        ''' 
+            get value(df) for mysql query(str) 
+        '''
         try:
             instance = self.__connect()
             
             cursor = instance.cursor(cursor_factory=RealDictCursor)
             
-            cursor.execute(query)
+            cursor.execute(query)  # the actualy query
             
             records = cursor.fetchall()
             
             cursor.close()
         
             records = DataFrame(records).convert_dtypes()
 
         except PostgresSQLError as e:
             raise e
         
         finally:
-            self.__close(instance)        
+            self.__close(instance) # handle closing the connection     
 
         return records
 
     def store(self, statement: str):
         try:
             instance = self.__connect()
             
@@ -310,23 +335,24 @@
             cursor.execute(statement)
 
             instance.commit()
             
             cursor.close()
             
         except PostgresSQLDatabaseError as e:
-            instance.rollback()
+            instance.rollback() # if an error occures, rollback
             raise e
         
         finally:
-            self.__close(instance)
+            self.__close(instance) # handle closing the connection
 
         return cursor.rowcount
 
     def describe(self, table: str = ''):
+        ''' Describe table or whole schema '''
         _query = f"SELECT table_name FROM information_schema.tables"
 
         if table:
             _query = (
                 'SELECT column_name as "Field", data_type as "Type", is_nullable as "Null", column_default as "Default"'
                 f" FROM INFORMATION_SCHEMA.COLUMNS WHERE table_name = '{table}'"
             )
@@ -357,26 +383,27 @@
         return self.__name or str(self.data)
 
     def __str__(self):
         return self.name
 
 class StorageController(ABC):
     '''
-        Handles Store&Retrieve from Data Storage
+        Handles Store & Retrieve from Data Storage
     '''
     @abstractmethod
     def store(): # Return Command to fetch the data
         pass
 
     @abstractmethod
     def retrieve(): # Return Command to fetch the data
         pass
 
     @staticmethod
     def value_of(param: str, default, func: callable, *args, **kwargs):
+        ''' determine if a param exists from given args, kwargs and return its value, otherwise return default'''
         return kwargs.get(param, StorageController.__value_of_arg(param, default, func, *args))
 
     @staticmethod
     def __value_of_arg(arg: str, default, func: callable, *args):
         try:
             index = getfullargspec(func).args.index(arg)
 
@@ -385,15 +412,15 @@
             return args[index]
 
         except (AssertionError, IndexError, KeyError, ValueError):
             return default
 
 class DefaultStorageController(StorageController):
     '''
-        Default Storage Controller
+        Default Storage Controller, The default way to handle store & retrieve from Storage instance
     '''
     NUM_OF_KEYS = 10
     MAX_ROWS = 100000
 
     @staticmethod
     def __table_index(func: callable, *args, **kwargs):
         try:
@@ -420,17 +447,17 @@
     ):  
         keys = DefaultStorageController.__keys(func, *args, **kwargs)
         values = value.split(size=DefaultStorageController.MAX_ROWS) # This is a banner function
         
         for key, val in zip(keys, values):
             resp = storage.set(
                 key, val.to_json(orient='records'), ex=ttl, nx=nx
-            )
+            ) # set each value under key
 
-            if not resp:
+            if not resp: 
                 raise redis.ResponseError
             
         return True
 
     @staticmethod
     def retrieve(
         storage: redis.client.Redis, func: callable, *args, **kwargs
@@ -453,19 +480,21 @@
             df._tables = [table] # Set table metadata
 
         return df
 
 class NewareCacheController(DefaultStorageController):
     '''
         Neware Cache Data(DataFrame) Storage Controller
+        Handle store & retrieve for neware cache tables
     '''
-    PRIMARY_KEY = ['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id']
+    PRIMARY_KEY = ['ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id'] # pk for cache table
 
     @staticmethod
     def __keys(func: callable, *args, **kwargs):
+        ''' return keys arg from callable else return digested key'''
         _keys_index = NewareCacheController.__keys_index(func, *args, **kwargs)
         
         try:
             assert(_keys_index >= 0)
             
             if (all(isinstance(item, Iterable) for item in args[_keys_index])):
                 _keys = [tuple(key) for key in args[_keys_index]] # Make sure each key(collection) is a tuple
@@ -505,14 +534,15 @@
         for pk, val in zip(reversed(NewareCacheController.PRIMARY_KEY), reversed(key.split('-'))):
             df.insert(0, pk, val)
         
         return df
 
     @staticmethod
     def __should_cache(condition: str, columns: list):
+        ''' Determine if the query should be cached'''
         try: # More cases may appear, this can include all
             if condition and condition.lower() not in ['true', 1]: # Make sure condition doesnt create a partial result
                 raise ValueError
             
             if set(columns) != NW_CACHE_COLUMNS: # Make sure we have all cache columns!
                 raise ValueError
 
@@ -531,28 +561,28 @@
         condition = kwargs.get('condition', False)
         columns = kwargs.get('columns')
 
         if not columns or columns == '*':
             columns = value.columns
 
         if not NewareCacheController.__should_cache(condition, columns): # Partial value is given #TODO, should still be cached
-            return DefaultStorageController.store(storage, value, func, *args, ttl=ttl, nx=nx, **kwargs)
+            return DefaultStorageController.store(storage, value, func, *args, ttl=ttl, nx=nx, **kwargs) # use default since, since its a partial result
 
         try: 
             data = value.groupby(NewareCacheController.PRIMARY_KEY).apply(NewareCacheController.__dump)
             
             for key, val in data.items():
                 _key = '-'.join(map(str, key))
                 
                 resp = storage.json().set(
                     _key, Path.root_path(), val, nx=nx
-                )
+                ) # set each series by _key
                 
                 if resp:
-                    storage.expire(_key, ttl)
+                    storage.expire(_key, ttl) # if it was set, update ttl
                 
             return True
 
         except (TypeError, KeyError, redis.ResponseError):
             raise
         
     @staticmethod
@@ -563,34 +593,34 @@
         condition = kwargs.get('condition', False)
         columns = kwargs.get('columns') # Requested columns
 
         if not columns or columns == '*':
             columns = NW_CACHE_COLUMNS
 
         if not NewareCacheController.__should_cache(condition, columns): # Partial value is given #TODO, value should be retrieved and completed!
-            return DefaultStorageController.retrieve(storage, func, *args, **kwargs)
+            return DefaultStorageController.retrieve(storage, func, *args, **kwargs) # use default since, since its a partial result
         
         keys = NewareCacheController.__keys(func, *args, **kwargs) # Expected Keys
         
         try:
             values = storage.json().mget(keys, Path.root_path())
             values = list(filter(None, values)) # Remove Empty entries
             
-            assert(len(values) == len(keys))
+            assert(len(values) == len(keys)) # make sure we have all values, #TODO more precise
             
             df = concat(
                 [NewareCacheController.__load(key, value) for key, value in zip(keys, values)],
                 ignore_index=True
-            )
+            ) #into a df
             
             for column in df[NewareCacheController.PRIMARY_KEY].columns:
-                df[column] = df[column].astype(int64)
+                df[column] = df[column].astype(int64) # All pk columns to type int
 
             for column in df.filter(like='time').columns:
-                df[column] = df[column].astype('datetime64[ms]')
+                df[column] = df[column].astype('datetime64[ms]') # time columns into datetime
             
             return df[list(columns)].convert_dtypes()
 
         except (AssertionError, redis.ResponseError):
             return DataFrame()
 
 class NewareTestController(NewareCacheController):
@@ -647,37 +677,37 @@
         func: callable, *args, 
         ttl=None, nx=True, **kwargs
     ):  
         kwargs = deepcopy(kwargs)
         cache_data, condition = kwargs.get('cache_data'), parse_mysql_to_pandas_query(kwargs.get('condition', ''))
         raw = kwargs.get('raw', False)
         
-        if not NewareTestController.__should_cache(cache_data, condition, raw):
-            return DefaultStorageController.store(storage, value, func, *args, ttl=43200, nx=nx, **kwargs)
+        if not NewareTestController.__should_cache(cache_data, condition, raw): # Partial value is given #TODO, should still be cached
+            return DefaultStorageController.store(storage, value, func, *args, ttl=43200, nx=nx, **kwargs) # use default since, since its a partial result
         
         try: 
             partial_key = list(cache_data[NewareTestController.PRIMARY_KEY].iloc[-1]) # A single test so grab any(last) row
             
             data = value.groupby(NewareTestController.VALUE_GROUP_KEY).apply(NewareTestController.__dump) 
             
             for cycle, cycle_data in data.items(): 
                 _key = f"{'-'.join(map(str, partial_key))}-{int(cycle)}"
                 
                 resp = storage.json().set(_key, Path.root_path(), {},  nx=nx) # Make sure Key exists
 
                 if resp:
-                    storage.expire(_key, ttl)
+                    storage.expire(_key, ttl) # if it was set, update ttl
                 
                 for column, column_data in cycle_data.items(): # TODO with a single command (currently not implemented by redis)
                     if column in NW_CACHE_COLUMNS: # Case column belong to NW_CACHE_COLUMNS
                         column_data = column_data[0] # Only first value since neware_cache values are per cycle!
                         
                     resp = storage.json().set(
                         _key, Path(column), column_data, nx=nx
-                    )
+                    ) # set series by _key path
                         
             return True
 
         except (TypeError, KeyError, IndexError, UndefinedVariableError, redis.ResponseError):
             raise
 
     @staticmethod
@@ -685,37 +715,37 @@
         storage: redis.client.Redis, func: callable, *args, **kwargs
     ):  
         kwargs = deepcopy(kwargs)
         cache_data, condition = kwargs.get('cache_data'), parse_mysql_to_pandas_query(kwargs.get('condition', ''))
         raw = kwargs.get('raw', False) 
         temperature = kwargs.get('temperature', False)
         
-        if not NewareTestController.__should_cache(cache_data, condition, raw):
-            return DefaultStorageController.retrieve(storage, func, *args, **kwargs)
+        if not NewareTestController.__should_cache(cache_data, condition, raw): # Partial value is given #TODO, value should be retrieved and completed!
+            return DefaultStorageController.retrieve(storage, func, *args, **kwargs) # use default since, since its a partial result
         
         try:
             if condition and condition.lower() not in ['true', 1]:
                 cache_data = cache_data.query(condition, engine='python') # Only supports query on cache
             
             cycles = set(cache_data[NewareTestController.VALUE_GROUP_KEY]) # Ordered by default
             
             partial_key = list(cache_data[NewareTestController.PRIMARY_KEY].iloc[-1]) # A single test so grab any(last) row
             
             keys = [f"{'-'.join(map(str, partial_key))}-{cycle}" for cycle in cycles]
             
-            values = storage.json().mget(keys, Path.root_path())
+            values = storage.json().mget(keys, Path.root_path()) # grab all data
             
             values = list(filter(None, values)) # Remove Empty entries
             
             assert(len(values) == len(keys)) # TODO - HANDLE PARTIAL RESULT! (ONLY certain cycles in cache)
             
             df = concat(
                 [NewareTestController.__load(cycle, value) for cycle, value in zip(cycles, values)],
                 ignore_index=True
-            )
+            ) # into df
             
             columns = kwargs.get('columns')
             
             if not isinstance(columns, list): # columns can be * (mysql all) or something invalid
                 columns = df.columns
 
             if temperature:
```

### Comparing `banner-storedot-2.3.0/src/banner/pandas_decorator.py` & `banner-storedot-2.3.1/src/banner/pandas_decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,18 @@
 # Wrapper around Queries.table_query
 def __join_table(
     df: DataFrame, table: str, columns: Union[list, str] = '*', condition: str = 'TRUE',
     left: Union[str, list, None] = None, right: Union[str, list, None] = None, how: Union[str, None] = None,
     connection: Union[RelationalConnection, str] = None, represent: bool = False,
     raw: bool = False, cache: Storage=None, ttl: Union[bool, None] = None, nx: bool = True,
     **kwargs
-):  
+):
+    ''' 
+        Join a df representing web2py table rows with another web2py table 
+    '''
     _df = df.copy()
     
     try:
         assert(isinstance(df._tables, list)) # Is a list
         assert(df._tables) # Is not empty
  
     except (AssertionError, AttributeError):
@@ -67,36 +70,37 @@
     
     if len(df._tables) == 1: #First Join
         _df.columns = [f'{df._tables[0]}.{column}' for column in _df.columns] # Prefix columns
 
     for df_table in df._tables: # Iterate available tables
         join_params = JOINS.get(df_table, dict()).get(table, dict())
 
-        _how = how if how else join_params.get('how')
-        _left = left if left else join_params.get('left')
-        _right = right if right else join_params.get('right')
+        _how = how if how else join_params.get('how') # how the join should be performed
+        _left = left if left else join_params.get('left') # left keys
+        _right = right if right else join_params.get('right') # right keys
         
         if not all([_left, _right, _how]):
             continue
         
         if not isinstance(_left, list):
-            _left = [_left]
+            _left = [_left] # a single value was given
     
         if not isinstance(_right, list):
-            _right = [_right]
+            _right = [_right] # a single value was given
         
         _left = [
             f'{df_table}.{column}' if f'{df_table}.{column}' in _df else f'{df_table}.{COLUMN_TO_LABEL.get(column)}'
             for column in _left
         ] #Add table prefix
         
         try:
             _keys = _df[_left].dropna() # Keys cannot contain NA values
             _keys = zip(*[_keys[column].values for column in _left]) # as Iterable
             # the neware cache tables contain only numeric values
+            # Cache tables are a special case
             if table == 'neware_cache':
                 table_df = Queries.neware_cache_query(
                     list(_keys), columns=columns, condition=condition, 
                     connection=connection, cache=cache, ttl=ttl,
                     **kwargs
                 )
 
@@ -117,40 +121,40 @@
             else:
                 # keys may contain str values
                 _keys = [to_mysql_tuple(values) for values in _keys] # as Iterable of strings
                 
                 table_df = Queries.table_query(
                     table, columns=columns, condition=f"({','.join(_right)}) IN ({','.join(_keys)}) AND {condition}",
                     represent=represent, raw=raw, connection=connection, cache=cache, ttl=ttl, nx=nx, **kwargs
-                )
+                ) # for any other table use table_query
             
             table_df.columns = [f'{table}.{column}' for column in table_df.columns] # Prefix columns
             
             _right = [
                 f'{table}.{column}' if f'{table}.{column}' in table_df else f'{table}.{COLUMN_TO_LABEL.get(column)}'
                 for column in _right
             ] #Add table prefix
             
-            tables = df._tables + [table]
+            tables = df._tables + [table] # the resulting tables metadata
             
             for left_column, right_column in zip(_left, _right):
                 table_df[right_column] = table_df[right_column].astype(_df[left_column].dtype) # Make sure right_column has same data type as left_column
             
             _df = _df.merge(
                 table_df, how=_how, 
                 left_on=_left, right_on=_right,
                 # suffixes=(f'_{df_table}', f'_{table}')
-            )
+            ) # join the dfs
             
             _df._tables = tables # Set Current Tables
             
             return _df
 
-        except (KeyError, MySQLError):
+        except (KeyError, MySQLError): # the given df may contain multiple tables, if one fails, try the next
             continue
         
-    raise TypeError(f'Failed to join {table} With {df._tables}')
+    raise TypeError(f'Failed to join {table} With {df._tables}') # No table was suitable for the join params, raise exception
 
 
 # Queries
 DataFrame.join_table = __join_table
 DataFrame.table_query = Queries.table_query
```

### Comparing `banner-storedot-2.3.0/src/banner/pandas_wrap.py` & `banner-storedot-2.3.1/src/banner/pandas_wrap.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.3.0/src/banner/queries.py` & `banner-storedot-2.3.1/src/banner/queries.py`

 * *Files 0% similar despite different names*

```diff
@@ -869,14 +869,15 @@
     COLUMN_UPDATED_ON_INDEX = '_updated_on' # index column suffix
 
     PER_CELL_UNIQUE_COLUMNS = ['cell_table', 'cell_id'] # Unique columns (pk) per cell table
     PER_TEST_UNIQUE_COLUMNS = ['augm_per_cell', 'test_id'] # Unique columns (pk) per test table
     PER_CYCLE_UNIQUE_COLUMNS = ['augm_per_test', 'ip', 'dev_uid', 'unit_id', 'chl_id', 'test_id', 'cycle'] # Unique columns (pk) per cycle table
 
     def __init__(self, connection: RelationalConnection):
+        # set instance values
         self._connection = connection
 
         self.prefix = 'augm'
 
         self.per_cycle_table = AugmentQueries.PER_CYCLE_TABLE
         self.per_cell_table = AugmentQueries.PER_CELL_TABLE
         self.per_test_table = AugmentQueries.PER_TEST_TABLE
@@ -903,46 +904,46 @@
             self.per_anode_table: AugmentQueries.PER_CYCLE_UNIQUE_COLUMNS,
             self.per_cell_table: AugmentQueries.PER_CELL_UNIQUE_COLUMNS,
             self.per_test_table: AugmentQueries.PER_TEST_UNIQUE_COLUMNS,
         }
 
         self.primary_columns = ['cell_table', 'cell_id', 'test_id', 'cycle']
 
-
     def __assert_table(self, table: str):
         if table not in self.tables:
             raise ValueError(f'Available {self.__class__.__name__} Tables: {self.tables}')
     
     def get_keys_per_table(self, data: pd.DataFrame, table: str):
         columns = self.required_columns_for_table.get(table)
         
         return [str(tuple(row)) for _, row in data[columns].iterrows()]
  
     def set_features(self, table: str, features: pd.DataFrame, columns: list, validate=True): # TABLE, CELL, TEST_ID, CYCLE 
+        ''' Given a features df, set/update columns'''
         # Only keep required columns + columns
         self.__assert_table(table)
 
         _columns = self.primary_columns + columns
         
         features = features[features.columns.intersection(set(_columns))]
         
         if validate:
-            features = self.__filter_non_existant(table, features)
+            features = self.__filter_non_existant(table, features) # make sure pks are valid 
         
-        keys = self.get_keys_per_table(features, self.per_cell_table)
+        keys = self.get_keys_per_table(features, self.per_cell_table) # table pks per cell
         
         self.__create_rows_per_table(keys, self.per_cell_table) # Create Per Cell Rows!
         
         features = features.merge(
             self.__get_per_table_rows(keys, self.per_cell_table), # Relevant Rows
             how='left', on=self.required_columns_for_table.get(self.per_cell_table)
         ) # Add params
         
         if table != self.per_cell_table: # Tests/Cycles/Pulses/Anode
-            keys = self.get_keys_per_table(features, self.per_test_table)
+            keys = self.get_keys_per_table(features, self.per_test_table) # table pks per cell
             
             self.__create_rows_per_table(keys, self.per_test_table) # Create Per Test Rows!
             
             features = features.merge(
                 self.__get_per_table_rows(keys, self.per_test_table), # Relevant Rows
                 how='left', 
                 on=self.required_columns_for_table.get(self.per_test_table)
@@ -951,14 +952,20 @@
             if table != self.per_test_table: # Cycles/Pulses/Anode
                 features = self.__create_and_get_rows_per_cycle_pulse_or_anode(features, table)
                 
         for part in features.split(): # Banner function 
             self.__set_feature(table, part, columns) # Set feature into table
         
     def add_feature(self, table: str, name: str, dtype: str, index=False, description=False, updated_on=False):
+        ''' 
+            Add a new column to the db(self._connection)
+            Set column as index if True,
+            Add column_description if True,
+            Add column_updated_on if True
+        '''
         self.__assert_table(table)
         
         self.__add_column(table, name, dtype)
 
         if index:
             self.__add_index(table, name)
 
@@ -1004,34 +1011,36 @@
                 ON DUPLICATE KEY
                 UPDATE {",".join(on_duplicate)};
             """,
             connection=self._connection
         )
 
     def __set_feature(self, table: str, features: pd.DataFrame, columns: list):
+        ''' Actual function to update the rows '''
         if not columns or features.empty:
             return
         
         columns = list(columns)
         
         _columns = [*self.required_columns_for_table.get(table), *columns]
         
         _features = features[_columns] # augm_per_test requires id!
         
-        table_description = Queries.describe_table(table, connection=self._connection)
+        table_description = Queries.describe_table(table, connection=self._connection) # description of the table
         
         updated_on_columns = list()
 
         for column in columns:
+            # Set updated_on for column
             if (column_updated_on_index := f'{column}{AugmentQueries.COLUMN_UPDATED_ON_INDEX}') in table_description.Field.values:
                 updated_on_columns.append(column_updated_on_index)
         
         _features = _features.assign(**{
             column: datetime.now().strftime(AugmentQueries.TIMESTAMP_FORMAT) for column in updated_on_columns
-        })
+        }) # with updated_on
         
         columns.extend(updated_on_columns)
 
         values = tuple(
             tuple(row) for row in _features.values.tolist() # Iterate every row
         )
         placeholders = ','.join('%s' for val in values)
@@ -1193,14 +1202,15 @@
         self.primary_columns = ['cell_table', 'cell_id', 'test_id', 'cycle', 'predictor']
 
         self.unique_columns = ['name', 'version']
 
         self.model_column = 'model'
 
     def set_update_predictors(self, predictors: pd.DataFrame):
+        ''' Predictor table has a blob type column, model, which requires special handling '''
         predictor_columns = Queries.describe_table('predictor', connection=self._connection)['Field'].values
 
         _predictors = predictors[predictors.columns.intersection(set(predictor_columns))] # Intersection of given columns with available columns
         
         _predictors = _predictors.loc[:,~_predictors.columns.str.endswith('updated_on')] # updated_on columns should not be set manually
         
         updated_on_columns = list() # list of updated_on columns
```

### Comparing `banner-storedot-2.3.0/src/banner/utils/const.py` & `banner-storedot-2.3.1/src/banner/utils/const.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.3.0/src/banner/utils/misc.py` & `banner-storedot-2.3.1/src/banner/utils/misc.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 from hashlib import md5
 from pandas import DataFrame
 
 def is_non_string_iterable(value):
     return isinstance(value, Iterable) and not isinstance(value, str)
 
 def to_sql_range(values:Union[Number, Iterable], column: str, table:str = '', op='IN'):
+    ''' Create a mysql condition from given args'''
     if not isinstance(values, Iterable):
         values = [values]
     
     __left_bracket, __join_by, __right_bracket = ('"', '|', '"') if op.lower() == 'regexp' else ('(', ', ', ')')
 
     __values = __join_by.join([str(value) for value in values])
 
     _column = f'{table}.{column}' if table else column
 
     return f'{_column} {op} {__left_bracket}{__values}{__right_bracket}'
 
 def digested_key(func: callable, *args, **kwargs):
+    ''' create a unique str identifier for given function call '''
     key = f'{func.__name__}-{"_".join(str(arg) for arg in args).strip()}'
 
     if kwargs:
         _kwargs = "_".join(
             [f'{key}:{str(value).strip()}' for key, value in kwargs.items() if type(value) not in (DataFrame, )]
         )
         key += f'-{_kwargs}'
```

### Comparing `banner-storedot-2.3.0/src/banner/utils/neware.py` & `banner-storedot-2.3.1/src/banner/utils/neware.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,22 +212,21 @@
         Merge neware dataframe(data)
         With neware cache dataframe(cache_data)
         Raises TypeError, IndexError for bad input
     '''
     assert_required_columns(df, NW_SEQ)
     assert_required_columns(cache_df, NW_CACHE_CYCLE_SEQ)
     
-    cache_df = cache_df.sort_values([NW_CACHE_CYCLE_SEQ])
+    cache_df = cache_df.sort_values([NW_CACHE_CYCLE_SEQ]) # make sure cache is order(asc)
     
-    CACHE_SEQ_RANGE = [0] + list(cache_df[NW_CACHE_CYCLE_SEQ]) + [np.inf]
+    CACHE_SEQ_RANGE = [0] + list(cache_df[NW_CACHE_CYCLE_SEQ]) + [np.inf] # Buckets for each cycle
     
     columns = cache_df.columns.intersection(set(columns))
 
     def __merge_cache(group):
-        
         try:
             cache_row = cache_df[cache_df[NW_CACHE_CYCLE_SEQ] == group.name.right].iloc[-1]
            
             return group.assign(**cache_row[columns])
             
         except IndexError:
             return group
```

### Comparing `banner-storedot-2.3.0/src/banner/utils/pandas.py` & `banner-storedot-2.3.1/src/banner/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `banner-storedot-2.3.0/src/banner/utils/web2py.py` & `banner-storedot-2.3.1/src/banner/utils/web2py.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     )
     
     target_column = f'{join_table}.{column}{REPRESENT_LABEL}'
     
     return table_df[target_column] if target_column in table_df else NA
 
 # This is only partial, we will fill the rest as requests come
-# Represent dict
+# Represent dict of columns in web2py
 REPRESENTS = dict(
     pilot_pouch=dict(
         id=lambda id: 'P-' + id.astype(str),
         electrolyte_ct=lambda electrolyte_ct: _repr_by_join('id', 'pilot_pouch', 'el_batch', electrolyte_ct),
         anode_id=lambda anode_id:  _repr_by_join('id', 'pilot_pouch', 'pouch_anode', anode_id),
         cathode_id=lambda cathode_id:  _repr_by_join('id', 'pilot_pouch', 'pouch_cathode', cathode_id),
     ),
@@ -585,14 +585,17 @@
         us_cell_test=dict(left='id', right='test_type_id', how='left'),
     ),
     material=dict(
         material_type=dict(left='type', right='id', how='left'),
     ),
 )
 
+# Column and its Label in web2py
+# This is static to avoid mysql queries
+# TODO PER TABLE
 COLUMN_TO_LABEL = {
     'a_batch_id': 'Anode batch',
     'a_chg': 'A Chg',
     'a_dchg': 'A Dchg',
     'a_el_batch': 'resulting batch (A)',
     'a_fraction_id': 'Anode fraction',
     'a_load': 'Anode load',
@@ -2205,14 +2208,17 @@
     'yield_analysis_observation_comment': 'Defective cells observation',
     'z_abs': 'Z Abs',
     'z_im': 'Z Im',
     'z_re': 'Z Re',
     'zero_voltage_on': 'NW API Zero voltage on',
 }
 
+# Label and its Column in web2py
+# This is static to avoid mysql queries
+# TODO PER TABLE
 LABEL_TO_COLUMN = {
     'Anode batch': 'a_batch_id',
     'A Chg': 'a_chg',
     'A Dchg': 'a_dchg',
     'resulting batch (A)': 'a_el_batch',
     'Anode fraction': 'a_fraction_id',
     'Anode load': 'a_load',
@@ -3825,10 +3831,11 @@
     'Defective cells observation': 'yield_analysis_observation_comment',
     'Z Abs': 'z_abs',
     'Z Im': 'z_im',
     'Z Re': 'z_re',
     'NW API Zero voltage on': 'zero_voltage_on',
 }
 
+# Place holder for prefix, suffix description (used mainly for tracker)
 PREFIX_SUFFIX = dict(
 
 )
```

### Comparing `banner-storedot-2.3.0/src/banner_storedot.egg-info/PKG-INFO` & `banner-storedot-2.3.1/src/banner_storedot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banner-storedot
-Version: 2.3.0
+Version: 2.3.1
 Summary: light dal package
 Home-page: https://https://github.com/storedot/banner
 Author: GB
 Author-email: gilb@store-dot.com
 Project-URL: Bug Tracker, https://https://github.com/storedot/banner/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `banner-storedot-2.3.0/src/banner_storedot.egg-info/SOURCES.txt` & `banner-storedot-2.3.1/src/banner_storedot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

