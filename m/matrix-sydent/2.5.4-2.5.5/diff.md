# Comparing `tmp/matrix_sydent-2.5.4.tar.gz` & `tmp/matrix_sydent-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matrix_sydent-2.5.4.tar", max compression
+gzip compressed data, was "matrix_sydent-2.5.5.tar", max compression
```

## Comparing `matrix_sydent-2.5.4.tar` & `matrix_sydent-2.5.5.tar`

### file list

```diff
@@ -1,134 +1,134 @@
--rw-r--r--   0        0        0    10174 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/LICENSE
--rw-r--r--   0        0        0     8216 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/README.rst
--rw-r--r--   0        0        0      431 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/matrix-sydent.service
--rw-r--r--   0        0        0        0 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/matrix_is_test/__init__.py
--rw-r--r--   0        0        0     3099 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/matrix_is_test/launcher.py
--rw-r--r--   0        0        0      231 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/matrix_is_test/res/is-test/invite_template.eml
--rw-r--r--   0        0        0      243 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/matrix_is_test/res/is-test/invite_template.eml.j2
--rw-r--r--   0        0        0       16 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/matrix_is_test/res/is-test/verification_template.eml
--rw-r--r--   0        0        0       18 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/matrix_is_test/res/is-test/verification_template.eml.j2
--rw-r--r--   0        0        0       43 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/matrix_is_test/res/is-test/verify_response_template.html
--rw-r--r--   0        0        0      581 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/matrix_is_test/terms.yaml
--rw-r--r--   0        0        0     3719 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/pyproject.toml
--rw-r--r--   0        0        0     5075 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/matrix-org/invite_template.eml
--rw-r--r--   0        0        0     5366 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/matrix-org/invite_template.eml.j2
--rw-r--r--   0        0        0     4648 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/matrix-org/migration_template.eml.j2
--rw-r--r--   0        0        0     2736 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/matrix-org/verification_template.eml
--rw-r--r--   0        0        0     2812 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/matrix-org/verification_template.eml.j2
--rw-r--r--   0        0        0      121 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/matrix-org/verify_response_template.html
--rw-r--r--   0        0        0     6303 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/vector-im/invite_template.eml
--rw-r--r--   0        0        0     6591 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/vector-im/invite_template.eml.j2
--rw-r--r--   0        0        0     5554 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/vector-im/migration_template.eml.j2
--rw-r--r--   0        0        0     5857 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/vector-im/verification_template.eml
--rw-r--r--   0        0        0     5923 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/vector-im/verification_template.eml.j2
--rw-r--r--   0        0        0      979 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/vector-im/verify_response_template.html
--rw-r--r--   0        0        0     5603 2023-06-22 13:25:07.837507 matrix_sydent-2.5.4/res/vector_verification_sample.txt
--rwxr-xr-x   0        0        0    15099 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/scripts/casefold_db.py
--rwxr-xr-x   0        0        0      601 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/scripts/generate-key
--rwxr-xr-x   0        0        0     1055 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/scripts/sydent-bind
--rwxr-xr-x   0        0        0     1903 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/scripts-dev/check_newsfragment.sh
--rwxr-xr-x   0        0        0      307 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/scripts-dev/lint.sh
--rw-r--r--   0        0        0      131 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/setup.cfg
--rw-r--r--   0        0        0        0 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/__init__.py
--rw-r--r--   0        0        0    11200 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/config/__init__.py
--rw-r--r--   0        0        0     1072 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/config/_base.py
--rw-r--r--   0        0        0     2713 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/config/crypto.py
--rw-r--r--   0        0        0      973 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/config/database.py
--rw-r--r--   0        0        0     4136 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/config/email.py
--rw-r--r--   0        0        0      633 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/config/exceptions.py
--rw-r--r--   0        0        0     5180 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/config/general.py
--rw-r--r--   0        0        0     2669 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/config/http.py
--rw-r--r--   0        0        0     3381 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/config/sms.py
--rw-r--r--   0        0        0        0 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/__init__.py
--rw-r--r--   0        0        0     3728 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/accounts.py
--rw-r--r--   0        0        0     5828 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/hashing_metadata.py
--rw-r--r--   0        0        0     5825 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/invite_tokens.py
--rw-r--r--   0        0        0     1495 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/invite_tokens.sql
--rw-r--r--   0        0        0     4949 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/peers.py
--rw-r--r--   0        0        0     1191 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/peers.sql
--rw-r--r--   0        0        0     9421 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/sqlitedb.py
--rw-r--r--   0        0        0     1997 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/terms.py
--rw-r--r--   0        0        0    17085 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/threepid_associations.py
--rw-r--r--   0        0        0     1428 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/threepid_associations.sql
--rw-r--r--   0        0        0     1130 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/threepid_validation.sql
--rw-r--r--   0        0        0     9570 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/db/valsession.py
--rw-r--r--   0        0        0        0 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/hs_federation/__init__.py
--rw-r--r--   0        0        0      714 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/hs_federation/types.py
--rw-r--r--   0        0        0    10338 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/hs_federation/verifier.py
--rw-r--r--   0        0        0        0 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/__init__.py
--rw-r--r--   0        0        0     2866 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/auth.py
--rw-r--r--   0        0        0     4893 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/blacklisting_reactor.py
--rw-r--r--   0        0        0     4003 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/federation_tls_options.py
--rw-r--r--   0        0        0     6991 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/httpclient.py
--rw-r--r--   0        0        0     7927 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/httpcommon.py
--rw-r--r--   0        0        0     3488 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/httpsclient.py
--rw-r--r--   0        0        0    10025 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/httpserver.py
--rw-r--r--   0        0        0    18071 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/matrixfederationagent.py
--rw-r--r--   0        0        0     9317 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/__init__.py
--rw-r--r--   0        0        0     1459 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/accountservlet.py
--rw-r--r--   0        0        0     1546 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/authenticated_bind_threepid_servlet.py
--rw-r--r--   0        0        0     1604 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/authenticated_unbind_threepid_servlet.py
--rw-r--r--   0        0        0     2571 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/blindlysignstuffservlet.py
--rw-r--r--   0        0        0     2222 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/bulklookupservlet.py
--rw-r--r--   0        0        0     1221 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/cors_servlet.py
--rw-r--r--   0        0        0     8454 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/emailservlet.py
--rw-r--r--   0        0        0     3072 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/getvalidated3pidservlet.py
--rw-r--r--   0        0        0     2026 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/hashdetailsservlet.py
--rw-r--r--   0        0        0     1720 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/logoutservlet.py
--rw-r--r--   0        0        0     3482 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/lookupservlet.py
--rw-r--r--   0        0        0     5726 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/lookupv2servlet.py
--rw-r--r--   0        0        0     9224 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/msisdnservlet.py
--rw-r--r--   0        0        0     2213 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/pubkeyservlets.py
--rw-r--r--   0        0        0     4934 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/registerservlet.py
--rw-r--r--   0        0        0     7168 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/replication.py
--rw-r--r--   0        0        0    10626 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/store_invite_servlet.py
--rw-r--r--   0        0        0     2712 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/termsservlet.py
--rw-r--r--   0        0        0     3582 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/threepidbindservlet.py
--rw-r--r--   0        0        0    10548 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/threepidunbindservlet.py
--rw-r--r--   0        0        0     1363 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/servlets/versions.py
--rw-r--r--   0        0        0     6278 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/http/srvresolver.py
--rw-r--r--   0        0        0        0 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/replication/__init__.py
--rw-r--r--   0        0        0    11503 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/replication/peer.py
--rw-r--r--   0        0        0     4703 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/replication/pusher.py
--rw-r--r--   0        0        0        0 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/sms/__init__.py
--rw-r--r--   0        0        0     5631 2023-06-22 13:25:07.841507 matrix_sydent-2.5.4/sydent/sms/openmarket.py
--rw-r--r--   0        0        0     1300 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/sms/types.py
--rw-r--r--   0        0        0    10439 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/sydent.py
--rw-r--r--   0        0        0        0 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/terms/__init__.py
--rw-r--r--   0        0        0     5221 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/terms/terms.py
--rw-r--r--   0        0        0     1857 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/threepid/__init__.py
--rw-r--r--   0        0        0     8133 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/threepid/bind.py
--rw-r--r--   0        0        0     1568 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/threepid/signer.py
--rw-r--r--   0        0        0      653 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/types.py
--rw-r--r--   0        0        0        0 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/users/__init__.py
--rw-r--r--   0        0        0     1144 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/users/accounts.py
--rw-r--r--   0        0        0     1477 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/users/tokens.py
--rw-r--r--   0        0        0     1110 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/util/__init__.py
--rw-r--r--   0        0        0     5476 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/util/emailutils.py
--rw-r--r--   0        0        0     1014 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/util/hash.py
--rw-r--r--   0        0        0     3601 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/util/ip_range.py
--rw-r--r--   0        0        0     3017 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/util/ratelimiter.py
--rw-r--r--   0        0        0     4109 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/util/stringutils.py
--rw-r--r--   0        0        0     1814 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/util/tokenutils.py
--rw-r--r--   0        0        0     4765 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/util/ttlcache.py
--rw-r--r--   0        0        0     1486 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/validators/__init__.py
--rw-r--r--   0        0        0     2358 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/validators/common.py
--rw-r--r--   0        0        0     5468 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/validators/emailvalidator.py
--rw-r--r--   0        0        0     5396 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/sydent/validators/msisdnvalidator.py
--rw-r--r--   0        0        0        0 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/__init__.py
--rw-r--r--   0        0        0     2475 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_auth.py
--rw-r--r--   0        0        0     7576 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_blacklisting.py
--rw-r--r--   0        0        0    11783 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_casefold_migration.py
--rw-r--r--   0        0        0     3167 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_email.py
--rw-r--r--   0        0        0     7346 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_invites.py
--rw-r--r--   0        0        0     8461 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_jinja_templates.py
--rw-r--r--   0        0        0     4047 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_msisdn.py
--rw-r--r--   0        0        0     2978 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_ratelimiter.py
--rw-r--r--   0        0        0     5054 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_register.py
--rw-r--r--   0        0        0     7473 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_replication.py
--rw-r--r--   0        0        0      752 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_start.py
--rw-r--r--   0        0        0     2137 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_store_invite.py
--rw-r--r--   0        0        0     2524 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_threepidunbind.py
--rw-r--r--   0        0        0     2004 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/test_util.py
--rw-r--r--   0        0        0    10302 2023-06-22 13:25:07.845507 matrix_sydent-2.5.4/tests/utils.py
--rw-r--r--   0        0        0     9762 1970-01-01 00:00:00.000000 matrix_sydent-2.5.4/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-06-22 14:11:59.284481 matrix_sydent-2.5.5/LICENSE
+-rw-r--r--   0        0        0     8216 2023-06-22 14:11:59.284481 matrix_sydent-2.5.5/README.rst
+-rw-r--r--   0        0        0      431 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/matrix-sydent.service
+-rw-r--r--   0        0        0        0 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/matrix_is_test/__init__.py
+-rw-r--r--   0        0        0     3099 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/matrix_is_test/launcher.py
+-rw-r--r--   0        0        0      231 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/matrix_is_test/res/is-test/invite_template.eml
+-rw-r--r--   0        0        0      243 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/matrix_is_test/res/is-test/invite_template.eml.j2
+-rw-r--r--   0        0        0       16 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/matrix_is_test/res/is-test/verification_template.eml
+-rw-r--r--   0        0        0       18 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/matrix_is_test/res/is-test/verification_template.eml.j2
+-rw-r--r--   0        0        0       43 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/matrix_is_test/res/is-test/verify_response_template.html
+-rw-r--r--   0        0        0      581 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/matrix_is_test/terms.yaml
+-rw-r--r--   0        0        0     3719 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/pyproject.toml
+-rw-r--r--   0        0        0     5075 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/res/matrix-org/invite_template.eml
+-rw-r--r--   0        0        0     5366 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/res/matrix-org/invite_template.eml.j2
+-rw-r--r--   0        0        0     4648 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/res/matrix-org/migration_template.eml.j2
+-rw-r--r--   0        0        0     2736 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/res/matrix-org/verification_template.eml
+-rw-r--r--   0        0        0     2812 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/res/matrix-org/verification_template.eml.j2
+-rw-r--r--   0        0        0      121 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/res/matrix-org/verify_response_template.html
+-rw-r--r--   0        0        0     6303 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/res/vector-im/invite_template.eml
+-rw-r--r--   0        0        0     6591 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/res/vector-im/invite_template.eml.j2
+-rw-r--r--   0        0        0     5554 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/res/vector-im/migration_template.eml.j2
+-rw-r--r--   0        0        0     5857 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/res/vector-im/verification_template.eml
+-rw-r--r--   0        0        0     5923 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/res/vector-im/verification_template.eml.j2
+-rw-r--r--   0        0        0      979 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/res/vector-im/verify_response_template.html
+-rw-r--r--   0        0        0     5603 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/res/vector_verification_sample.txt
+-rwxr-xr-x   0        0        0    15099 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/scripts/casefold_db.py
+-rwxr-xr-x   0        0        0      601 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/scripts/generate-key
+-rwxr-xr-x   0        0        0     1055 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/scripts/sydent-bind
+-rwxr-xr-x   0        0        0     1903 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/scripts-dev/check_newsfragment.sh
+-rwxr-xr-x   0        0        0      307 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/scripts-dev/lint.sh
+-rw-r--r--   0        0        0      131 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/setup.cfg
+-rw-r--r--   0        0        0        0 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/__init__.py
+-rw-r--r--   0        0        0    11200 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/config/__init__.py
+-rw-r--r--   0        0        0     1072 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/config/_base.py
+-rw-r--r--   0        0        0     2713 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/config/crypto.py
+-rw-r--r--   0        0        0      973 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/config/database.py
+-rw-r--r--   0        0        0     4136 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/config/email.py
+-rw-r--r--   0        0        0      633 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/config/exceptions.py
+-rw-r--r--   0        0        0     5180 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/config/general.py
+-rw-r--r--   0        0        0     2669 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/config/http.py
+-rw-r--r--   0        0        0     3381 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/config/sms.py
+-rw-r--r--   0        0        0        0 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/db/__init__.py
+-rw-r--r--   0        0        0     3728 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/db/accounts.py
+-rw-r--r--   0        0        0     5828 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/db/hashing_metadata.py
+-rw-r--r--   0        0        0     5825 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/db/invite_tokens.py
+-rw-r--r--   0        0        0     1495 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/db/invite_tokens.sql
+-rw-r--r--   0        0        0     4949 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/db/peers.py
+-rw-r--r--   0        0        0     1191 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/db/peers.sql
+-rw-r--r--   0        0        0     9421 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/db/sqlitedb.py
+-rw-r--r--   0        0        0     1997 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/db/terms.py
+-rw-r--r--   0        0        0    17085 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/db/threepid_associations.py
+-rw-r--r--   0        0        0     1428 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/db/threepid_associations.sql
+-rw-r--r--   0        0        0     1130 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/db/threepid_validation.sql
+-rw-r--r--   0        0        0     9570 2023-06-22 14:11:59.288481 matrix_sydent-2.5.5/sydent/db/valsession.py
+-rw-r--r--   0        0        0        0 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/hs_federation/__init__.py
+-rw-r--r--   0        0        0      714 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/hs_federation/types.py
+-rw-r--r--   0        0        0    10338 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/hs_federation/verifier.py
+-rw-r--r--   0        0        0        0 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/__init__.py
+-rw-r--r--   0        0        0     2866 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/auth.py
+-rw-r--r--   0        0        0     4893 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/blacklisting_reactor.py
+-rw-r--r--   0        0        0     4003 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/federation_tls_options.py
+-rw-r--r--   0        0        0     6991 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/httpclient.py
+-rw-r--r--   0        0        0     7927 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/httpcommon.py
+-rw-r--r--   0        0        0     3488 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/httpsclient.py
+-rw-r--r--   0        0        0    10025 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/httpserver.py
+-rw-r--r--   0        0        0    18071 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/matrixfederationagent.py
+-rw-r--r--   0        0        0     9317 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/__init__.py
+-rw-r--r--   0        0        0     1459 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/accountservlet.py
+-rw-r--r--   0        0        0     1546 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/authenticated_bind_threepid_servlet.py
+-rw-r--r--   0        0        0     1604 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/authenticated_unbind_threepid_servlet.py
+-rw-r--r--   0        0        0     2571 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/blindlysignstuffservlet.py
+-rw-r--r--   0        0        0     2222 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/bulklookupservlet.py
+-rw-r--r--   0        0        0     1221 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/cors_servlet.py
+-rw-r--r--   0        0        0     8454 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/emailservlet.py
+-rw-r--r--   0        0        0     3072 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/getvalidated3pidservlet.py
+-rw-r--r--   0        0        0     2026 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/hashdetailsservlet.py
+-rw-r--r--   0        0        0     1720 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/logoutservlet.py
+-rw-r--r--   0        0        0     3482 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/lookupservlet.py
+-rw-r--r--   0        0        0     5726 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/lookupv2servlet.py
+-rw-r--r--   0        0        0     9224 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/msisdnservlet.py
+-rw-r--r--   0        0        0     2213 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/pubkeyservlets.py
+-rw-r--r--   0        0        0     4934 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/registerservlet.py
+-rw-r--r--   0        0        0     7168 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/replication.py
+-rw-r--r--   0        0        0    10626 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/store_invite_servlet.py
+-rw-r--r--   0        0        0     2712 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/termsservlet.py
+-rw-r--r--   0        0        0     3582 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/threepidbindservlet.py
+-rw-r--r--   0        0        0    10548 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/threepidunbindservlet.py
+-rw-r--r--   0        0        0     1363 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/servlets/versions.py
+-rw-r--r--   0        0        0     6278 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/http/srvresolver.py
+-rw-r--r--   0        0        0        0 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/replication/__init__.py
+-rw-r--r--   0        0        0    11503 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/replication/peer.py
+-rw-r--r--   0        0        0     4703 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/replication/pusher.py
+-rw-r--r--   0        0        0        0 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/sms/__init__.py
+-rw-r--r--   0        0        0     5631 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/sms/openmarket.py
+-rw-r--r--   0        0        0     1300 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/sms/types.py
+-rw-r--r--   0        0        0    10439 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/sydent.py
+-rw-r--r--   0        0        0        0 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/terms/__init__.py
+-rw-r--r--   0        0        0     5221 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/terms/terms.py
+-rw-r--r--   0        0        0     1857 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/threepid/__init__.py
+-rw-r--r--   0        0        0     8133 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/threepid/bind.py
+-rw-r--r--   0        0        0     1568 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/threepid/signer.py
+-rw-r--r--   0        0        0      653 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/types.py
+-rw-r--r--   0        0        0        0 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/users/__init__.py
+-rw-r--r--   0        0        0     1144 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/users/accounts.py
+-rw-r--r--   0        0        0     1477 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/users/tokens.py
+-rw-r--r--   0        0        0     1110 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/util/__init__.py
+-rw-r--r--   0        0        0     5476 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/util/emailutils.py
+-rw-r--r--   0        0        0     1014 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/util/hash.py
+-rw-r--r--   0        0        0     3601 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/util/ip_range.py
+-rw-r--r--   0        0        0     3017 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/util/ratelimiter.py
+-rw-r--r--   0        0        0     4109 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/util/stringutils.py
+-rw-r--r--   0        0        0     1814 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/util/tokenutils.py
+-rw-r--r--   0        0        0     4765 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/util/ttlcache.py
+-rw-r--r--   0        0        0     1486 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/validators/__init__.py
+-rw-r--r--   0        0        0     2358 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/validators/common.py
+-rw-r--r--   0        0        0     5468 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/validators/emailvalidator.py
+-rw-r--r--   0        0        0     5396 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/sydent/validators/msisdnvalidator.py
+-rw-r--r--   0        0        0        0 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/tests/__init__.py
+-rw-r--r--   0        0        0     2475 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/tests/test_auth.py
+-rw-r--r--   0        0        0     7576 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/tests/test_blacklisting.py
+-rw-r--r--   0        0        0    11783 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/tests/test_casefold_migration.py
+-rw-r--r--   0        0        0     3167 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/tests/test_email.py
+-rw-r--r--   0        0        0     7346 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/tests/test_invites.py
+-rw-r--r--   0        0        0     8461 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/tests/test_jinja_templates.py
+-rw-r--r--   0        0        0     4047 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/tests/test_msisdn.py
+-rw-r--r--   0        0        0     2978 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/tests/test_ratelimiter.py
+-rw-r--r--   0        0        0     5054 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/tests/test_register.py
+-rw-r--r--   0        0        0     7473 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/tests/test_replication.py
+-rw-r--r--   0        0        0      752 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/tests/test_start.py
+-rw-r--r--   0        0        0     2137 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/tests/test_store_invite.py
+-rw-r--r--   0        0        0     2524 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/tests/test_threepidunbind.py
+-rw-r--r--   0        0        0     2004 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/tests/test_util.py
+-rw-r--r--   0        0        0    10302 2023-06-22 14:11:59.292482 matrix_sydent-2.5.5/tests/utils.py
+-rw-r--r--   0        0        0     9762 1970-01-01 00:00:00.000000 matrix_sydent-2.5.5/PKG-INFO
```

### Comparing `matrix_sydent-2.5.4/LICENSE` & `matrix_sydent-2.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/README.rst` & `matrix_sydent-2.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/matrix_is_test/launcher.py` & `matrix_sydent-2.5.5/matrix_is_test/launcher.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/matrix_is_test/terms.yaml` & `matrix_sydent-2.5.5/matrix_is_test/terms.yaml`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/pyproject.toml` & `matrix_sydent-2.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     "signedjson.*",
     "sortedcontainers",
 ]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "matrix-sydent"
-version = "2.5.4"
+version = "2.5.5"
 description = "Reference Matrix Identity Verification and Lookup Server"
 authors = ["Matrix.org Team and Contributors <packages@matrix.org>"]
 license = "Apache-2.0"
 readme = "README.rst"
 repository = "https://github.com/matrix-org/sydent"
 packages = [
     { include = "sydent" },
```

