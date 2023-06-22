# Comparing `tmp/dallinger-9.8.0.tar.gz` & `tmp/dallinger-9.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dallinger-9.8.0.tar", last modified: Mon Jun  5 06:09:37 2023, max compression
+gzip compressed data, was "dallinger-9.8.1.tar", last modified: Thu Jun 22 21:05:05 2023, max compression
```

## Comparing `dallinger-9.8.0.tar` & `dallinger-9.8.1.tar`

### file list

```diff
@@ -1,274 +1,274 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.797674 dallinger-9.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-05 06:08:49.000000 dallinger-9.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-05 06:08:49.000000 dallinger-9.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-05 06:09:37.797674 dallinger-9.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-05 06:08:49.000000 dallinger-9.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-05 06:09:31.000000 dallinger-9.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-06-05 06:08:49.000000 dallinger-9.8.0/constraints.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.773674 dallinger-9.8.0/dallinger/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/bots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.773674 dallinger-9.8.0/dallinger/command_line/
--rwxr-xr-x   0 runner    (1001) docker     (123)    30603 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/command_line/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24511 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/command_line/appdirs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/command_line/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/command_line/develop.py
--rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/command_line/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    26878 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/command_line/docker_ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/command_line/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.773674 dallinger-9.8.0/dallinger/default_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/default_configs/.dallingerconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/default_configs/global_config_defaults.txt
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/default_configs/local_config_defaults.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20250 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.773674 dallinger-9.8.0/dallinger/dev_server/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/dev_server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/dev_server/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.777674 dallinger-9.8.0/dallinger/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/docker/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/docker/docker-compose.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/docker/heroku.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/docker/prepare_docker_image.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.777674 dallinger-9.8.0/dallinger/docker/ssh_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/docker/ssh_templates/docker-compose-server.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/docker/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/docker/wheel_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)    60122 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.777674 dallinger-9.8.0/dallinger/experiment_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiment_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28025 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiment_server/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    58487 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiment_server/experiment_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiment_server/gunicorn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiment_server/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiment_server/sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiment_server/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiment_server/worker_events.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.777674 dallinger-9.8.0/dallinger/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.769674 dallinger-9.8.0/dallinger/frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.777674 dallinger-9.8.0/dallinger/frontend/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.777674 dallinger-9.8.0/dallinger/frontend/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   160403 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/css/dallinger.css
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/css/dashboard.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.777674 dallinger-9.8.0/dallinger/frontend/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.777674 dallinger-9.8.0/dallinger/frontend/static/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    60174 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/dallinger2.js
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/dallinger2.test.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.765674 dallinger-9.8.0/dallinger/frontend/static/scripts/fingerprintjs2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.781674 dallinger-9.8.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34376 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    21814 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/network-monitor.js
--rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/reconnecting-websocket.js
--rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/require.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     9342 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/reqwest.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/spin.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/store+json2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    36956 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/tracker.js
--rw-r--r--   0 runner    (1001) docker     (123)    44433 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/tracker.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.781674 dallinger-9.8.0/dallinger/frontend/static/scripts/tracking/
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/tracking/load-tracker.js
--rw-r--r--   0 runner    (1001) docker     (123)    29161 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/tracking/scribe-console.js
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.765674 dallinger-9.8.0/dallinger/frontend/static/vis@4.17.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.781674 dallinger-9.8.0/dallinger/frontend/static/vis@4.17.0/dist/
--rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   635830 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.781674 dallinger-9.8.0/dallinger/frontend/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.781674 dallinger-9.8.0/dallinger/frontend/templates/base/
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/base/ad.html
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/base/consent.html
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/base/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/base/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/base/questionnaire.html
--rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/dashboard_database.html
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/dashboard_develop.html
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/dashboard_heroku.html
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/dashboard_home.html
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/dashboard_lifecycle.html
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/dashboard_monitor.html
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/dashboard_mturk.html
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/error-complete.html
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/exit_recruiter.html
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/exit_recruiter_mturk.html
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/exit_recruiter_prolific.html
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/launch.html
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/questionnaire.html
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/frontend/templates/waiting.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.785674 dallinger-9.8.0/dallinger/heroku/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/heroku/Procfile
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/heroku/Procfile_no_clock
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/heroku/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/heroku/clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/heroku/rq_gevent_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    20061 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/heroku/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/heroku/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)    68521 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    28478 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/mturk.py
--rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/prolific.py
--rw-r--r--   0 runner    (1001) docker     (123)    20449 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/pytest_dallinger.py
--rw-r--r--   0 runner    (1001) docker     (123)    64023 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/recruiters.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/redis_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.773674 dallinger-9.8.0/dallinger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-05 06:09:37.000000 dallinger-9.8.0/dallinger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-05 06:09:37.000000 dallinger-9.8.0/dallinger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 06:09:37.000000 dallinger-9.8.0/dallinger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-05 06:09:37.000000 dallinger-9.8.0/dallinger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 06:09:37.000000 dallinger-9.8.0/dallinger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-05 06:09:37.000000 dallinger-9.8.0/dallinger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 06:09:37.000000 dallinger-9.8.0/dallinger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.785674 dallinger-9.8.0/dallinger_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger_scripts/clock.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger_scripts/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-05 06:08:49.000000 dallinger-9.8.0/dallinger_scripts/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-06-05 06:08:49.000000 dallinger-9.8.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.785674 dallinger-9.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.789674 dallinger-9.8.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.793674 dallinger-9.8.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/AvenirLTStd-Book_gdi.eot
--rw-r--r--   0 runner    (1001) docker     (123)    62093 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/AvenirLTStd-Book_gdi.svg
--rw-r--r--   0 runner    (1001) docker     (123)    46176 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/AvenirLTStd-Book_gdi.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/AvenirLTStd-Book_gdi.woff
--rw-r--r--   0 runner    (1001) docker     (123)   335782 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/Dallinger AWS Group.png
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/barplot.png
--rw-r--r--   0 runner    (1001) docker     (123)    21280 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/burst.png
--rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/chain.png
--rw-r--r--   0 runner    (1001) docker     (123)   317968 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/class_chart.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    32421 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/corner.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    44987 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/delayed.png
--rw-r--r--   0 runner    (1001) docker     (123)   419192 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/directories.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/empty.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   235602 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/front_back_layout.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    55137 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/full.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     9193 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/grid.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     6231 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/grid_mini.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     8152 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/grid_small.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    91384 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/heroku.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    21947 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_static/star.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.793674 dallinger-9.8.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/acknowledgments.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/aws_etc_keys.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/build_demo_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/building_documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/command_line_utility.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/communicating_with_the_server.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    19287 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/contributing_to_dallinger.rst
--rw-r--r--   0 runner    (1001) docker     (123)    61118 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/creating_an_experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/dallinger_the_scientist.rst
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/demo_index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/demoing_dallinger.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/demos_on_heroku.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21478 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/developing_dallinger_setup_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/docker_only.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/docker_support.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/docker_tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/email_setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/experiment_data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/extra_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/installing_dallinger_for_users.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/javascript_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/learning_to_use_dallinger.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/monitoring_a_live_experiment.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/networks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/postico_and_postgres.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/private_repo.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/python_module.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/recruitment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/registration_on_OSF.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/required_experiment_files.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/rewarding_participants.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/running_bots.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/running_the_tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/scheduled_tasks.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.793674 dallinger-9.8.0/docs/source/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/schemas/info.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/schemas/network.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/schemas/node.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/schemas/notification.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/schemas/participant.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/schemas/transformation.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/schemas/transmission.csvs
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/schemas/vector.csvs
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/the_experiment_class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/vagrant_setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/waiting_rooms.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/web_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-05 06:08:49.000000 dallinger-9.8.0/docs/source/writing_bots.rst
--rw-r--r--   0 runner    (1001) docker     (123)    85530 2023-06-05 06:08:49.000000 dallinger-9.8.0/incubator.png
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-06-05 06:08:49.000000 dallinger-9.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-05 06:09:37.797674 dallinger-9.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-05 06:08:49.000000 dallinger-9.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 06:09:37.797674 dallinger-9.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_bots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    40486 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    38988 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)    42171 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    77386 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_experiment_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_griduniverse.py
--rw-r--r--   0 runner    (1001) docker     (123)    24865 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_heroku.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    28921 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    50155 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_mturk.py
--rw-r--r--   0 runner    (1001) docker     (123)    23282 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_networks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_prolific.py
--rw-r--r--   0 runner    (1001) docker     (123)    57519 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_recruiters.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_replay_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-06-05 06:08:49.000000 dallinger-9.8.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.717707 dallinger-9.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-22 21:04:27.000000 dallinger-9.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-22 21:04:27.000000 dallinger-9.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-22 21:05:05.717707 dallinger-9.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-22 21:04:27.000000 dallinger-9.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-22 21:05:01.000000 dallinger-9.8.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12331 2023-06-22 21:04:27.000000 dallinger-9.8.1/constraints.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.693707 dallinger-9.8.1/dallinger/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/bots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.693707 dallinger-9.8.1/dallinger/command_line/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30603 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/command_line/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24511 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/command_line/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/command_line/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/command_line/develop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18044 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/command_line/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26878 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/command_line/docker_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/command_line/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.693707 dallinger-9.8.1/dallinger/default_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/default_configs/.dallingerconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/default_configs/global_config_defaults.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/default_configs/local_config_defaults.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20250 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.693707 dallinger-9.8.1/dallinger/dev_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/dev_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/dev_server/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.697707 dallinger-9.8.1/dallinger/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/docker/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/docker/docker-compose.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/docker/heroku.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/docker/prepare_docker_image.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.697707 dallinger-9.8.1/dallinger/docker/ssh_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/docker/ssh_templates/docker-compose-server.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14085 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/docker/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/docker/wheel_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60122 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.697707 dallinger-9.8.1/dallinger/experiment_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiment_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28025 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiment_server/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58487 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiment_server/experiment_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiment_server/gunicorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiment_server/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiment_server/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiment_server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiment_server/worker_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.697707 dallinger-9.8.1/dallinger/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.689707 dallinger-9.8.1/dallinger/frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.697707 dallinger-9.8.1/dallinger/frontend/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.697707 dallinger-9.8.1/dallinger/frontend/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   160403 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/css/dallinger.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/css/dashboard.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.697707 dallinger-9.8.1/dallinger/frontend/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.697707 dallinger-9.8.1/dallinger/frontend/static/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    60174 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/dallinger2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/dallinger2.test.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.689707 dallinger-9.8.1/dallinger/frontend/static/scripts/fingerprintjs2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.701707 dallinger-9.8.1/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34376 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/network-monitor.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/reconnecting-websocket.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17738 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/require.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9342 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/reqwest.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/spin.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/store+json2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36956 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/tracker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    44433 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/tracker.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.701707 dallinger-9.8.1/dallinger/frontend/static/scripts/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/tracking/load-tracker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29161 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/tracking/scribe-console.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.689707 dallinger-9.8.1/dallinger/frontend/static/vis@4.17.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.701707 dallinger-9.8.1/dallinger/frontend/static/vis@4.17.0/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)    15046 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   635830 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.701707 dallinger-9.8.1/dallinger/frontend/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.701707 dallinger-9.8.1/dallinger/frontend/templates/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/base/ad.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/base/consent.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/base/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/base/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/base/questionnaire.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/dashboard_database.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/dashboard_develop.html
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/dashboard_heroku.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/dashboard_home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/dashboard_lifecycle.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/dashboard_monitor.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/dashboard_mturk.html
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/error-complete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/exit_recruiter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/exit_recruiter_mturk.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/exit_recruiter_prolific.html
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/launch.html
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/questionnaire.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/frontend/templates/waiting.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.705707 dallinger-9.8.1/dallinger/heroku/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/heroku/Procfile
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/heroku/Procfile_no_clock
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/heroku/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/heroku/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/heroku/rq_gevent_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20322 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/heroku/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/heroku/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    68521 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28478 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/mturk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10230 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10182 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/prolific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20449 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/pytest_dallinger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64022 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/recruiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/redis_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.693707 dallinger-9.8.1/dallinger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-22 21:05:05.000000 dallinger-9.8.1/dallinger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-06-22 21:05:05.000000 dallinger-9.8.1/dallinger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:05:05.000000 dallinger-9.8.1/dallinger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-22 21:05:05.000000 dallinger-9.8.1/dallinger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:05:05.000000 dallinger-9.8.1/dallinger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-22 21:05:05.000000 dallinger-9.8.1/dallinger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-22 21:05:05.000000 dallinger-9.8.1/dallinger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.705707 dallinger-9.8.1/dallinger_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger_scripts/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger_scripts/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-22 21:04:27.000000 dallinger-9.8.1/dallinger_scripts/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-06-22 21:04:27.000000 dallinger-9.8.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.705707 dallinger-9.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.709707 dallinger-9.8.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.713707 dallinger-9.8.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20033 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/AvenirLTStd-Book_gdi.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    62093 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/AvenirLTStd-Book_gdi.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    46176 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/AvenirLTStd-Book_gdi.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/AvenirLTStd-Book_gdi.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   335782 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/Dallinger AWS Group.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/barplot.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21280 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/burst.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11068 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/chain.png
+-rw-r--r--   0 runner    (1001) docker     (123)   317968 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/class_chart.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    32421 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/corner.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    44987 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/delayed.png
+-rw-r--r--   0 runner    (1001) docker     (123)   419192 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/directories.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/empty.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   235602 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/front_back_layout.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    55137 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/full.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9193 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/grid.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6231 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/grid_mini.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8152 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/grid_small.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    91384 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/heroku.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    21947 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_static/star.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.713707 dallinger-9.8.1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/acknowledgments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/aws_etc_keys.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/build_demo_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/building_documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/command_line_utility.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/communicating_with_the_server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19287 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/contributing_to_dallinger.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    61118 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/creating_an_experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/dallinger_the_scientist.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/demo_index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/demoing_dallinger.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/demos_on_heroku.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21478 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/developing_dallinger_setup_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/docker_only.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/docker_support.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/docker_tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/email_setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/experiment_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/extra_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17494 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/installing_dallinger_for_users.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/javascript_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/learning_to_use_dallinger.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/monitoring_a_live_experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14663 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/networks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/postico_and_postgres.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/private_repo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/python_module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/recruitment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/registration_on_OSF.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/required_experiment_files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/rewarding_participants.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/running_bots.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/running_the_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/scheduled_tasks.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.713707 dallinger-9.8.1/docs/source/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/schemas/info.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/schemas/network.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/schemas/node.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/schemas/notification.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/schemas/participant.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/schemas/transformation.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/schemas/transmission.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/schemas/vector.csvs
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/the_experiment_class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/vagrant_setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/waiting_rooms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/web_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-06-22 21:04:27.000000 dallinger-9.8.1/docs/source/writing_bots.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    85530 2023-06-22 21:04:27.000000 dallinger-9.8.1/incubator.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-06-22 21:04:27.000000 dallinger-9.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-22 21:05:05.717707 dallinger-9.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-22 21:04:27.000000 dallinger-9.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:05:05.717707 dallinger-9.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_bots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40624 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38988 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13898 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42171 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77386 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_experiment_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_griduniverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25473 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_heroku.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28921 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50155 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_mturk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23282 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_networks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_prolific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57519 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_recruiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_replay_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-06-22 21:04:27.000000 dallinger-9.8.1/tests/test_utils.py
```

### Comparing `dallinger-9.8.0/LICENSE` & `dallinger-9.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/PKG-INFO` & `dallinger-9.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dallinger
-Version: 9.8.0
+Version: 9.8.1
 Summary: Laboratory automation for the behavioral and social sciences
 Home-page: http://github.com/Dallinger/Dallinger
 Maintainer: Jordan Suchow
 Maintainer-email: suchow@berkeley.edu
 License: MIT
 Keywords: science,cultural evolution,experiments,psychology
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dallinger-9.8.0/README.md` & `dallinger-9.8.1/README.md`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/README.rst` & `dallinger-9.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/constraints.txt` & `dallinger-9.8.1/constraints.txt`

 * *Files 1% similar despite different names*

