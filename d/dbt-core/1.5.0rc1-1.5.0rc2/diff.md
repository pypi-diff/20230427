# Comparing `tmp/dbt-core-1.5.0rc1.tar.gz` & `tmp/dbt-core-1.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-core-1.5.0rc1.tar", last modified: Fri Apr 14 00:23:11 2023, max compression
+gzip compressed data, was "dbt-core-1.5.0rc2.tar", last modified: Thu Apr 20 21:14:58 2023, max compression
```

## Comparing `dbt-core-1.5.0rc1.tar` & `dbt-core-1.5.0rc2.tar`

### file list

```diff
@@ -1,312 +1,312 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.559258 dbt-core-1.5.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-04-14 00:23:11.559258 dbt-core-1.5.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.523257 dbt-core-1.5.0rc1/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.523257 dbt-core-1.5.0rc1/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.523257 dbt-core-1.5.0rc1/dbt/adapters/base/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/adapters/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/adapters/base/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/adapters/base/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    55030 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/adapters/base/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/adapters/base/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/adapters/base/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/adapters/base/query_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14913 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/adapters/base/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/adapters/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/adapters/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/adapters/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/adapters/reference_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.523257 dbt-core-1.5.0rc1/dbt/adapters/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/adapters/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/adapters/sql/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/adapters/sql/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.523257 dbt-core-1.5.0rc1/dbt/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/cli/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    16615 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/cli/option_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/cli/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/cli/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/cli/resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.527257 dbt-core-1.5.0rc1/dbt/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/clients/_jinja_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/clients/agate_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/clients/git.py
--rw-r--r--   0 runner    (1001) docker     (123)    21425 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/clients/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/clients/jinja_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/clients/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/clients/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/clients/yaml_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19815 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/compilation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.527257 dbt-core-1.5.0rc1/dbt/config/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/config/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/config/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/config/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.527257 dbt-core-1.5.0rc1/dbt/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/context/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/context/configured.py
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/context/context_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/context/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/context/exceptions_jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/context/macro_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/context/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/context/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    57568 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/context/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/context/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/context/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.531257 dbt-core-1.5.0rc1/dbt/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/contracts/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/contracts/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.531257 dbt-core-1.5.0rc1/dbt/contracts/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/contracts/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46034 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/contracts/graph/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/contracts/graph/manifest_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/contracts/graph/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    20939 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/contracts/graph/model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    45320 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/contracts/graph/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/contracts/graph/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    20236 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/contracts/graph/unparsed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/contracts/graph/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/contracts/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/contracts/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13381 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/contracts/results.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/contracts/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/contracts/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/contracts/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/contracts/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/dataclass_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/deprecations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.531257 dbt-core-1.5.0rc1/dbt/deps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/deps/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/deps/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/deps/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/deps/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/deps/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/deps/tarball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.515257 dbt-core-1.5.0rc1/dbt/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.531257 dbt-core-1.5.0rc1/dbt/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.531257 dbt-core-1.5.0rc1/dbt/docs/source/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/docs/source/_ext/dbt_click.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.531257 dbt-core-1.5.0rc1/dbt/events/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/events/adapter_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/events/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/events/contextvars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/events/eventmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/events/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/events/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/events/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    58511 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/events/types.py
--rw-r--r--   0 runner    (1001) docker     (123)   101429 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/events/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    74919 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.535257 dbt-core-1.5.0rc1/dbt/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/graph/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/graph/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/graph/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    28073 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/graph/selector_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/graph/selector_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/helper_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.535257 dbt-core-1.5.0rc1/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.535257 dbt-core-1.5.0rc1/dbt/include/global_project/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.535257 dbt-core-1.5.0rc1/dbt/include/global_project/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/docs/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.515257 dbt-core-1.5.0rc1/dbt/include/global_project/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.535257 dbt-core-1.5.0rc1/dbt/include/global_project/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/adapters/freshness.sql
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/adapters/schema.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/adapters/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.535257 dbt-core-1.5.0rc1/dbt/include/global_project/macros/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/etc/datetime.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/etc/statement.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.539257 dbt-core-1.5.0rc1/dbt/include/global_project/macros/generic_test_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/generic_test_sql/not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/generic_test_sql/relationships.sql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/generic_test_sql/unique.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.539257 dbt-core-1.5.0rc1/dbt/include/global_project/macros/get_custom_name/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.539257 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/configs.sql
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/hooks.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.515257 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.539257 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.539257 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.543257 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/view/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.543257 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/seeds/seed.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.543257 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.543257 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/tests/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/tests/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.543257 dbt-core-1.5.0rc1/dbt/include/global_project/macros/python_model/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/python_model/python.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.547257 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/data_types.sql
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/except.sql
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/intersect.sql
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/literal.sql
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/replace.sql
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/split_part.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.519256 dbt-core-1.5.0rc1/dbt/include/global_project/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.547257 dbt-core-1.5.0rc1/dbt/include/global_project/tests/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/global_project/tests/generic/builtin.sql
--rw-r--r--   0 runner    (1001) docker     (123)  1497701 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.547257 dbt-core-1.5.0rc1/dbt/include/starter_project/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/starter_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/starter_project/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/starter_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.547257 dbt-core-1.5.0rc1/dbt/include/starter_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/starter_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/starter_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.547257 dbt-core-1.5.0rc1/dbt/include/starter_project/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/starter_project/macros/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.519256 dbt-core-1.5.0rc1/dbt/include/starter_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.551257 dbt-core-1.5.0rc1/dbt/include/starter_project/models/example/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/starter_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/starter_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/starter_project/models/example/schema.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.551257 dbt-core-1.5.0rc1/dbt/include/starter_project/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/starter_project/seeds/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.551257 dbt-core-1.5.0rc1/dbt/include/starter_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/starter_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.551257 dbt-core-1.5.0rc1/dbt/include/starter_project/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/include/starter_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/internal_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/links.py
--rw-r--r--   0 runner    (1001) docker     (123)    19932 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/node_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.555257 dbt-core-1.5.0rc1/dbt/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    16910 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/generic_test_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)    62437 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    25716 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    50860 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/partial.py
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/read_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/schema_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    58934 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/singular_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/parser/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/selected_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/semver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.555257 dbt-core-1.5.0rc1/dbt/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/freshness.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/list.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/run_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/task/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.559258 dbt-core-1.5.0rc1/dbt/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.559258 dbt-core-1.5.0rc1/dbt/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/tests/fixtures/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    18179 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    20505 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/dbt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 00:23:11.559258 dbt-core-1.5.0rc1/dbt_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-04-14 00:23:11.000000 dbt-core-1.5.0rc1/dbt_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-04-14 00:23:11.000000 dbt-core-1.5.0rc1/dbt_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:23:11.000000 dbt-core-1.5.0rc1/dbt_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 00:23:11.000000 dbt-core-1.5.0rc1/dbt_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 00:23:11.000000 dbt-core-1.5.0rc1/dbt_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-14 00:23:11.000000 dbt-core-1.5.0rc1/dbt_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-14 00:23:11.000000 dbt-core-1.5.0rc1/dbt_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 00:23:11.559258 dbt-core-1.5.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-14 00:23:01.000000 dbt-core-1.5.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.562554 dbt-core-1.5.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-04-20 21:14:58.562554 dbt-core-1.5.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.530555 dbt-core-1.5.0rc2/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.530555 dbt-core-1.5.0rc2/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.534555 dbt-core-1.5.0rc2/dbt/adapters/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/base/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/base/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55030 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/base/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/base/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/base/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/base/query_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14913 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/base/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/reference_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.534555 dbt-core-1.5.0rc2/dbt/adapters/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/sql/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/sql/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.534555 dbt-core-1.5.0rc2/dbt/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16615 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/option_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.534555 dbt-core-1.5.0rc2/dbt/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/clients/_jinja_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/clients/agate_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/clients/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21425 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/clients/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/clients/jinja_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/clients/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/clients/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/clients/yaml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19815 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/compilation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.538555 dbt-core-1.5.0rc2/dbt/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/config/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/config/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.538555 dbt-core-1.5.0rc2/dbt/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/configured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/context_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/exceptions_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/macro_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57568 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.538555 dbt-core-1.5.0rc2/dbt/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.542554 dbt-core-1.5.0rc2/dbt/contracts/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45991 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/graph/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/graph/manifest_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/graph/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20939 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/graph/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45470 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/graph/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/graph/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20236 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/graph/unparsed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/graph/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13381 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/dataclass_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/deprecations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.542554 dbt-core-1.5.0rc2/dbt/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/deps/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/deps/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/deps/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/deps/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/deps/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/deps/tarball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.526554 dbt-core-1.5.0rc2/dbt/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.542554 dbt-core-1.5.0rc2/dbt/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.542554 dbt-core-1.5.0rc2/dbt/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/docs/source/_ext/dbt_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.542554 dbt-core-1.5.0rc2/dbt/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/adapter_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/contextvars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/eventmgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58511 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101429 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74918 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.546554 dbt-core-1.5.0rc2/dbt/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/graph/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/graph/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/graph/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27989 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/graph/selector_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/graph/selector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/helper_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.546554 dbt-core-1.5.0rc2/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.546554 dbt-core-1.5.0rc2/dbt/include/global_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.546554 dbt-core-1.5.0rc2/dbt/include/global_project/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/docs/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.526554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.546554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/freshness.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/schema.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.546554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/etc/datetime.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/etc/statement.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.546554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/generic_test_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/generic_test_sql/not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/generic_test_sql/relationships.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/generic_test_sql/unique.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.550554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/get_custom_name/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.550554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/configs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/hooks.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.526554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.550554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.550554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.550554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/view/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.550554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/seeds/seed.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.550554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.550554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/tests/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/tests/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.550554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/python_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/python_model/python.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.554554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/data_types.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/except.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/intersect.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/literal.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/replace.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/split_part.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.526554 dbt-core-1.5.0rc2/dbt/include/global_project/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.554554 dbt-core-1.5.0rc2/dbt/include/global_project/tests/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/tests/generic/builtin.sql
+-rw-r--r--   0 runner    (1001) docker     (123)  1497701 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.554554 dbt-core-1.5.0rc2/dbt/include/starter_project/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.554554 dbt-core-1.5.0rc2/dbt/include/starter_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.554554 dbt-core-1.5.0rc2/dbt/include/starter_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/macros/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.526554 dbt-core-1.5.0rc2/dbt/include/starter_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.554554 dbt-core-1.5.0rc2/dbt/include/starter_project/models/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/models/example/schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.554554 dbt-core-1.5.0rc2/dbt/include/starter_project/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/seeds/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.554554 dbt-core-1.5.0rc2/dbt/include/starter_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.554554 dbt-core-1.5.0rc2/dbt/include/starter_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/internal_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19932 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/node_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.558554 dbt-core-1.5.0rc2/dbt/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16910 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/generic_test_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62438 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25716 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50860 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/schema_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59005 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/singular_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/selected_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/semver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.562554 dbt-core-1.5.0rc2/dbt/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/freshness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/run_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.562554 dbt-core-1.5.0rc2/dbt/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.562554 dbt-core-1.5.0rc2/dbt/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/tests/fixtures/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18179 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20505 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.562554 dbt-core-1.5.0rc2/dbt_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-04-20 21:14:58.000000 dbt-core-1.5.0rc2/dbt_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-04-20 21:14:58.000000 dbt-core-1.5.0rc2/dbt_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:14:58.000000 dbt-core-1.5.0rc2/dbt_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 21:14:58.000000 dbt-core-1.5.0rc2/dbt_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:14:58.000000 dbt-core-1.5.0rc2/dbt_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-20 21:14:58.000000 dbt-core-1.5.0rc2/dbt_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-20 21:14:58.000000 dbt-core-1.5.0rc2/dbt_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 21:14:58.562554 dbt-core-1.5.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/setup.py
```

### Comparing `dbt-core-1.5.0rc1/PKG-INFO` & `dbt-core-1.5.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.5.0rc1
+Version: 1.5.0rc2
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.5.0rc1 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.5.0rc2 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `dbt-core-1.5.0rc1/README.md` & `dbt-core-1.5.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/adapters/base/__init__.py` & `dbt-core-1.5.0rc2/dbt/adapters/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/adapters/base/column.py` & `dbt-core-1.5.0rc2/dbt/adapters/base/column.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/adapters/base/connections.py` & `dbt-core-1.5.0rc2/dbt/adapters/base/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/adapters/base/impl.py` & `dbt-core-1.5.0rc2/dbt/adapters/base/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/adapters/base/meta.py` & `dbt-core-1.5.0rc2/dbt/adapters/base/meta.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/adapters/base/plugin.py` & `dbt-core-1.5.0rc2/dbt/adapters/base/plugin.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/adapters/base/query_headers.py` & `dbt-core-1.5.0rc2/dbt/adapters/base/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/adapters/base/relation.py` & `dbt-core-1.5.0rc2/dbt/adapters/base/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/adapters/cache.py` & `dbt-core-1.5.0rc2/dbt/adapters/cache.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/adapters/factory.py` & `dbt-core-1.5.0rc2/dbt/adapters/factory.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/adapters/protocol.py` & `dbt-core-1.5.0rc2/dbt/adapters/protocol.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/adapters/reference_keys.py` & `dbt-core-1.5.0rc2/dbt/adapters/reference_keys.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/adapters/sql/connections.py` & `dbt-core-1.5.0rc2/dbt/adapters/sql/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/adapters/sql/impl.py` & `dbt-core-1.5.0rc2/dbt/adapters/sql/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/cli/exceptions.py` & `dbt-core-1.5.0rc2/dbt/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/cli/flags.py` & `dbt-core-1.5.0rc2/dbt/cli/flags.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/cli/main.py` & `dbt-core-1.5.0rc2/dbt/cli/main.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/cli/option_types.py` & `dbt-core-1.5.0rc2/dbt/cli/option_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/cli/options.py` & `dbt-core-1.5.0rc2/dbt/cli/options.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/cli/params.py` & `dbt-core-1.5.0rc2/dbt/cli/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pathlib import Path, PurePath
+from pathlib import Path
 
 import click
 from dbt.cli.options import MultiOption
 from dbt.cli.option_types import YAML, ChoiceTuple, WarnErrorOptionsType
 from dbt.cli.resolvers import default_project_dir, default_profiles_dir
 from dbt.version import get_version_information
 
@@ -19,15 +19,15 @@
     help="Wether or not to open a local web browser after starting the server",
     default=True,
 )
 
 cache_selected_only = click.option(
     "--cache-selected-only/--no-cache-selected-only",
     envvar="DBT_CACHE_SELECTED_ONLY",
-    help="Pre cache database objects relevant to selected resource only.",
+    help="At start of run, populate relational cache only for schemas containing selected nodes, or for all schemas of interest.",
 )
 
 introspect = click.option(
     "--introspect/--no-introspect",
     envvar="DBT_INTROSPECT",
     help="Whether to scaffold introspective queries as part of compilation",
     default=True,
@@ -117,15 +117,15 @@
     help="Choose which tests to select that are adjacent to selected resources. Eager is most inclusive, cautious is most exclusive, and buildable is in between. Empty includes no tests at all.",
     type=click.Choice(["eager", "cautious", "buildable", "empty"], case_sensitive=False),
     default="eager",
 )
 
 log_cache_events = click.option(
     "--log-cache-events/--no-log-cache-events",
-    help="Enable verbose adapter cache logging.",
+    help="Enable verbose logging for relational cache events to help when debugging.",
     envvar="DBT_LOG_CACHE_EVENTS",
 )
 
 log_format = click.option(
     "--log-format",
     envvar="DBT_LOG_FORMAT",
     help="Specify the format of logging to the console and the log file. Use --log-format-file to configure the format for the log file differently than the console.",
@@ -225,28 +225,28 @@
 
 output_path = click.option(
     "--output",
     "-o",
     envvar=None,
     help="Specify the output path for the JSON report. By default, outputs to 'target/sources.json'",
     type=click.Path(file_okay=True, dir_okay=False, writable=True),
-    default=PurePath.joinpath(Path.cwd(), "target/sources.json"),
+    default=None,
 )
 
 partial_parse = click.option(
     "--partial-parse/--no-partial-parse",
     envvar="DBT_PARTIAL_PARSE",
     help="Allow for partial parsing by looking for and writing to a pickle file in the target directory. This overrides the user configuration file.",
     default=True,
 )
 
 populate_cache = click.option(
     "--populate-cache/--no-populate-cache",
     envvar="DBT_POPULATE_CACHE",
-    help="Allow for partial parsing by looking for and writing to a pickle file in the target directory. This overrides the user configuration file.",
+    help="At start of run, use `show` or `information_schema` queries to populate a relational cache, which can speed up subsequent materializations.",
     default=True,
 )
 
 port = click.option(
     "--port",
     envvar=None,
     help="Specify the port number for the docs server",
```

