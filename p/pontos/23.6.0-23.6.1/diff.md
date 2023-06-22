# Comparing `tmp/pontos-23.6.0.tar.gz` & `tmp/pontos-23.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pontos-23.6.0.tar", max compression
+gzip compressed data, was "pontos-23.6.1.tar", max compression
```

## Comparing `pontos-23.6.0.tar` & `pontos-23.6.1.tar`

### file list

```diff
@@ -1,253 +1,253 @@
--rw-r--r--   0        0        0    35149 2023-06-07 15:06:11.823374 pontos-23.6.0/LICENSE
--rw-r--r--   0        0        0     3836 2023-06-07 15:06:11.823374 pontos-23.6.0/README.md
--rw-r--r--   0        0        0   111699 2023-06-07 15:06:11.827374 pontos-23.6.0/poetry.lock
--rw-r--r--   0        0        0       32 2023-06-07 15:06:11.827374 pontos-23.6.0/poetry.toml
--rw-r--r--   0        0        0      791 2023-06-07 15:06:11.827374 pontos-23.6.0/pontos/__init__.py
--rw-r--r--   0        0        0      968 2023-06-07 15:06:11.827374 pontos-23.6.0/pontos/changelog/__init__.py
--rw-r--r--   0        0        0     9995 2023-06-07 15:06:11.827374 pontos-23.6.0/pontos/changelog/conventional_commits.py
--rw-r--r--   0        0        0      965 2023-06-07 15:06:11.827374 pontos-23.6.0/pontos/changelog/errors.py
--rw-r--r--   0        0        0     4393 2023-06-07 15:06:11.827374 pontos-23.6.0/pontos/changelog/main.py
--rw-r--r--   0        0        0      806 2023-06-07 15:06:11.827374 pontos-23.6.0/pontos/errors.py
--rw-r--r--   0        0        0      882 2023-06-07 15:06:11.827374 pontos-23.6.0/pontos/git/__init__.py
--rw-r--r--   0        0        0    16153 2023-06-07 15:06:11.827374 pontos-23.6.0/pontos/git/git.py
--rw-r--r--   0        0        0     2538 2023-06-07 15:06:11.827374 pontos-23.6.0/pontos/git/status.py
--rw-r--r--   0        0        0      760 2023-06-07 15:06:11.827374 pontos-23.6.0/pontos/github/__init__.py
--rw-r--r--   0        0        0     1154 2023-06-07 15:06:11.827374 pontos-23.6.0/pontos/github/actions/__init__.py
--rw-r--r--   0        0        0     2239 2023-06-07 15:06:11.827374 pontos-23.6.0/pontos/github/actions/argparser.py
--rw-r--r--   0        0        0     1472 2023-06-07 15:06:11.827374 pontos-23.6.0/pontos/github/actions/cmds.py
--rw-r--r--   0        0        0     7327 2023-06-07 15:06:11.827374 pontos-23.6.0/pontos/github/actions/core.py
--rw-r--r--   0        0        0     2426 2023-06-07 15:06:11.827374 pontos-23.6.0/pontos/github/actions/env.py
--rw-r--r--   0        0        0      861 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/actions/errors.py
--rw-r--r--   0        0        0     4173 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/actions/event.py
--rw-r--r--   0        0        0     1100 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/actions/main.py
--rw-r--r--   0        0        0     2047 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/api/__init__.py
--rw-r--r--   0        0        0     5531 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/api/api.py
--rw-r--r--   0        0        0     6196 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/api/artifacts.py
--rw-r--r--   0        0        0    34561 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/api/branch.py
--rw-r--r--   0        0        0     9395 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/api/client.py
--rw-r--r--   0        0        0     1844 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/api/contents.py
--rw-r--r--   0        0        0      845 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/api/errors.py
--rw-r--r--   0        0        0     1320 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/api/helper.py
--rw-r--r--   0        0        0     2813 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/api/labels.py
--rw-r--r--   0        0        0    10311 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/api/organizations.py
--rw-r--r--   0        0        0    13090 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/api/pull_requests.py
--rw-r--r--   0        0        0    11942 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/api/release.py
--rw-r--r--   0        0        0    21512 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/api/repositories.py
--rw-r--r--   0        0        0     3276 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/api/search.py
--rw-r--r--   0        0        0     6004 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/api/tags.py
--rw-r--r--   0        0        0    15207 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/api/teams.py
--rw-r--r--   0        0        0     9182 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/api/workflows.py
--rw-r--r--   0        0        0    11128 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/argparser.py
--rw-r--r--   0        0        0     8863 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/cmds.py
--rw-r--r--   0        0        0     1347 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/main.py
--rw-r--r--   0        0        0     1114 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/models/__init__.py
--rw-r--r--   0        0        0     2336 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/models/artifact.py
--rw-r--r--   0        0        0     7532 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/models/base.py
--rw-r--r--   0        0        0     6915 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/models/branch.py
--rw-r--r--   0        0        0    16573 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/models/organization.py
--rw-r--r--   0        0        0    14248 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/models/pull_request.py
--rw-r--r--   0        0        0     4607 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/models/release.py
--rw-r--r--   0        0        0     4299 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/models/search.py
--rw-r--r--   0        0        0     4606 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/models/tag.py
--rw-r--r--   0        0        0    11477 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/models/workflow.py
--rw-r--r--   0        0        0      790 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/pr_template.md
--rw-r--r--   0        0        0     3207 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/script/__init__.py
--rw-r--r--   0        0        0      835 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/script/errors.py
--rw-r--r--   0        0        0     4854 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/script/load.py
--rw-r--r--   0        0        0     1495 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/github/script/parser.py
--rw-r--r--   0        0        0    14685 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/helper.py
--rw-r--r--   0        0        0     6211 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/models/__init__.py
--rw-r--r--   0        0        0      821 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/nvd/__init__.py
--rw-r--r--   0        0        0     4660 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/nvd/api.py
--rw-r--r--   0        0        0     2149 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/nvd/cpe/__init__.py
--rw-r--r--   0        0        0     6708 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/nvd/cpe/api.py
--rw-r--r--   0        0        0     2618 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/nvd/cve/__init__.py
--rw-r--r--   0        0        0    10802 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/nvd/cve/api.py
--rw-r--r--   0        0        0      716 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/nvd/models/__init__.py
--rw-r--r--   0        0        0     2973 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/nvd/models/cpe.py
--rw-r--r--   0        0        0     7250 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/nvd/models/cve.py
--rw-r--r--   0        0        0     3254 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/nvd/models/cvss_v2.py
--rw-r--r--   0        0        0     4471 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/nvd/models/cvss_v3.py
--rw-r--r--   0        0        0     3561 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/pontos.py
--rw-r--r--   0        0        0        0 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/py.typed
--rw-r--r--   0        0        0     1164 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/release/__init__.py
--rw-r--r--   0        0        0     2472 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/release/helper.py
--rw-r--r--   0        0        0     2127 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/release/main.py
--rw-r--r--   0        0        0     8333 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/release/parser.py
--rw-r--r--   0        0        0    14408 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/release/release.py
--rw-r--r--   0        0        0    12499 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/release/sign.py
--rw-r--r--   0        0        0      886 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/terminal/__init__.py
--rw-r--r--   0        0        0     1770 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/terminal/null.py
--rw-r--r--   0        0        0     4717 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/terminal/rich.py
--rw-r--r--   0        0        0     9416 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/terminal/terminal.py
--rw-r--r--   0        0        0     7231 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/testing/__init__.py
--rw-r--r--   0        0        0      773 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/updateheader/__init__.py
--rw-r--r--   0        0        0      838 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/updateheader/__main__.py
--rw-r--r--   0        0        0      102 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       97 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       90 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       93 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       97 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       97 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      224 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       90 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       90 2023-06-07 15:06:11.831374 pontos-23.6.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
--rw-r--r--   0        0        0      100 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       85 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      117 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      117 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0       92 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-2.0-only/template.c
--rw-r--r--   0        0        0       92 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-2.0-only/template.h
--rw-r--r--   0        0        0      219 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-2.0-only/template.nasl
--rw-r--r--   0        0        0      101 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-2.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
--rw-r--r--   0        0        0       96 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-2.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-2.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-2.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-2.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
--rw-r--r--   0        0        0      101 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       92 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       96 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-3.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0    12149 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/updateheader/updateheader.py
--rw-r--r--   0        0        0     1067 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/__init__.py
--rw-r--r--   0        0        0      816 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/__main__.py
--rw-r--r--   0        0        0      103 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/__version__.py
--rw-r--r--   0        0        0     8837 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/_calculator.py
--rw-r--r--   0        0        0     1596 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/commands/__init__.py
--rw-r--r--   0        0        0     2723 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/commands/_cargo.py
--rw-r--r--   0        0        0     7752 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/commands/_cmake.py
--rw-r--r--   0        0        0     2553 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/commands/_command.py
--rw-r--r--   0        0        0     3792 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/commands/_go.py
--rw-r--r--   0        0        0     4043 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/commands/_java.py
--rw-r--r--   0        0        0     6263 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/commands/_javascript.py
--rw-r--r--   0        0        0     8216 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/commands/_python.py
--rw-r--r--   0        0        0      961 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/errors.py
--rw-r--r--   0        0        0     2812 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/helper.py
--rw-r--r--   0        0        0     3692 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/main.py
--rw-r--r--   0        0        0     4163 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/parser.py
--rw-r--r--   0        0        0     3750 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/project.py
--rw-r--r--   0        0        0     2163 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/schemes/__init__.py
--rw-r--r--   0        0        0    13439 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/schemes/_pep440.py
--rw-r--r--   0        0        0     2159 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/schemes/_scheme.py
--rw-r--r--   0        0        0    16043 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/schemes/_semantic.py
--rw-r--r--   0        0        0     5317 2023-06-07 15:06:11.835374 pontos-23.6.0/pontos/version/version.py
--rw-r--r--   0        0        0     2911 2023-06-07 15:06:11.835374 pontos-23.6.0/pyproject.toml
--rw-r--r--   0        0        0     1872 2023-06-07 15:06:11.835374 pontos-23.6.0/scripts/github/artifacts-download.py
--rw-r--r--   0        0        0     1862 2023-06-07 15:06:11.835374 pontos-23.6.0/scripts/github/artifacts.py
--rw-r--r--   0        0        0     1605 2023-06-07 15:06:11.835374 pontos-23.6.0/scripts/github/branchprotection.py
--rw-r--r--   0        0        0     5606 2023-06-07 15:06:11.835374 pontos-23.6.0/scripts/github/create-repository.py
--rw-r--r--   0        0        0     2212 2023-06-07 15:06:11.835374 pontos-23.6.0/scripts/github/enforce-admins.py
--rw-r--r--   0        0        0     1834 2023-06-07 15:06:11.835374 pontos-23.6.0/scripts/github/lock-branch.py
--rw-r--r--   0        0        0     2577 2023-06-07 15:06:11.835374 pontos-23.6.0/scripts/github/members.py
--rw-r--r--   0        0        0     2179 2023-06-07 15:06:11.835374 pontos-23.6.0/scripts/github/release-assets-download.py
--rw-r--r--   0        0        0     2294 2023-06-07 15:06:11.835374 pontos-23.6.0/scripts/github/repositories.py
--rw-r--r--   0        0        0     6717 2023-06-07 15:06:11.835374 pontos-23.6.0/scripts/github/search-repositories.py
--rw-r--r--   0        0        0     3689 2023-06-07 15:06:11.835374 pontos-23.6.0/scripts/github/team-repositories.py
--rw-r--r--   0        0        0     1654 2023-06-07 15:06:11.835374 pontos-23.6.0/scripts/github/teams.py
--rw-r--r--   0        0        0     2789 2023-06-07 15:06:11.835374 pontos-23.6.0/scripts/github/workflow-runs.py
--rw-r--r--   0        0        0     1518 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/__init__.py
--rw-r--r--   0        0        0     1031 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/changelog/__init__.py
--rw-r--r--   0        0        0      375 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/changelog/changelog.toml
--rw-r--r--   0        0        0    17925 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/changelog/test_conventional_commits.py
--rw-r--r--   0        0        0     1925 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/changelog/test_parser.py
--rw-r--r--   0        0        0       69 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/fake_pyproject.toml
--rw-r--r--   0        0        0      716 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/git/__init__.py
--rw-r--r--   0        0        0    28296 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/git/test_git.py
--rw-r--r--   0        0        0     4215 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/git/test_status.py
--rw-r--r--   0        0        0      716 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/github/__init__.py
--rw-r--r--   0        0        0      716 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/github/actions/__init__.py
--rw-r--r--   0        0        0    29628 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/github/actions/test-pull-request-event.json
--rw-r--r--   0        0        0     5430 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/github/actions/test_core.py
--rw-r--r--   0        0        0     3534 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/github/actions/test_env.py
--rw-r--r--   0        0        0     2086 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/github/actions/test_event.py
--rw-r--r--   0        0        0     1232 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/github/api/__init__.py
--rw-r--r--   0        0        0    20021 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/github/api/pr-files.json
--rw-r--r--   0        0        0     5624 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/github/api/release-response.json
--rw-r--r--   0        0        0    12076 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/github/api/test_artifacts.py
--rw-r--r--   0        0        0    20096 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/github/api/test_branch.py
--rw-r--r--   0        0        0     9619 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/github/api/test_client.py
--rw-r--r--   0        0        0     2087 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/github/api/test_contents.py
--rw-r--r--   0        0        0     2801 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/github/api/test_labels.py
--rw-r--r--   0        0        0    71096 2023-06-07 15:06:11.835374 pontos-23.6.0/tests/github/api/test_organizations.py
--rw-r--r--   0        0        0    58514 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/api/test_pull_requests.py
--rw-r--r--   0        0        0    17774 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/api/test_release.py
--rw-r--r--   0        0        0    37847 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/api/test_repositories.py
--rw-r--r--   0        0        0    24490 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/api/test_search.py
--rw-r--r--   0        0        0     9471 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/api/test_tags.py
--rw-r--r--   0        0        0    39045 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/api/test_teams.py
--rw-r--r--   0        0        0   129346 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/api/test_workflows.py
--rw-r--r--   0        0        0      716 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/models/__init__.py
--rw-r--r--   0        0        0     3210 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/models/test_artifact.py
--rw-r--r--   0        0        0     9831 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/models/test_base.py
--rw-r--r--   0        0        0    31873 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/models/test_branch.py
--rw-r--r--   0        0        0    19874 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/models/test_organization.py
--rw-r--r--   0        0        0    80894 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/models/test_pull_request.py
--rw-r--r--   0        0        0    12062 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/models/test_release.py
--rw-r--r--   0        0        0     2216 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/models/test_search.py
--rw-r--r--   0        0        0     3400 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/models/test_tag.py
--rw-r--r--   0        0        0    41463 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/models/test_workflow.py
--rw-r--r--   0        0        0      716 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/script/__init__.py
--rw-r--r--   0        0        0     3520 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/script/test_load.py
--rw-r--r--   0        0        0     2052 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/script/test_parser.py
--rw-r--r--   0        0        0     6371 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/test_argparser.py
--rw-r--r--   0        0        0     9562 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/github/test_cmds.py
--rw-r--r--   0        0        0      716 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/models/__init__.py
--rw-r--r--   0        0        0     6424 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/models/test_models.py
--rw-r--r--   0        0        0     2505 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/nvd/__init__.py
--rw-r--r--   0        0        0      716 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/nvd/cpe/__init__.py
--rw-r--r--   0        0        0    11271 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/nvd/cpe/test_api.py
--rw-r--r--   0        0        0      716 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/nvd/cve/__init__.py
--rw-r--r--   0        0        0    26602 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/nvd/cve/test_api.py
--rw-r--r--   0        0        0      716 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/nvd/models/__init__.py
--rw-r--r--   0        0        0     3706 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/nvd/models/test_cpe.py
--rw-r--r--   0        0        0    25911 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/nvd/models/test_cve.py
--rw-r--r--   0        0        0     3994 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/nvd/test_api.py
--rw-r--r--   0        0        0      721 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/release/__init__.py
--rw-r--r--   0        0        0     3265 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/release/test_helper.py
--rw-r--r--   0        0        0     9077 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/release/test_parser.py
--rw-r--r--   0        0        0    83503 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/release/test_release.py
--rw-r--r--   0        0        0    25286 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/release/test_sign.py
--rw-r--r--   0        0        0      345 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/release/v1.2.3.md
--rw-r--r--   0        0        0      745 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/terminal/__init__.py
--rw-r--r--   0        0        0     6653 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/terminal/test_terminal.py
--rw-r--r--   0        0        0    19355 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/test_helper.py
--rw-r--r--   0        0        0     1685 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/test_pontos.py
--rw-r--r--   0        0        0      716 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/testing/__init__.py
--rw-r--r--   0        0        0     7785 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/testing/test_testing.py
--rw-r--r--   0        0        0      721 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/updateheader/__init__.py
--rw-r--r--   0        0        0    15848 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/updateheader/test_header.py
--rw-r--r--   0        0        0     1031 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/version/__init__.py
--rw-r--r--   0        0        0      727 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/version/commands/__init__.py
--rw-r--r--   0        0        0     3847 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/version/commands/test_cargo.py
--rw-r--r--   0        0        0    11322 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/version/commands/test_cmake.py
--rw-r--r--   0        0        0    10400 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/version/commands/test_go.py
--rw-r--r--   0        0        0     8737 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/version/commands/test_java.py
--rw-r--r--   0        0        0    15376 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/version/commands/test_javascript.py
--rw-r--r--   0        0        0    16667 2023-06-07 15:06:11.839374 pontos-23.6.0/tests/version/commands/test_python.py
--rw-r--r--   0        0        0      727 2023-06-07 15:06:11.843374 pontos-23.6.0/tests/version/schemes/__init__.py
--rw-r--r--   0        0        0    25664 2023-06-07 15:06:11.843374 pontos-23.6.0/tests/version/schemes/test_pep440.py
--rw-r--r--   0        0        0    27735 2023-06-07 15:06:11.843374 pontos-23.6.0/tests/version/schemes/test_semantic.py
--rw-r--r--   0        0        0      919 2023-06-07 15:06:11.843374 pontos-23.6.0/tests/version/test_commands.py
--rw-r--r--   0        0        0     1096 2023-06-07 15:06:11.843374 pontos-23.6.0/tests/version/test_errors.py
--rw-r--r--   0        0        0     7621 2023-06-07 15:06:11.843374 pontos-23.6.0/tests/version/test_helper.py
--rw-r--r--   0        0        0    10908 2023-06-07 15:06:11.843374 pontos-23.6.0/tests/version/test_main.py
--rw-r--r--   0        0        0     1131 2023-06-07 15:06:11.843374 pontos-23.6.0/tests/version/test_parser.py
--rw-r--r--   0        0        0     6187 2023-06-07 15:06:11.843374 pontos-23.6.0/tests/version/test_project.py
--rw-r--r--   0        0        0     1791 2023-06-07 15:06:11.843374 pontos-23.6.0/tests/version/test_version.py
--rw-r--r--   0        0        0     5188 1970-01-01 00:00:00.000000 pontos-23.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-22 07:56:38.365392 pontos-23.6.1/LICENSE
+-rw-r--r--   0        0        0     3836 2023-06-22 07:56:38.365392 pontos-23.6.1/README.md
+-rw-r--r--   0        0        0   110390 2023-06-22 07:56:38.369392 pontos-23.6.1/poetry.lock
+-rw-r--r--   0        0        0       32 2023-06-22 07:56:38.369392 pontos-23.6.1/poetry.toml
+-rw-r--r--   0        0        0      791 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/__init__.py
+-rw-r--r--   0        0        0      968 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/changelog/__init__.py
+-rw-r--r--   0        0        0     9995 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/changelog/conventional_commits.py
+-rw-r--r--   0        0        0      965 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/changelog/errors.py
+-rw-r--r--   0        0        0     4393 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/changelog/main.py
+-rw-r--r--   0        0        0      806 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/errors.py
+-rw-r--r--   0        0        0      882 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/git/__init__.py
+-rw-r--r--   0        0        0    16153 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/git/git.py
+-rw-r--r--   0        0        0     2538 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/git/status.py
+-rw-r--r--   0        0        0      760 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/github/__init__.py
+-rw-r--r--   0        0        0     1154 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/github/actions/__init__.py
+-rw-r--r--   0        0        0     2239 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/github/actions/argparser.py
+-rw-r--r--   0        0        0     1472 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/github/actions/cmds.py
+-rw-r--r--   0        0        0     7327 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/github/actions/core.py
+-rw-r--r--   0        0        0     2426 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/github/actions/env.py
+-rw-r--r--   0        0        0      861 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/github/actions/errors.py
+-rw-r--r--   0        0        0     4173 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/github/actions/event.py
+-rw-r--r--   0        0        0     1100 2023-06-22 07:56:38.369392 pontos-23.6.1/pontos/github/actions/main.py
+-rw-r--r--   0        0        0     2047 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/__init__.py
+-rw-r--r--   0        0        0     5531 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/api.py
+-rw-r--r--   0        0        0     6196 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/artifacts.py
+-rw-r--r--   0        0        0    34561 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/branch.py
+-rw-r--r--   0        0        0     9395 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/client.py
+-rw-r--r--   0        0        0     1844 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/contents.py
+-rw-r--r--   0        0        0      845 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/errors.py
+-rw-r--r--   0        0        0     1320 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/helper.py
+-rw-r--r--   0        0        0     2813 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/labels.py
+-rw-r--r--   0        0        0    10311 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/organizations.py
+-rw-r--r--   0        0        0    13090 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/pull_requests.py
+-rw-r--r--   0        0        0    11942 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/release.py
+-rw-r--r--   0        0        0    21512 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/repositories.py
+-rw-r--r--   0        0        0     3276 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/search.py
+-rw-r--r--   0        0        0     6004 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/tags.py
+-rw-r--r--   0        0        0    15207 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/teams.py
+-rw-r--r--   0        0        0     9182 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/api/workflows.py
+-rw-r--r--   0        0        0    11128 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/argparser.py
+-rw-r--r--   0        0        0     8863 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/cmds.py
+-rw-r--r--   0        0        0     1347 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/main.py
+-rw-r--r--   0        0        0     1114 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/__init__.py
+-rw-r--r--   0        0        0     2336 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/artifact.py
+-rw-r--r--   0        0        0     7532 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/base.py
+-rw-r--r--   0        0        0     6915 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/branch.py
+-rw-r--r--   0        0        0    16573 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/organization.py
+-rw-r--r--   0        0        0    14248 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/pull_request.py
+-rw-r--r--   0        0        0     4607 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/release.py
+-rw-r--r--   0        0        0     4299 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/search.py
+-rw-r--r--   0        0        0     4606 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/tag.py
+-rw-r--r--   0        0        0    11477 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/models/workflow.py
+-rw-r--r--   0        0        0      790 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/pr_template.md
+-rw-r--r--   0        0        0     3207 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/script/__init__.py
+-rw-r--r--   0        0        0      835 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/script/errors.py
+-rw-r--r--   0        0        0     4854 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/script/load.py
+-rw-r--r--   0        0        0     1495 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/github/script/parser.py
+-rw-r--r--   0        0        0    14685 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/helper.py
+-rw-r--r--   0        0        0     6211 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/models/__init__.py
+-rw-r--r--   0        0        0      821 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/__init__.py
+-rw-r--r--   0        0        0     4660 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/api.py
+-rw-r--r--   0        0        0     2149 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0     6708 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/cpe/api.py
+-rw-r--r--   0        0        0     2618 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    10802 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/cve/api.py
+-rw-r--r--   0        0        0      716 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/models/__init__.py
+-rw-r--r--   0        0        0     2973 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/models/cpe.py
+-rw-r--r--   0        0        0     7250 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/models/cve.py
+-rw-r--r--   0        0        0     3254 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/models/cvss_v2.py
+-rw-r--r--   0        0        0     4471 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/nvd/models/cvss_v3.py
+-rw-r--r--   0        0        0     3561 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/pontos.py
+-rw-r--r--   0        0        0        0 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/py.typed
+-rw-r--r--   0        0        0     1164 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/release/__init__.py
+-rw-r--r--   0        0        0     2472 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/release/helper.py
+-rw-r--r--   0        0        0     2127 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/release/main.py
+-rw-r--r--   0        0        0     8333 2023-06-22 07:56:38.373392 pontos-23.6.1/pontos/release/parser.py
+-rw-r--r--   0        0        0    14408 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/release/release.py
+-rw-r--r--   0        0        0    12499 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/release/sign.py
+-rw-r--r--   0        0        0      886 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/terminal/__init__.py
+-rw-r--r--   0        0        0     1770 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/terminal/null.py
+-rw-r--r--   0        0        0     4717 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/terminal/rich.py
+-rw-r--r--   0        0        0     9416 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/terminal/terminal.py
+-rw-r--r--   0        0        0     7231 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/testing/__init__.py
+-rw-r--r--   0        0        0      773 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/__init__.py
+-rw-r--r--   0        0        0      838 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/__main__.py
+-rw-r--r--   0        0        0      102 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       97 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       90 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       93 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       97 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       97 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      224 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       90 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       90 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0      100 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       85 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      117 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      117 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0       92 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-only/template.c
+-rw-r--r--   0        0        0       92 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-only/template.h
+-rw-r--r--   0        0        0      219 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-only/template.nasl
+-rw-r--r--   0        0        0      101 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
+-rw-r--r--   0        0        0       96 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
+-rw-r--r--   0        0        0      101 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       92 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       96 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0    12149 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/updateheader/updateheader.py
+-rw-r--r--   0        0        0     1067 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/__init__.py
+-rw-r--r--   0        0        0      816 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/__main__.py
+-rw-r--r--   0        0        0      103 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/__version__.py
+-rw-r--r--   0        0        0     8837 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/_calculator.py
+-rw-r--r--   0        0        0     1596 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/commands/__init__.py
+-rw-r--r--   0        0        0     2723 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/commands/_cargo.py
+-rw-r--r--   0        0        0     7752 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/commands/_cmake.py
+-rw-r--r--   0        0        0     2553 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/commands/_command.py
+-rw-r--r--   0        0        0     3792 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/commands/_go.py
+-rw-r--r--   0        0        0     6445 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/commands/_java.py
+-rw-r--r--   0        0        0     6263 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/commands/_javascript.py
+-rw-r--r--   0        0        0     8216 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/commands/_python.py
+-rw-r--r--   0        0        0      961 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/errors.py
+-rw-r--r--   0        0        0     2812 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/helper.py
+-rw-r--r--   0        0        0     3692 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/main.py
+-rw-r--r--   0        0        0     4163 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/parser.py
+-rw-r--r--   0        0        0     3750 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/project.py
+-rw-r--r--   0        0        0     2163 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/schemes/__init__.py
+-rw-r--r--   0        0        0    13439 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/schemes/_pep440.py
+-rw-r--r--   0        0        0     2159 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/schemes/_scheme.py
+-rw-r--r--   0        0        0    16043 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/schemes/_semantic.py
+-rw-r--r--   0        0        0     5317 2023-06-22 07:56:38.377392 pontos-23.6.1/pontos/version/version.py
+-rw-r--r--   0        0        0     2911 2023-06-22 07:56:38.377392 pontos-23.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1872 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/artifacts-download.py
+-rw-r--r--   0        0        0     1862 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/artifacts.py
+-rw-r--r--   0        0        0     1605 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/branchprotection.py
+-rw-r--r--   0        0        0     5606 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/create-repository.py
+-rw-r--r--   0        0        0     2212 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/enforce-admins.py
+-rw-r--r--   0        0        0     1834 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/lock-branch.py
+-rw-r--r--   0        0        0     2577 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/members.py
+-rw-r--r--   0        0        0     2179 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/release-assets-download.py
+-rw-r--r--   0        0        0     2294 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/repositories.py
+-rw-r--r--   0        0        0     6717 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/search-repositories.py
+-rw-r--r--   0        0        0     3689 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/team-repositories.py
+-rw-r--r--   0        0        0     1654 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/teams.py
+-rw-r--r--   0        0        0     2789 2023-06-22 07:56:38.381392 pontos-23.6.1/scripts/github/workflow-runs.py
+-rw-r--r--   0        0        0     1518 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/__init__.py
+-rw-r--r--   0        0        0     1031 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/changelog/__init__.py
+-rw-r--r--   0        0        0      375 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/changelog/changelog.toml
+-rw-r--r--   0        0        0    17925 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/changelog/test_conventional_commits.py
+-rw-r--r--   0        0        0     1925 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/changelog/test_parser.py
+-rw-r--r--   0        0        0       69 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/fake_pyproject.toml
+-rw-r--r--   0        0        0      716 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/git/__init__.py
+-rw-r--r--   0        0        0    28296 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/git/test_git.py
+-rw-r--r--   0        0        0     4215 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/git/test_status.py
+-rw-r--r--   0        0        0      716 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/__init__.py
+-rw-r--r--   0        0        0      716 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/actions/__init__.py
+-rw-r--r--   0        0        0    29628 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/actions/test-pull-request-event.json
+-rw-r--r--   0        0        0     5430 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/actions/test_core.py
+-rw-r--r--   0        0        0     3534 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/actions/test_env.py
+-rw-r--r--   0        0        0     2086 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/actions/test_event.py
+-rw-r--r--   0        0        0     1232 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/__init__.py
+-rw-r--r--   0        0        0    20021 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/pr-files.json
+-rw-r--r--   0        0        0     5624 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/release-response.json
+-rw-r--r--   0        0        0    12076 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_artifacts.py
+-rw-r--r--   0        0        0    20096 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_branch.py
+-rw-r--r--   0        0        0     9619 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_client.py
+-rw-r--r--   0        0        0     2087 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_contents.py
+-rw-r--r--   0        0        0     2801 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_labels.py
+-rw-r--r--   0        0        0    71096 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_organizations.py
+-rw-r--r--   0        0        0    58514 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_pull_requests.py
+-rw-r--r--   0        0        0    17774 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_release.py
+-rw-r--r--   0        0        0    37847 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_repositories.py
+-rw-r--r--   0        0        0    24490 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_search.py
+-rw-r--r--   0        0        0     9471 2023-06-22 07:56:38.381392 pontos-23.6.1/tests/github/api/test_tags.py
+-rw-r--r--   0        0        0    39045 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/api/test_teams.py
+-rw-r--r--   0        0        0   129346 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/api/test_workflows.py
+-rw-r--r--   0        0        0      716 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/__init__.py
+-rw-r--r--   0        0        0     3210 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/test_artifact.py
+-rw-r--r--   0        0        0     9831 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/test_base.py
+-rw-r--r--   0        0        0    31873 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/test_branch.py
+-rw-r--r--   0        0        0    19874 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/test_organization.py
+-rw-r--r--   0        0        0    80894 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/test_pull_request.py
+-rw-r--r--   0        0        0    12062 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/test_release.py
+-rw-r--r--   0        0        0     2216 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/test_search.py
+-rw-r--r--   0        0        0     3400 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/test_tag.py
+-rw-r--r--   0        0        0    41463 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/models/test_workflow.py
+-rw-r--r--   0        0        0      716 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/script/__init__.py
+-rw-r--r--   0        0        0     3520 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/script/test_load.py
+-rw-r--r--   0        0        0     2052 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/script/test_parser.py
+-rw-r--r--   0        0        0     6371 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/test_argparser.py
+-rw-r--r--   0        0        0     9562 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/github/test_cmds.py
+-rw-r--r--   0        0        0      716 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/models/__init__.py
+-rw-r--r--   0        0        0     6424 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/models/test_models.py
+-rw-r--r--   0        0        0     2505 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/nvd/__init__.py
+-rw-r--r--   0        0        0      716 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0    11271 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/nvd/cpe/test_api.py
+-rw-r--r--   0        0        0      716 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    26602 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/nvd/cve/test_api.py
+-rw-r--r--   0        0        0      716 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/nvd/models/__init__.py
+-rw-r--r--   0        0        0     3706 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/nvd/models/test_cpe.py
+-rw-r--r--   0        0        0    25911 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/nvd/models/test_cve.py
+-rw-r--r--   0        0        0     3994 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/nvd/test_api.py
+-rw-r--r--   0        0        0      721 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/release/__init__.py
+-rw-r--r--   0        0        0     3265 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/release/test_helper.py
+-rw-r--r--   0        0        0     9077 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/release/test_parser.py
+-rw-r--r--   0        0        0    83503 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/release/test_release.py
+-rw-r--r--   0        0        0    25286 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/release/test_sign.py
+-rw-r--r--   0        0        0      345 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/release/v1.2.3.md
+-rw-r--r--   0        0        0      745 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/terminal/__init__.py
+-rw-r--r--   0        0        0     6653 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/terminal/test_terminal.py
+-rw-r--r--   0        0        0    19355 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/test_helper.py
+-rw-r--r--   0        0        0     1685 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/test_pontos.py
+-rw-r--r--   0        0        0      716 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/testing/__init__.py
+-rw-r--r--   0        0        0     7785 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/testing/test_testing.py
+-rw-r--r--   0        0        0      721 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/updateheader/__init__.py
+-rw-r--r--   0        0        0    15848 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/updateheader/test_header.py
+-rw-r--r--   0        0        0     1031 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/version/__init__.py
+-rw-r--r--   0        0        0      727 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/version/commands/__init__.py
+-rw-r--r--   0        0        0     3847 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/version/commands/test_cargo.py
+-rw-r--r--   0        0        0    11322 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/version/commands/test_cmake.py
+-rw-r--r--   0        0        0    10400 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/version/commands/test_go.py
+-rw-r--r--   0        0        0    11614 2023-06-22 07:56:38.385392 pontos-23.6.1/tests/version/commands/test_java.py
+-rw-r--r--   0        0        0    15376 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/commands/test_javascript.py
+-rw-r--r--   0        0        0    16667 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/commands/test_python.py
+-rw-r--r--   0        0        0      727 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/schemes/__init__.py
+-rw-r--r--   0        0        0    25664 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/schemes/test_pep440.py
+-rw-r--r--   0        0        0    27735 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/schemes/test_semantic.py
+-rw-r--r--   0        0        0      919 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/test_commands.py
+-rw-r--r--   0        0        0     1096 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/test_errors.py
+-rw-r--r--   0        0        0     7621 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/test_helper.py
+-rw-r--r--   0        0        0    10908 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/test_main.py
+-rw-r--r--   0        0        0     1131 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/test_parser.py
+-rw-r--r--   0        0        0     6187 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/test_project.py
+-rw-r--r--   0        0        0     1791 2023-06-22 07:56:38.389392 pontos-23.6.1/tests/version/test_version.py
+-rw-r--r--   0        0        0     5188 1970-01-01 00:00:00.000000 pontos-23.6.1/PKG-INFO
```

### Comparing `pontos-23.6.0/LICENSE` & `pontos-23.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/README.md` & `pontos-23.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/poetry.lock` & `pontos-23.6.1/poetry.lock`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-# This file is automatically @generated by Poetry and should not be changed by hand.
+# This file is automatically @generated by Poetry 1.5.1 and should not be changed by hand.
 
 [[package]]
 name = "alabaster"
 version = "0.7.13"
 description = "A configurable sidebar-enabled Sphinx theme"
-category = "dev"
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "alabaster-0.7.13-py3-none-any.whl", hash = "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3"},
     {file = "alabaster-0.7.13.tar.gz", hash = "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"},
 ]
 
 [[package]]
 name = "anyio"
 version = "3.7.0"
 description = "High level compatibility layer for multiple asynchronous event loop implementations"
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "anyio-3.7.0-py3-none-any.whl", hash = "sha256:eddca883c4175f14df8aedce21054bfca3adb70ffe76a9f607aef9d7fa2ea7f0"},
     {file = "anyio-3.7.0.tar.gz", hash = "sha256:275d9973793619a5374e1c89a4f4ad3f4b0a5510a2b5b939444bee8f4c4d37ce"},
 ]
 
@@ -34,15 +32,14 @@
 test = ["anyio[trio]", "coverage[toml] (>=4.5)", "hypothesis (>=4.0)", "mock (>=4)", "psutil (>=5.9)", "pytest (>=7.0)", "pytest-mock (>=3.6.1)", "trustme", "uvloop (>=0.17)"]
 trio = ["trio (<0.22)"]
 
 [[package]]
 name = "astroid"
 version = "2.15.5"
 description = "An abstract syntax tree for Python with inference support."
-category = "dev"
 optional = false
 python-versions = ">=3.7.2"
 files = [
     {file = "astroid-2.15.5-py3-none-any.whl", hash = "sha256:078e5212f9885fa85fbb0cf0101978a336190aadea6e13305409d099f71b2324"},
     {file = "astroid-2.15.5.tar.gz", hash = "sha256:1039262575027b441137ab4a62a793a9b43defb42c32d5670f38686207cd780f"},
 ]
 
@@ -54,15 +51,14 @@
     {version = ">=1.14,<2", markers = "python_version >= \"3.11\""},
 ]
 
 [[package]]
 name = "autohooks"
 version = "23.4.0"
 description = "Library for managing git hooks"
-category = "dev"
 optional = false
 python-versions = ">=3.7.2,<4.0.0"
 files = [
     {file = "autohooks-23.4.0-py3-none-any.whl", hash = "sha256:2c3b8506890565ad8c9b690db9b70a9b65068ff9f1c2a2d601d2914ad576cfff"},
     {file = "autohooks-23.4.0.tar.gz", hash = "sha256:6880ad263f0aaab607bbfc1d42afc407de6234320fcff10d75d4e89f4e711ccd"},
 ]
 
@@ -71,15 +67,14 @@
 rich = ">=12.5.1"
 tomlkit = ">=0.5.11"
 
 [[package]]
 name = "autohooks-plugin-black"
 version = "23.4.0"
 description = "An autohooks plugin for python code formatting via black"
-category = "dev"
 optional = false
 python-versions = ">=3.7.2,<4.0.0"
 files = [
     {file = "autohooks_plugin_black-23.4.0-py3-none-any.whl", hash = "sha256:1a65814ab573a40799cf52af7aa026e73ef60d784cf14a8eba33aaf245811899"},
     {file = "autohooks_plugin_black-23.4.0.tar.gz", hash = "sha256:31b0497f8987def02d5387b9eb03c46837621097c9814d19ff6b9da960867a06"},
 ]
 
@@ -87,15 +82,14 @@
 autohooks = ">=21.6.0"
 black = ">=20.8"
 
 [[package]]
 name = "autohooks-plugin-isort"
 version = "23.4.0"
 description = "An autohooks plugin for python code formatting via isort"
-category = "dev"
 optional = false
 python-versions = ">=3.7,<4.0"
 files = [
     {file = "autohooks_plugin_isort-23.4.0-py3-none-any.whl", hash = "sha256:ada2aad42a2c6e12b4b931a524c971968b4f2426bd7bc96f7806867e1237e449"},
     {file = "autohooks_plugin_isort-23.4.0.tar.gz", hash = "sha256:309188365bfed8f2841545f7484bc9e4872d031ef8d495128a86e409483c5b6a"},
 ]
 
@@ -103,15 +97,14 @@
 autohooks = ">=21.6.0"
 isort = ">=5.8.0,<6.0.0"
 
 [[package]]
 name = "autohooks-plugin-pylint"
 version = "23.4.0"
 description = "An autohooks plugin for python code linting via pylint"
-category = "dev"
 optional = false
 python-versions = ">=3.7.2,<4.0.0"
 files = [
     {file = "autohooks_plugin_pylint-23.4.0-py3-none-any.whl", hash = "sha256:2dd581c3764949ef9c1041f5a34206cac796a342a900f47e5f42346e80598009"},
     {file = "autohooks_plugin_pylint-23.4.0.tar.gz", hash = "sha256:746c24a73bb312e9883f531d13db16da4bd05949969e7adeee3e8d1105a9c6c2"},
 ]
 
@@ -119,27 +112,25 @@
 autohooks = ">=2.2.0"
 pylint = ">=2.8.3"
 
 [[package]]
 name = "babel"
 version = "2.12.1"
 description = "Internationalization utilities"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "Babel-2.12.1-py3-none-any.whl", hash = "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610"},
     {file = "Babel-2.12.1.tar.gz", hash = "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"},
 ]
 
 [[package]]
 name = "beautifulsoup4"
 version = "4.12.2"
 description = "Screen-scraping library"
-category = "dev"
 optional = false
 python-versions = ">=3.6.0"
 files = [
     {file = "beautifulsoup4-4.12.2-py3-none-any.whl", hash = "sha256:bd2520ca0d9d7d12694a53d44ac482d181b4ec1888909b035a3dbf40d0f57d4a"},
     {file = "beautifulsoup4-4.12.2.tar.gz", hash = "sha256:492bbc69dca35d12daac71c4db1bfff0c876c00ef4a2ffacce226d4638eb72da"},
 ]
 
@@ -150,15 +141,14 @@
 html5lib = ["html5lib"]
 lxml = ["lxml"]
 
 [[package]]
 name = "black"
 version = "23.3.0"
 description = "The uncompromising code formatter."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "black-23.3.0-cp310-cp310-macosx_10_16_arm64.whl", hash = "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915"},
     {file = "black-23.3.0-cp310-cp310-macosx_10_16_universal2.whl", hash = "sha256:67de8d0c209eb5b330cce2469503de11bca4085880d62f1628bd9972cc3366b9"},
     {file = "black-23.3.0-cp310-cp310-macosx_10_16_x86_64.whl", hash = "sha256:7c3eb7cea23904399866c55826b31c1f55bbcd3890ce22ff70466b907b6775c2"},
     {file = "black-23.3.0-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:32daa9783106c28815d05b724238e30718f34155653d4d6e125dc7daec8e260c"},
@@ -200,27 +190,25 @@
 jupyter = ["ipython (>=7.8.0)", "tokenize-rt (>=3.2.0)"]
 uvloop = ["uvloop (>=0.15.2)"]
 
 [[package]]
 name = "certifi"
 version = "2023.5.7"
 description = "Python package for providing Mozilla's CA Bundle."
-category = "main"
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "certifi-2023.5.7-py3-none-any.whl", hash = "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"},
     {file = "certifi-2023.5.7.tar.gz", hash = "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7"},
 ]
 
 [[package]]
 name = "charset-normalizer"
 version = "3.1.0"
 description = "The Real First Universal Charset Detector. Open, modern and actively maintained alternative to Chardet."
-category = "dev"
 optional = false
 python-versions = ">=3.7.0"
 files = [
     {file = "charset-normalizer-3.1.0.tar.gz", hash = "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5"},
     {file = "charset_normalizer-3.1.0-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b"},
     {file = "charset_normalizer-3.1.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60"},
     {file = "charset_normalizer-3.1.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1"},
@@ -297,57 +285,53 @@
     {file = "charset_normalizer-3.1.0-py3-none-any.whl", hash = "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d"},
 ]
 
 [[package]]
 name = "click"
 version = "8.1.3"
 description = "Composable command line interface toolkit"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "click-8.1.3-py3-none-any.whl", hash = "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"},
     {file = "click-8.1.3.tar.gz", hash = "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e"},
 ]
 
 [package.dependencies]
 colorama = {version = "*", markers = "platform_system == \"Windows\""}
 
 [[package]]
 name = "colorama"
 version = "0.4.6"
 description = "Cross-platform colored terminal text."
-category = "main"
 optional = false
 python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*,>=2.7"
 files = [
     {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
     {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
 ]
 
 [[package]]
 name = "colorful"
 version = "0.5.5"
 description = "Terminal string styling done right, in Python."
-category = "main"
 optional = false
 python-versions = "*"
 files = [
     {file = "colorful-0.5.5-py2.py3-none-any.whl", hash = "sha256:62c187e27c1433db9463ff93b1451898d1e7e23a7e553583fd9daeb6325182e4"},
     {file = "colorful-0.5.5.tar.gz", hash = "sha256:66f8c1264b2a26f7293b96a03bb7a76c4bc8b9634369a0bffdcd12d618056a1d"},
 ]
 
 [package.dependencies]
 colorama = {version = "*", markers = "platform_system == \"Windows\""}
 
 [[package]]
 name = "coverage"
 version = "7.2.7"
 description = "Code coverage measurement for Python"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "coverage-7.2.7-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8"},
     {file = "coverage-7.2.7-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb"},
     {file = "coverage-7.2.7-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6"},
     {file = "coverage-7.2.7-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2"},
@@ -412,57 +396,53 @@
 [package.extras]
 toml = ["tomli"]
 
 [[package]]
 name = "dill"
 version = "0.3.6"
 description = "serialize all of python"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "dill-0.3.6-py3-none-any.whl", hash = "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0"},
     {file = "dill-0.3.6.tar.gz", hash = "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"},
 ]
 
 [package.extras]
 graph = ["objgraph (>=1.7.2)"]
 
 [[package]]
 name = "docutils"
 version = "0.19"
 description = "Docutils -- Python Documentation Utilities"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "docutils-0.19-py3-none-any.whl", hash = "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"},
     {file = "docutils-0.19.tar.gz", hash = "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6"},
 ]
 
 [[package]]
 name = "exceptiongroup"
 version = "1.1.1"
 description = "Backport of PEP 654 (exception groups)"
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "exceptiongroup-1.1.1-py3-none-any.whl", hash = "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e"},
     {file = "exceptiongroup-1.1.1.tar.gz", hash = "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"},
 ]
 
 [package.extras]
 test = ["pytest (>=6)"]
 
 [[package]]
 name = "furo"
 version = "2023.5.20"
 description = "A clean customisable Sphinx documentation theme."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "furo-2023.5.20-py3-none-any.whl", hash = "sha256:594a8436ddfe0c071f3a9e9a209c314a219d8341f3f1af33fdf7c69544fab9e6"},
     {file = "furo-2023.5.20.tar.gz", hash = "sha256:40e09fa17c6f4b22419d122e933089226dcdb59747b5b6c79363089827dea16f"},
 ]
 
@@ -472,27 +452,25 @@
 sphinx = ">=6.0,<8.0"
 sphinx-basic-ng = "*"
 
 [[package]]
 name = "h11"
 version = "0.14.0"
 description = "A pure-Python, bring-your-own-I/O implementation of HTTP/1.1"
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "h11-0.14.0-py3-none-any.whl", hash = "sha256:e3fe4ac4b851c468cc8363d500db52c2ead036020723024a109d37346efaa761"},
     {file = "h11-0.14.0.tar.gz", hash = "sha256:8f19fbbe99e72420ff35c00b27a34cb9937e902a8b810e2c88300c6f0a3b699d"},
 ]
 
 [[package]]
 name = "h2"
 version = "4.1.0"
 description = "HTTP/2 State-Machine based protocol implementation"
-category = "main"
 optional = false
 python-versions = ">=3.6.1"
 files = [
     {file = "h2-4.1.0-py3-none-any.whl", hash = "sha256:03a46bcf682256c95b5fd9e9a99c1323584c3eec6440d379b9903d709476bc6d"},
     {file = "h2-4.1.0.tar.gz", hash = "sha256:a83aca08fbe7aacb79fec788c9c0bac936343560ed9ec18b82a13a12c28d2abb"},
 ]
 
@@ -500,49 +478,46 @@
 hpack = ">=4.0,<5"
 hyperframe = ">=6.0,<7"
 
 [[package]]
 name = "hpack"
 version = "4.0.0"
 description = "Pure-Python HPACK header compression"
-category = "main"
 optional = false
 python-versions = ">=3.6.1"
 files = [
     {file = "hpack-4.0.0-py3-none-any.whl", hash = "sha256:84a076fad3dc9a9f8063ccb8041ef100867b1878b25ef0ee63847a5d53818a6c"},
     {file = "hpack-4.0.0.tar.gz", hash = "sha256:fc41de0c63e687ebffde81187a948221294896f6bdc0ae2312708df339430095"},
 ]
 
 [[package]]
 name = "httpcore"
 version = "0.17.2"
 description = "A minimal low-level HTTP client."
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "httpcore-0.17.2-py3-none-any.whl", hash = "sha256:5581b9c12379c4288fe70f43c710d16060c10080617001e6b22a3b6dbcbefd36"},
     {file = "httpcore-0.17.2.tar.gz", hash = "sha256:125f8375ab60036db632f34f4b627a9ad085048eef7cb7d2616fea0f739f98af"},
 ]
 
 [package.dependencies]
 anyio = ">=3.0,<5.0"
 certifi = "*"
 h11 = ">=0.13,<0.15"
-sniffio = ">=1.0.0,<2.0.0"
+sniffio = "==1.*"
 
 [package.extras]
 http2 = ["h2 (>=3,<5)"]
-socks = ["socksio (>=1.0.0,<2.0.0)"]
+socks = ["socksio (==1.*)"]
 
 [[package]]
 name = "httpx"
 version = "0.24.1"
 description = "The next generation HTTP client."
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "httpx-0.24.1-py3-none-any.whl", hash = "sha256:06781eb9ac53cde990577af654bd990a4949de37a28bdb4a230d434f3a30b9bd"},
     {file = "httpx-0.24.1.tar.gz", hash = "sha256:5853a43053df830c20f8110c5e69fe44d035d850b2dfe795e196f00fdb774bdd"},
 ]
 
@@ -551,59 +526,55 @@
 h2 = {version = ">=3,<5", optional = true, markers = "extra == \"http2\""}
 httpcore = ">=0.15.0,<0.18.0"
 idna = "*"
 sniffio = "*"
 
 [package.extras]
 brotli = ["brotli", "brotlicffi"]
-cli = ["click (>=8.0.0,<9.0.0)", "pygments (>=2.0.0,<3.0.0)", "rich (>=10,<14)"]
+cli = ["click (==8.*)", "pygments (==2.*)", "rich (>=10,<14)"]
 http2 = ["h2 (>=3,<5)"]
-socks = ["socksio (>=1.0.0,<2.0.0)"]
+socks = ["socksio (==1.*)"]
 
 [[package]]
 name = "hyperframe"
 version = "6.0.1"
 description = "HTTP/2 framing layer for Python"
-category = "main"
 optional = false
 python-versions = ">=3.6.1"
 files = [
     {file = "hyperframe-6.0.1-py3-none-any.whl", hash = "sha256:0ec6bafd80d8ad2195c4f03aacba3a8265e57bc4cff261e802bf39970ed02a15"},
     {file = "hyperframe-6.0.1.tar.gz", hash = "sha256:ae510046231dc8e9ecb1a6586f63d2347bf4c8905914aa84ba585ae85f28a914"},
 ]
 
 [[package]]
 name = "idna"
 version = "3.4"
 description = "Internationalized Domain Names in Applications (IDNA)"
-category = "main"
 optional = false
 python-versions = ">=3.5"
 files = [
     {file = "idna-3.4-py3-none-any.whl", hash = "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"},
     {file = "idna-3.4.tar.gz", hash = "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4"},
 ]
 
 [[package]]
 name = "imagesize"
 version = "1.4.1"
 description = "Getting image size from png/jpeg/jpeg2000/gif file"
-category = "dev"
 optional = false
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
 files = [
     {file = "imagesize-1.4.1-py2.py3-none-any.whl", hash = "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b"},
     {file = "imagesize-1.4.1.tar.gz", hash = "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"},
 ]
 
 [[package]]
 name = "importlib-metadata"
 version = "6.6.0"
 description = "Read metadata from Python packages"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "importlib_metadata-6.6.0-py3-none-any.whl", hash = "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed"},
     {file = "importlib_metadata-6.6.0.tar.gz", hash = "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"},
 ]
 
@@ -615,15 +586,14 @@
 perf = ["ipython"]
 testing = ["flake8 (<5)", "flufl.flake8", "importlib-resources (>=1.3)", "packaging", "pyfakefs", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)", "pytest-perf (>=0.9.2)"]
 
 [[package]]
 name = "isort"
 version = "5.12.0"
 description = "A Python utility / library to sort Python imports."
-category = "dev"
 optional = false
 python-versions = ">=3.8.0"
 files = [
     {file = "isort-5.12.0-py3-none-any.whl", hash = "sha256:f84c2818376e66cf843d497486ea8fed8700b340f308f076c6fb1229dff318b6"},
     {file = "isort-5.12.0.tar.gz", hash = "sha256:8bef7dde241278824a6d83f44a544709b065191b95b6e50894bdc722fcba0504"},
 ]
 
@@ -633,15 +603,14 @@
 plugins = ["setuptools"]
 requirements-deprecated-finder = ["pip-api", "pipreqs"]
 
 [[package]]
 name = "jinja2"
 version = "3.1.2"
 description = "A very fast and expressive template engine."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "Jinja2-3.1.2-py3-none-any.whl", hash = "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"},
     {file = "Jinja2-3.1.2.tar.gz", hash = "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852"},
 ]
 
@@ -651,15 +620,14 @@
 [package.extras]
 i18n = ["Babel (>=2.7)"]
 
 [[package]]
 name = "lazy-object-proxy"
 version = "1.9.0"
 description = "A fast and thorough lazy object proxy."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "lazy-object-proxy-1.9.0.tar.gz", hash = "sha256:659fb5809fa4629b8a1ac5106f669cfc7bef26fbb389dda53b3e010d1ac4ebae"},
     {file = "lazy_object_proxy-1.9.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:b40387277b0ed2d0602b8293b94d7257e17d1479e257b4de114ea11a8cb7f2d7"},
     {file = "lazy_object_proxy-1.9.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e8c6cfb338b133fbdbc5cfaa10fe3c6aeea827db80c978dbd13bc9dd8526b7d4"},
     {file = "lazy_object_proxy-1.9.0-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:721532711daa7db0d8b779b0bb0318fa87af1c10d7fe5e52ef30f8eff254d0cd"},
@@ -697,15 +665,14 @@
     {file = "lazy_object_proxy-1.9.0-cp39-cp39-win_amd64.whl", hash = "sha256:db1c1722726f47e10e0b5fdbf15ac3b8adb58c091d12b3ab713965795036985f"},
 ]
 
 [[package]]
 name = "livereload"
 version = "2.6.3"
 description = "Python LiveReload is an awesome tool for web developers"
-category = "dev"
 optional = false
 python-versions = "*"
 files = [
     {file = "livereload-2.6.3-py2.py3-none-any.whl", hash = "sha256:ad4ac6f53b2d62bb6ce1a5e6e96f1f00976a32348afedcb4b6d68df2a1d346e4"},
     {file = "livereload-2.6.3.tar.gz", hash = "sha256:776f2f865e59fde56490a56bcc6773b6917366bce0c267c60ee8aaf1a0959869"},
 ]
 
@@ -713,15 +680,14 @@
 six = "*"
 tornado = {version = "*", markers = "python_version > \"2.7\""}
 
 [[package]]
 name = "lxml"
 version = "4.9.2"
 description = "Powerful and Pythonic XML processing library combining libxml2/libxslt with the ElementTree API."
-category = "main"
 optional = false
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, != 3.4.*"
 files = [
     {file = "lxml-4.9.2-cp27-cp27m-macosx_10_15_x86_64.whl", hash = "sha256:76cf573e5a365e790396a5cc2b909812633409306c6531a6877c59061e42c4f2"},
     {file = "lxml-4.9.2-cp27-cp27m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:b1f42b6921d0e81b1bcb5e395bc091a70f41c4d4e55ba99c6da2b31626c44892"},
     {file = "lxml-4.9.2-cp27-cp27m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:9f102706d0ca011de571de32c3247c6476b55bb6bc65a20f682f000b07a4852a"},
     {file = "lxml-4.9.2-cp27-cp27m-win32.whl", hash = "sha256:8d0b4612b66ff5d62d03bcaa043bb018f74dfea51184e53f067e6fdcba4bd8de"},
@@ -806,15 +772,14 @@
 htmlsoup = ["BeautifulSoup4"]
 source = ["Cython (>=0.29.7)"]
 
 [[package]]
 name = "markdown-it-py"
 version = "2.2.0"
 description = "Python port of markdown-it. Markdown parsing, done right!"
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "markdown-it-py-2.2.0.tar.gz", hash = "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"},
     {file = "markdown_it_py-2.2.0-py3-none-any.whl", hash = "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30"},
 ]
 
@@ -831,15 +796,14 @@
 rtd = ["attrs", "myst-parser", "pyyaml", "sphinx", "sphinx-copybutton", "sphinx-design", "sphinx_book_theme"]
 testing = ["coverage", "pytest", "pytest-cov", "pytest-regressions"]
 
 [[package]]
 name = "markupsafe"
 version = "2.1.3"
 description = "Safely add untrusted strings to HTML/XML markup."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "MarkupSafe-2.1.3-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa"},
     {file = "MarkupSafe-2.1.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57"},
     {file = "MarkupSafe-2.1.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f"},
     {file = "MarkupSafe-2.1.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52"},
@@ -891,27 +855,25 @@
     {file = "MarkupSafe-2.1.3.tar.gz", hash = "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad"},
 ]
 
 [[package]]
 name = "mccabe"
 version = "0.7.0"
 description = "McCabe checker, plugin for flake8"
-category = "dev"
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "mccabe-0.7.0-py2.py3-none-any.whl", hash = "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"},
     {file = "mccabe-0.7.0.tar.gz", hash = "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325"},
 ]
 
 [[package]]
 name = "mdit-py-plugins"
 version = "0.3.5"
 description = "Collection of plugins for markdown-it-py"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "mdit-py-plugins-0.3.5.tar.gz", hash = "sha256:eee0adc7195e5827e17e02d2a258a2ba159944a0748f59c5099a4a27f78fcf6a"},
     {file = "mdit_py_plugins-0.3.5-py3-none-any.whl", hash = "sha256:ca9a0714ea59a24b2b044a1831f48d817dd0c817e84339f20e7889f392d77c4e"},
 ]
 
@@ -923,39 +885,36 @@
 rtd = ["attrs", "myst-parser (>=0.16.1,<0.17.0)", "sphinx-book-theme (>=0.1.0,<0.2.0)"]
 testing = ["coverage", "pytest", "pytest-cov", "pytest-regressions"]
 
 [[package]]
 name = "mdurl"
 version = "0.1.2"
 description = "Markdown URL utilities"
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "mdurl-0.1.2-py3-none-any.whl", hash = "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8"},
     {file = "mdurl-0.1.2.tar.gz", hash = "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"},
 ]
 
 [[package]]
 name = "mypy-extensions"
 version = "1.0.0"
 description = "Type system extensions for programs checked with the mypy type checker."
-category = "dev"
 optional = false
 python-versions = ">=3.5"
 files = [
     {file = "mypy_extensions-1.0.0-py3-none-any.whl", hash = "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d"},
     {file = "mypy_extensions-1.0.0.tar.gz", hash = "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"},
 ]
 
 [[package]]
 name = "myst-parser"
 version = "1.0.0"
 description = "An extended [CommonMark](https://spec.commonmark.org/) compliant parser,"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "myst-parser-1.0.0.tar.gz", hash = "sha256:502845659313099542bd38a2ae62f01360e7dd4b1310f025dd014dfc0439cdae"},
     {file = "myst_parser-1.0.0-py3-none-any.whl", hash = "sha256:69fb40a586c6fa68995e6521ac0a525793935db7e724ca9bac1d33be51be9a4c"},
 ]
 
@@ -974,70 +933,65 @@
 testing = ["beautifulsoup4", "coverage[toml]", "pytest (>=7,<8)", "pytest-cov", "pytest-param-files (>=0.3.4,<0.4.0)", "pytest-regressions", "sphinx-pytest"]
 testing-docutils = ["pygments", "pytest (>=7,<8)", "pytest-param-files (>=0.3.4,<0.4.0)"]
 
 [[package]]
 name = "packaging"
 version = "23.1"
 description = "Core utilities for Python packages"
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "packaging-23.1-py3-none-any.whl", hash = "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61"},
     {file = "packaging-23.1.tar.gz", hash = "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"},
 ]
 
 [[package]]
 name = "pathspec"
 version = "0.11.1"
 description = "Utility library for gitignore style pattern matching of file paths."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "pathspec-0.11.1-py3-none-any.whl", hash = "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"},
     {file = "pathspec-0.11.1.tar.gz", hash = "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687"},
 ]
 
 [[package]]
 name = "platformdirs"
-version = "3.5.1"
+version = "3.5.3"
 description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "platformdirs-3.5.1-py3-none-any.whl", hash = "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"},
-    {file = "platformdirs-3.5.1.tar.gz", hash = "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f"},
+    {file = "platformdirs-3.5.3-py3-none-any.whl", hash = "sha256:0ade98a4895e87dc51d47151f7d2ec290365a585151d97b4d8d6312ed6132fed"},
+    {file = "platformdirs-3.5.3.tar.gz", hash = "sha256:e48fabd87db8f3a7df7150a4a5ea22c546ee8bc39bc2473244730d4b56d2cc4e"},
 ]
 
 [package.extras]
-docs = ["furo (>=2023.3.27)", "proselint (>=0.13)", "sphinx (>=6.2.1)", "sphinx-autodoc-typehints (>=1.23,!=1.23.4)"]
-test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.3.1)", "pytest-cov (>=4)", "pytest-mock (>=3.10)"]
+docs = ["furo (>=2023.5.20)", "proselint (>=0.13)", "sphinx (>=7.0.1)", "sphinx-autodoc-typehints (>=1.23,!=1.23.4)"]
+test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.3.1)", "pytest-cov (>=4.1)", "pytest-mock (>=3.10)"]
 
 [[package]]
 name = "pygments"
 version = "2.15.1"
 description = "Pygments is a syntax highlighting package written in Python."
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "Pygments-2.15.1-py3-none-any.whl", hash = "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"},
     {file = "Pygments-2.15.1.tar.gz", hash = "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c"},
 ]
 
 [package.extras]
 plugins = ["importlib-metadata"]
 
 [[package]]
 name = "pylint"
 version = "2.17.4"
 description = "python code static checker"
-category = "dev"
 optional = false
 python-versions = ">=3.7.2"
 files = [
     {file = "pylint-2.17.4-py3-none-any.whl", hash = "sha256:7a1145fb08c251bdb5cca11739722ce64a63db479283d10ce718b2460e54123c"},
     {file = "pylint-2.17.4.tar.gz", hash = "sha256:5dcf1d9e19f41f38e4e85d10f511e5b9c35e1aa74251bf95cdd8cb23584e2db1"},
 ]
 
@@ -1059,30 +1013,28 @@
 spelling = ["pyenchant (>=3.2,<4.0)"]
 testutils = ["gitpython (>3)"]
 
 [[package]]
 name = "python-dateutil"
 version = "2.8.2"
 description = "Extensions to the standard Python datetime module"
-category = "main"
 optional = false
 python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,>=2.7"
 files = [
     {file = "python-dateutil-2.8.2.tar.gz", hash = "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86"},
     {file = "python_dateutil-2.8.2-py2.py3-none-any.whl", hash = "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"},
 ]
 
 [package.dependencies]
 six = ">=1.5"
 
 [[package]]
 name = "pytoolconfig"
 version = "1.2.5"
 description = "Python tool configuration"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "pytoolconfig-1.2.5-py3-none-any.whl", hash = "sha256:239ba9d3e537b91d0243275a497700ea39a5e259ddb80421c366e3b288bf30fe"},
     {file = "pytoolconfig-1.2.5.tar.gz", hash = "sha256:a50f9dfe23b03a9d40414c1fdf902fefbeae12f2ac75a3c8f915944d6ffac279"},
 ]
 
@@ -1097,15 +1049,14 @@
 global = ["platformdirs (>=1.4.4)"]
 validation = ["pydantic (>=1.7.4)"]
 
 [[package]]
 name = "pyyaml"
 version = "6.0"
 description = "YAML parser and emitter for Python"
-category = "dev"
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "PyYAML-6.0-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53"},
     {file = "PyYAML-6.0-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c"},
     {file = "PyYAML-6.0-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc"},
     {file = "PyYAML-6.0-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b"},
@@ -1147,15 +1098,14 @@
     {file = "PyYAML-6.0.tar.gz", hash = "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2"},
 ]
 
 [[package]]
 name = "requests"
 version = "2.31.0"
 description = "Python HTTP for Humans."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "requests-2.31.0-py3-none-any.whl", hash = "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f"},
     {file = "requests-2.31.0.tar.gz", hash = "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"},
 ]
 
@@ -1167,36 +1117,34 @@
 
 [package.extras]
 socks = ["PySocks (>=1.5.6,!=1.5.7)"]
 use-chardet-on-py3 = ["chardet (>=3.0.2,<6)"]
 
 [[package]]
 name = "rich"
-version = "13.4.1"
+version = "13.4.2"
 description = "Render rich text, tables, progress bars, syntax highlighting, markdown and more to the terminal"
-category = "main"
 optional = false
 python-versions = ">=3.7.0"
 files = [
-    {file = "rich-13.4.1-py3-none-any.whl", hash = "sha256:d204aadb50b936bf6b1a695385429d192bc1fdaf3e8b907e8e26f4c4e4b5bf75"},
-    {file = "rich-13.4.1.tar.gz", hash = "sha256:76f6b65ea7e5c5d924ba80e322231d7cb5b5981aa60bfc1e694f1bc097fe6fe1"},
+    {file = "rich-13.4.2-py3-none-any.whl", hash = "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec"},
+    {file = "rich-13.4.2.tar.gz", hash = "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"},
 ]
 
 [package.dependencies]
-markdown-it-py = ">=2.2.0,<3.0.0"
+markdown-it-py = ">=2.2.0"
 pygments = ">=2.13.0,<3.0.0"
 
 [package.extras]
 jupyter = ["ipywidgets (>=7.5.1,<9)"]
 
 [[package]]
 name = "rope"
 version = "1.8.0"
 description = "a python refactoring library..."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "rope-1.8.0-py3-none-any.whl", hash = "sha256:0767424ed40ce237dcf1c1f5088054fef960e5b19f4a0850783a259a3600d7bd"},
     {file = "rope-1.8.0.tar.gz", hash = "sha256:3de1d1f1cf2412540c6a150067fe25298175e7c2b72455b6ca8395f61678da82"},
 ]
 
@@ -1205,77 +1153,71 @@
 
 [package.extras]
 dev = ["build (>=0.7.0)", "pip-tools (>=6.12.1)", "pre-commit (>=2.20.0)", "pytest (>=7.0.1)", "pytest-timeout (>=2.1.0)", "toml (>=0.10.2)"]
 doc = ["pytoolconfig[doc]", "sphinx (>=4.5.0)", "sphinx-autodoc-typehints (>=1.18.1)", "sphinx-rtd-theme (>=1.0.0)"]
 
 [[package]]
 name = "semver"
-version = "3.0.0"
+version = "3.0.1"
 description = "Python helper for Semantic Versioning (https://semver.org)"
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "semver-3.0.0-py3-none-any.whl", hash = "sha256:ab4f69fb1d1ecfb5d81f96411403d7a611fa788c45d252cf5b408025df3ab6ce"},
-    {file = "semver-3.0.0.tar.gz", hash = "sha256:94df43924c4521ec7d307fc86da1531db6c2c33d9d5cdc3e64cca0eb68569269"},
+    {file = "semver-3.0.1-py3-none-any.whl", hash = "sha256:2a23844ba1647362c7490fe3995a86e097bb590d16f0f32dfc383008f19e4cdf"},
+    {file = "semver-3.0.1.tar.gz", hash = "sha256:9ec78c5447883c67b97f98c3b6212796708191d22e4ad30f4570f840171cbce1"},
 ]
 
 [[package]]
 name = "six"
 version = "1.16.0"
 description = "Python 2 and 3 compatibility utilities"
-category = "main"
 optional = false
 python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*"
 files = [
     {file = "six-1.16.0-py2.py3-none-any.whl", hash = "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"},
     {file = "six-1.16.0.tar.gz", hash = "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926"},
 ]
 
 [[package]]
 name = "sniffio"
 version = "1.3.0"
 description = "Sniff out which async library your code is running under"
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "sniffio-1.3.0-py3-none-any.whl", hash = "sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384"},
     {file = "sniffio-1.3.0.tar.gz", hash = "sha256:e60305c5e5d314f5389259b7f22aaa33d8f7dee49763119234af3755c55b9101"},
 ]
 
 [[package]]
 name = "snowballstemmer"
 version = "2.2.0"
 description = "This package provides 29 stemmers for 28 languages generated from Snowball algorithms."
-category = "dev"
 optional = false
 python-versions = "*"
 files = [
     {file = "snowballstemmer-2.2.0-py2.py3-none-any.whl", hash = "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"},
     {file = "snowballstemmer-2.2.0.tar.gz", hash = "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1"},
 ]
 
 [[package]]
 name = "soupsieve"
 version = "2.4.1"
 description = "A modern CSS selector implementation for Beautiful Soup."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "soupsieve-2.4.1-py3-none-any.whl", hash = "sha256:1c1bfee6819544a3447586c889157365a27e10d88cde3ad3da0cf0ddf646feb8"},
     {file = "soupsieve-2.4.1.tar.gz", hash = "sha256:89d12b2d5dfcd2c9e8c22326da9d9aa9cb3dfab0a83a024f05704076ee8d35ea"},
 ]
 
 [[package]]
 name = "sphinx"
 version = "6.2.1"
 description = "Python documentation generator"
-category = "dev"
 optional = false
 python-versions = ">=3.8"
 files = [
     {file = "Sphinx-6.2.1.tar.gz", hash = "sha256:6d56a34697bb749ffa0152feafc4b19836c755d90a7c59b72bc7dfd371b9cc6b"},
     {file = "sphinx-6.2.1-py3-none-any.whl", hash = "sha256:97787ff1fa3256a3eef9eda523a63dbf299f7b47e053cfcf684a1c2a8380c912"},
 ]
 
@@ -1303,15 +1245,14 @@
 lint = ["docutils-stubs", "flake8 (>=3.5.0)", "flake8-simplify", "isort", "mypy (>=0.990)", "ruff", "sphinx-lint", "types-requests"]
 test = ["cython", "filelock", "html5lib", "pytest (>=4.6)"]
 
 [[package]]
 name = "sphinx-autobuild"
 version = "2021.3.14"
 description = "Rebuild Sphinx documentation on changes, with live-reload in the browser."
-category = "dev"
 optional = false
 python-versions = ">=3.6"
 files = [
     {file = "sphinx-autobuild-2021.3.14.tar.gz", hash = "sha256:de1ca3b66e271d2b5b5140c35034c89e47f263f2cd5db302c9217065f7443f05"},
     {file = "sphinx_autobuild-2021.3.14-py3-none-any.whl", hash = "sha256:8fe8cbfdb75db04475232f05187c776f46f6e9e04cacf1e49ce81bdac649ccac"},
 ]
 
@@ -1323,15 +1264,14 @@
 [package.extras]
 test = ["pytest", "pytest-cov"]
 
 [[package]]
 name = "sphinx-basic-ng"
 version = "1.0.0b1"
 description = "A modern skeleton for Sphinx themes."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "sphinx_basic_ng-1.0.0b1-py3-none-any.whl", hash = "sha256:ade597a3029c7865b24ad0eda88318766bcc2f9f4cef60df7e28126fde94db2a"},
     {file = "sphinx_basic_ng-1.0.0b1.tar.gz", hash = "sha256:89374bd3ccd9452a301786781e28c8718e99960f2d4f411845ea75fc7bb5a9b0"},
 ]
 
@@ -1341,15 +1281,14 @@
 [package.extras]
 docs = ["furo", "ipython", "myst-parser", "sphinx-copybutton", "sphinx-inline-tabs"]
 
 [[package]]
 name = "sphinxcontrib-applehelp"
 version = "1.0.4"
 description = "sphinxcontrib-applehelp is a Sphinx extension which outputs Apple help books"
-category = "dev"
 optional = false
 python-versions = ">=3.8"
 files = [
     {file = "sphinxcontrib-applehelp-1.0.4.tar.gz", hash = "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"},
     {file = "sphinxcontrib_applehelp-1.0.4-py3-none-any.whl", hash = "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228"},
 ]
 
@@ -1357,15 +1296,14 @@
 lint = ["docutils-stubs", "flake8", "mypy"]
 test = ["pytest"]
 
 [[package]]
 name = "sphinxcontrib-devhelp"
 version = "1.0.2"
 description = "sphinxcontrib-devhelp is a sphinx extension which outputs Devhelp document."
-category = "dev"
 optional = false
 python-versions = ">=3.5"
 files = [
     {file = "sphinxcontrib-devhelp-1.0.2.tar.gz", hash = "sha256:ff7f1afa7b9642e7060379360a67e9c41e8f3121f2ce9164266f61b9f4b338e4"},
     {file = "sphinxcontrib_devhelp-1.0.2-py2.py3-none-any.whl", hash = "sha256:8165223f9a335cc1af7ffe1ed31d2871f325254c0423bc0c4c7cd1c1e4734a2e"},
 ]
 
@@ -1373,15 +1311,14 @@
 lint = ["docutils-stubs", "flake8", "mypy"]
 test = ["pytest"]
 
 [[package]]
 name = "sphinxcontrib-htmlhelp"
 version = "2.0.1"
 description = "sphinxcontrib-htmlhelp is a sphinx extension which renders HTML help files"
-category = "dev"
 optional = false
 python-versions = ">=3.8"
 files = [
     {file = "sphinxcontrib-htmlhelp-2.0.1.tar.gz", hash = "sha256:0cbdd302815330058422b98a113195c9249825d681e18f11e8b1f78a2f11efff"},
     {file = "sphinxcontrib_htmlhelp-2.0.1-py3-none-any.whl", hash = "sha256:c38cb46dccf316c79de6e5515e1770414b797162b23cd3d06e67020e1d2a6903"},
 ]
 
@@ -1389,30 +1326,28 @@
 lint = ["docutils-stubs", "flake8", "mypy"]
 test = ["html5lib", "pytest"]
 
 [[package]]
 name = "sphinxcontrib-jsmath"
 version = "1.0.1"
 description = "A sphinx extension which renders display math in HTML via JavaScript"
-category = "dev"
 optional = false
 python-versions = ">=3.5"
 files = [
     {file = "sphinxcontrib-jsmath-1.0.1.tar.gz", hash = "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"},
     {file = "sphinxcontrib_jsmath-1.0.1-py2.py3-none-any.whl", hash = "sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178"},
 ]
 
 [package.extras]
 test = ["flake8", "mypy", "pytest"]
 
 [[package]]
 name = "sphinxcontrib-qthelp"
 version = "1.0.3"
 description = "sphinxcontrib-qthelp is a sphinx extension which outputs QtHelp document."
-category = "dev"
 optional = false
 python-versions = ">=3.5"
 files = [
     {file = "sphinxcontrib-qthelp-1.0.3.tar.gz", hash = "sha256:4c33767ee058b70dba89a6fc5c1892c0d57a54be67ddd3e7875a18d14cba5a72"},
     {file = "sphinxcontrib_qthelp-1.0.3-py2.py3-none-any.whl", hash = "sha256:bd9fc24bcb748a8d51fd4ecaade681350aa63009a347a8c14e637895444dfab6"},
 ]
 
@@ -1420,15 +1355,14 @@
 lint = ["docutils-stubs", "flake8", "mypy"]
 test = ["pytest"]
 
 [[package]]
 name = "sphinxcontrib-serializinghtml"
 version = "1.1.5"
 description = "sphinxcontrib-serializinghtml is a sphinx extension which outputs \"serialized\" HTML files (json and pickle)."
-category = "dev"
 optional = false
 python-versions = ">=3.5"
 files = [
     {file = "sphinxcontrib-serializinghtml-1.1.5.tar.gz", hash = "sha256:aa5f6de5dfdf809ef505c4895e51ef5c9eac17d0f287933eb49ec495280b6952"},
     {file = "sphinxcontrib_serializinghtml-1.1.5-py2.py3-none-any.whl", hash = "sha256:352a9a00ae864471d3a7ead8d7d79f5fc0b57e8b3f95e9867eb9eb28999b92fd"},
 ]
 
@@ -1436,39 +1370,36 @@
 lint = ["docutils-stubs", "flake8", "mypy"]
 test = ["pytest"]
 
 [[package]]
 name = "tomli"
 version = "2.0.1"
 description = "A lil' TOML parser"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "tomli-2.0.1-py3-none-any.whl", hash = "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc"},
     {file = "tomli-2.0.1.tar.gz", hash = "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"},
 ]
 
 [[package]]
 name = "tomlkit"
 version = "0.11.8"
 description = "Style preserving TOML library"
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "tomlkit-0.11.8-py3-none-any.whl", hash = "sha256:8c726c4c202bdb148667835f68d68780b9a003a9ec34167b6c673b38eff2a171"},
     {file = "tomlkit-0.11.8.tar.gz", hash = "sha256:9330fc7faa1db67b541b28e62018c17d20be733177d290a13b24c62d1614e0c3"},
 ]
 
 [[package]]
 name = "tornado"
 version = "6.3.2"
 description = "Tornado is a Python web framework and asynchronous networking library, originally developed at FriendFeed."
-category = "dev"
 optional = false
 python-versions = ">= 3.8"
 files = [
     {file = "tornado-6.3.2-cp38-abi3-macosx_10_9_universal2.whl", hash = "sha256:c367ab6c0393d71171123ca5515c61ff62fe09024fa6bf299cd1339dc9456829"},
     {file = "tornado-6.3.2-cp38-abi3-macosx_10_9_x86_64.whl", hash = "sha256:b46a6ab20f5c7c1cb949c72c1994a4585d2eaa0be4853f50a03b5031e964fc7c"},
     {file = "tornado-6.3.2-cp38-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:c2de14066c4a38b4ecbbcd55c5cc4b5340eb04f1c5e81da7451ef555859c833f"},
     {file = "tornado-6.3.2-cp38-abi3-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:05615096845cf50a895026f749195bf0b10b8909f9be672f50b0fe69cba368e4"},
@@ -1481,45 +1412,42 @@
     {file = "tornado-6.3.2.tar.gz", hash = "sha256:4b927c4f19b71e627b13f3db2324e4ae660527143f9e1f2e2fb404f3a187e2ba"},
 ]
 
 [[package]]
 name = "typing-extensions"
 version = "4.6.3"
 description = "Backported and Experimental Type Hints for Python 3.7+"
-category = "main"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "typing_extensions-4.6.3-py3-none-any.whl", hash = "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26"},
     {file = "typing_extensions-4.6.3.tar.gz", hash = "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"},
 ]
 
 [[package]]
 name = "urllib3"
-version = "2.0.2"
+version = "2.0.3"
 description = "HTTP library with thread-safe connection pooling, file post, and more."
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "urllib3-2.0.2-py3-none-any.whl", hash = "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"},
-    {file = "urllib3-2.0.2.tar.gz", hash = "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc"},
+    {file = "urllib3-2.0.3-py3-none-any.whl", hash = "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1"},
+    {file = "urllib3-2.0.3.tar.gz", hash = "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"},
 ]
 
 [package.extras]
 brotli = ["brotli (>=1.0.9)", "brotlicffi (>=0.8.0)"]
 secure = ["certifi", "cryptography (>=1.9)", "idna (>=2.0.0)", "pyopenssl (>=17.1.0)", "urllib3-secure-extra"]
 socks = ["pysocks (>=1.5.6,!=1.5.7,<2.0)"]
 zstd = ["zstandard (>=0.18.0)"]
 
 [[package]]
 name = "wrapt"
 version = "1.15.0"
 description = "Module for decorators, wrappers and monkey patching."
-category = "dev"
 optional = false
 python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,>=2.7"
 files = [
     {file = "wrapt-1.15.0-cp27-cp27m-macosx_10_9_x86_64.whl", hash = "sha256:ca1cccf838cd28d5a0883b342474c630ac48cac5df0ee6eacc9c7290f76b11c1"},
     {file = "wrapt-1.15.0-cp27-cp27m-manylinux1_i686.whl", hash = "sha256:e826aadda3cae59295b95343db8f3d965fb31059da7de01ee8d1c40a60398b29"},
     {file = "wrapt-1.15.0-cp27-cp27m-manylinux1_x86_64.whl", hash = "sha256:5fc8e02f5984a55d2c653f5fea93531e9836abbd84342c1d1e17abc4a15084c2"},
     {file = "wrapt-1.15.0-cp27-cp27m-manylinux2010_i686.whl", hash = "sha256:96e25c8603a155559231c19c0349245eeb4ac0096fe3c1d0be5c47e075bd4f46"},
@@ -1596,15 +1524,14 @@
     {file = "wrapt-1.15.0.tar.gz", hash = "sha256:d06730c6aed78cee4126234cf2d071e01b44b915e725a6cb439a879ec9754a3a"},
 ]
 
 [[package]]
 name = "zipp"
 version = "3.15.0"
 description = "Backport of pathlib-compatible object wrapper for zip files"
-category = "dev"
 optional = false
 python-versions = ">=3.7"
 files = [
     {file = "zipp-3.15.0-py3-none-any.whl", hash = "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"},
     {file = "zipp-3.15.0.tar.gz", hash = "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b"},
 ]
```

