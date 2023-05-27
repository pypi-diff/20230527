# Comparing `tmp/salat-0.2.0.tar.gz` & `tmp/salat-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salat-0.2.0.tar", last modified: Sun Mar  6 20:52:59 2022, max compression
+gzip compressed data, was "salat-1.0.1.tar", last modified: Sat May 27 07:56:47 2023, max compression
```

## Comparing `salat-0.2.0.tar` & `salat-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 zainhussaini   (501) staff       (20)        0 2022-03-06 20:52:59.277984 salat-0.2.0/
--rw-r--r--   0 zainhussaini   (501) staff       (20)     1053 2022-03-06 20:08:57.000000 salat-0.2.0/LICENSE
--rw-r--r--   0 zainhussaini   (501) staff       (20)     4457 2022-03-06 20:52:59.277669 salat-0.2.0/PKG-INFO
--rw-r--r--   0 zainhussaini   (501) staff       (20)     4004 2022-03-06 20:04:21.000000 salat-0.2.0/README.md
-drwxr-xr-x   0 zainhussaini   (501) staff       (20)        0 2022-03-06 20:52:59.275173 salat-0.2.0/salat/
--rw-r--r--   0 zainhussaini   (501) staff       (20)       62 2021-10-23 22:23:49.000000 salat-0.2.0/salat/__init__.py
--rw-r--r--   0 zainhussaini   (501) staff       (20)    13921 2022-03-06 20:28:14.000000 salat-0.2.0/salat/calculations.py
--rw-r--r--   0 zainhussaini   (501) staff       (20)     8676 2022-03-06 20:00:21.000000 salat-0.2.0/salat/methods.py
-drwxr-xr-x   0 zainhussaini   (501) staff       (20)        0 2022-03-06 20:52:59.277168 salat-0.2.0/salat.egg-info/
--rw-r--r--   0 zainhussaini   (501) staff       (20)     4457 2022-03-06 20:52:59.000000 salat-0.2.0/salat.egg-info/PKG-INFO
--rw-r--r--   0 zainhussaini   (501) staff       (20)      199 2022-03-06 20:52:59.000000 salat-0.2.0/salat.egg-info/SOURCES.txt
--rw-r--r--   0 zainhussaini   (501) staff       (20)        1 2022-03-06 20:52:59.000000 salat-0.2.0/salat.egg-info/dependency_links.txt
--rw-r--r--   0 zainhussaini   (501) staff       (20)        6 2022-03-06 20:52:59.000000 salat-0.2.0/salat.egg-info/top_level.txt
--rw-r--r--   0 zainhussaini   (501) staff       (20)       38 2022-03-06 20:52:59.278135 salat-0.2.0/setup.cfg
--rw-r--r--   0 zainhussaini   (501) staff       (20)      839 2022-03-06 20:50:50.000000 salat-0.2.0/setup.py
+drwxr-xr-x   0 zainhussaini   (501) staff       (20)        0 2023-05-27 07:56:47.626066 salat-1.0.1/
+-rw-r--r--   0 zainhussaini   (501) staff       (20)     1053 2022-03-06 20:08:57.000000 salat-1.0.1/LICENSE
+-rw-r--r--   0 zainhussaini   (501) staff       (20)     4246 2023-05-27 07:56:47.624877 salat-1.0.1/PKG-INFO
+-rw-r--r--   0 zainhussaini   (501) staff       (20)     3813 2023-05-27 06:54:58.000000 salat-1.0.1/README.md
+drwxr-xr-x   0 zainhussaini   (501) staff       (20)        0 2023-05-27 07:56:47.617523 salat-1.0.1/salat/
+-rw-r--r--   0 zainhussaini   (501) staff       (20)       62 2021-10-23 22:23:49.000000 salat-1.0.1/salat/__init__.py
+-rw-r--r--   0 zainhussaini   (501) staff       (20)    13292 2023-05-27 06:54:58.000000 salat-1.0.1/salat/calculations.py
+-rw-r--r--   0 zainhussaini   (501) staff       (20)     7229 2023-05-27 06:54:58.000000 salat-1.0.1/salat/methods.py
+drwxr-xr-x   0 zainhussaini   (501) staff       (20)        0 2023-05-27 07:56:47.620224 salat-1.0.1/salat.egg-info/
+-rw-r--r--   0 zainhussaini   (501) staff       (20)     4246 2023-05-27 07:56:47.000000 salat-1.0.1/salat.egg-info/PKG-INFO
+-rw-r--r--   0 zainhussaini   (501) staff       (20)      277 2023-05-27 07:56:47.000000 salat-1.0.1/salat.egg-info/SOURCES.txt
+-rw-r--r--   0 zainhussaini   (501) staff       (20)        1 2023-05-27 07:56:47.000000 salat-1.0.1/salat.egg-info/dependency_links.txt
+-rw-r--r--   0 zainhussaini   (501) staff       (20)        6 2023-05-27 07:56:47.000000 salat-1.0.1/salat.egg-info/top_level.txt
+-rw-r--r--   0 zainhussaini   (501) staff       (20)       38 2023-05-27 07:56:47.626240 salat-1.0.1/setup.cfg
+-rw-r--r--   0 zainhussaini   (501) staff       (20)      839 2023-05-27 07:56:23.000000 salat-1.0.1/setup.py
+drwxr-xr-x   0 zainhussaini   (501) staff       (20)        0 2023-05-27 07:56:47.622478 salat-1.0.1/tests/
+-rw-r--r--   0 zainhussaini   (501) staff       (20)     8194 2023-05-27 06:54:58.000000 salat-1.0.1/tests/test_calculations.py
+-rw-r--r--   0 zainhussaini   (501) staff       (20)     6690 2023-05-27 06:54:58.000000 salat-1.0.1/tests/test_methods.py
+-rw-r--r--   0 zainhussaini   (501) staff       (20)     1198 2023-05-27 06:54:58.000000 salat-1.0.1/tests/test_readme_example.py
```

### Comparing `salat-0.2.0/LICENSE` & `salat-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `salat-0.2.0/PKG-INFO` & `salat-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: salat
-Version: 0.2.0
+Version: 1.0.1
 Summary: Tool to calculate accurate salat (prayer) times
 Home-page: https://github.com/zainhussaini/salat
 Author: Zain Hussaini
 Author-email: zih301@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # salat
 
 One of the pillars of Islam is salat, which is the act of praying five times a day. Each prayer has a specific time interval, defined in terms of the Sun's position so anyone anywhere in the world can know when it is time to pray.
 
 However with modern computation most Muslims use calculated prayer times to determine when to pray instead of watching the Sun. This package performs accurate calculations using orbital dynamics equations instead of common approximations, and native Python tools like datetime to calculate these times.
 
 ## Prayer Times
 
-In general terms, the time range of a prayer is from it's start until the start of the next prayer, except for Fajr which ends at sunrise and Isha which is recommended to end before midnight. The start of the prayer time intervals are the following:
+In general terms, the time range of a prayer is from it's start until the start of the next prayer, except for Fajr which ends at sunrise. The start of the prayer time intervals are the following:
 
 | Name | Start of Time Range |
 |------|------------|
 | Fajr | Beginning of twilight |
 | Sunrise | Sunrise. Note that this marks the end of Fajr |
 | Dhuhr | When the Sun passes its zenith |
 | Asr | When the length of a shadow is the same as the length of the object (or with Hanafi method, twice the length of the object) plus its length when the Sun is at zenith |
 | Maghrib | Sunset |
 | Isha | When the red light of sunset is gone |
-| Midnight | Halfway point of the night. Note that this marks the recommended end of Isha |
 
 However there are various methods and standards for what exact times these general terms correspond to. For example, according to the Muslim World League, Fajr starts when the altitude of the Sun is 18 degrees below the horizon, while the Islamic Society of North America determined it's when the sun is 15 degrees below the horizon.
 
 ## Motivation
 
 There are many websites with prayer time tables and apps that show automatically updating prayer times for your location for each day. However there are not many Python ones, and they either query the websites for time tables or use approximate methods.
 
@@ -90,24 +88,21 @@
     readable_time = time.strftime("%m/%d/%Y, %I:%M:%S %p %Z")
     table.append([name, readable_time])
 print(tabulate.tabulate(table, headers='firstrow'))
 ```
 
 Output
 ```
-Name      Time
---------  ---------------------------
-fajr      01/01/2000, 05:58:15 AM EST
-sunrise   01/01/2000, 07:20:09 AM EST
-dhuhr     01/01/2000, 11:59:25 AM EST
-asr       01/01/2000, 02:20:58 PM EST
-maghrib   01/01/2000, 04:38:50 PM EST
-isha      01/01/2000, 06:00:44 PM EST
-midnight  01/01/2000, 11:59:33 PM EST
+Name     Time
+-------  ---------------------------
+fajr     01/01/2000, 05:58:15 AM EST
+sunrise  01/01/2000, 07:20:09 AM EST
+dhuhr    01/01/2000, 11:59:25 AM EST
+asr      01/01/2000, 02:20:58 PM EST
+maghrib  01/01/2000, 04:38:50 PM EST
+isha     01/01/2000, 06:00:44 PM EST
 ```
 
 ## Planned features
 1. Adjustment for higher altitudes
 2. Options for Isha/Fajr calculation in high altitudes based on "middle of the night" and "sevent of the night" methods
 3. Add additional calculation methods
