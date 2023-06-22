# Comparing `tmp/gimme aws creds-2.6.1.tar.gz` & `tmp/gimme aws creds-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimme aws creds-2.6.1.tar", last modified: Thu May  4 16:36:43 2023, max compression
+gzip compressed data, was "gimme aws creds-2.7.0.tar", last modified: Thu Jun 22 16:25:25 2023, max compression
```

## Comparing `gimme aws creds-2.6.1.tar` & `gimme aws creds-2.7.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:36:43.429546 gimme aws creds-2.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/LONG_DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-04 16:36:43.429546 gimme aws creds-2.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:36:43.425546 gimme aws creds-2.6.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      753 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/bin/gimme-aws-creds
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/bin/gimme-aws-creds-autocomplete.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/bin/gimme-aws-creds.cmd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:36:43.425546 gimme aws creds-2.6.1/gimme_aws_creds/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    26779 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/duo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    38888 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    47402 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/okta_classic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/okta_identity_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/registered_authenticators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/u2f.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/gimme_aws_creds/webauthn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:36:43.429546 gimme aws creds-2.6.1/gimme_aws_creds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-04 16:36:43.000000 gimme aws creds-2.6.1/gimme_aws_creds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-04 16:36:43.000000 gimme aws creds-2.6.1/gimme_aws_creds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:36:43.000000 gimme aws creds-2.6.1/gimme_aws_creds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-04 16:36:43.000000 gimme aws creds-2.6.1/gimme_aws_creds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-04 16:36:43.000000 gimme aws creds-2.6.1/gimme_aws_creds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-04 16:36:43.429546 gimme aws creds-2.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-04 16:36:31.000000 gimme aws creds-2.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:25:25.518840 gimme aws creds-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/LONG_DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-22 16:25:25.518840 gimme aws creds-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19434 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:25:25.514840 gimme aws creds-2.7.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      753 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/bin/gimme-aws-creds
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/bin/gimme-aws-creds-autocomplete.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/bin/gimme-aws-creds.cmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:25:25.518840 gimme aws creds-2.7.0/gimme_aws_creds/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/gimme_aws_creds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/gimme_aws_creds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/gimme_aws_creds/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30174 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/gimme_aws_creds/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/gimme_aws_creds/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/gimme_aws_creds/duo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/gimme_aws_creds/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37379 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/gimme_aws_creds/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47519 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/gimme_aws_creds/okta_classic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/gimme_aws_creds/okta_identity_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/gimme_aws_creds/registered_authenticators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/gimme_aws_creds/u2f.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/gimme_aws_creds/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/gimme_aws_creds/webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:25:25.518840 gimme aws creds-2.7.0/gimme_aws_creds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-22 16:25:25.000000 gimme aws creds-2.7.0/gimme_aws_creds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-22 16:25:25.000000 gimme aws creds-2.7.0/gimme_aws_creds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:25:25.000000 gimme aws creds-2.7.0/gimme_aws_creds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-22 16:25:25.000000 gimme aws creds-2.7.0/gimme_aws_creds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 16:25:25.000000 gimme aws creds-2.7.0/gimme_aws_creds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-22 16:25:25.518840 gimme aws creds-2.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-22 16:25:14.000000 gimme aws creds-2.7.0/setup.py
```

### Comparing `gimme aws creds-2.6.1/LICENSE` & `gimme aws creds-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.1/LONG_DESCRIPTION.md` & `gimme aws creds-2.7.0/LONG_DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.1/NOTICE` & `gimme aws creds-2.7.0/NOTICE`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.1/PKG-INFO` & `gimme aws creds-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimme aws creds
-Version: 2.6.1
+Version: 2.7.0
 Summary: A CLI to get temporary AWS credentials from Okta
 Home-page: https://github.com/Nike-Inc/gimme-aws-creds
 Author: Eric Pierce
 Author-email: eric.pierce@nike.com
 License: Apache License, v2.0
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `gimme aws creds-2.6.1/README.md` & `gimme aws creds-2.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -153,23 +153,35 @@
 autoload bashcompinit
 bashcompinit
 source ${INSTALL_DIR}/gimme-aws-creds-autocomplete.sh
 ```
 
 ## Using gimme-aws-creds with Okta Identity Engine
 
+There are two options for using gimme-aws-creds with an OIE domain:
+* Device Authorization Flow
+* Forcing the use of the Okta Classic login flow
+
+### Okta Identity Engine and Device Authorization Flow
+This is the recommended method for authentication with OIE.  It matches the flow used by Okta's [AWS client](https://github.com/okta/okta-aws-cli).  When using gimme-aws-creds with the Device Authorization flow, you will authenticate using your browser.  Storing credentials in keychain or passing MFA codes through the command-line is NOT POSSIBLE.
+
 To use gimme-aws-creds with an Okta Identity Engine (OIE) domain, you must create a new OIDC Native Application and connect it to your AWS integration app(s).
 
 The OIDC Native Application requires Grant Types `Authorization Code`, `Device Authorization` , and `Token Exchange`. These settings are in the Okta Admin UI at `Applications > [the OIDC app] > General Settings > Grant type`.
 
 The pairing with the AWS Federation Application is achieved in the Fed app's Sign On Settings. These settings are in the Okta Admin UI at `Applications > [the AWS Fed app] > Sign On`. Make sure to set the `Allowed Web SSO Client` value to the Client ID of the OIDC Native Application. Repeat that setting for each AWS application you want to access with gimme-aws-creds.
 
 Finally, set the Client ID in gimme-aws-creds (`gimme-aws-creds --action-configure` or update the `client_id` parameter in your config file)
 
-**When using gimme-aws-creds with an OIE domain, you will authenticate using your browser.  Storing credentials in keychain or passing MFA codes through the command-line is NOT POSSIBLE.**
+### Forcing the use of the Okta Classic login flow ###
+The login flow used in Okta Classic currently still works with Okta Identity Engine domains, BUT there are a couple caveats:
+* The Okta classic flow passes the `stateToken` parameter when requesting "step-up" authentication.  This capability was removed in OIE, so if the authentication policy on your AWS app(s) requires MFA but the Global Session Policy does not (or if a higher level of MFA factor is required to access AWS), you cannot authenticate using the classic login flow.
+* MFA using Okta Verify is only supported on mobile devices.  Okta Verify on macOS/Windows is not supported.
+* Passwordless authentication and endpoint security checks are not supported.
+
 
 ## Configuration
 
 To set-up the configuration run:
 
 ```bash
 gimme-aws-creds --action-configure
