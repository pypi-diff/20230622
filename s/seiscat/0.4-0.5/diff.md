# Comparing `tmp/seiscat-0.4.tar.gz` & `tmp/seiscat-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seiscat-0.4.tar", last modified: Tue Jun 20 15:25:37 2023, max compression
+gzip compressed data, was "seiscat-0.5.tar", last modified: Thu Jun 22 15:36:04 2023, max compression
```

## Comparing `seiscat-0.4.tar` & `seiscat-0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:25:37.510487 seiscat-0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-20 15:25:29.000000 seiscat-0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 15:25:29.000000 seiscat-0.4/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 15:25:29.000000 seiscat-0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-20 15:25:29.000000 seiscat-0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-20 15:25:37.510487 seiscat-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-06-20 15:25:29.000000 seiscat-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:25:37.510487 seiscat-0.4/seiscat/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-20 15:25:37.510487 seiscat-0.4/seiscat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:25:37.510487 seiscat-0.4/seiscat/conf/
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/conf/configspec.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:25:37.510487 seiscat-0.4/seiscat/configobj/
--rw-r--r--   0 runner    (1001) docker     (123)    88030 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/configobj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/configobj/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    46990 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/configobj/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/fdsnws.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/print.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:25:37.510487 seiscat-0.4/seiscat/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/scripts/seiscat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-20 15:25:29.000000 seiscat-0.4/seiscat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:25:37.510487 seiscat-0.4/seiscat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-20 15:25:37.000000 seiscat-0.4/seiscat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-20 15:25:37.000000 seiscat-0.4/seiscat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:25:37.000000 seiscat-0.4/seiscat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 15:25:37.000000 seiscat-0.4/seiscat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 15:25:37.000000 seiscat-0.4/seiscat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 15:25:37.000000 seiscat-0.4/seiscat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-20 15:25:37.510487 seiscat-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-20 15:25:29.000000 seiscat-0.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-06-20 15:25:29.000000 seiscat-0.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:36:04.985955 seiscat-0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-22 15:35:56.000000 seiscat-0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-22 15:35:56.000000 seiscat-0.5/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-22 15:35:56.000000 seiscat-0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-22 15:35:56.000000 seiscat-0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-22 15:36:04.985955 seiscat-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-06-22 15:35:56.000000 seiscat-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:36:04.989955 seiscat-0.5/seiscat/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-22 15:36:04.989955 seiscat-0.5/seiscat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:36:04.985955 seiscat-0.5/seiscat/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/conf/configspec.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:36:04.985955 seiscat-0.5/seiscat/configobj/
+-rw-r--r--   0 runner    (1001) docker     (123)    88030 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/configobj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/configobj/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46990 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/configobj/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/fdsnws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/print.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:36:04.985955 seiscat-0.5/seiscat/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/scripts/seiscat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:36:04.985955 seiscat-0.5/seiscat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-22 15:36:04.000000 seiscat-0.5/seiscat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-22 15:36:04.000000 seiscat-0.5/seiscat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 15:36:04.000000 seiscat-0.5/seiscat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-22 15:36:04.000000 seiscat-0.5/seiscat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 15:36:04.000000 seiscat-0.5/seiscat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 15:36:04.000000 seiscat-0.5/seiscat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-22 15:36:04.985955 seiscat-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-22 15:35:56.000000 seiscat-0.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-06-22 15:35:56.000000 seiscat-0.5/versioneer.py
```

### Comparing `seiscat-0.4/LICENSE.txt` & `seiscat-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seiscat-0.4/PKG-INFO` & `seiscat-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seiscat
-Version: 0.4
+Version: 0.5
 Summary: Keep a local seismic catalog
 Home-page: https://seiscat.seismicsource.org
 Author: Claudio Satriano
 Author-email: satriano@ipgp.fr
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://seiscat.seismicsource.org
 Project-URL: Source, https://github.com/SeismicSource/seiscat
