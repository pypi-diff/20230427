# Comparing `tmp/sgp4-2.8.tar.gz` & `tmp/sgp4-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sgp4-2.8.tar", last modified: Thu May  7 14:46:10 2020, max compression
+gzip compressed data, was "dist/sgp4-2.9.tar", last modified: Thu May 21 18:06:38 2020, max compression
```

## Comparing `sgp4-2.8.tar` & `sgp4-2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2020-05-07 14:46:09.000000 sgp4-2.8/
--rw-rw-r--   0 brandon   (1000) brandon   (1000)    17559 2020-05-07 14:46:09.000000 sgp4-2.8/PKG-INFO
-drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2020-05-07 14:46:09.000000 sgp4-2.8/extension/
--rw-rw-r--   0 brandon   (1000) brandon   (1000)   110037 2020-04-24 19:18:53.000000 sgp4-2.8/extension/SGP4.cpp
--rw-rw-r--   0 brandon   (1000) brandon   (1000)     6652 2020-01-30 17:12:29.000000 sgp4-2.8/extension/SGP4.h
--rw-rw-r--   0 brandon   (1000) brandon   (1000)    17825 2020-04-24 21:34:31.000000 sgp4-2.8/extension/wrapper.cpp
--rw-rw-r--   0 brandon   (1000) brandon   (1000)     2333 2020-05-07 14:45:20.000000 sgp4-2.8/setup.py
-drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2020-05-07 14:46:09.000000 sgp4-2.8/sgp4/
--rw-r-----   0 brandon   (1000) brandon   (1000)     8616 2019-12-09 20:17:01.000000 sgp4-2.8/sgp4/SGP4-VER.TLE
--rw-rw-r--   0 brandon   (1000) brandon   (1000)    12984 2020-05-07 14:45:11.000000 sgp4-2.8/sgp4/__init__.py
--rw-rw-r--   0 brandon   (1000) brandon   (1000)      813 2020-03-22 10:38:56.000000 sgp4-2.8/sgp4/api.py
--rw-rw-r--   0 brandon   (1000) brandon   (1000)     1706 2020-05-07 14:42:38.000000 sgp4-2.8/sgp4/conveniences.py
--rw-r-----   0 brandon   (1000) brandon   (1000)      375 2019-08-19 20:16:57.000000 sgp4-2.8/sgp4/earth_gravity.py
--rw-rw-r--   0 brandon   (1000) brandon   (1000)     3102 2020-04-20 20:10:46.000000 sgp4-2.8/sgp4/exporter.py
--rw-r-----   0 brandon   (1000) brandon   (1000)    19547 2020-01-30 16:01:05.000000 sgp4-2.8/sgp4/ext.py
--rw-rw-r--   0 brandon   (1000) brandon   (1000)     1417 2020-05-07 14:39:50.000000 sgp4-2.8/sgp4/functions.py
--rw-rw-r--   0 brandon   (1000) brandon   (1000)    10402 2020-04-21 17:23:14.000000 sgp4-2.8/sgp4/io.py
--rw-rw-r--   0 brandon   (1000) brandon   (1000)     7820 2020-04-24 21:34:31.000000 sgp4-2.8/sgp4/model.py
--rw-rw-r--   0 brandon   (1000) brandon   (1000)    74125 2020-04-24 21:34:31.000000 sgp4-2.8/sgp4/propagation.py
--rw-r-----   0 brandon   (1000) brandon   (1000)   140162 2019-12-09 20:18:24.000000 sgp4-2.8/sgp4/tcppver.out
--rw-rw-r--   0 brandon   (1000) brandon   (1000)    19936 2020-05-07 14:42:21.000000 sgp4-2.8/sgp4/tests.py
--rw-rw-r--   0 brandon   (1000) brandon   (1000)     2283 2020-03-21 15:13:43.000000 sgp4-2.8/sgp4/wrapper.py
--rw-rw-r--   0 brandon   (1000) brandon   (1000)      815 2020-04-24 21:34:31.000000 sgp4-2.8/sgp4/wulfgar.py
+drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2020-05-21 18:06:37.000000 sgp4-2.9/
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)    20645 2020-05-21 18:06:37.000000 sgp4-2.9/PKG-INFO
+drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2020-05-21 18:06:37.000000 sgp4-2.9/extension/
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)   110037 2020-04-24 19:18:53.000000 sgp4-2.9/extension/SGP4.cpp
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)     6652 2020-01-30 17:12:29.000000 sgp4-2.9/extension/SGP4.h
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)    18011 2020-05-21 18:03:40.000000 sgp4-2.9/extension/wrapper.cpp
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)     2333 2020-05-21 18:03:40.000000 sgp4-2.9/setup.py
+drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2020-05-21 18:06:37.000000 sgp4-2.9/sgp4/
+-rw-r-----   0 brandon   (1000) brandon   (1000)     8616 2019-12-09 20:17:01.000000 sgp4-2.9/sgp4/SGP4-VER.TLE
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)    15534 2020-05-21 18:03:40.000000 sgp4-2.9/sgp4/__init__.py
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)      852 2020-05-21 18:03:40.000000 sgp4-2.9/sgp4/api.py
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)     2307 2020-05-21 18:03:40.000000 sgp4-2.9/sgp4/conveniences.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)      375 2019-08-19 20:16:57.000000 sgp4-2.9/sgp4/earth_gravity.py
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)     3102 2020-04-20 20:10:46.000000 sgp4-2.9/sgp4/exporter.py
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)    17276 2020-05-21 18:03:40.000000 sgp4-2.9/sgp4/ext.py
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)     3120 2020-05-21 18:03:40.000000 sgp4-2.9/sgp4/functions.py
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)    10402 2020-05-21 13:30:36.000000 sgp4-2.9/sgp4/io.py
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)     8021 2020-05-21 18:03:40.000000 sgp4-2.9/sgp4/model.py
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)    74125 2020-04-24 21:34:31.000000 sgp4-2.9/sgp4/propagation.py
+-rw-r-----   0 brandon   (1000) brandon   (1000)   140162 2019-12-09 20:18:24.000000 sgp4-2.9/sgp4/tcppver.out
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)    21391 2020-05-21 18:03:40.000000 sgp4-2.9/sgp4/tests.py
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)     2283 2020-03-21 15:13:43.000000 sgp4-2.9/sgp4/wrapper.py
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)      815 2020-04-24 21:34:31.000000 sgp4-2.9/sgp4/wulfgar.py
```

### Comparing `sgp4-2.8/PKG-INFO` & `sgp4-2.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sgp4
-Version: 2.8
+Version: 2.9
 Summary: Track earth satellite TLE orbits using up-to-date 2010 version of SGP4
 Home-page: https://github.com/brandon-rhodes/python-sgp4
 Author: Brandon Rhodes
 Author-email: brandon@rhodesmill.org
 License: MIT
 Description: 
         This Python package computes the position and velocity of an
