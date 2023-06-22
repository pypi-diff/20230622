# Comparing `tmp/followthemoney-3.4.0.tar.gz` & `tmp/followthemoney-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "followthemoney-3.4.0.tar", last modified: Tue May 23 06:19:57 2023, max compression
+gzip compressed data, was "followthemoney-3.4.1.tar", last modified: Thu Jun 22 12:06:23 2023, max compression
```

## Comparing `followthemoney-3.4.0.tar` & `followthemoney-3.4.1.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.251635 followthemoney-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-23 06:18:02.000000 followthemoney-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-23 06:18:02.000000 followthemoney-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-23 06:19:57.251635 followthemoney-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-23 06:18:02.000000 followthemoney-3.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.235635 followthemoney-3.4.0/followthemoney/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.235635 followthemoney-3.4.0/followthemoney/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/cli/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/cli/exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/cli/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/cli/sieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.235635 followthemoney-3.4.0/followthemoney/export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/export/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/export/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/export/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/export/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/export/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/export/rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.235635 followthemoney-3.4.0/followthemoney/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/mapping/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/mapping/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/mapping/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/mapping/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/mapping/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/mapping/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/offshore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/property.py
--rw-r--r--   0 runner    (1001) docker     (123)    19523 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/rdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.243635 followthemoney-3.4.0/followthemoney/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Address.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Airplane.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Analyzable.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Article.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Assessment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Asset.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Associate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Audio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/BankAccount.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Call.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/CallForTenders.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Company.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Contract.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/ContractAward.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/CourtCase.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/CourtCaseParty.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/CryptoWallet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Debt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Directorship.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Document.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/EconomicActivity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Email.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Employment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Event.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Family.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Folder.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/HyperText.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Identification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Image.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Interest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Interval.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/LegalEntity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/License.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Membership.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Mention.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Message.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Note.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Organization.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Ownership.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Package.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Page.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Pages.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Passport.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Payment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Person.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/PlainText.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Post.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Project.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/ProjectParticipant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/PublicBody.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/RealEstate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Representation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Sanction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Security.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Similar.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Succession.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Table.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/TaxRoll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Thing.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Trip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/UnknownLink.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/UserAccount.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Value.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Vehicle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Vessel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Video.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Workbook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.243635 followthemoney-3.4.0/followthemoney/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.231635 followthemoney-3.4.0/followthemoney/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.243635 followthemoney-3.4.0/followthemoney/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    39021 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   110484 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.231635 followthemoney-3.4.0/followthemoney/translations/bs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.243635 followthemoney-3.4.0/followthemoney/translations/bs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    93147 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.231635 followthemoney-3.4.0/followthemoney/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.243635 followthemoney-3.4.0/followthemoney/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    36742 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   105691 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.231635 followthemoney-3.4.0/followthemoney/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.247635 followthemoney-3.4.0/followthemoney/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    32360 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   104328 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.247635 followthemoney-3.4.0/followthemoney/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.247635 followthemoney-3.4.0/followthemoney/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    43316 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   109418 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (123)   106802 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/fr/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (123)    99827 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.231635 followthemoney-3.4.0/followthemoney/translations/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.247635 followthemoney-3.4.0/followthemoney/translations/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/nb/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    89796 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.231635 followthemoney-3.4.0/followthemoney/translations/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.247635 followthemoney-3.4.0/followthemoney/translations/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/nl/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    90876 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.231635 followthemoney-3.4.0/followthemoney/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.247635 followthemoney-3.4.0/followthemoney/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    89847 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.247635 followthemoney-3.4.0/followthemoney/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.247635 followthemoney-3.4.0/followthemoney/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    61028 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   131500 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (123)   130621 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/ru/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.231635 followthemoney-3.4.0/followthemoney/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.247635 followthemoney-3.4.0/followthemoney/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/tr/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    89829 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.251635 followthemoney-3.4.0/followthemoney/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/address.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/country.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/gender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/iban.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/mimetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/phone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.235635 followthemoney-3.4.0/followthemoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-23 06:19:57.000000 followthemoney-3.4.0/followthemoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-23 06:19:57.000000 followthemoney-3.4.0/followthemoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:19:57.000000 followthemoney-3.4.0/followthemoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-23 06:19:57.000000 followthemoney-3.4.0/followthemoney.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:19:57.000000 followthemoney-3.4.0/followthemoney.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:19:34.000000 followthemoney-3.4.0/followthemoney.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-23 06:19:57.000000 followthemoney-3.4.0/followthemoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 06:19:57.000000 followthemoney-3.4.0/followthemoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-23 06:19:57.251635 followthemoney-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-23 06:18:02.000000 followthemoney-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.298807 followthemoney-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-22 12:04:20.000000 followthemoney-3.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-22 12:04:20.000000 followthemoney-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-22 12:06:23.298807 followthemoney-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-22 12:04:20.000000 followthemoney-3.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.282807 followthemoney-3.4.1/followthemoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.282807 followthemoney-3.4.1/followthemoney/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/cli/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/cli/exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/cli/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/cli/sieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.286807 followthemoney-3.4.1/followthemoney/export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/export/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/export/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/export/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/export/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/export/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/export/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.286807 followthemoney-3.4.1/followthemoney/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/mapping/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/mapping/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/mapping/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/mapping/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/mapping/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/mapping/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/offshore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19523 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/rdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.290807 followthemoney-3.4.1/followthemoney/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Address.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Airplane.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Analyzable.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Article.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Assessment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Asset.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Associate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Audio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/BankAccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Call.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/CallForTenders.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Company.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Contract.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/ContractAward.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/CourtCase.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/CourtCaseParty.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/CryptoWallet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Debt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Directorship.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Document.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/EconomicActivity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Email.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Employment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Event.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Family.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Folder.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/HyperText.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Identification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Image.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Interest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Interval.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/LegalEntity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/License.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Membership.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Mention.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Message.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Note.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Organization.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Ownership.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Package.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Page.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Passport.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Payment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Person.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/PlainText.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Post.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/ProjectParticipant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/PublicBody.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/RealEstate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Representation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Sanction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Security.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Similar.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Succession.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Table.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/TaxRoll.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Thing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Trip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/UnknownLink.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/UserAccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Value.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Vehicle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Vessel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Video.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema/Workbook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.290807 followthemoney-3.4.1/followthemoney/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.278807 followthemoney-3.4.1/followthemoney/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    39021 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   110484 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.278807 followthemoney-3.4.1/followthemoney/translations/bs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/bs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    93147 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.278807 followthemoney-3.4.1/followthemoney/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    36742 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   105691 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/de/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.278807 followthemoney-3.4.1/followthemoney/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    32360 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   104328 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/es/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    43316 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   109418 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (123)   106802 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/fr/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (123)    99827 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.278807 followthemoney-3.4.1/followthemoney/translations/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/nb/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    89796 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.278807 followthemoney-3.4.1/followthemoney/translations/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/nl/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    90876 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.278807 followthemoney-3.4.1/followthemoney/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    89847 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.294807 followthemoney-3.4.1/followthemoney/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    61028 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   131500 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (123)   130621 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/ru/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.278807 followthemoney-3.4.1/followthemoney/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.298807 followthemoney-3.4.1/followthemoney/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/tr/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    89829 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.298807 followthemoney-3.4.1/followthemoney/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/gender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/iban.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/mimetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/phone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/types/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-22 12:04:20.000000 followthemoney-3.4.1/followthemoney/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:06:23.282807 followthemoney-3.4.1/followthemoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-22 12:06:23.000000 followthemoney-3.4.1/followthemoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-22 12:06:23.000000 followthemoney-3.4.1/followthemoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:06:23.000000 followthemoney-3.4.1/followthemoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-22 12:06:23.000000 followthemoney-3.4.1/followthemoney.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:06:23.000000 followthemoney-3.4.1/followthemoney.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:06:01.000000 followthemoney-3.4.1/followthemoney.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-22 12:06:23.000000 followthemoney-3.4.1/followthemoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 12:06:23.000000 followthemoney-3.4.1/followthemoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-22 12:06:23.298807 followthemoney-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-22 12:04:20.000000 followthemoney-3.4.1/setup.py
```

### Comparing `followthemoney-3.4.0/LICENSE` & `followthemoney-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/PKG-INFO` & `followthemoney-3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: followthemoney
-Version: 3.4.0
+Version: 3.4.1
 Home-page: https://followthemoney.tech/
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `followthemoney-3.4.0/README.md` & `followthemoney-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/cli/aggregate.py` & `followthemoney-3.4.1/followthemoney/cli/aggregate.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from followthemoney.namespace import Namespace
 from followthemoney.cli.cli import cli
 from followthemoney.cli.util import InPath, OutPath, path_entities
 from followthemoney.cli.util import path_writer, write_entity
 
 
 def sorted_aggregate(path: Path, outpath: Path, entity_type: Type[E]) -> None:
-    """Aggregate entities based on the premise that the fragements in the source
+    """Aggregate entities based on the premise that the fragments in the source
     stream are sorted by their ID."""
     entity: Optional[E] = None
     with path_writer(outpath) as outfh:
         for next_entity in path_entities(path, entity_type=entity_type):
             if entity is None:
                 entity = next_entity
                 continue
```

