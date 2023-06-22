# Comparing `tmp/couchcopy-0.1.5.tar.gz` & `tmp/couchcopy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "couchcopy-0.1.5.tar", last modified: Mon Jan 10 13:45:17 2022, max compression
+gzip compressed data, was "couchcopy-0.2.0.tar", last modified: Thu Jun 22 10:36:35 2023, max compression
```

## Comparing `couchcopy-0.1.5.tar` & `couchcopy-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,13 @@
-drwxr-xr-x   0 hoel      (1000) hoel      (1000)        0 2022-01-10 13:45:17.135788 couchcopy-0.1.5/
-drwxr-xr-x   0 hoel      (1000) hoel      (1000)        0 2022-01-10 13:45:17.133788 couchcopy-0.1.5/.github/
-drwxr-xr-x   0 hoel      (1000) hoel      (1000)        0 2022-01-10 13:45:17.134788 couchcopy-0.1.5/.github/workflows/
--rw-rw-r--   0 hoel      (1000) hoel      (1000)      533 2021-09-06 15:22:45.000000 couchcopy-0.1.5/.github/workflows/ci.yaml
--rw-rw-r--   0 hoel      (1000) hoel      (1000)       41 2021-09-06 15:22:45.000000 couchcopy-0.1.5/.gitignore
--rw-rw-r--   0 hoel      (1000) hoel      (1000)    35147 2021-09-06 15:22:45.000000 couchcopy-0.1.5/LICENSE
--rw-r--r--   0 hoel      (1000) hoel      (1000)     6010 2022-01-10 13:45:17.135788 couchcopy-0.1.5/PKG-INFO
--rw-rw-r--   0 hoel      (1000) hoel      (1000)     5758 2021-09-06 15:22:45.000000 couchcopy-0.1.5/README.rst
--rwxr-xr-x   0 hoel      (1000) hoel      (1000)    23990 2022-01-10 13:43:37.000000 couchcopy-0.1.5/couchcopy
-drwxr-xr-x   0 hoel      (1000) hoel      (1000)        0 2022-01-10 13:45:17.135788 couchcopy-0.1.5/couchcopy.egg-info/
--rw-r--r--   0 hoel      (1000) hoel      (1000)     6010 2022-01-10 13:45:16.000000 couchcopy-0.1.5/couchcopy.egg-info/PKG-INFO
--rw-r--r--   0 hoel      (1000) hoel      (1000)      248 2022-01-10 13:45:16.000000 couchcopy-0.1.5/couchcopy.egg-info/SOURCES.txt
--rw-r--r--   0 hoel      (1000) hoel      (1000)        1 2022-01-10 13:45:16.000000 couchcopy-0.1.5/couchcopy.egg-info/dependency_links.txt
--rw-r--r--   0 hoel      (1000) hoel      (1000)       29 2022-01-10 13:45:16.000000 couchcopy-0.1.5/couchcopy.egg-info/requires.txt
--rw-r--r--   0 hoel      (1000) hoel      (1000)        1 2022-01-10 13:45:16.000000 couchcopy-0.1.5/couchcopy.egg-info/top_level.txt
--rw-rw-r--   0 hoel      (1000) hoel      (1000)       76 2022-01-10 13:45:17.136788 couchcopy-0.1.5/setup.cfg
--rw-rw-r--   0 hoel      (1000) hoel      (1000)      725 2021-09-06 15:22:45.000000 couchcopy-0.1.5/setup.py
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2023-06-22 10:36:35.922452 couchcopy-0.2.0/
+-rw-r--r--   0 adrien    (1000) adrien    (1000)    35147 2021-11-19 06:19:19.000000 couchcopy-0.2.0/LICENSE
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     5990 2023-06-22 10:36:35.922452 couchcopy-0.2.0/PKG-INFO
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     5758 2023-06-06 09:37:26.000000 couchcopy-0.2.0/README.rst
+-rwxr-xr-x   0 adrien    (1000) adrien    (1000)    24757 2023-06-22 10:33:20.000000 couchcopy-0.2.0/couchcopy
+drwxr-xr-x   0 adrien    (1000) adrien    (1000)        0 2023-06-22 10:36:35.922452 couchcopy-0.2.0/couchcopy.egg-info/
+-rw-r--r--   0 adrien    (1000) adrien    (1000)     5990 2023-06-22 10:36:35.000000 couchcopy-0.2.0/couchcopy.egg-info/PKG-INFO
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      211 2023-06-22 10:36:35.000000 couchcopy-0.2.0/couchcopy.egg-info/SOURCES.txt
+-rw-r--r--   0 adrien    (1000) adrien    (1000)        1 2023-06-22 10:36:35.000000 couchcopy-0.2.0/couchcopy.egg-info/dependency_links.txt
+-rw-r--r--   0 adrien    (1000) adrien    (1000)       29 2023-06-22 10:36:35.000000 couchcopy-0.2.0/couchcopy.egg-info/requires.txt
+-rw-r--r--   0 adrien    (1000) adrien    (1000)        1 2023-06-22 10:36:35.000000 couchcopy-0.2.0/couchcopy.egg-info/top_level.txt
+-rw-r--r--   0 adrien    (1000) adrien    (1000)       76 2023-06-22 10:36:35.922452 couchcopy-0.2.0/setup.cfg
+-rw-r--r--   0 adrien    (1000) adrien    (1000)      725 2021-11-19 06:19:19.000000 couchcopy-0.2.0/setup.py
```

### Comparing `couchcopy-0.1.5/LICENSE` & `couchcopy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `couchcopy-0.1.5/PKG-INFO` & `couchcopy-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: couchcopy
-Version: 0.1.5
+Version: 0.2.0
 Summary: Backup, load and restore CouchDB clusters
 Home-page: https://github.com/tolteck/couchcopy
 Author: Hoël Iris
 License: GPLv3
-Platform: UNKNOWN
 Requires-Python: >=3.8
 License-File: LICENSE
 
-couchcopy
+Couchcopy
 =========
 
 Create an archive of a running CouchDB node, saving CouchDB files
 ``data/.shards``, ``data/_dbs.couch`` and ``data/shards`` in this order.
 To allow backup of a running CouchDB, files are copied before archive creation.
 
 Restore an archive of a CouchDB node to a new CouchDB. The new CouchDB can be a
 cluster of multiple nodes.
-The new CouchDB configuration should already be done before using couchcopy,
+The new CouchDB configuration should already be done before using Couchcopy,
 however, all existing data will be deleted.
 During restoration, CouchDB will be stopped and restarted on each cluster
 nodes.
 
 Limitations
 -----------
 
 Tested with CouchDB 3.1.1 only.
 
-To restore an archive, couchcopy needs to stop and start CouchDB. It assumes
+To restore an archive, Couchcopy needs to stop and start CouchDB. It assumes
 that CouchDB is controlled by systemd. If you don't use systemd you can
 change parameters ``--couchdb-start`` and ``--couchdb-stop``.
 
 Your CouchDB ``n`` value should be higher or equal to the number of nodes in
 your CouchDB cluster.
 Otherwise saving shards from one node would not be enough to save and restore
 all databases.
@@ -40,22 +39,22 @@
 <https://docs.couchdb.org/en/3.1.1/cluster/theory.html#theory>`_ for more
 details on replicas and nodes.
 
 The number of shards per database, i.e. the value of ``q``, should be the same
 for the origin CouchDB and the destination CouchDB.
 Otherwise, ``tree /data/shards`` is not the same.
 
