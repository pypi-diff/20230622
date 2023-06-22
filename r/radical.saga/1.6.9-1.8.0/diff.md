# Comparing `tmp/radical.saga-1.6.9.tar.gz` & `tmp/radical.saga-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/radical.saga-1.6.9.tar", last modified: Thu Jul 15 20:10:46 2021, max compression
+gzip compressed data, was "dist/radical.saga-1.8.0.tar", last modified: Thu Sep 23 11:55:47 2021, max compression
```

## Comparing `radical.saga-1.6.9.tar` & `radical.saga-1.8.0.tar`

### file list

```diff
@@ -1,284 +1,283 @@
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.349438 radical.saga-1.6.9/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    41184 2021-07-15 20:10:19.000000 radical.saga-1.6.9/CHANGES.md
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1284 2021-04-14 10:16:16.000000 radical.saga-1.6.9/LICENSE.md
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      138 2021-04-14 10:16:16.000000 radical.saga-1.6.9/MANIFEST.in
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1092 2021-07-15 20:10:46.349438 radical.saga-1.6.9/PKG-INFO
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1260 2021-06-14 10:07:23.000000 radical.saga-1.6.9/README.md
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        6 2021-07-15 20:09:53.000000 radical.saga-1.6.9/VERSION
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.329438 radical.saga-1.6.9/bin/
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)       79 2021-04-14 10:16:16.000000 radical.saga-1.6.9/bin/radical-saga-version
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.325438 radical.saga-1.6.9/examples/
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.329438 radical.saga-1.6.9/examples/context/
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)      919 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/context/context_ssh.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.329438 radical.saga-1.6.9/examples/files/
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2102 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/files/go_file_copy.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1941 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/files/go_remotedir_list.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1119 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/files/http_file_copy.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1702 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/files/sftp_file_copy.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1607 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/files/sftp_remotedir_list.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1478 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/files/srm_get_size.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.329438 radical.saga-1.6.9/examples/jobs/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     5194 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/jobs/cobalt.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3278 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/jobs/condorjob.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2843 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/jobs/loadlevelerjob.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3068 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/jobs/localjob.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3431 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/jobs/localjobcontainer.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3711 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/jobs/lsfjob.py
--rwxr-xr-x   0 merzky    (1001) merzky    (1001)      943 2020-01-08 22:16:58.000000 radical.saga-1.6.9/examples/jobs/noopjob.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3846 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/jobs/pbsgsisshjob.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3872 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/jobs/pbsjob.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3630 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/jobs/pbsprojob.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3433 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/jobs/sgejob.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     5234 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/jobs/slurmjob.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3624 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/jobs/slurmjobcontainer.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3539 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/jobs/torque_gsissh_job.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.329438 radical.saga-1.6.9/examples/master_worker/
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     4885 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/master_worker/master.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1438 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/master_worker/worker.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.329438 radical.saga-1.6.9/examples/misc/
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)      505 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/misc/inherit_context.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.325438 radical.saga-1.6.9/examples/replica/
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.329438 radical.saga-1.6.9/examples/replica/irods/
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     5006 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/replica/irods/irods_test.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.329438 radical.saga-1.6.9/examples/resource/
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     5158 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/resource/amazon_ec2.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)    11695 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/resource/ec2.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.333438 radical.saga-1.6.9/examples/tutorial/
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.333438 radical.saga-1.6.9/examples/tutorial/mandelbrot/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2880 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/tutorial/mandelbrot/mandelbrot.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     5448 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/tutorial/mandelbrot/saga_mandelbrot.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     3960 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/tutorial/mandelbrot/saga_mandelbrot_osg.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1996 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/tutorial/saga_example_local.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2385 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/tutorial/saga_example_remote.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2532 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/tutorial/saga_example_remote_cluster_staging.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2671 2021-04-14 10:16:16.000000 radical.saga-1.6.9/examples/tutorial/saga_example_remote_staging.py
--rw-r--r--   0 merzky    (1001) merzky    (1001)       87 2021-07-15 20:10:46.349438 radical.saga-1.6.9/setup.cfg
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     9101 2021-06-14 10:07:23.000000 radical.saga-1.6.9/setup.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.325438 radical.saga-1.6.9/src/
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.325438 radical.saga-1.6.9/src/radical/
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.333438 radical.saga-1.6.9/src/radical/saga/
--rw-r--r--   0 merzky    (1001) merzky    (1001)       40 2021-07-15 20:10:46.000000 radical.saga-1.6.9/src/radical/saga/SDIST
--rw-r--r--   0 merzky    (1001) merzky    (1001)       20 2021-07-15 20:10:46.000000 radical.saga-1.6.9/src/radical/saga/VERSION
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1217 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/__init__.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.333438 radical.saga-1.6.9/src/radical/saga/adaptors/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      110 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/__init__.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.333438 radical.saga-1.6.9/src/radical/saga/adaptors/aws/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/aws/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    41488 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/aws/ec2_resource.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2774 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/base.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.333438 radical.saga-1.6.9/src/radical/saga/adaptors/cobalt/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      108 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cobalt/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    51241 2021-07-08 07:53:29.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cobalt/cobaltjob.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.337438 radical.saga-1.6.9/src/radical/saga/adaptors/condor/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      106 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/condor/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    65110 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/condor/condorjob.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     3713 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/condor/transferdirectives.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.337438 radical.saga-1.6.9/src/radical/saga/adaptors/context/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/context/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     4880 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/context/myproxy.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     9994 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/context/ssh.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2717 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/context/userpass.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     4351 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/context/x509.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.337438 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      139 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/__init__.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.337438 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/advert/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      172 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/advert/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1968 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/advert/directory.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1803 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/advert/entry.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      644 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/attributes.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2687 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/base.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      467 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/context.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     4831 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/decorators.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.337438 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/filesystem/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      258 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/filesystem/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1725 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/filesystem/directory.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     3102 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/filesystem/file.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.337438 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/job/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      247 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/job/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     4854 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/job/job.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2567 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/job/service.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.337438 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/namespace/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      259 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/namespace/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     3531 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/namespace/directory.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2989 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/namespace/entry.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.337438 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/replica/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      270 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/replica/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2102 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/replica/logical_directory.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2464 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/replica/logical_file.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.337438 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/resource/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      351 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/resource/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2210 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/resource/manager.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2588 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/resource/resource.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      420 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/cpi/sasync.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.337438 radical.saga-1.6.9/src/radical/saga/adaptors/globus_online/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/globus_online/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    42822 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/globus_online/go_file.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.337438 radical.saga-1.6.9/src/radical/saga/adaptors/http/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      104 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/http/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     7867 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/http/http_file.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.337438 radical.saga-1.6.9/src/radical/saga/adaptors/irods/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      114 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/irods/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    32419 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/irods/irods_replica.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.337438 radical.saga-1.6.9/src/radical/saga/adaptors/loadl/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      104 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/loadl/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    41758 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/loadl/loadljob.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.341438 radical.saga-1.6.9/src/radical/saga/adaptors/lsf/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      106 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/lsf/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    38592 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/lsf/lsfjob.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.341438 radical.saga-1.6.9/src/radical/saga/adaptors/mock/
--rw-r--r--   0 merzky    (1001) merzky    (1001)        0 2020-12-21 14:02:41.000000 radical.saga-1.6.9/src/radical/saga/adaptors/mock/__init__.py
--rw-r--r--   0 merzky    (1001) merzky    (1001)    43999 2020-12-21 14:05:37.000000 radical.saga-1.6.9/src/radical/saga/adaptors/mock/shell_file.py
--rw-r--r--   0 merzky    (1001) merzky    (1001)    59601 2020-12-21 14:04:14.000000 radical.saga-1.6.9/src/radical/saga/adaptors/mock/shell_job.py
--rw-r--r--   0 merzky    (1001) merzky    (1001)    12187 2020-12-21 14:04:03.000000 radical.saga-1.6.9/src/radical/saga/adaptors/mock/shell_resource.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.341438 radical.saga-1.6.9/src/radical/saga/adaptors/noop/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/noop/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    18449 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/noop/noop_job.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.341438 radical.saga-1.6.9/src/radical/saga/adaptors/pbs/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      106 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/pbs/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    46718 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/pbs/pbsjob.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.341438 radical.saga-1.6.9/src/radical/saga/adaptors/pbspro/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      106 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/pbspro/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    46969 2021-07-15 20:09:46.000000 radical.saga-1.6.9/src/radical/saga/adaptors/pbspro/pbsprojob.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.341438 radical.saga-1.6.9/src/radical/saga/adaptors/redis/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/redis/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1584 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/redis/redis_1.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      904 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/redis/redis_2.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    15418 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/redis/redis_advert.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2896 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/redis/redis_cache.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    20614 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/redis/redis_namespace.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.341438 radical.saga-1.6.9/src/radical/saga/adaptors/sge/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      106 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/sge/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    50011 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/sge/sgejob.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.341438 radical.saga-1.6.9/src/radical/saga/adaptors/shell/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/shell/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    47096 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/shell/shell_file.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    59786 2021-07-08 07:54:58.000000 radical.saga-1.6.9/src/radical/saga/adaptors/shell/shell_job.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    12225 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/shell/shell_resource.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      307 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/shell/shell_wrapper.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    28614 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/shell/shell_wrapper.sh
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.341438 radical.saga-1.6.9/src/radical/saga/adaptors/slurm/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/slurm/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    52287 2021-07-09 07:54:27.000000 radical.saga-1.6.9/src/radical/saga/adaptors/slurm/slurm_job.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.341438 radical.saga-1.6.9/src/radical/saga/adaptors/srm/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/srm/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    21845 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/srm/srmfile.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.341438 radical.saga-1.6.9/src/radical/saga/adaptors/torque/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      109 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/torque/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    50168 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/adaptors/torque/torquejob.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.341438 radical.saga-1.6.9/src/radical/saga/advert/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      203 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/advert/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      935 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/advert/constants.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     7433 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/advert/directory.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     7308 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/advert/entry.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)   100992 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/attributes.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     4844 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/base.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.345438 radical.saga-1.6.9/src/radical/saga/configs/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      238 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/adaptors_cobaltjob.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      115 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/adaptors_condorjob.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1055 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/adaptors_globus_online_file.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      360 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/adaptors_loadljob.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      247 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/adaptors_myproxy.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      577 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/adaptors_sgejob.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      919 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/adaptors_shell_job.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1263 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/registry_default.json
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.345438 radical.saga-1.6.9/src/radical/saga/configs/resources/
--rw-r--r--   0 merzky    (1001) merzky    (1001)       21 2020-02-03 15:02:11.000000 radical.saga-1.6.9/src/radical/saga/configs/resources/stampede.json
--rw-r--r--   0 merzky    (1001) merzky    (1001)      175 2020-02-03 15:02:35.000000 radical.saga-1.6.9/src/radical/saga/configs/resources.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1311 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/session.json
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.345438 radical.saga-1.6.9/src/radical/saga/configs/tests/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       46 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_advert_redis_local.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       74 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_advert_redis_repex1.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      296 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_condor_osg_engage.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      326 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_condor_ssh_osg.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      228 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_default.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       51 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_file_localhost.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      132 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_fork_localhost.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      169 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_gsisftp_kraken.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      138 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_gsissh_kraken.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      217 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_irods_replica.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      201 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_lsf_localhost_yellowstone.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      286 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_pbs_gsissh_kraken.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      233 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_pbs_gsissh_trestles.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      223 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_pbs_ssh_alamo.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      214 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_pbs_ssh_archer.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      223 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_pbs_ssh_hotel.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      223 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_pbs_ssh_india.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      224 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_pbs_ssh_sierra.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      230 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_pbs_ssh_trestles.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      157 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_sftp_india.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      161 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_sftp_stampede.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      323 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_sge_gsissh_lonestar.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      398 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_sge_ssh_lonestar.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      273 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_slurm_ssh_comet.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      358 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_slurm_ssh_stampede.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      345 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_ssh_boskop.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      132 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_ssh_gw86.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      118 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_ssh_india.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      172 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_ssh_localhost.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      169 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_ssh_silver.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      311 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/tests/test_torque_gsissh_supermic.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1314 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/configs/utils_default.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1377 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/constants.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     5895 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/context.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.349438 radical.saga-1.6.9/src/radical/saga/engine/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      306 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/engine/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    22540 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/engine/engine.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    16389 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/exceptions.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.349438 radical.saga-1.6.9/src/radical/saga/filesystem/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      202 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/filesystem/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      872 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/filesystem/constants.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     7788 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/filesystem/directory.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    11356 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/filesystem/file.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.349438 radical.saga-1.6.9/src/radical/saga/job/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      320 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/job/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     7244 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/job/constants.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1745 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/job/container.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     5730 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/job/description.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    27060 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/job/job.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    14806 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/job/service.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.349438 radical.saga-1.6.9/src/radical/saga/messages/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     3240 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/messages/message.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2452 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/monitorable.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.349438 radical.saga-1.6.9/src/radical/saga/namespace/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      206 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/namespace/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      492 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/namespace/constants.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    17201 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/namespace/directory.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    11856 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/namespace/entry.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)   353638 2021-06-30 19:41:03.000000 radical.saga-1.6.9/src/radical/saga/radical.saga-1.6.6-scalems-stable-3-ge70b9f8b-devel.tar.gz
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.349438 radical.saga-1.6.9/src/radical/saga/replica/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      237 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/replica/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      756 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/replica/constants.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     6918 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/replica/logical_directory.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     8558 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/replica/logical_file.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.349438 radical.saga-1.6.9/src/radical/saga/resource/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      222 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/resource/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2952 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/resource/constants.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     9163 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/resource/description.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     9522 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/resource/manager.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    19649 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/resource/resource.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      390 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/sasync.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    10720 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/session.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    22267 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/task.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2113 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/url.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.349438 radical.saga-1.6.9/src/radical/saga/utils/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      247 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/utils/__init__.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.349438 radical.saga-1.6.9/src/radical/saga/utils/job/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      166 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/utils/job/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     4594 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/utils/job/transfer_directives.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     9454 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/utils/misc.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2154 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/utils/pty_exceptions.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    31387 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/utils/pty_process.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    42924 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/utils/pty_shell.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    30526 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/utils/pty_shell_factory.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2551 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/utils/test_config.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      413 2021-04-14 10:16:16.000000 radical.saga-1.6.9/src/radical/saga/version.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-07-15 20:10:46.333438 radical.saga-1.6.9/src/radical.saga.egg-info/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1092 2021-07-15 20:10:46.000000 radical.saga-1.6.9/src/radical.saga.egg-info/PKG-INFO
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     9423 2021-07-15 20:10:46.000000 radical.saga-1.6.9/src/radical.saga.egg-info/SOURCES.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2021-07-15 20:10:46.000000 radical.saga-1.6.9/src/radical.saga.egg-info/dependency_links.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        8 2021-07-15 20:10:46.000000 radical.saga-1.6.9/src/radical.saga.egg-info/namespace_packages.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2021-07-15 20:10:46.000000 radical.saga-1.6.9/src/radical.saga.egg-info/not-zip-safe
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       36 2021-07-15 20:10:46.000000 radical.saga-1.6.9/src/radical.saga.egg-info/requires.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        8 2021-07-15 20:10:46.000000 radical.saga-1.6.9/src/radical.saga.egg-info/top_level.txt
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.753540 radical.saga-1.8.0/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    41432 2021-09-23 11:53:53.000000 radical.saga-1.8.0/CHANGES.md
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1284 2021-04-14 10:16:16.000000 radical.saga-1.8.0/LICENSE.md
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      138 2021-04-14 10:16:16.000000 radical.saga-1.8.0/MANIFEST.in
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1092 2021-09-23 11:55:47.753540 radical.saga-1.8.0/PKG-INFO
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1260 2021-06-14 10:07:23.000000 radical.saga-1.8.0/README.md
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        6 2021-09-23 11:53:02.000000 radical.saga-1.8.0/VERSION
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.717540 radical.saga-1.8.0/bin/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)       79 2021-04-14 10:16:16.000000 radical.saga-1.8.0/bin/radical-saga-version
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.713540 radical.saga-1.8.0/examples/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.717540 radical.saga-1.8.0/examples/context/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)      919 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/context/context_ssh.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.717540 radical.saga-1.8.0/examples/files/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2102 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/files/go_file_copy.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1941 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/files/go_remotedir_list.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1119 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/files/http_file_copy.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1702 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/files/sftp_file_copy.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1607 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/files/sftp_remotedir_list.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1478 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/files/srm_get_size.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.721540 radical.saga-1.8.0/examples/jobs/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     5194 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/cobalt.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3278 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/condorjob.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2843 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/loadlevelerjob.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3068 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/localjob.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3431 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/localjobcontainer.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3711 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/lsfjob.py
+-rwxr-xr-x   0 merzky    (1001) merzky    (1001)      943 2020-01-08 22:16:58.000000 radical.saga-1.8.0/examples/jobs/noopjob.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3846 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/pbsgsisshjob.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3872 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/pbsjob.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3630 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/pbsprojob.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3433 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/sgejob.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     5234 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/slurmjob.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3624 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/slurmjobcontainer.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3539 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/jobs/torque_gsissh_job.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.721540 radical.saga-1.8.0/examples/master_worker/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     4885 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/master_worker/master.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1438 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/master_worker/worker.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.721540 radical.saga-1.8.0/examples/misc/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)      505 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/misc/inherit_context.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.713540 radical.saga-1.8.0/examples/replica/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.721540 radical.saga-1.8.0/examples/replica/irods/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     5006 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/replica/irods/irods_test.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.721540 radical.saga-1.8.0/examples/resource/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     5158 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/resource/amazon_ec2.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)    11695 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/resource/ec2.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.721540 radical.saga-1.8.0/examples/tutorial/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.721540 radical.saga-1.8.0/examples/tutorial/mandelbrot/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2880 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/tutorial/mandelbrot/mandelbrot.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     5448 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/tutorial/mandelbrot/saga_mandelbrot.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3960 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/tutorial/mandelbrot/saga_mandelbrot_osg.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1996 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/tutorial/saga_example_local.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2385 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/tutorial/saga_example_remote.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2532 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/tutorial/saga_example_remote_cluster_staging.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2671 2021-04-14 10:16:16.000000 radical.saga-1.8.0/examples/tutorial/saga_example_remote_staging.py
+-rw-r--r--   0 merzky    (1001) merzky    (1001)       87 2021-09-23 11:55:47.753540 radical.saga-1.8.0/setup.cfg
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     9101 2021-09-23 09:22:40.000000 radical.saga-1.8.0/setup.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.713540 radical.saga-1.8.0/src/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.713540 radical.saga-1.8.0/src/radical/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.725540 radical.saga-1.8.0/src/radical/saga/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       40 2021-09-23 11:55:47.000000 radical.saga-1.8.0/src/radical/saga/SDIST
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       20 2021-09-23 11:55:47.000000 radical.saga-1.8.0/src/radical/saga/VERSION
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1217 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/__init__.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.725540 radical.saga-1.8.0/src/radical/saga/adaptors/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      110 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/__init__.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.725540 radical.saga-1.8.0/src/radical/saga/adaptors/aws/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/aws/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    41488 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/aws/ec2_resource.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2774 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/base.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.725540 radical.saga-1.8.0/src/radical/saga/adaptors/cobalt/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      108 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cobalt/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    51241 2021-07-08 07:53:29.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cobalt/cobaltjob.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.725540 radical.saga-1.8.0/src/radical/saga/adaptors/condor/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      106 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/condor/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    65110 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/condor/condorjob.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3713 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/condor/transferdirectives.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.729540 radical.saga-1.8.0/src/radical/saga/adaptors/context/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/context/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     4880 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/context/myproxy.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     9994 2021-09-23 09:22:40.000000 radical.saga-1.8.0/src/radical/saga/adaptors/context/ssh.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2717 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/context/userpass.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     4351 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/context/x509.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.729540 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      139 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/__init__.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.729540 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/advert/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      172 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/advert/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1968 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/advert/directory.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1803 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/advert/entry.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      644 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/attributes.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2687 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/base.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      467 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/context.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     4831 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/decorators.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.729540 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/filesystem/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      258 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/filesystem/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1725 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/filesystem/directory.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3102 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/filesystem/file.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.729540 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/job/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      247 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/job/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     4854 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/job/job.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2567 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/job/service.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.729540 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/namespace/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      259 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/namespace/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3531 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/namespace/directory.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2989 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/namespace/entry.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.729540 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/replica/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      270 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/replica/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2102 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/replica/logical_directory.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2464 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/replica/logical_file.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.733540 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/resource/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      351 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/resource/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2210 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/resource/manager.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2588 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/resource/resource.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      420 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/cpi/sasync.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.733540 radical.saga-1.8.0/src/radical/saga/adaptors/globus_online/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/globus_online/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    42822 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/globus_online/go_file.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.733540 radical.saga-1.8.0/src/radical/saga/adaptors/http/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      104 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/http/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     7867 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/http/http_file.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.733540 radical.saga-1.8.0/src/radical/saga/adaptors/irods/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      114 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/irods/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    32419 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/irods/irods_replica.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.733540 radical.saga-1.8.0/src/radical/saga/adaptors/loadl/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      104 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/loadl/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    41758 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/loadl/loadljob.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.733540 radical.saga-1.8.0/src/radical/saga/adaptors/lsf/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      106 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/lsf/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    38592 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/lsf/lsfjob.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.733540 radical.saga-1.8.0/src/radical/saga/adaptors/mock/
+-rw-r--r--   0 merzky    (1001) merzky    (1001)        0 2020-12-21 14:02:41.000000 radical.saga-1.8.0/src/radical/saga/adaptors/mock/__init__.py
+-rw-r--r--   0 merzky    (1001) merzky    (1001)    43999 2020-12-21 14:05:37.000000 radical.saga-1.8.0/src/radical/saga/adaptors/mock/shell_file.py
+-rw-r--r--   0 merzky    (1001) merzky    (1001)    59601 2020-12-21 14:04:14.000000 radical.saga-1.8.0/src/radical/saga/adaptors/mock/shell_job.py
+-rw-r--r--   0 merzky    (1001) merzky    (1001)    12187 2020-12-21 14:04:03.000000 radical.saga-1.8.0/src/radical/saga/adaptors/mock/shell_resource.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.733540 radical.saga-1.8.0/src/radical/saga/adaptors/noop/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/noop/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    18449 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/noop/noop_job.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.737540 radical.saga-1.8.0/src/radical/saga/adaptors/pbs/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      106 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/pbs/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    46718 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/pbs/pbsjob.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.737540 radical.saga-1.8.0/src/radical/saga/adaptors/pbspro/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      106 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/pbspro/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    46968 2021-09-23 09:22:40.000000 radical.saga-1.8.0/src/radical/saga/adaptors/pbspro/pbsprojob.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.737540 radical.saga-1.8.0/src/radical/saga/adaptors/redis/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/redis/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1584 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_1.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      904 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_2.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    15418 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_advert.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2896 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_cache.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    20614 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_namespace.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.737540 radical.saga-1.8.0/src/radical/saga/adaptors/sge/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      106 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/sge/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    50011 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/sge/sgejob.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.737540 radical.saga-1.8.0/src/radical/saga/adaptors/shell/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/shell/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    47096 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/shell/shell_file.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    59786 2021-08-25 14:26:29.000000 radical.saga-1.8.0/src/radical/saga/adaptors/shell/shell_job.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    12225 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/shell/shell_resource.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      307 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/shell/shell_wrapper.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    28614 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/shell/shell_wrapper.sh
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.737540 radical.saga-1.8.0/src/radical/saga/adaptors/slurm/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/slurm/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    52416 2021-09-23 11:52:49.000000 radical.saga-1.8.0/src/radical/saga/adaptors/slurm/slurm_job.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.741540 radical.saga-1.8.0/src/radical/saga/adaptors/srm/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/srm/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    21845 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/srm/srmfile.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.741540 radical.saga-1.8.0/src/radical/saga/adaptors/torque/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      109 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/torque/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    50168 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/adaptors/torque/torquejob.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.741540 radical.saga-1.8.0/src/radical/saga/advert/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      203 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/advert/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      935 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/advert/constants.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     7433 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/advert/directory.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     7308 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/advert/entry.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)   100992 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/attributes.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     4844 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/base.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.741540 radical.saga-1.8.0/src/radical/saga/configs/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      238 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/adaptors_cobaltjob.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      115 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/adaptors_condorjob.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1055 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/adaptors_globus_online_file.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      360 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/adaptors_loadljob.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      247 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/adaptors_myproxy.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      577 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/adaptors_sgejob.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      919 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/adaptors_shell_job.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1263 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/registry_default.json
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.741540 radical.saga-1.8.0/src/radical/saga/configs/resources/
+-rw-r--r--   0 merzky    (1001) merzky    (1001)       21 2020-02-03 15:02:11.000000 radical.saga-1.8.0/src/radical/saga/configs/resources/stampede.json
+-rw-r--r--   0 merzky    (1001) merzky    (1001)      175 2020-02-03 15:02:35.000000 radical.saga-1.8.0/src/radical/saga/configs/resources.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1311 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/session.json
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.749540 radical.saga-1.8.0/src/radical/saga/configs/tests/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       46 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_advert_redis_local.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       74 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_advert_redis_repex1.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      296 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_condor_osg_engage.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      326 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_condor_ssh_osg.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      228 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_default.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       51 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_file_localhost.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      132 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_fork_localhost.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      169 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_gsisftp_kraken.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      138 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_gsissh_kraken.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      217 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_irods_replica.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      201 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_lsf_localhost_yellowstone.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      286 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_pbs_gsissh_kraken.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      233 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_pbs_gsissh_trestles.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      223 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_pbs_ssh_alamo.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      214 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_pbs_ssh_archer.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      223 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_pbs_ssh_hotel.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      223 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_pbs_ssh_india.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      224 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_pbs_ssh_sierra.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      230 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_pbs_ssh_trestles.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      157 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_sftp_india.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      161 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_sftp_stampede.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      323 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_sge_gsissh_lonestar.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      398 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_sge_ssh_lonestar.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      273 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_slurm_ssh_comet.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      358 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_slurm_ssh_stampede.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      345 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_ssh_boskop.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      132 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_ssh_gw86.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      118 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_ssh_india.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      172 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_ssh_localhost.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      169 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_ssh_silver.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      311 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/tests/test_torque_gsissh_supermic.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1314 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/configs/utils_default.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1377 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/constants.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     5895 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/context.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.749540 radical.saga-1.8.0/src/radical/saga/engine/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      306 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/engine/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    22540 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/engine/engine.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    16389 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/exceptions.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.749540 radical.saga-1.8.0/src/radical/saga/filesystem/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      202 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/filesystem/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      872 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/filesystem/constants.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     7788 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/filesystem/directory.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    11356 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/filesystem/file.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.749540 radical.saga-1.8.0/src/radical/saga/job/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      320 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/job/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     7244 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/job/constants.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1745 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/job/container.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     5730 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/job/description.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    27060 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/job/job.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    14806 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/job/service.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.749540 radical.saga-1.8.0/src/radical/saga/messages/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3240 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/messages/message.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2452 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/monitorable.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.749540 radical.saga-1.8.0/src/radical/saga/namespace/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      206 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/namespace/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      492 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/namespace/constants.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    17201 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/namespace/directory.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    11856 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/namespace/entry.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.749540 radical.saga-1.8.0/src/radical/saga/replica/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      237 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/replica/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      756 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/replica/constants.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     6918 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/replica/logical_directory.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     8558 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/replica/logical_file.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.753540 radical.saga-1.8.0/src/radical/saga/resource/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      222 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/resource/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2952 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/resource/constants.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     9163 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/resource/description.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     9522 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/resource/manager.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    19649 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/resource/resource.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      390 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/sasync.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    10720 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/session.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    22267 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/task.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2113 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/url.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.753540 radical.saga-1.8.0/src/radical/saga/utils/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      247 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/utils/__init__.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.753540 radical.saga-1.8.0/src/radical/saga/utils/job/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      166 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/utils/job/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     4594 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/utils/job/transfer_directives.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     9454 2021-09-23 09:22:40.000000 radical.saga-1.8.0/src/radical/saga/utils/misc.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2154 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/utils/pty_exceptions.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    31387 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/utils/pty_process.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    43400 2021-09-23 11:52:49.000000 radical.saga-1.8.0/src/radical/saga/utils/pty_shell.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    30526 2021-09-23 09:22:40.000000 radical.saga-1.8.0/src/radical/saga/utils/pty_shell_factory.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2551 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/utils/test_config.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      413 2021-04-14 10:16:16.000000 radical.saga-1.8.0/src/radical/saga/version.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 11:55:47.721540 radical.saga-1.8.0/src/radical.saga.egg-info/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1092 2021-09-23 11:55:47.000000 radical.saga-1.8.0/src/radical.saga.egg-info/PKG-INFO
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     9347 2021-09-23 11:55:47.000000 radical.saga-1.8.0/src/radical.saga.egg-info/SOURCES.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2021-09-23 11:55:47.000000 radical.saga-1.8.0/src/radical.saga.egg-info/dependency_links.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        8 2021-09-23 11:55:47.000000 radical.saga-1.8.0/src/radical.saga.egg-info/namespace_packages.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2021-09-23 11:55:47.000000 radical.saga-1.8.0/src/radical.saga.egg-info/not-zip-safe
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       36 2021-09-23 11:55:47.000000 radical.saga-1.8.0/src/radical.saga.egg-info/requires.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        8 2021-09-23 11:55:47.000000 radical.saga-1.8.0/src/radical.saga.egg-info/top_level.txt
```

### Comparing `radical.saga-1.6.9/CHANGES.md` & `radical.saga-1.8.0/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 
 
 For a list of open issues and known problems, see:
 https://github.com/radical-cybertools/radical.saga/issues
 
