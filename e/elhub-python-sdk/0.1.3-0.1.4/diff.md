# Comparing `tmp/elhub_python_sdk-0.1.3.tar.gz` & `tmp/elhub_python_sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elhub_python_sdk-0.1.3.tar", max compression
+gzip compressed data, was "elhub_python_sdk-0.1.4.tar", max compression
```

## Comparing `elhub_python_sdk-0.1.3.tar` & `elhub_python_sdk-0.1.4.tar`

### file list

```diff
@@ -1,106 +1,105 @@
--rw-r--r--   0        0        0    35149 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/LICENSE
--rw-r--r--   0        0        0     1282 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/README.md
--rw-r--r--   0        0        0      130 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/__init__.py
--rw-r--r--   0        0        0     3684 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/client.py
--rw-r--r--   0        0        0       92 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/constants.py
--rw-r--r--   0        0        0     5807 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/consumption.py
--rw-r--r--   0        0        0     3285 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/enrollment.py
--rw-r--r--   0        0        0     1493 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/enums.py
--rw-r--r--   0        0        0     1522 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/settings.py
--rw-r--r--   0        0        0     3791 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/third_party.py
--rw-r--r--   0        0        0     1033 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/Acknowledgement.xsd
--rw-r--r--   0        0        0      996 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/PollForData.xsd
--rw-r--r--   0        0        0    43445 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/common/Elhub_AggregatedBusinessInformationEntities.xsd
--rw-r--r--   0        0        0    42145 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/common/Elhub_BusinessDataType.xsd
--rw-r--r--   0        0        0     1072 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/market/ConfirmEndOfSupply.xsd
--rw-r--r--   0        0        0     1084 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/market/ConfirmStartOfSupply.xsd
--rw-r--r--   0        0        0     1065 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/market/NotifyEndOfSupply.xsd
--rw-r--r--   0        0        0     1077 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/market/NotifyStartOfSupply.xsd
--rw-r--r--   0        0        0     1068 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/market/RejectEndOfSupply.xsd
--rw-r--r--   0        0        0     1078 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/market/RejectStartOfSupply.xsd
--rw-r--r--   0        0        0     1066 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/market/RequestEndOfSupply.xsd
--rw-r--r--   0        0        0     1078 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/market/RequestStartOfSupply.xsd
--rw-r--r--   0        0        0     1126 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/masterdata/NotifyCustomerInformation.xsd
--rw-r--r--   0        0        0     1188 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/masterdata/NotifyMeteringPointCharacteristics.xsd
--rw-r--r--   0        0        0     1168 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/masterdata/RequestUpdateCustomerInformation.xsd
--rw-r--r--   0        0        0     1393 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/masterdata/RequestUpdateMasterDataMeteringPoint.xsd
--rw-r--r--   0        0        0     1415 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/metering/CollectedData.xsd
--rw-r--r--   0        0        0     1184 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/metering/NotifyValidatedDataForBillingEnergy.xsd
--rw-r--r--   0        0        0     1207 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/metering/PriceVolumeCombinationForReconciliation.xsd
--rw-r--r--   0        0        0     1094 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/metering/RequestCollectedData.xsd
--rw-r--r--   0        0        0     1076 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/query/RequestDataFromElhub.xsd
--rw-r--r--   0        0        0     1040 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/query/RequestToElhub.xsd
--rw-r--r--   0        0        0     1118 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/query/RequestToGridAccessProvider.xsd
--rw-r--r--   0        0        0     1208 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/query/RequestUpfrontMeteringPointCharacteristics.xsd
--rw-r--r--   0        0        0     1064 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseFromElhub.xsd
--rw-r--r--   0        0        0     1142 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseFromGridAccessProvider.xsd
--rw-r--r--   0        0        0     1225 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseUpfrontMeteringPointCharacteristics.xsd
--rw-r--r--   0        0        0     1110 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/thirdpartyaccess/UpdateThirdPartyAccess.xsd
--rw-r--r--   0        0        0    43165 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim v22 sorted/Elhub_AggregatedBusinessInformationEntities_v22_sorted.xsd
--rw-r--r--   0        0        0        0 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim v22 sorted/Elhub_BusinessDataType_v22_sorted.xsd
--rw-r--r--   0        0        0   126666 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bindings/jaxb_numeric.xml
--rw-r--r--   0        0        0    12376 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/MarketProcesses - WS-Security.wsdl
--rw-r--r--   0        0        0     6742 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/MeteringValues - WS-Security.wsdl
--rw-r--r--   0        0        0     6972 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/PollMarketProcesses - WS-Security.wsdl
--rw-r--r--   0        0        0     6961 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/PollMeteringValues - WS-Security.wsdl
--rw-r--r--   0        0        0    11193 2023-01-30 12:53:05.978082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/Query - WS-Security.wsdl
--rw-r--r--   0        0        0     3056 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/MarketProcesses.xsd
--rw-r--r--   0        0        0     1159 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/MeteringValues.xsd
--rw-r--r--   0        0        0     6206 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/PollMarketProcesses.xsd
--rw-r--r--   0        0        0     3176 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/PollMeteringValues.xsd
--rw-r--r--   0        0        0     3263 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/Query.xsd
--rw-r--r--   0        0        0     1613 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/common.xsd
--rw-r--r--   0        0        0     1033 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/Acknowledgement.xsd
--rw-r--r--   0        0        0      996 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/PollForData.xsd
--rw-r--r--   0        0        0    43445 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/common/Elhub_AggregatedBusinessInformationEntities.xsd
--rw-r--r--   0        0        0    42145 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/common/Elhub_BusinessDataType.xsd
--rw-r--r--   0        0        0     1072 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/market/ConfirmEndOfSupply.xsd
--rw-r--r--   0        0        0     1084 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/market/ConfirmStartOfSupply.xsd
--rw-r--r--   0        0        0     1065 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/market/NotifyEndOfSupply.xsd
--rw-r--r--   0        0        0     1077 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/market/NotifyStartOfSupply.xsd
--rw-r--r--   0        0        0     1068 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/market/RejectEndOfSupply.xsd
--rw-r--r--   0        0        0     1078 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/market/RejectStartOfSupply.xsd
--rw-r--r--   0        0        0     1066 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/market/RequestEndOfSupply.xsd
--rw-r--r--   0        0        0     1078 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/market/RequestStartOfSupply.xsd
--rw-r--r--   0        0        0     1126 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/masterdata/NotifyCustomerInformation.xsd
--rw-r--r--   0        0        0     1188 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/masterdata/NotifyMeteringPointCharacteristics.xsd
--rw-r--r--   0        0        0     1168 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/masterdata/RequestUpdateCustomerInformation.xsd
--rw-r--r--   0        0        0     1393 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/masterdata/RequestUpdateMasterDataMeteringPoint.xsd
--rw-r--r--   0        0        0     1415 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/metering/CollectedData.xsd
--rw-r--r--   0        0        0     1184 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/metering/NotifyValidatedDataForBillingEnergy.xsd
--rw-r--r--   0        0        0     1207 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/metering/PriceVolumeCombinationForReconciliation.xsd
--rw-r--r--   0        0        0     1094 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/metering/RequestCollectedData.xsd
--rw-r--r--   0        0        0     1076 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/query/RequestDataFromElhub.xsd
--rw-r--r--   0        0        0     1040 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/query/RequestToElhub.xsd
--rw-r--r--   0        0        0     1118 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/query/RequestToGridAccessProvider.xsd
--rw-r--r--   0        0        0     1208 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/query/RequestUpfrontMeteringPointCharacteristics.xsd
--rw-r--r--   0        0        0     1064 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/query/ResponseFromElhub.xsd
--rw-r--r--   0        0        0     1142 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/query/ResponseFromGridAccessProvider.xsd
--rw-r--r--   0        0        0     1225 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/query/ResponseUpfrontMeteringPointCharacteristics.xsd
--rw-r--r--   0        0        0     1110 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/thirdpartyaccess/UpdateThirdPartyAccess.xsd
--rw-r--r--   0        0        0    43165 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim v22 sorted/Elhub_AggregatedBusinessInformationEntities_v22_sorted.xsd
--rw-r--r--   0        0        0        0 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim v22 sorted/Elhub_BusinessDataType_v22_sorted.xsd
--rw-r--r--   0        0        0   126666 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bindings/jaxb_numeric.xml
--rw-r--r--   0        0        0    12375 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/MarketProcesses - WS-Security.wsdl
--rw-r--r--   0        0        0     6741 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/MeteringValues - WS-Security.wsdl
--rw-r--r--   0        0        0     6971 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/PollMarketProcesses - WS-Security.wsdl
--rw-r--r--   0        0        0     6960 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/PollMeteringValues - WS-Security.wsdl
--rw-r--r--   0        0        0    11192 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/Query - WS-Security.wsdl
--rw-r--r--   0        0        0     3056 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/xsd/MarketProcesses.xsd
--rw-r--r--   0        0        0     1159 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/xsd/MeteringValues.xsd
--rw-r--r--   0        0        0     6206 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/xsd/PollMarketProcesses.xsd
--rw-r--r--   0        0        0     3176 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/xsd/PollMeteringValues.xsd
--rw-r--r--   0        0        0     3263 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/xsd/Query.xsd
--rw-r--r--   0        0        0     1613 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/xsd/common.xsd
--rw-r--r--   0        0        0     2506 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       46 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     2630 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/tests/test_integration.py
--rw-r--r--   0        0        0     3914 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/tests/test_integration_soap.py
--rw-r--r--   0        0        0      283 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/tests/tests_examples/README.md
--rw-r--r--   0        0        0        0 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/tests/tests_examples/__init__.py
--rw-r--r--   0        0        0      932 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/tests/tests_examples/ag611-01-actor-test.py
--rw-r--r--   0        0        0     1987 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/tests/tests_examples/ag622-01-actor-test.py
--rw-r--r--   0        0        0     1966 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/tests/tests_examples/ag622-02-actor-test.py
--rw-r--r--   0        0        0      401 2023-01-30 12:53:05.982082 elhub_python_sdk-0.1.3/tests/tests_examples/config.py
--rw-r--r--   0        0        0     4114 1970-01-01 00:00:00.000000 elhub_python_sdk-0.1.3/setup.py
--rw-r--r--   0        0        0     3572 1970-01-01 00:00:00.000000 elhub_python_sdk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-04-27 10:56:54.310448 elhub_python_sdk-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1283 2023-04-27 10:56:54.310448 elhub_python_sdk-0.1.4/README.md
+-rw-r--r--   0        0        0      130 2023-04-27 10:56:54.310448 elhub_python_sdk-0.1.4/elhub_sdk/__init__.py
+-rw-r--r--   0        0        0     3684 2023-04-27 10:56:54.310448 elhub_python_sdk-0.1.4/elhub_sdk/client.py
+-rw-r--r--   0        0        0       92 2023-04-27 10:56:54.310448 elhub_python_sdk-0.1.4/elhub_sdk/constants.py
+-rw-r--r--   0        0        0     5777 2023-04-27 10:56:54.310448 elhub_python_sdk-0.1.4/elhub_sdk/consumption.py
+-rw-r--r--   0        0        0     3269 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/enrollment.py
+-rw-r--r--   0        0        0     1453 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/enums.py
+-rw-r--r--   0        0        0     1522 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/settings.py
+-rw-r--r--   0        0        0     3783 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/third_party.py
+-rw-r--r--   0        0        0     1033 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/Acknowledgement.xsd
+-rw-r--r--   0        0        0      996 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/PollForData.xsd
+-rw-r--r--   0        0        0    43445 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/common/Elhub_AggregatedBusinessInformationEntities.xsd
+-rw-r--r--   0        0        0    42145 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/common/Elhub_BusinessDataType.xsd
+-rw-r--r--   0        0        0     1072 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/ConfirmEndOfSupply.xsd
+-rw-r--r--   0        0        0     1084 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/ConfirmStartOfSupply.xsd
+-rw-r--r--   0        0        0     1065 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/NotifyEndOfSupply.xsd
+-rw-r--r--   0        0        0     1077 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/NotifyStartOfSupply.xsd
+-rw-r--r--   0        0        0     1068 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/RejectEndOfSupply.xsd
+-rw-r--r--   0        0        0     1078 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/RejectStartOfSupply.xsd
+-rw-r--r--   0        0        0     1066 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/RequestEndOfSupply.xsd
+-rw-r--r--   0        0        0     1078 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/RequestStartOfSupply.xsd
+-rw-r--r--   0        0        0     1126 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/masterdata/NotifyCustomerInformation.xsd
+-rw-r--r--   0        0        0     1188 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/masterdata/NotifyMeteringPointCharacteristics.xsd
+-rw-r--r--   0        0        0     1168 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/masterdata/RequestUpdateCustomerInformation.xsd
+-rw-r--r--   0        0        0     1393 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/masterdata/RequestUpdateMasterDataMeteringPoint.xsd
+-rw-r--r--   0        0        0     1415 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/metering/CollectedData.xsd
+-rw-r--r--   0        0        0     1184 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/metering/NotifyValidatedDataForBillingEnergy.xsd
+-rw-r--r--   0        0        0     1207 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/metering/PriceVolumeCombinationForReconciliation.xsd
+-rw-r--r--   0        0        0     1094 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/metering/RequestCollectedData.xsd
+-rw-r--r--   0        0        0     1076 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/RequestDataFromElhub.xsd
+-rw-r--r--   0        0        0     1040 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/RequestToElhub.xsd
+-rw-r--r--   0        0        0     1118 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/RequestToGridAccessProvider.xsd
+-rw-r--r--   0        0        0     1208 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/RequestUpfrontMeteringPointCharacteristics.xsd
+-rw-r--r--   0        0        0     1064 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseFromElhub.xsd
+-rw-r--r--   0        0        0     1142 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseFromGridAccessProvider.xsd
+-rw-r--r--   0        0        0     1225 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseUpfrontMeteringPointCharacteristics.xsd
+-rw-r--r--   0        0        0     1110 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/thirdpartyaccess/UpdateThirdPartyAccess.xsd
+-rw-r--r--   0        0        0    43165 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim v22 sorted/Elhub_AggregatedBusinessInformationEntities_v22_sorted.xsd
+-rw-r--r--   0        0        0        0 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim v22 sorted/Elhub_BusinessDataType_v22_sorted.xsd
+-rw-r--r--   0        0        0   126666 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bindings/jaxb_numeric.xml
+-rw-r--r--   0        0        0    12376 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/MarketProcesses - WS-Security.wsdl
+-rw-r--r--   0        0        0     6742 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/MeteringValues - WS-Security.wsdl
+-rw-r--r--   0        0        0     6972 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/PollMarketProcesses - WS-Security.wsdl
+-rw-r--r--   0        0        0     6961 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/PollMeteringValues - WS-Security.wsdl
+-rw-r--r--   0        0        0    11193 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/Query - WS-Security.wsdl
+-rw-r--r--   0        0        0     3056 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/MarketProcesses.xsd
+-rw-r--r--   0        0        0     1159 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/MeteringValues.xsd
+-rw-r--r--   0        0        0     6206 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/PollMarketProcesses.xsd
+-rw-r--r--   0        0        0     3176 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/PollMeteringValues.xsd
+-rw-r--r--   0        0        0     3263 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/Query.xsd
+-rw-r--r--   0        0        0     1613 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/common.xsd
+-rw-r--r--   0        0        0     1033 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/Acknowledgement.xsd
+-rw-r--r--   0        0        0      996 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/PollForData.xsd
+-rw-r--r--   0        0        0    43445 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/common/Elhub_AggregatedBusinessInformationEntities.xsd
+-rw-r--r--   0        0        0    42145 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/common/Elhub_BusinessDataType.xsd
+-rw-r--r--   0        0        0     1072 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/ConfirmEndOfSupply.xsd
+-rw-r--r--   0        0        0     1084 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/ConfirmStartOfSupply.xsd
+-rw-r--r--   0        0        0     1065 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/NotifyEndOfSupply.xsd
+-rw-r--r--   0        0        0     1077 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/NotifyStartOfSupply.xsd
+-rw-r--r--   0        0        0     1068 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/RejectEndOfSupply.xsd
+-rw-r--r--   0        0        0     1078 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/RejectStartOfSupply.xsd
+-rw-r--r--   0        0        0     1066 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/RequestEndOfSupply.xsd
+-rw-r--r--   0        0        0     1078 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/RequestStartOfSupply.xsd
+-rw-r--r--   0        0        0     1126 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/masterdata/NotifyCustomerInformation.xsd
+-rw-r--r--   0        0        0     1188 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/masterdata/NotifyMeteringPointCharacteristics.xsd
+-rw-r--r--   0        0        0     1168 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/masterdata/RequestUpdateCustomerInformation.xsd
+-rw-r--r--   0        0        0     1393 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/masterdata/RequestUpdateMasterDataMeteringPoint.xsd
+-rw-r--r--   0        0        0     1415 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/metering/CollectedData.xsd
+-rw-r--r--   0        0        0     1184 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/metering/NotifyValidatedDataForBillingEnergy.xsd
+-rw-r--r--   0        0        0     1207 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/metering/PriceVolumeCombinationForReconciliation.xsd
+-rw-r--r--   0        0        0     1094 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/metering/RequestCollectedData.xsd
+-rw-r--r--   0        0        0     1076 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/RequestDataFromElhub.xsd
+-rw-r--r--   0        0        0     1040 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/RequestToElhub.xsd
+-rw-r--r--   0        0        0     1118 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/RequestToGridAccessProvider.xsd
+-rw-r--r--   0        0        0     1208 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/RequestUpfrontMeteringPointCharacteristics.xsd
+-rw-r--r--   0        0        0     1064 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/ResponseFromElhub.xsd
+-rw-r--r--   0        0        0     1142 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/ResponseFromGridAccessProvider.xsd
+-rw-r--r--   0        0        0     1225 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/ResponseUpfrontMeteringPointCharacteristics.xsd
+-rw-r--r--   0        0        0     1110 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/thirdpartyaccess/UpdateThirdPartyAccess.xsd
+-rw-r--r--   0        0        0    43165 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim v22 sorted/Elhub_AggregatedBusinessInformationEntities_v22_sorted.xsd
+-rw-r--r--   0        0        0        0 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim v22 sorted/Elhub_BusinessDataType_v22_sorted.xsd
+-rw-r--r--   0        0        0   126666 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bindings/jaxb_numeric.xml
+-rw-r--r--   0        0        0    12375 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/MarketProcesses - WS-Security.wsdl
+-rw-r--r--   0        0        0     6741 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/MeteringValues - WS-Security.wsdl
+-rw-r--r--   0        0        0     6971 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/PollMarketProcesses - WS-Security.wsdl
+-rw-r--r--   0        0        0     6960 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/PollMeteringValues - WS-Security.wsdl
+-rw-r--r--   0        0        0    11192 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/Query - WS-Security.wsdl
+-rw-r--r--   0        0        0     3056 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/MarketProcesses.xsd
+-rw-r--r--   0        0        0     1159 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/MeteringValues.xsd
+-rw-r--r--   0        0        0     6206 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/PollMarketProcesses.xsd
+-rw-r--r--   0        0        0     3176 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/PollMeteringValues.xsd
+-rw-r--r--   0        0        0     3263 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/Query.xsd
+-rw-r--r--   0        0        0     1613 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/common.xsd
+-rw-r--r--   0        0        0     2506 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     3218 2023-04-27 10:56:54.314448 elhub_python_sdk-0.1.4/tests/test_integration.py
+-rw-r--r--   0        0        0     3914 2023-04-27 10:56:54.318448 elhub_python_sdk-0.1.4/tests/test_integration_soap.py
+-rw-r--r--   0        0        0      283 2023-04-27 10:56:54.318448 elhub_python_sdk-0.1.4/tests/tests_examples/README.md
+-rw-r--r--   0        0        0        0 2023-04-27 10:56:54.318448 elhub_python_sdk-0.1.4/tests/tests_examples/__init__.py
+-rw-r--r--   0        0        0      932 2023-04-27 10:56:54.318448 elhub_python_sdk-0.1.4/tests/tests_examples/ag611-01-actor-test.py
+-rw-r--r--   0        0        0     1987 2023-04-27 10:56:54.318448 elhub_python_sdk-0.1.4/tests/tests_examples/ag622-01-actor-test.py
+-rw-r--r--   0        0        0     1966 2023-04-27 10:56:54.318448 elhub_python_sdk-0.1.4/tests/tests_examples/ag622-02-actor-test.py
+-rw-r--r--   0        0        0      401 2023-04-27 10:56:54.318448 elhub_python_sdk-0.1.4/tests/tests_examples/config.py
+-rw-r--r--   0        0        0     3573 1970-01-01 00:00:00.000000 elhub_python_sdk-0.1.4/PKG-INFO
```

### Comparing `elhub_python_sdk-0.1.3/README.md` & `elhub_python_sdk-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,14 @@
 * GitHub: <https://github.com/bkkas/elhub-python-sdk>
 * GitHub: <https://github.com/bkkas/elhub-python-sdk/discussions>
 * PyPI: <https://pypi.org/project/elhub-python-sdk/>
 
 
 ## License
 
