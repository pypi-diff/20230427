# Comparing `tmp/proxycurl-py-0.0.18.tar.gz` & `tmp/proxycurl-py-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxycurl-py-0.0.18.tar", last modified: Mon Dec 12 07:26:35 2022, max compression
+gzip compressed data, was "proxycurl-py-0.0.19.tar", last modified: Thu Apr 27 05:48:53 2023, max compression
```

## Comparing `proxycurl-py-0.0.18.tar` & `proxycurl-py-0.0.19.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2022-12-12 07:26:35.883373 proxycurl-py-0.0.18/
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    10540 2022-12-12 07:26:35.883373 proxycurl-py-0.0.18/PKG-INFO
--rw-r--r--   0 adiguna7  (1000) adiguna7  (1000)    10245 2022-12-12 06:49:30.000000 proxycurl-py-0.0.18/README.md
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2022-12-12 07:26:35.879373 proxycurl-py-0.0.18/proxycurl_py/
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)        0 2022-12-08 23:13:26.000000 proxycurl-py-0.0.18/proxycurl_py/__init__.py
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2022-12-12 07:26:35.879373 proxycurl-py-0.0.18/proxycurl_py/asyncio/
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       56 2022-12-07 06:05:27.000000 proxycurl-py-0.0.18/proxycurl_py/asyncio/__init__.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)     4709 2022-12-12 06:47:54.000000 proxycurl-py-0.0.18/proxycurl_py/asyncio/base.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    27719 2022-12-12 06:47:57.000000 proxycurl-py-0.0.18/proxycurl_py/asyncio/library.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      283 2022-12-07 06:29:54.000000 proxycurl-py-0.0.18/proxycurl_py/config.py
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2022-12-12 07:26:35.879373 proxycurl-py-0.0.18/proxycurl_py/gevent/
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       56 2022-12-07 06:05:26.000000 proxycurl-py-0.0.18/proxycurl_py/gevent/__init__.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)     4171 2022-12-12 06:47:34.000000 proxycurl-py-0.0.18/proxycurl_py/gevent/base.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    26611 2022-12-12 06:47:43.000000 proxycurl-py-0.0.18/proxycurl_py/gevent/library.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)     7913 2022-12-12 07:24:46.000000 proxycurl-py-0.0.18/proxycurl_py/models.py
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2022-12-12 07:26:35.883373 proxycurl-py-0.0.18/proxycurl_py/twisted/
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       56 2022-12-07 06:05:26.000000 proxycurl-py-0.0.18/proxycurl_py/twisted/__init__.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)     4995 2022-12-12 06:47:47.000000 proxycurl-py-0.0.18/proxycurl_py/twisted/base.py
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    26554 2022-12-12 06:47:51.000000 proxycurl-py-0.0.18/proxycurl_py/twisted/library.py
-drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2022-12-12 07:26:35.883373 proxycurl-py-0.0.18/proxycurl_py.egg-info/
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    10540 2022-12-12 07:26:35.000000 proxycurl-py-0.0.18/proxycurl_py.egg-info/PKG-INFO
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      586 2022-12-12 07:26:35.000000 proxycurl-py-0.0.18/proxycurl_py.egg-info/SOURCES.txt
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)        1 2022-12-12 07:26:35.000000 proxycurl-py-0.0.18/proxycurl_py.egg-info/dependency_links.txt
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      168 2022-12-12 07:26:35.000000 proxycurl-py-0.0.18/proxycurl_py.egg-info/requires.txt
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       13 2022-12-12 07:26:35.000000 proxycurl-py-0.0.18/proxycurl_py.egg-info/top_level.txt
--rw-r--r--   0 adiguna7  (1000) adiguna7  (1000)      772 2022-12-12 07:26:06.000000 proxycurl-py-0.0.18/pyproject.toml
--rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       38 2022-12-12 07:26:35.883373 proxycurl-py-0.0.18/setup.cfg
--rw-r--r--   0 adiguna7  (1000) adiguna7  (1000)      986 2022-12-12 07:26:11.000000 proxycurl-py-0.0.18/setup.py
+drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 05:48:53.729798 proxycurl-py-0.0.19/
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    12529 2023-04-27 05:48:53.729798 proxycurl-py-0.0.19/PKG-INFO
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    12288 2023-04-27 02:41:27.000000 proxycurl-py-0.0.19/README.md
+drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 05:48:53.729798 proxycurl-py-0.0.19/proxycurl_py/
+drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 05:48:53.729798 proxycurl-py-0.0.19/proxycurl_py/asyncio/
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       56 2023-04-27 02:41:52.000000 proxycurl-py-0.0.19/proxycurl_py/asyncio/__init__.py
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)     4709 2023-04-27 02:41:27.000000 proxycurl-py-0.0.19/proxycurl_py/asyncio/base.py
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    72492 2023-04-27 02:41:52.000000 proxycurl-py-0.0.19/proxycurl_py/asyncio/library.py
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      283 2023-04-27 02:41:27.000000 proxycurl-py-0.0.19/proxycurl_py/config.py
+drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 05:48:53.729798 proxycurl-py-0.0.19/proxycurl_py/gevent/
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       56 2023-04-27 02:41:52.000000 proxycurl-py-0.0.19/proxycurl_py/gevent/__init__.py
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)     4171 2023-04-27 02:41:27.000000 proxycurl-py-0.0.19/proxycurl_py/gevent/base.py
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    70856 2023-04-27 02:41:52.000000 proxycurl-py-0.0.19/proxycurl_py/gevent/library.py
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    14796 2023-04-27 02:41:52.000000 proxycurl-py-0.0.19/proxycurl_py/models.py
+drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 05:48:53.729798 proxycurl-py-0.0.19/proxycurl_py/twisted/
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       56 2023-04-27 02:41:52.000000 proxycurl-py-0.0.19/proxycurl_py/twisted/__init__.py
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)     4995 2023-04-27 02:41:27.000000 proxycurl-py-0.0.19/proxycurl_py/twisted/base.py
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    70542 2023-04-27 02:41:52.000000 proxycurl-py-0.0.19/proxycurl_py/twisted/library.py
+drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 05:48:53.729798 proxycurl-py-0.0.19/proxycurl_py.egg-info/
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)    12529 2023-04-27 05:48:53.000000 proxycurl-py-0.0.19/proxycurl_py.egg-info/PKG-INFO
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      583 2023-04-27 05:48:53.000000 proxycurl-py-0.0.19/proxycurl_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)        1 2023-04-27 05:48:53.000000 proxycurl-py-0.0.19/proxycurl_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      168 2023-04-27 05:48:53.000000 proxycurl-py-0.0.19/proxycurl_py.egg-info/requires.txt
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       13 2023-04-27 05:48:53.000000 proxycurl-py-0.0.19/proxycurl_py.egg-info/top_level.txt
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      772 2023-04-27 02:41:27.000000 proxycurl-py-0.0.19/pyproject.toml
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       38 2023-04-27 05:48:53.729798 proxycurl-py-0.0.19/setup.cfg
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)      985 2023-04-27 05:48:42.000000 proxycurl-py-0.0.19/setup.py
+drwxrwxr-x   0 adiguna7  (1000) adiguna7  (1000)        0 2023-04-27 05:48:53.729798 proxycurl-py-0.0.19/tests/
+-rw-rw-r--   0 adiguna7  (1000) adiguna7  (1000)       80 2023-04-27 02:41:27.000000 proxycurl-py-0.0.19/tests/test_proxycurl.py
```

### Comparing `proxycurl-py-0.0.18/PKG-INFO` & `proxycurl-py-0.0.19/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-Metadata-Version: 2.1
-Name: proxycurl-py
-Version: 0.0.18
-Summary: UNKNOWN
-Author: Nubela
-Author-email: tech@nubela.co
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.7,<4.0
-Description-Content-Type: text/markdown
-Provides-Extra: asyncio
-Provides-Extra: gevent
-Provides-Extra: twisted
-
 # `proxycurl-py` -  The official Python client for Proxycurl API to scrape and enrich LinkedIn profiles
 