-Hotfix Version 1.6.9 Release                                          2021-07-16
+Hotfix 1.8.0 Release                                                  2021-09-23
+--------------------------------------------------------------------------------
+
+  - fix directory creation (recursive flag is set)
+  - add longhorn GRES exception
+
+
+Hotfix Version 1.6.10 Release                                         2021-07-16
 --------------------------------------------------------------------------------
 
   - typo
 
 
 Version 1.6.8 Release                                                 2021-07-08
 --------------------------------------------------------------------------------
```

### Comparing `radical.saga-1.6.9/LICENSE.md` & `radical.saga-1.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/PKG-INFO` & `radical.saga-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: radical.saga
-Version: 1.6.9
+Version: 1.8.0
 Summary: A light-weight access layer for distributed computing infrastructure (http://radical.rutgers.edu/)
 Home-page: http://radical-cybertools.github.io/radical.saga/
 Author: RADICAL Group at Rutgers University
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Group
 Maintainer-email: radical@rutgers.edu
 License: MIT
```

### Comparing `radical.saga-1.6.9/README.md` & `radical.saga-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/context/context_ssh.py` & `radical.saga-1.8.0/examples/context/context_ssh.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/files/go_file_copy.py` & `radical.saga-1.8.0/examples/files/go_file_copy.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/files/go_remotedir_list.py` & `radical.saga-1.8.0/examples/files/go_remotedir_list.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/files/http_file_copy.py` & `radical.saga-1.8.0/examples/files/http_file_copy.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/files/sftp_file_copy.py` & `radical.saga-1.8.0/examples/files/sftp_file_copy.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/files/sftp_remotedir_list.py` & `radical.saga-1.8.0/examples/files/sftp_remotedir_list.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/files/srm_get_size.py` & `radical.saga-1.8.0/examples/files/srm_get_size.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/jobs/cobalt.py` & `radical.saga-1.8.0/examples/jobs/cobalt.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/jobs/condorjob.py` & `radical.saga-1.8.0/examples/jobs/condorjob.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/jobs/loadlevelerjob.py` & `radical.saga-1.8.0/examples/jobs/loadlevelerjob.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/jobs/localjob.py` & `radical.saga-1.8.0/examples/jobs/localjob.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/jobs/localjobcontainer.py` & `radical.saga-1.8.0/examples/jobs/localjobcontainer.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/jobs/lsfjob.py` & `radical.saga-1.8.0/examples/jobs/lsfjob.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/jobs/noopjob.py` & `radical.saga-1.8.0/examples/jobs/noopjob.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/jobs/pbsgsisshjob.py` & `radical.saga-1.8.0/examples/jobs/pbsgsisshjob.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/jobs/pbsjob.py` & `radical.saga-1.8.0/examples/jobs/pbsjob.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/jobs/pbsprojob.py` & `radical.saga-1.8.0/examples/jobs/pbsprojob.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/jobs/sgejob.py` & `radical.saga-1.8.0/examples/jobs/sgejob.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/jobs/slurmjob.py` & `radical.saga-1.8.0/examples/jobs/slurmjob.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/jobs/slurmjobcontainer.py` & `radical.saga-1.8.0/examples/jobs/slurmjobcontainer.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/jobs/torque_gsissh_job.py` & `radical.saga-1.8.0/examples/jobs/torque_gsissh_job.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/master_worker/master.py` & `radical.saga-1.8.0/examples/master_worker/master.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/master_worker/worker.py` & `radical.saga-1.8.0/examples/master_worker/worker.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/replica/irods/irods_test.py` & `radical.saga-1.8.0/examples/replica/irods/irods_test.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/resource/amazon_ec2.py` & `radical.saga-1.8.0/examples/resource/amazon_ec2.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/resource/ec2.py` & `radical.saga-1.8.0/examples/resource/ec2.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/tutorial/mandelbrot/mandelbrot.py` & `radical.saga-1.8.0/examples/tutorial/mandelbrot/mandelbrot.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/tutorial/mandelbrot/saga_mandelbrot.py` & `radical.saga-1.8.0/examples/tutorial/mandelbrot/saga_mandelbrot.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/tutorial/mandelbrot/saga_mandelbrot_osg.py` & `radical.saga-1.8.0/examples/tutorial/mandelbrot/saga_mandelbrot_osg.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/tutorial/saga_example_local.py` & `radical.saga-1.8.0/examples/tutorial/saga_example_local.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/tutorial/saga_example_remote.py` & `radical.saga-1.8.0/examples/tutorial/saga_example_remote.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/tutorial/saga_example_remote_cluster_staging.py` & `radical.saga-1.8.0/examples/tutorial/saga_example_remote_cluster_staging.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/examples/tutorial/saga_example_remote_staging.py` & `radical.saga-1.8.0/examples/tutorial/saga_example_remote_staging.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/setup.py` & `radical.saga-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/__init__.py` & `radical.saga-1.8.0/src/radical/saga/__init__.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/aws/ec2_resource.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/aws/ec2_resource.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/base.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/base.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/cobalt/cobaltjob.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cobalt/cobaltjob.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/condor/condorjob.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/condor/condorjob.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/condor/transferdirectives.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/condor/transferdirectives.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/context/myproxy.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/context/myproxy.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/context/ssh.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/context/ssh.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/context/userpass.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/context/userpass.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/context/x509.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/context/x509.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/cpi/advert/directory.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/advert/directory.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/cpi/advert/entry.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/advert/entry.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/cpi/attributes.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/attributes.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/cpi/base.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/base.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/cpi/decorators.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/decorators.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/cpi/filesystem/directory.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/filesystem/directory.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/cpi/filesystem/file.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/filesystem/file.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/cpi/job/job.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/job/job.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/cpi/job/service.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/job/service.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/cpi/namespace/directory.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/namespace/directory.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/cpi/namespace/entry.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/namespace/entry.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/cpi/replica/logical_directory.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/replica/logical_directory.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/cpi/replica/logical_file.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/replica/logical_file.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/cpi/resource/manager.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/resource/manager.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/cpi/resource/resource.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/cpi/resource/resource.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/globus_online/go_file.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/globus_online/go_file.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/http/http_file.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/http/http_file.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/irods/irods_replica.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/irods/irods_replica.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/loadl/loadljob.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/loadl/loadljob.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/lsf/lsfjob.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/lsf/lsfjob.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/mock/shell_file.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/mock/shell_file.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/mock/shell_job.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/mock/shell_job.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/mock/shell_resource.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/mock/shell_resource.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/noop/noop_job.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/noop/noop_job.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/pbs/pbsjob.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/pbs/pbsjob.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/pbspro/pbsprojob.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/pbspro/pbsprojob.py`

 * *Files 0% similar despite different names*

```diff
@@ -882,15 +882,15 @@
                   #        modification time) which is generally also end time.
                   #        TORQUE has an "comp_time" (completion? time), that is
                   #        generally the same as mtime.
                   #
                   #        For now we use mtime for both TORQUE and PBS Pro.
 
             # split exec hosts list if set
-            if job_info['exec_hosst']:
+            if job_info['exec_host']:
                 job_info['exec_hosts'] = job_info['exec_hosts'].split('+')
 
             # TORQUE doesn't allow us to distinguish DONE/FAILED on final state
             # alone, we need to consider the exit_status.
             retcode = job_info.get('returncode', -1)
             job_info['state'] = _to_saga_jobstate(job_state, retcode)
```

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/redis/redis_1.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_1.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/redis/redis_2.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_2.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/redis/redis_advert.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_advert.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/redis/redis_cache.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_cache.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/redis/redis_namespace.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/redis/redis_namespace.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/sge/sgejob.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/sge/sgejob.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/shell/shell_file.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/shell/shell_file.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/shell/shell_job.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/shell/shell_job.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/shell/shell_resource.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/shell/shell_resource.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/shell/shell_wrapper.sh` & `radical.saga-1.8.0/src/radical/saga/adaptors/shell/shell_wrapper.sh`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/slurm/slurm_job.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/slurm/slurm_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -637,14 +637,17 @@
         elif 'cori' in self.rm.host.lower():
 
             # Set to "haswell" for Haswell nodes, to "knl,quad,cache" (or other
             # modes) for KNL, etc.
             if cpu_arch : script += "#SBATCH -C %s\n"     % cpu_arch
             if gpu_count: script += "#SBATCH --gpus=%s\n" % gpu_count
 
+        elif 'longhorn' in self.rm.host.lower():
+            self._logger.debug("SLURM GRES is not set (longhorn exception)\n")
+
         elif queue == 'tmp3':
 
             # this is a special queue, which is associated with SuperMUC-NG,
             # but since there is no machine name in config data we only track
             # this queue name to set SLURM QoS option
             script += "#SBATCH --qos=nolimit\n"
             self._logger.debug("SLURM QoS is set (SuperMUC-NG only)\n")
```

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/srm/srmfile.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/srm/srmfile.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/adaptors/torque/torquejob.py` & `radical.saga-1.8.0/src/radical/saga/adaptors/torque/torquejob.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/advert/constants.py` & `radical.saga-1.8.0/src/radical/saga/advert/constants.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/advert/directory.py` & `radical.saga-1.8.0/src/radical/saga/advert/directory.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/advert/entry.py` & `radical.saga-1.8.0/src/radical/saga/advert/entry.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/attributes.py` & `radical.saga-1.8.0/src/radical/saga/attributes.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/base.py` & `radical.saga-1.8.0/src/radical/saga/base.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/configs/adaptors_globus_online_file.json` & `radical.saga-1.8.0/src/radical/saga/configs/adaptors_globus_online_file.json`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/configs/adaptors_sgejob.json` & `radical.saga-1.8.0/src/radical/saga/configs/adaptors_sgejob.json`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/configs/adaptors_shell_job.json` & `radical.saga-1.8.0/src/radical/saga/configs/adaptors_shell_job.json`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/configs/registry_default.json` & `radical.saga-1.8.0/src/radical/saga/configs/registry_default.json`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/configs/session.json` & `radical.saga-1.8.0/src/radical/saga/configs/session.json`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/configs/utils_default.json` & `radical.saga-1.8.0/src/radical/saga/configs/utils_default.json`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/constants.py` & `radical.saga-1.8.0/src/radical/saga/constants.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/context.py` & `radical.saga-1.8.0/src/radical/saga/context.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/engine/engine.py` & `radical.saga-1.8.0/src/radical/saga/engine/engine.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/exceptions.py` & `radical.saga-1.8.0/src/radical/saga/exceptions.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/filesystem/constants.py` & `radical.saga-1.8.0/src/radical/saga/filesystem/constants.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/filesystem/directory.py` & `radical.saga-1.8.0/src/radical/saga/filesystem/directory.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/filesystem/file.py` & `radical.saga-1.8.0/src/radical/saga/filesystem/file.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/job/constants.py` & `radical.saga-1.8.0/src/radical/saga/job/constants.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/job/container.py` & `radical.saga-1.8.0/src/radical/saga/job/container.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/job/description.py` & `radical.saga-1.8.0/src/radical/saga/job/description.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/job/job.py` & `radical.saga-1.8.0/src/radical/saga/job/job.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/job/service.py` & `radical.saga-1.8.0/src/radical/saga/job/service.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/messages/message.py` & `radical.saga-1.8.0/src/radical/saga/messages/message.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/monitorable.py` & `radical.saga-1.8.0/src/radical/saga/monitorable.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/namespace/directory.py` & `radical.saga-1.8.0/src/radical/saga/namespace/directory.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/namespace/entry.py` & `radical.saga-1.8.0/src/radical/saga/namespace/entry.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/replica/constants.py` & `radical.saga-1.8.0/src/radical/saga/replica/constants.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/replica/logical_directory.py` & `radical.saga-1.8.0/src/radical/saga/replica/logical_directory.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/replica/logical_file.py` & `radical.saga-1.8.0/src/radical/saga/replica/logical_file.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/resource/constants.py` & `radical.saga-1.8.0/src/radical/saga/resource/constants.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/resource/description.py` & `radical.saga-1.8.0/src/radical/saga/resource/description.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/resource/manager.py` & `radical.saga-1.8.0/src/radical/saga/resource/manager.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/resource/resource.py` & `radical.saga-1.8.0/src/radical/saga/resource/resource.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/session.py` & `radical.saga-1.8.0/src/radical/saga/session.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/task.py` & `radical.saga-1.8.0/src/radical/saga/task.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/url.py` & `radical.saga-1.8.0/src/radical/saga/url.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/utils/job/transfer_directives.py` & `radical.saga-1.8.0/src/radical/saga/utils/job/transfer_directives.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/utils/misc.py` & `radical.saga-1.8.0/src/radical/saga/utils/misc.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/utils/pty_exceptions.py` & `radical.saga-1.8.0/src/radical/saga/utils/pty_exceptions.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/utils/pty_process.py` & `radical.saga-1.8.0/src/radical/saga/utils/pty_process.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/utils/pty_shell.py` & `radical.saga-1.8.0/src/radical/saga/utils/pty_shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -974,40 +974,48 @@
             # run the actual copy command.
             if  not self.cp_slave :
                 self._trace ("get cp slave")
                 self.cp_slave = self.factory.get_cp_slave (s_cmd, info, posix)
 
             self.cp_slave.flush ()
             if  'sftp' in s_cmd :
+
+                # ensure that parent directory exists in case of recursive copy
+                # (*) option "-p" for "mkdir" is not applicable within "sftp"
+                if '-r' in cp_flags and os.path.split(tgt)[0]:
+                    # with recursive flag it is assumed that `tgt` is directory
+                    if tgt.endswith('/'):
+                        tgt = os.path.dirname(tgt)
+                    # TODO: this needs to be numeric and checking the flag
+                    prep = "mkdir %s\n" % tgt
+                    # TODO: this doesn't deal with multiple levels of creation
+
+                    self.cp_slave.flush()
+                    self.cp_slave.write("%s\n" % prep)
+                    self.cp_slave.find(['[\$\>\]]\s*$'], -1)
+                    # TODO: check return values
+
                 # prepare target dirs for recursive copy, if needed
                 import glob
                 src_list = glob.glob (src)
                 for s in src_list :
-                    if  os.path.isdir (s) :
+                    if os.path.isdir (s) :
+                        if s.endswith('/'):
+                            s = os.path.dirname(s)
                         prep = "mkdir %s/%s\n" % (tgt, os.path.basename (s))
                         # TODO: handle multiple levels of creation
 
                         self.cp_slave.flush()
                         self.cp_slave.write("%s\n" % prep)
                         self.cp_slave.find(['[\$\>\]]\s*$'], -1)
                         # TODO: check return values
 
-                if cp_flags == sfs.CREATE_PARENTS and os.path.split(tgt)[0]:
-                    # TODO: this needs to be numeric and checking the flag
-                    prep = "mkdir %s\n" % os.path.dirname(tgt)
-                    # TODO: this doesn't deal with multiple levels of creation
-
-                    self.cp_slave.flush()
-                    self.cp_slave.write("%s\n" % prep)
-                    self.cp_slave.find(['[\$\>\]]\s*$'], -1)
-                    # TODO: check return values
-
             self.cp_slave.flush()
-            _ = self.cp_slave.write("%s\n" % s_in)
-            _, out = self.cp_slave.find(['[\$\>\]]\s*$'], -1)
+            self.cp_slave.write("%s\n" % s_in)
+            out = self.cp_slave.find(['[\$\>\]]\s*$'], -1)[1]
 
             # FIXME: we don't really get exit codes from copy
             # if  self.cp_slave.exit_code != 0 :
             #     raise rse.NoSuccess._log (info['logger'],
             #                              "file copy failed: %s" % str(out))
 
             if 'Invalid flag' in out :
@@ -1106,20 +1114,22 @@
                 # prepare target dirs for recursive copy, if needed
                 self.cp_slave.write (" ls %s\n" % src)
                 _, out = self.cp_slave.find (["^sftp> "], -1)
 
                 src_list = out[1].split('\n')
 
                 for s in src_list :
-                    if  os.path.isdir (s) :
+                    if os.path.isdir (s) :
+                        if s.endswith('/'):
+                            s = os.path.dirname(s)
                         prep += "lmkdir %s/%s\n" % (tgt, os.path.basename (s))
 
             self.cp_slave.flush ()
-            _      = self.cp_slave.write("%s%s\n" % (prep, s_in))
-            _, out = self.cp_slave.find (['[\$\>\]] *$'], -1)
+            self.cp_slave.write("%s%s\n" % (prep, s_in))
+            out = self.cp_slave.find (['[\$\>\]] *$'], -1)[1]
 
             # FIXME: we don't really get exit codes from copy
           # if  self.cp_slave.exit_code != 0 :
           #     raise NoSuccess._log (info['logger'],
           #                           "file copy failed: %s" % out)
 
             if 'Invalid flag' in out :
```

### Comparing `radical.saga-1.6.9/src/radical/saga/utils/pty_shell_factory.py` & `radical.saga-1.8.0/src/radical/saga/utils/pty_shell_factory.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical/saga/utils/test_config.py` & `radical.saga-1.8.0/src/radical/saga/utils/test_config.py`

 * *Files identical despite different names*

### Comparing `radical.saga-1.6.9/src/radical.saga.egg-info/PKG-INFO` & `radical.saga-1.8.0/src/radical.saga.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: radical.saga
-Version: 1.6.9
+Version: 1.8.0
 Summary: A light-weight access layer for distributed computing infrastructure (http://radical.rutgers.edu/)
 Home-page: http://radical-cybertools.github.io/radical.saga/
 Author: RADICAL Group at Rutgers University
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Group
 Maintainer-email: radical@rutgers.edu
 License: MIT
```

### Comparing `radical.saga-1.6.9/src/radical.saga.egg-info/SOURCES.txt` & `radical.saga-1.8.0/src/radical.saga.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 src/radical/saga/__init__.py
 src/radical/saga/attributes.py
 src/radical/saga/base.py
 src/radical/saga/constants.py
 src/radical/saga/context.py
 src/radical/saga/exceptions.py
 src/radical/saga/monitorable.py
-src/radical/saga/radical.saga-1.6.6-scalems-stable-3-ge70b9f8b-devel.tar.gz
 src/radical/saga/sasync.py
 src/radical/saga/session.py
 src/radical/saga/task.py
 src/radical/saga/url.py
 src/radical/saga/version.py
 src/radical/saga/adaptors/__init__.py
 src/radical/saga/adaptors/base.py
```