-
-
```

### Comparing `salat-0.2.0/README.md` & `salat-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 
 One of the pillars of Islam is salat, which is the act of praying five times a day. Each prayer has a specific time interval, defined in terms of the Sun's position so anyone anywhere in the world can know when it is time to pray.
 
 However with modern computation most Muslims use calculated prayer times to determine when to pray instead of watching the Sun. This package performs accurate calculations using orbital dynamics equations instead of common approximations, and native Python tools like datetime to calculate these times.
 
 ## Prayer Times
 
-In general terms, the time range of a prayer is from it's start until the start of the next prayer, except for Fajr which ends at sunrise and Isha which is recommended to end before midnight. The start of the prayer time intervals are the following:
+In general terms, the time range of a prayer is from it's start until the start of the next prayer, except for Fajr which ends at sunrise. The start of the prayer time intervals are the following:
 
 | Name | Start of Time Range |
 |------|------------|
 | Fajr | Beginning of twilight |
 | Sunrise | Sunrise. Note that this marks the end of Fajr |
 | Dhuhr | When the Sun passes its zenith |
 | Asr | When the length of a shadow is the same as the length of the object (or with Hanafi method, twice the length of the object) plus its length when the Sun is at zenith |
 | Maghrib | Sunset |
 | Isha | When the red light of sunset is gone |
