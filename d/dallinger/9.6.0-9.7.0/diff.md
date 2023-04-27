# Comparing `tmp/dallinger-9.6.0.tar.gz` & `tmp/dallinger-9.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dallinger-9.6.0.tar", last modified: Tue Apr 18 22:00:43 2023, max compression
+gzip compressed data, was "dallinger-9.7.0.tar", last modified: Thu Apr 27 20:42:48 2023, max compression
```

## Comparing `dallinger-9.6.0.tar` & `dallinger-9.7.0.tar`

### file list

```diff
@@ -1,274 +1,274 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.988801 dallinger-9.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-18 21:59:55.000000 dallinger-9.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-18 21:59:55.000000 dallinger-9.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-18 22:00:43.988801 dallinger-9.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-18 21:59:55.000000 dallinger-9.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-18 22:00:38.000000 dallinger-9.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12287 2023-04-18 21:59:55.000000 dallinger-9.6.0/constraints.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.900801 dallinger-9.6.0/dallinger/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/bots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.904801 dallinger-9.6.0/dallinger/command_line/
--rwxr-xr-x   0 runner    (1001) docker     (123)    30603 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/command_line/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24511 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/command_line/appdirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/command_line/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/command_line/develop.py
--rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/command_line/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    25919 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/command_line/docker_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/command_line/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.904801 dallinger-9.6.0/dallinger/default_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/default_configs/.dallingerconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/default_configs/global_config_defaults.txt
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/default_configs/local_config_defaults.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20172 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.904801 dallinger-9.6.0/dallinger/dev_server/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/dev_server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/dev_server/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.908801 dallinger-9.6.0/dallinger/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/docker/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/docker/docker-compose.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/docker/heroku.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/docker/prepare_docker_image.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.908801 dallinger-9.6.0/dallinger/docker/ssh_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/docker/ssh_templates/docker-compose-server.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13935 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/docker/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/docker/wheel_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)    60122 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.912801 dallinger-9.6.0/dallinger/experiment_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiment_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27557 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiment_server/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    57902 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiment_server/experiment_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiment_server/gunicorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiment_server/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiment_server/sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiment_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiment_server/worker_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.912801 dallinger-9.6.0/dallinger/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.884801 dallinger-9.6.0/dallinger/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.912801 dallinger-9.6.0/dallinger/frontend/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.916801 dallinger-9.6.0/dallinger/frontend/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   160403 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/css/dallinger.css
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/css/dashboard.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.916801 dallinger-9.6.0/dallinger/frontend/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.920801 dallinger-9.6.0/dallinger/frontend/static/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    60174 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    24824 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/dallinger2.js
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/dallinger2.test.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.880801 dallinger-9.6.0/dallinger/frontend/static/scripts/fingerprintjs2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.920801 dallinger-9.6.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34376 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    21814 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/network-monitor.js
--rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/reconnecting-websocket.js
--rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/require.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     9342 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/reqwest.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/spin.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/store+json2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    36956 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/tracker.js
--rw-r--r--   0 runner    (1001) docker     (123)    44433 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/tracker.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.924801 dallinger-9.6.0/dallinger/frontend/static/scripts/tracking/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/tracking/load-tracker.js
--rw-r--r--   0 runner    (1001) docker     (123)    29161 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/tracking/scribe-console.js
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.880801 dallinger-9.6.0/dallinger/frontend/static/vis@4.17.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.924801 dallinger-9.6.0/dallinger/frontend/static/vis@4.17.0/dist/
--rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   635830 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.932801 dallinger-9.6.0/dallinger/frontend/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.932801 dallinger-9.6.0/dallinger/frontend/templates/base/
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/base/ad.html
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/base/consent.html
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/base/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/base/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/base/questionnaire.html
--rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/dashboard_database.html
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/dashboard_develop.html
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/dashboard_heroku.html
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/dashboard_home.html
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/dashboard_lifecycle.html
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/dashboard_monitor.html
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/dashboard_mturk.html
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/error-complete.html
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/exit_recruiter.html
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/exit_recruiter_mturk.html
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/exit_recruiter_prolific.html
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/launch.html
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/questionnaire.html
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/frontend/templates/waiting.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.936801 dallinger-9.6.0/dallinger/heroku/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/heroku/Procfile
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/heroku/Procfile_no_clock
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/heroku/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/heroku/clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/heroku/rq_gevent_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    20061 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/heroku/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/heroku/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)    68520 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    28478 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/mturk.py
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/prolific.py
--rw-r--r--   0 runner    (1001) docker     (123)    20249 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/pytest_dallinger.py
--rw-r--r--   0 runner    (1001) docker     (123)    64023 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/recruiters.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/redis_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    32799 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.900801 dallinger-9.6.0/dallinger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-18 22:00:43.000000 dallinger-9.6.0/dallinger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-04-18 22:00:43.000000 dallinger-9.6.0/dallinger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:00:43.000000 dallinger-9.6.0/dallinger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-18 22:00:43.000000 dallinger-9.6.0/dallinger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:00:43.000000 dallinger-9.6.0/dallinger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-18 22:00:43.000000 dallinger-9.6.0/dallinger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 22:00:43.000000 dallinger-9.6.0/dallinger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.936801 dallinger-9.6.0/dallinger_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger_scripts/clock.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger_scripts/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-18 21:59:55.000000 dallinger-9.6.0/dallinger_scripts/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-04-18 21:59:55.000000 dallinger-9.6.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.940801 dallinger-9.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.960801 dallinger-9.6.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.972801 dallinger-9.6.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/AvenirLTStd-Book_gdi.eot
--rw-r--r--   0 runner    (1001) docker     (123)    62093 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/AvenirLTStd-Book_gdi.svg
--rw-r--r--   0 runner    (1001) docker     (123)    46176 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/AvenirLTStd-Book_gdi.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/AvenirLTStd-Book_gdi.woff
--rw-r--r--   0 runner    (1001) docker     (123)   335782 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/Dallinger AWS Group.png
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/barplot.png
--rw-r--r--   0 runner    (1001) docker     (123)    21280 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/burst.png
--rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/chain.png
--rw-r--r--   0 runner    (1001) docker     (123)   317968 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/class_chart.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    32421 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/corner.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    44987 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/delayed.png
--rw-r--r--   0 runner    (1001) docker     (123)   419192 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/directories.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/empty.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   235602 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/front_back_layout.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    55137 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/full.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     9193 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/grid.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     6231 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/grid_mini.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     8152 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/grid_small.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    91384 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/heroku.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    21947 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_static/star.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.972801 dallinger-9.6.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/acknowledgments.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/aws_etc_keys.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/build_demo_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/building_documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/command_line_utility.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/communicating_with_the_server.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    19021 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/contributing_to_dallinger.rst
--rw-r--r--   0 runner    (1001) docker     (123)    61118 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/creating_an_experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/dallinger_the_scientist.rst
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/demo_index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/demoing_dallinger.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/demos_on_heroku.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21478 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/developing_dallinger_setup_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/docker_only.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/docker_support.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/docker_tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/email_setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/experiment_data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/extra_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/installing_dallinger_for_users.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/javascript_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/learning_to_use_dallinger.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/monitoring_a_live_experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/networks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/postico_and_postgres.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/private_repo.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/python_module.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/recruitment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/registration_on_OSF.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/required_experiment_files.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/rewarding_participants.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/running_bots.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/running_the_tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/scheduled_tasks.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.976801 dallinger-9.6.0/docs/source/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/schemas/info.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/schemas/network.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/schemas/node.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/schemas/notification.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/schemas/participant.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/schemas/transformation.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/schemas/transmission.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/schemas/vector.csvs
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/the_experiment_class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/vagrant_setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/waiting_rooms.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/web_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-18 21:59:55.000000 dallinger-9.6.0/docs/source/writing_bots.rst
--rw-r--r--   0 runner    (1001) docker     (123)    85530 2023-04-18 21:59:55.000000 dallinger-9.6.0/incubator.png
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-04-18 21:59:55.000000 dallinger-9.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-18 22:00:43.988801 dallinger-9.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-18 21:59:55.000000 dallinger-9.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:00:43.988801 dallinger-9.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_bots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    40472 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    38988 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13889 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)    42354 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    76131 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_experiment_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_griduniverse.py
--rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_heroku.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    28921 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    50155 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_mturk.py
--rw-r--r--   0 runner    (1001) docker     (123)    23282 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_prolific.py
--rw-r--r--   0 runner    (1001) docker     (123)    57519 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_recruiters.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_replay_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-04-18 21:59:55.000000 dallinger-9.6.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.637323 dallinger-9.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-27 20:41:50.000000 dallinger-9.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-27 20:41:50.000000 dallinger-9.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-27 20:42:48.637323 dallinger-9.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-27 20:41:50.000000 dallinger-9.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-27 20:42:41.000000 dallinger-9.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-04-27 20:41:50.000000 dallinger-9.7.0/constraints.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.553322 dallinger-9.7.0/dallinger/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/bots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.561322 dallinger-9.7.0/dallinger/command_line/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30603 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/command_line/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24511 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/command_line/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/command_line/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/command_line/develop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/command_line/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26720 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/command_line/docker_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/command_line/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14107 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.561322 dallinger-9.7.0/dallinger/default_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/default_configs/.dallingerconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/default_configs/global_config_defaults.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/default_configs/local_config_defaults.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20250 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.561322 dallinger-9.7.0/dallinger/dev_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/dev_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/dev_server/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.565322 dallinger-9.7.0/dallinger/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/docker/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/docker/docker-compose.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/docker/heroku.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/docker/prepare_docker_image.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.565322 dallinger-9.7.0/dallinger/docker/ssh_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/docker/ssh_templates/docker-compose-server.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13935 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/docker/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/docker/wheel_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60122 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.569322 dallinger-9.7.0/dallinger/experiment_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiment_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28025 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiment_server/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58202 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiment_server/experiment_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiment_server/gunicorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiment_server/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiment_server/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiment_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiment_server/worker_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.569322 dallinger-9.7.0/dallinger/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.533321 dallinger-9.7.0/dallinger/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.569322 dallinger-9.7.0/dallinger/frontend/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.569322 dallinger-9.7.0/dallinger/frontend/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   160403 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/css/dallinger.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/css/dashboard.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.569322 dallinger-9.7.0/dallinger/frontend/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.577322 dallinger-9.7.0/dallinger/frontend/static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    60174 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/dallinger2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/dallinger2.test.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.533321 dallinger-9.7.0/dallinger/frontend/static/scripts/fingerprintjs2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.577322 dallinger-9.7.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34376 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21814 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/network-monitor.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/reconnecting-websocket.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/require.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9342 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/reqwest.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/spin.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/store+json2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36956 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/tracker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44433 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/tracker.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.577322 dallinger-9.7.0/dallinger/frontend/static/scripts/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/tracking/load-tracker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29161 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/tracking/scribe-console.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.533321 dallinger-9.7.0/dallinger/frontend/static/vis@4.17.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.577322 dallinger-9.7.0/dallinger/frontend/static/vis@4.17.0/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   635830 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.585322 dallinger-9.7.0/dallinger/frontend/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.589322 dallinger-9.7.0/dallinger/frontend/templates/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/base/ad.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/base/consent.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/base/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/base/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/base/questionnaire.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/dashboard_database.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/dashboard_develop.html
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/dashboard_heroku.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/dashboard_home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/dashboard_lifecycle.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/dashboard_monitor.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/dashboard_mturk.html
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/error-complete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/exit_recruiter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/exit_recruiter_mturk.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/exit_recruiter_prolific.html
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/launch.html
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/questionnaire.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/frontend/templates/waiting.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.589322 dallinger-9.7.0/dallinger/heroku/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/heroku/Procfile
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/heroku/Procfile_no_clock
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/heroku/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/heroku/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/heroku/rq_gevent_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20061 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/heroku/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/heroku/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    68520 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28478 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/mturk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/prolific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20456 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/pytest_dallinger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64023 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/recruiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/redis_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32799 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.557322 dallinger-9.7.0/dallinger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-27 20:42:48.000000 dallinger-9.7.0/dallinger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-04-27 20:42:48.000000 dallinger-9.7.0/dallinger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:42:48.000000 dallinger-9.7.0/dallinger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-27 20:42:48.000000 dallinger-9.7.0/dallinger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:42:48.000000 dallinger-9.7.0/dallinger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-27 20:42:48.000000 dallinger-9.7.0/dallinger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 20:42:48.000000 dallinger-9.7.0/dallinger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.593322 dallinger-9.7.0/dallinger_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger_scripts/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger_scripts/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-27 20:41:50.000000 dallinger-9.7.0/dallinger_scripts/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12324 2023-04-27 20:41:50.000000 dallinger-9.7.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.593322 dallinger-9.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.609323 dallinger-9.7.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.621323 dallinger-9.7.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/AvenirLTStd-Book_gdi.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    62093 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/AvenirLTStd-Book_gdi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    46176 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/AvenirLTStd-Book_gdi.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/AvenirLTStd-Book_gdi.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   335782 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/Dallinger AWS Group.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/barplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21280 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/burst.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/chain.png
+-rw-r--r--   0 runner    (1001) docker     (123)   317968 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/class_chart.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    32421 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/corner.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    44987 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/delayed.png
+-rw-r--r--   0 runner    (1001) docker     (123)   419192 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/directories.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/empty.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   235602 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/front_back_layout.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    55137 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/full.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9193 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/grid.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6231 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/grid_mini.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8152 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/grid_small.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    91384 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/heroku.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    21947 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_static/star.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.621323 dallinger-9.7.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/acknowledgments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/aws_etc_keys.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/build_demo_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/building_documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/command_line_utility.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/communicating_with_the_server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19287 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/contributing_to_dallinger.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    61118 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/creating_an_experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/dallinger_the_scientist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/demo_index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/demoing_dallinger.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/demos_on_heroku.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21478 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/developing_dallinger_setup_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/docker_only.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/docker_support.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/docker_tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/email_setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/experiment_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/extra_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/installing_dallinger_for_users.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/javascript_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/learning_to_use_dallinger.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/monitoring_a_live_experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/networks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/postico_and_postgres.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/private_repo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/python_module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/recruitment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/registration_on_OSF.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/required_experiment_files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/rewarding_participants.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/running_bots.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/running_the_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/scheduled_tasks.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.621323 dallinger-9.7.0/docs/source/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/schemas/info.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/schemas/network.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/schemas/node.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/schemas/notification.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/schemas/participant.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/schemas/transformation.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/schemas/transmission.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/schemas/vector.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/the_experiment_class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/vagrant_setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/waiting_rooms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/web_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-27 20:41:50.000000 dallinger-9.7.0/docs/source/writing_bots.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    85530 2023-04-27 20:41:50.000000 dallinger-9.7.0/incubator.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-27 20:41:50.000000 dallinger-9.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-27 20:42:48.637323 dallinger-9.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-27 20:41:50.000000 dallinger-9.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:42:48.637323 dallinger-9.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_bots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40472 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38988 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13889 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42400 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77379 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_experiment_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_griduniverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_heroku.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28921 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50155 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_mturk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23282 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_prolific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57519 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_recruiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_replay_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-04-27 20:41:50.000000 dallinger-9.7.0/tests/test_utils.py
```

### Comparing `dallinger-9.6.0/LICENSE` & `dallinger-9.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/PKG-INFO` & `dallinger-9.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dallinger
-Version: 9.6.0
+Version: 9.7.0
 Summary: Laboratory automation for the behavioral and social sciences
 Home-page: http://github.com/Dallinger/Dallinger
 Maintainer: Jordan Suchow
 Maintainer-email: suchow@berkeley.edu
 License: MIT
 Keywords: science,cultural evolution,experiments,psychology
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dallinger-9.6.0/README.md` & `dallinger-9.7.0/README.md`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/README.rst` & `dallinger-9.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/constraints.txt` & `dallinger-9.7.0/constraints.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,17 +42,19 @@
     # via paramiko
 beautifulsoup4==4.12.2
     # via nbconvert
 black==23.3.0
     # via dallinger
 bleach==6.0.0
     # via nbconvert
-boto3==1.26.115
+blinker==1.6.2
+    # via flask
+boto3==1.26.121
     # via dallinger
-botocore==1.29.115
+botocore==1.29.121
     # via
     #   boto3
     #   s3transfer
 build==0.10.0
     # via
     #   dallinger
     #   pip-tools
@@ -122,25 +124,25 @@
 exceptiongroup==1.1.1
     # via
     #   pytest
     #   trio
     #   trio-websocket
 executing==1.2.0
     # via stack-data
-faker==18.4.0
+faker==18.5.1
     # via dallinger
 fastjsonschema==2.16.3
     # via nbformat
 filelock==3.12.0
     # via
     #   tox
     #   virtualenv
 flake8==6.0.0
     # via dallinger
-flask==2.2.3
+flask==2.3.1
     # via
     #   dallinger
     #   flask-crossdomain
     #   flask-login
     #   flask-sockets
     #   flask-wtf
 flask-crossdomain==0.1
@@ -169,15 +171,15 @@
     #   sqlalchemy
 gunicorn==20.1.0
     # via dallinger
 h11==0.14.0
     # via wsproto
 heroku3==5.2.1
     # via dallinger
-identify==2.5.22
+identify==2.5.23
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   jsonschema
     #   requests
     #   trio
@@ -304,15 +306,15 @@
     # via dallinger
 mypy-extensions==1.0.0
     # via black
 myst-parser==1.0.0
     # via dallinger
 nbclassic==0.5.5
     # via notebook
-nbclient==0.7.3
+nbclient==0.7.4
     # via nbconvert
 nbconvert==7.3.1
     # via
     #   jupyter
     #   jupyter-server
     #   nbclassic
     #   notebook
@@ -328,17 +330,17 @@
     #   ipykernel
     #   nbclassic
     #   notebook
 nodeenv==1.7.0
     # via pre-commit
 notebook==6.5.4
     # via jupyter
-notebook-shim==0.2.2
+notebook-shim==0.2.3
     # via nbclassic
-numpy==1.24.2
+numpy==1.24.3
     # via pandas
 odfpy==1.4.1
     # via tablib
 openpyxl==3.1.2
     # via tablib
 outcome==1.2.0
     # via trio
@@ -353,15 +355,15 @@
     #   pyproject-api
     #   pytest
     #   pytest-rerunfailures
     #   qtconsole
     #   qtpy
     #   sphinx
     #   tox
-pandas==2.0.0
+pandas==2.0.1
     # via
     #   dallinger
     #   tablib
 pandocfilters==1.5.0
     # via nbconvert
 paramiko==3.1.0
     # via
@@ -375,15 +377,15 @@
     # via
     #   dallinger
     #   ipython
 pickleshare==0.7.5
     # via ipython
 pip-tools==6.13.0
     # via dallinger
-platformdirs==3.2.0
+platformdirs==3.4.0
     # via
     #   black
     #   jupyter-core
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via
@@ -486,15 +488,15 @@
     # via jupyter
 qtpy==2.3.1
     # via qtconsole
 redis==4.5.4
     # via
     #   dallinger
     #   rq
-requests==2.28.2
+requests==2.29.0
     # via
     #   dallinger
     #   docker
     #   heroku3
     #   sphinx
 rfc3339-validator==0.1.4
     # via
@@ -504,15 +506,15 @@
     # via
     #   jsonschema
     #   jupyter-events
 rq==1.13.0
     # via dallinger
 s3transfer==0.6.0
     # via boto3
-selenium==4.8.3
+selenium==4.9.0
     # via dallinger
 send2trash==1.8.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 six==1.16.0
@@ -530,15 +532,15 @@
     #   trio
 snowballstemmer==2.2.0
     # via sphinx
 sortedcontainers==2.4.0
     # via trio
 soupsieve==2.4.1
     # via beautifulsoup4
-sphinx==6.1.3
+sphinx==6.2.1
     # via
     #   dallinger
     #   myst-parser
     #   sphinx-rtd-theme
     #   sphinxcontrib-jquery
     #   sphinxcontrib-spelling
 sphinx-rtd-theme==1.2.0
@@ -591,23 +593,23 @@
     # via
     #   black
     #   build
     #   pyproject-api
     #   pyproject-hooks
     #   pytest
     #   tox
-tornado==6.3
+tornado==6.3.1
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
     #   terminado
-tox==4.4.12
+tox==4.5.1
     # via dallinger
 traitlets==5.9.0
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
@@ -647,15 +649,15 @@
     # via
     #   botocore
     #   docker
     #   requests
     #   selenium
 user-agents==2.2.0
     # via dallinger
-virtualenv==20.21.0
+virtualenv==20.22.0
     # via
     #   pre-commit
     #   tox
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
@@ -663,15 +665,15 @@
     # via
     #   bleach
     #   tinycss2
 websocket-client==1.5.1
     # via
     #   docker
     #   jupyter-server
-werkzeug==2.2.3
+werkzeug==2.3.0
     # via
     #   flask
     #   flask-login
 wheel==0.40.0
     # via pip-tools
 widgetsnbextension==4.0.7
     # via ipywidgets
```

