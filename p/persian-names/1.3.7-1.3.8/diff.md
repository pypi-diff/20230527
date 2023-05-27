# Comparing `tmp/persian-names-1.3.7.tar.gz` & `tmp/persian-names-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persian-names-1.3.7.tar", last modified: Fri Apr  7 21:14:01 2023, max compression
+gzip compressed data, was "persian-names-1.3.8.tar", last modified: Sat May 27 20:31:35 2023, max compression
```

## Comparing `persian-names-1.3.7.tar` & `persian-names-1.3.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-04-07 21:14:01.660453 persian-names-1.3.7/
--rw-r--r--   0 arman      (501) staff       (20)     1068 2022-11-15 18:36:04.000000 persian-names-1.3.7/LICENSE
--rw-r--r--   0 arman      (501) staff       (20)     4006 2023-04-07 21:14:01.660333 persian-names-1.3.7/PKG-INFO
--rw-r--r--   0 arman      (501) staff       (20)     2700 2023-03-06 21:55:33.000000 persian-names-1.3.7/README.md
-drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-04-07 21:14:01.658272 persian-names-1.3.7/persian_names/
--rw-r--r--   0 arman      (501) staff       (20)       28 2022-11-21 18:59:10.000000 persian-names-1.3.7/persian_names/__init__.py
-drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-04-07 21:14:01.660062 persian-names-1.3.7/persian_names/data/
--rw-r--r--   0 arman      (501) staff       (20)     2239 2023-04-07 21:05:49.000000 persian-names-1.3.7/persian_names/data/female_en.txt
--rw-r--r--   0 arman      (501) staff       (20)     3380 2023-04-07 21:06:05.000000 persian-names-1.3.7/persian_names/data/female_fa.txt
--rw-r--r--   0 arman      (501) staff       (20)     2045 2023-04-07 21:06:37.000000 persian-names-1.3.7/persian_names/data/male_en.txt
--rw-r--r--   0 arman      (501) staff       (20)     3069 2023-04-07 21:08:00.000000 persian-names-1.3.7/persian_names/data/male_fa.txt
--rw-r--r--   0 arman      (501) staff       (20)        0 2023-03-06 21:07:00.000000 persian-names-1.3.7/persian_names/p.py
--rw-r--r--   0 arman      (501) staff       (20)     7711 2023-04-07 21:10:44.000000 persian-names-1.3.7/persian_names/persian_names.py
-drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-04-07 21:14:01.658965 persian-names-1.3.7/persian_names.egg-info/
--rw-r--r--   0 arman      (501) staff       (20)     4006 2023-04-07 21:14:01.000000 persian-names-1.3.7/persian_names.egg-info/PKG-INFO
--rw-r--r--   0 arman      (501) staff       (20)      378 2023-04-07 21:14:01.000000 persian-names-1.3.7/persian_names.egg-info/SOURCES.txt
--rw-r--r--   0 arman      (501) staff       (20)        1 2023-04-07 21:14:01.000000 persian-names-1.3.7/persian_names.egg-info/dependency_links.txt
--rw-r--r--   0 arman      (501) staff       (20)       14 2023-04-07 21:14:01.000000 persian-names-1.3.7/persian_names.egg-info/top_level.txt
--rw-r--r--   0 arman      (501) staff       (20)       38 2023-04-07 21:14:01.660571 persian-names-1.3.7/setup.cfg
--rw-r--r--   0 arman      (501) staff       (20)     1722 2023-04-07 21:05:21.000000 persian-names-1.3.7/setup.py
+drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-05-27 20:31:35.372847 persian-names-1.3.8/
+-rw-r--r--   0 arman      (501) staff       (20)     1068 2022-11-15 18:36:04.000000 persian-names-1.3.8/LICENSE
+-rw-r--r--   0 arman      (501) staff       (20)     4006 2023-05-27 20:31:35.372724 persian-names-1.3.8/PKG-INFO
+-rw-r--r--   0 arman      (501) staff       (20)     2700 2023-03-06 21:55:33.000000 persian-names-1.3.8/README.md
+drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-05-27 20:31:35.370750 persian-names-1.3.8/persian_names/
+-rw-r--r--   0 arman      (501) staff       (20)       28 2022-11-21 18:59:10.000000 persian-names-1.3.8/persian_names/__init__.py
+drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-05-27 20:31:35.372429 persian-names-1.3.8/persian_names/data/
+-rw-r--r--   0 arman      (501) staff       (20)     2239 2023-04-07 21:05:49.000000 persian-names-1.3.8/persian_names/data/female_en.txt
+-rw-r--r--   0 arman      (501) staff       (20)     3380 2023-04-07 21:06:05.000000 persian-names-1.3.8/persian_names/data/female_fa.txt
+-rw-r--r--   0 arman      (501) staff       (20)     2089 2023-05-27 20:27:16.000000 persian-names-1.3.8/persian_names/data/male_en.txt
+-rw-r--r--   0 arman      (501) staff       (20)     3133 2023-05-27 20:27:47.000000 persian-names-1.3.8/persian_names/data/male_fa.txt
+-rw-r--r--   0 arman      (501) staff       (20)        0 2023-03-06 21:07:00.000000 persian-names-1.3.8/persian_names/p.py
+-rw-r--r--   0 arman      (501) staff       (20)     7834 2023-05-27 20:28:55.000000 persian-names-1.3.8/persian_names/persian_names.py
+drwxr-xr-x   0 arman      (501) staff       (20)        0 2023-05-27 20:31:35.371350 persian-names-1.3.8/persian_names.egg-info/
+-rw-r--r--   0 arman      (501) staff       (20)     4006 2023-05-27 20:31:35.000000 persian-names-1.3.8/persian_names.egg-info/PKG-INFO
+-rw-r--r--   0 arman      (501) staff       (20)      378 2023-05-27 20:31:35.000000 persian-names-1.3.8/persian_names.egg-info/SOURCES.txt
+-rw-r--r--   0 arman      (501) staff       (20)        1 2023-05-27 20:31:35.000000 persian-names-1.3.8/persian_names.egg-info/dependency_links.txt
+-rw-r--r--   0 arman      (501) staff       (20)       14 2023-05-27 20:31:35.000000 persian-names-1.3.8/persian_names.egg-info/top_level.txt
+-rw-r--r--   0 arman      (501) staff       (20)       38 2023-05-27 20:31:35.372960 persian-names-1.3.8/setup.cfg
+-rw-r--r--   0 arman      (501) staff       (20)     1722 2023-05-27 20:30:06.000000 persian-names-1.3.8/setup.py
```

### Comparing `persian-names-1.3.7/LICENSE` & `persian-names-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `persian-names-1.3.7/PKG-INFO` & `persian-names-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persian-names
-Version: 1.3.7
+Version: 1.3.8
 Summary: A Python library for generating random Persian (Farsi) names.
 Home-page: https://github.com/armanyazdi/persian-names
 Author: Arman Yazdi
 License: MIT
 Project-URL: Source, https://github.com/armanyazdi/persian-names
 Project-URL: Documentation, https://pypi.org/project/persian-names
 Keywords: persian names,farsi names,iranian names,name generator
```

