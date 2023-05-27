# Comparing `tmp/money-lib-3.0.1.tar.gz` & `tmp/money-lib-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/money-lib-3.0.1.tar", last modified: Thu Oct 29 01:15:05 2020, max compression
+gzip compressed data, was "/home/runner/work/money-lib/money-lib/dist/.tmp-5sw5517h/money-lib-3.1.0.tar", last modified: Sat May 27 09:03:49 2023, max compression
```

## Comparing `money-lib-3.0.1.tar` & `money-lib-3.1.0.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-29 01:15:05.000000 money-lib-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (116)     6001 2020-10-29 01:15:05.000000 money-lib-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1343 2020-10-29 01:14:54.000000 money-lib-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-29 01:15:05.000000 money-lib-3.0.1/money/
--rw-r--r--   0 runner    (1001) docker     (116)      170 2020-10-29 01:14:54.000000 money-lib-3.0.1/money/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4811 2020-10-29 01:14:54.000000 money-lib-3.0.1/money/money.py
--rw-r--r--   0 runner    (1001) docker     (116)     2584 2020-10-29 01:14:54.000000 money-lib-3.0.1/money/exchange.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-29 01:15:05.000000 money-lib-3.0.1/money/django/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-29 01:14:54.000000 money-lib-3.0.1/money/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      564 2020-10-29 01:14:54.000000 money-lib-3.0.1/money/django/widgets.py
--rw-r--r--   0 runner    (1001) docker     (116)     1297 2020-10-29 01:14:54.000000 money-lib-3.0.1/money/django/forms.py
--rw-r--r--   0 runner    (1001) docker     (116)     3270 2020-10-29 01:14:54.000000 money-lib-3.0.1/money/django/fields.py
--rw-r--r--   0 runner    (1001) docker     (116)     1066 2020-10-29 01:14:54.000000 money-lib-3.0.1/money/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     1775 2020-10-29 01:14:54.000000 money-lib-3.0.1/money/currency.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-29 01:15:05.000000 money-lib-3.0.1/money_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-29 01:15:05.000000 money-lib-3.0.1/money_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)     6001 2020-10-29 01:15:05.000000 money-lib-3.0.1/money_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       35 2020-10-29 01:15:05.000000 money-lib-3.0.1/money_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)      365 2020-10-29 01:15:05.000000 money-lib-3.0.1/money_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2020-10-29 01:15:05.000000 money-lib-3.0.1/money_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     4090 2020-10-29 01:14:54.000000 money-lib-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-10-29 01:15:05.000000 money-lib-3.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:49.000000 money-lib-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-27 09:03:29.000000 money-lib-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-27 09:03:49.000000 money-lib-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-27 09:03:29.000000 money-lib-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:49.000000 money-lib-3.1.0/money/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-27 09:03:29.000000 money-lib-3.1.0/money/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-27 09:03:29.000000 money-lib-3.1.0/money/currency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:49.000000 money-lib-3.1.0/money/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:29.000000 money-lib-3.1.0/money/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-27 09:03:29.000000 money-lib-3.1.0/money/django/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-27 09:03:29.000000 money-lib-3.1.0/money/django/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-27 09:03:29.000000 money-lib-3.1.0/money/django/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-27 09:03:29.000000 money-lib-3.1.0/money/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-27 09:03:29.000000 money-lib-3.1.0/money/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-27 09:03:29.000000 money-lib-3.1.0/money/money.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:49.000000 money-lib-3.1.0/money_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-27 09:03:49.000000 money-lib-3.1.0/money_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-27 09:03:49.000000 money-lib-3.1.0/money_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 09:03:49.000000 money-lib-3.1.0/money_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-27 09:03:49.000000 money-lib-3.1.0/money_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 09:03:49.000000 money-lib-3.1.0/money_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-27 09:03:29.000000 money-lib-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 09:03:49.000000 money-lib-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 09:03:49.000000 money-lib-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-27 09:03:29.000000 money-lib-3.1.0/tests/test_currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-27 09:03:29.000000 money-lib-3.1.0/tests/test_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-27 09:03:29.000000 money-lib-3.1.0/tests/test_money.py
```

### Comparing `money-lib-3.0.1/money/money.py` & `money-lib-3.1.0/money/money.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,23 @@
             return NotImplemented
 
         return self.__class__(result, self._currency)
 
     return operator_func
 
 
