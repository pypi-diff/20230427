# Comparing `tmp/waveforms-1.5.90.tar.gz` & `tmp/waveforms-1.5.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waveforms-1.5.90.tar", last modified: Fri Apr 21 06:23:24 2023, max compression
+gzip compressed data, was "waveforms-1.5.92.tar", last modified: Thu Apr 27 16:46:14 2023, max compression
```

## Comparing `waveforms-1.5.90.tar` & `waveforms-1.5.92.tar`

### file list

```diff
@@ -1,199 +1,202 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.931371 waveforms-1.5.90/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-21 06:22:27.000000 waveforms-1.5.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-21 06:22:27.000000 waveforms-1.5.90/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-21 06:23:24.931371 waveforms-1.5.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-21 06:22:27.000000 waveforms-1.5.90/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-21 06:22:27.000000 waveforms-1.5.90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 06:23:24.931371 waveforms-1.5.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-21 06:22:27.000000 waveforms-1.5.90/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.915371 waveforms-1.5.90/src/
--rw-r--r--   0 runner    (1001) docker     (123)    32248 2023-04-21 06:22:27.000000 waveforms-1.5.90/src/ikcp.c
--rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-04-21 06:22:27.000000 waveforms-1.5.90/src/ikcp.h
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-21 06:22:27.000000 waveforms-1.5.90/src/kcp.c
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-21 06:22:27.000000 waveforms-1.5.90/src/prime.c
--rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-21 06:22:27.000000 waveforms-1.5.90/src/waveform.c
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-21 06:22:27.000000 waveforms-1.5.90/src/waveform.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.919371 waveforms-1.5.90/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-21 06:22:27.000000 waveforms-1.5.90/tests/test_clifford.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-21 06:22:27.000000 waveforms-1.5.90/tests/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-21 06:22:27.000000 waveforms-1.5.90/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-21 06:22:27.000000 waveforms-1.5.90/tests/test_dicttree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-21 06:22:27.000000 waveforms-1.5.90/tests/test_lisp.py
--rw-r--r--   0 runner    (1001) docker     (123)    32676 2023-04-21 06:22:27.000000 waveforms-1.5.90/tests/test_msgpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-21 06:22:27.000000 waveforms-1.5.90/tests/test_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-21 06:22:27.000000 waveforms-1.5.90/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-04-21 06:22:27.000000 waveforms-1.5.90/tests/test_scan_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-21 06:22:27.000000 waveforms-1.5.90/tests/test_tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-21 06:22:27.000000 waveforms-1.5.90/tests/test_verify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-21 06:22:27.000000 waveforms-1.5.90/tests/test_vm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-21 06:22:27.000000 waveforms-1.5.90/tests/test_waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.919371 waveforms-1.5.90/waveforms/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/baseconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/dicttree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.919371 waveforms-1.5.90/waveforms/math/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/math/bayes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/math/fibheap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.919371 waveforms-1.5.90/waveforms/math/fit/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/math/fit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/math/fit/_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/math/fit/delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/math/fit/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/math/fit/qubit_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/math/fit/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/math/fit/resonator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/math/fit/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/math/fit/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/math/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/math/prime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.923371 waveforms-1.5.90/waveforms/math/signal/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/math/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/math/signal/demodulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/math/signal/distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/math/signal/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/math/transmon.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.923371 waveforms-1.5.90/waveforms/qlisp/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.923371 waveforms-1.5.90/waveforms/qlisp/arch/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/arch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/library.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.923371 waveforms-1.5.90/waveforms/qlisp/libs/
--rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/macro.py
--rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/prog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.923371 waveforms-1.5.90/waveforms/qlisp/qasm/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.923371 waveforms-1.5.90/waveforms/qlisp/qasm/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/libs/qelib1.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.927371 waveforms-1.5.90/waveforms/qlisp/qasm/node/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/barrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/binaryop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/binaryoperator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/creg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/customunitary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/expressionlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/external.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/gatebody.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/idlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/if_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/indexedid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/intnode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/nodeexception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/opaque.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/primarylist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/qreg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/real.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/node/unaryoperator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/qasm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/qasmlexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/qasm/qasmparser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.927371 waveforms-1.5.90/waveforms/qlisp/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/simulator/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9743 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/simulator/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/qlisp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.927371 waveforms-1.5.90/waveforms/quantum/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.927371 waveforms-1.5.90/waveforms/quantum/circuit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/circuit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.927371 waveforms-1.5.90/waveforms/quantum/circuit/qlisp/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/circuit/qlisp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.927371 waveforms-1.5.90/waveforms/quantum/circuit/qlisp/arch/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/circuit/qlisp/arch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/circuit/qlisp/arch/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/circuit/qlisp/assembly_left.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/circuit/qlisp/assembly_right.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/circuit/qlisp/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/circuit/qlisp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/circuit/qlisp/library.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/circuit/qlisp/macro.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/circuit/qlisp/qasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/circuit/qlisp/qlisp.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/circuit/qlisp/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/circuit/qlisp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.927371 waveforms-1.5.90/waveforms/quantum/circuit/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/circuit/simulator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.927371 waveforms-1.5.90/waveforms/quantum/clifford/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/clifford/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/clifford/clifford.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/clifford/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/clifford/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/clifford/seq2mat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/rb.py
--rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/tomo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/transmon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/quantum/xeb.py
--rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    23839 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/scan_iter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.927371 waveforms-1.5.90/waveforms/security/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/security/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.927371 waveforms-1.5.90/waveforms/server/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32530 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/server/umsgpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.931371 waveforms-1.5.90/waveforms/sys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/sys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/sys/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.931371 waveforms-1.5.90/waveforms/sys/device/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/sys/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/sys/device/basedevice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/sys/device/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/sys/device/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.931371 waveforms-1.5.90/waveforms/sys/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/sys/drivers/FakeInstrument.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/sys/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/sys/ipy_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.931371 waveforms-1.5.90/waveforms/sys/net/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/sys/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23509 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/sys/net/dhcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/sys/net/dhcpd.py
--rw-r--r--   0 runner    (1001) docker     (123)    38172 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/sys/net/kad.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/sys/net/kcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/sys/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.931371 waveforms-1.5.90/waveforms/sys/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/sys/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/sys/storage/crud.py
--rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/sys/storage/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.931371 waveforms-1.5.90/waveforms/units/
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.931371 waveforms-1.5.90/waveforms/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/visualization/plot_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/visualization/plot_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)    35656 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/waveform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-04-21 06:22:27.000000 waveforms-1.5.90/waveforms/waveform_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 06:23:24.919371 waveforms-1.5.90/waveforms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-21 06:23:24.000000 waveforms-1.5.90/waveforms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-04-21 06:23:24.000000 waveforms-1.5.90/waveforms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 06:23:24.000000 waveforms-1.5.90/waveforms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 06:23:24.000000 waveforms-1.5.90/waveforms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-21 06:23:24.000000 waveforms-1.5.90/waveforms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 06:23:24.000000 waveforms-1.5.90/waveforms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.634696 waveforms-1.5.92/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-27 16:45:12.000000 waveforms-1.5.92/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-27 16:45:12.000000 waveforms-1.5.92/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-27 16:46:14.634696 waveforms-1.5.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-27 16:45:12.000000 waveforms-1.5.92/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-27 16:45:12.000000 waveforms-1.5.92/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 16:46:14.634696 waveforms-1.5.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-27 16:45:12.000000 waveforms-1.5.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.622695 waveforms-1.5.92/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    32248 2023-04-27 16:45:12.000000 waveforms-1.5.92/src/ikcp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12165 2023-04-27 16:45:12.000000 waveforms-1.5.92/src/ikcp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-27 16:45:12.000000 waveforms-1.5.92/src/kcp.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-27 16:45:12.000000 waveforms-1.5.92/src/prime.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-27 16:45:12.000000 waveforms-1.5.92/src/waveform.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-27 16:45:12.000000 waveforms-1.5.92/src/waveform.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.622695 waveforms-1.5.92/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-27 16:45:12.000000 waveforms-1.5.92/tests/test_clifford.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-27 16:45:12.000000 waveforms-1.5.92/tests/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-27 16:45:12.000000 waveforms-1.5.92/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-04-27 16:45:12.000000 waveforms-1.5.92/tests/test_dicttree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-27 16:45:12.000000 waveforms-1.5.92/tests/test_lisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32676 2023-04-27 16:45:12.000000 waveforms-1.5.92/tests/test_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-27 16:45:12.000000 waveforms-1.5.92/tests/test_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-27 16:45:12.000000 waveforms-1.5.92/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-04-27 16:45:12.000000 waveforms-1.5.92/tests/test_scan_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-27 16:45:12.000000 waveforms-1.5.92/tests/test_tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-27 16:45:12.000000 waveforms-1.5.92/tests/test_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-27 16:45:12.000000 waveforms-1.5.92/tests/test_vm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-27 16:45:12.000000 waveforms-1.5.92/tests/test_waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.622695 waveforms-1.5.92/waveforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/baseconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/dicttree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.626695 waveforms-1.5.92/waveforms/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/bayes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/fibheap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.626695 waveforms-1.5.92/waveforms/math/fit/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/fit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/fit/_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/fit/delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/fit/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/fit/qubit_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/fit/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/fit/resonator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/fit/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/fit/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.626695 waveforms-1.5.92/waveforms/math/group/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/group/_SU_n_.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7131 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/prime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.626695 waveforms-1.5.92/waveforms/math/signal/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/signal/demodulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/signal/distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/signal/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/math/transmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.626695 waveforms-1.5.92/waveforms/qlisp/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.626695 waveforms-1.5.92/waveforms/qlisp/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/library.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.626695 waveforms-1.5.92/waveforms/qlisp/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/macro.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16227 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/prog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.626695 waveforms-1.5.92/waveforms/qlisp/qasm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.626695 waveforms-1.5.92/waveforms/qlisp/qasm/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/libs/qelib1.inc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.630695 waveforms-1.5.92/waveforms/qlisp/qasm/node/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/binaryop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/binaryoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/creg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/customunitary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/expressionlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/gatebody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/idlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/if_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/indexedid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/intnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/nodeexception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/opaque.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/primarylist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/qreg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/node/unaryoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/qasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/qasmlexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/qasm/qasmparser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.630695 waveforms-1.5.92/waveforms/qlisp/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/simulator/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10003 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/simulator/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/qlisp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.630695 waveforms-1.5.92/waveforms/quantum/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.630695 waveforms-1.5.92/waveforms/quantum/circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/circuit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.630695 waveforms-1.5.92/waveforms/quantum/circuit/qlisp/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/circuit/qlisp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.630695 waveforms-1.5.92/waveforms/quantum/circuit/qlisp/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/circuit/qlisp/arch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/circuit/qlisp/arch/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/circuit/qlisp/assembly_left.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/circuit/qlisp/assembly_right.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/circuit/qlisp/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/circuit/qlisp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/circuit/qlisp/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/circuit/qlisp/macro.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/circuit/qlisp/qasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/circuit/qlisp/qlisp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/circuit/qlisp/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/circuit/qlisp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.634696 waveforms-1.5.92/waveforms/quantum/circuit/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/circuit/simulator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.634696 waveforms-1.5.92/waveforms/quantum/clifford/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/clifford/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/clifford/clifford.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/clifford/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/clifford/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/clifford/seq2mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/rb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/tomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/transmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/quantum/xeb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21432 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26353 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/scan_iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.634696 waveforms-1.5.92/waveforms/security/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/security/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.634696 waveforms-1.5.92/waveforms/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32530 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/server/umsgpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.634696 waveforms-1.5.92/waveforms/sys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/sys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/sys/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.634696 waveforms-1.5.92/waveforms/sys/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/sys/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/sys/device/basedevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/sys/device/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/sys/device/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.634696 waveforms-1.5.92/waveforms/sys/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/sys/drivers/FakeInstrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/sys/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/sys/ipy_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.634696 waveforms-1.5.92/waveforms/sys/net/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/sys/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23509 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/sys/net/dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/sys/net/dhcpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38172 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/sys/net/kad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/sys/net/kcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/sys/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.634696 waveforms-1.5.92/waveforms/sys/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/sys/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/sys/storage/crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/sys/storage/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.634696 waveforms-1.5.92/waveforms/units/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.634696 waveforms-1.5.92/waveforms/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/visualization/plot_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/visualization/plot_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38227 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/waveform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-04-27 16:45:12.000000 waveforms-1.5.92/waveforms/waveform_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 16:46:14.622695 waveforms-1.5.92/waveforms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-27 16:46:14.000000 waveforms-1.5.92/waveforms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-27 16:46:14.000000 waveforms-1.5.92/waveforms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 16:46:14.000000 waveforms-1.5.92/waveforms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 16:46:14.000000 waveforms-1.5.92/waveforms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-27 16:46:14.000000 waveforms-1.5.92/waveforms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 16:46:14.000000 waveforms-1.5.92/waveforms.egg-info/top_level.txt
```

### Comparing `waveforms-1.5.90/LICENSE` & `waveforms-1.5.92/LICENSE`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/PKG-INFO` & `waveforms-1.5.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveforms
-Version: 1.5.90
+Version: 1.5.92
 Summary: Edit waveforms used in experiment
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/feihoo87/waveforms
 Project-URL: Bug Reports, https://github.com/feihoo87/waveforms/issues
 Project-URL: Source, https://github.com/feihoo87/waveforms/
```

