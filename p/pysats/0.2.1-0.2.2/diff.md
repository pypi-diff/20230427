# Comparing `tmp/pysats-0.2.1.tar.gz` & `tmp/pysats-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysats-0.2.1.tar", max compression
+gzip compressed data, was "pysats-0.2.2.tar", max compression
```

## Comparing `pysats-0.2.1.tar` & `pysats-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    34519 2023-02-08 08:00:31.622670 pysats-0.2.1/LICENSE
--rw-r--r--   0        0        0     1745 2023-02-08 08:00:31.622670 pysats-0.2.1/README.md
--rw-r--r--   0        0        0      565 2023-02-08 09:10:26.708327 pysats-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       43 2023-02-08 08:00:31.622670 pysats-0.2.1/pysats/__init__.py
--rw-r--r--   0        0        0     4991 2023-02-08 08:00:31.622670 pysats-0.2.1/pysats/generic_model.py
--rw-r--r--   0        0        0     1526 2023-02-08 08:00:31.622670 pysats-0.2.1/pysats/gsvm.py
--rw-r--r--   0        0        0     1525 2023-02-08 08:00:31.622670 pysats-0.2.1/pysats/lsvm.py
--rw-r--r--   0        0        0     1674 2023-02-08 08:00:31.622670 pysats-0.2.1/pysats/mrvm.py
--rw-r--r--   0        0        0     2084 2023-02-08 08:00:31.622670 pysats-0.2.1/pysats/pysats.py
--rw-r--r--   0        0        0     8543 2023-02-08 08:00:31.622670 pysats-0.2.1/pysats/simple_model.py
--rw-r--r--   0        0        0     1929 2023-02-08 08:00:31.622670 pysats-0.2.1/pysats/srvm.py
--rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 pysats-0.2.1/setup.py
--rw-r--r--   0        0        0     2560 1970-01-01 00:00:00.000000 pysats-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    34519 2023-02-08 08:00:31.622670 pysats-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1745 2023-02-08 08:00:31.622670 pysats-0.2.2/README.md
+-rw-r--r--   0        0        0      565 2023-04-27 09:15:59.095024 pysats-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-04-13 09:52:12.933546 pysats-0.2.2/pysats/__init__.py
+-rw-r--r--   0        0        0     5522 2023-04-27 09:11:57.456446 pysats-0.2.2/pysats/generic_model.py
+-rw-r--r--   0        0        0     1591 2023-04-13 09:52:12.963547 pysats-0.2.2/pysats/gsvm.py
+-rw-r--r--   0        0        0     1590 2023-04-13 09:52:12.963547 pysats-0.2.2/pysats/lsvm.py
+-rw-r--r--   0        0        0     1740 2023-04-13 09:52:12.983548 pysats-0.2.2/pysats/mrvm.py
+-rw-r--r--   0        0        0     2600 2023-04-13 09:52:13.023548 pysats-0.2.2/pysats/pysats.py
+-rw-r--r--   0        0        0     8945 2023-04-27 09:13:41.985501 pysats-0.2.2/pysats/simple_model.py
+-rw-r--r--   0        0        0     2001 2023-04-13 09:52:12.973547 pysats-0.2.2/pysats/srvm.py
+-rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 pysats-0.2.2/setup.py
+-rw-r--r--   0        0        0     2560 1970-01-01 00:00:00.000000 pysats-0.2.2/PKG-INFO
```

### Comparing `pysats-0.2.1/LICENSE` & `pysats-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysats-0.2.1/README.md` & `pysats-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pysats-0.2.1/pyproject.toml` & `pysats-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysats"
-version = "0.2.1"
+version = "0.2.2"
 description = "GNU Affero General Public License v3"
 authors = ["Fabio Isler <islerfab@gmail.com>"]
 readme = "README.md"
 license = "GNU Affero General Public License v3"
 homepage = "https://github.com/marketdesignresearch/pysats"
 repository = "https://github.com/marketdesignresearch/pysats"
```

### Comparing `pysats-0.2.1/pysats/generic_model.py` & `pysats-0.2.2/pysats/generic_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,80 +1,117 @@
 from jnius import autoclass, cast
 from .simple_model import SimpleModel
 
-LinkedHashMap = autoclass('java.util.LinkedHashMap')
-Price = autoclass('org.marketdesignresearch.mechlib.core.price.Price')
-LinearPrices = autoclass('org.marketdesignresearch.mechlib.core.price.LinearPrices')
+LinkedHashMap = autoclass("java.util.LinkedHashMap")
+Price = autoclass("org.marketdesignresearch.mechlib.core.price.Price")
+LinearPrices = autoclass("org.marketdesignresearch.mechlib.core.price.LinearPrices")
 
