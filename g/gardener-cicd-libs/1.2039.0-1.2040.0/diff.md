# Comparing `tmp/gardener-cicd-libs-1.2039.0.tar.gz` & `tmp/gardener-cicd-libs-1.2040.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-libs-1.2039.0.tar", last modified: Wed Apr 26 09:06:51 2023, max compression
+gzip compressed data, was "gardener-cicd-libs-1.2040.0.tar", last modified: Thu Apr 27 07:34:45 2023, max compression
```

## Comparing `gardener-cicd-libs-1.2039.0.tar` & `gardener-cicd-libs-1.2040.0.tar`

### file list

```diff
@@ -1,278 +1,279 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.629016 gardener-cicd-libs-1.2039.0/
--rw-r--r--   0 root         (0) root         (0)    16830 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      132 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/NOTICE.md
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-26 09:06:51.629016 gardener-cicd-libs-1.2039.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1820 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.597016 gardener-cicd-libs-1.2039.0/ccc/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ccc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      631 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ccc/alicloud.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ccc/aws.py
--rw-r--r--   0 root         (0) root         (0)      127 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ccc/cfg.py
--rw-r--r--   0 root         (0) root         (0)     1725 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ccc/clamav.py
--rw-r--r--   0 root         (0) root         (0)     4131 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ccc/concourse.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ccc/delivery.py
--rw-r--r--   0 root         (0) root         (0)     6490 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ccc/elasticsearch.py
--rw-r--r--   0 root         (0) root         (0)     8491 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ccc/gcp.py
--rw-r--r--   0 root         (0) root         (0)    10735 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ccc/github.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ccc/grafeas_model.py
--rw-r--r--   0 root         (0) root         (0)     1074 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ccc/jira.py
--rw-r--r--   0 root         (0) root         (0)     4925 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ccc/oci.py
--rw-r--r--   0 root         (0) root         (0)     1525 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ccc/protecode.py
--rw-r--r--   0 root         (0) root         (0)     7274 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ccc/secrets_server.py
--rw-r--r--   0 root         (0) root         (0)      139 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ccc/slack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.601016 gardener-cicd-libs-1.2039.0/cfg_mgmt/
--rw-r--r--   0 root         (0) root         (0)      244 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cfg_mgmt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4989 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cfg_mgmt/alicloud.py
--rw-r--r--   0 root         (0) root         (0)     3198 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cfg_mgmt/aws.py
--rw-r--r--   0 root         (0) root         (0)     6025 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cfg_mgmt/azure.py
--rw-r--r--   0 root         (0) root         (0)     8833 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cfg_mgmt/btp_application_certificate.py
--rw-r--r--   0 root         (0) root         (0)     7254 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cfg_mgmt/btp_service_binding.py
--rw-r--r--   0 root         (0) root         (0)     3433 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cfg_mgmt/gcp.py
--rw-r--r--   0 root         (0) root         (0)     6051 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cfg_mgmt/github.py
--rw-r--r--   0 root         (0) root         (0)     7730 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cfg_mgmt/kubernetes.py
--rw-r--r--   0 root         (0) root         (0)     3635 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cfg_mgmt/metrics.py
--rw-r--r--   0 root         (0) root         (0)     9713 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cfg_mgmt/model.py
--rw-r--r--   0 root         (0) root         (0)    16043 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cfg_mgmt/reporting.py
--rw-r--r--   0 root         (0) root         (0)     6143 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cfg_mgmt/rotate.py
--rw-r--r--   0 root         (0) root         (0)     9233 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cfg_mgmt/util.py
--rwxr-xr-x   0 root         (0) root         (0)     9186 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.601016 gardener-cicd-libs-1.2039.0/cnudie/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cnudie/__init__.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cnudie/access.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cnudie/iter.py
--rw-r--r--   0 root         (0) root         (0)      197 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cnudie/migrate.py
--rw-r--r--   0 root         (0) root         (0)     5996 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cnudie/purge.py
--rw-r--r--   0 root         (0) root         (0)     3582 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cnudie/replicate.py
--rw-r--r--   0 root         (0) root         (0)    20986 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cnudie/retrieve.py
--rw-r--r--   0 root         (0) root         (0)    19528 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cnudie/util.py
--rw-r--r--   0 root         (0) root         (0)     2662 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cnudie/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.605016 gardener-cicd-libs-1.2039.0/concourse/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.605016 gardener-cicd-libs-1.2039.0/concourse/client/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14969 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/client/api.py
--rw-r--r--   0 root         (0) root         (0)    15599 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/client/model.py
--rw-r--r--   0 root         (0) root         (0)     6557 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/client/routes.py
--rw-r--r--   0 root         (0) root         (0)    12621 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/client/util.py
--rw-r--r--   0 root         (0) root         (0)    20369 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/enumerator.py
--rw-r--r--   0 root         (0) root         (0)    10077 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.605016 gardener-cicd-libs-1.2039.0/concourse/model/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7643 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/base.py
--rw-r--r--   0 root         (0) root         (0)    10402 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/job.py
--rw-r--r--   0 root         (0) root         (0)     1156 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    12384 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/resources.py
--rw-r--r--   0 root         (0) root         (0)    17522 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/step.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.609016 gardener-cicd-libs-1.2039.0/concourse/model/traits/
--rw-r--r--   0 root         (0) root         (0)     2587 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/traits/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14494 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/traits/component_descriptor.py
--rw-r--r--   0 root         (0) root         (0)     5217 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/traits/cronjob.py
--rw-r--r--   0 root         (0) root         (0)     2763 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/traits/draft_release.py
--rw-r--r--   0 root         (0) root         (0)     4548 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/traits/filter.py
--rw-r--r--   0 root         (0) root         (0)    19200 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/traits/image_scan.py
--rw-r--r--   0 root         (0) root         (0)     5660 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/traits/images.py
--rw-r--r--   0 root         (0) root         (0)     2297 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/traits/meta.py
--rw-r--r--   0 root         (0) root         (0)     6530 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/traits/notifications.py
--rw-r--r--   0 root         (0) root         (0)     1948 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/traits/options.py
--rw-r--r--   0 root         (0) root         (0)    17352 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/traits/publish.py
--rw-r--r--   0 root         (0) root         (0)     4400 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/traits/pullrequest.py
--rw-r--r--   0 root         (0) root         (0)    10248 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/traits/release.py
--rw-r--r--   0 root         (0) root         (0)     8268 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/traits/scan_sources.py
--rw-r--r--   0 root         (0) root         (0)     1591 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/traits/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     2705 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/traits/slack.py
--rw-r--r--   0 root         (0) root         (0)     9849 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/traits/update_component_deps.py
--rw-r--r--   0 root         (0) root         (0)     4420 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/model/traits/version.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/paths.py
--rw-r--r--   0 root         (0) root         (0)    27053 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/replicator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.609016 gardener-cicd-libs-1.2039.0/concourse/resources/
--rw-r--r--   0 root         (0) root         (0)        9 2023-04-26 09:06:46.000000 gardener-cicd-libs-1.2039.0/concourse/resources/LAST_RELEASED_TAG
--rw-r--r--   0 root         (0) root         (0)     1040 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/resources/defaults.mako
--rw-r--r--   0 root         (0) root         (0)     1039 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/resources/email.mako
--rw-r--r--   0 root         (0) root         (0)     4192 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/resources/github.mako
--rw-r--r--   0 root         (0) root         (0)      463 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/resources/image.mako
--rw-r--r--   0 root         (0) root         (0)      639 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/resources/resource_types.mako
--rw-r--r--   0 root         (0) root         (0)      389 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/resources/time.mako
--rw-r--r--   0 root         (0) root         (0)     1301 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/resources/variants.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.613016 gardener-cicd-libs-1.2039.0/concourse/steps/
--rw-r--r--   0 root         (0) root         (0)     1368 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1357 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/alter_container_images.py
--rw-r--r--   0 root         (0) root         (0)     9157 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/build_oci_image.mako
--rw-r--r--   0 root         (0) root         (0)     3137 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/build_oci_image.py
--rw-r--r--   0 root         (0) root         (0)     3016 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/cfg_reporting.mako
--rw-r--r--   0 root         (0) root         (0)     4097 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/cfg_reporting.py
--rw-r--r--   0 root         (0) root         (0)    11982 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/component_descriptor.mako
--rw-r--r--   0 root         (0) root         (0)     5479 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/component_descriptor.py
--rw-r--r--   0 root         (0) root         (0)     3439 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/component_descriptor_util.py
--rw-r--r--   0 root         (0) root         (0)     3909 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/draft_release.mako
--rw-r--r--   0 root         (0) root         (0)     1497 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/images.py
--rw-r--r--   0 root         (0) root         (0)     9852 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/malware_scan.mako
--rw-r--r--   0 root         (0) root         (0)      676 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/meta.mako
--rw-r--r--   0 root         (0) root         (0)      977 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/meta.py
--rw-r--r--   0 root         (0) root         (0)     8822 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/notification.mako
--rw-r--r--   0 root         (0) root         (0)     4621 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/notification.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/os_id.mako
--rw-r--r--   0 root         (0) root         (0)     5203 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/os_id.py
--rw-r--r--   0 root         (0) root         (0)     1743 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/prepare.mako
--rw-r--r--   0 root         (0) root         (0)     3660 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/publish.mako
--rw-r--r--   0 root         (0) root         (0)     4039 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/release.mako
--rw-r--r--   0 root         (0) root         (0)    35385 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/release.py
--rw-r--r--   0 root         (0) root         (0)     1145 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/replicate_pipelines.mako
--rw-r--r--   0 root         (0) root         (0)     1002 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/replicate_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     4579 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/replicate_secrets.mako
--rw-r--r--   0 root         (0) root         (0)     4902 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/replicate_secrets.py
--rw-r--r--   0 root         (0) root         (0)     1518 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/rm_pr_label.mako
--rw-r--r--   0 root         (0) root         (0)     7028 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/scan_container_images.mako
--rw-r--r--   0 root         (0) root         (0)     8649 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/scan_container_images.py
--rw-r--r--   0 root         (0) root         (0)     4703 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/scan_sources.mako
--rw-r--r--   0 root         (0) root         (0)     2107 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/scan_sources.py
--rw-r--r--   0 root         (0) root         (0)     6482 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/update_component_deps.mako
--rw-r--r--   0 root         (0) root         (0)    18639 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/update_component_deps.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/version.mako
--rw-r--r--   0 root         (0) root         (0)     1165 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/steps/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.613016 gardener-cicd-libs-1.2039.0/concourse/templates/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23433 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/templates/default.mako
--rw-r--r--   0 root         (0) root         (0)     5362 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/util.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/concourse/validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.613016 gardener-cicd-libs-1.2039.0/container/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/container/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16315 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/container/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.613016 gardener-cicd-libs-1.2039.0/cosign/
--rw-r--r--   0 root         (0) root         (0)      735 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cosign/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/cosign/payload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.617016 gardener-cicd-libs-1.2039.0/ctt/
--rw-r--r--   0 root         (0) root         (0)      132 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ctt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1802 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ctt/cosign.py
--rw-r--r--   0 root         (0) root         (0)     2085 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ctt/filters.py
--rw-r--r--   0 root         (0) root         (0)     2769 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ctt/platform.py
--rwxr-xr-x   0 root         (0) root         (0)    26860 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ctt/process_dependencies.py
--rw-r--r--   0 root         (0) root         (0)      559 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ctt/processing_model.py
--rw-r--r--   0 root         (0) root         (0)     1212 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ctt/processors.py
--rw-r--r--   0 root         (0) root         (0)     6811 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ctt/rbsc_bom.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.617016 gardener-cicd-libs-1.2039.0/ctt/test/
--rw-r--r--   0 root         (0) root         (0)      306 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ctt/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1683 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ctt/test/filters_test.py
--rw-r--r--   0 root         (0) root         (0)     2719 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ctt/test/platform_test.py
--rw-r--r--   0 root         (0) root         (0)     1272 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ctt/test/process_deps_test.py
--rw-r--r--   0 root         (0) root         (0)     1048 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ctt/test/processors_test.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ctt/test/uploaders_test.py
--rw-r--r--   0 root         (0) root         (0)     7562 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ctt/uploaders.py
--rw-r--r--   0 root         (0) root         (0)     2719 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ctt/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.617016 gardener-cicd-libs-1.2039.0/delivery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/delivery/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10448 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/delivery/client.py
--rw-r--r--   0 root         (0) root         (0)     2921 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/delivery/model.py
--rw-r--r--   0 root         (0) root         (0)     1815 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/delivery/util.py
--rw-r--r--   0 root         (0) root         (0)     2025 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/dockerutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.617016 gardener-cicd-libs-1.2039.0/dso/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/dso/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9505 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/dso/cvss.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/dso/labels.py
--rw-r--r--   0 root         (0) root         (0)     5098 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/dso/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.617016 gardener-cicd-libs-1.2039.0/gardener_cicd_libs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-26 09:06:51.000000 gardener-cicd-libs-1.2039.0/gardener_cicd_libs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6182 2023-04-26 09:06:51.000000 gardener-cicd-libs-1.2039.0/gardener_cicd_libs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 09:06:51.000000 gardener-cicd-libs-1.2039.0/gardener_cicd_libs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      945 2023-04-26 09:06:51.000000 gardener-cicd-libs-1.2039.0/gardener_cicd_libs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      233 2023-04-26 09:06:51.000000 gardener-cicd-libs-1.2039.0/gardener_cicd_libs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.621016 gardener-cicd-libs-1.2039.0/github/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/github/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8440 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/github/codeowners.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.621016 gardener-cicd-libs-1.2039.0/github/compliance/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/github/compliance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11313 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/github/compliance/issue.py
--rw-r--r--   0 root         (0) root         (0)      823 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/github/compliance/milestone.py
--rw-r--r--   0 root         (0) root         (0)     9092 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/github/compliance/model.py
--rw-r--r--   0 root         (0) root         (0)    34570 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/github/compliance/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.621016 gardener-cicd-libs-1.2039.0/github/release_notes/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/github/release_notes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4159 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/github/release_notes/model.py
--rw-r--r--   0 root         (0) root         (0)    12572 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/github/release_notes/renderer.py
--rw-r--r--   0 root         (0) root         (0)    19528 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/github/release_notes/util.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/github/retry.py
--rw-r--r--   0 root         (0) root         (0)     1360 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/github/user.py
--rw-r--r--   0 root         (0) root         (0)    33961 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/github/util.py
--rw-r--r--   0 root         (0) root         (0)     2170 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/github/webhook.py
--rw-r--r--   0 root         (0) root         (0)    14123 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/gitutil.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/gziputil.py
--rw-r--r--   0 root         (0) root         (0)     6926 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/http_requests.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/ioutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.621016 gardener-cicd-libs-1.2039.0/kube/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/kube/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4912 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/kube/ctx.py
--rw-r--r--   0 root         (0) root         (0)     2932 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/kube/helm.py
--rw-r--r--   0 root         (0) root         (0)    26693 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/kube/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.621016 gardener-cicd-libs-1.2039.0/mail/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/mail/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1981 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/mail/template_mailer.py
--rw-r--r--   0 root         (0) root         (0)     9573 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/mailutil.py
--rw-r--r--   0 root         (0) root         (0)       87 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/makoutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.621016 gardener-cicd-libs-1.2039.0/product/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/product/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1373 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/product/util.py
--rw-r--r--   0 root         (0) root         (0)    22448 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/product/v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.621016 gardener-cicd-libs-1.2039.0/release_notes/
--rw-r--r--   0 root         (0) root         (0)      913 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/release_notes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10859 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/release_notes/fetch.py
--rw-r--r--   0 root         (0) root         (0)     8252 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/release_notes/model.py
--rw-r--r--   0 root         (0) root         (0)     7716 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/release_notes/utils.py
--rw-r--r--   0 root         (0) root         (0)     1576 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/reutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.621016 gardener-cicd-libs-1.2039.0/saf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/saf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1306 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/saf/client.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/saf/model.py
--rw-r--r--   0 root         (0) root         (0)      174 2023-04-26 09:06:51.629016 gardener-cicd-libs-1.2039.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2096 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.625016 gardener-cicd-libs-1.2039.0/slackclient/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/slackclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3454 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/slackclient/util.py
--rw-r--r--   0 root         (0) root         (0)     6591 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/tarutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.625016 gardener-cicd-libs-1.2039.0/test/
--rw-r--r--   0 root         (0) root         (0)     1241 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2148 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/_test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.625016 gardener-cicd-libs-1.2039.0/test/concourse/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4266 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/client_test.py
--rw-r--r--   0 root         (0) root         (0)     4760 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/factory_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.625016 gardener-cicd-libs-1.2039.0/test/concourse/model/
--rw-r--r--   0 root         (0) root         (0)     1124 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6657 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/model/job_test.py
--rw-r--r--   0 root         (0) root         (0)     3272 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/model/resources_test.py
--rw-r--r--   0 root         (0) root         (0)     2712 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/model/step_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.625016 gardener-cicd-libs-1.2039.0/test/concourse/model/traits/
--rw-r--r--   0 root         (0) root         (0)     1124 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/model/traits/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2465 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/model/traits/component_descriptor_test.py
--rw-r--r--   0 root         (0) root         (0)     7482 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/model/traits/filter_test.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/model/traits/slack_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.625016 gardener-cicd-libs-1.2039.0/test/concourse/resources/
--rw-r--r--   0 root         (0) root         (0)     1458 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6308 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/resources/github_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.625016 gardener-cicd-libs-1.2039.0/test/concourse/steps/
--rw-r--r--   0 root         (0) root         (0)     1124 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/steps/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3035 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/steps/component_descriptor_test.py
--rw-r--r--   0 root         (0) root         (0)     6544 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/steps/notification_test.py
--rw-r--r--   0 root         (0) root         (0)     9484 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/steps/release_test.py
--rw-r--r--   0 root         (0) root         (0)     2153 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/steps/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     6498 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/steps/update_component_deps_test.py
--rw-r--r--   0 root         (0) root         (0)     2273 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/steps/version_test.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/concourse/util_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.625016 gardener-cicd-libs-1.2039.0/test/container/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/container/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.629016 gardener-cicd-libs-1.2039.0/test/github/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/github/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6142 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/github/github_util_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.629016 gardener-cicd-libs-1.2039.0/test/github/release_notes/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/github/release_notes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5803 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/github/release_notes/default_util.py
--rw-r--r--   0 root         (0) root         (0)    18172 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/github/release_notes/renderer_test.py
--rw-r--r--   0 root         (0) root         (0)    21822 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/github/release_notes/util_test.py
--rw-r--r--   0 root         (0) root         (0)     2262 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/kubeutil_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.629016 gardener-cicd-libs-1.2039.0/test/product_/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/product_/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/reutil_test.py
--rw-r--r--   0 root         (0) root         (0)     5754 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/test/version_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:06:51.629016 gardener-cicd-libs-1.2039.0/unixutil/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/unixutil/__init__.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/unixutil/model.py
--rw-r--r--   0 root         (0) root         (0)     3717 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/unixutil/scan.py
--rw-r--r--   0 root         (0) root         (0)    15220 2023-04-26 08:39:59.000000 gardener-cicd-libs-1.2039.0/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.010174 gardener-cicd-libs-1.2040.0/
+-rw-r--r--   0 root         (0) root         (0)    16830 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/NOTICE.md
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-27 07:34:45.010174 gardener-cicd-libs-1.2040.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:44.978173 gardener-cicd-libs-1.2040.0/ccc/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ccc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      631 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ccc/alicloud.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ccc/aws.py
+-rw-r--r--   0 root         (0) root         (0)      127 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ccc/cfg.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ccc/clamav.py
+-rw-r--r--   0 root         (0) root         (0)     4131 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ccc/concourse.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ccc/delivery.py
+-rw-r--r--   0 root         (0) root         (0)     6490 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ccc/elasticsearch.py
+-rw-r--r--   0 root         (0) root         (0)     8491 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ccc/gcp.py
+-rw-r--r--   0 root         (0) root         (0)    10735 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ccc/github.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ccc/grafeas_model.py
+-rw-r--r--   0 root         (0) root         (0)     1074 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ccc/jira.py
+-rw-r--r--   0 root         (0) root         (0)     4925 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ccc/oci.py
+-rw-r--r--   0 root         (0) root         (0)     1525 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ccc/protecode.py
+-rw-r--r--   0 root         (0) root         (0)     7274 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ccc/secrets_server.py
+-rw-r--r--   0 root         (0) root         (0)      139 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ccc/slack.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:44.982174 gardener-cicd-libs-1.2040.0/cfg_mgmt/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cfg_mgmt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4989 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cfg_mgmt/alicloud.py
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cfg_mgmt/aws.py
+-rw-r--r--   0 root         (0) root         (0)     6025 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cfg_mgmt/azure.py
+-rw-r--r--   0 root         (0) root         (0)     8833 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cfg_mgmt/btp_application_certificate.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cfg_mgmt/btp_service_binding.py
+-rw-r--r--   0 root         (0) root         (0)     3433 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cfg_mgmt/gcp.py
+-rw-r--r--   0 root         (0) root         (0)     6051 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cfg_mgmt/github.py
+-rw-r--r--   0 root         (0) root         (0)     7730 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cfg_mgmt/kubernetes.py
+-rw-r--r--   0 root         (0) root         (0)     3635 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cfg_mgmt/metrics.py
+-rw-r--r--   0 root         (0) root         (0)     9713 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cfg_mgmt/model.py
+-rw-r--r--   0 root         (0) root         (0)    16043 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cfg_mgmt/reporting.py
+-rw-r--r--   0 root         (0) root         (0)     6143 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cfg_mgmt/rotate.py
+-rw-r--r--   0 root         (0) root         (0)     9233 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cfg_mgmt/util.py
+-rwxr-xr-x   0 root         (0) root         (0)     9186 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:44.982174 gardener-cicd-libs-1.2040.0/cnudie/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cnudie/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cnudie/access.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cnudie/iter.py
+-rw-r--r--   0 root         (0) root         (0)      197 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cnudie/migrate.py
+-rw-r--r--   0 root         (0) root         (0)     5996 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cnudie/purge.py
+-rw-r--r--   0 root         (0) root         (0)     3582 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cnudie/replicate.py
+-rw-r--r--   0 root         (0) root         (0)    20986 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cnudie/retrieve.py
+-rw-r--r--   0 root         (0) root         (0)    19528 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cnudie/util.py
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cnudie/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:44.982174 gardener-cicd-libs-1.2040.0/concourse/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:44.986173 gardener-cicd-libs-1.2040.0/concourse/client/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14969 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/client/api.py
+-rw-r--r--   0 root         (0) root         (0)    15599 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/client/model.py
+-rw-r--r--   0 root         (0) root         (0)     6557 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/client/routes.py
+-rw-r--r--   0 root         (0) root         (0)    12621 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/client/util.py
+-rw-r--r--   0 root         (0) root         (0)    20369 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/enumerator.py
+-rw-r--r--   0 root         (0) root         (0)    10077 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:44.986173 gardener-cicd-libs-1.2040.0/concourse/model/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7643 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/base.py
+-rw-r--r--   0 root         (0) root         (0)    10402 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/job.py
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    12384 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/resources.py
+-rw-r--r--   0 root         (0) root         (0)    17522 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/step.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:44.990173 gardener-cicd-libs-1.2040.0/concourse/model/traits/
+-rw-r--r--   0 root         (0) root         (0)     2587 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/traits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14494 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/traits/component_descriptor.py
+-rw-r--r--   0 root         (0) root         (0)     5217 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/traits/cronjob.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/traits/draft_release.py
+-rw-r--r--   0 root         (0) root         (0)     4548 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/traits/filter.py
+-rw-r--r--   0 root         (0) root         (0)    19200 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/traits/image_scan.py
+-rw-r--r--   0 root         (0) root         (0)     5660 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/traits/images.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/traits/meta.py
+-rw-r--r--   0 root         (0) root         (0)     6530 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/traits/notifications.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/traits/options.py
+-rw-r--r--   0 root         (0) root         (0)    17352 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/traits/publish.py
+-rw-r--r--   0 root         (0) root         (0)     4400 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/traits/pullrequest.py
+-rw-r--r--   0 root         (0) root         (0)    11334 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/traits/release.py
+-rw-r--r--   0 root         (0) root         (0)     8268 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/traits/scan_sources.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/traits/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/traits/slack.py
+-rw-r--r--   0 root         (0) root         (0)     9849 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/traits/update_component_deps.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/model/traits/version.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/paths.py
+-rw-r--r--   0 root         (0) root         (0)    27053 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/replicator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:44.990173 gardener-cicd-libs-1.2040.0/concourse/resources/
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-27 07:34:39.000000 gardener-cicd-libs-1.2040.0/concourse/resources/LAST_RELEASED_TAG
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/resources/defaults.mako
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/resources/email.mako
+-rw-r--r--   0 root         (0) root         (0)     4192 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/resources/github.mako
+-rw-r--r--   0 root         (0) root         (0)      463 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/resources/image.mako
+-rw-r--r--   0 root         (0) root         (0)      639 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/resources/resource_types.mako
+-rw-r--r--   0 root         (0) root         (0)      389 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/resources/time.mako
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/resources/variants.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:44.994174 gardener-cicd-libs-1.2040.0/concourse/steps/
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/alter_container_images.py
+-rw-r--r--   0 root         (0) root         (0)     9157 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/build_oci_image.mako
+-rw-r--r--   0 root         (0) root         (0)     3137 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/build_oci_image.py
+-rw-r--r--   0 root         (0) root         (0)     3016 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/cfg_reporting.mako
+-rw-r--r--   0 root         (0) root         (0)     4097 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/cfg_reporting.py
+-rw-r--r--   0 root         (0) root         (0)    11982 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/component_descriptor.mako
+-rw-r--r--   0 root         (0) root         (0)     5479 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/component_descriptor.py
+-rw-r--r--   0 root         (0) root         (0)     3439 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/component_descriptor_util.py
+-rw-r--r--   0 root         (0) root         (0)     3909 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/draft_release.mako
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/images.py
+-rw-r--r--   0 root         (0) root         (0)     9852 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/malware_scan.mako
+-rw-r--r--   0 root         (0) root         (0)      676 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/meta.mako
+-rw-r--r--   0 root         (0) root         (0)      977 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/meta.py
+-rw-r--r--   0 root         (0) root         (0)     8822 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/notification.mako
+-rw-r--r--   0 root         (0) root         (0)     4621 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/notification.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/os_id.mako
+-rw-r--r--   0 root         (0) root         (0)     5203 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/os_id.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/prepare.mako
+-rw-r--r--   0 root         (0) root         (0)     3660 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/publish.mako
+-rw-r--r--   0 root         (0) root         (0)     4201 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/release.mako
+-rw-r--r--   0 root         (0) root         (0)    37186 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/release.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/replicate_pipelines.mako
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/replicate_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     4579 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/replicate_secrets.mako
+-rw-r--r--   0 root         (0) root         (0)     4902 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/replicate_secrets.py
+-rw-r--r--   0 root         (0) root         (0)     1518 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/rm_pr_label.mako
+-rw-r--r--   0 root         (0) root         (0)     7028 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/scan_container_images.mako
+-rw-r--r--   0 root         (0) root         (0)     8649 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/scan_container_images.py
+-rw-r--r--   0 root         (0) root         (0)     4703 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/scan_sources.mako
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/scan_sources.py
+-rw-r--r--   0 root         (0) root         (0)     6482 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/update_component_deps.mako
+-rw-r--r--   0 root         (0) root         (0)    18639 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/update_component_deps.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/version.mako
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/steps/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:44.994174 gardener-cicd-libs-1.2040.0/concourse/templates/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23433 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/templates/default.mako
+-rw-r--r--   0 root         (0) root         (0)     5362 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/util.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/concourse/validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:44.994174 gardener-cicd-libs-1.2040.0/container/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/container/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16315 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/container/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:44.994174 gardener-cicd-libs-1.2040.0/cosign/
+-rw-r--r--   0 root         (0) root         (0)      735 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cosign/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/cosign/payload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:44.998174 gardener-cicd-libs-1.2040.0/ctt/
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ctt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ctt/cosign.py
+-rw-r--r--   0 root         (0) root         (0)     2085 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ctt/filters.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ctt/platform.py
+-rwxr-xr-x   0 root         (0) root         (0)    26860 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ctt/process_dependencies.py
+-rw-r--r--   0 root         (0) root         (0)      559 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ctt/processing_model.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ctt/processors.py
+-rw-r--r--   0 root         (0) root         (0)     6811 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ctt/rbsc_bom.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:44.998174 gardener-cicd-libs-1.2040.0/ctt/test/
+-rw-r--r--   0 root         (0) root         (0)      306 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ctt/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1683 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ctt/test/filters_test.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ctt/test/platform_test.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ctt/test/process_deps_test.py
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ctt/test/processors_test.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ctt/test/uploaders_test.py
+-rw-r--r--   0 root         (0) root         (0)     7562 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ctt/uploaders.py
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ctt/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:44.998174 gardener-cicd-libs-1.2040.0/delivery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/delivery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10448 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/delivery/client.py
+-rw-r--r--   0 root         (0) root         (0)     2921 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/delivery/model.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/delivery/util.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/dockerutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:44.998174 gardener-cicd-libs-1.2040.0/dso/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/dso/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9505 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/dso/cvss.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/dso/labels.py
+-rw-r--r--   0 root         (0) root         (0)     5098 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/dso/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:44.998174 gardener-cicd-libs-1.2040.0/gardener_cicd_libs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-27 07:34:44.000000 gardener-cicd-libs-1.2040.0/gardener_cicd_libs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6208 2023-04-27 07:34:44.000000 gardener-cicd-libs-1.2040.0/gardener_cicd_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 07:34:44.000000 gardener-cicd-libs-1.2040.0/gardener_cicd_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      945 2023-04-27 07:34:44.000000 gardener-cicd-libs-1.2040.0/gardener_cicd_libs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      233 2023-04-27 07:34:44.000000 gardener-cicd-libs-1.2040.0/gardener_cicd_libs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:44.998174 gardener-cicd-libs-1.2040.0/github/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/github/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8440 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/github/codeowners.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.002174 gardener-cicd-libs-1.2040.0/github/compliance/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/github/compliance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11313 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/github/compliance/issue.py
+-rw-r--r--   0 root         (0) root         (0)      823 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/github/compliance/milestone.py
+-rw-r--r--   0 root         (0) root         (0)     9092 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/github/compliance/model.py
+-rw-r--r--   0 root         (0) root         (0)    34570 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/github/compliance/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.002174 gardener-cicd-libs-1.2040.0/github/release_notes/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/github/release_notes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/github/release_notes/model.py
+-rw-r--r--   0 root         (0) root         (0)    12572 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/github/release_notes/renderer.py
+-rw-r--r--   0 root         (0) root         (0)    19222 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/github/release_notes/util.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/github/retry.py
+-rw-r--r--   0 root         (0) root         (0)     1360 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/github/user.py
+-rw-r--r--   0 root         (0) root         (0)    33961 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/github/util.py
+-rw-r--r--   0 root         (0) root         (0)     2170 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/github/webhook.py
+-rw-r--r--   0 root         (0) root         (0)    15039 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/gitutil.py
+-rw-r--r--   0 root         (0) root         (0)     1740 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/gziputil.py
+-rw-r--r--   0 root         (0) root         (0)     6926 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/http_requests.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/ioutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.002174 gardener-cicd-libs-1.2040.0/kube/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/kube/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4912 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/kube/ctx.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/kube/helm.py
+-rw-r--r--   0 root         (0) root         (0)    26693 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/kube/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.002174 gardener-cicd-libs-1.2040.0/mail/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/mail/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/mail/template_mailer.py
+-rw-r--r--   0 root         (0) root         (0)     9573 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/mailutil.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/makoutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.002174 gardener-cicd-libs-1.2040.0/product/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/product/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1373 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/product/util.py
+-rw-r--r--   0 root         (0) root         (0)    22448 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/product/v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.002174 gardener-cicd-libs-1.2040.0/release_notes/
+-rw-r--r--   0 root         (0) root         (0)      913 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/release_notes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11045 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/release_notes/fetch.py
+-rw-r--r--   0 root         (0) root         (0)     4577 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/release_notes/markdown.py
+-rw-r--r--   0 root         (0) root         (0)     8252 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/release_notes/model.py
+-rw-r--r--   0 root         (0) root         (0)     7272 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/release_notes/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/reutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.002174 gardener-cicd-libs-1.2040.0/saf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/saf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1306 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/saf/client.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/saf/model.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-04-27 07:34:45.010174 gardener-cicd-libs-1.2040.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.002174 gardener-cicd-libs-1.2040.0/slackclient/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/slackclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3454 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/slackclient/util.py
+-rw-r--r--   0 root         (0) root         (0)     6591 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/tarutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.006173 gardener-cicd-libs-1.2040.0/test/
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/_test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.006173 gardener-cicd-libs-1.2040.0/test/concourse/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/client_test.py
+-rw-r--r--   0 root         (0) root         (0)     4760 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/factory_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.006173 gardener-cicd-libs-1.2040.0/test/concourse/model/
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6657 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/model/job_test.py
+-rw-r--r--   0 root         (0) root         (0)     3272 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/model/resources_test.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/model/step_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.006173 gardener-cicd-libs-1.2040.0/test/concourse/model/traits/
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/model/traits/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/model/traits/component_descriptor_test.py
+-rw-r--r--   0 root         (0) root         (0)     7482 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/model/traits/filter_test.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/model/traits/slack_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.006173 gardener-cicd-libs-1.2040.0/test/concourse/resources/
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6308 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/resources/github_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.006173 gardener-cicd-libs-1.2040.0/test/concourse/steps/
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/steps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/steps/component_descriptor_test.py
+-rw-r--r--   0 root         (0) root         (0)     6544 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/steps/notification_test.py
+-rw-r--r--   0 root         (0) root         (0)     9495 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/steps/release_test.py
+-rw-r--r--   0 root         (0) root         (0)     2153 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/steps/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6498 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/steps/update_component_deps_test.py
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/steps/version_test.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/concourse/util_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.006173 gardener-cicd-libs-1.2040.0/test/container/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/container/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.006173 gardener-cicd-libs-1.2040.0/test/github/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/github/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6142 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/github/github_util_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.010174 gardener-cicd-libs-1.2040.0/test/github/release_notes/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/github/release_notes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5803 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/github/release_notes/default_util.py
+-rw-r--r--   0 root         (0) root         (0)    18172 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/github/release_notes/renderer_test.py
+-rw-r--r--   0 root         (0) root         (0)    21822 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/github/release_notes/util_test.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/kubeutil_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.010174 gardener-cicd-libs-1.2040.0/test/product_/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/product_/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/reutil_test.py
+-rw-r--r--   0 root         (0) root         (0)     5754 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/test/version_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 07:34:45.010174 gardener-cicd-libs-1.2040.0/unixutil/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/unixutil/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/unixutil/model.py
+-rw-r--r--   0 root         (0) root         (0)     3717 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/unixutil/scan.py
+-rw-r--r--   0 root         (0) root         (0)    15220 2023-04-27 07:33:17.000000 gardener-cicd-libs-1.2040.0/version.py
```

### Comparing `gardener-cicd-libs-1.2039.0/LICENSE.md` & `gardener-cicd-libs-1.2040.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/README.md` & `gardener-cicd-libs-1.2040.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ccc/__init__.py` & `gardener-cicd-libs-1.2040.0/ccc/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ccc/alicloud.py` & `gardener-cicd-libs-1.2040.0/ccc/alicloud.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ccc/aws.py` & `gardener-cicd-libs-1.2040.0/ccc/aws.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ccc/clamav.py` & `gardener-cicd-libs-1.2040.0/ccc/clamav.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ccc/concourse.py` & `gardener-cicd-libs-1.2040.0/ccc/concourse.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ccc/delivery.py` & `gardener-cicd-libs-1.2040.0/ccc/delivery.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ccc/elasticsearch.py` & `gardener-cicd-libs-1.2040.0/ccc/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ccc/gcp.py` & `gardener-cicd-libs-1.2040.0/ccc/gcp.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ccc/github.py` & `gardener-cicd-libs-1.2040.0/ccc/github.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ccc/grafeas_model.py` & `gardener-cicd-libs-1.2040.0/ccc/grafeas_model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ccc/jira.py` & `gardener-cicd-libs-1.2040.0/ccc/jira.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ccc/oci.py` & `gardener-cicd-libs-1.2040.0/ccc/oci.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ccc/protecode.py` & `gardener-cicd-libs-1.2040.0/ccc/protecode.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ccc/secrets_server.py` & `gardener-cicd-libs-1.2040.0/ccc/secrets_server.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cfg_mgmt/alicloud.py` & `gardener-cicd-libs-1.2040.0/cfg_mgmt/alicloud.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cfg_mgmt/aws.py` & `gardener-cicd-libs-1.2040.0/cfg_mgmt/aws.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cfg_mgmt/azure.py` & `gardener-cicd-libs-1.2040.0/cfg_mgmt/azure.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cfg_mgmt/btp_application_certificate.py` & `gardener-cicd-libs-1.2040.0/cfg_mgmt/btp_application_certificate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cfg_mgmt/btp_service_binding.py` & `gardener-cicd-libs-1.2040.0/cfg_mgmt/btp_service_binding.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cfg_mgmt/gcp.py` & `gardener-cicd-libs-1.2040.0/cfg_mgmt/gcp.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cfg_mgmt/github.py` & `gardener-cicd-libs-1.2040.0/cfg_mgmt/github.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cfg_mgmt/kubernetes.py` & `gardener-cicd-libs-1.2040.0/cfg_mgmt/kubernetes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cfg_mgmt/metrics.py` & `gardener-cicd-libs-1.2040.0/cfg_mgmt/metrics.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cfg_mgmt/model.py` & `gardener-cicd-libs-1.2040.0/cfg_mgmt/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cfg_mgmt/reporting.py` & `gardener-cicd-libs-1.2040.0/cfg_mgmt/reporting.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cfg_mgmt/rotate.py` & `gardener-cicd-libs-1.2040.0/cfg_mgmt/rotate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cfg_mgmt/util.py` & `gardener-cicd-libs-1.2040.0/cfg_mgmt/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cli.py` & `gardener-cicd-libs-1.2040.0/cli.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cnudie/access.py` & `gardener-cicd-libs-1.2040.0/cnudie/access.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cnudie/iter.py` & `gardener-cicd-libs-1.2040.0/cnudie/iter.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cnudie/purge.py` & `gardener-cicd-libs-1.2040.0/cnudie/purge.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cnudie/replicate.py` & `gardener-cicd-libs-1.2040.0/cnudie/replicate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cnudie/retrieve.py` & `gardener-cicd-libs-1.2040.0/cnudie/retrieve.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cnudie/util.py` & `gardener-cicd-libs-1.2040.0/cnudie/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cnudie/validate.py` & `gardener-cicd-libs-1.2040.0/cnudie/validate.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/__init__.py` & `gardener-cicd-libs-1.2040.0/concourse/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/client/__init__.py` & `gardener-cicd-libs-1.2040.0/concourse/client/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/client/api.py` & `gardener-cicd-libs-1.2040.0/concourse/client/api.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/client/model.py` & `gardener-cicd-libs-1.2040.0/concourse/client/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/client/routes.py` & `gardener-cicd-libs-1.2040.0/concourse/client/routes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/client/util.py` & `gardener-cicd-libs-1.2040.0/concourse/client/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/enumerator.py` & `gardener-cicd-libs-1.2040.0/concourse/enumerator.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/factory.py` & `gardener-cicd-libs-1.2040.0/concourse/factory.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/__init__.py` & `gardener-cicd-libs-1.2040.0/concourse/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/base.py` & `gardener-cicd-libs-1.2040.0/concourse/model/base.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/job.py` & `gardener-cicd-libs-1.2040.0/concourse/model/job.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/pipeline.py` & `gardener-cicd-libs-1.2040.0/concourse/model/pipeline.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/resources.py` & `gardener-cicd-libs-1.2040.0/concourse/model/resources.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/step.py` & `gardener-cicd-libs-1.2040.0/concourse/model/step.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/traits/__init__.py` & `gardener-cicd-libs-1.2040.0/concourse/model/traits/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/traits/component_descriptor.py` & `gardener-cicd-libs-1.2040.0/concourse/model/traits/component_descriptor.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/traits/cronjob.py` & `gardener-cicd-libs-1.2040.0/concourse/model/traits/cronjob.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/traits/draft_release.py` & `gardener-cicd-libs-1.2040.0/concourse/model/traits/draft_release.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/traits/filter.py` & `gardener-cicd-libs-1.2040.0/concourse/model/traits/filter.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/traits/image_scan.py` & `gardener-cicd-libs-1.2040.0/concourse/model/traits/image_scan.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/traits/images.py` & `gardener-cicd-libs-1.2040.0/concourse/model/traits/images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/traits/meta.py` & `gardener-cicd-libs-1.2040.0/concourse/model/traits/meta.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/traits/notifications.py` & `gardener-cicd-libs-1.2040.0/concourse/model/traits/notifications.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/traits/options.py` & `gardener-cicd-libs-1.2040.0/concourse/model/traits/options.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/traits/publish.py` & `gardener-cicd-libs-1.2040.0/concourse/model/traits/publish.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/traits/pullrequest.py` & `gardener-cicd-libs-1.2040.0/concourse/model/traits/pullrequest.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/traits/release.py` & `gardener-cicd-libs-1.2040.0/concourse/model/traits/release.py`

 * *Files 12% similar despite different names*

```diff
@@ -82,14 +82,35 @@
 
     TAG_ONLY = EnumValueWithDocumentation(
         value='tag_only',
         doc='publish release tag to dead-end',
     )
 
 
