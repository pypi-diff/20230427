# Comparing `tmp/pontos-23.4.6.tar.gz` & `tmp/pontos-23.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pontos-23.4.6.tar", max compression
+gzip compressed data, was "pontos-23.4.7.tar", max compression
```

## Comparing `pontos-23.4.6.tar` & `pontos-23.4.7.tar`

### file list

```diff
@@ -1,251 +1,251 @@
--rw-r--r--   0        0        0    35149 2023-04-25 10:07:35.281387 pontos-23.4.6/LICENSE
--rw-r--r--   0        0        0     3349 2023-04-25 10:07:35.281387 pontos-23.4.6/README.md
--rw-r--r--   0        0        0    97087 2023-04-25 10:07:35.285387 pontos-23.4.6/poetry.lock
--rw-r--r--   0        0        0       32 2023-04-25 10:07:35.285387 pontos-23.4.6/poetry.toml
--rw-r--r--   0        0        0      791 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/__init__.py
--rw-r--r--   0        0        0      968 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/changelog/__init__.py
--rw-r--r--   0        0        0     9914 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/changelog/conventional_commits.py
--rw-r--r--   0        0        0      965 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/changelog/errors.py
--rw-r--r--   0        0        0     4427 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/changelog/main.py
--rw-r--r--   0        0        0      806 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/errors.py
--rw-r--r--   0        0        0      882 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/git/__init__.py
--rw-r--r--   0        0        0    16153 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/git/git.py
--rw-r--r--   0        0        0     2538 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/git/status.py
--rw-r--r--   0        0        0      760 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/__init__.py
--rw-r--r--   0        0        0     1154 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/actions/__init__.py
--rw-r--r--   0        0        0     2239 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/actions/argparser.py
--rw-r--r--   0        0        0     1472 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/actions/cmds.py
--rw-r--r--   0        0        0     6158 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/actions/core.py
--rw-r--r--   0        0        0     2426 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/actions/env.py
--rw-r--r--   0        0        0      861 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/actions/errors.py
--rw-r--r--   0        0        0     4173 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/actions/event.py
--rw-r--r--   0        0        0     1100 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/actions/main.py
--rw-r--r--   0        0        0     2047 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/__init__.py
--rw-r--r--   0        0        0     5531 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/api.py
--rw-r--r--   0        0        0     6196 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/artifacts.py
--rw-r--r--   0        0        0    34561 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/branch.py
--rw-r--r--   0        0        0     9395 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/client.py
--rw-r--r--   0        0        0     1844 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/contents.py
--rw-r--r--   0        0        0      845 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/errors.py
--rw-r--r--   0        0        0     1320 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/helper.py
--rw-r--r--   0        0        0     2813 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/labels.py
--rw-r--r--   0        0        0    10311 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/organizations.py
--rw-r--r--   0        0        0    13090 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/pull_requests.py
--rw-r--r--   0        0        0    11942 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/release.py
--rw-r--r--   0        0        0    21512 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/repositories.py
--rw-r--r--   0        0        0     3276 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/search.py
--rw-r--r--   0        0        0     6004 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/tags.py
--rw-r--r--   0        0        0    15207 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/teams.py
--rw-r--r--   0        0        0     9182 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/api/workflows.py
--rw-r--r--   0        0        0    11128 2023-04-25 10:07:35.285387 pontos-23.4.6/pontos/github/argparser.py
--rw-r--r--   0        0        0     8863 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/cmds.py
--rw-r--r--   0        0        0     1347 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/main.py
--rw-r--r--   0        0        0     1114 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/__init__.py
--rw-r--r--   0        0        0     2336 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/artifact.py
--rw-r--r--   0        0        0     7532 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/base.py
--rw-r--r--   0        0        0     6915 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/branch.py
--rw-r--r--   0        0        0    16573 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/organization.py
--rw-r--r--   0        0        0    14248 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/pull_request.py
--rw-r--r--   0        0        0     4607 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/release.py
--rw-r--r--   0        0        0     4299 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/search.py
--rw-r--r--   0        0        0     4606 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/tag.py
--rw-r--r--   0        0        0    11477 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/models/workflow.py
--rw-r--r--   0        0        0      790 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/pr_template.md
--rw-r--r--   0        0        0     3207 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/script/__init__.py
--rw-r--r--   0        0        0      835 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/script/errors.py
--rw-r--r--   0        0        0     4854 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/script/load.py
--rw-r--r--   0        0        0     1495 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/github/script/parser.py
--rw-r--r--   0        0        0    14685 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/helper.py
--rw-r--r--   0        0        0     6211 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/models/__init__.py
--rw-r--r--   0        0        0      821 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/__init__.py
--rw-r--r--   0        0        0     4660 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/api.py
--rw-r--r--   0        0        0     2149 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/cpe/__init__.py
--rw-r--r--   0        0        0     6708 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/cpe/api.py
--rw-r--r--   0        0        0     2618 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/cve/__init__.py
--rw-r--r--   0        0        0    10802 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/cve/api.py
--rw-r--r--   0        0        0      716 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/models/__init__.py
--rw-r--r--   0        0        0     2973 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/models/cpe.py
--rw-r--r--   0        0        0     7250 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/models/cve.py
--rw-r--r--   0        0        0     3254 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/models/cvss_v2.py
--rw-r--r--   0        0        0     4471 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/nvd/models/cvss_v3.py
--rw-r--r--   0        0        0     3400 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/pontos.py
--rw-r--r--   0        0        0        0 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/py.typed
--rw-r--r--   0        0        0     1164 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/release/__init__.py
--rw-r--r--   0        0        0     2472 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/release/helper.py
--rw-r--r--   0        0        0     2127 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/release/main.py
--rw-r--r--   0        0        0     8044 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/release/parser.py
--rw-r--r--   0        0        0    12786 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/release/release.py
--rw-r--r--   0        0        0    12499 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/release/sign.py
--rw-r--r--   0        0        0      886 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/terminal/__init__.py
--rw-r--r--   0        0        0     1770 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/terminal/null.py
--rw-r--r--   0        0        0     4717 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/terminal/rich.py
--rw-r--r--   0        0        0     9416 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/terminal/terminal.py
--rw-r--r--   0        0        0     7231 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/testing/__init__.py
--rw-r--r--   0        0        0      773 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/__init__.py
--rw-r--r--   0        0        0      838 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/__main__.py
--rw-r--r--   0        0        0      102 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       97 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       90 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       93 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       97 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       97 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      224 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       90 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       90 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
--rw-r--r--   0        0        0      100 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       85 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      117 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      117 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0       92 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-only/template.c
--rw-r--r--   0        0        0       92 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-only/template.h
--rw-r--r--   0        0        0      219 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-only/template.nasl
--rw-r--r--   0        0        0      101 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
--rw-r--r--   0        0        0       96 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
--rw-r--r--   0        0        0      101 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       92 2023-04-25 10:07:35.289387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       96 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0    12122 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/updateheader/updateheader.py
--rw-r--r--   0        0        0     1067 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/__init__.py
--rw-r--r--   0        0        0      816 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/__main__.py
--rw-r--r--   0        0        0      103 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/__version__.py
--rw-r--r--   0        0        0     8837 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/_calculator.py
--rw-r--r--   0        0        0     1508 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/commands/__init__.py
--rw-r--r--   0        0        0     2723 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/commands/_cargo.py
--rw-r--r--   0        0        0     7752 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/commands/_cmake.py
--rw-r--r--   0        0        0     2553 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/commands/_command.py
--rw-r--r--   0        0        0     3792 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/commands/_go.py
--rw-r--r--   0        0        0     6263 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/commands/_javascript.py
--rw-r--r--   0        0        0     8216 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/commands/_python.py
--rw-r--r--   0        0        0      961 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/errors.py
--rw-r--r--   0        0        0     2812 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/helper.py
--rw-r--r--   0        0        0     3692 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/main.py
--rw-r--r--   0        0        0     4163 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/parser.py
--rw-r--r--   0        0        0     3750 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/project.py
--rw-r--r--   0        0        0     2163 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/schemes/__init__.py
--rw-r--r--   0        0        0    13419 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/schemes/_pep440.py
--rw-r--r--   0        0        0     2145 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/schemes/_scheme.py
--rw-r--r--   0        0        0    16023 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/schemes/_semantic.py
--rw-r--r--   0        0        0     5317 2023-04-25 10:07:35.293387 pontos-23.4.6/pontos/version/version.py
--rw-r--r--   0        0        0     2895 2023-04-25 10:07:35.293387 pontos-23.4.6/pyproject.toml
--rw-r--r--   0        0        0     1872 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/artifacts-download.py
--rw-r--r--   0        0        0     1862 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/artifacts.py
--rw-r--r--   0        0        0     1605 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/branchprotection.py
--rw-r--r--   0        0        0     5606 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/create-repository.py
--rw-r--r--   0        0        0     2212 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/enforce-admins.py
--rw-r--r--   0        0        0     1834 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/lock-branch.py
--rw-r--r--   0        0        0     2577 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/members.py
--rw-r--r--   0        0        0     2179 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/release-assets-download.py
--rw-r--r--   0        0        0     2294 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/repositories.py
--rw-r--r--   0        0        0     6717 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/search-repositories.py
--rw-r--r--   0        0        0     3689 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/team-repositories.py
--rw-r--r--   0        0        0     1654 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/teams.py
--rw-r--r--   0        0        0     2789 2023-04-25 10:07:35.293387 pontos-23.4.6/scripts/github/workflow-runs.py
--rw-r--r--   0        0        0     1518 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/__init__.py
--rw-r--r--   0        0        0     1031 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/changelog/__init__.py
--rw-r--r--   0        0        0      375 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/changelog/changelog.toml
--rw-r--r--   0        0        0    17750 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/changelog/test_conventional_commits.py
--rw-r--r--   0        0        0     1925 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/changelog/test_parser.py
--rw-r--r--   0        0        0       69 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/fake_pyproject.toml
--rw-r--r--   0        0        0      716 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/git/__init__.py
--rw-r--r--   0        0        0    28296 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/git/test_git.py
--rw-r--r--   0        0        0     4215 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/git/test_status.py
--rw-r--r--   0        0        0      716 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/__init__.py
--rw-r--r--   0        0        0      716 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/actions/__init__.py
--rw-r--r--   0        0        0    29628 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/actions/test-pull-request-event.json
--rw-r--r--   0        0        0     4385 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/actions/test_core.py
--rw-r--r--   0        0        0     3534 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/actions/test_env.py
--rw-r--r--   0        0        0     2086 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/actions/test_event.py
--rw-r--r--   0        0        0     1232 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/api/__init__.py
--rw-r--r--   0        0        0    20021 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/api/pr-files.json
--rw-r--r--   0        0        0     5624 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/api/release-response.json
--rw-r--r--   0        0        0    12076 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/api/test_artifacts.py
--rw-r--r--   0        0        0    20096 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/api/test_branch.py
--rw-r--r--   0        0        0     9619 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/api/test_client.py
--rw-r--r--   0        0        0     2087 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/api/test_contents.py
--rw-r--r--   0        0        0     2801 2023-04-25 10:07:35.293387 pontos-23.4.6/tests/github/api/test_labels.py
--rw-r--r--   0        0        0    71096 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/api/test_organizations.py
--rw-r--r--   0        0        0    58514 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/api/test_pull_requests.py
--rw-r--r--   0        0        0    17774 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/api/test_release.py
--rw-r--r--   0        0        0    37847 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/api/test_repositories.py
--rw-r--r--   0        0        0    24490 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/api/test_search.py
--rw-r--r--   0        0        0     9471 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/api/test_tags.py
--rw-r--r--   0        0        0    39045 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/api/test_teams.py
--rw-r--r--   0        0        0   129346 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/api/test_workflows.py
--rw-r--r--   0        0        0      716 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/__init__.py
--rw-r--r--   0        0        0     3210 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/test_artifact.py
--rw-r--r--   0        0        0     9831 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/test_base.py
--rw-r--r--   0        0        0    31873 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/test_branch.py
--rw-r--r--   0        0        0    19874 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/test_organization.py
--rw-r--r--   0        0        0    80894 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/test_pull_request.py
--rw-r--r--   0        0        0    12062 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/test_release.py
--rw-r--r--   0        0        0     2216 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/test_search.py
--rw-r--r--   0        0        0     3400 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/test_tag.py
--rw-r--r--   0        0        0    41463 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/models/test_workflow.py
--rw-r--r--   0        0        0      716 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/script/__init__.py
--rw-r--r--   0        0        0     3520 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/script/test_load.py
--rw-r--r--   0        0        0     2052 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/script/test_parser.py
--rw-r--r--   0        0        0     6371 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/test_argparser.py
--rw-r--r--   0        0        0     9562 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/github/test_cmds.py
--rw-r--r--   0        0        0      716 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/models/__init__.py
--rw-r--r--   0        0        0     6424 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/models/test_models.py
--rw-r--r--   0        0        0     2505 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/nvd/__init__.py
--rw-r--r--   0        0        0      716 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/nvd/cpe/__init__.py
--rw-r--r--   0        0        0    11271 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/nvd/cpe/test_api.py
--rw-r--r--   0        0        0      716 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/nvd/cve/__init__.py
--rw-r--r--   0        0        0    26602 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/nvd/cve/test_api.py
--rw-r--r--   0        0        0      716 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/nvd/models/__init__.py
--rw-r--r--   0        0        0     3706 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/nvd/models/test_cpe.py
--rw-r--r--   0        0        0    25911 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/nvd/models/test_cve.py
--rw-r--r--   0        0        0     3994 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/nvd/test_api.py
--rw-r--r--   0        0        0      721 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/release/__init__.py
--rw-r--r--   0        0        0     3265 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/release/test_helper.py
--rw-r--r--   0        0        0     8597 2023-04-25 10:07:35.297387 pontos-23.4.6/tests/release/test_parser.py
--rw-r--r--   0        0        0    76187 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/release/test_release.py
--rw-r--r--   0        0        0    25286 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/release/test_sign.py
--rw-r--r--   0        0        0      345 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/release/v1.2.3.md
--rw-r--r--   0        0        0      745 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/terminal/__init__.py
--rw-r--r--   0        0        0     6653 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/terminal/test_terminal.py
--rw-r--r--   0        0        0    19355 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/test_helper.py
--rw-r--r--   0        0        0     1373 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/test_pontos.py
--rw-r--r--   0        0        0      716 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/testing/__init__.py
--rw-r--r--   0        0        0     7785 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/testing/test_testing.py
--rw-r--r--   0        0        0      721 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/updateheader/__init__.py
--rw-r--r--   0        0        0    15842 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/updateheader/test_header.py
--rw-r--r--   0        0        0     1031 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/__init__.py
--rw-r--r--   0        0        0      727 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/commands/__init__.py
--rw-r--r--   0        0        0     3847 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/commands/test_cargo.py
--rw-r--r--   0        0        0    11322 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/commands/test_cmake.py
--rw-r--r--   0        0        0    10400 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/commands/test_go.py
--rw-r--r--   0        0        0    15371 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/commands/test_javascript.py
--rw-r--r--   0        0        0    16667 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/commands/test_python.py
--rw-r--r--   0        0        0      727 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/schemes/__init__.py
--rw-r--r--   0        0        0    25525 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/schemes/test_pep440.py
--rw-r--r--   0        0        0    27735 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/schemes/test_semantic.py
--rw-r--r--   0        0        0      919 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/test_commands.py
--rw-r--r--   0        0        0     1096 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/test_errors.py
--rw-r--r--   0        0        0     7621 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/test_helper.py
--rw-r--r--   0        0        0    10908 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/test_main.py
--rw-r--r--   0        0        0     1131 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/test_parser.py
--rw-r--r--   0        0        0     6187 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/test_project.py
--rw-r--r--   0        0        0     1791 2023-04-25 10:07:35.301387 pontos-23.4.6/tests/version/test_version.py
--rw-r--r--   0        0        0     4816 1970-01-01 00:00:00.000000 pontos-23.4.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-27 09:37:35.119824 pontos-23.4.7/LICENSE
+-rw-r--r--   0        0        0     3836 2023-04-27 09:37:35.119824 pontos-23.4.7/README.md
+-rw-r--r--   0        0        0    97087 2023-04-27 09:37:35.123824 pontos-23.4.7/poetry.lock
+-rw-r--r--   0        0        0       32 2023-04-27 09:37:35.123824 pontos-23.4.7/poetry.toml
+-rw-r--r--   0        0        0      791 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/__init__.py
+-rw-r--r--   0        0        0      968 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/changelog/__init__.py
+-rw-r--r--   0        0        0     9914 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/changelog/conventional_commits.py
+-rw-r--r--   0        0        0      965 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/changelog/errors.py
+-rw-r--r--   0        0        0     4427 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/changelog/main.py
+-rw-r--r--   0        0        0      806 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/errors.py
+-rw-r--r--   0        0        0      882 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/git/__init__.py
+-rw-r--r--   0        0        0    16153 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/git/git.py
+-rw-r--r--   0        0        0     2538 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/git/status.py
+-rw-r--r--   0        0        0      760 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/__init__.py
+-rw-r--r--   0        0        0     1154 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/actions/__init__.py
+-rw-r--r--   0        0        0     2239 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/actions/argparser.py
+-rw-r--r--   0        0        0     1472 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/actions/cmds.py
+-rw-r--r--   0        0        0     6158 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/actions/core.py
+-rw-r--r--   0        0        0     2426 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/actions/env.py
+-rw-r--r--   0        0        0      861 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/actions/errors.py
+-rw-r--r--   0        0        0     4173 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/actions/event.py
+-rw-r--r--   0        0        0     1100 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/actions/main.py
+-rw-r--r--   0        0        0     2047 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/__init__.py
+-rw-r--r--   0        0        0     5531 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/api.py
+-rw-r--r--   0        0        0     6196 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/artifacts.py
+-rw-r--r--   0        0        0    34561 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/branch.py
+-rw-r--r--   0        0        0     9395 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/client.py
+-rw-r--r--   0        0        0     1844 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/contents.py
+-rw-r--r--   0        0        0      845 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/errors.py
+-rw-r--r--   0        0        0     1320 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/helper.py
+-rw-r--r--   0        0        0     2813 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/labels.py
+-rw-r--r--   0        0        0    10311 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/organizations.py
+-rw-r--r--   0        0        0    13090 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/pull_requests.py
+-rw-r--r--   0        0        0    11942 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/release.py
+-rw-r--r--   0        0        0    21512 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/repositories.py
+-rw-r--r--   0        0        0     3276 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/search.py
+-rw-r--r--   0        0        0     6004 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/tags.py
+-rw-r--r--   0        0        0    15207 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/teams.py
+-rw-r--r--   0        0        0     9182 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/api/workflows.py
+-rw-r--r--   0        0        0    11128 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/argparser.py
+-rw-r--r--   0        0        0     8863 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/cmds.py
+-rw-r--r--   0        0        0     1347 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/main.py
+-rw-r--r--   0        0        0     1114 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/__init__.py
+-rw-r--r--   0        0        0     2336 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/artifact.py
+-rw-r--r--   0        0        0     7532 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/base.py
+-rw-r--r--   0        0        0     6915 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/branch.py
+-rw-r--r--   0        0        0    16573 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/organization.py
+-rw-r--r--   0        0        0    14248 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/pull_request.py
+-rw-r--r--   0        0        0     4607 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/release.py
+-rw-r--r--   0        0        0     4299 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/search.py
+-rw-r--r--   0        0        0     4606 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/tag.py
+-rw-r--r--   0        0        0    11477 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/models/workflow.py
+-rw-r--r--   0        0        0      790 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/pr_template.md
+-rw-r--r--   0        0        0     3207 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/script/__init__.py
+-rw-r--r--   0        0        0      835 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/script/errors.py
+-rw-r--r--   0        0        0     4854 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/script/load.py
+-rw-r--r--   0        0        0     1495 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/github/script/parser.py
+-rw-r--r--   0        0        0    14685 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/helper.py
+-rw-r--r--   0        0        0     6211 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/models/__init__.py
+-rw-r--r--   0        0        0      821 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/nvd/__init__.py
+-rw-r--r--   0        0        0     4660 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/nvd/api.py
+-rw-r--r--   0        0        0     2149 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0     6708 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/nvd/cpe/api.py
+-rw-r--r--   0        0        0     2618 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    10802 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/nvd/cve/api.py
+-rw-r--r--   0        0        0      716 2023-04-27 09:37:35.123824 pontos-23.4.7/pontos/nvd/models/__init__.py
+-rw-r--r--   0        0        0     2973 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/nvd/models/cpe.py
+-rw-r--r--   0        0        0     7250 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/nvd/models/cve.py
+-rw-r--r--   0        0        0     3254 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/nvd/models/cvss_v2.py
+-rw-r--r--   0        0        0     4471 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/nvd/models/cvss_v3.py
+-rw-r--r--   0        0        0     3400 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/pontos.py
+-rw-r--r--   0        0        0        0 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/py.typed
+-rw-r--r--   0        0        0     1164 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/release/__init__.py
+-rw-r--r--   0        0        0     2472 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/release/helper.py
+-rw-r--r--   0        0        0     2127 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/release/main.py
+-rw-r--r--   0        0        0     8333 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/release/parser.py
+-rw-r--r--   0        0        0    13170 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/release/release.py
+-rw-r--r--   0        0        0    12499 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/release/sign.py
+-rw-r--r--   0        0        0      886 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/terminal/__init__.py
+-rw-r--r--   0        0        0     1770 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/terminal/null.py
+-rw-r--r--   0        0        0     4717 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/terminal/rich.py
+-rw-r--r--   0        0        0     9416 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/terminal/terminal.py
+-rw-r--r--   0        0        0     7231 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/testing/__init__.py
+-rw-r--r--   0        0        0      773 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/__init__.py
+-rw-r--r--   0        0        0      838 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/__main__.py
+-rw-r--r--   0        0        0      102 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       97 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       90 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       93 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       97 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       97 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      224 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       90 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       90 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0      100 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       85 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      117 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      117 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0       92 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-only/template.c
+-rw-r--r--   0        0        0       92 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-only/template.h
+-rw-r--r--   0        0        0      219 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-only/template.nasl
+-rw-r--r--   0        0        0      101 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
+-rw-r--r--   0        0        0       96 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
+-rw-r--r--   0        0        0      101 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       92 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       96 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0    12122 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/updateheader/updateheader.py
+-rw-r--r--   0        0        0     1067 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/__init__.py
+-rw-r--r--   0        0        0      816 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/__main__.py
+-rw-r--r--   0        0        0      103 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/__version__.py
+-rw-r--r--   0        0        0     8837 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/_calculator.py
+-rw-r--r--   0        0        0     1508 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/commands/__init__.py
+-rw-r--r--   0        0        0     2723 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/commands/_cargo.py
+-rw-r--r--   0        0        0     7752 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/commands/_cmake.py
+-rw-r--r--   0        0        0     2553 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/commands/_command.py
+-rw-r--r--   0        0        0     3792 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/commands/_go.py
+-rw-r--r--   0        0        0     6263 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/commands/_javascript.py
+-rw-r--r--   0        0        0     8216 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/commands/_python.py
+-rw-r--r--   0        0        0      961 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/errors.py
+-rw-r--r--   0        0        0     2812 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/helper.py
+-rw-r--r--   0        0        0     3692 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/main.py
+-rw-r--r--   0        0        0     4163 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/parser.py
+-rw-r--r--   0        0        0     3750 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/project.py
+-rw-r--r--   0        0        0     2163 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/schemes/__init__.py
+-rw-r--r--   0        0        0    13419 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/schemes/_pep440.py
+-rw-r--r--   0        0        0     2145 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/schemes/_scheme.py
+-rw-r--r--   0        0        0    16023 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/schemes/_semantic.py
+-rw-r--r--   0        0        0     5317 2023-04-27 09:37:35.127824 pontos-23.4.7/pontos/version/version.py
+-rw-r--r--   0        0        0     2895 2023-04-27 09:37:35.127824 pontos-23.4.7/pyproject.toml
+-rw-r--r--   0        0        0     1872 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/artifacts-download.py
+-rw-r--r--   0        0        0     1862 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/artifacts.py
+-rw-r--r--   0        0        0     1605 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/branchprotection.py
+-rw-r--r--   0        0        0     5606 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/create-repository.py
+-rw-r--r--   0        0        0     2212 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/enforce-admins.py
+-rw-r--r--   0        0        0     1834 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/lock-branch.py
+-rw-r--r--   0        0        0     2577 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/members.py
+-rw-r--r--   0        0        0     2179 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/release-assets-download.py
+-rw-r--r--   0        0        0     2294 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/repositories.py
+-rw-r--r--   0        0        0     6717 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/search-repositories.py
+-rw-r--r--   0        0        0     3689 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/team-repositories.py
+-rw-r--r--   0        0        0     1654 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/teams.py
+-rw-r--r--   0        0        0     2789 2023-04-27 09:37:35.127824 pontos-23.4.7/scripts/github/workflow-runs.py
+-rw-r--r--   0        0        0     1518 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/__init__.py
+-rw-r--r--   0        0        0     1031 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/changelog/__init__.py
+-rw-r--r--   0        0        0      375 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/changelog/changelog.toml
+-rw-r--r--   0        0        0    17750 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/changelog/test_conventional_commits.py
+-rw-r--r--   0        0        0     1925 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/changelog/test_parser.py
+-rw-r--r--   0        0        0       69 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/fake_pyproject.toml
+-rw-r--r--   0        0        0      716 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/git/__init__.py
+-rw-r--r--   0        0        0    28296 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/git/test_git.py
+-rw-r--r--   0        0        0     4215 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/git/test_status.py
+-rw-r--r--   0        0        0      716 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/github/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/github/actions/__init__.py
+-rw-r--r--   0        0        0    29628 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/github/actions/test-pull-request-event.json
+-rw-r--r--   0        0        0     4385 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/github/actions/test_core.py
+-rw-r--r--   0        0        0     3534 2023-04-27 09:37:35.127824 pontos-23.4.7/tests/github/actions/test_env.py
+-rw-r--r--   0        0        0     2086 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/actions/test_event.py
+-rw-r--r--   0        0        0     1232 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/__init__.py
+-rw-r--r--   0        0        0    20021 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/pr-files.json
+-rw-r--r--   0        0        0     5624 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/release-response.json
+-rw-r--r--   0        0        0    12076 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_artifacts.py
+-rw-r--r--   0        0        0    20096 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_branch.py
+-rw-r--r--   0        0        0     9619 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_client.py
+-rw-r--r--   0        0        0     2087 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_contents.py
+-rw-r--r--   0        0        0     2801 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_labels.py
+-rw-r--r--   0        0        0    71096 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_organizations.py
+-rw-r--r--   0        0        0    58514 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_pull_requests.py
+-rw-r--r--   0        0        0    17774 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_release.py
+-rw-r--r--   0        0        0    37847 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_repositories.py
+-rw-r--r--   0        0        0    24490 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_search.py
+-rw-r--r--   0        0        0     9471 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_tags.py
+-rw-r--r--   0        0        0    39045 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_teams.py
+-rw-r--r--   0        0        0   129346 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/api/test_workflows.py
+-rw-r--r--   0        0        0      716 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/__init__.py
+-rw-r--r--   0        0        0     3210 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/test_artifact.py
+-rw-r--r--   0        0        0     9831 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/test_base.py
+-rw-r--r--   0        0        0    31873 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/test_branch.py
+-rw-r--r--   0        0        0    19874 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/test_organization.py
+-rw-r--r--   0        0        0    80894 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/test_pull_request.py
+-rw-r--r--   0        0        0    12062 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/test_release.py
+-rw-r--r--   0        0        0     2216 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/test_search.py
+-rw-r--r--   0        0        0     3400 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/test_tag.py
+-rw-r--r--   0        0        0    41463 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/models/test_workflow.py
+-rw-r--r--   0        0        0      716 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/script/__init__.py
+-rw-r--r--   0        0        0     3520 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/script/test_load.py
+-rw-r--r--   0        0        0     2052 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/script/test_parser.py
+-rw-r--r--   0        0        0     6371 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/test_argparser.py
+-rw-r--r--   0        0        0     9562 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/github/test_cmds.py
+-rw-r--r--   0        0        0      716 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/models/__init__.py
+-rw-r--r--   0        0        0     6424 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/models/test_models.py
+-rw-r--r--   0        0        0     2505 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/nvd/__init__.py
+-rw-r--r--   0        0        0      716 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0    11271 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/nvd/cpe/test_api.py
+-rw-r--r--   0        0        0      716 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    26602 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/nvd/cve/test_api.py
+-rw-r--r--   0        0        0      716 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/nvd/models/__init__.py
+-rw-r--r--   0        0        0     3706 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/nvd/models/test_cpe.py
+-rw-r--r--   0        0        0    25911 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/nvd/models/test_cve.py
+-rw-r--r--   0        0        0     3994 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/nvd/test_api.py
+-rw-r--r--   0        0        0      721 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/release/__init__.py
+-rw-r--r--   0        0        0     3265 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/release/test_helper.py
+-rw-r--r--   0        0        0     9077 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/release/test_parser.py
+-rw-r--r--   0        0        0    78709 2023-04-27 09:37:35.131824 pontos-23.4.7/tests/release/test_release.py
+-rw-r--r--   0        0        0    25286 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/release/test_sign.py
+-rw-r--r--   0        0        0      345 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/release/v1.2.3.md
+-rw-r--r--   0        0        0      745 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/terminal/__init__.py
+-rw-r--r--   0        0        0     6653 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/terminal/test_terminal.py
+-rw-r--r--   0        0        0    19355 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/test_helper.py
+-rw-r--r--   0        0        0     1373 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/test_pontos.py
+-rw-r--r--   0        0        0      716 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/testing/__init__.py
+-rw-r--r--   0        0        0     7785 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/testing/test_testing.py
+-rw-r--r--   0        0        0      721 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/updateheader/__init__.py
+-rw-r--r--   0        0        0    15842 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/updateheader/test_header.py
+-rw-r--r--   0        0        0     1031 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/__init__.py
+-rw-r--r--   0        0        0      727 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/commands/__init__.py
+-rw-r--r--   0        0        0     3847 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/commands/test_cargo.py
+-rw-r--r--   0        0        0    11322 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/commands/test_cmake.py
+-rw-r--r--   0        0        0    10400 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/commands/test_go.py
+-rw-r--r--   0        0        0    15371 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/commands/test_javascript.py
+-rw-r--r--   0        0        0    16667 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/commands/test_python.py
+-rw-r--r--   0        0        0      727 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/schemes/__init__.py
+-rw-r--r--   0        0        0    25525 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/schemes/test_pep440.py
+-rw-r--r--   0        0        0    27735 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/schemes/test_semantic.py
+-rw-r--r--   0        0        0      919 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/test_commands.py
+-rw-r--r--   0        0        0     1096 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/test_errors.py
+-rw-r--r--   0        0        0     7621 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/test_helper.py
+-rw-r--r--   0        0        0    10908 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/test_main.py
+-rw-r--r--   0        0        0     1131 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/test_parser.py
+-rw-r--r--   0        0        0     6187 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/test_project.py
+-rw-r--r--   0        0        0     1791 2023-04-27 09:37:35.135824 pontos-23.4.7/tests/version/test_version.py
+-rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 pontos-23.4.7/PKG-INFO
```

### Comparing `pontos-23.4.6/LICENSE` & `pontos-23.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/README.md` & `pontos-23.4.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 the titan of the sea.
 
 ## Table of Contents <!-- omit in toc -->
 
 - [Documentation](#documentation)
 - [Installation](#installation)
   - [Requirements](#requirements)
+  - [Install using pipx](#install-using-pipx)
   - [Install using pip](#install-using-pip)
   - [Install using poetry](#install-using-poetry)
 - [Development](#development)
 - [Maintainer](#maintainer)
 - [Contributing](#contributing)
 - [License](#license)
 
@@ -31,16 +32,27 @@
 
 ## Installation
 
 ### Requirements
 
 Python 3.9 and later is supported.
 
+### Install using pipx
+
+You can install the latest stable release of **pontos** from the Python
+Package Index (pypi) using [pipx]
+
+    python3 -m pipx install pontos
+
 ### Install using pip
 
+**NOTE:** The ‘pip install’ command does no longer work out-of-the-box in newer
+distributions like Ubuntu 23.04 because of [PEP 668](https://peps.python.org/pep-0668).
+Please use the [installation via pipx](#install-using-pipx) instead.
+
 You can install the latest stable release of **pontos** from the Python
 Package Index (pypi) using [pip]
 
     python3 -m pip install --user pontos
 
 ### Install using poetry
 
@@ -54,17 +66,17 @@
     poetry add pontos
 
 ## Development
 
 **pontos** uses [poetry] for its own dependency management and build
 process.
 
-First install poetry via pip
+First install poetry via pipx
 
-    python3 -m pip install --user poetry
+    python3 -m pipx install poetry
 
 Afterwards run
 
     poetry install
 
 in the checkout directory of **pontos** (the directory containing the
 `pyproject.toml` file) to install all dependencies including the packages only
@@ -96,8 +108,9 @@
 Copyright (C) 2020-2023 [Greenbone AG][Greenbone Networks]
 
 Licensed under the [GNU General Public License v3.0 or later](LICENSE).
 
 [Greenbone Networks]: https://www.greenbone.net/
 [poetry]: https://python-poetry.org/
 [pip]: https://pip.pypa.io/
+[pipx]: https://pypa.github.io/pipx/
 [autohooks]: https://github.com/greenbone/autohooks
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pontos-23.4.6/poetry.lock` & `pontos-23.4.7/poetry.lock`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/__init__.py` & `pontos-23.4.7/pontos/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/changelog/__init__.py` & `pontos-23.4.7/pontos/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/changelog/conventional_commits.py` & `pontos-23.4.7/pontos/changelog/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/changelog/errors.py` & `pontos-23.4.7/pontos/changelog/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/changelog/main.py` & `pontos-23.4.7/pontos/changelog/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/errors.py` & `pontos-23.4.7/pontos/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/git/__init__.py` & `pontos-23.4.7/pontos/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/git/git.py` & `pontos-23.4.7/pontos/git/git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/git/status.py` & `pontos-23.4.7/pontos/git/status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/__init__.py` & `pontos-23.4.7/pontos/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/actions/__init__.py` & `pontos-23.4.7/pontos/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/actions/argparser.py` & `pontos-23.4.7/pontos/github/actions/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/actions/cmds.py` & `pontos-23.4.7/pontos/github/actions/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/actions/core.py` & `pontos-23.4.7/pontos/github/actions/core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/actions/env.py` & `pontos-23.4.7/pontos/github/actions/env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/actions/errors.py` & `pontos-23.4.7/pontos/github/actions/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/actions/event.py` & `pontos-23.4.7/pontos/github/actions/event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/actions/main.py` & `pontos-23.4.7/pontos/github/actions/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/api/__init__.py` & `pontos-23.4.7/pontos/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/api/api.py` & `pontos-23.4.7/pontos/github/api/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/api/artifacts.py` & `pontos-23.4.7/pontos/github/api/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/api/branch.py` & `pontos-23.4.7/pontos/github/api/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/api/client.py` & `pontos-23.4.7/pontos/github/api/client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/api/contents.py` & `pontos-23.4.7/pontos/github/api/contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/api/errors.py` & `pontos-23.4.7/pontos/github/api/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/api/helper.py` & `pontos-23.4.7/pontos/github/api/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/api/labels.py` & `pontos-23.4.7/pontos/github/api/labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/api/organizations.py` & `pontos-23.4.7/pontos/github/api/organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/api/pull_requests.py` & `pontos-23.4.7/pontos/github/api/pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/api/release.py` & `pontos-23.4.7/pontos/github/api/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/api/repositories.py` & `pontos-23.4.7/pontos/github/api/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/api/search.py` & `pontos-23.4.7/pontos/github/api/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/api/tags.py` & `pontos-23.4.7/pontos/github/api/tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/api/teams.py` & `pontos-23.4.7/pontos/github/api/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/api/workflows.py` & `pontos-23.4.7/pontos/github/api/workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/argparser.py` & `pontos-23.4.7/pontos/github/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/cmds.py` & `pontos-23.4.7/pontos/github/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/main.py` & `pontos-23.4.7/pontos/github/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/models/__init__.py` & `pontos-23.4.7/pontos/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/models/artifact.py` & `pontos-23.4.7/pontos/github/models/artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/models/base.py` & `pontos-23.4.7/pontos/github/models/base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/models/branch.py` & `pontos-23.4.7/pontos/github/models/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/models/organization.py` & `pontos-23.4.7/pontos/github/models/organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/models/pull_request.py` & `pontos-23.4.7/pontos/github/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/models/release.py` & `pontos-23.4.7/pontos/github/models/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/models/search.py` & `pontos-23.4.7/pontos/github/models/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/models/tag.py` & `pontos-23.4.7/pontos/github/models/tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/models/workflow.py` & `pontos-23.4.7/pontos/github/models/workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/pr_template.md` & `pontos-23.4.7/pontos/github/pr_template.md`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/script/__init__.py` & `pontos-23.4.7/pontos/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/script/errors.py` & `pontos-23.4.7/pontos/github/script/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/script/load.py` & `pontos-23.4.7/pontos/github/script/load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/github/script/parser.py` & `pontos-23.4.7/pontos/github/script/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/helper.py` & `pontos-23.4.7/pontos/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/models/__init__.py` & `pontos-23.4.7/pontos/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/nvd/__init__.py` & `pontos-23.4.7/pontos/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/nvd/api.py` & `pontos-23.4.7/pontos/nvd/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/nvd/cpe/__init__.py` & `pontos-23.4.7/pontos/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/nvd/cpe/api.py` & `pontos-23.4.7/pontos/nvd/cpe/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/nvd/cve/__init__.py` & `pontos-23.4.7/pontos/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/nvd/cve/api.py` & `pontos-23.4.7/pontos/nvd/cve/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/nvd/models/__init__.py` & `pontos-23.4.7/pontos/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/nvd/models/cpe.py` & `pontos-23.4.7/pontos/nvd/models/cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/nvd/models/cve.py` & `pontos-23.4.7/pontos/nvd/models/cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/nvd/models/cvss_v2.py` & `pontos-23.4.7/pontos/nvd/models/cvss_v2.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/nvd/models/cvss_v3.py` & `pontos-23.4.7/pontos/nvd/models/cvss_v3.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/pontos.py` & `pontos-23.4.7/pontos/pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/release/__init__.py` & `pontos-23.4.7/pontos/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/release/helper.py` & `pontos-23.4.7/pontos/release/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/release/main.py` & `pontos-23.4.7/pontos/release/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/release/parser.py` & `pontos-23.4.7/pontos/release/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import argparse
 import os
-from argparse import ArgumentParser, ArgumentTypeError, Namespace
+from argparse import (
+    ArgumentParser,
+    ArgumentTypeError,
+    BooleanOptionalAction,
+    Namespace,
+)
 from enum import Enum
 from pathlib import Path
 from typing import Callable, Tuple, Type
 
 from pontos.release.helper import ReleaseType
 from pontos.version.schemes import (
     VERSIONING_SCHEMES,
@@ -154,14 +159,21 @@
     release_parser.add_argument(
         "--conventional-commits-config",
         dest="cc_config",
         type=Path,
         help="Conventional commits config file (toml), including conventions."
         " If not set defaults are used.",
     )
+    release_parser.add_argument(
+        "--update-project",
+        help="Update version in project files like pyproject.toml. By default "
+        "project files are updated.",
+        action=BooleanOptionalAction,
+        default=True,
+    )
 
     sign_parser = subparsers.add_parser("sign")
     sign_parser.set_defaults(func=sign)
     sign_parser.add_argument(
         "--signing-key",
         default=DEFAULT_SIGNING_KEY,
         help="The key to sign zip, tarballs of a release. Default %(default)s.",
```

### Comparing `pontos-23.4.6/pontos/release/release.py` & `pontos-23.4.7/pontos/release/release.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,15 @@
         next_version: Optional[str],
         git_signing_key: str,
         git_remote_name: Optional[str],
         git_tag_prefix: Optional[str],
         cc_config: Optional[Path],
         local: Optional[bool] = False,
         release_series: Optional[str] = None,
+        update_project: bool = True,
     ) -> ReleaseReturnValue:
         """
         Create a release
 
         Args:
             token: A token for creating a release on GitHub
             space: GitHub username or organization. Required for generating
@@ -180,14 +181,15 @@
                 from the release version.
             cc_config: A path to a settings file for creating conventional
                 commits.
             local: Only create changes locally and don't push changes to
                 remote repository. Also don't create a GitHub release.
             release_series: Optional release series to use.
                 For example: "1.2", "2", "23".
+            update_project: Update version in project files.
         """
         git_signing_key = (
             git_signing_key
             if git_signing_key is not None
             else find_signing_key(self.terminal)
         )
         self.git_tag_prefix = git_tag_prefix or ""
@@ -243,33 +245,36 @@
 
         git_version = f"{self.git_tag_prefix}{release_version}"
 
         if self._has_tag(git_version):
             self.terminal.error(f"Git tag {git_version} already exists.")
             return ReleaseReturnValue.ALREADY_TAKEN
 
-        try:
-            project = Project(versioning_scheme)
-        except PontosError as e:
-            self.terminal.error(f"Unable to determine project settings. {e}")
-            return ReleaseReturnValue.PROJECT_SETTINGS_NOT_FOUND
+        if update_project:
+            try:
+                project = Project(versioning_scheme)
+            except PontosError as e:
+                self.terminal.error(
+                    f"Unable to determine project settings. {e}"
+                )
+                return ReleaseReturnValue.PROJECT_SETTINGS_NOT_FOUND
 
-        try:
-            updated = project.update_version(release_version)
+            try:
+                updated = project.update_version(release_version)
 
-            self.terminal.ok(f"Updated version to {release_version}")
+                self.terminal.ok(f"Updated version to {release_version}")
 
-            for path in updated.changed_files:
-                self.terminal.info(f"Adding changes of {path}")
-                self.git.add(path)
-        except VersionError as e:
-            self.terminal.error(
-                f"Unable to update version to {release_version}. {e}"
-            )
-            return ReleaseReturnValue.UPDATE_VERSION_ERROR
+                for path in updated.changed_files:
+                    self.terminal.info(f"Adding changes of {path}")
+                    self.git.add(path)
+            except VersionError as e:
+                self.terminal.error(
+                    f"Unable to update version to {release_version}. {e}"
+                )
+                return ReleaseReturnValue.UPDATE_VERSION_ERROR
 
         self.terminal.info(
             f"Creating changelog for {release_version} since "
             f"{last_release_version}"
         )
 
         release_text = self._create_changelog(
@@ -300,26 +305,29 @@
             except httpx.HTTPStatusError as e:
                 self.terminal.error(str(e))
                 return ReleaseReturnValue.CREATE_RELEASE_ERROR
 
         if not next_version:
             next_version = calculator.next_dev_version(release_version)
 
-        try:
-            updated = project.update_version(next_version)
-            self.terminal.ok(f"Updated version after release to {next_version}")
-        except VersionError as e:
-            self.terminal.error(
-                f"Error while updating version after release. {e}"
-            )
-            return ReleaseReturnValue.UPDATE_VERSION_AFTER_RELEASE_ERROR
+        if update_project:
+            try:
+                updated = project.update_version(next_version)
+                self.terminal.ok(
+                    f"Updated version after release to {next_version}"
+                )
+            except VersionError as e:
+                self.terminal.error(
+                    f"Error while updating version after release. {e}"
+                )
+                return ReleaseReturnValue.UPDATE_VERSION_AFTER_RELEASE_ERROR
 
-        for f in updated.changed_files:
-            self.terminal.info(f"Adding changes of {f}")
-            self.git.add(f)
+            for f in updated.changed_files:
+                self.terminal.info(f"Adding changes of {f}")
+                self.git.add(f)
 
         commit_msg = f"""Automatic adjustments after release
 
 * Update to version {next_version}
 """
 
         self.terminal.info("Committing changes")
@@ -360,9 +368,10 @@
             next_version=args.next_version,
             git_remote_name=args.git_remote_name,
             git_signing_key=args.git_signing_key,
             git_tag_prefix=args.git_tag_prefix,
             cc_config=args.cc_config,
             local=args.local,
             release_series=args.release_series,
+            update_project=args.update_project,
         )
     )
```

### Comparing `pontos-23.4.6/pontos/release/sign.py` & `pontos-23.4.7/pontos/release/sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/terminal/__init__.py` & `pontos-23.4.7/pontos/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/terminal/null.py` & `pontos-23.4.7/pontos/terminal/null.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/terminal/rich.py` & `pontos-23.4.7/pontos/terminal/rich.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/terminal/terminal.py` & `pontos-23.4.7/pontos/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/testing/__init__.py` & `pontos-23.4.7/pontos/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/updateheader/__init__.py` & `pontos-23.4.7/pontos/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/updateheader/__main__.py` & `pontos-23.4.7/pontos/updateheader/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/updateheader/updateheader.py` & `pontos-23.4.7/pontos/updateheader/updateheader.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/__init__.py` & `pontos-23.4.7/pontos/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/__main__.py` & `pontos-23.4.7/pontos/version/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/_calculator.py` & `pontos-23.4.7/pontos/version/_calculator.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/commands/__init__.py` & `pontos-23.4.7/pontos/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/commands/_cargo.py` & `pontos-23.4.7/pontos/version/commands/_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/commands/_cmake.py` & `pontos-23.4.7/pontos/version/commands/_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/commands/_command.py` & `pontos-23.4.7/pontos/version/commands/_command.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/commands/_go.py` & `pontos-23.4.7/pontos/version/commands/_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/commands/_javascript.py` & `pontos-23.4.7/pontos/version/commands/_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/commands/_python.py` & `pontos-23.4.7/pontos/version/commands/_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/errors.py` & `pontos-23.4.7/pontos/version/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/helper.py` & `pontos-23.4.7/pontos/version/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/main.py` & `pontos-23.4.7/pontos/version/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/parser.py` & `pontos-23.4.7/pontos/version/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/project.py` & `pontos-23.4.7/pontos/version/project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/schemes/__init__.py` & `pontos-23.4.7/pontos/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/schemes/_pep440.py` & `pontos-23.4.7/pontos/version/schemes/_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/schemes/_scheme.py` & `pontos-23.4.7/pontos/version/schemes/_scheme.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/schemes/_semantic.py` & `pontos-23.4.7/pontos/version/schemes/_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pontos/version/version.py` & `pontos-23.4.7/pontos/version/version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/pyproject.toml` & `pontos-23.4.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pontos"
-version = "23.4.6"
+version = "23.4.7"
 description = "Common utilities and tools maintained by Greenbone Networks"
 authors = ["Greenbone AG <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/pontos/"
 repository = "https://github.com/greenbone/pontos/"
 documentation = "https://greenbone.github.io/pontos/"
```

### Comparing `pontos-23.4.6/scripts/github/artifacts-download.py` & `pontos-23.4.7/scripts/github/artifacts-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/scripts/github/artifacts.py` & `pontos-23.4.7/scripts/github/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/scripts/github/branchprotection.py` & `pontos-23.4.7/scripts/github/branchprotection.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/scripts/github/create-repository.py` & `pontos-23.4.7/scripts/github/create-repository.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/scripts/github/enforce-admins.py` & `pontos-23.4.7/scripts/github/enforce-admins.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/scripts/github/lock-branch.py` & `pontos-23.4.7/scripts/github/lock-branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/scripts/github/members.py` & `pontos-23.4.7/scripts/github/members.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/scripts/github/release-assets-download.py` & `pontos-23.4.7/scripts/github/release-assets-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/scripts/github/repositories.py` & `pontos-23.4.7/scripts/github/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/scripts/github/search-repositories.py` & `pontos-23.4.7/scripts/github/search-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/scripts/github/team-repositories.py` & `pontos-23.4.7/scripts/github/team-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/scripts/github/teams.py` & `pontos-23.4.7/scripts/github/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/scripts/github/workflow-runs.py` & `pontos-23.4.7/scripts/github/workflow-runs.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/__init__.py` & `pontos-23.4.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/changelog/__init__.py` & `pontos-23.4.7/tests/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/changelog/test_conventional_commits.py` & `pontos-23.4.7/tests/changelog/test_conventional_commits.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/changelog/test_parser.py` & `pontos-23.4.7/tests/changelog/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/git/__init__.py` & `pontos-23.4.7/tests/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/git/test_git.py` & `pontos-23.4.7/tests/git/test_git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/git/test_status.py` & `pontos-23.4.7/tests/git/test_status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/__init__.py` & `pontos-23.4.7/tests/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/actions/__init__.py` & `pontos-23.4.7/tests/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/actions/test-pull-request-event.json` & `pontos-23.4.7/tests/github/actions/test-pull-request-event.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/actions/test_core.py` & `pontos-23.4.7/tests/github/actions/test_core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/actions/test_env.py` & `pontos-23.4.7/tests/github/actions/test_env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/actions/test_event.py` & `pontos-23.4.7/tests/github/actions/test_event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/api/__init__.py` & `pontos-23.4.7/tests/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/api/pr-files.json` & `pontos-23.4.7/tests/github/api/pr-files.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/api/release-response.json` & `pontos-23.4.7/tests/github/api/release-response.json`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/api/test_artifacts.py` & `pontos-23.4.7/tests/github/api/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/api/test_branch.py` & `pontos-23.4.7/tests/github/api/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/api/test_client.py` & `pontos-23.4.7/tests/github/api/test_client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/api/test_contents.py` & `pontos-23.4.7/tests/github/api/test_contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/api/test_labels.py` & `pontos-23.4.7/tests/github/api/test_labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/api/test_organizations.py` & `pontos-23.4.7/tests/github/api/test_organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/api/test_pull_requests.py` & `pontos-23.4.7/tests/github/api/test_pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/api/test_release.py` & `pontos-23.4.7/tests/github/api/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/api/test_repositories.py` & `pontos-23.4.7/tests/github/api/test_repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/api/test_search.py` & `pontos-23.4.7/tests/github/api/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/api/test_tags.py` & `pontos-23.4.7/tests/github/api/test_tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/api/test_teams.py` & `pontos-23.4.7/tests/github/api/test_teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/api/test_workflows.py` & `pontos-23.4.7/tests/github/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/models/__init__.py` & `pontos-23.4.7/tests/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/models/test_artifact.py` & `pontos-23.4.7/tests/github/models/test_artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/models/test_base.py` & `pontos-23.4.7/tests/github/models/test_base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/models/test_branch.py` & `pontos-23.4.7/tests/github/models/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/models/test_organization.py` & `pontos-23.4.7/tests/github/models/test_organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/models/test_pull_request.py` & `pontos-23.4.7/tests/github/models/test_pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/models/test_release.py` & `pontos-23.4.7/tests/github/models/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/models/test_search.py` & `pontos-23.4.7/tests/github/models/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/models/test_tag.py` & `pontos-23.4.7/tests/github/models/test_tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/models/test_workflow.py` & `pontos-23.4.7/tests/github/models/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/script/__init__.py` & `pontos-23.4.7/tests/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/script/test_load.py` & `pontos-23.4.7/tests/github/script/test_load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/script/test_parser.py` & `pontos-23.4.7/tests/github/script/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/test_argparser.py` & `pontos-23.4.7/tests/github/test_argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/github/test_cmds.py` & `pontos-23.4.7/tests/github/test_cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/models/__init__.py` & `pontos-23.4.7/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/models/test_models.py` & `pontos-23.4.7/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/nvd/__init__.py` & `pontos-23.4.7/tests/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/nvd/cpe/__init__.py` & `pontos-23.4.7/tests/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/nvd/cpe/test_api.py` & `pontos-23.4.7/tests/nvd/cpe/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/nvd/cve/__init__.py` & `pontos-23.4.7/tests/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/nvd/cve/test_api.py` & `pontos-23.4.7/tests/nvd/cve/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/nvd/models/__init__.py` & `pontos-23.4.7/tests/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/nvd/models/test_cpe.py` & `pontos-23.4.7/tests/nvd/models/test_cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/nvd/models/test_cve.py` & `pontos-23.4.7/tests/nvd/models/test_cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/nvd/test_api.py` & `pontos-23.4.7/tests/nvd/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/release/__init__.py` & `pontos-23.4.7/tests/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/release/test_helper.py` & `pontos-23.4.7/tests/release/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/release/test_parser.py` & `pontos-23.4.7/tests/release/test_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,31 @@
     def test_release_series(self):
         _, _, args = parse_args(
             ["release", "--release-type", "patch", "--release-series", "22.4"]
         )
 
         self.assertEqual(args.release_series, "22.4")
 
+    def test_update_project(self):
+        _, _, args = parse_args(["release", "--release-type", "patch"])
+
+        self.assertTrue(args.update_project)
+
+        _, _, args = parse_args(
+            ["release", "--release-type", "patch", "--update-project"]
+        )
+
+        self.assertTrue(args.update_project)
+
+        _, _, args = parse_args(
+            ["release", "--release-type", "patch", "--no-update-project"]
+        )
+
+        self.assertFalse(args.update_project)
+
 
 class SignParseArgsTestCase(unittest.TestCase):
     def test_sign_func(self):
         _, _, args = parse_args(["sign"])
 
         self.assertEqual(args.func, sign)
```

### Comparing `pontos-23.4.6/tests/release/test_release.py` & `pontos-23.4.7/tests/release/test_release.py`

 * *Files 2% similar despite different names*

```diff
@@ -1022,14 +1022,93 @@
                 token=token,
             )
 
         self.assertEqual(
             released, ReleaseReturnValue.PROJECT_SETTINGS_NOT_FOUND
         )
 
+    @patch("pontos.release.release.Git", autospec=True)
+    @patch("pontos.release.release.get_last_release_version", autospec=True)
+    @patch(
+        "pontos.release.release.ReleaseCommand._create_release", autospec=True
+    )
+    @patch(
+        "pontos.release.release.ReleaseCommand._create_changelog",
+        autospec=True,
+    )
+    @patch("pontos.release.release.Project", autospec=True)
+    def test_no_update_project(
+        self,
+        project_mock: MagicMock,
+        create_changelog_mock: MagicMock,
+        create_release_mock: AsyncMock,
+        get_last_release_version_mock: MagicMock,
+        git_mock: MagicMock,
+    ):
+        current_version = PEP440Version("0.0.1")
+        release_version = PEP440Version("0.0.2")
+        create_changelog_mock.return_value = "A Changelog"
+        get_last_release_version_mock.return_value = current_version
+
+        _, token, args = parse_args(
+            [
+                "release",
+                "--project",
+                "foo",
+                "--release-version",
+                "0.0.2",
+                "--next-version",
+                "1.0.0.dev1",
+                "--no-update-project",
+            ]
+        )
+
+        with temp_git_repository():
+            released = release(
+                terminal=mock_terminal(),
+                args=args,
+                token=token,
+            )
+
+        git_mock.return_value.push.assert_has_calls(
+            [
+                call(follow_tags=True, remote=None),
+                call(follow_tags=True, remote=None),
+            ],
+        )
+
+        self.assertEqual(
+            create_release_mock.await_args.args[1:],
+            (release_version, "foo", "A Changelog"),
+        )
+
+        git_mock.return_value.add.assert_not_called()
+        git_mock.return_value.commit.assert_has_calls(
+            [
+                call(
+                    "Automatic release to 0.0.2",
+                    verify=False,
+                    gpg_signing_key="1234",
+                ),
+                call(
+                    "Automatic adjustments after release\n\n"
+                    "* Update to version 1.0.0.dev1\n",
+                    verify=False,
+                    gpg_signing_key="1234",
+                ),
+            ]
+        )
+        git_mock.return_value.tag.assert_called_once_with(
+            "v0.0.2", gpg_key_id="1234", message="Automatic release to 0.0.2"
+        )
+
+        self.assertEqual(released, ReleaseReturnValue.SUCCESS)
+
+        project_mock.assert_not_called()
+
     def test_last_release_version_error(self):
         _, token, args = parse_args(
             [
                 "release",
                 "--project",
                 "foo",
                 "--release-type",
```

### Comparing `pontos-23.4.6/tests/release/test_sign.py` & `pontos-23.4.7/tests/release/test_sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/terminal/__init__.py` & `pontos-23.4.7/tests/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/terminal/test_terminal.py` & `pontos-23.4.7/tests/terminal/test_terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/test_helper.py` & `pontos-23.4.7/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/test_pontos.py` & `pontos-23.4.7/tests/test_pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/testing/__init__.py` & `pontos-23.4.7/tests/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/testing/test_testing.py` & `pontos-23.4.7/tests/testing/test_testing.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/updateheader/__init__.py` & `pontos-23.4.7/tests/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/updateheader/test_header.py` & `pontos-23.4.7/tests/updateheader/test_header.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/version/__init__.py` & `pontos-23.4.7/tests/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/version/commands/__init__.py` & `pontos-23.4.7/tests/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/version/commands/test_cargo.py` & `pontos-23.4.7/tests/version/commands/test_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/version/commands/test_cmake.py` & `pontos-23.4.7/tests/version/commands/test_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/version/commands/test_go.py` & `pontos-23.4.7/tests/version/commands/test_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/version/commands/test_javascript.py` & `pontos-23.4.7/tests/version/commands/test_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/version/commands/test_python.py` & `pontos-23.4.7/tests/version/commands/test_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/version/schemes/__init__.py` & `pontos-23.4.7/tests/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/version/schemes/test_pep440.py` & `pontos-23.4.7/tests/version/schemes/test_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/version/schemes/test_semantic.py` & `pontos-23.4.7/tests/version/schemes/test_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/version/test_commands.py` & `pontos-23.4.7/tests/version/test_commands.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/version/test_errors.py` & `pontos-23.4.7/tests/version/test_errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/version/test_helper.py` & `pontos-23.4.7/tests/version/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/version/test_main.py` & `pontos-23.4.7/tests/version/test_main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/version/test_parser.py` & `pontos-23.4.7/tests/version/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/version/test_project.py` & `pontos-23.4.7/tests/version/test_project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/tests/version/test_version.py` & `pontos-23.4.7/tests/version/test_version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.4.6/PKG-INFO` & `pontos-23.4.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pontos
-Version: 23.4.6
+Version: 23.4.7
 Summary: Common utilities and tools maintained by Greenbone Networks
 Home-page: https://github.com/greenbone/pontos/
 License: GPL-3.0-or-later
 Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -48,14 +48,15 @@
 the titan of the sea.
 
 ## Table of Contents <!-- omit in toc -->
 
 - [Documentation](#documentation)
 - [Installation](#installation)
   - [Requirements](#requirements)
+  - [Install using pipx](#install-using-pipx)
   - [Install using pip](#install-using-pip)
   - [Install using poetry](#install-using-poetry)
 - [Development](#development)
 - [Maintainer](#maintainer)
 - [Contributing](#contributing)
 - [License](#license)
 
@@ -65,16 +66,27 @@
 
 ## Installation
 
 ### Requirements
 
 Python 3.9 and later is supported.
 
+### Install using pipx
+
+You can install the latest stable release of **pontos** from the Python
+Package Index (pypi) using [pipx]
+
+    python3 -m pipx install pontos
+
 ### Install using pip
 
+**NOTE:** The ‘pip install’ command does no longer work out-of-the-box in newer
+distributions like Ubuntu 23.04 because of [PEP 668](https://peps.python.org/pep-0668).
+Please use the [installation via pipx](#install-using-pipx) instead.
+
 You can install the latest stable release of **pontos** from the Python
 Package Index (pypi) using [pip]
 
     python3 -m pip install --user pontos
 
 ### Install using poetry
 
@@ -88,17 +100,17 @@
     poetry add pontos
 
 ## Development
 
 **pontos** uses [poetry] for its own dependency management and build
 process.
 
-First install poetry via pip
+First install poetry via pipx
 
-    python3 -m pip install --user poetry
+    python3 -m pipx install poetry
 
 Afterwards run
 
     poetry install
 
 in the checkout directory of **pontos** (the directory containing the
 `pyproject.toml` file) to install all dependencies including the packages only
@@ -130,9 +142,10 @@
 Copyright (C) 2020-2023 [Greenbone AG][Greenbone Networks]
 
 Licensed under the [GNU General Public License v3.0 or later](LICENSE).
 
 [Greenbone Networks]: https://www.greenbone.net/
 [poetry]: https://python-poetry.org/
 [pip]: https://pip.pypa.io/
+[pipx]: https://pypa.github.io/pipx/
 [autohooks]: https://github.com/greenbone/autohooks
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

