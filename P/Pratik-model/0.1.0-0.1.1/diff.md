# Comparing `tmp/Pratik_model-0.1.0.tar.gz` & `tmp/Pratik_model-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pratik_model-0.1.0.tar", last modified: Fri Mar 31 12:45:30 2023, max compression
+gzip compressed data, was "Pratik_model-0.1.1.tar", last modified: Thu Apr 27 05:15:55 2023, max compression
```

## Comparing `Pratik_model-0.1.0.tar` & `Pratik_model-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 12:45:30.612257 Pratik_model-0.1.0/
--rw-rw-rw-   0        0        0    35823 2023-03-29 14:19:20.000000 Pratik_model-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3064 2023-03-31 12:45:30.611256 Pratik_model-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-31 12:45:30.580605 Pratik_model-0.1.0/Pratik_model/
--rw-rw-rw-   0        0        0    15056 2023-03-30 04:58:00.000000 Pratik_model-0.1.0/Pratik_model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-31 12:45:30.609260 Pratik_model-0.1.0/Pratik_model.egg-info/
--rw-rw-rw-   0        0        0     3064 2023-03-31 12:45:30.000000 Pratik_model-0.1.0/Pratik_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-03-31 12:45:30.000000 Pratik_model-0.1.0/Pratik_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 12:45:30.000000 Pratik_model-0.1.0/Pratik_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-03-31 12:45:30.000000 Pratik_model-0.1.0/Pratik_model.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-31 12:45:30.000000 Pratik_model-0.1.0/Pratik_model.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2473 2023-03-31 12:45:24.000000 Pratik_model-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-03-31 12:45:30.612257 Pratik_model-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      834 2023-03-31 12:43:41.000000 Pratik_model-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:15:55.253690 Pratik_model-0.1.1/
+-rw-rw-rw-   0        0        0    35823 2023-03-29 14:19:20.000000 Pratik_model-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3064 2023-04-27 05:15:55.252691 Pratik_model-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-27 05:15:55.198588 Pratik_model-0.1.1/Pratik_model/
+-rw-rw-rw-   0        0        0    14916 2023-04-27 05:14:10.000000 Pratik_model-0.1.1/Pratik_model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 05:15:55.251690 Pratik_model-0.1.1/Pratik_model.egg-info/
+-rw-rw-rw-   0        0        0     3064 2023-04-27 05:15:54.000000 Pratik_model-0.1.1/Pratik_model.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-04-27 05:15:54.000000 Pratik_model-0.1.1/Pratik_model.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 05:15:54.000000 Pratik_model-0.1.1/Pratik_model.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-27 05:15:54.000000 Pratik_model-0.1.1/Pratik_model.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-27 05:15:54.000000 Pratik_model-0.1.1/Pratik_model.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2473 2023-03-31 12:45:24.000000 Pratik_model-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-27 05:15:55.253690 Pratik_model-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      823 2023-04-27 05:12:13.000000 Pratik_model-0.1.1/setup.py
```

### Comparing `Pratik_model-0.1.0/LICENSE.txt` & `Pratik_model-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Pratik_model-0.1.0/PKG-INFO` & `Pratik_model-0.1.1/Pratik_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Pratik_model
-Version: 0.1.0
+Name: Pratik-model
+Version: 0.1.1
 Summary: This package directly gives you output performance on 13 different algorithms
 Home-page: 
 Author: pratik
 Author-email: pratikvdatey@gmail.com
 License: MIT
 Project-URL: source_code, https://github.com/pratikdatey/Pratik_model
 Keywords: Pratik_model
```

### Comparing `Pratik_model-0.1.0/Pratik_model/__init__.py` & `Pratik_model-0.1.1/Pratik_model/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from sklearn.model_selection import train_test_split,cross_val_score
 from sklearn.linear_model import LogisticRegression,LinearRegression,PassiveAggressiveClassifier,PassiveAggressiveRegressor,Lasso,RidgeClassifier
 from sklearn.ensemble import ExtraTreesClassifier,RandomForestClassifier,RandomForestRegressor,ExtraTreesRegressor,GradientBoostingRegressor,VotingRegressor,HistGradientBoostingRegressor,HistGradientBoostingClassifier
 from sklearn.tree import DecisionTreeClassifier,DecisionTreeRegressor
 from sklearn.svm import SVC,SVR
 from sklearn.naive_bayes import GaussianNB
 from sklearn.neighbors import KNeighborsClassifier,KNeighborsRegressor
