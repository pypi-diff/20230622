# Comparing `tmp/matrix_sydent-2.5.3.tar.gz` & `tmp/matrix_sydent-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrix_sydent-2.5.3.tar", max compression
+gzip compressed data, was "matrix_sydent-2.5.4.tar", max compression
```

## Comparing `matrix_sydent-2.5.3.tar` & `matrix_sydent-2.5.4.tar`

### file list

```diff
@@ -1,134 +1,134 @@
--rw-r--r--   0        0        0    10174 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/LICENSE
--rw-r--r--   0        0        0     7202 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/README.rst
--rw-r--r--   0        0        0      431 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/matrix-sydent.service
--rw-r--r--   0        0        0        0 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/matrix_is_test/__init__.py
--rw-r--r--   0        0        0     3099 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/matrix_is_test/launcher.py
--rw-r--r--   0        0        0      231 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/matrix_is_test/res/is-test/invite_template.eml
--rw-r--r--   0        0        0      243 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/matrix_is_test/res/is-test/invite_template.eml.j2
--rw-r--r--   0        0        0       16 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/matrix_is_test/res/is-test/verification_template.eml
--rw-r--r--   0        0        0       18 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/matrix_is_test/res/is-test/verification_template.eml.j2
--rw-r--r--   0        0        0       43 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/matrix_is_test/res/is-test/verify_response_template.html
--rw-r--r--   0        0        0      581 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/matrix_is_test/terms.yaml
--rw-r--r--   0        0        0     3719 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/pyproject.toml
--rw-r--r--   0        0        0     5075 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/res/matrix-org/invite_template.eml
--rw-r--r--   0        0        0     5366 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/res/matrix-org/invite_template.eml.j2
--rw-r--r--   0        0        0     4648 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/res/matrix-org/migration_template.eml.j2
--rw-r--r--   0        0        0     2736 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/res/matrix-org/verification_template.eml
--rw-r--r--   0        0        0     2812 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/res/matrix-org/verification_template.eml.j2
--rw-r--r--   0        0        0      121 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/res/matrix-org/verify_response_template.html
--rw-r--r--   0        0        0     6303 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/res/vector-im/invite_template.eml
--rw-r--r--   0        0        0     6591 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/res/vector-im/invite_template.eml.j2
--rw-r--r--   0        0        0     5554 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/res/vector-im/migration_template.eml.j2
--rw-r--r--   0        0        0     5857 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/res/vector-im/verification_template.eml
--rw-r--r--   0        0        0     5923 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/res/vector-im/verification_template.eml.j2
--rw-r--r--   0        0        0      979 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/res/vector-im/verify_response_template.html
--rw-r--r--   0        0        0     5603 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/res/vector_verification_sample.txt
--rwxr-xr-x   0        0        0    15099 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/scripts/casefold_db.py
--rwxr-xr-x   0        0        0      601 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/scripts/generate-key
--rwxr-xr-x   0        0        0     1055 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/scripts/sydent-bind
--rwxr-xr-x   0        0        0     1903 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/scripts-dev/check_newsfragment.sh
--rwxr-xr-x   0        0        0      307 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/scripts-dev/lint.sh
--rw-r--r--   0        0        0      131 2023-03-02 18:46:00.430689 matrix_sydent-2.5.3/setup.cfg
--rw-r--r--   0        0        0        0 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/__init__.py
--rw-r--r--   0        0        0    10731 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/config/__init__.py
--rw-r--r--   0        0        0     1072 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/config/_base.py
--rw-r--r--   0        0        0     2713 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/config/crypto.py
--rw-r--r--   0        0        0      973 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/config/database.py
--rw-r--r--   0        0        0     4136 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/config/email.py
--rw-r--r--   0        0        0      633 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/config/exceptions.py
--rw-r--r--   0        0        0     4417 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/config/general.py
--rw-r--r--   0        0        0     2669 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/config/http.py
--rw-r--r--   0        0        0     3381 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/config/sms.py
--rw-r--r--   0        0        0        0 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/db/__init__.py
--rw-r--r--   0        0        0     3728 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/db/accounts.py
--rw-r--r--   0        0        0     5828 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/db/hashing_metadata.py
--rw-r--r--   0        0        0     5825 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/db/invite_tokens.py
--rw-r--r--   0        0        0     1495 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/db/invite_tokens.sql
--rw-r--r--   0        0        0     4949 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/db/peers.py
--rw-r--r--   0        0        0     1191 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/db/peers.sql
--rw-r--r--   0        0        0     9421 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/db/sqlitedb.py
--rw-r--r--   0        0        0     1997 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/db/terms.py
--rw-r--r--   0        0        0    17085 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/db/threepid_associations.py
--rw-r--r--   0        0        0     1428 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/db/threepid_associations.sql
--rw-r--r--   0        0        0     1130 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/db/threepid_validation.sql
--rw-r--r--   0        0        0     9570 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/db/valsession.py
--rw-r--r--   0        0        0        0 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/hs_federation/__init__.py
--rw-r--r--   0        0        0      714 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/hs_federation/types.py
--rw-r--r--   0        0        0    10338 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/hs_federation/verifier.py
--rw-r--r--   0        0        0        0 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/__init__.py
--rw-r--r--   0        0        0     2866 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/auth.py
--rw-r--r--   0        0        0     4893 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/blacklisting_reactor.py
--rw-r--r--   0        0        0     4003 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/federation_tls_options.py
--rw-r--r--   0        0        0     6991 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/httpclient.py
--rw-r--r--   0        0        0     7927 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/httpcommon.py
--rw-r--r--   0        0        0     3488 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/httpsclient.py
--rw-r--r--   0        0        0     9892 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/httpserver.py
--rw-r--r--   0        0        0    18071 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/matrixfederationagent.py
--rw-r--r--   0        0        0     9317 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/servlets/__init__.py
--rw-r--r--   0        0        0     1459 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/servlets/accountservlet.py
--rw-r--r--   0        0        0     1546 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/servlets/authenticated_bind_threepid_servlet.py
--rw-r--r--   0        0        0     1604 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/servlets/authenticated_unbind_threepid_servlet.py
--rw-r--r--   0        0        0     2571 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/servlets/blindlysignstuffservlet.py
--rw-r--r--   0        0        0     2222 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/servlets/bulklookupservlet.py
--rw-r--r--   0        0        0     1221 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/servlets/cors_servlet.py
--rw-r--r--   0        0        0     8454 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/servlets/emailservlet.py
--rw-r--r--   0        0        0     3072 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/servlets/getvalidated3pidservlet.py
--rw-r--r--   0        0        0     2026 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/servlets/hashdetailsservlet.py
--rw-r--r--   0        0        0     1720 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/servlets/logoutservlet.py
--rw-r--r--   0        0        0     3482 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/servlets/lookupservlet.py
--rw-r--r--   0        0        0     5726 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/servlets/lookupv2servlet.py
--rw-r--r--   0        0        0     9224 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/servlets/msisdnservlet.py
--rw-r--r--   0        0        0     2213 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/servlets/pubkeyservlets.py
--rw-r--r--   0        0        0     4560 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/servlets/registerservlet.py
--rw-r--r--   0        0        0     7168 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/servlets/replication.py
--rw-r--r--   0        0        0    10626 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/servlets/store_invite_servlet.py
--rw-r--r--   0        0        0     2712 2023-03-02 18:46:00.434689 matrix_sydent-2.5.3/sydent/http/servlets/termsservlet.py
--rw-r--r--   0        0        0     3582 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/http/servlets/threepidbindservlet.py
--rw-r--r--   0        0        0    10548 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/http/servlets/threepidunbindservlet.py
--rw-r--r--   0        0        0     1363 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/http/servlets/versions.py
--rw-r--r--   0        0        0     6278 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/http/srvresolver.py
--rw-r--r--   0        0        0        0 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/replication/__init__.py
--rw-r--r--   0        0        0    11503 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/replication/peer.py
--rw-r--r--   0        0        0     4703 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/replication/pusher.py
--rw-r--r--   0        0        0        0 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/sms/__init__.py
--rw-r--r--   0        0        0     5631 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/sms/openmarket.py
--rw-r--r--   0        0        0     1300 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/sms/types.py
--rw-r--r--   0        0        0    10439 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/sydent.py
--rw-r--r--   0        0        0        0 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/terms/__init__.py
--rw-r--r--   0        0        0     5221 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/terms/terms.py
--rw-r--r--   0        0        0     1857 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/threepid/__init__.py
--rw-r--r--   0        0        0     8133 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/threepid/bind.py
--rw-r--r--   0        0        0     1568 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/threepid/signer.py
--rw-r--r--   0        0        0      653 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/types.py
--rw-r--r--   0        0        0        0 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/users/__init__.py
--rw-r--r--   0        0        0     1144 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/users/accounts.py
--rw-r--r--   0        0        0     1477 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/users/tokens.py
--rw-r--r--   0        0        0     1110 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/util/__init__.py
--rw-r--r--   0        0        0     5476 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/util/emailutils.py
--rw-r--r--   0        0        0     1014 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/util/hash.py
--rw-r--r--   0        0        0     3601 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/util/ip_range.py
--rw-r--r--   0        0        0     3017 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/util/ratelimiter.py
--rw-r--r--   0        0        0     4109 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/util/stringutils.py
--rw-r--r--   0        0        0     1814 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/util/tokenutils.py
--rw-r--r--   0        0        0     4765 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/util/ttlcache.py
--rw-r--r--   0        0        0     1486 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/validators/__init__.py
--rw-r--r--   0        0        0     2358 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/validators/common.py
--rw-r--r--   0        0        0     5468 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/validators/emailvalidator.py
--rw-r--r--   0        0        0     5396 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/sydent/validators/msisdnvalidator.py
--rw-r--r--   0        0        0        0 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/tests/__init__.py
--rw-r--r--   0        0        0     2475 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/tests/test_auth.py
--rw-r--r--   0        0        0     7576 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/tests/test_blacklisting.py
--rw-r--r--   0        0        0    11783 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/tests/test_casefold_migration.py
--rw-r--r--   0        0        0     3167 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/tests/test_email.py
--rw-r--r--   0        0        0     7346 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/tests/test_invites.py
--rw-r--r--   0        0        0     8461 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/tests/test_jinja_templates.py
--rw-r--r--   0        0        0     4047 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/tests/test_msisdn.py
--rw-r--r--   0        0        0     2978 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/tests/test_ratelimiter.py
--rw-r--r--   0        0        0     4069 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/tests/test_register.py
--rw-r--r--   0        0        0     7473 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/tests/test_replication.py
--rw-r--r--   0        0        0      243 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/tests/test_start.py
--rw-r--r--   0        0        0     2137 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/tests/test_store_invite.py
--rw-r--r--   0        0        0     2524 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/tests/test_threepidunbind.py
--rw-r--r--   0        0        0     2004 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/tests/test_util.py
--rw-r--r--   0        0        0    10302 2023-03-02 18:46:00.438690 matrix_sydent-2.5.3/tests/utils.py
--rw-r--r--   0        0        0     8748 1970-01-01 00:00:00.000000 matrix_sydent-2.5.3/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/LICENSE
+-rw-r--r--   0        0        0     8216 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/README.rst
+-rw-r--r--   0        0        0      431 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/matrix-sydent.service
+-rw-r--r--   0        0        0        0 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/matrix_is_test/__init__.py
+-rw-r--r--   0        0        0     3099 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/matrix_is_test/launcher.py
+-rw-r--r--   0        0        0      231 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/matrix_is_test/res/is-test/invite_template.eml
+-rw-r--r--   0        0        0      243 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/matrix_is_test/res/is-test/invite_template.eml.j2
+-rw-r--r--   0        0        0       16 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/matrix_is_test/res/is-test/verification_template.eml
+-rw-r--r--   0        0        0       18 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/matrix_is_test/res/is-test/verification_template.eml.j2
+-rw-r--r--   0        0        0       43 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/matrix_is_test/res/is-test/verify_response_template.html
+-rw-r--r--   0        0        0      581 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/matrix_is_test/terms.yaml
+-rw-r--r--   0        0        0     3719 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/pyproject.toml
+-rw-r--r--   0        0        0     5075 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/matrix-org/invite_template.eml
+-rw-r--r--   0        0        0     5366 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/matrix-org/invite_template.eml.j2
+-rw-r--r--   0        0        0     4648 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/matrix-org/migration_template.eml.j2
+-rw-r--r--   0        0        0     2736 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/matrix-org/verification_template.eml
+-rw-r--r--   0        0        0     2812 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/matrix-org/verification_template.eml.j2
+-rw-r--r--   0        0        0      121 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/matrix-org/verify_response_template.html
+-rw-r--r--   0        0        0     6303 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/vector-im/invite_template.eml
+-rw-r--r--   0        0        0     6591 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/vector-im/invite_template.eml.j2
+-rw-r--r--   0        0        0     5554 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/vector-im/migration_template.eml.j2
+-rw-r--r--   0        0        0     5857 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/vector-im/verification_template.eml
+-rw-r--r--   0        0        0     5923 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/vector-im/verification_template.eml.j2
+-rw-r--r--   0        0        0      979 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/vector-im/verify_response_template.html
+-rw-r--r--   0        0        0     5603 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/vector_verification_sample.txt
+-rwxr-xr-x   0        0        0    15099 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/scripts/casefold_db.py
+-rwxr-xr-x   0        0        0      601 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/scripts/generate-key
+-rwxr-xr-x   0        0        0     1055 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/scripts/sydent-bind
+-rwxr-xr-x   0        0        0     1903 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/scripts-dev/check_newsfragment.sh
+-rwxr-xr-x   0        0        0      307 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/scripts-dev/lint.sh
+-rw-r--r--   0        0        0      131 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/setup.cfg
+-rw-r--r--   0        0        0        0 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/__init__.py
+-rw-r--r--   0        0        0    11200 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/config/__init__.py
+-rw-r--r--   0        0        0     1072 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/config/_base.py
+-rw-r--r--   0        0        0     2713 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/config/crypto.py
+-rw-r--r--   0        0        0      973 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/config/database.py
+-rw-r--r--   0        0        0     4136 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/config/email.py
+-rw-r--r--   0        0        0      633 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/config/exceptions.py
+-rw-r--r--   0        0        0     5180 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/config/general.py
+-rw-r--r--   0        0        0     2669 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/config/http.py
+-rw-r--r--   0        0        0     3381 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/config/sms.py
+-rw-r--r--   0        0        0        0 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/__init__.py
+-rw-r--r--   0        0        0     3728 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/accounts.py
+-rw-r--r--   0        0        0     5828 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/hashing_metadata.py
+-rw-r--r--   0        0        0     5825 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/invite_tokens.py
+-rw-r--r--   0        0        0     1495 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/invite_tokens.sql
+-rw-r--r--   0        0        0     4949 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/peers.py
+-rw-r--r--   0        0        0     1191 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/peers.sql
+-rw-r--r--   0        0        0     9421 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/sqlitedb.py
+-rw-r--r--   0        0        0     1997 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/terms.py
+-rw-r--r--   0        0        0    17085 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/threepid_associations.py
+-rw-r--r--   0        0        0     1428 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/threepid_associations.sql
+-rw-r--r--   0        0        0     1130 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/threepid_validation.sql
+-rw-r--r--   0        0        0     9570 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/valsession.py
+-rw-r--r--   0        0        0        0 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/hs_federation/__init__.py
+-rw-r--r--   0        0        0      714 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/hs_federation/types.py
+-rw-r--r--   0        0        0    10338 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/hs_federation/verifier.py
+-rw-r--r--   0        0        0        0 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/__init__.py
+-rw-r--r--   0        0        0     2866 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/auth.py
+-rw-r--r--   0        0        0     4893 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/blacklisting_reactor.py
+-rw-r--r--   0        0        0     4003 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/federation_tls_options.py
+-rw-r--r--   0        0        0     6991 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/httpclient.py
+-rw-r--r--   0        0        0     7927 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/httpcommon.py
+-rw-r--r--   0        0        0     3488 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/httpsclient.py
+-rw-r--r--   0        0        0    10025 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/httpserver.py
+-rw-r--r--   0        0        0    18071 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/matrixfederationagent.py
+-rw-r--r--   0        0        0     9317 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/__init__.py
+-rw-r--r--   0        0        0     1459 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/accountservlet.py
+-rw-r--r--   0        0        0     1546 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/authenticated_bind_threepid_servlet.py
+-rw-r--r--   0        0        0     1604 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/authenticated_unbind_threepid_servlet.py
+-rw-r--r--   0        0        0     2571 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/blindlysignstuffservlet.py
+-rw-r--r--   0        0        0     2222 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/bulklookupservlet.py
+-rw-r--r--   0        0        0     1221 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/cors_servlet.py
+-rw-r--r--   0        0        0     8454 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/emailservlet.py
+-rw-r--r--   0        0        0     3072 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/getvalidated3pidservlet.py
+-rw-r--r--   0        0        0     2026 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/hashdetailsservlet.py
+-rw-r--r--   0        0        0     1720 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/logoutservlet.py
+-rw-r--r--   0        0        0     3482 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/lookupservlet.py
+-rw-r--r--   0        0        0     5726 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/lookupv2servlet.py
+-rw-r--r--   0        0        0     9224 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/msisdnservlet.py
+-rw-r--r--   0        0        0     2213 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/pubkeyservlets.py
+-rw-r--r--   0        0        0     4934 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/registerservlet.py
+-rw-r--r--   0        0        0     7168 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/replication.py
+-rw-r--r--   0        0        0    10626 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/store_invite_servlet.py
+-rw-r--r--   0        0        0     2712 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/termsservlet.py
+-rw-r--r--   0        0        0     3582 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/threepidbindservlet.py
+-rw-r--r--   0        0        0    10548 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/threepidunbindservlet.py
+-rw-r--r--   0        0        0     1363 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/versions.py
+-rw-r--r--   0        0        0     6278 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/srvresolver.py
+-rw-r--r--   0        0        0        0 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/replication/__init__.py
+-rw-r--r--   0        0        0    11503 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/replication/peer.py
+-rw-r--r--   0        0        0     4703 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/replication/pusher.py
+-rw-r--r--   0        0        0        0 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/sms/__init__.py
+-rw-r--r--   0        0        0     5631 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/sms/openmarket.py
+-rw-r--r--   0        0        0     1300 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/sms/types.py
+-rw-r--r--   0        0        0    10439 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/sydent.py
+-rw-r--r--   0        0        0        0 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/terms/__init__.py
+-rw-r--r--   0        0        0     5221 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/terms/terms.py
+-rw-r--r--   0        0        0     1857 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/threepid/__init__.py
+-rw-r--r--   0        0        0     8133 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/threepid/bind.py
+-rw-r--r--   0        0        0     1568 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/threepid/signer.py
+-rw-r--r--   0        0        0      653 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/types.py
+-rw-r--r--   0        0        0        0 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/users/__init__.py
+-rw-r--r--   0        0        0     1144 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/users/accounts.py
+-rw-r--r--   0        0        0     1477 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/users/tokens.py
+-rw-r--r--   0        0        0     1110 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/util/__init__.py
+-rw-r--r--   0        0        0     5476 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/util/emailutils.py
+-rw-r--r--   0        0        0     1014 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/util/hash.py
+-rw-r--r--   0        0        0     3601 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/util/ip_range.py
+-rw-r--r--   0        0        0     3017 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/util/ratelimiter.py
+-rw-r--r--   0        0        0     4109 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/util/stringutils.py
+-rw-r--r--   0        0        0     1814 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/util/tokenutils.py
+-rw-r--r--   0        0        0     4765 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/util/ttlcache.py
+-rw-r--r--   0        0        0     1486 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/validators/__init__.py
+-rw-r--r--   0        0        0     2358 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/validators/common.py
+-rw-r--r--   0        0        0     5468 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/validators/emailvalidator.py
+-rw-r--r--   0        0        0     5396 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/validators/msisdnvalidator.py
+-rw-r--r--   0        0        0        0 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/__init__.py
+-rw-r--r--   0        0        0     2475 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_auth.py
+-rw-r--r--   0        0        0     7576 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_blacklisting.py
+-rw-r--r--   0        0        0    11783 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_casefold_migration.py
+-rw-r--r--   0        0        0     3167 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_email.py
+-rw-r--r--   0        0        0     7346 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_invites.py
+-rw-r--r--   0        0        0     8461 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_jinja_templates.py
+-rw-r--r--   0        0        0     4047 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_msisdn.py
+-rw-r--r--   0        0        0     2978 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_ratelimiter.py
+-rw-r--r--   0        0        0     5054 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_register.py
+-rw-r--r--   0        0        0     7473 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_replication.py
+-rw-r--r--   0        0        0      752 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_start.py
+-rw-r--r--   0        0        0     2137 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_store_invite.py
+-rw-r--r--   0        0        0     2524 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_threepidunbind.py
+-rw-r--r--   0        0        0     2004 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_util.py
+-rw-r--r--   0        0        0    10302 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/utils.py
+-rw-r--r--   0        0        0     9762 1970-01-01 00:00:00.000000 matrix_sydent-2.5.4/PKG-INFO
```

### Comparing `matrix_sydent-2.5.3/LICENSE` & `matrix_sydent-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/README.rst` & `matrix_sydent-2.5.4/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+What is Sydent?
+===============
+
+Sydent is an `identity server <https://spec.matrix.org/v1.6/identity-service-api/>`_ for the `Matrix communications protocol <matrix.org>`_. It allows Matrix users to prove that they own an email address or phone number, and allows _other_ Matrix users to look them up using that email address or phone number.
+
+Do I need to run Sydent to run my own homeserver?
+-------------------------------------------------
+
+Short answer: **no**.
+
+Medium answer: **probably not**. Most homeservers and clients use the Sydent
+instance run by `matrix.org`, or use no identity server whatsoever.
+
+Longer answer: if you want to allow user lookup via emails and phone numbers in
+a private federation of multiple homeservers, Sydent _might_ be useful for you.
+If you want your homeserver to be able to verify phone numbers via SMS and
+you have an API token for the `OpenMarket HTTP SMS API
+<https://www.openmarket.com/docs/Content/apis/v4http/overview.htm>`_, then
+Sydent might be useful for you.
+
+
 Installation
 ============
 
 Installing the system dependencies
 ----------------------------------
 
 To install Sydent's dependencies on a Debian-based system, run::