### Comparing `pontos-23.6.0/pontos/__init__.py` & `pontos-23.6.1/pontos/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/changelog/__init__.py` & `pontos-23.6.1/pontos/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/changelog/conventional_commits.py` & `pontos-23.6.1/pontos/changelog/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/changelog/errors.py` & `pontos-23.6.1/pontos/changelog/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/changelog/main.py` & `pontos-23.6.1/pontos/changelog/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/errors.py` & `pontos-23.6.1/pontos/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/git/__init__.py` & `pontos-23.6.1/pontos/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/git/git.py` & `pontos-23.6.1/pontos/git/git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/git/status.py` & `pontos-23.6.1/pontos/git/status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/__init__.py` & `pontos-23.6.1/pontos/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/actions/__init__.py` & `pontos-23.6.1/pontos/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/actions/argparser.py` & `pontos-23.6.1/pontos/github/actions/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/actions/cmds.py` & `pontos-23.6.1/pontos/github/actions/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/actions/core.py` & `pontos-23.6.1/pontos/github/actions/core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/actions/env.py` & `pontos-23.6.1/pontos/github/actions/env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/actions/errors.py` & `pontos-23.6.1/pontos/github/actions/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/actions/event.py` & `pontos-23.6.1/pontos/github/actions/event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/actions/main.py` & `pontos-23.6.1/pontos/github/actions/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/api/__init__.py` & `pontos-23.6.1/pontos/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/api/api.py` & `pontos-23.6.1/pontos/github/api/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/api/artifacts.py` & `pontos-23.6.1/pontos/github/api/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/api/branch.py` & `pontos-23.6.1/pontos/github/api/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/api/client.py` & `pontos-23.6.1/pontos/github/api/client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/api/contents.py` & `pontos-23.6.1/pontos/github/api/contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/api/errors.py` & `pontos-23.6.1/pontos/github/api/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/api/helper.py` & `pontos-23.6.1/pontos/github/api/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/api/labels.py` & `pontos-23.6.1/pontos/github/api/labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/api/organizations.py` & `pontos-23.6.1/pontos/github/api/organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/api/pull_requests.py` & `pontos-23.6.1/pontos/github/api/pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/api/release.py` & `pontos-23.6.1/pontos/github/api/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/api/repositories.py` & `pontos-23.6.1/pontos/github/api/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/api/search.py` & `pontos-23.6.1/pontos/github/api/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/api/tags.py` & `pontos-23.6.1/pontos/github/api/tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/api/teams.py` & `pontos-23.6.1/pontos/github/api/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/api/workflows.py` & `pontos-23.6.1/pontos/github/api/workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/argparser.py` & `pontos-23.6.1/pontos/github/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/cmds.py` & `pontos-23.6.1/pontos/github/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/main.py` & `pontos-23.6.1/pontos/github/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/models/__init__.py` & `pontos-23.6.1/pontos/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/models/artifact.py` & `pontos-23.6.1/pontos/github/models/artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/models/base.py` & `pontos-23.6.1/pontos/github/models/base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/models/branch.py` & `pontos-23.6.1/pontos/github/models/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/models/organization.py` & `pontos-23.6.1/pontos/github/models/organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/models/pull_request.py` & `pontos-23.6.1/pontos/github/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/models/release.py` & `pontos-23.6.1/pontos/github/models/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/models/search.py` & `pontos-23.6.1/pontos/github/models/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/models/tag.py` & `pontos-23.6.1/pontos/github/models/tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/models/workflow.py` & `pontos-23.6.1/pontos/github/models/workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/pr_template.md` & `pontos-23.6.1/pontos/github/pr_template.md`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/script/__init__.py` & `pontos-23.6.1/pontos/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/script/errors.py` & `pontos-23.6.1/pontos/github/script/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/script/load.py` & `pontos-23.6.1/pontos/github/script/load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/github/script/parser.py` & `pontos-23.6.1/pontos/github/script/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/helper.py` & `pontos-23.6.1/pontos/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/models/__init__.py` & `pontos-23.6.1/pontos/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/nvd/__init__.py` & `pontos-23.6.1/pontos/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/nvd/api.py` & `pontos-23.6.1/pontos/nvd/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/nvd/cpe/__init__.py` & `pontos-23.6.1/pontos/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/nvd/cpe/api.py` & `pontos-23.6.1/pontos/nvd/cpe/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/nvd/cve/__init__.py` & `pontos-23.6.1/pontos/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/nvd/cve/api.py` & `pontos-23.6.1/pontos/nvd/cve/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/nvd/models/__init__.py` & `pontos-23.6.1/pontos/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/nvd/models/cpe.py` & `pontos-23.6.1/pontos/nvd/models/cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/nvd/models/cve.py` & `pontos-23.6.1/pontos/nvd/models/cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/nvd/models/cvss_v2.py` & `pontos-23.6.1/pontos/nvd/models/cvss_v2.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/nvd/models/cvss_v3.py` & `pontos-23.6.1/pontos/nvd/models/cvss_v3.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/pontos.py` & `pontos-23.6.1/pontos/pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/release/__init__.py` & `pontos-23.6.1/pontos/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/release/helper.py` & `pontos-23.6.1/pontos/release/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/release/main.py` & `pontos-23.6.1/pontos/release/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/release/parser.py` & `pontos-23.6.1/pontos/release/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/release/release.py` & `pontos-23.6.1/pontos/release/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/release/sign.py` & `pontos-23.6.1/pontos/release/sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/terminal/__init__.py` & `pontos-23.6.1/pontos/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/terminal/null.py` & `pontos-23.6.1/pontos/terminal/null.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/terminal/rich.py` & `pontos-23.6.1/pontos/terminal/rich.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/terminal/terminal.py` & `pontos-23.6.1/pontos/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/testing/__init__.py` & `pontos-23.6.1/pontos/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/updateheader/__init__.py` & `pontos-23.6.1/pontos/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/updateheader/__main__.py` & `pontos-23.6.1/pontos/updateheader/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/updateheader/updateheader.py` & `pontos-23.6.1/pontos/updateheader/updateheader.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/version/__init__.py` & `pontos-23.6.1/pontos/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/version/__main__.py` & `pontos-23.6.1/pontos/version/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/version/_calculator.py` & `pontos-23.6.1/pontos/version/_calculator.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/version/commands/__init__.py` & `pontos-23.6.1/pontos/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/version/commands/_cargo.py` & `pontos-23.6.1/pontos/version/commands/_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/version/commands/_cmake.py` & `pontos-23.6.1/pontos/version/commands/_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/version/commands/_command.py` & `pontos-23.6.1/pontos/version/commands/_command.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/version/commands/_go.py` & `pontos-23.6.1/pontos/version/commands/_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/version/commands/_java.py` & `pontos-23.6.1/pontos/version/project.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2020-2022 Greenbone AG
+# Copyright (C) 2023 Greenbone AG
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,111 +11,107 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from typing import Literal, Optional, Union
 