-from lightgbm import LGBMClassifier,LGBMRegressor
 from catboost import CatBoostClassifier,CatBoostRegressor
 from xgboost import XGBClassifier,XGBRegressor
 
 import warnings
 warnings.simplefilter('ignore',) 
 
 
@@ -20,15 +19,14 @@
 exc=ExtraTreesClassifier(random_state=42)
 dc=DecisionTreeClassifier(random_state=42)
 svc=SVC(random_state=42)
 gbc=GaussianNB()
 knn=KNeighborsClassifier()
 pacc=PassiveAggressiveClassifier(random_state=42)
 rc=RidgeClassifier(random_state=42)
-lgbmc=LGBMClassifier(random_state=42)
 hgbc=HistGradientBoostingClassifier(random_state=42,verbose=0)
 xgbc=XGBClassifier(random_state=42,verbosity = 0)
 cbc=CatBoostClassifier(random_state=42,verbose=0)
 
 
 
 
@@ -39,25 +37,24 @@
 ext=ExtraTreesRegressor(random_state=42)
 gbr=GradientBoostingRegressor(random_state=42)
 svr=SVR()
 knnr=KNeighborsRegressor()
 dtr=DecisionTreeRegressor(random_state=42)
 pacr=PassiveAggressiveRegressor(random_state=42,average=3)
 las=Lasso(random_state=42)
-lgbmr=LGBMRegressor(random_state=42)
 hgbr=HistGradientBoostingRegressor(random_state=42)
 xgbr=XGBRegressor(random_state=42,verbosity = 0)
 cbr=CatBoostRegressor(random_state=42,verbose=0)
 
 
 
 
 
-name=[hgbc,pacc,dc,rfc,exc,logreg,rc,lgbmc,knn,svc,cbc,xgbc,gbc]
-name_r=[pacr,hgbr,gbr,dtr,rfr,ext,lgbmr,las,knnr,linereg,cbr,xgbr,svr]
+name=[hgbc,pacc,dc,rfc,exc,logreg,rc,knn,svc,cbc,xgbc,gbc]
+name_r=[pacr,hgbr,gbr,dtr,rfr,ext,las,knnr,linereg,cbr,xgbr,svr]
 
 
 
 class smart_classifier:
     def __init__(self,x,y):
         self.__x=x
         self.__y=y
```

### Comparing `Pratik_model-0.1.0/Pratik_model.egg-info/PKG-INFO` & `Pratik_model-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Pratik-model
-Version: 0.1.0
+Name: Pratik_model
+Version: 0.1.1
 Summary: This package directly gives you output performance on 13 different algorithms
 Home-page: 
 Author: pratik
 Author-email: pratikvdatey@gmail.com
 License: MIT
 Project-URL: source_code, https://github.com/pratikdatey/Pratik_model
 Keywords: Pratik_model
```

### Comparing `Pratik_model-0.1.0/README.md` & `Pratik_model-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `Pratik_model-0.1.0/setup.py` & `Pratik_model-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,21 +6,21 @@
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
   ]
 
 
 setup(
     name='Pratik_model',
-    version='0.1.0',
+    version='0.1.1',
     description='This package directly gives you output performance on 13 different algorithms',
     url='',
     license='MIT',
     author='pratik',
     long_description_content_type = open('README.md').read(),
     classifiers=classifiers,
     author_email='pratikvdatey@gmail.com',
     keywords='Pratik_model',
-    install_requires=['sklearn','lightgbm','catboost','xgboost'],
+    install_requires=['sklearn','catboost','xgboost'],
     project_urls= {'source_code' : "https://github.com/pratikdatey/Pratik_model"
                    }
    
 )
```