-| Midnight | Halfway point of the night. Note that this marks the recommended end of Isha |
 
 However there are various methods and standards for what exact times these general terms correspond to. For example, according to the Muslim World League, Fajr starts when the altitude of the Sun is 18 degrees below the horizon, while the Islamic Society of North America determined it's when the sun is 15 degrees below the horizon.
 
 ## Motivation
 
 There are many websites with prayer time tables and apps that show automatically updating prayer times for your location for each day. However there are not many Python ones, and they either query the websites for time tables or use approximate methods.
 
@@ -75,22 +74,21 @@
     readable_time = time.strftime("%m/%d/%Y, %I:%M:%S %p %Z")
     table.append([name, readable_time])
 print(tabulate.tabulate(table, headers='firstrow'))
 ```
 
 Output
 ```
-Name      Time
---------  ---------------------------
-fajr      01/01/2000, 05:58:15 AM EST
-sunrise   01/01/2000, 07:20:09 AM EST
-dhuhr     01/01/2000, 11:59:25 AM EST
-asr       01/01/2000, 02:20:58 PM EST
-maghrib   01/01/2000, 04:38:50 PM EST
-isha      01/01/2000, 06:00:44 PM EST
-midnight  01/01/2000, 11:59:33 PM EST
+Name     Time
+-------  ---------------------------
+fajr     01/01/2000, 05:58:15 AM EST
+sunrise  01/01/2000, 07:20:09 AM EST
+dhuhr    01/01/2000, 11:59:25 AM EST
+asr      01/01/2000, 02:20:58 PM EST
+maghrib  01/01/2000, 04:38:50 PM EST
+isha     01/01/2000, 06:00:44 PM EST
 ```
 
 ## Planned features
 1. Adjustment for higher altitudes
 2. Options for Isha/Fajr calculation in high altitudes based on "middle of the night" and "sevent of the night" methods
 3. Add additional calculation methods
```

### Comparing `salat-0.2.0/salat/calculations.py` & `salat-1.0.1/salat/calculations.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,34 +2,33 @@
 from typing import Callable
 import math
 
 
 def eot_decl(time: dt.datetime) -> "tuple[dt.timedelta, float]":
     """Calculates the equation of time and Sun's declination at a given time.
 
-    The term equation of time referes to the difference between mean solar time
-    (what you would get if the sun had uniform motion along the celestial
-    equator) and apparent solar time (what you would get by measuing the angle
-    of the sun and calculating the time). This is because the ecliptic is tilted
-    relative to Earth's equator and the Earth's orbit has eccentricity. See
-    https://en.wikipedia.org/wiki/Equation_of_time
+    The term equation of time referes to the difference between mean solar time (what you would get
+    if the sun had uniform motion along the celestial equator) and apparent solar time (what you
+    would get by measuing the angle of the sun and calculating the time). This is because the
+    ecliptic is tilted relative to Earth's equator and the Earth's orbit has eccentricity.
+    See https://en.wikipedia.org/wiki/Equation_of_time
 
-    The declination of the sun is the angle between the Sun's rays and the plane
-    of Earth's equator. It's periodic with the orbit of Earth around the Sun.
+    The declination of the sun is the angle between the Sun's rays and the plane of Earth's equator.
+    It's periodic with the orbit of Earth around the Sun.
     See https://en.wikipedia.org/wiki/Position_of_the_Sun
 
     Args:
         time (datetime): time to calculate equation of time and declination for
 
     Returns:
         float: equation of time (in minutes)
         float: declination of sun (in radians)
     """
     # January 1, 2000 at noon in UTC
-    utc = dt.timezone(dt.timedelta())
+    utc = dt.timezone.utc
     epoch = dt.datetime(2000, 1, 1, 12, tzinfo=utc)
     days_since_epoch = (time - epoch).total_seconds() / 60 / 60 / 24
 
     # e = 0.016709
     # lam_p = 4.938201
     # epsilon = 0.409093
 
@@ -40,15 +39,15 @@
     epsilon = math.radians(23.4393 - 0.013 * y100 - 2e-7 * y100 ** 2 + 5e-7 * y100 ** 3)
 
     MD = 6.24004077  # M at epoch (Jan 1 2000 at noon)
     TY = 365.2596358  # days in a year
     D = days_since_epoch % TY
     M = MD + 2 * math.pi * D / TY
     M = M % (2 * math.pi)
-    E = KeplerSolve(M, e)
+    E = kepler_solve(M, e)
 
     nu = math.acos((math.cos(E) - e) / (1 - e * math.cos(E)))
     if E > math.pi:
         nu = 2 * math.pi - nu
 
     lam = nu + lam_p
     # put lam in range [0, 2*pi)
