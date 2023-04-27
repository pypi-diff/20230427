# Comparing `tmp/pySLALIB-1.0.6.tar.gz` & `tmp/pySLALIB-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pySLALIB-1.0.6.tar", last modified: Fri Apr  7 16:52:37 2023, max compression
+gzip compressed data, was "pySLALIB-1.0.7.tar", last modified: Thu Apr 27 17:54:29 2023, max compression
```

## Comparing `pySLALIB-1.0.6.tar` & `pySLALIB-1.0.7.tar`

### file list

```diff
@@ -1,211 +1,211 @@
-drwxr-xr-x   0 gamma     (1000) gamma     (1000)        0 2023-04-07 16:52:37.734305 pySLALIB-1.0.6/
--rw-r--r--   0 gamma     (1000) gamma     (1000)      154 2023-04-07 16:52:37.734305 pySLALIB-1.0.6/PKG-INFO
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2530 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/README.txt
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2343 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/addet.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     4347 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/afin.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2517 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/airmas.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     4980 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/altaz.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2949 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/amp.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3951 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/ampqk.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     9180 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/aop.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     7446 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/aoppa.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1821 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/aoppat.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     9677 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/aopqk.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     5348 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/atmdsp.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1749 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/atms.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2318 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/atmt.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2290 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/av2m.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1791 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/bear.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2097 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/caf2r.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2103 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/caldj.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2551 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/calyd.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1790 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/cc2s.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2467 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/cc62s.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2318 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/cd2tf.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2600 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/cldj.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3461 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/clyd.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     4305 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/combn.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2450 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/cr2af.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2376 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/cr2tf.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1621 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/cs2c.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1904 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/cs2c6.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2041 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/ctf2d.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1954 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/ctf2r.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2126 2023-04-06 22:27:01.547660 pySLALIB-1.0.6/daf2r.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     6035 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dafin.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     6485 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dat.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2319 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dav2m.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1836 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dbear.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3824 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dbjin.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2491 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dc62s.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1821 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dcc2s.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3908 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dcmpf.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1649 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dcs2c.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3023 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dd2tf.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3124 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/de2h.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     5250 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/deuler.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     9091 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dfltin.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2932 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dh2e.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1731 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dimxv.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2594 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/djcal.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2189 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/djcl.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2168 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dm2av.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     4302 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dmat.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)    27899 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dmoon.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1846 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dmxm.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1772 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dmxv.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2281 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dpav.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2466 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dr2af.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2429 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dr2tf.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1508 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/drange.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1394 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dranrm.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1899 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/ds2c6.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2522 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/ds2tp.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1690 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dsep.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2142 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dsepv.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3052 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dt.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2060 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dtf2d.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1987 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dtf2r.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1642 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dtp2s.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2046 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dtp2v.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3552 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dtps2c.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3287 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dtpv2c.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1904 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dtt.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2592 2023-04-06 22:27:01.550994 pySLALIB-1.0.6/dv2tp.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1309 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/dvdv.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1802 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/dvn.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1505 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/dvxv.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3079 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/e2h.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3499 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/earth.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2104 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/ecleq.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1943 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/ecmat.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2824 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/ecor.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2938 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/eg50.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)    10437 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/el2ue.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1357 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/epb.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1370 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/epb2d.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2166 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/epco.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1337 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/epj.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1350 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/epj2d.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)   158276 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/epv.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2104 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/eqecl.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2286 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/eqeqx.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2787 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/eqgal.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2266 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/etrms.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2887 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/euler.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)    16115 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/evp.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     9084 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/fitxy.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     8523 2023-04-06 22:27:01.554327 pySLALIB-1.0.6/fk425.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     6225 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/fk45z.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     8671 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/fk524.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3743 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/fk52h.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3012 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/fk54z.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3779 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/fk5hz.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     5320 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/flotin.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2787 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/galeq.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2797 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/galsup.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2944 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/ge50.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2058 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/geoc.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2009 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/get_docstring.py
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2687 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/gmst.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3585 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/gmsta.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3073 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/gresid.F
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2963 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/h2e.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3846 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/h2fk5.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     4273 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/hfk5z.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2974 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/idchf.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2797 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/idchi.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1709 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/imxv.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     5438 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/intin.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2626 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/invf.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1850 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/kbj.f
-drwxr-xr-x   0 gamma     (1000) gamma     (1000)        0 2023-04-07 16:52:37.734305 pySLALIB-1.0.6/lib/
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1250 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/lib/__init__.py
--rw-r--r--   0 gamma     (1000) gamma     (1000)   483102 2023-04-07 16:52:37.710972 pySLALIB-1.0.6/lib/docstring_pickle.pkl
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2145 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/m2av.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3511 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/map.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     4174 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/mappa.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     5005 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/mapqk.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     4047 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/mapqkz.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)    15722 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/moon.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1819 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/mxm.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1747 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/mxv.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2391 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/nut.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)    38617 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/nutc.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)    10349 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/nutc80.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     9130 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/oap.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     8626 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/oapqk.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)    26728 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/obs.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1974 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/pa.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2019 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/pav.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2186 2023-04-06 22:27:01.557661 pySLALIB-1.0.6/pcd.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3078 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/pda2h.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3047 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/pdq2h.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     4557 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/permut.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     6833 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/pertel.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)    21026 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/pertue.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     7115 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/planel.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)    29743 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/planet.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     9128 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/plante.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     5239 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/plantu.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2972 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/pm.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     5751 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/polmo.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2437 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/prebn.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3189 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/prec.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3003 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/preces.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     4266 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/precl.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1843 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/prenut.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)    11537 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/pv2el.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     5037 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/pv2ue.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1950 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/pvobs.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2976 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/pxy.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)      123 2023-04-07 16:46:31.985871 pySLALIB-1.0.6/pyproject.toml
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2278 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/random.F
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1454 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/range.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1385 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/ranorm.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)    58810 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/rcc.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     5814 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/rdplan.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3097 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/refco.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     8525 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/refcoq.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)    14128 2023-04-06 22:27:01.560994 pySLALIB-1.0.6/refro.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     4509 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/refv.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     5657 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/refz.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2028 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/rverot.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2533 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/rvgalc.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2174 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/rvlg.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3097 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/rvlsrd.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2971 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/rvlsrk.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2465 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/s2tp.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1533 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/sep.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1903 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/sepv.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1191 2023-04-07 16:29:20.029039 pySLALIB-1.0.6/setup.py
--rw-r--r--   0 gamma     (1000) gamma     (1000)    49356 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/sla.c
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1942 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/sla_config.h
--rw-r--r--   0 gamma     (1000) gamma     (1000)    17440 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/slalib.h
--rw-r--r--   0 gamma     (1000) gamma     (1000)    61502 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/slalib.pyf
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2981 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/slamac.h
--rw-r--r--   0 gamma     (1000) gamma     (1000)     4306 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/smat.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)      106 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/stdeb.cfg
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2302 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/subet.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2790 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/supgal.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)    12328 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/svd.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2196 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/svdcov.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3891 2023-04-06 22:27:01.564327 pySLALIB-1.0.6/svdsol.f
-drwxr-xr-x   0 gamma     (1000) gamma     (1000)        0 2023-04-07 16:52:37.734305 pySLALIB-1.0.6/test/
--rw-r--r--   0 gamma     (1000) gamma     (1000)    77894 2023-04-06 22:27:01.567661 pySLALIB-1.0.6/test/test_slalib.py
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1602 2023-04-06 22:27:01.567661 pySLALIB-1.0.6/tp2s.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2014 2023-04-06 22:27:01.567661 pySLALIB-1.0.6/tp2v.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3508 2023-04-06 22:27:01.567661 pySLALIB-1.0.6/tps2c.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     3255 2023-04-06 22:27:01.567661 pySLALIB-1.0.6/tpv2c.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     8394 2023-04-06 22:27:01.567661 pySLALIB-1.0.6/ue2el.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     8253 2023-04-06 22:27:01.567661 pySLALIB-1.0.6/ue2pv.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     4312 2023-04-06 22:27:01.567661 pySLALIB-1.0.6/unpcd.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2548 2023-04-06 22:27:01.567661 pySLALIB-1.0.6/v2tp.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1281 2023-04-06 22:27:01.567661 pySLALIB-1.0.6/vdv.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1556 2023-04-06 22:27:01.567661 pySLALIB-1.0.6/veri.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1820 2023-04-06 22:27:01.567661 pySLALIB-1.0.6/vers.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1562 2023-04-06 22:27:01.567661 pySLALIB-1.0.6/vn.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1479 2023-04-06 22:27:01.567661 pySLALIB-1.0.6/vxv.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1395 2023-04-06 22:27:01.567661 pySLALIB-1.0.6/wait.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     1887 2023-04-06 22:27:01.567661 pySLALIB-1.0.6/xy2xy.f
--rw-r--r--   0 gamma     (1000) gamma     (1000)     2595 2023-04-06 22:27:01.567661 pySLALIB-1.0.6/zd.f
+drwxr-xr-x   0 gamma     (1000) gamma     (1000)        0 2023-04-27 17:54:29.323268 pySLALIB-1.0.7/
+-rw-r--r--   0 gamma     (1000) gamma     (1000)      154 2023-04-27 17:54:29.323268 pySLALIB-1.0.7/PKG-INFO
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2530 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/README.txt
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2343 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/addet.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     4347 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/afin.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2517 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/airmas.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     4980 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/altaz.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2949 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/amp.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3951 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/ampqk.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     9180 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/aop.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     7446 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/aoppa.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1821 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/aoppat.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     9677 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/aopqk.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     5348 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/atmdsp.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1749 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/atms.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2318 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/atmt.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2290 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/av2m.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1791 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/bear.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2097 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/caf2r.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2103 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/caldj.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2551 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/calyd.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1790 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/cc2s.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2467 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/cc62s.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2318 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/cd2tf.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2600 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/cldj.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3461 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/clyd.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     4305 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/combn.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2450 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/cr2af.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2376 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/cr2tf.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1621 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/cs2c.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1904 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/cs2c6.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2041 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/ctf2d.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1954 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/ctf2r.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2126 2023-04-06 22:27:01.547660 pySLALIB-1.0.7/daf2r.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     6035 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dafin.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     6485 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dat.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2319 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dav2m.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1836 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dbear.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3824 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dbjin.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2491 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dc62s.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1821 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dcc2s.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3908 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dcmpf.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1649 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dcs2c.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3023 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dd2tf.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3124 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/de2h.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     5250 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/deuler.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     9091 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dfltin.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2932 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dh2e.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1731 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dimxv.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2594 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/djcal.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2189 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/djcl.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2168 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dm2av.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     4302 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dmat.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)    27899 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dmoon.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1846 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dmxm.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1772 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dmxv.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2281 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dpav.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2466 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dr2af.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2429 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dr2tf.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1508 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/drange.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1394 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dranrm.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1899 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/ds2c6.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2522 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/ds2tp.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1690 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dsep.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2142 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dsepv.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3052 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dt.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2060 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dtf2d.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1987 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dtf2r.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1642 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dtp2s.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2046 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dtp2v.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3552 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dtps2c.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3287 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dtpv2c.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1904 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dtt.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2592 2023-04-06 22:27:01.550994 pySLALIB-1.0.7/dv2tp.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1309 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/dvdv.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1802 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/dvn.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1505 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/dvxv.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3079 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/e2h.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3499 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/earth.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2104 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/ecleq.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1943 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/ecmat.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2824 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/ecor.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2938 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/eg50.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)    10437 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/el2ue.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1357 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/epb.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1370 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/epb2d.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2166 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/epco.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1337 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/epj.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1350 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/epj2d.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)   158276 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/epv.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2104 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/eqecl.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2286 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/eqeqx.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2787 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/eqgal.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2266 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/etrms.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2887 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/euler.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)    16115 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/evp.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     9084 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/fitxy.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     8523 2023-04-06 22:27:01.554327 pySLALIB-1.0.7/fk425.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     6225 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/fk45z.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     8671 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/fk524.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3743 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/fk52h.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3012 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/fk54z.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3779 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/fk5hz.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     5320 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/flotin.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2787 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/galeq.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2797 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/galsup.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2944 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/ge50.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2058 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/geoc.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2009 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/get_docstring.py
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2687 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/gmst.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3585 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/gmsta.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3073 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/gresid.F
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2963 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/h2e.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3846 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/h2fk5.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     4273 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/hfk5z.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2974 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/idchf.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2797 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/idchi.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1709 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/imxv.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     5438 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/intin.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2626 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/invf.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1850 2023-04-27 17:45:47.208692 pySLALIB-1.0.7/kbj.f
+drwxr-xr-x   0 gamma     (1000) gamma     (1000)        0 2023-04-27 17:54:29.323268 pySLALIB-1.0.7/lib/
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1250 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/lib/__init__.py
+-rw-r--r--   0 gamma     (1000) gamma     (1000)   483102 2023-04-27 17:54:29.299934 pySLALIB-1.0.7/lib/docstring_pickle.pkl
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2145 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/m2av.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3511 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/map.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     4174 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/mappa.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     5005 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/mapqk.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     4047 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/mapqkz.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)    15722 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/moon.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1819 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/mxm.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1747 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/mxv.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2391 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/nut.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)    38617 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/nutc.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)    10349 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/nutc80.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     9130 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/oap.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     8626 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/oapqk.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)    26728 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/obs.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1974 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/pa.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2019 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/pav.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2186 2023-04-06 22:27:01.557661 pySLALIB-1.0.7/pcd.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3078 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/pda2h.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3047 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/pdq2h.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     4557 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/permut.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     6833 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/pertel.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)    21026 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/pertue.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     7115 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/planel.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)    29743 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/planet.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     9128 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/plante.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     5239 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/plantu.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2972 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/pm.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     5751 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/polmo.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2437 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/prebn.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3189 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/prec.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3003 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/preces.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     4266 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/precl.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1843 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/prenut.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)    11537 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/pv2el.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     5037 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/pv2ue.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1950 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/pvobs.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2976 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/pxy.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)      123 2023-04-27 17:48:35.018896 pySLALIB-1.0.7/pyproject.toml
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2278 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/random.F
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1454 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/range.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1385 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/ranorm.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)    58810 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/rcc.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     5814 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/rdplan.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3097 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/refco.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     8525 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/refcoq.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)    14128 2023-04-06 22:27:01.560994 pySLALIB-1.0.7/refro.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     4509 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/refv.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     5657 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/refz.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2028 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/rverot.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2533 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/rvgalc.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2174 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/rvlg.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3097 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/rvlsrd.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2971 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/rvlsrk.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2465 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/s2tp.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1533 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/sep.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1903 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/sepv.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1220 2023-04-27 16:46:10.159241 pySLALIB-1.0.7/setup.py
+-rw-r--r--   0 gamma     (1000) gamma     (1000)    49356 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/sla.c
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1942 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/sla_config.h
+-rw-r--r--   0 gamma     (1000) gamma     (1000)    17440 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/slalib.h
+-rw-r--r--   0 gamma     (1000) gamma     (1000)    61504 2023-04-27 17:46:01.568699 pySLALIB-1.0.7/slalib.pyf
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2981 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/slamac.h
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     4306 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/smat.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)      106 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/stdeb.cfg
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2302 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/subet.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2790 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/supgal.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)    12328 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/svd.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2196 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/svdcov.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3891 2023-04-06 22:27:01.564327 pySLALIB-1.0.7/svdsol.f
+drwxr-xr-x   0 gamma     (1000) gamma     (1000)        0 2023-04-27 17:54:29.323268 pySLALIB-1.0.7/test/
+-rw-r--r--   0 gamma     (1000) gamma     (1000)    77894 2023-04-06 22:27:01.567661 pySLALIB-1.0.7/test/test_slalib.py
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1602 2023-04-06 22:27:01.567661 pySLALIB-1.0.7/tp2s.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2014 2023-04-06 22:27:01.567661 pySLALIB-1.0.7/tp2v.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3508 2023-04-06 22:27:01.567661 pySLALIB-1.0.7/tps2c.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     3255 2023-04-06 22:27:01.567661 pySLALIB-1.0.7/tpv2c.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     8394 2023-04-06 22:27:01.567661 pySLALIB-1.0.7/ue2el.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     8253 2023-04-06 22:27:01.567661 pySLALIB-1.0.7/ue2pv.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     4312 2023-04-06 22:27:01.567661 pySLALIB-1.0.7/unpcd.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2548 2023-04-06 22:27:01.567661 pySLALIB-1.0.7/v2tp.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1281 2023-04-06 22:27:01.567661 pySLALIB-1.0.7/vdv.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1556 2023-04-06 22:27:01.567661 pySLALIB-1.0.7/veri.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1820 2023-04-06 22:27:01.567661 pySLALIB-1.0.7/vers.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1562 2023-04-06 22:27:01.567661 pySLALIB-1.0.7/vn.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1479 2023-04-06 22:27:01.567661 pySLALIB-1.0.7/vxv.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1395 2023-04-06 22:27:01.567661 pySLALIB-1.0.7/wait.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     1887 2023-04-06 22:27:01.567661 pySLALIB-1.0.7/xy2xy.f
+-rw-r--r--   0 gamma     (1000) gamma     (1000)     2595 2023-04-06 22:27:01.567661 pySLALIB-1.0.7/zd.f
```

### Comparing `pySLALIB-1.0.6/README.txt` & `pySLALIB-1.0.7/README.txt`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/addet.f` & `pySLALIB-1.0.7/addet.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/afin.f` & `pySLALIB-1.0.7/afin.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/airmas.f` & `pySLALIB-1.0.7/airmas.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/altaz.f` & `pySLALIB-1.0.7/altaz.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/amp.f` & `pySLALIB-1.0.7/amp.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/ampqk.f` & `pySLALIB-1.0.7/ampqk.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/aop.f` & `pySLALIB-1.0.7/aop.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/aoppa.f` & `pySLALIB-1.0.7/aoppa.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/aoppat.f` & `pySLALIB-1.0.7/aoppat.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/aopqk.f` & `pySLALIB-1.0.7/aopqk.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/atmdsp.f` & `pySLALIB-1.0.7/atmdsp.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/atms.f` & `pySLALIB-1.0.7/atms.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/atmt.f` & `pySLALIB-1.0.7/atmt.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/av2m.f` & `pySLALIB-1.0.7/av2m.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/bear.f` & `pySLALIB-1.0.7/bear.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/caf2r.f` & `pySLALIB-1.0.7/caf2r.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/caldj.f` & `pySLALIB-1.0.7/caldj.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/calyd.f` & `pySLALIB-1.0.7/calyd.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/cc2s.f` & `pySLALIB-1.0.7/cc2s.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/cc62s.f` & `pySLALIB-1.0.7/cc62s.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/cd2tf.f` & `pySLALIB-1.0.7/cd2tf.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/cldj.f` & `pySLALIB-1.0.7/cldj.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/clyd.f` & `pySLALIB-1.0.7/clyd.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/combn.f` & `pySLALIB-1.0.7/combn.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/cr2af.f` & `pySLALIB-1.0.7/cr2af.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/cr2tf.f` & `pySLALIB-1.0.7/cr2tf.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/cs2c.f` & `pySLALIB-1.0.7/cs2c.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/cs2c6.f` & `pySLALIB-1.0.7/cs2c6.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/ctf2d.f` & `pySLALIB-1.0.7/ctf2d.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/ctf2r.f` & `pySLALIB-1.0.7/ctf2r.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/daf2r.f` & `pySLALIB-1.0.7/daf2r.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dafin.f` & `pySLALIB-1.0.7/dafin.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dat.f` & `pySLALIB-1.0.7/dat.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dav2m.f` & `pySLALIB-1.0.7/dav2m.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dbear.f` & `pySLALIB-1.0.7/dbear.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dbjin.f` & `pySLALIB-1.0.7/dbjin.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dc62s.f` & `pySLALIB-1.0.7/dc62s.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dcc2s.f` & `pySLALIB-1.0.7/dcc2s.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dcmpf.f` & `pySLALIB-1.0.7/dcmpf.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dcs2c.f` & `pySLALIB-1.0.7/dcs2c.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dd2tf.f` & `pySLALIB-1.0.7/dd2tf.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/de2h.f` & `pySLALIB-1.0.7/de2h.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/deuler.f` & `pySLALIB-1.0.7/deuler.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dfltin.f` & `pySLALIB-1.0.7/dfltin.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dh2e.f` & `pySLALIB-1.0.7/dh2e.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dimxv.f` & `pySLALIB-1.0.7/dimxv.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/djcal.f` & `pySLALIB-1.0.7/djcal.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/djcl.f` & `pySLALIB-1.0.7/djcl.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dm2av.f` & `pySLALIB-1.0.7/dm2av.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dmat.f` & `pySLALIB-1.0.7/dmat.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dmoon.f` & `pySLALIB-1.0.7/dmoon.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dmxm.f` & `pySLALIB-1.0.7/dmxm.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dmxv.f` & `pySLALIB-1.0.7/dmxv.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dpav.f` & `pySLALIB-1.0.7/dpav.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dr2af.f` & `pySLALIB-1.0.7/dr2af.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dr2tf.f` & `pySLALIB-1.0.7/dr2tf.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/drange.f` & `pySLALIB-1.0.7/drange.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dranrm.f` & `pySLALIB-1.0.7/dranrm.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/ds2c6.f` & `pySLALIB-1.0.7/ds2c6.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/ds2tp.f` & `pySLALIB-1.0.7/ds2tp.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dsep.f` & `pySLALIB-1.0.7/dsep.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dsepv.f` & `pySLALIB-1.0.7/dsepv.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dt.f` & `pySLALIB-1.0.7/dt.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dtf2d.f` & `pySLALIB-1.0.7/dtf2d.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dtf2r.f` & `pySLALIB-1.0.7/dtf2r.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dtp2s.f` & `pySLALIB-1.0.7/dtp2s.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dtp2v.f` & `pySLALIB-1.0.7/dtp2v.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dtps2c.f` & `pySLALIB-1.0.7/dtps2c.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dtpv2c.f` & `pySLALIB-1.0.7/dtpv2c.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dtt.f` & `pySLALIB-1.0.7/dtt.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dv2tp.f` & `pySLALIB-1.0.7/dv2tp.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dvdv.f` & `pySLALIB-1.0.7/dvdv.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dvn.f` & `pySLALIB-1.0.7/dvn.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/dvxv.f` & `pySLALIB-1.0.7/dvxv.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/e2h.f` & `pySLALIB-1.0.7/e2h.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/earth.f` & `pySLALIB-1.0.7/earth.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/ecleq.f` & `pySLALIB-1.0.7/ecleq.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/ecmat.f` & `pySLALIB-1.0.7/ecmat.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/ecor.f` & `pySLALIB-1.0.7/ecor.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/eg50.f` & `pySLALIB-1.0.7/eg50.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/el2ue.f` & `pySLALIB-1.0.7/el2ue.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/epb.f` & `pySLALIB-1.0.7/epb.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/epb2d.f` & `pySLALIB-1.0.7/epb2d.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/epco.f` & `pySLALIB-1.0.7/epco.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/epj.f` & `pySLALIB-1.0.7/epj.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/epj2d.f` & `pySLALIB-1.0.7/epj2d.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/epv.f` & `pySLALIB-1.0.7/epv.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/eqecl.f` & `pySLALIB-1.0.7/eqecl.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/eqeqx.f` & `pySLALIB-1.0.7/eqeqx.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/eqgal.f` & `pySLALIB-1.0.7/eqgal.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/etrms.f` & `pySLALIB-1.0.7/etrms.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/euler.f` & `pySLALIB-1.0.7/euler.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/evp.f` & `pySLALIB-1.0.7/evp.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/fitxy.f` & `pySLALIB-1.0.7/fitxy.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/fk425.f` & `pySLALIB-1.0.7/fk425.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/fk45z.f` & `pySLALIB-1.0.7/fk45z.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/fk524.f` & `pySLALIB-1.0.7/fk524.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/fk52h.f` & `pySLALIB-1.0.7/fk52h.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/fk54z.f` & `pySLALIB-1.0.7/fk54z.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/fk5hz.f` & `pySLALIB-1.0.7/fk5hz.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/flotin.f` & `pySLALIB-1.0.7/flotin.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/galeq.f` & `pySLALIB-1.0.7/galeq.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/galsup.f` & `pySLALIB-1.0.7/galsup.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/ge50.f` & `pySLALIB-1.0.7/ge50.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/geoc.f` & `pySLALIB-1.0.7/geoc.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/get_docstring.py` & `pySLALIB-1.0.7/get_docstring.py`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/gmst.f` & `pySLALIB-1.0.7/gmst.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/gmsta.f` & `pySLALIB-1.0.7/gmsta.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/gresid.F` & `pySLALIB-1.0.7/gresid.F`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/h2e.f` & `pySLALIB-1.0.7/h2e.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/h2fk5.f` & `pySLALIB-1.0.7/h2fk5.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/hfk5z.f` & `pySLALIB-1.0.7/hfk5z.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/idchf.f` & `pySLALIB-1.0.7/idchf.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/idchi.f` & `pySLALIB-1.0.7/idchi.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/imxv.f` & `pySLALIB-1.0.7/imxv.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/intin.f` & `pySLALIB-1.0.7/intin.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/invf.f` & `pySLALIB-1.0.7/invf.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/kbj.f` & `pySLALIB-1.0.7/kbj.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/lib/__init__.py` & `pySLALIB-1.0.7/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/lib/docstring_pickle.pkl` & `pySLALIB-1.0.7/lib/docstring_pickle.pkl`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/m2av.f` & `pySLALIB-1.0.7/m2av.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/map.f` & `pySLALIB-1.0.7/map.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/mappa.f` & `pySLALIB-1.0.7/mappa.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/mapqk.f` & `pySLALIB-1.0.7/mapqk.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/mapqkz.f` & `pySLALIB-1.0.7/mapqkz.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/moon.f` & `pySLALIB-1.0.7/moon.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/mxm.f` & `pySLALIB-1.0.7/mxm.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/mxv.f` & `pySLALIB-1.0.7/mxv.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/nut.f` & `pySLALIB-1.0.7/nut.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/nutc.f` & `pySLALIB-1.0.7/nutc.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/nutc80.f` & `pySLALIB-1.0.7/nutc80.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/oap.f` & `pySLALIB-1.0.7/oap.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/oapqk.f` & `pySLALIB-1.0.7/oapqk.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/obs.f` & `pySLALIB-1.0.7/obs.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/pa.f` & `pySLALIB-1.0.7/pa.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/pav.f` & `pySLALIB-1.0.7/pav.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/pcd.f` & `pySLALIB-1.0.7/pcd.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/pda2h.f` & `pySLALIB-1.0.7/pda2h.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/pdq2h.f` & `pySLALIB-1.0.7/pdq2h.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/permut.f` & `pySLALIB-1.0.7/permut.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/pertel.f` & `pySLALIB-1.0.7/pertel.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/pertue.f` & `pySLALIB-1.0.7/pertue.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/planel.f` & `pySLALIB-1.0.7/planel.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/planet.f` & `pySLALIB-1.0.7/planet.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/plante.f` & `pySLALIB-1.0.7/plante.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/plantu.f` & `pySLALIB-1.0.7/plantu.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/pm.f` & `pySLALIB-1.0.7/pm.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/polmo.f` & `pySLALIB-1.0.7/polmo.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/prebn.f` & `pySLALIB-1.0.7/prebn.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/prec.f` & `pySLALIB-1.0.7/prec.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/preces.f` & `pySLALIB-1.0.7/preces.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/precl.f` & `pySLALIB-1.0.7/precl.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/prenut.f` & `pySLALIB-1.0.7/prenut.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/pv2el.f` & `pySLALIB-1.0.7/pv2el.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/pv2ue.f` & `pySLALIB-1.0.7/pv2ue.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/pvobs.f` & `pySLALIB-1.0.7/pvobs.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/pxy.f` & `pySLALIB-1.0.7/pxy.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/random.F` & `pySLALIB-1.0.7/random.F`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/range.f` & `pySLALIB-1.0.7/range.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/ranorm.f` & `pySLALIB-1.0.7/ranorm.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/rcc.f` & `pySLALIB-1.0.7/rcc.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/rdplan.f` & `pySLALIB-1.0.7/rdplan.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/refco.f` & `pySLALIB-1.0.7/refco.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/refcoq.f` & `pySLALIB-1.0.7/refcoq.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/refro.f` & `pySLALIB-1.0.7/refro.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/refv.f` & `pySLALIB-1.0.7/refv.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/refz.f` & `pySLALIB-1.0.7/refz.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/rverot.f` & `pySLALIB-1.0.7/rverot.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/rvgalc.f` & `pySLALIB-1.0.7/rvgalc.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/rvlg.f` & `pySLALIB-1.0.7/rvlg.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/rvlsrd.f` & `pySLALIB-1.0.7/rvlsrd.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/rvlsrk.f` & `pySLALIB-1.0.7/rvlsrk.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/s2tp.f` & `pySLALIB-1.0.7/s2tp.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/sep.f` & `pySLALIB-1.0.7/sep.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/sepv.f` & `pySLALIB-1.0.7/sepv.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/setup.py` & `pySLALIB-1.0.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python
 import glob
+import numpy
 from numpy.distutils.core import setup, Extension
 import pickle
 import get_docstring
 from distutils.command.sdist import sdist
 
 # Generate documentation dictionary and save it in "lib/"
 docstring = get_docstring.get_docstring()
@@ -14,21 +15,21 @@
 ext1 = Extension(name = 'pyslalib.slalib',
                  include_dirs = ['.'],
                  sources = ['slalib.pyf']+\
                            glob.glob("*.f")+\
                            glob.glob("*.F"))
 
 if __name__ == "__main__":
+    numpy_version = numpy.__version__
     setup(name = 'pySLALIB',
           description       = "f2py and numpy based wrappers for SLALIB",
-          version           = "1.0.6",
+          version           = "1.0.7",
           author            = "Scott Ransom",
           author_email      = "sransom@nrao.edu",
-          setup_requires = ['numpy<1.22'],
-          install_requires = ['numpy<1.22'],
+          install_requires = ['numpy=={}'.format(numpy_version)],
           tests_require=["unittest-xml-reporting"],
           packages = ['pyslalib'],
           package_dir = {'pyslalib': 'lib'},
           package_data = {'pyslalib': ['docstring_pickle.pkl']},
           ext_modules = [ext1],
           cmdclass={'sdist': sdist},
           )
```