+def _make_class_operator(name):
+    method = getattr(Decimal, name, None)
+
+    def operator_func(self, *args):
+        return self.__class__(method(self, *args), self._currency)
+
+    return operator_func
+
+
 class Money(Decimal):
     """Class representing a monetary amount."""
 
     _rounding_mode = ROUND_HALF_UP
 
     __slots__ = ('_currency',)
 
@@ -60,37 +69,41 @@
 
     @property
     def currency(self):
         """Returns the currency."""
 
         return self._currency
 
+    def __composite_values__(self):
+        # https://docs.sqlalchemy.org/en/14/orm/composites.html
+        return Decimal(self), str(self._currency)
+
     def __repr__(self):
-        return 'Money({}, \'{}\')'.format(super().__repr__(), self._currency)
+        return f"Money({super().__repr__()}, {self._currency!r})"
 
     def __str__(self):
         return self.format()
 
     def __reduce__(self):
         return self.__class__, (Decimal.__str__(self), self._currency)
 
     def __eq__(self, other):
         result = super().__eq__(other)
         if result is NotImplemented:
             return NotImplemented
 
         if isinstance(other, Money):
             return result and other._currency == self._currency
-        else:
-            return result
+        return result
 
     def __ne__(self, other):
         return not self == other
 
-    __hash__ = Decimal.__hash__
+    def __hash__(self):
+        return hash((Decimal(self), self._currency.code))
 
     __lt__ = _make_comparison_operator('__lt__')
     __le__ = _make_comparison_operator('__le__')
     __gt__ = _make_comparison_operator('__gt__')
     __ge__ = _make_comparison_operator('__ge__')
 
     __add__ = _make_arithmetic_operator('__add__')
@@ -106,31 +119,20 @@
     __mod__ = _make_arithmetic_operator('__mod__')
     __rmod__ = _make_arithmetic_operator('__rmod__')
     __floordiv__ = _make_arithmetic_operator('__floordiv__')
     __rfloordiv__ = _make_arithmetic_operator('__rfloordiv__')
     __pow__ = _make_arithmetic_operator('__pow__')
     __rpow__ = _make_arithmetic_operator('__rpow__')
 
-    def __neg__(self):
-        return self.__class__(super().__neg__(), self._currency)
-
-    def __pos__(self):
-        return self.__class__(super().__pos__(), self._currency)
-
-    def __abs__(self):
-        return self.__class__(super().__abs__(), self._currency)
-
-    def __round__(self, n=0):
-        return self.__class__(super().__round__(n), self._currency)
-
-    def __floor__(self):
-        return self.__class__(super().__floor__(), self._currency)
-
-    def __ceil__(self):
-        return self.__class__(super().__ceil__(), self._currency)
+    __neg__ = _make_class_operator('__neg__')
+    __pos__ = _make_class_operator('__pos__')
+    __abs__ = _make_class_operator('__abs__')
+    __round__ = _make_class_operator('__round__')
+    __floor__ = _make_class_operator('__floor__')
+    __ceil__ = _make_class_operator('__ceil__')
 
     def to(self, currency):
         """Returns the equivalent money object in another currency."""
 
         if currency == self._currency:
             return self
 
@@ -145,12 +147,12 @@
             raise ExchangeRateNotFound(xrates.backend_name, self._currency, currency)
 
         return self.__class__(self * rate, currency)
 
     def format(self, locale='en_US'):
         """Returns a string of the currency formatted for the specified locale."""
 
-        return format_currency(self, self.currency.code, locale=locale).replace(u'\xa0', u' ')
+        return format_currency(self, self.currency.code, locale=locale).replace('\xa0', ' ')
 
     @classmethod
     def set_rounding_mode(cls, mode):
         cls._rounding_mode = mode
```

### Comparing `money-lib-3.0.1/money/exchange.py` & `money-lib-3.1.0/money/exchange.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     def __getattr__(self, item):
         if self._backend is None:
             raise ExchangeBackendNotSet()
         return getattr(self._backend, item)
 
     def __setattr__(self, key, value):