+class ReleaseNotesHandling(EnumWithDocumentation):
+    DEFAULT = EnumValueWithDocumentation(
+        value='default',
+        doc='''
+        Use default version of release note creation code. Use this if you are interested in
+        stability rather than the latest features.
+        ''',
+    )
+    PREVIEW = EnumValueWithDocumentation(
+        value='preview',
+        doc='''
+            Use preview version of release note creation code. Use this to join new features and
+            feature-rollouts.
+
+            .. note::
+                if no features are being tested/rolled-out, using this value is the same as using
+                `default`.
+        '''
+    )
+
+
 ATTRIBUTES = (
     AttributeSpec.optional(
         name='nextversion',
         default=NextVersion.BUMP_MINOR.value,
         doc='specifies how the next development version is to be calculated',
         type=NextVersion,
     ),
@@ -180,15 +201,23 @@
     AttributeSpec.optional(
         name='release_on_github',
         default=True,
         doc='''
         if true, a github release is published.
         ''',
         type=bool
-    )
+    ),
+    AttributeSpec.optional(
+        name='release_notes_handling',
+        default=ReleaseNotesHandling.DEFAULT.value,
+        doc='''
+        configures which iteration of the code to use when generating release notes.
+        ''',
+        type=ReleaseNotesHandling,
+    ),
 )
 
 
 class ReleaseTrait(Trait):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
