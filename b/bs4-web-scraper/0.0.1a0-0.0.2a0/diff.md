# Comparing `tmp/bs4_web_scraper-0.0.1a0.tar.gz` & `tmp/bs4_web_scraper-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs4_web_scraper-0.0.1a0.tar", last modified: Fri May 26 23:22:29 2023, max compression
+gzip compressed data, was "bs4_web_scraper-0.0.2a0.tar", last modified: Sat May 27 13:17:27 2023, max compression
```

## Comparing `bs4_web_scraper-0.0.1a0.tar` & `bs4_web_scraper-0.0.2a0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 23:22:29.895487 bs4_web_scraper-0.0.1a0/
--rw-rw-rw-   0        0        0     1104 2023-03-07 14:14:59.000000 bs4_web_scraper-0.0.1a0/LICENSE.md
--rw-rw-rw-   0        0        0     8982 2023-05-26 23:22:29.887485 bs4_web_scraper-0.0.1a0/PKG-INFO
--rw-rw-rw-   0        0        0     7640 2023-05-23 10:51:10.000000 bs4_web_scraper-0.0.1a0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 23:22:29.599099 bs4_web_scraper-0.0.1a0/bs4_web_scraper/
--rw-rw-rw-   0        0        0     3540 2023-05-26 23:04:23.000000 bs4_web_scraper-0.0.1a0/bs4_web_scraper/__init__.py
--rw-rw-rw-   0        0        0    40789 2023-05-23 10:50:11.000000 bs4_web_scraper-0.0.1a0/bs4_web_scraper/base.py
--rw-rw-rw-   0        0        0     2102 2023-03-29 00:08:41.000000 bs4_web_scraper-0.0.1a0/bs4_web_scraper/exceptions.py
--rw-rw-rw-   0        0        0    12777 2023-05-23 09:26:13.000000 bs4_web_scraper-0.0.1a0/bs4_web_scraper/file_handler.py
--rw-rw-rw-   0        0        0     5646 2023-05-23 10:16:08.000000 bs4_web_scraper-0.0.1a0/bs4_web_scraper/logging.py
--rw-rw-rw-   0        0        0     4858 2023-03-29 00:08:41.000000 bs4_web_scraper-0.0.1a0/bs4_web_scraper/request_limiter.py
--rw-rw-rw-   0        0        0    34749 2023-05-23 10:08:35.000000 bs4_web_scraper-0.0.1a0/bs4_web_scraper/scraper.py
--rw-rw-rw-   0        0        0    22653 2023-05-23 10:23:40.000000 bs4_web_scraper-0.0.1a0/bs4_web_scraper/translate.py
--rw-rw-rw-   0        0        0     3906 2023-03-29 00:08:41.000000 bs4_web_scraper-0.0.1a0/bs4_web_scraper/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 23:22:29.879483 bs4_web_scraper-0.0.1a0/bs4_web_scraper.egg-info/
--rw-rw-rw-   0        0        0     8982 2023-05-26 23:22:29.000000 bs4_web_scraper-0.0.1a0/bs4_web_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      486 2023-05-26 23:22:29.000000 bs4_web_scraper-0.0.1a0/bs4_web_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 23:22:29.000000 bs4_web_scraper-0.0.1a0/bs4_web_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2023-05-26 23:22:29.000000 bs4_web_scraper-0.0.1a0/bs4_web_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-26 23:22:29.000000 bs4_web_scraper-0.0.1a0/bs4_web_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1732 2023-05-26 23:19:16.000000 bs4_web_scraper-0.0.1a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 23:22:29.895487 bs4_web_scraper-0.0.1a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-27 13:17:27.724143 bs4_web_scraper-0.0.2a0/
+-rw-rw-rw-   0        0        0     1104 2023-03-07 14:14:59.000000 bs4_web_scraper-0.0.2a0/LICENSE.md
+-rw-rw-rw-   0        0        0    19317 2023-05-27 13:17:27.721146 bs4_web_scraper-0.0.2a0/PKG-INFO
+-rw-rw-rw-   0        0        0    17975 2023-05-27 12:26:05.000000 bs4_web_scraper-0.0.2a0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 13:17:27.461665 bs4_web_scraper-0.0.2a0/bs4_web_scraper/
+-rw-rw-rw-   0        0        0     3623 2023-05-27 13:15:42.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper/__init__.py
+-rw-rw-rw-   0        0        0    41404 2023-05-27 13:07:58.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper/base.py
+-rw-rw-rw-   0        0        0     2102 2023-03-29 00:08:41.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper/exceptions.py
+-rw-rw-rw-   0        0        0    12777 2023-05-23 09:26:13.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper/file_handler.py
+-rw-rw-rw-   0        0        0     5642 2023-05-27 10:03:10.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper/logging.py
+-rw-rw-rw-   0        0        0     4858 2023-03-29 00:08:41.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper/request_limiter.py
+-rw-rw-rw-   0        0        0    35513 2023-05-27 13:08:15.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper/scraper.py
+-rw-rw-rw-   0        0        0    22737 2023-05-27 12:41:04.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper/translate.py
+-rw-rw-rw-   0        0        0     3906 2023-03-29 00:08:41.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-27 13:17:27.712146 bs4_web_scraper-0.0.2a0/bs4_web_scraper.egg-info/
+-rw-rw-rw-   0        0        0    19317 2023-05-27 13:17:27.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      486 2023-05-27 13:17:27.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 13:17:27.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2023-05-27 13:17:27.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-27 13:17:27.000000 bs4_web_scraper-0.0.2a0/bs4_web_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1732 2023-05-27 13:15:22.000000 bs4_web_scraper-0.0.2a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-27 13:17:27.725142 bs4_web_scraper-0.0.2a0/setup.cfg
```

### Comparing `bs4_web_scraper-0.0.1a0/LICENSE.md` & `bs4_web_scraper-0.0.2a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.0.1a0/bs4_web_scraper/__init__.py` & `bs4_web_scraper-0.0.2a0/bs4_web_scraper/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 __date__ = ''
 __author__ = 'ti-oluwa'
 __doc__ = 'A web scraper that uses BeautifulSoup4 to scrape web pages and can translate them to other languages.'
 __license__ = 'MIT'
 __title__ = 'bs4_web_scraper'
 __url__ = 'https://github.com/ti-oluwa/bs4_web_scraper'
 __description__ = 'A web scraper that uses BeautifulSoup4 to scrape web pages and can translates them to other languages.'
