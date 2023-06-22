# Comparing `tmp/dynaconf_aws_loader-0.3.2.tar.gz` & `tmp/dynaconf_aws_loader-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynaconf_aws_loader-0.3.2.tar", max compression
+gzip compressed data, was "dynaconf_aws_loader-0.4.0.tar", max compression
```

## Comparing `dynaconf_aws_loader-0.3.2.tar` & `dynaconf_aws_loader-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      282 2023-06-07 19:08:03.503127 dynaconf_aws_loader-0.3.2/CHANGELOG.md
--rw-r--r--   0        0        0     1072 2023-06-07 19:08:03.503127 dynaconf_aws_loader-0.3.2/LICENSE
--rw-r--r--   0        0        0     6557 2023-06-07 19:08:03.503127 dynaconf_aws_loader-0.3.2/README.rst
--rw-r--r--   0        0        0      369 2023-06-07 19:08:03.503127 dynaconf_aws_loader-0.3.2/dynaconf_aws_loader/__init__.py
--rw-r--r--   0        0        0     5702 2023-06-07 19:08:03.503127 dynaconf_aws_loader-0.3.2/dynaconf_aws_loader/loader.py
--rw-r--r--   0        0        0      757 2023-06-07 19:08:03.503127 dynaconf_aws_loader-0.3.2/dynaconf_aws_loader/util.py
--rw-r--r--   0        0        0     1249 2023-06-07 19:08:03.503127 dynaconf_aws_loader-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     7648 1970-01-01 00:00:00.000000 dynaconf_aws_loader-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      965 2023-06-22 21:50:27.706709 dynaconf_aws_loader-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1072 2023-06-22 21:50:27.706709 dynaconf_aws_loader-0.4.0/LICENSE
+-rw-r--r--   0        0        0     7962 2023-06-22 21:50:27.706709 dynaconf_aws_loader-0.4.0/README.rst
+-rw-r--r--   0        0        0      369 2023-06-22 21:50:27.706709 dynaconf_aws_loader-0.4.0/dynaconf_aws_loader/__init__.py
+-rw-r--r--   0        0        0     8797 2023-06-22 21:50:27.706709 dynaconf_aws_loader-0.4.0/dynaconf_aws_loader/loader.py
+-rw-r--r--   0        0        0     1752 2023-06-22 21:50:27.706709 dynaconf_aws_loader-0.4.0/dynaconf_aws_loader/util.py
+-rw-r--r--   0        0        0     1249 2023-06-22 21:50:27.710709 dynaconf_aws_loader-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9054 1970-01-01 00:00:00.000000 dynaconf_aws_loader-0.4.0/PKG-INFO
```

### Comparing `dynaconf_aws_loader-0.3.2/LICENSE` & `dynaconf_aws_loader-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dynaconf_aws_loader-0.3.2/README.rst` & `dynaconf_aws_loader-0.4.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -23,19 +23,31 @@
 
 
 Note that for the basic functioning of this loader, the `environments <https://www.dynaconf.com/configuration/#environments>`_ option for ``Dynaconf`` must be set, and an environment must be used.
 
 Configuration Variables
 -----------------------
 