-class GenericModel(SimpleModel):
 
-    def __init__(self, seed, mip_path: str, generic_definition_path: str, store_files=False):
+class GenericModel(SimpleModel):
+    def __init__(
+        self, seed, mip_path: str, generic_definition_path: str, store_files=False
+    ):
         super().__init__(seed, mip_path, store_files)
         self.generic_definition_path = generic_definition_path
 
-    def get_random_bids(self, bidder_id, number_of_bids, seed=None, mean_bundle_size=49, standard_deviation_bundle_size=24.5):
+    def get_random_bids(
+        self,
+        bidder_id,
+        number_of_bids,
+        seed=None,
+        mean_bundle_size=49,
+        standard_deviation_bundle_size=24.5,
+    ):
         """
         Keeping this one because of the different default values that were set.
         """
-        return super().get_random_bids(bidder_id, number_of_bids, seed, mean_bundle_size, standard_deviation_bundle_size)
-    
+        return super().get_random_bids(
+            bidder_id,
+            number_of_bids,
+            seed,
+            mean_bundle_size,
+            standard_deviation_bundle_size,
+        )
+
     def get_efficient_allocation(self, display_output=False):
         """
         The efficient allocation is calculated on a generic definition. It is then "translated" into individual licenses that are assigned to bidders.
         Note that this does NOT result in a consistent allocation, since a single license can be assigned to multiple bidders.
         The value per bidder is still consistent, which is why this method can still be useful.
         """
         if self.efficient_allocation:
-            return self.efficient_allocation, sum([self.efficient_allocation[bidder_id]['value'] for bidder_id in self.efficient_allocation.keys()])
+            return self.efficient_allocation, sum(
+                [
+                    self.efficient_allocation[bidder_id]["value"]
+                    for bidder_id in self.efficient_allocation.keys()
+                ]
+            )
 
         mip = autoclass(self.mip_path)(self._bidder_list)
         mip.setDisplayOutput(display_output)
 
         allocation = mip.calculateAllocation()
 
         self.efficient_allocation = {}
 
         available = self.get_good_ids()
 
         for bidder_id, bidder in self.population.items():
             self.efficient_allocation[bidder_id] = {}
-            self.efficient_allocation[bidder_id]['good_ids'] = []
+            self.efficient_allocation[bidder_id]["good_ids"] = []
             if allocation.getWinners().contains(bidder):
                 bidder_allocation = allocation.allocationOf(bidder)
-                bundle_entry_iterator = bidder_allocation.getBundle().getBundleEntries().iterator()
+                bundle_entry_iterator = (
+                    bidder_allocation.getBundle().getBundleEntries().iterator()
+                )
                 while bundle_entry_iterator.hasNext():
                     bundle_entry = bundle_entry_iterator.next()
                     count = bundle_entry.getAmount()
-                    licenses_iterator = cast(self.generic_definition_path, bundle_entry.getGood()).containedGoods().iterator()
+                    licenses_iterator = (
+                        cast(self.generic_definition_path, bundle_entry.getGood())
+                        .containedGoods()
+                        .iterator()
+                    )
                     given = 0
                     while licenses_iterator.hasNext() and given < count:
                         lic_id = licenses_iterator.next().getLongId()
                         if lic_id in available:
-                            self.efficient_allocation[bidder_id]['good_ids'].append(lic_id)
+                            self.efficient_allocation[bidder_id]["good_ids"].append(
+                                lic_id
+                            )
                             available.remove(lic_id)
                             given += 1
                     assert given == count
 
-            self.efficient_allocation[bidder_id]['value'] = bidder_allocation.getValue().doubleValue() if allocation.getWinners().contains(bidder) else 0.0
-
-        return self.efficient_allocation, allocation.getTotalAllocationValue().doubleValue()
+            self.efficient_allocation[bidder_id]["value"] = (
+                bidder_allocation.getValue().doubleValue()
+                if allocation.getWinners().contains(bidder)
+                else 0.0
+            )
+
+        return (
+            self.efficient_allocation,
+            allocation.getTotalAllocationValue().doubleValue(),
+        )
 
     def get_best_bundles(self, bidder_id, price_vector, max_number_of_bundles):
         """
         Careful: So far, it seems it was possible to sneak through PySats without caring about the fact that
         these models are generic. Generic means that there are subsets of goods that are complete comlements.
         From a set of goods (A{3}, B{2}) a bidder doesn't care if she gets the first, second or third A.
         For generic models, asking values is easy - if asked for A.1 or A.2, it will just return the same value.
         That's why it was OKish so far. For the efficient allocation above, the generic allocation was broken down
         into concrete licenses again, since it did not really matter - the value of this allocation was still consistent.
-        
+
         When asking demand queries, this model breaks. A bidder of a generic world expects a price vector of length 2 in
         the example above, with a price for good A and a price for good B. If we're in a concrete-licenses world, we
         would have to ask with a price vector [price(A), price(A), price(A), price(B), price(B)]. I'm currently not sure
-        where this inconsistent use of generic and concrete models would cause problems, but my fear is that it's in 
+        where this inconsistent use of generic and concrete models would cause problems, but my fear is that it's in
         the core idea itself, while it would technically run through. So think twice if you want to use PySats for generic
         demand queries - and if you need it, we'll need to carefully think about this and implement it.
-        
+
         We're not even talking about the fact that breaking down a generic model into concrete goods is highly inefficient
         and it's going a step away from the original idea of generic models - losing much of its power...
         """