@@ -54,14 +54,17 @@
 
 credentials_template = {
     'auth_url': '<Login URL>',
     'auth_username_field': '<Username Field>',
     'auth_password_field': '<Password Field>',
     'auth_username': '<Username>',
     'auth_password': '<Password>',
+    'additional_auth_fields': {
+        '<Field Name>': '<Field Value>',
+    },
 }
 
 
 # NOTE: 
 # 'rra' means 'resource-related-attribute'
 # A 'resource-related-attribute' in this case refers to any HTML tag attribute that points to a resource. Examples of
 # resource-related-attributes include; 'href'(of the <link> tag) and 'src'(of the <img> tag).
```

### Comparing `bs4_web_scraper-0.0.1a0/bs4_web_scraper/base.py` & `bs4_web_scraper-0.0.2a0/bs4_web_scraper/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from . import translate
 from .logging import Logger
 from .exceptions import (InvalidURLError, UnsupportedLanguageError, FileError, InvalidScrapableTagError)
 from .request_limiter import RequestLimitSetting
 from .file_handler import FileHandler
 
 
-# SCRAPE SITES WITH PAGINATION
 class BS4BaseScraper:
     """
     #### Base web scraper class
 
     Avoid instantiating this class directly. Instead, create a subclass of this class and override the `scrape` method.
 
     #### Creating a subclass::
@@ -74,24 +73,15 @@
 
     @param str `log_filepath`: Name or path (relative or absolute) of the file logs will be written into. Defaults to '<self.__class__.__name__.lower()>.log'.
     This can also be a path to an already existing log file. It is independent of self.base_storage_dir(can be saved somewhere outside the base directory)
 
     For instance:
     >>> bs4_scraper = BS4WebScraper(..., log_filepath="/<directory_path>/<filename>/")
 
-    @param str `translation_engine`: The translation engine to use for translation. Case sensitive. Defaults to 'google'. This can be any of the supported translation engines.
-    If the translation engine is not supported, the default translation engine will be used. See `translators` package for more information or do:
 
-    To use a different translation engine, do:
-    >>> bs4_scraper = BS4WebScraper(..., translation_engine='bing')
-
-    #### Supported translation engines:
-    To get a list of the supported translation engines do:
-    >>> print(bs4_web_scraper.translation_engines)
-    
     #### Attributes:
     @attr str `base_url`: The base url of the website being scraped. The base url is the url that will be used to construct the absolute url of all relative urls in a website.
 
     @attr int `level_reached`: The depth or number of levels successfully scraped.
 
     @attr int `_max_no_of_threads`: Maximum number of threads to use for scraping. Defaults to 10.
 
@@ -123,15 +113,15 @@
     _auth_credentials: Dict[str, str] = None
     _is_authenticated: bool = False
     _level_reached: int = 0
     _max_no_of_threads: int = 10
     _session: requests.Session = requests.Session()
     _request_user_agent: str = None
     url_query_params: Dict = {}
-    translator: translate.Translator = translate.Translator()
+    translator: translate.Translator = None
     translate_to: str | None = None
     logger: Logger = None
     _scrapable_tags = (
         'script', 'link|{"rel": "stylesheet"}', 'img', 'use', 'audio',
         'video', 'link|{"as": "font"}', 'link|{"rel": "shortcut"}', 'link|{"rel": "icon"}',
         'link|{"rel": "shortcut icon"}', 'link|{"rel": "apple-touch-icon"}',
         'link|{"type": "image/x-icon"}', 'link|{"type": "image/png"}',
@@ -140,34 +130,28 @@
         'meta|{"content": "og:image"}',
     )
     _tc_: List = []
 
     def __init__(self, parser: str = 'lxml', markup_filename: str = "index.html", 
                 no_of_requests_before_pause: int = 20, scrape_session_pause_duration: int | float | Any = "auto",
                 max_no_of_retries: int = 3, base_storage_dir: str = '.', storage_path: str = '', 
-                log_filepath: str | None = None, translation_engine: str | None = 'default') -> None:
+                log_filepath: str | None = None) -> None:
         """
         Initializes the web scraper instance.
         """
         if not markup_filename.split('.')[-1] in ['xhtml', 'htm', 'shtml', 'html', 'xml']:
             raise FileError('Unsupported filename for `markup_filename`')
         if scrape_session_pause_duration == 'auto':
             scrape_session_pause_duration = max(math.ceil(0.542 * no_of_requests_before_pause), 5)
-        if translation_engine and (translation_engine != 'default' 
-                                    and translation_engine not in translate.translation_engines):
-            raise UnsupportedLanguageError("Unsupported translation engine")
 
         if log_filepath:
             self.logger = Logger(name=f"Logger for {self.__class__.__name__}", log_filepath=log_filepath)
             self.logger.set_base_level('INFO')
             self.logger.to_console = True
 
-        if translation_engine != "default":
-            self.translator.translation_engine = translation_engine
-        self.translator.logger = self.logger
         self.parser = parser
         self.markup_filename = markup_filename
         self.max_no_of_retries = max_no_of_retries
         self.base_storage_dir = os.path.abspath(base_storage_dir)
         self.storage_path = storage_path
         self.request_limit_setting = RequestLimitSetting(
                                                         no_of_requests_before_pause, 
@@ -262,23 +246,26 @@
         Returns the authentication URL.
 
         Args:
             credentials (dict): A dictionary containing the authentication credentials.
         '''
         req_cr = (
             'auth_username_field', 'auth_password_field',
-            'auth_username', 'auth_password', 'auth_url'
+            'auth_username', 'auth_password', 'auth_url',
+            'additional_auth_fields',
         )
         for cr in req_cr:
-            if not credentials.get(cr, None):
+            if not credentials.get(cr, None) and cr != 'additional_auth_fields':
                 raise KeyError(f"`{cr}` not found in `credentials`")
 
         for key, value in credentials.items():
-            if not isinstance(value, str):
+            if key != 'additional_auth_fields' and not isinstance(value, str):
                 raise TypeError(f'Invalid type for `{key}`. `{key}` should be of type str')
+            if key == 'additional_auth_fields' and not isinstance(value, dict):
+                raise TypeError(f'Invalid type for `{key}`. `{key}` should be of type dict')
 
         auth_url_obj = parse_url(credentials.get("auth_url"))
         if not (auth_url_obj.host and auth_url_obj.scheme):
             raise InvalidURLError("`auth_url` is not a valid URL")
      
         if parse_url(self.base_url).host not in auth_url_obj.host:
             raise InvalidURLError("`auth_url` might be invalid as it is not related to `self.base_url`. Please re-check credentials.")
@@ -288,21 +275,26 @@
     def set_auth_credentials(self, credentials: Dict[str, str]) -> None:
         '''
         Sets the instance's request authentication related attributes from user provided credentials.
         
         Args:
             credentials (Dict[str, str]): Authentication credentials
         '''
+        self.set_base_url(credentials['auth_url'])
+        self._auth_url = self._validate_auth_credentials(credentials)
+
         if not self.base_url:
             raise AttributeError("`self.base_url` must be set.")
 
-        self._auth_url = self._validate_auth_credentials(credentials)
         _credentials = {}
         _credentials[credentials['auth_username_field']] = credentials['auth_username']
         _credentials[credentials['auth_password_field']] = credentials['auth_password']
+        if credentials.get('additional_auth_fields', None):
+            for key, value in credentials['additional_auth_fields'].items():
+                _credentials[key] = value
         self._auth_credentials = _credentials
         return None
 
 
     def _get_suitable_no_threads(self, item_count: int) -> int:
         '''
         Calculates the number of threads to use for the current scraping session based on the 
@@ -349,24 +341,47 @@
         """
         response = self.get(url)
         if response:
             return self.make_soup(response.content, **kwargs)
         return None
 
 
