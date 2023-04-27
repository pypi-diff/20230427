# Comparing `tmp/apache-airflow-providers-amazon-8.0.0rc2.tar.gz` & `tmp/apache-airflow-providers-amazon-8.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apache-airflow-providers-amazon-8.0.0rc2.tar", last modified: Mon Apr 24 21:39:43 2023, max compression
+gzip compressed data, was "dist/apache-airflow-providers-amazon-8.0.0rc3.tar", last modified: Wed Apr 26 09:36:03 2023, max compression
```

## Comparing `apache-airflow-providers-amazon-8.0.0rc2.tar` & `apache-airflow-providers-amazon-8.0.0rc3.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:43.000000 apache-airflow-providers-amazon-8.0.0rc2/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-8.0.0rc2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1219 2023-04-24 21:39:38.000000 apache-airflow-providers-amazon-8.0.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-8.0.0rc2/NOTICE
--rw-r--r--   0 root         (0) root         (0)    57034 2023-04-24 21:39:43.000000 apache-airflow-providers-amazon-8.0.0rc2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    55213 2023-04-24 21:39:38.000000 apache-airflow-providers-amazon-8.0.0rc2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:42.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4856 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/appflow.py
--rw-r--r--   0 root         (0) root         (0)    12240 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/athena.py
--rw-r--r--   0 root         (0) root         (0)    45421 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/base_aws.py
--rw-r--r--   0 root         (0) root         (0)    20629 2023-04-13 08:25:21.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/batch_client.py
--rw-r--r--   0 root         (0) root         (0)     2511 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/batch_waiters.json
--rw-r--r--   0 root         (0) root         (0)     9697 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/batch_waiters.py
--rw-r--r--   0 root         (0) root         (0)     3376 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    14133 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/datasync.py
--rw-r--r--   0 root         (0) root         (0)     7906 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/dms.py
--rw-r--r--   0 root         (0) root         (0)     2668 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     7641 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ec2.py
--rw-r--r--   0 root         (0) root         (0)     3702 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ecr.py
--rw-r--r--   0 root         (0) root         (0)     9194 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ecs.py
--rw-r--r--   0 root         (0) root         (0)    23957 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/eks.py
--rw-r--r--   0 root         (0) root         (0)    12114 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
--rw-r--r--   0 root         (0) root         (0)    20348 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/emr.py
--rw-r--r--   0 root         (0) root         (0)     3518 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/glacier.py
--rw-r--r--   0 root         (0) root         (0)    13816 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/glue.py
--rw-r--r--   0 root         (0) root         (0)     7611 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/glue_catalog.py
--rw-r--r--   0 root         (0) root         (0)     8895 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     1993 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/kinesis.py
--rw-r--r--   0 root         (0) root         (0)     8008 2023-02-24 18:53:47.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     4823 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/logs.py
--rw-r--r--   0 root         (0) root         (0)     7219 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    15272 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/rds.py
--rw-r--r--   0 root         (0) root         (0)    13108 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     7720 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)     5020 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/redshift_sql.py
--rw-r--r--   0 root         (0) root         (0)    42450 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/s3.py
--rw-r--r--   0 root         (0) root         (0)    56676 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2692 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     4143 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ses.py
--rw-r--r--   0 root         (0) root         (0)     3461 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/sns.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/sqs.py
--rw-r--r--   0 root         (0) root         (0)     2449 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ssm.py
--rw-r--r--   0 root         (0) root         (0)     3072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/step_function.py
--rw-r--r--   0 root         (0) root         (0)     1817 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/sts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:42.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/base_aws.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/batch.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/emr.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/glue.py
--rw-r--r--   0 root         (0) root         (0)     1607 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:42.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/log/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
--rw-r--r--   0 root         (0) root         (0)     9635 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/log/s3_task_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:42.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19677 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/appflow.py
--rw-r--r--   0 root         (0) root         (0)     6141 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/athena.py
--rw-r--r--   0 root         (0) root         (0)    15828 2023-04-13 08:25:21.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/batch.py
--rw-r--r--   0 root         (0) root         (0)     3633 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)    18419 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/datasync.py
--rw-r--r--   0 root         (0) root         (0)    10715 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/dms.py
--rw-r--r--   0 root         (0) root         (0)     9589 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/ec2.py
--rw-r--r--   0 root         (0) root         (0)    29018 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/ecs.py
--rw-r--r--   0 root         (0) root         (0)    31753 2023-04-14 11:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/eks.py
--rw-r--r--   0 root         (0) root         (0)    50180 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/emr.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/glacier.py
--rw-r--r--   0 root         (0) root         (0)     7471 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/glue.py
--rw-r--r--   0 root         (0) root         (0)     3306 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     7755 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/quicksight.py
--rw-r--r--   0 root         (0) root         (0)    29868 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/rds.py
--rw-r--r--   0 root         (0) root         (0)    28991 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)     5559 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/redshift_data.py
--rw-r--r--   0 root         (0) root         (0)    29966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/s3.py
--rw-r--r--   0 root         (0) root         (0)    49835 2023-03-01 07:06:45.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     2959 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/sns.py
--rw-r--r--   0 root         (0) root         (0)     3563 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/sqs.py
--rw-r--r--   0 root         (0) root         (0)     4469 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:42.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/secrets/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15533 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/secrets/secrets_manager.py
--rw-r--r--   0 root         (0) root         (0)     8503 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/secrets/systems_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:42.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/athena.py
--rw-r--r--   0 root         (0) root         (0)     7384 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/batch.py
--rw-r--r--   0 root         (0) root         (0)     4163 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/cloud_formation.py
--rw-r--r--   0 root         (0) root         (0)     3998 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/dms.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-04-19 10:00:26.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     2674 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/ec2.py
--rw-r--r--   0 root         (0) root         (0)     7203 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/ecs.py
--rw-r--r--   0 root         (0) root         (0)     9786 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/eks.py
--rw-r--r--   0 root         (0) root         (0)    18505 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/emr.py
--rw-r--r--   0 root         (0) root         (0)     4129 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/glacier.py
--rw-r--r--   0 root         (0) root         (0)     3428 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/glue.py
--rw-r--r--   0 root         (0) root         (0)     3732 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
--rw-r--r--   0 root         (0) root         (0)     2963 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/glue_crawler.py
--rw-r--r--   0 root         (0) root         (0)     3064 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/lambda_function.py
--rw-r--r--   0 root         (0) root         (0)     3641 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/quicksight.py
--rw-r--r--   0 root         (0) root         (0)     6447 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/rds.py
--rw-r--r--   0 root         (0) root         (0)     2637 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/redshift_cluster.py
--rw-r--r--   0 root         (0) root         (0)    11650 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/s3.py
--rw-r--r--   0 root         (0) root         (0)    13057 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     9584 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/sqs.py
--rw-r--r--   0 root         (0) root         (0)     3400 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/step_function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:43.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2768 2023-03-15 08:58:48.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/base.py
--rw-r--r--   0 root         (0) root         (0)     5843 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     6435 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     7676 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4701 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
--rw-r--r--   0 root         (0) root         (0)     9042 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4172 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
--rw-r--r--   0 root         (0) root         (0)     4248 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/local_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     5863 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8108 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
--rw-r--r--   0 root         (0) root         (0)     8268 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
--rw-r--r--   0 root         (0) root         (0)     4620 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/s3_to_sql.py
--rw-r--r--   0 root         (0) root         (0)     5679 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     3679 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
--rw-r--r--   0 root         (0) root         (0)     8475 2023-04-19 10:00:26.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/sql_to_s3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:43.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-03-14 06:24:40.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5579 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/triggers/redshift_cluster.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:43.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/
--rw-r--r--   0 root         (0) root         (0)     2215 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20348 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/connection_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     2561 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/eks_get_token.py
--rw-r--r--   0 root         (0) root         (0)     1853 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/emailer.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/rds.py
--rw-r--r--   0 root         (0) root         (0)     1913 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/redshift.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/sagemaker.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     3583 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/waiter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:43.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/
--rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/appflow.json
--rw-r--r--   0 root         (0) root         (0)     1853 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/base_waiter.py
--rw-r--r--   0 root         (0) root         (0)     2720 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/ecs.json
--rw-r--r--   0 root         (0) root         (0)      659 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/eks.json
--rw-r--r--   0 root         (0) root         (0)      430 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/emr-serverless.json
--rw-r--r--   0 root         (0) root         (0)     2559 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/emr.json
--rw-r--r--   0 root         (0) root         (0)    36867 2023-04-24 21:39:38.000000 apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 21:39:43.000000 apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/
--rw-r--r--   0 root         (0) root         (0)    57034 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7264 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      803 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-24 21:39:41.000000 apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-amazon-8.0.0rc2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     2110 2023-04-24 21:39:43.000000 apache-airflow-providers-amazon-8.0.0rc2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2356 2023-04-24 21:39:37.000000 apache-airflow-providers-amazon-8.0.0rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:03.000000 apache-airflow-providers-amazon-8.0.0rc3/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-8.0.0rc3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-04-26 09:35:58.000000 apache-airflow-providers-amazon-8.0.0rc3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-02-24 18:43:54.000000 apache-airflow-providers-amazon-8.0.0rc3/NOTICE
+-rw-r--r--   0 root         (0) root         (0)    57184 2023-04-26 09:36:03.000000 apache-airflow-providers-amazon-8.0.0rc3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    55363 2023-04-26 09:35:58.000000 apache-airflow-providers-amazon-8.0.0rc3/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:02.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4856 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/appflow.py
+-rw-r--r--   0 root         (0) root         (0)    12240 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/athena.py
+-rw-r--r--   0 root         (0) root         (0)    45461 2023-04-26 05:04:56.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)    20629 2023-04-13 08:25:21.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)     2511 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/batch_waiters.json
+-rw-r--r--   0 root         (0) root         (0)     9697 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/batch_waiters.py
+-rw-r--r--   0 root         (0) root         (0)     3376 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    14133 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/datasync.py
+-rw-r--r--   0 root         (0) root         (0)     7906 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/dms.py
+-rw-r--r--   0 root         (0) root         (0)     2668 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     7641 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     3702 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ecr.py
+-rw-r--r--   0 root         (0) root         (0)     9194 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    23957 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/eks.py
+-rw-r--r--   0 root         (0) root         (0)    12114 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py
+-rw-r--r--   0 root         (0) root         (0)    20348 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3518 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/glacier.py
+-rw-r--r--   0 root         (0) root         (0)    13816 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/glue.py
+-rw-r--r--   0 root         (0) root         (0)     7611 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/glue_catalog.py
+-rw-r--r--   0 root         (0) root         (0)     8895 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     1993 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/kinesis.py
+-rw-r--r--   0 root         (0) root         (0)     8008 2023-02-24 18:53:47.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     4823 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/logs.py
+-rw-r--r--   0 root         (0) root         (0)     7219 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    15272 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/rds.py
+-rw-r--r--   0 root         (0) root         (0)    13108 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     7720 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)     5020 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/redshift_sql.py
+-rw-r--r--   0 root         (0) root         (0)    42450 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/s3.py
+-rw-r--r--   0 root         (0) root         (0)    56676 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2692 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4143 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ses.py
+-rw-r--r--   0 root         (0) root         (0)     3461 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     2449 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ssm.py
+-rw-r--r--   0 root         (0) root         (0)     3072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/step_function.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/sts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:02.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2940 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/base_aws.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/batch.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/emr.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/glue.py
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:02.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/log/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5072 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py
+-rw-r--r--   0 root         (0) root         (0)     9635 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/log/s3_task_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:02.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19677 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/appflow.py
+-rw-r--r--   0 root         (0) root         (0)     6141 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/athena.py
+-rw-r--r--   0 root         (0) root         (0)    15828 2023-04-13 08:25:21.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/batch.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)    18419 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/datasync.py
+-rw-r--r--   0 root         (0) root         (0)    10715 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/dms.py
+-rw-r--r--   0 root         (0) root         (0)     9589 2023-03-10 19:31:58.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/ec2.py
+-rw-r--r--   0 root         (0) root         (0)    29018 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/ecs.py
+-rw-r--r--   0 root         (0) root         (0)    31753 2023-04-14 11:39:41.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/eks.py
+-rw-r--r--   0 root         (0) root         (0)    50180 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/emr.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     7471 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/glue.py
+-rw-r--r--   0 root         (0) root         (0)     3306 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)    29868 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/rds.py
+-rw-r--r--   0 root         (0) root         (0)    28991 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     5559 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/redshift_data.py
+-rw-r--r--   0 root         (0) root         (0)    29966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/s3.py
+-rw-r--r--   0 root         (0) root         (0)    49835 2023-03-01 07:06:45.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/sns.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     4469 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:02.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/secrets/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15533 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/secrets/secrets_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8503 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/secrets/systems_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:02.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/athena.py
+-rw-r--r--   0 root         (0) root         (0)     7384 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/batch.py
+-rw-r--r--   0 root         (0) root         (0)     4163 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/cloud_formation.py
+-rw-r--r--   0 root         (0) root         (0)     3998 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/dms.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-04-19 10:00:26.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     2674 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/ec2.py
+-rw-r--r--   0 root         (0) root         (0)     7203 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     9786 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/eks.py
+-rw-r--r--   0 root         (0) root         (0)    18505 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/emr.py
+-rw-r--r--   0 root         (0) root         (0)     4129 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/glacier.py
+-rw-r--r--   0 root         (0) root         (0)     3428 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/glue.py
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/glue_crawler.py
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/lambda_function.py
+-rw-r--r--   0 root         (0) root         (0)     3641 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/quicksight.py
+-rw-r--r--   0 root         (0) root         (0)     6447 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/rds.py
+-rw-r--r--   0 root         (0) root         (0)     2637 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/redshift_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    11650 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/s3.py
+-rw-r--r--   0 root         (0) root         (0)    13057 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     9584 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/sqs.py
+-rw-r--r--   0 root         (0) root         (0)     3400 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/step_function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:02.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2768 2023-03-15 08:58:48.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/base.py
+-rw-r--r--   0 root         (0) root         (0)     5843 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/exasol_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     6435 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/ftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     7676 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/gcs_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4701 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py
+-rw-r--r--   0 root         (0) root         (0)     9042 2023-04-21 10:05:41.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/google_api_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4172 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/local_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     5863 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/mongo_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8108 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/redshift_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/s3_to_ftp.py
+-rw-r--r--   0 root         (0) root         (0)     8268 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/s3_to_redshift.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-04-21 18:38:06.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/s3_to_sftp.py
+-rw-r--r--   0 root         (0) root         (0)     4620 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/s3_to_sql.py
+-rw-r--r--   0 root         (0) root         (0)     5679 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     3679 2023-04-07 12:28:57.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/sftp_to_s3.py
+-rw-r--r--   0 root         (0) root         (0)     8475 2023-04-19 10:00:26.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/sql_to_s3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:02.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-03-14 06:24:40.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/triggers/redshift_cluster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:03.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/
+-rw-r--r--   0 root         (0) root         (0)     2215 2023-03-06 20:52:28.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20348 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/connection_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     2561 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/eks_get_token.py
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/emailer.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/rds.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/redshift.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/sagemaker.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     3583 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/waiter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:03.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-03-27 08:32:48.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/appflow.json
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/base_waiter.py
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-03-02 08:17:44.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/ecs.json
+-rw-r--r--   0 root         (0) root         (0)      659 2023-02-24 18:43:53.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/eks.json
+-rw-r--r--   0 root         (0) root         (0)      430 2023-04-24 21:04:25.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/emr-serverless.json
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-03-05 08:19:18.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/emr.json
+-rw-r--r--   0 root         (0) root         (0)    36833 2023-04-26 09:35:58.000000 apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 09:36:03.000000 apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    57184 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7264 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      784 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-26 09:36:01.000000 apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5246 2023-04-07 12:28:58.000000 apache-airflow-providers-amazon-8.0.0rc3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-04-26 09:36:03.000000 apache-airflow-providers-amazon-8.0.0rc3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2363 2023-04-26 09:35:57.000000 apache-airflow-providers-amazon-8.0.0rc3/setup.py
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/LICENSE` & `apache-airflow-providers-amazon-8.0.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/MANIFEST.in` & `apache-airflow-providers-amazon-8.0.0rc3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/PKG-INFO` & `apache-airflow-providers-amazon-8.0.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-amazon
-Version: 8.0.0rc2
+Version: 8.0.0rc3
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.0.0/
@@ -60,15 +60,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.0.0rc2``
+Release: ``8.0.0rc3``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
@@ -102,15 +102,14 @@
 ``watchtower``                           ``~=2.0.1``
 ``jsonpath_ng``                          ``>=1.5.3``
 ``redshift_connector``                   ``>=2.0.888``
 ``sqlalchemy_redshift``                  ``>=0.8.6``
 ``mypy-boto3-rds``                       ``>=1.24.0``
 ``mypy-boto3-redshift-data``             ``>=1.24.0``
 ``mypy-boto3-appflow``                   ``>=1.24.0``