-        raise NotImplementedError("Generic models are not yet supported for demand queries.")
+        raise NotImplementedError(
+            "Generic models are not yet supported for demand queries."
+        )
```

### Comparing `pysats-0.2.1/pysats/gsvm.py` & `pysats-0.2.2/pysats/gsvm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 from jnius import MetaJavaClass, JavaMethod
 from .simple_model import SimpleModel
 
+
 class _Gsvm(SimpleModel, metaclass=MetaJavaClass):
     # We have to define the java class and any method we're going to use in this child class
-    __javaclass__ = 'org/spectrumauctions/sats/core/model/gsvm/GlobalSynergyValueModel'
-    setNumberOfNationalBidders = JavaMethod('(I)V')
-    setNumberOfRegionalBidders = JavaMethod('(I)V')
+    __javaclass__ = "org/spectrumauctions/sats/core/model/gsvm/GlobalSynergyValueModel"
+    setNumberOfNationalBidders = JavaMethod("(I)V")
+    setNumberOfRegionalBidders = JavaMethod("(I)V")
     createWorld = JavaMethod(
-        '(Lorg/spectrumauctions/sats/core/util/random/RNGSupplier;)Lorg/spectrumauctions/sats/core/model/gsvm/GSVMWorld;')
+        "(Lorg/spectrumauctions/sats/core/util/random/RNGSupplier;)Lorg/spectrumauctions/sats/core/model/gsvm/GSVMWorld;"
+    )
     createPopulation = JavaMethod(
-        '(Lorg/spectrumauctions/sats/core/model/World;Lorg/spectrumauctions/sats/core/util/random/RNGSupplier;)Ljava/util/List;')
-    setLegacyGSVM = JavaMethod('(Z)V')
+        "(Lorg/spectrumauctions/sats/core/model/World;Lorg/spectrumauctions/sats/core/util/random/RNGSupplier;)Ljava/util/List;"
+    )
+    setLegacyGSVM = JavaMethod("(Z)V")
 
-    def __init__(self, seed, number_of_national_bidders, number_of_regional_bidders, isLegacyGSVM=False, store_files=False):
+    def __init__(
+        self,
+        seed,
+        number_of_national_bidders,
+        number_of_regional_bidders,
+        isLegacyGSVM=False,
+        store_files=False,
+    ):
         self.number_of_national_bidders = number_of_national_bidders
         self.number_of_regional_bidders = number_of_regional_bidders
         self.isLegacy = isLegacyGSVM
         super().__init__(
             seed=seed,
-            mip_path='org.spectrumauctions.sats.opt.model.gsvm.GSVMStandardMIP',
-            store_files=store_files
+            mip_path="org.spectrumauctions.sats.opt.model.gsvm.GSVMStandardMIP",
+            store_files=store_files,
         )
 
     def prepare_world(self):
         self.setNumberOfNationalBidders(self.number_of_national_bidders)
         self.setNumberOfRegionalBidders(self.number_of_regional_bidders)
         self.setLegacyGSVM(self.isLegacy)
 
     def get_model_name(self):
-        return ('GSVM')
+        return "GSVM"
```

### Comparing `pysats-0.2.1/pysats/lsvm.py` & `pysats-0.2.2/pysats/lsvm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 from jnius import MetaJavaClass, JavaMethod
 from .simple_model import SimpleModel
 
+
 class _Lsvm(SimpleModel, metaclass=MetaJavaClass):
     # We have to define the java class and any method we're going to use in this child class
