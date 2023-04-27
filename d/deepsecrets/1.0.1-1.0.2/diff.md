# Comparing `tmp/deepsecrets-1.0.1.tar.gz` & `tmp/deepsecrets-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsecrets-1.0.1.tar", max compression
+gzip compressed data, was "deepsecrets-1.0.2.tar", max compression
```

## Comparing `deepsecrets-1.0.1.tar` & `deepsecrets-1.0.2.tar`

### file list

```diff
@@ -1,145 +1,145 @@
--rw-r--r--   0        0        0     1061 2023-03-27 10:35:08.129343 deepsecrets-1.0.1/LICENSE
--rw-r--r--   0        0        0     3889 2023-04-22 04:46:27.734564 deepsecrets-1.0.1/README.md
--rw-r--r--   0        0        0     8196 2023-03-28 08:59:04.340095 deepsecrets-1.0.1/deepsecrets/.DS_Store
--rw-r--r--   0        0        0      629 2023-04-22 04:36:53.671874 deepsecrets-1.0.1/deepsecrets/__init__.py
--rw-r--r--   0        0        0      107 2023-04-22 04:37:11.360189 deepsecrets-1.0.1/deepsecrets/__main__.py
--rw-r--r--   0        0        0     6429 2023-04-17 13:31:34.040560 deepsecrets-1.0.1/deepsecrets/cli.py
--rw-r--r--   0        0        0     1675 2023-04-17 13:19:49.920625 deepsecrets-1.0.1/deepsecrets/config.py
--rw-r--r--   0        0        0     8196 2023-02-26 15:19:47.000000 deepsecrets-1.0.1/deepsecrets/core/.DS_Store
--rw-r--r--   0        0        0        0 2022-05-17 09:51:36.000000 deepsecrets-1.0.1/deepsecrets/core/engines/__init__.py
--rw-r--r--   0        0        0      150 2023-01-28 13:47:04.000000 deepsecrets-1.0.1/deepsecrets/core/engines/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2696 2023-04-17 12:40:25.353990 deepsecrets-1.0.1/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc
--rw-r--r--   0        0        0     2660 2023-04-17 13:34:38.819504 deepsecrets-1.0.1/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc
--rw-r--r--   0        0        0     1992 2023-04-17 13:35:10.334351 deepsecrets-1.0.1/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     6184 2023-04-14 12:59:29.927306 deepsecrets-1.0.1/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc
--rw-r--r--   0        0        0     1611 2023-04-17 12:40:24.547637 deepsecrets-1.0.1/deepsecrets/core/engines/hashed_secret.py
--rw-r--r--   0        0        0     1200 2023-04-17 13:34:38.199667 deepsecrets-1.0.1/deepsecrets/core/engines/iengine.py
--rw-r--r--   0        0        0     1196 2023-04-17 13:35:09.681785 deepsecrets-1.0.1/deepsecrets/core/engines/regex.py
--rw-r--r--   0        0        0     4333 2023-04-14 12:59:29.251562 deepsecrets-1.0.1/deepsecrets/core/engines/semantic.py
--rw-r--r--   0        0        0     2561 2023-02-28 16:49:26.000000 deepsecrets-1.0.1/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc
--rw-r--r--   0        0        0     1495 2022-09-15 09:37:41.000000 deepsecrets-1.0.1/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc
--rw-r--r--   0        0        0     2971 2023-04-14 12:50:22.603515 deepsecrets-1.0.1/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc
--rw-r--r--   0        0        0     1686 2022-09-15 09:36:08.000000 deepsecrets-1.0.1/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc
--rw-r--r--   0        0        0     1145 2023-02-28 16:18:28.000000 deepsecrets-1.0.1/deepsecrets/core/helpers/content_analyzer.py
--rw-r--r--   0        0        0     1831 2023-04-14 12:50:21.979920 deepsecrets-1.0.1/deepsecrets/core/helpers/entropy.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.1/deepsecrets/core/model/.DS_Store
--rw-r--r--   0        0        0       82 2023-02-23 12:04:19.000000 deepsecrets-1.0.1/deepsecrets/core/model/__init__.py
--rw-r--r--   0        0        0      292 2023-02-23 12:04:20.000000 deepsecrets-1.0.1/deepsecrets/core/model/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6910 2023-04-14 13:22:42.127475 deepsecrets-1.0.1/deepsecrets/core/model/__pycache__/file.cpython-311.pyc
--rw-r--r--   0        0        0     8418 2023-03-27 20:52:52.004543 deepsecrets-1.0.1/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc
--rw-r--r--   0        0        0      695 2023-02-28 15:59:52.000000 deepsecrets-1.0.1/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc
--rw-r--r--   0        0        0     3926 2023-04-17 12:50:07.084349 deepsecrets-1.0.1/deepsecrets/core/model/__pycache__/token.cpython-311.pyc
--rw-r--r--   0        0        0     3719 2023-04-14 13:22:41.393440 deepsecrets-1.0.1/deepsecrets/core/model/file.py
--rw-r--r--   0        0        0     4374 2023-03-27 20:52:51.349485 deepsecrets-1.0.1/deepsecrets/core/model/finding.py
--rw-r--r--   0        0        0        0 2023-01-27 16:18:29.000000 deepsecrets-1.0.1/deepsecrets/core/model/rules/__init__.py
--rw-r--r--   0        0        0      154 2023-01-28 13:47:51.000000 deepsecrets-1.0.1/deepsecrets/core/model/rules/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      954 2023-02-23 12:04:24.000000 deepsecrets-1.0.1/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc
--rw-r--r--   0        0        0      488 2023-04-17 13:45:18.933981 deepsecrets-1.0.1/deepsecrets/core/model/rules/__pycache__/false_finding.cpython-311.pyc
--rw-r--r--   0        0        0     2589 2023-04-17 13:06:29.025295 deepsecrets-1.0.1/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc
--rw-r--r--   0        0        0      510 2023-04-17 12:50:07.086386 deepsecrets-1.0.1/deepsecrets/core/model/rules/__pycache__/hashing.cpython-311.pyc
--rw-r--r--   0        0        0     5588 2023-04-14 12:57:25.499628 deepsecrets-1.0.1/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     2295 2023-04-14 12:57:56.098733 deepsecrets-1.0.1/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc
--rw-r--r--   0        0        0      269 2023-02-23 11:55:43.000000 deepsecrets-1.0.1/deepsecrets/core/model/rules/exlcuded_path.py
--rw-r--r--   0        0        0      121 2023-04-17 13:44:30.761705 deepsecrets-1.0.1/deepsecrets/core/model/rules/false_finding.py
--rw-r--r--   0        0        0     1438 2023-04-17 13:06:28.309253 deepsecrets-1.0.1/deepsecrets/core/model/rules/hashed_secret.py
--rw-r--r--   0        0        0      119 2023-04-17 12:41:47.443006 deepsecrets-1.0.1/deepsecrets/core/model/rules/hashing.py
--rw-r--r--   0        0        0     2971 2023-04-14 12:57:24.773737 deepsecrets-1.0.1/deepsecrets/core/model/rules/regex.py
--rw-r--r--   0        0        0      871 2023-04-14 12:57:55.404355 deepsecrets-1.0.1/deepsecrets/core/model/rules/rule.py
--rw-r--r--   0        0        0       88 2023-02-23 11:55:43.000000 deepsecrets-1.0.1/deepsecrets/core/model/rules/semantic.py
--rw-r--r--   0        0        0      237 2023-02-28 15:59:50.000000 deepsecrets-1.0.1/deepsecrets/core/model/semantic.py
--rw-r--r--   0        0        0     2007 2023-04-17 12:50:06.475278 deepsecrets-1.0.1/deepsecrets/core/model/token.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.1/deepsecrets/core/modes/.DS_Store
--rw-r--r--   0        0        0     8325 2023-04-17 13:54:28.457157 deepsecrets-1.0.1/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc
--rw-r--r--   0        0        0     4968 2023-04-17 13:54:27.800941 deepsecrets-1.0.1/deepsecrets/core/modes/iscan_mode.py
--rw-r--r--   0        0        0      214 2023-01-25 14:00:27.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/confidence.cpython-311.pyc
--rw-r--r--   0        0        0      184 2022-09-13 14:18:23.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/confidence.cpython-39.pyc
--rw-r--r--   0        0        0      648 2023-02-28 15:59:52.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc
--rw-r--r--   0        0        0      649 2023-04-17 13:45:18.931553 deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc
--rw-r--r--   0        0        0     1424 2022-11-24 10:59:56.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc
--rw-r--r--   0        0        0     1796 2022-01-29 06:07:43.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc
--rw-r--r--   0        0        0     1059 2022-05-17 09:51:38.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc
--rw-r--r--   0        0        0     2551 2023-04-17 13:11:28.556085 deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc
--rw-r--r--   0        0        0     1515 2022-10-14 09:00:28.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc
--rw-r--r--   0        0        0     2281 2023-02-28 16:49:26.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc
--rw-r--r--   0        0        0     4653 2022-11-24 10:59:56.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc
--rw-r--r--   0        0        0     2752 2022-05-17 09:51:38.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc
--rw-r--r--   0        0        0      682 2023-01-28 14:26:39.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc
--rw-r--r--   0        0        0      821 2022-01-29 06:16:36.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc
--rw-r--r--   0        0        0      855 2022-10-13 11:40:21.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc
--rw-r--r--   0        0        0      783 2022-01-28 15:38:18.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc
--rw-r--r--   0        0        0     1661 2022-02-02 13:16:29.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc
--rw-r--r--   0        0        0      615 2023-02-28 15:59:52.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     2903 2022-10-13 11:43:01.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc
--rw-r--r--   0        0        0      250 2023-02-28 15:59:51.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/excluded_paths.py
--rw-r--r--   0        0        0      252 2023-04-17 13:45:18.253008 deepsecrets-1.0.1/deepsecrets/core/rulesets/false_findings.py
--rw-r--r--   0        0        0     1434 2023-04-17 13:11:27.888766 deepsecrets-1.0.1/deepsecrets/core/rulesets/hashed_secrets.py
--rw-r--r--   0        0        0      627 2023-02-28 16:35:44.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/ibuilder.py
--rw-r--r--   0        0        0      220 2023-02-28 15:59:51.000000 deepsecrets-1.0.1/deepsecrets/core/rulesets/regex.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/.DS_Store
--rw-r--r--   0        0        0      181 2023-02-23 11:55:44.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/__init__.py
--rw-r--r--   0        0        0      366 2023-02-23 11:55:45.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      129 2022-09-12 09:34:48.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1059 2023-02-15 14:21:01.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc
--rw-r--r--   0        0        0      649 2022-01-28 16:00:02.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc
--rw-r--r--   0        0        0      732 2022-10-13 14:47:47.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc
--rw-r--r--   0        0        0     1948 2023-02-28 15:59:52.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc
--rw-r--r--   0        0        0      520 2022-01-28 13:54:30.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc
--rw-r--r--   0        0        0     1549 2022-10-13 14:13:37.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc
--rw-r--r--   0        0        0     2569 2022-04-25 16:49:33.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc
--rw-r--r--   0        0        0     9685 2023-03-27 20:23:09.189108 deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc
--rw-r--r--   0        0        0     4195 2022-05-27 10:40:16.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc
--rw-r--r--   0        0        0     1482 2023-04-14 12:50:35.476023 deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc
--rw-r--r--   0        0        0      852 2022-01-28 17:43:01.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc
--rw-r--r--   0        0        0      899 2022-09-12 09:34:48.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc
--rw-r--r--   0        0        0     1723 2023-01-25 14:00:28.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc
--rw-r--r--   0        0        0      977 2022-01-28 18:09:20.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc
--rw-r--r--   0        0        0     1010 2022-09-12 09:34:48.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc
--rw-r--r--   0        0        0      349 2023-02-15 13:58:04.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/full_content.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/.DS_Store
--rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/__init__.py
--rw-r--r--   0        0        0      153 2023-01-25 14:00:28.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      135 2022-09-12 09:34:48.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9952 2023-02-10 11:22:52.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc
--rw-r--r--   0        0        0     6003 2022-10-13 14:25:20.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc
--rw-r--r--   0        0        0     3570 2023-04-14 12:50:43.000351 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc
--rw-r--r--   0        0        0     2799 2023-04-21 14:40:38.036123 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store
--rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/__init__.py
--rw-r--r--   0        0        0      162 2023-01-25 14:00:28.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      144 2022-09-12 10:58:48.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1353 2023-04-13 12:42:45.606082 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc
--rw-r--r--   0        0        0     2684 2022-06-08 15:19:48.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc
--rw-r--r--   0        0        0    10645 2023-02-10 11:00:04.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc
--rw-r--r--   0        0        0     4836 2022-10-13 14:38:14.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc
--rw-r--r--   0        0        0      529 2023-04-13 12:42:44.862774 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/language.py
--rw-r--r--   0        0        0        0 2023-02-10 15:56:26.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__init__.py
--rw-r--r--   0        0        0      184 2023-02-10 15:56:27.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5347 2023-04-14 13:00:04.497720 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc
--rw-r--r--   0        0        0     6476 2023-04-14 13:10:20.748746 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0     2711 2023-04-14 13:00:03.807886 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py
--rw-r--r--   0        0        0     5781 2023-04-14 13:10:20.026707 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py
--rw-r--r--   0        0        0     2027 2023-04-14 12:50:42.345036 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/spot_improvements.py
--rw-r--r--   0        0        0     1801 2023-04-21 14:40:37.153608 deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/type_stream.py
--rw-r--r--   0        0        0      735 2023-02-28 15:59:51.000000 deepsecrets-1.0.1/deepsecrets/core/tokenizers/itokenizer.py
--rw-r--r--   0        0        0     6015 2023-03-27 20:23:08.303488 deepsecrets-1.0.1/deepsecrets/core/tokenizers/lexer.py
--rw-r--r--   0        0        0      600 2023-04-14 12:50:34.810801 deepsecrets-1.0.1/deepsecrets/core/tokenizers/per_line.py
--rw-r--r--   0        0        0     1022 2023-04-14 12:50:38.878506 deepsecrets-1.0.1/deepsecrets/core/tokenizers/per_word.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.1/deepsecrets/core/utils/.DS_Store
--rw-r--r--   0        0        0        0 2019-08-30 09:25:52.000000 deepsecrets-1.0.1/deepsecrets/core/utils/__init__.py
--rw-r--r--   0        0        0      148 2023-02-10 10:44:34.000000 deepsecrets-1.0.1/deepsecrets/core/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      586 2023-02-28 15:32:35.000000 deepsecrets-1.0.1/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0        0        0     5469 2023-03-27 20:23:09.183623 deepsecrets-1.0.1/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc
--rw-r--r--   0        0        0     1415 2023-02-28 16:49:26.000000 deepsecrets-1.0.1/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc
--rw-r--r--   0        0        0     1774 2023-04-17 12:50:07.088140 deepsecrets-1.0.1/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc
--rw-r--r--   0        0        0      100 2023-02-28 15:32:34.000000 deepsecrets-1.0.1/deepsecrets/core/utils/exceptions.py
--rw-r--r--   0        0        0     3018 2023-03-27 20:23:08.288214 deepsecrets-1.0.1/deepsecrets/core/utils/file_analyzer.py
--rw-r--r--   0        0        0      517 2023-02-28 16:47:36.000000 deepsecrets-1.0.1/deepsecrets/core/utils/fs.py
--rw-r--r--   0        0        0      771 2023-04-17 12:49:00.602766 deepsecrets-1.0.1/deepsecrets/core/utils/hashing.py
--rw-r--r--   0        0        0     2562 2023-01-29 12:25:02.000000 deepsecrets-1.0.1/deepsecrets/rules/excluded_paths.json
--rw-r--r--   0        0        0     3990 2023-03-27 20:07:41.216976 deepsecrets-1.0.1/deepsecrets/rules/regexes.json
--rw-r--r--   0        0        0        2 2023-02-22 17:11:42.000000 deepsecrets-1.0.1/deepsecrets/rules/semantic.json
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.1/deepsecrets/scan_modes/.DS_Store
--rw-r--r--   0        0        0     5698 2023-04-17 13:42:10.557066 deepsecrets-1.0.1/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0        0        0     3268 2023-04-17 13:42:09.893195 deepsecrets-1.0.1/deepsecrets/scan_modes/cli.py
--rw-r--r--   0        0        0     1669 2023-04-22 04:48:49.121743 deepsecrets-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5068 1970-01-01 00:00:00.000000 deepsecrets-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-03-27 10:35:08.129343 deepsecrets-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3889 2023-04-22 04:46:27.734564 deepsecrets-1.0.2/README.md
+-rw-r--r--   0        0        0     8196 2023-03-28 08:59:04.340095 deepsecrets-1.0.2/deepsecrets/.DS_Store
+-rw-r--r--   0        0        0      629 2023-04-22 04:36:53.671874 deepsecrets-1.0.2/deepsecrets/__init__.py
+-rw-r--r--   0        0        0      107 2023-04-22 04:37:11.360189 deepsecrets-1.0.2/deepsecrets/__main__.py
+-rw-r--r--   0        0        0     6429 2023-04-17 13:31:34.040560 deepsecrets-1.0.2/deepsecrets/cli.py
+-rw-r--r--   0        0        0     1675 2023-04-17 13:19:49.920625 deepsecrets-1.0.2/deepsecrets/config.py
+-rw-r--r--   0        0        0     8196 2023-02-26 15:19:47.000000 deepsecrets-1.0.2/deepsecrets/core/.DS_Store
+-rw-r--r--   0        0        0        0 2022-05-17 09:51:36.000000 deepsecrets-1.0.2/deepsecrets/core/engines/__init__.py
+-rw-r--r--   0        0        0      150 2023-01-28 13:47:04.000000 deepsecrets-1.0.2/deepsecrets/core/engines/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2696 2023-04-17 12:40:25.353990 deepsecrets-1.0.2/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc
+-rw-r--r--   0        0        0     2660 2023-04-17 13:34:38.819504 deepsecrets-1.0.2/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc
+-rw-r--r--   0        0        0     1992 2023-04-17 13:35:10.334351 deepsecrets-1.0.2/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     6184 2023-04-14 12:59:29.927306 deepsecrets-1.0.2/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc
+-rw-r--r--   0        0        0     1611 2023-04-17 12:40:24.547637 deepsecrets-1.0.2/deepsecrets/core/engines/hashed_secret.py
+-rw-r--r--   0        0        0     1200 2023-04-17 13:34:38.199667 deepsecrets-1.0.2/deepsecrets/core/engines/iengine.py
+-rw-r--r--   0        0        0     1196 2023-04-17 13:35:09.681785 deepsecrets-1.0.2/deepsecrets/core/engines/regex.py
+-rw-r--r--   0        0        0     4333 2023-04-14 12:59:29.251562 deepsecrets-1.0.2/deepsecrets/core/engines/semantic.py
+-rw-r--r--   0        0        0     2561 2023-02-28 16:49:26.000000 deepsecrets-1.0.2/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc
+-rw-r--r--   0        0        0     1495 2022-09-15 09:37:41.000000 deepsecrets-1.0.2/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc
+-rw-r--r--   0        0        0     2971 2023-04-14 12:50:22.603515 deepsecrets-1.0.2/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc
+-rw-r--r--   0        0        0     1686 2022-09-15 09:36:08.000000 deepsecrets-1.0.2/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc
+-rw-r--r--   0        0        0     1145 2023-02-28 16:18:28.000000 deepsecrets-1.0.2/deepsecrets/core/helpers/content_analyzer.py
+-rw-r--r--   0        0        0     1831 2023-04-14 12:50:21.979920 deepsecrets-1.0.2/deepsecrets/core/helpers/entropy.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.2/deepsecrets/core/model/.DS_Store
+-rw-r--r--   0        0        0       82 2023-02-23 12:04:19.000000 deepsecrets-1.0.2/deepsecrets/core/model/__init__.py
+-rw-r--r--   0        0        0      292 2023-02-23 12:04:20.000000 deepsecrets-1.0.2/deepsecrets/core/model/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6910 2023-04-14 13:22:42.127475 deepsecrets-1.0.2/deepsecrets/core/model/__pycache__/file.cpython-311.pyc
+-rw-r--r--   0        0        0     8418 2023-03-27 20:52:52.004543 deepsecrets-1.0.2/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc
+-rw-r--r--   0        0        0      695 2023-02-28 15:59:52.000000 deepsecrets-1.0.2/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc
+-rw-r--r--   0        0        0     3926 2023-04-17 12:50:07.084349 deepsecrets-1.0.2/deepsecrets/core/model/__pycache__/token.cpython-311.pyc
+-rw-r--r--   0        0        0     3719 2023-04-14 13:22:41.393440 deepsecrets-1.0.2/deepsecrets/core/model/file.py
+-rw-r--r--   0        0        0     4374 2023-03-27 20:52:51.349485 deepsecrets-1.0.2/deepsecrets/core/model/finding.py
+-rw-r--r--   0        0        0        0 2023-01-27 16:18:29.000000 deepsecrets-1.0.2/deepsecrets/core/model/rules/__init__.py
+-rw-r--r--   0        0        0      154 2023-01-28 13:47:51.000000 deepsecrets-1.0.2/deepsecrets/core/model/rules/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      954 2023-02-23 12:04:24.000000 deepsecrets-1.0.2/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc
+-rw-r--r--   0        0        0      488 2023-04-17 13:45:18.933981 deepsecrets-1.0.2/deepsecrets/core/model/rules/__pycache__/false_finding.cpython-311.pyc
+-rw-r--r--   0        0        0     2589 2023-04-17 13:06:29.025295 deepsecrets-1.0.2/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc
+-rw-r--r--   0        0        0      510 2023-04-17 12:50:07.086386 deepsecrets-1.0.2/deepsecrets/core/model/rules/__pycache__/hashing.cpython-311.pyc
+-rw-r--r--   0        0        0     5588 2023-04-14 12:57:25.499628 deepsecrets-1.0.2/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     2295 2023-04-14 12:57:56.098733 deepsecrets-1.0.2/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc
+-rw-r--r--   0        0        0      269 2023-02-23 11:55:43.000000 deepsecrets-1.0.2/deepsecrets/core/model/rules/exlcuded_path.py
+-rw-r--r--   0        0        0      121 2023-04-17 13:44:30.761705 deepsecrets-1.0.2/deepsecrets/core/model/rules/false_finding.py
+-rw-r--r--   0        0        0     1438 2023-04-17 13:06:28.309253 deepsecrets-1.0.2/deepsecrets/core/model/rules/hashed_secret.py
+-rw-r--r--   0        0        0      119 2023-04-17 12:41:47.443006 deepsecrets-1.0.2/deepsecrets/core/model/rules/hashing.py
+-rw-r--r--   0        0        0     2971 2023-04-14 12:57:24.773737 deepsecrets-1.0.2/deepsecrets/core/model/rules/regex.py
+-rw-r--r--   0        0        0      871 2023-04-14 12:57:55.404355 deepsecrets-1.0.2/deepsecrets/core/model/rules/rule.py
+-rw-r--r--   0        0        0       88 2023-02-23 11:55:43.000000 deepsecrets-1.0.2/deepsecrets/core/model/rules/semantic.py
+-rw-r--r--   0        0        0      237 2023-02-28 15:59:50.000000 deepsecrets-1.0.2/deepsecrets/core/model/semantic.py
+-rw-r--r--   0        0        0     2007 2023-04-17 12:50:06.475278 deepsecrets-1.0.2/deepsecrets/core/model/token.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.2/deepsecrets/core/modes/.DS_Store
+-rw-r--r--   0        0        0     8325 2023-04-17 13:54:28.457157 deepsecrets-1.0.2/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc
+-rw-r--r--   0        0        0     4968 2023-04-17 13:54:27.800941 deepsecrets-1.0.2/deepsecrets/core/modes/iscan_mode.py
+-rw-r--r--   0        0        0      214 2023-01-25 14:00:27.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/confidence.cpython-311.pyc
+-rw-r--r--   0        0        0      184 2022-09-13 14:18:23.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/confidence.cpython-39.pyc
+-rw-r--r--   0        0        0      648 2023-02-28 15:59:52.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc
+-rw-r--r--   0        0        0      649 2023-04-17 13:45:18.931553 deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc
+-rw-r--r--   0        0        0     1424 2022-11-24 10:59:56.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc
+-rw-r--r--   0        0        0     1796 2022-01-29 06:07:43.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc
+-rw-r--r--   0        0        0     1059 2022-05-17 09:51:38.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc
+-rw-r--r--   0        0        0     2551 2023-04-17 13:11:28.556085 deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc
+-rw-r--r--   0        0        0     1515 2022-10-14 09:00:28.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc
+-rw-r--r--   0        0        0     2281 2023-02-28 16:49:26.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc
+-rw-r--r--   0        0        0     4653 2022-11-24 10:59:56.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc
+-rw-r--r--   0        0        0     2752 2022-05-17 09:51:38.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc
+-rw-r--r--   0        0        0      682 2023-01-28 14:26:39.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc
+-rw-r--r--   0        0        0      821 2022-01-29 06:16:36.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc
+-rw-r--r--   0        0        0      855 2022-10-13 11:40:21.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc
+-rw-r--r--   0        0        0      783 2022-01-28 15:38:18.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc
+-rw-r--r--   0        0        0     1661 2022-02-02 13:16:29.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc
+-rw-r--r--   0        0        0      615 2023-02-28 15:59:52.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     2903 2022-10-13 11:43:01.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc
+-rw-r--r--   0        0        0      250 2023-02-28 15:59:51.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/excluded_paths.py
+-rw-r--r--   0        0        0      252 2023-04-17 13:45:18.253008 deepsecrets-1.0.2/deepsecrets/core/rulesets/false_findings.py
+-rw-r--r--   0        0        0     1434 2023-04-17 13:11:27.888766 deepsecrets-1.0.2/deepsecrets/core/rulesets/hashed_secrets.py
+-rw-r--r--   0        0        0      627 2023-02-28 16:35:44.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/ibuilder.py
+-rw-r--r--   0        0        0      220 2023-02-28 15:59:51.000000 deepsecrets-1.0.2/deepsecrets/core/rulesets/regex.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/.DS_Store
+-rw-r--r--   0        0        0      181 2023-02-23 11:55:44.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/__init__.py
+-rw-r--r--   0        0        0      366 2023-02-23 11:55:45.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      129 2022-09-12 09:34:48.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1059 2023-02-15 14:21:01.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc
+-rw-r--r--   0        0        0      649 2022-01-28 16:00:02.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc
+-rw-r--r--   0        0        0      732 2022-10-13 14:47:47.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc
+-rw-r--r--   0        0        0     1948 2023-02-28 15:59:52.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc
+-rw-r--r--   0        0        0      520 2022-01-28 13:54:30.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc
+-rw-r--r--   0        0        0     1549 2022-10-13 14:13:37.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc
+-rw-r--r--   0        0        0     2569 2022-04-25 16:49:33.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     9685 2023-03-27 20:23:09.189108 deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc
+-rw-r--r--   0        0        0     4195 2022-05-27 10:40:16.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc
+-rw-r--r--   0        0        0     1482 2023-04-14 12:50:35.476023 deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc
+-rw-r--r--   0        0        0      852 2022-01-28 17:43:01.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc
+-rw-r--r--   0        0        0      899 2022-09-12 09:34:48.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc
+-rw-r--r--   0        0        0     1723 2023-01-25 14:00:28.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc
+-rw-r--r--   0        0        0      977 2022-01-28 18:09:20.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc
+-rw-r--r--   0        0        0     1010 2022-09-12 09:34:48.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc
+-rw-r--r--   0        0        0      349 2023-02-15 13:58:04.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/full_content.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/.DS_Store
+-rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/__init__.py
+-rw-r--r--   0        0        0      153 2023-01-25 14:00:28.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      135 2022-09-12 09:34:48.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9952 2023-02-10 11:22:52.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc
+-rw-r--r--   0        0        0     6003 2022-10-13 14:25:20.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc
+-rw-r--r--   0        0        0     3570 2023-04-14 12:50:43.000351 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc
+-rw-r--r--   0        0        0     2799 2023-04-21 14:40:38.036123 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store
+-rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/__init__.py
+-rw-r--r--   0        0        0      162 2023-01-25 14:00:28.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      144 2022-09-12 10:58:48.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1353 2023-04-13 12:42:45.606082 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc
+-rw-r--r--   0        0        0     2684 2022-06-08 15:19:48.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc
+-rw-r--r--   0        0        0    10645 2023-02-10 11:00:04.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc
+-rw-r--r--   0        0        0     4836 2022-10-13 14:38:14.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc
+-rw-r--r--   0        0        0      529 2023-04-13 12:42:44.862774 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/language.py
+-rw-r--r--   0        0        0        0 2023-02-10 15:56:26.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__init__.py
+-rw-r--r--   0        0        0      184 2023-02-10 15:56:27.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5347 2023-04-14 13:00:04.497720 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc
+-rw-r--r--   0        0        0     6476 2023-04-14 13:10:20.748746 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0     2711 2023-04-14 13:00:03.807886 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py
+-rw-r--r--   0        0        0     5781 2023-04-14 13:10:20.026707 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py
+-rw-r--r--   0        0        0     2027 2023-04-14 12:50:42.345036 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/spot_improvements.py
+-rw-r--r--   0        0        0     1801 2023-04-21 14:40:37.153608 deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/type_stream.py
+-rw-r--r--   0        0        0      735 2023-02-28 15:59:51.000000 deepsecrets-1.0.2/deepsecrets/core/tokenizers/itokenizer.py
+-rw-r--r--   0        0        0     6015 2023-03-27 20:23:08.303488 deepsecrets-1.0.2/deepsecrets/core/tokenizers/lexer.py
+-rw-r--r--   0        0        0      600 2023-04-14 12:50:34.810801 deepsecrets-1.0.2/deepsecrets/core/tokenizers/per_line.py
+-rw-r--r--   0        0        0     1022 2023-04-14 12:50:38.878506 deepsecrets-1.0.2/deepsecrets/core/tokenizers/per_word.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.2/deepsecrets/core/utils/.DS_Store
+-rw-r--r--   0        0        0        0 2019-08-30 09:25:52.000000 deepsecrets-1.0.2/deepsecrets/core/utils/__init__.py
+-rw-r--r--   0        0        0      148 2023-02-10 10:44:34.000000 deepsecrets-1.0.2/deepsecrets/core/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      586 2023-02-28 15:32:35.000000 deepsecrets-1.0.2/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0     5469 2023-03-27 20:23:09.183623 deepsecrets-1.0.2/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc
+-rw-r--r--   0        0        0     1415 2023-02-28 16:49:26.000000 deepsecrets-1.0.2/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc
+-rw-r--r--   0        0        0     1774 2023-04-17 12:50:07.088140 deepsecrets-1.0.2/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc
+-rw-r--r--   0        0        0      100 2023-02-28 15:32:34.000000 deepsecrets-1.0.2/deepsecrets/core/utils/exceptions.py
+-rw-r--r--   0        0        0     3018 2023-03-27 20:23:08.288214 deepsecrets-1.0.2/deepsecrets/core/utils/file_analyzer.py
+-rw-r--r--   0        0        0      517 2023-02-28 16:47:36.000000 deepsecrets-1.0.2/deepsecrets/core/utils/fs.py
+-rw-r--r--   0        0        0      771 2023-04-17 12:49:00.602766 deepsecrets-1.0.2/deepsecrets/core/utils/hashing.py
+-rw-r--r--   0        0        0     2562 2023-01-29 12:25:02.000000 deepsecrets-1.0.2/deepsecrets/rules/excluded_paths.json
+-rw-r--r--   0        0        0     3990 2023-03-27 20:07:41.216976 deepsecrets-1.0.2/deepsecrets/rules/regexes.json
+-rw-r--r--   0        0        0        2 2023-02-22 17:11:42.000000 deepsecrets-1.0.2/deepsecrets/rules/semantic.json
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.2/deepsecrets/scan_modes/.DS_Store
+-rw-r--r--   0        0        0     5698 2023-04-17 13:42:10.557066 deepsecrets-1.0.2/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0        0        0     3268 2023-04-17 13:42:09.893195 deepsecrets-1.0.2/deepsecrets/scan_modes/cli.py
+-rw-r--r--   0        0        0     1666 2023-04-27 12:33:25.416409 deepsecrets-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5065 1970-01-01 00:00:00.000000 deepsecrets-1.0.2/PKG-INFO
```

### Comparing `deepsecrets-1.0.1/LICENSE` & `deepsecrets-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/README.md` & `deepsecrets-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/.DS_Store` & `deepsecrets-1.0.2/deepsecrets/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/__init__.py` & `deepsecrets-1.0.2/deepsecrets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/cli.py` & `deepsecrets-1.0.2/deepsecrets/cli.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/config.py` & `deepsecrets-1.0.2/deepsecrets/config.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/.DS_Store` & `deepsecrets-1.0.2/deepsecrets/core/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/engines/hashed_secret.py` & `deepsecrets-1.0.2/deepsecrets/core/engines/hashed_secret.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/engines/iengine.py` & `deepsecrets-1.0.2/deepsecrets/core/engines/iengine.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/engines/regex.py` & `deepsecrets-1.0.2/deepsecrets/core/engines/regex.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/engines/semantic.py` & `deepsecrets-1.0.2/deepsecrets/core/engines/semantic.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc` & `deepsecrets-1.0.2/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc` & `deepsecrets-1.0.2/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/helpers/content_analyzer.py` & `deepsecrets-1.0.2/deepsecrets/core/helpers/content_analyzer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/helpers/entropy.py` & `deepsecrets-1.0.2/deepsecrets/core/helpers/entropy.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/model/.DS_Store` & `deepsecrets-1.0.2/deepsecrets/core/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/model/__pycache__/file.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/model/__pycache__/file.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/model/__pycache__/token.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/model/__pycache__/token.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/model/file.py` & `deepsecrets-1.0.2/deepsecrets/core/model/file.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/model/finding.py` & `deepsecrets-1.0.2/deepsecrets/core/model/finding.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/model/rules/hashed_secret.py` & `deepsecrets-1.0.2/deepsecrets/core/model/rules/hashed_secret.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/model/rules/regex.py` & `deepsecrets-1.0.2/deepsecrets/core/model/rules/regex.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/model/rules/rule.py` & `deepsecrets-1.0.2/deepsecrets/core/model/rules/rule.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/model/token.py` & `deepsecrets-1.0.2/deepsecrets/core/model/token.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/modes/.DS_Store` & `deepsecrets-1.0.2/deepsecrets/core/modes/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/modes/iscan_mode.py` & `deepsecrets-1.0.2/deepsecrets/core/modes/iscan_mode.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc` & `deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc` & `deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc` & `deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc` & `deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc` & `deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc` & `deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc` & `deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc` & `deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc` & `deepsecrets-1.0.2/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/rulesets/hashed_secrets.py` & `deepsecrets-1.0.2/deepsecrets/core/rulesets/hashed_secrets.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/rulesets/ibuilder.py` & `deepsecrets-1.0.2/deepsecrets/core/rulesets/ibuilder.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/.DS_Store` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/.DS_Store` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/language.py` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/language.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/spot_improvements.py` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/spot_improvements.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/helpers/type_stream.py` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/helpers/type_stream.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/itokenizer.py` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/itokenizer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/lexer.py` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/lexer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/per_line.py` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/per_line.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/tokenizers/per_word.py` & `deepsecrets-1.0.2/deepsecrets/core/tokenizers/per_word.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/utils/.DS_Store` & `deepsecrets-1.0.2/deepsecrets/core/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/utils/file_analyzer.py` & `deepsecrets-1.0.2/deepsecrets/core/utils/file_analyzer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/utils/fs.py` & `deepsecrets-1.0.2/deepsecrets/core/utils/fs.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/core/utils/hashing.py` & `deepsecrets-1.0.2/deepsecrets/core/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/rules/excluded_paths.json` & `deepsecrets-1.0.2/deepsecrets/rules/excluded_paths.json`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/rules/regexes.json` & `deepsecrets-1.0.2/deepsecrets/rules/regexes.json`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/scan_modes/.DS_Store` & `deepsecrets-1.0.2/deepsecrets/scan_modes/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc` & `deepsecrets-1.0.2/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/deepsecrets/scan_modes/cli.py` & `deepsecrets-1.0.2/deepsecrets/scan_modes/cli.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.1/pyproject.toml` & `deepsecrets-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepsecrets"
-version = "1.0.1"
+version = "1.0.2"
 description = "A better tool for secrets search"
 license = "MIT"
 authors = [
   "Nikolai Khechumov <khechumov@gmail.com>",
 ]
 keywords = ["security", "secrets", "credentials", "scanning", "appsec"]
 packages = [{include = "deepsecrets"}]
@@ -25,15 +25,15 @@
 "Bug Tracker" = "https://github.com/avito-tech/deepsecrets/issues"
 
 [tool.poetry.scripts]
 deepsecrets = "deepsecrets:__main__"
 
 
 [tool.poetry.dependencies]
-python = ">=3.9,<=3.11.1"
+python = ">=3.9,<3.12"
 pydantic = "^1.10.4"
 pyyaml = "^5.4.1"
 pygments = "^2.14.0"
 ordered-set = "^4.1.0"
 dotwiz = "^0.4.0"
 mmh3 = "^3.0.0"
 argparse = "^1.4.0"
```

### Comparing `deepsecrets-1.0.1/PKG-INFO` & `deepsecrets-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: deepsecrets
-Version: 1.0.1
+Version: 1.0.2
 Summary: A better tool for secrets search
 License: MIT
 Keywords: security,secrets,credentials,scanning,appsec
 Author: Nikolai Khechumov
 Author-email: khechumov@gmail.com
-Requires-Python: >=3.9,<=3.11.1
+Requires-Python: >=3.9,<3.12
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