### Comparing `dallinger-9.6.0/dallinger/__init__.py` & `dallinger-9.7.0/dallinger/__init__.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/bots.py` & `dallinger-9.7.0/dallinger/bots.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/command_line/__init__.py` & `dallinger-9.7.0/dallinger/command_line/__init__.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/command_line/appdirs.py` & `dallinger-9.7.0/dallinger/command_line/appdirs.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/command_line/config.py` & `dallinger-9.7.0/dallinger/command_line/config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/command_line/develop.py` & `dallinger-9.7.0/dallinger/command_line/develop.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/command_line/docker.py` & `dallinger-9.7.0/dallinger/command_line/docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,16 @@
     """Build and push the docker image for this experiment."""
     from docker import client
 
     from dallinger.docker.tools import build_image
 
     config = get_config()
     config.load()
-    _, tmp = setup_experiment(log=log, debug=True, local_checks=False)
+    app_name = kwargs.get("app_name", None)
+    _, tmp = setup_experiment(log=log, debug=True, local_checks=False, app=app_name)
     image_name_with_tag = build_image(
         tmp,
         config.get("docker_image_base_name"),
         Output(),
         force_build=not use_existing,
     )
     docker_client = client.from_env()
@@ -199,26 +200,29 @@
 @click.option("--live", "mode", flag_value="live", help="Deploy to the real MTurk")
 @click.option("--image", required=True, help="Name of the docker image to deploy")
 @click.option("--config", "-c", "config_options", nargs=2, multiple=True)
 def deploy_image(image_name, mode, config_options):
     """Deploy Heroku app using a docker image and MTurk."""
     config = get_config()
     config.load()
