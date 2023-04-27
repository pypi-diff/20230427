# Comparing `tmp/keepa-1.3.5.tar.gz` & `tmp/keepa-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keepa-1.3.5.tar", last modified: Wed Jan 11 00:08:41 2023, max compression
+gzip compressed data, was "keepa-1.3.6.tar", last modified: Thu Apr 27 00:46:20 2023, max compression
```

## Comparing `keepa-1.3.5.tar` & `keepa-1.3.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 00:08:41.043215 keepa-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-01-11 00:07:28.000000 keepa-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-01-11 00:08:41.043215 keepa-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-01-11 00:07:28.000000 keepa-1.3.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 00:08:41.039215 keepa-1.3.5/keepa/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-01-11 00:07:28.000000 keepa-1.3.5/keepa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-01-11 00:07:28.000000 keepa-1.3.5/keepa/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)   120062 2023-01-11 00:07:28.000000 keepa-1.3.5/keepa/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-01-11 00:07:28.000000 keepa-1.3.5/keepa/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    38310 2023-01-11 00:07:28.000000 keepa-1.3.5/keepa/query_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 00:08:41.043215 keepa-1.3.5/keepa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-01-11 00:08:40.000000 keepa-1.3.5/keepa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-11 00:08:41.000000 keepa-1.3.5/keepa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 00:08:40.000000 keepa-1.3.5/keepa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-11 00:08:40.000000 keepa-1.3.5/keepa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-11 00:08:40.000000 keepa-1.3.5/keepa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 00:08:41.043215 keepa-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-01-11 00:07:28.000000 keepa-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:46:20.236931 keepa-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-27 00:45:00.000000 keepa-1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-04-27 00:46:20.236931 keepa-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-04-27 00:45:00.000000 keepa-1.3.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:46:20.236931 keepa-1.3.6/keepa/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-27 00:45:00.000000 keepa-1.3.6/keepa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-27 00:45:00.000000 keepa-1.3.6/keepa/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120472 2023-04-27 00:45:00.000000 keepa-1.3.6/keepa/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-04-27 00:45:00.000000 keepa-1.3.6/keepa/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38339 2023-04-27 00:45:00.000000 keepa-1.3.6/keepa/query_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:46:20.236931 keepa-1.3.6/keepa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-04-27 00:46:20.000000 keepa-1.3.6/keepa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-27 00:46:20.000000 keepa-1.3.6/keepa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 00:46:20.000000 keepa-1.3.6/keepa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-27 00:46:20.000000 keepa-1.3.6/keepa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 00:46:20.000000 keepa-1.3.6/keepa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 00:46:20.236931 keepa-1.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-27 00:45:00.000000 keepa-1.3.6/setup.py
```

### Comparing `keepa-1.3.5/LICENSE` & `keepa-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `keepa-1.3.5/PKG-INFO` & `keepa-1.3.6/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,60 +1,40 @@
-Metadata-Version: 2.1
-Name: keepa
-Version: 1.3.5
-Summary: Interfaces with keepa.com
-Home-page: https://github.com/akaszynski/keepa
-Author: Alex Kaszynski
-Author-email: akascap@gmail.com
-License: Apache Software License
-Keywords: keepa
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Topic :: Database :: Front-Ends
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-License-File: LICENSE
-
-keepa
-=====
+Python keepa Client Library
+===========================
 
 .. image:: https://img.shields.io/pypi/v/keepa.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/keepa/
 
-.. image:: https://travis-ci.org/akaszynski/keepa.svg?branch=master
-    :target: https://travis-ci.org/akaszynski/keepa
+.. image:: https://github.com/akaszynski/keepa/actions/workflows/testing-and-deployment.yml/badge.svg
+    :target: https://github.com/akaszynski/keepa/actions/workflows/testing-and-deployment.yml
 
 .. image:: https://readthedocs.org/projects/keepaapi/badge/?version=latest
     :target: https://keepaapi.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://codecov.io/gh/akaszynski/keepa/branch/master/graph/badge.svg
+.. image:: https://codecov.io/gh/akaszynski/keepa/branch/main/graph/badge.svg
   :target: https://codecov.io/gh/akaszynski/keepa
 
 .. image:: https://app.codacy.com/project/badge/Grade/9452f99f297c4a6eac14e2d21189ab6f
   :target: https://www.codacy.com/gh/akaszynski/keepa/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=akaszynski/keepa&amp;utm_campaign=Badge_Grade
 
 
-This Python module allows you to interface with the API at `Keepa
+This Python library allows you to interface with the API at `Keepa
 <https://keepa.com/>`_ to query for Amazon product information and
 history.  It also contains a plotting module to allow for plotting of
 a product.
 