-    __javaclass__ = 'org/spectrumauctions/sats/core/model/lsvm/LocalSynergyValueModel'
-    setNumberOfNationalBidders = JavaMethod('(I)V')
-    setNumberOfRegionalBidders = JavaMethod('(I)V')
+    __javaclass__ = "org/spectrumauctions/sats/core/model/lsvm/LocalSynergyValueModel"
+    setNumberOfNationalBidders = JavaMethod("(I)V")
+    setNumberOfRegionalBidders = JavaMethod("(I)V")
     createWorld = JavaMethod(
-        '(Lorg/spectrumauctions/sats/core/util/random/RNGSupplier;)Lorg/spectrumauctions/sats/core/model/lsvm/LSVMWorld;')
+        "(Lorg/spectrumauctions/sats/core/util/random/RNGSupplier;)Lorg/spectrumauctions/sats/core/model/lsvm/LSVMWorld;"
+    )
     createPopulation = JavaMethod(
-        '(Lorg/spectrumauctions/sats/core/model/World;Lorg/spectrumauctions/sats/core/util/random/RNGSupplier;)Ljava/util/List;')
-    setLegacyLSVM = JavaMethod('(Z)V')
-
+        "(Lorg/spectrumauctions/sats/core/model/World;Lorg/spectrumauctions/sats/core/util/random/RNGSupplier;)Ljava/util/List;"
+    )
+    setLegacyLSVM = JavaMethod("(Z)V")
 
-    def __init__(self, seed, number_of_national_bidders, number_of_regional_bidders, isLegacyLSVM=False, store_files=False):
+    def __init__(
+        self,
+        seed,
+        number_of_national_bidders,
+        number_of_regional_bidders,
+        isLegacyLSVM=False,
+        store_files=False,
+    ):
         self.number_of_national_bidders = number_of_national_bidders
         self.number_of_regional_bidders = number_of_regional_bidders
         self.isLegacy = isLegacyLSVM
         super().__init__(
             seed=seed,
-            mip_path='org.spectrumauctions.sats.opt.model.lsvm.LSVMStandardMIP',
-            store_files=store_files
+            mip_path="org.spectrumauctions.sats.opt.model.lsvm.LSVMStandardMIP",
+            store_files=store_files,
         )
 
     def prepare_world(self):
         self.setNumberOfNationalBidders(self.number_of_national_bidders)
         self.setNumberOfRegionalBidders(self.number_of_regional_bidders)
         self.setLegacyLSVM(self.isLegacy)
 
     def get_model_name(self):
-        return ('LSVM')
+        return "LSVM"
```

### Comparing `pysats-0.2.1/pysats/mrvm.py` & `pysats-0.2.2/pysats/srvm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,46 @@
 from jnius import MetaJavaClass, JavaMethod
 from .generic_model import GenericModel
 
-class _Mrvm(GenericModel, metaclass=MetaJavaClass):
+
+class _Srvm(GenericModel, metaclass=MetaJavaClass):
     # We have to define the java class and any method we're going to use in this child class
-    __javaclass__ ='org/spectrumauctions/sats/core/model/mrvm/MultiRegionModel'
-    setNumberOfNationalBidders = JavaMethod('(I)V')
-    setNumberOfRegionalBidders = JavaMethod('(I)V')
-    setNumberOfLocalBidders = JavaMethod('(I)V')
+    __javaclass__ = "org/spectrumauctions/sats/core/model/srvm/SingleRegionModel"
+    setNumberOfSmallBidders = JavaMethod("(I)V")
+    setNumberOfHighFrequencyBidders = JavaMethod("(I)V")
+    setNumberOfSecondaryBidders = JavaMethod("(I)V")
+    setNumberOfPrimaryBidders = JavaMethod("(I)V")
     createWorld = JavaMethod(
-        '(Lorg/spectrumauctions/sats/core/util/random/RNGSupplier;)Lorg/spectrumauctions/sats/core/model/World;')
+        "(Lorg/spectrumauctions/sats/core/util/random/RNGSupplier;)Lorg/spectrumauctions/sats/core/model/srvm/SRVMWorld;"
+    )
     createPopulation = JavaMethod(
-        '(Lorg/spectrumauctions/sats/core/model/World;Lorg/spectrumauctions/sats/core/util/random/RNGSupplier;)Ljava/util/List;')
+        "(Lorg/spectrumauctions/sats/core/model/World;Lorg/spectrumauctions/sats/core/util/random/RNGSupplier;)Ljava/util/List;"
+    )
 
-    def __init__(self, seed, number_of_national_bidders, number_of_regional_bidders, number_of_local_bidders, store_files=False):
-        self.number_of_national_bidders = number_of_national_bidders
-        self.number_of_regional_bidders = number_of_regional_bidders
-        self.number_of_local_bidders = number_of_local_bidders
+    def __init__(
+        self,
+        seed,
+        number_of_small_bidders,
+        number_of_high_frequency_bidders,
+        number_of_secondary_bidders,
+        number_of_primary_bidders,
+        store_files=False,
+    ):
+        self.number_of_small_bidders = number_of_small_bidders
+        self.number_of_high_frequency_bidders = number_of_high_frequency_bidders
+        self.number_of_secondary_bidders = number_of_secondary_bidders
+        self.number_of_primary_bidders = number_of_primary_bidders
         super().__init__(
             seed=seed,
-            mip_path='org.spectrumauctions.sats.opt.model.mrvm.MRVM_MIP',
-            generic_definition_path='org.spectrumauctions.sats.core.model.mrvm.MRVMGenericDefinition',
-            store_files=store_files
+            mip_path="org.spectrumauctions.sats.opt.model.srvm.SRVM_MIP",
+            generic_definition_path="org.spectrumauctions.sats.core.model.srvm.SRVMBand",
+            store_files=store_files,
         )
 
     def prepare_world(self):