-GPL-3.0
+LGPL-3.0
 
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and
 the [waynerv/cookiecutter-pypackage](https://github.com/waynerv/cookiecutter-pypackage) project template.
```

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/client.py` & `elhub_python_sdk-0.1.4/elhub_sdk/client.py`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/consumption.py` & `elhub_python_sdk-0.1.4/elhub_sdk/consumption.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 import zeep
 from zeep.plugins import HistoryPlugin
 
 from elhub_sdk.constants import ELHUB_GSN, TIME_FORMAT
 from elhub_sdk.enums import (
     BSR_IDS,
-    DOCUMENT_TYPE_EBIX,
     DOCUMENT_TYPE_UN_CEFACT,
     ENERGY_INDUSTRY_CLASSIFICATION,
     LIST_AGENCY_IDENTIFIER,
     QUERY_MARKET,
     ROLES,
     SCHEME_AGENCY_IDENTIFIER,
 )
@@ -56,16 +55,16 @@
     """
 
     factory = client.type_factory('ns4')
     eh_request = factory.RequestDataFromElhub(
         Header={
             'Identification': uuid.uuid4(),
             'DocumentType': {
-                '_value_1': DOCUMENT_TYPE_EBIX.METERING_DATA.value,
-                'listAgencyIdentifier': LIST_AGENCY_IDENTIFIER.EBIX.value,
+                '_value_1': DOCUMENT_TYPE_UN_CEFACT.QUERY.value,
+                'listAgencyIdentifier': LIST_AGENCY_IDENTIFIER.UN_CEFACT.value,
             },
             'Creation': f'{datetime.utcnow().strftime(TIME_FORMAT)}',
             'PhysicalSenderEnergyParty': {
                 'Identification': {
                     '_value_1': sender_gsn,
                     'schemeAgencyIdentifier': SCHEME_AGENCY_IDENTIFIER.GS1.value,
                 }
@@ -76,15 +75,15 @@
                     'schemeAgencyIdentifier': SCHEME_AGENCY_IDENTIFIER.GS1.value,
                 }
             },
             'JuridicalRecipientEnergyParty': {
                 'Identification': {'_value_1': ELHUB_GSN, 'schemeAgencyIdentifier': SCHEME_AGENCY_IDENTIFIER.GS1.value}
             },
         },
-        ProcessEnergyContext={  # https://dok.elhub.no/ediel200utkast/general#General-Process
+        ProcessEnergyContext={  # https://dok.elhub.no/ediel2/general#General-Process
             'EnergyBusinessProcess': {
                 '_value_1': BSR_IDS.METERING_VALUES.value,
                 'listAgencyIdentifier': LIST_AGENCY_IDENTIFIER.ELHUB.value,
             },
             'EnergyBusinessProcessRole': {
                 '_value_1': process_role.value,
                 'listAgencyIdentifier': LIST_AGENCY_IDENTIFIER.UN_CEFACT.value,
```

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/enrollment.py` & `elhub_python_sdk-0.1.4/elhub_sdk/enrollment.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     client: zeep.Client,
     history: zeep.plugins.HistoryPlugin,
     meter_identificator: str,
     sender_gsn: str,
     process_role: ROLES = ROLES.THIRD_PARTY,
 ) -> Optional[str]:
     """
-    https://dok.elhub.no/ediel200utkast/requestupfrontmeteringpointcharacteristics
+    https://dok.elhub.no/ediel2/requestupfrontmeteringpointcharacteristics
     Args:
         client: zeep client
         history: zeep history
         meter_identificator: meter identificator
         sender_gsn: sender gsn
         process_role: process role
 
@@ -56,15 +56,15 @@
                     'schemeAgencyIdentifier': SCHEME_AGENCY_IDENTIFIER.GS1.value,
                 }
             },
             'JuridicalRecipientEnergyParty': {
                 'Identification': {'_value_1': ELHUB_GSN, 'schemeAgencyIdentifier': SCHEME_AGENCY_IDENTIFIER.GS1.value}
             },
         },