```diff
@@ -44,17 +44,17 @@
     # via nbconvert
 black==23.3.0
     # via dallinger
 bleach==6.0.0
     # via nbconvert
 blinker==1.6.2
     # via flask
-boto3==1.26.146
+boto3==1.26.158
     # via dallinger
-botocore==1.29.146
+botocore==1.29.158
     # via
     #   boto3
     #   s3transfer
 build==0.10.0
     # via
     #   dallinger
     #   pip-tools
@@ -125,19 +125,19 @@
     # via
     #   anyio
     #   pytest
     #   trio
     #   trio-websocket
 executing==1.2.0
     # via stack-data
-faker==18.10.1
+faker==18.11.1
     # via dallinger
 fastjsonschema==2.17.1
     # via nbformat
-filelock==3.12.0
+filelock==3.12.2
     # via
     #   tox
     #   virtualenv
 flake8==6.0.0
     # via dallinger
 flask==2.3.2
     # via
@@ -184,15 +184,15 @@
     #   jsonschema
     #   requests
     #   trio
 imagesize==1.4.1
     # via sphinx
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.23.1
+ipykernel==6.23.2
     # via
     #   ipywidgets
     #   jupyter
     #   jupyter-console
     #   nbclassic
     #   notebook
     #   qtconsole
@@ -230,15 +230,15 @@
     #   nbconvert
     #   notebook
     #   sphinx
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
 jsonschema==4.17.3
     # via
     #   jupyter-events
     #   nbformat
 jupyter==1.0.0
     # via dallinger
@@ -249,15 +249,15 @@
     #   jupyter-server
     #   nbclassic
     #   nbclient
     #   notebook
     #   qtconsole
 jupyter-console==6.6.3
     # via jupyter
-jupyter-core==5.3.0
+jupyter-core==5.3.1
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-console
     #   jupyter-server
     #   nbclassic
     #   nbclient
@@ -276,15 +276,15 @@
     # via jupyter-server
 jupyterlab-pygments==0.2.2
     # via nbconvert
 jupyterlab-widgets==3.0.7
     # via ipywidgets
 localconfig==1.1.3
     # via dallinger
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
 markuppy==1.14
     # via tablib
 markupsafe==2.1.3
     # via
@@ -294,31 +294,31 @@
     #   wtforms
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
 mccabe==0.7.0
     # via flake8
-mdit-py-plugins==0.3.5
+mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
-mistune==2.0.5
+mistune==3.0.1
     # via nbconvert
 mock==5.0.2
     # via dallinger
 mypy-extensions==1.0.0
     # via black
-myst-parser==1.0.0
+myst-parser==2.0.0
     # via dallinger
 nbclassic==1.0.0
     # via notebook
 nbclient==0.8.0
     # via nbconvert
-nbconvert==7.4.0
+nbconvert==7.6.0
     # via
     #   jupyter
     #   jupyter-server
     #   nbclassic
     #   notebook
 nbformat==5.9.0
     # via
@@ -335,15 +335,17 @@
 nodeenv==1.8.0
     # via pre-commit
 notebook==6.5.4
     # via jupyter
 notebook-shim==0.2.3
     # via nbclassic
 numpy==1.24.3
-    # via pandas
+    # via
+    #   dallinger
+    #   pandas
 odfpy==1.4.1
     # via tablib
 openpyxl==3.1.2
     # via tablib
 outcome==1.2.0
     # via trio
 overrides==7.3.1
@@ -381,25 +383,25 @@
     # via
     #   dallinger
     #   ipython
 pickleshare==0.7.5
     # via ipython
 pip-tools==6.13.0
     # via dallinger
-platformdirs==3.5.1
+platformdirs==3.7.0
     # via
     #   black
     #   jupyter-core
     #   tox
     #   virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via
     #   pytest
     #   tox
-pre-commit==3.3.2
+pre-commit==3.3.3
     # via dallinger
 prometheus-client==0.17.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 prompt-toolkit==3.0.38
@@ -439,23 +441,23 @@
     #   sphinx
 pynacl==1.5.0
     # via paramiko
 pyopenssl==23.2.0
     # via dallinger
 pypandoc==1.11
     # via dallinger
-pyproject-api==1.5.1
+pyproject-api==1.5.2
     # via tox
 pyproject-hooks==1.0.0
     # via build
 pyrsistent==0.19.3
     # via jsonschema
 pysocks==1.7.1
     # via urllib3
-pytest==7.3.1
+pytest==7.3.2
     # via
     #   dallinger
     #   pytest-rerunfailures
 pytest-rerunfailures==11.1.2
     # via dallinger
 python-dateutil==2.8.2
     # via
@@ -504,19 +506,19 @@
     # via
     #   jsonschema
     #   jupyter-events
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
-rq==1.15.0
+rq==1.15.1
     # via dallinger
 s3transfer==0.6.1
     # via boto3
-selenium==4.9.1
+selenium==4.10.0
     # via dallinger
 send2trash==1.8.2
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 six==1.16.0
@@ -541,15 +543,15 @@
 sphinx==6.2.1
     # via
     #   dallinger
     #   myst-parser
     #   sphinx-rtd-theme
     #   sphinxcontrib-jquery
     #   sphinxcontrib-spelling
-sphinx-rtd-theme==1.2.1
+sphinx-rtd-theme==1.2.2
     # via dallinger
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
@@ -569,15 +571,15 @@
     #   sqlalchemy-postgres-copy
 sqlalchemy-postgres-copy==0.5.0
     # via dallinger
 sshtunnel==0.4.0
     # via dallinger
 stack-data==0.6.2
     # via ipython
-tablib==3.4.0
+tablib==3.5.0
     # via dallinger
 tabulate==0.9.0
     # via
     #   dallinger
     #   tablib
 tenacity==8.2.2
     # via dallinger
@@ -603,15 +605,15 @@
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
     #   terminado
-tox==4.5.2
+tox==4.6.3
     # via dallinger
 traitlets==5.9.0
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
@@ -627,53 +629,53 @@
     #   nbformat
     #   notebook
     #   qtconsole
 trio==0.22.0
     # via
     #   selenium
     #   trio-websocket
-trio-websocket==0.10.2
+trio-websocket==0.10.3
     # via selenium
 tzdata==2023.3
     # via pandas
 tzlocal==5.0.1
     # via
     #   apscheduler
     #   dallinger
 ua-parser==0.16.1
     # via
     #   dallinger
     #   user-agents
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
 urllib3==1.26.16
     # via
     #   botocore
     #   docker
     #   requests
     #   selenium
 user-agents==2.2.0
     # via dallinger
-virtualenv==20.23.0
+virtualenv==20.23.1
     # via
     #   pre-commit
     #   tox
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
-websocket-client==1.5.2
+websocket-client==1.6.0
     # via
     #   docker
     #   jupyter-server
-werkzeug==2.3.4
+werkzeug==2.3.6
     # via
     #   flask
     #   flask-login
 wheel==0.40.0
     # via pip-tools
 widgetsnbextension==4.0.7
     # via ipywidgets
```