-        self.setNumberOfNationalBidders(self.number_of_national_bidders)
-        self.setNumberOfRegionalBidders(self.number_of_regional_bidders)
-        self.setNumberOfLocalBidders(self.number_of_local_bidders)
+        self.setNumberOfSmallBidders(self.number_of_small_bidders)
+        self.setNumberOfHighFrequencyBidders(self.number_of_high_frequency_bidders)
+        self.setNumberOfSecondaryBidders(self.number_of_secondary_bidders)
+        self.setNumberOfPrimaryBidders(self.number_of_primary_bidders)
 
     def get_model_name(self):
-        return ('MRVM')
+        return "SRVM"
```

### Comparing `pysats-0.2.1/pysats/simple_model.py` & `pysats-0.2.2/pysats/simple_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,62 @@
-from jnius import JavaClass, MetaJavaClass, JavaMethod, JavaMultipleMethod, cast, autoclass
+from jnius import (
+    JavaClass,
+    MetaJavaClass,
+    JavaMethod,
+    JavaMultipleMethod,
+    cast,
+    autoclass,
+)
 
 SizeBasedUniqueRandomXOR = autoclass(
-    'org.spectrumauctions.sats.core.bidlang.xor.SizeBasedUniqueRandomXOR')
+    "org.spectrumauctions.sats.core.bidlang.xor.SizeBasedUniqueRandomXOR"
+)
 JavaUtilRNGSupplier = autoclass(
-    'org.spectrumauctions.sats.core.util.random.JavaUtilRNGSupplier')
-Random = autoclass('java.util.Random')
-HashSet = autoclass('java.util.HashSet')
-LinkedList = autoclass('java.util.LinkedList')
-Bundle = autoclass(
-    'org.marketdesignresearch.mechlib.core.Bundle')
-BundleEntry = autoclass(
-    'org.marketdesignresearch.mechlib.core.BundleEntry')
+    "org.spectrumauctions.sats.core.util.random.JavaUtilRNGSupplier"
+)
+Random = autoclass("java.util.Random")
+HashSet = autoclass("java.util.HashSet")
+LinkedList = autoclass("java.util.LinkedList")
+Bundle = autoclass("org.marketdesignresearch.mechlib.core.Bundle")
+BundleEntry = autoclass("org.marketdesignresearch.mechlib.core.BundleEntry")
 InstanceHandler = autoclass(
-    'org.spectrumauctions.sats.core.util.instancehandling.InstanceHandler')
+    "org.spectrumauctions.sats.core.util.instancehandling.InstanceHandler"
+)
 InMemoryInstanceHandler = autoclass(
-    'org.spectrumauctions.sats.core.util.instancehandling.InMemoryInstanceHandler')
+    "org.spectrumauctions.sats.core.util.instancehandling.InMemoryInstanceHandler"
+)
 JSONInstanceHandler = autoclass(
-    'org.spectrumauctions.sats.core.util.instancehandling.JSONInstanceHandler')
-LinkedHashMap = autoclass('java.util.LinkedHashMap')
-Price = autoclass('org.marketdesignresearch.mechlib.core.price.Price')
-LinearPrices = autoclass('org.marketdesignresearch.mechlib.core.price.LinearPrices')
+    "org.spectrumauctions.sats.core.util.instancehandling.JSONInstanceHandler"
+)
+LinkedHashMap = autoclass("java.util.LinkedHashMap")
+Price = autoclass("org.marketdesignresearch.mechlib.core.price.Price")
+LinearPrices = autoclass("org.marketdesignresearch.mechlib.core.price.LinearPrices")
 
-class SimpleModel(JavaClass):
 
-    def __init__(self, seed, mip_path: str, store_files = False):
+class SimpleModel(JavaClass):
+    def __init__(self, seed, mip_path: str, store_files=False):
         super().__init__()
         if seed:
             rng = JavaUtilRNGSupplier(seed)
         else:
             rng = JavaUtilRNGSupplier()
 
         self.population = {}
         self.goods = {}
         self.mip_path = mip_path
         self.efficient_allocation = None
         # The following sets the instance handler to InMemory (i.e., no files are stored), if store_files is false
         # Note that since InstanceHandler is a singleton, if you're running experiments in parallel, it may lead
         # to troubles to have this flag set to True in one experiment and False in another one. This is best used
         # in a consistent way, which is probably the idea anyway in most cases.