```

### Comparing `matrix_sydent-2.5.3/matrix_is_test/launcher.py` & `matrix_sydent-2.5.4/matrix_is_test/launcher.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/matrix_is_test/terms.yaml` & `matrix_sydent-2.5.4/matrix_is_test/terms.yaml`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/pyproject.toml` & `matrix_sydent-2.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     "signedjson.*",
     "sortedcontainers",
 ]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "matrix-sydent"
-version = "2.5.3"
+version = "2.5.4"
 description = "Reference Matrix Identity Verification and Lookup Server"
 authors = ["Matrix.org Team and Contributors <packages@matrix.org>"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://github.com/matrix-org/sydent"
 packages = [
     { include = "sydent" },
```

### Comparing `matrix_sydent-2.5.3/res/matrix-org/invite_template.eml` & `matrix_sydent-2.5.4/res/matrix-org/invite_template.eml`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/res/matrix-org/invite_template.eml.j2` & `matrix_sydent-2.5.4/res/matrix-org/invite_template.eml.j2`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/res/matrix-org/migration_template.eml.j2` & `matrix_sydent-2.5.4/res/matrix-org/migration_template.eml.j2`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/res/matrix-org/verification_template.eml` & `matrix_sydent-2.5.4/res/matrix-org/verification_template.eml`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/res/matrix-org/verification_template.eml.j2` & `matrix_sydent-2.5.4/res/matrix-org/verification_template.eml.j2`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/res/vector-im/invite_template.eml` & `matrix_sydent-2.5.4/res/vector-im/invite_template.eml`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/res/vector-im/invite_template.eml.j2` & `matrix_sydent-2.5.4/res/vector-im/invite_template.eml.j2`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/res/vector-im/migration_template.eml.j2` & `matrix_sydent-2.5.4/res/vector-im/migration_template.eml.j2`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/res/vector-im/verification_template.eml` & `matrix_sydent-2.5.4/res/vector-im/verification_template.eml`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/res/vector-im/verification_template.eml.j2` & `matrix_sydent-2.5.4/res/vector-im/verification_template.eml.j2`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/res/vector-im/verify_response_template.html` & `matrix_sydent-2.5.4/res/vector-im/verify_response_template.html`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/res/vector_verification_sample.txt` & `matrix_sydent-2.5.4/res/vector_verification_sample.txt`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/scripts/casefold_db.py` & `matrix_sydent-2.5.4/scripts/casefold_db.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/scripts/generate-key` & `matrix_sydent-2.5.4/scripts/generate-key`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/scripts/sydent-bind` & `matrix_sydent-2.5.4/scripts/sydent-bind`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/scripts-dev/check_newsfragment.sh` & `matrix_sydent-2.5.4/scripts-dev/check_newsfragment.sh`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/config/__init__.py` & `matrix_sydent-2.5.4/sydent/config/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,16 @@
         "brand.default": "matrix-org",
         # The following can be added to your local config file to enable prometheus
         # support.
         # 'prometheus_port': '8080',  # The port to serve metrics on
         # 'prometheus_addr': '',  # The address to bind to. Empty string means bind to all.
         # The following can be added to your local config file to enable sentry support.
         # 'sentry_dsn': 'https://...'  # The DSN has configured in the sentry instance project.