@@ -204,22 +216,24 @@
 - okta_username - use this username to authenticate
 - preferred_mfa_type - automatically select a particular  device when prompted for MFA:
   - push - Okta Verify App push or DUO push (depends on okta supplied provider type)
   - token:software:totp - OTP using the Okta Verify App
   - token:hardware - OTP using hardware like Yubikey
   - call - OTP via Voice call
   - sms - OTP via SMS message
+  - email - OTP via email
   - web - DUO uses localhost webbrowser to support push|call|passcode
   - passcode - DUO uses `OKTA_MFA_CODE` or `--mfa-code` if set, or prompts user for passcode(OTP).
   
 - resolve_aws_alias - y or n. If yes, gimme-aws-creds will try to resolve AWS account ids with respective alias names (default: n). This option can also be set interactively in the command line using `-r` or `--resolve` parameter
 - include_path - (optional) Includes full role path to the role name in AWS credential profile name. (default: n).  If `y`: `<acct>-/some/path/administrator`. If `n`: `<acct>-administrator`
 - remember_device - y or n. If yes, the MFA device will be remembered by Okta service for a limited time. This option can also be set interactively in the command line using `-m` or `--remember-device`
 - output_format - `json` , `export` or `windows`, determines default credential output format, can be also specified by `--output-format FORMAT` and `-o FORMAT`.
 - open-browser - Open the device authentication link in the default web browser automatically (Okta Identity Engine domains only)