-        InstanceHandler.setDefaultHandler(JSONInstanceHandler.getInstance() if store_files else InMemoryInstanceHandler.getInstance())
+        InstanceHandler.setDefaultHandler(
+            JSONInstanceHandler.getInstance()
+            if store_files
+            else InMemoryInstanceHandler.getInstance()
+        )
         self.prepare_world()
         world = self.createWorld(rng)
         self._bidder_list = self.createPopulation(world, rng)
 
         # Store bidders
         bidderator = self._bidder_list.iterator()
         count = 0
@@ -55,18 +69,18 @@
         goods_iterator = world.getLicenses().iterator()
         count = 0
         while goods_iterator.hasNext():
             good = goods_iterator.next()
             assert good.getLongId() == count
             count += 1
             self.goods[good.getLongId()] = good
-        
+
         # Python maintains insertion order since 3.7, so it's fine to fill these dictionaries this way
         # -> https://stackoverflow.com/a/40007169
-    
+
     def prepare_world(self):
         """
         Here, child classes will set the parameters for the world creation, e.g. the
         number of bidders
         """
         raise NotImplementedError("Child class has to implement this method")
 
@@ -87,24 +101,28 @@
     def calculate_values(self, bidder_id, goods_vector_2D):
         bidder = self.population[bidder_id]
         bundles = LinkedList()
         for goods_vector in goods_vector_2D:
             bundle = self._vector_to_bundle(goods_vector)
             bundles.add(bundle)
         return [x.doubleValue() for x in bidder.calculateValues(bundles)]
-    
-    def get_best_bundles(self, bidder_id, price_vector, max_number_of_bundles):
+
+    def get_best_bundles(
+        self, bidder_id, price_vector, max_number_of_bundles, allow_negative=False
+    ):
         assert len(price_vector) == len(self.goods.keys())
         bidder = self.population[bidder_id]
         prices_map = LinkedHashMap()
         index = 0
         for good in self.goods.values():
             prices_map.put(good, Price.of(price_vector[index]))
             index += 1
-        bundles = bidder.getBestBundles(LinearPrices(prices_map), max_number_of_bundles)
+        bundles = bidder.getBestBundles(
+            LinearPrices(prices_map), max_number_of_bundles, allow_negative
+        )
         result = []
         for bundle in bundles:
             assert bundle.areSingleQuantityGoods()
             bundle_vector = []
             for i in range(len(price_vector)):
                 if bundle.contains(self.goods[i]):
                     bundle_vector.append(1)
@@ -123,80 +141,103 @@
             if bidder.getValue(bundle, True).doubleValue() > 0:
                 goods_of_interest.append(good_id)
         return goods_of_interest
 
     def get_uniform_random_bids(self, bidder_id, number_of_bids, seed=None):
         bidder = self.population[bidder_id]
         goods = LinkedList()
-        for good in self.goods.values(): goods.add(good)
+        for good in self.goods.values():
+            goods.add(good)
         if seed:
             random = Random(seed)
         else:
             random = Random()
 
         bids = []
         for i in range(number_of_bids):
             bid = []
             bundle = bidder.getAllocationLimit().getUniformRandomBundle(random, goods)
             for good_id, good in self.goods.items():
-                if (bundle.contains(good)):
+                if bundle.contains(good):
                     bid.append(1)
                 else:
                     bid.append(0)
             bid.append(bidder.getValue(bundle).doubleValue())
             bids.append(bid)
         return bids
 
-    def get_random_bids(self, bidder_id, number_of_bids, seed=None, mean_bundle_size=9, standard_deviation_bundle_size=4.5):
+    def get_random_bids(
+        self,
+        bidder_id,
+        number_of_bids,
+        seed=None,
+        mean_bundle_size=9,
+        standard_deviation_bundle_size=4.5,
+    ):
         bidder = self.population[bidder_id]
         if seed:
             rng = JavaUtilRNGSupplier(seed)
         else:
             rng = JavaUtilRNGSupplier()
-        valueFunction = cast('org.spectrumauctions.sats.core.bidlang.xor.SizeBasedUniqueRandomXOR',
-                                bidder.getValueFunction(SizeBasedUniqueRandomXOR, rng))
-        valueFunction.setDistribution(
-            mean_bundle_size, standard_deviation_bundle_size)
+        valueFunction = cast(
+            "org.spectrumauctions.sats.core.bidlang.xor.SizeBasedUniqueRandomXOR",
+            bidder.getValueFunction(SizeBasedUniqueRandomXOR, rng),
+        )
+        valueFunction.setDistribution(mean_bundle_size, standard_deviation_bundle_size)
         valueFunction.setIterations(number_of_bids)
         xorBidIterator = valueFunction.iterator()
         bids = []