-    def _scrape(self, url: str, scrape_depth: int = 1, credentials: Dict[str, str] | None = None, translate_to: str | None = None) -> None:
+    def set_translator(self, translation_engine: str = "default") -> None:
+        """
+        Sets the translator to use for translation.
+
+        Args:
+            translation_engine (str): The translation engine to use. 
+        """
+        if translation_engine and (translation_engine != 'default' 
+                                    and translation_engine not in translate.translation_engines):
+                raise UnsupportedLanguageError("Unsupported translation engine")
+
+        self.translator = translate.Translator()
+        if translation_engine != "default":
+            self.translator.translation_engine = translation_engine
+        self.translator.logger = self.logger
+        return None
+
+
+    def _scrape(self, url: str, scrape_depth: int = 0, credentials: Dict[str, str] | None = None, 
+                translate_to: str | None = None, translation_engine: str = "default"):
         '''
         Main scraping method.
         
         NOTE:
         * This method is not meant to be called directly. Use the `scrape` method instead.
         * This method is not thread safe. It is not meant to be called by multiple threads.
         '''
         if translate_to:
+            if not self.translator:
+                self.set_translator(translation_engine)
+            self.log(f"TRANSLATION ENGINE: {self.translator.translation_engine.upper()}\n")
             self.translate_to = translate_to
+
         if self.level_reached == 0:
             self._base_url = self.get_base_url(url)
         if credentials:
             self.set_auth_credentials(credentials)   
 
         # Scraping 'n' levels (for n >= 0)
         # Initially, Scrape base level -> 'n = 0'
@@ -404,15 +419,15 @@
                     soup = self.make_soup(markup_file_hdl.file)
                     self.storage_path = markup_file_hdl.filepath
                     self.markup_filename = markup_file_hdl.filename
             continue
         return None
 
 