-        # Whether clients and homeservers can register an association using v1 endpoints.
+        # Whether clients and homeservers can register an association using v1 endpoints. This
+        # option is now deprecated and will be superceded by the option `enable_v1_access`
         "enable_v1_associations": "true",
         "delete_tokens_on_bind": "true",
         # Prevent outgoing requests from being sent to the following blacklisted
         # IP address CIDR ranges. If this option is not specified or empty then
         # it defaults to private IP address ranges.
         #
         # The blacklist applies to all outbound requests except replication
@@ -68,14 +69,20 @@
         # List of IP address CIDR ranges that should be allowed for outbound
         # requests. This is useful for specifying exceptions to wide-ranging
         # blacklisted target IP ranges.
         #
         # This whitelist overrides `ip.blacklist` and defaults to an empty
         # list.
         "ip.whitelist": "",
+        # A list of homeservers that are allowed to register with this identity server. Defaults to
+        # allowing all homeservers. If a list is specified, the config option `enable_v1_access` must be
+        # set to 'false'.
+        "homeserver_allow_list": "",
+        # If set to 'false', entirely disable access via the V1 api.
+        "enable_v1_access": "true",
     },
     "db": {
         "db.file": os.environ.get("SYDENT_DB_PATH", "sydent.db"),
     },
     "http": {
         "clientapi.http.bind_address": "::",
         "clientapi.http.port": "8090",
```

### Comparing `matrix_sydent-2.5.3/sydent/config/_base.py` & `matrix_sydent-2.5.4/sydent/config/_base.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/config/crypto.py` & `matrix_sydent-2.5.4/sydent/config/crypto.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/config/database.py` & `matrix_sydent-2.5.4/sydent/config/database.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/config/email.py` & `matrix_sydent-2.5.4/sydent/config/email.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/config/exceptions.py` & `matrix_sydent-2.5.4/sydent/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/config/general.py` & `matrix_sydent-2.5.4/sydent/config/general.py`

 * *Files 11% similar despite different names*

```diff
@@ -78,31 +78,47 @@
         self.prometheus_enabled = (
             self.prometheus_port is not None and self.prometheus_addr is not None
         )
 
         self.sentry_enabled = cfg.has_option("general", "sentry_dsn")
         self.sentry_dsn = cfg.get("general", "sentry_dsn", fallback=None)
 
-        self.enable_v1_associations = parse_cfg_bool(
-            cfg.get("general", "enable_v1_associations")
-        )
-
         self.delete_tokens_on_bind = parse_cfg_bool(
             cfg.get("general", "delete_tokens_on_bind")
         )
 
         ip_blacklist = list_from_comma_sep_string(cfg.get("general", "ip.blacklist"))
         if not ip_blacklist:
             ip_blacklist = DEFAULT_IP_RANGE_BLACKLIST
 
         ip_whitelist = list_from_comma_sep_string(cfg.get("general", "ip.whitelist"))
 
         self.ip_blacklist = generate_ip_set(ip_blacklist)
         self.ip_whitelist = generate_ip_set(ip_whitelist)
 
+        self.enable_v1_access = parse_cfg_bool(cfg.get("general", "enable_v1_access"))
+
+        homeserver_allow_list = list_from_comma_sep_string(
+            cfg.get("general", "homeserver_allow_list")
+        )
+        if homeserver_allow_list and self.enable_v1_access:
+            raise RuntimeError(
+                """The V1 api must be disabled for the `homeserver_allow_list` to function, if you have 
+                specified a `homeserver_allow_list` in the config file please ensure that the config 
+                option `enable_v1_access` is set to 'false'."""
+            )
+        self.homeserver_allow_list = homeserver_allow_list
+
+        if not self.enable_v1_access:
+            self.enable_v1_associations = False
+        else:
+            self.enable_v1_associations = parse_cfg_bool(
+                cfg.get("general", "enable_v1_associations")
+            )
+
         return False
 
 
 def list_from_comma_sep_string(rawstr: str) -> List[str]:
     """
     Parse the a comma seperated string into a list
```

### Comparing `matrix_sydent-2.5.3/sydent/config/http.py` & `matrix_sydent-2.5.4/sydent/config/http.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/config/sms.py` & `matrix_sydent-2.5.4/sydent/config/sms.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/db/accounts.py` & `matrix_sydent-2.5.4/sydent/db/accounts.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/db/hashing_metadata.py` & `matrix_sydent-2.5.4/sydent/db/hashing_metadata.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/db/invite_tokens.py` & `matrix_sydent-2.5.4/sydent/db/invite_tokens.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/db/invite_tokens.sql` & `matrix_sydent-2.5.4/sydent/db/invite_tokens.sql`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/db/peers.py` & `matrix_sydent-2.5.4/sydent/db/peers.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/db/peers.sql` & `matrix_sydent-2.5.4/sydent/db/peers.sql`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/db/sqlitedb.py` & `matrix_sydent-2.5.4/sydent/db/sqlitedb.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/db/terms.py` & `matrix_sydent-2.5.4/sydent/db/terms.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/db/threepid_associations.py` & `matrix_sydent-2.5.4/sydent/db/threepid_associations.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/db/threepid_associations.sql` & `matrix_sydent-2.5.4/sydent/db/threepid_associations.sql`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/db/threepid_validation.sql` & `matrix_sydent-2.5.4/sydent/db/threepid_validation.sql`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/db/valsession.py` & `matrix_sydent-2.5.4/sydent/db/valsession.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/hs_federation/types.py` & `matrix_sydent-2.5.4/sydent/hs_federation/types.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/hs_federation/verifier.py` & `matrix_sydent-2.5.4/sydent/hs_federation/verifier.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/auth.py` & `matrix_sydent-2.5.4/sydent/http/auth.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/blacklisting_reactor.py` & `matrix_sydent-2.5.4/sydent/http/blacklisting_reactor.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/federation_tls_options.py` & `matrix_sydent-2.5.4/sydent/http/federation_tls_options.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/httpclient.py` & `matrix_sydent-2.5.4/sydent/http/httpclient.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/httpcommon.py` & `matrix_sydent-2.5.4/sydent/http/httpcommon.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/httpsclient.py` & `matrix_sydent-2.5.4/sydent/http/httpsclient.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/httpserver.py` & `matrix_sydent-2.5.4/sydent/http/httpserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,74 +95,76 @@
         ephemeralPubkey = Resource()
 
         root.putChild(b"_matrix", matrix)
         matrix.putChild(b"identity", identity)
         identity.putChild(b"api", api)
         identity.putChild(b"v2", v2)
         identity.putChild(b"versions", VersionsServlet())
-        api.putChild(b"v1", v1)
 
-        validate.putChild(b"email", email)
-        validate.putChild(b"msisdn", msisdn)
-
-        validate_v2.putChild(b"email", email_v2)
-        validate_v2.putChild(b"msisdn", msisdn_v2)
-
-        v1.putChild(b"validate", validate)
-
-        v1.putChild(b"lookup", LookupServlet(sydent))
-        v1.putChild(b"bulk_lookup", BulkLookupServlet(sydent))
-
-        v1.putChild(b"pubkey", pubkey)
         pubkey.putChild(b"isvalid", PubkeyIsValidServlet(sydent))
         pubkey.putChild(b"ed25519:0", Ed25519Servlet(sydent))
         pubkey.putChild(b"ephemeral", ephemeralPubkey)
         ephemeralPubkey.putChild(b"isvalid", EphemeralPubkeyIsValidServlet(sydent))
 
-        threepid_v2.putChild(
-            b"getValidated3pid", GetValidated3pidServlet(sydent, require_auth=True)
-        )
-        threepid_v2.putChild(b"bind", ThreePidBindServlet(sydent, require_auth=True))
-        threepid_v2.putChild(b"unbind", unbind)
+        # v1
+        if self.sydent.config.general.enable_v1_access:
+            api.putChild(b"v1", v1)
+            validate.putChild(b"email", email)
+            validate.putChild(b"msisdn", msisdn)
+            v1.putChild(b"validate", validate)
+
+            v1.putChild(b"lookup", LookupServlet(sydent))
+            v1.putChild(b"bulk_lookup", BulkLookupServlet(sydent))
+
+            v1.putChild(b"pubkey", pubkey)
+
+            threepid_v1.putChild(b"getValidated3pid", GetValidated3pidServlet(sydent))
+            threepid_v1.putChild(b"unbind", unbind)
+            v1.putChild(b"3pid", threepid_v1)
+
+            email.putChild(b"requestToken", EmailRequestCodeServlet(sydent))
+            email.putChild(b"submitToken", EmailValidateCodeServlet(sydent))
+
+            msisdn.putChild(b"requestToken", MsisdnRequestCodeServlet(sydent))
+            msisdn.putChild(b"submitToken", MsisdnValidateCodeServlet(sydent))
+
+            v1.putChild(b"store-invite", StoreInviteServlet(sydent))
+
+            v1.putChild(b"sign-ed25519", BlindlySignStuffServlet(sydent))
 
-        threepid_v1.putChild(b"getValidated3pid", GetValidated3pidServlet(sydent))
-        threepid_v1.putChild(b"unbind", unbind)
         if self.sydent.config.general.enable_v1_associations:
             threepid_v1.putChild(b"bind", ThreePidBindServlet(sydent))
 
-        v1.putChild(b"3pid", threepid_v1)
+        # v2
+        # note v2 loses the /api so goes on 'identity' not 'api'
+        identity.putChild(b"v2", v2)
 
-        email.putChild(b"requestToken", EmailRequestCodeServlet(sydent))
-        email.putChild(b"submitToken", EmailValidateCodeServlet(sydent))
+        validate_v2.putChild(b"email", email_v2)
+        validate_v2.putChild(b"msisdn", msisdn_v2)
+
+        threepid_v2.putChild(
+            b"getValidated3pid", GetValidated3pidServlet(sydent, require_auth=True)
+        )
+        threepid_v2.putChild(b"bind", ThreePidBindServlet(sydent, require_auth=True))
+        threepid_v2.putChild(b"unbind", unbind)
 
         email_v2.putChild(
             b"requestToken", EmailRequestCodeServlet(sydent, require_auth=True)
         )
         email_v2.putChild(
             b"submitToken", EmailValidateCodeServlet(sydent, require_auth=True)
         )
 
-        msisdn.putChild(b"requestToken", MsisdnRequestCodeServlet(sydent))
-        msisdn.putChild(b"submitToken", MsisdnValidateCodeServlet(sydent))
-
         msisdn_v2.putChild(
             b"requestToken", MsisdnRequestCodeServlet(sydent, require_auth=True)
         )
         msisdn_v2.putChild(
             b"submitToken", MsisdnValidateCodeServlet(sydent, require_auth=True)
         )
 
-        v1.putChild(b"store-invite", StoreInviteServlet(sydent))
-
-        v1.putChild(b"sign-ed25519", BlindlySignStuffServlet(sydent))
-
-        # v2
-        # note v2 loses the /api so goes on 'identity' not 'api'
-        identity.putChild(b"v2", v2)
-
         # v2 exclusive APIs
         v2.putChild(b"terms", TermsServlet(sydent))
         account = AccountServlet(sydent)
         v2.putChild(b"account", account)
         account.putChild(b"register", RegisterServlet(sydent))
         account.putChild(b"logout", LogoutServlet(sydent))
```

### Comparing `matrix_sydent-2.5.3/sydent/http/matrixfederationagent.py` & `matrix_sydent-2.5.4/sydent/http/matrixfederationagent.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/__init__.py` & `matrix_sydent-2.5.4/sydent/http/servlets/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/accountservlet.py` & `matrix_sydent-2.5.4/sydent/http/servlets/accountservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/authenticated_bind_threepid_servlet.py` & `matrix_sydent-2.5.4/sydent/http/servlets/authenticated_bind_threepid_servlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/authenticated_unbind_threepid_servlet.py` & `matrix_sydent-2.5.4/sydent/http/servlets/authenticated_unbind_threepid_servlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/blindlysignstuffservlet.py` & `matrix_sydent-2.5.4/sydent/http/servlets/blindlysignstuffservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/bulklookupservlet.py` & `matrix_sydent-2.5.4/sydent/http/servlets/bulklookupservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/cors_servlet.py` & `matrix_sydent-2.5.4/sydent/http/servlets/cors_servlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/emailservlet.py` & `matrix_sydent-2.5.4/sydent/http/servlets/emailservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/getvalidated3pidservlet.py` & `matrix_sydent-2.5.4/sydent/http/servlets/getvalidated3pidservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/hashdetailsservlet.py` & `matrix_sydent-2.5.4/sydent/http/servlets/hashdetailsservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/logoutservlet.py` & `matrix_sydent-2.5.4/sydent/http/servlets/logoutservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/lookupservlet.py` & `matrix_sydent-2.5.4/sydent/http/servlets/lookupservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/lookupv2servlet.py` & `matrix_sydent-2.5.4/sydent/http/servlets/lookupv2servlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/msisdnservlet.py` & `matrix_sydent-2.5.4/sydent/http/servlets/msisdnservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/pubkeyservlets.py` & `matrix_sydent-2.5.4/sydent/http/servlets/pubkeyservlets.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/registerservlet.py` & `matrix_sydent-2.5.4/sydent/http/servlets/registerservlet.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,22 @@
         """
         send_cors(request)
 
         args = get_args(request, ("matrix_server_name", "access_token"))
 
         matrix_server = args["matrix_server_name"].lower()
 
+        if self.sydent.config.general.homeserver_allow_list:
+            if matrix_server not in self.sydent.config.general.homeserver_allow_list:
+                request.setResponseCode(403)
+                return {
+                    "errcode": "M_UNAUTHORIZED",
+                    "error": "This homeserver is not authorized to access this server.",
+                }
+
         if not is_valid_matrix_server_name(matrix_server):
             request.setResponseCode(400)
             return {
                 "errcode": "M_INVALID_PARAM",
                 "error": "matrix_server_name must be a valid Matrix server name (IP address or hostname)",
             }
```

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/replication.py` & `matrix_sydent-2.5.4/sydent/http/servlets/replication.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/store_invite_servlet.py` & `matrix_sydent-2.5.4/sydent/http/servlets/store_invite_servlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/termsservlet.py` & `matrix_sydent-2.5.4/sydent/http/servlets/termsservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/threepidbindservlet.py` & `matrix_sydent-2.5.4/sydent/http/servlets/threepidbindservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/threepidunbindservlet.py` & `matrix_sydent-2.5.4/sydent/http/servlets/threepidunbindservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/servlets/versions.py` & `matrix_sydent-2.5.4/sydent/http/servlets/versions.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/http/srvresolver.py` & `matrix_sydent-2.5.4/sydent/http/srvresolver.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/replication/peer.py` & `matrix_sydent-2.5.4/sydent/replication/peer.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/replication/pusher.py` & `matrix_sydent-2.5.4/sydent/replication/pusher.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/sms/openmarket.py` & `matrix_sydent-2.5.4/sydent/sms/openmarket.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/sms/types.py` & `matrix_sydent-2.5.4/sydent/sms/types.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/sydent.py` & `matrix_sydent-2.5.4/sydent/sydent.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/terms/terms.py` & `matrix_sydent-2.5.4/sydent/terms/terms.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/threepid/__init__.py` & `matrix_sydent-2.5.4/sydent/threepid/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/threepid/bind.py` & `matrix_sydent-2.5.4/sydent/threepid/bind.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/threepid/signer.py` & `matrix_sydent-2.5.4/sydent/threepid/signer.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/types.py` & `matrix_sydent-2.5.4/sydent/types.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/users/accounts.py` & `matrix_sydent-2.5.4/sydent/users/accounts.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/users/tokens.py` & `matrix_sydent-2.5.4/sydent/users/tokens.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/util/__init__.py` & `matrix_sydent-2.5.4/sydent/util/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/util/emailutils.py` & `matrix_sydent-2.5.4/sydent/util/emailutils.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/util/hash.py` & `matrix_sydent-2.5.4/sydent/util/hash.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/util/ip_range.py` & `matrix_sydent-2.5.4/sydent/util/ip_range.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/util/ratelimiter.py` & `matrix_sydent-2.5.4/sydent/util/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/util/stringutils.py` & `matrix_sydent-2.5.4/sydent/util/stringutils.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/util/tokenutils.py` & `matrix_sydent-2.5.4/sydent/util/tokenutils.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/util/ttlcache.py` & `matrix_sydent-2.5.4/sydent/util/ttlcache.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/validators/__init__.py` & `matrix_sydent-2.5.4/sydent/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/validators/common.py` & `matrix_sydent-2.5.4/sydent/validators/common.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/validators/emailvalidator.py` & `matrix_sydent-2.5.4/sydent/validators/emailvalidator.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/sydent/validators/msisdnvalidator.py` & `matrix_sydent-2.5.4/sydent/validators/msisdnvalidator.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/tests/test_auth.py` & `matrix_sydent-2.5.4/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/tests/test_blacklisting.py` & `matrix_sydent-2.5.4/tests/test_blacklisting.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/tests/test_casefold_migration.py` & `matrix_sydent-2.5.4/tests/test_casefold_migration.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/tests/test_email.py` & `matrix_sydent-2.5.4/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/tests/test_invites.py` & `matrix_sydent-2.5.4/tests/test_invites.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/tests/test_jinja_templates.py` & `matrix_sydent-2.5.4/tests/test_jinja_templates.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/tests/test_msisdn.py` & `matrix_sydent-2.5.4/tests/test_msisdn.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/tests/test_ratelimiter.py` & `matrix_sydent-2.5.4/tests/test_ratelimiter.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/tests/test_register.py` & `matrix_sydent-2.5.4/tests/test_register.py`

 * *Files 13% similar despite different names*

```diff
@@ -94,7 +94,34 @@
                 },
             )
         self.assertEqual(channel.code, HTTPStatus.INTERNAL_SERVER_ERROR)
         self.assertEqual(channel.json_body["errcode"], "M_UNKNOWN")
         # Check that we haven't just returned the generic error message in asyncjsonwrap
         self.assertNotEqual(channel.json_body["error"], "Internal Server Error")
         self.assertIn("JSON", channel.json_body["error"])
+
+
+class RegisterAllowListTestCase(unittest.TestCase):
+    """
+    Test registering works with the `homeserver_allow_list` config option specified
+    """
+
+    def test_registering_not_allowed_if_homeserver_not_in_allow_list(self) -> None:
+        config = {
+            "general": {
+                "homeserver_allow_list": "friendly.com, example.com",
+                "enable_v1_access": "false",
+            }
+        }
+        # Create a new sydent with a homeserver_allow_list specified
+        self.sydent = make_sydent(test_config=config)
+        self.sydent.run()
+
+        request, channel = make_request(
+            self.sydent.reactor,
+            self.sydent.clientApiHttpServer.factory,
+            "POST",
+            "/_matrix/identity/v2/account/register",
+            content={"matrix_server_name": "not.example.com", "access_token": "foo"},
+        )
+        self.assertEqual(channel.code, 403)
+        self.assertEqual(channel.json_body["errcode"], "M_UNAUTHORIZED")
```

### Comparing `matrix_sydent-2.5.3/tests/test_replication.py` & `matrix_sydent-2.5.4/tests/test_replication.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/tests/test_store_invite.py` & `matrix_sydent-2.5.4/tests/test_store_invite.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/tests/test_threepidunbind.py` & `matrix_sydent-2.5.4/tests/test_threepidunbind.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/tests/test_util.py` & `matrix_sydent-2.5.4/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/tests/utils.py` & `matrix_sydent-2.5.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.3/PKG-INFO` & `matrix_sydent-2.5.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrix-sydent
-Version: 2.5.3
+Version: 2.5.4
 Summary: Reference Matrix Identity Verification and Lookup Server
 Home-page: https://github.com/matrix-org/sydent
 License: Apache-2.0
 Author: Matrix.org Team and Contributors
 Author-email: packages@matrix.org
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -33,14 +33,35 @@
 Requires-Dist: twisted (>=18.4.0)
 Requires-Dist: typing-extensions (>=3.7.4)
 Requires-Dist: unpaddedbase64 (>=1.1.0)
 Requires-Dist: zope.interface (>=4.6.0)
 Project-URL: Repository, https://github.com/matrix-org/sydent
 Description-Content-Type: text/x-rst
 
+What is Sydent?
+===============
+
+Sydent is an `identity server <https://spec.matrix.org/v1.6/identity-service-api/>`_ for the `Matrix communications protocol <matrix.org>`_. It allows Matrix users to prove that they own an email address or phone number, and allows _other_ Matrix users to look them up using that email address or phone number.
+
+Do I need to run Sydent to run my own homeserver?
+-------------------------------------------------
+
+Short answer: **no**.
+
+Medium answer: **probably not**. Most homeservers and clients use the Sydent
+instance run by `matrix.org`, or use no identity server whatsoever.
+
+Longer answer: if you want to allow user lookup via emails and phone numbers in
+a private federation of multiple homeservers, Sydent _might_ be useful for you.
+If you want your homeserver to be able to verify phone numbers via SMS and
+you have an API token for the `OpenMarket HTTP SMS API
+<https://www.openmarket.com/docs/Content/apis/v4http/overview.htm>`_, then
+Sydent might be useful for you.
+
+
 Installation
 ============
 
 Installing the system dependencies
 ----------------------------------
 
 To install Sydent's dependencies on a Debian-based system, run::
```