-[toc]
+* [What is Proxycurl?](#what-is-proxycurl-)
+* [Before you install](#before-you-install)
+* [Installation and supported Python versions](#installation-and-supported-python-versions)
+* [Initializing `proxycurl-py` with an API Key](#initializing--proxycurl-py--with-an-api-key)
+* [Usage with examples](#usage-with-examples)
+  + [Enrich a Person Profile](#enrich-a-person-profile)
+  + [Enrich a Company Profile](#enrich-a-company-profile)
+  + [Lookup a person](#lookup-a-person)
+  + [Lookup a company](#lookup-a-company)
+  + [Lookup a LinkedIn Profile URL from a work email address](#lookup-a-linkedin-profile-url-from-a-work-email-address)
+  + [Enrich LinkedIn member profiles in bulk (from a CSV)](#enrich-linkedin-member-profiles-in-bulk--from-a-csv-)
+  + [More *asyncio* examples](#more--asyncio--examples)
+* [Rate limit and error handling](#rate-limit-and-error-handling)
+* [API Endpoints and their corresponding documentation](#api-endpoints-and-their-corresponding-documentation)
 
 ## What is Proxycurl?
 
 **Proxycurl** is an enrichment API to fetch fresh data on people and businesses. We are a fully-managed API that sits between your application and raw data so that you can focus on building the application; instead of worrying about building a web-scraping team and processing data at scale.
 
 With Proxycurl, you can programatically:
 
 - Enrich profiles on people and companies
 - Lookup people and companies
 - Lookup contact information on people and companies
 - Check if an email address is of a disposable nature
 - [And more..](https://nubela.co/proxycurl/docs#explain-it-to-me-like-i-39-m-5)
 
-Visit [Proxycurl's website](https://nubela.co/proxycurl) for more details.
+Visit [Proxycurl&#39;s website](https://nubela.co/proxycurl) for more details.
 
 ## Before you install
 
 You should understand that `proxycurl-py` was designed with concurrency as a first class citizen from ground-up. To install `proxycurl-py`, *you have to pick a concurency model*.
 
 We support the following concurrency models:
 
@@ -160,29 +159,26 @@
 
 However, there is a need for you to handle other error codes. Errors will be returned in the form of `ProxycurlException`. The [list of possible errors](https://nubela.co/proxycurl/docs#overview-errors) is listed in our API documentation.
 
 ## API Endpoints and their corresponding documentation
 
 Here we list the possible API endpoints and their corresponding library functions. Do refer to each endpoint's relevant API documentation to find out the required arguments that needs to be fed into the function.
 
-
-| Function | Endpoint | API |
-| - | - | - |
-| `linkedin.company.employee_count(**kwargs)` | [Employee Count Endpoint](https://nubela.co/proxycurl/docs#company-api-employee-count-endpoint) | [Company API](https://nubela.co/proxycurl/docs#company-api) |
-| `linkedin.company.resolve(**kwargs)` | [Company Lookup Endpoint](https://nubela.co/proxycurl/docs#company-api-company-profile-endpoint) | [Company API](https://nubela.co/proxycurl/docs#company-api) |
-| `linkedin.company.employee_list(**kwargs)` | [Employee Listing Endpoint](https://nubela.co/proxycurl/docs#company-api-employee-listing-endpoint) | [Company API](https://nubela.co/proxycurl/docs#company-api) |
-| `linkedin.company.get(**kwargs)` | [Company Profile Endpoint](https://nubela.co/proxycurl/docs#company-api-company-profile-endpoint) | [Company API](https://nubela.co/proxycurl/docs#company-api) |
-| `linkedin.person.resolve_by_email(**kwargs)` | [Reverse Work Email Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-reverse-work-email-lookup-endpoint) | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
-| `linkedin.person.lookup_email(**kwargs)` | [Work Email Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-work-email-lookup-endpoint) | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
+| Function                                       | Endpoint                                                                                                                     | API                                                      |
+| ---------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
+| `linkedin.company.employee_count(**kwargs)`  | [Employee Count Endpoint](https://nubela.co/proxycurl/docs#company-api-employee-count-endpoint)                                 | [Company API](https://nubela.co/proxycurl/docs#company-api) |
+| `linkedin.company.resolve(**kwargs)`         | [Company Lookup Endpoint](https://nubela.co/proxycurl/docs#company-api-company-profile-endpoint)                                | [Company API](https://nubela.co/proxycurl/docs#company-api) |
+| `linkedin.company.employee_list(**kwargs)`   | [Employee Listing Endpoint](https://nubela.co/proxycurl/docs#company-api-employee-listing-endpoint)                             | [Company API](https://nubela.co/proxycurl/docs#company-api) |
+| `linkedin.company.get(**kwargs)`             | [Company Profile Endpoint](https://nubela.co/proxycurl/docs#company-api-company-profile-endpoint)                               | [Company API](https://nubela.co/proxycurl/docs#company-api) |
+| `linkedin.person.resolve_by_email(**kwargs)` | [Reverse Work Email Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-reverse-work-email-lookup-endpoint)           | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
+| `linkedin.person.lookup_email(**kwargs)`     | [Work Email Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-work-email-lookup-endpoint)                           | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
 | `linkedin.person.personal_contact(**kwargs)` | [Personal Contact Number Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-personal-contact-number-lookup-endpoint) | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
-| `linkedin.person.personal_email(**kwargs)` | [Personal Email Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-personal-email-lookup-endpoint) | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
-| `linkedin.disposable_email(**kwargs)` | [Disposable Email Address Check Endpoint](https://nubela.co/proxycurl/docs#contact-api-disposable-email-address-check-endpoint) | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
-| `linkedin.company.find_job(**kwargs)` | [Job Listings Endpoint](https://nubela.co/proxycurl/docs#jobs-api-jobs-listing-endpoint) | [Jobs API](https://nubela.co/proxycurl/docs#jobs-api) |
-| `linkedin.job.get(**kwargs)` | [Jobs Profile Endpoint](https://nubela.co/proxycurl/docs#jobs-api-job-profile-endpoint) | [Jobs API](https://nubela.co/proxycurl/docs#jobs-api) |
-| `linkedin.person.resolve(**kwargs)` | [Person Lookup Endpoint](https://nubela.co/proxycurl/docs#people-api-person-lookup-endpoint) | [People API](https://nubela.co/proxycurl/docs#people-api) |
-| `linkedin.company.role_lookup(**kwargs)` | [Role Lookup Endpoint](https://nubela.co/proxycurl/docs#people-api-role-lookup-endpoint) | [People API](https://nubela.co/proxycurl/docs#people-api) |
-| `linkedin.person.get(**kwargs)` | [Person Profile Endpoint](https://nubela.co/proxycurl/docs#people-api-person-profile-endpoint) | [People API](https://nubela.co/proxycurl/docs#people-api) |
-| `linkedin.school.get(**kwargs)` | [School Profile Endpoint](https://nubela.co/proxycurl/docs#school-api-school-profile-endpoint) | [School API](https://nubela.co/proxycurl/docs#school-api) |
-| `linkedin.company.reveal` | [Reveal Endpoint](https://nubela.co/proxycurl/docs#reveal-api-reveal-endpoint) | [Reveal API](https://nubela.co/proxycurl/docs#reveal-api) |
-| `get_balance(**kwargs)` | [View Credit Balance Endpoint](https://nubela.co/proxycurl/docs#meta-api-view-credit-balance-endpoint) | [Meta API](https://nubela.co/proxycurl/docs#meta-api) |
-
-
+| `linkedin.person.personal_email(**kwargs)`   | [Personal Email Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-personal-email-lookup-endpoint)                   | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
+| `linkedin.disposable_email(**kwargs)`        | [Disposable Email Address Check Endpoint](https://nubela.co/proxycurl/docs#contact-api-disposable-email-address-check-endpoint) | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
+| `linkedin.company.find_job(**kwargs)`        | [Job Listings Endpoint](https://nubela.co/proxycurl/docs#jobs-api-jobs-listing-endpoint)                                        | [Jobs API](https://nubela.co/proxycurl/docs#jobs-api)       |
+| `linkedin.job.get(**kwargs)`                 | [Jobs Profile Endpoint](https://nubela.co/proxycurl/docs#jobs-api-job-profile-endpoint)                                         | [Jobs API](https://nubela.co/proxycurl/docs#jobs-api)       |
+| `linkedin.person.resolve(**kwargs)`          | [Person Lookup Endpoint](https://nubela.co/proxycurl/docs#people-api-person-lookup-endpoint)                                    | [People API](https://nubela.co/proxycurl/docs#people-api)   |
+| `linkedin.company.role_lookup(**kwargs)`     | [Role Lookup Endpoint](https://nubela.co/proxycurl/docs#people-api-role-lookup-endpoint)                                        | [People API](https://nubela.co/proxycurl/docs#people-api)   |
+| `linkedin.person.get(**kwargs)`              | [Person Profile Endpoint](https://nubela.co/proxycurl/docs#people-api-person-profile-endpoint)                                  | [People API](https://nubela.co/proxycurl/docs#people-api)   |
+| `linkedin.school.get(**kwargs)`              | [School Profile Endpoint](https://nubela.co/proxycurl/docs#school-api-school-profile-endpoint)                                  | [School API](https://nubela.co/proxycurl/docs#school-api)   |
+| `linkedin.company.reveal`                    | [Reveal Endpoint](https://nubela.co/proxycurl/docs#reveal-api-reveal-endpoint)                                                  | [Reveal API](https://nubela.co/proxycurl/docs#reveal-api)   |
+| `get_balance(**kwargs)`                      | [View Credit Balance Endpoint](https://nubela.co/proxycurl/docs#meta-api-view-credit-balance-endpoint)                          | [Meta API](https://nubela.co/proxycurl/docs#meta-api)       |
```

### Comparing `proxycurl-py-0.0.18/README.md` & `proxycurl-py-0.0.19/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,48 @@
+Metadata-Version: 2.1
+Name: proxycurl-py
+Version: 0.0.19
+Author: Nubela
+Author-email: tech@nubela.co
+Requires-Python: >=3.7,<4.0
+Description-Content-Type: text/markdown
+Provides-Extra: asyncio
+Provides-Extra: gevent
+Provides-Extra: twisted
+
 # `proxycurl-py` -  The official Python client for Proxycurl API to scrape and enrich LinkedIn profiles
 
-[toc]
+* [What is Proxycurl?](#what-is-proxycurl-)
+* [Before you install](#before-you-install)
+* [Installation and supported Python versions](#installation-and-supported-python-versions)
+* [Initializing `proxycurl-py` with an API Key](#initializing--proxycurl-py--with-an-api-key)
+* [Usage with examples](#usage-with-examples)
+  + [Enrich a Person Profile](#enrich-a-person-profile)
+  + [Enrich a Company Profile](#enrich-a-company-profile)
+  + [Lookup a person](#lookup-a-person)
+  + [Lookup a company](#lookup-a-company)
+  + [Lookup a LinkedIn Profile URL from a work email address](#lookup-a-linkedin-profile-url-from-a-work-email-address)
+  + [Enrich LinkedIn member profiles in bulk (from a CSV)](#enrich-linkedin-member-profiles-in-bulk--from-a-csv-)
+  + [More *asyncio* examples](#more--asyncio--examples)
+* [Rate limit and error handling](#rate-limit-and-error-handling)
+* [API Endpoints and their corresponding documentation](#api-endpoints-and-their-corresponding-documentation)
 
 ## What is Proxycurl?
 
 **Proxycurl** is an enrichment API to fetch fresh data on people and businesses. We are a fully-managed API that sits between your application and raw data so that you can focus on building the application; instead of worrying about building a web-scraping team and processing data at scale.
 
 With Proxycurl, you can programatically:
 
 - Enrich profiles on people and companies
 - Lookup people and companies
 - Lookup contact information on people and companies
 - Check if an email address is of a disposable nature
 - [And more..](https://nubela.co/proxycurl/docs#explain-it-to-me-like-i-39-m-5)
 
-Visit [Proxycurl's website](https://nubela.co/proxycurl) for more details.
+Visit [Proxycurl&#39;s website](https://nubela.co/proxycurl) for more details.
 
 ## Before you install
 
 You should understand that `proxycurl-py` was designed with concurrency as a first class citizen from ground-up. To install `proxycurl-py`, *you have to pick a concurency model*.
 
 We support the following concurrency models:
 
@@ -146,27 +170,26 @@
 
 However, there is a need for you to handle other error codes. Errors will be returned in the form of `ProxycurlException`. The [list of possible errors](https://nubela.co/proxycurl/docs#overview-errors) is listed in our API documentation.
 
 ## API Endpoints and their corresponding documentation
 
 Here we list the possible API endpoints and their corresponding library functions. Do refer to each endpoint's relevant API documentation to find out the required arguments that needs to be fed into the function.
 
-
-| Function | Endpoint | API |
-| - | - | - |
-| `linkedin.company.employee_count(**kwargs)` | [Employee Count Endpoint](https://nubela.co/proxycurl/docs#company-api-employee-count-endpoint) | [Company API](https://nubela.co/proxycurl/docs#company-api) |
-| `linkedin.company.resolve(**kwargs)` | [Company Lookup Endpoint](https://nubela.co/proxycurl/docs#company-api-company-profile-endpoint) | [Company API](https://nubela.co/proxycurl/docs#company-api) |
-| `linkedin.company.employee_list(**kwargs)` | [Employee Listing Endpoint](https://nubela.co/proxycurl/docs#company-api-employee-listing-endpoint) | [Company API](https://nubela.co/proxycurl/docs#company-api) |
-| `linkedin.company.get(**kwargs)` | [Company Profile Endpoint](https://nubela.co/proxycurl/docs#company-api-company-profile-endpoint) | [Company API](https://nubela.co/proxycurl/docs#company-api) |
-| `linkedin.person.resolve_by_email(**kwargs)` | [Reverse Work Email Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-reverse-work-email-lookup-endpoint) | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
-| `linkedin.person.lookup_email(**kwargs)` | [Work Email Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-work-email-lookup-endpoint) | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
+| Function                                       | Endpoint                                                                                                                     | API                                                      |
+| ---------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
+| `linkedin.company.employee_count(**kwargs)`  | [Employee Count Endpoint](https://nubela.co/proxycurl/docs#company-api-employee-count-endpoint)                                 | [Company API](https://nubela.co/proxycurl/docs#company-api) |
+| `linkedin.company.resolve(**kwargs)`         | [Company Lookup Endpoint](https://nubela.co/proxycurl/docs#company-api-company-profile-endpoint)                                | [Company API](https://nubela.co/proxycurl/docs#company-api) |
+| `linkedin.company.employee_list(**kwargs)`   | [Employee Listing Endpoint](https://nubela.co/proxycurl/docs#company-api-employee-listing-endpoint)                             | [Company API](https://nubela.co/proxycurl/docs#company-api) |
+| `linkedin.company.get(**kwargs)`             | [Company Profile Endpoint](https://nubela.co/proxycurl/docs#company-api-company-profile-endpoint)                               | [Company API](https://nubela.co/proxycurl/docs#company-api) |
+| `linkedin.person.resolve_by_email(**kwargs)` | [Reverse Work Email Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-reverse-work-email-lookup-endpoint)           | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
+| `linkedin.person.lookup_email(**kwargs)`     | [Work Email Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-work-email-lookup-endpoint)                           | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
 | `linkedin.person.personal_contact(**kwargs)` | [Personal Contact Number Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-personal-contact-number-lookup-endpoint) | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
-| `linkedin.person.personal_email(**kwargs)` | [Personal Email Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-personal-email-lookup-endpoint) | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
-| `linkedin.disposable_email(**kwargs)` | [Disposable Email Address Check Endpoint](https://nubela.co/proxycurl/docs#contact-api-disposable-email-address-check-endpoint) | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
-| `linkedin.company.find_job(**kwargs)` | [Job Listings Endpoint](https://nubela.co/proxycurl/docs#jobs-api-jobs-listing-endpoint) | [Jobs API](https://nubela.co/proxycurl/docs#jobs-api) |
-| `linkedin.job.get(**kwargs)` | [Jobs Profile Endpoint](https://nubela.co/proxycurl/docs#jobs-api-job-profile-endpoint) | [Jobs API](https://nubela.co/proxycurl/docs#jobs-api) |
-| `linkedin.person.resolve(**kwargs)` | [Person Lookup Endpoint](https://nubela.co/proxycurl/docs#people-api-person-lookup-endpoint) | [People API](https://nubela.co/proxycurl/docs#people-api) |
-| `linkedin.company.role_lookup(**kwargs)` | [Role Lookup Endpoint](https://nubela.co/proxycurl/docs#people-api-role-lookup-endpoint) | [People API](https://nubela.co/proxycurl/docs#people-api) |
-| `linkedin.person.get(**kwargs)` | [Person Profile Endpoint](https://nubela.co/proxycurl/docs#people-api-person-profile-endpoint) | [People API](https://nubela.co/proxycurl/docs#people-api) |
-| `linkedin.school.get(**kwargs)` | [School Profile Endpoint](https://nubela.co/proxycurl/docs#school-api-school-profile-endpoint) | [School API](https://nubela.co/proxycurl/docs#school-api) |
-| `linkedin.company.reveal` | [Reveal Endpoint](https://nubela.co/proxycurl/docs#reveal-api-reveal-endpoint) | [Reveal API](https://nubela.co/proxycurl/docs#reveal-api) |
-| `get_balance(**kwargs)` | [View Credit Balance Endpoint](https://nubela.co/proxycurl/docs#meta-api-view-credit-balance-endpoint) | [Meta API](https://nubela.co/proxycurl/docs#meta-api) |
+| `linkedin.person.personal_email(**kwargs)`   | [Personal Email Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-personal-email-lookup-endpoint)                   | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
+| `linkedin.disposable_email(**kwargs)`        | [Disposable Email Address Check Endpoint](https://nubela.co/proxycurl/docs#contact-api-disposable-email-address-check-endpoint) | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
+| `linkedin.company.find_job(**kwargs)`        | [Job Listings Endpoint](https://nubela.co/proxycurl/docs#jobs-api-jobs-listing-endpoint)                                        | [Jobs API](https://nubela.co/proxycurl/docs#jobs-api)       |
+| `linkedin.job.get(**kwargs)`                 | [Jobs Profile Endpoint](https://nubela.co/proxycurl/docs#jobs-api-job-profile-endpoint)                                         | [Jobs API](https://nubela.co/proxycurl/docs#jobs-api)       |
+| `linkedin.person.resolve(**kwargs)`          | [Person Lookup Endpoint](https://nubela.co/proxycurl/docs#people-api-person-lookup-endpoint)                                    | [People API](https://nubela.co/proxycurl/docs#people-api)   |
+| `linkedin.company.role_lookup(**kwargs)`     | [Role Lookup Endpoint](https://nubela.co/proxycurl/docs#people-api-role-lookup-endpoint)                                        | [People API](https://nubela.co/proxycurl/docs#people-api)   |
+| `linkedin.person.get(**kwargs)`              | [Person Profile Endpoint](https://nubela.co/proxycurl/docs#people-api-person-profile-endpoint)                                  | [People API](https://nubela.co/proxycurl/docs#people-api)   |
+| `linkedin.school.get(**kwargs)`              | [School Profile Endpoint](https://nubela.co/proxycurl/docs#school-api-school-profile-endpoint)                                  | [School API](https://nubela.co/proxycurl/docs#school-api)   |
+| `linkedin.company.reveal`                    | [Reveal Endpoint](https://nubela.co/proxycurl/docs#reveal-api-reveal-endpoint)                                                  | [Reveal API](https://nubela.co/proxycurl/docs#reveal-api)   |
+| `get_balance(**kwargs)`                      | [View Credit Balance Endpoint](https://nubela.co/proxycurl/docs#meta-api-view-credit-balance-endpoint)                          | [Meta API](https://nubela.co/proxycurl/docs#meta-api)       |
```

### Comparing `proxycurl-py-0.0.18/proxycurl_py/asyncio/base.py` & `proxycurl-py-0.0.19/proxycurl_py/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `proxycurl-py-0.0.18/proxycurl_py/gevent/base.py` & `proxycurl-py-0.0.19/proxycurl_py/gevent/base.py`

 * *Files identical despite different names*

### Comparing `proxycurl-py-0.0.18/proxycurl_py/twisted/base.py` & `proxycurl-py-0.0.19/proxycurl_py/twisted/base.py`

 * *Files identical despite different names*

### Comparing `proxycurl-py-0.0.18/proxycurl_py.egg-info/PKG-INFO` & `proxycurl-py-0.0.19/proxycurl_py.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 Metadata-Version: 2.1
 Name: proxycurl-py
-Version: 0.0.18
-Summary: UNKNOWN
+Version: 0.0.19
 Author: Nubela
 Author-email: tech@nubela.co
-License: UNKNOWN
-Platform: UNKNOWN
 Requires-Python: >=3.7,<4.0
 Description-Content-Type: text/markdown
 Provides-Extra: asyncio
 Provides-Extra: gevent
 Provides-Extra: twisted
 
 # `proxycurl-py` -  The official Python client for Proxycurl API to scrape and enrich LinkedIn profiles
 
-[toc]
+* [What is Proxycurl?](#what-is-proxycurl-)
+* [Before you install](#before-you-install)
+* [Installation and supported Python versions](#installation-and-supported-python-versions)
+* [Initializing `proxycurl-py` with an API Key](#initializing--proxycurl-py--with-an-api-key)
+* [Usage with examples](#usage-with-examples)
+  + [Enrich a Person Profile](#enrich-a-person-profile)
+  + [Enrich a Company Profile](#enrich-a-company-profile)
+  + [Lookup a person](#lookup-a-person)
+  + [Lookup a company](#lookup-a-company)
+  + [Lookup a LinkedIn Profile URL from a work email address](#lookup-a-linkedin-profile-url-from-a-work-email-address)
+  + [Enrich LinkedIn member profiles in bulk (from a CSV)](#enrich-linkedin-member-profiles-in-bulk--from-a-csv-)
+  + [More *asyncio* examples](#more--asyncio--examples)
+* [Rate limit and error handling](#rate-limit-and-error-handling)
+* [API Endpoints and their corresponding documentation](#api-endpoints-and-their-corresponding-documentation)
 
 ## What is Proxycurl?
 
 **Proxycurl** is an enrichment API to fetch fresh data on people and businesses. We are a fully-managed API that sits between your application and raw data so that you can focus on building the application; instead of worrying about building a web-scraping team and processing data at scale.
 
 With Proxycurl, you can programatically:
 
 - Enrich profiles on people and companies
 - Lookup people and companies
 - Lookup contact information on people and companies
 - Check if an email address is of a disposable nature
 - [And more..](https://nubela.co/proxycurl/docs#explain-it-to-me-like-i-39-m-5)
 
-Visit [Proxycurl's website](https://nubela.co/proxycurl) for more details.
+Visit [Proxycurl&#39;s website](https://nubela.co/proxycurl) for more details.
 
 ## Before you install
 
 You should understand that `proxycurl-py` was designed with concurrency as a first class citizen from ground-up. To install `proxycurl-py`, *you have to pick a concurency model*.
 
 We support the following concurrency models:
 
@@ -160,29 +170,26 @@
 
 However, there is a need for you to handle other error codes. Errors will be returned in the form of `ProxycurlException`. The [list of possible errors](https://nubela.co/proxycurl/docs#overview-errors) is listed in our API documentation.
 
 ## API Endpoints and their corresponding documentation
 
 Here we list the possible API endpoints and their corresponding library functions. Do refer to each endpoint's relevant API documentation to find out the required arguments that needs to be fed into the function.
 
-
-| Function | Endpoint | API |
-| - | - | - |
-| `linkedin.company.employee_count(**kwargs)` | [Employee Count Endpoint](https://nubela.co/proxycurl/docs#company-api-employee-count-endpoint) | [Company API](https://nubela.co/proxycurl/docs#company-api) |
-| `linkedin.company.resolve(**kwargs)` | [Company Lookup Endpoint](https://nubela.co/proxycurl/docs#company-api-company-profile-endpoint) | [Company API](https://nubela.co/proxycurl/docs#company-api) |
-| `linkedin.company.employee_list(**kwargs)` | [Employee Listing Endpoint](https://nubela.co/proxycurl/docs#company-api-employee-listing-endpoint) | [Company API](https://nubela.co/proxycurl/docs#company-api) |
-| `linkedin.company.get(**kwargs)` | [Company Profile Endpoint](https://nubela.co/proxycurl/docs#company-api-company-profile-endpoint) | [Company API](https://nubela.co/proxycurl/docs#company-api) |
-| `linkedin.person.resolve_by_email(**kwargs)` | [Reverse Work Email Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-reverse-work-email-lookup-endpoint) | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
-| `linkedin.person.lookup_email(**kwargs)` | [Work Email Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-work-email-lookup-endpoint) | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
+| Function                                       | Endpoint                                                                                                                     | API                                                      |
+| ---------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
+| `linkedin.company.employee_count(**kwargs)`  | [Employee Count Endpoint](https://nubela.co/proxycurl/docs#company-api-employee-count-endpoint)                                 | [Company API](https://nubela.co/proxycurl/docs#company-api) |
+| `linkedin.company.resolve(**kwargs)`         | [Company Lookup Endpoint](https://nubela.co/proxycurl/docs#company-api-company-profile-endpoint)                                | [Company API](https://nubela.co/proxycurl/docs#company-api) |
+| `linkedin.company.employee_list(**kwargs)`   | [Employee Listing Endpoint](https://nubela.co/proxycurl/docs#company-api-employee-listing-endpoint)                             | [Company API](https://nubela.co/proxycurl/docs#company-api) |
+| `linkedin.company.get(**kwargs)`             | [Company Profile Endpoint](https://nubela.co/proxycurl/docs#company-api-company-profile-endpoint)                               | [Company API](https://nubela.co/proxycurl/docs#company-api) |
+| `linkedin.person.resolve_by_email(**kwargs)` | [Reverse Work Email Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-reverse-work-email-lookup-endpoint)           | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
+| `linkedin.person.lookup_email(**kwargs)`     | [Work Email Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-work-email-lookup-endpoint)                           | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
 | `linkedin.person.personal_contact(**kwargs)` | [Personal Contact Number Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-personal-contact-number-lookup-endpoint) | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
-| `linkedin.person.personal_email(**kwargs)` | [Personal Email Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-personal-email-lookup-endpoint) | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
-| `linkedin.disposable_email(**kwargs)` | [Disposable Email Address Check Endpoint](https://nubela.co/proxycurl/docs#contact-api-disposable-email-address-check-endpoint) | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
-| `linkedin.company.find_job(**kwargs)` | [Job Listings Endpoint](https://nubela.co/proxycurl/docs#jobs-api-jobs-listing-endpoint) | [Jobs API](https://nubela.co/proxycurl/docs#jobs-api) |
-| `linkedin.job.get(**kwargs)` | [Jobs Profile Endpoint](https://nubela.co/proxycurl/docs#jobs-api-job-profile-endpoint) | [Jobs API](https://nubela.co/proxycurl/docs#jobs-api) |
-| `linkedin.person.resolve(**kwargs)` | [Person Lookup Endpoint](https://nubela.co/proxycurl/docs#people-api-person-lookup-endpoint) | [People API](https://nubela.co/proxycurl/docs#people-api) |
-| `linkedin.company.role_lookup(**kwargs)` | [Role Lookup Endpoint](https://nubela.co/proxycurl/docs#people-api-role-lookup-endpoint) | [People API](https://nubela.co/proxycurl/docs#people-api) |
-| `linkedin.person.get(**kwargs)` | [Person Profile Endpoint](https://nubela.co/proxycurl/docs#people-api-person-profile-endpoint) | [People API](https://nubela.co/proxycurl/docs#people-api) |
-| `linkedin.school.get(**kwargs)` | [School Profile Endpoint](https://nubela.co/proxycurl/docs#school-api-school-profile-endpoint) | [School API](https://nubela.co/proxycurl/docs#school-api) |
-| `linkedin.company.reveal` | [Reveal Endpoint](https://nubela.co/proxycurl/docs#reveal-api-reveal-endpoint) | [Reveal API](https://nubela.co/proxycurl/docs#reveal-api) |
-| `get_balance(**kwargs)` | [View Credit Balance Endpoint](https://nubela.co/proxycurl/docs#meta-api-view-credit-balance-endpoint) | [Meta API](https://nubela.co/proxycurl/docs#meta-api) |
-
-
+| `linkedin.person.personal_email(**kwargs)`   | [Personal Email Lookup Endpoint](https://nubela.co/proxycurl/docs#contact-api-personal-email-lookup-endpoint)                   | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
+| `linkedin.disposable_email(**kwargs)`        | [Disposable Email Address Check Endpoint](https://nubela.co/proxycurl/docs#contact-api-disposable-email-address-check-endpoint) | [Contact API](https://nubela.co/proxycurl/docs#contact-api) |
+| `linkedin.company.find_job(**kwargs)`        | [Job Listings Endpoint](https://nubela.co/proxycurl/docs#jobs-api-jobs-listing-endpoint)                                        | [Jobs API](https://nubela.co/proxycurl/docs#jobs-api)       |
+| `linkedin.job.get(**kwargs)`                 | [Jobs Profile Endpoint](https://nubela.co/proxycurl/docs#jobs-api-job-profile-endpoint)                                         | [Jobs API](https://nubela.co/proxycurl/docs#jobs-api)       |
+| `linkedin.person.resolve(**kwargs)`          | [Person Lookup Endpoint](https://nubela.co/proxycurl/docs#people-api-person-lookup-endpoint)                                    | [People API](https://nubela.co/proxycurl/docs#people-api)   |
+| `linkedin.company.role_lookup(**kwargs)`     | [Role Lookup Endpoint](https://nubela.co/proxycurl/docs#people-api-role-lookup-endpoint)                                        | [People API](https://nubela.co/proxycurl/docs#people-api)   |
+| `linkedin.person.get(**kwargs)`              | [Person Profile Endpoint](https://nubela.co/proxycurl/docs#people-api-person-profile-endpoint)                                  | [People API](https://nubela.co/proxycurl/docs#people-api)   |
+| `linkedin.school.get(**kwargs)`              | [School Profile Endpoint](https://nubela.co/proxycurl/docs#school-api-school-profile-endpoint)                                  | [School API](https://nubela.co/proxycurl/docs#school-api)   |
+| `linkedin.company.reveal`                    | [Reveal Endpoint](https://nubela.co/proxycurl/docs#reveal-api-reveal-endpoint)                                                  | [Reveal API](https://nubela.co/proxycurl/docs#reveal-api)   |
+| `get_balance(**kwargs)`                      | [View Credit Balance Endpoint](https://nubela.co/proxycurl/docs#meta-api-view-credit-balance-endpoint)                          | [Meta API](https://nubela.co/proxycurl/docs#meta-api)       |
```

### Comparing `proxycurl-py-0.0.18/proxycurl_py.egg-info/SOURCES.txt` & `proxycurl-py-0.0.19/proxycurl_py.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 README.md
 pyproject.toml
 setup.py
-./proxycurl_py/__init__.py
 ./proxycurl_py/config.py
 ./proxycurl_py/models.py
 ./proxycurl_py/asyncio/__init__.py
 ./proxycurl_py/asyncio/base.py
 ./proxycurl_py/asyncio/library.py
 ./proxycurl_py/gevent/__init__.py
 ./proxycurl_py/gevent/base.py
@@ -13,8 +12,9 @@
 ./proxycurl_py/twisted/__init__.py
 ./proxycurl_py/twisted/base.py
 ./proxycurl_py/twisted/library.py
 proxycurl_py.egg-info/PKG-INFO
 proxycurl_py.egg-info/SOURCES.txt
 proxycurl_py.egg-info/dependency_links.txt
 proxycurl_py.egg-info/requires.txt
-proxycurl_py.egg-info/top_level.txt
+proxycurl_py.egg-info/top_level.txt
+tests/test_proxycurl.py
```

### Comparing `proxycurl-py-0.0.18/pyproject.toml` & `proxycurl-py-0.0.19/pyproject.toml`

 * *Files identical despite different names*

### Comparing `proxycurl-py-0.0.18/setup.py` & `proxycurl-py-0.0.19/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 extras_require = \
 {'asyncio': ['asyncio>=3.4.3,<4.0.0', 'aiohttp>=3.7.4,<4.0.0'],
  'gevent': ['gevent>=21.1.1,<22.0.0', 'requests>=2.25.0,<3.0.0'],
  'twisted': ['Twisted>=21.7.0,<22.0.0', 'treq>=21.5.0,<22.0.0']}
 
 setup_kwargs = {
     'name': 'proxycurl-py',
-    'version': '0.0.18',
+    'version': '0.0.19',
     'description': '',
     'long_description_content_type':"text/markdown",
     'long_description': long_description,
     'author': 'Nubela',
     'author_email': 'tech@nubela.co',
     'maintainer': None,
     'maintainer_email': None,
@@ -33,8 +33,8 @@
     'package_data': package_data,
     'package_dir': {'': '.'},
     'extras_require': extras_require,
     'python_requires': '>=3.7,<4.0',
 }
 
 
-setup(**setup_kwargs)
+setup(**setup_kwargs)
```