@@ -76,15 +75,15 @@
     eot_min = eot_rad / (2 * math.pi) * 60 * 24
     eot = dt.timedelta(minutes=eot_min)
     decl = math.asin(math.sin(epsilon) * math.sin(lam))
 
     return eot, decl
 
 
-def KeplerSolve(M: float, e: float) -> float:
+def kepler_solve(M: float, e: float) -> float:
     """Solves Kepler's equation inverse problem for elliptical orbits.
 
     Args:
         M (float): mean anomaly
         e (float): eccentricity
 
     Returns:
@@ -98,47 +97,51 @@
     while not math.isclose(M, E - e * math.sin(E)):
         E = E - (E - e * math.sin(E) - M) / (1 - e * math.cos(E))
         # E = M + e * math.sin(E)
     return E
 
 
 def calc_altitude(shadow_factor: float, declination: float, latitude: float) -> float:
-    """Calculates altitude when shadow of object is show_factor times the height
-    of the object.
+    """Calculates altitude when shadow of object is shadow_factor times the height of the object
+    plus the length at zenith.
 
     Args:
         shadow_factor (float): Multiplication factor from height to shadow length
         declination (float): Declination of sun in radians
         latitude (float): The latitude in degrees North
 
     Returns:
         float: The Sun's altitude below the horizon in radians
     """
     phi = math.radians(latitude)
     delta = declination
-    alt = math.atan(1 / (shadow_factor + math.tan(phi - delta)))
+
+    # See https://en.wikipedia.org/wiki/Salah_times#Time_calculation
+    shadow_factor_zenith = abs(math.tan(phi - delta))
+    alt = math.atan(1 / (shadow_factor + shadow_factor_zenith))
+
     return alt
 
 
 def timedelta_at_altitude(altitude: float, declination: float, latitude: float) -> dt.timedelta:
     """Calculates the difference from zenith to the time when Sun is at altitude.
 
     Args:
-        altitude (float): Altitude of sun in radians
+        altitude (float): Altitude of sun above the horizon in radians
         declination (float): Declination of sun in radians
         latitude (float): Latitude of position on Earth in degrees North
 
     Returns:
         timedelta: Offset from zenith. Note that this is always positive
     """
     alpha = altitude
     phi = math.radians(latitude)
     delta = declination
 
-    numerator = -math.sin(alpha) - math.sin(phi) * math.sin(delta)
+    numerator = math.sin(alpha) - math.sin(phi) * math.sin(delta)
     denominator = math.cos(phi) * math.cos(delta)
     cos_hour_rad = numerator / denominator
     if cos_hour_rad < -1 or cos_hour_rad > 1:
         raise ValueError("Sun does not reach altitude")
 
     hour_rad = math.acos(cos_hour_rad)
     hours = hour_rad / (2 * math.pi) * 24
@@ -150,21 +153,20 @@
 def linear_interpolation(
     diff_function: Callable[[dt.datetime], dt.timedelta],
     guess1: dt.datetime,
     guess2: dt.datetime,
 ):
     """Uses linear interpolation to calculate when diff_function ouputs zero.
 
-    More specifically, this uses the secant method to calculate guess such that
-    diff_function(guess) is zero. For more information about the secant method
-    see https://en.wikipedia.org/wiki/Secant_method
+    More specifically, this uses the secant method to calculate guess such that diff_function(guess)
+    is zero. For more information about the secant method
+    See https://en.wikipedia.org/wiki/Secant_method
 
     Args:
-        diff_function (Callable[[datetime, datetime], timedelta]): The
-            function to find the root for
+        diff_function (Callable[[datetime, datetime], timedelta]): The function to find the root for
         guess1 (datetime): First guess
         guess2 (datetime): Second guess (cannot be the same as first guess)
 
     Returns:
         datetime: input to diff_function which results in zero timedelta output
     """
     if math.isclose((guess1 - guess2).total_seconds(), 0):
@@ -182,32 +184,28 @@
         diff3 = diff_function(guess3)
 
         guess1, diff1 = guess2, diff2
         guess2, diff2 = guess3, diff3
     return guess1
 
 
-def time_zenith(local_noon: dt.datetime, longitude: float) -> dt.datetime:
-    """Calculates time of Sun reaching it's zenith on date specified by local
-    noon time, at longitude
+def time_zenith(date: dt.date, longitude: float) -> dt.datetime:
+    """Calculates time of Sun reaching its zenith on a date.
 
     Args:
-        local_noon (datetime): The datetime corresponding to noon in local timezone
+        date (date): The utc date for which the zenith should be found
         longitude (float): The longitude in degrees East
 
     Returns:
-        datetime: The specific time of zenith in same timezone as local_noon
+        datetime: The specific time of zenith. The zenith found will be the closest to utc noon on
+            the given date
     """
-    # local_noon = utc_noon + timezone_offset
-    # zenith = utc_noon + dt.timedelta(hours=longitude / 15) - eot
-    # find utc_noon such that dhuhr(utc_noon) is approx local_noon
-    utc_noon_approx = local_noon + dt.timedelta(hours=longitude / 15)
-    utc_noon_approx = utc_noon_approx.astimezone(dt.timezone.utc)
-    utcna = utc_noon_approx
-    utc_noon = dt.datetime(utcna.year, utcna.month, utcna.day, 12, tzinfo=dt.timezone.utc)
+    # Calculate when sun will be at zenith ignoring equation of time (eot)
+    utc_noon = dt.datetime(date.year, date.month, date.day, 12, tzinfo=dt.timezone.utc)
+    time_zenith_approx = utc_noon - dt.timedelta(hours=longitude/15)
 
     # The equation of time depends on the date (and therefore changes slightly
     # over the day) the time of zenith depends on the equation of time. therefore
     # this is a circular dependency, so use interpolation method to find
     # solution. However equation of time is periodic over year scales, so this
     # is not that necessary, but also only takes 3 iterations usually.
 
@@ -216,75 +214,67 @@
     #   declination and the guess itself
     # here x is guess and f(x) is diff (found with calc_difference)
 
     def calc_difference(guess: dt.datetime) -> dt.timedelta:
         """Using guess to calculate eot, calculate the time of dhuhr, and return
         difference between guess and calculated dhuhr.
         """
-        eot, declination = eot_decl(guess)
-        actual = utc_noon - dt.timedelta(hours=longitude / 15) - eot
+        eot, _ = eot_decl(guess)
+        actual = utc_noon - dt.timedelta(hours=longitude/15) - eot
         return actual - guess
 
-    # guess is when sun would be at zenith ignoring eot
-    guess = utc_noon - dt.timedelta(hours=longitude / 15)
     # eot is usually between -14 to +16 minutes, so bound that by guess1 and guess2
-    guess1 = guess - dt.timedelta(minutes=20)
-    guess2 = guess + dt.timedelta(minutes=20)
+    guess1 = time_zenith_approx - dt.timedelta(minutes=20)
+    guess2 = time_zenith_approx + dt.timedelta(minutes=20)
 
     return linear_interpolation(calc_difference, guess1, guess2)
 
 
 def time_altitude(
-    local_noon: dt.datetime,
+    zenith: dt.datetime,
     altitude: float,
-    longitude: float,
     latitude: float,
     rising: bool,
 ) -> dt.datetime:
-    """Calculates the time when Sun's altitude below the horizon is as given.
+    """Calculates the time when Sun's altitude is as given.
 
-    There are generally two times in a day when the Sun's altitude is a certain
-    value, one when the Sun is rising and one when it is setting. Specify which
-    one with the rising parameter.
+    There are generally two times in a day when the Sun's altitude is a certain value, one when the
+    Sun is rising and one when it is setting. Specify which one with the rising parameter.
 
     Args:
-        local_noon (datetime): The datetime corresponding to noon in local timezone
-        altitude (float): The desired altitude of the Sun BELOW THE HORIZON at
-            the output time, in radians
-        longitude (float): The longitude in degrees East
+        zenith (datetime): The datetime corresponding to zenith of the day
+        altitude (float): The desired altitude of the Sun above the horizon at the output time, in
+            radians
         latitude (float): The latitude in degrees North
-        rising (bool): Whether to calculate first time (before zenith, when Sun
-            is rising) or to calculate the second time (after zenith, when sun is
-            setting)
+        rising (bool): Whether to calculate first time (before zenith, when Sun is rising) or to
+            calculate the second time (after zenith, when sun is setting)
 
     Returns:
-        datetime: The time on the given date when Sun's altitude is as given and
-            it is either rising or setting, depending on value of rising
+        datetime: The time on the given date when Sun's altitude is as given and it is either rising
+            or setting, depending on value of rising
     """
-    # TODO: error checking to see if altitude is possible (timedelta_at_altitude)
-    # will handle it probably, but make it more explicit
-    zenith = time_zenith(local_noon, longitude)
-
-    # The declination depends on the date (and therefore changes slightly over
-    # the day), and the time when the sun is at a given altitude depends on the
-    # declination therefore this is a circular dependency, so use interpolation
-    # method to find solution. However equation of time is periodic over year
-    # scales, so this is not that necessary, but also only takes 3 iterations
+    # TODO: error checking to see if altitude is possible. timedelta_at_altitude will handle it
+    # probably, but make it more explicit
+
+    # The declination depends on the date (and therefore changes slightly over the day), and the
+    # time when the sun is at a given altitude depends on the declination therefore this is a
+    # circular dependency, so use interpolation method to find solution. However equation of time is
+    # periodic over year scales, so this is not that necessary, but also only takes 3 iterations
     # usually.
 
     # x is the datetime guess
-    # f(x) is the difference between time calculated using the guess's
-    #   declination and the guess itself
+    # f(x) is the difference between time calculated using the guess's declination and the guess
+    #   itself
     # here x is guess and f(x) is diff (found with calc_difference)
 
     def calc_difference(guess: dt.datetime) -> dt.timedelta:
-        """Using guess to calculate declination, calculate the time of when Sun
-        is at altitude, and return difference between guess and calculated time.
+        """Using guess to calculate declination, calculate the time of when Sun is at altitude, and
+        return difference between guess and calculated time.
         """
-        eot, declination = eot_decl(guess)
+        _, declination = eot_decl(guess)
         T = timedelta_at_altitude(altitude, declination, latitude)
         if rising:
             actual = zenith - T
         else:
             actual = zenith + T
         return actual - guess
 
@@ -297,57 +287,49 @@
         guess1 = zenith
         guess2 = zenith + dt.timedelta(hours=12)
 
     return linear_interpolation(calc_difference, guess1, guess2)
 
 
 def time_shadow_factor(
-    local_noon: dt.datetime,
+    zenith: dt.datetime,
     shadow_factor: float,
-    longitude: float,
     latitude: float,
     rising: bool,
 ) -> dt.datetime:
-    """Calculates the time when shadow of an object is shadow_factor times its
-    height, plus the length at zenith.
+    """Calculates the time when shadow of an object is shadow_factor times its height, plus the
+    length at zenith.
 
     Args:
-        local_noon (datetime): The datetime corresponding to noon in local timezone
+        zenith (datetime): The datetime corresponding to the zenith of the day
         shadow_factor (float): Multiplication factor from height to shadow length
-        longitude (float): The longitude in degrees East
         latitude (float): The latitude in degrees North
-        rising (bool): Whether to calculate first time (before zenith, when Sun
-            is rising) or to calculate the second time (after zenith, when sun is
-            setting)
+        rising (bool): Whether to calculate first time (before zenith, when Sun is rising) or to
+            calculate the second time (after zenith, when sun is setting)
 
     Returns:
-        datetime: The time on the given date when shadow factor is as given and
-            it is either rising or setting, depending on value of rising
+        datetime: The time on the given date when shadow factor is as given and it is either rising
+            or setting, depending on value of rising
     """
-    zenith = time_zenith(local_noon, longitude)
-
-    # the declination depends on the date (and therefore changes slightly over
-    # the day) the time when the sun is at a given altitude depends on the
-    # declination therefore this is a circular dependency, so use interpolation
-    # method to find solution
+    # The declination depends on the date (and therefore changes slightly over the day) the time
+    # when the sun is at a given altitude depends on the declination therefore this is a circular
+    # dependency, so use interpolation method to find solution
 
     # x is the datetime guess
     # f(x) is the difference between time calculated using the guess's
     #   declination and the guess itself
     # here x is guess and f(x) is diff (found with calc_difference)
 
     def calc_difference(guess: dt.datetime) -> dt.timedelta:
-        """Using guess to calculate declination, calculate the time of when
-        shadow is at given length, and return difference between guess and
-        calculated time.
+        """Using guess to calculate declination, calculate the time of when shadow is at given
+        length, and return difference between guess and calculated time.
         """
-        eot, declination = eot_decl(guess)
+        _, declination = eot_decl(guess)
         altitude = calc_altitude(shadow_factor, declination, latitude)
-        # negative altitude since timedelta_at_altitude uses altitude positive for below the horizon
-        T = timedelta_at_altitude(-altitude, declination, latitude)
+        T = timedelta_at_altitude(altitude, declination, latitude)
         if rising:
             actual = zenith - T
         else:
             actual = zenith + T
         return actual - guess
 
     if rising:
```

### Comparing `salat-0.2.0/salat/methods.py` & `salat-1.0.1/salat/methods.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,141 +27,113 @@
         self,
         fajr_altitude_deg: float,
         isha_altitude_deg: float,
         asr_method: AsrMethod = AsrMethod.STANDARD,
     ):
         """General system to define a method using Fajr and Isha altitudes.
 
-        Asr calculation method is provided as an arugment, and Fajr is when Sun
-        is at fajr_altitude_deg below the horizon. Isha is similarly when Sun is
-        at isha_altitude_deg below the horizon. Midnight is halfway between
-        sunset and sunrise. Sunrise is when the Sun is 0.833 degrees below the
-        horizon (accounting for diameter and atmospheric refraction) and Maghrib
-        is at sunset, which is at the same angle (0.833 degrees) except after
-        noon. Dhuhr is when sun is at it's peak, and Asr is when the shadow of
-        an object is either the same length as the height of the object, or
-        twice that length, depending on the asr_method provided.
+        Asr calculation method is provided as an arugment, and Fajr is when Sun is at
+        fajr_altitude_deg below the horizon. Isha is similarly when Sun is at isha_altitude_deg
+        below the horizon. Sunrise is when the Sun is 0.833 degrees below the horizon (accounting
+        for diameter and atmospheric refraction) and Maghrib is at sunset, which is at the same
+        angle (0.833 degrees) except after noon. Dhuhr is when sun is at it's peak, and Asr is when
+        the shadow of an object is either the same length as the height of the object, or twice that
+        length, depending on the asr_method provided.
 
         Raises:
             ValueError: If asr_method is not of type AsrMethod
 
 
         Args:
             fajr_altitude_deg (float): Altitude of Sun for Fajr in degrees below horizon
             isha_altitude_deg (float): Altitude of Sun for Isha in degrees below horizon