-    def scrape(self, url: str, scrape_depth: int = 1, credentials: Dict[str, str] | None=None, translate_to: str = None) -> None:
+    def scrape(self, url: str, scrape_depth: int = 0, credentials: Dict[str, str] | None=None, translate_to: str = None) -> None:
         """
         #### Wrapper function for the private `_scrape` function of the class.
 
         Scrapes the website provided in the url argument. 
         The scraped content is saved to the `self.storage_path` directory.
 
         Args::
@@ -463,18 +478,19 @@
         '''
         if not credentials and not (self.auth_credentials or self.auth_url):
             raise Exception('`credentials` must be provided if `self.auth_credentials` or `self.auth_url` have not been set.')
         if credentials:
             self.set_auth_credentials(credentials)
 
         self.log(f'AUTHENTICATING AT... --> {self.auth_url}\n')
-        resp = self.session.get(url=self.auth_url) 
+        headers = self.get_request_headers()
+        resp = self.session.get(url=self.auth_url, headers=headers)
         # get and set csrftoken
         self._auth_credentials['csrfmiddlewaretoken'] = resp.cookies.get('csrftoken')
-        resp = self.session.post(url=self.auth_url, data=self.auth_credentials)
+        resp = self.session.post(url=self.auth_url, data=self.auth_credentials, headers=headers)
         self._is_authenticated = resp.ok
 
         if self.is_authenticated:
             self.log('AUTHENTICATED!!!\n')
         else:
             self.log('AUTHENTICATION FAILED!!!\n', level='ERROR')
 
@@ -620,25 +636,26 @@
         if tag_name in ['audio', 'iframe', 'track', 'img', 'source', 'script', 'embed', 'video']:
             src = 'src'
         if tag_name in ['link', 'a', 'use']:
             src = 'href'
         return src
         
 
-    def download_url(self, url: str, save_as: str | None = None, save_to: str | None = None, 
+    def download_url(self, url: str, save_as: str | None = None, save_to: str | None = None, overwrite: bool = False,
                         check_ext: bool = True, unique_if_query_params: bool = False):
         '''
         Download file from the given url. Saves the file in a storage path in `self.base_storage_dir`.
 
         Returns the FileHandler object for the downloaded file if downloaded or already existing else None.
 
         Args::
         * url (str): Url to be downloaded.
         * save_as Optional[str]: Name of the file to be downloaded or name with which the file should be saved.
         * save_to Optional[str]: Path to the directory where the file should be saved in `self.base_storage_dir`.
+        * overwrite (bool, optional): Whether to overwrite the file if it already exists. Defaults to False.
         * check_ext (bool, optional): Whether to check for extension in the url and use it for filename validation. Defaults to True.
         * unique_if_query_params (bool, optional): Whether to add a unique string to the filename if the url has query parameters. Defaults to False.
         
         #### NOTE::
         * If `save_as` is not provided, the filename will be extracted from the url.
         * If `save_to` is not provided, then `save_to` will automatically be the url path.
         * If the url you want to download from does not have an filename with extension, you should set `check_ext` to False and provide a value for `save_as`.
@@ -649,19 +666,19 @@
 
         * If the url already has a filename with extension, but you want to save the file with a different name, you can provide a value for `save_as` and set `check_ext` to False. 
             Just be careful as this may lead to saving files with no or incorrect file extensions.
 
         Example Usage::
             >>> bs4_scraper.download_url(url="https://example.com/", save_as="example.html", save_to="/examples", check_ext="False")
         '''
-        url_obj = parse_url(url)
+        url_obj = parse_url(url.removesuffix('/'))
         if not url_obj.netloc:
             raise InvalidURLError
     
-        url_based_name, url_based_ext = os.path.splitext((url_obj.path or '').split('/')[-1])
+        url_based_name, url_based_ext = os.path.splitext((url_obj.path or '').removesuffix('/').split('/')[-1])
         if check_ext and not url_based_ext:
             raise ValueError('Invalid url. No extension found in url. The url may be incorrect.')
         filename = f"{url_based_name}{url_based_ext}"
 
         if save_as:
             if not isinstance(save_as, str):
                 raise TypeError('`save_as` should be of type str')
@@ -671,49 +688,47 @@
             if check_ext and save_as_ext != url_based_ext:
                 raise ValueError('Invalid extension! `save_as` extension does not match the extension in the url.')
             filename = f"{save_as_name}{save_as_ext}"
 
         if not filename:
             raise ValueError('`filename` seems to be empty. Please check the url "%s" or provide a `save_as` name.' % url)
 
-        has_query_params = False
         response = None
         file_storage_path = save_to.replace('/', '\\').strip() if save_to is not None else save_to
         # check if element src has query params
-        if url_obj.query:
-            has_query_params = True
+        has_query_params = bool(url_obj.query)
         if file_storage_path is None:
             file_storage_path = self.parse_storage_path_from_Url(url_obj, remove_str=f"{url_based_name}{url_based_ext}")
             # Clean up storage path
-            file_storage_path = file_storage_path.replace(filename, '') if file_storage_path.endswith(f"{url_based_name}{url_based_ext}") else file_storage_path
-            file_storage_path = file_storage_path[:-1] if file_storage_path.endswith('\\') else file_storage_path
-            file_storage_path = file_storage_path[1:] if file_storage_path.startswith('\\') else file_storage_path        
+            file_storage_path = file_storage_path.removeprefix('\\').removesuffix('\\')        
                 
         if has_query_params and (url_obj.query not in self.url_query_params.keys()):
             if unique_if_query_params is True:
                 filename = utils.generate_unique_filename(filename)
                 
         if has_query_params and (url_obj.query in self.url_query_params.keys()):
             file_hdl: FileHandler = self.url_query_params[url_obj.query]
             return file_hdl
             
-
         if not has_query_params or (url_obj.query not in self.url_query_params.keys()):
             # check if file already exists
             if os.path.exists(f'{self.base_storage_dir}\{file_storage_path}\{filename}') is False:
-                response = self.get(url)
+                response = self.get(url_obj.url)
             else:
-                return FileHandler(f'{self.base_storage_dir}\{file_storage_path}\{filename}', exists_ok=True, allow_any=True)
+                file_hdl = FileHandler(f'{self.base_storage_dir}\{file_storage_path}\{filename}', exists_ok=True, allow_any=True)
+                if overwrite is True:
+                    file_hdl.delete_file()
+                    response = self.get(url_obj.url)
+                else:
+                    return file_hdl
 
         if response:
             downloaded_file_hdl = self.save_to_file(filename=filename, storage_path=file_storage_path, content=response.content)
-            if downloaded_file_hdl:
-                if has_query_params:
-                    self.url_query_params[url_obj.query] = downloaded_file_hdl 
-
+            if downloaded_file_hdl and has_query_params:
+                self.url_query_params[url_obj.query] = downloaded_file_hdl 
             return downloaded_file_hdl
         return None
 
 
     def get_associated_files_and_return_soup(self, markup_file_handler: FileHandler):
         '''
         Scrapes all the soup tags present in `self._scrapable_tags`. The method simply get all the files associated to a markup
@@ -742,29 +757,33 @@
                     tag_name = parts[0]
                     attrs = json.loads(parts[1])
                     tags.extend(soup.find_all(tag_name, attrs=attrs))
 
             except Exception:
                 raise InvalidScrapableTagError(f"Invalid scrapable_tag, `{scrapable_tag}`, found in `self._scrapable_tags`")
 
-        for tag in tags:
-            rra_file_hdl = self.get_tag_rra(tag, download=True)
-            # change the element's src to be compatible with the scraped website
-            if isinstance(rra_file_hdl, FileHandler):
-                # Find the relative path starting from the directory of the file from which the tag was gotten to the directory of the downloaded file
-                src = self.get_rra_by_tag_name(tag.name)
-                start_path = os.path.dirname(markup_file_handler.filepath) if markup_file_handler.filepath else f'{self.base_storage_dir}\\{self.storage_path}'
-                dest_path = rra_file_hdl.filepath
-                s_p = os.path.relpath(dest_path, start=start_path)
-                s_p = s_p.replace('\\', '/')
-                tag[src] = s_p if s_p.startswith('.') else f'./{s_p}'
-            continue
+        with ThreadPoolExecutor() as executor:
+            _ = executor.map(lambda tag: self._get_tag_rra(tag, markup_file_handler), tags)
         return soup
 
 
+    def _get_tag_rra(self, tag: Tag, markup_file_handler: FileHandler):
+        rra_file_hdl = self.get_tag_rra(tag, download=True)
+        # change the element's src to be compatible with the scraped website
+        if isinstance(rra_file_hdl, FileHandler):
+            # Find the relative path starting from the directory of the file from which the tag was gotten to the directory of the downloaded file
+            src = self.get_rra_by_tag_name(tag.name)
+            start_path = os.path.dirname(markup_file_handler.filepath) if markup_file_handler.filepath else f'{self.base_storage_dir}\\{self.storage_path}'
+            dest_path = rra_file_hdl.filepath
+            s_p = os.path.relpath(dest_path, start=start_path)
+            s_p = s_p.replace('\\', '/')
+            tag[src] = s_p if s_p.startswith('.') else f'./{s_p}'
+        return None
+
+
     def get_actual_url_from_rra(self, rra: str):
         '''
         Parses the url from a bs4.element.Tag rra
 
         Args::
         * `rra` (str): bs4.element.Tag resource-related-attribute
         '''
```

### Comparing `bs4_web_scraper-0.0.1a0/bs4_web_scraper/exceptions.py` & `bs4_web_scraper-0.0.2a0/bs4_web_scraper/exceptions.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.0.1a0/bs4_web_scraper/file_handler.py` & `bs4_web_scraper-0.0.2a0/bs4_web_scraper/file_handler.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.0.1a0/bs4_web_scraper/logging.py` & `bs4_web_scraper-0.0.2a0/bs4_web_scraper/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,18 @@
     def __str__(self) -> str:
         if self._logger.name:
             return self._logger.name
         return super().__str__()
     
     def __setattr__(self, __name: str, __value: Any) -> None:
         super().__setattr__(__name, __value)
-        self.__update_config()
+        self._update_config()
 
     
-    def __to_console(self) -> None:
+    def _to_console(self) -> None:
         '''
         Logs messages to the console.
 
         If `self.to_console` is True, all subsequent log messages will be logged to the console.
         '''
         # set up logging to console
         console = logging.StreamHandler()
@@ -73,22 +73,22 @@
         # add the handler to the logger object and remove any existing handlers
         handlers = self._logger.handlers
         for h in handlers:
             self._logger.removeHandler(h)
         self._logger.addHandler(console)
 
 
-    def __update_config(self) -> None:
+    def _update_config(self) -> None:
         '''Updates the logger's configuration.'''
         logging.basicConfig(filename=self.filename, level=self._base_level, 
                             format=self._format, datefmt=self.date_format,
                             filemode=self.file_mode, force=True)
         if self.to_console:
             try:
-                self.__to_console()
+                self._to_console()
             except Exception as e:
                 self.log_error(e)
         return None
 
 
     def set_base_level(self, level: str) -> None:
         '''
```

### Comparing `bs4_web_scraper-0.0.1a0/bs4_web_scraper/request_limiter.py` & `bs4_web_scraper-0.0.2a0/bs4_web_scraper/request_limiter.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.0.1a0/bs4_web_scraper/scraper.py` & `bs4_web_scraper-0.0.2a0/bs4_web_scraper/scraper.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,37 +119,47 @@
     @attr Logger `logger`: `Logger` object for creating and writing logs.
 
     @attr str `_request_user_agent`: 'User-Agent' header used in requests.
 
     """
 
     