### Comparing `pySLALIB-1.0.6/sla.c` & `pySLALIB-1.0.7/sla.c`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/sla_config.h` & `pySLALIB-1.0.7/sla_config.h`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/slalib.h` & `pySLALIB-1.0.7/slalib.h`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/slalib.pyf` & `pySLALIB-1.0.7/slalib.pyf`

 * *Files 0% similar despite different names*

```diff
@@ -810,15 +810,15 @@
             double precision dimension(6) :: fwds
             double precision dimension(6),intent(out) ::  bkwds
             integer intent(out) ::  j
         end subroutine sla_invf
         subroutine sla_kbj(jb,e,k,j) ! in :slalib:kbj.f
             integer :: jb
             double precision :: e
-            character*1 intent(out) ::  k
+            character*1 intent(out,c) ::  k
             integer intent(out) ::  j
         end subroutine sla_kbj
         subroutine sla_m2av(rmat,axvec) ! in :slalib:m2av.f
             real dimension(3,3) :: rmat
             real dimension(3),intent(out) ::  axvec
         end subroutine sla_m2av
         subroutine sla_map(rm,dm,pr,pd,px,rv,eq,date,ra,da) ! in :slalib:map.f
```

### Comparing `pySLALIB-1.0.6/slamac.h` & `pySLALIB-1.0.7/slamac.h`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/smat.f` & `pySLALIB-1.0.7/smat.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/subet.f` & `pySLALIB-1.0.7/subet.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/supgal.f` & `pySLALIB-1.0.7/supgal.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/svd.f` & `pySLALIB-1.0.7/svd.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/svdcov.f` & `pySLALIB-1.0.7/svdcov.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/svdsol.f` & `pySLALIB-1.0.7/svdsol.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/test/test_slalib.py` & `pySLALIB-1.0.7/test/test_slalib.py`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/tp2s.f` & `pySLALIB-1.0.7/tp2s.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/tp2v.f` & `pySLALIB-1.0.7/tp2v.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/tps2c.f` & `pySLALIB-1.0.7/tps2c.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/tpv2c.f` & `pySLALIB-1.0.7/tpv2c.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/ue2el.f` & `pySLALIB-1.0.7/ue2el.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/ue2pv.f` & `pySLALIB-1.0.7/ue2pv.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/unpcd.f` & `pySLALIB-1.0.7/unpcd.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/v2tp.f` & `pySLALIB-1.0.7/v2tp.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/vdv.f` & `pySLALIB-1.0.7/vdv.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/veri.f` & `pySLALIB-1.0.7/veri.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/vers.f` & `pySLALIB-1.0.7/vers.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/vn.f` & `pySLALIB-1.0.7/vn.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/vxv.f` & `pySLALIB-1.0.7/vxv.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/wait.f` & `pySLALIB-1.0.7/wait.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/xy2xy.f` & `pySLALIB-1.0.7/xy2xy.f`

 * *Files identical despite different names*

### Comparing `pySLALIB-1.0.6/zd.f` & `pySLALIB-1.0.7/zd.f`

 * *Files identical despite different names*