### Comparing `dbt-core-1.5.0rc1/dbt/cli/requires.py` & `dbt-core-1.5.0rc2/dbt/cli/requires.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/cli/resolvers.py` & `dbt-core-1.5.0rc2/dbt/cli/resolvers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/clients/_jinja_blocks.py` & `dbt-core-1.5.0rc2/dbt/clients/_jinja_blocks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/clients/agate_helper.py` & `dbt-core-1.5.0rc2/dbt/clients/agate_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/clients/git.py` & `dbt-core-1.5.0rc2/dbt/clients/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/clients/jinja.py` & `dbt-core-1.5.0rc2/dbt/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/clients/jinja_static.py` & `dbt-core-1.5.0rc2/dbt/clients/jinja_static.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/clients/registry.py` & `dbt-core-1.5.0rc2/dbt/clients/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/clients/system.py` & `dbt-core-1.5.0rc2/dbt/clients/system.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/clients/yaml_helper.py` & `dbt-core-1.5.0rc2/dbt/clients/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/compilation.py` & `dbt-core-1.5.0rc2/dbt/compilation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/config/profile.py` & `dbt-core-1.5.0rc2/dbt/config/profile.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/config/project.py` & `dbt-core-1.5.0rc2/dbt/config/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/config/renderer.py` & `dbt-core-1.5.0rc2/dbt/config/renderer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/config/runtime.py` & `dbt-core-1.5.0rc2/dbt/config/runtime.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/config/selectors.py` & `dbt-core-1.5.0rc2/dbt/config/selectors.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/config/utils.py` & `dbt-core-1.5.0rc2/dbt/config/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/context/base.py` & `dbt-core-1.5.0rc2/dbt/context/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/context/configured.py` & `dbt-core-1.5.0rc2/dbt/context/configured.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/context/context_config.py` & `dbt-core-1.5.0rc2/dbt/context/context_config.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/context/docs.py` & `dbt-core-1.5.0rc2/dbt/context/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/context/exceptions_jinja.py` & `dbt-core-1.5.0rc2/dbt/context/exceptions_jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/context/macro_resolver.py` & `dbt-core-1.5.0rc2/dbt/context/macro_resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/context/macros.py` & `dbt-core-1.5.0rc2/dbt/context/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/context/manifest.py` & `dbt-core-1.5.0rc2/dbt/context/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/context/providers.py` & `dbt-core-1.5.0rc2/dbt/context/providers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/context/secret.py` & `dbt-core-1.5.0rc2/dbt/context/secret.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/context/target.py` & `dbt-core-1.5.0rc2/dbt/context/target.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/contracts/connection.py` & `dbt-core-1.5.0rc2/dbt/contracts/connection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/contracts/files.py` & `dbt-core-1.5.0rc2/dbt/contracts/files.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/contracts/graph/manifest.py` & `dbt-core-1.5.0rc2/dbt/contracts/graph/manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         return None
 
     def add_node(self, node: ManifestNode):
         if node.resource_type in self._lookup_types:
             if node.name not in self.storage:
                 self.storage[node.name] = {}
 