@@ -236,14 +265,17 @@
         if tags := self.raw.get('git_tags'):
             return tags[0]
         return None
 
     def release_on_github(self) -> bool:
         return self.raw['release_on_github']
 
+    def release_notes_handling(self) -> ReleaseNotesHandling:
+        return ReleaseNotesHandling(self.raw['release_notes_handling'])
+
     def validate(self):
         super().validate()
         if self.nextversion() == version.NOOP and self.next_version_callback_path():
             raise ModelValidationError(
                 f'not possible to configure "next_version_callback" if version is "{version.NOOP}"'
             )
         if not self.github_release_tag():
```

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/traits/scan_sources.py` & `gardener-cicd-libs-1.2040.0/concourse/model/traits/scan_sources.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/traits/scheduling.py` & `gardener-cicd-libs-1.2040.0/concourse/model/traits/scheduling.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/traits/slack.py` & `gardener-cicd-libs-1.2040.0/concourse/model/traits/slack.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/traits/update_component_deps.py` & `gardener-cicd-libs-1.2040.0/concourse/model/traits/update_component_deps.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/model/traits/version.py` & `gardener-cicd-libs-1.2040.0/concourse/model/traits/version.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/replicator.py` & `gardener-cicd-libs-1.2040.0/concourse/replicator.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/resources/defaults.mako` & `gardener-cicd-libs-1.2040.0/concourse/resources/defaults.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/resources/email.mako` & `gardener-cicd-libs-1.2040.0/concourse/resources/email.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/resources/github.mako` & `gardener-cicd-libs-1.2040.0/concourse/resources/github.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/resources/resource_types.mako` & `gardener-cicd-libs-1.2040.0/concourse/resources/resource_types.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/resources/variants.mako` & `gardener-cicd-libs-1.2040.0/concourse/resources/variants.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/__init__.py` & `gardener-cicd-libs-1.2040.0/concourse/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/alter_container_images.py` & `gardener-cicd-libs-1.2040.0/concourse/steps/alter_container_images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/build_oci_image.mako` & `gardener-cicd-libs-1.2040.0/concourse/steps/build_oci_image.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/build_oci_image.py` & `gardener-cicd-libs-1.2040.0/concourse/steps/build_oci_image.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/cfg_reporting.mako` & `gardener-cicd-libs-1.2040.0/concourse/steps/cfg_reporting.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/cfg_reporting.py` & `gardener-cicd-libs-1.2040.0/concourse/steps/cfg_reporting.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/component_descriptor.mako` & `gardener-cicd-libs-1.2040.0/concourse/steps/component_descriptor.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/component_descriptor.py` & `gardener-cicd-libs-1.2040.0/concourse/steps/component_descriptor.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/component_descriptor_util.py` & `gardener-cicd-libs-1.2040.0/concourse/steps/component_descriptor_util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/draft_release.mako` & `gardener-cicd-libs-1.2040.0/concourse/steps/draft_release.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/images.py` & `gardener-cicd-libs-1.2040.0/concourse/steps/images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/malware_scan.mako` & `gardener-cicd-libs-1.2040.0/concourse/steps/malware_scan.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/meta.mako` & `gardener-cicd-libs-1.2040.0/concourse/steps/meta.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/meta.py` & `gardener-cicd-libs-1.2040.0/concourse/steps/meta.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/notification.mako` & `gardener-cicd-libs-1.2040.0/concourse/steps/notification.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/notification.py` & `gardener-cicd-libs-1.2040.0/concourse/steps/notification.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/os_id.mako` & `gardener-cicd-libs-1.2040.0/concourse/steps/os_id.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/os_id.py` & `gardener-cicd-libs-1.2040.0/concourse/steps/os_id.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/prepare.mako` & `gardener-cicd-libs-1.2040.0/concourse/steps/prepare.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/publish.mako` & `gardener-cicd-libs-1.2040.0/concourse/steps/publish.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/release.mako` & `gardener-cicd-libs-1.2040.0/concourse/steps/release.mako`

 * *Files 4% similar despite different names*