### Comparing `waveforms-1.5.90/README.md` & `waveforms-1.5.92/README.md`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/pyproject.toml` & `waveforms-1.5.92/pyproject.toml`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/setup.py` & `waveforms-1.5.92/setup.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/src/ikcp.c` & `waveforms-1.5.92/src/ikcp.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/src/ikcp.h` & `waveforms-1.5.92/src/ikcp.h`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/src/kcp.c` & `waveforms-1.5.92/src/kcp.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/src/prime.c` & `waveforms-1.5.92/src/prime.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/src/waveform.c` & `waveforms-1.5.92/src/waveform.c`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/src/waveform.h` & `waveforms-1.5.92/src/waveform.h`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/tests/test_compile.py` & `waveforms-1.5.92/tests/test_compile.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/tests/test_dicttree.py` & `waveforms-1.5.92/tests/test_dicttree.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/tests/test_lisp.py` & `waveforms-1.5.92/tests/test_lisp.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/tests/test_msgpack.py` & `waveforms-1.5.92/tests/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/tests/test_namespace.py` & `waveforms-1.5.92/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/tests/test_registry.py` & `waveforms-1.5.92/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/tests/test_scan_iter.py` & `waveforms-1.5.92/tests/test_scan_iter.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
         assert data['iq'].shape == (101, 121, 1024)
         assert np.all((z == data['z'])[np.isnan(z) == False])
         assert np.all((iq == data['iq'])[np.isnan(iq) == False])
 
     assert set(data1.keys()) == {'bias', 'freq', 'z', 'iq', 'obj'}
 
     assert set(data2.keys()) == {'bias', 'freq', 'z', 'iq', 'obj', 'center'}