```

### Comparing `seiscat-0.4/README.md` & `seiscat-0.5/README.md`

 * *Files identical despite different names*

### Comparing `seiscat-0.4/seiscat/conf/configspec.conf` & `seiscat-0.5/seiscat/conf/configspec.conf`

 * *Files 8% similar despite different names*

```diff
@@ -44,14 +44,19 @@
 # and plural or singular).
 #  ex.: recheck_period = 1 day
 #  ex.: recheck_period = 10 hours
 # This option is only used if end_time is None. Every time the program is run,
 # it will check if new events have been added or if existing events have been
 # updated during the recheck_period.
 recheck_period = string(default=None)
+# Overwrite updated events if they changed during recheck_period (boolean).
+# If False, a new version of the event will be added to the database.
+# The eventid will be the same, but the event version ("ver" column) will be
+# incremented.
+overwrite_updated_events = boolean(default=False)
 # Geographic box selection (decimal degrees or None)
 lat_min = float(min=-90, max=90, default=None)
 lat_max = float(min=-90, max=90, default=None)
 lon_min = float(min=-180, max=360, default=None)
 lon_max = float(min=-180, max=360, default=None)
 # Geographic circular selection.
 # Note, this will override the box selection if both are specified
```

### Comparing `seiscat-0.4/seiscat/configobj/__init__.py` & `seiscat-0.5/seiscat/configobj/__init__.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.4/seiscat/configobj/validate.py` & `seiscat-0.5/seiscat/configobj/validate.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.4/seiscat/fdsnws.py` & `seiscat-0.5/seiscat/fdsnws.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.4/seiscat/plot.py` & `seiscat-0.5/seiscat/plot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-
 # -*- coding: utf8 -*-
 # SPDX-License-Identifier: GPL-3.0-or-later
 """
 Plotting functions for seiscat.
 
 :copyright:
     2022-2023 Claudio Satriano <satriano@ipgp.fr>
 :license:
     GNU General Public License v3.0 or later
     (https://www.gnu.org/licenses/gpl-3.0-standalone.html)
 """
-import sqlite3
 import numpy as np
 import matplotlib.pyplot as plt