-            if node.resource_type in self._versioned_types and node.version:
+            if node.is_versioned:
                 if node.search_name not in self.storage:
                     self.storage[node.search_name] = {}
                 self.storage[node.search_name][node.package_name] = node.unique_id
                 if node.is_latest_version:  # type: ignore
                     self.storage[node.name][node.package_name] = node.unique_id
             else:
                 self.storage[node.name][node.package_name] = node.unique_id
```

### Comparing `dbt-core-1.5.0rc1/dbt/contracts/graph/manifest_upgrade.py` & `dbt-core-1.5.0rc2/dbt/contracts/graph/manifest_upgrade.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/contracts/graph/metrics.py` & `dbt-core-1.5.0rc2/dbt/contracts/graph/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/contracts/graph/model_config.py` & `dbt-core-1.5.0rc2/dbt/contracts/graph/model_config.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/contracts/graph/nodes.py` & `dbt-core-1.5.0rc2/dbt/contracts/graph/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,14 +116,18 @@
 
     # will this node map to an object in the database?
     @property
     def is_relational(self):
         return self.resource_type in NodeType.refable()
 
     @property
+    def is_versioned(self):
+        return self.resource_type in NodeType.versioned() and self.version is not None
+
+    @property
     def is_ephemeral(self):
         return self.config.materialized == "ephemeral"
 
     @property
     def is_ephemeral_model(self):
         return self.is_refable and self.is_ephemeral
 
