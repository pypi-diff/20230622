# Comparing `tmp/netbox-topology-views-3.6.0b1.tar.gz` & `tmp/netbox-topology-views-3.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-topology-views-3.6.0b1.tar", last modified: Tue May 30 14:58:04 2023, max compression
+gzip compressed data, was "netbox-topology-views-3.6.0b2.tar", last modified: Thu Jun 22 07:20:47 2023, max compression
```

## Comparing `netbox-topology-views-3.6.0b1.tar` & `netbox-topology-views-3.6.0b2.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.392943 netbox-topology-views-3.6.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-05-30 14:58:04.392943 netbox-topology-views-3.6.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.380943 netbox-topology-views-3.6.0b1/netbox_topology_views/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.384943 netbox-topology-views-3.6.0b1/netbox_topology_views/api/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.384943 netbox-topology-views-3.6.0b1/netbox_topology_views/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/migrations/0002_individualoptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/migrations/0003_individualoptions_show_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/migrations/0004_coordinategroup_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/migrations/0005_individualoptions_save_coords.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.380943 netbox-topology-views-3.6.0b1/netbox_topology_views/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.380943 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.384943 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/css/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/css/app.css
--rw-r--r--   0 runner    (1001) docker     (123)   220074 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/css/vendor.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.388943 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/
--rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/backup.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/camera.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/circuit.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/console-server.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/core-router.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/database-server.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/database.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/desktop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/firewall.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/kvm.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17466 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/modem.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/notebook.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/pabx.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/pdu.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/phone.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/power-units.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/printer.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/proxy.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/router.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/server.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/siem.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/storage.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/switch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/ups.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.388943 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/js/
--rw-r--r--   0 runner    (1001) docker     (123)   350175 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/js/app.js
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/js/images.js
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/js/images.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.380943 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.392943 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/coordinate.html
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/coordinate_add.html
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/coordinate_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/coordinate_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/coordinategroup.html
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/coordinategroup_add.html
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/coordinategroup_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/coordinategroup_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/images.html
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/individual_options.html
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/location_button.html
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/site_button.html
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/toasts.html
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    10707 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36634 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/netbox_topology_views/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:04.380943 netbox-topology-views-3.6.0b1/netbox_topology_views.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-05-30 14:58:04.000000 netbox-topology-views-3.6.0b1/netbox_topology_views.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-30 14:58:04.000000 netbox-topology-views-3.6.0b1/netbox_topology_views.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:58:04.000000 netbox-topology-views-3.6.0b1/netbox_topology_views.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 14:58:04.000000 netbox-topology-views-3.6.0b1/netbox_topology_views.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:58:04.392943 netbox-topology-views-3.6.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-30 14:57:52.000000 netbox-topology-views-3.6.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:20:47.358682 netbox-topology-views-3.6.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-06-22 07:20:47.358682 netbox-topology-views-3.6.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:20:47.338681 netbox-topology-views-3.6.0b2/netbox_topology_views/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:20:47.342681 netbox-topology-views-3.6.0b2/netbox_topology_views/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:20:47.342681 netbox-topology-views-3.6.0b2/netbox_topology_views/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/migrations/0002_individualoptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/migrations/0003_individualoptions_show_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/migrations/0004_coordinategroup_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/migrations/0005_individualoptions_save_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:20:47.338681 netbox-topology-views-3.6.0b2/netbox_topology_views/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:20:47.338681 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:20:47.342681 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/css/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)   220074 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/css/vendor.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:20:47.354681 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    20139 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/backup.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/camera.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10537 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/circuit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/console-server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/core-router.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/database-server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/database.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/desktop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/firewall.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/kvm.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17466 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/modem.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/notebook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/pabx.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/pdu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/phone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/power-units.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/printer.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/proxy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/router.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/server.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/siem.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/storage.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7764 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/ups.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:20:47.354681 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   350199 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/js/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/js/images.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/js/images.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:20:47.338681 netbox-topology-views-3.6.0b2/netbox_topology_views/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:20:47.358682 netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/coordinate.html
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/coordinate_add.html
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/coordinate_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/coordinate_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/coordinategroup.html
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/coordinategroup_add.html
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/coordinategroup_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/coordinategroup_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/images.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/individual_options.html
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/location_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/site_button.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/toasts.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36784 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/netbox_topology_views/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:20:47.342681 netbox-topology-views-3.6.0b2/netbox_topology_views.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-06-22 07:20:47.000000 netbox-topology-views-3.6.0b2/netbox_topology_views.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-06-22 07:20:47.000000 netbox-topology-views-3.6.0b2/netbox_topology_views.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 07:20:47.000000 netbox-topology-views-3.6.0b2/netbox_topology_views.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 07:20:47.000000 netbox-topology-views-3.6.0b2/netbox_topology_views.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 07:20:47.358682 netbox-topology-views-3.6.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-22 07:20:32.000000 netbox-topology-views-3.6.0b2/setup.py
```

### Comparing `netbox-topology-views-3.6.0b1/LICENSE` & `netbox-topology-views-3.6.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/PKG-INFO` & `netbox-topology-views-3.6.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-topology-views
-Version: 3.6.0b1
+Version: 3.6.0b2
 Summary: An NetBox plugin to create Topology maps
 Home-page: https://github.com/mattieserver/netbox-topology-views
 Author: Mattijs Vanhaverbeke
 License: Apache 2.0
 Project-URL: Source, https://github.com/mattieserver/netbox-topology-views
 Keywords: netbox-plugin
 Classifier: Programming Language :: Python