-from lxml import etree
+from typing import List, Literal, Union
 
-from ..errors import VersionError
-from ..schemes import PEP440VersioningScheme
-from ..version import Version, VersionUpdate
-from ._command import VersionCommand
+from .commands import VersionCommand, get_commands
+from .errors import ProjectError
+from .schemes import VersioningScheme
+from .version import Version, VersionUpdate
 
-TEMPLATE = """# pylint: disable=invalid-name
+__all__ = ("Project",)
 
-# THIS IS AN AUTOGENERATED FILE. DO NOT TOUCH!
 
-__version__ = "{}"\n"""
+class Project:
+    """
+    A project for handling versioning
 
+    Example:
+        .. code-block:: python
 
-# This class is used for Java Version command(s)
-class JavaVersionCommand(VersionCommand):
-    project_file_name = "pom.xml"
-    _pom_xml: Optional[etree.Element] = None
+            from pontos.version.scheme import PEP440VersioningScheme
+            from pontos.version.project import Project
 
-    def _get_version_from_pom_xml(self) -> Version:
-        """
-        Return the version information from the <version> tag of the
-        pom.xml file. The version may be in non standardized form.
-        """
-
-        pom_xml: etree.Element = self.pom_xml
+            project = Project(PEP440VersioningScheme)
+    """
 
