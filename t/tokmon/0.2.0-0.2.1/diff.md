# Comparing `tmp/tokmon-0.2.0.tar.gz` & `tmp/tokmon-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokmon-0.2.0.tar", last modified: Wed Apr 26 02:14:59 2023, max compression
+gzip compressed data, was "tokmon-0.2.1.tar", last modified: Thu Apr 27 17:37:04 2023, max compression
```

## Comparing `tokmon-0.2.0.tar` & `tokmon-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:14:59.357382 tokmon-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-04-26 02:14:46.000000 tokmon-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-04-26 02:14:59.357382 tokmon-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-04-26 02:14:46.000000 tokmon-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 02:14:59.357382 tokmon-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-26 02:14:46.000000 tokmon-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:14:59.357382 tokmon-0.2.0/tokmon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:14:46.000000 tokmon-0.2.0/tokmon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-26 02:14:46.000000 tokmon-0.2.0/tokmon/beam.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7617 2023-04-26 02:14:46.000000 tokmon-0.2.0/tokmon/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-26 02:14:46.000000 tokmon-0.2.0/tokmon/costcalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-26 02:14:46.000000 tokmon-0.2.0/tokmon/openai-pricing.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     9442 2023-04-26 02:14:46.000000 tokmon-0.2.0/tokmon/tokmon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-26 02:14:46.000000 tokmon-0.2.0/tokmon/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:14:59.357382 tokmon-0.2.0/tokmon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-04-26 02:14:59.000000 tokmon-0.2.0/tokmon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-26 02:14:59.000000 tokmon-0.2.0/tokmon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 02:14:59.000000 tokmon-0.2.0/tokmon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-26 02:14:59.000000 tokmon-0.2.0/tokmon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-26 02:14:59.000000 tokmon-0.2.0/tokmon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 02:14:59.000000 tokmon-0.2.0/tokmon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:37:04.507243 tokmon-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-04-27 17:36:45.000000 tokmon-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-04-27 17:37:04.507243 tokmon-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10076 2023-04-27 17:36:45.000000 tokmon-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 17:37:04.507243 tokmon-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-27 17:36:45.000000 tokmon-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:37:04.503243 tokmon-0.2.1/tokmon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 17:36:45.000000 tokmon-0.2.1/tokmon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-27 17:36:45.000000 tokmon-0.2.1/tokmon/beam.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7617 2023-04-27 17:36:45.000000 tokmon-0.2.1/tokmon/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-27 17:36:45.000000 tokmon-0.2.1/tokmon/costcalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-27 17:36:45.000000 tokmon-0.2.1/tokmon/openai-pricing.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9735 2023-04-27 17:36:45.000000 tokmon-0.2.1/tokmon/tokmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-27 17:36:45.000000 tokmon-0.2.1/tokmon/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 17:37:04.507243 tokmon-0.2.1/tokmon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-04-27 17:37:04.000000 tokmon-0.2.1/tokmon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-27 17:37:04.000000 tokmon-0.2.1/tokmon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 17:37:04.000000 tokmon-0.2.1/tokmon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-27 17:37:04.000000 tokmon-0.2.1/tokmon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-27 17:37:04.000000 tokmon-0.2.1/tokmon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 17:37:04.000000 tokmon-0.2.1/tokmon.egg-info/top_level.txt
```

### Comparing `tokmon-0.2.0/LICENSE` & `tokmon-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tokmon-0.2.0/PKG-INFO` & `tokmon-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,40 @@
-Metadata-Version: 2.1
-Name: tokmon
-Version: 0.2.0
-Summary: tokmon is a CLI utility to monitor OpenAI token usage and costs
-Home-page: https://github.com/yagil/tokmon
-Project-URL: Bug Reports, https://github.com/yagil/tokmon/issues
-Project-URL: Source, https://github.com/yagil/tokmon/
-Description-Content-Type: text/markdown
-License-File: LICENSE
+<h4 align="center">⚡️<i><b>NEW</b></i>: <a href="https://github.com/yagil/tokmon-beam"> tokmon beam </a> - a self-hosted web UI to monitor API usage data, running from <code>localhost</code>.</h4>
 
 <pre align="center">
 
  ______   ______    __  __    __    __    ______    __   __    
 /\__  _\ /\  __ \  /\ \/ /   /\ "-./  \  /\  __ \  /\ "-.\ \   
 \/_/\ \/ \ \ \/\ \ \ \  _"-. \ \ \-./\ \ \ \ \/\ \ \ \ \-.  \  
    \ \_\  \ \_____\ \ \_\ \_\ \ \_\ \ \_\ \ \_____\ \ \_\\"\_\ 
     \/_/   \/_____/  \/_/\/_/  \/_/  \/_/  \/_____/  \/_/ \/_/ 
                                                                    
 
 CLI utility to monitor your OpenAI API token usage
-                                                                   
-</pre>
 
-<p align="center">⚡️<i><b>NEW</b></i>: <a href="https://github.com/yagil/tokmon-beam"> tokmon beam </a> - a self-hosted web UI to monitor API usage data, running from <code>localhost</code>.</p>
+</pre>
 
 <p align="center">
   <a href="https://github.com/yagil/tokmon/blob/main/LICENSE" target="_blank">
       <img src="https://img.shields.io/badge/License-Apache2.0-orange.svg" alt="License">
   </a>
 </p>
 
 # `tokmon` 🔤🧐 - CLI to monitor OpenAI API usage
 
-`tokmon` (**Tok**en **Mon**itor) keeps track of your program's OpenAI API token usage.
+`tokmon` (**Tok**en **Mon**itor) lets you keep track of your program's OpenAI API token usage.
 
-You can use `tokmon` just like you would use the `time` utility, but instead of execution time you get token usage and cost.
+You can use `tokmon` just like you would use the `time` utility, but instead of execution time you get OpenAI usage and cost stats.
 
 ## Installation
 ```
 pip install tokmon
 ```
 ## Usage