-    assert data2['center'].shape == (101, 121)
+    assert data2['center'].shape == (101, )
 
     for key in ['z', 'iq', 'obj']:
         assert np.allclose(data1.timestamps[key], data2.timestamps[key])
 
 
 def test_storage_future(spectrum_data):
     from concurrent.futures import ThreadPoolExecutor
```

### Comparing `waveforms-1.5.90/tests/test_tomo.py` & `waveforms-1.5.92/tests/test_tomo.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/tests/test_vm.py` & `waveforms-1.5.92/tests/test_vm.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/tests/test_waveform.py` & `waveforms-1.5.92/tests/test_waveform.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/__init__.py` & `waveforms-1.5.92/waveforms/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/autoreload.py` & `waveforms-1.5.92/waveforms/autoreload.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/baseconfig.py` & `waveforms-1.5.92/waveforms/baseconfig.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/cache.py` & `waveforms-1.5.92/waveforms/cache.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/dicttree.py` & `waveforms-1.5.92/waveforms/dicttree.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/loader.py` & `waveforms-1.5.92/waveforms/loader.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/math/bayes.py` & `waveforms-1.5.92/waveforms/math/bayes.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/math/fibheap.py` & `waveforms-1.5.92/waveforms/math/fibheap.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/math/fit/__init__.py` & `waveforms-1.5.92/waveforms/math/fit/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/math/fit/_fit.py` & `waveforms-1.5.92/waveforms/math/fit/_fit.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/math/fit/delay.py` & `waveforms-1.5.92/waveforms/math/fit/delay.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/math/fit/geo.py` & `waveforms-1.5.92/waveforms/math/fit/geo.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/math/fit/qubit_dynamics.py` & `waveforms-1.5.92/waveforms/math/fit/qubit_dynamics.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/math/fit/readout.py` & `waveforms-1.5.92/waveforms/math/fit/readout.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/math/fit/resonator.py` & `waveforms-1.5.92/waveforms/math/fit/resonator.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/math/fit/simple.py` & `waveforms-1.5.92/waveforms/math/fit/simple.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/math/fit/spectrum.py` & `waveforms-1.5.92/waveforms/math/fit/spectrum.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/math/graph.py` & `waveforms-1.5.92/waveforms/math/graph.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/math/prime.py` & `waveforms-1.5.92/waveforms/math/prime.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/math/signal/demodulate.py` & `waveforms-1.5.92/waveforms/math/signal/demodulate.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/math/signal/distortion.py` & `waveforms-1.5.92/waveforms/math/signal/distortion.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/math/signal/func.py` & `waveforms-1.5.92/waveforms/math/signal/func.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/math/transmon.py` & `waveforms-1.5.92/waveforms/math/transmon.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/namespace.py` & `waveforms-1.5.92/waveforms/namespace.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/__init__.py` & `waveforms-1.5.92/waveforms/qlisp/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/arch/__init__.py` & `waveforms-1.5.92/waveforms/qlisp/arch/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/assembly.py` & `waveforms-1.5.92/waveforms/qlisp/assembly.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/base.py` & `waveforms-1.5.92/waveforms/qlisp/base.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/commands.py` & `waveforms-1.5.92/waveforms/qlisp/commands.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/compiler.py` & `waveforms-1.5.92/waveforms/qlisp/compiler.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/config.py` & `waveforms-1.5.92/waveforms/qlisp/config.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/interpreter.py` & `waveforms-1.5.92/waveforms/qlisp/interpreter.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/library.py` & `waveforms-1.5.92/waveforms/qlisp/library.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/libs/__init__.py` & `waveforms-1.5.92/waveforms/qlisp/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/macro.py` & `waveforms-1.5.92/waveforms/qlisp/macro.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/parse.py` & `waveforms-1.5.92/waveforms/qlisp/parse.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/prog.py` & `waveforms-1.5.92/waveforms/qlisp/prog.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/__init__.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/eval.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/eval.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/exceptions.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/exceptions.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/libs/qelib1.inc` & `waveforms-1.5.92/waveforms/qlisp/qasm/libs/qelib1.inc`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/__init__.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/barrier.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/barrier.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/binaryop.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/binaryop.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/binaryoperator.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/binaryoperator.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/creg.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/creg.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/customunitary.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/customunitary.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/expressionlist.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/expressionlist.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/external.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/external.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/format.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/format.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/gate.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/gate.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/gatebody.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/gatebody.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/id.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/id.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/idlist.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/idlist.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/if_.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/if_.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/indexedid.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/indexedid.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/intnode.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/intnode.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/measure.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/measure.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/node.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/node.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/nodeexception.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/nodeexception.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/opaque.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/opaque.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/prefix.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/prefix.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/primarylist.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/primarylist.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/program.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/program.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/qreg.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/qreg.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/real.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/real.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/reset.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/reset.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/node/unaryoperator.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/node/unaryoperator.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/qasm.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/qasm.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/qasmlexer.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/qasmlexer.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/qasm/qasmparser.py` & `waveforms-1.5.92/waveforms/qlisp/qasm/qasmparser.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/simulator/__init__.py` & `waveforms-1.5.92/waveforms/qlisp/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/simulator/mat.py` & `waveforms-1.5.92/waveforms/qlisp/simulator/mat.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/simulator/simple.py` & `waveforms-1.5.92/waveforms/qlisp/simulator/simple.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                 *gate[1:]), __matrix_of_gates[gate[0]][1]
         else:
             raise ValueError(
                 f"Could not call {gate[0]}(*{gate[1:]}), `{gate[0]}` is not callable."
             )
     elif gate_name(gate) == 'C':
         U, N = gate2mat(gate[1])
-        ret = np.eye(2 * U.shape[0], dtype=np.complex)
+        ret = np.eye(2 * U.shape[0], dtype=complex)
         ret[U.shape[0]:, U.shape[0]:] = U
         return ret, N + 1
     else:
         raise ValueError(f'Unexcept gate {gate}')
 
 
 def splite_at(l, bits):
@@ -113,16 +113,18 @@
         raise ValueError(f'Unexcept gate {gate} and qubits {qubits}')
 
 
 def _measure_process(rho):
     return np.array([[rho[0, 0], 0], [0, rho[1, 1]]])
 
 
-def _reset_process(rho):
-    return np.array([[rho[0, 0] + rho[1, 1], 0], [0, 0]])
+def _reset_process(rho, p1):
+    s0 = np.array([[rho[0, 0] + rho[1, 1], 0], [0, 0]])
+    s1 = np.array([[0, 0], [0, rho[0, 0] + rho[1, 1]]])
+    return (1 - p1) * s0 + p1 * s1
 
 
 def _decohherence_process(rho, Gamma_t, gamma_t):
     rho00 = rho[0, 0] + rho[1, 1] * (1 - np.exp(-Gamma_t))
     rho11 = rho[1, 1] * np.exp(-Gamma_t)
     rho01 = rho[0, 1] * np.exp(-Gamma_t / 2 - gamma_t**2)
     rho10 = rho[1, 0] * np.exp(-Gamma_t / 2 - gamma_t**2)
@@ -165,34 +167,39 @@
                     _, t, T1 = gate
                     Gamma_t = t / T1
                     gamma_t = 0
                 else:
                     _, t, T1, Tphi = gate
                     Gamma_t = t / T1
                     gamma_t = t / Tphi
+        if gate_name(gate) in ['Reset']:
+            if isinstance(gate, tuple) and len(gate) == 2:
+                _, p1 = gate
+            else:
+                p1 = 0.0
         if gate_name(gate) in ['Measure', 'Reset', 'Delay'] and psi.ndim == 1:
             psi, unitary_process, psi0 = _set_vector_to_rho(psi)
 
         if gate_name(gate) == 'Measure':
             reduceSubspace(qubits, N, psi, _measure_process, ())
         elif gate_name(gate) == 'Reset':
-            reduceSubspace(qubits, N, psi, _reset_process, ())
+            reduceSubspace(qubits, N, psi, _reset_process, (p1, ))
         elif gate_name(gate) == 'Delay':
             reduceSubspace(qubits, N, psi, _decohherence_process,
                            (Gamma_t, gamma_t))
         else:
             _apply_gate(gate, psi, unitary_process, qubits, N)
 
     return psi
 
 
 def seq2mat(seq, U=None):
-    I = np.eye(2, dtype=np.complex)
+    I = np.eye(2, dtype=complex)
     if U is None:
-        U = np.eye(2, dtype=np.complex)
+        U = np.eye(2, dtype=complex)
         N = 1
     else:
         N = round(np.log2(U.shape[0]))
 
     unitary_process = lambda U0, U: U @ U0
 
     for gate, *qubits in seq:
```

