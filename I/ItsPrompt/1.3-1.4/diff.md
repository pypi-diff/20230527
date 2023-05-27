# Comparing `tmp/ItsPrompt-1.3.tar.gz` & `tmp/ItsPrompt-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ItsPrompt-1.3.tar", last modified: Sun May 14 14:06:15 2023, max compression
+gzip compressed data, was "ItsPrompt-1.4.tar", last modified: Sat May 27 07:09:38 2023, max compression
```

## Comparing `ItsPrompt-1.3.tar` & `ItsPrompt-1.4.tar`

### file list

```diff
@@ -1,34 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:06:15.027732 ItsPrompt-1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:06:15.023732 ItsPrompt-1.3/ItsPrompt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:06:15.023732 ItsPrompt-1.3/ItsPrompt/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/data/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/data/expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/data/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/data/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/data/table.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/data/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/keyboard_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20522 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:06:15.027732 ItsPrompt-1.3/ItsPrompt/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/prompts/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/prompts/confirm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/prompts/expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/prompts/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/prompts/raw_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/prompts/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-14 14:06:02.000000 ItsPrompt-1.3/ItsPrompt/prompts/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:06:15.023732 ItsPrompt-1.3/ItsPrompt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-05-14 14:06:15.000000 ItsPrompt-1.3/ItsPrompt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-14 14:06:15.000000 ItsPrompt-1.3/ItsPrompt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:06:15.000000 ItsPrompt-1.3/ItsPrompt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-14 14:06:15.000000 ItsPrompt-1.3/ItsPrompt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-14 14:06:15.000000 ItsPrompt-1.3/ItsPrompt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-14 14:06:02.000000 ItsPrompt-1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16861 2023-05-14 14:06:15.027732 ItsPrompt-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15054 2023-05-14 14:06:02.000000 ItsPrompt-1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-14 14:06:02.000000 ItsPrompt-1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 14:06:15.027732 ItsPrompt-1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:06:15.027732 ItsPrompt-1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-05-14 14:06:02.000000 ItsPrompt-1.3/tests/test_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:38.985905 ItsPrompt-1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:38.985905 ItsPrompt-1.4/ItsPrompt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:38.985905 ItsPrompt-1.4/ItsPrompt/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/data/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/data/expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/data/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/data/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/data/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/data/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/keyboard_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:38.985905 ItsPrompt-1.4/ItsPrompt/objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:38.985905 ItsPrompt-1.4/ItsPrompt/objects/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/objects/table/table_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/objects/table/table_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/objects/table/table_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21146 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:38.985905 ItsPrompt-1.4/ItsPrompt/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/prompts/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/prompts/confirm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/prompts/expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/prompts/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/prompts/raw_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/prompts/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-27 07:09:28.000000 ItsPrompt-1.4/ItsPrompt/prompts/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:38.985905 ItsPrompt-1.4/ItsPrompt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-05-27 07:09:38.000000 ItsPrompt-1.4/ItsPrompt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-27 07:09:38.000000 ItsPrompt-1.4/ItsPrompt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 07:09:38.000000 ItsPrompt-1.4/ItsPrompt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-27 07:09:38.000000 ItsPrompt-1.4/ItsPrompt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 07:09:38.000000 ItsPrompt-1.4/ItsPrompt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-27 07:09:28.000000 ItsPrompt-1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-05-27 07:09:38.985905 ItsPrompt-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15456 2023-05-27 07:09:28.000000 ItsPrompt-1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-27 07:09:28.000000 ItsPrompt-1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 07:09:38.985905 ItsPrompt-1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 07:09:38.985905 ItsPrompt-1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-05-27 07:09:28.000000 ItsPrompt-1.4/tests/test_prompt.py
```

### Comparing `ItsPrompt-1.3/ItsPrompt/data/checkbox.py` & `ItsPrompt-1.4/ItsPrompt/data/checkbox.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,40 +4,29 @@
 @dataclass
 class CheckboxOption:
     name: str
     id: str
     is_selected: bool
 
 
-def process_data(
-        options: tuple[str | tuple[str, str], ...]) -> list[CheckboxOption]:
-    '''
+def process_data(options: tuple[str | tuple[str, str], ...]) -> list[CheckboxOption]:
+    """
     Processes the given `options` and returns the processed list
 
     :param options: A list of options to process
     :type options: tuple[str  |  tuple[str, str], ...]
     :raises TypeError: If an option is not processable, a `TypeError` will be raised
     :return: a list of `CheckboxOption`
     :rtype: list[CheckboxOption]
-    '''
+    """
     processed_options: list[CheckboxOption] = []
 
     # process given options
     for option in options:
         if type(option) is str:
-            processed_options.append(
-                CheckboxOption(
-                    name=option,
-                    id=option,
-                    is_selected=False,
-                ))
+            processed_options.append(CheckboxOption(name=option, id=option, is_selected=False))
         elif type(option) is tuple:
-            processed_options.append(
-                CheckboxOption(
-                    name=option[0],
-                    id=option[1],
-                    is_selected=False,
-                ))
+            processed_options.append(CheckboxOption(name=option[0], id=option[1], is_selected=False))
         else:
             raise TypeError('Argument is not processable')
 
     return processed_options
```

### Comparing `ItsPrompt-1.3/ItsPrompt/data/expand.py` & `ItsPrompt-1.4/ItsPrompt/data/expand.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,29 +4,28 @@
 @dataclass
 class ExpandOption:
     key: str
     name: str
     id: str
 
 
-def process_data(
-        options: tuple[str | tuple[str, str, str], ...]) -> list[ExpandOption]:
-    '''
+def process_data(options: tuple[str | tuple[str, str, str], ...]) -> list[ExpandOption]:
+    """
     Processes the given `options` and returns the processed list
 
     :param options: A list of options to process
     :type options: tuple[str  |  tuple[str, str, str], ...]
     :raises ValueError: If the keys are not unique
     :raises ValueError: If the keys are not of length 1
     :raises ValueError: If the keys are not ascii
     :raises ValueError: If the keys are using h
     :raises TypeError: If an option is not processable
     :return: A list of `ExpandOptions`
     :rtype: list[ExpandOption]
-    '''
+    """
     # check if every key is unique, otherwise return error
     keys = [option[0] for option in options]
     if len(set(keys)) < len(keys):
         raise ValueError('Keys must be unique!')
 
     # check that every key string is only one char long
     if any([len(option[0]) > 1 or len(option[0]) < 1 for option in options]):
@@ -42,32 +41,17 @@
 
     processed_options: list[ExpandOption] = []
 
     # process given options
     for option in options:
         if type(option) is str:
             # use first letter as key, and str as name and id
-            processed_options.append(
-                ExpandOption(
-                    key=option[0],
-                    name=option,
-                    id=option,
-                ))
+            processed_options.append(ExpandOption(key=option[0], name=option, id=option))
         elif type(option) is tuple:
-            processed_options.append(
-                ExpandOption(
-                    key=option[0],
-                    name=option[1],
-                    id=option[2],
-                ))
+            processed_options.append(ExpandOption(key=option[0], name=option[1], id=option[2]))
         else:
             raise TypeError('Argument is not processable')
 
     # append a help option
-    processed_options.append(
-        ExpandOption(
-            key='h',
-            name='Help Menu, list or hide all options',
-            id='',
-        ))
+    processed_options.append(ExpandOption(key='h', name='Help Menu, list or hide all options', id=''))
 
     return processed_options
```

### Comparing `ItsPrompt-1.3/ItsPrompt/data/select.py` & `ItsPrompt-1.4/ItsPrompt/data/select.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,37 +3,29 @@
 
 @dataclass
 class SelectOption:
     name: str
     id: str
 
 
-def process_data(
-        options: tuple[str | tuple[str, str], ...]) -> list[SelectOption]:
-    '''
+def process_data(options: tuple[str | tuple[str, str], ...]) -> list[SelectOption]:
+    """
     Processes the given `options` and returns the processed list
 
     :param options: A list of options to process
     :type options: tuple[str  |  tuple[str, str], ...]
     :raises TypeError: If an option is not processable, a `TypeError` will be raised
     :return: a list of `SelectOptions`
     :rtype: list[SelectOption]
-    '''
+    """
     processed_options: list[SelectOption] = []
 
     # process given options
     for option in options:
         if type(option) is str:
-            processed_options.append(SelectOption(
-                name=option,
-                id=option,
-            ))
+            processed_options.append(SelectOption(name=option, id=option))
         elif type(option) is tuple:
-            processed_options.append(
-                SelectOption(
-                    name=option[0],
-                    id=option[1],
-                ))
+            processed_options.append(SelectOption(name=option[0], id=option[1]))
         else:
             raise TypeError('Argument is not processable')
 
     return processed_options
```

### Comparing `ItsPrompt-1.3/ItsPrompt/data/style.py` & `ItsPrompt-1.4/ItsPrompt/data/style.py`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.3/ItsPrompt/data/table.py` & `ItsPrompt-1.4/ItsPrompt/data/table.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,134 +1,140 @@
 import os
+from typing import TYPE_CHECKING, Union
 
-from pandas import DataFrame
+from ..objects.table.table_base import TableDataBase
+from ..objects.table.table_dict import TableDataFromDict
+
+# only import pandas and TableData if pandas is installed
+try:
+    from pandas import DataFrame
+
+    from ..objects.table.table_df import TableDataFromDF
+except ModuleNotFoundError:  # pragma: no cover
+    # pandas were not installed
+    pass
+
+if TYPE_CHECKING:  # pragma: no cover
+    from pandas import DataFrame
 
 
 class Table:
 
-    def __init__(self, data: DataFrame) -> None:
-        '''
+    def __init__(self, data: Union["DataFrame", dict[str, list[str]]]) -> None:
+        """
         Creates a table object for storing the drawable table instance
 
         :param data: the data to display
         :type data: DataFrame
-        '''
+        """
         # change type of all columns to str
         # TODO maybe later support more datatypes
-        self.data = data.astype('string')
+        self.data: TableDataBase
+        if type(data) is dict:
+            self.data = TableDataFromDict(data)
+        elif type(data) is DataFrame:
+            self.data = TableDataFromDF(data)
 
         # save amount of rows
-        self.row_count = len(self.data) + 1
-        self.col_count = len(self.data.columns)
+        self.row_count = self.data.row_count
+        self.col_count = self.data.col_count
 
         # get max cell width
         max_width = os.get_terminal_size().columns
 
         # get width for each cell
-        self.cell_width = (max_width - 1) // len(self.data.columns) - 1
+        self.cell_width = (max_width - 1) // self.col_count - 1
 
         # save current selected cell
         self.cur_cell = [0, 0]  # ignoring header, as this can not be selected
 
     def _col_is_last(self, col) -> bool:
-        '''checks if the given column is the last column in the DataFrame'''
-        return self.data.columns.get_loc(col) == len(self.data.columns) - 1
+        """checks if the given column is the last column in the DataFrame"""
+        return self.data.get_column_location(col) == self.col_count - 1
 
     def _char_if_last_else_otherchar(
         self,
         col,
         char: str,
         otherchar: str,
     ) -> str:
-        '''returns the `char` if the given column is the last in the DataFrame, otherwise returns the `otherchar`'''
+        """returns the `char` if the given column is the last in the DataFrame, otherwise returns the `otherchar`"""
         return char if self._col_is_last(col) else otherchar
 
     def get_table_as_str(self) -> str:
-        '''
+        """
         Returns the table as a printable string
-        
+
         Respects the width of the terminal at time of creation of the table object. Later this may be made dynamic.
-        '''
+        """
 
         # set initial list (each entry represents a line to print)
-        table_out = [''] * (self.row_count * 2 + 1
-                            )  # 2 lines for every row + bottom border
+        table_out = [''] * (self.row_count * 2 + 1)  # 2 lines for every row + bottom border
 
         # append left border to every string
         table_out[0] += '┌'
 
         for i in range(1, len(table_out), 2):
             table_out[i] += '│'
             table_out[i + 1] += '├'
 
         table_out[-1] = '└'
 
         # add headers
         for header in self.data.columns:
-            table_out[
-                0] += '─' * self.cell_width + self._char_if_last_else_otherchar(
-                    header, '┐', '┬')
+            table_out[0] += '─' * self.cell_width + self._char_if_last_else_otherchar(header, '┐', '┬')
 
             if len(str(header)) > self.cell_width:
                 #   /\ convert the header to str in case the user did not give a header, so it is an integer
                 header = header[:self.cell_width - 1] + '.'
 
             table_out[1] += f'{header:^{self.cell_width}}' + '│'
 
         # add values, iterate over each column
         for header, values in self.data.items():
             # iterate over each row
-            for i, val in zip(
-                    range(2, len(table_out), 2),
-                    values):  # start at 2, because first two rows are header
-                table_out[
-                    i] += '─' * self.cell_width + self._char_if_last_else_otherchar(
-                        header, '┤', '┼')
+            for i, val in zip(range(2, len(table_out), 2), values):  # start at 2, because first two rows are header
+                table_out[i] += '─' * self.cell_width + self._char_if_last_else_otherchar(header, '┤', '┼')
                 table_out[i + 1] += f'{str(val):{self.cell_width}}' + '│'
 
-            table_out[
-                -1] += '─' * self.cell_width + self._char_if_last_else_otherchar(
-                    header, '┘', '┴')
+            table_out[-1] += '─' * self.cell_width + self._char_if_last_else_otherchar(header, '┘', '┴')
 
         return '\n'.join(table_out)
 
     def on_up(self):
-        '''when up is pressed, select same column, but row one above (or last row if current is 0)'''
+        """when up is pressed, select same column, but row one above (or last row if current is 0)"""
 
         self.cur_cell[1] = (self.cur_cell[1] - 1) % (self.row_count - 1)
 
     def on_down(self):
-        '''when down is pressed, select same column, but row one below (or first row if current is last)'''
+        """when down is pressed, select same column, but row one below (or first row if current is last)"""
 
         self.cur_cell[1] = (self.cur_cell[1] + 1) % (self.row_count - 1)
 
     def on_left(self):
-        '''when left is pressed, select same row, but column one to the left (or last column if current is 0)'''
+        """when left is pressed, select same row, but column one to the left (or last column if current is 0)"""
 
-        self.cur_cell[0] = (self.cur_cell[0] - 1) % (self.col_count)
+        self.cur_cell[0] = (self.cur_cell[0] - 1) % self.col_count
 
     def on_right(self):
-        '''when right is pressed, select same row, but column one to the right (or first column if current is last)'''
+        """when right is pressed, select same row, but column one to the right (or first column if current is last)"""
 
-        self.cur_cell[0] = (self.cur_cell[0] + 1) % (self.col_count)
+        self.cur_cell[0] = (self.cur_cell[0] + 1) % self.col_count
 
     def add_key(self, key: str):
-        '''add key to current selected cell'''
-        self.data.iat[self.cur_cell[1], self.cur_cell[0]] += key
+        """add key to current selected cell"""
+        self.data.add_key(self.cur_cell[1], self.cur_cell[0], key)
 
     def del_key(self):
-        '''remove last key from current selected cell'''
-        self.data.iat[self.cur_cell[1],
-                      self.cur_cell[0]] = self.data.iat[self.cur_cell[1],
-                                                        self.cur_cell[0]][:-1]
+        """remove last key from current selected cell"""
+        self.data.del_key(self.cur_cell[1], self.cur_cell[0])
 
     def get_current_cursor_position(self) -> tuple[int, int]:
-        '''returns the current position of the cursor, relative to the top left corner character as (0, 0)'''
+        """returns the current position of the cursor, relative to the top left corner character as (0, 0)"""
         y = self.cur_cell[1] * 2 + 3  # 3 is offset for header
 
-        item_length = len(self.data.iat[
-            self.cur_cell[1],
-            self.cur_cell[0]])  # length of the item in the current cell
-
-        x = (self.cell_width + 1) * self.cur_cell[
-            0] + 1 + item_length  # 1 is offset for left border, item_length is length of item
-        return (x, y)
+        item_length = len(self.data.get_item_at(self.cur_cell[1], self.cur_cell[0]))
+        # length of the item in the current cell
+
+        x = (self.cell_width + 1) * self.cur_cell[0] + 1 + item_length
+        # 1 is offset for left border, item_length is length of item
+        return x, y
```