+> **Note**:  tokmon works for `gpt-*` models (`gpt-3.5-turbo`, `gpt-4`, etc.). If you need support for other models (e.g. `davinci`) see [tokmon#6](https://github.com/yagil/tokmon/issues/6).
 ```bash
 $ tokmon /path/to/your/<your program> [arg1] [arg2] ...
 ```
 
 ```css
 tokmon cost report:
 ================================================================================
@@ -95,15 +86,28 @@
 
 Prepend `tokmon` to your normal program invocation like so:
 ```bash
 $ tokmon /path/to/your/<your program> [arg1] [arg2] ...
 ```
 Run and use your program just like you would normally (arguments and all). Interactive usage is supported as well.
 
-#### Using `tokmon` with `npm run` (e.g. with NextJS)
+## Python
+Simply add `tokmon` to the beginning of your regular invocation
+```bash
+$ tokmon python /path/to/your/script.py
+```
+This will work for scripts and long running programs like Django / Flask / FastAPI servers.
+
+## Node
+For scripts:
+```bash
+$ tokmon node /path/to/your/script.js
+```
+
+### `npm run`
 Edit your `package.json`'s "scripts" entry to include `tokmon`. 
 
 ```js
 {
     "scripts": {
         "dev": "tokmon next dev",
         ...
@@ -197,39 +201,41 @@
 > For best results, make sure to check that you have the latest pricing.
 
 ## Misc
 
 ### Golang
 Hacky workaround for Golang programs. Add this to your program:
 ```go
-	// Import these packages
-	import (
-		"os"
-	    "crypto/tls"
-    	"crypto/x509"
-    	"io/ioutil"
-    	"net/http"
-    )
-
-	// Place this code somewhere in your go program *before* you make any calls to OpenAI's API.
-	certFile := os.Getenv("TOKMON_SSL_CERT_FILE") // This env variable is set by tokmon whenever it runs your program.
-	caCert, err := ioutil.ReadFile(certFile)
-	if err == nil { 
-		caCertPool, _ := x509.SystemCertPool()
-		caCertPool.AppendCertsFromPEM(caCert)
-		http.DefaultTransport.(*http.Transport).TLSClientConfig = &tls.Config{
-			RootCAs: caCertPool,
-		}
+// Import these packages
+import (
+	"os"
+	"crypto/tls"
+	"crypto/x509"
+	"io/ioutil"
+	"net/http"
+)
+
+// Place this code somewhere in your go program *before* you make any calls to OpenAI's API.
+certFile := os.Getenv("TOKMON_SSL_CERT_FILE") // This env variable will be set by tokmon
+caCert, err := ioutil.ReadFile(certFile)
+if err == nil { 
+	caCertPool, _ := x509.SystemCertPool()
+	caCertPool.AppendCertsFromPEM(caCert)
+	http.DefaultTransport.(*http.Transport).TLSClientConfig = &tls.Config{
+		RootCAs: caCertPool,
 	}
+}
 ```
 
 ## Current Limitations
 1. Event streaming: `tokmon` buffers Server-Sent Events (SSE) until the `data: [DONE]` chunk is received. If the monitored program leverages event streaming, its behavior will be modified.
-    - Issue: [yagil/tokmon#4](https://github.com/yagil/tokmon/issues/4)
-2
+    - Issue: [tokmon#4](https://github.com/yagil/tokmon/issues/4)
+2. Only chat models are supported (`gpt-3.5-turbo`, `gpt-4` and variants)
+    - Issue: [tokmon#6](https://github.com/yagil/tokmon/issues/6)
+
 ## Contributing
 If you'd like to contribute to the project, please follow these steps:
 1. Fork the repository.
 2. Create a new branch for your changes.
 3. Make your changes and test them.
 4. Submit a pull request with a clear description of your changes and any relevant information.
```

#### html2text {}

```diff
@@ -1,31 +1,27 @@
-Metadata-Version: 2.1 Name: tokmon Version: 0.2.0 Summary: tokmon is a CLI
-utility to monitor OpenAI token usage and costs Home-page: https://github.com/
-yagil/tokmon Project-URL: Bug Reports, https://github.com/yagil/tokmon/issues
-Project-URL: Source, https://github.com/yagil/tokmon/ Description-Content-Type:
-text/markdown License-File: LICENSE
+ *** â¡ï¸NEW: tokmon_beam - a self-hosted web UI to monitor API usage data,
+                          running from localhost. ***
 
  ______   ______    __  __    __    __    ______    __   __
 /\__  _\ /\  __ \  /\ \/ /   /\ "-./  \  /\  __ \  /\ "-.\ \
 \/_/\ \/ \ \ \/\ \ \ \  _"-. \ \ \-./\ \ \ \ \/\ \ \ \ \-.  \
    \ \_\  \ \_____\ \ \_\ \_\ \ \_\ \ \_\ \ \_____\ \ \_\\"\_\
     \/_/   \/_____/  \/_/\/_/  \/_/  \/_/  \/_____/  \/_/ \/_/
 
 
 CLI utility to monitor your OpenAI API token usage
-
-   â¡ï¸NEW: tokmon_beam - a self-hosted web UI to monitor API usage data,
-                            running from localhost.
                                    [License]
 # `tokmon` ð¤ð§ - CLI to monitor OpenAI API usage `tokmon` (**Tok**en
-**Mon**itor) keeps track of your program's OpenAI API token usage. You can use
-`tokmon` just like you would use the `time` utility, but instead of execution
-time you get token usage and cost. ## Installation ``` pip install tokmon ```
-## Usage ```bash $ tokmon /path/to/your/ [arg1] [arg2] ... ``` ```css tokmon
-cost report:
+**Mon**itor) lets you keep track of your program's OpenAI API token usage. You
+can use `tokmon` just like you would use the `time` utility, but instead of
+execution time you get OpenAI usage and cost stats. ## Installation ``` pip
+install tokmon ``` ## Usage > **Note**: tokmon works for `gpt-*` models (`gpt-
+3.5-turbo`, `gpt-4`, etc.). If you need support for other models (e.g.
+`davinci`) see [tokmon#6](https://github.com/yagil/tokmon/issues/6). ```bash $
+tokmon /path/to/your/ [arg1] [arg2] ... ``` ```css tokmon cost report:
 ================================================================================
 Monitored invocation: python3 ./tests/python_example.py --prompt say 'hello,
 tokmon!' Models: ['gpt-3.5-turbo-0301'] Total Usage: {'total_prompt_tokens':
 26, 'total_completion_tokens': 12, 'total_tokens': 38} Pricing: {'gpt-3.5-
 turbo-0301': {'prompt_cost': 0.002, 'completion_cost': 0.002, 'per_tokens':
 1000}} Total Cost: $0.000076
 ================================================================================
@@ -54,28 +50,31 @@
 format.
 ===============================================================================
 ## Use `tokmon` with your application or script > **Warning** > This is a
 debugging tool. It is not intended to be used in any consequential setting. Use
 your best judgement! Prepend `tokmon` to your normal program invocation like
 so: ```bash $ tokmon /path/to/your/ [arg1] [arg2] ... ``` Run and use your
 program just like you would normally (arguments and all). Interactive usage is
-supported as well. #### Using `tokmon` with `npm run` (e.g. with NextJS) Edit
-your `package.json`'s "scripts" entry to include `tokmon`. ```js { "scripts":
-{ "dev": "tokmon next dev", ... } } ``` ## Full usage and cost summary (JSON)
-```json { "total_cost": 0.0019199999999999998, "total_usage":
-{ "total_prompt_tokens": 18, "total_completion_tokens": 23, "total_tokens": 41
-}, "pricing_data": "{'gpt-4-0314': {'prompt_cost': 0.03, 'completion_cost':
-0.06, 'per_tokens': 1000}}", "models": [ "gpt-4-0314" ], "raw_data": [
-{ "model": "gpt-4-0314", "usage": { "prompt_tokens": 18, "completion_tokens":
-23, "total_tokens": 41 }, "cost": 0.0019199999999999998, "messages": [
-{ "role": "system", "content": "You're a helpful assistant." }, { "role":
-"user", "content": "hello" }, { "role": "assistant", "content": "Hello! How can
-I help you today? If you have any questions or need assistance, feel free to
-ask." } ] } ] } ``` ## How it works `tokmon` uses the [mitmproxy library]
-(https://github.com/mitmproxy/mitmproxy) to intercept HTTP requests and
+supported as well. ## Python Simply add `tokmon` to the beginning of your
+regular invocation ```bash $ tokmon python /path/to/your/script.py ``` This
+will work for scripts and long running programs like Django / Flask / FastAPI
+servers. ## Node For scripts: ```bash $ tokmon node /path/to/your/script.js ```
+### `npm run` Edit your `package.json`'s "scripts" entry to include `tokmon`.
+```js { "scripts": { "dev": "tokmon next dev", ... } } ``` ## Full usage and
+cost summary (JSON) ```json { "total_cost": 0.0019199999999999998,
+"total_usage": { "total_prompt_tokens": 18, "total_completion_tokens": 23,
+"total_tokens": 41 }, "pricing_data": "{'gpt-4-0314': {'prompt_cost': 0.03,
+'completion_cost': 0.06, 'per_tokens': 1000}}", "models": [ "gpt-4-0314" ],
+"raw_data": [ { "model": "gpt-4-0314", "usage": { "prompt_tokens": 18,
+"completion_tokens": 23, "total_tokens": 41 }, "cost": 0.0019199999999999998,
+"messages": [ { "role": "system", "content": "You're a helpful assistant." },
+{ "role": "user", "content": "hello" }, { "role": "assistant", "content":
+"Hello! How can I help you today? If you have any questions or need assistance,
+feel free to ask." } ] } ] } ``` ## How it works `tokmon` uses the [mitmproxy
+library](https://github.com/mitmproxy/mitmproxy) to intercept HTTP requests and
 responses between your program and the OpenAI API. It then processes the
 request and response data to calculate token usage and cost based on [tokmon/
 openai-pricing.json](tokmon/openai-pricing.json). > `tokmon` works for programs
 in `python` / `node` (using OpenAI's clients), or `curl` (run directly, and not
 i.e. in a bash script). > See [Golang instructions](#golang) for instructions
 on how to use `tokmon` with Golang programs. > if you [manually install
 `mitmproxy`'s CA certificate](https://docs.mitmproxy.org/stable/concepts-
@@ -107,23 +106,25 @@
 to/your/custom-openai-pricing.json ...` > This pricing JSON is incomplete
 (missing DALL-E, etc.), it may be incorrect, and it may go out of date. > For
 best results, make sure to check that you have the latest pricing. ## Misc ###
 Golang Hacky workaround for Golang programs. Add this to your program: ```go /
 / Import these packages import ( "os" "crypto/tls" "crypto/x509" "io/ioutil"
 "net/http" ) // Place this code somewhere in your go program *before* you make
 any calls to OpenAI's API. certFile := os.Getenv("TOKMON_SSL_CERT_FILE") /
-/ This env variable is set by tokmon whenever it runs your program. caCert, err
-:= ioutil.ReadFile(certFile) if err == nil { caCertPool, _ :
-= x509.SystemCertPool() caCertPool.AppendCertsFromPEM(caCert)
-http.DefaultTransport.(*http.Transport).TLSClientConfig = &tls.Config{ RootCAs:
-caCertPool, } } ``` ## Current Limitations 1. Event streaming: `tokmon` buffers
-Server-Sent Events (SSE) until the `data: [DONE]` chunk is received. If the
-monitored program leverages event streaming, its behavior will be modified. -
-Issue: [yagil/tokmon#4](https://github.com/yagil/tokmon/issues/4) 2 ##
-Contributing If you'd like to contribute to the project, please follow these
-steps: 1. Fork the repository. 2. Create a new branch for your changes. 3. Make
-your changes and test them. 4. Submit a pull request with a clear description
-of your changes and any relevant information. ## Warning 1. `tokmon` comes
-without any warranty or guarantee whatsoever. 2. `tokmon` was tested on macOS
-only. It might not work on other platforms. 3. This tool may not work as
-intended, have unknown side effects, may output incorrect information, or not
-work at all. 4. The pricing data in `openai-pricing.json` may go out of date.
+/ This env variable will be set by tokmon caCert, err := ioutil.ReadFile
+(certFile) if err == nil { caCertPool, _ := x509.SystemCertPool()
+caCertPool.AppendCertsFromPEM(caCert) http.DefaultTransport.
+(*http.Transport).TLSClientConfig = &tls.Config{ RootCAs: caCertPool, } } ```
+## Current Limitations 1. Event streaming: `tokmon` buffers Server-Sent Events
+(SSE) until the `data: [DONE]` chunk is received. If the monitored program
+leverages event streaming, its behavior will be modified. - Issue: [tokmon#4]
+(https://github.com/yagil/tokmon/issues/4) 2. Only chat models are supported
+(`gpt-3.5-turbo`, `gpt-4` and variants) - Issue: [tokmon#6](https://github.com/
+yagil/tokmon/issues/6) ## Contributing If you'd like to contribute to the
+project, please follow these steps: 1. Fork the repository. 2. Create a new
+branch for your changes. 3. Make your changes and test them. 4. Submit a pull
+request with a clear description of your changes and any relevant information.
+## Warning 1. `tokmon` comes without any warranty or guarantee whatsoever. 2.
+`tokmon` was tested on macOS only. It might not work on other platforms. 3.
+This tool may not work as intended, have unknown side effects, may output
+incorrect information, or not work at all. 4. The pricing data in `openai-
+pricing.json` may go out of date.
```

### Comparing `tokmon-0.2.0/README.md` & `tokmon-0.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,50 @@
+Metadata-Version: 2.1
+Name: tokmon
+Version: 0.2.1
+Summary: tokmon is a CLI utility to monitor OpenAI token usage and costs
+Home-page: https://github.com/yagil/tokmon
+Project-URL: Bug Reports, https://github.com/yagil/tokmon/issues
+Project-URL: Source, https://github.com/yagil/tokmon/
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<h4 align="center">⚡️<i><b>NEW</b></i>: <a href="https://github.com/yagil/tokmon-beam"> tokmon beam </a> - a self-hosted web UI to monitor API usage data, running from <code>localhost</code>.</h4>
+
 <pre align="center">
 
  ______   ______    __  __    __    __    ______    __   __    
 /\__  _\ /\  __ \  /\ \/ /   /\ "-./  \  /\  __ \  /\ "-.\ \   
 \/_/\ \/ \ \ \/\ \ \ \  _"-. \ \ \-./\ \ \ \ \/\ \ \ \ \-.  \  
    \ \_\  \ \_____\ \ \_\ \_\ \ \_\ \ \_\ \ \_____\ \ \_\\"\_\ 
     \/_/   \/_____/  \/_/\/_/  \/_/  \/_/  \/_____/  \/_/ \/_/ 
                                                                    
 
 CLI utility to monitor your OpenAI API token usage
-                                                                   
-</pre>
 
-<p align="center">⚡️<i><b>NEW</b></i>: <a href="https://github.com/yagil/tokmon-beam"> tokmon beam </a> - a self-hosted web UI to monitor API usage data, running from <code>localhost</code>.</p>
+</pre>
 
 <p align="center">
   <a href="https://github.com/yagil/tokmon/blob/main/LICENSE" target="_blank">
       <img src="https://img.shields.io/badge/License-Apache2.0-orange.svg" alt="License">
   </a>
 </p>
 
 # `tokmon` 🔤🧐 - CLI to monitor OpenAI API usage
 
-`tokmon` (**Tok**en **Mon**itor) keeps track of your program's OpenAI API token usage.
+`tokmon` (**Tok**en **Mon**itor) lets you keep track of your program's OpenAI API token usage.
 
-You can use `tokmon` just like you would use the `time` utility, but instead of execution time you get token usage and cost.
+You can use `tokmon` just like you would use the `time` utility, but instead of execution time you get OpenAI usage and cost stats.
 
 ## Installation
 ```
 pip install tokmon
 ```
 ## Usage
+> **Note**:  tokmon works for `gpt-*` models (`gpt-3.5-turbo`, `gpt-4`, etc.). If you need support for other models (e.g. `davinci`) see [tokmon#6](https://github.com/yagil/tokmon/issues/6).
 ```bash
 $ tokmon /path/to/your/<your program> [arg1] [arg2] ...
 ```
 
 ```css
 tokmon cost report:
 ================================================================================
@@ -85,15 +96,28 @@
 
 Prepend `tokmon` to your normal program invocation like so:
 ```bash
 $ tokmon /path/to/your/<your program> [arg1] [arg2] ...
 ```
 Run and use your program just like you would normally (arguments and all). Interactive usage is supported as well.
 
-#### Using `tokmon` with `npm run` (e.g. with NextJS)
+## Python
+Simply add `tokmon` to the beginning of your regular invocation
+```bash
+$ tokmon python /path/to/your/script.py
+```
+This will work for scripts and long running programs like Django / Flask / FastAPI servers.
+
+## Node
+For scripts:
+```bash
+$ tokmon node /path/to/your/script.js
+```
+
+### `npm run`
 Edit your `package.json`'s "scripts" entry to include `tokmon`. 
 
 ```js
 {
     "scripts": {
         "dev": "tokmon next dev",
         ...
@@ -187,39 +211,41 @@
 > For best results, make sure to check that you have the latest pricing.
 
 ## Misc
 
 ### Golang
 Hacky workaround for Golang programs. Add this to your program:
 ```go
-	// Import these packages
-	import (
-		"os"
-	    "crypto/tls"
-    	"crypto/x509"
-    	"io/ioutil"
-    	"net/http"
-    )
-
-	// Place this code somewhere in your go program *before* you make any calls to OpenAI's API.
-	certFile := os.Getenv("TOKMON_SSL_CERT_FILE") // This env variable is set by tokmon whenever it runs your program.
-	caCert, err := ioutil.ReadFile(certFile)
-	if err == nil { 
-		caCertPool, _ := x509.SystemCertPool()
-		caCertPool.AppendCertsFromPEM(caCert)
-		http.DefaultTransport.(*http.Transport).TLSClientConfig = &tls.Config{
-			RootCAs: caCertPool,
-		}
+// Import these packages
+import (
+	"os"
+	"crypto/tls"
+	"crypto/x509"
+	"io/ioutil"
+	"net/http"
+)
+
+// Place this code somewhere in your go program *before* you make any calls to OpenAI's API.
+certFile := os.Getenv("TOKMON_SSL_CERT_FILE") // This env variable will be set by tokmon
+caCert, err := ioutil.ReadFile(certFile)
+if err == nil { 
+	caCertPool, _ := x509.SystemCertPool()
+	caCertPool.AppendCertsFromPEM(caCert)
+	http.DefaultTransport.(*http.Transport).TLSClientConfig = &tls.Config{
+		RootCAs: caCertPool,
 	}
+}
 ```
 
 ## Current Limitations
 1. Event streaming: `tokmon` buffers Server-Sent Events (SSE) until the `data: [DONE]` chunk is received. If the monitored program leverages event streaming, its behavior will be modified.
-    - Issue: [yagil/tokmon#4](https://github.com/yagil/tokmon/issues/4)
-2
+    - Issue: [tokmon#4](https://github.com/yagil/tokmon/issues/4)
+2. Only chat models are supported (`gpt-3.5-turbo`, `gpt-4` and variants)
+    - Issue: [tokmon#6](https://github.com/yagil/tokmon/issues/6)
+
 ## Contributing
 If you'd like to contribute to the project, please follow these steps:
 1. Fork the repository.
 2. Create a new branch for your changes.
 3. Make your changes and test them.
 4. Submit a pull request with a clear description of your changes and any relevant information.
```

#### html2text {}

```diff
@@ -1,26 +1,32 @@
+Metadata-Version: 2.1 Name: tokmon Version: 0.2.1 Summary: tokmon is a CLI
+utility to monitor OpenAI token usage and costs Home-page: https://github.com/
+yagil/tokmon Project-URL: Bug Reports, https://github.com/yagil/tokmon/issues
+Project-URL: Source, https://github.com/yagil/tokmon/ Description-Content-Type:
+text/markdown License-File: LICENSE
+ *** â¡ï¸NEW: tokmon_beam - a self-hosted web UI to monitor API usage data,
+                          running from localhost. ***
 
  ______   ______    __  __    __    __    ______    __   __
 /\__  _\ /\  __ \  /\ \/ /   /\ "-./  \  /\  __ \  /\ "-.\ \
 \/_/\ \/ \ \ \/\ \ \ \  _"-. \ \ \-./\ \ \ \ \/\ \ \ \ \-.  \
    \ \_\  \ \_____\ \ \_\ \_\ \ \_\ \ \_\ \ \_____\ \ \_\\"\_\
     \/_/   \/_____/  \/_/\/_/  \/_/  \/_/  \/_____/  \/_/ \/_/
 
 
 CLI utility to monitor your OpenAI API token usage
-
-   â¡ï¸NEW: tokmon_beam - a self-hosted web UI to monitor API usage data,
-                            running from localhost.
                                    [License]
 # `tokmon` ð¤ð§ - CLI to monitor OpenAI API usage `tokmon` (**Tok**en
-**Mon**itor) keeps track of your program's OpenAI API token usage. You can use
-`tokmon` just like you would use the `time` utility, but instead of execution
-time you get token usage and cost. ## Installation ``` pip install tokmon ```
-## Usage ```bash $ tokmon /path/to/your/ [arg1] [arg2] ... ``` ```css tokmon
-cost report:
+**Mon**itor) lets you keep track of your program's OpenAI API token usage. You
+can use `tokmon` just like you would use the `time` utility, but instead of
+execution time you get OpenAI usage and cost stats. ## Installation ``` pip
+install tokmon ``` ## Usage > **Note**: tokmon works for `gpt-*` models (`gpt-
+3.5-turbo`, `gpt-4`, etc.). If you need support for other models (e.g.
+`davinci`) see [tokmon#6](https://github.com/yagil/tokmon/issues/6). ```bash $
+tokmon /path/to/your/ [arg1] [arg2] ... ``` ```css tokmon cost report:
 ================================================================================
 Monitored invocation: python3 ./tests/python_example.py --prompt say 'hello,
 tokmon!' Models: ['gpt-3.5-turbo-0301'] Total Usage: {'total_prompt_tokens':
 26, 'total_completion_tokens': 12, 'total_tokens': 38} Pricing: {'gpt-3.5-
 turbo-0301': {'prompt_cost': 0.002, 'completion_cost': 0.002, 'per_tokens':
 1000}} Total Cost: $0.000076
 ================================================================================
@@ -49,28 +55,31 @@
 format.
 ===============================================================================
 ## Use `tokmon` with your application or script > **Warning** > This is a
 debugging tool. It is not intended to be used in any consequential setting. Use
 your best judgement! Prepend `tokmon` to your normal program invocation like
 so: ```bash $ tokmon /path/to/your/ [arg1] [arg2] ... ``` Run and use your
 program just like you would normally (arguments and all). Interactive usage is
-supported as well. #### Using `tokmon` with `npm run` (e.g. with NextJS) Edit
-your `package.json`'s "scripts" entry to include `tokmon`. ```js { "scripts":
-{ "dev": "tokmon next dev", ... } } ``` ## Full usage and cost summary (JSON)
-```json { "total_cost": 0.0019199999999999998, "total_usage":
-{ "total_prompt_tokens": 18, "total_completion_tokens": 23, "total_tokens": 41
-}, "pricing_data": "{'gpt-4-0314': {'prompt_cost': 0.03, 'completion_cost':
-0.06, 'per_tokens': 1000}}", "models": [ "gpt-4-0314" ], "raw_data": [
-{ "model": "gpt-4-0314", "usage": { "prompt_tokens": 18, "completion_tokens":
-23, "total_tokens": 41 }, "cost": 0.0019199999999999998, "messages": [
-{ "role": "system", "content": "You're a helpful assistant." }, { "role":
-"user", "content": "hello" }, { "role": "assistant", "content": "Hello! How can
-I help you today? If you have any questions or need assistance, feel free to
-ask." } ] } ] } ``` ## How it works `tokmon` uses the [mitmproxy library]
-(https://github.com/mitmproxy/mitmproxy) to intercept HTTP requests and
+supported as well. ## Python Simply add `tokmon` to the beginning of your
+regular invocation ```bash $ tokmon python /path/to/your/script.py ``` This
+will work for scripts and long running programs like Django / Flask / FastAPI
+servers. ## Node For scripts: ```bash $ tokmon node /path/to/your/script.js ```
+### `npm run` Edit your `package.json`'s "scripts" entry to include `tokmon`.
+```js { "scripts": { "dev": "tokmon next dev", ... } } ``` ## Full usage and
+cost summary (JSON) ```json { "total_cost": 0.0019199999999999998,
+"total_usage": { "total_prompt_tokens": 18, "total_completion_tokens": 23,
+"total_tokens": 41 }, "pricing_data": "{'gpt-4-0314': {'prompt_cost': 0.03,
+'completion_cost': 0.06, 'per_tokens': 1000}}", "models": [ "gpt-4-0314" ],
+"raw_data": [ { "model": "gpt-4-0314", "usage": { "prompt_tokens": 18,
+"completion_tokens": 23, "total_tokens": 41 }, "cost": 0.0019199999999999998,
+"messages": [ { "role": "system", "content": "You're a helpful assistant." },
+{ "role": "user", "content": "hello" }, { "role": "assistant", "content":
+"Hello! How can I help you today? If you have any questions or need assistance,
+feel free to ask." } ] } ] } ``` ## How it works `tokmon` uses the [mitmproxy
+library](https://github.com/mitmproxy/mitmproxy) to intercept HTTP requests and
 responses between your program and the OpenAI API. It then processes the
 request and response data to calculate token usage and cost based on [tokmon/
 openai-pricing.json](tokmon/openai-pricing.json). > `tokmon` works for programs
 in `python` / `node` (using OpenAI's clients), or `curl` (run directly, and not
 i.e. in a bash script). > See [Golang instructions](#golang) for instructions
 on how to use `tokmon` with Golang programs. > if you [manually install
 `mitmproxy`'s CA certificate](https://docs.mitmproxy.org/stable/concepts-
@@ -102,23 +111,25 @@
 to/your/custom-openai-pricing.json ...` > This pricing JSON is incomplete
 (missing DALL-E, etc.), it may be incorrect, and it may go out of date. > For
 best results, make sure to check that you have the latest pricing. ## Misc ###
 Golang Hacky workaround for Golang programs. Add this to your program: ```go /
 / Import these packages import ( "os" "crypto/tls" "crypto/x509" "io/ioutil"
 "net/http" ) // Place this code somewhere in your go program *before* you make
 any calls to OpenAI's API. certFile := os.Getenv("TOKMON_SSL_CERT_FILE") /
-/ This env variable is set by tokmon whenever it runs your program. caCert, err
-:= ioutil.ReadFile(certFile) if err == nil { caCertPool, _ :
-= x509.SystemCertPool() caCertPool.AppendCertsFromPEM(caCert)
-http.DefaultTransport.(*http.Transport).TLSClientConfig = &tls.Config{ RootCAs:
-caCertPool, } } ``` ## Current Limitations 1. Event streaming: `tokmon` buffers
-Server-Sent Events (SSE) until the `data: [DONE]` chunk is received. If the
-monitored program leverages event streaming, its behavior will be modified. -
-Issue: [yagil/tokmon#4](https://github.com/yagil/tokmon/issues/4) 2 ##
-Contributing If you'd like to contribute to the project, please follow these
-steps: 1. Fork the repository. 2. Create a new branch for your changes. 3. Make
-your changes and test them. 4. Submit a pull request with a clear description
-of your changes and any relevant information. ## Warning 1. `tokmon` comes
-without any warranty or guarantee whatsoever. 2. `tokmon` was tested on macOS
-only. It might not work on other platforms. 3. This tool may not work as
-intended, have unknown side effects, may output incorrect information, or not
-work at all. 4. The pricing data in `openai-pricing.json` may go out of date.
+/ This env variable will be set by tokmon caCert, err := ioutil.ReadFile
+(certFile) if err == nil { caCertPool, _ := x509.SystemCertPool()
+caCertPool.AppendCertsFromPEM(caCert) http.DefaultTransport.
+(*http.Transport).TLSClientConfig = &tls.Config{ RootCAs: caCertPool, } } ```
+## Current Limitations 1. Event streaming: `tokmon` buffers Server-Sent Events
+(SSE) until the `data: [DONE]` chunk is received. If the monitored program
+leverages event streaming, its behavior will be modified. - Issue: [tokmon#4]
+(https://github.com/yagil/tokmon/issues/4) 2. Only chat models are supported
+(`gpt-3.5-turbo`, `gpt-4` and variants) - Issue: [tokmon#6](https://github.com/
+yagil/tokmon/issues/6) ## Contributing If you'd like to contribute to the
+project, please follow these steps: 1. Fork the repository. 2. Create a new
+branch for your changes. 3. Make your changes and test them. 4. Submit a pull
+request with a clear description of your changes and any relevant information.
+## Warning 1. `tokmon` comes without any warranty or guarantee whatsoever. 2.
+`tokmon` was tested on macOS only. It might not work on other platforms. 3.
+This tool may not work as intended, have unknown side effects, may output
+incorrect information, or not work at all. 4. The pricing data in `openai-
+pricing.json` may go out of date.
```

### Comparing `tokmon-0.2.0/setup.py` & `tokmon-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the contents of the README.md file
 with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='tokmon',
-    version='0.2.0',
+    version='0.2.1',
     packages=find_packages(),
     install_requires=[
         'mitmproxy',
         'tiktoken',
     ],
     package_data={
         "tokmon": ["openai-pricing.json"],
```

### Comparing `tokmon-0.2.0/tokmon/beam.py` & `tokmon-0.2.1/tokmon/beam.py`

 * *Files identical despite different names*

### Comparing `tokmon-0.2.0/tokmon/cli.py` & `tokmon-0.2.1/tokmon/cli.py`

 * *Files identical despite different names*

### Comparing `tokmon-0.2.0/tokmon/costcalculator.py` & `tokmon-0.2.1/tokmon/costcalculator.py`

 * *Files identical despite different names*

### Comparing `tokmon-0.2.0/tokmon/openai-pricing.json` & `tokmon-0.2.1/tokmon/openai-pricing.json`

 * *Files identical despite different names*

### Comparing `tokmon-0.2.0/tokmon/tokmon.py` & `tokmon-0.2.1/tokmon/tokmon.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,19 @@
                 model = response_data["model"]
                 content = response_data["choices"][0]["message"]["content"]
                 usage = response_data["usage"]
         else:
             raise Exception("No response data")
         
         request = self.current_request
+        
+        # The messages are sent to OpenAI in the order that it makes sense for the LLM to read them
+        # But we want to display them in the order that they were sent by the user (i.e., the reversed order)
+        request["messages"] = [x for x in reversed(request["messages"])]
+
         response = {
             "model": model,
             "messages": [{"role": "assistant", "content": content}],
             "usage": usage
         }
 
         # Add the request and response to the rolling history
```

### Comparing `tokmon-0.2.0/tokmon/utils.py` & `tokmon-0.2.1/tokmon/utils.py`

 * *Files identical despite different names*

### Comparing `tokmon-0.2.0/tokmon.egg-info/PKG-INFO` & `tokmon-0.2.1/tokmon.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 Metadata-Version: 2.1
 Name: tokmon
-Version: 0.2.0
+Version: 0.2.1
 Summary: tokmon is a CLI utility to monitor OpenAI token usage and costs
 Home-page: https://github.com/yagil/tokmon
 Project-URL: Bug Reports, https://github.com/yagil/tokmon/issues
 Project-URL: Source, https://github.com/yagil/tokmon/
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+<h4 align="center">⚡️<i><b>NEW</b></i>: <a href="https://github.com/yagil/tokmon-beam"> tokmon beam </a> - a self-hosted web UI to monitor API usage data, running from <code>localhost</code>.</h4>
+
 <pre align="center">
 
  ______   ______    __  __    __    __    ______    __   __    
 /\__  _\ /\  __ \  /\ \/ /   /\ "-./  \  /\  __ \  /\ "-.\ \   
 \/_/\ \/ \ \ \/\ \ \ \  _"-. \ \ \-./\ \ \ \ \/\ \ \ \ \-.  \  
    \ \_\  \ \_____\ \ \_\ \_\ \ \_\ \ \_\ \ \_____\ \ \_\\"\_\ 
     \/_/   \/_____/  \/_/\/_/  \/_/  \/_/  \/_____/  \/_/ \/_/ 
                                                                    
 
 CLI utility to monitor your OpenAI API token usage
-                                                                   
-</pre>
 
-<p align="center">⚡️<i><b>NEW</b></i>: <a href="https://github.com/yagil/tokmon-beam"> tokmon beam </a> - a self-hosted web UI to monitor API usage data, running from <code>localhost</code>.</p>
+</pre>
 
 <p align="center">
   <a href="https://github.com/yagil/tokmon/blob/main/LICENSE" target="_blank">
       <img src="https://img.shields.io/badge/License-Apache2.0-orange.svg" alt="License">
   </a>
 </p>
 
 # `tokmon` 🔤🧐 - CLI to monitor OpenAI API usage
 
-`tokmon` (**Tok**en **Mon**itor) keeps track of your program's OpenAI API token usage.
+`tokmon` (**Tok**en **Mon**itor) lets you keep track of your program's OpenAI API token usage.
 
-You can use `tokmon` just like you would use the `time` utility, but instead of execution time you get token usage and cost.
+You can use `tokmon` just like you would use the `time` utility, but instead of execution time you get OpenAI usage and cost stats.
 
 ## Installation
 ```
 pip install tokmon
 ```
 ## Usage
+> **Note**:  tokmon works for `gpt-*` models (`gpt-3.5-turbo`, `gpt-4`, etc.). If you need support for other models (e.g. `davinci`) see [tokmon#6](https://github.com/yagil/tokmon/issues/6).
 ```bash
 $ tokmon /path/to/your/<your program> [arg1] [arg2] ...
 ```
 
 ```css
 tokmon cost report:
 ================================================================================
@@ -95,15 +96,28 @@
 
 Prepend `tokmon` to your normal program invocation like so:
 ```bash
 $ tokmon /path/to/your/<your program> [arg1] [arg2] ...
 ```
 Run and use your program just like you would normally (arguments and all). Interactive usage is supported as well.
 
-#### Using `tokmon` with `npm run` (e.g. with NextJS)
+## Python
+Simply add `tokmon` to the beginning of your regular invocation
+```bash
+$ tokmon python /path/to/your/script.py
+```
+This will work for scripts and long running programs like Django / Flask / FastAPI servers.
+
+## Node
+For scripts:
+```bash
+$ tokmon node /path/to/your/script.js
+```
+
+### `npm run`
 Edit your `package.json`'s "scripts" entry to include `tokmon`. 
 
 ```js
 {
     "scripts": {
         "dev": "tokmon next dev",
         ...
@@ -197,39 +211,41 @@
 > For best results, make sure to check that you have the latest pricing.
 
 ## Misc
 
 ### Golang
 Hacky workaround for Golang programs. Add this to your program:
 ```go
-	// Import these packages
-	import (
-		"os"
-	    "crypto/tls"
-    	"crypto/x509"
-    	"io/ioutil"
-    	"net/http"
-    )
-
-	// Place this code somewhere in your go program *before* you make any calls to OpenAI's API.
-	certFile := os.Getenv("TOKMON_SSL_CERT_FILE") // This env variable is set by tokmon whenever it runs your program.
-	caCert, err := ioutil.ReadFile(certFile)
-	if err == nil { 
-		caCertPool, _ := x509.SystemCertPool()
-		caCertPool.AppendCertsFromPEM(caCert)
-		http.DefaultTransport.(*http.Transport).TLSClientConfig = &tls.Config{
-			RootCAs: caCertPool,
-		}
+// Import these packages
+import (
+	"os"
+	"crypto/tls"
+	"crypto/x509"
+	"io/ioutil"
+	"net/http"
+)
+
+// Place this code somewhere in your go program *before* you make any calls to OpenAI's API.
+certFile := os.Getenv("TOKMON_SSL_CERT_FILE") // This env variable will be set by tokmon
+caCert, err := ioutil.ReadFile(certFile)
+if err == nil { 
+	caCertPool, _ := x509.SystemCertPool()
+	caCertPool.AppendCertsFromPEM(caCert)
+	http.DefaultTransport.(*http.Transport).TLSClientConfig = &tls.Config{
+		RootCAs: caCertPool,
 	}
+}
 ```
 
 ## Current Limitations
 1. Event streaming: `tokmon` buffers Server-Sent Events (SSE) until the `data: [DONE]` chunk is received. If the monitored program leverages event streaming, its behavior will be modified.
-    - Issue: [yagil/tokmon#4](https://github.com/yagil/tokmon/issues/4)
-2
+    - Issue: [tokmon#4](https://github.com/yagil/tokmon/issues/4)
+2. Only chat models are supported (`gpt-3.5-turbo`, `gpt-4` and variants)
+    - Issue: [tokmon#6](https://github.com/yagil/tokmon/issues/6)
+
 ## Contributing
 If you'd like to contribute to the project, please follow these steps:
 1. Fork the repository.
 2. Create a new branch for your changes.
 3. Make your changes and test them.
 4. Submit a pull request with a clear description of your changes and any relevant information.
```

#### html2text {}

```diff
@@ -1,31 +1,32 @@
-Metadata-Version: 2.1 Name: tokmon Version: 0.2.0 Summary: tokmon is a CLI
+Metadata-Version: 2.1 Name: tokmon Version: 0.2.1 Summary: tokmon is a CLI
 utility to monitor OpenAI token usage and costs Home-page: https://github.com/
 yagil/tokmon Project-URL: Bug Reports, https://github.com/yagil/tokmon/issues
 Project-URL: Source, https://github.com/yagil/tokmon/ Description-Content-Type:
 text/markdown License-File: LICENSE
+ *** â¡ï¸NEW: tokmon_beam - a self-hosted web UI to monitor API usage data,
+                          running from localhost. ***
 
  ______   ______    __  __    __    __    ______    __   __
 /\__  _\ /\  __ \  /\ \/ /   /\ "-./  \  /\  __ \  /\ "-.\ \
 \/_/\ \/ \ \ \/\ \ \ \  _"-. \ \ \-./\ \ \ \ \/\ \ \ \ \-.  \
    \ \_\  \ \_____\ \ \_\ \_\ \ \_\ \ \_\ \ \_____\ \ \_\\"\_\
     \/_/   \/_____/  \/_/\/_/  \/_/  \/_/  \/_____/  \/_/ \/_/
 
 
 CLI utility to monitor your OpenAI API token usage
-
-   â¡ï¸NEW: tokmon_beam - a self-hosted web UI to monitor API usage data,
-                            running from localhost.
                                    [License]
 # `tokmon` ð¤ð§ - CLI to monitor OpenAI API usage `tokmon` (**Tok**en
-**Mon**itor) keeps track of your program's OpenAI API token usage. You can use
-`tokmon` just like you would use the `time` utility, but instead of execution
-time you get token usage and cost. ## Installation ``` pip install tokmon ```
-## Usage ```bash $ tokmon /path/to/your/ [arg1] [arg2] ... ``` ```css tokmon
-cost report:
+**Mon**itor) lets you keep track of your program's OpenAI API token usage. You
+can use `tokmon` just like you would use the `time` utility, but instead of
+execution time you get OpenAI usage and cost stats. ## Installation ``` pip
+install tokmon ``` ## Usage > **Note**: tokmon works for `gpt-*` models (`gpt-
+3.5-turbo`, `gpt-4`, etc.). If you need support for other models (e.g.
+`davinci`) see [tokmon#6](https://github.com/yagil/tokmon/issues/6). ```bash $
+tokmon /path/to/your/ [arg1] [arg2] ... ``` ```css tokmon cost report:
 ================================================================================
 Monitored invocation: python3 ./tests/python_example.py --prompt say 'hello,
 tokmon!' Models: ['gpt-3.5-turbo-0301'] Total Usage: {'total_prompt_tokens':
 26, 'total_completion_tokens': 12, 'total_tokens': 38} Pricing: {'gpt-3.5-
 turbo-0301': {'prompt_cost': 0.002, 'completion_cost': 0.002, 'per_tokens':
 1000}} Total Cost: $0.000076
 ================================================================================
@@ -54,28 +55,31 @@
 format.
 ===============================================================================
 ## Use `tokmon` with your application or script > **Warning** > This is a
 debugging tool. It is not intended to be used in any consequential setting. Use
 your best judgement! Prepend `tokmon` to your normal program invocation like
 so: ```bash $ tokmon /path/to/your/ [arg1] [arg2] ... ``` Run and use your
 program just like you would normally (arguments and all). Interactive usage is
-supported as well. #### Using `tokmon` with `npm run` (e.g. with NextJS) Edit
-your `package.json`'s "scripts" entry to include `tokmon`. ```js { "scripts":
-{ "dev": "tokmon next dev", ... } } ``` ## Full usage and cost summary (JSON)
-```json { "total_cost": 0.0019199999999999998, "total_usage":
-{ "total_prompt_tokens": 18, "total_completion_tokens": 23, "total_tokens": 41
-}, "pricing_data": "{'gpt-4-0314': {'prompt_cost': 0.03, 'completion_cost':
-0.06, 'per_tokens': 1000}}", "models": [ "gpt-4-0314" ], "raw_data": [
-{ "model": "gpt-4-0314", "usage": { "prompt_tokens": 18, "completion_tokens":
-23, "total_tokens": 41 }, "cost": 0.0019199999999999998, "messages": [
-{ "role": "system", "content": "You're a helpful assistant." }, { "role":
-"user", "content": "hello" }, { "role": "assistant", "content": "Hello! How can
-I help you today? If you have any questions or need assistance, feel free to
-ask." } ] } ] } ``` ## How it works `tokmon` uses the [mitmproxy library]
-(https://github.com/mitmproxy/mitmproxy) to intercept HTTP requests and
+supported as well. ## Python Simply add `tokmon` to the beginning of your
+regular invocation ```bash $ tokmon python /path/to/your/script.py ``` This
+will work for scripts and long running programs like Django / Flask / FastAPI
+servers. ## Node For scripts: ```bash $ tokmon node /path/to/your/script.js ```
+### `npm run` Edit your `package.json`'s "scripts" entry to include `tokmon`.
+```js { "scripts": { "dev": "tokmon next dev", ... } } ``` ## Full usage and
+cost summary (JSON) ```json { "total_cost": 0.0019199999999999998,
+"total_usage": { "total_prompt_tokens": 18, "total_completion_tokens": 23,
+"total_tokens": 41 }, "pricing_data": "{'gpt-4-0314': {'prompt_cost': 0.03,
+'completion_cost': 0.06, 'per_tokens': 1000}}", "models": [ "gpt-4-0314" ],
+"raw_data": [ { "model": "gpt-4-0314", "usage": { "prompt_tokens": 18,
+"completion_tokens": 23, "total_tokens": 41 }, "cost": 0.0019199999999999998,
+"messages": [ { "role": "system", "content": "You're a helpful assistant." },
+{ "role": "user", "content": "hello" }, { "role": "assistant", "content":
+"Hello! How can I help you today? If you have any questions or need assistance,
+feel free to ask." } ] } ] } ``` ## How it works `tokmon` uses the [mitmproxy
+library](https://github.com/mitmproxy/mitmproxy) to intercept HTTP requests and
 responses between your program and the OpenAI API. It then processes the
 request and response data to calculate token usage and cost based on [tokmon/
 openai-pricing.json](tokmon/openai-pricing.json). > `tokmon` works for programs
 in `python` / `node` (using OpenAI's clients), or `curl` (run directly, and not
 i.e. in a bash script). > See [Golang instructions](#golang) for instructions
 on how to use `tokmon` with Golang programs. > if you [manually install
 `mitmproxy`'s CA certificate](https://docs.mitmproxy.org/stable/concepts-
@@ -107,23 +111,25 @@
 to/your/custom-openai-pricing.json ...` > This pricing JSON is incomplete
 (missing DALL-E, etc.), it may be incorrect, and it may go out of date. > For
 best results, make sure to check that you have the latest pricing. ## Misc ###
 Golang Hacky workaround for Golang programs. Add this to your program: ```go /
 / Import these packages import ( "os" "crypto/tls" "crypto/x509" "io/ioutil"
 "net/http" ) // Place this code somewhere in your go program *before* you make
 any calls to OpenAI's API. certFile := os.Getenv("TOKMON_SSL_CERT_FILE") /
-/ This env variable is set by tokmon whenever it runs your program. caCert, err
-:= ioutil.ReadFile(certFile) if err == nil { caCertPool, _ :
-= x509.SystemCertPool() caCertPool.AppendCertsFromPEM(caCert)
-http.DefaultTransport.(*http.Transport).TLSClientConfig = &tls.Config{ RootCAs:
-caCertPool, } } ``` ## Current Limitations 1. Event streaming: `tokmon` buffers
-Server-Sent Events (SSE) until the `data: [DONE]` chunk is received. If the
-monitored program leverages event streaming, its behavior will be modified. -
-Issue: [yagil/tokmon#4](https://github.com/yagil/tokmon/issues/4) 2 ##
-Contributing If you'd like to contribute to the project, please follow these
-steps: 1. Fork the repository. 2. Create a new branch for your changes. 3. Make
-your changes and test them. 4. Submit a pull request with a clear description
-of your changes and any relevant information. ## Warning 1. `tokmon` comes
-without any warranty or guarantee whatsoever. 2. `tokmon` was tested on macOS
-only. It might not work on other platforms. 3. This tool may not work as
-intended, have unknown side effects, may output incorrect information, or not
-work at all. 4. The pricing data in `openai-pricing.json` may go out of date.
+/ This env variable will be set by tokmon caCert, err := ioutil.ReadFile
+(certFile) if err == nil { caCertPool, _ := x509.SystemCertPool()
+caCertPool.AppendCertsFromPEM(caCert) http.DefaultTransport.
+(*http.Transport).TLSClientConfig = &tls.Config{ RootCAs: caCertPool, } } ```
+## Current Limitations 1. Event streaming: `tokmon` buffers Server-Sent Events
+(SSE) until the `data: [DONE]` chunk is received. If the monitored program
+leverages event streaming, its behavior will be modified. - Issue: [tokmon#4]
+(https://github.com/yagil/tokmon/issues/4) 2. Only chat models are supported
+(`gpt-3.5-turbo`, `gpt-4` and variants) - Issue: [tokmon#6](https://github.com/
+yagil/tokmon/issues/6) ## Contributing If you'd like to contribute to the
+project, please follow these steps: 1. Fork the repository. 2. Create a new
+branch for your changes. 3. Make your changes and test them. 4. Submit a pull
+request with a clear description of your changes and any relevant information.
+## Warning 1. `tokmon` comes without any warranty or guarantee whatsoever. 2.
+`tokmon` was tested on macOS only. It might not work on other platforms. 3.
+This tool may not work as intended, have unknown side effects, may output
+incorrect information, or not work at all. 4. The pricing data in `openai-
+pricing.json` may go out of date.
```