### Comparing `dallinger-9.8.0/dallinger/__init__.py` & `dallinger-9.8.1/dallinger/__init__.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/bots.py` & `dallinger-9.8.1/dallinger/bots.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/command_line/__init__.py` & `dallinger-9.8.1/dallinger/command_line/__init__.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/command_line/appdirs.py` & `dallinger-9.8.1/dallinger/command_line/appdirs.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/command_line/config.py` & `dallinger-9.8.1/dallinger/command_line/config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/command_line/develop.py` & `dallinger-9.8.1/dallinger/command_line/develop.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/command_line/docker.py` & `dallinger-9.8.1/dallinger/command_line/docker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/command_line/docker_ssh.py` & `dallinger-9.8.1/dallinger/command_line/docker_ssh.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/command_line/utils.py` & `dallinger-9.8.1/dallinger/command_line/utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/config.py` & `dallinger-9.8.1/dallinger/config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/data.py` & `dallinger-9.8.1/dallinger/data.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/db.py` & `dallinger-9.8.1/dallinger/db.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/default_configs/global_config_defaults.txt` & `dallinger-9.8.1/dallinger/default_configs/global_config_defaults.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/deployment.py` & `dallinger-9.8.1/dallinger/deployment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/dev_server/app.py` & `dallinger-9.8.1/dallinger/dev_server/app.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/docker/deployment.py` & `dallinger-9.8.1/dallinger/docker/deployment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/docker/docker-compose.yml.j2` & `dallinger-9.8.1/dallinger/docker/docker-compose.yml.j2`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     volumes:
       - "/dev/shm:/dev/shm"
 {%- for volumestr in volumes %}
       - "{{ volumestr }}"
 {%- endfor %}
 {%- if config.get("docker_volumes", "") %}
 {%- for volume in config.get("docker_volumes", "").split(",") %}