-            asr_method (AsrMethod, optional): Method to calculate Asr time.
-                Defaults to AsrMethod.STANDARD.
+            asr_method (AsrMethod, optional): Method to calculate Asr time. Defaults to
+                AsrMethod.STANDARD.
         """
         self.asr_method = asr_method
 
         if self.asr_method == AsrMethod.STANDARD:
             self.shadow_factor = 1
         elif self.asr_method == AsrMethod.HANAFI:
             self.shadow_factor = 2
         else:
             raise ValueError(f"Unknown AsrMethod {self.asr_method}")
 
-        self.fajr_altitude = math.radians(fajr_altitude_deg)
-        self.isha_altitude = math.radians(isha_altitude_deg)
-        self.sunset_altitude = math.radians(0.833)
+        self.fajr_altitude = -math.radians(fajr_altitude_deg)
+        self.isha_altitude = -math.radians(isha_altitude_deg)
+        self.sunset_altitude = -math.radians(0.833)
 
     def calc_times(
         self, date: dt.date, timezone: dt.tzinfo, longitude: float, latitude: float
     ) -> "dict[str, dt.datetime]":
-        """Calculates prayer times including sunrise and midnight.
+        """Calculates prayer times.
 
         Args:
-            date (dt.date): Date to calculate the prayer times for. Note that
-                "midnight" might be past 12 am therefore on next day
+            date (dt.date): Date to calculate the prayer times for. This centers dhuhr on the date
+                and the other prayer times are calculated surrounding it.
             timezone (dt.tzinfo): Timezone of the output datetimes
             longitude (float): Longitude of position in degrees East
             latitude (float): Latitude of position in degrees North
 
         Returns:
             dict[str, dt.datetime]: dictionary from time of interest (string) to time
         """
-        local_noon = dt.datetime(date.year, date.month, date.day, 12).astimezone(timezone)
+        # use zenith as reference point for other calculations.
+        zenith = time_zenith(date, longitude)
 
-        fajr = time_altitude(local_noon, self.fajr_altitude, longitude, latitude, rising=True)
-        sunrise = time_altitude(local_noon, self.sunset_altitude, longitude, latitude, rising=True)
-        dhuhr = time_zenith(local_noon, longitude)
-        asr = time_shadow_factor(local_noon, self.shadow_factor, longitude, latitude, rising=False)
-        maghrib = time_altitude(local_noon, self.sunset_altitude, longitude, latitude, rising=False)
-        isha = time_altitude(local_noon, self.isha_altitude, longitude, latitude, rising=False)
-
-        sunset = maghrib
-        next_local_noon = local_noon + dt.timedelta(days=1)
-        next_sunrise = time_altitude(next_local_noon, self.sunset_altitude, longitude, latitude, rising=True)
-        midnight = sunset + (next_sunrise - sunset) / 2
+        fajr = time_altitude(zenith, self.fajr_altitude, latitude, True)
+        sunrise = time_altitude(zenith, self.sunset_altitude, latitude, True)
+        asr = time_shadow_factor(zenith, self.shadow_factor, latitude, False)
+        maghrib = time_altitude(zenith, self.sunset_altitude, latitude, False)
+        isha = time_altitude(zenith, self.isha_altitude, latitude, False)
 
         times = {
             "fajr": fajr,
             "sunrise": sunrise,
-            "dhuhr": dhuhr,
+            "dhuhr": zenith,
             "asr": asr,
             "maghrib": maghrib,
             "isha": isha,
-            "midnight": midnight,
         }
 
         for name in times:
             times[name] = times[name].astimezone(timezone)
         return times
 
 
 class TehranMethod(GeneralMethod):
-    """Uses Fajr angle 17.7 deg, Isha angle 14 deg, Maghrib angle 4.5, midnight
-    between sunset and Fajr"""
+    """Uses Fajr angle 17.7 deg, Isha angle 14 deg, Maghrib angle 4.5"""
 
     def __init__(self, asr_method: AsrMethod = AsrMethod.STANDARD):
         super().__init__(17.7, 14, asr_method=asr_method)
 
     def calc_times(self, date: dt.date, timezone: dt.tzinfo, longitude: float, latitude: float):
-        local_noon = dt.datetime(date.year, date.month, date.day, 12).astimezone(timezone)
-
-        magrib_altitude = math.radians(4.5)
         times = super().calc_times(date, timezone, longitude, latitude)
-        sunset = times["maghrib"]
 
         # maghrib time is different
-        maghrib = time_altitude(local_noon, magrib_altitude, longitude, latitude, rising=False)
-        times["maghrib"] = maghrib
-
-        # midnight is different, it is between sunset and fajr
-        next_local_noon = local_noon + dt.timedelta(days=1)
-        next_fajr = time_altitude(next_local_noon, self.fajr_altitude, longitude, latitude, rising=True)
-        midnight = sunset + (next_fajr - sunset) / 2
-        times["midnight"] = midnight
+        zenith = time_zenith(date, longitude)
+        magrib_altitude = -math.radians(4.5)
+        times["maghrib"] = time_altitude(zenith, magrib_altitude, latitude, rising=False)
 
         return times
 
 
 class JafariMethod(GeneralMethod):
-    """Uses Fajr angle 16 deg, Isha angle 14 deg, Maghrib angle 4 deg, midnight
-    between sunset and Fajr"""
+    """Uses Fajr angle 16 deg, Isha angle 14 deg, Maghrib angle 4 deg"""
 
     def __init__(self, asr_method: AsrMethod = AsrMethod.STANDARD):
         super().__init__(16, 14, asr_method=asr_method)
 
     def calc_times(self, date: dt.date, timezone: dt.tzinfo, longitude: float, latitude: float):