### Comparing `persian-names-1.3.7/README.md` & `persian-names-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `persian-names-1.3.7/persian_names/data/female_en.txt` & `persian-names-1.3.8/persian_names/data/female_en.txt`

 * *Files identical despite different names*

### Comparing `persian-names-1.3.7/persian_names/data/female_fa.txt` & `persian-names-1.3.8/persian_names/data/female_fa.txt`

 * *Files identical despite different names*

### Comparing `persian-names-1.3.7/persian_names/data/male_en.txt` & `persian-names-1.3.8/persian_names/data/male_en.txt`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 Saeid
 Saleh
 Soleiman
 Soltan
 Yousef
 Abtin
 Ahoura
+Aidin
 Arash
 Aria
 Arian
 Arman
 Armin
 Arsham
 Arta
@@ -122,24 +123,28 @@
 Fariborz
 Farid
 Farrokh
 Farshad
 Farshid
 Farzad
 Farzam
+Farzan
 Farzin
 Fazel
 Ferdos
 Fereidoun
+Garsha
+Garshasb
 Ghader
 Ghasem
 Gholam
 Gholamreza
 Gholi
 Ghorban
+Goudarz
 Habib
 Hadi
 Hamed
 Hamid
 Hamidreza
 Hamoun
 Hashem
@@ -276,8 +281,9 @@
 Yahya
 Yaser
 Yashar
 Yasin
 Yazdan
 Younes
 Zaker
-Zia
+Zia
+Zobeir
```

### Comparing `persian-names-1.3.7/persian_names/data/male_fa.txt` & `persian-names-1.3.8/persian_names/data/male_fa.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 آرش
 آرشام
 آرمان
 آرمین
 آروین
 آریا
 آریان
+آیدین
 اشکان
 اهورا
 باربد
 بردیا
 حسام
 سامیار
 رادین
@@ -125,14 +126,15 @@
 رامبد
 رامتین
 رامین
 رحمت
 رستم
 رشید
 روزبه