### Comparing `ItsPrompt-1.3/ItsPrompt/keyboard_handler.py` & `ItsPrompt-1.4/ItsPrompt/keyboard_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 from prompt_toolkit import Application
 from prompt_toolkit.key_binding import KeyBindings, KeyPressEvent
 
 
 def generate_key_bindings(app: type[Application]) -> KeyBindings:
-    '''
+    """
     Generates a KeyBindings object for use in a Prompt class
 
-    The `app` is used to check whether specific functions for handling the key events exist. It has to be a Prompt object (e.g. InputPrompt).
-    
+    The `app` is used to check whether specific functions for handling the key events exist. It has to be a Prompt
+    object (e.g. InputPrompt).
+
     The available functions are:
-    
+
     `on_up()`
-    
+
     `on_down()`
-    
+
     `on_left()`
-    
+
     `on_right()`
-    
+
     `on_enter()`
-    
+
     `on_space()`
-    
+
     `on_alt_enter()`
-    
+
     `on_backspace()`
-    
+
     `on_ctrl_backspace()`
-    
+
     `on_key()`
 
     :param app: An application type to check whether one of the above functions exists
     :type app: type[Application]
     :return: An usable KeyBindings instance
     :rtype: KeyBindings
-    '''
+    """
 
     kb = KeyBindings()
 
-    # Each of the options gets the keyboard input and runs the equivalent function in the event.app class, if the function exists.
+    # Each of the options gets the keyboard input and runs the equivalent function in the event.app class,
+    # if the function exists.
 
     @kb.add('c-c')
     def quit(event: KeyPressEvent):
         event.app.exit()
 
     @kb.add('up', filter=hasattr(app, 'on_up'))
     def up(event: KeyPressEvent):
@@ -83,11 +85,10 @@
     # @kb.add('c-w', filter=hasattr(app, 'on_ctrl_backspace'))
     # def ctrl_backspace(event: KeyPressEvent):
     #     event.app.on_ctrl_backspace()  # type: ignore
 
     @kb.add('<any>', filter=hasattr(app, 'on_key'))
     def wildcard(event: KeyPressEvent):
         # wildcard function, used for prompts which need standard key presses like numbers or characters
-        event.app.on_key(  # type: ignore
-            [key.key for key in event.key_sequence], )
+        event.app.on_key([key.key for key in event.key_sequence])  # type: ignore
 
     return kb
```

### Comparing `ItsPrompt-1.3/ItsPrompt/prompt.py` & `ItsPrompt-1.4/ItsPrompt/prompt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,114 @@
-'''
+"""
 # ItsPrompt
 
 created by ItsNameless
 
 :copyright: (c) 2023-present ItsNameless
 :license: MIT, see LICENSE for more details.
-'''
+"""
 
 # mypy: disable-error-code=return-value
 
-from typing import Callable
+from typing import Callable, TYPE_CHECKING, Union
 
-from pandas import DataFrame
 from prompt_toolkit import HTML
 from prompt_toolkit.buffer import Buffer
 from prompt_toolkit.completion import Completer
-from prompt_toolkit.layout.containers import (Float, FloatContainer, HSplit,
-                                              VSplit, Window)
+from prompt_toolkit.layout.containers import (
+    Float,
+    FloatContainer,
+    HSplit,
+    VSplit,
+    Window,
+)
 from prompt_toolkit.layout.controls import BufferControl, FormattedTextControl
 from prompt_toolkit.layout.layout import Layout
-from prompt_toolkit.layout.menus import (CompletionsMenu,
-                                         MultiColumnCompletionsMenu)
+from prompt_toolkit.layout.menus import (
+    CompletionsMenu,
+    MultiColumnCompletionsMenu,
+)
 
 from .data.style import PromptStyle, convert_style, default_style
 from .data.type import CompletionDict
 from .keyboard_handler import generate_key_bindings
 from .prompts.checkbox import CheckboxPrompt
 from .prompts.confirm import ConfirmPrompt
 from .prompts.expand import ExpandPrompt
 from .prompts.input import InputPrompt
 from .prompts.raw_select import RawSelectPrompt
 from .prompts.select import SelectPrompt
 from .prompts.table import TablePrompt
 
+if TYPE_CHECKING:  # pragma: no cover
+    from pandas import DataFrame
+
 
 class Prompt:
-    '''
+    """
     # Modern python prompter
-    
+
     This tool is used to ask the user questions, the fancy way.
-    
+
     Usage:
     ```
     answer = Prompt.checkbox('option 1', 'option 2')
     ```
-    '''
+    """
 
     @classmethod
     def select(
         cls,
         question: str,
         options: tuple[str | tuple[str, str], ...],
         default: str | None = None,
         style: PromptStyle | None = None,
     ) -> str:
-        '''
+        """
         Ask the user for selecting ONE of the given `options`.
 
-        This method shows the question alongside the `options` as a nice list. The user has the ability to use the up, down and enter keys to navigate between the options and select the one thats right.
+        This method shows the question alongside the `options` as a nice list. The user has the ability to use the
+        up, down and enter keys to navigate between the options and select the one thats right.
 
-        The `options` are either a string, which is used as the display value and the id, or a tuple[str, str], where the first string is the display value and the second is the option's id.
+        The `options` are either a string, which is used as the display value and the id, or a tuple[str, str],
+        where the first string is the display value and the second is the option's id.
 
         :param question: The question to display
         :type question: str
         :param options: A list of possible options
         :type options: tuple[str  |  tuple[str, str], ...]
-        :param default: The id of the default option to select (empty or None if the first should be default), defaults to None
+        :param default: The id of the default option to select (empty or None if the first should be default),
+        defaults to None
         :type default: str | None, optional
         :param style: A separate style to style the prompt (empty or None for default style), defaults to None
         :type style: PromptStyle | None, optional
         :raises KeyboardInterrupt: When the user presses ctrl-c, `KeyboardInterrupt` will be raised
         :return: The id of the selected option
         :rtype: str
-        '''
+        """
         app = SelectPrompt(
             question,
             options,
             default,
             layout=Layout(
-                HSplit([
-                    Window(FormattedTextControl(), always_hide_cursor=True),
-                    Window(FormattedTextControl(
-                        HTML('Use UP, DOWN to select, ENTER to submit')),
-                           char=' ',
-                           style='class:tooltip',
-                           height=1)
-                ])),
+                HSplit(
+                    [
+                        Window(FormattedTextControl(), always_hide_cursor=True),
+                        Window(
+                            FormattedTextControl(HTML('Use UP, DOWN to select, ENTER to submit')),
+                            char=' ',
+                            style='class:tooltip',
+                            height=1
+                        )
+                    ]
+                )
+            ),
             key_bindings=generate_key_bindings(SelectPrompt),
             erase_when_done=True,
-            style=convert_style(style)
-            if style else convert_style(default_style),
+            style=convert_style(style) if style else convert_style(default_style),
         )
         ans = app.prompt()
         if ans == None:
             raise KeyboardInterrupt()
         return ans
 
     @classmethod
@@ -101,55 +116,59 @@
         cls,
         question: str,
         options: tuple[str | tuple[str, str], ...],
         default: str | None = None,
         allow_keyboard: bool = False,
         style: PromptStyle | None = None,
     ) -> str:
-        '''
+        """
         Ask the user for selection ONE of the given `options`.
 
-        This method shows the question alongside the `options` as a nice list. The user needs to type the index of the answer. If `allow_keyboard` is given, the user may use the keyboard as in the `select()` method.
+        This method shows the question alongside the `options` as a nice list. The user needs to type the index of
+        the answer. If `allow_keyboard` is given, the user may use the keyboard as in the `select()` method.
 
-        The `options` are either a string, which is used as the display value and the id, or a tuple[str, str], where the first string is the display value and the second is the option's id.
+        The `options` are either a string, which is used as the display value and the id, or a tuple[str, str],
+        where the first string is the display value and the second is the option's id.
 
         :param question: The question to display
         :type question: str
         :param options: A list of possible options
         :type options: tuple[str  |  tuple[str, str], ...]
-        :param default: The id of the default option to select (empty or None if the first should be default), defaults to None
+        :param default: The id of the default option to select (empty or None if the first should be default),
+        defaults to None
         :type default: str | None, optional
         :param allow_keyboard: Whether the user should be able to select the answer with up and down, defaults to False
         :type allow_keyboard: bool, optional
         :param style: A separate style to style the prompt (empty or None for default style), defaults to None
         :type style: PromptStyle | None, optional
         :raises KeyboardInterrupt: When the user presses ctrl-c, `KeyboardInterrupt` will be raised
         :return: The id of the selected option
         :rtype: str
-        '''
+        """
         app = RawSelectPrompt(
             question,
             options,
             default,
             allow_keyboard,
             layout=Layout(
-                HSplit([
-                    Window(FormattedTextControl(), always_hide_cursor=True),
-                    Window(FormattedTextControl(
-                        HTML(
-                            'Type the INDEX of your selection, ENTER to submit'
-                        )),
-                           char=' ',
-                           style='class:tooltip',
-                           height=1)
-                ])),
+                HSplit(
+                    [
+                        Window(FormattedTextControl(), always_hide_cursor=True),
+                        Window(
+                            FormattedTextControl(HTML('Type the INDEX of your selection, ENTER to submit')),
+                            char=' ',
+                            style='class:tooltip',
+                            height=1
+                        )
+                    ]
+                )
+            ),
             key_bindings=generate_key_bindings(RawSelectPrompt),
             erase_when_done=True,
-            style=convert_style(style)
-            if style else convert_style(default_style),
+            style=convert_style(style) if style else convert_style(default_style),
         )
         ans = app.prompt()
         if ans == None:
             raise KeyboardInterrupt()
         return ans
 
     @classmethod
@@ -157,170 +176,182 @@
         cls,
         question: str,
         options: tuple[str | tuple[str, str, str], ...],
         default: str | None = None,
         allow_keyboard: bool = False,
         style: PromptStyle | None = None,
     ) -> str:
-        '''
+        """
         Ask the user for selecting ONE of the given `options`.
 
         The user needs to type the key of the option. If the user types `h`, all options will be shown.
 
-        The `options` are either a string, where `s[0]` will be the key to select and the string will be used as name and id, or a tuple[str, str, str] where `t[0]` will be the key, `t[1]` the name and `t[2]` the id of the option.
+        The `options` are either a string, where `s[0]` will be the key to select and the string will be used as name
+        and id, or a tuple[str, str, str] where `t[0]` will be the key, `t[1]` the name and `t[2]` the id of the option.
 
         Every key must be a unique ascii character and of length 1, and there may not be a key assigned to `h`.
 
         :param question: The question to display
         :type question: str
         :param options: A list of possible options
         :type options: tuple[str  |  tuple[str, str, str], ...]
-        :param default: The id of the default option to select (empty or None if `h` should be default), defaults to None
+        :param default: The id of the default option to select (empty or None if `h` should be default), defaults to
+        None
         :type default: str | None, optional
         :param allow_keyboard: Whether the user should be able to select the answer with up and down, defaults to False
         :type allow_keyboard: bool, optional
         :param style: A separate style to style the prompt (empty or None for default style), defaults to None
         :type style: PromptStyle | None, optional
         :raises KeyboardInterrupt: When the user presses ctrl-c, `KeyboardInterrupt` will be raised
         :return: The id of the selected option
         :rtype: str
-        '''
+        """
         app = ExpandPrompt(
             question,
             options,
             default,
             allow_keyboard,
             layout=Layout(
-                HSplit([
-                    Window(FormattedTextControl(), always_hide_cursor=True),
-                    Window(FormattedTextControl(
-                        HTML(
-                            'Type the KEY for your selection, ENTER to submit (use h to show all options)'
-                        )),
-                           char=' ',
-                           style='class:tooltip',
-                           height=1)
-                ])),
+                HSplit(
+                    [
+                        Window(FormattedTextControl(), always_hide_cursor=True),
+                        Window(
+                            FormattedTextControl(
+                                HTML('Type the KEY for your selection, ENTER to submit (use h to show all options)')
+                            ),
+                            char=' ',
+                            style='class:tooltip',
+                            height=1
+                        )
+                    ]
+                )
+            ),
             key_bindings=generate_key_bindings(ExpandPrompt),
             erase_when_done=True,
-            style=convert_style(style)
-            if style else convert_style(default_style),
+            style=convert_style(style) if style else convert_style(default_style),
         )
         ans = app.prompt()
         if ans == None:
             raise KeyboardInterrupt()
         return ans
 
     @classmethod
     def checkbox(
         cls,
         question: str,
         options: tuple[str | tuple[str, str], ...],
-        pointer_at: int
-        | None = None,
+        pointer_at: int | None = None,
         default_checked: tuple[str, ...] | None = None,
         min_selections: int = 0,
         style: PromptStyle | None = None,
     ) -> list[str]:
-        '''
+        """
         Ask the user for selecting MULTIPLE of the given `options`.
 
-        The `options` will be shown as a nice list. The user may navigate with up and down, select or deselect with space and submit with enter.
+        The `options` will be shown as a nice list. The user may navigate with up and down, select or deselect with
+        space and submit with enter.
 
-        The `options` are either a string, which is used as the display value and the id, or a tuple[str, str], where the first string is the display value and the second is the option's id.
+        The `options` are either a string, which is used as the display value and the id, or a tuple[str, str],
+        where the first string is the display value and the second is the option's id.
 
         :param question: The question to display
         :type question: str
         :param options: A list of possible options
         :type options: tuple[str  |  tuple[str, str], ...]
         :param pointer_at: A 0-indexed value, where the pointer should start (0 if None), defaults to None
         :type pointer_at: int | None, optional
         :param default_checked: A list of ids, which should be checked by default (empty if None)
         :type default_checked: tuple[str, ...] | None, optional
-        :param min_selections: A minimum amount of options that need to be checked before submitting (prohibits the user of submitting, if not enough are checked; 0 if None)
+        :param min_selections: A minimum amount of options that need to be checked before submitting (prohibits the
+        user of submitting, if not enough are checked; 0 if None)
         :type min_selections: int, optional
         :param style: A separate style to style the prompt (empty or None for default style), defaults to None
         :type style: PromptStyle | None, optional
         :raises KeyboardInterrupt: When the user presses ctrl-c, `KeyboardInterrupt` will be raised
         :return: The ids of the selected options
         :rtype: list[str]
-        '''
+        """
         app = CheckboxPrompt(
             question,
             options,
             pointer_at,
             default_checked,
             min_selections,
             layout=Layout(
-                HSplit([
-                    Window(FormattedTextControl(), always_hide_cursor=True),
-                    Window(FormattedTextControl(
-                        HTML(
-                            'Use UP, DOWN to change selection, SPACE to select, ENTER to submit'
-                        )),
-                           char=' ',
-                           style='class:tooltip',
-                           height=1)
-                ])),
+                HSplit(
+                    [
+                        Window(FormattedTextControl(), always_hide_cursor=True),
+                        Window(
+                            FormattedTextControl(
+                                HTML('Use UP, DOWN to change selection, SPACE to select, ENTER to submit')
+                            ),
+                            char=' ',
+                            style='class:tooltip',
+                            height=1
+                        )
+                    ]
+                )
+            ),
             key_bindings=generate_key_bindings(CheckboxPrompt),
             erase_when_done=True,
-            style=convert_style(style)
-            if style else convert_style(default_style),
+            style=convert_style(style) if style else convert_style(default_style),
         )
         ans = app.prompt()
         if ans == None:
             raise KeyboardInterrupt()
         return ans
 
     @classmethod
     def confirm(
         cls,
         question: str,
         default: bool | None = None,
         style: PromptStyle | None = None,
     ) -> bool:
-        '''
+        """
         Ask the user for confirming or denying your prompt.
 
         The user needs to type "y", "n" or enter (only if default is given).
 
         If `default` is `True`, the prompt will be in the style of (Y/n).
 
         If `default` is `False`, the prompt will be in the style of (n/Y).
 
