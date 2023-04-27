# Comparing `tmp/pycomex-0.8.8.tar.gz` & `tmp/pycomex-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycomex-0.8.8.tar", max compression
+gzip compressed data, was "pycomex-0.9.0.tar", max compression
```

## Comparing `pycomex-0.8.8.tar` & `pycomex-0.9.0.tar`

### file list

```diff
@@ -1,226 +1,226 @@
--rwxr-xr-x   0        0        0     1071 2022-07-09 08:06:36.748803 pycomex-0.8.8/LICENSE
--rwxr-xr-x   0        0        0     6820 2023-02-09 14:59:34.788632 pycomex-0.8.8/README.rst
--rwxr-xr-x   0        0        0        6 2023-02-24 07:28:31.627843 pycomex-0.8.8/pycomex/VERSION
--rwxr-xr-x   0        0        0      178 2022-09-19 07:18:59.122787 pycomex-0.8.8/pycomex/__init__.py
--rwxr-xr-x   0        0        0        0 2022-08-20 17:22:07.854881 pycomex-0.8.8/pycomex/app/__init__.py
--rwxr-xr-x   0        0        0     7375 2023-01-03 06:49:42.464926 pycomex-0.8.8/pycomex/cli.py
--rwxr-xr-x   0        0        0      899 2023-02-13 20:56:26.976515 pycomex-0.8.8/pycomex/examples/README.rst
--rwxr-xr-x   0        0        0     3887 2023-02-13 20:36:41.593997 pycomex-0.8.8/pycomex/examples/analysing.py
--rwxr-xr-x   0        0        0     3256 2023-02-09 14:55:10.188721 pycomex-0.8.8/pycomex/examples/basic.py
--rwxr-xr-x   0        0        0     3888 2023-02-16 19:07:05.131685 pycomex-0.8.8/pycomex/examples/example/inheritance/debug/00_random.txt
--rwxr-xr-x   0        0        0     3793 2023-02-16 19:07:05.133113 pycomex-0.8.8/pycomex/examples/example/inheritance/debug/01_random.txt
--rwxr-xr-x   0        0        0     3748 2023-02-16 19:07:05.134542 pycomex-0.8.8/pycomex/examples/example/inheritance/debug/02_random.txt
--rwxr-xr-x   0        0        0     3802 2023-02-16 19:07:05.135962 pycomex-0.8.8/pycomex/examples/example/inheritance/debug/03_random.txt
--rwxr-xr-x   0        0        0     3843 2023-02-16 19:07:05.137577 pycomex-0.8.8/pycomex/examples/example/inheritance/debug/04_random.txt
--rwxr-xr-x   0        0        0     3887 2023-02-16 19:07:05.159992 pycomex-0.8.8/pycomex/examples/example/inheritance/debug/analysing.py
--rwxr-xr-x   0        0        0     2000 2023-02-16 19:07:05.161471 pycomex-0.8.8/pycomex/examples/example/inheritance/debug/analysis.py
--rwxr-xr-x   0        0        0      118 2023-02-16 19:07:05.158584 pycomex-0.8.8/pycomex/examples/example/inheritance/debug/analysis_results.json
--rwxr-xr-x   0        0        0      692 2023-02-16 19:07:05.141950 pycomex-0.8.8/pycomex/examples/example/inheritance/debug/annotations.rst
--rwxr-xr-x   0        0        0     1948 2023-02-16 19:07:05.149422 pycomex-0.8.8/pycomex/examples/example/inheritance/debug/experiment_data.json
--rwxr-xr-x   0        0        0     1932 2023-02-16 19:07:05.161028 pycomex-0.8.8/pycomex/examples/example/inheritance/debug/experiment_log.txt
--rwxr-xr-x   0        0        0      367 2023-02-16 19:07:05.149762 pycomex-0.8.8/pycomex/examples/example/inheritance/debug/experiment_meta.json
--rwxr-xr-x   0        0        0     4712 2023-02-16 19:07:05.139235 pycomex-0.8.8/pycomex/examples/example/inheritance/debug/snapshot.py
--rwxr-xr-x   0        0        0     5173 2023-02-16 19:10:46.863704 pycomex-0.8.8/pycomex/examples/inheritance.py
--rwxr-xr-x   0        0        0     1774 2023-02-09 14:55:10.030448 pycomex-0.8.8/pycomex/examples/quickstart.py
--rwxr-xr-x   0        0        0      249 2023-02-13 21:10:16.382151 pycomex-0.8.8/pycomex/examples/run_experiment.py
--rwxr-xr-x   0        0        0    66277 2023-02-16 19:06:03.939387 pycomex-0.8.8/pycomex/experiment.py
--rwxr-xr-x   0        0        0      865 2023-02-13 19:06:58.700540 pycomex-0.8.8/pycomex/templates/analysis.py.j2
--rwxr-xr-x   0        0        0      336 2022-07-17 07:15:39.751824 pycomex-0.8.8/pycomex/templates/annotations.py.j2
--rwxr-xr-x   0        0        0      464 2022-09-12 19:13:15.159972 pycomex-0.8.8/pycomex/templates/experiment_ended.text.j2
--rwxr-xr-x   0        0        0     1083 2022-09-19 07:16:21.662861 pycomex-0.8.8/pycomex/templates/experiment_info.out.j2
--rwxr-xr-x   0        0        0      389 2022-08-21 07:30:07.791594 pycomex-0.8.8/pycomex/templates/experiment_started.text.j2
--rwxr-xr-x   0        0        0     1106 2022-08-21 08:59:19.545111 pycomex-0.8.8/pycomex/templates/experiment_status.text.j2
--rwxr-xr-x   0        0        0      204 2022-09-18 17:25:07.672803 pycomex-0.8.8/pycomex/templates/list_experiments.out.j2
--rwxr-xr-x   0        0        0     3728 2023-02-13 21:09:19.222087 pycomex-0.8.8/pycomex/testing.py
--rwxr-xr-x   0        0        0     9863 2023-02-13 20:28:25.808003 pycomex-0.8.8/pycomex/util.py
--rwxr-xr-x   0        0        0     1837 2022-07-11 10:00:30.134647 pycomex-0.8.8/pycomex/work.py
--rwxr-xr-x   0        0        0     1325 2023-03-27 10:58:26.809630 pycomex-0.8.8/pyproject.toml
--rwxr-xr-x   0        0        0       37 2022-09-18 15:40:41.988324 pycomex-0.8.8/tests/__init__.py
--rwxr-xr-x   0        0        0      957 2023-01-02 15:46:48.951178 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/000/analysis.py
--rwxr-xr-x   0        0        0      369 2023-01-02 15:46:48.783777 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/000/annotations.rst
--rwxr-xr-x   0        0        0     1900 2023-01-02 15:46:48.783969 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/000/experiment_data.json
--rwxr-xr-x   0        0        0     1127 2023-01-02 15:46:48.785525 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/000/experiment_log.txt
--rwxr-xr-x   0        0        0      341 2023-01-02 15:46:48.784089 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/000/experiment_meta.json
--rwxr-xr-x   0        0        0     1156 2023-01-02 15:46:48.783269 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/000/snapshot.py
--rwxr-xr-x   0        0        0     6923 2023-01-02 15:46:48.950780 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/000/values.pdf
--rwxr-xr-x   0        0        0      957 2023-01-02 15:47:19.128244 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/001/analysis.py
--rwxr-xr-x   0        0        0      369 2023-01-02 15:47:18.914939 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/001/annotations.rst
--rwxr-xr-x   0        0        0     1916 2023-01-02 15:47:18.915253 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/001/experiment_data.json
--rwxr-xr-x   0        0        0     1127 2023-01-02 15:47:18.917195 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/001/experiment_log.txt
--rwxr-xr-x   0        0        0      344 2023-01-02 15:47:18.915489 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/001/experiment_meta.json
--rwxr-xr-x   0        0        0     1156 2023-01-02 15:47:18.914184 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/001/snapshot.py
--rwxr-xr-x   0        0        0     6370 2023-01-02 15:47:19.127694 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/001/values.pdf
--rwxr-xr-x   0        0        0      957 2023-01-02 15:47:30.434164 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/002/analysis.py
--rwxr-xr-x   0        0        0      369 2023-01-02 15:47:30.267263 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/002/annotations.rst
--rwxr-xr-x   0        0        0     1904 2023-01-02 15:47:30.267475 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/002/experiment_data.json
--rwxr-xr-x   0        0        0     1127 2023-01-02 15:47:30.269319 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/002/experiment_log.txt
--rwxr-xr-x   0        0        0      342 2023-01-02 15:47:30.267606 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/002/experiment_meta.json
--rwxr-xr-x   0        0        0     1156 2023-01-02 15:47:30.266744 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/002/snapshot.py
--rwxr-xr-x   0        0        0     6379 2023-01-02 15:47:30.433760 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/002/values.pdf
--rwxr-xr-x   0        0        0      957 2023-01-02 15:49:14.379201 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/003/analysis.py
--rwxr-xr-x   0        0        0      369 2023-01-02 15:49:14.202254 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/003/annotations.rst
--rwxr-xr-x   0        0        0     1896 2023-01-02 15:49:14.202489 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/003/experiment_data.json
--rwxr-xr-x   0        0        0     1127 2023-01-02 15:49:14.204568 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/003/experiment_log.txt
--rwxr-xr-x   0        0        0      342 2023-01-02 15:49:14.202654 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/003/experiment_meta.json
--rwxr-xr-x   0        0        0     1156 2023-01-02 15:49:14.201756 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/003/snapshot.py
--rwxr-xr-x   0        0        0     6391 2023-01-02 15:49:14.378768 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/003/values.pdf
--rwxr-xr-x   0        0        0      957 2023-01-02 15:49:37.467530 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/004/analysis.py
--rwxr-xr-x   0        0        0      369 2023-01-02 15:49:37.287142 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/004/annotations.rst
--rwxr-xr-x   0        0        0     1907 2023-01-02 15:49:37.287342 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/004/experiment_data.json
--rwxr-xr-x   0        0        0     1127 2023-01-02 15:49:37.289004 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/004/experiment_log.txt
--rwxr-xr-x   0        0        0      343 2023-01-02 15:49:37.287471 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/004/experiment_meta.json
--rwxr-xr-x   0        0        0     1156 2023-01-02 15:49:37.286677 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/004/snapshot.py
--rwxr-xr-x   0        0        0     7208 2023-01-02 15:49:37.467104 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/004/values.pdf
--rwxr-xr-x   0        0        0      957 2023-01-02 15:49:50.104737 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/005/analysis.py
--rwxr-xr-x   0        0        0      369 2023-01-02 15:49:49.884836 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/005/annotations.rst
--rwxr-xr-x   0        0        0     1904 2023-01-02 15:49:49.885186 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/005/experiment_data.json
--rwxr-xr-x   0        0        0     1127 2023-01-02 15:49:49.887193 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/005/experiment_log.txt
--rwxr-xr-x   0        0        0      343 2023-01-02 15:49:49.885443 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/005/experiment_meta.json
--rwxr-xr-x   0        0        0     1156 2023-01-02 15:49:49.884027 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/005/snapshot.py
--rwxr-xr-x   0        0        0     5912 2023-01-02 15:49:50.104269 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/005/values.pdf
--rwxr-xr-x   0        0        0      957 2023-01-02 15:50:05.144934 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/006/analysis.py
--rwxr-xr-x   0        0        0      369 2023-01-02 15:50:04.972110 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/006/annotations.rst
--rwxr-xr-x   0        0        0     1901 2023-01-02 15:50:04.972303 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/006/experiment_data.json
--rwxr-xr-x   0        0        0     1127 2023-01-02 15:50:04.973999 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/006/experiment_log.txt
--rwxr-xr-x   0        0        0      344 2023-01-02 15:50:04.972432 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/006/experiment_meta.json
--rwxr-xr-x   0        0        0     1156 2023-01-02 15:50:04.971691 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/006/snapshot.py
--rwxr-xr-x   0        0        0     6456 2023-01-02 15:50:05.144487 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/006/values.pdf
--rwxr-xr-x   0        0        0      978 2023-02-13 21:33:12.322572 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/debug/analysis.py
--rwxr-xr-x   0        0        0      445 2023-02-13 21:33:12.162545 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/debug/annotations.rst
--rwxr-xr-x   0        0        0    21717 2023-02-13 21:33:12.163484 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/debug/experiment_data.json
--rwxr-xr-x   0        0        0     1212 2023-02-13 21:33:12.163961 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/debug/experiment_log.txt
--rwxr-xr-x   0        0        0      487 2023-02-13 21:33:12.163615 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/debug/experiment_meta.json
--rwxr-xr-x   0        0        0       17 2023-02-13 21:33:12.060533 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/debug/mock.txt
--rwxr-xr-x   0        0        0     1856 2023-02-13 21:33:12.322995 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/debug/mock_experiment.py
--rwxr-xr-x   0        0        0     1856 2023-02-13 21:33:12.162004 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/debug/snapshot.py
--rwxr-xr-x   0        0        0     5362 2023-02-13 21:33:12.322200 pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/debug/values.pdf
--rwxr-xr-x   0        0        0      957 2023-01-02 15:50:36.977352 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/000/analysis.py
--rwxr-xr-x   0        0        0      369 2023-01-02 15:50:36.912652 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/000/annotations.rst
--rwxr-xr-x   0        0        0     4944 2023-01-02 15:50:36.913010 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/000/experiment_data.json
--rwxr-xr-x   0        0        0     1245 2023-01-02 15:50:36.913476 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/000/experiment_log.txt
--rwxr-xr-x   0        0        0      343 2023-01-02 15:50:36.913132 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/000/experiment_meta.json
--rwxr-xr-x   0        0        0     1156 2023-01-02 15:50:36.912268 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/000/snapshot.py
--rwxr-xr-x   0        0        0     6365 2023-01-02 15:50:36.976974 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/000/values.pdf
--rwxr-xr-x   0        0        0      957 2023-01-02 15:58:55.049762 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/001/analysis.py
--rwxr-xr-x   0        0        0      369 2023-01-02 15:58:54.870546 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/001/annotations.rst
--rwxr-xr-x   0        0        0     4906 2023-01-02 15:58:54.870877 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/001/experiment_data.json
--rwxr-xr-x   0        0        0     1240 2023-01-02 15:58:54.872601 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/001/experiment_log.txt
--rwxr-xr-x   0        0        0      343 2023-01-02 15:58:54.871028 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/001/experiment_meta.json
--rwxr-xr-x   0        0        0     1156 2023-01-02 15:58:54.870067 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/001/snapshot.py
--rwxr-xr-x   0        0        0     6806 2023-01-02 15:58:55.049272 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/001/values.pdf
--rwxr-xr-x   0        0        0      978 2023-01-20 12:50:07.826043 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/analysis.py
--rwxr-xr-x   0        0        0      445 2023-01-20 12:50:07.761822 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/annotations.rst
--rwxr-xr-x   0        0        0    21901 2023-01-20 12:50:07.762745 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/experiment_data.json
--rwxr-xr-x   0        0        0     1256 2023-01-20 12:50:07.763324 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/experiment_log.txt
--rwxr-xr-x   0        0        0      529 2023-01-20 12:50:07.762911 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/experiment_meta.json
--rwxr-xr-x   0        0        0       17 2023-01-20 12:50:07.659399 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/mock.txt
--rwxr-xr-x   0        0        0     1856 2023-01-20 12:50:07.826589 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/snapshot.py
--rwxr-xr-x   0        0        0     5679 2023-01-20 12:50:07.825661 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/values.pdf
--rwxr-xr-x   0        0        0     1009 2023-02-13 21:33:03.661966 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/analysis.py
--rwxr-xr-x   0        0        0      445 2023-02-13 21:33:03.593862 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/annotations.rst
--rwxr-xr-x   0        0        0     5187 2023-02-13 21:33:03.594188 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/experiment_data.json
--rwxr-xr-x   0        0        0     1260 2023-02-13 21:33:03.594721 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/experiment_log.txt
--rwxr-xr-x   0        0        0      533 2023-02-13 21:33:03.594335 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/experiment_meta.json
--rwxr-xr-x   0        0        0       17 2023-02-13 21:33:03.491556 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/mock.txt
--rwxr-xr-x   0        0        0     1856 2023-02-13 21:33:03.662453 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/mock_experiment.py
--rwxr-xr-x   0        0        0      949 2023-02-13 21:33:03.663008 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/snapshot.py
--rwxr-xr-x   0        0        0     6702 2023-02-13 21:33:03.661604 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/values.pdf
--rwxr-xr-x   0        0        0     1009 2023-02-13 21:33:03.429324 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/debug/analysis.py
--rwxr-xr-x   0        0        0      445 2023-02-13 21:33:03.265929 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/debug/annotations.rst
--rwxr-xr-x   0        0        0     5004 2023-02-13 21:33:03.266314 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/debug/experiment_data.json
--rwxr-xr-x   0        0        0     1211 2023-02-13 21:33:03.267871 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/debug/experiment_log.txt
--rwxr-xr-x   0        0        0      483 2023-02-13 21:33:03.266439 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/debug/experiment_meta.json
--rwxr-xr-x   0        0        0       17 2023-02-13 21:33:03.163977 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/debug/mock.txt
--rwxr-xr-x   0        0        0     1856 2023-02-13 21:33:03.429745 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/debug/mock_experiment.py
--rwxr-xr-x   0        0        0      949 2023-02-13 21:33:03.430210 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/debug/mock_sub_experiment.py
--rwxr-xr-x   0        0        0      949 2023-02-13 21:33:03.265481 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/debug/snapshot.py
--rwxr-xr-x   0        0        0     6725 2023-02-13 21:33:03.428951 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/debug/values.pdf
--rwxr-xr-x   0        0        0     1009 2023-02-13 21:32:58.661913 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/analysis.py
--rwxr-xr-x   0        0        0      445 2023-02-13 21:32:58.590223 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/annotations.rst
--rwxr-xr-x   0        0        0     4954 2023-02-13 21:32:58.590516 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/experiment_data.json
--rwxr-xr-x   0        0        0     1224 2023-02-13 21:32:58.590983 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/experiment_log.txt
--rwxr-xr-x   0        0        0      494 2023-02-13 21:32:58.590646 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/experiment_meta.json
--rwxr-xr-x   0        0        0       17 2023-02-13 21:32:58.488424 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/mock.txt
--rwxr-xr-x   0        0        0     1856 2023-02-13 21:32:58.662299 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/mock_experiment.py
--rwxr-xr-x   0        0        0      949 2023-02-13 21:32:58.662768 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/mock_sub_experiment.py
--rwxr-xr-x   0        0        0      989 2023-02-13 21:32:58.663228 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/mock_sub_sub_experiment.py
--rwxr-xr-x   0        0        0      989 2023-02-13 21:32:58.589836 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/snapshot.py
--rwxr-xr-x   0        0        0     7253 2023-02-13 21:32:58.661572 pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/values.pdf
--rwxr-xr-x   0        0        0       17 2023-01-20 12:33:31.779888 pycomex-0.8.8/tests/assets/mock.txt
--rwxr-xr-x   0        0        0     1856 2023-01-20 12:33:31.710161 pycomex-0.8.8/tests/assets/mock_experiment.py
--rwxr-xr-x   0        0        0      949 2023-01-17 12:51:25.591489 pycomex-0.8.8/tests/assets/mock_sub_experiment.py
--rwxr-xr-x   0        0        0      989 2023-01-27 15:29:38.792716 pycomex-0.8.8/tests/assets/mock_sub_sub_experiment.py
--rwxr-xr-x   0        0        0     7671 2023-02-13 21:33:36.001438 pycomex-0.8.8/tests/example/analysing/000/00_random.txt
--rwxr-xr-x   0        0        0     7571 2023-02-13 21:33:36.004062 pycomex-0.8.8/tests/example/analysing/000/01_random.txt
--rwxr-xr-x   0        0        0     7532 2023-02-13 21:33:36.006843 pycomex-0.8.8/tests/example/analysing/000/02_random.txt
--rwxr-xr-x   0        0        0     7556 2023-02-13 21:33:36.009517 pycomex-0.8.8/tests/example/analysing/000/03_random.txt
--rwxr-xr-x   0        0        0     7655 2023-02-13 21:33:36.011445 pycomex-0.8.8/tests/example/analysing/000/04_random.txt
--rwxr-xr-x   0        0        0     7763 2023-02-13 21:33:36.013563 pycomex-0.8.8/tests/example/analysing/000/05_random.txt
--rwxr-xr-x   0        0        0     7586 2023-02-13 21:33:36.015679 pycomex-0.8.8/tests/example/analysing/000/06_random.txt
--rwxr-xr-x   0        0        0     7649 2023-02-13 21:33:36.017853 pycomex-0.8.8/tests/example/analysing/000/07_random.txt
--rwxr-xr-x   0        0        0     7523 2023-02-13 21:33:36.019954 pycomex-0.8.8/tests/example/analysing/000/08_random.txt
--rwxr-xr-x   0        0        0     7698 2023-02-13 21:33:36.022092 pycomex-0.8.8/tests/example/analysing/000/09_random.txt
--rwxr-xr-x   0        0        0     3887 2023-02-13 21:33:36.041579 pycomex-0.8.8/tests/example/analysing/000/analysing.py
--rwxr-xr-x   0        0        0     1820 2023-02-13 21:33:36.040870 pycomex-0.8.8/tests/example/analysing/000/analysis.py
--rwxr-xr-x   0        0        0      118 2023-02-13 21:33:36.040481 pycomex-0.8.8/tests/example/analysing/000/analysis_results.json
--rwxr-xr-x   0        0        0      782 2023-02-13 21:33:36.024003 pycomex-0.8.8/tests/example/analysing/000/annotations.rst
--rwxr-xr-x   0        0        0     2348 2023-02-13 21:33:36.024343 pycomex-0.8.8/tests/example/analysing/000/experiment_data.json
--rwxr-xr-x   0        0        0     1858 2023-02-13 21:33:36.040554 pycomex-0.8.8/tests/example/analysing/000/experiment_log.txt
--rwxr-xr-x   0        0        0      366 2023-02-13 21:33:36.024611 pycomex-0.8.8/tests/example/analysing/000/experiment_meta.json
--rwxr-xr-x   0        0        0     3887 2023-02-13 21:33:36.023149 pycomex-0.8.8/tests/example/analysing/000/snapshot.py
--rwxr-xr-x   0        0        0     7648 2023-02-13 21:33:35.776773 pycomex-0.8.8/tests/example/basic/000/00_random.txt
--rwxr-xr-x   0        0        0     7565 2023-02-13 21:33:35.779250 pycomex-0.8.8/tests/example/basic/000/01_random.txt
--rwxr-xr-x   0        0        0     7589 2023-02-13 21:33:35.781716 pycomex-0.8.8/tests/example/basic/000/02_random.txt
--rwxr-xr-x   0        0        0     7640 2023-02-13 21:33:35.784178 pycomex-0.8.8/tests/example/basic/000/03_random.txt
--rwxr-xr-x   0        0        0     7565 2023-02-13 21:33:35.786600 pycomex-0.8.8/tests/example/basic/000/04_random.txt
--rwxr-xr-x   0        0        0     7765 2023-02-13 21:33:35.789270 pycomex-0.8.8/tests/example/basic/000/05_random.txt
--rwxr-xr-x   0        0        0     7592 2023-02-13 21:33:35.792338 pycomex-0.8.8/tests/example/basic/000/06_random.txt
--rwxr-xr-x   0        0        0     7559 2023-02-13 21:33:35.795469 pycomex-0.8.8/tests/example/basic/000/07_random.txt
--rwxr-xr-x   0        0        0     7607 2023-02-13 21:33:35.798057 pycomex-0.8.8/tests/example/basic/000/08_random.txt
--rwxr-xr-x   0        0        0     7603 2023-02-13 21:33:35.800467 pycomex-0.8.8/tests/example/basic/000/09_random.txt
--rwxr-xr-x   0        0        0      724 2023-02-13 21:33:35.802073 pycomex-0.8.8/tests/example/basic/000/analysis.py
--rwxr-xr-x   0        0        0      791 2023-02-13 21:33:35.802380 pycomex-0.8.8/tests/example/basic/000/annotations.rst
--rwxr-xr-x   0        0        0     3256 2023-02-13 21:33:35.804827 pycomex-0.8.8/tests/example/basic/000/basic.py
--rwxr-xr-x   0        0        0     2299 2023-02-13 21:33:35.802731 pycomex-0.8.8/tests/example/basic/000/experiment_data.json
--rwxr-xr-x   0        0        0     1735 2023-02-13 21:33:35.803644 pycomex-0.8.8/tests/example/basic/000/experiment_log.txt
--rwxr-xr-x   0        0        0      367 2023-02-13 21:33:35.802997 pycomex-0.8.8/tests/example/basic/000/experiment_meta.json
--rwxr-xr-x   0        0        0     3256 2023-02-13 21:33:35.801532 pycomex-0.8.8/tests/example/basic/000/snapshot.py
--rwxr-xr-x   0        0        0     3759 2023-02-13 21:33:36.280038 pycomex-0.8.8/tests/example/inheritance/debug/00_random.txt
--rwxr-xr-x   0        0        0     3878 2023-02-13 21:33:36.281321 pycomex-0.8.8/tests/example/inheritance/debug/01_random.txt
--rwxr-xr-x   0        0        0     3819 2023-02-13 21:33:36.282733 pycomex-0.8.8/tests/example/inheritance/debug/02_random.txt
--rwxr-xr-x   0        0        0     3887 2023-02-13 21:33:36.301507 pycomex-0.8.8/tests/example/inheritance/debug/analysing.py
--rwxr-xr-x   0        0        0     2000 2023-02-13 21:33:36.314005 pycomex-0.8.8/tests/example/inheritance/debug/analysis.py
--rwxr-xr-x   0        0        0      130 2023-02-13 21:33:36.300308 pycomex-0.8.8/tests/example/inheritance/debug/analysis_results.json
--rwxr-xr-x   0        0        0      656 2023-02-13 21:33:36.284811 pycomex-0.8.8/tests/example/inheritance/debug/annotations.rst
--rwxr-xr-x   0        0        0     1625 2023-02-13 21:33:36.285138 pycomex-0.8.8/tests/example/inheritance/debug/experiment_data.json
--rwxr-xr-x   0        0        0     1585 2023-02-13 21:33:36.313658 pycomex-0.8.8/tests/example/inheritance/debug/experiment_log.txt
--rwxr-xr-x   0        0        0      366 2023-02-13 21:33:36.285405 pycomex-0.8.8/tests/example/inheritance/debug/experiment_meta.json
--rwxr-xr-x   0        0        0     3374 2023-02-13 21:33:36.314792 pycomex-0.8.8/tests/example/inheritance/debug/inheritance.py
--rwxr-xr-x   0        0        0     3374 2023-02-13 21:33:36.283977 pycomex-0.8.8/tests/example/inheritance/debug/snapshot.py
--rwxr-xr-x   0        0        0      980 2023-02-13 21:33:35.547515 pycomex-0.8.8/tests/example/quickstart/000/analysis.py
--rwxr-xr-x   0        0        0      295 2023-02-13 21:33:35.534993 pycomex-0.8.8/tests/example/quickstart/000/annotations.rst
--rwxr-xr-x   0        0        0     1017 2023-02-13 21:33:35.535217 pycomex-0.8.8/tests/example/quickstart/000/experiment_data.json
--rwxr-xr-x   0        0        0     1200 2023-02-13 21:33:35.547197 pycomex-0.8.8/tests/example/quickstart/000/experiment_log.txt
--rwxr-xr-x   0        0        0      369 2023-02-13 21:33:35.535410 pycomex-0.8.8/tests/example/quickstart/000/experiment_meta.json
--rwxr-xr-x   0        0        0       12 2023-02-13 21:33:35.533623 pycomex-0.8.8/tests/example/quickstart/000/hello_world.txt
--rwxr-xr-x   0        0        0     1774 2023-02-13 21:33:35.548177 pycomex-0.8.8/tests/example/quickstart/000/quickstart.py
--rwxr-xr-x   0        0        0     1774 2023-02-13 21:33:35.534359 pycomex-0.8.8/tests/example/quickstart/000/snapshot.py
--rwxr-xr-x   0        0        0      980 2023-02-13 21:33:36.456532 pycomex-0.8.8/tests/example/quickstart/001/analysis.py
--rwxr-xr-x   0        0        0      295 2023-02-13 21:33:36.443361 pycomex-0.8.8/tests/example/quickstart/001/annotations.rst
--rwxr-xr-x   0        0        0     1016 2023-02-13 21:33:36.443650 pycomex-0.8.8/tests/example/quickstart/001/experiment_data.json
--rwxr-xr-x   0        0        0     1200 2023-02-13 21:33:36.456185 pycomex-0.8.8/tests/example/quickstart/001/experiment_log.txt
--rwxr-xr-x   0        0        0      368 2023-02-13 21:33:36.443889 pycomex-0.8.8/tests/example/quickstart/001/experiment_meta.json
--rwxr-xr-x   0        0        0       12 2023-02-13 21:33:36.441753 pycomex-0.8.8/tests/example/quickstart/001/hello_world.txt
--rwxr-xr-x   0        0        0     1774 2023-02-13 21:33:36.457399 pycomex-0.8.8/tests/example/quickstart/001/quickstart.py
--rwxr-xr-x   0        0        0     1774 2023-02-13 21:33:36.442602 pycomex-0.8.8/tests/example/quickstart/001/snapshot.py
--rwxr-xr-x   0        0        0      560 2023-01-03 09:13:00.380908 pycomex-0.8.8/tests/templates/test_experiment_analysis.py.j2
--rwxr-xr-x   0        0        0      400 2022-09-18 15:40:41.988877 pycomex-0.8.8/tests/templates/test_experiment_registry.py.j2
--rwxr-xr-x   0        0        0     2826 2023-01-03 07:25:15.309756 pycomex-0.8.8/tests/test_cli.py
--rwxr-xr-x   0        0        0     3189 2023-02-13 21:33:34.622148 pycomex-0.8.8/tests/test_examples.py
--rwxr-xr-x   0        0        0    33551 2023-02-13 20:57:05.967594 pycomex-0.8.8/tests/test_experiment.py
--rwxr-xr-x   0        0        0     5455 2023-01-02 13:33:12.128124 pycomex-0.8.8/tests/test_experiment_abstract_experiment.py
--rwxr-xr-x   0        0        0     8312 2023-01-27 15:40:33.354393 pycomex-0.8.8/tests/test_experiment_sub_experiment.py
--rwxr-xr-x   0        0        0     3156 2023-02-13 19:50:05.086725 pycomex-0.8.8/tests/test_util.py
--rwxr-xr-x   0        0        0      837 2023-01-02 15:58:44.359970 pycomex-0.8.8/tests/util.py
--rw-r--r--   0        0        0     9108 1970-01-01 00:00:00.000000 pycomex-0.8.8/setup.py
--rw-r--r--   0        0        0     7656 1970-01-01 00:00:00.000000 pycomex-0.8.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1071 2022-07-09 08:06:36.748803 pycomex-0.9.0/LICENSE
+-rwxr-xr-x   0        0        0     6820 2023-02-09 14:59:34.788632 pycomex-0.9.0/README.rst
+-rwxr-xr-x   0        0        0        6 2023-02-24 07:28:31.627843 pycomex-0.9.0/pycomex/VERSION
+-rwxr-xr-x   0        0        0      178 2022-09-19 07:18:59.122787 pycomex-0.9.0/pycomex/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-08-20 17:22:07.854881 pycomex-0.9.0/pycomex/app/__init__.py
+-rwxr-xr-x   0        0        0     7375 2023-01-03 06:49:42.464926 pycomex-0.9.0/pycomex/cli.py
+-rwxr-xr-x   0        0        0      899 2023-02-13 20:56:26.976515 pycomex-0.9.0/pycomex/examples/README.rst
+-rwxr-xr-x   0        0        0     3887 2023-02-13 20:36:41.593997 pycomex-0.9.0/pycomex/examples/analysing.py
+-rwxr-xr-x   0        0        0     3256 2023-02-09 14:55:10.188721 pycomex-0.9.0/pycomex/examples/basic.py
+-rwxr-xr-x   0        0        0     3888 2023-02-16 19:07:05.131685 pycomex-0.9.0/pycomex/examples/example/inheritance/debug/00_random.txt
+-rwxr-xr-x   0        0        0     3793 2023-02-16 19:07:05.133113 pycomex-0.9.0/pycomex/examples/example/inheritance/debug/01_random.txt
+-rwxr-xr-x   0        0        0     3748 2023-02-16 19:07:05.134542 pycomex-0.9.0/pycomex/examples/example/inheritance/debug/02_random.txt
+-rwxr-xr-x   0        0        0     3802 2023-02-16 19:07:05.135962 pycomex-0.9.0/pycomex/examples/example/inheritance/debug/03_random.txt
+-rwxr-xr-x   0        0        0     3843 2023-02-16 19:07:05.137577 pycomex-0.9.0/pycomex/examples/example/inheritance/debug/04_random.txt
+-rwxr-xr-x   0        0        0     3887 2023-02-16 19:07:05.159992 pycomex-0.9.0/pycomex/examples/example/inheritance/debug/analysing.py
+-rwxr-xr-x   0        0        0     2000 2023-02-16 19:07:05.161471 pycomex-0.9.0/pycomex/examples/example/inheritance/debug/analysis.py
+-rwxr-xr-x   0        0        0      118 2023-02-16 19:07:05.158584 pycomex-0.9.0/pycomex/examples/example/inheritance/debug/analysis_results.json
+-rwxr-xr-x   0        0        0      692 2023-02-16 19:07:05.141950 pycomex-0.9.0/pycomex/examples/example/inheritance/debug/annotations.rst
+-rwxr-xr-x   0        0        0     1948 2023-02-16 19:07:05.149422 pycomex-0.9.0/pycomex/examples/example/inheritance/debug/experiment_data.json
+-rwxr-xr-x   0        0        0     1932 2023-02-16 19:07:05.161028 pycomex-0.9.0/pycomex/examples/example/inheritance/debug/experiment_log.txt
+-rwxr-xr-x   0        0        0      367 2023-02-16 19:07:05.149762 pycomex-0.9.0/pycomex/examples/example/inheritance/debug/experiment_meta.json
+-rwxr-xr-x   0        0        0     4712 2023-02-16 19:07:05.139235 pycomex-0.9.0/pycomex/examples/example/inheritance/debug/snapshot.py
+-rwxr-xr-x   0        0        0     5173 2023-02-16 19:10:46.863704 pycomex-0.9.0/pycomex/examples/inheritance.py
+-rwxr-xr-x   0        0        0     1774 2023-02-09 14:55:10.030448 pycomex-0.9.0/pycomex/examples/quickstart.py
+-rwxr-xr-x   0        0        0      249 2023-02-13 21:10:16.382151 pycomex-0.9.0/pycomex/examples/run_experiment.py
+-rwxr-xr-x   0        0        0    66277 2023-02-16 19:06:03.939387 pycomex-0.9.0/pycomex/experiment.py
+-rwxr-xr-x   0        0        0      865 2023-02-13 19:06:58.700540 pycomex-0.9.0/pycomex/templates/analysis.py.j2
+-rwxr-xr-x   0        0        0      336 2022-07-17 07:15:39.751824 pycomex-0.9.0/pycomex/templates/annotations.py.j2
+-rwxr-xr-x   0        0        0      464 2022-09-12 19:13:15.159972 pycomex-0.9.0/pycomex/templates/experiment_ended.text.j2
+-rwxr-xr-x   0        0        0     1083 2022-09-19 07:16:21.662861 pycomex-0.9.0/pycomex/templates/experiment_info.out.j2
+-rwxr-xr-x   0        0        0      389 2022-08-21 07:30:07.791594 pycomex-0.9.0/pycomex/templates/experiment_started.text.j2
+-rwxr-xr-x   0        0        0     1106 2022-08-21 08:59:19.545111 pycomex-0.9.0/pycomex/templates/experiment_status.text.j2
+-rwxr-xr-x   0        0        0      204 2022-09-18 17:25:07.672803 pycomex-0.9.0/pycomex/templates/list_experiments.out.j2
+-rwxr-xr-x   0        0        0     3728 2023-02-13 21:09:19.222087 pycomex-0.9.0/pycomex/testing.py
+-rwxr-xr-x   0        0        0     9863 2023-02-13 20:28:25.808003 pycomex-0.9.0/pycomex/util.py
+-rwxr-xr-x   0        0        0     1837 2022-07-11 10:00:30.134647 pycomex-0.9.0/pycomex/work.py
+-rwxr-xr-x   0        0        0     1325 2023-04-27 14:31:38.449653 pycomex-0.9.0/pyproject.toml
+-rwxr-xr-x   0        0        0       37 2022-09-18 15:40:41.988324 pycomex-0.9.0/tests/__init__.py
+-rwxr-xr-x   0        0        0      957 2023-01-02 15:46:48.951178 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/000/analysis.py
+-rwxr-xr-x   0        0        0      369 2023-01-02 15:46:48.783777 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/000/annotations.rst
+-rwxr-xr-x   0        0        0     1900 2023-01-02 15:46:48.783969 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/000/experiment_data.json
+-rwxr-xr-x   0        0        0     1127 2023-01-02 15:46:48.785525 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/000/experiment_log.txt
+-rwxr-xr-x   0        0        0      341 2023-01-02 15:46:48.784089 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/000/experiment_meta.json
+-rwxr-xr-x   0        0        0     1156 2023-01-02 15:46:48.783269 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/000/snapshot.py
+-rwxr-xr-x   0        0        0     6923 2023-01-02 15:46:48.950780 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/000/values.pdf
+-rwxr-xr-x   0        0        0      957 2023-01-02 15:47:19.128244 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/001/analysis.py
+-rwxr-xr-x   0        0        0      369 2023-01-02 15:47:18.914939 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/001/annotations.rst
+-rwxr-xr-x   0        0        0     1916 2023-01-02 15:47:18.915253 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/001/experiment_data.json
+-rwxr-xr-x   0        0        0     1127 2023-01-02 15:47:18.917195 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/001/experiment_log.txt
+-rwxr-xr-x   0        0        0      344 2023-01-02 15:47:18.915489 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/001/experiment_meta.json
+-rwxr-xr-x   0        0        0     1156 2023-01-02 15:47:18.914184 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/001/snapshot.py
+-rwxr-xr-x   0        0        0     6370 2023-01-02 15:47:19.127694 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/001/values.pdf
+-rwxr-xr-x   0        0        0      957 2023-01-02 15:47:30.434164 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/002/analysis.py
+-rwxr-xr-x   0        0        0      369 2023-01-02 15:47:30.267263 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/002/annotations.rst
+-rwxr-xr-x   0        0        0     1904 2023-01-02 15:47:30.267475 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/002/experiment_data.json
+-rwxr-xr-x   0        0        0     1127 2023-01-02 15:47:30.269319 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/002/experiment_log.txt
+-rwxr-xr-x   0        0        0      342 2023-01-02 15:47:30.267606 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/002/experiment_meta.json
+-rwxr-xr-x   0        0        0     1156 2023-01-02 15:47:30.266744 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/002/snapshot.py
+-rwxr-xr-x   0        0        0     6379 2023-01-02 15:47:30.433760 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/002/values.pdf
+-rwxr-xr-x   0        0        0      957 2023-01-02 15:49:14.379201 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/003/analysis.py
+-rwxr-xr-x   0        0        0      369 2023-01-02 15:49:14.202254 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/003/annotations.rst
+-rwxr-xr-x   0        0        0     1896 2023-01-02 15:49:14.202489 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/003/experiment_data.json
+-rwxr-xr-x   0        0        0     1127 2023-01-02 15:49:14.204568 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/003/experiment_log.txt
+-rwxr-xr-x   0        0        0      342 2023-01-02 15:49:14.202654 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/003/experiment_meta.json
+-rwxr-xr-x   0        0        0     1156 2023-01-02 15:49:14.201756 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/003/snapshot.py
+-rwxr-xr-x   0        0        0     6391 2023-01-02 15:49:14.378768 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/003/values.pdf
+-rwxr-xr-x   0        0        0      957 2023-01-02 15:49:37.467530 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/004/analysis.py
+-rwxr-xr-x   0        0        0      369 2023-01-02 15:49:37.287142 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/004/annotations.rst
+-rwxr-xr-x   0        0        0     1907 2023-01-02 15:49:37.287342 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/004/experiment_data.json
+-rwxr-xr-x   0        0        0     1127 2023-01-02 15:49:37.289004 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/004/experiment_log.txt
+-rwxr-xr-x   0        0        0      343 2023-01-02 15:49:37.287471 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/004/experiment_meta.json
+-rwxr-xr-x   0        0        0     1156 2023-01-02 15:49:37.286677 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/004/snapshot.py
+-rwxr-xr-x   0        0        0     7208 2023-01-02 15:49:37.467104 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/004/values.pdf
+-rwxr-xr-x   0        0        0      957 2023-01-02 15:49:50.104737 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/005/analysis.py
+-rwxr-xr-x   0        0        0      369 2023-01-02 15:49:49.884836 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/005/annotations.rst
+-rwxr-xr-x   0        0        0     1904 2023-01-02 15:49:49.885186 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/005/experiment_data.json
+-rwxr-xr-x   0        0        0     1127 2023-01-02 15:49:49.887193 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/005/experiment_log.txt
+-rwxr-xr-x   0        0        0      343 2023-01-02 15:49:49.885443 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/005/experiment_meta.json
+-rwxr-xr-x   0        0        0     1156 2023-01-02 15:49:49.884027 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/005/snapshot.py
+-rwxr-xr-x   0        0        0     5912 2023-01-02 15:49:50.104269 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/005/values.pdf
+-rwxr-xr-x   0        0        0      957 2023-01-02 15:50:05.144934 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/006/analysis.py
+-rwxr-xr-x   0        0        0      369 2023-01-02 15:50:04.972110 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/006/annotations.rst
+-rwxr-xr-x   0        0        0     1901 2023-01-02 15:50:04.972303 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/006/experiment_data.json
+-rwxr-xr-x   0        0        0     1127 2023-01-02 15:50:04.973999 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/006/experiment_log.txt
+-rwxr-xr-x   0        0        0      344 2023-01-02 15:50:04.972432 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/006/experiment_meta.json
+-rwxr-xr-x   0        0        0     1156 2023-01-02 15:50:04.971691 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/006/snapshot.py
+-rwxr-xr-x   0        0        0     6456 2023-01-02 15:50:05.144487 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/006/values.pdf
+-rwxr-xr-x   0        0        0      978 2023-02-13 21:33:12.322572 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/debug/analysis.py
+-rwxr-xr-x   0        0        0      445 2023-02-13 21:33:12.162545 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/debug/annotations.rst
+-rwxr-xr-x   0        0        0    21717 2023-02-13 21:33:12.163484 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/debug/experiment_data.json
+-rwxr-xr-x   0        0        0     1212 2023-02-13 21:33:12.163961 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/debug/experiment_log.txt
+-rwxr-xr-x   0        0        0      487 2023-02-13 21:33:12.163615 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/debug/experiment_meta.json
+-rwxr-xr-x   0        0        0       17 2023-02-13 21:33:12.060533 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/debug/mock.txt
+-rwxr-xr-x   0        0        0     1856 2023-02-13 21:33:12.322995 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/debug/mock_experiment.py
+-rwxr-xr-x   0        0        0     1856 2023-02-13 21:33:12.162004 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/debug/snapshot.py
+-rwxr-xr-x   0        0        0     5362 2023-02-13 21:33:12.322200 pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/debug/values.pdf
+-rwxr-xr-x   0        0        0      957 2023-01-02 15:50:36.977352 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/000/analysis.py
+-rwxr-xr-x   0        0        0      369 2023-01-02 15:50:36.912652 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/000/annotations.rst
+-rwxr-xr-x   0        0        0     4944 2023-01-02 15:50:36.913010 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/000/experiment_data.json
+-rwxr-xr-x   0        0        0     1245 2023-01-02 15:50:36.913476 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/000/experiment_log.txt
+-rwxr-xr-x   0        0        0      343 2023-01-02 15:50:36.913132 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/000/experiment_meta.json
+-rwxr-xr-x   0        0        0     1156 2023-01-02 15:50:36.912268 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/000/snapshot.py
+-rwxr-xr-x   0        0        0     6365 2023-01-02 15:50:36.976974 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/000/values.pdf
+-rwxr-xr-x   0        0        0      957 2023-01-02 15:58:55.049762 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/001/analysis.py
+-rwxr-xr-x   0        0        0      369 2023-01-02 15:58:54.870546 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/001/annotations.rst
+-rwxr-xr-x   0        0        0     4906 2023-01-02 15:58:54.870877 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/001/experiment_data.json
+-rwxr-xr-x   0        0        0     1240 2023-01-02 15:58:54.872601 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/001/experiment_log.txt
+-rwxr-xr-x   0        0        0      343 2023-01-02 15:58:54.871028 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/001/experiment_meta.json
+-rwxr-xr-x   0        0        0     1156 2023-01-02 15:58:54.870067 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/001/snapshot.py
+-rwxr-xr-x   0        0        0     6806 2023-01-02 15:58:55.049272 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/001/values.pdf
+-rwxr-xr-x   0        0        0      978 2023-01-20 12:50:07.826043 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/analysis.py
+-rwxr-xr-x   0        0        0      445 2023-01-20 12:50:07.761822 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/annotations.rst
+-rwxr-xr-x   0        0        0    21901 2023-01-20 12:50:07.762745 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/experiment_data.json
+-rwxr-xr-x   0        0        0     1256 2023-01-20 12:50:07.763324 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/experiment_log.txt
+-rwxr-xr-x   0        0        0      529 2023-01-20 12:50:07.762911 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/experiment_meta.json
+-rwxr-xr-x   0        0        0       17 2023-01-20 12:50:07.659399 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/mock.txt
+-rwxr-xr-x   0        0        0     1856 2023-01-20 12:50:07.826589 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/snapshot.py
+-rwxr-xr-x   0        0        0     5679 2023-01-20 12:50:07.825661 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/values.pdf
+-rwxr-xr-x   0        0        0     1009 2023-02-13 21:33:03.661966 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/analysis.py
+-rwxr-xr-x   0        0        0      445 2023-02-13 21:33:03.593862 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/annotations.rst
+-rwxr-xr-x   0        0        0     5187 2023-02-13 21:33:03.594188 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/experiment_data.json
+-rwxr-xr-x   0        0        0     1260 2023-02-13 21:33:03.594721 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/experiment_log.txt
+-rwxr-xr-x   0        0        0      533 2023-02-13 21:33:03.594335 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/experiment_meta.json
+-rwxr-xr-x   0        0        0       17 2023-02-13 21:33:03.491556 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/mock.txt
+-rwxr-xr-x   0        0        0     1856 2023-02-13 21:33:03.662453 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/mock_experiment.py
+-rwxr-xr-x   0        0        0      949 2023-02-13 21:33:03.663008 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/snapshot.py
+-rwxr-xr-x   0        0        0     6702 2023-02-13 21:33:03.661604 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/values.pdf
+-rwxr-xr-x   0        0        0     1009 2023-02-13 21:33:03.429324 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/debug/analysis.py
+-rwxr-xr-x   0        0        0      445 2023-02-13 21:33:03.265929 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/debug/annotations.rst
+-rwxr-xr-x   0        0        0     5004 2023-02-13 21:33:03.266314 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/debug/experiment_data.json
+-rwxr-xr-x   0        0        0     1211 2023-02-13 21:33:03.267871 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/debug/experiment_log.txt
+-rwxr-xr-x   0        0        0      483 2023-02-13 21:33:03.266439 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/debug/experiment_meta.json
+-rwxr-xr-x   0        0        0       17 2023-02-13 21:33:03.163977 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/debug/mock.txt
+-rwxr-xr-x   0        0        0     1856 2023-02-13 21:33:03.429745 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/debug/mock_experiment.py
+-rwxr-xr-x   0        0        0      949 2023-02-13 21:33:03.430210 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/debug/mock_sub_experiment.py
+-rwxr-xr-x   0        0        0      949 2023-02-13 21:33:03.265481 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/debug/snapshot.py
+-rwxr-xr-x   0        0        0     6725 2023-02-13 21:33:03.428951 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/debug/values.pdf
+-rwxr-xr-x   0        0        0     1009 2023-02-13 21:32:58.661913 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/analysis.py
+-rwxr-xr-x   0        0        0      445 2023-02-13 21:32:58.590223 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/annotations.rst
+-rwxr-xr-x   0        0        0     4954 2023-02-13 21:32:58.590516 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/experiment_data.json
+-rwxr-xr-x   0        0        0     1224 2023-02-13 21:32:58.590983 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/experiment_log.txt
+-rwxr-xr-x   0        0        0      494 2023-02-13 21:32:58.590646 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/experiment_meta.json
+-rwxr-xr-x   0        0        0       17 2023-02-13 21:32:58.488424 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/mock.txt
+-rwxr-xr-x   0        0        0     1856 2023-02-13 21:32:58.662299 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/mock_experiment.py
+-rwxr-xr-x   0        0        0      949 2023-02-13 21:32:58.662768 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/mock_sub_experiment.py
+-rwxr-xr-x   0        0        0      989 2023-02-13 21:32:58.663228 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/mock_sub_sub_experiment.py
+-rwxr-xr-x   0        0        0      989 2023-02-13 21:32:58.589836 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/snapshot.py
+-rwxr-xr-x   0        0        0     7253 2023-02-13 21:32:58.661572 pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/values.pdf
+-rwxr-xr-x   0        0        0       17 2023-01-20 12:33:31.779888 pycomex-0.9.0/tests/assets/mock.txt
+-rwxr-xr-x   0        0        0     1856 2023-01-20 12:33:31.710161 pycomex-0.9.0/tests/assets/mock_experiment.py
+-rwxr-xr-x   0        0        0      949 2023-01-17 12:51:25.591489 pycomex-0.9.0/tests/assets/mock_sub_experiment.py
+-rwxr-xr-x   0        0        0      989 2023-01-27 15:29:38.792716 pycomex-0.9.0/tests/assets/mock_sub_sub_experiment.py
+-rwxr-xr-x   0        0        0     7671 2023-02-13 21:33:36.001438 pycomex-0.9.0/tests/example/analysing/000/00_random.txt
+-rwxr-xr-x   0        0        0     7571 2023-02-13 21:33:36.004062 pycomex-0.9.0/tests/example/analysing/000/01_random.txt
+-rwxr-xr-x   0        0        0     7532 2023-02-13 21:33:36.006843 pycomex-0.9.0/tests/example/analysing/000/02_random.txt
+-rwxr-xr-x   0        0        0     7556 2023-02-13 21:33:36.009517 pycomex-0.9.0/tests/example/analysing/000/03_random.txt
+-rwxr-xr-x   0        0        0     7655 2023-02-13 21:33:36.011445 pycomex-0.9.0/tests/example/analysing/000/04_random.txt
+-rwxr-xr-x   0        0        0     7763 2023-02-13 21:33:36.013563 pycomex-0.9.0/tests/example/analysing/000/05_random.txt
+-rwxr-xr-x   0        0        0     7586 2023-02-13 21:33:36.015679 pycomex-0.9.0/tests/example/analysing/000/06_random.txt
+-rwxr-xr-x   0        0        0     7649 2023-02-13 21:33:36.017853 pycomex-0.9.0/tests/example/analysing/000/07_random.txt
+-rwxr-xr-x   0        0        0     7523 2023-02-13 21:33:36.019954 pycomex-0.9.0/tests/example/analysing/000/08_random.txt
+-rwxr-xr-x   0        0        0     7698 2023-02-13 21:33:36.022092 pycomex-0.9.0/tests/example/analysing/000/09_random.txt
+-rwxr-xr-x   0        0        0     3887 2023-02-13 21:33:36.041579 pycomex-0.9.0/tests/example/analysing/000/analysing.py
+-rwxr-xr-x   0        0        0     1820 2023-02-13 21:33:36.040870 pycomex-0.9.0/tests/example/analysing/000/analysis.py
+-rwxr-xr-x   0        0        0      118 2023-02-13 21:33:36.040481 pycomex-0.9.0/tests/example/analysing/000/analysis_results.json
+-rwxr-xr-x   0        0        0      782 2023-02-13 21:33:36.024003 pycomex-0.9.0/tests/example/analysing/000/annotations.rst
+-rwxr-xr-x   0        0        0     2348 2023-02-13 21:33:36.024343 pycomex-0.9.0/tests/example/analysing/000/experiment_data.json
+-rwxr-xr-x   0        0        0     1858 2023-02-13 21:33:36.040554 pycomex-0.9.0/tests/example/analysing/000/experiment_log.txt
+-rwxr-xr-x   0        0        0      366 2023-02-13 21:33:36.024611 pycomex-0.9.0/tests/example/analysing/000/experiment_meta.json
+-rwxr-xr-x   0        0        0     3887 2023-02-13 21:33:36.023149 pycomex-0.9.0/tests/example/analysing/000/snapshot.py
+-rwxr-xr-x   0        0        0     7648 2023-02-13 21:33:35.776773 pycomex-0.9.0/tests/example/basic/000/00_random.txt
+-rwxr-xr-x   0        0        0     7565 2023-02-13 21:33:35.779250 pycomex-0.9.0/tests/example/basic/000/01_random.txt
+-rwxr-xr-x   0        0        0     7589 2023-02-13 21:33:35.781716 pycomex-0.9.0/tests/example/basic/000/02_random.txt
+-rwxr-xr-x   0        0        0     7640 2023-02-13 21:33:35.784178 pycomex-0.9.0/tests/example/basic/000/03_random.txt
+-rwxr-xr-x   0        0        0     7565 2023-02-13 21:33:35.786600 pycomex-0.9.0/tests/example/basic/000/04_random.txt
+-rwxr-xr-x   0        0        0     7765 2023-02-13 21:33:35.789270 pycomex-0.9.0/tests/example/basic/000/05_random.txt
+-rwxr-xr-x   0        0        0     7592 2023-02-13 21:33:35.792338 pycomex-0.9.0/tests/example/basic/000/06_random.txt
+-rwxr-xr-x   0        0        0     7559 2023-02-13 21:33:35.795469 pycomex-0.9.0/tests/example/basic/000/07_random.txt
+-rwxr-xr-x   0        0        0     7607 2023-02-13 21:33:35.798057 pycomex-0.9.0/tests/example/basic/000/08_random.txt
+-rwxr-xr-x   0        0        0     7603 2023-02-13 21:33:35.800467 pycomex-0.9.0/tests/example/basic/000/09_random.txt
+-rwxr-xr-x   0        0        0      724 2023-02-13 21:33:35.802073 pycomex-0.9.0/tests/example/basic/000/analysis.py
+-rwxr-xr-x   0        0        0      791 2023-02-13 21:33:35.802380 pycomex-0.9.0/tests/example/basic/000/annotations.rst
+-rwxr-xr-x   0        0        0     3256 2023-02-13 21:33:35.804827 pycomex-0.9.0/tests/example/basic/000/basic.py
+-rwxr-xr-x   0        0        0     2299 2023-02-13 21:33:35.802731 pycomex-0.9.0/tests/example/basic/000/experiment_data.json
+-rwxr-xr-x   0        0        0     1735 2023-02-13 21:33:35.803644 pycomex-0.9.0/tests/example/basic/000/experiment_log.txt
+-rwxr-xr-x   0        0        0      367 2023-02-13 21:33:35.802997 pycomex-0.9.0/tests/example/basic/000/experiment_meta.json
+-rwxr-xr-x   0        0        0     3256 2023-02-13 21:33:35.801532 pycomex-0.9.0/tests/example/basic/000/snapshot.py
+-rwxr-xr-x   0        0        0     3759 2023-02-13 21:33:36.280038 pycomex-0.9.0/tests/example/inheritance/debug/00_random.txt
+-rwxr-xr-x   0        0        0     3878 2023-02-13 21:33:36.281321 pycomex-0.9.0/tests/example/inheritance/debug/01_random.txt
+-rwxr-xr-x   0        0        0     3819 2023-02-13 21:33:36.282733 pycomex-0.9.0/tests/example/inheritance/debug/02_random.txt
+-rwxr-xr-x   0        0        0     3887 2023-02-13 21:33:36.301507 pycomex-0.9.0/tests/example/inheritance/debug/analysing.py
+-rwxr-xr-x   0        0        0     2000 2023-02-13 21:33:36.314005 pycomex-0.9.0/tests/example/inheritance/debug/analysis.py
+-rwxr-xr-x   0        0        0      130 2023-02-13 21:33:36.300308 pycomex-0.9.0/tests/example/inheritance/debug/analysis_results.json
+-rwxr-xr-x   0        0        0      656 2023-02-13 21:33:36.284811 pycomex-0.9.0/tests/example/inheritance/debug/annotations.rst
+-rwxr-xr-x   0        0        0     1625 2023-02-13 21:33:36.285138 pycomex-0.9.0/tests/example/inheritance/debug/experiment_data.json
+-rwxr-xr-x   0        0        0     1585 2023-02-13 21:33:36.313658 pycomex-0.9.0/tests/example/inheritance/debug/experiment_log.txt
+-rwxr-xr-x   0        0        0      366 2023-02-13 21:33:36.285405 pycomex-0.9.0/tests/example/inheritance/debug/experiment_meta.json
+-rwxr-xr-x   0        0        0     3374 2023-02-13 21:33:36.314792 pycomex-0.9.0/tests/example/inheritance/debug/inheritance.py
+-rwxr-xr-x   0        0        0     3374 2023-02-13 21:33:36.283977 pycomex-0.9.0/tests/example/inheritance/debug/snapshot.py
+-rwxr-xr-x   0        0        0      980 2023-02-13 21:33:35.547515 pycomex-0.9.0/tests/example/quickstart/000/analysis.py
+-rwxr-xr-x   0        0        0      295 2023-02-13 21:33:35.534993 pycomex-0.9.0/tests/example/quickstart/000/annotations.rst
+-rwxr-xr-x   0        0        0     1017 2023-02-13 21:33:35.535217 pycomex-0.9.0/tests/example/quickstart/000/experiment_data.json
+-rwxr-xr-x   0        0        0     1200 2023-02-13 21:33:35.547197 pycomex-0.9.0/tests/example/quickstart/000/experiment_log.txt
+-rwxr-xr-x   0        0        0      369 2023-02-13 21:33:35.535410 pycomex-0.9.0/tests/example/quickstart/000/experiment_meta.json
+-rwxr-xr-x   0        0        0       12 2023-02-13 21:33:35.533623 pycomex-0.9.0/tests/example/quickstart/000/hello_world.txt
+-rwxr-xr-x   0        0        0     1774 2023-02-13 21:33:35.548177 pycomex-0.9.0/tests/example/quickstart/000/quickstart.py
+-rwxr-xr-x   0        0        0     1774 2023-02-13 21:33:35.534359 pycomex-0.9.0/tests/example/quickstart/000/snapshot.py
+-rwxr-xr-x   0        0        0      980 2023-02-13 21:33:36.456532 pycomex-0.9.0/tests/example/quickstart/001/analysis.py
+-rwxr-xr-x   0        0        0      295 2023-02-13 21:33:36.443361 pycomex-0.9.0/tests/example/quickstart/001/annotations.rst
+-rwxr-xr-x   0        0        0     1016 2023-02-13 21:33:36.443650 pycomex-0.9.0/tests/example/quickstart/001/experiment_data.json
+-rwxr-xr-x   0        0        0     1200 2023-02-13 21:33:36.456185 pycomex-0.9.0/tests/example/quickstart/001/experiment_log.txt
+-rwxr-xr-x   0        0        0      368 2023-02-13 21:33:36.443889 pycomex-0.9.0/tests/example/quickstart/001/experiment_meta.json
+-rwxr-xr-x   0        0        0       12 2023-02-13 21:33:36.441753 pycomex-0.9.0/tests/example/quickstart/001/hello_world.txt
+-rwxr-xr-x   0        0        0     1774 2023-02-13 21:33:36.457399 pycomex-0.9.0/tests/example/quickstart/001/quickstart.py
+-rwxr-xr-x   0        0        0     1774 2023-02-13 21:33:36.442602 pycomex-0.9.0/tests/example/quickstart/001/snapshot.py
+-rwxr-xr-x   0        0        0      560 2023-01-03 09:13:00.380908 pycomex-0.9.0/tests/templates/test_experiment_analysis.py.j2
+-rwxr-xr-x   0        0        0      400 2022-09-18 15:40:41.988877 pycomex-0.9.0/tests/templates/test_experiment_registry.py.j2
+-rwxr-xr-x   0        0        0     2826 2023-01-03 07:25:15.309756 pycomex-0.9.0/tests/test_cli.py
+-rwxr-xr-x   0        0        0     3189 2023-02-13 21:33:34.622148 pycomex-0.9.0/tests/test_examples.py
+-rwxr-xr-x   0        0        0    33551 2023-02-13 20:57:05.967594 pycomex-0.9.0/tests/test_experiment.py
+-rwxr-xr-x   0        0        0     5455 2023-01-02 13:33:12.128124 pycomex-0.9.0/tests/test_experiment_abstract_experiment.py
+-rwxr-xr-x   0        0        0     8312 2023-01-27 15:40:33.354393 pycomex-0.9.0/tests/test_experiment_sub_experiment.py
+-rwxr-xr-x   0        0        0     3156 2023-02-13 19:50:05.086725 pycomex-0.9.0/tests/test_util.py
+-rwxr-xr-x   0        0        0      837 2023-01-02 15:58:44.359970 pycomex-0.9.0/tests/util.py
+-rw-r--r--   0        0        0     9108 1970-01-01 00:00:00.000000 pycomex-0.9.0/setup.py
+-rw-r--r--   0        0        0     7707 1970-01-01 00:00:00.000000 pycomex-0.9.0/PKG-INFO
```

### Comparing `pycomex-0.8.8/LICENSE` & `pycomex-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/README.rst` & `pycomex-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/cli.py` & `pycomex-0.9.0/pycomex/cli.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/examples/README.rst` & `pycomex-0.9.0/pycomex/examples/README.rst`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/examples/analysing.py` & `pycomex-0.9.0/pycomex/examples/analysing.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/examples/basic.py` & `pycomex-0.9.0/pycomex/examples/basic.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/examples/example/inheritance/debug/00_random.txt` & `pycomex-0.9.0/pycomex/examples/example/inheritance/debug/00_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/examples/example/inheritance/debug/01_random.txt` & `pycomex-0.9.0/pycomex/examples/example/inheritance/debug/01_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/examples/example/inheritance/debug/02_random.txt` & `pycomex-0.9.0/pycomex/examples/example/inheritance/debug/02_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/examples/example/inheritance/debug/03_random.txt` & `pycomex-0.9.0/pycomex/examples/example/inheritance/debug/03_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/examples/example/inheritance/debug/04_random.txt` & `pycomex-0.9.0/pycomex/examples/example/inheritance/debug/04_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/examples/example/inheritance/debug/analysing.py` & `pycomex-0.9.0/pycomex/examples/example/inheritance/debug/analysing.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/examples/example/inheritance/debug/analysis.py` & `pycomex-0.9.0/pycomex/examples/example/inheritance/debug/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/examples/example/inheritance/debug/annotations.rst` & `pycomex-0.9.0/pycomex/examples/example/inheritance/debug/annotations.rst`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/examples/example/inheritance/debug/experiment_data.json` & `pycomex-0.9.0/pycomex/examples/example/inheritance/debug/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/examples/example/inheritance/debug/experiment_log.txt` & `pycomex-0.9.0/pycomex/examples/example/inheritance/debug/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/examples/example/inheritance/debug/snapshot.py` & `pycomex-0.9.0/pycomex/examples/example/inheritance/debug/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/examples/inheritance.py` & `pycomex-0.9.0/pycomex/examples/inheritance.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/examples/quickstart.py` & `pycomex-0.9.0/pycomex/examples/quickstart.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/experiment.py` & `pycomex-0.9.0/pycomex/experiment.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/templates/analysis.py.j2` & `pycomex-0.9.0/pycomex/templates/analysis.py.j2`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/templates/experiment_info.out.j2` & `pycomex-0.9.0/pycomex/templates/experiment_info.out.j2`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/templates/experiment_status.text.j2` & `pycomex-0.9.0/pycomex/templates/experiment_status.text.j2`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/testing.py` & `pycomex-0.9.0/pycomex/testing.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/util.py` & `pycomex-0.9.0/pycomex/util.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pycomex/work.py` & `pycomex-0.9.0/pycomex/work.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/pyproject.toml` & `pycomex-0.9.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry.core>=1.2.0b2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pycomex"
-version = "0.8.8"
+version = "0.9.0"
 description = "Python Computational Experiments"
 license = "MIT"
 authors = ["Jonas Teufel <jonseb1998@gmail.com>"]
 maintainers = ["Jonas Teufel <jonseb1998@gmail.com>"]
 readme = "README.rst"
 documentation = "https://pycomex.readthedocs.io"
 keywords = ["computational experiments", "data science", "maschine learning", "academia"]
```

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/000/analysis.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/000/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/000/experiment_data.json` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/000/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/000/experiment_log.txt` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/000/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/000/snapshot.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/000/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/000/values.pdf` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/000/values.pdf`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/001/analysis.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/001/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/001/experiment_data.json` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/001/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/001/experiment_log.txt` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/001/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/001/snapshot.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/001/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/001/values.pdf` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/001/values.pdf`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/002/analysis.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/002/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/002/experiment_data.json` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/002/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/002/experiment_log.txt` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/002/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/002/snapshot.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/002/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/002/values.pdf` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/002/values.pdf`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/003/analysis.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/003/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/003/experiment_data.json` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/003/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/003/experiment_log.txt` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/003/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/003/snapshot.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/003/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/003/values.pdf` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/003/values.pdf`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/004/analysis.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/004/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/004/experiment_data.json` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/004/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/004/experiment_log.txt` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/004/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/004/snapshot.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/004/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/004/values.pdf` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/004/values.pdf`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/005/analysis.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/005/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/005/experiment_data.json` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/005/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/005/experiment_log.txt` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/005/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/005/snapshot.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/005/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/005/values.pdf` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/005/values.pdf`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/006/analysis.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/006/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/006/experiment_data.json` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/006/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/006/experiment_log.txt` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/006/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/006/snapshot.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/006/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/006/values.pdf` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/006/values.pdf`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/debug/analysis.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/debug/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/debug/experiment_data.json` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/debug/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/debug/experiment_log.txt` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/debug/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/debug/mock_experiment.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/debug/mock_experiment.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/debug/snapshot.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/debug/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_experiment/debug/values.pdf` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_experiment/debug/values.pdf`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/000/analysis.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/000/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/000/experiment_data.json` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/000/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/000/experiment_log.txt` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/000/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/000/snapshot.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/000/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/000/values.pdf` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/000/values.pdf`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/001/analysis.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/001/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/001/experiment_data.json` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/001/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/001/experiment_log.txt` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/001/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/001/snapshot.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/001/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/001/values.pdf` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/001/values.pdf`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/analysis.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/experiment_data.json` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/experiment_log.txt` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/experiment_meta.json` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/experiment_meta.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/snapshot.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/values.pdf` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_experiment/debug/values.pdf`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/analysis.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/experiment_data.json` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/experiment_log.txt` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/experiment_meta.json` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/experiment_meta.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/mock_experiment.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/mock_experiment.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/snapshot.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/values.pdf` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/artifacts/experiment_results/mock_sub_experiment/debug/values.pdf`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/debug/analysis.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/debug/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/debug/experiment_data.json` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/debug/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/debug/experiment_log.txt` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/debug/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/debug/mock_experiment.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/debug/mock_experiment.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/debug/mock_sub_experiment.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/debug/mock_sub_experiment.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/debug/snapshot.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/debug/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_experiment/debug/values.pdf` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_experiment/debug/values.pdf`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/analysis.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/experiment_data.json` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/experiment_log.txt` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/mock_experiment.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/mock_experiment.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/mock_sub_experiment.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/mock_sub_experiment.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/mock_sub_sub_experiment.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/mock_sub_sub_experiment.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/snapshot.py` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/values.pdf` & `pycomex-0.9.0/tests/artifacts/experiment_results/mock_sub_sub_experiment/debug/values.pdf`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/assets/mock_experiment.py` & `pycomex-0.9.0/tests/assets/mock_experiment.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/assets/mock_sub_experiment.py` & `pycomex-0.9.0/tests/assets/mock_sub_experiment.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/assets/mock_sub_sub_experiment.py` & `pycomex-0.9.0/tests/assets/mock_sub_sub_experiment.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/analysing/000/00_random.txt` & `pycomex-0.9.0/tests/example/analysing/000/00_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/analysing/000/01_random.txt` & `pycomex-0.9.0/tests/example/analysing/000/01_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/analysing/000/02_random.txt` & `pycomex-0.9.0/tests/example/analysing/000/02_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/analysing/000/03_random.txt` & `pycomex-0.9.0/tests/example/analysing/000/03_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/analysing/000/04_random.txt` & `pycomex-0.9.0/tests/example/analysing/000/04_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/analysing/000/05_random.txt` & `pycomex-0.9.0/tests/example/analysing/000/05_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/analysing/000/06_random.txt` & `pycomex-0.9.0/tests/example/analysing/000/06_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/analysing/000/07_random.txt` & `pycomex-0.9.0/tests/example/analysing/000/07_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/analysing/000/08_random.txt` & `pycomex-0.9.0/tests/example/analysing/000/08_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/analysing/000/09_random.txt` & `pycomex-0.9.0/tests/example/analysing/000/09_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/analysing/000/analysing.py` & `pycomex-0.9.0/tests/example/analysing/000/analysing.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/analysing/000/analysis.py` & `pycomex-0.9.0/tests/example/analysing/000/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/analysing/000/annotations.rst` & `pycomex-0.9.0/tests/example/analysing/000/annotations.rst`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/analysing/000/experiment_data.json` & `pycomex-0.9.0/tests/example/analysing/000/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/analysing/000/experiment_log.txt` & `pycomex-0.9.0/tests/example/analysing/000/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/analysing/000/snapshot.py` & `pycomex-0.9.0/tests/example/analysing/000/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/basic/000/00_random.txt` & `pycomex-0.9.0/tests/example/basic/000/00_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/basic/000/01_random.txt` & `pycomex-0.9.0/tests/example/basic/000/01_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/basic/000/02_random.txt` & `pycomex-0.9.0/tests/example/basic/000/02_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/basic/000/03_random.txt` & `pycomex-0.9.0/tests/example/basic/000/03_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/basic/000/04_random.txt` & `pycomex-0.9.0/tests/example/basic/000/04_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/basic/000/05_random.txt` & `pycomex-0.9.0/tests/example/basic/000/05_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/basic/000/06_random.txt` & `pycomex-0.9.0/tests/example/basic/000/06_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/basic/000/07_random.txt` & `pycomex-0.9.0/tests/example/basic/000/07_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/basic/000/08_random.txt` & `pycomex-0.9.0/tests/example/basic/000/08_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/basic/000/09_random.txt` & `pycomex-0.9.0/tests/example/basic/000/09_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/basic/000/analysis.py` & `pycomex-0.9.0/tests/example/basic/000/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/basic/000/annotations.rst` & `pycomex-0.9.0/tests/example/basic/000/annotations.rst`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/basic/000/basic.py` & `pycomex-0.9.0/tests/example/basic/000/basic.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/basic/000/experiment_data.json` & `pycomex-0.9.0/tests/example/basic/000/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/basic/000/experiment_log.txt` & `pycomex-0.9.0/tests/example/basic/000/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/basic/000/snapshot.py` & `pycomex-0.9.0/tests/example/basic/000/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/inheritance/debug/00_random.txt` & `pycomex-0.9.0/tests/example/inheritance/debug/00_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/inheritance/debug/01_random.txt` & `pycomex-0.9.0/tests/example/inheritance/debug/01_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/inheritance/debug/02_random.txt` & `pycomex-0.9.0/tests/example/inheritance/debug/02_random.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/inheritance/debug/analysing.py` & `pycomex-0.9.0/tests/example/inheritance/debug/analysing.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/inheritance/debug/analysis.py` & `pycomex-0.9.0/tests/example/inheritance/debug/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/inheritance/debug/annotations.rst` & `pycomex-0.9.0/tests/example/inheritance/debug/annotations.rst`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/inheritance/debug/experiment_data.json` & `pycomex-0.9.0/tests/example/inheritance/debug/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/inheritance/debug/experiment_log.txt` & `pycomex-0.9.0/tests/example/inheritance/debug/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/inheritance/debug/inheritance.py` & `pycomex-0.9.0/tests/example/inheritance/debug/inheritance.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/inheritance/debug/snapshot.py` & `pycomex-0.9.0/tests/example/inheritance/debug/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/quickstart/000/analysis.py` & `pycomex-0.9.0/tests/example/quickstart/000/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/quickstart/000/experiment_data.json` & `pycomex-0.9.0/tests/example/quickstart/000/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/quickstart/000/experiment_log.txt` & `pycomex-0.9.0/tests/example/quickstart/000/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/quickstart/000/quickstart.py` & `pycomex-0.9.0/tests/example/quickstart/000/quickstart.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/quickstart/000/snapshot.py` & `pycomex-0.9.0/tests/example/quickstart/000/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/quickstart/001/analysis.py` & `pycomex-0.9.0/tests/example/quickstart/001/analysis.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/quickstart/001/experiment_data.json` & `pycomex-0.9.0/tests/example/quickstart/001/experiment_data.json`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/quickstart/001/experiment_log.txt` & `pycomex-0.9.0/tests/example/quickstart/001/experiment_log.txt`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/quickstart/001/quickstart.py` & `pycomex-0.9.0/tests/example/quickstart/001/quickstart.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/example/quickstart/001/snapshot.py` & `pycomex-0.9.0/tests/example/quickstart/001/snapshot.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/templates/test_experiment_analysis.py.j2` & `pycomex-0.9.0/tests/templates/test_experiment_analysis.py.j2`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/test_cli.py` & `pycomex-0.9.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/test_examples.py` & `pycomex-0.9.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/test_experiment.py` & `pycomex-0.9.0/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/test_experiment_abstract_experiment.py` & `pycomex-0.9.0/tests/test_experiment_abstract_experiment.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/test_experiment_sub_experiment.py` & `pycomex-0.9.0/tests/test_experiment_sub_experiment.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/test_util.py` & `pycomex-0.9.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/tests/util.py` & `pycomex-0.9.0/tests/util.py`

 * *Files identical despite different names*

### Comparing `pycomex-0.8.8/setup.py` & `pycomex-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
  'psutil>=5.7.2']
 
 entry_points = \
 {'console_scripts': ['pycomex = pycomex.cli:main']}
 
 setup_kwargs = {
     'name': 'pycomex',
-    'version': '0.8.8',
+    'version': '0.9.0',
     'description': 'Python Computational Experiments',
     'long_description': '.. image:: https://img.shields.io/pypi/v/pycomex.svg\n        :target: https://pypi.python.org/pypi/pycomex\n\n.. image:: https://readthedocs.org/projects/pycomex/badge/?version=latest\n        :target: https://pycomex.readthedocs.io/en/latest/?version=latest\n        :alt: Documentation Status\n\nPyComex - Python Computational Experiments\n================================================\n\nMicroframework to improve the experience of running and managing records of computational experiments,\nsuch as machine learning and data science experiments, in Python.\n\n* Free software: MIT license\n\nFeatures\n--------\n\n* Automatically create (nested) folder structure for results of each run of an experiment\n* Simply attach metadata such as performance metrics to experiment object and they will be automatically\n  stored as JSON file\n* Easily attach file artifacts such as ``matplotlib`` figures to experiment records\n* Log messages to stdout as well as permanently store into log file\n* Ready-to-use automatically generated boilerplate code for the analysis and post-processing of\n  experiment data after experiments have terminated.\n* Experiment inheritance: Experiment modules can inherit from other modules and extend their functionality\n  via parameter overwrites and hooks!\n\nInstallation\n------------\n\nInstall stable version with ``pip``\n\n.. code-block:: console\n\n    pip3 install pycomex\n\nOr the most recent development version\n\n.. code-block:: console\n\n    git clone https://github.com/the16thpythonist/pycomex.git\n    cd pycomex ; pip3 install .\n\nQuickstart\n----------\n\nEach computational experiment has to be bundled as a standalone python module. Important experiment\nparameters are placed at the top. Actual execution of the experiment is placed within the ``Experiment``\ncontext manager.\n\nUpon entering the context, a new archive folder for each run of the experiment is created.\n\nArchiving of metadata, file artifacts and error handling is automatically managed on context exit.\n\n.. code-block:: python\n\n    # quickstart.py\n    """\n    This doc string will be saved as the "description" meta data of the experiment records\n    """\n    import os\n    from pycomex.experiment import Experiment\n    from pycomex.util import Skippable\n\n    # Experiment parameters can simply be defined as uppercase global variables.\n    # These are automatically detected and can possibly be overwritten in command\n    # line invocation\n    HELLO = "hello "\n    WORLD = "world!"\n\n    # Experiment context manager needs 3 positional arguments:\n    # - Path to an existing folder in which to store the results\n    # - A namespace name unique for each experiment\n    # - access to the local globals() dict\n    with Skippable(), (e := Experiment(os.getcwd(), "results/example/quickstart", globals())):\n\n        # Internally saved into automatically created nested dict\n        # {\'strings\': {\'hello_world\': \'...\'}}\n        e["strings/hello_world"] = HELLO + WORLD\n\n        # Alternative to "print". Message is printed to stdout as well as\n        # recorded to log file\n        e.info("some debug message")\n\n        # Automatically saves text file artifact to the experiment record folder\n        file_name = "hello_world.txt"\n        e.commit_raw(file_name, HELLO + WORLD)\n        # e.commit_fig(file_name, fig)\n        # e.commit_png(file_name, image)\n        # ...\n\n    # All the code inside this context will be copied to the "analysis.py"\n    # file which will be created as an experiment artifact.\n    with Skippable(), e.analysis:\n        # And we can access all the internal fields of the experiment object\n        # and the experiment parameters here!\n        print(HELLO, WORLD)\n        print(e[\'strings/hello_world\'])\n        # logging will print to stdout but not modify the log file\n        e.info(\'analysis done\')\n\nThis example would create the following folder structure:\n\n.. code-block:: python\n\n    cwd\n    |- results\n       |- example\n          |- 000\n             |+ experiment_log.txt     # Contains all the log messages printed by experiment\n             |+ experiment_meta.txt    # Meta information about the experiment\n             |+ experiment_data.json   # All the data that was added to the internal exp. dict\n             |+ hello_world.txt        # Text artifact that was committed to the experiment\n             |+ snapshot.py            # Copy of the original experiment python module\n             |+ analysis.py            # boilerplate code to get started with analysis of results\n\nThe ``analysis.py`` file is of special importance. It is created as a boilerplate starting\nplace for additional code, which performs analysis or post processing on the results of the experiment.\nThis can for example be used to transform data into a different format or create plots for visualization.\n\nSpecifically note these two aspects:\n\n1. The analysis file contains all of the code which was defined in the ``e.analysis`` context of the\n   original experiment file! This code snippet is automatically transferred at the end of the experiment.\n2. The analysis file actually imports the snapshot copy of the original experiment file. This does not\n   trigger the experiment to be executed again! The ``Experiment`` instance automatically notices that it\n   is being imported and not explicitly executed. It will also populate all of it\'s internal attributes\n   from the persistently saved data in ``experiment_data.json``, which means it is still possible to access\n   all the data of the experiment without having to execute it again!\n\n.. code-block:: python\n\n    # analysis.py\n\n    # [...] imports omitted\n    # Importing the experiment itself\n    from snapshot import *\n\n    PATH = pathlib.Path(__file__).parent.absolute()\n    DATA_PATH = os.path.join(PATH, \'experiment_data.json\')\n    # Load the all raw data of the experiment\n    with open(DATA_PATH, mode=\'r\') as json_file:\n        DATA: Dict[str, Any] = json.load(json_file)\n\n\n    if __name__ == \'__main__\':\n        print(\'RAW DATA KEYS:\')\n        pprint(list(DATA.keys()))\n\n        # ~ The analysis template from the experiment file\n        # And we can access all the internal fields of the experiment object\n        # and the experiment parameters here!\n        print(HELLO, WORLD)\n        print(e[\'strings/hello_world\'])\n        # logging will print to stdout but not modify the log file\n        e.info(\'analysis done\')\n\n\nFor an introduction to more advanced features take a look at the examples in\n``pycomex/examples`` ( https://github.com/the16thpythonist/pycomex/tree/master/pycomex/examples )\n\nCredits\n-------\n\nThis package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.\n\n.. _Cookiecutter: https://github.com/audreyr/cookiecutter\n.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage\n',
     'author': 'Jonas Teufel',
     'author_email': 'jonseb1998@gmail.com',
     'maintainer': 'Jonas Teufel',
     'maintainer_email': 'jonseb1998@gmail.com',
     'url': 'None',
```

### Comparing `pycomex-0.8.8/PKG-INFO` & `pycomex-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pycomex
-Version: 0.8.8
+Version: 0.9.0
 Summary: Python Computational Experiments
 License: MIT
 Keywords: computational experiments,data science,maschine learning,academia
 Author: Jonas Teufel
 Author-email: jonseb1998@gmail.com
 Maintainer: Jonas Teufel
 Maintainer-email: jonseb1998@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (==7.1.2)
 Requires-Dist: jinja2 (==3.0.3)
 Requires-Dist: matplotlib (>=3.5.3)
 Requires-Dist: numpy (>=1.23.2)
 Requires-Dist: psutil (>=5.7.2)
 Project-URL: Documentation, https://pycomex.readthedocs.io
 Description-Content-Type: text/x-rst
```