-- ``AWS_SSM_PARAMETER_PROJECT_PREFIX``: Required.
-  The ``project`` prefix in the parameter store path. This value is required. It may be set in ``settings.toml`` (or equivalent), *or* may be sourced from the environment directly. This latter is a useful option if you wish to avoid using materialized settings files and instead wish to use environment variables only.
+Both of the following configuration values should be set in the *environment* to avoid a chicken/egg scenario for initializing this custom loader:
+
+- ``SSM_PARAMETER_PROJECT_PREFIX_FOR_DYNACONF``: Required.
+  The ``project`` prefix in the parameter store path. For example, if the parameter hierarchy looks something like ``/baldur/development/database_uri``, then in this case ``SSM_PARAMETER_PROJECT_PREFIX_FOR_DYNACONF=baldur``.
+
+- ``SSM_PARAMETER_NAMESPACE_FOR_DYNACONF``: Optional.
+  This provides an additional level of grouping once the project and environment have been determined. For example, if the parameter hierarchy looks something like ``/baldur/pr-123/development/database_uri``, then ``SSM_PARAMETER_NAMESPACE_FOR_DYNACONF=pr-123``.
+
+.. note::
+   If a namespace is utilized, be aware that namespaced settings will be *merged* with non-namespaced settings. This merge is a naive one, where namespaced settings will completely overwrite non-namespaced settings with the same key.
+
+The following optional variables should be set in your ``settings.toml`` (or equivalent format), if desired:
+
+- ``SSM_ENDPOINT_URL_FOR_DYNACONF``: If your AWS SSM uses a different endpoint than the AWS default. This can be useful for local development when you are running something like `LocalStack <https://localstack.cloud/>`_.
+- ``SSM_SESSION_FOR_DYNACONF``: If you require custom `boto3.session.Session <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/core/session.html>`_ arguments, you can specify then as a dictionary here. Note that this will override the default ``boto3`` credential configuration.
+- ``SSM_LOAD_DEFAULT_ENV_FOR_DYNACONF``: Boolean, defaults to ``True``. If you want the SSM loader to load keys under the ``default`` environment name. The key name itself can be set via the Dynaconf setting of ``DEFAULT_ENV_FOR_DYNACONF`` if you want it to be something other than ``default``.
 
-- ``AWS_SSM_PARAMETER_NAMESPACE``: Optional.
-  This provides an additional level of grouping once the project and environment have been determined.
 
 Parameter Store Details
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 The structure that this loader expects from the path-based organization in SSM is:
 
 .. code-block::
@@ -48,15 +60,16 @@
 .. code-block::
 
     /<project-name>/<environment>/<namespace>/<parameter-name>
 
 
 Note that if you choose to use a ``namespace`` identifier, it must not conflict with existing ``environment`` identifiers.
 
-The ``environment`` identifiers of: ``default``, ``main``, ``global``, and ``dynaconf`` indicate that any parameters nested below said identifiers will be inherited by *all* environments; these names are Dynaconf defaults. This can be useful for setting a default value that can then be overridden on a per-environment basis as necessary.
+If ``SSM_LOAD_DEFAULT_ENV_FOR_DYNACONF`` is set to ``True`` (which is the default value), the loader will add whatever the value of ``DEFAULT_ENV_FOR_DYNACONF`` as an ``environment`` key to load from SSM. The typical use case here is to have a default value for all environments that can be overriden on a per-environment basis as necessary.
+
 
 Security Considerations
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 For this loader to function correctly and securely, the use of IAM policies to restrict which parameters can be read/mutated is highly encouraged.
 
 Policies can be enacted on a glob-path basis, which will ensure that the only parameters that can be fetched/hydrated into the local object instance are the ones that the current environment is permitted to load.
```

### Comparing `dynaconf_aws_loader-0.3.2/pyproject.toml` & `dynaconf_aws_loader-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "dynaconf-aws-loader"
-version = "0.3.2"
-description = "A custom loader for Dynaconf that uses AWS Systems Manager Parameter Store as a source of truth"
+version = "0.4.0"
+description = "A custom loader for Dynaconf that uses AWS Systems Manager Parameter Store as a source of truth."
 homepage = "https://github.com/fictivekin/dynaconf-aws-loader"
 repository = "https://github.com/fictivekin/dynaconf-aws-loader"
 authors = [
     "Joël Perras <joel@fictivekin.com>",
 ]
 readme = "README.rst"
 packages = [{include = "dynaconf_aws_loader"}]
@@ -18,15 +18,14 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = [
     "LICENSE",
     "CHANGELOG.md"
 ]
 
-
 [tool.poetry.dependencies]
 python = "^3.8"
 boto3 = "^1.26"
 botocore = "^1.29"
 dynaconf = "^3.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `dynaconf_aws_loader-0.3.2/PKG-INFO` & `dynaconf_aws_loader-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dynaconf-aws-loader
-Version: 0.3.2
-Summary: A custom loader for Dynaconf that uses AWS Systems Manager Parameter Store as a source of truth
+Version: 0.4.0
+Summary: A custom loader for Dynaconf that uses AWS Systems Manager Parameter Store as a source of truth.
 Home-page: https://github.com/fictivekin/dynaconf-aws-loader
 License: MIT
 Keywords: dynaconf,AWS,SSM
 Author: Joël Perras
 Author-email: joel@fictivekin.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