```diff
@@ -43,32 +43,33 @@
 component_descriptor_trait = job_variant.trait('component_descriptor')
 component_name = component_descriptor_trait.component_name()
 
 release_callback_path = release_trait.release_callback_path()
 next_version_callback_path = release_trait.next_version_callback_path()
 %>
 import ccc.github
+import ci.util
 import concourse.steps.component_descriptor_util as cdu
-
-${step_lib('release')}
+import concourse.steps.release
+import github.util
 
 with open('${version_file}') as f:
   version_str = f.read()
 
-repo_dir = existing_dir('${repo.resource_name()}')
+repo_dir = ci.util.existing_dir('${repo.resource_name()}')
 repository_branch = '${repo.branch()}'
 
 github_cfg = ccc.github.github_cfg_for_repo_url(
   ci.util.urljoin(
     '${repo.repo_hostname()}',
     '${repo.repo_path()}',
   )
 )
 
-githubrepobranch = GitHubRepoBranch(
+githubrepobranch = github.util.GitHubRepoBranch(
     github_config=github_cfg,
     repo_owner='${repo.repo_owner()}',
     repo_name='${repo.repo_name()}',
     branch=repository_branch,
 )
 
 try:
@@ -81,15 +82,15 @@
 
 % if release_commit_callback_image_reference:
 release_commit_callback_image_reference = '${release_commit_callback_image_reference}'
 % else:
 release_commit_callback_image_reference = None
 % endif
 
-release_and_prepare_next_dev_cycle(
+concourse.steps.release.release_and_prepare_next_dev_cycle(
   component_name=component_name,
   component_descriptor_path='${component_descriptor_path}',
   ctf_path='${ctf_path}',
   % if has_slack_trait:
   slack_channel_configs=${slack_channel_cfgs},
   % endif
   % if release_callback_path:
@@ -111,10 +112,11 @@
   % if release_commit_message_prefix:
   release_commit_message_prefix='${release_commit_message_prefix}',
   % endif
   % if next_cycle_commit_message_prefix:
   next_cycle_commit_message_prefix='${next_cycle_commit_message_prefix}',
   % endif
   github_release_tag=${github_release_tag},
-  git_tags=${git_tags}
+  git_tags=${git_tags},
+  release_notes_handling='${release_trait.release_notes_handling().value}',
 )
 </%def>
```

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/release.py` & `gardener-cicd-libs-1.2040.0/concourse/steps/release.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,29 +24,32 @@
     not_none,
 )
 import cnudie.iter
 import cnudie.retrieve
 import cnudie.util
 import cnudie.validate
 import dockerutil