-    dashboard_password = secrets.token_urlsafe(8)
+    dashboard_user = config.get("dashboard_user", "admin")
+    dashboard_password = config.get("dashboard_password", secrets.token_urlsafe(8))
     dallinger_uid = str(uuid.uuid4())
     config_dict = {
         "AWS_ACCESS_KEY_ID": config.get("aws_access_key_id"),
         "AWS_SECRET_ACCESS_KEY": config.get("aws_secret_access_key"),
         "AWS_DEFAULT_REGION": config.get("aws_region"),
         "prolific_api_token": config["prolific_api_token"],
+        "activate_recruiter_on_start": config.get("activate_recruiter_on_start"),
         "auto_recruit": config.get("auto_recruit"),
         "smtp_username": config.get("smtp_username"),
         "smtp_password": config.get("smtp_password"),
         "whimsical": config.get("whimsical"),
         "FLASK_SECRET_KEY": secrets.token_urlsafe(16),
+        "dashboard_user": dashboard_user,
         "dashboard_password": dashboard_password,
         "mode": mode,
         "CREATOR": netrc.netrc().hosts["api.heroku.com"][0],
         "DALLINGER_UID": dallinger_uid,
     }
     config_dict.update(config_options)
     heroku_conn = Heroku3Client(session=requests.session())