-``aiobotocore[boto3]``                   ``>=2.2.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
@@ -217,30 +216,33 @@
 ~~~~~~~~~
 
 * ``Fixed logging issue (#30703)``
 * ``DynamoDBHook - waiter_path() to consider 'resource_type' or 'client_type' (#30595)``
 * ``Add ability to override waiter delay in EcsRunTaskOperator (#30586)``
 * ``Add support in AWS Batch Operator for multinode jobs (#29522)``
 * ``AWS logs. Exit fast when 3 consecutive responses are returned from AWS Cloudwatch logs (#30756)``
+* ``Fix async conn for none aws_session_token (#30868)``
 
 Misc
 ~~~~
 
 * ``Remove @poke_mode_only from EmrStepSensor (#30774)``
 * ``Organize Amazon providers docs index (#30541)``
 * ``Remove duplicate param docstring in EksPodOperator (#30634)``
 * ``Update AWS EMR Cluster Link to use the new dashboard (#30844)``
+* ``Restore aiobotocore as optional dependency of amazon provider (#30874)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Decouple "job runner" from BaseJob ORM model (#30255)``
    * ``Upgrade ruff to 0.0.262 (#30809)``
    * ``fixes to system tests following obsolete cleanup (#30804)``
    * ``restore fallback to empty connection behavior (#30806)``
    * ``Prepare docs for adhoc release of providers (#30787)``
+   * ``Prepare docs for ad-hoc release of Amazon provider (#30848)``
 
 7.4.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/README.rst` & `apache-airflow-providers-amazon-8.0.0rc3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.0.0rc2``
+Release: ``8.0.0rc3``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
@@ -57,15 +57,14 @@
 ``watchtower``                           ``~=2.0.1``
 ``jsonpath_ng``                          ``>=1.5.3``
 ``redshift_connector``                   ``>=2.0.888``
 ``sqlalchemy_redshift``                  ``>=0.8.6``
 ``mypy-boto3-rds``                       ``>=1.24.0``
 ``mypy-boto3-redshift-data``             ``>=1.24.0``
 ``mypy-boto3-appflow``                   ``>=1.24.0``
-``aiobotocore[boto3]``                   ``>=2.2.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
@@ -172,30 +171,33 @@
 ~~~~~~~~~
 
 * ``Fixed logging issue (#30703)``
 * ``DynamoDBHook - waiter_path() to consider 'resource_type' or 'client_type' (#30595)``
 * ``Add ability to override waiter delay in EcsRunTaskOperator (#30586)``
 * ``Add support in AWS Batch Operator for multinode jobs (#29522)``
 * ``AWS logs. Exit fast when 3 consecutive responses are returned from AWS Cloudwatch logs (#30756)``
+* ``Fix async conn for none aws_session_token (#30868)``
 
 Misc
 ~~~~
 
 * ``Remove @poke_mode_only from EmrStepSensor (#30774)``
 * ``Organize Amazon providers docs index (#30541)``
 * ``Remove duplicate param docstring in EksPodOperator (#30634)``
 * ``Update AWS EMR Cluster Link to use the new dashboard (#30844)``
+* ``Restore aiobotocore as optional dependency of amazon provider (#30874)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Decouple "job runner" from BaseJob ORM model (#30255)``
    * ``Upgrade ruff to 0.0.262 (#30809)``
    * ``fixes to system tests following obsolete cleanup (#30804)``
    * ``restore fallback to empty connection behavior (#30806)``
    * ``Prepare docs for adhoc release of providers (#30787)``
+   * ``Prepare docs for ad-hoc release of Amazon provider (#30848)``
 
 7.4.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/exceptions.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/appflow.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/athena.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/base_aws.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/base_aws.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,17 +134,17 @@
 
         if (
             self.conn.session_kwargs.get("aws_access_key_id", None)
             or self.conn.session_kwargs.get("aws_secret_access_key", None)
             or self.conn.session_kwargs.get("aws_session_token", None)
         ):
             session.set_credentials(
-                self.conn.session_kwargs["aws_access_key_id"],
-                self.conn.session_kwargs["aws_secret_access_key"],
-                self.conn.session_kwargs["aws_session_token"],
+                access_key=self.conn.session_kwargs.get("aws_access_key_id"),
+                secret_key=self.conn.session_kwargs.get("aws_secret_access_key"),
+                token=self.conn.session_kwargs.get("aws_session_token"),
             )
 
         if self.conn.session_kwargs.get("region_name", None) is not None:
             session.set_config_variable("region", self.conn.session_kwargs["region_name"])
 
     def get_async_session(self):
         from aiobotocore.session import get_session as async_get_session
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/batch_client.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/batch_client.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/batch_waiters.json` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/batch_waiters.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/batch_waiters.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/batch_waiters.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/cloud_formation.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/datasync.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/dms.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/dynamodb.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ec2.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ecr.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ecr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ecs.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/eks.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/elasticache_replication_group.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/emr.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/glacier.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/glue.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/glue_catalog.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/glue_catalog.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/glue_crawler.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/kinesis.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/kinesis.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/lambda_function.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/logs.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/quicksight.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/rds.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/redshift_cluster.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/redshift_data.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/redshift_sql.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/redshift_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/s3.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/sagemaker.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/secrets_manager.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ses.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ses.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/sns.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/sqs.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/ssm.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/ssm.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/step_function.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/hooks/sts.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/hooks/sts.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/base_aws.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/base_aws.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/batch.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/emr.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/glue.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/links/logs.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/links/logs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/log/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/log/cloudwatch_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/log/s3_task_handler.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/log/s3_task_handler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/appflow.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/appflow.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/athena.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/batch.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/cloud_formation.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/datasync.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/datasync.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/dms.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/ec2.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/ecs.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/eks.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/emr.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/glacier.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/glue.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/glue_crawler.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/lambda_function.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/quicksight.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/rds.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/redshift_cluster.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/redshift_data.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/redshift_data.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/s3.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/sagemaker.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/sns.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/sns.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/sqs.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/operators/step_function.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/operators/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/secrets/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/secrets/secrets_manager.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/secrets/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/secrets/systems_manager.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/secrets/systems_manager.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/athena.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/athena.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/batch.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/batch.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/cloud_formation.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/cloud_formation.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/dms.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/dms.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/dynamodb.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/ec2.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/ec2.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/ecs.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/ecs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/eks.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/eks.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/emr.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/emr.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/glacier.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/glacier.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/glue.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/glue.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/glue_catalog_partition.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/glue_crawler.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/lambda_function.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/lambda_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/quicksight.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/quicksight.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/rds.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/redshift_cluster.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/s3.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/sagemaker.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/sqs.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/sqs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/sensors/step_function.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/sensors/step_function.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/base.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/base.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/dynamodb_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/exasol_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/exasol_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/ftp_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/ftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/gcs_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/gcs_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/glacier_to_gcs.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/google_api_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/google_api_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/hive_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/imap_attachment_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/local_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/local_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/mongo_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/mongo_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/redshift_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/redshift_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/s3_to_ftp.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/s3_to_ftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/s3_to_redshift.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/s3_to_redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/s3_to_sftp.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/s3_to_sftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/s3_to_sql.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/s3_to_sql.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/salesforce_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/sftp_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/sftp_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/transfers/sql_to_s3.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/transfers/sql_to_s3.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/triggers/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/triggers/redshift_cluster.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/triggers/redshift_cluster.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/connection_wrapper.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/connection_wrapper.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/eks_get_token.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/eks_get_token.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/emailer.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/emailer.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/rds.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/rds.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/redshift.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/redshift.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/sagemaker.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/sagemaker.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/tags.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/tags.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/utils/waiter.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/utils/waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/__init__.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/appflow.json` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/appflow.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/base_waiter.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/base_waiter.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/ecs.json` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/ecs.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/eks.json` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/eks.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/aws/waiters/emr.json` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/aws/waiters/emr.json`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/airflow/providers/amazon/get_provider_info.py` & `apache-airflow-providers-amazon-8.0.0rc3/airflow/providers/amazon/get_provider_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,14 @@
             "watchtower~=2.0.1",
             "jsonpath_ng>=1.5.3",
             "redshift_connector>=2.0.888",
             "sqlalchemy_redshift>=0.8.6",
             "mypy-boto3-rds>=1.24.0",
             "mypy-boto3-redshift-data>=1.24.0",
             "mypy-boto3-appflow>=1.24.0",
-            "aiobotocore[boto3]>=2.2.0",
         ],
         "integrations": [
             {
                 "integration-name": "Amazon Athena",
                 "external-doc-url": "https://aws.amazon.com/athena/",
                 "logo": "/integration-logos/aws/Amazon-Athena_light-bg@4x.png",
                 "how-to-guide": ["/docs/apache-airflow-providers-amazon/operators/athena.rst"],
@@ -768,10 +767,10 @@
         ],
         "logging": [
             "airflow.providers.amazon.aws.log.s3_task_handler.S3TaskHandler",
             "airflow.providers.amazon.aws.log.cloudwatch_task_handler.CloudwatchTaskHandler",
         ],
         "additional-extras": [
             {"name": "pandas", "dependencies": ["pandas>=0.17.1"]},
-            {"name": "aiobotocore", "dependencies": ["aiobotocore>=2.1.1"]},
+            {"name": "aiobotocore", "dependencies": ["aiobotocore[boto3]>=2.2.0"]},
         ],
     }
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/PKG-INFO` & `apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-amazon
-Version: 8.0.0rc2
+Version: 8.0.0rc3
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-amazon package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-amazon/8.0.0/
@@ -60,15 +60,15 @@
    KIND, either express or implied.  See the License for the
    specific language governing permissions and limitations
    under the License.
 
 
 Package ``apache-airflow-providers-amazon``
 
-Release: ``8.0.0rc2``
+Release: ``8.0.0rc3``
 
 
 Amazon integration (including `Amazon Web Services (AWS) <https://aws.amazon.com/>`__).
 
 
 Provider package
 ----------------
@@ -102,15 +102,14 @@
 ``watchtower``                           ``~=2.0.1``
 ``jsonpath_ng``                          ``>=1.5.3``
 ``redshift_connector``                   ``>=2.0.888``
 ``sqlalchemy_redshift``                  ``>=0.8.6``
 ``mypy-boto3-rds``                       ``>=1.24.0``
 ``mypy-boto3-redshift-data``             ``>=1.24.0``
 ``mypy-boto3-appflow``                   ``>=1.24.0``
-``aiobotocore[boto3]``                   ``>=2.2.0``
 =======================================  ==================
 
 Cross provider package dependencies
 -----------------------------------
 
 Those are dependencies that might be needed in order to use all the features of the package.
 You need to install the specified provider packages in order to use them.
@@ -217,30 +216,33 @@
 ~~~~~~~~~
 
 * ``Fixed logging issue (#30703)``
 * ``DynamoDBHook - waiter_path() to consider 'resource_type' or 'client_type' (#30595)``
 * ``Add ability to override waiter delay in EcsRunTaskOperator (#30586)``
 * ``Add support in AWS Batch Operator for multinode jobs (#29522)``
 * ``AWS logs. Exit fast when 3 consecutive responses are returned from AWS Cloudwatch logs (#30756)``
+* ``Fix async conn for none aws_session_token (#30868)``
 
 Misc
 ~~~~
 
 * ``Remove @poke_mode_only from EmrStepSensor (#30774)``
 * ``Organize Amazon providers docs index (#30541)``
 * ``Remove duplicate param docstring in EksPodOperator (#30634)``
 * ``Update AWS EMR Cluster Link to use the new dashboard (#30844)``
+* ``Restore aiobotocore as optional dependency of amazon provider (#30874)``
 
 .. Below changes are excluded from the changelog. Move them to
    appropriate section above if needed. Do not delete the lines(!):
    * ``Decouple "job runner" from BaseJob ORM model (#30255)``
    * ``Upgrade ruff to 0.0.262 (#30809)``
    * ``fixes to system tests following obsolete cleanup (#30804)``
    * ``restore fallback to empty connection behavior (#30806)``
    * ``Prepare docs for adhoc release of providers (#30787)``
+   * ``Prepare docs for ad-hoc release of Amazon provider (#30848)``
 
 7.4.1
 .....
 
 Bug Fixes
 ~~~~~~~~~
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/SOURCES.txt` & `apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/apache_airflow_providers_amazon.egg-info/requires.txt` & `apache-airflow-providers-amazon-8.0.0rc3/apache_airflow_providers_amazon.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-aiobotocore[boto3]>=2.2.0
 apache-airflow-providers-common-sql>=1.3.1.dev0
 apache-airflow>=2.3.0.dev0
 asgiref
 boto3>=1.24.0
 jsonpath_ng>=1.5.3
 mypy-boto3-appflow>=1.24.0
 mypy-boto3-rds>=1.24.0
 mypy-boto3-redshift-data>=1.24.0
 redshift_connector>=2.0.888
 sqlalchemy_redshift>=0.8.6
 watchtower~=2.0.1
 
 [aiobotocore]
-aiobotocore>=2.1.1
+aiobotocore[boto3]>=2.2.0
 
 [apache.hive]
 apache-airflow-providers-apache-hive
 
 [cncf.kubernetes]
 apache-airflow-providers-cncf-kubernetes
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/pyproject.toml` & `apache-airflow-providers-amazon-8.0.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/setup.cfg` & `apache-airflow-providers-amazon-8.0.0rc3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 include_package_data = True
 python_requires = ~=3.7
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	aiobotocore[boto3]>=2.2.0
 	apache-airflow-providers-common-sql>=1.3.1.dev0
 	apache-airflow>=2.3.0.dev0
 	asgiref
 	boto3>=1.24.0
 	jsonpath_ng>=1.5.3
 	mypy-boto3-appflow>=1.24.0
 	mypy-boto3-rds>=1.24.0
@@ -63,10 +62,10 @@
 apache_airflow_provider = 
 	provider_info=airflow.providers.amazon.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.amazon
 
 [egg_info]
-tag_build = rc2
+tag_build = rc3
 tag_date = 0
```

### Comparing `apache-airflow-providers-amazon-8.0.0rc2/setup.py` & `apache-airflow-providers-amazon-8.0.0rc3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             "ftp": ["apache-airflow-providers-ftp"],
             "google": ["apache-airflow-providers-google"],
             "imap": ["apache-airflow-providers-imap"],
             "mongo": ["apache-airflow-providers-mongo"],
             "salesforce": ["apache-airflow-providers-salesforce"],
             "ssh": ["apache-airflow-providers-ssh"],
             "pandas": ["pandas>=0.17.1"],
-            "aiobotocore": ["aiobotocore>=2.1.1"],
+            "aiobotocore": ["aiobotocore[boto3]>=2.2.0"],
         },
         packages=find_namespace_packages(
             include=[
                 "airflow.providers.amazon",
                 "airflow.providers.amazon.*",
                 "airflow.providers.amazon_vendor",
                 "airflow.providers.amazon_vendor.*",
```