-        local_noon = dt.datetime(date.year, date.month, date.day, 12).astimezone(timezone)
-
-        magrib_altitude = math.radians(4)
         times = super().calc_times(date, timezone, longitude, latitude)
-        sunset = times["maghrib"]
 
         # maghrib time is different
-        maghrib = time_altitude(local_noon, magrib_altitude, longitude, latitude, rising=False)
-        times["maghrib"] = maghrib
-
-        # midnight is different, it is between sunset and fajr
-        next_local_noon = local_noon + dt.timedelta(days=1)
-        next_fajr = time_altitude(next_local_noon, self.fajr_altitude, longitude, latitude, rising=True)
-        midnight = sunset + (next_fajr - sunset) / 2
-        times["midnight"] = midnight
+        zenith = time_zenith(date, longitude)
+        magrib_altitude = -math.radians(4)
+        times["maghrib"] = time_altitude(zenith, magrib_altitude, latitude, rising=False)
 
         return times
 
 
 class MakkahMethod(GeneralMethod):
     """Uses Fajr angle 18.5 deg, Isha 90 minutes after Maghrib in general and
     120 during Ramadan.
```

### Comparing `salat-0.2.0/salat.egg-info/PKG-INFO` & `salat-1.0.1/salat.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: salat
-Version: 0.2.0
+Version: 1.0.1
 Summary: Tool to calculate accurate salat (prayer) times
 Home-page: https://github.com/zainhussaini/salat
 Author: Zain Hussaini
 Author-email: zih301@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # salat
 
 One of the pillars of Islam is salat, which is the act of praying five times a day. Each prayer has a specific time interval, defined in terms of the Sun's position so anyone anywhere in the world can know when it is time to pray.
 
 However with modern computation most Muslims use calculated prayer times to determine when to pray instead of watching the Sun. This package performs accurate calculations using orbital dynamics equations instead of common approximations, and native Python tools like datetime to calculate these times.
 
 ## Prayer Times
 
-In general terms, the time range of a prayer is from it's start until the start of the next prayer, except for Fajr which ends at sunrise and Isha which is recommended to end before midnight. The start of the prayer time intervals are the following:
+In general terms, the time range of a prayer is from it's start until the start of the next prayer, except for Fajr which ends at sunrise. The start of the prayer time intervals are the following:
 
 | Name | Start of Time Range |
 |------|------------|
 | Fajr | Beginning of twilight |
 | Sunrise | Sunrise. Note that this marks the end of Fajr |
 | Dhuhr | When the Sun passes its zenith |
 | Asr | When the length of a shadow is the same as the length of the object (or with Hanafi method, twice the length of the object) plus its length when the Sun is at zenith |
 | Maghrib | Sunset |
 | Isha | When the red light of sunset is gone |
-| Midnight | Halfway point of the night. Note that this marks the recommended end of Isha |
 
 However there are various methods and standards for what exact times these general terms correspond to. For example, according to the Muslim World League, Fajr starts when the altitude of the Sun is 18 degrees below the horizon, while the Islamic Society of North America determined it's when the sun is 15 degrees below the horizon.
 
 ## Motivation
 
 There are many websites with prayer time tables and apps that show automatically updating prayer times for your location for each day. However there are not many Python ones, and they either query the websites for time tables or use approximate methods.
 
@@ -90,24 +88,21 @@
     readable_time = time.strftime("%m/%d/%Y, %I:%M:%S %p %Z")
     table.append([name, readable_time])
 print(tabulate.tabulate(table, headers='firstrow'))
 ```
 
 Output
 ```
-Name      Time
---------  ---------------------------
-fajr      01/01/2000, 05:58:15 AM EST
-sunrise   01/01/2000, 07:20:09 AM EST
-dhuhr     01/01/2000, 11:59:25 AM EST
-asr       01/01/2000, 02:20:58 PM EST
-maghrib   01/01/2000, 04:38:50 PM EST
-isha      01/01/2000, 06:00:44 PM EST
-midnight  01/01/2000, 11:59:33 PM EST
+Name     Time
+-------  ---------------------------
+fajr     01/01/2000, 05:58:15 AM EST
+sunrise  01/01/2000, 07:20:09 AM EST
+dhuhr    01/01/2000, 11:59:25 AM EST
+asr      01/01/2000, 02:20:58 PM EST
+maghrib  01/01/2000, 04:38:50 PM EST
+isha     01/01/2000, 06:00:44 PM EST
 ```
 
 ## Planned features
 1. Adjustment for higher altitudes
 2. Options for Isha/Fajr calculation in high altitudes based on "middle of the night" and "sevent of the night" methods
 3. Add additional calculation methods
-
-
```

### Comparing `salat-0.2.0/setup.py` & `salat-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="salat",
-    version="0.2.0",
+    version="1.0.1",
     description="Tool to calculate accurate salat (prayer) times",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/zainhussaini/salat",
     author="Zain Hussaini",
     author_email="zih301@gmail.com",
     license="MIT",
```