-      - {{ volume | string() | tojson }}
+      - {{ volume | string() }}
 {%- endfor %}
 {%- endif %}
     environment: &commonenv
 {%- if needs_chrome %}
       HOST: web # Tell the worker where we expect the web service to be
 {%- endif %}
       REDIS_URL: redis://redis:6379
@@ -72,15 +72,15 @@
     volumes:
       - "/dev/shm:/dev/shm"
 {%- for volumestr in volumes %}
       - "{{ volumestr }}"
 {%- endfor %}
 {%- if config.get("docker_volumes", "") %}
 {%- for volume in config.get("docker_volumes", "").split(",") %}
-      - {{ volume | string() | tojson }}
+      - {{ volume | string() }}
 {%- endfor %}
 {%- endif %}
     environment:
       <<: *commonenv
       PORT: 5000
     ports:
       - "5000:5000"
```

### Comparing `dallinger-9.8.0/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2` & `dallinger-9.8.1/dallinger/docker/ssh_templates/docker-compose-experiment.yml.j2`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     {%- endfor %}
     networks:
       - dallinger
     volumes:
       - ${HOME}/dallinger-data/{{ experiment_id }}:/var/lib/dallinger
     {%- if docker_volumes | length > 0 %}
       {%- for volume in docker_volumes.split(",") %}
-        - {{ volume | string() | tojson }}
+      - {{ volume | string() }}
       {%- endfor %}
     {%- endif %}
 
   web:
     image: {{ experiment_image }}
     user: "${UID}:${GID}"
     command: dallinger_heroku_web
@@ -48,15 +48,15 @@
       dallinger:
         aliases:
           - {{ experiment_id }}_web
     volumes:
       - ${HOME}/dallinger-data/{{ experiment_id }}:/var/lib/dallinger
     {%- if docker_volumes | length > 0 %}
       {%- for volume in docker_volumes.split(",") %}
-        - {{ volume | string() | tojson }}
+      - {{ volume | string() }}
       {%- endfor %}
     {%- endif %}
 
 {%- if config["clock_on"] %}
   clock:
     image: {{ experiment_image }}
     user: "${UID}:${GID}"
```

### Comparing `dallinger-9.8.0/dallinger/docker/ssh_templates/docker-compose-server.yml` & `dallinger-9.8.1/dallinger/docker/ssh_templates/docker-compose-server.yml`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/docker/tools.py` & `dallinger-9.8.1/dallinger/docker/tools.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/docker/wheel_filename.py` & `dallinger-9.8.1/dallinger/docker/wheel_filename.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/experiment.py` & `dallinger-9.8.1/dallinger/experiment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/experiment_server/dashboard.py` & `dallinger-9.8.1/dallinger/experiment_server/dashboard.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/experiment_server/experiment_server.py` & `dallinger-9.8.1/dallinger/experiment_server/experiment_server.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/experiment_server/gunicorn.py` & `dallinger-9.8.1/dallinger/experiment_server/gunicorn.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/experiment_server/replay.py` & `dallinger-9.8.1/dallinger/experiment_server/replay.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/experiment_server/sockets.py` & `dallinger-9.8.1/dallinger/experiment_server/sockets.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/experiment_server/utils.py` & `dallinger-9.8.1/dallinger/experiment_server/utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/experiment_server/worker_events.py` & `dallinger-9.8.1/dallinger/experiment_server/worker_events.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/experiments/__init__.py` & `dallinger-9.8.1/dallinger/experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/css/bootstrap.min.css` & `dallinger-9.8.1/dallinger/frontend/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/css/dashboard.css` & `dallinger-9.8.1/dallinger/frontend/static/css/dashboard.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/scripts/bootstrap.min.js` & `dallinger-9.8.1/dallinger/frontend/static/scripts/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/scripts/clipboard.min.js` & `dallinger-9.8.1/dallinger/frontend/static/scripts/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/scripts/dallinger2.js` & `dallinger-9.8.1/dallinger/frontend/static/scripts/dallinger2.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/scripts/dallinger2.test.js` & `dallinger-9.8.1/dallinger/frontend/static/scripts/dallinger2.test.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js` & `dallinger-9.8.1/dallinger/frontend/static/scripts/fingerprintjs2/1.5.1/fingerprint2.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/scripts/jquery-3.6.0.min.js` & `dallinger-9.8.1/dallinger/frontend/static/scripts/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/scripts/network-monitor.js` & `dallinger-9.8.1/dallinger/frontend/static/scripts/network-monitor.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -312,14 +312,16 @@
             }
             if (node.failed) {
                 clr = 'red';
             } else {
                 clr = participant.clr;
             }
 
