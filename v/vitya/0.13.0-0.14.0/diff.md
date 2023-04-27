# Comparing `tmp/vitya-0.13.0.tar.gz` & `tmp/vitya-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vitya-0.13.0.tar", last modified: Wed Apr 12 12:39:07 2023, max compression
+gzip compressed data, was "dist/vitya-0.14.0.tar", last modified: Thu Apr 27 10:02:51 2023, max compression
```

## Comparing `vitya-0.13.0.tar` & `vitya-0.14.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:39:07.000000 vitya-0.13.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-12 12:39:04.000000 vitya-0.13.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-12 12:39:07.000000 vitya-0.13.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-12 12:39:04.000000 vitya-0.13.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-12 12:39:04.000000 vitya-0.13.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 12:39:07.000000 vitya-0.13.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-12 12:39:04.000000 vitya-0.13.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:39:07.000000 vitya-0.13.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-04-12 12:39:04.000000 vitya-0.13.0/tests/test_vitya.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:39:07.000000 vitya-0.13.0/vitya/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:39:07.000000 vitya-0.13.0/vitya/payment_order/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/payment_order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/payment_order/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    17630 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/payment_order/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/payment_order/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:39:07.000000 vitya-0.13.0/vitya/payment_order/payments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/payment_order/payments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/payment_order/payments/checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12805 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/payment_order/payments/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/payment_order/payments/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/payment_order/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/pydantic_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-04-12 12:39:04.000000 vitya-0.13.0/vitya/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:39:07.000000 vitya-0.13.0/vitya.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-12 12:39:07.000000 vitya-0.13.0/vitya.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-12 12:39:07.000000 vitya-0.13.0/vitya.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:39:07.000000 vitya-0.13.0/vitya.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-12 12:39:07.000000 vitya-0.13.0/vitya.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:02:51.000000 vitya-0.14.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-27 10:02:48.000000 vitya-0.14.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-27 10:02:51.000000 vitya-0.14.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-27 10:02:48.000000 vitya-0.14.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-27 10:02:48.000000 vitya-0.14.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 10:02:51.000000 vitya-0.14.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-27 10:02:48.000000 vitya-0.14.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:02:51.000000 vitya-0.14.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-04-27 10:02:48.000000 vitya-0.14.0/tests/test_vitya.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:02:51.000000 vitya-0.14.0/vitya/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/errors_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:02:51.000000 vitya-0.14.0/vitya/payment_order/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/payment_order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/payment_order/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28380 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/payment_order/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/payment_order/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:02:51.000000 vitya-0.14.0/vitya/payment_order/payments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/payment_order/payments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8970 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/payment_order/payments/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/payment_order/payments/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/payment_order/payments/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/payment_order/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/pydantic_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-04-27 10:02:48.000000 vitya-0.14.0/vitya/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 10:02:51.000000 vitya-0.14.0/vitya.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-27 10:02:51.000000 vitya-0.14.0/vitya.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-27 10:02:51.000000 vitya-0.14.0/vitya.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 10:02:51.000000 vitya-0.14.0/vitya.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 10:02:51.000000 vitya-0.14.0/vitya.egg-info/top_level.txt
```

### Comparing `vitya-0.13.0/LICENSE` & `vitya-0.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vitya-0.13.0/PKG-INFO` & `vitya-0.14.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitya
-Version: 0.13.0
+Version: 0.14.0
 Summary: Validators for different russian banking values
 Home-page: https://github.com/hicebank/vitya
 Author: hicebank.ru
 Author-email: inyutin@hicebank.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vitya-0.13.0/README.md` & `vitya-0.14.0/README.md`

 * *Files identical despite different names*

### Comparing `vitya-0.13.0/setup.py` & `vitya-0.14.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='vitya',
-    version='0.13.0',
+    version='0.14.0',
     author='hicebank.ru',
     author_email='inyutin@hicebank.ru',
     description='Validators for different russian banking values',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/hicebank/vitya',
     packages=setuptools.find_packages(),
```

### Comparing `vitya-0.13.0/tests/test_vitya.py` & `vitya-0.14.0/tests/test_vitya.py`

 * *Files identical despite different names*

### Comparing `vitya-0.13.0/vitya/payment_order/enums.py` & `vitya-0.14.0/vitya/payment_order/enums.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,7 +13,20 @@
     @classmethod
     def budget_types(cls) -> List['PaymentType']:
         return [PaymentType.FNS, PaymentType.CUSTOMS, PaymentType.BUDGET_OTHER]
 
     @property
     def is_budget(self) -> bool:
         return self in self.budget_types()