-See API pricing at `Keepa API <https://keepa.com/#!api>`_
+See API pricing at `Keepa API <https://keepa.com/#!api>`_.
 
 Documentation can be found on readthedocs at `keepa Documentation <https://keepaapi.readthedocs.io/en/latest/>`_.
 
 
 Requirements
 ------------
-Module is compatible with Python >= 3.6 and requires:
+This library is compatible with Python >= 3.7 and requires:
 
 - ``numpy``
 - ``aiohttp``
 - ``matplotlib``
 - ``tqdm``
 
 Product history can be plotted from the raw data when ``matplotlib``
@@ -87,20 +67,20 @@
 
     # Single ASIN query
     products = api.query('B0088PUEPK') # returns list of product data
 
     # Plot result (requires matplotlib)
     keepa.plot_product(products[0])
 
-.. figure:: https://github.com/akaszynski/keepa/raw/master/docs/source/images/Product_Price_Plot.png
+.. figure:: https://github.com/akaszynski/keepa/raw/main/docs/source/images/Product_Price_Plot.png
     :width: 500pt
 
     Product Price Plot
 
-.. figure:: https://github.com/akaszynski/keepa/raw/master/docs/source/images/Product_Offer_Plot.png
+.. figure:: https://github.com/akaszynski/keepa/raw/main/docs/source/images/Product_Offer_Plot.png
     :width: 500pt
 
     Product Offers Plot
 
 
 Brief Example using async
 -------------------------
```

### Comparing `keepa-1.3.5/keepa/interface.py` & `keepa-1.3.6/keepa/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
         target.__doc__ = original.__doc__
         return target
 
     return wrapper
 
 
 log = logging.getLogger(__name__)
-log.setLevel("DEBUG")
 
 # hardcoded ordinal time from
 KEEPA_ST_ORDINAL = np.datetime64("2011-01-01")
 
 # Request limit
 REQUEST_LIMIT = 100
 
@@ -355,14 +354,18 @@
     timeout : float, optional
         Default timeout when issuing any request.  This is not a time
         limit on the entire response download; rather, an exception is
         raised if the server has not issued a response for timeout
         seconds.  Setting this to 0 disables the timeout, but will
         cause any request to hang indefiantly should keepa.com be down
 
+    logging_level: string, optional
+        Logging level to use.  Default is 'DEBUG'.  Other options are
+        'INFO', 'WARNING', 'ERROR', and 'CRITICAL'.
+
     Examples
     --------
     Create the api object.
 
     >>> import keepa
     >>> key = '<REAL_KEEPA_KEY>'
     >>> api = keepa.Keepa(key)