@@ -660,16 +664,16 @@
     resource_type: NodeType = field(metadata={"restrict": [NodeType.Model]})
     access: AccessType = AccessType.Protected
     constraints: List[ModelLevelConstraint] = field(default_factory=list)
     version: Optional[NodeVersion] = None
     latest_version: Optional[NodeVersion] = None
 
     @property
-    def is_latest_version(self):
-        return self.version and self.version == self.latest_version
+    def is_latest_version(self) -> bool:
+        return self.version is not None and self.version == self.latest_version
 
     @property
     def search_name(self):
         if self.version is None:
             return self.name
         else:
             return f"{self.name}.v{self.version}"
```

### Comparing `dbt-core-1.5.0rc1/dbt/contracts/graph/unparsed.py` & `dbt-core-1.5.0rc2/dbt/contracts/graph/unparsed.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/contracts/graph/utils.py` & `dbt-core-1.5.0rc2/dbt/contracts/graph/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/contracts/project.py` & `dbt-core-1.5.0rc2/dbt/contracts/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/contracts/relation.py` & `dbt-core-1.5.0rc2/dbt/contracts/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/contracts/results.py` & `dbt-core-1.5.0rc2/dbt/contracts/results.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/contracts/selection.py` & `dbt-core-1.5.0rc2/dbt/contracts/selection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/contracts/sql.py` & `dbt-core-1.5.0rc2/dbt/contracts/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/contracts/state.py` & `dbt-core-1.5.0rc2/dbt/contracts/state.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/contracts/util.py` & `dbt-core-1.5.0rc2/dbt/contracts/util.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/dataclass_schema.py` & `dbt-core-1.5.0rc2/dbt/dataclass_schema.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/deprecations.py` & `dbt-core-1.5.0rc2/dbt/deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/deps/base.py` & `dbt-core-1.5.0rc2/dbt/deps/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/deps/git.py` & `dbt-core-1.5.0rc2/dbt/deps/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/deps/local.py` & `dbt-core-1.5.0rc2/dbt/deps/local.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/deps/registry.py` & `dbt-core-1.5.0rc2/dbt/deps/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/deps/resolver.py` & `dbt-core-1.5.0rc2/dbt/deps/resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/deps/tarball.py` & `dbt-core-1.5.0rc2/dbt/deps/tarball.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/docs/source/_ext/dbt_click.py` & `dbt-core-1.5.0rc2/dbt/docs/source/_ext/dbt_click.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/docs/source/conf.py` & `dbt-core-1.5.0rc2/dbt/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/events/adapter_endpoint.py` & `dbt-core-1.5.0rc2/dbt/events/adapter_endpoint.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/events/base_types.py` & `dbt-core-1.5.0rc2/dbt/events/base_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/events/contextvars.py` & `dbt-core-1.5.0rc2/dbt/events/contextvars.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/events/eventmgr.py` & `dbt-core-1.5.0rc2/dbt/events/eventmgr.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/events/format.py` & `dbt-core-1.5.0rc2/dbt/events/format.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/events/functions.py` & `dbt-core-1.5.0rc2/dbt/events/functions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/events/helpers.py` & `dbt-core-1.5.0rc2/dbt/events/helpers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/events/types.py` & `dbt-core-1.5.0rc2/dbt/events/types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/events/types_pb2.py` & `dbt-core-1.5.0rc2/dbt/events/types_pb2.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/exceptions.py` & `dbt-core-1.5.0rc2/dbt/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
 
         reasons = "\n\n".join(breaking_changes)
 
         return (
             "While comparing to previous project state, dbt detected a breaking change to an enforced contract."
             f"\n\n{reasons}\n\n"
             "Consider making an additive (non-breaking) change instead, if possible.\n"
-            "Otherwise, create a new model version: https://docs.getdbt.com/docs/collaborate/publish/model-versions"
+            "Otherwise, create a new model version: https://docs.getdbt.com/docs/collaborate/govern/model-versions"
         )
 
 
 class RecursionError(DbtRuntimeError):
     pass