+import release_notes.fetch
+import release_notes.markdown
 
 from gitutil import GitHelper
 from github.util import (
     GitHubRepositoryHelper,
     GitHubRepoBranch,
 )
 import product.v2
 from github.release_notes.util import (
     fetch_release_notes,
     post_to_slack,
     ReleaseNotes,
 )
 from concourse.model.traits.release import (
-    ReleaseNotesPolicy,
     ReleaseCommitPublishingPolicy,
+    ReleaseNotesHandling,
+    ReleaseNotesPolicy,
 )
 import model.container_registry as cr
 import oci.model
 
 logger = logging.getLogger('step.release')
 
 
@@ -283,15 +286,15 @@
 
 class CreateTagsStep(TransactionalStep):
     def __init__(
         self,
         github_release_tag,
         git_tags,
         github_helper: GitHubRepositoryHelper,
-        git_helper,
+        git_helper: GitHelper,
         release_version,
         publishing_policy: ReleaseCommitPublishingPolicy
     ):
         self.github_helper = github_helper
         self.git_helper = git_helper
 
         self.publishing_policy = publishing_policy
@@ -734,29 +737,29 @@
         return f"Post Slack Release ({self.slack_channel})"
 
     def __init__(
         self,
         slack_cfg_name: str,
         slack_channel: str,
         release_version: str,
-        release_notes: ReleaseNotes,
+        release_notes_markdown: str,
         githubrepobranch: GitHubRepoBranch,
     ):
         self.slack_cfg_name = not_empty(slack_cfg_name)
         self.slack_channel = not_empty(slack_channel)
         self.release_version = not_empty(release_version)
         self.githubrepobranch = not_none(githubrepobranch)
-        self.release_notes = not_none(release_notes)
+        self.release_notes_markdown = not_none(release_notes_markdown)
 
     def validate(self):
         version.parse_to_semver(self.release_version)
 
     def apply(self):
         responses = post_to_slack(
-            release_notes=self.release_notes,
+            release_notes_markdown=self.release_notes_markdown,
             github_repository_name=self.githubrepobranch.github_repo_path(),
             slack_cfg_name=self.slack_cfg_name,
             slack_channel=self.slack_channel,
             release_version=self.release_version,
         )
 
         for response in responses:
@@ -868,14 +871,15 @@
     release_notes_policy: str,
     release_version: str,
     repo_dir: str,
     repository_version_file_path: str,
     git_tags: list,
     github_release_tag: dict,
     release_commit_callback_image_reference: str,
+    release_notes_handling: str,
     component_descriptor_path: str=None,
     ctf_path: str=None,
     next_cycle_commit_message_prefix: str=None,
     next_version_callback: str=None,
     prerelease_suffix: str="dev",
     rebase_before_release: bool=False,
     release_on_github: bool=True,
@@ -907,14 +911,15 @@
 
     transaction_ctx = TransactionContext() # shared between all steps/trxs
 
     release_notes_policy = ReleaseNotesPolicy(release_notes_policy)
     release_commit_publishing_policy = ReleaseCommitPublishingPolicy(
         release_commit_publishing_policy
     )