### Comparing `waveforms-1.5.90/waveforms/qlisp/tokenize.py` & `waveforms-1.5.92/waveforms/qlisp/tokenize.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/qlisp/utils.py` & `waveforms-1.5.92/waveforms/qlisp/utils.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/quantum/clifford/clifford.py` & `waveforms-1.5.92/waveforms/quantum/clifford/clifford.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/quantum/clifford/db.py` & `waveforms-1.5.92/waveforms/quantum/clifford/db.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/quantum/clifford/mat.py` & `waveforms-1.5.92/waveforms/quantum/clifford/mat.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/quantum/clifford/seq2mat.py` & `waveforms-1.5.92/waveforms/quantum/clifford/seq2mat.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/quantum/math.py` & `waveforms-1.5.92/waveforms/quantum/math.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/quantum/rb.py` & `waveforms-1.5.92/waveforms/quantum/rb.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/quantum/tomo.py` & `waveforms-1.5.92/waveforms/quantum/tomo.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/quantum/transmon.py` & `waveforms-1.5.92/waveforms/quantum/transmon.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/quantum/xeb.py` & `waveforms-1.5.92/waveforms/quantum/xeb.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/registry.py` & `waveforms-1.5.92/waveforms/registry.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/scan_iter.py` & `waveforms-1.5.92/waveforms/scan_iter.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,16 @@
 
     def __repr__(self):
         return f'End(level={self.level}, kwds={self.kwds}, vars={self.vars})'
 
 
 class Tracker():
 