### Comparing `followthemoney-3.4.0/followthemoney/cli/cli.py` & `followthemoney-3.4.1/followthemoney/cli/cli.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/cli/exports.py` & `followthemoney-3.4.1/followthemoney/cli/exports.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/cli/mapping.py` & `followthemoney-3.4.1/followthemoney/cli/mapping.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/cli/sieve.py` & `followthemoney-3.4.1/followthemoney/cli/sieve.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/cli/util.py` & `followthemoney-3.4.1/followthemoney/cli/util.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/compare.py` & `followthemoney-3.4.1/followthemoney/compare.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/exc.py` & `followthemoney-3.4.1/followthemoney/exc.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/export/common.py` & `followthemoney-3.4.1/followthemoney/export/common.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/export/csv.py` & `followthemoney-3.4.1/followthemoney/export/csv.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/export/excel.py` & `followthemoney-3.4.1/followthemoney/export/excel.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/export/graph.py` & `followthemoney-3.4.1/followthemoney/export/graph.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/export/neo4j.py` & `followthemoney-3.4.1/followthemoney/export/neo4j.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/export/rdf.py` & `followthemoney-3.4.1/followthemoney/export/rdf.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/graph.py` & `followthemoney-3.4.1/followthemoney/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         if self.prop is not None:
             return self.prop.reverse
         # NOTE: this edge points at a value node.
         return None
 
     @property
     def type_name(self) -> str:
-        """Return a machine-readable descripton of the type of the edge.
+        """Return a machine-readable description of the type of the edge.
         This is either a property name or a schema name."""
         if self.schema is not None:
             return self.schema.name
         if self.prop is None:
             raise InvalidModel("Invalid edge: %r" % self)
         return self.prop.name
```

### Comparing `followthemoney-3.4.0/followthemoney/helpers.py` & `followthemoney-3.4.1/followthemoney/helpers.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/mapping/csv.py` & `followthemoney-3.4.1/followthemoney/mapping/csv.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/mapping/entity.py` & `followthemoney-3.4.1/followthemoney/mapping/entity.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/mapping/property.py` & `followthemoney-3.4.1/followthemoney/mapping/property.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/mapping/query.py` & `followthemoney-3.4.1/followthemoney/mapping/query.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/mapping/source.py` & `followthemoney-3.4.1/followthemoney/mapping/source.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/mapping/sql.py` & `followthemoney-3.4.1/followthemoney/mapping/sql.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/messages.py` & `followthemoney-3.4.1/followthemoney/messages.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/model.py` & `followthemoney-3.4.1/followthemoney/model.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/namespace.py` & `followthemoney-3.4.1/followthemoney/namespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 *We like our abstractions like our offshore banks: leaky.*
 
 Entity ID namespaces are a security mechanism related to the Aleph search index.
 
-Aleph allows the user (via mappings or the API) to create arbitary entity IDs.
+Aleph allows the user (via mappings or the API) to create arbitrary entity IDs.
 Entity IDs that are controlled by the user and not the system are unusual.
 However, this makes it possible to generate bulk data outside Aleph,
 and then load entities into the system as a continuous :ref:`streams`.
 
 The problem is that having user controlled entity IDs increases the chance
 of conflict in the search index.
```

### Comparing `followthemoney-3.4.0/followthemoney/offshore.py` & `followthemoney-3.4.1/followthemoney/offshore.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/ontology.py` & `followthemoney-3.4.1/followthemoney/ontology.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/property.py` & `followthemoney-3.4.1/followthemoney/property.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/proxy.py` & `followthemoney-3.4.1/followthemoney/proxy.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Address.yaml` & `followthemoney-3.4.1/followthemoney/schema/Address.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
       label: "Full address"
       type: address
     remarks:
       label: "Remarks"
       description: "Handling instructions, like 'care of'."
     postOfficeBox:
       label: "PO Box"
-      description: "A mailbox indentifier at the post office"
+      description: "A mailbox identifier at the post office"
     street:
       label: "Street address"
     street2:
       label: "Street address (ctd.)"
     city:
       label: "City"
       description: "City, town, village or other locality"
```

### Comparing `followthemoney-3.4.0/followthemoney/schema/Airplane.yaml` & `followthemoney-3.4.1/followthemoney/schema/Airplane.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Analyzable.yaml` & `followthemoney-3.4.1/followthemoney/schema/Analyzable.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Assessment.yaml` & `followthemoney-3.4.1/followthemoney/schema/Assessment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Associate.yaml` & `followthemoney-3.4.1/followthemoney/schema/Associate.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/BankAccount.yaml` & `followthemoney-3.4.1/followthemoney/schema/BankAccount.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Call.yaml` & `followthemoney-3.4.1/followthemoney/schema/Call.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/CallForTenders.yaml` & `followthemoney-3.4.1/followthemoney/schema/CallForTenders.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -50,22 +50,22 @@
       label: "Directive"
     procedure:
       label: "Procedure"
     involvesOutcome:
       label: "Call for tenders result"
       description: "The nature of the contractual agreement that will result from this CfT"
     cpvCode:
-      label: "CPV codes"
+      label: "CPV code"
       description: "Common Procurement Vocabulary (CPV)"
       type: identifier
     reverseAuctionsIncluded:
       label: "Inclusion of e-Auctions"
       # cf. https://mita.gov.mt/2021/10/05/reverse-bidding-for-data-connectivity-across-the-public-service-a-first-for-malta/
     nutsCode:
-      label: "NUTS codes"
+      label: "NUTS code"
       description: "Nomenclature of Territorial Units for Statistics (NUTS)"
       type: identifier
     relationToThreshold:
       label: "Above or below threshold"
     paymentOptions:
       label: "Payment options"
     submissionDeadline:
```

### Comparing `followthemoney-3.4.0/followthemoney/schema/Company.yaml` & `followthemoney-3.4.1/followthemoney/schema/Company.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     voenCode:
       label: "VOEN"
       description: "Azerbaijan taxpayer ID"
       type: identifier
     coatoCode:
       label: "COATO / SOATO / OKATO"
       type: identifier
-      descrption: "Soviet classifier for territories, regions, districts, villages. Aka. SOATO and same as OKATO"
+      description: "Soviet classifier for territories, regions, districts, villages. Aka. SOATO and same as OKATO"
       matchable: false
     irsCode:
       label: "IRS Number"
       description: "US tax ID"
       type: identifier
     ipoCode:
       label: "IPO"
@@ -90,15 +90,15 @@
       description: "Russian bank account code"
     pfrNumber:
       label: "PFR Number"
       description: "(RU, ПФР) Pension Fund Registration number. AAA-BBB-CCCCCC, where AAA is organisation region, BBB is district, CCCCCC number at a specific branch"
       type: identifier
     oksmCode:
       label: OKSM
-      description: "Russian (ОКСМ) countries classifer"
+      description: "Russian (ОКСМ) countries classifier"
       matchable: false
     isinCode:
       label: ISIN
       description: International Securities Identification Number
       type: identifier
     ticker:
       label: Stock ticker symbol
```

### Comparing `followthemoney-3.4.0/followthemoney/schema/Contract.yaml` & `followthemoney-3.4.1/followthemoney/schema/Contract.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     - name
     - procedureNumber
   temporalExtent:
     start:
       - contractDate
   properties:
     title:
-      label: "Contract title"
+      label: "Title"
       type: string
     authority:
       label: "Contract authority"
       plural: "Contract authorities"
       reverse:
         name: contractAuthority
         label: "Contracts issued"
```

### Comparing `followthemoney-3.4.0/followthemoney/schema/ContractAward.yaml` & `followthemoney-3.4.1/followthemoney/schema/ContractAward.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
       plural: "Contracts"
       reverse:
         name: awards
         label: "Lots awarded"
       type: entity
       range: Contract
     callForTenders:
-      label: "Call For Tender"
+      label: "Call For Tenders"
       type: entity
       reverse:
         name: contractAwards
         label: "Contract Awards"
       range: CallForTenders
     lotNumber:
       label: "Lot number"
@@ -54,13 +54,15 @@
       label: "Document type"
     decisionReason:
       label: "Decision reason"
       type: text
     cpvCode:
       label: "CPV code"
       description: "Contract Procurement Vocabulary (what type of goods/services, EU)"
+      type: identifier
     nutsCode:
       label: "NUTS code"
       description: "Nomencalture of Territorial Units for Statistics (NUTS)"
+      type: identifier
     amended:
       label: "Amended"
       description: "Was this award amended, modified or updated by a subsequent document?"
```

### Comparing `followthemoney-3.4.0/followthemoney/schema/CourtCase.yaml` & `followthemoney-3.4.1/followthemoney/schema/CourtCase.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/CourtCaseParty.yaml` & `followthemoney-3.4.1/followthemoney/schema/CourtCaseParty.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/CryptoWallet.yaml` & `followthemoney-3.4.1/followthemoney/schema/CryptoWallet.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Debt.yaml` & `followthemoney-3.4.1/followthemoney/schema/Debt.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Directorship.yaml` & `followthemoney-3.4.1/followthemoney/schema/Directorship.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Document.yaml` & `followthemoney-3.4.1/followthemoney/schema/Document.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Documentation.yml` & `followthemoney-3.4.1/followthemoney/schema/Documentation.yml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/EconomicActivity.yaml` & `followthemoney-3.4.1/followthemoney/schema/EconomicActivity.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Email.yaml` & `followthemoney-3.4.1/followthemoney/schema/Email.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Employment.yaml` & `followthemoney-3.4.1/followthemoney/schema/Employment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Event.yaml` & `followthemoney-3.4.1/followthemoney/schema/Event.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Family.yaml` & `followthemoney-3.4.1/followthemoney/schema/Family.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Identification.yaml` & `followthemoney-3.4.1/followthemoney/schema/Identification.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Interval.yaml` & `followthemoney-3.4.1/followthemoney/schema/Interval.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/LegalEntity.yaml` & `followthemoney-3.4.1/followthemoney/schema/LegalEntity.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Membership.yaml` & `followthemoney-3.4.1/followthemoney/schema/Membership.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Mention.yaml` & `followthemoney-3.4.1/followthemoney/schema/Mention.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Message.yaml` & `followthemoney-3.4.1/followthemoney/schema/Message.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Ownership.yaml` & `followthemoney-3.4.1/followthemoney/schema/Ownership.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Page.yaml` & `followthemoney-3.4.1/followthemoney/schema/Page.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Passport.yaml` & `followthemoney-3.4.1/followthemoney/schema/Passport.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Payment.yaml` & `followthemoney-3.4.1/followthemoney/schema/Payment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Person.yaml` & `followthemoney-3.4.1/followthemoney/schema/Person.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Post.yaml` & `followthemoney-3.4.1/followthemoney/schema/Post.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -31,10 +31,10 @@
       type: entity
       range: Person
     organization:
       # This is a stub text version of the org, describing it by name.
       label: "Organization"
       type: string
     wikidataId:
-      label: "Wikidata ID of the post"
+      label: "Wikidata ID"
       hidden: true
       type: identifier
```

### Comparing `followthemoney-3.4.0/followthemoney/schema/ProjectParticipant.yaml` & `followthemoney-3.4.1/followthemoney/schema/ProjectParticipant.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/RealEstate.yaml` & `followthemoney-3.4.1/followthemoney/schema/RealEstate.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Representation.yaml` & `followthemoney-3.4.1/followthemoney/schema/Representation.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Sanction.yaml` & `followthemoney-3.4.1/followthemoney/schema/Sanction.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Security.yaml` & `followthemoney-3.4.1/followthemoney/schema/Security.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
       label: ISIN
       description: International Securities Identification Number
       type: identifier
     registrationNumber:
       label: Registration number
       type: identifier
     ticker:
-      label: Ticker
+      label: Stock ticker symbol
       type: identifier
     issuer:
       label: "Issuer"
       type: entity
       range: LegalEntity
       reverse:
         label: "Issued securities"
```

### Comparing `followthemoney-3.4.0/followthemoney/schema/Similar.yaml` & `followthemoney-3.4.1/followthemoney/schema/Similar.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Succession.yaml` & `followthemoney-3.4.1/followthemoney/schema/Succession.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Table.yaml` & `followthemoney-3.4.1/followthemoney/schema/Table.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/TaxRoll.yaml` & `followthemoney-3.4.1/followthemoney/schema/TaxRoll.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Thing.yaml` & `followthemoney-3.4.1/followthemoney/schema/Thing.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Trip.yaml` & `followthemoney-3.4.1/followthemoney/schema/Trip.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/UnknownLink.yaml` & `followthemoney-3.4.1/followthemoney/schema/UnknownLink.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/UserAccount.yaml` & `followthemoney-3.4.1/followthemoney/schema/UserAccount.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Vehicle.yaml` & `followthemoney-3.4.1/followthemoney/schema/Vehicle.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema/Vessel.yaml` & `followthemoney-3.4.1/followthemoney/schema/Vessel.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/schema.py` & `followthemoney-3.4.1/followthemoney/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
         #: Mark a set of properties as required. This is applied only when
         #: an entity is created by the user - bulk created entities will
         #: slip through even if it is technically invalid.
         self.required = ensure_list(data.get("required", []))
 
         #: Mark a set of properties to be used for the entity's caption.
-        #: They will be checked in order and the first existant value will
+        #: They will be checked in order and the first existent value will
         #: be used.
         self.caption = ensure_list(data.get("caption", []))
 
         # A transform of the entity into an edge for its representation in
         # the context of a property graph representation like Neo4J/Gephi.
         edge = data.get("edge", {})
         self.edge_source = edge.get("source")
```

### Comparing `followthemoney-3.4.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.1/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.1/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.1/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.1/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.1/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.1/followthemoney/translations/de/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.1/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.1/followthemoney/translations/es/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.1/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.1/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/translations/fr/followthemoney.po` & `followthemoney-3.4.1/followthemoney/translations/fr/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/translations/messages.pot` & `followthemoney-3.4.1/followthemoney/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.1/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.1/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.1/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.1/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.1/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/translations/ru/followthemoney.po` & `followthemoney-3.4.1/followthemoney/translations/ru/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.1/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/types/__init__.py` & `followthemoney-3.4.1/followthemoney/types/__init__.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/types/address.py` & `followthemoney-3.4.1/followthemoney/types/address.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/types/checksum.py` & `followthemoney-3.4.1/followthemoney/types/checksum.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/types/common.py` & `followthemoney-3.4.1/followthemoney/types/common.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/types/country.py` & `followthemoney-3.4.1/followthemoney/types/country.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/types/date.py` & `followthemoney-3.4.1/followthemoney/types/date.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/types/email.py` & `followthemoney-3.4.1/followthemoney/types/email.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/types/entity.py` & `followthemoney-3.4.1/followthemoney/types/entity.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/types/gender.py` & `followthemoney-3.4.1/followthemoney/types/gender.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/types/iban.py` & `followthemoney-3.4.1/followthemoney/types/iban.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from followthemoney.proxy import EntityProxy
 
 
 class IbanType(PropertyType):
     """An international bank account number, as defined in ISO 13616. IBANs are
     managed by SWIFT used in the European SEPA payment system.
 