+
+    _TO_RU = {
+        FNS: 'ФНС',
+        CUSTOMS: 'Таможня',
+        BUDGET_OTHER: 'Иные',
+        IP: 'ИП',
+        FL: 'ФЛ',
+        LE: 'ЮЛ',
+    }
+
+    @property
+    def name_ru(self) -> str:
+        return self._TO_RU[self]
```

### Comparing `vitya-0.13.0/vitya/payment_order/fields.py` & `vitya-0.14.0/vitya/payment_order/fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from decimal import Decimal
 from typing import Any, Callable, Generator, Optional
 
 from vitya.payment_order.validators import (
     validate_account_number,
     validate_amount,
     validate_cbc,
+    validate_customer,
     validate_document_date,
     validate_document_number,
     validate_number,
     validate_operation_kind,
     validate_payee,
     validate_payer,
     validate_payer_status,
@@ -41,20 +42,24 @@
 
 
 class Customer(FieldMixin, str):
     """Общий класс для описания сущности владельца денег"""
 
     @classmethod
     def _validate(cls, value: str) -> str:
-        return validate_payer(value)
+        return validate_customer(value)
 
 
 class Payer(Customer):
     """Плательщик (8)"""
 
+    @classmethod
+    def _validate(cls, value: str) -> str:
+        return validate_payer(value)
+
 
 class Payee(Customer):
     """Наименование получателя (16)"""
 
     @classmethod
     def _validate(cls, value: str) -> str:
         return validate_payee(value)
```

### Comparing `vitya-0.13.0/vitya/payment_order/payments/checkers.py` & `vitya-0.14.0/vitya/payment_order/payments/checkers.py`

 * *Files identical despite different names*

### Comparing `vitya-0.13.0/vitya/payment_order/payments/checks.py` & `vitya-0.14.0/vitya/payment_order/payments/checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     PayerStatusValidationCustoms05NotAllowedError,
     PayerStatusValidationNullNotAllowedError,
     PaymentTypeValueError,
     PurposeCodeValidationFlError,
     PurposeCodeValidationNullError,
     PurposeValidationIPNDSError,
     ReasonValidationFNSOnlyEmptyError,
+    ReasonValidationValueErrorCustoms,
     TaxPeriodValidationBOValueLenError,
     TaxPeriodValidationCustomsEmptyNotAllowed,
     TaxPeriodValidationCustomsValueLenError,
     TaxPeriodValidationFNS01OnlyEmpty,
     TaxPeriodValidationFNS02EmptyNotAllowed,
     TaxPeriodValidationFNSEmptyNotAllowed,
     TaxPeriodValidationFNSValueLenError,
@@ -61,15 +62,16 @@
     DocumentNumber,
     OperationKind,
     PayerStatus,
     Purpose,
     Reason,
     TaxPeriod,
 )
-from vitya.payment_order.payments.helpers import (
+from vitya.payment_order.payments.constants import (
+    CUSTOMS_REASONS,
     DOCUMENT_NUMBERS,
     FNS_PAYEE_ACCOUNT_NUMBER,
 )
 from vitya.pydantic_fields import BIC, INN, KPP, OKTMO
 
 
 def check_account_by_bic(
@@ -304,19 +306,20 @@
     payment_type: PaymentType,
 ) -> Optional[Reason]:
     if not payment_type.is_budget:
         return None
 
     if payment_type in {PaymentType.CUSTOMS, PaymentType.BUDGET_OTHER} and value is None:
         return None
-
     if payment_type == PaymentType.FNS:
         if value is not None:
             raise ReasonValidationFNSOnlyEmptyError
         return None
+    if payment_type == PaymentType.CUSTOMS and value not in CUSTOMS_REASONS:
+        raise ReasonValidationValueErrorCustoms
     return value
 
 
 def check_tax_period(
     value: Optional[TaxPeriod],
     payment_type: PaymentType,
     payer_status: PayerStatus,
@@ -390,15 +393,15 @@
             reason in {'ИЛ', 'ИН', 'ПБ', 'КЭ'}
             and (
                 value is None or len(value) > 15
             )
         ):
             raise DocumentNumberValidationCustomsValueLen15Error
         return value
-    raise PaymentTypeValueError(payment_type=str(payment_type))  # pragma: no cover
+    raise PaymentTypeValueError(payment_type=payment_type)  # pragma: no cover
 
 
 def check_document_date(
     value: Optional[DocumentDate],
     payment_type: PaymentType,
 ) -> Optional[DocumentDate]:
     if not payment_type.is_budget:
```

### Comparing `vitya-0.13.0/vitya/payment_order/payments/helpers.py` & `vitya-0.14.0/vitya/payment_order/payments/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     '17',
     '24',
     '28',
     '30',
     '31'
 }
 