-from obspy import UTCDateTime
+from .db import read_events_from_db, get_catalog_stats
 from .utils import err_exit
 
 
 def _get_map_extent_for_suffix(config, suffix=None):
     """
     Get the map extent for a suffix.
 
@@ -90,65 +88,36 @@
         )
     )
     tile_scale = tile_autoscaler.scale_from_extent(extent)
     # print(f'tile_scale: {tile_scale}')
     return int(tile_scale)
 
 
-def _read_event_db(config):
-    """
-    Read event database. Return a list of events.
-
-    :param config: config object
-    :returns: list of events, each event is a dictionary
-    """
-    db_file = config.get('db_file', None)
-    if db_file is None:
-        err_exit('db_file not set in config file')
-    try:
-        open(db_file, 'r')
-    except FileNotFoundError:
-        err_exit(f'Database file "{db_file}" not found.')
-    conn = sqlite3.connect(db_file)
-    c = conn.cursor()
-    # read field names
-    c.execute('PRAGMA table_info(events)')
-    fields = c.fetchall()
-    # read events
-    c.execute('SELECT * FROM events')
-    events = c.fetchall()
-    conn.close()
-    # create a list of dictionaries
-    events_list = []
-    for event in events:
-        event_dict = {field[1]: event[i] for i, field in enumerate(fields)}
-        event_dict['time'] = UTCDateTime(event_dict['time'])
-        events_list.append(event_dict)
-    return events_list
-
-
-def _plot_events(events, scale, ax):
+def _plot_events(ax, events, scale, plot_version_number=False):
     """
     Plot events on a map.
 
     :param events: list of events, each event is a dictionary
     :param scale: scale for event markers
     :param ax: matplotlib axes object
     """
     import cartopy.crs as ccrs
     marker_scale = scale / 10. * 2
     ev_attributes = [
-        (e['evid'], e['time'], e['lon'], e['lat'], e['dep'],
+        (e['evid'], e['ver'], e['time'], e['lon'], e['lat'], e['depth'],
          e['mag'], np.exp(e['mag']) * marker_scale)
         for e in events
     ]
+    # Sort events by time, so that the latest event is plotted on top
+    ev_attributes.sort(key=lambda x: x[2])
     markers = []
-    for evid, time, lon, lat, dep, mag, size in ev_attributes:
+    for evid, ver, time, lon, lat, depth, mag, size in ev_attributes:
+        _evid = f'{evid} v{ver}' if plot_version_number else evid
         marker_label = (
-            f'{evid} M{mag:.1f} {dep:.1f} km\n'
+            f'{_evid} M{mag:.1f} {depth:.1f} km\n'
             f'{time.strftime("%Y-%m-%d %H:%M:%S")}')
         marker = ax.scatter(
             lon, lat,
             s=size,
             facecolor='red', edgecolor='black',
             label=marker_label,
             zorder=10,
@@ -215,21 +184,13 @@
         ccrs.cartopy.feature.BORDERS, edgecolor='black', linewidth=1)
     g_kwargs = dict(draw_labels=True, dms=True, x_inline=False, y_inline=False)
     ax.gridlines(**g_kwargs)
 
     def redraw_gridlines(ax):
         ax.gridlines(**g_kwargs)
     ax.callbacks.connect('xlim_changed', lambda ax: redraw_gridlines(ax))
-    events = _read_event_db(config)
-    _plot_events(events, config['args'].scale, ax)
-    nevents = len(events)
-    tmin = min(event['time'] for event in events)
-    tmax = max(event['time'] for event in events)
-    tmin = tmin.strftime('%Y-%m-%dT%H:%M:%S')
-    tmax = tmax.strftime('%Y-%m-%dT%H:%M:%S')
-    mag_min = min(event['mag'] for event in events)
-    mag_max = max(event['mag'] for event in events)
-    ax.set_title(
-        f'{nevents} events from {tmin} to {tmax}\n'
-        f'Magnitude range: {mag_min:.1f} - {mag_max:.1f}'
-    )
+    events = read_events_from_db(config)
+    scale = config['args'].scale
+    plot_version_number = config['args'].allversions
+    _plot_events(ax, events, scale, plot_version_number)
+    ax.set_title(get_catalog_stats(config))
     plt.show()
```

### Comparing `seiscat-0.4/seiscat/print.py` & `seiscat-0.5/seiscat/print.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,50 +5,63 @@
 
 :copyright:
     2022-2023 Claudio Satriano <satriano@ipgp.fr>
 :license:
     GNU General Public License v3.0 or later
     (https://www.gnu.org/licenses/gpl-3.0-standalone.html)
 """
-import sqlite3
+from .db import read_fields_and_rows_from_db, get_catalog_stats
 from .utils import err_exit
 
 
-def print_catalog(config):
+def print_catalog_stats(config):
+    """
+    Print catalog statistics.
+
+    :param config: config object
+    """
+    print(get_catalog_stats(config))
+
+
+def print_catalog_table(config):
     """
     Pretty-print the catalog as a table.
 
     :param config: config object
     """
-    db_file = config.get('db_file', None)
-    if db_file is None:
-        err_exit('db_file not set in config file')
-    try:
-        open(db_file, 'r')
-    except FileNotFoundError:
-        err_exit(f'Database file "{db_file}" not found.')
-    conn = sqlite3.connect(db_file)
-    c = conn.cursor()
-    # get fields
-    c.execute('PRAGMA table_info(events)')
-    fields = c.fetchall()
-    c.execute('SELECT * FROM events')
-    rows = c.fetchall()
+    fields, rows = read_fields_and_rows_from_db(config)
     if len(rows) == 0:
         print('No events in catalog')
         return
     # get max length of each field
-    max_len = [len(f[1]) for f in fields]
+    max_len = [len(f) for f in fields]
     for row in rows:
         for i, val in enumerate(row):
             max_len[i] = max(max_len[i], len(str(val)))
     # print header
     for i, f in enumerate(fields):
-        print(f'{f[1]:{max_len[i]}}', end=' ')
+        print(f'{f:{max_len[i]}}', end=' ')
     print()