-    A noteable aspect of IBANs is that they share a country prefix and validation
+    A notable aspect of IBANs is that they share a country prefix and validation
     mechanism, but the specific length of an IBAN is dependent on the country
     code defined in the first two characters: `NO8330001234567` and
     `CY21002001950000357001234567` are both valid values."""
 
     name = "iban"
     group = "ibans"
     label = _("IBAN")
```

### Comparing `followthemoney-3.4.0/followthemoney/types/identifier.py` & `followthemoney-3.4.1/followthemoney/types/identifier.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/types/ip.py` & `followthemoney-3.4.1/followthemoney/types/ip.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/types/json.py` & `followthemoney-3.4.1/followthemoney/types/json.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/types/language.py` & `followthemoney-3.4.1/followthemoney/types/language.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/types/mimetype.py` & `followthemoney-3.4.1/followthemoney/types/mimetype.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 if TYPE_CHECKING:
     from followthemoney.proxy import EntityProxy
 
 
 class MimeType(PropertyType):
     """A MIME media type are a specification of a content type on a network.
-    Each MIME type is assinged by IANA and consists of two parts: the type
+    Each MIME type is assigned by IANA and consists of two parts: the type
     and sub-type. Common examples are: `text/plain`, `application/json` and
     `application/pdf`.
 
     MIME type properties do not contain parameters as used in HTTP headers,
     like `charset=UTF-8`."""
 
     name = "mimetype"
```

### Comparing `followthemoney-3.4.0/followthemoney/types/name.py` & `followthemoney-3.4.1/followthemoney/types/name.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/types/number.py` & `followthemoney-3.4.1/followthemoney/types/number.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/types/phone.py` & `followthemoney-3.4.1/followthemoney/types/phone.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/types/registry.py` & `followthemoney-3.4.1/followthemoney/types/registry.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/types/string.py` & `followthemoney-3.4.1/followthemoney/types/string.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/types/topic.py` & `followthemoney-3.4.1/followthemoney/types/topic.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         "gov.muni": _("Municipal government"),
         "gov.soe": _("State-owned enterprise"),
         "gov.igo": _("Intergovernmental organization"),
         "fin": _("Financial services"),
         "fin.bank": _("Bank"),
         "fin.fund": _("Fund"),
         "fin.adivsor": _("Financial advisor"),
-        "role.pep": _("Politican"),
+        "role.pep": _("Political"),
         "role.rca": _("Close Associate"),
         "role.judge": _("Judge"),
         "role.civil": _("Civil servant"),
         "role.diplo": _("Diplomat"),
         "role.lawyer": _("Lawyer"),
         "role.acct": _("Accountant"),
         "role.spy": _("Spy"),
```

### Comparing `followthemoney-3.4.0/followthemoney/types/url.py` & `followthemoney-3.4.1/followthemoney/types/url.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney/util.py` & `followthemoney-3.4.1/followthemoney/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         "followthemoney", i18n_path, [str(locale)], fallback=True
     )
 
 
 def get_locale() -> Locale:
     if not hasattr(state, "locale"):
         return Locale.parse(DEFAULT_LOCALE)
-    return cast(Locale, state.locale)
+    return Locale.parse(state.locale)
 
 
 def get_env_list(name: str, default: List[str] = []) -> List[str]:
     value = stringify(os.environ.get(name))
     if value is not None:
         values = value.split(":")
         if len(values):
```

### Comparing `followthemoney-3.4.0/followthemoney.egg-info/PKG-INFO` & `followthemoney-3.4.1/followthemoney.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: followthemoney
-Version: 3.4.0
+Version: 3.4.1
 Home-page: https://followthemoney.tech/
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `followthemoney-3.4.0/followthemoney.egg-info/SOURCES.txt` & `followthemoney-3.4.1/followthemoney.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney.egg-info/entry_points.txt` & `followthemoney-3.4.1/followthemoney.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/followthemoney.egg-info/requires.txt` & `followthemoney-3.4.1/followthemoney.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.0/setup.py` & `followthemoney-3.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages  # type: ignore
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="followthemoney",
-    version="3.4.0",
+    version="3.4.1",
     author="Organized Crime and Corruption Reporting Project",
     author_email="data@occrp.org",
     url="https://followthemoney.tech/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
```