@@ -49,19 +49,31 @@
 
 
 Note that for the basic functioning of this loader, the `environments <https://www.dynaconf.com/configuration/#environments>`_ option for ``Dynaconf`` must be set, and an environment must be used.
 
 Configuration Variables
 -----------------------
 
-- ``AWS_SSM_PARAMETER_PROJECT_PREFIX``: Required.
-  The ``project`` prefix in the parameter store path. This value is required. It may be set in ``settings.toml`` (or equivalent), *or* may be sourced from the environment directly. This latter is a useful option if you wish to avoid using materialized settings files and instead wish to use environment variables only.
+Both of the following configuration values should be set in the *environment* to avoid a chicken/egg scenario for initializing this custom loader:
+
+- ``SSM_PARAMETER_PROJECT_PREFIX_FOR_DYNACONF``: Required.
+  The ``project`` prefix in the parameter store path. For example, if the parameter hierarchy looks something like ``/baldur/development/database_uri``, then in this case ``SSM_PARAMETER_PROJECT_PREFIX_FOR_DYNACONF=baldur``.
+
+- ``SSM_PARAMETER_NAMESPACE_FOR_DYNACONF``: Optional.
+  This provides an additional level of grouping once the project and environment have been determined. For example, if the parameter hierarchy looks something like ``/baldur/pr-123/development/database_uri``, then ``SSM_PARAMETER_NAMESPACE_FOR_DYNACONF=pr-123``.
+
+.. note::
+   If a namespace is utilized, be aware that namespaced settings will be *merged* with non-namespaced settings. This merge is a naive one, where namespaced settings will completely overwrite non-namespaced settings with the same key.
+
+The following optional variables should be set in your ``settings.toml`` (or equivalent format), if desired:
+
+- ``SSM_ENDPOINT_URL_FOR_DYNACONF``: If your AWS SSM uses a different endpoint than the AWS default. This can be useful for local development when you are running something like `LocalStack <https://localstack.cloud/>`_.
+- ``SSM_SESSION_FOR_DYNACONF``: If you require custom `boto3.session.Session <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/core/session.html>`_ arguments, you can specify then as a dictionary here. Note that this will override the default ``boto3`` credential configuration.
+- ``SSM_LOAD_DEFAULT_ENV_FOR_DYNACONF``: Boolean, defaults to ``True``. If you want the SSM loader to load keys under the ``default`` environment name. The key name itself can be set via the Dynaconf setting of ``DEFAULT_ENV_FOR_DYNACONF`` if you want it to be something other than ``default``.
 
-- ``AWS_SSM_PARAMETER_NAMESPACE``: Optional.
-  This provides an additional level of grouping once the project and environment have been determined.
 
 Parameter Store Details
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 The structure that this loader expects from the path-based organization in SSM is:
 
 .. code-block::
@@ -74,15 +86,16 @@
 .. code-block::
 
     /<project-name>/<environment>/<namespace>/<parameter-name>
 
 
 Note that if you choose to use a ``namespace`` identifier, it must not conflict with existing ``environment`` identifiers.
 
-The ``environment`` identifiers of: ``default``, ``main``, ``global``, and ``dynaconf`` indicate that any parameters nested below said identifiers will be inherited by *all* environments; these names are Dynaconf defaults. This can be useful for setting a default value that can then be overridden on a per-environment basis as necessary.
+If ``SSM_LOAD_DEFAULT_ENV_FOR_DYNACONF`` is set to ``True`` (which is the default value), the loader will add whatever the value of ``DEFAULT_ENV_FOR_DYNACONF`` as an ``environment`` key to load from SSM. The typical use case here is to have a default value for all environments that can be overriden on a per-environment basis as necessary.
+
 
 Security Considerations
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 For this loader to function correctly and securely, the use of IAM policies to restrict which parameters can be read/mutated is highly encouraged.
 
 Policies can be enacted on a glob-path basis, which will ensure that the only parameters that can be fetched/hydrated into the local object instance are the ones that the current environment is permitted to load.
```