-        while (xorBidIterator.hasNext()):
+        while xorBidIterator.hasNext():
             bundleValue = xorBidIterator.next()
             bid = []
             for good_id, good in self.goods.items():
-                if (bundleValue.getBundle().contains(good)):
+                if bundleValue.getBundle().contains(good):
                     bid.append(1)
                 else:
                     bid.append(0)
             bid.append(bundleValue.getAmount().doubleValue())
             bids.append(bid)
         return bids
 
     def get_efficient_allocation(self, display_output=False):
         if self.efficient_allocation:
-            return self.efficient_allocation, sum([self.efficient_allocation[bidder_id]['value'] for bidder_id in self.efficient_allocation.keys()])
+            return self.efficient_allocation, sum(
+                [
+                    self.efficient_allocation[bidder_id]["value"]
+                    for bidder_id in self.efficient_allocation.keys()
+                ]
+            )
 
         mip = autoclass(self.mip_path)(self._bidder_list)
         mip.setDisplayOutput(display_output)
 
         allocation = mip.calculateAllocation()
 
         self.efficient_allocation = {}
 
         for bidder_id, bidder in self.population.items():
             self.efficient_allocation[bidder_id] = {}
-            self.efficient_allocation[bidder_id]['good_ids'] = []
+            self.efficient_allocation[bidder_id]["good_ids"] = []
             bidder_allocation = allocation.allocationOf(bidder)
-            good_iterator = bidder_allocation.getBundle().getSingleQuantityGoods().iterator()
+            good_iterator = (
+                bidder_allocation.getBundle().getSingleQuantityGoods().iterator()
+            )
             while good_iterator.hasNext():
-                self.efficient_allocation[bidder_id]['good_ids'].append(good_iterator.next().getLongId())
-
-            self.efficient_allocation[bidder_id]['value'] = bidder_allocation.getValue().doubleValue()
-
-        return self.efficient_allocation, allocation.getTotalAllocationValue().doubleValue()
+                self.efficient_allocation[bidder_id]["good_ids"].append(
+                    good_iterator.next().getLongId()
+                )
+
+            self.efficient_allocation[bidder_id][
+                "value"
+            ] = bidder_allocation.getValue().doubleValue()
+
+        return (
+            self.efficient_allocation,
+            allocation.getTotalAllocationValue().doubleValue(),
+        )
 
     def _vector_to_bundle(self, vector):
         assert len(vector) == len(self.goods.keys())
         bundleEntries = HashSet()
         for i in range(len(vector)):
             if vector[i] == 1:
                 bundleEntries.add(BundleEntry(self.goods[i], 1))
```

### Comparing `pysats-0.2.1/pysats/srvm.py` & `pysats-0.2.2/pysats/mrvm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 from jnius import MetaJavaClass, JavaMethod
 from .generic_model import GenericModel
 
-class _Srvm(GenericModel, metaclass=MetaJavaClass):
+
+class _Mrvm(GenericModel, metaclass=MetaJavaClass):
     # We have to define the java class and any method we're going to use in this child class
-    __javaclass__ = 'org/spectrumauctions/sats/core/model/srvm/SingleRegionModel'
-    setNumberOfSmallBidders = JavaMethod('(I)V')
-    setNumberOfHighFrequencyBidders = JavaMethod('(I)V')
-    setNumberOfSecondaryBidders = JavaMethod('(I)V')
-    setNumberOfPrimaryBidders = JavaMethod('(I)V')
+    __javaclass__ = "org/spectrumauctions/sats/core/model/mrvm/MultiRegionModel"
+    setNumberOfNationalBidders = JavaMethod("(I)V")
+    setNumberOfRegionalBidders = JavaMethod("(I)V")
+    setNumberOfLocalBidders = JavaMethod("(I)V")
     createWorld = JavaMethod(
-        '(Lorg/spectrumauctions/sats/core/util/random/RNGSupplier;)Lorg/spectrumauctions/sats/core/model/srvm/SRVMWorld;')
+        "(Lorg/spectrumauctions/sats/core/util/random/RNGSupplier;)Lorg/spectrumauctions/sats/core/model/World;"
+    )
     createPopulation = JavaMethod(
-        '(Lorg/spectrumauctions/sats/core/model/World;Lorg/spectrumauctions/sats/core/util/random/RNGSupplier;)Ljava/util/List;')
-
+        "(Lorg/spectrumauctions/sats/core/model/World;Lorg/spectrumauctions/sats/core/util/random/RNGSupplier;)Ljava/util/List;"
+    )
 
