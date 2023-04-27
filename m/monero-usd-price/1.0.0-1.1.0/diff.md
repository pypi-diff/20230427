# Comparing `tmp/monero_usd_price-1.0.0.tar.gz` & `tmp/monero_usd_price-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monero_usd_price-1.0.0.tar", last modified: Sat Apr 22 02:40:59 2023, max compression
+gzip compressed data, was "monero_usd_price-1.1.0.tar", last modified: Thu Apr 27 02:25:18 2023, max compression
```

## Comparing `monero_usd_price-1.0.0.tar` & `monero_usd_price-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 02:40:59.798940 monero_usd_price-1.0.0/
--rw-rw-rw-   0        0        0      466 2023-04-22 02:40:59.798940 monero_usd_price-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1622 2023-04-22 02:38:56.000000 monero_usd_price-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 02:40:59.794939 monero_usd_price-1.0.0/monero_usd_price/
--rw-rw-rw-   0        0        0       33 2023-04-22 02:06:02.000000 monero_usd_price-1.0.0/monero_usd_price/__init__.py
--rw-rw-rw-   0        0        0     9881 2023-04-22 01:20:57.000000 monero_usd_price-1.0.0/monero_usd_price/monero_usd_price.py
-drwxrwxrwx   0        0        0        0 2023-04-22 02:40:59.797940 monero_usd_price-1.0.0/monero_usd_price.egg-info/
--rw-rw-rw-   0        0        0      466 2023-04-22 02:40:59.000000 monero_usd_price-1.0.0/monero_usd_price.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-04-22 02:40:59.000000 monero_usd_price-1.0.0/monero_usd_price.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 02:40:59.000000 monero_usd_price-1.0.0/monero_usd_price.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-22 02:40:59.000000 monero_usd_price-1.0.0/monero_usd_price.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-22 02:40:59.000000 monero_usd_price-1.0.0/monero_usd_price.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 02:40:59.798940 monero_usd_price-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      609 2023-04-22 02:10:35.000000 monero_usd_price-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 02:25:18.610567 monero_usd_price-1.1.0/
+-rw-rw-rw-   0        0        0      466 2023-04-27 02:25:18.609567 monero_usd_price-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1622 2023-04-22 02:38:56.000000 monero_usd_price-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 02:25:18.605567 monero_usd_price-1.1.0/monero_usd_price/
+-rw-rw-rw-   0        0        0       33 2023-04-22 02:06:02.000000 monero_usd_price-1.1.0/monero_usd_price/__init__.py
+-rw-rw-rw-   0        0        0    12290 2023-04-27 02:22:31.000000 monero_usd_price-1.1.0/monero_usd_price/monero_usd_price.py
+drwxrwxrwx   0        0        0        0 2023-04-27 02:25:18.609567 monero_usd_price-1.1.0/monero_usd_price.egg-info/
+-rw-rw-rw-   0        0        0      466 2023-04-27 02:25:18.000000 monero_usd_price-1.1.0/monero_usd_price.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-04-27 02:25:18.000000 monero_usd_price-1.1.0/monero_usd_price.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 02:25:18.000000 monero_usd_price-1.1.0/monero_usd_price.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-27 02:25:18.000000 monero_usd_price-1.1.0/monero_usd_price.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-27 02:25:18.000000 monero_usd_price-1.1.0/monero_usd_price.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-27 02:25:18.610567 monero_usd_price-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      609 2023-04-27 02:24:04.000000 monero_usd_price-1.1.0/setup.py
```

### Comparing `monero_usd_price-1.0.0/README.md` & `monero_usd_price-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `monero_usd_price-1.0.0/monero_usd_price/monero_usd_price.py` & `monero_usd_price-1.1.0/monero_usd_price/monero_usd_price.py`

 * *Files 16% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         if ticker:
             xmr_usd_rate = round(float(ticker.get('last')), 2)  # round to 2 decimals
             print(f'HitBTC: {xmr_usd_rate}') if print_price_to_console else None
             return xmr_usd_rate
     return None
 
 
-def get_monero_price_from_all_exchanges(print_price_to_console=False):
+def get_monero_price_from_all_exchanges_not_threaded(print_price_to_console=False):
     prices = []
 
     coingecko_price = coingecko(print_price_to_console=print_price_to_console)
     if coingecko_price:
         prices.append(coingecko_price)
 
     coinmarketcap_price = coinmarketcap(print_price_to_console=print_price_to_console)
@@ -174,14 +174,34 @@
         sorted_prices = sorted(prices)  # low to high
         return sorted_prices
     else:
         print("Error! Didn't get any XMR/USD prices!")
         return None
 
 