-        If `default` is `None` (or not given), the prompt will be in the style of (y/n). In this case, the user may not use enter to submit the default, as there is no default given.
+        If `default` is `None` (or not given), the prompt will be in the style of (y/n). In this case, the user may
+        not use enter to submit the default, as there is no default given.
 
         :param question: The question to display
         :type question: str
         :param default: The default answer to select when pressing enter, defaults to None
         :type default: bool | None, optional
         :param style: A separate style to style the prompt (empty or None for default style), defaults to None
         :type style: PromptStyle | None, optional
         :raises KeyboardInterrupt: When the user presses ctrl-c, `KeyboardInterrupt` will be raised
         :return: Whether the user selected "y" or "n"
         :rtype: bool
-        '''
+        """
         app = ConfirmPrompt(
             question,
             default,
             layout=Layout(
-                HSplit([
-                    Window(FormattedTextControl(), always_hide_cursor=True),
-                    Window(FormattedTextControl(
-                        HTML(
-                            'Press Y or N, ENTER if default value is available'
-                        )),
-                           char=' ',
-                           style='class:tooltip',
-                           height=1)
-                ])),
+                HSplit(
+                    [
+                        Window(FormattedTextControl(), always_hide_cursor=True),
+                        Window(
+                            FormattedTextControl(HTML('Press Y or N, ENTER if default value is available')),
+                            char=' ',
+                            style='class:tooltip',
+                            height=1
+                        )
+                    ]
+                )
+            ),
             key_bindings=generate_key_bindings(ConfirmPrompt),
             erase_when_done=True,
-            style=convert_style(style)
-            if style else convert_style(default_style),
+            style=convert_style(style) if style else convert_style(default_style),
         )
 
         ans = app.prompt()
         if ans == None:
             raise KeyboardInterrupt()
         return ans
 
@@ -333,26 +364,32 @@
         show_symbol: str | None = None,
         validate: Callable[[str], str | None] | None = None,
         completions: list[str] | CompletionDict | None = None,
         completer: Completer | None = None,
         completion_show_multicolumn: bool = False,
         style: PromptStyle | None = None,
     ) -> str:
-        '''
+        """
         Ask the user for typing an input.
 
-        If default is given, it will be returned if enter was pressed and no input was given by the user. If the user writes an input, the default will be overwritten.
+        If default is given, it will be returned if enter was pressed and no input was given by the user. If the user
+        writes an input, the default will be overwritten.
 
         If multiline is activated, enter will not submit, but rather create a newline. Use `alt+enter` to submit.
 
-        If show_symbol is given, all chars (except newlines) will be replaced with this character in the interface. The result will still be the input the user typed, it just will not appear in the CLI.
+        If show_symbol is given, all chars (except newlines) will be replaced with this character in the interface.
+        The result will still be the input the user typed, it just will not appear in the CLI.
 
-        Validate takes a function which receives a `str` (the current input of the user) and may return None or a `str`. If the function returns None, the prompt may assume that the input is valid. If it returns a `str`, this will be the error shown to the user. The user will not be able to submit the input, if validate returns an error.
+        Validate takes a function which receives a `str` (the current input of the user) and may return None or a
+        `str`. If the function returns None, the prompt may assume that the input is valid. If it returns a `str`,
+        this will be the error shown to the user. The user will not be able to submit the input, if validate returns
+        an error.
 
-        Completions may be a list of possible completion strings or a nested dictionary where the key is a completion string and the value is a new dict in the same style (more in the README.md).
+        Completions may be a list of possible completion strings or a nested dictionary where the key is a completion
+        string and the value is a new dict in the same style (more in the README.md).
 
         You can use your own Completer as well (more in the README.md).
 
         THESE VALUES ARE MUTUALLY EXCLUSIVE. You may not use both. If you use a completer, you can not use show_symbol!
 
         :param question: The question to display
         :type question: str
@@ -364,119 +401,127 @@
         :type show_symbol: str | None, optional
         :param validate: A function to check the users input in real-time, defaults to None
         :type validate: Callable[[str], str | None] | None, optional
         :param completions: The completions to use, defaults to None
         :type completions: list[str] | CompletionDict | None, optional
         :param completer: A completer to use, defaults to None
         :type completer: Completer | None, optional
-        :param completion_show_multicolumn: Whether to show the completions as a scrollable list or as multiple columns, defaults to False
+        :param completion_show_multicolumn: Whether to show the completions as a scrollable list or as multiple
+        columns, defaults to False
         :type completion_show_multicolumn: bool, optional
         :param style: A separate style to style the prompt (empty or None for default style), defaults to None
         :type style: PromptStyle | None, optional
         :raises KeyboardInterrupt: When the user presses ctrl-c, `KeyboardInterrupt` will be raised
         :return: The input of the user
         :rtype: str
-        '''
+        """
 
         # extracting the body, so we can display a floating auto completion field
-        body = HSplit([
-            VSplit([
-                Window(
-                    FormattedTextControl(),
-                    always_hide_cursor=True,
-                    dont_extend_width=True,
+        body = HSplit(
+            [
+                VSplit(
+                    [
+                        Window(
+                            FormattedTextControl(),
+                            always_hide_cursor=True,
+                            dont_extend_width=True,
+                        ),
+                        Window(BufferControl(Buffer(complete_while_typing=True))),
+                        # the completer will be passed in the Application class
+                    ]
                 ),
                 Window(
-                    BufferControl(Buffer(complete_while_typing=True))
-                ),  # the completer will be passed in the Application class
-            ]),
-            Window(
-                FormattedTextControl(
-                    HTML(
-                        f'Type your answer, {"ALT+ENTER" if multiline else "ENTER"} to submit'
-                    )),
-                char=' ',
-                style='class:tooltip',
-                height=1,
-            )
-        ])
+                    FormattedTextControl(HTML(f'Type your answer, {"ALT+ENTER" if multiline else "ENTER"} to submit')),
+                    char=' ',
+                    style='class:tooltip',
+                    height=1,
+                )
+            ]
+        )
 
         app = InputPrompt(
             question,
             default,
             multiline,
             show_symbol,
             validate,
             completions,
             completer,
             layout=Layout(
                 FloatContainer(
                     content=body,
                     floats=[
                         Float(
-                            MultiColumnCompletionsMenu(show_meta=False) if
-                            completion_show_multicolumn else CompletionsMenu(),
+                            MultiColumnCompletionsMenu(show_meta=False)
+                            if completion_show_multicolumn else CompletionsMenu(),
                             xcursor=True,
                             ycursor=True,
                         )
-                    ])),
+                    ]
+                )
+            ),
             key_bindings=generate_key_bindings(InputPrompt),
             erase_when_done=True,