-        version_element = pom_xml.find("{*}version")
-        if version_element is None:
-            raise VersionError("Version tag missing in pom.xml")
+    def __init__(self, versioning_scheme: VersioningScheme) -> None:
+        """
+        Creates a new project instance
 
-        return PEP440VersioningScheme.parse_version(version_element.text)
+        Args:
+            versioning_scheme: Scheme for version handling
 
-    def _update_pom_version(
-        self,
-        new_version: Version,
-    ) -> None:
+        Raises:
+            ProjectError: If no fitting VersionCommand could be found
         """
-        Update the version in the pom.xml file
+        self._versioning_scheme = versioning_scheme
+        self._commands = self._gather_commands()
+
+    def _gather_commands(self) -> List[VersionCommand]:
         """
-        pom_xml: etree.Element = self.pom_xml
+        Initialize the project with the fitting VersionCommands of the current
+        working directory
 
-        version_element = pom_xml.find("{*}version")
-        if version_element is None:
-            raise VersionError("Version tag missing in pom.xml")
-        version_element.text = str(new_version)
+        Raises:
+            ProjectError: If no fitting VersionCommand could be found
+        """
+        commands = []
+        for cmd in get_commands():
+            command = cmd(versioning_scheme=self._versioning_scheme)
+            if command.project_found():
+                commands.append(command)
 