+زبیر
 ساسان
 سالار
 سامان
 سبحان
 سجاد
 سروش
 سلمان
@@ -179,14 +181,15 @@
 فربد
 فرخ
 فرداد
 فردوس
 فردین
 فرزاد
 فرزام
+فرزان
 فرزین
 فرشاد
 فرشید
 فرهنگ
 فریبرز
 فرید
 فریدون
@@ -269,14 +272,17 @@
 کمال
 کوروش
 کوشا
 کیارش
 کیان
 کیهان
 کیوان
+گرشا
+گرشاسب
+گودرز
 یاسر
 یاسین
 یاشار
 یحیی
 یزدان
 یعقوب
 یغما
```

### Comparing `persian-names-1.3.7/persian_names/persian_names.py` & `persian-names-1.3.8/persian_names/persian_names.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,16 @@
         'Amir',
         'Aziz',
         'Shah',
         'Nik',
         'Haj',
         'Haji',
         'Soufi',
+        'Afzal',
+        'Fazel',
         'Sheikh',
         'Mirza',
         'Ostad',
         'Malek',
         'Khan',
         'Beig',
         'Arab'
@@ -69,14 +71,15 @@
         'nejad', '',
         'bayat', '',
         'yekta' '',
         'sabet' '',
         'azad', '',
         'zare', '',
         'moghaddam', '',
+        'roshan', '',
     ]
     more_suffixes = [
         'pour', 'i',
         'zadeh', 'i',
         'far', 'i',
         'fard', 'i',
         'khani', 'i',
@@ -95,15 +98,15 @@
     names = f.read().split('\n')
     f.close()
     last_name = names[randrange(len(names))]
 
     for i in names[:26]:
         arabic_names.append(i)
 
-    for i in names[26:50]:
+    for i in names[26:51]:
         illegal_names.append(i)
 
     while last_name in illegal_names:
         last_name = names[randrange(len(names))]
 
     if last_name == 'Mostafa' or last_name == 'Mousa' or last_name == 'Yahya' or last_name == 'Kasra' or last_name == 'Mojtaba':
         last_name += 'vi'
@@ -182,14 +185,16 @@
         'امیر',
         'عزیز',
         'شاه ',
         'نیک ',
         'حاج ',
         'حاجی ',
         'صوفی ',
+        'افضل ',
+        'فاضل ',
         'شیخ ',
         'میرزا ',
         'استاد ',
         'ملک ',
         'خان ',
         'بیگ ',
         'عرب '
@@ -212,14 +217,15 @@
         ' نژاد', '',
         ' بیات', '',
         ' یکتا', '',
         ' ثابت', '',
         ' آزاد', '',
         ' زارع', '',
         ' مقدم', '',
+        ' روشن', '',
     ]
     more_suffixes = [
         ' پور', 'ی',
         ' زاده', 'ی',
         ' فر', 'ی',
         ' فرد', 'ی',
         ' خانی', 'ی',
@@ -238,15 +244,15 @@
     names = f.read().split('\n')
     f.close()
     last_name = names[randrange(len(names))]
 
     for i in names[:26]:
         arabic_names.append(i)
 
-    for i in names[26:50]:
+    for i in names[26:51]:
         illegal_names.append(i)
 
     while last_name in illegal_names:
         last_name = names[randrange(len(names))]
 
     if last_name == 'مرتضی' or last_name == 'مصطفی' or last_name == 'موسی' or last_name == 'کسری' or last_name == 'مجتبی':
         last_name = last_name.replace('ی', 'وی')
```

### Comparing `persian-names-1.3.7/persian_names.egg-info/PKG-INFO` & `persian-names-1.3.8/persian_names.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persian-names
-Version: 1.3.7
+Version: 1.3.8
 Summary: A Python library for generating random Persian (Farsi) names.
 Home-page: https://github.com/armanyazdi/persian-names
 Author: Arman Yazdi
 License: MIT
 Project-URL: Source, https://github.com/armanyazdi/persian-names
 Project-URL: Documentation, https://pypi.org/project/persian-names
 Keywords: persian names,farsi names,iranian names,name generator
```

### Comparing `persian-names-1.3.7/setup.py` & `persian-names-1.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('./README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='persian-names',
-    version='1.3.7',
+    version='1.3.8',
     packages=['persian_names'],
     include_package_data=True,
     data_files=[('', [
         'persian_names/data/female_en.txt',
         'persian_names/data/female_fa.txt',
         'persian_names/data/male_en.txt',
         'persian_names/data/male_fa.txt'
```