-couchcopy assumes you have read and write permissions on CouchDB data
+Couchcopy assumes you have read and write permissions on CouchDB data
 directories. If you don't have them, you can try to use the ``--use-sudo``
 option.
 
 Get started
 -----------
 
-Install couchcopy:
+Install Couchcopy:
 
 .. code:: shell
 
  pip install --user couchcopy
 
 Make a backup to ``backup.tar.gz``, from machine ``old-server`` with CouchDB
 data at ``/var/lib/couchdb``:
@@ -117,21 +116,21 @@
 ----------------------
 
 During restoration, if the new CouchDB nodes names are not the same as the
 old CouchDB, nodes names are updated using  CouchDB ``/_node/_local/_dbs``
 endpoint. See CouchDB ``/_node/_local/_dbs`` `endpoint documentation
 <https://docs.couchdb.org/en/3.1.1/cluster/sharding.html#updating-cluster-metadata-to-reflect-the-new-target-shard-s>`_.
 
-During restoration, couchcopy first updates one CouchDB node metadata (i.e. the
+During restoration, Couchcopy first updates one CouchDB node metadata (i.e. the
 list of nodes names) then it lets CouchDB itself synchronize metadata to the
 other nodes.
-couchcopy exits when the synchronization is finished for all nodes, using
+Couchcopy exits when the synchronization is finished for all nodes, using
 undocumented CouchDB ``/_dbs`` endpoint to monitor CouchDB nodes
 synchronization.
-You can skip that part if you want, i.e. you can exit couchcopy safely when the
+You can skip that part if you want, i.e. you can exit Couchcopy safely when the
 following log trace is displayed
 ``[Waiting for CouchDB cluster synchronization...]``.
 For a CouchDB of 10^5 databases, updating the first node metadata takes 35
 minutes then metadata synchronization to the other nodes takes 6 minutes.
 For a CouchDB of 100 databases only, both operations are nearly instantaneous.
 
 Developer notes
@@ -172,9 +171,7 @@
  python setup.py sdist
  twine upload dist/*
 
 License
 -------
 
 This program is licensed under the GNU General Public License version 3.
-
-
```

### Comparing `couchcopy-0.1.5/README.rst` & `couchcopy-0.2.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-couchcopy
+Couchcopy
 =========
 
 Create an archive of a running CouchDB node, saving CouchDB files
 ``data/.shards``, ``data/_dbs.couch`` and ``data/shards`` in this order.
 To allow backup of a running CouchDB, files are copied before archive creation.
 
 Restore an archive of a CouchDB node to a new CouchDB. The new CouchDB can be a
 cluster of multiple nodes.
-The new CouchDB configuration should already be done before using couchcopy,
+The new CouchDB configuration should already be done before using Couchcopy,
 however, all existing data will be deleted.
 During restoration, CouchDB will be stopped and restarted on each cluster
 nodes.
 
 Limitations
 -----------
 
 Tested with CouchDB 3.1.1 only.
 
-To restore an archive, couchcopy needs to stop and start CouchDB. It assumes
+To restore an archive, Couchcopy needs to stop and start CouchDB. It assumes
 that CouchDB is controlled by systemd. If you don't use systemd you can
 change parameters ``--couchdb-start`` and ``--couchdb-stop``.
 
 Your CouchDB ``n`` value should be higher or equal to the number of nodes in
 your CouchDB cluster.
 Otherwise saving shards from one node would not be enough to save and restore
 all databases.
@@ -29,22 +29,22 @@
 <https://docs.couchdb.org/en/3.1.1/cluster/theory.html#theory>`_ for more
 details on replicas and nodes.
 
 The number of shards per database, i.e. the value of ``q``, should be the same
 for the origin CouchDB and the destination CouchDB.
 Otherwise, ``tree /data/shards`` is not the same.
 
-couchcopy assumes you have read and write permissions on CouchDB data
+Couchcopy assumes you have read and write permissions on CouchDB data
 directories. If you don't have them, you can try to use the ``--use-sudo``
 option.
 
 Get started
 -----------
 
-Install couchcopy:
+Install Couchcopy:
 
 .. code:: shell
 
  pip install --user couchcopy
 
 Make a backup to ``backup.tar.gz``, from machine ``old-server`` with CouchDB
 data at ``/var/lib/couchdb``:
@@ -106,21 +106,21 @@
 ----------------------
 
 During restoration, if the new CouchDB nodes names are not the same as the
 old CouchDB, nodes names are updated using  CouchDB ``/_node/_local/_dbs``
 endpoint. See CouchDB ``/_node/_local/_dbs`` `endpoint documentation
 <https://docs.couchdb.org/en/3.1.1/cluster/sharding.html#updating-cluster-metadata-to-reflect-the-new-target-shard-s>`_.
 
-During restoration, couchcopy first updates one CouchDB node metadata (i.e. the
+During restoration, Couchcopy first updates one CouchDB node metadata (i.e. the
 list of nodes names) then it lets CouchDB itself synchronize metadata to the
 other nodes.
-couchcopy exits when the synchronization is finished for all nodes, using
+Couchcopy exits when the synchronization is finished for all nodes, using
 undocumented CouchDB ``/_dbs`` endpoint to monitor CouchDB nodes
 synchronization.
-You can skip that part if you want, i.e. you can exit couchcopy safely when the
+You can skip that part if you want, i.e. you can exit Couchcopy safely when the
 following log trace is displayed
 ``[Waiting for CouchDB cluster synchronization...]``.
 For a CouchDB of 10^5 databases, updating the first node metadata takes 35
 minutes then metadata synchronization to the other nodes takes 6 minutes.
 For a CouchDB of 100 databases only, both operations are nearly instantaneous.
 
 Developer notes
```

### Comparing `couchcopy-0.1.5/couchcopy` & `couchcopy-0.2.0/couchcopy`

 * *Files 5% similar despite different names*

```diff
@@ -14,32 +14,34 @@
 import sys
 from tempfile import TemporaryDirectory
 
 import aiocouch
 import yaml
 
 
-__version__ = '0.1.5'
+__version__ = '0.2.0'
 # Tweak this parameter to your needs: From 17 minutes with 16 workers to 28
 # minutes with 8 workers for 10^5 databases on my machine.
 N_WORKERS = 16
 
 
-async def subprocess(*args, shell=False):
+async def subprocess(*args, shell=False, input=None):
+    stdin = None if input is None else asyncio.subprocess.PIPE
+
     # For debugging purposes:
     # print('> ' + str(args))
     if shell:
         p = await asyncio.create_subprocess_shell(
-            *args, stdout=asyncio.subprocess.PIPE,
+            *args, stdin=stdin, stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.PIPE)
     else:
         p = await asyncio.create_subprocess_exec(
-            *args, stdout=asyncio.subprocess.PIPE,
+            *args, stdin=stdin, stdout=asyncio.subprocess.PIPE,
             stderr=asyncio.subprocess.PIPE)
-    stdout, stderr = await p.communicate()
+    stdout, stderr = await p.communicate(input=input)
     stdout, stderr = stdout.decode(), stderr.decode()
     if args[0] == 'rsync' and p.returncode == 24:
         # When a file is deleted between the start of rsync and the moment
         # the file is copied, rsync outputs a "warning: some files vanished"
         # log and it exits with return code 24.
         # See upstream explanation:
         # https://bugzilla.samba.org/show_bug.cgi?id=10356
@@ -53,49 +55,77 @@
         return stdout
     if p.returncode == 0:
         return stdout
     raise Exception(f'Command {args[0]} returned code {p.returncode}, stdout: '
                     f'{stdout}, stderr: {stderr}')
 
 
-async def backup(hostname, path, output, reuse_dir=None, tmp_dir=None,
-                 nodes_names=None):
-    tmp_dir = TemporaryDirectory(prefix='couchcopy-', dir=tmp_dir)
-    tmp_path = reuse_dir or tmp_dir.name
-    if not os.path.exists(tmp_path + '/data'):
-        os.mkdir(tmp_path + '/data')
-
-    with open(tmp_path + '/metadata.yaml', 'w') as f:
-        yaml.dump({
-            'backup': {
-                'date': datetime.now().isoformat(),
-                'source': {'nodes-names': nodes_names or []},
-            },
-            'couchcopy': {'version': __version__},
-        }, f, default_flow_style=False)
-
-    # rsync is used to copy from remote machine, but also to save files
-    # in a specific order, and to avoid using `tar` on files that are used in
-    # parallel by a running CouchDB.
-    print('[rsync...]')
-    hostname = hostname + ':' if hostname != 'localhost' else ''
-    await subprocess('rsync', '--del', '--ignore-missing-args',
-                     '-av', hostname + path + '/.shards', tmp_path + '/data')
-    await subprocess('rsync', '--del', '-av', hostname + path + '/_dbs.couch',
-                     tmp_path + '/data')
-    await subprocess('rsync', '--del', '--ignore-missing-args',
-                     '-av', hostname + path + '/shards', tmp_path + '/data')
-
-    print('[tar...]')
-    await subprocess('tar', '-I', 'pigz', '-cf', output, '-C', tmp_path,
-                     'metadata.yaml', 'data')
-    # For debugging purposes:
-    # if tmp_dir:
-    #     shutil.rmtree('/tmp/couchcopy', True)
-    #     shutil.copytree(tmp_dir.name, '/tmp/couchcopy')
+async def backup(hostname, path, output, nodes_names=None):
+    metadata = yaml.dump({
+        'backup': {
+            'date': datetime.now().isoformat(),
+            'source': {'nodes-names': nodes_names or []},
+        },
+        'couchcopy': {'version': __version__},
+    }, default_flow_style=False).encode()
+
+    print('[tar+ssh+gzip...]')
+
+    ssh_if_needed = ('ssh', hostname, '--') if hostname != 'localhost' else ()
+    tempdir = await subprocess(*ssh_if_needed,
+                               'mktemp', '-d', '--tmpdir', 'couchcopy-XXXXX')
+
+    try:
+        tempdir = tempdir.strip()
+        await subprocess(*ssh_if_needed,
+                         'dd', f'of={tempdir}/metadata.yaml', 'status=none',
+                         input=metadata)
+
+        with open(output, 'wb') as archive:
+            pipe_out, pipe_in = os.pipe()
+            p1 = await asyncio.create_subprocess_exec(
+                *ssh_if_needed,
+                'tar',
+                '-C', tempdir, '-c', 'metadata.yaml',
+                '-C', os.path.dirname(path),
+                '-c', os.path.basename(path) + '/.shards',
+                os.path.basename(path) + '/_dbs.couch',
+                os.path.basename(path) + '/shards',
+                '--transform', f's/^{re.escape(os.path.basename(path))}/data/',
+                stdout=pipe_in, stderr=asyncio.subprocess.PIPE,
+                env={'LANG': 'C'})
+            p2 = await asyncio.create_subprocess_exec(
+                'pigz', stdin=pipe_out, stdout=archive,
+                stderr=asyncio.subprocess.PIPE)
+            os.close(pipe_in)
+            os.close(pipe_out)
+            _, stderr1, returncode1 = *await p1.communicate(), p1.returncode
+            _, stderr2, returncode2 = *await p2.communicate(), p2.returncode
+
+            # tar can exit with return code 1 if files are modified on disk
+            # during the archive creation. This is normal behavior when the
+            # CouchDB instance is running, so let's filter out these errors and
+            # fail only on other ones.
+            if returncode1 == 1:
+                stderr1 = '\n'.join(
+                    l for l in stderr1.decode().splitlines()
+                    if not l.endswith('file changed as we read it')).encode()
+                if not stderr1:
+                    returncode1 = 0
+
+            if returncode1 != 0:
+                raise Exception(f'Command tar returned code {returncode1}, '
+                                f'stderr: {stderr1.decode()}')
+            if returncode2 != 0:
+                raise Exception(f'Command pigz returned code {returncode2}, '
+                                f'stderr: {stderr2.decode()}')
+
+    finally:
+        await subprocess(*ssh_if_needed,
+                         'rm', '-rf', tempdir)
 
 
 async def couch_conn(url, user, password):
     conn = aiocouch.CouchDB(url, user=user, password=password)
     for i in range(6):
         try:
             await conn.info()
@@ -296,15 +326,15 @@
     return node_name, tmp_dir
 
 
 async def unbrand(old_archive, new_archive, tmp_dir=None):
     node_name, origin_tmp_dir = await load(
         old_archive, tmp_dir=tmp_dir, blocking=False)
     await backup('localhost', origin_tmp_dir.name + '/data', new_archive,
-                 tmp_dir=tmp_dir, nodes_names=[node_name])
+                 nodes_names=[node_name])
 
 
 async def restore(archive, cred, hostnames, paths, ports, names, couchdb_start,
                   couchdb_stop, force, use_sudo):
     user, password = cred.split(':')
     remote = hostnames[0] != 'localhost'
     urls = [f'http://{hostname if remote else "localhost"}:{port}'
@@ -454,19 +484,14 @@
     subparsers = parser.add_subparsers(dest='action')
     sub = {}
     sub['backup'] = subparsers.add_parser('backup', description=(
         'Backup a CouchDB cluster from one of its node.'))
     sub['backup'].add_argument('couchdb',
                                metavar='hostname,/couchdb/data/dir')
     sub['backup'].add_argument('archive', metavar='backup.tar.gz')
-    sub['backup'].add_argument('--rsync-reuse-dir', help=(
-        'directory on the local machine to store data reused between '
-        'executions, if not set rsync starts from scratch'))
-    sub['backup'].add_argument('--tmp-dir', help=(
-        'directory on the local machine to store temporary data'))
     sub['unbrand'] = subparsers.add_parser('unbrand', description=(
         'Unbrand shards inside a backup.tar.gz file from their origin CouchDB '
         'node name to a unique and reusable node name. Use this option to '
         'improve the local load speed of the archive.'))
     sub['unbrand'].add_argument('old_archive', metavar='backup.tar.gz')
     sub['unbrand'].add_argument('new_archive', metavar='new_backup.tar.gz')
     sub['unbrand'].add_argument('--tmp-dir', help=(
@@ -507,19 +532,16 @@
     elif args.action == 'backup':
         splitted = args.couchdb.split(',')
         if len(splitted) != 2:
             sub['backup'].error('wrong "hostname,/couchdb/data/dir"')
         hostname, path = splitted
         if hostname and any(c in hostname for c in (':', '@')):
             sub['backup'].error('wrong "hostname,/couchdb/data/dir"')
-        assert not args.rsync_reuse_dir or not args.tmp_dir, \
-            'cannot use --tmp-dir and --rsync-reuse-dir in the same time'
 
-        await backup(hostname, path, args.archive, args.rsync_reuse_dir,
-                     args.tmp_dir)
+        await backup(hostname, path, args.archive)
     elif args.action == 'unbrand':
         await unbrand(args.old_archive, args.new_archive, args.tmp_dir)
     elif args.action == 'load':
         await load(args.archive, args.admin, args.tmp_dir)
     elif args.action == 'restore':
         creds = []
         hostnames = []
```

### Comparing `couchcopy-0.1.5/couchcopy.egg-info/PKG-INFO` & `couchcopy-0.2.0/couchcopy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: couchcopy
-Version: 0.1.5
+Version: 0.2.0
 Summary: Backup, load and restore CouchDB clusters
 Home-page: https://github.com/tolteck/couchcopy
 Author: Hoël Iris
 License: GPLv3
-Platform: UNKNOWN
 Requires-Python: >=3.8
 License-File: LICENSE
 
-couchcopy
+Couchcopy
 =========
 
 Create an archive of a running CouchDB node, saving CouchDB files
 ``data/.shards``, ``data/_dbs.couch`` and ``data/shards`` in this order.
 To allow backup of a running CouchDB, files are copied before archive creation.
 
 Restore an archive of a CouchDB node to a new CouchDB. The new CouchDB can be a
 cluster of multiple nodes.
-The new CouchDB configuration should already be done before using couchcopy,
+The new CouchDB configuration should already be done before using Couchcopy,
 however, all existing data will be deleted.
 During restoration, CouchDB will be stopped and restarted on each cluster
 nodes.
 
 Limitations
 -----------
 
 Tested with CouchDB 3.1.1 only.
 
-To restore an archive, couchcopy needs to stop and start CouchDB. It assumes
+To restore an archive, Couchcopy needs to stop and start CouchDB. It assumes
 that CouchDB is controlled by systemd. If you don't use systemd you can
 change parameters ``--couchdb-start`` and ``--couchdb-stop``.
 
 Your CouchDB ``n`` value should be higher or equal to the number of nodes in
 your CouchDB cluster.
 Otherwise saving shards from one node would not be enough to save and restore
 all databases.
@@ -40,22 +39,22 @@
 <https://docs.couchdb.org/en/3.1.1/cluster/theory.html#theory>`_ for more
 details on replicas and nodes.
 
 The number of shards per database, i.e. the value of ``q``, should be the same
 for the origin CouchDB and the destination CouchDB.
 Otherwise, ``tree /data/shards`` is not the same.
 
-couchcopy assumes you have read and write permissions on CouchDB data
+Couchcopy assumes you have read and write permissions on CouchDB data
 directories. If you don't have them, you can try to use the ``--use-sudo``
 option.
 
 Get started
 -----------
 
-Install couchcopy:
+Install Couchcopy:
 
 .. code:: shell
 
  pip install --user couchcopy
 
 Make a backup to ``backup.tar.gz``, from machine ``old-server`` with CouchDB
 data at ``/var/lib/couchdb``:
@@ -117,21 +116,21 @@
 ----------------------
 
 During restoration, if the new CouchDB nodes names are not the same as the
 old CouchDB, nodes names are updated using  CouchDB ``/_node/_local/_dbs``
 endpoint. See CouchDB ``/_node/_local/_dbs`` `endpoint documentation
 <https://docs.couchdb.org/en/3.1.1/cluster/sharding.html#updating-cluster-metadata-to-reflect-the-new-target-shard-s>`_.
 
-During restoration, couchcopy first updates one CouchDB node metadata (i.e. the
+During restoration, Couchcopy first updates one CouchDB node metadata (i.e. the
 list of nodes names) then it lets CouchDB itself synchronize metadata to the
 other nodes.
-couchcopy exits when the synchronization is finished for all nodes, using
+Couchcopy exits when the synchronization is finished for all nodes, using
 undocumented CouchDB ``/_dbs`` endpoint to monitor CouchDB nodes
 synchronization.
-You can skip that part if you want, i.e. you can exit couchcopy safely when the
+You can skip that part if you want, i.e. you can exit Couchcopy safely when the
 following log trace is displayed
 ``[Waiting for CouchDB cluster synchronization...]``.
 For a CouchDB of 10^5 databases, updating the first node metadata takes 35
 minutes then metadata synchronization to the other nodes takes 6 minutes.
 For a CouchDB of 100 databases only, both operations are nearly instantaneous.
 
 Developer notes
@@ -172,9 +171,7 @@
  python setup.py sdist
  twine upload dist/*
 
 License
 -------
 
 This program is licensed under the GNU General Public License version 3.
-
-
```

### Comparing `couchcopy-0.1.5/setup.py` & `couchcopy-0.2.0/setup.py`

 * *Files identical despite different names*