-REASONS = {
+CUSTOMS_REASONS = {
     'ПК',
     'КЭ',
     'УВ',
     'ИЛ',
     'ПБ',
     'ТГ',
     'ТБ',
```

### Comparing `vitya-0.13.0/vitya/payment_order/validators.py` & `vitya-0.14.0/vitya/payment_order/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,27 +25,25 @@
     PayerValidationSizeError,
     PaymentOrderValidationError,
     PurposeCodeValidationTypeError,
     PurposeValidationCharactersError,
     PurposeValidationMaxLenError,
     PurposeValidationTypeError,
     ReasonValidationTypeError,
-    ReasonValidationValueError,
     ReasonValidationValueLenError,
     TaxPeriodValidationTypeError,
     UINValidationControlSumError,
     UINValidationDigitsOnlyError,
     UINValidationLenError,
     UINValidationOnlyZeroError,
     UINValidationTypeError,
 )
-from vitya.payment_order.payments.helpers import (
+from vitya.payment_order.payments.constants import (
     CHARS_FOR_PURPOSE,
     PAYER_STATUSES,
-    REASONS,
     REPLACE_CHARS_FOR_SPACE,
 )
 
 
 def validate_number(
     value: str,
 ) -> str:
@@ -159,15 +157,15 @@
     if mod_11 != int(value[-1]):
         raise UINValidationControlSumError
 
 
 def validate_uin(value: str) -> Optional[str]:
     if not isinstance(value, str):
         raise UINValidationTypeError
-    if value == '':
+    if value in {'', '0'}:
         return None
     if not (len(value) == 4 or len(value) == 20 or len(value) == 25):
         raise UINValidationLenError
     if len(value) == 4 and value == '0000':
         raise UINValidationOnlyZeroError
     validate_uin_control_sum(value)
     return value
@@ -227,16 +225,14 @@
 def validate_reason(value: str) -> Optional[str]:
     if not isinstance(value, str):
         raise ReasonValidationTypeError
     elif value in {'', '0'}:
         return None
     elif len(value) != 2:
         raise ReasonValidationValueLenError
-    elif value not in REASONS:
-        raise ReasonValidationValueError
     return value
 
 
 def validate_tax_period(value: str) -> Optional[str]:
     if not isinstance(value, str):
         raise TaxPeriodValidationTypeError
     elif value in {'', '0'}:
```

### Comparing `vitya-0.13.0/vitya/pydantic_fields.py` & `vitya-0.14.0/vitya/pydantic_fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,16 @@
         raise PydanticValidationError(name=name, reason=str(e))
 
     return value
 
 
 class FieldMixin(ABC):
     def __new__(cls, value: Any) -> 'FieldMixin':
+        if type(value) == cls:
+            return value  # type: ignore
         value = cls._validate(value)
         if value is None:
             raise EmptyError
         return super().__new__(cls, value)  # type: ignore
 
     @classmethod
     @abstractmethod
```

### Comparing `vitya-0.13.0/vitya/validators.py` & `vitya-0.14.0/vitya/validators.py`

 * *Files identical despite different names*

### Comparing `vitya-0.13.0/vitya.egg-info/PKG-INFO` & `vitya-0.14.0/vitya.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitya
-Version: 0.13.0
+Version: 0.14.0
 Summary: Validators for different russian banking values
 Home-page: https://github.com/hicebank/vitya
 Author: hicebank.ru
 Author-email: inyutin@hicebank.ru
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vitya-0.13.0/vitya.egg-info/SOURCES.txt` & `vitya-0.14.0/vitya.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 tests/test_vitya.py
 vitya/__init__.py
 vitya/errors.py
+vitya/errors_base.py
 vitya/py.typed
 vitya/pydantic_fields.py
 vitya/validators.py
 vitya.egg-info/PKG-INFO
 vitya.egg-info/SOURCES.txt
 vitya.egg-info/dependency_links.txt
 vitya.egg-info/top_level.txt
@@ -16,8 +17,8 @@
 vitya/payment_order/enums.py
 vitya/payment_order/errors.py
 vitya/payment_order/fields.py
 vitya/payment_order/validators.py
 vitya/payment_order/payments/__init__.py
 vitya/payment_order/payments/checkers.py
 vitya/payment_order/payments/checks.py
-vitya/payment_order/payments/helpers.py
+vitya/payment_order/payments/constants.py
```