-    def scrape(self, url: str, scrape_depth: int = 1, credentials: Dict[str, str] | None=None, translate_to: str = None) -> None:
+    def scrape(self, url: str, scrape_depth: int = 0, credentials: Dict[str, str] | None=None, 
+                translate_to: str = None, translation_engine: str = "default") -> None:
         """
         #### Wrapper function for the private `_scrape` function of the class.
 
         Scrapes the website provided in the url argument. 
         The scraped content is saved to the `self.storage_path` directory.
 
         Args: ::
             url (str): The url of the website or webpage to be scraped.
             scrape_depth (int, optional): The number of levels deep to scrape. Defaults to 1.
             credentials (Dict[str, str], optional): Authentication or login details for website. Defaults to None.
             translate_to (str, optional): Language code for the language scraped content will be translated to. The source language
             is automatically detected by `self.translator`. Defaults to None.
+            translation_engine (str, optional): The translation engine to use for translation. Case sensitive. Defaults to 'default'. This can be any of the supported translation engines.
+            See `translators` package for more information or do:
 
+        #### Supported translation engines:
+        To get a list of the supported translation engines do:
+        >>> print(bs4_web_scraper.translation_engines)
+        
         #### AUTHENTICATION
         To scrape websites that require authentication. pass in the authentication credentials as an argument to the function.
         #### NOTE: credentials should take the format
         >>> credentials = {
             'auth_url': '<authentication_url>',
             'auth_username_field': '<username_field_name>',
             'auth_password_field': '<password_field_name>',
             'auth_username': '<username>',
             'auth_password': '<password>',
+            'additional_auth_fields': {
+                '<Field Name>': '<Field Value>',
+            },
         }
         bs4_scraper = BS4WebScraper(...)
         bs4_scraper.scrape(..., credentials=credentials)
 
 
         #### TRANSLATION
         To translate scraped content to a specific language, the `translate_to` argument has to be provided. 
@@ -167,19 +177,18 @@
         #### NOTE: The `translate_to` argument is case insensitive.
 
         #
         """
         self.log("STARTING SCRAPING ACTIVITY...\n")
         self.log(f"SCRAPING DEPTH: {scrape_depth if scrape_depth > 0 else 'BASE LEVEL'}\n")
         if translate_to:
-            self.log(f"TRANSLATION ENGINE: {self.translator.translation_engine.upper()}\n")
             self.log(f"TRANSLATING TO: {translate_to.upper()}\n")
 
         start_time = time.perf_counter()
-        super()._scrape(url, scrape_depth, credentials, translate_to)
+        super()._scrape(url, scrape_depth, credentials, translate_to, translation_engine)
         finish_time = time.perf_counter()
         time_taken = finish_time - start_time
 
         if self._level_reached > 0:
             self.log(f"SCRAPED {self._level_reached} LEVEL{'S'[:self._level_reached^1]} SUCCESSFULLY! \n")
         else:
             self.log("SCRAPED BASE LEVEL SUCCESSFULLY! \n")