@@ -21,19 +21,27 @@
           source code from the official C++ version of SGP4.  You can call the
           routine directly, or through an array API that loops over arrays of
           satellites and arrays of times with machine code instead of Python.
         
         * Otherwise, a slower but reliable Python implementation of SGP4 is used
           instead.
         
-        Note that this package produces raw Earth-centered cartesian
-        coordinates.  It does not implement all the steps necessary to convert
-        satellite positions into geographic coordinates.  For that, look for a
-        comprehensive astronomy library that is built atop this one, like the
-        `Skyfield <http://rhodesmill.org/skyfield/>`_ library:
+        Note that the SGP4 propagator returns raw *x,y,z* Cartesian coordinates
+        in a “True Equator Mean Equinox” (TEME) reference frame that’s centered
+        on the Earth but does not rotate with it — an “Earth centered inertial”
+        (ECI) reference frame.  The SGP4 propagator itself does not implement
+        the math that’s necessary to convert these positions into more official
+        ECI frames like J2000 or the ICRF.  Nor does it provide conversion into
+        any Earth-centered Earth-fixed (ECEF) frames whose coordinates are fixed
+        with respect to the Earth’s surface, like the ITRF that defines latitude
+        and longitude.
+        
+        For conversions into other coordinate frames, look for a comprehensive
+        astronomy library that is built atop this one, like the `Skyfield
+        <http://rhodesmill.org/skyfield/>`_ library:
         
         http://rhodesmill.org/skyfield/earth-satellites.html
         
         Usage
         -----
         
         This library uses the same function names as the official C++ code, to
@@ -102,14 +110,68 @@
         >>> from sgp4.api import jday
         >>> jd, fr = jday(2019, 12, 9, 12, 0, 0)
         >>> jd
         2458826.5
         >>> fr
         0.5
         
+        Epoch
+        -----
+        
+        Over a given satellite’s lifetime, dozens or hundreds of different TLE
+        records will be produced as its orbit evolves.  Each TLE record
+        specifies the “epoch date” for which it is most accurate.  Typically a
+        TLE is only useful for a couple of weeks to either side of its epoch
+        date, beyond which its predictions become unreliable.
+        
+        Satellite objects natively provide their epoch as a two-digit year and
+        then a fractional number of days into the year:
+        
+        >>> satellite.epochyr
+        19
+        >>> satellite.epochdays
+        343.69339541
+        
+        Because Sputnik was launched in 1957, satellite element sets will never
+        refer to an earlier year, so years 57 through 99 mean 1957–1999 while 0
+        through 56 mean 2000–2056.  The TLE format will presumably be obsolete
+        in 2057 and have to be upgraded to 4-digit years.
+        
+        To turn the number of days and its fraction into a calendar date and
+        time, use the ``days2mdhms()`` function.
+        
+        >>> from sgp4.api import days2mdhms
+        >>> month, day, hour, minute, second = days2mdhms(19, 343.69339541)
+        >>> month
+        12
+        >>> day
+        9
+        >>> hour
+        16
+        >>> minute
+        38
+        >>> second
+        29.363424
+        
+        The SGP4 library also translates those two numbers into a Julian date
+        and fractional Julian date, since Julian dates are more commonly used in
+        astronomy.
+        
+        >>> satellite.jdsatepoch
+        2458826.5
+        >>> satellite.jdsatepochF
+        0.69339541
+        
+        Finally, a convenience function is available in the library if you need
+        the epoch date and time as Python ``datetime``.
+        
+        >>> from sgp4.conveniences import sat_epoch_datetime
+        >>> sat_epoch_datetime(satellite)
+        datetime.datetime(2019, 12, 9, 16, 38, 29, 363423, tzinfo=UTC)
+        
         Array Acceleration
         ------------------
         
         To avoid the expense of Python loops when you have many dates, you can
         pass them as arrays to another method that understands NumPy:
         
         >>> import numpy as np