+- force-classic - Force the use of the Okta Classic login process (Okta Identity Engine domains only)
 
 ## Configuration File
 
 The config file follows a [configfile](https://docs.python.org/3/library/configparser.html) format.
 By default, it is located in $HOME/.okta_aws_login_config
 
 Example file:
@@ -293,14 +307,15 @@
 - `GIMME_AWS_CREDS_CRED_PROFILE` - corresponds to `cred_profile` configuration
 - `GIMME_AWS_CREDS_OUTPUT_FORMAT` - corresponds to `output_format` configuration and `--output-format` CLI option
 - `OKTA_AUTH_SERVER` - corresponds to `okta_auth_server` configuration
 - `OKTA_DEVICE_TOKEN` - corresponds to `device_token` configuration, can be used in CI
 - `OKTA_MFA_CODE` - corresponds to `--mfa-code` CLI option
 - `OKTA_PASSWORD` - provides password during authentication, can be used in CI
 - `OKTA_USERNAME` - corresponds to `okta_username` configuration and `--username` CLI option
+- `AWS_STS_REGION` - force the use of the STS in a specific region (`us-east-1`, `eu-north-1`, etc.)
 
 Example: `GIMME_AWS_CREDS_CLIENT_ID='foobar' AWS_DEFAULT_DURATION=12345 gimme-aws-creds`
 
 For changing variables outside of this, you'd need to create a separate profile altogether with `gimme-aws-creds --action-configure --profile profileName`
 
 ### Viewing Profiles
```

### Comparing `gimme aws creds-2.6.1/bin/gimme-aws-creds` & `gimme aws creds-2.7.0/bin/gimme-aws-creds`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.1/bin/gimme-aws-creds-autocomplete.sh` & `gimme aws creds-2.7.0/bin/gimme-aws-creds-autocomplete.sh`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.1/bin/gimme-aws-creds.cmd` & `gimme aws creds-2.7.0/bin/gimme-aws-creds.cmd`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.1/gimme_aws_creds/aws.py` & `gimme aws creds-2.7.0/gimme_aws_creds/aws.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.1/gimme_aws_creds/common.py` & `gimme aws creds-2.7.0/gimme_aws_creds/common.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.1/gimme_aws_creds/config.py` & `gimme aws creds-2.7.0/gimme_aws_creds/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and* limitations under the License.*
 """
 import argparse
 import configparser
 import os
+import requests
 from urllib.parse import urlparse
 
 from . import errors, ui, version
 
 
 class Config(object):
     """
@@ -51,14 +52,15 @@
         self.action_configure = False
         self.action_list_profiles = False
         self.action_list_roles = False
         self.action_store_json_creds = False
         self.action_setup_fido_authenticator = False
         self.action_output_format = False
         self.output_format = 'export'
+        self.force_classic = False
         self.roles = []
 
         if self.ui.environ.get("OKTA_USERNAME") is not None:
             self.username = self.ui.environ.get("OKTA_USERNAME")
 
         if self.ui.environ.get("OKTA_API_KEY") is not None:
             self.api_key = self.ui.environ.get("OKTA_API_KEY")
@@ -146,23 +148,28 @@
             '--action-setup-fido-authenticator', action='store_true',
             help='Sets up a new FIDO WebAuthn authenticator in Okta'
         )
         parser.add_argument(
             '--open-browser', action='store_true',
             help='Automatically open a webbrowser for device authorization (Okta Identity Engine only)'
         )
+        parser.add_argument(
+            '--force-classic', action='store_true',
+            help='Force the use of the Okta Classic login process (Okta Identity Engine only)'
+        )
         args = parser.parse_args(self.ui.args)
 
         self.action_configure = args.action_configure
         self.action_list_profiles = args.action_list_profiles
         self.action_list_roles = args.action_list_roles
         self.action_store_json_creds = args.action_store_json_creds
         self.action_register_device = args.action_register_device
         self.action_setup_fido_authenticator = args.action_setup_fido_authenticator
         self.open_browser = args.open_browser
+        self.force_classic = args.force_classic
 
         if args.insecure is True:
             ui.default.warning("Warning: SSL certificate validation is disabled!")
             self.verify_ssl_certs = False
         else:
             self.verify_ssl_certs = True
 
@@ -249,16 +256,17 @@
             'okta_username': '',
             'app_url': '',
             'resolve_aws_alias': 'n',
             'include_path': 'n',
             'preferred_mfa_type': '',
             'remember_device': 'n',
             'aws_default_duration': '3600',
-            'device_token': '',
             'output_format': 'export',
+            'force_classic': '',
+            'open_browser': ''
         }
 
         # See if a config file already exists.
         # If so, use current values as defaults
         if os.path.isfile(self.OKTA_CONFIG):
             config.read(self.OKTA_CONFIG)
 
@@ -267,32 +275,46 @@
 
                 for default in defaults:
                     defaults[default] = profile.get(default, defaults[default])
 
         # Prompt user for config details and store in config_dict
         config_dict = defaults
         config_dict['okta_org_url'] = self._get_org_url_entry(defaults['okta_org_url'])
-        config_dict['gimme_creds_server'] = self._get_gimme_creds_server_entry(defaults['gimme_creds_server'])
+        client_id_set = False
 
+        # Options specific to OIE domains
+        if self._okta_platform == 'identity_engine':
+            config_dict['force_classic'] = self._get_force_classic(defaults['force_classic'])
+            if config_dict['force_classic'] is False:
+                config_dict['open_browser'] = self._get_open_browser(defaults['open_browser'])
+                config_dict['client_id'] = self._get_client_id_entry(defaults['client_id'])
+                client_id_set = True
+
+        # These options are only used in the Classic authentication flow
+        if self._okta_platform == 'classic' or config_dict['force_classic'] is True:
+            config_dict['okta_username'] = self._get_okta_username(defaults['okta_username'])
+            config_dict['preferred_mfa_type'] = self._get_preferred_mfa_type(defaults['preferred_mfa_type'])
+            config_dict['remember_device'] = self._get_remember_device(defaults['remember_device'])
+
+        # The rest of the options are used in both OIE and Classic
+        config_dict['gimme_creds_server'] = self._get_gimme_creds_server_entry(defaults['gimme_creds_server'])
         if config_dict['gimme_creds_server'] == 'appurl':
             config_dict['app_url'] = self._get_appurl_entry(defaults['app_url'])
         elif config_dict['gimme_creds_server'] != 'internal':
-            config_dict['client_id'] = self._get_client_id_entry(defaults['client_id'])
+            if client_id_set is False:
+                config_dict['client_id'] = self._get_client_id_entry(defaults['client_id'])
             config_dict['okta_auth_server'] = self._get_auth_server_entry(defaults['okta_auth_server'])
-
         config_dict['write_aws_creds'] = self._get_write_aws_creds(defaults['write_aws_creds'])
-        if config_dict['gimme_creds_server'] != 'appurl':
-            config_dict['aws_appname'] = self._get_aws_appname(defaults['aws_appname'])
-        config_dict['resolve_aws_alias'] = self._get_resolve_aws_alias(defaults['resolve_aws_alias'])
         config_dict['include_path'] = self._get_include_path(defaults['include_path'])
         config_dict['aws_rolename'] = self._get_aws_rolename(defaults['aws_rolename'])
-        config_dict['okta_username'] = self._get_okta_username(defaults['okta_username'])
+        config_dict['resolve_aws_alias'] = self._get_resolve_aws_alias(defaults['resolve_aws_alias'])
         config_dict['aws_default_duration'] = self._get_aws_default_duration(defaults['aws_default_duration'])
-        config_dict['preferred_mfa_type'] = self._get_preferred_mfa_type(defaults['preferred_mfa_type'])
-        config_dict['remember_device'] = self._get_remember_device(defaults['remember_device'])
+        if config_dict['gimme_creds_server'] != 'appurl':
+            config_dict['aws_appname'] = self._get_aws_appname(defaults['aws_appname'])
+        
         config_dict["output_format"] = ''
         if not config_dict["write_aws_creds"]:
             config_dict['output_format'] = self._get_output_format(defaults['output_format'])
 
         # If write_aws_creds is True get the profile name
         if config_dict['write_aws_creds'] is True:
             config_dict['cred_profile'] = self._get_cred_profile(defaults['cred_profile'])
@@ -314,27 +336,47 @@
         """ Get and validate okta_org_url """
         ui.default.info("Enter the Okta URL for your organization. This is https://something.okta[preview].com")
         okta_org_url_valid = False
         okta_org_url = default_entry
 
         while okta_org_url_valid is False:
             okta_org_url = self._get_user_input("Okta URL for your organization", default_entry).strip('/')
-            # Validate that okta_org_url is a well formed okta URL
-            url_parse_results = urlparse(okta_org_url)
-            allowlist = [
-                "okta.com",
-                "oktapreview.com",
-                "okta-emea.com",
-            ]
 
-            if url_parse_results.scheme == "https" and any(urlelement in url_parse_results.hostname for urlelement in allowlist):
-                okta_org_url_valid = True
+            # Validate that the URL given is an Okta domain and what the platform is
+            url_parse_results = urlparse(okta_org_url)
+            if url_parse_results.scheme == "https":
+                try:
+                    response = requests.get(
+                        okta_org_url + '/.well-known/okta-organization',
+                        headers={
+                            'Accept': 'application/json',
+                            'User-Agent': "gimme-aws-creds {}".format(version)
+                        },
+                        timeout=30
+                    )
+
+                    response_data = response.json()
+
+                    if response.status_code == 200:
+                        if response_data['pipeline'] == 'v1':
+                            self._okta_platform = 'classic'
+                            okta_org_url_valid = True
+                            ui.default.notify("Okta Classic domain detected")
+                        elif response_data['pipeline'] == 'idx':
+                            self._okta_platform = 'identity_engine'
+                            okta_org_url_valid = True
+                            ui.default.notify("Okta Identity Engine domain detected")
+                        else:
+                            ui.default.error('Unknown Okta platform type: {}'.format(response_data['pipeline']))
+                    else:
+                        response.raise_for_status()
+                except Exception as err:
+                    ui.default.error('{} is not a valid Okta domain'.format(okta_org_url))
             else:
-                ui.default.error(
-                    "Okta organization URL must be HTTPS URL for okta.com or oktapreview.com or okta-emea.com domain")
+                ui.default.error("Okta organization URL must be HTTPS URL")
 
         self._okta_org_url = okta_org_url
 
         return okta_org_url
 
     def _get_auth_server_entry(self, default_entry):
         """ Get and validate okta_auth_server """
@@ -380,15 +422,15 @@
 
         self._app_url = app_url
 
         return app_url
 
     def _get_gimme_creds_server_entry(self, default_entry):
         """ Get gimme_creds_server """
-        ui.default.message("Enter the URL for the gimme-creds-server or 'internal' for handling Okta APIs locally.")
+        ui.default.message("Enter the URL for the gimme-creds-server, 'appurl' for an Okta Application URL or 'internal' for handling Okta APIs locally.")
         gimme_creds_server_valid = False
         gimme_creds_server = default_entry
 
         while gimme_creds_server_valid is False:
             gimme_creds_server = self._get_user_input(
                 "URL for gimme-creds-server", default_entry)
             if gimme_creds_server == "internal":
@@ -485,15 +527,15 @@
         conf_profile = self._get_user_input(
             "Okta Configuration Profile Name", default_entry)
         return conf_profile
 
     def _get_okta_username(self, default_entry):
         """Get and validate okta username. [Optional]"""
         ui.default.message(
-            "If you'd like to set your okta username in the config file, specify the username\n."
+            "If you'd like to set your okta username in the config file, specify the username.\n"
             "This is optional.")
         okta_username = self._get_user_input(
             "Okta User Name", default_entry)
         return okta_username
 
     def _get_aws_default_duration(self, default_entry):
         """Get and validate the aws default session duration. [Optional]"""
@@ -511,14 +553,15 @@
             "This is optional. valid devices types:\n"
             """
             - push - Okta Verify App push or DUO push (depends on okta supplied provider type)
             - token:software:totp - OTP using the Okta Verify App
             - token:hardware - OTP using hardware like Yubikey
             - call - OTP via Voice call
             - sms - OTP via SMS message
+            - email - OTP via email message
             - web - DUO uses localhost webbrowser to support push|call|passcode
             - passcode - DUO uses `OKTA_MFA_CODE` or `--mfa-code` if set, or prompts user for passcode(OTP).
             """
         )
         okta_username = self._get_user_input(
             "Preferred MFA Device Type", default_entry)
         return okta_username
@@ -540,14 +583,38 @@
         while True:
             try:
                 return self._get_user_input_yes_no(
                     "Remember device", default_entry)
             except ValueError:
                 ui.default.warning("Remember the MFA device must be either y or n.")
 
+    def _get_force_classic(self, default_entry):
+        """Option to force the Okta Classic login process"""
+        ui.default.message(
+            "Do you want to force the Okta Classic login flow? (Okta Identity Engine domains only)\n"
+            "Please answer y or n.")
+        while True:
+            try:
+                return self._get_user_input_yes_no(
+                    "Force classic login flow", default_entry)
+            except ValueError:
+                ui.default.warning("Force Classic login flow must be either y or n.")
+    
+    def _get_open_browser(self, default_entry):
+        """Option to automatically open the default browser for OIE authentication"""
+        ui.default.message(
+            "Do you want to automatically open the default browser for authentication? (Okta Identity Engine domains only)\n"
+            "Please answer y or n.")
+        while True:
+            try:
+                return self._get_user_input_yes_no(
+                    "Open default browser automatically", default_entry)
+            except ValueError:
+                ui.default.warning("Open browser must be either y or n.")
+
     def _get_user_input(self, message, default=None):
         """formats message to include default and then prompts user for input
         via keyboard with message. Returns user's input or if user doesn't
         enter input will return the default."""
         if default and default != '':
             prompt_message = message + " [{}]: ".format(default)
         else:
```

### Comparing `gimme aws creds-2.6.1/gimme_aws_creds/default.py` & `gimme aws creds-2.7.0/gimme_aws_creds/default.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.1/gimme_aws_creds/duo.py` & `gimme aws creds-2.7.0/gimme_aws_creds/duo.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.1/gimme_aws_creds/errors.py` & `gimme aws creds-2.7.0/gimme_aws_creds/errors.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.1/gimme_aws_creds/main.py` & `gimme aws creds-2.7.0/gimme_aws_creds/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,77 +35,39 @@
 from .okta_classic import OktaClassicClient
 from .registered_authenticators import RegisteredAuthenticators
 
 
 class GimmeAWSCreds(object):
     """
        This is a CLI tool that gets temporary AWS credentials
-       from Okta based the available AWS Okta Apps and roles
-       assigned to the user. The user is able to select the app
-       and role from the CLI or specify them in a config file by
-       passing --action-configure to the CLI too.
-       gimme_aws_creds will either write the credentials to stdout
-       or ~/.aws/credentials depending on what was specified when
-       --action-configure was ran.
-
-       Usage:
-          -h, --help            show this help message and exit
-          --username USERNAME, -u USERNAME
-                                The username to use when logging into Okta. The
-                                username can also be set via the OKTA_USERNAME env
-                                variable. If not provided you will be prompted to
-                                enter a username.
-          --action-configure, -c       If set, will prompt user for configuration parameters
-                                and then exit.
-          --profile PROFILE, -p PROFILE
-                                If set, the specified configuration profile will be
-                                used instead of the default.
-          --resolve, -r         If set, performs alias resolution.
-          --insecure, -k        Allow connections to SSL sites without cert
-                                verification.
-          --mfa-code MFA_CODE   The MFA verification code to be used with SMS or TOTP
-                                authentication methods. If not provided you will be
-                                prompted to enter an MFA verification code.
-          --remember-device, -m
-                                The MFA device will be remembered by Okta service for
-                                a limited time, otherwise, you will be prompted for it
-                                every time.
-          --version             gimme-aws-creds version
-
-        Config Options:
-           okta_org_url = Okta URL
-           gimme_creds_server = URL of the gimme-creds-server
-           client_id = OAuth Client id for the gimme-creds-server
-           okta_auth_server = Server ID for the OAuth authorization server used by gimme-creds-server
-           write_aws_creds = Option to write creds to ~/.aws/credentials
-           cred_profile = Use DEFAULT or Role-based name as the profile in ~/.aws/credentials
-           aws_appname = (optional) Okta AWS App Name
-           aws_rolename =  (optional) AWS Role ARN. 'ALL' will retrieve all roles, can be a CSV for multiple roles.
-           okta_username = (optional) Okta User Name
+       from Okta based on the available AWS Okta Apps and roles
+       assigned to the user. 
     """
     resolver = DefaultResolver()
     envvar_list = [
         'AWS_DEFAULT_DURATION',
         'CLIENT_ID',
         'CRED_PROFILE',
         'GIMME_AWS_CREDS_CLIENT_ID',
         'GIMME_AWS_CREDS_CRED_PROFILE',
         'GIMME_AWS_CREDS_OUTPUT_FORMAT',
         'OKTA_AUTH_SERVER',
         'OKTA_DEVICE_TOKEN',
         'OKTA_MFA_CODE',
         'OKTA_PASSWORD',
         'OKTA_USERNAME',
+        'AWS_STS_REGION'
     ]
 
     envvar_conf_map = {
         'GIMME_AWS_CREDS_CLIENT_ID': 'client_id',
         'GIMME_AWS_CREDS_CRED_PROFILE': 'cred_profile',
         'GIMME_AWS_CREDS_OUTPUT_FORMAT': 'output_format',
         'OKTA_DEVICE_TOKEN': 'device_token',
+        'AWS_STS_REGION': 'aws_region'
     }
 
     def __init__(self, ui=ui.cli):
         """
         :type ui: ui.UserInterface
         """
         self.ui = ui
@@ -144,15 +106,15 @@
         config.set(profile, 'x_security_token_expires', expiration)
 
         # Write the updated config file
         with open(aws_config, 'w+') as configfile:
             config.write(configfile)
         # Update file permissions to secure  sensitive credentials file
         os.chmod(aws_config, 0o600)
-        self.ui.result('Written profile {} to {}'.format(profile, aws_config))
+        self.ui.message('Written profile {} to {}'.format(profile, aws_config))
 
     def write_aws_creds_from_data(self, data, aws_config=None):
         if not isinstance(data, dict):
             self.ui.warning('json line is not a dict! ' + repr(data))
             return
 
         aws_config = aws_config or data.get('shared_credentials_file')
@@ -182,15 +144,15 @@
 
         if errs:
             for error in errs:
                 self.ui.warning(error)
             return
 
         arn = data.get('role', {}).get('arn', '<no-arn>')
-        self.ui.result('Saving {} as {}'.format(arn, profile['name']))
+        self.ui.message('Saving {} as {}'.format(arn, profile['name']))
         self._write_aws_creds(
             profile['name'],
             credentials['aws_access_key_id'],
             credentials['aws_secret_access_key'],
             credentials['aws_session_token'],
             credentials['expiration'],
             aws_config=aws_config,
@@ -205,20 +167,24 @@
             return 'aws-cn'
         elif saml_acs_url == 'https://signin.amazonaws-us-gov.com/saml':
             return 'aws-us-gov'
         else:
             raise errors.GimmeAWSCredsError("{} is an unknown ACS URL".format(saml_acs_url))
 
     @staticmethod
-    def _get_sts_creds(partition, assertion, idp, role, duration=3600):
+    def _get_sts_creds(partition, region, assertion, idp, role, duration=3600):
         """ using the assertion and arns return aws sts creds """
 
-        # Use the first available region for partitions other than the public AWS
         session = boto3.session.Session(profile_name=None)
-        if partition != 'aws':
+
+        # If a region was passed, use that
+        if region is not None:
+            client = session.client('sts', region)
+        # Use the first available region for partitions other than the public AWS
+        elif partition != 'aws':
             regions = session.get_available_regions('sts', partition)
             client = session.client('sts', regions[0])
         else:
             client = session.client('sts')
 
         response = client.assume_role_with_saml(
             RoleArn=role,
@@ -522,20 +488,27 @@
         self._cache['okta_platform'] = okta_platform
     
     @property
     def okta_platform(self):
         if 'okta_platform' in self._cache:
             return self._cache['okta_platform']
         
+        # Treat this domain as classic, even if it's OIE
+        if self.config.force_classic == True or self.conf_dict.get('force_classic') == "True":
+            self.ui.message('Okta Classic login flow enabled')
+            self.set_okta_platform('classic')
+            return 'classic'
+        
         response = requests.get(
             self.okta_org_url + '/.well-known/okta-organization',
             headers={
                 'Accept': 'application/json',
                 'User-Agent': "gimme-aws-creds {}".format(version)
-            }
+            },
+            timeout=30
         )
 
         response_data = response.json()
 
         if response.status_code == 200:
             if response_data['pipeline'] == 'v1':
                 ret = 'classic'
@@ -622,15 +595,19 @@
     def set_auth_session(self, auth_session):
         self._cache['auth_session'] = auth_session
 
     @property
     def auth_session(self):
         if 'auth_session' in self._cache:
             return self._cache['auth_session']
-        auth_result = self.okta.auth_session(redirect_uri=self.conf_dict.get('app_url'), open_browser=self.config.open_browser)
+        if self.config.open_browser is True or self.conf_dict.get('open_browser') == "True":
+            open_browser = True
+        else:
+            open_browser = False
+        auth_result = self.okta.auth_session(redirect_uri=self.conf_dict.get('app_url'), open_browser=open_browser)
         self.set_auth_session(auth_result)
 
         return auth_result
 
     @property
     def aws_results(self):
         if 'aws_results' in self._cache:
@@ -675,14 +652,18 @@
                 self.okta.auth_oauth(
                     self.conf_dict['client_id'],
                     authorization_server=self.conf_dict['okta_auth_server'],
                     access_token=True,
                     id_token=False,
                     scopes=['openid']
                 )
+                
+                # auth_session isn't needed when using gimme_creds_lambda and Okta classic
+                self.set_auth_session(None)
+                
             elif self.okta_platform == 'identity_engine':
                 auth_result = self.auth_session
 
             # Add Access Tokens to Okta-protected requests
             self.okta.use_oauth_access_token(True)
 
             self.ui.info("Authentication Success! Calling Gimme-Creds Server...")
@@ -744,25 +725,27 @@
 
     def prepare_data(self, role, generate_credentials=False):
         aws_creds = {}
         if generate_credentials:
             try:
                 aws_creds = self._get_sts_creds(
                     self.aws_partition,
+                    self.conf_dict.get('aws_region'),
                     self.saml_data['SAMLResponse'],
                     role.idp,
                     role.role,
                     self.config.aws_default_duration,
                 )
             except ClientError as ex:
                 if 'requested DurationSeconds exceeds the MaxSessionDuration' in ex.response['Error']['Message']:
                     self.ui.warning(
                         "The requested session duration was too long for the role {}.  Falling back to 1 hour.".format(role.role))
                     aws_creds = self._get_sts_creds(
                         self.aws_partition,
+                        self.conf_dict.get('aws_region'),
                         self.saml_data['SAMLResponse'],
                         role.idp,
                         role.role,
                         3600,
                     )
                 else:
                     self.ui.error('Failed to generate credentials for {} due to {}'.format(role.role, ex))
@@ -846,17 +829,18 @@
 
     def _run(self):
         """ Pulling it all together to make the CLI """
         self.handle_action_configure()
         self.handle_action_list_profiles()
         if self.okta_platform == 'classic':
             self.handle_action_register_device()
-            self.handle_action_store_json_creds()
-            self.handle_action_list_roles()
             self.handle_setup_fido_authenticator()
+        self.handle_action_store_json_creds()
+        self.handle_action_list_roles()
+            
   
         # for each data item, if we have an override on output, prioritize that
         # if we do not, prioritize writing credentials to file if that is in our
         # configuration. If we are not writing to a credentials file, use whatever
         # is in the output format field (default to exports)
         for data in self.iter_selected_aws_credentials():
             if self.config.action_output_format:
@@ -928,15 +912,15 @@
                 self.ui.warning('error parsing json line {}'.format(repr(line)))
                 continue
             self.write_aws_creds_from_data(data)
         raise errors.GimmeAWSCredsExitSuccess()
 
     def handle_action_register_device(self):
         # Capture the Device Token and write it to the config file
-        if self.okta_platform == "classic" and ( self.device_token is None or self.config.action_register_device is True ):
+        if self.okta_platform == "classic" and ( not self.device_token or self.config.action_register_device is True ):
             if not self.config.action_register_device:
                 self.ui.notify('\n*** No device token found in configuration file, it will be created.')
                 self.ui.notify('*** You may be prompted for MFA more than once for this run.\n')
 
             auth_result = self.auth_session
             base_config = self.config.get_config_dict(include_inherits = False)
             base_config['device_token'] = auth_result['device_token']
```

### Comparing `gimme aws creds-2.6.1/gimme_aws_creds/okta_classic.py` & `gimme aws creds-2.7.0/gimme_aws_creds/okta_classic.py`

 * *Files 5% similar despite different names*

```diff
@@ -283,14 +283,21 @@
 
         response = self._http_client.post(
             self._okta_org_url + '/api/v1/authn',
             json={'stateToken': state_token},
             headers=self._get_headers(),
             verify=self._verify_ssl_certs
         )
+
+        # Passing the stateToken to the Authentication API for step-up auth doesn't work in OIE
+        if state_token is not None and response.status_code == 401:
+            raise errors.GimmeAWSCredsError(
+                "LOGIN ERROR: Step-up authetication is not supported when using the '--force_classic' parameter", 2
+            )
+
         response.raise_for_status()
         return {'stateToken': state_token, 'apiResponse': response.json()}
 
     def _next_login_step(self, state_token, login_data):
         """ decide what the next step in the login process is"""
         if 'errorCode' in login_data:
             raise errors.GimmeAWSCredsError(
@@ -385,14 +392,33 @@
         response_data = response.json()
 
         if 'stateToken' in response_data:
             return {'stateToken': response_data['stateToken'], 'apiResponse': response_data}
         if 'sessionToken' in response_data:
             return {'stateToken': None, 'sessionToken': response_data['sessionToken'], 'apiResponse': response_data}
 
+    def _login_send_email(self, state_token, factor):
+        """ Send email message for second factor authentication"""
+        response = self._http_client.post(
+            factor['_links']['verify']['href'],
+            params={'rememberDevice': self._remember_device},
+            json={'stateToken': state_token},
+            headers=self._get_headers(),
+            verify=self._verify_ssl_certs
+        )
+        response.raise_for_status()
+
+        self.ui.info("A verification code has been sent to " + factor['profile']['email'])
+        response_data = response.json()
+
+        if 'stateToken' in response_data:
+            return {'stateToken': response_data['stateToken'], 'apiResponse': response_data}
+        if 'sessionToken' in response_data:
+            return {'stateToken': None, 'sessionToken': response_data['sessionToken'], 'apiResponse': response_data}
+
     def _login_send_call(self, state_token, factor):
         """ Send Voice call for second factor authentication"""
         response = self._http_client.post(
             factor['_links']['verify']['href'],
             params={'rememberDevice': self._remember_device},
             json={'stateToken': state_token},
             headers=self._get_headers(),
@@ -550,14 +576,16 @@
         factor = self._choose_factor(login_data['_embedded']['factors'])
         if factor['provider'] == 'DUO':
             return self._login_duo_challenge(state_token, factor)
         elif factor['factorType'] == 'sms':
             return self._login_send_sms(state_token, factor)
         elif factor['factorType'] == 'call':
             return self._login_send_call(state_token, factor)
+        elif factor['factorType'] == 'email':
+            return self._login_send_email(state_token, factor)
         elif factor['factorType'] == 'token:software:totp':
             return self._login_input_mfa_challenge(state_token, factor['_links']['verify']['href'])
         elif factor['factorType'] == 'token':
             return self._login_input_mfa_challenge(state_token, factor['_links']['verify']['href'])
         elif factor['factorType'] == 'push':
             return self._login_send_push(state_token, factor)
         elif factor['factorType'] == 'u2f':
@@ -830,14 +858,16 @@
         """ Build the display name for a MFA factor based on the factor type"""
         if factor['provider'] == 'DUO':
             return factor['factorType'] + ": " + factor['provider'].capitalize()
         elif factor['factorType'] == 'push':
             return "Okta Verify App: " + factor['profile']['deviceType'] + ": " + factor['profile']['name']
         elif factor['factorType'] == 'sms':
             return factor['factorType'] + ": " + factor['profile']['phoneNumber']
+        elif factor['factorType'] == 'email':
+            return factor['factorType'] + ": " + factor['profile']['email']
         elif factor['factorType'] == 'call':
             return factor['factorType'] + ": " + factor['profile']['phoneNumber']
         elif factor['factorType'] == 'token:software:totp':
             return factor['factorType'] + "( " + factor['provider'] + " ) : " + factor['profile']['credentialId']
         elif factor['factorType'] == 'token':
             return factor['factorType'] + ": " + factor['profile']['credentialId']
         elif factor['factorType'] == 'u2f':
@@ -1027,55 +1057,20 @@
         if not factors:
             raise RuntimeError('Could not introspect factors')
 
         return factors
 
     @staticmethod
     def _extract_state_token_from_http_response(http_res):
-        saml_soup = BeautifulSoup(http_res.text, "html.parser")
-        
-        mfa_string = (
-            'Dodatečné ověření',
-            'Ekstra verificering',
-            'Zusätzliche Bestätigung',
-            'Πρόσθετη επαλήθευση',
-            'Extra Verification',
-            'Verificación adicional',
-            'Lisätodennus',
-            'Vérification supplémentaire',
-            'Extra ellenőrzés',
-            'Verifikasi Tambahan',
-            'Verifica aggiuntiva',
-            '追加認証',
-            '추가 확인',
-            'Penentusahan Tambahan',
-            'Ekstra verifisering',
-            'Extra verificatie',
-            'Dodatkowa weryfikacja',
-            'Verificação extra',
-            'Verificare suplimentară',
-            'Дополнительная проверка',
-            'Extra verifiering',
-            'การตรวจสอบพิเศษ',
-            'Ekstra Doğrulama',
-            'Додаткова верифікація',
-            'Xác minh bổ sung',
-            '额外验证',
-            '額外驗證'
-        )
-
-        if hasattr(saml_soup.title, 'string') and saml_soup.title.string.endswith(mfa_string):
-            # extract the stateToken from the Javascript code in the page and step up to MFA
-            # noinspection PyTypeChecker
-            state_token = decode(re.search(r"var stateToken = '(.*)';", http_res.text).group(1), "unicode-escape")
-            return state_token
+        # extract the stateToken from a javascript variable
+        state_token_re =  re.search(r"var stateToken = '(.*)';", http_res.text)
+        if state_token_re is not None:
+            return decode(state_token_re.group(1), "unicode-escape")
 
+        saml_soup = BeautifulSoup(http_res.text, "html.parser")
         for tag in saml_soup.find_all('body'):
-            # checking all the tags in body tag for Extra Verification string
-            if re.search(r"Extra Verification", tag.text, re.IGNORECASE):
-                # extract the stateToken from response (form action) instead of javascript variable
-                # noinspection PyTypeChecker
-                pre_state_token = decode(re.search(r"stateToken=(.*?[ \"])", http_res.text).group(1), "unicode-escape")
-                state_token = pre_state_token.rstrip('\"')
-                return state_token
-
-        return None
+            # extract the stateToken from response (form action) instead of javascript variable
+            # noinspection PyTypeChecker
+            state_token_re = re.search(r"stateToken=(.*?[ \"])", http_res.text)
+            if state_token_re is not None:
+                pre_state_token = decode(state_token_re.group(1), "unicode-escape")
+                return pre_state_token.rstrip('\"')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gimme aws creds-2.6.1/gimme_aws_creds/okta_identity_engine.py` & `gimme aws creds-2.7.0/gimme_aws_creds/okta_identity_engine.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.1/gimme_aws_creds/registered_authenticators.py` & `gimme aws creds-2.7.0/gimme_aws_creds/registered_authenticators.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.1/gimme_aws_creds/u2f.py` & `gimme aws creds-2.7.0/gimme_aws_creds/u2f.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.1/gimme_aws_creds/ui.py` & `gimme aws creds-2.7.0/gimme_aws_creds/ui.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.1/gimme_aws_creds/webauthn.py` & `gimme aws creds-2.7.0/gimme_aws_creds/webauthn.py`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.1/gimme_aws_creds.egg-info/PKG-INFO` & `gimme aws creds-2.7.0/gimme_aws_creds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimme-aws-creds
-Version: 2.6.1
+Version: 2.7.0
 Summary: A CLI to get temporary AWS credentials from Okta
 Home-page: https://github.com/Nike-Inc/gimme-aws-creds
 Author: Eric Pierce
 Author-email: eric.pierce@nike.com
 License: Apache License, v2.0
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `gimme aws creds-2.6.1/gimme_aws_creds.egg-info/SOURCES.txt` & `gimme aws creds-2.7.0/gimme_aws_creds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gimme aws creds-2.6.1/setup.py` & `gimme aws creds-2.7.0/setup.py`

 * *Files identical despite different names*