```

### Comparing `netbox-topology-views-3.6.0b1/README.md` & `netbox-topology-views-3.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/__init__.py` & `netbox-topology-views-3.6.0b2/netbox_topology_views/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from extras.plugins import PluginConfig
 
 
 class TopologyViewsConfig(PluginConfig):
     name = "netbox_topology_views"
     verbose_name = "Topology views"
     description = "An plugin to render topology maps"
-    version = "3.6.0-beta.1"
+    version = "3.6.0-beta.2"
     author = "Mattijs Vanhaverbeke"
     author_email = "author@example.com"
     base_url = "netbox_topology_views"
     required_settings = []
     default_settings = {
         "static_image_directory": "netbox_topology_views/img",
         "allow_coordinates_saving": False,
```

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/api/serializers.py` & `netbox-topology-views-3.6.0b2/netbox_topology_views/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/api/views.py` & `netbox-topology-views-3.6.0b2/netbox_topology_views/api/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,17 +138,20 @@
     @action(detail=False, methods=["post"])
     def save(self, request):
         if not isinstance(request.data, dict):
             return JsonResponse(
                 {"status": "Missing or malformed request body"}, status=400
             )
 
-        device_roles = {k: v for k, v in request.data.items() if k.isnumeric()}
+        device_roles = {
+            k: v.removeprefix(settings.STATIC_URL)
+            for k, v in request.data.items()
+            if k.isnumeric()}
         content_type_ids = {
-            k[2:]: v
+            k[2:]: v.removeprefix(settings.STATIC_URL)
             for k, v in request.data.items()
             if k.startswith("ct") and k[2:].isnumeric()
         }
 
         roles: Dict[int, DeviceRole] = DeviceRole.objects.in_bulk(device_roles.keys())
         content_types: Dict[int, ContentType] = ContentType.objects.in_bulk(
             content_type_ids.keys()
```

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/filters.py` & `netbox-topology-views-3.6.0b2/netbox_topology_views/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/forms.py` & `netbox-topology-views-3.6.0b2/netbox_topology_views/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/migrations/0001_initial.py` & `netbox-topology-views-3.6.0b2/netbox_topology_views/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/migrations/0002_individualoptions.py` & `netbox-topology-views-3.6.0b2/netbox_topology_views/migrations/0002_individualoptions.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/migrations/0004_coordinategroup_coordinate.py` & `netbox-topology-views-3.6.0b2/netbox_topology_views/migrations/0004_coordinategroup_coordinate.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/models.py` & `netbox-topology-views-3.6.0b2/netbox_topology_views/models.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/navigation.py` & `netbox-topology-views-3.6.0b2/netbox_topology_views/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/signals.py` & `netbox-topology-views-3.6.0b2/netbox_topology_views/signals.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/css/vendor.css` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/css/vendor.css`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/LICENSE` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/access-switch.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/backhaul.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/backup.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/backup.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/cable-doubler.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/camera-server.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/camera.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/camera.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/circuit.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/circuit.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/console-server.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/console-server.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/core-router.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/core-router.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/core-switch.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/database-server.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/database-server.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/database.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/database.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/dect-station.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/desktop.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/desktop.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/distribution-switch.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/docking-station.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/environment-monitor.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/fire-alarm-control-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/firewall.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/firewall.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/fo-patch-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/intrusion-alarm-system.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/kvm-over-ip.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/kvm.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/kvm.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/load-balancer.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/mobile-phone.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/modem.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/modem.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/network-socket.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/notebook.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/notebook.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/pabx.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/pabx.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/patch-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/pdu.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/pdu.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/phone.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/phone.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/power-panel.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/power-units.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/power-units.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/printer.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/printer.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/provider-networks.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/proxy.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/proxy.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/role-unknown.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/router.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/router.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/server.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/server.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/siem.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/siem.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/storage.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/storage.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/switch.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/switch.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/time-recording-terminal.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/ups.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/ups.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/usb-lan-adapter.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/wan-network.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/img/wireless-ap.svg`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/js/app.js` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/js/app.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -13155,15 +13155,15 @@
             Sn != null && (!Sn.checked || Promise.allSettled(Object.entries(Ge.getPositions(s.nodes)).map(a => Xi(this, [a], function*([o, r]) {
                 window.nodes.update({
                     id: parseInt(o),
                     physics: !1,
                     x: r.x,
                     y: r.y
                 });
-                let d = yield fetch("/api/plugins/netbox_topology_views/save-coords/save_coords/", {
+                let d = yield fetch("/" + basePath + "api/plugins/netbox_topology_views/save-coords/save_coords/", {
                     method: "PATCH",
                     headers: {
                         "X-CSRFToken": Ba,
                         Accept: "application/json",
                         "Content-Type": "application/json"
                     },
                     body: JSON.stringify({
@@ -13211,15 +13211,15 @@
                 var i = t.split(o)[1];
                 i = i.split("/")[0], e = "site_id=" + i + "&show_cables=on&show_unconnected=on"
             } else if (t.includes(r)) {
                 var s = t.split(r)[1];
                 s = s.split("/")[0], e = "location_id=" + s + "&show_cables=on&show_unconnected=on"
             }
         } else e = new URLSearchParams(window.location.search);
-        fetch("/api/plugins/netbox_topology_views/xml-export/?" + e).then(o => o.text()).then(o => {
+        fetch("/" + basePath + "api/plugins/netbox_topology_views/xml-export/?" + e).then(o => o.text()).then(o => {
             var r = new Blob([o], {
                 type: "text/plain"
             });
             n.setAttribute("href", window.URL.createObjectURL(r)), n.setAttribute("download", "topology.xml"), n.dataset.downloadurl = ["text/plain", n.download, n.href].join(":"), n.click()
         })
     }
     var ja = new MutationObserver(n => n.forEach(e => {
```

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/js/images.js` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/js/images.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -45,15 +45,15 @@
         }
     };
     var g = {},
         p = d("csrftoken");
     document.querySelector("form#images").addEventListener("submit", e => l(void 0, null, function*() {
         e.preventDefault();
         try {
-            let t = yield fetch("/api/plugins/netbox_topology_views/images/save/", {
+            let t = yield fetch("/" + basePath + "api/plugins/netbox_topology_views/images/save/", {
                 method: "POST",
                 body: JSON.stringify(g),
                 headers: {
                     "X-CSRFToken": p,
                     "Content-Type": "application/json"
                 }
             });
```

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/static/netbox_topology_views/js/images.js.map` & `netbox-topology-views-3.6.0b2/netbox_topology_views/static/netbox_topology_views/js/images.js.map`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'mappings'": "'mNAAO,GAAM,GAAY,AAAC,GAAS,CAC/B,GAAI,CAAC,SAAS,OAAQ,OAEtB,GAAI,GAAc,KACZ,EAAU,SAAS,OAAO,MAAM,KAEtC,OAAS,GAAI,EAAG,EAAI,EAAQ,OAAQ,IAAK,CACrC,GAAM,GAAS,EAAQ,GAAG,OAE1B,GAAI,EAAO,UAAU,EAAG,EAAK,OAAS,KAAO,EAAO,IAAK,CACrD,EAAc,mBAAmB,EAAO,UAAU,EAAK,OAAS,IAChE,OAIR,MAAO,ICfJ,GAAM,GAAQ,CACjB,QAAS,AAAC,GAAY,CAClB,GAAM,GAAK,SAAS,cAAc,kCAClC,GAAI,CAAC,EAAI,MAAO,SAAQ,MAAM,mCAC9B,GAAM,GAAU,EAAG,cAAc,QACjC,EAAQ,YAAc,EAEtB,AADc,GAAI,QAAO,MAAM,GACzB,QAEV,MAAO,AAAC,GAAY,CAChB,GAAM,GAAK,SAAS,cAAc,gCAClC,GAA […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "mappings": "mNAAO,GAAM,GAAY,AAAC,GAAS,CAC/B,GAAI,CAAC,SAAS,OAAQ,OAEtB,GAAI,GAAc,KACZ,EAAU,SAAS,OAAO,MAAM,KAEtC,OAAS,GAAI,EAAG,EAAI,EAAQ,OAAQ,IAAK,CACrC,GAAM,GAAS,EAAQ,GAAG,OAE1B,GAAI,EAAO,UAAU,EAAG,EAAK,OAAS,KAAO,EAAO,IAAK,CACrD,EAAc,mBAAmB,EAAO,UAAU,EAAK,OAAS,IAChE,OAIR,MAAO,ICfJ,GAAM,GAAQ,CACjB,QAAS,AAAC,GAAY,CAClB,GAAM,GAAK,SAAS,cAAc,kCAClC,GAAI,CAAC,EAAI,MAAO,SAAQ,MAAM,mCAC9B,GAAM,GAAU,EAAG,cAAc,QACjC,EAAQ,YAAc,EAEtB,AADc,GAAI,QAAO,MAAM,GACzB,QAEV,MAAO,AAAC,GAAY,CAChB,GAAM,GAAK,SAAS,cAAc,gCAClC,GAAI,CAAC,EAAI,MAAO,SAAQ,MAAM,mCAC9B,GAAM,GAAU,EAAG,cAAc,QACjC,EAAQ,YAAc,EAEtB,AADc,GAAI,QAAO,MAAM,GACzB,SCZd,GAAM,GAAU,GACV,EAAY,EAAU,aAE5B,SAAS,cAAc,eAAe,iBAAiB,SAAU,AAAO,GAAM,0BAC1E,EAAE,iBACF,GAAI,CACA,GAAM,GAAM,KAAM,OAAM,kDAAmD,CACvE,OAAQ,OACR,KAAM,KAAK,UAAU,GACrB,QAAS,CACL,cAAe,EACf,eAAgB,sBAIxB,GAAI,CAAC,EAAI,GAAI,KAAM,IAAI,OAAM,KAAM,GAAI,QACvC,EAAM,QAAQ,wBACT,EAAP,CACE,QAAQ,IAAI,GACZ,EAAM,MAAM,EAAI,aAIxB,SAAS,iBAAiB,kCAAkC,QAAQ,AAAC,GAAO,CACxE,EAAG,iBAAiB,QAAS,AAAC,GAAM,CA3BxC,MA4BQ,GAAI,CAAE,GAAE,wBAAyB,cAAc,OAC/C,GAAM,CACF,QAAS,CAAE,OAAM,UACjB,EAAE,cAEN,EAAQ,GAAQ,EAEhB,GAAM,GAAS,KAAE,cACZ,QAAQ,eADE,cAET,cAAc,sBAAsB,KAC1C,AAAI,GAAQ,GAAO,UAAY,aAAa",
+    "mappings": "mNAAO,GAAM,GAAY,AAAC,GAAS,CAC/B,GAAI,CAAC,SAAS,OAAQ,OAEtB,GAAI,GAAc,KACZ,EAAU,SAAS,OAAO,MAAM,KAEtC,OAAS,GAAI,EAAG,EAAI,EAAQ,OAAQ,IAAK,CACrC,GAAM,GAAS,EAAQ,GAAG,OAE1B,GAAI,EAAO,UAAU,EAAG,EAAK,OAAS,KAAO,EAAO,IAAK,CACrD,EAAc,mBAAmB,EAAO,UAAU,EAAK,OAAS,IAChE,OAIR,MAAO,ICfJ,GAAM,GAAQ,CACjB,QAAS,AAAC,GAAY,CAClB,GAAM,GAAK,SAAS,cAAc,kCAClC,GAAI,CAAC,EAAI,MAAO,SAAQ,MAAM,mCAC9B,GAAM,GAAU,EAAG,cAAc,QACjC,EAAQ,YAAc,EAEtB,AADc,GAAI,QAAO,MAAM,GACzB,QAEV,MAAO,AAAC,GAAY,CAChB,GAAM,GAAK,SAAS,cAAc,gCAClC,GAAI,CAAC,EAAI,MAAO,SAAQ,MAAM,mCAC9B,GAAM,GAAU,EAAG,cAAc,QACjC,EAAQ,YAAc,EAEtB,AADc,GAAI,QAAO,MAAM,GACzB,SCZd,GAAM,GAAU,GACV,EAAY,EAAU,aAE5B,SAAS,cAAc,eAAe,iBAAiB,SAAU,AAAO,GAAM,0BAC1E,EAAE,iBACF,GAAI,CACA,GAAM,GAAM,KAAM,OAAM,IAAM,SAAW,iDAAkD,CACvF,OAAQ,OACR,KAAM,KAAK,UAAU,GACrB,QAAS,CACL,cAAe,EACf,eAAgB,sBAIxB,GAAI,CAAC,EAAI,GAAI,KAAM,IAAI,OAAM,KAAM,GAAI,QACvC,EAAM,QAAQ,wBACT,EAAP,CACE,QAAQ,IAAI,GACZ,EAAM,MAAM,EAAI,aAIxB,SAAS,iBAAiB,kCAAkC,QAAQ,AAAC,GAAO,CACxE,EAAG,iBAAiB,QAAS,AAAC,GAAM,CA3BxC,MA4BQ,GAAI,CAAE,GAAE,wBAAyB,cAAc,OAC/C,GAAM,CACF,QAAS,CAAE,OAAM,UACjB,EAAE,cAEN,EAAQ,GAAQ,EAEhB,GAAM,GAAS,KAAE,cACZ,QAAQ,eADE,cAET,cAAc,sBAAsB,KAC1C,AAAI,GAAQ,GAAO,UAAY,aAAa",
     "names": [],
     "sources": [
         "../../../static_dev/js/csrftoken.js",
         "../../../static_dev/js/toast.js",
         "../../../static_dev/js/images.js"
     ],
     "version": 3
```

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/tables.py` & `netbox-topology-views-3.6.0b2/netbox_topology_views/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/template_content.py` & `netbox-topology-views-3.6.0b2/netbox_topology_views/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/coordinate.html` & `netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/coordinate.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/coordinategroup.html` & `netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/coordinategroup.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html` & `netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/htmx_topology.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/images.html` & `netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/images.html`

 * *Files 10% similar despite different names*

```diff
@@ -38,9 +38,12 @@
 
     <button class="btn btn-primary" type="submit">Save</button>
   </form>
   {% include 'netbox_topology_views/toasts.html' %}
 {% endblock content-wrapper %}
 
 {% block javascript %}
-  <script src="{% static 'netbox_topology_views/js/images.js' %}" defer></script>
-{% endblock javascript %}
+<script type="text/javascript">
+  const basePath = '{{ basepath }}';
+</script>
+<script src="{% static 'netbox_topology_views/js/images.js' %}" defer></script>
+{% endblock javascript %}
```

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/index.html` & `netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -73,10 +73,11 @@
   {% endwith %}
 {% endblock content-wrapper %}
 
 {% block javascript %}
   <script type="text/javascript">
     const brokenImage = '{{ broken_image }}';
     const topologyData = {{ topology_data | safe }};
+    const basePath = '{{ basepath }}';
   </script>
 	<script src="{% static 'netbox_topology_views/js/app.js' %}" defer></script>
 {% endblock javascript %}
```

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/templates/netbox_topology_views/toasts.html` & `netbox-topology-views-3.6.0b2/netbox_topology_views/templates/netbox_topology_views/toasts.html`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/urls.py` & `netbox-topology-views-3.6.0b2/netbox_topology_views/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/utils.py` & `netbox-topology-views-3.6.0b2/netbox_topology_views/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,26 +25,25 @@
         plugin_path_new = plugin_path[len(prefix):]
         CONF_IMAGE_DIR: Path = Path(settings.STATIC_ROOT) / plugin_path_new
     else:
         CONF_IMAGE_DIR: Path = Path(settings.STATIC_ROOT) / plugin_path
 
 
 def image_static_url(path: Path) -> str:
-    return settings.BASE_PATH + static(
+    return static(
         f"/{path.relative_to(Path(settings.STATIC_ROOT))}"
     )
 
 
 def get_image_from_url(url: str) -> str:
-    url_path = settings.BASE_PATH + settings.STATIC_URL
     if sys.version_info >= (3,9,0):
-        return url.removeprefix(url_path)
+        return url.removeprefix(settings.STATIC_URL)
     else:
-        if url.startswith(url_path):
-            url_new = url[len(url_path):]
+        if url.startswith(settings.STATIC_URL):
+            url_new = url[len(settings.STATIC_URL):]
             return url_new
         else:
             return url
 
 
 IMAGE_FILETYPES = (
     "apng",
@@ -246,15 +245,15 @@
 
         mxcell.appendChild(mxgeometry)
 
     # nodes
     noPositionX = 0
     noPositionY = 1000
     for node in data['nodes']:
-        with open(str(Path(settings.BASE_DIR)) + node['image'], "rb") as img:
+        with open(settings.STATIC_ROOT + '/' + get_image_from_url(node['image']), "rb") as img:
             svg = base64.b64encode(img.read()).decode('utf-8')
         mxcell = doc.createElement('mxCell')
         mxcell.setAttribute('id', 'node_' + str(node['id']))
         mxcell.setAttribute('value', str(node['label']))
         mxcell.setAttribute('style', 'shape=image;verticalLabelPosition=bottom;verticalAlign=top;imageAspect=0;aspect=fixed;image=data:image/svg+xml,' + svg + ';perimeter=elippsePerimeter;fontSize=10;strokeWidth=1;fontColor=#000000;')
         mxcell.setAttribute('vertex', '1')
         mxcell.setAttribute('parent', '1')
```

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views/views.py` & `netbox-topology-views-3.6.0b2/netbox_topology_views/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -719,26 +719,28 @@
             return render(
                 request,
                 "netbox_topology_views/htmx_topology.html",
                 {
                     "filter_form": DeviceFilterForm(request.GET, label_suffix=""),
                     "topology_data": json.dumps(topo_data),
                     "broken_image": find_image_url("role-unknown"),
-                    "epoch": int(time.time())
+                    "epoch": int(time.time()),
+                    "basepath": settings.BASE_PATH,
                 },
             )
 
         return render(
             request,
             "netbox_topology_views/index.html",
             {
                 "filter_form": DeviceFilterForm(request.GET, label_suffix=""),
                 "topology_data": json.dumps(topo_data),
                 "broken_image": find_image_url("role-unknown"),
-                "model": self.model
+                "model": self.model,
+                "basepath": settings.BASE_PATH,
             },
         )
 
 
 CONFIG = settings.PLUGINS_CONFIG["netbox_topology_views"]
 ADDITIONAL_ROLES = (PowerPanel, PowerFeed, Circuit)
 
@@ -789,14 +791,15 @@
 
         return render(
             request,
             "netbox_topology_views/images.html",
             {
                 "roles": sorted(list(roles.values()), key=lambda r: r["name"]),
                 "images": images,
+                "basepath": settings.BASE_PATH,
             },
         )
 
 class CoordinateView(PermissionRequiredMixin, ObjectView):
     permission_required = 'netbox_topology_views.view_coordinate'
 
     queryset = Coordinate.objects.all()
```

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views.egg-info/PKG-INFO` & `netbox-topology-views-3.6.0b2/netbox_topology_views.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-topology-views
-Version: 3.6.0b1
+Version: 3.6.0b2
 Summary: An NetBox plugin to create Topology maps
 Home-page: https://github.com/mattieserver/netbox-topology-views
 Author: Mattijs Vanhaverbeke
 License: Apache 2.0
 Project-URL: Source, https://github.com/mattieserver/netbox-topology-views
 Keywords: netbox-plugin
 Classifier: Programming Language :: Python
```

### Comparing `netbox-topology-views-3.6.0b1/netbox_topology_views.egg-info/SOURCES.txt` & `netbox-topology-views-3.6.0b2/netbox_topology_views.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-topology-views-3.6.0b1/setup.py` & `netbox-topology-views-3.6.0b2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 readme = Path(__file__).parent / "README.md"
 long_description = readme.read_text()
 
 setup(
     name="netbox-topology-views",
-    version="3.6.0-beta.1",
+    version="3.6.0-beta.2",
     description="An NetBox plugin to create Topology maps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mattieserver/netbox-topology-views",
     author="Mattijs Vanhaverbeke",
     license="Apache 2.0",
     install_requires=[],
```