@@ -188,24 +197,25 @@
             self.log(f"SCRAPING COMPLETED IN {(time_taken / 60):.2f} MINUTE{'S'[:round(time_taken / 60)^1]}\n")
         else:
             self.log(f"SCRAPING COMPLETED IN {time_taken:.2f} SECOND{'S'[:round(time_taken)^1]}\n")
 
         return None
 
     
-    def download_urls(self, urls: Iterable[Dict[str, str]], save_to: str | None = None, 
+    def download_urls(self, urls: Iterable[Dict[str, str]], save_to: str | None = None, overwrite: bool = False,
                         check_ext: bool = True, fast_download: bool = False, unique_if_query_params: bool = False):
         '''
         Download files from the given urls using the `download_url` method. Saves the files in a storage path in `self.base_storage_dir`.
 
         Returns the storage path of the downloaded files.
 
         Args:
             - urls (List[Dict[str, str]]): List of urls to be downloaded. The url in the list should be of type dict[str, str].
             - save_to Optional[str]: Path to the directory where the file should be saved in `self.base_storage_dir`.
+            - overwrite (bool, optional): Whether to overwrite existing files. Defaults to False.
             - check_ext (bool, optional): Whether to check for extension in the url and use it for filename validation. Defaults to True.
             Check the doc string of `download_url` for more info on setting this value.
             - unique_if_query_params (bool, optional): Whether to generate a unique filename if the any of the urls has query params. Defaults to False.
             - fast_download (bool, optional): Whether to download the urls in parallel. Defaults to False. 
             If the number or urls exceed 200 then fast download wont be used to avoid sending high frequency requests to the server.
 
         #### Example Usage: ::
@@ -219,15 +229,18 @@
 
         urls = list(filter(lambda url: isinstance(url, dict) and any(url), urls))
 
         if len(urls) < 1:
             raise ValueError("No valid url was found in `urls`")
 
         results = []
-        params = {'save_to': save_to, 'check_ext': check_ext, 'unique_if_query_params': unique_if_query_params}
+        params = {
+            'save_to': save_to, 'overwrite': overwrite, 
+            'check_ext': check_ext, 'unique_if_query_params': unique_if_query_params
+        }
         urls_download_params = map(lambda dict: {**params, **dict}, urls)
 
         if fast_download and len(urls) <= 200:
             self.log("FAST DOWNLOAD STARTED...\n")
             with ThreadPoolExecutor() as executor:
                 values = executor.map(lambda kwargs: self.download_url(**kwargs), urls_download_params)
             results.extend(values)
@@ -241,39 +254,39 @@
         if results:
             self.log("DOWNLOADS FINISHED!\n")
         else:
             self.log("NOTHING DOWNLOADED!\n")
         return results
 
 
-    def save_results(self, result: Iterable[str], path: str, **kwargs):
+    def save_results(self, result: Iterable[str], file_path: str, **kwargs):
         '''
-        Saves a list of results to the file in the given path inside the base storage directory
+        Saves a list of results to the file in the given file inside the base storage directory(if path is not an absolute path)
 
         Args::
             * result (Iterable[str]): An iterable containing strings to be saved.
-            * path (str): path to directory where the file containing `result` will be saved in the base storage directory.
+            * file_path (str): path to directory where the file containing `result` will be saved in the base storage directory.
             If it is an absolute path, the file will be saved in the specified path.
             * **kwargs (Dict | optional): optional parameters to be used when necessary
                     * `csv_head` (str): heading for csv file type
         '''
-        path = os.path.join(self.base_storage_dir, path)
+        path = os.path.join(self.base_storage_dir, file_path)
         file_handler = FileHandler(path)  
         if file_handler.filetype == 'csv':
             csv_head = kwargs.get('csv_head', "results").upper()
             url_lists = utils.slice_iterable(result, 1)
             detailed_url_list = [('S/N', csv_head)]
             detailed_url_list.extend([ (c + 1, url_lists[c][0]) for c in range(len(url_lists)) ])
             return file_handler.write_to_file(detailed_url_list)
         for r in result: 
             file_handler.write_to_file(f'{r}\n') 
         return None
 
 
-    def find_all(self, url: str, target: str, attrs: Dict[str, str] | Iterable[Dict[str, str]] = {}, 
+    def find_urls(self, url: str, target: str, attrs: Dict[str, str] | Iterable[Dict[str, str]] = {}, 
                         depth: int = 0, count: int = None, recursive: bool = True):
         """
         Parses out the url/links on all elements with the target name in specified url.
         NOTE: This only works for elements with a resource(url) related attribute. To get markup elements with no resource related attribute, use `find_all_tags`.
 
         Removes duplicates and returns a list of the links/urls.
 
@@ -308,15 +321,15 @@
                 link_tags = soup.find_all('a', recursive=recursive)
                 links = [ self.get_link_tag(link_tag, download=False) for link_tag in link_tags ]
                 links = filter(lambda link: bool(link), links)   
                 link_objs = [ (link, parse_url(link)) for link in links ]
                 links = [ link_obj[0] for link_obj in link_objs if (base_url_obj.netloc and link_obj[1].netloc) and (base_url_obj.netloc in link_obj[1].netloc) ] 
 
                 with ThreadPoolExecutor() as executor:
-                    results = executor.map(lambda args: self.find_all(*args), map(lambda link: (link, target, attrs, depth, count, recursive), links))
+                    results = executor.map(lambda args: self.find_urls(*args), map(lambda link: (link, target, attrs, depth, count, recursive), links))
                     for result in results:
                         if result:
                             urls.extend(result)
                 continue
         urls = list(set(urls))
         return urls
     
@@ -352,15 +365,15 @@
                 link_tags = soup.find_all('a', recursive=recursive)
                 links = [ self.get_link_tag(link_tag, download=False) for link_tag in link_tags ]
                 links = filter(lambda link: bool(link), links)   
                 link_objs = [ (link, parse_url(link)) for link in links ]
                 links = [ link_obj[0] for link_obj in link_objs if (base_url_obj.netloc and link_obj[1].netloc) and (base_url_obj.netloc in link_obj[1].netloc) ] 
 
                 with ThreadPoolExecutor() as executor:
-                    results = executor.map(lambda args: self.find_all_tags(*args), map(lambda link: (link, target, attrs, depth, count, recursive), links))
+                    results = executor.map(lambda args: self.find_urls_tags(*args), map(lambda link: (link, target, attrs, depth, count, recursive), links))
                     for result in results:
                         if result:
                             tags.extend(result)
                 continue
         return tags
 
     
@@ -376,15 +389,15 @@
             * save_to_file (bool, optional): Whether to save the links to a file. Defaults to False.
             * file_path (str, optional): File to save the links to. Defaults to "self.base_storage_dir/links.txt".
             If it is an absolute path, the file will be saved in the specified path.
             Available file formats are: csv, txt, doc, docx, pdf...
             * **kwargs (Dict | optional): optional parameters to be used for 
                     * `csv_head` (str): saving results and is passed to the `save_results` function if `save_to_file` is True.
         """
-        result = self.find_all(url, target='a', depth=depth)
+        result = self.find_urls(url, target='a', depth=depth)
         if result and save_to_file is True:
             kwargs['csv_head'] = kwargs.get('csv_head', 'Links')
             self.save_results(result, file_path, **kwargs)
         return result
 
 
     def find_stylesheets(self, url: str, depth: int = 0, save_to_file: bool = False, file_path: str = "styles.csv", **kwargs) -> List[str]:
@@ -403,15 +416,15 @@
             * **kwargs (Dict | optional): optional parameters to be used for 
                     * `csv_head` (str): saving results and is passed to the `save_results` function if `save_to_file` is True.
         """
         attrs = (
             {'rel': 'stylesheet'},
             {'type': 'text/css'}
         )
-        result = self.find_all(url, target='link', attrs=attrs, depth=depth)
+        result = self.find_urls(url, target='link', attrs=attrs, depth=depth)
         if result and save_to_file is True:
             kwargs['csv_head'] = kwargs.get('csv_head', 'Stylesheets')
             self.save_results(result, file_path, **kwargs)
         return result
             
 
     def find_scripts(self, url: str, depth: int = 0, save_to_file: bool = False, file_path: str = "scripts.csv", **kwargs) -> List[str]:
@@ -426,15 +439,15 @@
             * `save_to_file` (bool, optional): Whether to save the scripts to a file. Defaults to False.
             * `file_path` (str, optional): File to save the links to. Defaults to "self.base_storage_dir/scripts.txt".
             If it is an absolute path, the file will be saved in the specified path.
             Available file formats include: csv, txt, doc, docx, pdf...
             * `**kwargs` (Dict | optional): optional parameters to be used for 
                     * `csv_head` (str): saving results and is passed to the `save_results` function if `save_to_file` is True.
         """
-        result = self.find_all(url, target='script', depth=depth)
+        result = self.find_urls(url, target='script', depth=depth)
         if result and save_to_file is True:
             kwargs['csv_head'] = kwargs.get('csv_head', 'Scripts')
             self.save_results(result, file_path, **kwargs)
         return result
 
     
     def find_fonts(self, url: str, depth: int = 0, save_to_file: bool = False, file_path: str = "fonts.csv", **kwargs) -> List[str]:
@@ -453,15 +466,15 @@
             * **kwargs (Dict | optional): optional parameters to be used for 
                     * `csv_head` (str): saving results and is passed to the `save_results` function if `save_to_file` is True.
         """
         attrs = (
             {'rel': 'preload'},
             {'as': 'font'}
         )
-        result = self.find_all(url, target='link', attrs=attrs, depth=depth)
+        result = self.find_urls(url, target='link', attrs=attrs, depth=depth)
         if result and save_to_file is True:
             kwargs['csv_head'] = kwargs.get('csv_head', 'Font Links')
             self.save_results(result, file_path, **kwargs)
         return result
 
     
     def find_images(self, url: str, depth: int = 0, save_to_file: bool = False, file_path: str = "images.csv", **kwargs) -> List[str]:
@@ -476,15 +489,15 @@
             * save_to_file (bool, optional): Whether to save the images to a file. Defaults to False.
             * file_path (str, optional): File to save the links to. Defaults to "self.base_storage_dir/images.txt".
             If it is an absolute path, the file will be saved in the specified path.
             Available file formats include: csv, txt, doc, docx, pdf...
             * **kwargs (Dict | optional): optional parameters to be used for 
                     * `csv_head` (str): saving results and is passed to the `save_results` function if `save_to_file` is True.
         """
-        result = self.find_all(url, target='img', depth=depth)
+        result = self.find_urls(url, target='img', depth=depth)
         if result and save_to_file is True:
             kwargs['csv_head'] = kwargs.get('csv_head', 'Image Links')
             self.save_results(result, file_path, **kwargs)
         return result
 
 
     def find_videos(self, url: str, depth: int = 0, save_to_file: bool = False, file_path: str = "videos.csv", **kwargs) -> List[str]:
@@ -501,15 +514,15 @@
             If it is an absolute path, the file will be saved in the specified path.
             Available file formats include: csv, txt, doc, docx, pdf...
             * **kwargs (Dict | optional): optional parameters to be used when and where necessary
                     * `csv_head` (str): saving results and is passed to the `save_results` function if `save_to_file` is True.
         """
         video_types = ('video/mp4', 'video/mpeg', 'video/ogg', 'video/webm', 'video/3gpp', 'video/quicktime')
         v_list = [ {'type': v} for v in video_types ]
-        result = self.find_all(url, target='source', attrs=v_list, depth=depth)
+        result = self.find_urls(url, target='source', attrs=v_list, depth=depth)
         if result and save_to_file is True:
             kwargs['csv_head'] = kwargs.get('csv_head', 'Video Links')
             self.save_results(result, file_path, **kwargs)
         return result
 
 
     def find_audios(self, url: str, depth: int = 0, save_to_file: bool = False, file_path: str = "audios.csv", **kwargs) -> List[str]:
@@ -526,22 +539,22 @@
             If it is an absolute path, the file will be saved in the specified path.
             Available file formats include: csv, txt, doc, docx, pdf...
             * **kwargs (Dict | optional): optional parameters to be used for 
                     * `csv_head` (str): saving results and is passed to the `save_results` function if `save_to_file` is True.
         '''
         audio_types = ('audio/mpeg', 'audio/mp3', 'audio/ogg', 'audio/wav', 'audio/aac', 'audio/flac', 'audio/m4a', 'audio/wma')
         a_list = [ {'type': a} for a in audio_types ]
-        result = self.find_all(url, target='source', attrs=a_list, depth=depth)
+        result = self.find_urls(url, target='source', attrs=a_list, depth=depth)
         if result and save_to_file is True:
             kwargs['csv_head'] = kwargs.get('csv_head', 'Audio Links')
             self.save_results(result, file_path, **kwargs)
         return result
         
 
-    def get_emails(self, url: str, depth: int = 0, save_to_file: bool = False, file_path: str = "emails.csv", **kwargs) -> List[str]:
+    def find_emails(self, url: str, depth: int = 0, save_to_file: bool = False, file_path: str = "emails.csv", **kwargs) -> List[str]:
         """
         Searches for and returns a list of emails found in the given url.
 
         Args:
             * url (str): Url to get the emails from.
             * depth (int, optional): Number of levels to recursively search for emails. Defaults to 0.
             * save_to_file (bool, optional): Whether to save the emails to a file. Defaults to False.
```

### Comparing `bs4_web_scraper-0.0.1a0/bs4_web_scraper/translate.py` & `bs4_web_scraper-0.0.2a0/bs4_web_scraper/translate.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         elif self.logger and not isinstance(self.logger, Logger):
             raise TypeError('Invalid type for `self.logger`. `self.logger` should be an instance of bs4_web_scraper.logging.Logger')
         return print(message + '\n') 
     
 
     def lang_is_supported(self, lang_code: str) -> bool:
         '''
-        Check if the specified language code is supported by `self.translator`
+        Check if the specified language code is supported by `self.translation_engine`
         
         Returns True if supported, else False.
 
         Args:
             lang_code (str): The language code to check.
         
         '''
@@ -189,37 +189,39 @@
             element (str): The markup element to be removed from the list of translatable elements.
         '''
         if element in self._translatable_elements:
             return self._translatable_elements.remove(element)
         return None
 
 
-    def translate(self, content: str | bytes, src_lang: str="auto", target_lang: str="en", 
-                  cache: bool=True, markup: bool=False, **kwargs) -> str | bytes:
+    def translate(self, content: str | bytes | BeautifulSoup, src_lang: str="auto", target_lang: str="en", 
+                  cache: bool=True, is_markup: bool=False, **kwargs) -> str | bytes:
         '''
-        Translate `content` from `src_lang` to `target_lang` using `self.translator`.
+        Translate `content` from `src_lang` to `target_lang`.
 
         Returns translated content.
 
         Args:
-            content (str | bytes): Content to be translated
+            content (str | bytes | BeatifulSoup): Content to be translated
             src_lang (str, optional): Source language. Defaults to "auto".
             target_lang (str, optional): Target language. Defaults to "en".
             cache (bool, optional): Whether to cache translations. Defaults to True.
-            markup (bool, optional): Whether `content` is markup. Defaults to False.
+            is_markup (bool, optional): Whether `content` is markup. Defaults to False.
             **kwargs: Keyword arguments to be passed to `self.translate_text` or `self.translate_markup`.
         '''
-        if markup:
+        if is_markup:
             return self.translate_markup(content, src_lang, target_lang, **kwargs)
+        elif isinstance(content, BeautifulSoup):
+            return self.translate_soup(content, src_lang, target_lang, **kwargs)
         return self.translate_text(content, src_lang, target_lang, cache, **kwargs)
         
     
     def translate_text(self, text: str, src_lang: str="auto", target_lang: str="en", cache: bool=True, **kwargs) -> str:
         '''
-        Translate text from `src_lang` to `target_lang` using `self.translator`.
+        Translate text from `src_lang` to `target_lang`.
 
         Returns translated text.
 
         Args::
             text (str): Text to be translated
             src_lang (str, optional): Source language. Defaults to "auto".
             target_lang (str, optional): Target language. Defaults to "en".
@@ -304,15 +306,15 @@
             translated_markup = translated_markup.encode('utf-8')
         return translated_markup
 
 
     # NOT FUNCTIONAL FOR NOW
     # def translate_markup(self, markup: str | bytes, src_lang: str="auto", target_lang: str="en", **kwargs):
     #     '''
-    #     Translates the markup content from `src_lang` to `target_lang` using `self.translator`.
+    #     Translates the markup content from `src_lang` to `target_lang`.
 
     #     ### NOT FUNCTIONAL FOR NOW. CONVERT markup TO BEAUTIFULSOUP OBJECT AND USE THE `translate_soup` METHOD INSTEAD.
 
     #     Returns translated markup.
 
     #     Args:
     #         markup (str | bytes): markup content to be translated
@@ -352,15 +354,15 @@
     #         error_ = TranslationError(f"Error translating markup: {e}") 
     #         self._log(f"{error_}", level='error')
     #         return markup
 
 
     def translate_file(self, filepath: str, src_lang: str="auto", target_lang: str="en", **kwargs):
         '''
-        Translates file from `src_lang` to `target_lang` using `self.translator`.
+        Translates file from `src_lang` to `target_lang`.
 
         Returns translated file's FileHandler`.
 
         Supported file types include: .txt, .csv, .doc, .docx, .pdf, .md..., mostly files with text content.
 
         Args:
             filepath (str): path to the file to be translated.
```

### Comparing `bs4_web_scraper-0.0.1a0/bs4_web_scraper/utils.py` & `bs4_web_scraper-0.0.2a0/bs4_web_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `bs4_web_scraper-0.0.1a0/pyproject.toml` & `bs4_web_scraper-0.0.2a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bs4_web_scraper"
-version = "0.0.1a"
+version = "0.0.2a"
 authors = [
   { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
 ]
 maintainers = [
   { name="ti-oluwa", email="tioluwa.dev@gmail.com" },
 ]
 description = "A web scraper based on the BeautifulSoup4 library and translators package."
```