-        ProcessEnergyContext={  # https://dok.elhub.no/ediel200utkast/general#General-Process
+        ProcessEnergyContext={  # https://dok.elhub.no/ediel2/general#General-Process
             'EnergyBusinessProcess': {
                 '_value_1': BSR_IDS.METERING_POINT_CHARACTERISTICS.value,
                 'listAgencyIdentifier': LIST_AGENCY_IDENTIFIER.ELHUB.value,
             },
             'EnergyBusinessProcessRole': {
                 '_value_1': process_role.value,
                 'listAgencyIdentifier': LIST_AGENCY_IDENTIFIER.UN_CEFACT.value,
```

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/enums.py` & `elhub_python_sdk-0.1.4/elhub_sdk/enums.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     EBIX = '260'
     UN_CEFACT = '6'
     ELHUB = '89'
 
 
 class DOCUMENT_TYPE_EBIX(Enum):
     """
-    Metering data: https://dok.elhub.no/ediel200utkast/document-type
+    Metering data: https://dok.elhub.no/ediel2/document-type
     """
 
     CHANGE_DATA = "E10"
     METERING_DATA = "E13"
     MASTER_DATA = "E07"
 
 
@@ -41,44 +41,44 @@
 
     GS1 = '9'
 
 
 class BSR_IDS(Enum):
     """
     Query type
-    https://dok.elhub.no/ediel200utkast/elhub-brs-identifications
+    https://dok.elhub.no/ediel2/elhub-brs-identifications
     """
 
     METERING_VALUES = "BRS-NO-315"
     THIRD_PARTY = "BRS-NO-622"
     METERING_POINT_CHARACTERISTICS = "BRS-NO-611"
 
 
 class ROLES(Enum):
     """
     Roles:
-        https://dok.elhub.no/ediel200utkast/roles-and-domains
+        https://dok.elhub.no/ediel2/roles-and-domains
     """
 
     THIRD_PARTY = "AG"
     BALANCE_SUPPLIER = "DDQ"
 
 
 class QUERY_MARKET(Enum):
     """
-    https://dok.elhub.no/ediel200utkast/5-query-from-market-parties
+    https://dok.elhub.no/ediel2/5-query-from-market-parties
     """
 
     METERING_VALUES_TIME_SERIES = "MVTS"
 
 
 class ENERGY_INDUSTRY_CLASSIFICATION(Enum):
     """
     Industry codes
-    https://dok.elhub.no/ediel200utkast/general
+    https://dok.elhub.no/ediel2/general
     """
 
     ELECTRICITY_SUPPLY = "23"
 
 
 class THIRD_PARTY_ACTION(Enum):
     """
```

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/settings.py` & `elhub_python_sdk-0.1.4/elhub_sdk/settings.py`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/third_party.py` & `elhub_python_sdk-0.1.4/elhub_sdk/third_party.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                     'schemeAgencyIdentifier': SCHEME_AGENCY_IDENTIFIER.GS1.value,
                 }
             },
             'JuridicalRecipientEnergyParty': {
                 'Identification': {'_value_1': ELHUB_GSN, 'schemeAgencyIdentifier': SCHEME_AGENCY_IDENTIFIER.GS1.value}
             },
         },
-        ProcessEnergyContext={  # https://dok.elhub.no/ediel200utkast/general#General-Process
+        ProcessEnergyContext={  # https://dok.elhub.no/ediel2/general#General-Process
             'EnergyBusinessProcess': {
                 '_value_1': BSR_IDS.THIRD_PARTY.value,
                 'listAgencyIdentifier': LIST_AGENCY_IDENTIFIER.ELHUB.value,
             },
             'EnergyBusinessProcessRole': {
                 '_value_1': ROLES.THIRD_PARTY.value,
                 'listAgencyIdentifier': LIST_AGENCY_IDENTIFIER.UN_CEFACT.value,
```

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/Acknowledgement.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/Acknowledgement.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/PollForData.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/PollForData.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/common/Elhub_AggregatedBusinessInformationEntities.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/common/Elhub_AggregatedBusinessInformationEntities.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/common/Elhub_BusinessDataType.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/common/Elhub_BusinessDataType.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/market/ConfirmEndOfSupply.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/ConfirmEndOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/market/ConfirmStartOfSupply.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/ConfirmStartOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/market/NotifyEndOfSupply.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/NotifyEndOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/market/NotifyStartOfSupply.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/NotifyStartOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/market/RejectEndOfSupply.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/RejectEndOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/market/RejectStartOfSupply.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/RejectStartOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/market/RequestEndOfSupply.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/RequestEndOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/market/RequestStartOfSupply.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/market/RequestStartOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/masterdata/NotifyCustomerInformation.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/masterdata/NotifyCustomerInformation.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/masterdata/NotifyMeteringPointCharacteristics.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/masterdata/NotifyMeteringPointCharacteristics.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/masterdata/RequestUpdateCustomerInformation.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/masterdata/RequestUpdateCustomerInformation.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/masterdata/RequestUpdateMasterDataMeteringPoint.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/masterdata/RequestUpdateMasterDataMeteringPoint.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/metering/CollectedData.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/metering/CollectedData.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/metering/NotifyValidatedDataForBillingEnergy.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/metering/NotifyValidatedDataForBillingEnergy.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/metering/PriceVolumeCombinationForReconciliation.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/metering/PriceVolumeCombinationForReconciliation.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/metering/RequestCollectedData.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/metering/RequestCollectedData.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/query/RequestDataFromElhub.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/RequestDataFromElhub.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/query/RequestToElhub.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/RequestToElhub.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/query/RequestToGridAccessProvider.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/RequestToGridAccessProvider.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/query/RequestUpfrontMeteringPointCharacteristics.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/RequestUpfrontMeteringPointCharacteristics.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseFromElhub.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseFromElhub.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseFromGridAccessProvider.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseFromGridAccessProvider.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseUpfrontMeteringPointCharacteristics.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/query/ResponseUpfrontMeteringPointCharacteristics.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim/thirdpartyaccess/UpdateThirdPartyAccess.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim/thirdpartyaccess/UpdateThirdPartyAccess.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bim v22 sorted/Elhub_AggregatedBusinessInformationEntities_v22_sorted.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bim v22 sorted/Elhub_AggregatedBusinessInformationEntities_v22_sorted.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/bindings/jaxb_numeric.xml` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/bindings/jaxb_numeric.xml`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/MarketProcesses - WS-Security.wsdl` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/MarketProcesses - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/MeteringValues - WS-Security.wsdl` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/MeteringValues - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/PollMarketProcesses - WS-Security.wsdl` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/PollMarketProcesses - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/PollMeteringValues - WS-Security.wsdl` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/PollMeteringValues - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/Query - WS-Security.wsdl` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/Query - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/MarketProcesses.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/MarketProcesses.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/MeteringValues.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/MeteringValues.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/PollMarketProcesses.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/PollMarketProcesses.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/PollMeteringValues.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/PollMeteringValues.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/Query.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/Query.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/common.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/prod/2.3/wsdl/xsd/common.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/Acknowledgement.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/Acknowledgement.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/PollForData.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/PollForData.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/common/Elhub_AggregatedBusinessInformationEntities.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/common/Elhub_AggregatedBusinessInformationEntities.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/common/Elhub_BusinessDataType.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/common/Elhub_BusinessDataType.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/market/ConfirmEndOfSupply.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/ConfirmEndOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/market/ConfirmStartOfSupply.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/ConfirmStartOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/market/NotifyEndOfSupply.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/NotifyEndOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/market/NotifyStartOfSupply.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/NotifyStartOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/market/RejectEndOfSupply.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/RejectEndOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/market/RejectStartOfSupply.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/RejectStartOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/market/RequestEndOfSupply.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/RequestEndOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/market/RequestStartOfSupply.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/market/RequestStartOfSupply.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/masterdata/NotifyCustomerInformation.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/masterdata/NotifyCustomerInformation.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/masterdata/NotifyMeteringPointCharacteristics.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/masterdata/NotifyMeteringPointCharacteristics.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/masterdata/RequestUpdateCustomerInformation.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/masterdata/RequestUpdateCustomerInformation.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/masterdata/RequestUpdateMasterDataMeteringPoint.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/masterdata/RequestUpdateMasterDataMeteringPoint.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/metering/CollectedData.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/metering/CollectedData.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/metering/NotifyValidatedDataForBillingEnergy.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/metering/NotifyValidatedDataForBillingEnergy.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/metering/PriceVolumeCombinationForReconciliation.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/metering/PriceVolumeCombinationForReconciliation.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/metering/RequestCollectedData.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/metering/RequestCollectedData.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/query/RequestDataFromElhub.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/RequestDataFromElhub.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/query/RequestToElhub.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/RequestToElhub.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/query/RequestToGridAccessProvider.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/RequestToGridAccessProvider.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/query/RequestUpfrontMeteringPointCharacteristics.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/RequestUpfrontMeteringPointCharacteristics.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/query/ResponseFromElhub.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/ResponseFromElhub.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/query/ResponseFromGridAccessProvider.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/ResponseFromGridAccessProvider.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/query/ResponseUpfrontMeteringPointCharacteristics.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/query/ResponseUpfrontMeteringPointCharacteristics.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim/thirdpartyaccess/UpdateThirdPartyAccess.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim/thirdpartyaccess/UpdateThirdPartyAccess.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bim v22 sorted/Elhub_AggregatedBusinessInformationEntities_v22_sorted.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bim v22 sorted/Elhub_AggregatedBusinessInformationEntities_v22_sorted.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/bindings/jaxb_numeric.xml` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/bindings/jaxb_numeric.xml`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/MarketProcesses - WS-Security.wsdl` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/MarketProcesses - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/MeteringValues - WS-Security.wsdl` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/MeteringValues - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/PollMarketProcesses - WS-Security.wsdl` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/PollMarketProcesses - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/PollMeteringValues - WS-Security.wsdl` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/PollMeteringValues - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/Query - WS-Security.wsdl` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/Query - WS-Security.wsdl`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/xsd/MarketProcesses.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/MarketProcesses.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/xsd/MeteringValues.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/MeteringValues.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/xsd/PollMarketProcesses.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/PollMarketProcesses.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/xsd/PollMeteringValues.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/PollMeteringValues.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/xsd/Query.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/Query.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/elhub_sdk/wsdl/test/2.3/wsdl/xsd/common.xsd` & `elhub_python_sdk-0.1.4/elhub_sdk/wsdl/test/2.3/wsdl/xsd/common.xsd`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/pyproject.toml` & `elhub_python_sdk-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "elhub-python-sdk"
-version = "0.1.3"
+version = "0.1.4"
 homepage = "https://github.com/bkkas/elhub-python-sdk"
 description = "Non official Python SDK for ElHub API."
 authors = ["Volte <jesus.condon@eviny.no>"]
 readme = "README.md"
 license =  "GPL-3.0-only"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `elhub_python_sdk-0.1.3/tests/test_integration.py` & `elhub_python_sdk-0.1.4/tests/test_integration.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,43 @@
 import datetime
 import logging
 
 import pytest
 
 from elhub_sdk.client import APIClient, ElHubEnvironment, ElHubService
 from elhub_sdk.consumption import poll_consumption, request_consumption
+from elhub_sdk.enrollment import get_meter_characteristics
 from elhub_sdk.enums import THIRD_PARTY_ACTION
 from elhub_sdk.settings import CERT_FILE, KEY_FILE
 from elhub_sdk.third_party import request_action
 from tests.tests_examples.config import THIRD_PARTY_GSN_EXA
 
 logger = logging.getLogger(__name__)
 
 
 @pytest.mark.integrationtest
+def test_meter_characteristics():
+    """Test meter characteristics"""
+    meter_identificator = "707057500010503271"
+
+    client, history = APIClient.get_client(
+        environment=ElHubEnvironment.TEST,
+        service=ElHubService.QUERY,
+        key_file=KEY_FILE,
+        cert_file=CERT_FILE,
+    )
+
+    response = get_meter_characteristics(
+        client=client, history=history, meter_identificator=meter_identificator, sender_gsn=THIRD_PARTY_GSN_EXA
+    )
+
+    assert response is not None
+
+
+@pytest.mark.integrationtest
 def test_third_party_delete():
     """
     Tests the addition of a third party against Exa2
     Returns:
 
     """
```

### Comparing `elhub_python_sdk-0.1.3/tests/test_integration_soap.py` & `elhub_python_sdk-0.1.4/tests/test_integration_soap.py`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/tests/tests_examples/ag611-01-actor-test.py` & `elhub_python_sdk-0.1.4/tests/tests_examples/ag611-01-actor-test.py`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/tests/tests_examples/ag622-01-actor-test.py` & `elhub_python_sdk-0.1.4/tests/tests_examples/ag622-01-actor-test.py`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/tests/tests_examples/ag622-02-actor-test.py` & `elhub_python_sdk-0.1.4/tests/tests_examples/ag622-02-actor-test.py`

 * *Files identical despite different names*

### Comparing `elhub_python_sdk-0.1.3/PKG-INFO` & `elhub_python_sdk-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elhub-python-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Non official Python SDK for ElHub API.
 Home-page: https://github.com/bkkas/elhub-python-sdk
 License: GPL-3.0-only
 Author: Volte
 Author-email: jesus.condon@eviny.no
 Requires-Python: >=3.8.2,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -68,15 +68,15 @@
 * GitHub: <https://github.com/bkkas/elhub-python-sdk>
 * GitHub: <https://github.com/bkkas/elhub-python-sdk/discussions>
 * PyPI: <https://pypi.org/project/elhub-python-sdk/>
 
 
 ## License
 
-GPL-3.0
+LGPL-3.0
 
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and
 the [waynerv/cookiecutter-pypackage](https://github.com/waynerv/cookiecutter-pypackage) project template.
```