@@ -269,15 +273,15 @@
     if config.get("clock_on"):
         services.append("clock")
     payload = {
         "updates": [
             dict(
                 type=type,
                 quantity=config.get(f"num_dynos_{type}", 1),
-                size=config.get("dyno_type", "hobby"),
+                size=config.get("dyno_type", "basic"),
             )
             for type in services
         ]
     }
     app._h._http_resource(
         method="PATCH",
         resource=("apps", app.id, "formation"),
@@ -321,15 +325,15 @@
         log("Registering the experiment on configured services...")
         registration.register(heroku_app_id, snapshot=None)
 
     # Build experiment image
     build_image(tmp, Path(os.getcwd()).name, Output(), force_build=True)
 
     # Push the built image to get the registry sha256
-    image_name = push.callback(use_existing=True)
+    image_name = push.callback(use_existing=True, app_name=app)
 
     # Log in to Heroku if we aren't already.
     log("Making sure that you are logged in to Heroku.")
     heroku.log_in()
     log("Making sure that you are logged in to Heroku container registry.")
     heroku.container_log_in()
     config.set("heroku_auth_token", heroku.auth_token())
@@ -368,14 +372,15 @@
     addons_t0 = datetime.now().astimezone().replace(microsecond=0)
 
     heroku_config = {
         "AWS_ACCESS_KEY_ID": config["aws_access_key_id"],
         "AWS_SECRET_ACCESS_KEY": config["aws_secret_access_key"],
         "AWS_DEFAULT_REGION": config["aws_region"],
         "prolific_api_token": config["prolific_api_token"],
+        "activate_recruiter_on_start": config.get("activate_recruiter_on_start"),
         "auto_recruit": config["auto_recruit"],
         "smtp_username": config["smtp_username"],
         "smtp_password": config["smtp_password"],
         "whimsical": config["whimsical"],
         "dashboard_password": config["dashboard_password"],
         "FLASK_SECRET_KEY": codecs.encode(os.urandom(16), "hex").decode("ascii"),
         "docker_image_name": image_name,
```

### Comparing `dallinger-9.6.0/dallinger/command_line/docker_ssh.py` & `dallinger-9.7.0/dallinger/command_line/docker_ssh.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import hashlib
 import io
 import json
 import logging
 import os
+import re
+import secrets
 import select
 import socket
 import sys
 import zipfile
 from contextlib import contextmanager, redirect_stdout
 from email.utils import parseaddr
 from functools import wraps
@@ -219,19 +221,23 @@
                     print(f"Image {image_name} pushed to remote registry")
                     return f(*args, **kwargs)
                 # The image is not available, neither locally nor on the remote registry
                 print(
                     f"Could not find image {image_name} specified in experiment config as `docker_image_name`"
                 )
                 raise click.Abort
+        app_name = kwargs.get("app_name", None)
         _, tmp_dir = setup_experiment(
-            Output().log, exp_config=config.as_dict(), local_checks=False
+            Output().log,
+            exp_config=config.as_dict(),
+            local_checks=False,
+            app=app_name,
         )
         build_image(tmp_dir, config.get("docker_image_base_name"), out=Output())
-        image_name = push.callback(use_existing=True)
+        image_name = push.callback(use_existing=True, app_name=app_name)
         return f(image_name, *args, **kwargs)
 
     return wrapper
 
 
 @docker_ssh.command()
 @click.option(
@@ -289,44 +295,55 @@
 
     sftp = get_sftp(ssh_host, user=ssh_user)
     sftp.putfo(BytesIO(DOCKER_COMPOSE_SERVER), "dallinger/docker-compose.yml")
     sftp.putfo(
         BytesIO(CADDYFILE.format(host=dns_host, tls=tls).encode()),
         "dallinger/Caddyfile",
     )
+
+    print("Removing any pre-existing app with the same name.")
+    app_yml = f"~/dallinger/{app_name}/docker-compose.yml"
+    executor.run(
+        f"if [ -f {app_yml} ]; then docker compose -f {app_yml} down --remove-orphans; fi"
+    )
+
     print("Removing any pre-existing Redis volumes.")
     remove_redis_volumes(app_name, executor)
 
     print("Launching http and postgresql servers.")
     executor.run("docker compose -f ~/dallinger/docker-compose.yml up -d")
 
     print("Starting experiment.")
     experiment_uuid = str(uuid4())
     if app_name:
         experiment_id = app_name
     elif archive_path:
         experiment_id = get_experiment_id_from_archive(archive_path)
     else:
         experiment_id = f"dlgr-{experiment_uuid[:8]}"
-    dashboard_password = token_urlsafe(8)
+
+    dashboard_user = config.get("dashboard_user", "admin")
+    dashboard_password = config.get("dashboard_password", secrets.token_urlsafe(8))
 
     cfg = config.as_dict()
     for key in "aws_access_key_id", "aws_secret_access_key":
         # AWS credentials are not included by default in to_dict() result
         # but can be extracted explicitly from a config object
         cfg[key.upper()] = config[key]
 
     cfg.update(
         {
             "FLASK_SECRET_KEY": token_urlsafe(16),
             "AWS_DEFAULT_REGION": config["aws_region"],
             "smtp_username": config.get("smtp_username"),
             "smtp_password": config.get("smtp_password"),
             "prolific_api_token": config["prolific_api_token"],
+            "activate_recruiter_on_start": config["activate_recruiter_on_start"],
             "auto_recruit": config["auto_recruit"],
+            "dashboard_user": dashboard_user,
             "dashboard_password": dashboard_password,
             "mode": mode,
             "CREATOR": f"{USER}@{HOSTNAME}",
             "DALLINGER_UID": experiment_uuid,
             "ADMIN_USER": "admin",
             "docker_image_name": image_name,
         }
@@ -566,18 +583,22 @@
 def get_docker_compose_yml(
     config: Dict[str, str],
     experiment_id: str,
     experiment_image: str,
     postgresql_password: str,
 ) -> str:
     """Generate a docker-compose.yml file based on the given"""
+    docker_volumes = config.get("docker_volumes", "[]")
+    config_str = {key: re.sub("\\$", "$$", str(value)) for key, value in config.items()}
+
     return DOCKER_COMPOSE_EXP_TPL.render(
         experiment_id=experiment_id,
         experiment_image=experiment_image,
-        config=config,
+        config=config_str,
+        docker_volumes=docker_volumes,
         postgresql_password=postgresql_password,
     )
 
 
 def get_retrying_http_client():
     retry_strategy = Retry(
         total=30,
```

### Comparing `dallinger-9.6.0/dallinger/command_line/utils.py` & `dallinger-9.7.0/dallinger/command_line/utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/config.py` & `dallinger-9.7.0/dallinger/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 
 def is_valid_json(value):
     json.loads(value)
 
 
 default_keys = (
-    # These are the keys allowed in a dallinger experiment
-    # config.txt file.
+    # These are the keys allowed in a dallinger experiment config.txt file.
+    ("activate_recruiter_on_start", bool, []),
     ("ad_group", six.text_type, []),
     ("approve_requirement", int, []),
     ("assign_qualifications", bool, []),
     ("auto_recruit", bool, []),
     ("aws_access_key_id", six.text_type, ["AWS_ACCESS_KEY_ID"], True),
     (
         "aws_region",
@@ -177,15 +177,25 @@
 
     @contextmanager
     def override(self, *args, **kwargs):
         self.extend(*args, **kwargs)
         yield self
         self.data.popleft()
 
+    changeable_params = ["auto_recruit"]
+
     def get(self, key, default=marker):
+        # For now this is limited to "auto_recruit", but in the future it can be extended
+        # to other parameters as well
+        if key == "auto_recruit":
+            from dallinger.db import redis_conn
+
+            auto_recruit = redis_conn.get("auto_recruit")
+            if auto_recruit is not None:
+                return bool(int(auto_recruit))
         if not self.ready:
             raise RuntimeError("Config not loaded")
         for layer in self.data:
             try:
                 value = layer[key]
                 if isinstance(value, six.text_type):
                     value = value.strip()
```

### Comparing `dallinger-9.6.0/dallinger/data.py` & `dallinger-9.7.0/dallinger/data.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/db.py` & `dallinger-9.7.0/dallinger/db.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/default_configs/global_config_defaults.txt` & `dallinger-9.7.0/dallinger/default_configs/global_config_defaults.txt`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 [Experiment]
 replay = False
 mode = debug
 enable_global_experiment_registry = False
 language = en
 
 [Recruiter]
+activate_recruiter_on_start = True
 auto_recruit = False
 assign_qualifications = False
 us_only = False
 disable_when_duration_exceeded = True
 
 [Bots]
 webdriver_type = chrome_headless
@@ -41,8 +42,8 @@
 
 [Prolific]
 prolific_api_token = Set your Prolific API token in ~/.dallingerconfig!
 prolific_api_version = v1
 prolific_estimated_completion_minutes = 0
 prolific_maximum_allowed_minutes = 0
 prolific_recruitment_config = {}
-prolific_reward_cents = 0
+prolific_reward_cents = 0
```

### Comparing `dallinger-9.6.0/dallinger/deployment.py` & `dallinger-9.7.0/dallinger/deployment.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,15 @@
     for name in addons:
         heroku_app.addon(name)
 
     heroku_config = {
         "AWS_ACCESS_KEY_ID": config["aws_access_key_id"],
         "AWS_SECRET_ACCESS_KEY": config["aws_secret_access_key"],
         "AWS_DEFAULT_REGION": config["aws_region"],
+        "activate_recruiter_on_start": config["activate_recruiter_on_start"],
         "auto_recruit": config["auto_recruit"],
         "smtp_username": config["smtp_username"],
         "smtp_password": config["smtp_password"],
         "whimsical": config["whimsical"],
         "FLASK_SECRET_KEY": codecs.encode(os.urandom(16), "hex").decode("ascii"),
     }
```

### Comparing `dallinger-9.6.0/dallinger/dev_server/app.py` & `dallinger-9.7.0/dallinger/dev_server/app.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/docker/deployment.py` & `dallinger-9.7.0/dallinger/docker/deployment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/docker/docker-compose.yml.j2` & `dallinger-9.7.0/dallinger/docker/docker-compose.yml.j2`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2` & `dallinger-9.7.0/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2`

 * *Files 18% similar despite different names*

```diff
@@ -25,19 +25,17 @@
     {%- for key, value in config.items() %}
       {{ key }}: {{ value | string() | tojson }}
     {%- endfor %}
     networks:
       - dallinger
     volumes:
       - ${HOME}/dallinger-data/{{ experiment_id }}:/var/lib/dallinger
-    {%- if config.get("docker_volumes", "") %}
-    {%- for volume in config.get("docker_volumes", "").split(",") %}
+    {%- for volume in docker_volumes.split(",") %}
       - {{ volume | string() | tojson }}
     {%- endfor %}
-    {%- endif %}
 
   web:
     image: {{ experiment_image }}
     user: "${UID}:${GID}"
     command: dallinger_heroku_web
     depends_on:
       <<: *commondepends
@@ -46,19 +44,17 @@
       PORT: 5000
     networks:
       dallinger:
         aliases:
           - {{ experiment_id }}_web
     volumes:
       - ${HOME}/dallinger-data/{{ experiment_id }}:/var/lib/dallinger
-    {%- if config.get("docker_volumes", "") %}
-    {%- for volume in config.get("docker_volumes", "").split(",") %}
+    {%- for volume in docker_volumes.split(",") %}
       - {{ volume | string() | tojson }}
     {%- endfor %}
-    {%- endif %}
 
 {%- if config["clock_on"] %}
   clock:
     image: {{ experiment_image }}
     user: "${UID}:${GID}"
     command: dallinger_heroku_clock
     depends_on:
```

### Comparing `dallinger-9.6.0/dallinger/docker/ssh_templates/docker-compose-server.yml` & `dallinger-9.7.0/dallinger/docker/ssh_templates/docker-compose-server.yml`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/docker/tools.py` & `dallinger-9.7.0/dallinger/docker/tools.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/docker/wheel_filename.py` & `dallinger-9.7.0/dallinger/docker/wheel_filename.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/experiment.py` & `dallinger-9.7.0/dallinger/experiment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/experiment_server/dashboard.py` & `dallinger-9.7.0/dallinger/experiment_server/dashboard.py`

 * *Files 3% similar despite different names*

```diff
@@ -215,15 +215,15 @@
                 "polymorphic_identity": cls_info["polymorphic_identity"],
             },
         )
 
 
 dashboard_tabs = DashboardTabs(
     [
-        DashboardTab("Home", "dashboard.index"),
+        DashboardTab("Config", "dashboard.index"),
         DashboardTab("Heroku", "dashboard.heroku"),
         DashboardTab("MTurk", "dashboard.mturk"),
         DashboardTab("Monitoring", "dashboard.monitoring"),
         DashboardTab("Lifecycle", "dashboard.lifecycle"),
         DashboardTab("Database", "dashboard.database", database_children),
         DashboardTab("Development", "dashboard.develop"),
     ]
@@ -324,17 +324,24 @@
 
 
 @dashboard.route("/")
 @dashboard.route("/index")
 @login_required
 def index():
     """Displays active experiment configuation"""
-    config = sorted(get_config().as_dict().items())
+    config = get_config()
+    config.load()
+    config_dict = config.as_dict()
+    config_list = sorted(config_dict.items())
     return render_template(
-        "dashboard_home.html", title="Dashboard Home", configuration=config
+        "dashboard_home.html",
+        title="Config",
+        configuration=config_list,
+        configuration_dictionary=config_dict,
+        changeable_params=config.changeable_params,
     )
 
 
 @dashboard.route("/heroku")
 @login_required
 def heroku():
     """Assemble links from Heroku add-on info, stored in config, plus some
@@ -557,14 +564,25 @@
         "qualification_types_url": helper.qualification_types_url,
         "expire_command": helper.expire_command,
     }
 
     return render_template("dashboard_mturk.html", title="MTurk Dashboard", data=data)
 
 
+@dashboard.route("/auto_recruit/<bool_val>", methods=["POST"])
+@login_required
+def auto_recruit(bool_val):
+    from dallinger.db import redis_conn
+
+    num_val = int(bool_val)
+    assert num_val in [0, 1]
+    redis_conn.set("auto_recruit", num_val)
+    return success_response()
+
+
 @dashboard.route("/monitoring")
 @login_required
 def monitoring():
     from sqlalchemy import distinct, func
 
     from dallinger.experiment_server.experiment_server import Experiment, session
     from dallinger.models import Network
```

### Comparing `dallinger-9.6.0/dallinger/experiment_server/experiment_server.py` & `dallinger-9.7.0/dallinger/experiment_server/experiment_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,14 @@
     protected = Experiment(None).protected_routes
     if active_rule in protected:
         raise PermissionError(
             f'Unauthorized call to protected route "{active_rule}": {request}'
         )
 
 
-@app.before_first_request
 def _config():
     app.secret_key = app.config["SECRET_KEY"] = os.environ.get("FLASK_SECRET_KEY")
     config = get_config()
     if not config.ready:
         config.load()
     if config.get("dashboard_password", None):
         app.config["ADMIN_USER"] = dashboard.User(
@@ -82,14 +81,15 @@
             password=config.get("dashboard_password"),
         )
 
     return config
 
 
 def Experiment(args):
+    _config()
     klass = experiment.load()
     return klass(args)
 
 
 # Load the experiment's extra routes, if any.
 try:
     from dallinger_experiment.experiment import extra_routes
@@ -390,26 +390,28 @@
         return error_response(
             error_text="An error occurred when calling on_launch(), check experiment server log "
             "for details: {}".format(str(e)),
             status=500,
             simple=True,
         )
 
-    try:
-        recruitment_details = exp.recruiter.open_recruitment(
-            n=exp.initial_recruitment_size
-        )
-        session.commit()
-    except Exception as e:
-        return error_response(
-            error_text="Failed to open recruitment, check experiment server log "
-            "for details: {}".format(str(e)),
-            status=500,
-            simple=True,
-        )
+    recruitment_details = None
+    if _config().get("activate_recruiter_on_start"):
+        try:
+            recruitment_details = exp.recruiter.open_recruitment(
+                n=exp.initial_recruitment_size
+            )
+            session.commit()
+        except Exception as e:
+            return error_response(
+                error_text="Failed to open recruitment, check experiment server log "
+                "for details: {}".format(str(e)),
+                status=500,
+                simple=True,
+            )
 
     for task in exp.background_tasks:
         try:
             gevent.spawn(task)
         except Exception:
             return error_response(
                 error_text="Failed to spawn task on launch: {}, ".format(task)
@@ -442,23 +444,25 @@
                 error_text="Failed to subscribe to chat for channel on launch "
                 + "{}".format(exp.channel)
                 + ", check experiment server log for details",
                 status=500,
                 simple=True,
             )
 
-    message = "\n".join(
-        (
-            "Initial recruitment list:\n{}".format(
-                "\n".join(recruitment_details["items"])
-            ),
-            "Additional details:\n{}".format(recruitment_details["message"]),
+    if recruitment_details is not None:
+        message = "\n".join(
+            (
+                "Initial recruitment list:\n{}".format(
+                    "\n".join(recruitment_details["items"])
+                ),
+                "Additional details:\n{}".format(recruitment_details["message"]),
+            )
         )
-    )
-
+    else:
+        message = "Recruitment hasn't been started yet. Please, initialize recruitment manually!"
     return success_response(recruitment_msg=message)
 
 
 def prepare_advertisement():
     session = db.session
     config = _config()
     mode = config.get("mode")
@@ -543,15 +547,15 @@
         # Participant has not yet agreed to the consent. They might not
         # even have accepted the HIT.
         return render_template("ad.html", **kw)
 
 
 @app.route("/recruiter-exit", methods=["GET"])
 @nocache
-def recriter_exit():
+def recruiter_exit():
     """Display an exit page defined by the Participant's Recruiter.
     The Recruiter may in turn delegate to the Experiment for additional
     values to display.
     """
     participant_id = request.args.get("participant_id")
     if participant_id is None:
         return error_response(
```

### Comparing `dallinger-9.6.0/dallinger/experiment_server/gunicorn.py` & `dallinger-9.7.0/dallinger/experiment_server/gunicorn.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/experiment_server/replay.py` & `dallinger-9.7.0/dallinger/experiment_server/replay.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/experiment_server/sockets.py` & `dallinger-9.7.0/dallinger/experiment_server/sockets.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/experiment_server/utils.py` & `dallinger-9.7.0/dallinger/experiment_server/utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/experiment_server/worker_events.py` & `dallinger-9.7.0/dallinger/experiment_server/worker_events.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/experiments/__init__.py` & `dallinger-9.7.0/dallinger/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/css/bootstrap.min.css` & `dallinger-9.7.0/dallinger/frontend/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/css/dashboard.css` & `dallinger-9.7.0/dallinger/frontend/static/css/dashboard.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/scripts/bootstrap.min.js` & `dallinger-9.7.0/dallinger/frontend/static/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/scripts/clipboard.min.js` & `dallinger-9.7.0/dallinger/frontend/static/scripts/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/scripts/dallinger2.js` & `dallinger-9.7.0/dallinger/frontend/static/scripts/dallinger2.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -420,15 +420,15 @@
             exitRoute = "/recruiter-exit?participant_id=" + participantId;
 
         dlgr.post('/worker_complete', {
             'participant_id': participantId
         }).done(function() {
             deferred.resolve();
             dlgr.allowExit();
-            if (window.opener) {
+            if (window.opener && !window.opener.location.pathname.startsWith("/dashboard")) {
                 // If the parent window is still around, redirect it to the exit route
                 // and close the secondary window (this one) that held the main experiment:
                 window.opener.location = exitRoute;
                 window.close();
             } else {
                 // We're the only window, so show the exit route here:
                 window.location = exitRoute;
```

### Comparing `dallinger-9.6.0/dallinger/frontend/static/scripts/dallinger2.test.js` & `dallinger-9.7.0/dallinger/frontend/static/scripts/dallinger2.test.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js` & `dallinger-9.7.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/scripts/jquery-3.6.0.min.js` & `dallinger-9.7.0/dallinger/frontend/static/scripts/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/scripts/network-monitor.js` & `dallinger-9.7.0/dallinger/frontend/static/scripts/network-monitor.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/scripts/popper.min.js` & `dallinger-9.7.0/dallinger/frontend/static/scripts/popper.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/scripts/reconnecting-websocket.js` & `dallinger-9.7.0/dallinger/frontend/static/scripts/reconnecting-websocket.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/scripts/require.js` & `dallinger-9.7.0/dallinger/frontend/static/scripts/require.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/scripts/reqwest.min.js` & `dallinger-9.7.0/dallinger/frontend/static/scripts/reqwest.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/scripts/spin.min.js` & `dallinger-9.7.0/dallinger/frontend/static/scripts/spin.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/scripts/store+json2.min.js` & `dallinger-9.7.0/dallinger/frontend/static/scripts/store+json2.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/scripts/tracker.js` & `dallinger-9.7.0/dallinger/frontend/static/scripts/tracker.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/scripts/tracker.js.map` & `dallinger-9.7.0/dallinger/frontend/static/scripts/tracker.js.map`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/scripts/tracking/load-tracker.js` & `dallinger-9.7.0/dallinger/frontend/static/scripts/tracking/load-tracker.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js` & `dallinger-9.7.0/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js` & `dallinger-9.7.0/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css` & `dallinger-9.7.0/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js` & `dallinger-9.7.0/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/templates/base/ad.html` & `dallinger-9.7.0/dallinger/frontend/templates/base/ad.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/templates/base/consent.html` & `dallinger-9.7.0/dallinger/frontend/templates/base/consent.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/templates/base/dashboard.html` & `dallinger-9.7.0/dallinger/frontend/templates/base/dashboard.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/templates/base/layout.html` & `dallinger-9.7.0/dallinger/frontend/templates/base/layout.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/templates/base/questionnaire.html` & `dallinger-9.7.0/dallinger/frontend/templates/base/questionnaire.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/templates/dashboard_database.html` & `dallinger-9.7.0/dallinger/frontend/templates/dashboard_database.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/templates/dashboard_develop.html` & `dallinger-9.7.0/dallinger/frontend/templates/dashboard_develop.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/templates/dashboard_lifecycle.html` & `dallinger-9.7.0/dallinger/frontend/templates/dashboard_lifecycle.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/templates/dashboard_monitor.html` & `dallinger-9.7.0/dallinger/frontend/templates/dashboard_monitor.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/templates/dashboard_mturk.html` & `dallinger-9.7.0/dallinger/frontend/templates/dashboard_mturk.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/templates/error-complete.html` & `dallinger-9.7.0/dallinger/frontend/templates/error-complete.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/templates/error.html` & `dallinger-9.7.0/dallinger/frontend/templates/error.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/templates/exit_recruiter.html` & `dallinger-9.7.0/dallinger/frontend/templates/exit_recruiter.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/templates/exit_recruiter_mturk.html` & `dallinger-9.7.0/dallinger/frontend/templates/exit_recruiter_mturk.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/templates/exit_recruiter_prolific.html` & `dallinger-9.7.0/dallinger/frontend/templates/exit_recruiter_prolific.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/templates/login.html` & `dallinger-9.7.0/dallinger/frontend/templates/login.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/frontend/templates/waiting.html` & `dallinger-9.7.0/dallinger/frontend/templates/waiting.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/heroku/clock.py` & `dallinger-9.7.0/dallinger/heroku/clock.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/heroku/rq_gevent_worker.py` & `dallinger-9.7.0/dallinger/heroku/rq_gevent_worker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/heroku/tools.py` & `dallinger-9.7.0/dallinger/heroku/tools.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/jupyter.py` & `dallinger-9.7.0/dallinger/jupyter.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/models.py` & `dallinger-9.7.0/dallinger/models.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/mturk.py` & `dallinger-9.7.0/dallinger/mturk.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/networks.py` & `dallinger-9.7.0/dallinger/networks.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/nodes.py` & `dallinger-9.7.0/dallinger/nodes.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/notifications.py` & `dallinger-9.7.0/dallinger/notifications.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/processes.py` & `dallinger-9.7.0/dallinger/processes.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/prolific.py` & `dallinger-9.7.0/dallinger/prolific.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/pytest_dallinger.py` & `dallinger-9.7.0/dallinger/pytest_dallinger.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,15 @@
 @pytest.fixture
 def stub_config():
     """Builds a standardized Configuration object and returns it, but does
     not load it as the active configuration returned by
     dallinger.config.get_config()
     """
     defaults = {
+        "activate_recruiter_on_start": True,
         "ad_group": "Test ad group",
         "approve_requirement": 95,
         "assign_qualifications": True,
         "auto_recruit": True,
         "aws_access_key_id": "fake aws key",
         "aws_secret_access_key": "fake aws secret",
         "aws_region": "us-east-1",
@@ -651,7 +652,17 @@
             return el
     else:
         wait.until(condition)
         if value in el.text:
             return el
 
     raise AttributeError
+
+
+@pytest.fixture
+def redis_conn():
+    from dallinger.db import redis_conn as _redis
+
+    yield _redis
+
+    for key in _redis.keys():
+        _redis.delete(key)
```

### Comparing `dallinger-9.6.0/dallinger/recruiters.py` & `dallinger-9.7.0/dallinger/recruiters.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/redis_utils.py` & `dallinger-9.7.0/dallinger/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/registration.py` & `dallinger-9.7.0/dallinger/registration.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/transformations.py` & `dallinger-9.7.0/dallinger/transformations.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger/utils.py` & `dallinger-9.7.0/dallinger/utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger.egg-info/PKG-INFO` & `dallinger-9.7.0/dallinger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dallinger
-Version: 9.6.0
+Version: 9.7.0
 Summary: Laboratory automation for the behavioral and social sciences
 Home-page: http://github.com/Dallinger/Dallinger
 Maintainer: Jordan Suchow
 Maintainer-email: suchow@berkeley.edu
 License: MIT
 Keywords: science,cultural evolution,experiments,psychology
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dallinger-9.6.0/dallinger.egg-info/SOURCES.txt` & `dallinger-9.7.0/dallinger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger.egg-info/requires.txt` & `dallinger-9.7.0/dallinger.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dallinger_scripts/worker.py` & `dallinger-9.7.0/dallinger_scripts/worker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/dev-requirements.txt` & `dallinger-9.7.0/dev-requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,17 +42,19 @@
     # via paramiko
 beautifulsoup4==4.12.2
     # via nbconvert
 black==23.3.0
     # via dallinger
 bleach==6.0.0
     # via nbconvert
-boto3==1.26.115
+blinker==1.6.2
+    # via flask
+boto3==1.26.121
     # via dallinger
-botocore==1.29.115
+botocore==1.29.121
     # via
     #   boto3
     #   s3transfer
 build==0.10.0
     # via
     #   dallinger
     #   pip-tools
@@ -122,25 +124,25 @@
 exceptiongroup==1.1.1
     # via
     #   pytest
     #   trio
     #   trio-websocket
 executing==1.2.0
     # via stack-data
-faker==18.4.0
+faker==18.5.1
     # via dallinger
 fastjsonschema==2.16.3
     # via nbformat
 filelock==3.12.0
     # via
     #   tox
     #   virtualenv
 flake8==6.0.0
     # via dallinger
-flask==2.2.3
+flask==2.3.1
     # via
     #   dallinger
     #   flask-crossdomain
     #   flask-login
     #   flask-sockets
     #   flask-wtf
 flask-crossdomain==0.1
@@ -169,15 +171,15 @@
     #   sqlalchemy
 gunicorn==20.1.0
     # via dallinger
 h11==0.14.0
     # via wsproto
 heroku3==5.2.1
     # via dallinger
-identify==2.5.22
+identify==2.5.23
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   jsonschema
     #   requests
     #   trio
@@ -304,15 +306,15 @@
     # via dallinger
 mypy-extensions==1.0.0
     # via black
 myst-parser==1.0.0
     # via dallinger
 nbclassic==0.5.5
     # via notebook
-nbclient==0.7.3
+nbclient==0.7.4
     # via nbconvert
 nbconvert==7.3.1
     # via
     #   jupyter
     #   jupyter-server
     #   nbclassic
     #   notebook
@@ -328,17 +330,17 @@
     #   ipykernel
     #   nbclassic
     #   notebook
 nodeenv==1.7.0
     # via pre-commit
 notebook==6.5.4
     # via jupyter
-notebook-shim==0.2.2
+notebook-shim==0.2.3
     # via nbclassic
-numpy==1.24.2
+numpy==1.24.3
     # via pandas
 odfpy==1.4.1
     # via tablib
 openpyxl==3.1.2
     # via tablib
 outcome==1.2.0
     # via trio
@@ -353,15 +355,15 @@
     #   pyproject-api
     #   pytest
     #   pytest-rerunfailures
     #   qtconsole
     #   qtpy
     #   sphinx
     #   tox
-pandas==2.0.0
+pandas==2.0.1
     # via
     #   dallinger
     #   tablib
 pandocfilters==1.5.0
     # via nbconvert
 paramiko==3.1.0
     # via
@@ -375,15 +377,15 @@
     # via
     #   dallinger
     #   ipython
 pickleshare==0.7.5
     # via ipython
 pip-tools==6.13.0
     # via dallinger
-platformdirs==3.2.0
+platformdirs==3.4.0
     # via
     #   black
     #   jupyter-core
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via
@@ -486,15 +488,15 @@
     # via jupyter
 qtpy==2.3.1
     # via qtconsole
 redis==4.5.4
     # via
     #   dallinger
     #   rq
-requests==2.28.2
+requests==2.29.0
     # via
     #   dallinger
     #   docker
     #   heroku3
     #   sphinx
 rfc3339-validator==0.1.4
     # via
@@ -504,15 +506,15 @@
     # via
     #   jsonschema
     #   jupyter-events
 rq==1.13.0
     # via dallinger
 s3transfer==0.6.0
     # via boto3
-selenium==4.8.3
+selenium==4.9.0
     # via dallinger
 send2trash==1.8.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 six==1.16.0
@@ -530,15 +532,15 @@
     #   trio
 snowballstemmer==2.2.0
     # via sphinx
 sortedcontainers==2.4.0
     # via trio
 soupsieve==2.4.1
     # via beautifulsoup4
-sphinx==6.1.3
+sphinx==6.2.1
     # via
     #   dallinger
     #   myst-parser
     #   sphinx-rtd-theme
     #   sphinxcontrib-jquery
     #   sphinxcontrib-spelling
 sphinx-rtd-theme==1.2.0
@@ -591,23 +593,23 @@
     # via
     #   black
     #   build
     #   pyproject-api
     #   pyproject-hooks
     #   pytest
     #   tox
-tornado==6.3
+tornado==6.3.1
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
     #   terminado
-tox==4.4.12
+tox==4.5.1
     # via dallinger
 traitlets==5.9.0
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
@@ -647,15 +649,15 @@
     # via
     #   botocore
     #   docker
     #   requests
     #   selenium
 user-agents==2.2.0
     # via dallinger
-virtualenv==20.21.0
+virtualenv==20.22.0
     # via
     #   pre-commit
     #   tox
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
@@ -663,15 +665,15 @@
     # via
     #   bleach
     #   tinycss2
 websocket-client==1.5.1
     # via
     #   docker
     #   jupyter-server
-werkzeug==2.2.3
+werkzeug==2.3.0
     # via
     #   flask
     #   flask-login
 wheel==0.40.0
     # via pip-tools
 widgetsnbextension==4.0.7
     # via ipywidgets
```

### Comparing `dallinger-9.6.0/docs/Makefile` & `dallinger-9.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/make.bat` & `dallinger-9.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/AvenirLTStd-Book_gdi.eot` & `dallinger-9.7.0/docs/source/_static/AvenirLTStd-Book_gdi.eot`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/AvenirLTStd-Book_gdi.svg` & `dallinger-9.7.0/docs/source/_static/AvenirLTStd-Book_gdi.svg`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/AvenirLTStd-Book_gdi.ttf` & `dallinger-9.7.0/docs/source/_static/AvenirLTStd-Book_gdi.ttf`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/AvenirLTStd-Book_gdi.woff` & `dallinger-9.7.0/docs/source/_static/AvenirLTStd-Book_gdi.woff`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/Dallinger AWS Group.png` & `dallinger-9.7.0/docs/source/_static/Dallinger AWS Group.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/barplot.png` & `dallinger-9.7.0/docs/source/_static/barplot.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/burst.png` & `dallinger-9.7.0/docs/source/_static/burst.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/chain.png` & `dallinger-9.7.0/docs/source/_static/chain.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/class_chart.jpg` & `dallinger-9.7.0/docs/source/_static/class_chart.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/corner.jpg` & `dallinger-9.7.0/docs/source/_static/corner.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/custom.css` & `dallinger-9.7.0/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/delayed.png` & `dallinger-9.7.0/docs/source/_static/delayed.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/directories.jpg` & `dallinger-9.7.0/docs/source/_static/directories.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/empty.jpg` & `dallinger-9.7.0/docs/source/_static/empty.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/front_back_layout.jpg` & `dallinger-9.7.0/docs/source/_static/front_back_layout.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/full.png` & `dallinger-9.7.0/docs/source/_static/full.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/grid.png` & `dallinger-9.7.0/docs/source/_static/grid.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/grid_mini.png` & `dallinger-9.7.0/docs/source/_static/grid_mini.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/grid_small.png` & `dallinger-9.7.0/docs/source/_static/grid_small.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/heroku.jpg` & `dallinger-9.7.0/docs/source/_static/heroku.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/_static/star.png` & `dallinger-9.7.0/docs/source/_static/star.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/aws_etc_keys.rst` & `dallinger-9.7.0/docs/source/aws_etc_keys.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/build_demo_docs.py` & `dallinger-9.7.0/docs/source/build_demo_docs.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/building_documentation.rst` & `dallinger-9.7.0/docs/source/building_documentation.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/classes.rst` & `dallinger-9.7.0/docs/source/classes.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/command_line_utility.rst` & `dallinger-9.7.0/docs/source/command_line_utility.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/communicating_with_the_server.rst` & `dallinger-9.7.0/docs/source/communicating_with_the_server.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/conf.py` & `dallinger-9.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/configuration.rst` & `dallinger-9.7.0/docs/source/configuration.rst`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,19 @@
 ``language`` *unicode*
     A ``gettext`` language code to be used for the experiment.
 
 
 Recruitment (General)
 ~~~~~~~~~~~~~~~~~~~~~
 
+``activate_recruiter_on_start`` *boolean*
+    A boolean on whether recruitment should start automatically when the experiment launches.
+    If set to ``false`` the user has to manually initialize recruitment (e.g. via the Prolific panel).
+    Defaults to ``true``.
+
 ``auto_recruit`` *boolean*
     A boolean on whether recruitment should be automatic.
 
 ``browser_exclude_rule`` *unicode - comma separated*
     A set of rules you can apply to prevent participants with unsupported web
     browsers from participating in your experiment. Valid exclustion values are:
         * mobile
```

### Comparing `dallinger-9.6.0/docs/source/contributing_to_dallinger.rst` & `dallinger-9.7.0/docs/source/contributing_to_dallinger.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/creating_an_experiment.rst` & `dallinger-9.7.0/docs/source/creating_an_experiment.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/demo_index.rst` & `dallinger-9.7.0/docs/source/demo_index.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/demoing_dallinger.rst` & `dallinger-9.7.0/docs/source/demoing_dallinger.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/demos_on_heroku.rst` & `dallinger-9.7.0/docs/source/demos_on_heroku.rst`

 * *Files 9% similar despite different names*

```diff
@@ -16,10 +16,10 @@
 
 You can read more about Heroku's `Postgres Plans <https://devcenter.heroku.com/articles/heroku-postgres-plans/>`__ and
 their `Redis add-on <https://elements.heroku.com/addons/heroku-redis/>`__ offering.
 
 Also note that you may also need to set:
 ::
 
-    dyno_type = hobby
+    dyno_type = basic
 
 Read more about Heroku's `Dyno Types <https://devcenter.heroku.com/articles/dyno-types/>`__.
```

### Comparing `dallinger-9.6.0/docs/source/developing_dallinger_setup_guide.rst` & `dallinger-9.7.0/docs/source/developing_dallinger_setup_guide.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/docker_only.rst` & `dallinger-9.7.0/docs/source/docker_only.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/docker_support.rst` & `dallinger-9.7.0/docs/source/docker_support.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/docker_tutorial.rst` & `dallinger-9.7.0/docs/source/docker_tutorial.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/email_setup.rst` & `dallinger-9.7.0/docs/source/email_setup.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/experiment_data.rst` & `dallinger-9.7.0/docs/source/experiment_data.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/extra_configuration.rst` & `dallinger-9.7.0/docs/source/extra_configuration.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/index.rst` & `dallinger-9.7.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/installing_dallinger_for_users.rst` & `dallinger-9.7.0/docs/source/installing_dallinger_for_users.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/javascript_api.rst` & `dallinger-9.7.0/docs/source/javascript_api.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/learning_to_use_dallinger.rst` & `dallinger-9.7.0/docs/source/learning_to_use_dallinger.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/monitoring_a_live_experiment.rst` & `dallinger-9.7.0/docs/source/monitoring_a_live_experiment.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/networks.rst` & `dallinger-9.7.0/docs/source/networks.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/postico_and_postgres.rst` & `dallinger-9.7.0/docs/source/postico_and_postgres.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/private_repo.rst` & `dallinger-9.7.0/docs/source/private_repo.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/python_module.rst` & `dallinger-9.7.0/docs/source/python_module.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/recruitment.rst` & `dallinger-9.7.0/docs/source/recruitment.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/required_experiment_files.rst` & `dallinger-9.7.0/docs/source/required_experiment_files.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/rewarding_participants.rst` & `dallinger-9.7.0/docs/source/rewarding_participants.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/running_bots.rst` & `dallinger-9.7.0/docs/source/running_bots.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/running_the_tests.rst` & `dallinger-9.7.0/docs/source/running_the_tests.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/scheduled_tasks.rst` & `dallinger-9.7.0/docs/source/scheduled_tasks.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/spelling_wordlist.txt` & `dallinger-9.7.0/docs/source/spelling_wordlist.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/the_experiment_class.rst` & `dallinger-9.7.0/docs/source/the_experiment_class.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/troubleshooting.rst` & `dallinger-9.7.0/docs/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/vagrant_setup.rst` & `dallinger-9.7.0/docs/source/vagrant_setup.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/waiting_rooms.rst` & `dallinger-9.7.0/docs/source/waiting_rooms.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/web_api.rst` & `dallinger-9.7.0/docs/source/web_api.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/docs/source/writing_bots.rst` & `dallinger-9.7.0/docs/source/writing_bots.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/incubator.png` & `dallinger-9.7.0/incubator.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/requirements.txt` & `dallinger-9.7.0/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,19 @@
     # via trio
 async-timeout==4.0.2
     # via redis
 attrs==23.1.0
     # via
     #   outcome
     #   trio
-boto3==1.26.115
+blinker==1.6.2
+    # via flask
+boto3==1.26.121
     # via dallinger
-botocore==1.29.115
+botocore==1.29.121
     # via
     #   boto3
     #   s3transfer
 build==0.10.0
     # via
     #   dallinger
     #   pip-tools
@@ -44,17 +46,17 @@
     #   rq
 cryptography==40.0.2
     # via pyopenssl
 exceptiongroup==1.1.1
     # via
     #   trio
     #   trio-websocket
-faker==18.4.0
+faker==18.5.1
     # via dallinger
-flask==2.2.3
+flask==2.3.1
     # via
     #   dallinger
     #   flask-crossdomain
     #   flask-login
     #   flask-sockets
     #   flask-wtf
 flask-crossdomain==0.1
@@ -139,23 +141,23 @@
     # via apscheduler
 pytz-deprecation-shim==0.1.0.post0
     # via tzlocal
 redis==4.5.4
     # via
     #   dallinger
     #   rq
-requests==2.28.2
+requests==2.29.0
     # via
     #   dallinger
     #   heroku3
 rq==1.13.0
     # via dallinger
 s3transfer==0.6.0
     # via boto3
-selenium==4.8.3
+selenium==4.9.0
     # via dallinger
 six==1.16.0
     # via
     #   apscheduler
     #   dallinger
     #   python-dateutil
     #   sqlalchemy-postgres-copy
@@ -198,15 +200,15 @@
 urllib3==1.26.15
     # via
     #   botocore
     #   requests
     #   selenium
 user-agents==2.2.0
     # via dallinger
-werkzeug==2.2.3
+werkzeug==2.3.0
     # via
     #   flask
     #   flask-login
 wheel==0.40.0
     # via pip-tools
 wsproto==1.2.0
     # via trio-websocket
```

### Comparing `dallinger-9.6.0/setup.py` & `dallinger-9.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 README = (HERE / "README.md").read_text(encoding="utf-8")
 
 
 setup_args = dict(
     name="dallinger",
     packages=["dallinger", "dallinger_scripts"],
-    version="9.6.0",
+    version="9.7.0",
     description="Laboratory automation for the behavioral and social sciences",
     long_description=README,
     long_description_content_type="text/markdown",
     url="http://github.com/Dallinger/Dallinger",
     maintainer="Jordan Suchow",
     maintainer_email="suchow@berkeley.edu",
     license="MIT",
```

### Comparing `dallinger-9.6.0/tests/test_agents.py` & `dallinger-9.7.0/tests/test_agents.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_api.py` & `dallinger-9.7.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_bots.py` & `dallinger-9.7.0/tests/test_bots.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_cli_config.py` & `dallinger-9.7.0/tests/test_cli_config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_command_line.py` & `dallinger-9.7.0/tests/test_command_line.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_config.py` & `dallinger-9.7.0/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,14 +195,21 @@
         try:
             config.load_from_environment()
         finally:
             del os.environ["num_participants"]
         config.ready = True
         assert config.get("num_participants") == 1
 
+    def test_loading_auto_recruit_from_redis(self, active_config, redis_conn):
+        active_config.set("auto_recruit", False)
+        from dallinger.db import redis_conn
+
+        redis_conn.set("auto_recruit", 1)
+        assert active_config.get("auto_recruit") is True
+
 
 @pytest.mark.usefixtures("experiment_dir_merged")
 class TestConfigurationIntegrationTests(object):
     def test_experiment_defined_parameters(self):
         config = get_config()
         config.register_extra_parameters()
         config.load_from_file(LOCAL_CONFIG)
```

### Comparing `dallinger-9.6.0/tests/test_dashboard.py` & `dallinger-9.7.0/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_data.py` & `dallinger-9.7.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_db.py` & `dallinger-9.7.0/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_demos.py` & `dallinger-9.7.0/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_deployment.py` & `dallinger-9.7.0/tests/test_deployment.py`

 * *Files 1% similar despite different names*

```diff
@@ -651,14 +651,15 @@
                 mock.call("sentry"),
             ]
         )
 
     def test_sets_app_properties(self, dsss, heroku_mock):
         dsss(log=mock.Mock())
         heroku_mock.set_multiple.assert_called_once_with(
+            activate_recruiter_on_start=True,
             auto_recruit=True,
             AWS_ACCESS_KEY_ID="fake aws key",
             AWS_DEFAULT_REGION="us-east-1",
             AWS_SECRET_ACCESS_KEY="fake aws secret",
             FLASK_SECRET_KEY=mock.ANY,  # password is random
             smtp_password="fake email password",
             smtp_username="fake email username",
```

### Comparing `dallinger-9.6.0/tests/test_docker.py` & `dallinger-9.7.0/tests/test_docker.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,21 +29,27 @@
 
 
 def test_get_docker_compose_yml_env_vars_escaping():
     """Environment vars with special character should be correctly escaped."""
     result = get_yaml(
         {
             "foo": r'" a quote and a \ backslash ',
+            "bar": "Dollar signs should be escaped with another dollar sign: $1.50",
         }
     )
     assert (
         result["services"]["worker"]["environment"]["foo"]
         == r'" a quote and a \ backslash '
     )
 
+    assert (
+        result["services"]["worker"]["environment"]["bar"]
+        == "Dollar signs should be escaped with another dollar sign: $$1.50"
+    )
+
 
 def test_add_image_name(tempdir):
     from dallinger.command_line.docker import add_image_name
 
     file = Path(tempdir) / "test.txt"
 
     file.write_text("")
```

### Comparing `dallinger-9.6.0/tests/test_environments.py` & `dallinger-9.7.0/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_experiment.py` & `dallinger-9.7.0/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_experiment_server.py` & `dallinger-9.7.0/tests/test_experiment_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1564,14 +1564,43 @@
 @pytest.mark.slow
 class TestLaunchRoute(object):
     def test_launch(self, webapp):
         resp = webapp.post("/launch", data={})
         data = json.loads(resp.get_data())
         assert "recruitment_msg" in data
 
+    def test_launch_with_recruitment(self, webapp, active_config):
+        with mock.patch(
+            "dallinger.experiment_server.experiment_server.Experiment"
+        ) as mock_class:
+            mock_exp = mock.Mock()
+            mock_exp.protected_routes = []
+            mock_exp.background_tasks = []
+            mock_exp.recruiter.open_recruitment.return_value = {
+                "items": ["item"],
+                "message": "a message",
+            }
+            mock_class.return_value = mock_exp
+            resp = webapp.post("/launch", data={})
+        assert resp.status_code == 200
+        mock_exp.recruiter.open_recruitment.assert_called()
+
+    def test_launch_without_recruitment(self, webapp, active_config):
+        with mock.patch(
+            "dallinger.experiment_server.experiment_server.Experiment"
+        ) as mock_class:
+            active_config.extend({"activate_recruiter_on_start": False})
+            mock_exp = mock.Mock()
+            mock_exp.protected_routes = []
+            mock_exp.background_tasks = []
+            mock_class.return_value = mock_exp
+            resp = webapp.post("/launch", data={})
+        assert resp.status_code == 200
+        mock_exp.recruiter.open_recruitment.assert_not_called()
+
     def test_launch_logging_fails(self, webapp):
         with mock.patch(
             "dallinger.experiment_server.experiment_server.Experiment"
         ) as mock_class:
             bad_log = mock.Mock(side_effect=IOError)
             mock_exp = mock.Mock(log=bad_log)
             mock_exp.protected_routes = []
```

### Comparing `dallinger-9.6.0/tests/test_griduniverse.py` & `dallinger-9.7.0/tests/test_griduniverse.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_heroku.py` & `dallinger-9.7.0/tests/test_heroku.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_information.py` & `dallinger-9.7.0/tests/test_information.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_jupyter.py` & `dallinger-9.7.0/tests/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_models.py` & `dallinger-9.7.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_mturk.py` & `dallinger-9.7.0/tests/test_mturk.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_networks.py` & `dallinger-9.7.0/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_notifications.py` & `dallinger-9.7.0/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_processes.py` & `dallinger-9.7.0/tests/test_processes.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_prolific.py` & `dallinger-9.7.0/tests/test_prolific.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_recruiters.py` & `dallinger-9.7.0/tests/test_recruiters.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_replay.py` & `dallinger-9.7.0/tests/test_replay.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_replay_state.py` & `dallinger-9.7.0/tests/test_replay_state.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_sockets.py` & `dallinger-9.7.0/tests/test_sockets.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_sources.py` & `dallinger-9.7.0/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_transformations.py` & `dallinger-9.7.0/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.6.0/tests/test_utils.py` & `dallinger-9.7.0/tests/test_utils.py`

 * *Files identical despite different names*