### Comparing `matrix_sydent-2.5.4/res/matrix-org/invite_template.eml` & `matrix_sydent-2.5.5/res/matrix-org/invite_template.eml`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/res/matrix-org/invite_template.eml.j2` & `matrix_sydent-2.5.5/res/matrix-org/invite_template.eml.j2`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/res/matrix-org/migration_template.eml.j2` & `matrix_sydent-2.5.5/res/matrix-org/migration_template.eml.j2`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/res/matrix-org/verification_template.eml` & `matrix_sydent-2.5.5/res/matrix-org/verification_template.eml`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/res/matrix-org/verification_template.eml.j2` & `matrix_sydent-2.5.5/res/matrix-org/verification_template.eml.j2`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/res/vector-im/invite_template.eml` & `matrix_sydent-2.5.5/res/vector-im/invite_template.eml`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/res/vector-im/invite_template.eml.j2` & `matrix_sydent-2.5.5/res/vector-im/invite_template.eml.j2`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/res/vector-im/migration_template.eml.j2` & `matrix_sydent-2.5.5/res/vector-im/migration_template.eml.j2`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/res/vector-im/verification_template.eml` & `matrix_sydent-2.5.5/res/vector-im/verification_template.eml`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/res/vector-im/verification_template.eml.j2` & `matrix_sydent-2.5.5/res/vector-im/verification_template.eml.j2`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/res/vector-im/verify_response_template.html` & `matrix_sydent-2.5.5/res/vector-im/verify_response_template.html`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/res/vector_verification_sample.txt` & `matrix_sydent-2.5.5/res/vector_verification_sample.txt`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/scripts/casefold_db.py` & `matrix_sydent-2.5.5/scripts/casefold_db.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/scripts/generate-key` & `matrix_sydent-2.5.5/scripts/generate-key`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/scripts/sydent-bind` & `matrix_sydent-2.5.5/scripts/sydent-bind`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/scripts-dev/check_newsfragment.sh` & `matrix_sydent-2.5.5/scripts-dev/check_newsfragment.sh`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/config/__init__.py` & `matrix_sydent-2.5.5/sydent/config/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/config/_base.py` & `matrix_sydent-2.5.5/sydent/config/_base.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/config/crypto.py` & `matrix_sydent-2.5.5/sydent/config/crypto.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/config/database.py` & `matrix_sydent-2.5.5/sydent/config/database.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/config/email.py` & `matrix_sydent-2.5.5/sydent/config/email.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/config/exceptions.py` & `matrix_sydent-2.5.5/sydent/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/config/general.py` & `matrix_sydent-2.5.5/sydent/config/general.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/config/http.py` & `matrix_sydent-2.5.5/sydent/config/http.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/config/sms.py` & `matrix_sydent-2.5.5/sydent/config/sms.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/db/accounts.py` & `matrix_sydent-2.5.5/sydent/db/accounts.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/db/hashing_metadata.py` & `matrix_sydent-2.5.5/sydent/db/hashing_metadata.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/db/invite_tokens.py` & `matrix_sydent-2.5.5/sydent/db/invite_tokens.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/db/invite_tokens.sql` & `matrix_sydent-2.5.5/sydent/db/invite_tokens.sql`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/db/peers.py` & `matrix_sydent-2.5.5/sydent/db/peers.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/db/peers.sql` & `matrix_sydent-2.5.5/sydent/db/peers.sql`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/db/sqlitedb.py` & `matrix_sydent-2.5.5/sydent/db/sqlitedb.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/db/terms.py` & `matrix_sydent-2.5.5/sydent/db/terms.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/db/threepid_associations.py` & `matrix_sydent-2.5.5/sydent/db/threepid_associations.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/db/threepid_associations.sql` & `matrix_sydent-2.5.5/sydent/db/threepid_associations.sql`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/db/threepid_validation.sql` & `matrix_sydent-2.5.5/sydent/db/threepid_validation.sql`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/db/valsession.py` & `matrix_sydent-2.5.5/sydent/db/valsession.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/hs_federation/types.py` & `matrix_sydent-2.5.5/sydent/hs_federation/types.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/hs_federation/verifier.py` & `matrix_sydent-2.5.5/sydent/hs_federation/verifier.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/auth.py` & `matrix_sydent-2.5.5/sydent/http/auth.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/blacklisting_reactor.py` & `matrix_sydent-2.5.5/sydent/http/blacklisting_reactor.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/federation_tls_options.py` & `matrix_sydent-2.5.5/sydent/http/federation_tls_options.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/httpclient.py` & `matrix_sydent-2.5.5/sydent/http/httpclient.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/httpcommon.py` & `matrix_sydent-2.5.5/sydent/http/httpcommon.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/httpsclient.py` & `matrix_sydent-2.5.5/sydent/http/httpsclient.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/httpserver.py` & `matrix_sydent-2.5.5/sydent/http/httpserver.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/matrixfederationagent.py` & `matrix_sydent-2.5.5/sydent/http/matrixfederationagent.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/__init__.py` & `matrix_sydent-2.5.5/sydent/http/servlets/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/accountservlet.py` & `matrix_sydent-2.5.5/sydent/http/servlets/accountservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/authenticated_bind_threepid_servlet.py` & `matrix_sydent-2.5.5/sydent/http/servlets/authenticated_bind_threepid_servlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/authenticated_unbind_threepid_servlet.py` & `matrix_sydent-2.5.5/sydent/http/servlets/authenticated_unbind_threepid_servlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/blindlysignstuffservlet.py` & `matrix_sydent-2.5.5/sydent/http/servlets/blindlysignstuffservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/bulklookupservlet.py` & `matrix_sydent-2.5.5/sydent/http/servlets/bulklookupservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/cors_servlet.py` & `matrix_sydent-2.5.5/sydent/http/servlets/cors_servlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/emailservlet.py` & `matrix_sydent-2.5.5/sydent/http/servlets/emailservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/getvalidated3pidservlet.py` & `matrix_sydent-2.5.5/sydent/http/servlets/getvalidated3pidservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/hashdetailsservlet.py` & `matrix_sydent-2.5.5/sydent/http/servlets/hashdetailsservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/logoutservlet.py` & `matrix_sydent-2.5.5/sydent/http/servlets/logoutservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/lookupservlet.py` & `matrix_sydent-2.5.5/sydent/http/servlets/lookupservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/lookupv2servlet.py` & `matrix_sydent-2.5.5/sydent/http/servlets/lookupv2servlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/msisdnservlet.py` & `matrix_sydent-2.5.5/sydent/http/servlets/msisdnservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/pubkeyservlets.py` & `matrix_sydent-2.5.5/sydent/http/servlets/pubkeyservlets.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/registerservlet.py` & `matrix_sydent-2.5.5/sydent/http/servlets/registerservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/replication.py` & `matrix_sydent-2.5.5/sydent/http/servlets/replication.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/store_invite_servlet.py` & `matrix_sydent-2.5.5/sydent/http/servlets/store_invite_servlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/termsservlet.py` & `matrix_sydent-2.5.5/sydent/http/servlets/termsservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/threepidbindservlet.py` & `matrix_sydent-2.5.5/sydent/http/servlets/threepidbindservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/threepidunbindservlet.py` & `matrix_sydent-2.5.5/sydent/http/servlets/threepidunbindservlet.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/servlets/versions.py` & `matrix_sydent-2.5.5/sydent/http/servlets/versions.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/http/srvresolver.py` & `matrix_sydent-2.5.5/sydent/http/srvresolver.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/replication/peer.py` & `matrix_sydent-2.5.5/sydent/replication/peer.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/replication/pusher.py` & `matrix_sydent-2.5.5/sydent/replication/pusher.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/sms/openmarket.py` & `matrix_sydent-2.5.5/sydent/sms/openmarket.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/sms/types.py` & `matrix_sydent-2.5.5/sydent/sms/types.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/sydent.py` & `matrix_sydent-2.5.5/sydent/sydent.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/terms/terms.py` & `matrix_sydent-2.5.5/sydent/terms/terms.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/threepid/__init__.py` & `matrix_sydent-2.5.5/sydent/threepid/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/threepid/bind.py` & `matrix_sydent-2.5.5/sydent/threepid/bind.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/threepid/signer.py` & `matrix_sydent-2.5.5/sydent/threepid/signer.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/types.py` & `matrix_sydent-2.5.5/sydent/types.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/users/accounts.py` & `matrix_sydent-2.5.5/sydent/users/accounts.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/users/tokens.py` & `matrix_sydent-2.5.5/sydent/users/tokens.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/util/__init__.py` & `matrix_sydent-2.5.5/sydent/util/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/util/emailutils.py` & `matrix_sydent-2.5.5/sydent/util/emailutils.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/util/hash.py` & `matrix_sydent-2.5.5/sydent/util/hash.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/util/ip_range.py` & `matrix_sydent-2.5.5/sydent/util/ip_range.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/util/ratelimiter.py` & `matrix_sydent-2.5.5/sydent/util/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/util/stringutils.py` & `matrix_sydent-2.5.5/sydent/util/stringutils.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/util/tokenutils.py` & `matrix_sydent-2.5.5/sydent/util/tokenutils.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/util/ttlcache.py` & `matrix_sydent-2.5.5/sydent/util/ttlcache.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/validators/__init__.py` & `matrix_sydent-2.5.5/sydent/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/validators/common.py` & `matrix_sydent-2.5.5/sydent/validators/common.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/validators/emailvalidator.py` & `matrix_sydent-2.5.5/sydent/validators/emailvalidator.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/sydent/validators/msisdnvalidator.py` & `matrix_sydent-2.5.5/sydent/validators/msisdnvalidator.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/tests/test_auth.py` & `matrix_sydent-2.5.5/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/tests/test_blacklisting.py` & `matrix_sydent-2.5.5/tests/test_blacklisting.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/tests/test_casefold_migration.py` & `matrix_sydent-2.5.5/tests/test_casefold_migration.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/tests/test_email.py` & `matrix_sydent-2.5.5/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/tests/test_invites.py` & `matrix_sydent-2.5.5/tests/test_invites.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/tests/test_jinja_templates.py` & `matrix_sydent-2.5.5/tests/test_jinja_templates.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/tests/test_msisdn.py` & `matrix_sydent-2.5.5/tests/test_msisdn.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/tests/test_ratelimiter.py` & `matrix_sydent-2.5.5/tests/test_ratelimiter.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/tests/test_register.py` & `matrix_sydent-2.5.5/tests/test_register.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/tests/test_replication.py` & `matrix_sydent-2.5.5/tests/test_replication.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/tests/test_start.py` & `matrix_sydent-2.5.5/tests/test_start.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/tests/test_store_invite.py` & `matrix_sydent-2.5.5/tests/test_store_invite.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/tests/test_threepidunbind.py` & `matrix_sydent-2.5.5/tests/test_threepidunbind.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/tests/test_util.py` & `matrix_sydent-2.5.5/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/tests/utils.py` & `matrix_sydent-2.5.5/tests/utils.py`

 * *Files identical despite different names*

### Comparing `matrix_sydent-2.5.4/PKG-INFO` & `matrix_sydent-2.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matrix-sydent
-Version: 2.5.4
+Version: 2.5.5
 Summary: Reference Matrix Identity Verification and Lookup Server
 Home-page: https://github.com/matrix-org/sydent
 License: Apache-2.0
 Author: Matrix.org Team and Contributors
 Author-email: packages@matrix.org
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