-    def init(self, loops: dict):
+    def init(self, loops: dict, functions: dict, constants: dict, graph: dict,
+             order: list):
         pass
 
     def update(self, kwds: dict):
         return kwds
 
     def feed(self, step: StepStatus, obj: Any, **options):
         pass
@@ -322,54 +323,71 @@
 def _find_common_prefix(a: tuple, b: tuple):
     for i, (x, y) in enumerate(zip(a, b)):
         if x != y:
             return i
     return i
 
 
-def _build_dependence(loops, functions, constants):
+def _add_dependence(graph, keys, function, loop_names, var_names):
+    if isinstance(keys, str):
+        keys = (keys, )
+    for key in keys:
+        graph.setdefault(key, set())
+        for k, p in inspect.signature(function).parameters.items():
+            if p.kind in [
+                    p.POSITIONAL_ONLY, p.POSITIONAL_OR_KEYWORD, p.KEYWORD_ONLY
+            ] and k in var_names:
+                graph[key].add(k)
+            if p.kind == p.VAR_KEYWORD and key not in loop_names:
+                graph[key].update(loop_names)
+
+
+def _build_dependence(loops, functions, constants, loop_deps=True):
     graph = {}
     loop_names = set()
     var_names = set()
-    for keys in loops:
+    for keys, iters in loops.items():
         level_vars = set()
         if isinstance(keys, str):
             keys = (keys, )
-        for ks in keys:
+        if callable(iters):
+            iters = tuple([iters for _ in keys])
+        for ks, iter_vars in zip(keys, iters):
             if isinstance(ks, str):
                 ks = (ks, )
+            if callable(iters):
+                iter_vars = tuple([iter_vars for _ in ks])
             level_vars.update(ks)
-            for k in ks:
-                graph.setdefault(k, set()).update(loop_names)
+            for i, k in enumerate(ks):
+                d = graph.setdefault(k, set())
+                if loop_deps:
+                    d.update(loop_names)
+                else:
+                    if isinstance(iter_vars, tuple):
+                        iter_var = iter_vars[i]
+                    else:
+                        iter_var = iter_vars
+                    if callable(iter_var):
+                        d.update(
+                            set(
+                                inspect.signature(iter_vars).parameters.keys())
+                            & loop_names)
+
         loop_names.update(level_vars)
         var_names.update(level_vars)
     var_names.update(functions.keys())
     var_names.update(constants.keys())
 
-    def _add_dependence(keys, value):
-        if isinstance(keys, str):
-            keys = (keys, )
-        for key in keys:
-            graph.setdefault(key, set())
-            for k, p in inspect.signature(value).parameters.items():
-                if p.kind in [
-                        p.POSITIONAL_ONLY, p.POSITIONAL_OR_KEYWORD,
-                        p.KEYWORD_ONLY
-                ] and k in var_names:
-                    graph[key].add(k)
-                if p.kind == p.VAR_KEYWORD and key not in loop_names:
-                    graph[key].update(loop_names)
-
     for keys, values in chain(loops.items(), functions.items()):
         if callable(values):
-            _add_dependence(keys, values)
+            _add_dependence(graph, keys, values, loop_names, var_names)
         elif isinstance(values, tuple):
             for ks, v in zip(keys, values):
                 if callable(v):
-                    _add_dependence(ks, v)
+                    _add_dependence(graph, ks, v, loop_names, var_names)
 
     return graph
 
 
 def _get_all_dependence(key, graph):
     ret = set()
     if key not in graph:
@@ -458,14 +476,15 @@
     order = []
     ts.prepare()
     while ts.is_active():
         ready = ts.get_ready()
         for k in ready:
             ts.done(k)
         order.append(ready)
+    graph = _build_dependence(loops, functions, constants, False)
 
     for tracker in trackers:
         tracker.init(loops, functions, constants, graph, order)
 
     last_step = None
     index = ()
     iteration = count()
@@ -527,16 +546,17 @@
         self.cache = {}
         self.pos = {}
         self.timestamps = {}
         self.iteration = {}
         self._init_keys = list(self.storage.keys())
         self._frozen_keys = frozen_keys
         self._key_levels = ()
-        self._vars_dims = {}
         self.depends = {}