```

### Comparing `dbt-core-1.5.0rc1/dbt/flags.py` & `dbt-core-1.5.0rc2/dbt/flags.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/graph/cli.py` & `dbt-core-1.5.0rc2/dbt/graph/cli.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/graph/graph.py` & `dbt-core-1.5.0rc2/dbt/graph/graph.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/graph/queue.py` & `dbt-core-1.5.0rc2/dbt/graph/queue.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/graph/selector.py` & `dbt-core-1.5.0rc2/dbt/graph/selector.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/graph/selector_methods.py` & `dbt-core-1.5.0rc2/dbt/graph/selector_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,16 +206,15 @@
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         """Yield all nodes in the graph that match the selector.
 
         :param str selector: The selector or node name
         """
         parsed_nodes = list(self.parsed_nodes(included_nodes))
         for node, real_node in parsed_nodes:
-            is_versioned = isinstance(real_node, ModelNode) and real_node.version is not None
-            if self.node_is_match(selector, real_node.fqn, is_versioned):
+            if self.node_is_match(selector, real_node.fqn, real_node.is_versioned):
                 yield node
 
 
 class TagSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         """yields nodes from included that have the specified tag"""
         for node, real_node in self.all_nodes(included_nodes):
```

### Comparing `dbt-core-1.5.0rc1/dbt/graph/selector_spec.py` & `dbt-core-1.5.0rc2/dbt/graph/selector_spec.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/helper_types.py` & `dbt-core-1.5.0rc2/dbt/helper_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/README.md` & `dbt-core-1.5.0rc2/dbt/include/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/docs/overview.md` & `dbt-core-1.5.0rc2/dbt/include/global_project/docs/overview.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/adapters/apply_grants.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/adapters/columns.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/adapters/freshness.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/adapters/indexes.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/adapters/metadata.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/adapters/persist_docs.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/adapters/relation.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/adapters/schema.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/adapters/timestamps.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/etc/datetime.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/etc/datetime.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/etc/statement.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/etc/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/configs.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/configs.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/hooks.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/hooks.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/incremental/merge.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/table/table.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/models/view/view.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/seeds/helpers.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/seeds/seed.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/seeds/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/snapshots/helpers.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/snapshots/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/snapshots/strategies.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/snapshots/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/tests/helpers.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/materializations/tests/test.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/python_model/python.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/python_model/python.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/data_types.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/listagg.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/macros/utils/split_part.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/global_project/tests/generic/builtin.sql` & `dbt-core-1.5.0rc2/dbt/include/global_project/tests/generic/builtin.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/index.html` & `dbt-core-1.5.0rc2/dbt/include/index.html`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/starter_project/README.md` & `dbt-core-1.5.0rc2/dbt/include/starter_project/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/include/starter_project/dbt_project.yml` & `dbt-core-1.5.0rc2/dbt/include/starter_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/internal_deprecations.py` & `dbt-core-1.5.0rc2/dbt/internal_deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/logger.py` & `dbt-core-1.5.0rc2/dbt/logger.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/node_types.py` & `dbt-core-1.5.0rc2/dbt/node_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/parser/__init__.py` & `dbt-core-1.5.0rc2/dbt/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/parser/analysis.py` & `dbt-core-1.5.0rc2/dbt/parser/analysis.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/parser/base.py` & `dbt-core-1.5.0rc2/dbt/parser/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/parser/docs.py` & `dbt-core-1.5.0rc2/dbt/parser/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/parser/generic_test.py` & `dbt-core-1.5.0rc2/dbt/parser/generic_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/parser/generic_test_builders.py` & `dbt-core-1.5.0rc2/dbt/parser/generic_test_builders.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/parser/hooks.py` & `dbt-core-1.5.0rc2/dbt/parser/hooks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/parser/macros.py` & `dbt-core-1.5.0rc2/dbt/parser/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/parser/manifest.py` & `dbt-core-1.5.0rc2/dbt/parser/manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1102,15 +1102,15 @@
         name = node.name
         # the full node name is really defined by the adapter's relation
         relation_cls = get_relation_class_by_name(config.credentials.type)
         relation = relation_cls.create_from(config=config, node=node)
         full_node_name = str(relation)
 
         existing_node = names_resources.get(name)
-        if existing_node is not None and existing_node.version is None:
+        if existing_node is not None and not existing_node.is_versioned:
             raise dbt.exceptions.DuplicateResourceNameError(existing_node, node)
 
         existing_alias = alias_resources.get(full_node_name)
         if existing_alias is not None:
             raise AmbiguousAliasError(
                 node_1=existing_alias, node_2=node, duped_name=full_node_name
             )
```