-    def __init__(self, seed, number_of_small_bidders, number_of_high_frequency_bidders, number_of_secondary_bidders, number_of_primary_bidders, store_files=False):
-        self.number_of_small_bidders = number_of_small_bidders
-        self.number_of_high_frequency_bidders = number_of_high_frequency_bidders
-        self.number_of_secondary_bidders = number_of_secondary_bidders
-        self.number_of_primary_bidders = number_of_primary_bidders
+    def __init__(
+        self,
+        seed,
+        number_of_national_bidders,
+        number_of_regional_bidders,
+        number_of_local_bidders,
+        store_files=False,
+    ):
+        self.number_of_national_bidders = number_of_national_bidders
+        self.number_of_regional_bidders = number_of_regional_bidders
+        self.number_of_local_bidders = number_of_local_bidders
         super().__init__(
             seed=seed,
-            mip_path='org.spectrumauctions.sats.opt.model.srvm.SRVM_MIP',
-            generic_definition_path='org.spectrumauctions.sats.core.model.srvm.SRVMBand',
-            store_files=store_files
+            mip_path="org.spectrumauctions.sats.opt.model.mrvm.MRVM_MIP",
+            generic_definition_path="org.spectrumauctions.sats.core.model.mrvm.MRVMGenericDefinition",
+            store_files=store_files,
         )
 
     def prepare_world(self):
-        self.setNumberOfSmallBidders(self.number_of_small_bidders)
-        self.setNumberOfHighFrequencyBidders(self.number_of_high_frequency_bidders)
-        self.setNumberOfSecondaryBidders(self.number_of_secondary_bidders)
-        self.setNumberOfPrimaryBidders(self.number_of_primary_bidders)
+        self.setNumberOfNationalBidders(self.number_of_national_bidders)
+        self.setNumberOfRegionalBidders(self.number_of_regional_bidders)
+        self.setNumberOfLocalBidders(self.number_of_local_bidders)
 
     def get_model_name(self):
-        return ('SRVM')
+        return "MRVM"
```

### Comparing `pysats-0.2.1/setup.py` & `pysats-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['Cython>=0.29.23,<0.30.0', 'numpy>=1.24.1,<2.0.0', 'pyjnius>=1.3.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'pysats',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'GNU Affero General Public License v3',
     'long_description': "# PySATS\n\nThis is a bridge to use some features of [SATS](https://spectrumauctions.org/) in a Python project.\n\n## Requirements\n\n- Python: 3.8+ (required for guaranteeing insertion order in dicts)\n- Pyjnius 1.3.0\n\n## Set up\n\n1. Create a Python environment that satisfied above requirements. To install Pyjnius, follow the steps in <https://pyjnius.readthedocs.io/en/stable/installation.html>#.\n2. Download the latest SATS JAR from <https://github.com/spectrumauctions/sats/releases/>\n3. Place the SATS JAR together with the cplex.jar (which can be found in the CPLEX installation's `bin` folder) together in some directory on your machine, and set the PYJNIUS_CLASSPATH environment variable to the absolute path of this directory.\n\n## Usage\n\nAfter having set up the environment according the the previous section, install the package\n\n```bash\n$ pip install pysats\n...\n```\n\nUse it in your project as follows. Have a look at the `test/` directory for more examples.\n\n```python\nfrom pysats import PySats\n\ngsvm = PySats.getInstance().create_gsvm()\nfor bidder_id in gsvm.get_bidder_ids():\n    goods_of_interest = gsvm.get_goods_of_interest(bidder_id)\n    print(f'Bidder_{bidder_id}: {goods_of_interest}')\n```\n\n## Verify installation\n\nThe best way to verify installation, and check if everything is wired up correctly, is to check out the project and to run the tests:\n\n```bash\n$ python -m unittest\n...\n```\n\n### Alternative to set up locally: Poetry\n\nYou can use Poetry to set up and test pysats locally. Install it as described in <https://python-poetry.org/docs/#installation>, and then run:\n\n```bash\n$ poetry install\n...\n```\n\nThis will install all dependencies automatically. To test the setup, run:\n\n```bash\n$ poetry run python -m unittest\n...\n```\n",
     'author': 'Fabio Isler',
     'author_email': 'islerfab@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/marketdesignresearch/pysats',
```

### Comparing `pysats-0.2.1/PKG-INFO` & `pysats-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysats
-Version: 0.2.1
+Version: 0.2.2
 Summary: GNU Affero General Public License v3
 Home-page: https://github.com/marketdesignresearch/pysats
 License: GNU Affero General Public License v3
 Author: Fabio Isler
 Author-email: islerfab@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