@@ -251,15 +313,15 @@
         
         >>> sat = Satrec()
         >>> sat.sgp4init(
         ...     WGS72,           # gravity model
         ...     'i',             # 'a' = old AFSPC mode, 'i' = improved mode
         ...     5,               # satnum: Satellite number
         ...     18441.785,       # epoch: days since 1949 December 31 00:00 UT
-        ...     2.8098e-05,      # bstar: drag coefficient (kg/m2er)
+        ...     2.8098e-05,      # bstar: drag coefficient (/earth radii)
         ...     6.969196665e-13, # ndot: ballistic coefficient (revs/day)
         ...     0.0,             # nddot: second derivative of mean motion (revs/day^3)
         ...     0.1859667,       # ecco: eccentricity
         ...     5.7904160274885, # argpo: argument of perigee (radians)
         ...     0.5980929187319, # inclo: inclination (radians)
         ...     0.3373093125574, # mo: mean anomaly (radians)
         ...     0.0472294454407, # no_kozai: mean motion (radians/minute)
@@ -270,14 +332,18 @@
         subtract ``2433281.5`` days.
         
         The character provided as the second argument can be ``'a'`` to run the
         computations so that they are compatible with the old Air Force Space
         Command edition of the library, or ``'i'`` to run the new and improved
         version of the SGP4 algorithm.
         
+        You can also directly access a satellite’s orbital parameters by asking
+        for the attributes ``sat.epoch``, ``sat.bstar``, and so forth, using the
+        names given in the comments above.
+        
         Validation against the official algorithm
         -----------------------------------------
         
         This implementation passes all of the automated tests in the August 2010
         release of the reference implementation of SGP4 by Vallado et al., who
         originally published their revision of SGP4 in 2006:
         
@@ -316,14 +382,15 @@
         about it by reading the documentation from version 1.4 or earlier:
         
         https://pypi.org/project/sgp4/1.4/
         
         Changelog
         ---------
         
+        | 2020-05-21 — 2.9 — Added ``sat_epoch_datetime()``, expanded documentation around converting a satellite epoch to a date and time, and started rounding the epoch to exactly the digits provided in the TLE; and removed the ``Satrec.epoch`` attribute from Python fallback code to better match the C++ version.
         | 2020-05-07 — 2.8 — New function ``jday_datetime()`` is now available in the ``sgp4.conveniences`` module, thanks to Egemen Imre.
         | 2020-04-24 — 2.7 — New method ``sgp4init()`` (thank you, Chris Lewicki!) is available.
         | 2020-04-20 — 2.6 — New routine ``export_tle()`` (thank you, Egemen Imre!) is available. Improved how the accelerated C++ backend parses the ``intldesg`` string and the ``revnum`` integer.
         | 2020-03-22 — 2.5 — Gave the new accelerated ``twoline2rv()`` an optional argument that lets the user choose a non-standard set of gravity constants.
         | 2020-02-25 — 2.4 — Improved the ``jday()`` docstring; made the old legacy Python resilient if the day of the month is out-of-range (past the end of the month) in a TLE; and Mark Rutten fixed the C++ so it compiles on Windows!
         | 2020-02-04 — 2.3 — Removed experimental code that caused performance problems for users with Numba installed.
         | 2020-02-02 — 2.2 — A second release on Palindrome Day: fix the Satrec ``.epochyr`` attribute so it behaves the same way in Python as it does in the official C library, where it is only the last 2 digits of the year; and make ``.no`` available in the Python fallback case as well.
```

### Comparing `sgp4-2.8/extension/SGP4.cpp` & `sgp4-2.9/extension/SGP4.cpp`

 * *Files identical despite different names*

### Comparing `sgp4-2.8/extension/SGP4.h` & `sgp4-2.9/extension/SGP4.h`

 * *Files identical despite different names*

### Comparing `sgp4-2.8/extension/wrapper.cpp` & `sgp4-2.9/extension/wrapper.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -116,14 +116,18 @@
     SatrecObject *self = (SatrecObject*) cls->tp_alloc(cls, 0);
     if (!self)
         return NULL;
 
     SGP4Funcs::twoline2rv(line1, line2, ' ', ' ', 'i', whichconst,
                           dummy, dummy, dummy, self->satrec);
 
+    /* Usability bonus: round the fractional day to exactly the eight
+       digits specified in the TLE. */
+    self->satrec.jdsatepochF = round(self->satrec.jdsatepochF * 1e8) / 1e8;
+
     /* To avoid having scanf() interpret the "intldesg" as zero or as
        several fields, the C++ library changes spaces to periods and
        underscores.  Let's convert them back to avoid surprising users
        and to match our Python implementation. */
     if (self->satrec.intldesg[0] == '.')
          self->satrec.intldesg[0] = ' ';
     for (int i=1; i<11; i++)
```

### Comparing `sgp4-2.8/setup.py` & `sgp4-2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         # like these, adapted to as many platforms as possible, to use
         # multiple processors when available?
         # extra_compile_args=['-fopenmp'],
         # extra_link_args=['-fopenmp'],
     ))
 
 setup(name = 'sgp4',
-      version = '2.8',
+      version = '2.9',
       description = description,
       long_description = long_description,
       license = 'MIT',
       author = 'Brandon Rhodes',
       author_email = 'brandon@rhodesmill.org',
       url = 'https://github.com/brandon-rhodes/python-sgp4',
       classifiers = [
```

### Comparing `sgp4-2.8/sgp4/SGP4-VER.TLE` & `sgp4-2.9/sgp4/SGP4-VER.TLE`

 * *Files identical despite different names*

### Comparing `sgp4-2.8/sgp4/__init__.py` & `sgp4-2.9/sgp4/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,19 +15,27 @@
   source code from the official C++ version of SGP4.  You can call the
   routine directly, or through an array API that loops over arrays of
   satellites and arrays of times with machine code instead of Python.
 
 * Otherwise, a slower but reliable Python implementation of SGP4 is used
   instead.
 
-Note that this package produces raw Earth-centered cartesian
-coordinates.  It does not implement all the steps necessary to convert
-satellite positions into geographic coordinates.  For that, look for a
-comprehensive astronomy library that is built atop this one, like the
-`Skyfield <http://rhodesmill.org/skyfield/>`_ library:
+Note that the SGP4 propagator returns raw *x,y,z* Cartesian coordinates
+in a “True Equator Mean Equinox” (TEME) reference frame that’s centered
+on the Earth but does not rotate with it — an “Earth centered inertial”
+(ECI) reference frame.  The SGP4 propagator itself does not implement
+the math that’s necessary to convert these positions into more official
+ECI frames like J2000 or the ICRF.  Nor does it provide conversion into
+any Earth-centered Earth-fixed (ECEF) frames whose coordinates are fixed
+with respect to the Earth’s surface, like the ITRF that defines latitude
+and longitude.
+
+For conversions into other coordinate frames, look for a comprehensive
+astronomy library that is built atop this one, like the `Skyfield
+<http://rhodesmill.org/skyfield/>`_ library:
 
 http://rhodesmill.org/skyfield/earth-satellites.html
 
 Usage
 -----
 
 This library uses the same function names as the official C++ code, to
@@ -96,14 +104,68 @@
 >>> from sgp4.api import jday
 >>> jd, fr = jday(2019, 12, 9, 12, 0, 0)
 >>> jd
 2458826.5
 >>> fr
 0.5
 
+Epoch
+-----
+
+Over a given satellite’s lifetime, dozens or hundreds of different TLE
+records will be produced as its orbit evolves.  Each TLE record
+specifies the “epoch date” for which it is most accurate.  Typically a
+TLE is only useful for a couple of weeks to either side of its epoch
+date, beyond which its predictions become unreliable.
+
+Satellite objects natively provide their epoch as a two-digit year and
+then a fractional number of days into the year:
+
+>>> satellite.epochyr
+19
+>>> satellite.epochdays
+343.69339541
+
+Because Sputnik was launched in 1957, satellite element sets will never
+refer to an earlier year, so years 57 through 99 mean 1957–1999 while 0
+through 56 mean 2000–2056.  The TLE format will presumably be obsolete
+in 2057 and have to be upgraded to 4-digit years.
+
+To turn the number of days and its fraction into a calendar date and
+time, use the ``days2mdhms()`` function.
+
+>>> from sgp4.api import days2mdhms
+>>> month, day, hour, minute, second = days2mdhms(19, 343.69339541)
+>>> month
+12
+>>> day
+9
+>>> hour
+16
+>>> minute
+38
+>>> second
+29.363424
+
+The SGP4 library also translates those two numbers into a Julian date
+and fractional Julian date, since Julian dates are more commonly used in
+astronomy.
+
+>>> satellite.jdsatepoch
+2458826.5
+>>> satellite.jdsatepochF
+0.69339541
+
+Finally, a convenience function is available in the library if you need
+the epoch date and time as Python ``datetime``.
+
+>>> from sgp4.conveniences import sat_epoch_datetime
+>>> sat_epoch_datetime(satellite)
+datetime.datetime(2019, 12, 9, 16, 38, 29, 363423, tzinfo=UTC)
+
 Array Acceleration
 ------------------
 
 To avoid the expense of Python loops when you have many dates, you can
 pass them as arrays to another method that understands NumPy:
 
 >>> import numpy as np
@@ -212,15 +274,15 @@
 
 >>> sat = Satrec()
 >>> sat.sgp4init(
 ...     WGS72,           # gravity model
 ...     'i',             # 'a' = old AFSPC mode, 'i' = improved mode
 ...     5,               # satnum: Satellite number
 ...     18441.785,       # epoch: days since 1949 December 31 00:00 UT
-...     2.8098e-05,      # bstar: drag coefficient (kg/m2er)
+...     2.8098e-05,      # bstar: drag coefficient (/earth radii)
 ...     6.969196665e-13, # ndot: ballistic coefficient (revs/day)
 ...     0.0,             # nddot: second derivative of mean motion (revs/day^3)
 ...     0.1859667,       # ecco: eccentricity
 ...     5.7904160274885, # argpo: argument of perigee (radians)
 ...     0.5980929187319, # inclo: inclination (radians)
 ...     0.3373093125574, # mo: mean anomaly (radians)
 ...     0.0472294454407, # no_kozai: mean motion (radians/minute)
@@ -231,14 +293,18 @@
 subtract ``2433281.5`` days.
 
 The character provided as the second argument can be ``'a'`` to run the
 computations so that they are compatible with the old Air Force Space
 Command edition of the library, or ``'i'`` to run the new and improved
 version of the SGP4 algorithm.
 
+You can also directly access a satellite’s orbital parameters by asking
+for the attributes ``sat.epoch``, ``sat.bstar``, and so forth, using the
+names given in the comments above.
+
 Validation against the official algorithm
 -----------------------------------------
 
 This implementation passes all of the automated tests in the August 2010
 release of the reference implementation of SGP4 by Vallado et al., who
 originally published their revision of SGP4 in 2006:
 
@@ -277,14 +343,15 @@
 about it by reading the documentation from version 1.4 or earlier:
 
 https://pypi.org/project/sgp4/1.4/
 
 Changelog
 ---------
 
+| 2020-05-21 — 2.9 — Added ``sat_epoch_datetime()``, expanded documentation around converting a satellite epoch to a date and time, and started rounding the epoch to exactly the digits provided in the TLE; and removed the ``Satrec.epoch`` attribute from Python fallback code to better match the C++ version.
 | 2020-05-07 — 2.8 — New function ``jday_datetime()`` is now available in the ``sgp4.conveniences`` module, thanks to Egemen Imre.
 | 2020-04-24 — 2.7 — New method ``sgp4init()`` (thank you, Chris Lewicki!) is available.
 | 2020-04-20 — 2.6 — New routine ``export_tle()`` (thank you, Egemen Imre!) is available. Improved how the accelerated C++ backend parses the ``intldesg`` string and the ``revnum`` integer.
 | 2020-03-22 — 2.5 — Gave the new accelerated ``twoline2rv()`` an optional argument that lets the user choose a non-standard set of gravity constants.
 | 2020-02-25 — 2.4 — Improved the ``jday()`` docstring; made the old legacy Python resilient if the day of the month is out-of-range (past the end of the month) in a TLE; and Mark Rutten fixed the C++ so it compiles on Windows!
 | 2020-02-04 — 2.3 — Removed experimental code that caused performance problems for users with Numba installed.
 | 2020-02-02 — 2.2 — A second release on Palindrome Day: fix the Satrec ``.epochyr`` attribute so it behaves the same way in Python as it does in the official C library, where it is only the last 2 digits of the year; and make ``.no`` available in the Python fallback case as well.
```

### Comparing `sgp4-2.8/sgp4/api.py` & `sgp4-2.9/sgp4/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Public API that tries to import C++ module, but falls back to Python."""
 
-__all__ = 'Satrec', 'SatrecArray', 'jday', 'WGS72OLD', 'WGS72', 'WGS84'
+__all__ = ('Satrec', 'SatrecArray', 'WGS72OLD', 'WGS72', 'WGS84',
+           'jday', 'days2mdhms')
 
-from .functions import jday
+from .functions import jday, days2mdhms
 
 SGP4_ERRORS = {
     1: 'mean eccentricity is outside the range 0.0 to 1.0',
     2: 'nm is less than zero',
     3: 'perturbed eccentricity is outside the range 0.0 to 1.0',
     4: 'semilatus rectum is less than zero',
     5: '(error 5 no longer in use; it meant the satellite was underground)',
```

### Comparing `sgp4-2.8/sgp4/conveniences.py` & `sgp4-2.9/sgp4/conveniences.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 
 Higher-level libraries like Skyfield that use this one usually have
 their own date and time handling.  But for folks using this library by
 itself, native Python datetime handling could be convenient.
 
 """
 import datetime as dt
-from .functions import jday
+from .functions import days2mdhms, jday
 
 class _UTC(dt.tzinfo):
-     'UTC'
-     zero = dt.timedelta(0)
-     def utcoffset(self, datetime):
-          return self.zero
-     def tzname(self, datetime):
-          return 'UTC'
-     def dst(self, datetime):
-          return self.zero
+    'UTC'
+    zero = dt.timedelta(0)
+    def __repr__(self):
+        return 'UTC'
+    def dst(self, datetime):
+        return self.zero
+    def tzname(self, datetime):
+        return 'UTC'
+    def utcoffset(self, datetime):
+        return self.zero
 
 UTC = _UTC()
 
 def jday_datetime(datetime):
     """Return two floats that, when added, produce the specified Julian date.
 
     The first float returned gives the date, while the second float
@@ -50,7 +52,22 @@
     mon = u.month
     day = u.day
     hr = u.hour
     minute = u.minute
     sec = u.second + u.microsecond * 1e-6
 
     return jday(year, mon, day, hr, minute, sec)
+
+def sat_epoch_datetime(sat):
+    """Return the epoch of the given satellite as a Python datetime."""
+    year = sat.epochyr
+    year += 1900 + (year < 57) * 100
+    days = sat.epochdays
+    month, day, hour, minute, second = days2mdhms(year, days)
+    if month == 12 and day > 31:  # for that time the ISS epoch was "Dec 32"
+        year += 1
+        month = 1
+        day -= 31
+    second, fraction = divmod(second, 1.0)
+    second = int(second)
+    micro = int(fraction * 1e6)
+    return dt.datetime(year, month, day, hour, minute, second, micro, UTC)
```

### Comparing `sgp4-2.8/sgp4/exporter.py` & `sgp4-2.9/sgp4/exporter.py`

 * *Files identical despite different names*

### Comparing `sgp4-2.8/sgp4/ext.py` & `sgp4-2.9/sgp4/ext.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """Utility routines from "sgp4ext.cpp"."""
 
 from math import (acos, asinh, atan2, copysign, cos, fabs, fmod,
                   pi, sin, sinh, sqrt, tan)
+from .functions import days2mdhms
 
 undefined = None
 
 """
 /* -----------------------------------------------------------------------------
 *
 *                           function mag
@@ -479,81 +480,14 @@
           ((sec / 60.0 + minute) / 60.0 + hr) / 24.0  #  ut in days
           #  - 0.5*sgn(100.0*year + mon - 190002.5) + 0.5;
           )
 
 """
 /* -----------------------------------------------------------------------------
 *
-*                           procedure days2mdhms
-*
-*  this procedure converts the day of the year, days, to the equivalent month
-*    day, hour, minute and second.
-*
-*  algorithm     : set up array for the number of days per month
-*                  find leap year - use 1900 because 2000 is a leap year
-*                  loop through a temp value while the value is < the days
-*                  perform int conversions to the correct day and month
-*                  convert remainder into h m s using type conversions
-*
-*  author        : david vallado                  719-573-2600    1 mar 2001
-*
-*  inputs          description                    range / units
-*    year        - year                           1900 .. 2100
-*    days        - julian day of the year         0.0  .. 366.0
-*
-*  outputs       :
-*    mon         - month                          1 .. 12
-*    day         - day                            1 .. 28,29,30,31
-*    hr          - hour                           0 .. 23
-*    min         - minute                         0 .. 59
-*    sec         - second                         0.0 .. 59.999
-*
-*  locals        :
-*    dayofyr     - day of year
-*    temp        - temporary extended values
-*    inttemp     - temporary int value
-*    i           - index
-*    lmonth[12]  - int array containing the number of days per month
-*
-*  coupling      :
-*    none.
-* --------------------------------------------------------------------------- */
-"""
-
-def days2mdhms(year, days):
-
-     lmonth = (31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31);
-
-     dayofyr = int(days // 1.0);
-     #  ----------------- find month and day of month ----------------
-     if (year % 4) == 0:
-       lmonth = (31, 29, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31);
-
-     i = 1;
-     inttemp = 0;
-     while dayofyr > inttemp + lmonth[i-1] and i < 12:
-
-       inttemp = inttemp + lmonth[i-1];
-       i += 1;
-
-     mon = i;
-     day = dayofyr - inttemp;
-
-     #  ----------------- find hours minutes and seconds -------------
-     temp = (days - dayofyr) * 24.0;
-     hr   = int(temp // 1.0);
-     temp = (temp - hr) * 60.0;
-     minute  = int(temp // 1.0);
-     sec  = (temp - minute) * 60.0;
-
-     return mon, day, hr, minute, sec
-
-"""
-/* -----------------------------------------------------------------------------
-*
 *                           procedure invjday
 *
 *  this procedure finds the year, month, day, hour, minute and second
 *  given the julian date. tu can be ut1, tdt, tdb, etc.
 *
 *  algorithm     : set up starting values
 *                  find leap year - use 1900 because 2000 is a leap year
@@ -603,10 +537,10 @@
      #  ------------ check for case of beginning of a year -----------
      if (days < 1.0):
          year    = year - 1;
          leapyrs = int(((year - 1901) * 0.25) // 1.0);
          days    = temp - ((year - 1900) * 365.0 + leapyrs);
 
      #  ----------------- find remaing data  -------------------------
-     mon, day, hr, minute, sec = days2mdhms(year, days);
+     mon, day, hr, minute, sec = days2mdhms(year, days, None);
      sec = sec - 0.00000086400;
      return year, mon, day, hr, minute, sec
```

### Comparing `sgp4-2.8/sgp4/io.py` & `sgp4-2.9/sgp4/io.py`

 * *Files identical despite different names*

### Comparing `sgp4-2.8/sgp4/model.py` & `sgp4-2.9/sgp4/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,16 +51,21 @@
         whichconst = gravity_constants[whichconst]
         self = cls()
         twoline2rv(line1, line2, whichconst, 'i', self)
 
         # Install a fancy split JD of the kind the C++ natively supports.
         # We rebuild it from the TLE year and day to maintain precision.
         year = self.epochyr
-        month, day, h, m, s = days2mdhms(year, self.epochdays);
-        self.jdsatepoch, self.jdsatepochF = jday2(year, month, day, h, m, s)
+        days, fraction = divmod(self.epochdays, 1.0)
+        self.jdsatepoch = year * 365 + (year - 1) // 4 + days + 1721044.5
+        self.jdsatepochF = round(fraction, 8)  # exact number of digits in TLE
+
+        # Remove the legacy datetime "epoch", which is not provided by
+        # the C++ version of the object.
+        del self.epoch
 
         # Undo my non-standard 4-digit year
         self.epochyr %= 100
         return self
 
     def sgp4init(self, whichconst, opsmode, satnum, epoch, bstar,
                  ndot, nddot, ecco, argpo, inclo, mo, no_kozai, nodeo):
```

### Comparing `sgp4-2.8/sgp4/propagation.py` & `sgp4-2.9/sgp4/propagation.py`

 * *Files identical despite different names*

### Comparing `sgp4-2.8/sgp4/tcppver.out` & `sgp4-2.9/sgp4/tcppver.out`

 * *Files identical despite different names*

### Comparing `sgp4-2.8/sgp4/tests.py` & `sgp4-2.9/sgp4/tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 from doctest import DocTestSuite, ELLIPSIS
 from math import pi, isnan
 from pkgutil import get_data
 
 from sgp4.api import WGS72OLD, WGS72, WGS84, Satrec, jday, accelerated
 from sgp4.earth_gravity import wgs72
 from sgp4.ext import invjday, newtonnu, rv2coe
-from sgp4.conveniences import jday_datetime
+from sgp4.functions import _day_of_year_to_month_day
 from sgp4.propagation import sgp4, sgp4init
-from sgp4 import io
+from sgp4 import conveniences, io
 from sgp4.exporter import export_tle
 import sgp4.model as model
 
 _testcase = TestCase('setUp')
 assertEqual = _testcase.assertEqual
 assertAlmostEqual = _testcase.assertAlmostEqual
 assertRaises = _testcase.assertRaises
@@ -122,20 +122,26 @@
             return self.offset
         def tzname(self, datetime):
             return 'UTC plus 4'
         def dst(self, datetime):
             return self.offset
 
     datetime_local = dt.datetime(2011, 11, 4, 0, 5, 23, 0, UTC_plus_4())
-    jd, fr = jday_datetime(datetime_local)
+    jd, fr = conveniences.jday_datetime(datetime_local)
 
     # jd of this date is 2455868.5 + 0.8370717592592593
     assertEqual(jd, 2455868.5)
     assertAlmostEqual(fr, 0.8370717592592593)
 
+def test_sat_epoch_datetime():
+    sat = Satrec.twoline2rv(LINE1, LINE2)
+    datetime = conveniences.sat_epoch_datetime(sat)
+    zone = conveniences.UTC
+    assertEqual(datetime, dt.datetime(2000, 6, 27, 18, 50, 19, 733568, zone))
+
 def test_good_tle_checksum():
     for line in LINE1, LINE2:
         checksum = int(line[-1])
         assertEqual(io.compute_checksum(line), checksum)
         assertEqual(io.fix_checksum(line[:68]), line)
         io.verify_checksum(line)
 
@@ -283,28 +289,54 @@
     sat = io.twoline2rv(LINE1, LINE2, wgs72)
     assertEqual(sat.epochyr, 2000)
 
 def test_support_for_old_no_attribute():
     s = io.twoline2rv(LINE1, LINE2, wgs72)
     assert s.no == s.no_kozai
 
+def test_months_and_days():
+    # Make sure our hand-written months-and-days routine is perfect.
+
+    month_lengths = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
+
+    day_of_year = 1
+    for month, length in enumerate(month_lengths, 1):
+        for day in range(1, length + 1):
+            tup = _day_of_year_to_month_day(day_of_year, False)
+            assertEqual((month, day), tup)
+            day_of_year += 1
+
+    month_lengths[1] = 29  # February, during a leap year
+    day_of_year = 1
+    for month, length in enumerate(month_lengths, 1):
+        for day in range(1, length + 1):
+            tup = _day_of_year_to_month_day(day_of_year, True)
+            assertEqual((month, day), tup)
+            day_of_year += 1
+
+
 def test_december_32():
     # ISS [Orbit 606], whose date is 2019 plus 366.82137887 days.
     # The core SGP4 routines handled this fine, but my hamfisted
     # attempt to provide a Python datetime for "convenience" ran
     # into an overflow.
-    sat = io.twoline2rv(
-    '1 25544U 98067A   19366.82137887  .00016717  00000-0  10270-3 0  9129',
-    '2 25544  51.6392  96.6358 0005156  88.7140 271.4601 15.49497216  6061',
-    wgs72,
-    )
-    assertEqual(
-        dt.datetime(2020, 1, 1, 19, 42, 47, 134367),
-        sat.epoch,
-    )
+    a = '1 25544U 98067A   19366.82137887  .00016717  00000-0  10270-3 0  9129'
+    b = '2 25544  51.6392  96.6358 0005156  88.7140 271.4601 15.49497216  6061'
+    correct_epoch = dt.datetime(2020, 1, 1, 19, 42, 47, 134368)
+
+    # Legacy API.
+    sat = io.twoline2rv(a, b, wgs72)
+    assertEqual(sat.epoch, correct_epoch)
+
+    correct_epoch = correct_epoch.replace(tzinfo=conveniences.UTC)
+
+    # Modern API.
+    sat = Satrec.twoline2rv(a, b)
+    assertEqual(conveniences.sat_epoch_datetime(sat), correct_epoch)
+
 
 def test_bad_first_line():
     with assertRaisesRegex(ValueError, re.escape("""TLE format error
 
 The Two-Line Element (TLE) format was designed for punch cards, and so
 is very strict about the position of every period, space, and digit.
 Your line does not quite match.  Here is the official format for line 1
@@ -339,15 +371,20 @@
     attrs = VANGUARD_ATTRS
 
     if legacy:
         attrs = attrs.copy()
         del attrs['jdsatepoch']
 
     for name, value in attrs.items():
-        assertEqual(getattr(sat, name), value, name + ' attribute')
+        try:
+            assertEqual(getattr(sat, name), value)
+        except AssertionError as e:
+            message, = e.args
+            e.args = ('for attribute %s, %s' % (name, message),)
+            raise e
 
     if not legacy:
         assertAlmostEqual(sat.jdsatepochF, 0.78495062, delta=1e-13)
 
 def sgp4init_args(d):
     """Given a dict of orbital parameters, return them in sgp4init order."""
     return (d['bstar'], d['ndot'], d['nddot'], d['ecco'], d['argpo'],
@@ -550,30 +587,34 @@
 
     jd = satrec.jdsatepoch + satrec.jdsatepochF + tsince / 1440.0
     year, mon, day, hr, minute, sec = invjday(jd)
 
     (p, a, ecc, incl, node, argp, nu, m, arglat, truelon, lonper
      ) = rv2coe(r, v, mu)
 
-    return short + (' %14.6f %8.6f %10.5f %10.5f %10.5f %10.5f %10.5f'
-                    ' %5i%3i%3i %2i:%2i:%9.6f\n') % (
+    return short + (
+        ' %14.6f %8.6f %10.5f %10.5f %10.5f %10.5f %10.5f'
+        ' %5i%3i%3i %2i:%2i:%9.6f\n'
+    ) % (
         a, ecc, incl*rad, node*rad, argp*rad, nu*rad,
-        m*rad, year, mon, day, hr, minute, sec)
+        m*rad, year, mon, day, hr, minute, sec,
+    )
 
 # ----------------------------------------------------------------------
 
 def load_tests(loader, tests, ignore):
     """Run our main documentation as a test, plus all test functions."""
 
     from sgp4.wulfgar import add_test_functions
     add_test_functions(loader, tests, __name__)
 
     # Python 2.6 formats floating-point numbers a bit differently and
     # breaks the doctest, so we only run the doctest on later versions.
     if sys.version_info >= (2, 7):
         tests.addTests(DocTestSuite('sgp4', optionflags=ELLIPSIS))
+        tests.addTests(DocTestSuite('sgp4.conveniences', optionflags=ELLIPSIS))
         tests.addTests(DocTestSuite('sgp4.functions', optionflags=ELLIPSIS))
 
     return tests
 
 if __name__ == '__main__':
     main()
```

### Comparing `sgp4-2.8/sgp4/wrapper.py` & `sgp4-2.9/sgp4/wrapper.py`

 * *Files identical despite different names*

### Comparing `sgp4-2.8/sgp4/wulfgar.py` & `sgp4-2.9/sgp4/wulfgar.py`

 * *Files identical despite different names*