### Comparing `dbt-core-1.5.0rc1/dbt/parser/models.py` & `dbt-core-1.5.0rc2/dbt/parser/models.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/parser/partial.py` & `dbt-core-1.5.0rc2/dbt/parser/partial.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/parser/read_files.py` & `dbt-core-1.5.0rc2/dbt/parser/read_files.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/parser/schema_renderer.py` & `dbt-core-1.5.0rc2/dbt/parser/schema_renderer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/parser/schemas.py` & `dbt-core-1.5.0rc2/dbt/parser/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1064,15 +1064,17 @@
 
         versions = target.versions
         if not versions:
             super().parse_patch(block, refs)
         else:
             assert isinstance(self.yaml.file, SchemaSourceFile)
             source_file: SchemaSourceFile = self.yaml.file
-            latest_version = target.latest_version or max(versions).v
+            latest_version = (
+                target.latest_version if target.latest_version is not None else max(versions).v
+            )
             for unparsed_version in versions:
                 versioned_model_name = (
                     unparsed_version.defined_in or f"{block.name}_{unparsed_version.formatted_v}"
                 )
                 # ref lookup without version - version is not set yet
                 versioned_model_unique_id = self.manifest.ref_lookup.get_unique_id(
                     versioned_model_name, None, None
```

### Comparing `dbt-core-1.5.0rc1/dbt/parser/search.py` & `dbt-core-1.5.0rc2/dbt/parser/search.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/parser/seeds.py` & `dbt-core-1.5.0rc2/dbt/parser/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/parser/singular_test.py` & `dbt-core-1.5.0rc2/dbt/parser/singular_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/parser/snapshots.py` & `dbt-core-1.5.0rc2/dbt/parser/snapshots.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/parser/sources.py` & `dbt-core-1.5.0rc2/dbt/parser/sources.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/parser/sql.py` & `dbt-core-1.5.0rc2/dbt/parser/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/semver.py` & `dbt-core-1.5.0rc2/dbt/semver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/base.py` & `dbt-core-1.5.0rc2/dbt/task/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/build.py` & `dbt-core-1.5.0rc2/dbt/task/build.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/clean.py` & `dbt-core-1.5.0rc2/dbt/task/clean.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/compile.py` & `dbt-core-1.5.0rc2/dbt/task/compile.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/debug.py` & `dbt-core-1.5.0rc2/dbt/task/debug.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/deps.py` & `dbt-core-1.5.0rc2/dbt/task/deps.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/freshness.py` & `dbt-core-1.5.0rc2/dbt/task/freshness.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/generate.py` & `dbt-core-1.5.0rc2/dbt/task/generate.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/init.py` & `dbt-core-1.5.0rc2/dbt/task/init.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/list.py` & `dbt-core-1.5.0rc2/dbt/task/list.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/printer.py` & `dbt-core-1.5.0rc2/dbt/task/printer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/run.py` & `dbt-core-1.5.0rc2/dbt/task/run.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/run_operation.py` & `dbt-core-1.5.0rc2/dbt/task/run_operation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/runnable.py` & `dbt-core-1.5.0rc2/dbt/task/runnable.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/seed.py` & `dbt-core-1.5.0rc2/dbt/task/seed.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/serve.py` & `dbt-core-1.5.0rc2/dbt/task/serve.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/show.py` & `dbt-core-1.5.0rc2/dbt/task/show.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/snapshot.py` & `dbt-core-1.5.0rc2/dbt/task/snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/sql.py` & `dbt-core-1.5.0rc2/dbt/task/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/task/test.py` & `dbt-core-1.5.0rc2/dbt/task/test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/tests/fixtures/project.py` & `dbt-core-1.5.0rc2/dbt/tests/fixtures/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/tests/util.py` & `dbt-core-1.5.0rc2/dbt/tests/util.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/tracking.py` & `dbt-core-1.5.0rc2/dbt/tracking.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/ui.py` & `dbt-core-1.5.0rc2/dbt/ui.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/utils.py` & `dbt-core-1.5.0rc2/dbt/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/dbt/version.py` & `dbt-core-1.5.0rc2/dbt/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,9 +228,9 @@
             # the path is like .../dbt/adapters/{plugin_name}/__version__.py
             # except it could be \\ on windows!
             plugin_root, _ = os.path.split(version_path)
             _, plugin_name = os.path.split(plugin_root)
             yield plugin_name
 
 
-__version__ = "1.5.0rc1"
+__version__ = "1.5.0rc2"
 installed = get_installed_version()
```

### Comparing `dbt-core-1.5.0rc1/dbt_core.egg-info/PKG-INFO` & `dbt-core-1.5.0rc2/dbt_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.5.0rc1
+Version: 1.5.0rc2
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.5.0rc1 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.5.0rc2 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `dbt-core-1.5.0rc1/dbt_core.egg-info/SOURCES.txt` & `dbt-core-1.5.0rc2/dbt_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc1/setup.py` & `dbt-core-1.5.0rc2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 
 package_name = "dbt-core"
-package_version = "1.5.0rc1"
+package_version = "1.5.0rc2"
 description = """With dbt, data analysts and engineers can build analytics \
 the way engineers build applications."""
 
 
 setup(
     name=package_name,
     version=package_version,
@@ -54,15 +54,15 @@
         "isodate>=0.6,<0.7",
         "logbook>=1.5,<1.6",
         "mashumaro[msgpack]==3.6",
         "minimal-snowplow-tracker==0.0.2",
         "networkx>=2.3,<2.8.1;python_version<'3.8'",
         "networkx>=2.3,<3;python_version>='3.8'",
         "packaging>20.9",
-        "sqlparse>=0.2.3,<0.5",
+        "sqlparse>=0.2.3,<0.4.4",
         "dbt-extractor~=0.4.1",
         "typing-extensions>=3.7.4",
         "werkzeug>=1,<3",
         "pathspec>=0.9,<0.12",
         "protobuf>=3.18.3",
         "pytz>=2015.7",
         # the following are all to match snowflake-connector-python
```