+def get_monero_price_from_all_exchanges(print_price_to_console=False):
+    from concurrent.futures import ThreadPoolExecutor, as_completed
+    prices = []
+
+    with ThreadPoolExecutor(max_workers=10) as executor:
+        futures = [executor.submit(func, print_price_to_console=print_price_to_console) for func in [coingecko, coinmarketcap, binance, cryptocompare, kraken, bitfinex, localmonero, poloniex, huobi, kucoin, hitbtc]]
+
+        for future in as_completed(futures):
+            price = future.result()
+            if price:
+                prices.append(price)
+
+    if len(prices) >= 1:  # Make sure that getting at least 1 price was successful
+        sorted_prices = sorted(prices)  # low to high
+        return sorted_prices
+    else:
+        print("Error! Didn't get any XMR/USD prices!")
+        return None
+
+
 def average_price(print_price_to_console=False):
     # RECOMMENDED TO USE MEDIAN INSTEAD OF AVERAGE
     sorted_prices = get_monero_price_from_all_exchanges(print_price_to_console=print_price_to_console)
     if sorted_prices:
         # Get average price
         avg_price = sum(sorted_prices) / len(sorted_prices)
         # round to 2 decimals
@@ -207,14 +227,47 @@
 
         print(f'\nMedian price is: {median_price} out of {len(sorted_prices)} exchanges') if print_price_to_console else None
         return median_price
     else:
         return None
 
 
+def average_price_not_threaded(print_price_to_console=False):
+    # RECOMMENDED TO USE MEDIAN INSTEAD OF AVERAGE
+    sorted_prices = get_monero_price_from_all_exchanges_not_threaded(print_price_to_console=print_price_to_console)
+    if sorted_prices:
+        # Get average price
+        avg_price = sum(sorted_prices) / len(sorted_prices)
+        # round to 2 decimals
+        avg_price = round(avg_price, 2)
+        print(f'\nAverage price is: {avg_price} out of {len(sorted_prices)} exchanges') if print_price_to_console else None
+        return avg_price
+    else:
+        return None
+
+
+def median_price_not_threaded(print_price_to_console=False):
+    sorted_prices = get_monero_price_from_all_exchanges_not_threaded(print_price_to_console=print_price_to_console)
+    if sorted_prices:
+        # Get median price (less sensitive to outliers than average)
+        if len(sorted_prices) % 2 == 1:
+            # If the length of the list is odd, return the middle element
+            median_price = sorted_prices[len(sorted_prices) // 2]
+        else:
+            # If the length of the list is even, return the average of the two middle elements
+            median_price = (sorted_prices[len(sorted_prices) // 2 - 1] + sorted_prices[len(sorted_prices) // 2]) / 2
+
+        median_price = round(median_price, 2)  # round to 2 decimals
+
+        print(f'\nMedian price is: {median_price} out of {len(sorted_prices)} exchanges') if print_price_to_console else None
+        return median_price
+    else:
+        return None
+
+
 def print_monero_logo():
     print('''
                     k                                     d                   
                     0Kx                                 dOX                   
                     KMWKx                             dONMN                   
                     KMMMWKx                         dONMMMN                   
                     KMMMMMWKk                     d0NMMMMMN                   
@@ -224,8 +277,8 @@
                     KMMMMMXkNMMMMMMXk     dKWMMMMMW00MMMMMN                   
                     KMMMMM0  xNMMMMMMXk dKWMMMMMWOc dMMMMMN                   
                     KMMMMM0    xNMMMMMMNWMMMMMWOc   dMMMMMN                   
                     KMMMMM0      dXMMMMMMMMMNkc     dMMMMMN                   
                     KMMMMM0        oXMMMMMNx;       dMMMMMN                   
 KMMMMMMMMMMMMMMMMMMMMMMMMM0          dNMWk:         dMMMMMMMMMMMMMMMMMMMMMMMMK
 KMMMMMMMMMMMMMMMMMMMMMMMMM0            o            dMMMMMMMMMMMMMMMMMMMMMMMMK
-KMMMMMMMMMMMMMWNNNNNNNNNNNO                         oNNNNNNNNNNNNMMMMMMMMMMMMO''')
+KMMMMMMMMMMMMMWNNNNNNNNNNNO                         oNNNNNNNNNNNNMMMMMMMMMMMMO''')
```

### Comparing `monero_usd_price-1.0.0/setup.py` & `monero_usd_price-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='monero_usd_price',
-    version='1.0.0',
+    version='1.1.0',
     author="Luke Profits",
     description="Monero-USD-Price is an easy way to get the current median or average price of Monero (median is recommended over average, because it less sensitive to outliers.)",
     url="https://github.com/lukeprofits/Monero-USD-Price",
     packages=['monero_usd_price'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