+            node.object_type = 'Node';
+
             nodes.push({
                 id: list_of_node_indx[node.id],
                 label: msg + String(node.id),
                 title: (node.type || '') + ':' + String(node.id),
                 color: clr,
                 group: mgroup,
                 font: {
@@ -335,14 +337,15 @@
             from = vector.origin_id;
             to = vector.destination_id;
             if (vector.failed) {
                 mclr = 'red';
             } else {
                 mclr = 'blue';
             }
+            vector.object_type = 'Vector';
             edges.push({
                 from: list_of_node_indx[from],
                 to: list_of_node_indx[to],
                 arrows: 'to',
                 title: ('vector:' + String(vector.id) + ' (' + String(vector.origin_id) + '→' + String(vector.destination_id) + ')'),
                 data: vector,
                 color: mclr
@@ -379,14 +382,15 @@
             if (info.failed) {
                 mgroup = 'failed_infos';
                 clr = 'red';
             } else {
                 mgroup = 'good_infos';
                 clr = participant.clr;
             }
+            info.object_type = 'Info';
             nodes.push({
                 id: my_node_id,
                 label: info.type + ": " + String(info.id),
                 dashes: true,
                 title: info.type + ':' + String(info.id),
                 group: mgroup,
                 icon: {
@@ -394,14 +398,15 @@
                 },
                 font: {
                     align: 'inside'
                 },
                 data: info
             });
 
+            participant.object_type = 'Participant';
             if (participant_id > 0) {
                 edges.push({
                     from: list_of_node_indx[from],
                     to: to,
                     dashes: true,
                     data: participant,
                     label: "participant: " + String(participant_id),
@@ -428,14 +433,16 @@
         for (i = 0; i < net_structure.trans.length; i++) {
             tran = net_structure.trans[i];
             from = tran.info_in_id;
             to = tran.info_out_id;
             var from_n = map_infoid_to_infonum[from];
             var to_n = map_infoid_to_infonum[to];
 
+            tran.object_type = 'Transmission';
+
             if (tran.failed) {
                 rr = 200;
                 gg = 100;
                 bb = 100;
                 mclr = 'rgb(' + String(rr) + ',' + String(gg) + ',' + String(bb) + ')';
             } else {
                 //mclr='black'
@@ -525,14 +532,15 @@
                 mgroup = 'group_networks_open';
             } else {
                 mgroup = 'group_networks_close';
             }
 
             father = group_fathers[networks_roles[net.id]]; // find father network
             clr = roles_colors[networks_roles[net.id]];
+            net.object_type = 'Network';
             nodes.push({
                 id: my_node_id,
                 label: "network:" + String(net.id),
                 title: "network: " + net.type + ':' + String(net.id) + ' (' + net.role + ')',
                 group: mgroup,
                 font: {
                     align: 'inside'
@@ -604,21 +612,21 @@
                     var sub_title_el = document.createElement('h5');
                     sub_title_el.textContent = node.options.title;
                     stats.appendChild(sub_title_el);
                 }
                 if (node.options.data) {
                     var pre_el = document.createElement('pre');
                     pre_el.textContent = JSON.stringify(node.options.data, null, 2);
-                    stats.appendChild(pre_el);
                     if (node.options.data.id && node.options.data.object_type) {
                         var custom_node = document.createElement('div');
                         custom_node.classList.add('node-details');
                         stats.appendChild(custom_node);
                         $(custom_node).load('/dashboard/node_details/' + node.options.data.object_type + '/' + String(node.options.data.id));
                     }
+                    stats.appendChild(pre_el);
                 }
             }
         };
 
 
         // add event listeners
         network.on('select', function(params) {
```

### Comparing `dallinger-9.8.0/dallinger/frontend/static/scripts/popper.min.js` & `dallinger-9.8.1/dallinger/frontend/static/scripts/popper.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/scripts/reconnecting-websocket.js` & `dallinger-9.8.1/dallinger/frontend/static/scripts/reconnecting-websocket.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/scripts/require.js` & `dallinger-9.8.1/dallinger/frontend/static/scripts/require.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/scripts/reqwest.min.js` & `dallinger-9.8.1/dallinger/frontend/static/scripts/reqwest.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/scripts/spin.min.js` & `dallinger-9.8.1/dallinger/frontend/static/scripts/spin.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/scripts/store+json2.min.js` & `dallinger-9.8.1/dallinger/frontend/static/scripts/store+json2.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/scripts/tracker.js` & `dallinger-9.8.1/dallinger/frontend/static/scripts/tracker.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/scripts/tracker.js.map` & `dallinger-9.8.1/dallinger/frontend/static/scripts/tracker.js.map`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/scripts/tracking/load-tracker.js` & `dallinger-9.8.1/dallinger/frontend/static/scripts/tracking/load-tracker.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js` & `dallinger-9.8.1/dallinger/frontend/static/scripts/tracking/scribe-analytics.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js` & `dallinger-9.8.1/dallinger/frontend/static/scripts/tracking/scribe-dallinger.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css` & `dallinger-9.8.1/dallinger/frontend/static/vis@4.17.0/dist/vis-network.min.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js` & `dallinger-9.8.1/dallinger/frontend/static/vis@4.17.0/dist/vis.min.js`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/templates/base/ad.html` & `dallinger-9.8.1/dallinger/frontend/templates/base/ad.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/templates/base/consent.html` & `dallinger-9.8.1/dallinger/frontend/templates/base/consent.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/templates/base/dashboard.html` & `dallinger-9.8.1/dallinger/frontend/templates/base/dashboard.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/templates/base/layout.html` & `dallinger-9.8.1/dallinger/frontend/templates/base/layout.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/templates/base/questionnaire.html` & `dallinger-9.8.1/dallinger/frontend/templates/base/questionnaire.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/templates/dashboard_database.html` & `dallinger-9.8.1/dallinger/frontend/templates/dashboard_database.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/templates/dashboard_develop.html` & `dallinger-9.8.1/dallinger/frontend/templates/dashboard_develop.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/templates/dashboard_home.html` & `dallinger-9.8.1/dallinger/frontend/templates/dashboard_home.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/templates/dashboard_lifecycle.html` & `dallinger-9.8.1/dallinger/frontend/templates/dashboard_lifecycle.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/templates/dashboard_monitor.html` & `dallinger-9.8.1/dallinger/frontend/templates/dashboard_monitor.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/templates/dashboard_mturk.html` & `dallinger-9.8.1/dallinger/frontend/templates/dashboard_mturk.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/templates/error-complete.html` & `dallinger-9.8.1/dallinger/frontend/templates/error-complete.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/templates/error.html` & `dallinger-9.8.1/dallinger/frontend/templates/error.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/templates/exit_recruiter.html` & `dallinger-9.8.1/dallinger/frontend/templates/exit_recruiter.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/templates/exit_recruiter_mturk.html` & `dallinger-9.8.1/dallinger/frontend/templates/exit_recruiter_mturk.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/templates/exit_recruiter_prolific.html` & `dallinger-9.8.1/dallinger/frontend/templates/exit_recruiter_prolific.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/templates/login.html` & `dallinger-9.8.1/dallinger/frontend/templates/login.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/frontend/templates/waiting.html` & `dallinger-9.8.1/dallinger/frontend/templates/waiting.html`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/heroku/clock.py` & `dallinger-9.8.1/dallinger/heroku/clock.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/heroku/rq_gevent_worker.py` & `dallinger-9.8.1/dallinger/heroku/rq_gevent_worker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/heroku/tools.py` & `dallinger-9.8.1/dallinger/heroku/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import subprocess
 import sys
 import time
 import traceback
 
 import psutil
 import six
+from cached_property import cached_property
 from six.moves import shlex_quote as quote
 
 from dallinger.config import SENSITIVE_KEY_NAMES
 from dallinger.utils import check_call, check_output
 
 
 def app_name(experiment_uuid):
@@ -158,17 +159,26 @@
             ["heroku", "container:release", "web", "worker", "clock", "-a", self.name]
         )
 
     @property
     def name(self):
         return app_name(self.dallinger_uid)
 
-    @property
+    @cached_property
     def url(self):
-        return "https://{}.herokuapp.com".format(self.name)
+        app_info = self._result(
+            [
+                "heroku",
+                "apps:info",
+                "--app",
+                self.name,
+                "--json",
+            ]
+        )
+        return json.loads(app_info)["app"]["web_url"].rstrip("/")
 
     def addon(self, name):
         """Set up an addon"""
         cmd = ["heroku", "addons:create", name, "--app", self.name]
         self._run(cmd)
 
     def addon_destroy(self, name):
```

### Comparing `dallinger-9.8.0/dallinger/jupyter.py` & `dallinger-9.8.1/dallinger/jupyter.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/models.py` & `dallinger-9.8.1/dallinger/models.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/mturk.py` & `dallinger-9.8.1/dallinger/mturk.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/networks.py` & `dallinger-9.8.1/dallinger/networks.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/nodes.py` & `dallinger-9.8.1/dallinger/nodes.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/notifications.py` & `dallinger-9.8.1/dallinger/notifications.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/processes.py` & `dallinger-9.8.1/dallinger/processes.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/prolific.py` & `dallinger-9.8.1/dallinger/prolific.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/pytest_dallinger.py` & `dallinger-9.8.1/dallinger/pytest_dallinger.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/recruiters.py` & `dallinger-9.8.1/dallinger/recruiters.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
 
     def get_qualifications(self, hit_id, sandbox):
         """Return the JSON file containing rules to filter participants."""
         raise NotImplementedError
 
 
 def alphanumeric_code(seed: str, length: int = 8):
-    """Return and alphanumeric string of specified length based on a
+    """Return an alphanumeric string of specified length based on a
     seed value, so the same result will always be returned for a given
     seed.
     """
     chooser = random.Random(seed)
     alphabet = string.ascii_uppercase + string.digits
     return "".join(chooser.choice(alphabet) for i in range(length))
```

### Comparing `dallinger-9.8.0/dallinger/redis_utils.py` & `dallinger-9.8.1/dallinger/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/registration.py` & `dallinger-9.8.1/dallinger/registration.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/transformations.py` & `dallinger-9.8.1/dallinger/transformations.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger/utils.py` & `dallinger-9.8.1/dallinger/utils.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger.egg-info/PKG-INFO` & `dallinger-9.8.1/dallinger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dallinger
-Version: 9.8.0
+Version: 9.8.1
 Summary: Laboratory automation for the behavioral and social sciences
 Home-page: http://github.com/Dallinger/Dallinger
 Maintainer: Jordan Suchow
 Maintainer-email: suchow@berkeley.edu
 License: MIT
 Keywords: science,cultural evolution,experiments,psychology
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dallinger-9.8.0/dallinger.egg-info/SOURCES.txt` & `dallinger-9.8.1/dallinger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dallinger.egg-info/requires.txt` & `dallinger-9.8.1/dallinger.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 future
 gevent
 greenlet
 gunicorn
 heroku3
 ipython<8.13
 localconfig
+numpy<1.25
 pexpect
 pip>=20
 pip-tools
 psycopg2
 psutil
 pyopenssl
 redis
```

### Comparing `dallinger-9.8.0/dallinger_scripts/worker.py` & `dallinger-9.8.1/dallinger_scripts/worker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/dev-requirements.txt` & `dallinger-9.8.1/dev-requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,17 @@
     # via nbconvert
 black==23.3.0
     # via dallinger
 bleach==6.0.0
     # via nbconvert
 blinker==1.6.2
     # via flask
-boto3==1.26.146
+boto3==1.26.158
     # via dallinger
-botocore==1.29.146
+botocore==1.29.158
     # via
     #   boto3
     #   s3transfer
 build==0.10.0
     # via
     #   dallinger
     #   pip-tools
@@ -125,19 +125,19 @@
     # via
     #   anyio
     #   pytest
     #   trio
     #   trio-websocket
 executing==1.2.0
     # via stack-data
-faker==18.10.1
+faker==18.11.1
     # via dallinger
 fastjsonschema==2.17.1
     # via nbformat
-filelock==3.12.0
+filelock==3.12.2
     # via
     #   tox
     #   virtualenv
 flake8==6.0.0
     # via dallinger
 flask==2.3.2
     # via
@@ -184,15 +184,15 @@
     #   jsonschema
     #   requests
     #   trio
 imagesize==1.4.1
     # via sphinx
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.23.1
+ipykernel==6.23.2
     # via
     #   ipywidgets
     #   jupyter
     #   jupyter-console
     #   nbclassic
     #   notebook
     #   qtconsole
@@ -230,15 +230,15 @@
     #   nbconvert
     #   notebook
     #   sphinx
 jmespath==1.0.1
     # via
     #   boto3
     #   botocore
-jsonpointer==2.3
+jsonpointer==2.4
     # via jsonschema
 jsonschema==4.17.3
     # via
     #   jupyter-events
     #   nbformat
 jupyter==1.0.0
     # via dallinger
@@ -249,15 +249,15 @@
     #   jupyter-server
     #   nbclassic
     #   nbclient
     #   notebook
     #   qtconsole
 jupyter-console==6.6.3
     # via jupyter
-jupyter-core==5.3.0
+jupyter-core==5.3.1
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-console
     #   jupyter-server
     #   nbclassic
     #   nbclient
@@ -276,15 +276,15 @@
     # via jupyter-server
 jupyterlab-pygments==0.2.2
     # via nbconvert
 jupyterlab-widgets==3.0.7
     # via ipywidgets
 localconfig==1.1.3
     # via dallinger
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via
     #   mdit-py-plugins
     #   myst-parser
 markuppy==1.14
     # via tablib
 markupsafe==2.1.3
     # via
@@ -294,31 +294,31 @@
     #   wtforms
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
 mccabe==0.7.0
     # via flake8
-mdit-py-plugins==0.3.5
+mdit-py-plugins==0.4.0
     # via myst-parser
 mdurl==0.1.2
     # via markdown-it-py
-mistune==2.0.5
+mistune==3.0.1
     # via nbconvert
 mock==5.0.2
     # via dallinger
 mypy-extensions==1.0.0
     # via black
-myst-parser==1.0.0
+myst-parser==2.0.0
     # via dallinger
 nbclassic==1.0.0
     # via notebook
 nbclient==0.8.0
     # via nbconvert
-nbconvert==7.4.0
+nbconvert==7.6.0
     # via
     #   jupyter
     #   jupyter-server
     #   nbclassic
     #   notebook
 nbformat==5.9.0
     # via
@@ -335,15 +335,17 @@
 nodeenv==1.8.0
     # via pre-commit
 notebook==6.5.4
     # via jupyter
 notebook-shim==0.2.3
     # via nbclassic
 numpy==1.24.3
-    # via pandas
+    # via
+    #   dallinger
+    #   pandas
 odfpy==1.4.1
     # via tablib
 openpyxl==3.1.2
     # via tablib
 outcome==1.2.0
     # via trio
 overrides==7.3.1
@@ -381,25 +383,25 @@
     # via
     #   dallinger
     #   ipython
 pickleshare==0.7.5
     # via ipython
 pip-tools==6.13.0
     # via dallinger
-platformdirs==3.5.1
+platformdirs==3.7.0
     # via
     #   black
     #   jupyter-core
     #   tox
     #   virtualenv
-pluggy==1.0.0
+pluggy==1.2.0
     # via
     #   pytest
     #   tox
-pre-commit==3.3.2
+pre-commit==3.3.3
     # via dallinger
 prometheus-client==0.17.0
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 prompt-toolkit==3.0.38
@@ -439,23 +441,23 @@
     #   sphinx
 pynacl==1.5.0
     # via paramiko
 pyopenssl==23.2.0
     # via dallinger
 pypandoc==1.11
     # via dallinger
-pyproject-api==1.5.1
+pyproject-api==1.5.2
     # via tox
 pyproject-hooks==1.0.0
     # via build
 pyrsistent==0.19.3
     # via jsonschema
 pysocks==1.7.1
     # via urllib3
-pytest==7.3.1
+pytest==7.3.2
     # via
     #   dallinger
     #   pytest-rerunfailures
 pytest-rerunfailures==11.1.2
     # via dallinger
 python-dateutil==2.8.2
     # via
@@ -504,19 +506,19 @@
     # via
     #   jsonschema
     #   jupyter-events
 rfc3986-validator==0.1.1
     # via
     #   jsonschema
     #   jupyter-events
-rq==1.15.0
+rq==1.15.1
     # via dallinger
 s3transfer==0.6.1
     # via boto3
-selenium==4.9.1
+selenium==4.10.0
     # via dallinger
 send2trash==1.8.2
     # via
     #   jupyter-server
     #   nbclassic
     #   notebook
 six==1.16.0
@@ -541,15 +543,15 @@
 sphinx==6.2.1
     # via
     #   dallinger
     #   myst-parser
     #   sphinx-rtd-theme
     #   sphinxcontrib-jquery
     #   sphinxcontrib-spelling
-sphinx-rtd-theme==1.2.1
+sphinx-rtd-theme==1.2.2
     # via dallinger
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
@@ -569,15 +571,15 @@
     #   sqlalchemy-postgres-copy
 sqlalchemy-postgres-copy==0.5.0
     # via dallinger
 sshtunnel==0.4.0
     # via dallinger
 stack-data==0.6.2
     # via ipython
-tablib==3.4.0
+tablib==3.5.0
     # via dallinger
 tabulate==0.9.0
     # via
     #   dallinger
     #   tablib
 tenacity==8.2.2
     # via dallinger
@@ -603,15 +605,15 @@
     # via
     #   ipykernel
     #   jupyter-client
     #   jupyter-server
     #   nbclassic
     #   notebook
     #   terminado
-tox==4.5.2
+tox==4.6.3
     # via dallinger
 traitlets==5.9.0
     # via
     #   comm
     #   ipykernel
     #   ipython
     #   ipywidgets
@@ -627,53 +629,53 @@
     #   nbformat
     #   notebook
     #   qtconsole
 trio==0.22.0
     # via
     #   selenium
     #   trio-websocket
-trio-websocket==0.10.2
+trio-websocket==0.10.3
     # via selenium
 tzdata==2023.3
     # via pandas
 tzlocal==5.0.1
     # via
     #   apscheduler
     #   dallinger
 ua-parser==0.16.1
     # via
     #   dallinger
     #   user-agents
-uri-template==1.2.0
+uri-template==1.3.0
     # via jsonschema
 urllib3==1.26.16
     # via
     #   botocore
     #   docker
     #   requests
     #   selenium
 user-agents==2.2.0
     # via dallinger
-virtualenv==20.23.0
+virtualenv==20.23.1
     # via
     #   pre-commit
     #   tox
 wcwidth==0.2.6
     # via prompt-toolkit
 webcolors==1.13
     # via jsonschema
 webencodings==0.5.1
     # via
     #   bleach
     #   tinycss2
-websocket-client==1.5.2
+websocket-client==1.6.0
     # via
     #   docker
     #   jupyter-server
-werkzeug==2.3.4
+werkzeug==2.3.6
     # via
     #   flask
     #   flask-login
 wheel==0.40.0
     # via pip-tools
 widgetsnbextension==4.0.7
     # via ipywidgets
```

### Comparing `dallinger-9.8.0/docs/Makefile` & `dallinger-9.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/make.bat` & `dallinger-9.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/AvenirLTStd-Book_gdi.eot` & `dallinger-9.8.1/docs/source/_static/AvenirLTStd-Book_gdi.eot`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/AvenirLTStd-Book_gdi.svg` & `dallinger-9.8.1/docs/source/_static/AvenirLTStd-Book_gdi.svg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/AvenirLTStd-Book_gdi.ttf` & `dallinger-9.8.1/docs/source/_static/AvenirLTStd-Book_gdi.ttf`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/AvenirLTStd-Book_gdi.woff` & `dallinger-9.8.1/docs/source/_static/AvenirLTStd-Book_gdi.woff`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/Dallinger AWS Group.png` & `dallinger-9.8.1/docs/source/_static/Dallinger AWS Group.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/barplot.png` & `dallinger-9.8.1/docs/source/_static/barplot.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/burst.png` & `dallinger-9.8.1/docs/source/_static/burst.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/chain.png` & `dallinger-9.8.1/docs/source/_static/chain.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/class_chart.jpg` & `dallinger-9.8.1/docs/source/_static/class_chart.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/corner.jpg` & `dallinger-9.8.1/docs/source/_static/corner.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/custom.css` & `dallinger-9.8.1/docs/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/delayed.png` & `dallinger-9.8.1/docs/source/_static/delayed.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/directories.jpg` & `dallinger-9.8.1/docs/source/_static/directories.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/empty.jpg` & `dallinger-9.8.1/docs/source/_static/empty.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/front_back_layout.jpg` & `dallinger-9.8.1/docs/source/_static/front_back_layout.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/full.png` & `dallinger-9.8.1/docs/source/_static/full.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/grid.png` & `dallinger-9.8.1/docs/source/_static/grid.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/grid_mini.png` & `dallinger-9.8.1/docs/source/_static/grid_mini.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/grid_small.png` & `dallinger-9.8.1/docs/source/_static/grid_small.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/heroku.jpg` & `dallinger-9.8.1/docs/source/_static/heroku.jpg`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/_static/star.png` & `dallinger-9.8.1/docs/source/_static/star.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/aws_etc_keys.rst` & `dallinger-9.8.1/docs/source/aws_etc_keys.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/build_demo_docs.py` & `dallinger-9.8.1/docs/source/build_demo_docs.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/building_documentation.rst` & `dallinger-9.8.1/docs/source/building_documentation.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/classes.rst` & `dallinger-9.8.1/docs/source/classes.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/command_line_utility.rst` & `dallinger-9.8.1/docs/source/command_line_utility.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/communicating_with_the_server.rst` & `dallinger-9.8.1/docs/source/communicating_with_the_server.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/conf.py` & `dallinger-9.8.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/configuration.rst` & `dallinger-9.8.1/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/contributing_to_dallinger.rst` & `dallinger-9.8.1/docs/source/contributing_to_dallinger.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/creating_an_experiment.rst` & `dallinger-9.8.1/docs/source/creating_an_experiment.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/demo_index.rst` & `dallinger-9.8.1/docs/source/demo_index.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/demoing_dallinger.rst` & `dallinger-9.8.1/docs/source/demoing_dallinger.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/demos_on_heroku.rst` & `dallinger-9.8.1/docs/source/demos_on_heroku.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/developing_dallinger_setup_guide.rst` & `dallinger-9.8.1/docs/source/developing_dallinger_setup_guide.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/docker_only.rst` & `dallinger-9.8.1/docs/source/docker_only.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/docker_support.rst` & `dallinger-9.8.1/docs/source/docker_support.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/docker_tutorial.rst` & `dallinger-9.8.1/docs/source/docker_tutorial.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/email_setup.rst` & `dallinger-9.8.1/docs/source/email_setup.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/experiment_data.rst` & `dallinger-9.8.1/docs/source/experiment_data.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/extra_configuration.rst` & `dallinger-9.8.1/docs/source/extra_configuration.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/index.rst` & `dallinger-9.8.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/installing_dallinger_for_users.rst` & `dallinger-9.8.1/docs/source/installing_dallinger_for_users.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/javascript_api.rst` & `dallinger-9.8.1/docs/source/javascript_api.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/learning_to_use_dallinger.rst` & `dallinger-9.8.1/docs/source/learning_to_use_dallinger.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/monitoring_a_live_experiment.rst` & `dallinger-9.8.1/docs/source/monitoring_a_live_experiment.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/networks.rst` & `dallinger-9.8.1/docs/source/networks.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/postico_and_postgres.rst` & `dallinger-9.8.1/docs/source/postico_and_postgres.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/private_repo.rst` & `dallinger-9.8.1/docs/source/private_repo.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/python_module.rst` & `dallinger-9.8.1/docs/source/python_module.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/recruitment.rst` & `dallinger-9.8.1/docs/source/recruitment.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/required_experiment_files.rst` & `dallinger-9.8.1/docs/source/required_experiment_files.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/rewarding_participants.rst` & `dallinger-9.8.1/docs/source/rewarding_participants.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/running_bots.rst` & `dallinger-9.8.1/docs/source/running_bots.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/running_the_tests.rst` & `dallinger-9.8.1/docs/source/running_the_tests.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/scheduled_tasks.rst` & `dallinger-9.8.1/docs/source/scheduled_tasks.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/spelling_wordlist.txt` & `dallinger-9.8.1/docs/source/spelling_wordlist.txt`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/the_experiment_class.rst` & `dallinger-9.8.1/docs/source/the_experiment_class.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/troubleshooting.rst` & `dallinger-9.8.1/docs/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/vagrant_setup.rst` & `dallinger-9.8.1/docs/source/vagrant_setup.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/waiting_rooms.rst` & `dallinger-9.8.1/docs/source/waiting_rooms.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/web_api.rst` & `dallinger-9.8.1/docs/source/web_api.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/docs/source/writing_bots.rst` & `dallinger-9.8.1/docs/source/writing_bots.rst`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/incubator.png` & `dallinger-9.8.1/incubator.png`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/requirements.txt` & `dallinger-9.8.1/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
     # via
     #   outcome
     #   trio
 backcall==0.2.0
     # via ipython
 blinker==1.6.2
     # via flask
-boto3==1.26.146
+boto3==1.26.158
     # via dallinger
-botocore==1.29.146
+botocore==1.29.158
     # via
     #   boto3
     #   s3transfer
 build==0.10.0
     # via
     #   dallinger
     #   pip-tools
@@ -54,15 +54,15 @@
     # via ipython
 exceptiongroup==1.1.1
     # via
     #   trio
     #   trio-websocket
 executing==1.2.0
     # via stack-data
-faker==18.10.1
+faker==18.11.1
     # via dallinger
 flask==2.3.2
     # via
     #   dallinger
     #   flask-crossdomain
     #   flask-login
     #   flask-sockets
@@ -118,14 +118,16 @@
 markupsafe==2.1.3
     # via
     #   jinja2
     #   werkzeug
     #   wtforms
 matplotlib-inline==0.1.6
     # via ipython
+numpy==1.24.3
+    # via dallinger
 outcome==1.2.0
     # via trio
 packaging==23.1
     # via build
 parso==0.8.3
     # via jedi
 pexpect==4.8.0
@@ -169,19 +171,19 @@
     # via
     #   dallinger
     #   rq
 requests==2.31.0
     # via
     #   dallinger
     #   heroku3
-rq==1.15.0
+rq==1.15.1
     # via dallinger
 s3transfer==0.6.1
     # via boto3
-selenium==4.9.1
+selenium==4.10.0
     # via dallinger
 six==1.16.0
     # via
     #   apscheduler
     #   asttokens
     #   dallinger
     #   python-dateutil
@@ -212,15 +214,15 @@
     # via
     #   ipython
     #   matplotlib-inline
 trio==0.22.0
     # via
     #   selenium
     #   trio-websocket
-trio-websocket==0.10.2
+trio-websocket==0.10.3
     # via selenium
 tzlocal==5.0.1
     # via
     #   apscheduler
     #   dallinger
 ua-parser==0.16.1
     # via
@@ -231,15 +233,15 @@
     #   botocore
     #   requests
     #   selenium
 user-agents==2.2.0
     # via dallinger
 wcwidth==0.2.6
     # via prompt-toolkit
-werkzeug==2.3.4
+werkzeug==2.3.6
     # via
     #   flask
     #   flask-login
 wheel==0.40.0
     # via pip-tools
 wsproto==1.2.0
     # via trio-websocket
```

### Comparing `dallinger-9.8.0/setup.py` & `dallinger-9.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 README = (HERE / "README.md").read_text(encoding="utf-8")
 
 
 setup_args = dict(
     name="dallinger",
     packages=["dallinger", "dallinger_scripts"],
-    version="9.8.0",
+    version="9.8.1",
     description="Laboratory automation for the behavioral and social sciences",
     long_description=README,
     long_description_content_type="text/markdown",
     url="http://github.com/Dallinger/Dallinger",
     maintainer="Jordan Suchow",
     maintainer_email="suchow@berkeley.edu",
     license="MIT",
@@ -60,14 +60,15 @@
         "future",
         "gevent",
         "greenlet",
         "gunicorn",
         "heroku3",
         "ipython < 8.13",
         "localconfig",
+        "numpy < 1.25",
         "pexpect",
         "pip>=20",
         "pip-tools",
         "psycopg2",
         "psutil",
         "pyopenssl",
         "redis",
```

### Comparing `dallinger-9.8.0/tests/test_agents.py` & `dallinger-9.8.1/tests/test_agents.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_api.py` & `dallinger-9.8.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_bots.py` & `dallinger-9.8.1/tests/test_bots.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_cli_config.py` & `dallinger-9.8.1/tests/test_cli_config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_command_line.py` & `dallinger-9.8.1/tests/test_command_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,15 +366,16 @@
             "unfilled_networks": 0,
         }
         with mock.patch("dallinger.command_line.requests") as req:
             req.get.return_value = response
             yield req
 
     def test_summary(self, summary, patched_summary_route):
-        result = CliRunner().invoke(summary, ["--app", "some app id"])
+        with mock.patch("dallinger.heroku.tools.HerokuApp.url"):
+            result = CliRunner().invoke(summary, ["--app", "some app id"])
         assert "Yield: 50.00%" in result.output
 
 
 @pytest.mark.usefixtures("bartlett_dir")
 @pytest.mark.slow
 class TestBot(object):
     @pytest.fixture
@@ -396,15 +397,16 @@
         from dallinger.deployment import setup_experiment
 
         setup_experiment(log=mock.Mock())
         bot = bot_factory("some url")
         assert isinstance(bot, BotBase)
 
     def test_bot_no_debug_url(self, bot_command, mock_bot):
-        CliRunner().invoke(bot_command, ["--app", "some app id"])
+        with mock.patch("dallinger.heroku.tools.HerokuApp.url"):
+            CliRunner().invoke(bot_command, ["--app", "some app id"])
 
         assert mock_bot.run_experiment.called
 
     def test_bot_with_debug_url(self, bot_command, mock_bot):
         CliRunner().invoke(bot_command, ["--app", "some app id", "--debug", "some url"])
 
         assert mock_bot.run_experiment.called
```

### Comparing `dallinger-9.8.0/tests/test_config.py` & `dallinger-9.8.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_dashboard.py` & `dallinger-9.8.1/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_data.py` & `dallinger-9.8.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_db.py` & `dallinger-9.8.1/tests/test_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import mock
-import pytest
 
 
 def test_redis():
     from dallinger.db import redis_conn
 
     assert redis_conn.ping()
 
@@ -61,23 +60,22 @@
     serialized_write()
 
     # Which we can check by making sure that `add_participant`
     # calculated the count at least 3 times
     assert counts == [0, 0, 1]
 
 
-@pytest.mark.skip(reason="This test needs to be re-investigated.")
 def test_after_commit_hook(db_session):
-    with mock.patch("dallinger.db.redis_conn") as redis:
+    with mock.patch("dallinger.db.redis_conn.publish") as redis_publish:
         from dallinger.db import queue_message
 
         queue_message("test", "test")
         db_session.commit()
 
-        redis.assert_called_once_with("test", "test")
+        redis_publish.assert_called_once_with("test", "test")
 
 
 def test_create_db_engine_updates_postgresql_scheme():
     old_scheme_uri = "postgres://foo:bar@somehost:5432/blah"
     from dallinger.db import create_db_engine
 
     engine = create_db_engine(old_scheme_uri)
```

### Comparing `dallinger-9.8.0/tests/test_demos.py` & `dallinger-9.8.1/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_deployment.py` & `dallinger-9.8.1/tests/test_deployment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_docker.py` & `dallinger-9.8.1/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_environments.py` & `dallinger-9.8.1/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_experiment.py` & `dallinger-9.8.1/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_experiment_server.py` & `dallinger-9.8.1/tests/test_experiment_server.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_griduniverse.py` & `dallinger-9.8.1/tests/test_griduniverse.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_heroku.py` & `dallinger-9.8.1/tests/test_heroku.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,30 +213,45 @@
         with mock.patch("dallinger.heroku.tools.subprocess"):
             the_app = HerokuApp(dallinger_uid="fake-uid", output=None, team="fake team")
             yield the_app
 
     def test_name(self, app):
         assert app.name == "dlgr-fake-uid"
 
-    def test_url(self, app):
+    def test_url(self, app, check_call, check_output):
+        check_output.return_value = (
+            '{"app": {"web_url": "https://dlgr-fake-uid.herokuapp.com"}}'
+        )
         assert app.url == "https://dlgr-fake-uid.herokuapp.com"
+        check_output.assert_called_once_with(
+            [
+                "heroku",
+                "apps:info",
+                "--app",
+                app.name,
+                "--json",
+            ]
+        )
 
     def test_config_url(self, app):
         assert app.config_url == "https://api.heroku.com/apps/dlgr-fake-uid/config-vars"
 
     def test_dashboard_url(self, app):
         assert app.dashboard_url == "https://dashboard.heroku.com/apps/dlgr-fake-uid"
 
     def test_dashboard_metrics_url(self, app):
         assert (
             app.dashboard_metrics_url
             == "https://dashboard.heroku.com/apps/dlgr-fake-uid/metrics"
         )
 
     def test_bootstrap_creates_app_with_team(self, app, check_call, check_output):
+        check_output.return_value = (
+            '{"app": {"web_url": "https://dlgr-fake-uid.herokuapp.com"}}'
+        )
         app.team = "some-team"
         app.bootstrap()
         check_call.assert_has_calls(
             [
                 mock.call(
                     [
                         "heroku",
@@ -249,14 +264,17 @@
                     ],
                     stdout=None,
                 )
             ]
         )
 
     def test_bootstrap_sets_variables(self, app, check_call, check_output):
+        check_output.return_value = (
+            '{"app": {"web_url": "https://dlgr-fake-uid.herokuapp.com"}}'
+        )
         app.team = "some-team"
         app.bootstrap()
         check_call.assert_called_with(
             [
                 "heroku",
                 "config:set",
                 "CREATOR=test@example.com",
```

### Comparing `dallinger-9.8.0/tests/test_information.py` & `dallinger-9.8.1/tests/test_information.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_jupyter.py` & `dallinger-9.8.1/tests/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_models.py` & `dallinger-9.8.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_mturk.py` & `dallinger-9.8.1/tests/test_mturk.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_networks.py` & `dallinger-9.8.1/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_notifications.py` & `dallinger-9.8.1/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_processes.py` & `dallinger-9.8.1/tests/test_processes.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_prolific.py` & `dallinger-9.8.1/tests/test_prolific.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_recruiters.py` & `dallinger-9.8.1/tests/test_recruiters.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_replay.py` & `dallinger-9.8.1/tests/test_replay.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_replay_state.py` & `dallinger-9.8.1/tests/test_replay_state.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_sockets.py` & `dallinger-9.8.1/tests/test_sockets.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_sources.py` & `dallinger-9.8.1/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_transformations.py` & `dallinger-9.8.1/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `dallinger-9.8.0/tests/test_utils.py` & `dallinger-9.8.1/tests/test_utils.py`

 * *Files identical despite different names*