-            style=convert_style(style)
-            if style else convert_style(default_style),
+            style=convert_style(style) if style else convert_style(default_style),
         )
 
         ans = app.prompt()
         if ans == None:
             raise KeyboardInterrupt()
         return ans
 
     @classmethod
     def table(
         cls,
         question: str,
-        data: DataFrame,
+        data: Union["DataFrame", dict[str, list[str]]],
         style: PromptStyle | None = None,
-    ) -> DataFrame:
-        '''
+    ) -> Union["DataFrame", dict[str, list[str]]]:
+        """
         Ask the user for filling out the displayed table.
 
-        This method shows the question alongside a table, which the user may navigate with the arrow keys. The user has the ability to use the up, down and enter keys to navigate between the options and change the text in each cell.
+        This method shows the question alongside a table, which the user may navigate with the arrow keys. The user
+        has the ability to use the up, down and enter keys to navigate between the options and change the text in
+        each cell.
 
-        The `data` is a pandas DataFrame, where the values will be input in the cells by default.
+        The `data` is either a pandas DataFrame or a dictionary.
 
-        # TODO
         :param question: The question to display
         :type question: str
-        :param options: A list of possible options
-        :type options: tuple[str  |  tuple[str, str], ...]
-        :param default: The id of the default option to select (empty or None if the first should be default), defaults to None
-        :type default: str | None, optional
+        :param data: The data to display
+        :type data: DataFrame | dict[str, list[str]]
         :param style: A separate style to style the prompt (empty or None for default style), defaults to None
         :type style: PromptStyle | None, optional
         :raises KeyboardInterrupt: When the user presses ctrl-c, `KeyboardInterrupt` will be raised
         :return: The id of the selected option
         :rtype: str
-        '''
+        """
         app = TablePrompt(
             question,
             data,
             layout=Layout(
-                HSplit([
-                    Window(FormattedTextControl()),
-                    Window(FormattedTextControl(
-                        HTML(
-                            'Use UP, DOWN, LEFT, RIGHT to select a cell, TYPE to add char, BACKSPACE to delete char, ENTER to submit'
-                        )),
-                           char=' ',
-                           style='class:tooltip',
-                           height=1)
-                ])),
+                HSplit(
+                    [
+                        Window(FormattedTextControl()),
+                        Window(
+                            FormattedTextControl(
+                                HTML(
+                                    'Use UP, DOWN, LEFT, RIGHT to select a cell, TYPE to add char, BACKSPACE to '
+                                    'delete char, ENTER to submit'
+                                )
+                            ),
+                            char=' ',
+                            style='class:tooltip',
+                            height=1
+                        )
+                    ]
+                )
+            ),
             key_bindings=generate_key_bindings(TablePrompt),
             erase_when_done=True,
-            style=convert_style(style)
-            if style else convert_style(default_style),
+            style=convert_style(style) if style else convert_style(default_style),
         )
         ans = app.prompt()
-        if type(ans) != DataFrame and ans == None:
+        # if type(ans) is type(None):
+        if ans is None:
             raise KeyboardInterrupt()
-        return ans
+        return ans  # type: ignore
```

### Comparing `ItsPrompt-1.3/ItsPrompt/prompts/checkbox.py` & `ItsPrompt-1.4/ItsPrompt/prompts/checkbox.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from prompt_toolkit import HTML, Application
+from prompt_toolkit import Application, HTML
 from prompt_toolkit.layout.containers import Window
 from prompt_toolkit.layout.controls import FormattedTextControl
 
 from ..data.checkbox import process_data
 
 
 class CheckboxPrompt(Application):
-
     CHECKED_SIGN = '\u25cf'
     UNCHECKED_SIGN = '\u25cb'
 
     def __init__(
         self,
         question: str,
         options: tuple[str | tuple[str, str], ...],
@@ -19,22 +18,19 @@
         min_selections: int = 0,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
         # get prompt content box
-        self.prompt_content: FormattedTextControl = self.layout.container.get_children(
-        )[0].content  # type: ignore
+        self.prompt_content: FormattedTextControl = self.layout.container.get_children()[0].content  # type: ignore
 
         # save toolbar window and box (for showing errors)
-        self.toolbar_window: Window = self.layout.container.get_children()[
-            1]  # type: ignore
-        self.toolbar_content: FormattedTextControl = self.layout.container.get_children(
-        )[1].content  # type: ignore
+        self.toolbar_window: Window = self.layout.container.get_children()[1]  # type: ignore
+        self.toolbar_content: FormattedTextControl = self.layout.container.get_children()[1].content  # type: ignore
 
         # save standard toolbar content
         self.toolbar_content_default_text = self.toolbar_content.text
 
         # save whether error is currently shown
         self.is_error = False
 
@@ -58,70 +54,72 @@
             # so we raise an error.
             for option in self.options:
                 if option.id in default_checked:
                     option.is_selected = True
                     was_set += 1
 
             if was_set != len(default_checked):
-                raise ValueError(
-                    'At least one of the given default_checked values is invalid.'
-                )
+                raise ValueError('At least one of the given default_checked values is invalid.')
 
     def update(self):
-        '''update prompt content'''
+        """update prompt content"""
         content = f'[<question_mark>?</question_mark>] <question>{self.question}</question>:'
 
         for i, option in enumerate(self.options):
             if i == self.selection:
-                content += f'\n<selected_option>  > {self.__class__.CHECKED_SIGN if option.is_selected else self.__class__.UNCHECKED_SIGN} {option.name}</selected_option>'
+                content += f'\n<selected_option>  > ' \
+                           f'{self.__class__.CHECKED_SIGN if option.is_selected else self.__class__.UNCHECKED_SIGN} ' \
+                           f'{option.name}</selected_option>'
             else:
-                content += f'\n<option>    {self.__class__.CHECKED_SIGN if option.is_selected else self.__class__.UNCHECKED_SIGN} {option.name}</option>'
-
-        self.prompt_content.text = HTML(content)
-
-        # show error, if error should be shown, else show normal prompt
-        if not self.is_error:
-            # show normal prompt, change style to standard toolbar
-            self.toolbar_content.text = self.toolbar_content_default_text
-            self.toolbar_window.style = 'class:tooltip'
-        else:  # pragma: no cover
-            # show error prompt and error style
-            # the only error that might occur is that not enough options are selected
-            self.toolbar_content.text = f'ERROR: a minimum of {self.min_selections} options need to be selected!'
-            self.toolbar_window.style = 'class:error'
+                content += f'\n<option>    ' \
+                           f'{self.__class__.CHECKED_SIGN if option.is_selected else self.__class__.UNCHECKED_SIGN} ' \
+                           f' {option.name} </option> '
+
+                self.prompt_content.text = HTML(content)
+
+                # show error, if error should be shown, else show normal prompt
+                if not self.is_error:
+                    # show normal prompt, change style to standard toolbar
+                    self.toolbar_content.text = self.toolbar_content_default_text
+                    self.toolbar_window.style = 'class:tooltip'
+                else:  # pragma: no cover
+                    # show error prompt and error style
+                    # the only error that might occur is that not enough options are selected
+                    self.toolbar_content.text = f'ERROR: a minimum of {self.min_selections} options need to be ' \
+                                                f'selected!'
+                    self.toolbar_window.style = 'class:error'
 
     def prompt(self) -> list[str] | None:
-        '''start the application, returns the return value'''
+        """start the application, returns the return value"""
         self.update()
         out: list[str] | None = self.run()
 
         return out
 
     def on_up(self):
-        '''when up is pressed, the previous indexed option will be selected'''
+        """when up is pressed, the previous indexed option will be selected"""
         self.selection = (self.selection - 1) % len(self.options)
 
         # reset error
         self.is_error = False
 
         self.update()
 
     def on_down(self):
-        '''when down is pressed, the next indexed option will be selected'''
+        """when down is pressed, the next indexed option will be selected"""
         self.selection = (self.selection + 1) % len(self.options)
 
         # reset error
         self.is_error = False
 
         self.update()
 
     def on_space(self):
-        '''when space is pressed, select or deselect current selection'''
-        self.options[self.selection].is_selected = not self.options[
-            self.selection].is_selected
+        """when space is pressed, select or deselect current selection"""
+        self.options[self.selection].is_selected = not self.options[self.selection].is_selected
 
         # reset error
         self.is_error = False
 
         self.update()
 
     def on_enter(self):
```

### Comparing `ItsPrompt-1.3/ItsPrompt/prompts/confirm.py` & `ItsPrompt-1.4/ItsPrompt/prompts/confirm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from prompt_toolkit import HTML, Application
+from prompt_toolkit import Application, HTML
 from prompt_toolkit.layout.containers import Window
 from prompt_toolkit.layout.controls import FormattedTextControl
 
 
 class ConfirmPrompt(Application):
 
     def __init__(
@@ -11,38 +11,36 @@
         default: bool | None = None,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
         # get prompt content box
-        self.prompt_content: FormattedTextControl = self.layout.container.get_children(
-        )[0].content  # type: ignore
+        self.prompt_content: FormattedTextControl = self.layout.container.get_children()[0].content  # type: ignore
 
         # save toolbar window and box (for showing errors)
-        self.toolbar_window: Window = self.layout.container.get_children()[
-            1]  # type: ignore
-        self.toolbar_content: FormattedTextControl = self.layout.container.get_children(
-        )[1].content  # type: ignore
+        self.toolbar_window: Window = self.layout.container.get_children()[1]  # type: ignore
+        self.toolbar_content: FormattedTextControl = self.layout.container.get_children()[1].content  # type: ignore
 
         # save standard toolbar content
         self.toolbar_content_default_text = self.toolbar_content.text
 
         # save whether error is currently shown
         self.is_error = False
 
         # save question
         self.question = question
 
         # save default selection
         self.default = default
 
     def update(self):
-        '''update prompt content'''
-        content = f'[<question_mark>?</question_mark>] <question>{self.question}</question>: <text>({"Y" if self.default==True else "y"}/{"N" if self.default==False else "n"})</text>'
+        """update prompt content"""
+        content = f'[<question_mark>?</question_mark>] <question>{self.question}</question>: <text>(' \
+                  f'{"Y" if self.default == True else "y"}/{"N" if self.default == False else "n"})</text>'
 
         self.prompt_content.text = HTML(content)
 
         # show error, if error should be shown, else show normal prompt
         if not self.is_error:
             # show normal prompt, change style to standard toolbar
             self.toolbar_content.text = self.toolbar_content_default_text
@@ -50,22 +48,22 @@
         else:  # pragma: no cover
             # show error prompt and error style
             # the only error that might occur is that not enough options are selected
             self.toolbar_content.text = f'ERROR: a selection must be made!'
             self.toolbar_window.style = 'class:error'
 
     def prompt(self) -> bool | None:
-        '''start the application, returns the return value'''
+        """start the application, returns the return value"""
         self.update()
         out: bool | None = self.run()
 
         return out
 
     def on_key(self, key_sequence: list[str]):
-        '''when Y or N is pressed, select value and submit'''
+        """when Y or N is pressed, select value and submit"""
         key = key_sequence[0]
 
         # return if key is not an available key
         if not key in ['y', 'n']:
             return
 
         # exit with answer
```

### Comparing `ItsPrompt-1.3/ItsPrompt/prompts/expand.py` & `ItsPrompt-1.4/ItsPrompt/prompts/expand.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from prompt_toolkit import HTML, Application
+from prompt_toolkit import Application, HTML
 from prompt_toolkit.layout.controls import FormattedTextControl
 
 from ..data.expand import process_data
 
 
 class ExpandPrompt(Application):
 
@@ -14,16 +14,15 @@
         allow_keyboard: bool = False,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
         # get prompt content box
-        self.prompt_content: FormattedTextControl = self.layout.container.get_children(
-        )[0].content  # type: ignore
+        self.prompt_content: FormattedTextControl = self.layout.container.get_children()[0].content  # type: ignore
 
         # save question
         self.question = question
 
         # save keyboard option
         self.allow_keyboard = allow_keyboard
 
@@ -45,15 +44,15 @@
             if option.id == default:
                 self.selection = option.key
                 break
         else:
             raise ValueError('Default value is not a valid id.')
 
     def update(self):
-        '''update prompt content'''
+        """update prompt content"""
         # question
         content = f'[<question_mark>?</question_mark>] <question>{self.question}</question>: <text>({self.keys})</text>'
 
         # options, show only if it is expanded
         if self.is_expanded:
             for option in self.options:
                 if option.key == self.selection:
@@ -63,45 +62,43 @@
 
         # text
         content += f'\n<text>    Answer: {self.selection}</text>'
 
         self.prompt_content.text = HTML(content)
 
     def prompt(self) -> str | None:
-        '''start the application, returns the return value'''
+        """start the application, returns the return value"""
         self.update()
         out: str | None = self.run()
 
         return out
 
     def on_up(self):
-        '''when up is pressed, the previous indexed option will be selected'''
+        """when up is pressed, the previous indexed option will be selected"""
         if not self.allow_keyboard:
             return
 
-        self.selection = self.keys[(self.keys.index(self.selection) - 1) %
-                                   len(self.keys)]
+        self.selection = self.keys[(self.keys.index(self.selection) - 1) % len(self.keys)]
 
         self.update()
 
     def on_down(self):
-        '''when down is pressed, the next indexed option will be selected'''
+        """when down is pressed, the next indexed option will be selected"""
         if not self.allow_keyboard:
             return
 
-        self.selection = self.keys[(self.keys.index(self.selection) + 1) %
-                                   len(self.keys)]
+        self.selection = self.keys[(self.keys.index(self.selection) + 1) % len(self.keys)]
 
         self.update()
 
     def on_key(self, key_sequence: list[str]):
-        '''when a index is pressed, which is available to select, select this index'''
+        """when an index is pressed, which is available to select, select this index"""
         key = key_sequence[0]
 
-        # return if key is not a an available key
+        # return if key is not an available key
         if not key in self.keys:
             return
 
         # only expand if h is pressed, otherwise change selection
         if key == 'h':
             self.is_expanded = not self.is_expanded
         else:
```

### Comparing `ItsPrompt-1.3/ItsPrompt/prompts/input.py` & `ItsPrompt-1.4/ItsPrompt/prompts/input.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-import string
 from typing import Callable
 
-from prompt_toolkit import HTML, Application
+from prompt_toolkit import Application, HTML
 from prompt_toolkit.buffer import Buffer
-from prompt_toolkit.completion import (Completer, FuzzyCompleter,
-                                       FuzzyWordCompleter, NestedCompleter)
+from prompt_toolkit.completion import (
+    Completer,
+    FuzzyCompleter,
+    FuzzyWordCompleter,
+    NestedCompleter,
+)
 from prompt_toolkit.layout.containers import Window
 from prompt_toolkit.layout.controls import FormattedTextControl
 from prompt_toolkit.layout.processors import PasswordProcessor
 
 from ..data.type import CompletionDict
 
 
@@ -29,16 +32,15 @@
         super().__init__(*args, **kwargs)
 
         # temp body variable for making object accessing clearer
         _body = self.layout.container.content.get_children()  # type: ignore
         _vsplit = _body[0].get_children()
 
         # get prompt content box
-        self.prompt_content: FormattedTextControl = _vsplit[
-            0].content  # type: ignore
+        self.prompt_content: FormattedTextControl = _vsplit[0].content  # type: ignore
 
         # get input buffer
         self.buffer: Buffer = _vsplit[1].content.buffer  # type: ignore
 
         # save toolbar window and box (for showing errors)
         self.toolbar_window: Window = _body[1]  # type: ignore
         self.toolbar_content: FormattedTextControl = self.toolbar_window.content  # type: ignore
@@ -62,54 +64,48 @@
         self.multiline = multiline
 
         # save show_symbol
         self.show_symbol = show_symbol
 
         # when show_symbol is given, use PasswordProcessor to show the symbol instead of the text
         if self.show_symbol:
-            _vsplit[1].content.input_processors = [
-                PasswordProcessor(self.show_symbol)
-            ]
+            _vsplit[1].content.input_processors = [PasswordProcessor(self.show_symbol)]
 
         # save validator function
         self.validate = validate
 
         # save the completer
         self.completer: None | Completer = None
 
         if completions and completer:
-            raise ValueError(
-                'completions and completer are mutually exclusive! Please use only one of them!'
-            )
+            raise ValueError("completions and completer are mutually exclusive! Please use only one of them!")
 
         if show_symbol and (completions or completer):
             # symbol and completer are mutually exclusive
-            raise ValueError(
-                'Completions are not compatible with show_symbol!')
+            raise ValueError('Completions are not compatible with show_symbol!')
 
         if completions:  # pragma: no cover
             # a list or a dict of completions to use is given
             if type(completions) is list:
                 # we use FuzzyWordCompleter
                 self.completer = FuzzyWordCompleter(list(completions))
             elif type(completions) is dict:
                 # we use FuzzyCompleter with NestedCompleter
-                self.completer = FuzzyCompleter(
-                    NestedCompleter.from_nested_dict(completions))
+                self.completer = FuzzyCompleter(NestedCompleter.from_nested_dict(completions))
 
         elif completer:  # pragma: no cover
             # a self-created completer is given
             self.completer = completer
 
         # assign the created completer to the buffer
         if self.completer:  # pragma: no cover
             self.buffer.completer = self.completer
 
     def update(self):  # pragma: no cover
-        '''update prompt content'''
+        """update prompt content"""
         content = f'[<question_mark>?</question_mark>] <question>{self.question}</question>: '
 
         if self.default and self.buffer.text == '':
             content += f'<grayout>{self.default}</grayout>'
 
         self.prompt_content.text = HTML(content)
 
@@ -136,44 +132,44 @@
         # (and all of its commands) need to be run manually every time we press a key.
         # This does not in any way change the user experience,
         # as it does the exact same thing the standard completer does.
         if self.is_running:
             self.buffer.start_completion()
 
     def prompt(self) -> str | None:
-        '''start the application, returns the return value'''
+        """start the application, returns the return value"""
         self.update()
         out: str | None = self.run()
 
         return out
 
     def _submit(self):
-        '''method for submitting result, as this is done by two functions'''
+        """method for submitting result, as this is done by two functions"""
         # if an error is currently shown, prevent submit
         if self.is_error:  # pragma: no cover
             return
 
         # return buffer if given, else default if given, else empty string
         if self.buffer.text != '':
             self.exit(result=self.buffer.text)
         elif self.default:
             self.exit(result=self.default)
         else:
             self.exit(result='')
 
     def on_alt_enter(self):
-        '''if multiline is enabled, this will submit'''
+        """if multiline is enabled, this will submit"""
         if self.multiline:
             self._submit()
 
     def on_enter(self):
-        '''either submit key or in multiline, append new line'''
+        """either submit key or in multiline, append new line"""
         # run completion
-        if (self.is_running) and self.buffer.complete_state and (
-                completion := self.buffer.complete_state.current_completion
+        if self.is_running and self.buffer.complete_state and (
+            completion := self.buffer.complete_state.current_completion
         ):  # pragma: no cover
             self.buffer.apply_completion(completion)
 
         if self.multiline:
             self.buffer.text += '\n'
             self.buffer.cursor_down()
             self.update()
```

### Comparing `ItsPrompt-1.3/ItsPrompt/prompts/raw_select.py` & `ItsPrompt-1.4/ItsPrompt/prompts/raw_select.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from prompt_toolkit import HTML, Application
+from prompt_toolkit import Application, HTML
 from prompt_toolkit.layout.controls import FormattedTextControl
 
 from ..data.select import process_data
 
 
 class RawSelectPrompt(Application):
 
@@ -14,16 +14,15 @@
         allow_keyboard: bool = False,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
         # get prompt content box
-        self.prompt_content: FormattedTextControl = self.layout.container.get_children(
-        )[0].content  # type: ignore
+        self.prompt_content: FormattedTextControl = self.layout.container.get_children()[0].content  # type: ignore
 
         # save question
         self.question = question
 
         # self keyboard option
         self.allow_keyboard = allow_keyboard
 
@@ -39,57 +38,57 @@
             if option.id == default:
                 self.selection = i
                 break
         else:
             raise ValueError('Default value is not a valid id.')
 
     def update(self):
-        '''update prompt content'''
+        """update prompt content"""
         # question
         content = f'[<question_mark>?</question_mark>] <question>{self.question}</question>:'
 
         # options
         for i, option in enumerate(self.options):
             if i == self.selection:
-                content += f'\n<selected_option>    {i+1}) {option.name}</selected_option>'
+                content += f'\n<selected_option>    {i + 1}) {option.name}</selected_option>'
             else:
-                content += f'\n<option>    {i+1}) {option.name}</option>'
+                content += f'\n<option>    {i + 1}) {option.name}</option>'
 
         # text
-        content += f'\n<text>    Answer: {self.selection+1}</text>'
+        content += f'\n<text>    Answer: {self.selection + 1}</text>'
 
         self.prompt_content.text = HTML(content)
 
     def prompt(self) -> str | None:
-        '''start the application, returns the return value'''
+        """start the application, returns the return value"""
         self.update()
         out: str | None = self.run()
 
         return out
 
     def on_up(self):
-        '''when up is pressed, the previous indexed option will be selected'''
+        """when up is pressed, the previous indexed option will be selected"""
         if not self.allow_keyboard:
             return
 
         self.selection = (self.selection - 1) % len(self.options)
 
         self.update()
 
     def on_down(self):
-        '''when down is pressed, the next indexed option will be selected'''
+        """when down is pressed, the next indexed option will be selected"""
         if not self.allow_keyboard:
             return
 
         self.selection = (self.selection + 1) % len(self.options)
 
         self.update()
 
     def on_key(self, key_sequence: list[str]):
-        '''when a index is pressed, which is available to select, select this index'''
+        """when an index is pressed, which is available to select, select this index"""
         key = key_sequence[0]
 
         # return if key is not a number
         if not key.isnumeric():
             return
 
         id = int(key)
```

### Comparing `ItsPrompt-1.3/ItsPrompt/prompts/select.py` & `ItsPrompt-1.4/ItsPrompt/prompts/select.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from prompt_toolkit import HTML, Application
+from prompt_toolkit import Application, HTML
 from prompt_toolkit.layout.controls import FormattedTextControl
 
 from ..data.select import process_data
 
 
 class SelectPrompt(Application):
 
@@ -13,16 +13,15 @@
         default: str | None = None,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
         # get prompt content box
-        self.prompt_content: FormattedTextControl = self.layout.container.get_children(
-        )[0].content  # type: ignore
+        self.prompt_content: FormattedTextControl = self.layout.container.get_children()[0].content  # type: ignore
 
         # save question
         self.question = question
 
         # process options
         self.options = process_data(options)
 
@@ -35,40 +34,40 @@
             if option.id == default:
                 self.selection = i
                 break
         else:
             raise ValueError('Default value is not a valid id.')
 
     def update(self):
-        '''update prompt content'''
+        """update prompt content"""
         content = f'[<question_mark>?</question_mark>] <question>{self.question}</question>:'
 
         for i, option in enumerate(self.options):
             if i == self.selection:
                 content += f'\n<selected_option>  > {option.name}</selected_option>'
             else:
                 content += f'\n<option>    {option.name}</option>'
 
         self.prompt_content.text = HTML(content)
 
     def prompt(self) -> str | None:
-        '''start the application, returns the return value'''
+        """start the application, returns the return value"""
         self.update()
         out: str | None = self.run()
 
         return out
 
     def on_up(self):
-        '''when up is pressed, the previous indexed option will be selected'''
+        """when up is pressed, the previous indexed option will be selected"""
         self.selection = (self.selection - 1) % len(self.options)
 
         self.update()
 
     def on_down(self):
-        '''when down is pressed, the next indexed option will be selected'''
+        """when down is pressed, the next indexed option will be selected"""
         self.selection = (self.selection + 1) % len(self.options)
 
         self.update()
 
     def on_enter(self):
         # get selected id
         self.exit(result=self.options[self.selection].id)
```

### Comparing `ItsPrompt-1.3/ItsPrompt/prompts/table.py` & `ItsPrompt-1.4/ItsPrompt/prompts/table.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,97 @@
 import html
+from typing import TYPE_CHECKING, Union
 
-from pandas import DataFrame
-from prompt_toolkit import HTML, Application
+from prompt_toolkit import Application, HTML
 from prompt_toolkit.data_structures import Point
 from prompt_toolkit.layout.controls import FormattedTextControl
 
 from ..data.table import Table
 
+if TYPE_CHECKING:  # pragma: no cover
+    from pandas import DataFrame
+
 
 class TablePrompt(Application):
 
     def __init__(
         self,
         question: str,
-        data: DataFrame,
+        data: Union["DataFrame", dict[str, list[str]]],
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
         # get prompt content box
-        self.prompt_content: FormattedTextControl = self.layout.container.get_children(
-        )[0].content  # type: ignore
+        self.prompt_content: FormattedTextControl = self.layout.container.get_children()[0].content  # type: ignore
 
         # save question
         self.question = question
 
         # process data
         self.table = Table(data)
 
         # set cursor
         self.prompt_content.get_cursor_position = lambda: Point(
             self.table.get_current_cursor_position()[0],
-            self.table.get_current_cursor_position()[1] +
-            1,  # add 1 offset for height of question
+            self.table.get_current_cursor_position()[1] + 1,  # add 1 offset for height of question
         )
 
     def update(self):
-        '''update prompt content'''
+        """update prompt content"""
         content = f'[<question_mark>?</question_mark>] <question>{self.question}</question>:\n'
 
         # append table
         content += html.escape(
             self.table.get_table_as_str()
-        )  # escaping is needed so formatting from PromptToolkit wont destroy the whole table
+        )  # escaping is needed so formatting from PromptToolkit won't destroy the whole table
 
         self.prompt_content.text = HTML(content)
 
-    def prompt(self) -> DataFrame | None:
-        '''start the application, returns the return value'''
+    def prompt(self) -> Union["DataFrame", dict[str, list[str]], None]:
+        """start the application, returns the return value"""
         self.update()
-        out: DataFrame | None = self.run()
+        out: Union["DataFrame", dict[str, list[str]], None] = self.run()
 
         return out
 
     def on_up(self):
-        '''when up is pressed, the cell one above will be selected'''
+        """when up is pressed, the cell one above will be selected"""
         self.table.on_up()
 
         self.update()
 
     def on_down(self):
-        '''when down is pressed, the cell one below will be selected'''
+        """when down is pressed, the cell one below will be selected"""
         self.table.on_down()
 
         self.update()
 
     def on_left(self):
-        '''when left is pressed, the cell one to the left will be selected'''
+        """when left is pressed, the cell one to the left will be selected"""
         self.table.on_left()
 
         self.update()
 
     def on_right(self):
-        '''when left is pressed, the cell one to the right will be selected'''
+        """when left is pressed, the cell one to the right will be selected"""
         self.table.on_right()
 
         self.update()
 
     def on_key(self, key_sequence: list[str]):
-        '''when a key is pressed, the key will be added to the current cells content'''
+        """when a key is pressed, the key will be added to the current cells content"""
         key = key_sequence[0]
         self.table.add_key(key)
 
         self.update()
 
     def on_backspace(self):
-        '''when backspace is pressed, the last char will be removed from the current cells content'''
+        """when backspace is pressed, the last char will be removed from the current cells content"""
         self.table.del_key()
 
         self.update()
 
     def on_enter(self):
         # return the modified table
-        self.exit(result=self.table.data)
+        self.exit(result=self.table.data.get_data())
```

### Comparing `ItsPrompt-1.3/ItsPrompt.egg-info/PKG-INFO` & `ItsPrompt-1.4/ItsPrompt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ItsPrompt
-Version: 1.3
+Version: 1.4
 Summary: Prompting - the fancy way
 Author: ItsNameless
 License: MIT License
         
         Copyright (c) 2023-present ItsNameless
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,59 +47,66 @@
 
 ![Demonstration](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/ItsPrompt.gif)
 
 # ItsPrompt
 
 Do you ever feel the need to ask a user of your code for an input?
 
-Using `input()` is easy, but is it great? 
+Using `input()` is easy, but is it great?
 
 Do you want to give the user a selection list, a yes-or-no question, or maybe a multiline input field?
 
 And do you think all of this should be done easily, without caring to much how it all works?
 
 Then you are right here! **ItsPrompt** gives you the ability to ask the user for input, the *fancy* way.
 
-**ItsPrompt** tries to be an easy-to-use module for managing prompts for the user. You task is to create a great program, not how to ask the user for input. That is why **ItsPrompt** is there to take care of this problem, so you can focus on the important things!
+**ItsPrompt** tries to be an easy-to-use module for managing prompts for the user. You task is to create a great
+program, not how to ask the user for input. That is why **ItsPrompt** is there to take care of this problem, so you can
+focus on the important things!
 
 # TOC
 
 - [ItsPrompt](#itsprompt)
 - [TOC](#toc)
     - [A small, thankful note](#a-small-thankful-note)
-  - [Features](#features)
-  - [Installation](#installation)
-  - [Usage](#usage)
-  - [Prompt types](#prompt-types)
-    - [`select`](#select)
-    - [`raw_select`](#raw_select)
-    - [`expand`](#expand)
-    - [`checkbox`](#checkbox)
-    - [`confirm`](#confirm)
-    - [`input`](#input)
-    - [`table`](#table)
-  - [Additional Features and Tips](#additional-features-and-tips)
-    - [Options](#options)
-    - [Data](#data)
-    - [Styling](#styling)
-    - [Prompt Validation](#prompt-validation)
-    - [Prompt Completion](#prompt-completion)
-    - [Further Information](#further-information)
+    - [Features](#features)
+    - [Installation](#installation)
+    - [Usage](#usage)
+    - [Prompt types](#prompt-types)
+        - [`select`](#select)
+        - [`raw_select`](#raw_select)
+        - [`expand`](#expand)
+        - [`checkbox`](#checkbox)
+        - [`confirm`](#confirm)
+        - [`input`](#input)
+        - [`table`](#table)
+    - [Additional Features and Tips](#additional-features-and-tips)
+        - [Options](#options)
+        - [Data](#data)
+        - [Styling](#styling)
+        - [Prompt Validation](#prompt-validation)
+        - [Prompt Completion](#prompt-completion)
+        - [Further Information](#further-information)
 
 ---
 
 ### A small, thankful note
 
-This project is not the first to accomplish the above mentioned tasks. There is another package, `PyInquirer`, which inspired me to build **ItsPrompt**.
+This project is not the first to accomplish the above mentioned tasks. There is another package, `PyInquirer`, which
+inspired me to build **ItsPrompt**.
 
-On my way to create a small program I came to a point were I needed a simple GUI, and I tried `PyInquirer`. Unfortunately, at the current time it is not actively maintained and a bit outdated. I thought of updating it, but then I thought "*Isn't it easier to just create my own version?*" - And so I did!
+On my way to create a small program I came to a point were I needed a simple GUI, and I tried `PyInquirer`.
+Unfortunately, at the current time it is not actively maintained and a bit outdated. I thought of updating it, but then
+I thought "*Isn't it easier to just create my own version?*" - And so I did!
 
-**ItsPrompt** is not a copy or a fork of `PyInquirer`. I built this module from the ground up, without ever looking deep into the source code of `PyInquirer`.
+**ItsPrompt** is not a copy or a fork of `PyInquirer`. I built this module from the ground up, without ever looking deep
+into the source code of `PyInquirer`.
 
-On my way to build this package, I learned a lot about `prompt-toolkit`, and all of this just because of `PyInquirer`! Thanks!
+On my way to build this package, I learned a lot about `prompt-toolkit`, and all of this just because of `PyInquirer`!
+Thanks!
 
 ---
 
 ## Features
 
 - many prompt types (more details below):
     - select
@@ -120,14 +127,20 @@
 
 This package is hosted on pypi, so the installation is as simple as it can get:
 
 ```
 python3 -m pip install ItsPrompt
 ```
 
+This will install `ItsPrompt` without pandas. If you want to use `TablePrompt` (see [table](#table)) with
+`pandas.DataFrame`, you can install pandas support either by:
+
+- installing pandas separately
+- install `ItsPrompt` via `pip install ItsPrompt[df]`
+
 ---
 
 ## Usage
 
 Import the `Prompt` class:
 
 ```py
@@ -160,15 +173,14 @@
     default='option1',
     style=my_style,
 )
 ```
 
 *additional information on the function arguments can be found in the docstring*
 
-
 ### `raw_select`
 
 ![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/raw_select.png)
 
 ```py
 Prompt.raw_select(
     question='question',
@@ -233,76 +245,91 @@
 ![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/input.png)
 
 ```py
 Prompt.input(
     question='question',
     default='something',
     multiline=False,
-    show_symbol='*', # not compatible with complete, completer
+    show_symbol='*',  # not compatible with complete, completer
     validate=validation_function,
-    complete=['completion1', 'completion2'], # either use complete
-    completer=my_completer,                  # or completer
+    complete=['completion1', 'completion2'],  # either use complete
+    completer=my_completer,  # or completer
     completion_show_multicolumn=True,
     style=my_style,
 )
 ```
 
 *additional information on the function arguments can be found in the docstring*
 
 ### `table`
 
 ![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/table.png)
 
 ```py
 Prompt.table(
+    question="something",
+    data={"0": ["something"]},
+    style=my_style,
+)
+
+# or, after having installed pandas
+
+Prompt.table(
     question='something',
     data=DataFrame(['something']),
     style=my_style,
 )
 ```
 
 *additional information on the function arguments can be found in the docstring*
 
 ---
 
 ## Additional Features and Tips
 
 ### Options
 
-The `options` is always a `tuple` containing `str` and `tuple` objects. 
+The `options` is always a `tuple` containing `str` and `tuple` objects.
 
-If an option is given as a `str`, this will be used as the options display name and the id, which will be returned when selecting this option.
+If an option is given as a `str`, this will be used as the options display name and the id, which will be returned when
+selecting this option.
 
 *In case of `expand`, the first character of the `str` will be used as its key.*
 
 If an option is given as a `tuple`, the first value will be the options name, the second value the options id to return.
 
 *In case of `expand`, the first value will be the key, the second value the name and the third value the id.*
 
 ---
 
 ### Data
 
 The `table` prompt takes a mandatory `data` argument, which needs to be a `pandas.DataFrame`.
 
-This `DataFrame` is used as the content of the table. The user may change the fields of the table. The output of the `table` prompt is a `pandas.DataFrame` with the user given values.
+This `DataFrame` is used as the content of the table. The user may change the fields of the table. The output of
+the `table` prompt is a `pandas.DataFrame` with the user given values.
 
-Currently, the output will convert all input values to a `str`, so `int`, `bool`, ... will be converted to strings. This is a current limitation of the way the table is displayed, but may later be updated.
+Currently, the output will convert all input values to a `str`, so `int`, `bool`, ... will be converted to strings. This
+is a current limitation of the way the table is displayed, but may later be updated.
 
-Another limitation of the `table` prompt is the use of styling in the `DataFrame` fields. All styling tags will be displayed as-is, so a `<u>...</u>` will not be underlined, but rather displayed as its shown.
+Another limitation of the `table` prompt is the use of styling in the `DataFrame` fields. All styling tags will be
+displayed as-is, so a `<u>...</u>` will not be underlined, but rather displayed as its shown.
 
 ---
 
 ### Styling
 
-**ItsPrompt** uses `prompt-toolkit` for its prompts. This module not only provides an easy way to interact with the command line, but also a full set of styling features.
+**ItsPrompt** uses `prompt-toolkit` for its prompts. This module not only provides an easy way to interact with the
+command line, but also a full set of styling features.
 
-You can learn more about the available styling features in the documentation of `prompt-toolkit`: [Styling](https://python-prompt-toolkit.readthedocs.io/en/master/pages/printing_text.html#formatted-text).
+You can learn more about the available styling features in the documentation
+of `prompt-toolkit`: [Styling](https://python-prompt-toolkit.readthedocs.io/en/master/pages/printing_text.html#formatted-text).
 
-**ItsPrompt** makes it a bit easier for you to style each component of a prompt. For every component, we give a separate attribute in the `PromptStyle` class, which you can style with valid `prompt-toolkit` styling:
+**ItsPrompt** makes it a bit easier for you to style each component of a prompt. For every component, we give a separate
+attribute in the `PromptStyle` class, which you can style with valid `prompt-toolkit` styling:
 
 ```py
 # examples for the different styling class components
 Prompt.raw_select(
     question='question',
     options=(
         'option',
@@ -317,28 +344,27 @@
 )
 ```
 
 ![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/styling_raw_select_annotated.png)
 
 ![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/styling_input_annotated.png)
 
-| ID  |    styling tag    |             default style             |
-| --- | ----------------- | ------------------------------------- |
-| 1   | `question_mark`   | `fg:ansigreen`                        |
-| 2   | `question`        | *                                     |
-| 3   | `option`          | *                                     |
-| 4   | `selected_option` | `fg:ansicyan`                         |
-| 5   | `tooltip`         | `fg:ansibrightblue bg:ansiwhite bold` |
-| 6   | `text`            | *                                     |
-| 7   | `grayout`          | `fg:ansibrightblack`                  |
-| 8   | `error`           | `fg:ansiwhite bg:ansired bold`        |
+| ID | styling tag       | default style                         |
+|----|-------------------|---------------------------------------|
+| 1  | `question_mark`   | `fg:ansigreen`                        |
+| 2  | `question`        | *                                     |
+| 3  | `option`          | *                                     |
+| 4  | `selected_option` | `fg:ansicyan`                         |
+| 5  | `tooltip`         | `fg:ansibrightblue bg:ansiwhite bold` |
+| 6  | `text`            | *                                     |
+| 7  | `grayout`         | `fg:ansibrightblack`                  |
+| 8  | `error`           | `fg:ansiwhite bg:ansired bold`        |
 
 *\*These values are not changed from the default `prompt-toolkit` values.*
 
-
 To create your own style, there are two ways:
 
 ***Changing the default style***
 
 To change the default style, you need to import the `default_style` and change its values:
 
 ```py
@@ -347,151 +373,165 @@
 default_style.error = 'fg:ansired bg:ansiwhite'
 ```
 
 This will automatically change the style of all prompts, which do not have an own style defined.
 
 ***Creating your own style***
 
-To define your own style for a specific prompt, import `PromptStyle` and create an object. Then assign it to the `style` argument of a prompt.
+To define your own style for a specific prompt, import `PromptStyle` and create an object. Then assign it to the `style`
+argument of a prompt.
 
 ```py
 from ItsPrompt.data.style import PromptStyle
 
 my_style = PromptStyle(
     question_mark='fg:ansiblue',
     error='fg:ansired bg:ansiwhite',
 )
 ```
 
-All styles which are not given, **will not** be the same as the default style. Instead they will use the styling given by `prompt-toolkit`. If you want to change our default styles, then copy the `default_style` and change your values, instead of directly creating your own style:
+All styles which are not given, **will not** be the same as the default style. Instead they will use the styling given
+by `prompt-toolkit`. If you want to change our default styles, then copy the `default_style` and change your values,
+instead of directly creating your own style:
 
 ```py
 from ItsPrompt.data.style import create_from_default
 
 my_style = create_from_default()
 
 my_style.error = 'fg:ansired bg:ansiwhite'
 ```
 
-> Warning! Not copying the default style and changing it instead will result in all prompts using your changes, as a variable is by default not a copy, but a reference to the same object!
+> Warning! Not copying the default style and changing it instead will result in all prompts using your changes, as a
+> variable is by default not a copy, but a reference to the same object!
 
 ---
 
 ### Prompt Validation
 
-The `input` allows you to validate the input before submitting it. For every character the user types, the validation will be run and a friendly error will be shown in the toolbar.
+The `input` allows you to validate the input before submitting it. For every character the user types, the validation
+will be run and a friendly error will be shown in the toolbar.
 
-To use the validation feature, create a function which takes a `str` as an argument and returns either a `str` or `None`.
+To use the validation feature, create a function which takes a `str` as an argument and returns either a `str`
+or `None`.
 
 ```py
 def input_not_empty(input: str) -> str | None:
     if len(input) == 0:
         return 'Address can not be empty!'
 
+
 Prompt.input(
     ...
-    validate=input_not_empty,
-    ...
+validate = input_not_empty,
+...
 )
 ```
 
 The `str` argument will be the current user input, which can then be checked, but not changed!
 
 If you want to show that the validation succeeded, return `None` (or nothing). This will not trigger any errors.
 
-If you want to show an error, return a `str` with the errors text. Your text will be shown in the toolbar. As long as the validation returns a `str`, the user may not submit the input.
+If you want to show an error, return a `str` with the errors text. Your text will be shown in the toolbar. As long as
+the validation returns a `str`, the user may not submit the input.
 
 ---
 
 ### Prompt Completion
 
-The `input` prompt type supports auto completion as well. 
+The `input` prompt type supports auto completion as well.
 
 > If you use a completer, you are unable to use `show_symbol`!
 
 To give auto completion options, there are three ways:
 
 ***Creating a simple list of possible completions***
 
 `Input` takes a `list[str]` to use as simple word completions. Each `str` in the list is a possible value to complete.
 
 ```py
 prompt.input(
     ...
-    completions=['Mainstreet 4', 'Fifth way'],
-    ...
+completions = ['Mainstreet 4', 'Fifth way'],
+...
 )
 ```
 
 ***Creating a nested dictionary of possible completions***
 
-You can use a dictionary for nested completions. Each "layer" will be a completion, after the first was accepted. For example:
+You can use a dictionary for nested completions. Each "layer" will be a completion, after the first was accepted. For
+example:
 
 ```py
 completions = {
-    '1' : {
-        '1.1' : None,
-        '1.2' : {
+    '1': {
+        '1.1': None,
+        '1.2': {
             '1.2.1', '1.2.2'
         }
     },
-    '2' : {
-        '2.1' : { '2.1.1' }
+    '2': {
+        '2.1': {'2.1.1'}
     }
 }
 
 prompt.input(
     ...
-    completions=completions,
-    ...
+completions = completions,
+...
 )
 ```
 
-The key of each entry is the completion that will be shown. The key is either None if there are no further completions or a new dict, where the key is the completion and the value is the next "layer", and so on...
+The key of each entry is the completion that will be shown. The key is either None if there are no further completions
+or a new dict, where the key is the completion and the value is the next "layer", and so on...
 
 > For more information, the type signature of `CompletionDict` is:  
 > `dict[str, "CompletionDict | None"]`
 
 ***Using a given Completer by `prompt-toolkit` or creating your own***
 
 In the background your completions will be mapped to a `Completer`, provided by `prompt-toolkit`.
 
-If you need more customization, you can use a `Completer` given by `prompt-toolkit` or create your own completer. For more information on this process, read here: [Completions in prompt-toolkit](https://python-prompt-toolkit.readthedocs.io/en/stable/pages/asking_for_input.html#autocompletion).
+If you need more customization, you can use a `Completer` given by `prompt-toolkit` or create your own completer. For
+more information on this process, read
+here: [Completions in prompt-toolkit](https://python-prompt-toolkit.readthedocs.io/en/stable/pages/asking_for_input.html#autocompletion).
 
 There are a number of completers available, for example:
 
 - `PathCompleter`
     - automatically complete file system paths
 - `ExecutableCompleter`
     - automatically complete executables in file system
 - `WordCompleter`
-    - As simple as it can get. Just completes the letters of the word, that are actually present (the `FuzzyCompleter` which `completions` uses in background completes based on a probability, and may show matches which are not exact).
+    - As simple as it can get. Just completes the letters of the word, that are actually present (the `FuzzyCompleter`
+      which `completions` uses in background completes based on a probability, and may show matches which are not
+      exact).
 - ...
 
-
 To add your own completer to an input field, you can use the `completer` argument:
 
 ```py
 prompt.input(
     ...
-    completer=my_completer,
-    ...
+completer = my_completer,
+...
 )
 ```
 
 > `completions` and `completer` are **mutually exclusive**! You may not use both!
 
 ---
 
 ### Further Information
 
 If you need some easy examples, refer to [example.py](example.py)!
 
 If you want to contribute, check out the projects repository: [ItsPrompt](https://github.com/TheItsProjects/ItsPrompt)!
 
 If you got any other questions, or want to give an idea on how to improve **ItsPrompt**:
+
 - visit our discussions: [ItsPrompt Discussions](https://github.com/TheItsProjects/ItsPrompt/discussions)!
 - join our discord: [TheItsProjects](https://discord.gg/rP9Qke2jDs)!
 
 ---
 
 Puh, that was so much to read... But now, lets have fun with **ItsPrompt**!
```

### Comparing `ItsPrompt-1.3/ItsPrompt.egg-info/SOURCES.txt` & `ItsPrompt-1.4/ItsPrompt.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 ItsPrompt/data/__init__.py
 ItsPrompt/data/checkbox.py
 ItsPrompt/data/expand.py
 ItsPrompt/data/select.py
 ItsPrompt/data/style.py
 ItsPrompt/data/table.py
 ItsPrompt/data/type.py
+ItsPrompt/objects/table/table_base.py
+ItsPrompt/objects/table/table_df.py
+ItsPrompt/objects/table/table_dict.py
 ItsPrompt/prompts/__init__.py
 ItsPrompt/prompts/checkbox.py
 ItsPrompt/prompts/confirm.py
 ItsPrompt/prompts/expand.py
 ItsPrompt/prompts/input.py
 ItsPrompt/prompts/raw_select.py
 ItsPrompt/prompts/select.py
```

### Comparing `ItsPrompt-1.3/LICENSE` & `ItsPrompt-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.3/PKG-INFO` & `ItsPrompt-1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ItsPrompt
-Version: 1.3
+Version: 1.4
 Summary: Prompting - the fancy way
 Author: ItsNameless
 License: MIT License
         
         Copyright (c) 2023-present ItsNameless
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -47,59 +47,66 @@
 
 ![Demonstration](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/ItsPrompt.gif)
 
 # ItsPrompt
 
 Do you ever feel the need to ask a user of your code for an input?
 
-Using `input()` is easy, but is it great? 
+Using `input()` is easy, but is it great?
 
 Do you want to give the user a selection list, a yes-or-no question, or maybe a multiline input field?
 
 And do you think all of this should be done easily, without caring to much how it all works?
 
 Then you are right here! **ItsPrompt** gives you the ability to ask the user for input, the *fancy* way.
 
-**ItsPrompt** tries to be an easy-to-use module for managing prompts for the user. You task is to create a great program, not how to ask the user for input. That is why **ItsPrompt** is there to take care of this problem, so you can focus on the important things!
+**ItsPrompt** tries to be an easy-to-use module for managing prompts for the user. You task is to create a great
+program, not how to ask the user for input. That is why **ItsPrompt** is there to take care of this problem, so you can
+focus on the important things!
 
 # TOC
 
 - [ItsPrompt](#itsprompt)
 - [TOC](#toc)
     - [A small, thankful note](#a-small-thankful-note)
-  - [Features](#features)
-  - [Installation](#installation)
-  - [Usage](#usage)
-  - [Prompt types](#prompt-types)
-    - [`select`](#select)
-    - [`raw_select`](#raw_select)
-    - [`expand`](#expand)
-    - [`checkbox`](#checkbox)
-    - [`confirm`](#confirm)
-    - [`input`](#input)
-    - [`table`](#table)
-  - [Additional Features and Tips](#additional-features-and-tips)
-    - [Options](#options)
-    - [Data](#data)
-    - [Styling](#styling)
-    - [Prompt Validation](#prompt-validation)
-    - [Prompt Completion](#prompt-completion)
-    - [Further Information](#further-information)
+    - [Features](#features)
+    - [Installation](#installation)
+    - [Usage](#usage)
+    - [Prompt types](#prompt-types)
+        - [`select`](#select)
+        - [`raw_select`](#raw_select)
+        - [`expand`](#expand)
+        - [`checkbox`](#checkbox)
+        - [`confirm`](#confirm)
+        - [`input`](#input)
+        - [`table`](#table)
+    - [Additional Features and Tips](#additional-features-and-tips)
+        - [Options](#options)
+        - [Data](#data)
+        - [Styling](#styling)
+        - [Prompt Validation](#prompt-validation)
+        - [Prompt Completion](#prompt-completion)
+        - [Further Information](#further-information)
 
 ---
 
 ### A small, thankful note
 
-This project is not the first to accomplish the above mentioned tasks. There is another package, `PyInquirer`, which inspired me to build **ItsPrompt**.
+This project is not the first to accomplish the above mentioned tasks. There is another package, `PyInquirer`, which
+inspired me to build **ItsPrompt**.
 
-On my way to create a small program I came to a point were I needed a simple GUI, and I tried `PyInquirer`. Unfortunately, at the current time it is not actively maintained and a bit outdated. I thought of updating it, but then I thought "*Isn't it easier to just create my own version?*" - And so I did!
+On my way to create a small program I came to a point were I needed a simple GUI, and I tried `PyInquirer`.
+Unfortunately, at the current time it is not actively maintained and a bit outdated. I thought of updating it, but then
+I thought "*Isn't it easier to just create my own version?*" - And so I did!
 
-**ItsPrompt** is not a copy or a fork of `PyInquirer`. I built this module from the ground up, without ever looking deep into the source code of `PyInquirer`.
+**ItsPrompt** is not a copy or a fork of `PyInquirer`. I built this module from the ground up, without ever looking deep
+into the source code of `PyInquirer`.
 
-On my way to build this package, I learned a lot about `prompt-toolkit`, and all of this just because of `PyInquirer`! Thanks!
+On my way to build this package, I learned a lot about `prompt-toolkit`, and all of this just because of `PyInquirer`!
+Thanks!
 
 ---
 
 ## Features
 
 - many prompt types (more details below):
     - select
@@ -120,14 +127,20 @@
 
 This package is hosted on pypi, so the installation is as simple as it can get:
 
 ```
 python3 -m pip install ItsPrompt
 ```
 
+This will install `ItsPrompt` without pandas. If you want to use `TablePrompt` (see [table](#table)) with
+`pandas.DataFrame`, you can install pandas support either by:
+
+- installing pandas separately
+- install `ItsPrompt` via `pip install ItsPrompt[df]`
+
 ---
 
 ## Usage
 
 Import the `Prompt` class:
 
 ```py
@@ -160,15 +173,14 @@
     default='option1',
     style=my_style,
 )
 ```
 
 *additional information on the function arguments can be found in the docstring*
 
-
 ### `raw_select`
 
 ![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/raw_select.png)
 
 ```py
 Prompt.raw_select(
     question='question',
@@ -233,76 +245,91 @@
 ![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/input.png)
 
 ```py
 Prompt.input(
     question='question',
     default='something',
     multiline=False,
-    show_symbol='*', # not compatible with complete, completer
+    show_symbol='*',  # not compatible with complete, completer
     validate=validation_function,
-    complete=['completion1', 'completion2'], # either use complete
-    completer=my_completer,                  # or completer
+    complete=['completion1', 'completion2'],  # either use complete
+    completer=my_completer,  # or completer
     completion_show_multicolumn=True,
     style=my_style,
 )
 ```
 
 *additional information on the function arguments can be found in the docstring*
 
 ### `table`
 
 ![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/table.png)
 
 ```py
 Prompt.table(
+    question="something",
+    data={"0": ["something"]},
+    style=my_style,
+)
+
+# or, after having installed pandas
+
+Prompt.table(
     question='something',
     data=DataFrame(['something']),
     style=my_style,
 )
 ```
 
 *additional information on the function arguments can be found in the docstring*
 
 ---
 
 ## Additional Features and Tips
 
 ### Options
 
-The `options` is always a `tuple` containing `str` and `tuple` objects. 
+The `options` is always a `tuple` containing `str` and `tuple` objects.
 
-If an option is given as a `str`, this will be used as the options display name and the id, which will be returned when selecting this option.
+If an option is given as a `str`, this will be used as the options display name and the id, which will be returned when
+selecting this option.
 
 *In case of `expand`, the first character of the `str` will be used as its key.*
 
 If an option is given as a `tuple`, the first value will be the options name, the second value the options id to return.
 
 *In case of `expand`, the first value will be the key, the second value the name and the third value the id.*
 
 ---
 
 ### Data
 
 The `table` prompt takes a mandatory `data` argument, which needs to be a `pandas.DataFrame`.
 
-This `DataFrame` is used as the content of the table. The user may change the fields of the table. The output of the `table` prompt is a `pandas.DataFrame` with the user given values.
+This `DataFrame` is used as the content of the table. The user may change the fields of the table. The output of
+the `table` prompt is a `pandas.DataFrame` with the user given values.
 
-Currently, the output will convert all input values to a `str`, so `int`, `bool`, ... will be converted to strings. This is a current limitation of the way the table is displayed, but may later be updated.
+Currently, the output will convert all input values to a `str`, so `int`, `bool`, ... will be converted to strings. This
+is a current limitation of the way the table is displayed, but may later be updated.
 
-Another limitation of the `table` prompt is the use of styling in the `DataFrame` fields. All styling tags will be displayed as-is, so a `<u>...</u>` will not be underlined, but rather displayed as its shown.
+Another limitation of the `table` prompt is the use of styling in the `DataFrame` fields. All styling tags will be
+displayed as-is, so a `<u>...</u>` will not be underlined, but rather displayed as its shown.
 
 ---
 
 ### Styling
 
-**ItsPrompt** uses `prompt-toolkit` for its prompts. This module not only provides an easy way to interact with the command line, but also a full set of styling features.
+**ItsPrompt** uses `prompt-toolkit` for its prompts. This module not only provides an easy way to interact with the
+command line, but also a full set of styling features.
 
-You can learn more about the available styling features in the documentation of `prompt-toolkit`: [Styling](https://python-prompt-toolkit.readthedocs.io/en/master/pages/printing_text.html#formatted-text).
+You can learn more about the available styling features in the documentation
+of `prompt-toolkit`: [Styling](https://python-prompt-toolkit.readthedocs.io/en/master/pages/printing_text.html#formatted-text).
 
-**ItsPrompt** makes it a bit easier for you to style each component of a prompt. For every component, we give a separate attribute in the `PromptStyle` class, which you can style with valid `prompt-toolkit` styling:
+**ItsPrompt** makes it a bit easier for you to style each component of a prompt. For every component, we give a separate
+attribute in the `PromptStyle` class, which you can style with valid `prompt-toolkit` styling:
 
 ```py
 # examples for the different styling class components
 Prompt.raw_select(
     question='question',
     options=(
         'option',
@@ -317,28 +344,27 @@
 )
 ```
 
 ![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/styling_raw_select_annotated.png)
 
 ![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/styling_input_annotated.png)
 
-| ID  |    styling tag    |             default style             |
-| --- | ----------------- | ------------------------------------- |
-| 1   | `question_mark`   | `fg:ansigreen`                        |
-| 2   | `question`        | *                                     |
-| 3   | `option`          | *                                     |
-| 4   | `selected_option` | `fg:ansicyan`                         |
-| 5   | `tooltip`         | `fg:ansibrightblue bg:ansiwhite bold` |
-| 6   | `text`            | *                                     |
-| 7   | `grayout`          | `fg:ansibrightblack`                  |
-| 8   | `error`           | `fg:ansiwhite bg:ansired bold`        |
+| ID | styling tag       | default style                         |
+|----|-------------------|---------------------------------------|
+| 1  | `question_mark`   | `fg:ansigreen`                        |
+| 2  | `question`        | *                                     |
+| 3  | `option`          | *                                     |
+| 4  | `selected_option` | `fg:ansicyan`                         |
+| 5  | `tooltip`         | `fg:ansibrightblue bg:ansiwhite bold` |
+| 6  | `text`            | *                                     |
+| 7  | `grayout`         | `fg:ansibrightblack`                  |
+| 8  | `error`           | `fg:ansiwhite bg:ansired bold`        |
 
 *\*These values are not changed from the default `prompt-toolkit` values.*
 
-
 To create your own style, there are two ways:
 
 ***Changing the default style***
 
 To change the default style, you need to import the `default_style` and change its values:
 
 ```py
@@ -347,151 +373,165 @@
 default_style.error = 'fg:ansired bg:ansiwhite'
 ```
 
 This will automatically change the style of all prompts, which do not have an own style defined.
 
 ***Creating your own style***
 
-To define your own style for a specific prompt, import `PromptStyle` and create an object. Then assign it to the `style` argument of a prompt.
+To define your own style for a specific prompt, import `PromptStyle` and create an object. Then assign it to the `style`
+argument of a prompt.
 
 ```py
 from ItsPrompt.data.style import PromptStyle
 
 my_style = PromptStyle(
     question_mark='fg:ansiblue',
     error='fg:ansired bg:ansiwhite',
 )
 ```
 
-All styles which are not given, **will not** be the same as the default style. Instead they will use the styling given by `prompt-toolkit`. If you want to change our default styles, then copy the `default_style` and change your values, instead of directly creating your own style:
+All styles which are not given, **will not** be the same as the default style. Instead they will use the styling given
+by `prompt-toolkit`. If you want to change our default styles, then copy the `default_style` and change your values,
+instead of directly creating your own style:
 
 ```py
 from ItsPrompt.data.style import create_from_default
 
 my_style = create_from_default()
 
 my_style.error = 'fg:ansired bg:ansiwhite'
 ```
 
-> Warning! Not copying the default style and changing it instead will result in all prompts using your changes, as a variable is by default not a copy, but a reference to the same object!
+> Warning! Not copying the default style and changing it instead will result in all prompts using your changes, as a
+> variable is by default not a copy, but a reference to the same object!
 
 ---
 
 ### Prompt Validation
 
-The `input` allows you to validate the input before submitting it. For every character the user types, the validation will be run and a friendly error will be shown in the toolbar.
+The `input` allows you to validate the input before submitting it. For every character the user types, the validation
+will be run and a friendly error will be shown in the toolbar.
 
-To use the validation feature, create a function which takes a `str` as an argument and returns either a `str` or `None`.
+To use the validation feature, create a function which takes a `str` as an argument and returns either a `str`
+or `None`.
 
 ```py
 def input_not_empty(input: str) -> str | None:
     if len(input) == 0:
         return 'Address can not be empty!'
 
+
 Prompt.input(
     ...
-    validate=input_not_empty,
-    ...
+validate = input_not_empty,
+...
 )
 ```
 
 The `str` argument will be the current user input, which can then be checked, but not changed!
 
 If you want to show that the validation succeeded, return `None` (or nothing). This will not trigger any errors.
 
-If you want to show an error, return a `str` with the errors text. Your text will be shown in the toolbar. As long as the validation returns a `str`, the user may not submit the input.
+If you want to show an error, return a `str` with the errors text. Your text will be shown in the toolbar. As long as
+the validation returns a `str`, the user may not submit the input.
 
 ---
 
 ### Prompt Completion
 
-The `input` prompt type supports auto completion as well. 
+The `input` prompt type supports auto completion as well.
 
 > If you use a completer, you are unable to use `show_symbol`!
 
 To give auto completion options, there are three ways:
 
 ***Creating a simple list of possible completions***
 
 `Input` takes a `list[str]` to use as simple word completions. Each `str` in the list is a possible value to complete.
 
 ```py
 prompt.input(
     ...
-    completions=['Mainstreet 4', 'Fifth way'],
-    ...
+completions = ['Mainstreet 4', 'Fifth way'],
+...
 )
 ```
 
 ***Creating a nested dictionary of possible completions***
 
-You can use a dictionary for nested completions. Each "layer" will be a completion, after the first was accepted. For example:
+You can use a dictionary for nested completions. Each "layer" will be a completion, after the first was accepted. For
+example:
 
 ```py
 completions = {
-    '1' : {
-        '1.1' : None,
-        '1.2' : {
+    '1': {
+        '1.1': None,
+        '1.2': {
             '1.2.1', '1.2.2'
         }
     },
-    '2' : {
-        '2.1' : { '2.1.1' }
+    '2': {
+        '2.1': {'2.1.1'}
     }
 }
 
 prompt.input(
     ...
-    completions=completions,
-    ...
+completions = completions,
+...
 )
 ```
 
-The key of each entry is the completion that will be shown. The key is either None if there are no further completions or a new dict, where the key is the completion and the value is the next "layer", and so on...
+The key of each entry is the completion that will be shown. The key is either None if there are no further completions
+or a new dict, where the key is the completion and the value is the next "layer", and so on...
 
 > For more information, the type signature of `CompletionDict` is:  
 > `dict[str, "CompletionDict | None"]`
 
 ***Using a given Completer by `prompt-toolkit` or creating your own***
 
 In the background your completions will be mapped to a `Completer`, provided by `prompt-toolkit`.
 
-If you need more customization, you can use a `Completer` given by `prompt-toolkit` or create your own completer. For more information on this process, read here: [Completions in prompt-toolkit](https://python-prompt-toolkit.readthedocs.io/en/stable/pages/asking_for_input.html#autocompletion).
+If you need more customization, you can use a `Completer` given by `prompt-toolkit` or create your own completer. For
+more information on this process, read
+here: [Completions in prompt-toolkit](https://python-prompt-toolkit.readthedocs.io/en/stable/pages/asking_for_input.html#autocompletion).
 
 There are a number of completers available, for example:
 
 - `PathCompleter`
     - automatically complete file system paths
 - `ExecutableCompleter`
     - automatically complete executables in file system
 - `WordCompleter`
-    - As simple as it can get. Just completes the letters of the word, that are actually present (the `FuzzyCompleter` which `completions` uses in background completes based on a probability, and may show matches which are not exact).
+    - As simple as it can get. Just completes the letters of the word, that are actually present (the `FuzzyCompleter`
+      which `completions` uses in background completes based on a probability, and may show matches which are not
+      exact).
 - ...
 
-
 To add your own completer to an input field, you can use the `completer` argument:
 
 ```py
 prompt.input(
     ...
-    completer=my_completer,
-    ...
+completer = my_completer,
+...
 )
 ```
 
 > `completions` and `completer` are **mutually exclusive**! You may not use both!
 
 ---
 
 ### Further Information
 
 If you need some easy examples, refer to [example.py](example.py)!
 
 If you want to contribute, check out the projects repository: [ItsPrompt](https://github.com/TheItsProjects/ItsPrompt)!
 
 If you got any other questions, or want to give an idea on how to improve **ItsPrompt**:
+
 - visit our discussions: [ItsPrompt Discussions](https://github.com/TheItsProjects/ItsPrompt/discussions)!
 - join our discord: [TheItsProjects](https://discord.gg/rP9Qke2jDs)!
 
 ---
 
 Puh, that was so much to read... But now, lets have fun with **ItsPrompt**!
```

### Comparing `ItsPrompt-1.3/README.md` & `ItsPrompt-1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,59 +10,66 @@
 
 ![Demonstration](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/ItsPrompt.gif)
 
 # ItsPrompt
 
 Do you ever feel the need to ask a user of your code for an input?
 
-Using `input()` is easy, but is it great? 
+Using `input()` is easy, but is it great?
 
 Do you want to give the user a selection list, a yes-or-no question, or maybe a multiline input field?
 
 And do you think all of this should be done easily, without caring to much how it all works?
 
 Then you are right here! **ItsPrompt** gives you the ability to ask the user for input, the *fancy* way.
 
-**ItsPrompt** tries to be an easy-to-use module for managing prompts for the user. You task is to create a great program, not how to ask the user for input. That is why **ItsPrompt** is there to take care of this problem, so you can focus on the important things!
+**ItsPrompt** tries to be an easy-to-use module for managing prompts for the user. You task is to create a great
+program, not how to ask the user for input. That is why **ItsPrompt** is there to take care of this problem, so you can
+focus on the important things!
 
 # TOC
 
 - [ItsPrompt](#itsprompt)
 - [TOC](#toc)
     - [A small, thankful note](#a-small-thankful-note)
-  - [Features](#features)
-  - [Installation](#installation)
-  - [Usage](#usage)
-  - [Prompt types](#prompt-types)
-    - [`select`](#select)
-    - [`raw_select`](#raw_select)
-    - [`expand`](#expand)
-    - [`checkbox`](#checkbox)
-    - [`confirm`](#confirm)
-    - [`input`](#input)
-    - [`table`](#table)
-  - [Additional Features and Tips](#additional-features-and-tips)
-    - [Options](#options)
-    - [Data](#data)
-    - [Styling](#styling)
-    - [Prompt Validation](#prompt-validation)
-    - [Prompt Completion](#prompt-completion)
-    - [Further Information](#further-information)
+    - [Features](#features)
+    - [Installation](#installation)
+    - [Usage](#usage)
+    - [Prompt types](#prompt-types)
+        - [`select`](#select)
+        - [`raw_select`](#raw_select)
+        - [`expand`](#expand)
+        - [`checkbox`](#checkbox)
+        - [`confirm`](#confirm)
+        - [`input`](#input)
+        - [`table`](#table)
+    - [Additional Features and Tips](#additional-features-and-tips)
+        - [Options](#options)
+        - [Data](#data)
+        - [Styling](#styling)
+        - [Prompt Validation](#prompt-validation)
+        - [Prompt Completion](#prompt-completion)
+        - [Further Information](#further-information)
 
 ---
 
 ### A small, thankful note
 
-This project is not the first to accomplish the above mentioned tasks. There is another package, `PyInquirer`, which inspired me to build **ItsPrompt**.
+This project is not the first to accomplish the above mentioned tasks. There is another package, `PyInquirer`, which
+inspired me to build **ItsPrompt**.
 
-On my way to create a small program I came to a point were I needed a simple GUI, and I tried `PyInquirer`. Unfortunately, at the current time it is not actively maintained and a bit outdated. I thought of updating it, but then I thought "*Isn't it easier to just create my own version?*" - And so I did!
+On my way to create a small program I came to a point were I needed a simple GUI, and I tried `PyInquirer`.
+Unfortunately, at the current time it is not actively maintained and a bit outdated. I thought of updating it, but then
+I thought "*Isn't it easier to just create my own version?*" - And so I did!
 
-**ItsPrompt** is not a copy or a fork of `PyInquirer`. I built this module from the ground up, without ever looking deep into the source code of `PyInquirer`.
+**ItsPrompt** is not a copy or a fork of `PyInquirer`. I built this module from the ground up, without ever looking deep
+into the source code of `PyInquirer`.
 
-On my way to build this package, I learned a lot about `prompt-toolkit`, and all of this just because of `PyInquirer`! Thanks!
+On my way to build this package, I learned a lot about `prompt-toolkit`, and all of this just because of `PyInquirer`!
+Thanks!
 
 ---
 
 ## Features
 
 - many prompt types (more details below):
     - select
@@ -83,14 +90,20 @@
 
 This package is hosted on pypi, so the installation is as simple as it can get:
 
 ```
 python3 -m pip install ItsPrompt
 ```
 
+This will install `ItsPrompt` without pandas. If you want to use `TablePrompt` (see [table](#table)) with
+`pandas.DataFrame`, you can install pandas support either by:
+
+- installing pandas separately
+- install `ItsPrompt` via `pip install ItsPrompt[df]`
+
 ---
 
 ## Usage
 
 Import the `Prompt` class:
 
 ```py
@@ -123,15 +136,14 @@
     default='option1',
     style=my_style,
 )
 ```
 
 *additional information on the function arguments can be found in the docstring*
 
-
 ### `raw_select`
 
 ![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/raw_select.png)
 
 ```py
 Prompt.raw_select(
     question='question',
@@ -196,76 +208,91 @@
 ![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/input.png)
 
 ```py
 Prompt.input(
     question='question',
     default='something',
     multiline=False,
-    show_symbol='*', # not compatible with complete, completer
+    show_symbol='*',  # not compatible with complete, completer
     validate=validation_function,
-    complete=['completion1', 'completion2'], # either use complete
-    completer=my_completer,                  # or completer
+    complete=['completion1', 'completion2'],  # either use complete
+    completer=my_completer,  # or completer
     completion_show_multicolumn=True,
     style=my_style,
 )
 ```
 
 *additional information on the function arguments can be found in the docstring*
 
 ### `table`
 
 ![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/table.png)
 
 ```py
 Prompt.table(
+    question="something",
+    data={"0": ["something"]},
+    style=my_style,
+)
+
+# or, after having installed pandas
+
+Prompt.table(
     question='something',
     data=DataFrame(['something']),
     style=my_style,
 )
 ```
 
 *additional information on the function arguments can be found in the docstring*
 
 ---
 
 ## Additional Features and Tips
 
 ### Options
 
-The `options` is always a `tuple` containing `str` and `tuple` objects. 
+The `options` is always a `tuple` containing `str` and `tuple` objects.
 
-If an option is given as a `str`, this will be used as the options display name and the id, which will be returned when selecting this option.
+If an option is given as a `str`, this will be used as the options display name and the id, which will be returned when
+selecting this option.
 
 *In case of `expand`, the first character of the `str` will be used as its key.*
 
 If an option is given as a `tuple`, the first value will be the options name, the second value the options id to return.
 
 *In case of `expand`, the first value will be the key, the second value the name and the third value the id.*
 
 ---
 
 ### Data
 
 The `table` prompt takes a mandatory `data` argument, which needs to be a `pandas.DataFrame`.
 
-This `DataFrame` is used as the content of the table. The user may change the fields of the table. The output of the `table` prompt is a `pandas.DataFrame` with the user given values.
+This `DataFrame` is used as the content of the table. The user may change the fields of the table. The output of
+the `table` prompt is a `pandas.DataFrame` with the user given values.
 
-Currently, the output will convert all input values to a `str`, so `int`, `bool`, ... will be converted to strings. This is a current limitation of the way the table is displayed, but may later be updated.
+Currently, the output will convert all input values to a `str`, so `int`, `bool`, ... will be converted to strings. This
+is a current limitation of the way the table is displayed, but may later be updated.
 
-Another limitation of the `table` prompt is the use of styling in the `DataFrame` fields. All styling tags will be displayed as-is, so a `<u>...</u>` will not be underlined, but rather displayed as its shown.
+Another limitation of the `table` prompt is the use of styling in the `DataFrame` fields. All styling tags will be
+displayed as-is, so a `<u>...</u>` will not be underlined, but rather displayed as its shown.
 
 ---
 
 ### Styling
 
-**ItsPrompt** uses `prompt-toolkit` for its prompts. This module not only provides an easy way to interact with the command line, but also a full set of styling features.
+**ItsPrompt** uses `prompt-toolkit` for its prompts. This module not only provides an easy way to interact with the
+command line, but also a full set of styling features.
 
-You can learn more about the available styling features in the documentation of `prompt-toolkit`: [Styling](https://python-prompt-toolkit.readthedocs.io/en/master/pages/printing_text.html#formatted-text).
+You can learn more about the available styling features in the documentation
+of `prompt-toolkit`: [Styling](https://python-prompt-toolkit.readthedocs.io/en/master/pages/printing_text.html#formatted-text).
 
-**ItsPrompt** makes it a bit easier for you to style each component of a prompt. For every component, we give a separate attribute in the `PromptStyle` class, which you can style with valid `prompt-toolkit` styling:
+**ItsPrompt** makes it a bit easier for you to style each component of a prompt. For every component, we give a separate
+attribute in the `PromptStyle` class, which you can style with valid `prompt-toolkit` styling:
 
 ```py
 # examples for the different styling class components
 Prompt.raw_select(
     question='question',
     options=(
         'option',
@@ -280,28 +307,27 @@
 )
 ```
 
 ![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/styling_raw_select_annotated.png)
 
 ![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/styling_input_annotated.png)
 
-| ID  |    styling tag    |             default style             |
-| --- | ----------------- | ------------------------------------- |
-| 1   | `question_mark`   | `fg:ansigreen`                        |
-| 2   | `question`        | *                                     |
-| 3   | `option`          | *                                     |
-| 4   | `selected_option` | `fg:ansicyan`                         |
-| 5   | `tooltip`         | `fg:ansibrightblue bg:ansiwhite bold` |
-| 6   | `text`            | *                                     |
-| 7   | `grayout`          | `fg:ansibrightblack`                  |
-| 8   | `error`           | `fg:ansiwhite bg:ansired bold`        |
+| ID | styling tag       | default style                         |
+|----|-------------------|---------------------------------------|
+| 1  | `question_mark`   | `fg:ansigreen`                        |
+| 2  | `question`        | *                                     |
+| 3  | `option`          | *                                     |
+| 4  | `selected_option` | `fg:ansicyan`                         |
+| 5  | `tooltip`         | `fg:ansibrightblue bg:ansiwhite bold` |
+| 6  | `text`            | *                                     |
+| 7  | `grayout`         | `fg:ansibrightblack`                  |
+| 8  | `error`           | `fg:ansiwhite bg:ansired bold`        |
 
 *\*These values are not changed from the default `prompt-toolkit` values.*
 
-
 To create your own style, there are two ways:
 
 ***Changing the default style***
 
 To change the default style, you need to import the `default_style` and change its values:
 
 ```py
@@ -310,151 +336,165 @@
 default_style.error = 'fg:ansired bg:ansiwhite'
 ```
 
 This will automatically change the style of all prompts, which do not have an own style defined.
 
 ***Creating your own style***
 
-To define your own style for a specific prompt, import `PromptStyle` and create an object. Then assign it to the `style` argument of a prompt.
+To define your own style for a specific prompt, import `PromptStyle` and create an object. Then assign it to the `style`
+argument of a prompt.
 
 ```py
 from ItsPrompt.data.style import PromptStyle
 
 my_style = PromptStyle(
     question_mark='fg:ansiblue',
     error='fg:ansired bg:ansiwhite',
 )
 ```
 
-All styles which are not given, **will not** be the same as the default style. Instead they will use the styling given by `prompt-toolkit`. If you want to change our default styles, then copy the `default_style` and change your values, instead of directly creating your own style:
+All styles which are not given, **will not** be the same as the default style. Instead they will use the styling given
+by `prompt-toolkit`. If you want to change our default styles, then copy the `default_style` and change your values,
+instead of directly creating your own style:
 
 ```py
 from ItsPrompt.data.style import create_from_default
 
 my_style = create_from_default()
 
 my_style.error = 'fg:ansired bg:ansiwhite'
 ```
 
-> Warning! Not copying the default style and changing it instead will result in all prompts using your changes, as a variable is by default not a copy, but a reference to the same object!
+> Warning! Not copying the default style and changing it instead will result in all prompts using your changes, as a
+> variable is by default not a copy, but a reference to the same object!
 
 ---
 
 ### Prompt Validation
 
-The `input` allows you to validate the input before submitting it. For every character the user types, the validation will be run and a friendly error will be shown in the toolbar.
+The `input` allows you to validate the input before submitting it. For every character the user types, the validation
+will be run and a friendly error will be shown in the toolbar.
 
-To use the validation feature, create a function which takes a `str` as an argument and returns either a `str` or `None`.
+To use the validation feature, create a function which takes a `str` as an argument and returns either a `str`
+or `None`.
 
 ```py
 def input_not_empty(input: str) -> str | None:
     if len(input) == 0:
         return 'Address can not be empty!'
 
+
 Prompt.input(
     ...
-    validate=input_not_empty,
-    ...
+validate = input_not_empty,
+...
 )
 ```
 
 The `str` argument will be the current user input, which can then be checked, but not changed!
 
 If you want to show that the validation succeeded, return `None` (or nothing). This will not trigger any errors.
 
-If you want to show an error, return a `str` with the errors text. Your text will be shown in the toolbar. As long as the validation returns a `str`, the user may not submit the input.
+If you want to show an error, return a `str` with the errors text. Your text will be shown in the toolbar. As long as
+the validation returns a `str`, the user may not submit the input.
 
 ---
 
 ### Prompt Completion
 
-The `input` prompt type supports auto completion as well. 
+The `input` prompt type supports auto completion as well.
 
 > If you use a completer, you are unable to use `show_symbol`!
 
 To give auto completion options, there are three ways:
 
 ***Creating a simple list of possible completions***
 
 `Input` takes a `list[str]` to use as simple word completions. Each `str` in the list is a possible value to complete.
 
 ```py
 prompt.input(
     ...
-    completions=['Mainstreet 4', 'Fifth way'],
-    ...
+completions = ['Mainstreet 4', 'Fifth way'],
+...
 )
 ```
 
 ***Creating a nested dictionary of possible completions***
 
-You can use a dictionary for nested completions. Each "layer" will be a completion, after the first was accepted. For example:
+You can use a dictionary for nested completions. Each "layer" will be a completion, after the first was accepted. For
+example:
 
 ```py
 completions = {
-    '1' : {
-        '1.1' : None,
-        '1.2' : {
+    '1': {
+        '1.1': None,
+        '1.2': {
             '1.2.1', '1.2.2'
         }
     },
-    '2' : {
-        '2.1' : { '2.1.1' }
+    '2': {
+        '2.1': {'2.1.1'}
     }
 }
 
 prompt.input(
     ...
-    completions=completions,
-    ...
+completions = completions,
+...
 )
 ```
 
-The key of each entry is the completion that will be shown. The key is either None if there are no further completions or a new dict, where the key is the completion and the value is the next "layer", and so on...
+The key of each entry is the completion that will be shown. The key is either None if there are no further completions
+or a new dict, where the key is the completion and the value is the next "layer", and so on...
 
 > For more information, the type signature of `CompletionDict` is:  
 > `dict[str, "CompletionDict | None"]`
 
 ***Using a given Completer by `prompt-toolkit` or creating your own***
 
 In the background your completions will be mapped to a `Completer`, provided by `prompt-toolkit`.
 
-If you need more customization, you can use a `Completer` given by `prompt-toolkit` or create your own completer. For more information on this process, read here: [Completions in prompt-toolkit](https://python-prompt-toolkit.readthedocs.io/en/stable/pages/asking_for_input.html#autocompletion).
+If you need more customization, you can use a `Completer` given by `prompt-toolkit` or create your own completer. For
+more information on this process, read
+here: [Completions in prompt-toolkit](https://python-prompt-toolkit.readthedocs.io/en/stable/pages/asking_for_input.html#autocompletion).
 
 There are a number of completers available, for example:
 
 - `PathCompleter`
     - automatically complete file system paths
 - `ExecutableCompleter`
     - automatically complete executables in file system
 - `WordCompleter`
-    - As simple as it can get. Just completes the letters of the word, that are actually present (the `FuzzyCompleter` which `completions` uses in background completes based on a probability, and may show matches which are not exact).
+    - As simple as it can get. Just completes the letters of the word, that are actually present (the `FuzzyCompleter`
+      which `completions` uses in background completes based on a probability, and may show matches which are not
+      exact).
 - ...
 
-
 To add your own completer to an input field, you can use the `completer` argument:
 
 ```py
 prompt.input(
     ...
-    completer=my_completer,
-    ...
+completer = my_completer,
+...
 )
 ```
 
 > `completions` and `completer` are **mutually exclusive**! You may not use both!
 
 ---
 
 ### Further Information
 
 If you need some easy examples, refer to [example.py](example.py)!
 
 If you want to contribute, check out the projects repository: [ItsPrompt](https://github.com/TheItsProjects/ItsPrompt)!
 
 If you got any other questions, or want to give an idea on how to improve **ItsPrompt**:
+
 - visit our discussions: [ItsPrompt Discussions](https://github.com/TheItsProjects/ItsPrompt/discussions)!
 - join our discord: [TheItsProjects](https://discord.gg/rP9Qke2jDs)!
 
 ---
 
 Puh, that was so much to read... But now, lets have fun with **ItsPrompt**!
```

### Comparing `ItsPrompt-1.3/tests/test_prompt.py` & `ItsPrompt-1.4/tests/test_prompt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-from ItsPrompt.prompt import Prompt
-
-from prompt_toolkit.keys import Keys
-from prompt_toolkit.completion import FuzzyWordCompleter
-
+import pytest
 from pandas import DataFrame
 from pandas.testing import assert_frame_equal
+from prompt_toolkit.completion import FuzzyWordCompleter
+from prompt_toolkit.keys import Keys
 
-import pytest
+from ItsPrompt.prompt import Prompt
 
 
 # --- Select ---
 @pytest.mark.parametrize(
     "keys,i",
     [
-        [(Keys.Enter, ), 0],
+        [(Keys.Enter,), 0],
         [(Keys.Down, Keys.Enter), 1],
         [(Keys.Down, Keys.Down, Keys.Enter), 2],
         [(Keys.Up, Keys.Enter), 2],
     ],
 )
 def test_select(send_keys, keys: list[Keys | str], i: int):
     options = ("first", "second", "third")
@@ -28,15 +26,15 @@
 
     assert ans == options[i]
 
 
 @pytest.mark.parametrize(
     "keys,i",
     [
-        [(Keys.Enter, ), 1],
+        [(Keys.Enter,), 1],
         [(Keys.Down, Keys.Enter), 2],
         [(Keys.Down, Keys.Down, Keys.Enter), 0],
         [(Keys.Up, Keys.Enter), 0],
     ],
 )
 def test_select_with_default(send_keys, keys: list[Keys | str], i: int):
     options = ("first", "second", "third")
@@ -63,15 +61,15 @@
         ans = Prompt.select("", options)
 
 
 # --- RawSelect ---
 @pytest.mark.parametrize(
     "keys,i",
     [
-        [(Keys.Enter, ), 0],
+        [(Keys.Enter,), 0],
         [("1", Keys.Enter), 0],
         [("2", Keys.Enter), 1],
         [(Keys.Up, Keys.Down, "abc", "99", Keys.Enter), 0],
     ],
 )
 def test_raw_select(send_keys, keys: list[Keys | str], i: int):
     options = ("first", "second", "third")
@@ -82,15 +80,15 @@
 
     assert ans == options[i]
 
 
 @pytest.mark.parametrize(
     "keys,i",
     [
-        [(Keys.Enter, ), 1],
+        [(Keys.Enter,), 1],
         [("1", Keys.Enter), 0],
         [("2", Keys.Enter), 1],
     ],
 )
 def test_raw_select_with_default(send_keys, keys: list[Keys | str], i: int):
     options = ("first", "second", "third")
 
@@ -100,15 +98,15 @@
 
     assert ans == options[i]
 
 
 @pytest.mark.parametrize(
     "keys,i",
     [
-        [(Keys.Enter, ), 0],
+        [(Keys.Enter,), 0],
         [(Keys.Down, Keys.Enter), 1],
         [(Keys.Up, Keys.Enter), 2],
     ],
 )
 def test_raw_select_with_keyboard(send_keys, keys: list[Keys | str], i: int):
     options = ("first", "second", "third")
 
@@ -206,17 +204,17 @@
         ans = Prompt.expand("", options)
 
 
 # --- checkbox ---
 @pytest.mark.parametrize(
     "keys,i",
     [
-        [(Keys.Enter, ), ()],
-        [(" ", Keys.Enter), (0, )],
-        [(Keys.Down, " ", Keys.Enter), (1, )],
+        [(Keys.Enter,), ()],
+        [(" ", Keys.Enter), (0,)],
+        [(Keys.Down, " ", Keys.Enter), (1,)],
         [(" ", Keys.Up, " ", Keys.Enter), (0, 2)],
     ],
 )
 def test_checkbox(send_keys, keys: list[Keys | str], i: list[int]):
     options = ("first", "second", "third")
 
     send_keys(*keys)
@@ -225,36 +223,35 @@
 
     assert ans == [options[n] for n in i]
 
 
 @pytest.mark.parametrize(
     "keys,i",
     [
-        [(Keys.Enter, ), (0, )],
+        [(Keys.Enter,), (0,)],
         [(" ", Keys.Enter), ()],
         [(Keys.Down, " ", Keys.Enter), (0, 1)],
-        [(" ", Keys.Up, " ", Keys.Enter), (2, )],
+        [(" ", Keys.Up, " ", Keys.Enter), (2,)],
     ],
 )
-def test_checkbox_with_default(send_keys, keys: list[Keys | str],
-                               i: list[int]):
+def test_checkbox_with_default(send_keys, keys: list[Keys | str], i: list[int]):
     options = ("first", "second", "third")
 
     send_keys(*keys)
 
-    ans = Prompt.checkbox("", options, default_checked=("first", ))
+    ans = Prompt.checkbox("", options, default_checked=("first",))
 
     assert ans == [options[n] for n in i]
 
 
 def test_checkbox_raises_invalid_default():
     options = ("first", "second", "third")
 
     with pytest.raises(ValueError):
-        ans = Prompt.checkbox("", options, default_checked=("invalid", ))
+        ans = Prompt.checkbox("", options, default_checked=("invalid",))
 
 
 def test_checkbox_raises_keyboard_interrupt(send_keys):
     send_keys(Keys.ControlC)
 
     options = ("first", "second", "third")
 
@@ -308,30 +305,30 @@
 # TODO confirm selections with error box (visual)
 
 
 # --- input ---
 @pytest.mark.parametrize(
     "keys,a",
     [
-        [(Keys.Enter, ), ""],
+        [(Keys.Enter,), ""],
         [("test", Keys.Enter), "test"],
     ],
 )
 def test_input(send_keys, keys: list[Keys | str], a: str):
     send_keys(*keys)
 
     ans = Prompt.input("")
 
     assert ans == a
 
 
 @pytest.mark.parametrize(
     "keys,a",
     [
-        [(Keys.Enter, ), "default"],
+        [(Keys.Enter,), "default"],
         [("test", Keys.Enter), "test"],
     ],
 )
 def test_input_with_default(send_keys, keys: list[Keys | str], a: str):
     send_keys(*keys)
 
     ans = Prompt.input("", default="default")
@@ -341,15 +338,15 @@
 
 KeysAltEnter = Keys.Escape, Keys.Enter  # Vt100 terminals convert "alt+key" to "escape,key"
 
 
 @pytest.mark.parametrize(
     "keys,a",
     [
-        [(*KeysAltEnter, ), ""],
+        [(*KeysAltEnter,), ""],
         [("test", Keys.Enter, *KeysAltEnter), "test\n"],
     ],
 )
 def test_input_with_multiline(send_keys, keys: list[Keys | str], a: str):
     send_keys(*keys)
 
     ans = Prompt.input("", multiline=True)
@@ -385,42 +382,81 @@
 
 
 # --- table ---
 @pytest.mark.parametrize(
     "keys,a",
     [
         [
-            (Keys.Enter, ),
-            DataFrame(["first", "second", "third"], dtype="string"),
+            (Keys.Enter,),
+            DataFrame({"0": ["first", "second", "third"]}),
         ],
         [
             (Keys.Down, "new", Keys.Enter),
-            DataFrame(["first", "secondnew", "third"], dtype="string"),
+            DataFrame({"0": ["first", "secondnew", "third"]}),
         ],
         [
             (Keys.Left, Keys.Right, Keys.Up, Keys.Down, Keys.Enter),
-            DataFrame(["first", "second", "third"], dtype="string"),
+            DataFrame({"0": ["first", "second", "third"]}),
         ],
         [
             (Keys.Backspace, Keys.Enter),
-            DataFrame(["firs", "second", "third"], dtype="string"),
+            DataFrame({"0": ["firs", "second", "third"]}),
         ],
     ],
 )
-def test_table(send_keys, mock_terminal_size, keys: list[Keys | str],
-               a: DataFrame):
+def test_table_dataframe(send_keys, mock_terminal_size, keys: list[Keys | str], a: DataFrame):
     data = DataFrame(["first", "second", "third"])
 
     send_keys(*keys)
 
     ans = Prompt.table("", data)
 
     assert_frame_equal(ans, a)
 
 
-def test_able_raises_keyboard_interrupt(send_keys):
+@pytest.mark.parametrize(
+    "keys,a",
+    [
+        [
+            (Keys.Enter,),
+            {"0": ["first", "second", "third"]},
+        ],
+        [
+            (Keys.Down, "new", Keys.Enter),
+            {"0": ["first", "secondnew", "third"]},
+        ],
+        [
+            (Keys.Left, Keys.Right, Keys.Up, Keys.Down, Keys.Enter),
+            {"0": ["first", "second", "third"]},
+        ],
+        [
+            (Keys.Backspace, Keys.Enter),
+            {"0": ["firs", "second", "third"]},
+        ],
+    ],
+)
+def test_table_dictionary(send_keys, mock_terminal_size, keys: list[Keys | str], a: dict[str, list[str]]):
+    data = {"0": ["first", "second", "third"]}
+
+    send_keys(*keys)
+
+    ans = Prompt.table("", data)
+
+    assert ans == a
+
+
+def test_table_raises_keyboard_interrupt(send_keys):
     send_keys(Keys.ControlC)
 
     data = DataFrame(["first", "second", "third"])
 
     with pytest.raises(KeyboardInterrupt):
         ans = Prompt.table("", data)
+
+
+def test_table_dictionary_raises_lists_not_same_lengths(send_keys):
+    send_keys(Keys.ControlC)
+
+    data = {"0": ["first", "second", "third"], "1": ["other first"]}
+
+    with pytest.raises(ValueError):
+        ans = Prompt.table("", data)
```