-    # print rows
-    for row in rows:
+    # print rows sorted by time and version
+    time_idx = fields.index('time')
+    ver_idx = fields.index('ver')
+    reverse = config['args'].reverse
+    for row in sorted(
+            rows, key=lambda r: (r[time_idx], r[ver_idx]), reverse=reverse):
         for i, val in enumerate(row):
             val = 'None' if val is None else val
             print(f'{val:{max_len[i]}}', end=' ')
         print()
-    conn.close()
+
+
+def print_catalog(config):
+    """
+    Print catalog.
+
+    :param config: config object
+    """
+    if config['args'].format == 'stats':
+        print_catalog_stats(config)
+    elif config['args'].format == 'table':
+        print_catalog_table(config)
+    else:
+        err_exit(f'Unknown format "{config["args"].format}"')
```

### Comparing `seiscat-0.4/seiscat/scripts/seiscat.py` & `seiscat-0.5/seiscat/scripts/seiscat.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,16 +20,41 @@
 def parse_arguments():
     """Parse command line arguments."""
     parser = argparse.ArgumentParser(
         description='Keep a local seismic catalog.')
     subparser = parser.add_subparsers(dest='action')
     subparser.add_parser('initdb', help='initialize database')
     subparser.add_parser('updatedb', help='update database')
-    subparser.add_parser('print', help='print catalog')
-    plot_parser = subparser.add_parser('plot', help='plot catalog map')
+    versions_parser = argparse.ArgumentParser(add_help=False)
+    versions_parser.add_argument(
+        '-a',
+        '--allversions',
+        action='store_true',
+        default=False,
+        help='show all versions of each event (default: %(default)s)'
+    )
+    print_parser = subparser.add_parser(
+        'print', parents=[versions_parser], help='print catalog')
+    print_parser.add_argument(
+        '-f',
+        '--format',
+        type=str,
+        default='table',
+        choices=['table', 'stats'],
+        help='output format (default: %(default)s)'
+    )
+    print_parser.add_argument(
+        '-r',
+        '--reverse',
+        action='store_true',
+        default=False,
+        help='print catalog in reverse order (default: %(default)s)'
+    )
+    plot_parser = subparser.add_parser(
+        'plot', parents=[versions_parser], help='plot catalog map')
     plot_parser.add_argument(
         '-s',
         '--scale',
         type=float,
         default=10,
         help='scale factor for marker size (default: %(default)s)'
     )
@@ -60,16 +85,20 @@
     Download events and store them in the database.
 
     :param config: config object
     :param initdb: if True, create new database file
     """
     from ..db import check_db_exists, write_catalog_to_db
     from ..fdsnws import open_fdsn_connection, query_events
+    from ..utils import err_exit
     check_db_exists(config, initdb)
-    client = open_fdsn_connection(config)
+    try:
+        client = open_fdsn_connection(config)
+    except Exception as e:
+        err_exit(e)
     cat = query_events(client, config, first_query=initdb)
     write_catalog_to_db(cat, config, initdb)
 
 
 def run():
     """Run seiscat."""
     args = parse_arguments()
```

### Comparing `seiscat-0.4/seiscat/utils.py` & `seiscat-0.5/seiscat/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: utf-8 -*-
+# -*- coding: utf8 -*-
 # SPDX-License-Identifier: GPL-3.0-or-later
 """
 Utility functions for seiscat.
 
 :copyright:
     2022-2023 Claudio Satriano <satriano@ipgp.fr>
 :license:
```

### Comparing `seiscat-0.4/seiscat.egg-info/PKG-INFO` & `seiscat-0.5/seiscat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seiscat
-Version: 0.4
+Version: 0.5
 Summary: Keep a local seismic catalog
 Home-page: https://seiscat.seismicsource.org
 Author: Claudio Satriano
 Author-email: satriano@ipgp.fr
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://seiscat.seismicsource.org
 Project-URL: Source, https://github.com/SeismicSource/seiscat
```

### Comparing `seiscat-0.4/seiscat.egg-info/SOURCES.txt` & `seiscat-0.5/seiscat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seiscat-0.4/setup.py` & `seiscat-0.5/setup.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.4/versioneer.py` & `seiscat-0.5/versioneer.py`

 * *Files identical despite different names*