@@ -387,21 +390,26 @@
     >>> print('\t Used price: ${:.2f}'.format(usedprice[-1]))
     >>> print('\t as of: {:s}'.format(str(usedtimes[-1])))
         Used price: $0.52
         as of: 2023-01-03 04:46:00
 
     """
 
-    def __init__(self, accesskey, timeout=10):
+    def __init__(self, accesskey, timeout=10, logging_level="DEBUG"):
         """Initialize server connection."""
         self.accesskey = accesskey
         self.status = None
         self.tokens_left = 0
         self._timeout = timeout
 
+        # Set up logging
+        levels = ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
+        if logging_level not in levels:
+            raise TypeError("logging_level must be one of: " + ", ".join(levels))
+        log.setLevel(logging_level)
         # Store user's available tokens
         log.info("Connecting to keepa using key ending in %s", accesskey[-6:])
         self.update_status()
         log.info("%d tokens remain", self.tokens_left)
 
     @property
     def time_to_refill(self) -> float:
```

### Comparing `keepa-1.3.5/keepa/plotting.py` & `keepa-1.3.6/keepa/plotting.py`

 * *Files identical despite different names*

### Comparing `keepa-1.3.5/keepa/query_keys.py` & `keepa-1.3.6/keepa/query_keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -1041,9 +1041,10 @@
     "itemHeight_gte": int,
     "itemLength_lte": int,
     "itemLength_gte": int,
     "itemWidth_lte": int,
     "itemWidth_gte": int,
     "itemWeight_lte": int,
     "itemWeight_gte": int,
+    "singleVariation": bool,
     "sort": list,
 }
```

### Comparing `keepa-1.3.5/keepa.egg-info/PKG-INFO` & `keepa-1.3.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,307 +1,307 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: keepa
-Version: 1.3.5
+Version: 1.3.6
 Summary: Interfaces with keepa.com
 Home-page: https://github.com/akaszynski/keepa
 Author: Alex Kaszynski
 Author-email: akascap@gmail.com
 License: Apache Software License
+Description: Python keepa Client Library
+        ===========================
+        
+        .. image:: https://img.shields.io/pypi/v/keepa.svg?logo=python&logoColor=white
+           :target: https://pypi.org/project/keepa/
+        
+        .. image:: https://github.com/akaszynski/keepa/actions/workflows/testing-and-deployment.yml/badge.svg
+            :target: https://github.com/akaszynski/keepa/actions/workflows/testing-and-deployment.yml
+        
+        .. image:: https://readthedocs.org/projects/keepaapi/badge/?version=latest
+            :target: https://keepaapi.readthedocs.io/en/latest/?badge=latest
+            :alt: Documentation Status
+        
+        .. image:: https://codecov.io/gh/akaszynski/keepa/branch/main/graph/badge.svg
+          :target: https://codecov.io/gh/akaszynski/keepa
+        
+        .. image:: https://app.codacy.com/project/badge/Grade/9452f99f297c4a6eac14e2d21189ab6f
+          :target: https://www.codacy.com/gh/akaszynski/keepa/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=akaszynski/keepa&amp;utm_campaign=Badge_Grade
+        
+        
+        This Python library allows you to interface with the API at `Keepa
+        <https://keepa.com/>`_ to query for Amazon product information and
+        history.  It also contains a plotting module to allow for plotting of
+        a product.
+        
+        See API pricing at `Keepa API <https://keepa.com/#!api>`_.
+        
+        Documentation can be found on readthedocs at `keepa Documentation <https://keepaapi.readthedocs.io/en/latest/>`_.
+        
+        
+        Requirements
+        ------------
+        This library is compatible with Python >= 3.7 and requires:
+        
+        - ``numpy``
+        - ``aiohttp``
+        - ``matplotlib``
+        - ``tqdm``
+        
+        Product history can be plotted from the raw data when ``matplotlib``
+        is installed.
+        
+        Interfacing with the ``keepa`` requires an access key and a monthly
+        subscription from `Keepa API <https://keepa.com/#!api>`_
+        
+        Installation
+        ------------
+        Module can be installed from `PyPi <https://pypi.org/project/keepa/>`_ with:
+        
+        .. code::
+        
+            pip install keepa
+        
+        
+        Source code can also be downloaded from `GitHub
+        <https://github.com/akaszynski/keepa>`_ and installed using:
+        ``python setup.py install`` or ``pip install .``
+        
+        
+        Brief Example
+        -------------
+        .. code:: python
+        
+            import keepa
+            accesskey = 'XXXXXXXXXXXXXXXX' # enter real access key here
+            api = keepa.Keepa(accesskey)
+        
+            # Single ASIN query
+            products = api.query('B0088PUEPK') # returns list of product data
+        
+            # Plot result (requires matplotlib)
+            keepa.plot_product(products[0])
+        
+        .. figure:: https://github.com/akaszynski/keepa/raw/main/docs/source/images/Product_Price_Plot.png
+            :width: 500pt
+        
+            Product Price Plot
+        
+        .. figure:: https://github.com/akaszynski/keepa/raw/main/docs/source/images/Product_Offer_Plot.png
+            :width: 500pt
+        
+            Product Offers Plot
+        
+        
+        Brief Example using async
+        -------------------------
+        Here's an example of obtaining a product and plotting its price and
+        offer history using the ``keepa.AsyncKeepa`` class:
+        
+        .. code:: python
+        
+            >>> import asyncio
+            >>> import keepa
+            >>> product_parms = {'author': 'jim butcher'}
+            >>> async def main():
+            ...     key = '<REAL_KEEPA_KEY>'
+            ...     api = await keepa.AsyncKeepa().create(key)
+            ...     return await api.product_finder(product_parms)
+            >>> asins = asyncio.run(main())
+            >>> asins
+            ['B000HRMAR2',
+             '0578799790',
+             'B07PW1SVHM',
+            ...
+             'B003MXM744',
+             '0133235750',
+             'B01MXXLJPZ']
+        
+        Query for product with ASIN ``'B0088PUEPK'`` using the asynchronous
+        keepa interface.
+        
+        .. code:: python
+        
+            >>> import asyncio
+            >>> import keepa
+            >>> async def main():
+            ...     key = '<REAL_KEEPA_KEY>'
+            ...     api = await keepa.AsyncKeepa().create(key)
+            ...     return await api.query('B0088PUEPK')
+            >>> response = asyncio.run(main())
+            >>> response[0]['title']
+            'Western Digital 1TB WD Blue PC Internal Hard Drive HDD - 7200 RPM,
+            SATA 6 Gb/s, 64 MB Cache, 3.5" - WD10EZEX'
+        
+        
+        Detailed Examples
+        -----------------
+        Import interface and establish connection to server
+        
+        .. code:: python
+        
+            import keepa
+            accesskey = 'XXXXXXXXXXXXXXXX' # enter real access key here
+            api = keepa.Keepa(accesskey)
+        
+        
+        Single ASIN query
+        
+        .. code:: python
+        
+            products = api.query('059035342X')
+        
+            # See help(api.query) for available options when querying the API
+        
+        
+        You can use keepa witch async / await too
+        
+        .. code:: python
+        
+            import keepa
+            accesskey = 'XXXXXXXXXXXXXXXX' # enter real access key here
+            api = await keepa.AsyncKeepa.create(accesskey)
+        
+        
+        Single ASIN query (async)
+        
+        .. code:: python
+        
+            products = await api.query('059035342X')
+        
+        
+        Multiple ASIN query from List
+        
+        .. code:: python
+        
+            asins = ['0022841350', '0022841369', '0022841369', '0022841369']
+            products = api.query(asins)
+        
+        Multiple ASIN query from numpy array
+        
+        .. code:: python
+        
+            asins = np.asarray(['0022841350', '0022841369', '0022841369', '0022841369'])
+            products = api.query(asins)
+        
+        Products is a list of product data with one entry per successful result from the Keepa server. Each entry is a dictionary containing the same product data available from `Amazon <http://www.amazon.com>`_.
+        
+        .. code:: python
+        
+            # Available keys
+            print(products[0].keys())
+        
+            # Print ASIN and title
+            print('ASIN is ' + products[0]['asin'])
+            print('Title is ' + products[0]['title'])
+        
+        The raw data is contained within each product result. Raw data is stored as a dictionary with each key paired with its associated time history.
+        
+        .. code:: python
+        
+            # Access new price history and associated time data
+            newprice = products[0]['data']['NEW']
+            newpricetime = products[0]['data']['NEW_time']
+        
+            # Can be plotted with matplotlib using:
+            import matplotlib.pyplot as plt
+            plt.step(newpricetime, newprice, where='pre')
+        
+            # Keys can be listed by
+            print(products[0]['data'].keys())
+        
+        The product history can also be plotted from the module if ``matplotlib`` is installed
+        
+        .. code:: python
+        
+            keepa.plot_product(products[0])
+        
+        You can obtain the offers history for an ASIN (or multiple ASINs) using the ``offers`` parameter.  See the documentation at `Request Products <https://keepa.com/#!discuss/t/request-products/110/1>`_ for further details.
+        
+        .. code:: python
+        
+            products = api.query(asins, offers=20)
+            product = products[0]
+            offers = product['offers']
+        
+            # each offer contains the price history of each offer
+            offer = offers[0]
+            csv = offer['offerCSV']
+        
+            # convert these values to numpy arrays
+            times, prices = keepa.convert_offer_history(csv)
+        
+            # for a list of active offers, see
+            indices = product['liveOffersOrder']
+        
+            # with this you can loop through active offers:
+            indices = product['liveOffersOrder']
+            offer_times = []
+            offer_prices = []
+            for index in indices:
+                csv = offers[index]['offerCSV']
+                times, prices = keepa.convert_offer_history(csv)
+                offer_times.append(times)
+                offer_prices.append(prices)
+        
+            # you can aggregate these using np.hstack or plot at the history individually
+            import matplotlib.pyplot as plt
+            for i in range(len(offer_prices)):
+                plt.step(offer_times[i], offer_prices[i])
+            plt.show()
+        
+        If you plan to do a lot of simulatneous query, you might want to speedup query using
+        ``wait=False`` arguments.
+        
+        .. code:: python
+        
+            products = await api.query('059035342X', wait=False)
+        
+        
+        Contributing
+        ------------
+        Contribute to this repository by forking this repository and installing in
+        development mode with::
+        
+          git clone https://github.com/<USERNAME>/keepa
+          pip install -e .
+        
+        You can then add your feature or commit your bug fix and then run your unit
+        testing with::
+        
+          pip install requirements_test.txt
+          pytest
+        
+        Unit testing will automatically enforce minimum code coverage standards.
+        
+        Next, to ensure your code meets minimum code styling standards, run::
+        
+          pip install pre-commit
+          pre-commit run --all-files
+        
+        Finally, `create a pull request`_ from your fork and I'll be sure to review it.
+        
+        
+        Credits
+        -------
+        This Python module, written by Alex Kaszynski and several contribitors, is
+        based on Java code written by Marius Johann, CEO Keepa. Java source is can be
+        found at `keepacom/api_backend <https://github.com/keepacom/api_backend/>`_.
+        
+        
+        License
+        -------
+        Apache License, please see license file. Work is credited to both Alex
+        Kaszynski and Marius Johann.
+        
+        
+        .. _create a pull request: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request
+        
 Keywords: keepa
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Database :: Front-Ends
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-License-File: LICENSE
-
-keepa
-=====
-
-.. image:: https://img.shields.io/pypi/v/keepa.svg?logo=python&logoColor=white
-   :target: https://pypi.org/project/keepa/
-
-.. image:: https://travis-ci.org/akaszynski/keepa.svg?branch=master
-    :target: https://travis-ci.org/akaszynski/keepa
-
-.. image:: https://readthedocs.org/projects/keepaapi/badge/?version=latest
-    :target: https://keepaapi.readthedocs.io/en/latest/?badge=latest
-    :alt: Documentation Status
-
-.. image:: https://codecov.io/gh/akaszynski/keepa/branch/master/graph/badge.svg
-  :target: https://codecov.io/gh/akaszynski/keepa
-
-.. image:: https://app.codacy.com/project/badge/Grade/9452f99f297c4a6eac14e2d21189ab6f
-  :target: https://www.codacy.com/gh/akaszynski/keepa/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=akaszynski/keepa&amp;utm_campaign=Badge_Grade
-
-
-This Python module allows you to interface with the API at `Keepa
-<https://keepa.com/>`_ to query for Amazon product information and
-history.  It also contains a plotting module to allow for plotting of
-a product.
-
-See API pricing at `Keepa API <https://keepa.com/#!api>`_
-
-Documentation can be found on readthedocs at `keepa Documentation <https://keepaapi.readthedocs.io/en/latest/>`_.
-
-
-Requirements
-------------
-Module is compatible with Python >= 3.6 and requires:
-
-- ``numpy``
-- ``aiohttp``
-- ``matplotlib``
-- ``tqdm``
-
-Product history can be plotted from the raw data when ``matplotlib``
-is installed.
-
-Interfacing with the ``keepa`` requires an access key and a monthly
-subscription from `Keepa API <https://keepa.com/#!api>`_
-
-Installation
-------------
-Module can be installed from `PyPi <https://pypi.org/project/keepa/>`_ with:
-
-.. code::
-
-    pip install keepa
-
-
-Source code can also be downloaded from `GitHub
-<https://github.com/akaszynski/keepa>`_ and installed using:
-``python setup.py install`` or ``pip install .``
-
-
-Brief Example
--------------
-.. code:: python
-
-    import keepa
-    accesskey = 'XXXXXXXXXXXXXXXX' # enter real access key here
-    api = keepa.Keepa(accesskey)
-
-    # Single ASIN query
-    products = api.query('B0088PUEPK') # returns list of product data
-
-    # Plot result (requires matplotlib)
-    keepa.plot_product(products[0])
-
-.. figure:: https://github.com/akaszynski/keepa/raw/master/docs/source/images/Product_Price_Plot.png
-    :width: 500pt
-
-    Product Price Plot
-
-.. figure:: https://github.com/akaszynski/keepa/raw/master/docs/source/images/Product_Offer_Plot.png
-    :width: 500pt
-
-    Product Offers Plot
-
-
-Brief Example using async
--------------------------
-Here's an example of obtaining a product and plotting its price and
-offer history using the ``keepa.AsyncKeepa`` class:
-
-.. code:: python
-
-    >>> import asyncio
-    >>> import keepa
-    >>> product_parms = {'author': 'jim butcher'}
-    >>> async def main():
-    ...     key = '<REAL_KEEPA_KEY>'
-    ...     api = await keepa.AsyncKeepa().create(key)
-    ...     return await api.product_finder(product_parms)
-    >>> asins = asyncio.run(main())
-    >>> asins
-    ['B000HRMAR2',
-     '0578799790',
-     'B07PW1SVHM',
-    ...
-     'B003MXM744',
-     '0133235750',
-     'B01MXXLJPZ']
-
-Query for product with ASIN ``'B0088PUEPK'`` using the asynchronous
-keepa interface.
-
-.. code:: python
-
-    >>> import asyncio
-    >>> import keepa
-    >>> async def main():
-    ...     key = '<REAL_KEEPA_KEY>'
-    ...     api = await keepa.AsyncKeepa().create(key)
-    ...     return await api.query('B0088PUEPK')
-    >>> response = asyncio.run(main())
-    >>> response[0]['title']
-    'Western Digital 1TB WD Blue PC Internal Hard Drive HDD - 7200 RPM,
-    SATA 6 Gb/s, 64 MB Cache, 3.5" - WD10EZEX'
-
-
-Detailed Examples
------------------
-Import interface and establish connection to server
-
-.. code:: python
-
-    import keepa
-    accesskey = 'XXXXXXXXXXXXXXXX' # enter real access key here
-    api = keepa.Keepa(accesskey)
-
-
-Single ASIN query
-
-.. code:: python
-
-    products = api.query('059035342X')
-
-    # See help(api.query) for available options when querying the API
-
-
-You can use keepa witch async / await too
-
-.. code:: python
-
-    import keepa
-    accesskey = 'XXXXXXXXXXXXXXXX' # enter real access key here
-    api = await keepa.AsyncKeepa.create(accesskey)
-
-
-Single ASIN query (async)
-
-.. code:: python
-
-    products = await api.query('059035342X')
-
-
-Multiple ASIN query from List
-
-.. code:: python
-
-    asins = ['0022841350', '0022841369', '0022841369', '0022841369']
-    products = api.query(asins)
-
-Multiple ASIN query from numpy array
-
-.. code:: python
-
-    asins = np.asarray(['0022841350', '0022841369', '0022841369', '0022841369'])
-    products = api.query(asins)
-
-Products is a list of product data with one entry per successful result from the Keepa server. Each entry is a dictionary containing the same product data available from `Amazon <http://www.amazon.com>`_.
-
-.. code:: python
-
-    # Available keys
-    print(products[0].keys())
-
-    # Print ASIN and title
-    print('ASIN is ' + products[0]['asin'])
-    print('Title is ' + products[0]['title'])
-
-The raw data is contained within each product result. Raw data is stored as a dictionary with each key paired with its associated time history.
-
-.. code:: python
-
-    # Access new price history and associated time data
-    newprice = products[0]['data']['NEW']
-    newpricetime = products[0]['data']['NEW_time']
-
-    # Can be plotted with matplotlib using:
-    import matplotlib.pyplot as plt
-    plt.step(newpricetime, newprice, where='pre')
-
-    # Keys can be listed by
-    print(products[0]['data'].keys())
-
-The product history can also be plotted from the module if ``matplotlib`` is installed
-
-.. code:: python
-
-    keepa.plot_product(products[0])
-
-You can obtain the offers history for an ASIN (or multiple ASINs) using the ``offers`` parameter.  See the documentation at `Request Products <https://keepa.com/#!discuss/t/request-products/110/1>`_ for further details.
-
-.. code:: python
-
-    products = api.query(asins, offers=20)
-    product = products[0]
-    offers = product['offers']
-
-    # each offer contains the price history of each offer
-    offer = offers[0]
-    csv = offer['offerCSV']
-
-    # convert these values to numpy arrays
-    times, prices = keepa.convert_offer_history(csv)
-
-    # for a list of active offers, see
-    indices = product['liveOffersOrder']
-
-    # with this you can loop through active offers:
-    indices = product['liveOffersOrder']
-    offer_times = []
-    offer_prices = []
-    for index in indices:
-        csv = offers[index]['offerCSV']
-        times, prices = keepa.convert_offer_history(csv)
-        offer_times.append(times)
-        offer_prices.append(prices)
-
-    # you can aggregate these using np.hstack or plot at the history individually
-    import matplotlib.pyplot as plt
-    for i in range(len(offer_prices)):
-        plt.step(offer_times[i], offer_prices[i])
-    plt.show()
-
-If you plan to do a lot of simulatneous query, you might want to speedup query using
-``wait=False`` arguments.
-
-.. code:: python
-
-    products = await api.query('059035342X', wait=False)
-
-
-Contributing
-------------
-Contribute to this repository by forking this repository and installing in
-development mode with::
-
-  git clone https://github.com/<USERNAME>/keepa
-  pip install -e .
-
-You can then add your feature or commit your bug fix and then run your unit
-testing with::
-
-  pip install requirements_test.txt
-  pytest
-
-Unit testing will automatically enforce minimum code coverage standards.
-
-Next, to ensure your code meets minimum code styling standards, run::
-
-  pip install pre-commit
-  pre-commit run --all-files
-
-Finally, `create a pull request`_ from your fork and I'll be sure to review it.
-
-
-Credits
--------
-This Python module, written by Alex Kaszynski and several contribitors, is
-based on Java code written by Marius Johann, CEO Keepa. Java source is can be
-found at `keepacom/api_backend <https://github.com/keepacom/api_backend/>`_.
-
-
-License
--------
-Apache License, please see license file. Work is credited to both Alex
-Kaszynski and Marius Johann.
-
-
-.. _create a pull request: https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request
```

### Comparing `keepa-1.3.5/setup.py` & `keepa-1.3.6/setup.py`

 * *Files identical despite different names*