-        etree.ElementTree(pom_xml).write(
-            self.project_file_path, pretty_print=True, encoding="utf-8"
-        )
+        if not commands:
+            raise ProjectError("No project settings file found")
 
-    @property
-    def pom_xml(self) -> etree.Element:
-        if self._pom_xml is not None:
-            return self._pom_xml
+        return commands
 
-        if not self.project_file_path.exists():
-            raise VersionError("pom.xml file not found.")
+    def update_version(
+        self, new_version: Version, *, force: bool = False
+    ) -> VersionUpdate:
+        """
+        Update the current version of this project
 
-        try:
-            pom_xml: etree.ElementTree = etree.parse(self.project_file_path)
-        except etree.XMLSyntaxError as e:
-            raise VersionError(e) from e
+        Args:
+            new_version: Use this version in the update
+            force: Force updating the version even if the current version is the
+                same as the new version
 
-        self._pom_xml = pom_xml.getroot()
+        Returns:
+            The version update including the changed files
+        """
+        update = self._commands[0].update_version(new_version, force=force)
+        for cmd in self._commands[1:]:
+            next_update = cmd.update_version(new_version, force=force)
+            update.changed_files.extend(next_update.changed_files)
 
-        return self._pom_xml
+        return update
 
     def get_current_version(self) -> Version:
-        """Get the current version of this project
-        In go the version is only defined within the repository
-        tags, thus we need to check git, what tag is the latest"""
-        return self._get_version_from_pom_xml()
+        """
+        Get the current version of the project
+
+        Returns:
+            The current version
+        """
+        return self._commands[0].get_current_version()
 
     def verify_version(
-        self, version: Union[Literal["current"], Version, None]
+        self, version: Union[Literal["current"], Version]
     ) -> None:
-        """Verify the current version of this project"""
-        current_version = self.get_current_version()
-
-        if current_version != version:
-            raise VersionError(
-                f"Provided version {version} does not match the "
-                f"current version {current_version} in "
-                f"{self.project_file_path}."
-            )
+        """
+        Verify the current version of this project
 
-    def update_version(
-        self, new_version: Version, *, force: bool = False
-    ) -> VersionUpdate:
-        package_version = self.get_current_version()
-        if not force and new_version == package_version:
-            return VersionUpdate(previous=package_version, new=new_version)
-
-        changed_files = [self.project_file_path]
-        self._update_pom_version(new_version=new_version)
-
-        return VersionUpdate(
-            previous=package_version,
-            new=new_version,
-            changed_files=changed_files,
-        )
+        Args:
+            version: Version to check against the current applied version of
+                this project. If version is "current" the command should verify
+                if all version information is consistent, for example if the
+                version information in several files is the same.
+        """
+        for cmd in self._commands:
+            cmd.verify_version(version)
```

### Comparing `pontos-23.6.0/pontos/version/commands/_javascript.py` & `pontos-23.6.1/pontos/version/commands/_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/version/commands/_python.py` & `pontos-23.6.1/pontos/version/commands/_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/version/errors.py` & `pontos-23.6.1/pontos/version/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/version/helper.py` & `pontos-23.6.1/pontos/version/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/version/main.py` & `pontos-23.6.1/pontos/version/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/version/parser.py` & `pontos-23.6.1/pontos/version/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/version/schemes/__init__.py` & `pontos-23.6.1/pontos/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/version/schemes/_pep440.py` & `pontos-23.6.1/pontos/version/schemes/_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/version/schemes/_scheme.py` & `pontos-23.6.1/pontos/version/schemes/_scheme.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/version/schemes/_semantic.py` & `pontos-23.6.1/pontos/version/schemes/_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pontos/version/version.py` & `pontos-23.6.1/pontos/version/version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/pyproject.toml` & `pontos-23.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pontos"
-version = "23.6.0"
+version = "23.6.1"
 description = "Common utilities and tools maintained by Greenbone Networks"
 authors = ["Greenbone AG <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/pontos/"
 repository = "https://github.com/greenbone/pontos/"
 documentation = "https://greenbone.github.io/pontos/"
```

### Comparing `pontos-23.6.0/scripts/github/artifacts-download.py` & `pontos-23.6.1/scripts/github/artifacts-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/scripts/github/artifacts.py` & `pontos-23.6.1/scripts/github/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/scripts/github/branchprotection.py` & `pontos-23.6.1/scripts/github/branchprotection.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/scripts/github/create-repository.py` & `pontos-23.6.1/scripts/github/create-repository.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/scripts/github/enforce-admins.py` & `pontos-23.6.1/scripts/github/enforce-admins.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/scripts/github/lock-branch.py` & `pontos-23.6.1/scripts/github/lock-branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/scripts/github/members.py` & `pontos-23.6.1/scripts/github/members.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/scripts/github/release-assets-download.py` & `pontos-23.6.1/scripts/github/release-assets-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/scripts/github/repositories.py` & `pontos-23.6.1/scripts/github/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/scripts/github/search-repositories.py` & `pontos-23.6.1/scripts/github/search-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/scripts/github/team-repositories.py` & `pontos-23.6.1/scripts/github/team-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/scripts/github/teams.py` & `pontos-23.6.1/scripts/github/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/scripts/github/workflow-runs.py` & `pontos-23.6.1/scripts/github/workflow-runs.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/__init__.py` & `pontos-23.6.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/changelog/__init__.py` & `pontos-23.6.1/tests/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/changelog/test_conventional_commits.py` & `pontos-23.6.1/tests/changelog/test_conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/changelog/test_parser.py` & `pontos-23.6.1/tests/changelog/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/git/__init__.py` & `pontos-23.6.1/tests/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/git/test_git.py` & `pontos-23.6.1/tests/git/test_git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/git/test_status.py` & `pontos-23.6.1/tests/git/test_status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/__init__.py` & `pontos-23.6.1/tests/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/actions/__init__.py` & `pontos-23.6.1/tests/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/actions/test-pull-request-event.json` & `pontos-23.6.1/tests/github/actions/test-pull-request-event.json`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/actions/test_core.py` & `pontos-23.6.1/tests/github/actions/test_core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/actions/test_env.py` & `pontos-23.6.1/tests/github/actions/test_env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/actions/test_event.py` & `pontos-23.6.1/tests/github/actions/test_event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/api/__init__.py` & `pontos-23.6.1/tests/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/api/pr-files.json` & `pontos-23.6.1/tests/github/api/pr-files.json`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/api/release-response.json` & `pontos-23.6.1/tests/github/api/release-response.json`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/api/test_artifacts.py` & `pontos-23.6.1/tests/github/api/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/api/test_branch.py` & `pontos-23.6.1/tests/github/api/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/api/test_client.py` & `pontos-23.6.1/tests/github/api/test_client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/api/test_contents.py` & `pontos-23.6.1/tests/github/api/test_contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/api/test_labels.py` & `pontos-23.6.1/tests/github/api/test_labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/api/test_organizations.py` & `pontos-23.6.1/tests/github/api/test_organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/api/test_pull_requests.py` & `pontos-23.6.1/tests/github/api/test_pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/api/test_release.py` & `pontos-23.6.1/tests/github/api/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/api/test_repositories.py` & `pontos-23.6.1/tests/github/api/test_repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/api/test_search.py` & `pontos-23.6.1/tests/github/api/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/api/test_tags.py` & `pontos-23.6.1/tests/github/api/test_tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/api/test_teams.py` & `pontos-23.6.1/tests/github/api/test_teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/api/test_workflows.py` & `pontos-23.6.1/tests/github/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/models/__init__.py` & `pontos-23.6.1/tests/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/models/test_artifact.py` & `pontos-23.6.1/tests/github/models/test_artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/models/test_base.py` & `pontos-23.6.1/tests/github/models/test_base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/models/test_branch.py` & `pontos-23.6.1/tests/github/models/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/models/test_organization.py` & `pontos-23.6.1/tests/github/models/test_organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/models/test_pull_request.py` & `pontos-23.6.1/tests/github/models/test_pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/models/test_release.py` & `pontos-23.6.1/tests/github/models/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/models/test_search.py` & `pontos-23.6.1/tests/github/models/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/models/test_tag.py` & `pontos-23.6.1/tests/github/models/test_tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/models/test_workflow.py` & `pontos-23.6.1/tests/github/models/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/script/__init__.py` & `pontos-23.6.1/tests/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/script/test_load.py` & `pontos-23.6.1/tests/github/script/test_load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/script/test_parser.py` & `pontos-23.6.1/tests/github/script/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/test_argparser.py` & `pontos-23.6.1/tests/github/test_argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/github/test_cmds.py` & `pontos-23.6.1/tests/github/test_cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/models/__init__.py` & `pontos-23.6.1/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/models/test_models.py` & `pontos-23.6.1/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/nvd/__init__.py` & `pontos-23.6.1/tests/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/nvd/cpe/__init__.py` & `pontos-23.6.1/tests/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/nvd/cpe/test_api.py` & `pontos-23.6.1/tests/nvd/cpe/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/nvd/cve/__init__.py` & `pontos-23.6.1/tests/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/nvd/cve/test_api.py` & `pontos-23.6.1/tests/nvd/cve/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/nvd/models/__init__.py` & `pontos-23.6.1/tests/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/nvd/models/test_cpe.py` & `pontos-23.6.1/tests/nvd/models/test_cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/nvd/models/test_cve.py` & `pontos-23.6.1/tests/nvd/models/test_cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/nvd/test_api.py` & `pontos-23.6.1/tests/nvd/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/release/__init__.py` & `pontos-23.6.1/tests/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/release/test_helper.py` & `pontos-23.6.1/tests/release/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/release/test_parser.py` & `pontos-23.6.1/tests/release/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/release/test_release.py` & `pontos-23.6.1/tests/release/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/release/test_sign.py` & `pontos-23.6.1/tests/release/test_sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/terminal/__init__.py` & `pontos-23.6.1/tests/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/terminal/test_terminal.py` & `pontos-23.6.1/tests/terminal/test_terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/test_helper.py` & `pontos-23.6.1/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/test_pontos.py` & `pontos-23.6.1/tests/test_pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/testing/__init__.py` & `pontos-23.6.1/tests/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/testing/test_testing.py` & `pontos-23.6.1/tests/testing/test_testing.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/updateheader/__init__.py` & `pontos-23.6.1/tests/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/updateheader/test_header.py` & `pontos-23.6.1/tests/updateheader/test_header.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/version/__init__.py` & `pontos-23.6.1/tests/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/version/commands/__init__.py` & `pontos-23.6.1/tests/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/version/commands/test_cargo.py` & `pontos-23.6.1/tests/version/commands/test_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/version/commands/test_cmake.py` & `pontos-23.6.1/tests/version/commands/test_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/version/commands/test_go.py` & `pontos-23.6.1/tests/version/commands/test_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/version/commands/test_java.py` & `pontos-23.6.1/tests/version/commands/test_java.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,23 +14,108 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 # pylint: disable=line-too-long
 
 import unittest
+from pathlib import Path
 
 from lxml import etree
 
 from pontos.testing import temp_directory, temp_file
 from pontos.version import VersionError
 from pontos.version.commands import JavaVersionCommand
+from pontos.version.commands._java import find_file, replace_string_in_file
 from pontos.version.schemes import PEP440VersioningScheme
 
 
+class TestFindFile(unittest.TestCase):
+    def test_file_found(self):
+        with temp_directory() as temp_dir:
+            deep_path = Path(temp_dir / "foo/bat/config/swagger/")
+            deep_path.mkdir(parents=True)
+            Path(deep_path / "SwaggerConfig.java").touch()
+            self.assertTrue(
+                Path(
+                    temp_dir / "foo/bat/config/swagger/SwaggerConfig.java"
+                ).exists()
+            )
+            filename = Path("SwaggerConfig.java")
+            search_path = temp_dir  # Assuming 'config/swagger' is two levels up
+            search_glob = "**/config/swagger/*"
+
+            result = find_file(filename, search_path, search_glob)
+
+            self.assertIsNotNone(result)
+            self.assertEqual(result.name, filename.name)
+
+    def test_file_not_found(self):
+        with temp_directory() as temp_dir:
+            Path(
+                temp_dir / "foo/bat/config/swagger/SwaggerConfig.java",
+                parents=True,
+            )
+            filename = Path("NonExistentFile.java")
+            search_path = temp_dir
+            search_glob = "**/config/swagger/*"
+
+            result = find_file(filename, search_path, search_glob)
+
+            self.assertIsNone(result)
+
+
+class TestReplaceString(unittest.TestCase):
+    def test_replace_string_in_file(self):
+        # Define the test parameters
+        content = """
+        Foo, bar
+        baz
+            .version("1.2.3")
+        glubb
+        """
+        pattern = r'.version\("([0-9]+\.[0-9]+\.[0-9]+)"\)'
+        replacement = "1.2.4"
+
+        with temp_file(content=content) as tmp:
+            replace_string_in_file(tmp, pattern, replacement)
+
+            updated_content = tmp.read_text(encoding="utf-8")
+
+            # Verify the replacement was performed correctly
+            self.assertNotRegex(
+                updated_content, "1.2.3"
+            )  # Pattern should not be present
+            self.assertIn(
+                replacement, updated_content
+            )  # Replacement should be present
+
+    def test_replace_string_in_file_no_match(self):
+        # Define the test parameters
+        content = """
+        Foo, bar
+        baz
+            .versio("1.2.3")
+        glubb
+        """
+        pattern = r'.version\("([0-9]+\.[0-9]+\.[0-9]+)"\)'
+        replacement = "1.2.4"
+
+        with temp_file(content=content) as tmp:
+            # Call the function under test
+            replace_string_in_file(tmp, pattern, replacement)
+
+            # Read the content of the unmodified file
+            updated_content = tmp.read_text(encoding="utf-8")
+
+            # Verify the content remains unchanged
+            self.assertNotRegex(updated_content, replacement)
+            self.assertEqual(updated_content, content)
+
+
 class GetCurrentJavaVersionCommandTestCase(unittest.TestCase):
     def test_get_current_version(self):
         content = """<?xml version="1.0" encoding="UTF-8"?>
         <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 https://maven.apache.org/xsd/maven-4.0.0.xsd">
         <modelVersion>4.0.0</modelVersion><groupId>net.greenbone.umbrella</groupId>
         <artifactId>msspadminservice</artifactId><version>2023.5.3</version></project>"""
         with temp_file(content, name="pom.xml", change_into=True):
```

### Comparing `pontos-23.6.0/tests/version/commands/test_javascript.py` & `pontos-23.6.1/tests/version/commands/test_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/version/commands/test_python.py` & `pontos-23.6.1/tests/version/commands/test_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/version/schemes/__init__.py` & `pontos-23.6.1/tests/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/version/schemes/test_pep440.py` & `pontos-23.6.1/tests/version/schemes/test_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/version/schemes/test_semantic.py` & `pontos-23.6.1/tests/version/schemes/test_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/version/test_commands.py` & `pontos-23.6.1/tests/version/test_commands.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/version/test_errors.py` & `pontos-23.6.1/tests/version/test_errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/version/test_helper.py` & `pontos-23.6.1/tests/version/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/version/test_main.py` & `pontos-23.6.1/tests/version/test_main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/version/test_parser.py` & `pontos-23.6.1/tests/version/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/version/test_project.py` & `pontos-23.6.1/tests/version/test_project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/tests/version/test_version.py` & `pontos-23.6.1/tests/version/test_version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.6.0/PKG-INFO` & `pontos-23.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pontos
-Version: 23.6.0
+Version: 23.6.1
 Summary: Common utilities and tools maintained by Greenbone Networks
 Home-page: https://github.com/greenbone/pontos/
 License: GPL-3.0-or-later
 Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