-        if key == '_backend' or key == 'backend':
+        if key in ('_backend', 'backend'):
             return super().__setattr__(key, value)
         if self._backend is None:
             raise ExchangeBackendNotSet()
         return setattr(self._backend, key, value)
 
 
 xrates = ExchangeRates()
```

### Comparing `money-lib-3.0.1/money/django/widgets.py` & `money-lib-3.1.0/money/django/widgets.py`

 * *Files identical despite different names*

### Comparing `money-lib-3.0.1/money/django/forms.py` & `money-lib-3.1.0/money/django/forms.py`

 * *Files identical despite different names*

### Comparing `money-lib-3.0.1/money/django/fields.py` & `money-lib-3.1.0/money/django/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
 from money import Currency, Money
 from money.django import forms
 
 
-def _currency_field_name(name): return '{}_currency'.format(name)
+def _currency_field_name(name): return f"{name}_currency"
 
 
-class MoneyFieldProxy(object):
+class MoneyFieldProxy:
     def __init__(self, field):
         self.field = field
         self.currency_name = _currency_field_name(self.field.name)
 
     def __set__(self, obj, value):
         if isinstance(value, Money):
             obj.__dict__[self.field.name] = value
@@ -25,16 +25,15 @@
     def __get__(self, obj, type=None):
         if obj is None:
             return self
 
         amount = obj.__dict__[self.field.name]
         if amount is None:
             return None
-        else:
-            return Money(amount, getattr(obj, self.currency_name))
+        return Money(amount, getattr(obj, self.currency_name))
 
 
 class CurrencyField(models.CharField):
     description = _("Currency Object")
 
     def __init__(self, *args, **kwargs):
         default = kwargs.get('default', None)
```

### Comparing `money-lib-3.0.1/money/exceptions.py` & `money-lib-3.1.0/money/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 class CurrencyException(MoneyException):
     pass
 
 
 class InvalidCurrencyFormat(CurrencyException, ValueError):
     def __init__(self, currency):
         msg = (
-            'Currency not in ISO 4217 format: \'{}\'.'
-        ).format(currency)
+            f"Currency not in ISO 4217 format: '{currency}'."
+        )
         super().__init__(msg)
 
 
 class ExchangeError(MoneyException):
     pass
 
 
@@ -34,10 +34,10 @@
         )
         super().__init__(msg)
 
 
 class ExchangeRateNotFound(ExchangeError):
     def __init__(self, backend, origin, target):
         msg = (
-            'Rate not found in backend \'{}\': {}/{}.'
-        ).format(backend, origin, target)
+            f"Rate not found in backend '{backend}': {origin}/{target}."
+        )
         super().__init__(msg)
```

### Comparing `money-lib-3.0.1/money/currency.py` & `money-lib-3.1.0/money/currency.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
     Raises
     ------
     InvalidCurrencyFormat
         If the given currency_code isn't a valid ISO 4217 format
     """
 
+    __slots__ = ('_code',)
+
     def __init__(self, currency_code):
         if not CURRENCY_REGEX.match(currency_code):
             raise InvalidCurrencyFormat(currency_code)
 
         self._code = currency_code
 
     @property
@@ -47,15 +49,15 @@
 
     def symbol(self, locale='en_US'):
         """Returns the symbol used by the locale for this currency."""
 
         return get_currency_symbol(self._code, locale=locale)
 
     def __repr__(self):
-        return 'Currency(\'{}\')'.format(self._code)
+        return f"Currency({self._code!r})"
 
     def __str__(self):
         return self._code
 
     def __reduce__(self):
         return self.__class__, (self._code,)
```

### Comparing `money-lib-3.0.1/README.md` & `money-lib-3.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # money-lib
 
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/r4g3baby/money-lib/Test)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/r4g3baby/money-lib/test.yml?branch=main)
 ![PyPI - Version](https://img.shields.io/pypi/v/money-lib.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/money-lib.svg)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/money-lib)
 ![PyPI - License](https://img.shields.io/pypi/l/money-lib.svg)
 
 Python 3 money lib with decimal precision and currency exchange support.
 
 ## Installation
 
 Install the latest release with:
```