+    release_notes_handling = ReleaseNotesHandling(release_notes_handling)
     github_helper = GitHubRepositoryHelper.from_githubrepobranch(githubrepobranch)
     git_helper = GitHelper.from_githubrepobranch(
         githubrepobranch=githubrepobranch,
         repo_path=repo_dir,
     )
 
     step_list = []
@@ -988,23 +993,14 @@
         steps=step_list,
     )
 
     release_transaction.validate()
     if not release_transaction.execute():
         raise RuntimeError('An error occurred while creating the Release.')
 
-    if release_on_github:
-        publish_release_notes_step = PublishReleaseNotesStep(
-            githubrepobranch=githubrepobranch,
-            github_helper=github_helper,
-            component=component,
-            release_version=release_version,
-            repo_dir=repo_dir,
-        )
-
     cleanup_draft_releases_step = TryCleanupDraftReleasesStep(
         github_helper=github_helper,
     )
 
     cleanup_draft_releases_transaction = Transaction(
         ctx=transaction_ctx,
         steps=(cleanup_draft_releases_step,),
@@ -1017,37 +1013,76 @@
         return logger.info('release notes were disabled - skipping')
     elif release_notes_policy == ReleaseNotesPolicy.DEFAULT:
         pass
     else:
         raise NotImplementedError(release_notes_policy)
 
     if release_on_github:
-        release_notes_transaction = Transaction(
-            ctx=transaction_ctx,
-            steps=(publish_release_notes_step,),
-        )
-        release_notes_transaction.validate()
-        if not release_notes_transaction.execute():
-            raise RuntimeError('An error occurred while publishing the release notes.')
+        if release_notes_handling is ReleaseNotesHandling.DEFAULT:
+            publish_release_notes_step = PublishReleaseNotesStep(
+                githubrepobranch=githubrepobranch,
+                github_helper=github_helper,
+                component=component,
+                release_version=release_version,
+                repo_dir=repo_dir,
+            )
+            release_notes_transaction = Transaction(
+                ctx=transaction_ctx,
+                steps=(publish_release_notes_step,),
+            )
+            release_notes_transaction.validate()
+            if not release_notes_transaction.execute():
+                raise RuntimeError('An error occurred while publishing the release notes.')
+        elif release_notes_handling is ReleaseNotesHandling.PREVIEW:
+            release_note_blocks = release_notes.fetch.fetch_release_notes(
+                repo_path=repo_dir,
+                component=component,
+                current_version=version.parse_to_semver(release_version),
+            )
+            release_notes_markdown = '\n'.join(
+                str(i) for i in release_notes.markdown.render(release_note_blocks)
+            )
+            github_helper.update_release_notes(
+                tag_name=release_version,
+                body=release_notes_markdown,
+                component_name=component.name,
+            )
+        else:
+            raise NotImplementedError(release_notes_handling)
 
     if slack_channel_configs:
         if not release_on_github:
             raise RuntimeError('Cannot post to slack without a github release')
-        release_notes = transaction_ctx.step_output(
-            publish_release_notes_step.name()
+
+        if release_notes_handling is ReleaseNotesHandling.DEFAULT:
+            release_notes_raw = transaction_ctx.step_output(
+                publish_release_notes_step.name()
             ).get('release notes')
+            # slack can't auto link pull requests, commits or users
+            # hence we force the link generation when building the markdown string
+            logger.info('Creating release-note markdown before posting to Slack')
+            release_notes_markdown = release_notes_raw.to_markdown(
+                force_link_generation=True
+            )
+        elif release_notes_handling is ReleaseNotesHandling.PREVIEW:
+            # release_notes_markdown already prepared earlier albeit without special link
+            # preparation for Slack.
+            pass
+        else:
+            raise NotImplementedError(release_notes_handling)
+
         all_slack_releases_successful = True
         for slack_cfg in slack_channel_configs:
             slack_cfg_name = slack_cfg['slack_cfg_name']
             slack_channel = slack_cfg['channel_name']
             post_to_slack_step = PostSlackReleaseStep(
                 slack_cfg_name=slack_cfg_name,
                 slack_channel=slack_channel,
                 release_version=release_version,
-                release_notes=release_notes,
+                release_notes_markdown=release_notes_markdown,
                 githubrepobranch=githubrepobranch,
             )
             slack_transaction = Transaction(
                 ctx=transaction_ctx,
                 steps=(post_to_slack_step,),
             )
             slack_transaction.validate()
```

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/replicate_pipelines.mako` & `gardener-cicd-libs-1.2040.0/concourse/steps/replicate_pipelines.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/replicate_pipelines.py` & `gardener-cicd-libs-1.2040.0/concourse/steps/replicate_pipelines.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/replicate_secrets.mako` & `gardener-cicd-libs-1.2040.0/concourse/steps/replicate_secrets.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/replicate_secrets.py` & `gardener-cicd-libs-1.2040.0/concourse/steps/replicate_secrets.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/rm_pr_label.mako` & `gardener-cicd-libs-1.2040.0/concourse/steps/rm_pr_label.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/scan_container_images.mako` & `gardener-cicd-libs-1.2040.0/concourse/steps/scan_container_images.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/scan_container_images.py` & `gardener-cicd-libs-1.2040.0/concourse/steps/scan_container_images.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/scan_sources.mako` & `gardener-cicd-libs-1.2040.0/concourse/steps/scan_sources.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/scan_sources.py` & `gardener-cicd-libs-1.2040.0/concourse/steps/scan_sources.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/update_component_deps.mako` & `gardener-cicd-libs-1.2040.0/concourse/steps/update_component_deps.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/update_component_deps.py` & `gardener-cicd-libs-1.2040.0/concourse/steps/update_component_deps.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/version.mako` & `gardener-cicd-libs-1.2040.0/concourse/steps/version.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/steps/version.py` & `gardener-cicd-libs-1.2040.0/concourse/steps/version.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/templates/__init__.py` & `gardener-cicd-libs-1.2040.0/concourse/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/templates/default.mako` & `gardener-cicd-libs-1.2040.0/concourse/templates/default.mako`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/util.py` & `gardener-cicd-libs-1.2040.0/concourse/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/concourse/validator.py` & `gardener-cicd-libs-1.2040.0/concourse/validator.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/container/__init__.py` & `gardener-cicd-libs-1.2040.0/container/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/container/util.py` & `gardener-cicd-libs-1.2040.0/container/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cosign/__init__.py` & `gardener-cicd-libs-1.2040.0/cosign/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/cosign/payload.py` & `gardener-cicd-libs-1.2040.0/cosign/payload.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ctt/cosign.py` & `gardener-cicd-libs-1.2040.0/ctt/cosign.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ctt/filters.py` & `gardener-cicd-libs-1.2040.0/ctt/filters.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ctt/platform.py` & `gardener-cicd-libs-1.2040.0/ctt/platform.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ctt/process_dependencies.py` & `gardener-cicd-libs-1.2040.0/ctt/process_dependencies.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ctt/processing_model.py` & `gardener-cicd-libs-1.2040.0/ctt/processing_model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ctt/processors.py` & `gardener-cicd-libs-1.2040.0/ctt/processors.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ctt/rbsc_bom.py` & `gardener-cicd-libs-1.2040.0/ctt/rbsc_bom.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ctt/test/filters_test.py` & `gardener-cicd-libs-1.2040.0/ctt/test/filters_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ctt/test/platform_test.py` & `gardener-cicd-libs-1.2040.0/ctt/test/platform_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ctt/test/process_deps_test.py` & `gardener-cicd-libs-1.2040.0/ctt/test/process_deps_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ctt/test/processors_test.py` & `gardener-cicd-libs-1.2040.0/ctt/test/processors_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ctt/test/uploaders_test.py` & `gardener-cicd-libs-1.2040.0/ctt/test/uploaders_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ctt/uploaders.py` & `gardener-cicd-libs-1.2040.0/ctt/uploaders.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/ctt/util.py` & `gardener-cicd-libs-1.2040.0/ctt/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/delivery/client.py` & `gardener-cicd-libs-1.2040.0/delivery/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/delivery/model.py` & `gardener-cicd-libs-1.2040.0/delivery/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/delivery/util.py` & `gardener-cicd-libs-1.2040.0/delivery/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/dockerutil.py` & `gardener-cicd-libs-1.2040.0/dockerutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/dso/cvss.py` & `gardener-cicd-libs-1.2040.0/dso/cvss.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/dso/labels.py` & `gardener-cicd-libs-1.2040.0/dso/labels.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/dso/model.py` & `gardener-cicd-libs-1.2040.0/dso/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/gardener_cicd_libs.egg-info/SOURCES.txt` & `gardener-cicd-libs-1.2040.0/gardener_cicd_libs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,15 @@
 mail/__init__.py
 mail/template_mailer.py
 product/__init__.py
 product/util.py
 product/v2.py
 release_notes/__init__.py
 release_notes/fetch.py
+release_notes/markdown.py
 release_notes/model.py
 release_notes/utils.py
 saf/__init__.py
 saf/client.py
 saf/model.py
 slackclient/__init__.py
 slackclient/util.py
```

### Comparing `gardener-cicd-libs-1.2039.0/gardener_cicd_libs.egg-info/requires.txt` & `gardener-cicd-libs-1.2040.0/gardener_cicd_libs.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-gardener-cicd-base>=1.2039.0
-gardener-oci>=1.2039.0
+gardener-cicd-base>=1.2040.0
+gardener-oci>=1.2040.0
 GitPython
 Mako<2.0.0
 Sphinx
 aliyun-python-sdk-core==2.13.36
 aliyun-python-sdk-ecs==4.24.31
 aliyun-python-sdk-ram==3.3.0
 awesomeversion
```

### Comparing `gardener-cicd-libs-1.2039.0/github/__init__.py` & `gardener-cicd-libs-1.2040.0/github/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/github/codeowners.py` & `gardener-cicd-libs-1.2040.0/github/codeowners.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/github/compliance/issue.py` & `gardener-cicd-libs-1.2040.0/github/compliance/issue.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/github/compliance/milestone.py` & `gardener-cicd-libs-1.2040.0/github/compliance/milestone.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/github/compliance/model.py` & `gardener-cicd-libs-1.2040.0/github/compliance/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/github/compliance/report.py` & `gardener-cicd-libs-1.2040.0/github/compliance/report.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/github/release_notes/__init__.py` & `gardener-cicd-libs-1.2040.0/github/release_notes/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/github/release_notes/model.py` & `gardener-cicd-libs-1.2040.0/github/release_notes/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/github/release_notes/renderer.py` & `gardener-cicd-libs-1.2040.0/github/release_notes/renderer.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/github/release_notes/util.py` & `gardener-cicd-libs-1.2040.0/github/release_notes/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,56 +62,49 @@
 ):
     release_notes = ReleaseNotes(component, repo_dir)
     release_notes.create(start_ref=repository_branch)
     return release_notes
 
 
 def post_to_slack(
-    release_notes: ReleaseNote,
+    release_notes_markdown: str,
     github_repository_name: str,
     slack_cfg_name: str,
     slack_channel: str,
     release_version: str,
     max_msg_size_bytes: int=20000,
 ):
-    # slack can't auto link pull requests, commits or users
-    # hence we force the link generation when building the markdown string
-    logger.info('Creating release-note markdown before posting to Slack')
-    release_notes_md_links = release_notes.to_markdown(
-        force_link_generation=True
-    )
-
     # XXX slack imposes a maximum msg size
     # https://api.slack.com/changelog/2018-04-truncating-really-long-messages#
 
     slack_cfg = ctx().cfg_factory().slack(slack_cfg_name)
     slack_helper = SlackHelper(slack_cfg)
 
     idx = 0
     i = 0
 
     try:
         while True:
             title = f'[{github_repository_name}:{release_version} released'
 
             # abort on last
-            if idx + max_msg_size_bytes > len(release_notes_md_links):
+            if idx + max_msg_size_bytes > len(release_notes_markdown):
                 did_split = i > 0
                 if did_split:
                     title += ' - final]'
                 else:
                     title += ']'
 
-                msg = release_notes_md_links[idx:]
+                msg = release_notes_markdown[idx:]
                 yield slack_helper.post_to_slack(channel=slack_channel, title=title, message=msg)
                 break
 
             # post part
             title += f' - part {i} ]'
-            msg = release_notes_md_links[idx: idx+max_msg_size_bytes]
+            msg = release_notes_markdown[idx: idx+max_msg_size_bytes]
             logger.info(f"Posting release-note '{title}'")
             yield slack_helper.post_to_slack(channel=slack_channel, title=title, message=msg)
 
             i += 1
             idx += max_msg_size_bytes
 
     except RuntimeError as e:
```

### Comparing `gardener-cicd-libs-1.2039.0/github/retry.py` & `gardener-cicd-libs-1.2040.0/github/retry.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/github/user.py` & `gardener-cicd-libs-1.2040.0/github/user.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/github/util.py` & `gardener-cicd-libs-1.2040.0/github/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/github/webhook.py` & `gardener-cicd-libs-1.2040.0/github/webhook.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/gitutil.py` & `gardener-cicd-libs-1.2040.0/gitutil.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     id_only = '-o "IdentitiesOnly yes"'
     cmd_env = os.environ.copy()
     cmd_env['GIT_SSH_COMMAND'] = f'ssh -v -i {tmp_id.name} {suppress_hostcheck} {id_only}'
     return (cmd_env, tmp_id)
 
 
 class GitHelper:
-    def __init__(self, repo, github_cfg, github_repo_path):
+    def __init__(self, repo, github_cfg: GithubConfig, github_repo_path):
         not_none(repo)
         if not isinstance(repo, git.Repo):
             # assume it's a file path if it's not already a git.Repo
             repo = git.Repo(str(repo))
         self.repo = repo
         self.github_cfg = github_cfg
         self.github_repo_path = github_repo_path
@@ -117,23 +117,33 @@
         lines = git.cmd.Git(self.repo.working_tree_dir).status('--porcelain=1', '-z').split('\x00')
         # output of git status --porcelain=1 and -z is guaranteed to not change in the future
         return [line[3:] for line in lines if line]
 
     @contextlib.contextmanager
     def _authenticated_remote(self):
         protocol = self.github_cfg.preferred_protocol()
+        credentials = self.github_cfg.credentials()
         if protocol is Protocol.SSH:
             url = urljoin(self.github_cfg.ssh_url(), self.github_repo_path)
             cmd_env, tmp_id = _ssh_auth_env(github_cfg=self.github_cfg)
         elif protocol is Protocol.HTTPS:
-            url = url_with_credentials(self.github_cfg, self.github_repo_path)
+            url = url_with_credentials(
+                github_cfg=self.github_cfg,
+                github_repo_path=self.github_repo_path,
+                technical_user_name=credentials.username(),
+            )
             cmd_env = os.environ
         else:
             raise NotImplementedError
 
+        cmd_env["GIT_AUTHOR_NAME"] = credentials.username()
+        cmd_env["GIT_AUTHOR_EMAIL"] = credentials.email_address()
+        cmd_env['GIT_COMMITTER_NAME'] = credentials.username()
+        cmd_env['GIT_COMMITTER_EMAIL'] = credentials.email_address()
+
         remote = git.remote.Remote.add(
             repo=self.repo,
             name=random_str(),
             url=url,
         )
         logger.info(f'autenticated {remote.name=} using {protocol=}')
 
@@ -238,24 +248,37 @@
                 push_info: git.remote.PushInfo = results[0]
                 if push_info.flags & push_info.ERROR:
                     raise RuntimeError('git-push failed (see stderr output)')
 
     def rebase(self, commit_ish: str):
         self.repo.git.rebase('--quiet', commit_ish)
 
+    def add_note(self, body: str, commit: str):
+        with self._authenticated_remote() as (cmd_env, remote):
+            with remote.repo.git.custom_environment(**cmd_env):
+                remote.repo.git.notes('add', '-f', '-m', body, commit.hexsha)
+
     def fetch_head(self, ref: str):
         with self._authenticated_remote() as (cmd_env, remote):
             with remote.repo.git.custom_environment(**cmd_env):
                 fetch_result = remote.fetch(ref)[0]
                 return fetch_result.commit
 
 
-def url_with_credentials(github_cfg, github_repo_path):
+def url_with_credentials(
+    github_cfg: GithubConfig,
+    github_repo_path: str,
+    technical_user_name: str | None =None
+):
     base_url = urllib.parse.urlparse(github_cfg.http_url())
-    credentials = github_cfg.credentials()
+
+    if technical_user_name:
+        credentials = github_cfg.credentials(technical_user_name=technical_user_name)
+    else:
+        credentials = github_cfg.credentials()
 
     # prefer auth token
     secret = credentials.auth_token() or credentials.passwd()
 
     credentials_str = ':'.join((credentials.username(), secret))
     url = urllib.parse.urlunparse((
         base_url.scheme,
```

### Comparing `gardener-cicd-libs-1.2039.0/gziputil.py` & `gardener-cicd-libs-1.2040.0/gziputil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/http_requests.py` & `gardener-cicd-libs-1.2040.0/http_requests.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/kube/__init__.py` & `gardener-cicd-libs-1.2040.0/kube/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/kube/ctx.py` & `gardener-cicd-libs-1.2040.0/kube/ctx.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/kube/helm.py` & `gardener-cicd-libs-1.2040.0/kube/helm.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/kube/helper.py` & `gardener-cicd-libs-1.2040.0/kube/helper.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/mail/__init__.py` & `gardener-cicd-libs-1.2040.0/mail/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/mail/template_mailer.py` & `gardener-cicd-libs-1.2040.0/mail/template_mailer.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/mailutil.py` & `gardener-cicd-libs-1.2040.0/mailutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/product/__init__.py` & `gardener-cicd-libs-1.2040.0/product/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/product/util.py` & `gardener-cicd-libs-1.2040.0/product/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/product/v2.py` & `gardener-cicd-libs-1.2040.0/product/v2.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/release_notes/__init__.py` & `gardener-cicd-libs-1.2040.0/release_notes/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/release_notes/fetch.py` & `gardener-cicd-libs-1.2040.0/release_notes/fetch.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import git
 import github3.repos
 import semver
 
 import cnudie.retrieve
 import cnudie.util
 import github.release_notes.util as ghrnu
+import gitutil
 import release_notes.model as rnm
 import release_notes.utils as rnu
 import version
 
 logger = logging.getLogger(__name__)
 
 
@@ -36,15 +37,15 @@
         raise RuntimeError('cannot find merge base')
     return tuple(repo.iter_commits(f'{main_tag.commit.hexsha}...{merge_commit.hexsha}'))
 
 
 def _get_release_note_commits_tuple_for_minor_release(
         previous_version: semver.VersionInfo,
         component_versions: dict[semver.VersionInfo, str],
-        git_helper,
+        git_helper: gitutil.GitHelper,
         github_repo: github3.repos.Repository,
         current_version_tag: git.TagReference,
 ) -> tuple[tuple[git.Commit], tuple[git.Commit]]:
     '''
     :return: a tuple of commits which should be included in the release notes
     and a tuple of commits which should not be included in the release notes
     '''
@@ -55,40 +56,45 @@
     previous_minor_version_tag = git_helper.repo.tag(component_versions[previous_minor_version])
     if not previous_minor_version_tag:
         raise RuntimeError('cannot find previous minor version in component versions / tags')
     logger.info(f'found previous minor tag: {previous_minor_version_tag}')
 
     # if the current version tag and the previous minor tag are ancestors, just
     # add the range (old method)
-    if git_helper.repo.is_ancestor(previous_minor_version_tag.commit, current_version_tag.commit):
+    previous_version_tag_commit_sha = git_helper.fetch_head(
+        f'refs/tags/{previous_minor_version_tag}'
+    )
+    current_tag_commit_sha = git_helper.fetch_head(f'refs/tags/{current_version_tag}')
+    if git_helper.repo.is_ancestor(previous_version_tag_commit_sha, current_tag_commit_sha):
         logger.info('it\'s an ancestor. simple range should be enough.')
         return tuple(git_helper.repo.iter_commits(
-            f'{current_version_tag.commit.hexsha}...{previous_minor_version_tag.commit.hexsha}')
+            f'{current_tag_commit_sha}...{previous_version_tag_commit_sha}')
         ), tuple()
 
     # otherwise, use the new method
     # find start of previous minor-release tag
     if not (previous_branch_starts := git_helper.repo.merge_base(
         github_repo.default_branch,
-        previous_minor_version_tag.commit.hexsha)):
+        previous_version_tag_commit_sha)):
         raise RuntimeError('cannot find the branch start for the previous version')
 
     previous_branch_start: git.Commit = previous_branch_starts.pop()
     logger.info(f'it\'s not an ancestor. the branch start appears to be {previous_branch_start}')
 
     # all commits from the branch start to the previous minor-release tag
     # should be removed from the release notes