+        self.dims = {}
+        self.vars_dims = {}
         self.shape = shape
         self.count = 0
         self.save_kwds = save_kwds
         self.queue = Queue()
         self._queue_buffer = None
 
     def init(self, loops: dict, functions: dict, constants: dict, graph: dict,
@@ -574,34 +594,52 @@
                     self.storage[key] = iters[:, i]
                     self._frozen_keys = self._frozen_keys + (key, )
                     self._init_keys.append(key)
                 continue
             if not isinstance(iters, tuple) or len(keys) != len(iters):
                 continue
             for key, iter in zip(keys, iters):
-                self._vars_dims[key] = (level, )
+                if self.depends.get(key, set()):
+                    dims = set()
+                    for dep in self.depends[key]:
+                        if dep in self.vars_dims:
+                            dims.update(set(self.vars_dims[dep]))
+                    dims.add(level)
+                    self.vars_dims[key] = tuple(sorted(dims))
+                else:
+                    self.vars_dims[key] = (level, )
+                if level not in self.dims:
+                    self.dims[level] = ()
+                self.dims[level] = self.dims[level] + (key, )
                 if key not in self.storage and isinstance(
                         iter, (list, range, ndarray)):
                     self.storage[key] = iter
                     self._frozen_keys = self._frozen_keys + (key, )
                     self._init_keys.append(key)
 
         for key, value in constants.items():
             self.storage[key] = value
             self._init_keys.append(key)
-            self._vars_dims[key] = ()
+            self.vars_dims[key] = ()
 
         for ready in order:
             for key in ready:
                 if key in functions:
                     deps = _get_all_dependence(key, graph)
                     dims = set()
                     for k in deps:
-                        dims.update(set(self._vars_dims.get(k, ())))
-                    self._vars_dims[key] = tuple(sorted(dims))
+                        dims.update(set(self.vars_dims.get(k, ())))
+                    self.vars_dims[key] = tuple(sorted(dims))
+
+        for k, v in self.vars_dims.items():
+            if len(v) == 1:
+                if v[0] in self.dims and k not in self.dims[v[0]]:
+                    self.dims[v[0]] = self.dims[v[0]] + (k, )
+                elif v[0] not in self.dims:
+                    self.dims[v[0]] = (k, )
 
     def feed(self, step: StepStatus, dataframe: dict, store=False, **options):
         """
         Feed the results of the step to the storage.
 
         Parameters
         ----------
@@ -635,28 +673,40 @@
 
     def _append(self, iteration, pos, dataframe, kwds, now):
         for k, v in chain(kwds.items(), dataframe.items()):
             if k in self._frozen_keys:
                 continue
             if k.startswith('__'):
                 continue
+            if self.vars_dims.get(k, ()) == () and k not in dataframe:
+                continue
             self.count += 1
             if k not in self.storage:
                 self.storage[k] = [v]
-                self.pos[k] = tuple([i] for i in pos)
+                if k in self.vars_dims:
+                    self.pos[k] = tuple([pos[i]] for i in self.vars_dims[k])
+                else:
+                    self.pos[k] = tuple([i] for i in pos)
                 self.timestamps[k] = [now.timestamp()]
                 self.iteration[k] = [iteration]
             else:
-                self.storage[k].append(v)
-                for i, l in zip(pos, self.pos[k]):
-                    l.append(i)
+                if k in self.vars_dims:
+                    pos_k = tuple(pos[i] for i in self.vars_dims[k])
+                    if k not in dataframe and pos_k in zip(*self.pos[k]):
+                        continue
+                    for i, l in zip(pos_k, self.pos[k]):
+                        l.append(i)
+                else:
+                    for i, l in zip(pos, self.pos[k]):
+                        l.append(i)
                 self.timestamps[k].append(now.timestamp())
                 self.iteration[k].append(iteration)
+                self.storage[k].append(v)
 
-    def _flush(self, block=False):
+    def flush(self, block=False):
         if self._queue_buffer is not None:
             iteration, pos, fut, kwds, now = self._queue_buffer
             if fut.done() or block:
                 self._append(iteration, pos, fut.result(), kwds, now)
                 self._queue_buffer = None
             else:
                 return
@@ -670,62 +720,69 @@
                     self._append(iteration, pos, dataframe.result(), kwds, now)
             else:
                 self._append(iteration, pos, dataframe, kwds, now)
 
     def _get_array(self, key, shape, count):
         import numpy as np
 
+        if key in self.vars_dims:
+            shape = tuple([shape[i] for i in self.vars_dims[key]])
+
         data, data_shape, data_count = self.cache.get(key, (None, (), 0))
         if (data_shape, data_count) == (shape, count):
             return data
         try:
             tmp = np.asarray(self.storage[key])
             if data_shape != shape:
                 data = np.full(shape + tmp.shape[1:], np.nan, dtype=tmp.dtype)
         except:
             tmp = self.storage[key]
             if data_shape != shape:
                 data = np.full(shape, np.nan, dtype=object)
-        data[self.pos[key]] = tmp
+        try:
+            data[self.pos[key]] = tmp
+        except:
+            print(data.shape, self.pos[key], tmp)
+            raise
         self.cache[key] = (data, shape, count)
         return data
 
     def _get_part(self, key, skip):
         i = bisect.bisect_left(self.iteration[key], skip)
         pos = tuple(p[i:] for p in self.pos[key])
         iteration = self.iteration[key][i:]
         data = self.storage[key][i:]
         return data, iteration, pos
 
     def keys(self):
         """
         Get the keys of the storage.
         """
-        self._flush()
+        self.flush()
         return self.storage.keys()
 
     def values(self):
         """
         Get the values of the storage.
         """
-        self._flush()
+        self.flush()
         return [self[k] for k in self.storage]
 
     def items(self):
         """
         Get the items of the storage.
         """
-        self._flush()
+        self.flush()
         return list(zip(self.keys(), self.values()))
 
     def get(self, key, default=_NODEFAULT, skip=None, block=False):
         """
         Get the value of the storage.
         """
-        self._flush(block)
+        self.flush(block)
         if key in self._init_keys:
             return self.storage[key]
         elif key in self.storage:
             if skip is None:
                 return self._get_array(key, self.shape, self.count)
             else:
                 return self._get_part(key, skip)
@@ -734,24 +791,25 @@
         else:
             return default
 
     def __getitem__(self, key):
         return self.get(key)
 
     def __getstate__(self):
-        self._flush()
+        self.flush()
         storage = dict(self.items())
         return {
             'storage': storage,
             'pos': self.pos,
             'timestamps': self.timestamps,
             'iteration': self.iteration,
             'depends': self.depends,
             'shape': self.shape,
+            'dims': self.dims,
+            'vars_dims': self.vars_dims,
             'ctime': self.ctime,
             'mtime': self.mtime,
             '_init_keys': self._init_keys,
             '_frozen_keys': self._frozen_keys,
             '_key_levels': self._key_levels,
-            '_vars_dims': self._vars_dims,
             'save_kwds': self.save_kwds,
         }
```

### Comparing `waveforms-1.5.90/waveforms/security/verify.py` & `waveforms-1.5.92/waveforms/security/verify.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/server/__init__.py` & `waveforms-1.5.92/waveforms/server/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/server/__main__.py` & `waveforms-1.5.92/waveforms/server/__main__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/server/umsgpack.py` & `waveforms-1.5.92/waveforms/server/umsgpack.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/sys/chat.py` & `waveforms-1.5.92/waveforms/sys/chat.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/sys/device/basedevice.py` & `waveforms-1.5.92/waveforms/sys/device/basedevice.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/sys/device/loader.py` & `waveforms-1.5.92/waveforms/sys/device/loader.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/sys/device/utils.py` & `waveforms-1.5.92/waveforms/sys/device/utils.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/sys/drivers/FakeInstrument.py` & `waveforms-1.5.92/waveforms/sys/drivers/FakeInstrument.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/sys/ipy_events.py` & `waveforms-1.5.92/waveforms/sys/ipy_events.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/sys/net/dhcp.py` & `waveforms-1.5.92/waveforms/sys/net/dhcp.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/sys/net/dhcpd.py` & `waveforms-1.5.92/waveforms/sys/net/dhcpd.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/sys/net/kad.py` & `waveforms-1.5.92/waveforms/sys/net/kad.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/sys/net/kcp.py` & `waveforms-1.5.92/waveforms/sys/net/kcp.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/sys/progress.py` & `waveforms-1.5.92/waveforms/sys/progress.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/sys/storage/crud.py` & `waveforms-1.5.92/waveforms/sys/storage/crud.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/sys/storage/models.py` & `waveforms-1.5.92/waveforms/sys/storage/models.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/units/__init__.py` & `waveforms-1.5.92/waveforms/units/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/visualization/__init__.py` & `waveforms-1.5.92/waveforms/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/visualization/plot_layout.py` & `waveforms-1.5.92/waveforms/visualization/plot_layout.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/visualization/plot_seq.py` & `waveforms-1.5.92/waveforms/visualization/plot_seq.py`

 * *Files identical despite different names*

### Comparing `waveforms-1.5.90/waveforms/waveform.py` & `waveforms-1.5.92/waveforms/waveform.py`

 * *Files 3% similar despite different names*

```diff
@@ -804,14 +804,28 @@
 def _format_ERF(shift, *args):
     if shift != 0:
         return '\\mathrm{erf}(\\frac{t-' + f"{shift:g}" + '}{' + f'{args[0]:g}' + '})'
     else:
         return '\\mathrm{erf}(\\frac{t}{' + f'{args[0]:g}' + '})'
 
 
+def _format_COSH(shift, *args):
+    if shift != 0:
+        return '\\cosh(\\frac{t-' + f"{shift:g}" + '}{' + f'{1/args[0]:g}' + '})'
+    else:
+        return '\\cosh(\\frac{t}{' + f'{1/args[0]:g}' + '})'
+
+
+def _format_SINH(shift, *args):
+    if shift != 0:
+        return '\\sinh(\\frac{t-' + f"{shift:g}" + '}{' + f'{args[0]:g}' + '})'
+    else:
+        return '\\sinh(\\frac{t}{' + f'{args[0]:g}' + '})'
+
+
 def _format_EXP(shift, *args):
     if shift != 0:
         return '\\exp(-' + f'{args[0]:g}' + '(t-' + f"{shift:g}" + '))'
     else:
         return '\\exp(-' + f'{args[0]:g}' + 't)'
 
 
@@ -827,14 +841,16 @@
     t, np.linspace(start, stop, len(points)), points))
 LINEARCHIRP = registerBaseFunc(lambda t, f0, f1, T, phi0: np.sin(
     phi0 + 2 * np.pi * ((f1 - f0) / (2 * T) * t**2 + f0 * t)))
 EXPONENTIALCHIRP = registerBaseFunc(lambda t, f0, alpha, phi0: np.sin(
     phi0 + 2 * pi * f0 * (np.exp(alpha * t) - 1) / alpha))
 HYPERBOLICCHIRP = registerBaseFunc(lambda t, f0, k, phi0: np.sin(
     phi0 + 2 * np.pi * f0 / k * np.log(1 + k * t)))
+COSH = registerBaseFunc(lambda t, w: np.cosh(w * t), _format_COSH)
+SINH = registerBaseFunc(lambda t, w: np.sinh(w * t), _format_SINH)
 
 # register derivative
 registerDerivative(LINEAR, lambda shift, *args: _one)
 
 registerDerivative(
     GAUSSIAN, lambda shift, *args: (((((LINEAR, shift),
                                        (GAUSSIAN, *args, shift)), (1, 1)), ),
@@ -859,14 +875,22 @@
                                (args[0], )))
 
 registerDerivative(
     INTERP, lambda shift, start, stop, points:
     (((((INTERP, start, stop, tuple(np.gradient(np.asarray(points))), shift),
         ), (1, )), ), ((len(points) - 1) / (stop - start), )))
 
+registerDerivative(
+    COSH, lambda shift, *args: (((((SINH, *args, shift), ), (1, )), ),
+                                (args[0], )))
+
+registerDerivative(
+    SINH, lambda shift, *args: (((((COSH, *args, shift), ), (1, )), ),
+                                (args[0], )))
+
 
 def _d_LINEARCHIRP(shift, f0, f1, T, phi0):
     tlist = (
         (((LINEARCHIRP, f0, f1, T, phi0 + pi / 2, shift), ), (1, )),
         (((LINEAR, shift), (LINEARCHIRP, f0, f1, T, phi0 + pi / 2, shift)),
          (1, 1)),
     )
@@ -1035,14 +1059,57 @@
                     seq=(_zero, pulse, _zero))
 
 
 def hanning(width):
     return cosPulse(width)
 
 
+def cosh(w):
+    return Waveform(seq=(_basic_wave(COSH, w), ))
+
+
+def sinh(w):
+    return Waveform(seq=(_basic_wave(SINH, w), ))
+
+
+def coshPulse(width, steepness=1.0, plateau=0.0):
+    """
+    pulse edge shape:
+            cosh(w * T / 2) - cosh(w * t)
+    f(t) = -------------------------------
+                cosh(w * T / 2) - 1
+    where T is the pulse width and w = steepness / width
+    plateau is the fraction of the pulse width where the pulse is flat.
+    """
+    if width <= 0 and plateau <= 0:
+        return zero()
+    w = steepness / width
+    A = np.cosh(steepness / 2)
+
+    if plateau == 0.0 or round(-0.5 * plateau, NDIGITS) == round(
+            0.5 * plateau, NDIGITS):
+        pulse = ((((), ()), (((COSH, w, 0), ), (1, ))), (A / (A - 1),
+                                                         -1 / (A - 1)))
+        return Waveform(bounds=(round(-0.5 * width,
+                                      NDIGITS), round(0.5 * width,
+                                                      NDIGITS), +inf),
+                        seq=(_zero, pulse, _zero))
+    else:
+        raising = ((((), ()), (((COSH, w, -0.5 * plateau), ), (1, ))),
+                   (A / (A - 1), -1 / (A - 1)))
+        falling = ((((), ()), (((COSH, w, 0.5 * plateau), ), (1, ))),
+                   (A / (A - 1), -1 / (A - 1)))
+        return Waveform(bounds=(round(-0.5 * width - 0.5 * plateau,
+                                      NDIGITS), round(-0.5 * plateau, NDIGITS),
+                                round(0.5 * plateau, NDIGITS),
+                                round(0.5 * width + 0.5 * plateau,
+                                      NDIGITS), +inf),
+                        seq=(_zero, raising, _one, falling, _zero))
+
+
 def general_cosine(duration, *arg):
     wav = zero()
     arg = np.asarray(arg)
     arg /= arg[::2].sum()
     for i, a in enumerate(arg, start=1):
         wav += a / 2 * (1 - (-1)**i * cos(i * 2 * pi / duration))
     return wav * square(duration)
@@ -1204,12 +1271,13 @@
 
     Qout = ratioIQ * Qout
 
     return Iout, Qout
 
 
 __all__ = [
-    'D', 'Waveform', 'chirp', 'const', 'cos', 'cosPulse', 'cut', 'exp',
-    'function', 'gaussian', 'general_cosine', 'hanning', 'interp', 'mixing',
-    'one', 'poly', 'registerBaseFunc', 'registerDerivative', 'samplingPoints',
-    'sign', 'sin', 'sinc', 'square', 'step', 'zero'
+    'D', 'Waveform', 'chirp', 'const', 'cos', 'cosh', 'coshPulse', 'cosPulse',
+    'cut', 'exp', 'function', 'gaussian', 'general_cosine', 'hanning',
+    'interp', 'mixing', 'one', 'poly', 'registerBaseFunc',
+    'registerDerivative', 'samplingPoints', 'sign', 'sin', 'sinc', 'sinh',
+    'square', 'step', 'zero'
 ]
```

### Comparing `waveforms-1.5.90/waveforms/waveform_parser.py` & `waveforms-1.5.92/waveforms/waveform_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,18 @@
     def token(self):
         """Return the next token."""
         ret = self.lexer.token()
         return ret
 
     literals = r'=()[]<>,.+-/*^'
     functions = [
-        'D', 'chirp', 'const', 'cos', 'cosPulse', 'cut', 'exp', 'gaussian',
-        'general_cosine', 'hanning', 'interp', 'mixing', 'one', 'poly',
-        'samplingPoints', 'sign', 'sin', 'sinc', 'square', 'step', 'zero'
+        'D', 'chirp', 'const', 'cos', 'cosh', 'coshPulse', 'cosPulse', 'cut',
+        'exp', 'gaussian', 'general_cosine', 'hanning', 'interp', 'mixing',
+        'one', 'poly', 'samplingPoints', 'sign', 'sin', 'sinc', 'sinh',
+        'square', 'step', 'zero'
     ]
     tokens = [
         'REAL', 'IMAG', 'INT', 'STRING', 'ID', 'LSHIFT', 'RSHIFT', 'POW',
         'CONST', 'FUNCTION'
     ]
 
     def t_ID(self, t):
```

### Comparing `waveforms-1.5.90/waveforms.egg-info/PKG-INFO` & `waveforms-1.5.92/waveforms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waveforms
-Version: 1.5.90
+Version: 1.5.92
 Summary: Edit waveforms used in experiment
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/feihoo87/waveforms
 Project-URL: Bug Reports, https://github.com/feihoo87/waveforms/issues
 Project-URL: Source, https://github.com/feihoo87/waveforms/
```

### Comparing `waveforms-1.5.90/waveforms.egg-info/SOURCES.txt` & `waveforms-1.5.92/waveforms.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,16 @@
 waveforms/math/fit/delay.py
 waveforms/math/fit/geo.py
 waveforms/math/fit/qubit_dynamics.py
 waveforms/math/fit/readout.py
 waveforms/math/fit/resonator.py
 waveforms/math/fit/simple.py
 waveforms/math/fit/spectrum.py
+waveforms/math/group/_SU_n_.py
+waveforms/math/group/__init__.py
 waveforms/math/signal/__init__.py
 waveforms/math/signal/demodulate.py
 waveforms/math/signal/distortion.py
 waveforms/math/signal/func.py
 waveforms/qlisp/__init__.py
 waveforms/qlisp/assembly.py
 waveforms/qlisp/base.py
```