-    filter_out_commits_range = \
-        f'{previous_minor_version_tag.commit.hexsha}...{previous_branch_start}'
+    filter_out_commits_range = (
+        f'{previous_version_tag_commit_sha}...{previous_branch_start}'
+    )
     logger.debug(f'{filter_out_commits_range=}')
     filter_out_commits = git_helper.repo.iter_commits(filter_out_commits_range)
 
     # all commits (and release notes!) not included in {filter_out_commits} should be added to the
     # final generated release notes
-    filter_in_commits_range = f'{current_version_tag.commit.hexsha}...{previous_branch_start}'
+    filter_in_commits_range = f'{current_tag_commit_sha}...{previous_branch_start}'
     logger.debug(f'{filter_in_commits_range=}')
     filter_in_commits = git_helper.repo.iter_commits(filter_in_commits_range)
 
     return tuple(filter_in_commits), tuple(filter_out_commits)
 
 
 def get_release_note_commits_tuple(
@@ -132,16 +138,15 @@
         raise RuntimeError(
             'cannot create patch-release notes because previous version cannot be found'
         )
     return _list_commits_between_tags(
             git_helper.repo,
             current_version_tag,
             previous_version_tag
-    ),
-    tuple()
+    ), tuple()
 
 
 def fetch_release_notes(
         component: gci.componentmodel.Component,
         repo_path: str,
         current_version: typing.Optional[semver.VersionInfo] = None,
 ) -> set[rnm.ReleaseNote]:
@@ -206,15 +211,15 @@
     )
 
     logger.info(f'requesting associated pull requests for {len(filter_in_commits)} ' +
                 f'filter in and {len(filter_out_commits)} filter out commits')
 
     # find associated pull requests for commits
     commit_pulls = rnu.request_pull_requests_from_api(
-        repo=git_helper.repo,
+        git_helper=git_helper,
         gh=github_helper.github,
         owner=github_repo.owner,
         repo_name=github_repo.name,
         commits=[*filter_in_commits, *filter_out_commits]
     )
     logger.info(f'commit_pulls: {len(commit_pulls)}')
```

### Comparing `gardener-cicd-libs-1.2039.0/release_notes/model.py` & `gardener-cicd-libs-1.2040.0/release_notes/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/release_notes/utils.py` & `gardener-cicd-libs-1.2040.0/release_notes/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import git
 import git.exc as gitexc
 import github3
 import github3.exceptions as gh3e
 import github3.pulls as gh3p
 import github3.structs as gh3s
+import gitutil
 import semver
 import yaml
 import yaml.scanner
 
 import release_notes.model as rnm
 
 _meta_key = 'gardener.cloud/release-notes-metadata/v1'
@@ -40,31 +41,14 @@
         url = gh._build_url('repos', owner, repo, 'commits', sha, 'pulls')
         return tuple(gh._iter(-1, url, gh3p.ShortPullRequest))
     except gh3e.UnprocessableEntity as e:
         logger.debug(f'cannot find any pull request related to commit {sha}: {e}')
         return None
 
 
-def _write_to_git_notes(
-        repo: git.Repo,
-        commit: git.Commit,
-        body: str
-) -> None:
-    ''' Notes can be attached to a commit using
-    `$ git notes add -m <message> <sha>`
-
-    :param repo: the repository the commit belongs to
-    :param commit: the commit to add notes to
-    :param body: the body to write to the commit notes
-    :return:
-    '''
-    logger.debug(f'writing\n{body}\nto{commit.hexsha}\n')
-    repo.git.notes('add', '-f', '-m', body, commit.hexsha)
-
-
 # pylint: disable=protected-access
 # noinspection PyProtectedMember
 def list_pulls(
         gh: github3.GitHub,
         owner: str,
         repo: str,
         state: str = 'closed'
@@ -161,15 +145,15 @@
     if index is not None:
         documents[index] = instance
     else:
         documents.append(instance)
 
 
 def request_pull_requests_from_api(
-        repo: git.Repo,
+        git_helper: gitutil.GitHelper,
         gh: github3.GitHub,
         owner: str,
         repo_name: str,
         commits: list[git.Commit]
 ) -> dict[str, list[gh3p.ShortPullRequest]]:
     ''' This function requests pull requests from the GitHub API and returns a
     dictionary mapping commit SHA to a list of pull requests.
@@ -187,15 +171,15 @@
     pending = collections.defaultdict(list)
     # commit_sha -> [ list of pull requests ]
     result = collections.defaultdict(list)
 
     for commit in commits:
         yaml_documents = []
         is_yaml_content = True
-        if note_content := _find_git_notes_for_commit(repo, commit):
+        if note_content := _find_git_notes_for_commit(git_helper.repo, commit):
             try:
                 yaml_documents = list(yaml.safe_load_all(note_content))
             except yaml.scanner.ScannerError as e:  # YAML parsing error
                 logger.debug(f'the notes of commit {commit.hexsha} do not contain valid YAML: {e}')
                 is_yaml_content = False
 
         # if there is already a ReleaseNotesMetadata
@@ -212,15 +196,15 @@
             if note_content or not is_yaml_content:
                 continue
             data = dataclasses.asdict(
                 rnm.ReleaseNotesMetadata(round(time.time() * 1000), [z.number for z in prs])
             )
             meta = rnm.get_meta_obj(_meta_key, data)
             _upsert_document(yaml_documents, _meta_key, meta)
-            _write_to_git_notes(repo, commit, yaml.safe_dump_all(yaml_documents))
+            git_helper.add_note(body=yaml.safe_dump_all(yaml_documents), commit=commit)
 
     if pending:
         for pull in list_pulls(gh, owner, repo_name):
             if pull.number in pending:
                 for sha in pending[pull.number]:
                     result[sha].append(pull)
                 del pending[pull.number]
```

### Comparing `gardener-cicd-libs-1.2039.0/reutil.py` & `gardener-cicd-libs-1.2040.0/reutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/saf/client.py` & `gardener-cicd-libs-1.2040.0/saf/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/saf/model.py` & `gardener-cicd-libs-1.2040.0/saf/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/setup.py` & `gardener-cicd-libs-1.2040.0/setup.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/slackclient/__init__.py` & `gardener-cicd-libs-1.2040.0/slackclient/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/slackclient/util.py` & `gardener-cicd-libs-1.2040.0/slackclient/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/tarutil.py` & `gardener-cicd-libs-1.2040.0/tarutil.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/__init__.py` & `gardener-cicd-libs-1.2040.0/test/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/_test_utils.py` & `gardener-cicd-libs-1.2040.0/test/_test_utils.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/__init__.py` & `gardener-cicd-libs-1.2040.0/test/concourse/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/client_test.py` & `gardener-cicd-libs-1.2040.0/test/concourse/client_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/factory_test.py` & `gardener-cicd-libs-1.2040.0/test/concourse/factory_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/model/__init__.py` & `gardener-cicd-libs-1.2040.0/test/concourse/model/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/model/job_test.py` & `gardener-cicd-libs-1.2040.0/test/concourse/model/job_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/model/resources_test.py` & `gardener-cicd-libs-1.2040.0/test/concourse/model/resources_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/model/step_test.py` & `gardener-cicd-libs-1.2040.0/test/concourse/model/step_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/model/traits/__init__.py` & `gardener-cicd-libs-1.2040.0/test/concourse/model/traits/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/model/traits/component_descriptor_test.py` & `gardener-cicd-libs-1.2040.0/test/concourse/model/traits/component_descriptor_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/model/traits/filter_test.py` & `gardener-cicd-libs-1.2040.0/test/concourse/model/traits/filter_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/model/traits/slack_test.py` & `gardener-cicd-libs-1.2040.0/test/concourse/model/traits/slack_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/resources/__init__.py` & `gardener-cicd-libs-1.2040.0/test/concourse/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/resources/github_test.py` & `gardener-cicd-libs-1.2040.0/test/concourse/resources/github_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/steps/__init__.py` & `gardener-cicd-libs-1.2040.0/test/concourse/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/steps/component_descriptor_test.py` & `gardener-cicd-libs-1.2040.0/test/concourse/steps/component_descriptor_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/steps/notification_test.py` & `gardener-cicd-libs-1.2040.0/test/concourse/steps/notification_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/steps/release_test.py` & `gardener-cicd-libs-1.2040.0/test/concourse/steps/release_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,22 +238,22 @@
             slack_channel='test_channel',
             githubrepobranch=GitHubRepoBranch(
                 github_config='test_config',
                 repo_owner='test_owner',
                 repo_name='test_name',
                 branch='master',
             ),
-            release_notes=ReleaseNotes(None),
+            release_notes_markdown="",
             release_version='1.0.0',
         ):
             return concourse.steps.release.PostSlackReleaseStep(
                 slack_cfg_name=slack_cfg_name,
                 slack_channel=slack_channel,
                 githubrepobranch=githubrepobranch,
-                release_notes=release_notes,
+                release_notes_markdown=release_notes_markdown,
                 release_version=release_version,
             )
         return _examinee
 
     def test_validation(self, examinee):
         examinee().validate()
```

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/steps/test_utils.py` & `gardener-cicd-libs-1.2040.0/test/concourse/steps/test_utils.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/steps/update_component_deps_test.py` & `gardener-cicd-libs-1.2040.0/test/concourse/steps/update_component_deps_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/steps/version_test.py` & `gardener-cicd-libs-1.2040.0/test/concourse/steps/version_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/concourse/util_test.py` & `gardener-cicd-libs-1.2040.0/test/concourse/util_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/container/__init__.py` & `gardener-cicd-libs-1.2040.0/test/container/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/github/__init__.py` & `gardener-cicd-libs-1.2040.0/test/github/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/github/github_util_test.py` & `gardener-cicd-libs-1.2040.0/test/github/github_util_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/github/release_notes/__init__.py` & `gardener-cicd-libs-1.2040.0/test/github/release_notes/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/github/release_notes/default_util.py` & `gardener-cicd-libs-1.2040.0/test/github/release_notes/default_util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/github/release_notes/renderer_test.py` & `gardener-cicd-libs-1.2040.0/test/github/release_notes/renderer_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/github/release_notes/util_test.py` & `gardener-cicd-libs-1.2040.0/test/github/release_notes/util_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/kubeutil_test.py` & `gardener-cicd-libs-1.2040.0/test/kubeutil_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/product_/__init__.py` & `gardener-cicd-libs-1.2040.0/test/product_/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/reutil_test.py` & `gardener-cicd-libs-1.2040.0/test/reutil_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/test/version_test.py` & `gardener-cicd-libs-1.2040.0/test/version_test.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/unixutil/model.py` & `gardener-cicd-libs-1.2040.0/unixutil/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/unixutil/scan.py` & `gardener-cicd-libs-1.2040.0/unixutil/scan.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-libs-1.2039.0/version.py` & `gardener-cicd-libs-1.2040.0/version.py`

 * *Files identical despite different names*

