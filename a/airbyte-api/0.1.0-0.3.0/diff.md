# Comparing `tmp/airbyte-api-0.1.0.tar.gz` & `tmp/airbyte-api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-api-0.1.0.tar", last modified: Mon Apr 24 22:27:32 2023, max compression
+gzip compressed data, was "airbyte-api-0.3.0.tar", last modified: Thu Apr 27 19:10:11 2023, max compression
```

## Comparing `airbyte-api-0.1.0.tar` & `airbyte-api-0.3.0.tar`

### file list

```diff
@@ -1,311 +1,311 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:27:32.374912 airbyte-api-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-04-24 22:27:32.374912 airbyte-api-0.1.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6413 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 22:27:32.374912 airbyte-api-0.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1095 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:27:32.342911 airbyte-api-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:27:32.346911 airbyte-api-0.1.0/src/airbyte/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5278 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5349 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/destinations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5390 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:27:32.346911 airbyte-api-0.1.0/src/airbyte/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:27:32.346911 airbyte-api-0.1.0/src/airbyte/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1697 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/canceljob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      652 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/createconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      658 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/createdestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      690 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/createjob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      979 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/createorupdateworkspaceoauthcredentials.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/createsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/createworkspace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      641 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/deleteconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      645 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/deletedestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      625 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/deletesource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/getconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      881 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/getdestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/getjob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      831 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/getsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1093 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/getstreamproperties.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/getworkspace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      432 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/initiateoauth.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1707 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/listconnections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1718 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/listdestinations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1617 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/listjobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1663 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/listsources.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1682 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/operations/listworkspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:27:32.370912 airbyte-api-0.1.0/src/airbyte/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)    49472 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3230 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/connectioncreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1857 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/connectionresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/connectionschedulecreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/connectionscheduleresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      961 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/connectionsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      255 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/connectionstatusenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      391 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/connectionsyncmodeenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3478 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_amazon_sqs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9302 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_aws_datalake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4632 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_azure_blob_storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12180 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_bigquery.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10929 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_bigquery_denormalized.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1996 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_cassandra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6174 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_clickhouse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1026 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_convex.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1812 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_databend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8062 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_databricks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2764 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_dynamodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3515 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_elasticsearch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3777 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_firebolt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1343 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_firestore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21101 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_gcs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2056 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_google_sheets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_keen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1855 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_kinesis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6322 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_mariadb_columnstore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1210 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_meilisearch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9235 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_mongodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8155 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_mssql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6089 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_mysql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6790 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_oracle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11178 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_postgres.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2760 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_pubsub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5831 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_pulsar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2251 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_rabbitmq.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8064 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_redis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14025 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_redshift.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1235 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_rockset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18946 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_s3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8961 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_s3_glue.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1731 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_scylla.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1597 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_sftp_json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16133 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_snowflake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1778 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destination_typesense.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destinationcreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      891 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destinationresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      826 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/destinationsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      216 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/geographyenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1391 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/initiateoauthrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      836 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/jobcreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1957 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/jobresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/jobsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/jobstatusenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      289 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/jobtypeenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      213 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/scheduletypeenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/scheduletypewithbasicenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3391 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_airtable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7535 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_alloydb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4960 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_amazon_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5171 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_amazon_seller_partner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3935 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_amazon_sqs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2390 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_amplitude.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_apify_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2795 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_asana.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3326 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_auth0.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2029 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_aws_cloudtrail.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3061 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_azure_blob_storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1587 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_azure_table.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1631 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_bamboo_hr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1287 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_bigcommerce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1585 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_bigquery.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2755 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_bing_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2519 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_braintree.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1245 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_braze.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2240 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_chargebee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2021 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_chartmogul.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5739 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_clickhouse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2909 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_clickup_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_close_com.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      738 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_coda.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2584 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_coin_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2060 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_coinmarketcap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1100 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_configcat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_confluence.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_datascope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1169 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_delighted.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1210 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_dixa.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_dockerhub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      958 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_dremio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2754 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_dynamodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4302 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_e2e_test_cloud.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      949 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_emailoctopus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1974 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_exchange_rates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17598 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_facebook_marketing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_facebook_pages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2141 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_faker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4626 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_fauna.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10324 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_file_secure.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1796 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_firebolt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_freshcaller.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1970 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_freshdesk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1109 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_freshsales.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1215 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_gcs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      821 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_getlago.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4341 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_github.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4152 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_gitlab.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      784 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_glassfrog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9633 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_gnews.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5986 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_google_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5213 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_google_analytics_data_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4971 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_google_analytics_v4.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1231 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_google_directory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5235 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_google_search_console.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3280 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_google_sheets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1597 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_google_webfonts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1624 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_google_workspace_admin_reports.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      919 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_greenhouse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_gridly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_harvest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_hubplanner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3668 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_hubspot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_insightly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1588 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_instagram.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      769 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_instatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_intercom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1181 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_ip2whois.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1404 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_iterable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3240 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_jira.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_k6_cloud.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1924 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_klarna.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1332 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_klaviyo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1134 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_kustomer_singer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_launchdarkly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      757 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_lemlist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3583 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_linkedin_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3010 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_linkedin_pages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1550 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_linnworks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1112 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_lokalise.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2746 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_mailchimp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_mailgun.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1473 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_mailjet_sms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1973 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_marketo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1829 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_metabase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4251 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_microsoft_teams.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6254 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_mixpanel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2588 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_monday.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4422 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_mongodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12234 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_mssql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_my_hours.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12863 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_mysql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2487 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_netsuite.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_notion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2251 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_nytimes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3007 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_okta.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      755 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_omnisend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2695 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_onesignal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3403 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_openweather.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10232 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_oracle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2764 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_orb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1327 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_orbit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1813 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_outreach.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1989 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_paypal_transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1749 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_paystack.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      715 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_pendo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_persistiq.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2551 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_pexels_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3240 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_pinterest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1959 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_pipedrive.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3920 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_pocket.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      782 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_pokeapi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2981 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_polygon_stock_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7554 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_postgres.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1624 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_posthog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_postmarkapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1468 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_prestashop.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      630 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_public_apis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_punk_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_pypi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1814 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_qualaroo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3543 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_quickbooks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1065 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_railz.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_recharge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_recreation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1160 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_recruitee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1500 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_recurly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2267 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_redshift.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      883 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_retently.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      840 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_rki_covid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      717 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_rss.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13850 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_s3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3785 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_salesforce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3520 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_salesforce_singer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3552 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_salesloft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_sap_fieldglass.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_secoda.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1368 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_sendgrid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_sendinblue.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3353 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_senseforce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1964 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_sentry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3653 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_sftp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3477 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_sftp_bulk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3217 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_shopify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1135 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_shortio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4288 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_slack.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1255 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_smaily.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      776 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_smartengage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4183 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_smartsheets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2135 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_snapchat_marketing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4413 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_snowflake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2206 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_sonar_cloud.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      997 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_spacex_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3714 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_square.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2103 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_strava.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2529 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_stripe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2702 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_survey_sparrow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3738 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_surveymonkey.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_tempo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2981 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_the_guardian_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4470 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_tiktok_marketing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_todoist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2023 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_trello.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3853 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_trustpilot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1797 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_tvmaze_schedule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1662 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_twilio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      988 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_twilio_taskrouter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2178 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_twitter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1789 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_typeform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1315 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_us_census.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_vantage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1084 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_webflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_whisky_hunter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2403 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_wikipedia_pageviews.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1581 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_woocommerce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2469 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_xero.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_xkcd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_yandex_metrica.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1447 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_younium.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      836 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_youtube_analytics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3567 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_zendesk_chat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3150 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_zendesk_sunshine.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2067 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_zendesk_support.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1787 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_zendesk_talk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1889 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_zenloop.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3102 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_zoho_crm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      733 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_zoom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1706 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/source_zuora.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/sourcecreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/sourceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/sourcesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1598 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/streamconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      709 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/streamconfigurations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1778 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/streamproperties.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      469 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/workspacecreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/workspaceoauthcredentialsrequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      857 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/workspaceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      816 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/models/shared/workspacesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3591 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6839 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/sources.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1982 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:27:32.370912 airbyte-api-0.1.0/src/airbyte/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6106 2023-04-24 22:27:21.000000 airbyte-api-0.1.0/src/airbyte/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 22:27:32.374912 airbyte-api-0.1.0/src/airbyte_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-04-24 22:27:32.000000 airbyte-api-0.1.0/src/airbyte_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-04-24 22:27:32.000000 airbyte-api-0.1.0/src/airbyte_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 22:27:32.000000 airbyte-api-0.1.0/src/airbyte_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-24 22:27:32.000000 airbyte-api-0.1.0/src/airbyte_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 22:27:32.000000 airbyte-api-0.1.0/src/airbyte_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:10:11.896006 airbyte-api-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-27 19:10:11.896006 airbyte-api-0.3.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7285 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 19:10:11.896006 airbyte-api-0.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1094 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:10:11.868006 airbyte-api-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:10:11.868006 airbyte-api-0.3.0/src/airbyte/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5278 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5349 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/destinations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5390 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:10:11.868006 airbyte-api-0.3.0/src/airbyte/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:10:11.872006 airbyte-api-0.3.0/src/airbyte/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1697 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/canceljob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      652 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/createconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      658 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/createdestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      690 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/createjob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      979 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/createorupdateworkspaceoauthcredentials.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/createsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/createworkspace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      641 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/deleteconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      645 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/deletedestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      625 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/deletesource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/getconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      881 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/getdestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/getjob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      831 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/getsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1093 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/getstreamproperties.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/getworkspace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      432 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/initiateoauth.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1707 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/listconnections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1718 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/listdestinations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1617 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/listjobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1663 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/listsources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1682 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/operations/listworkspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:10:11.896006 airbyte-api-0.3.0/src/airbyte/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49472 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3230 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/connectioncreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1857 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/connectionresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/connectionschedulecreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1104 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/connectionscheduleresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      961 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/connectionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      255 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/connectionstatusenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      391 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/connectionsyncmodeenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3478 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_amazon_sqs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9302 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_aws_datalake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4632 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_azure_blob_storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12180 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_bigquery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10929 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_bigquery_denormalized.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1996 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_cassandra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6174 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_clickhouse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1026 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_convex.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1812 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_databend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8062 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_databricks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2764 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_dynamodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3515 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_elasticsearch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3777 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_firebolt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1343 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_firestore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21101 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_gcs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2056 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_google_sheets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_keen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1855 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_kinesis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6322 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_mariadb_columnstore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1210 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_meilisearch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9235 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_mongodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8155 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_mssql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6089 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_mysql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6790 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_oracle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11178 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_postgres.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2760 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_pubsub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5831 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_pulsar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2251 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_rabbitmq.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8064 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_redis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14025 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_redshift.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1235 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_rockset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18946 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_s3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8961 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_s3_glue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1731 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_scylla.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1597 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_sftp_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16133 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_snowflake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1778 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destination_typesense.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      787 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destinationcreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      891 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destinationresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      826 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/destinationsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      216 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/geographyenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1391 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/initiateoauthrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      836 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/jobcreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1957 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/jobresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/jobsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/jobstatusenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      289 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/jobtypeenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      213 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/scheduletypeenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/scheduletypewithbasicenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3391 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_airtable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7535 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_alloydb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4960 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_amazon_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5171 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_amazon_seller_partner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3935 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_amazon_sqs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2390 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_amplitude.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_apify_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2795 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_asana.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3326 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_auth0.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2029 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_aws_cloudtrail.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3061 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_azure_blob_storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1587 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_azure_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1631 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_bamboo_hr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1287 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_bigcommerce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1585 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_bigquery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2755 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_bing_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2519 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_braintree.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1245 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_braze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2240 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_chargebee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2021 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_chartmogul.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5739 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_clickhouse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2909 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_clickup_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_close_com.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      738 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_coda.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2584 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_coin_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2060 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_coinmarketcap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1100 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_configcat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1296 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_confluence.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_datascope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1169 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_delighted.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1210 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_dixa.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_dockerhub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      958 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_dremio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2754 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_dynamodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4302 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_e2e_test_cloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      949 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_emailoctopus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1974 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_exchange_rates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17598 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_facebook_marketing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      962 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_facebook_pages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2141 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_faker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4626 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_fauna.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10324 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_file_secure.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1796 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_firebolt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_freshcaller.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1970 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_freshdesk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1109 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_freshsales.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1215 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_gcs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      821 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_getlago.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4341 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_github.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4152 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_gitlab.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      784 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_glassfrog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9633 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_gnews.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5986 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_google_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5213 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_google_analytics_data_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4971 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_google_analytics_v4.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1231 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_google_directory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5235 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_google_search_console.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3280 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_google_sheets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1597 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_google_webfonts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1624 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_google_workspace_admin_reports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      919 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_greenhouse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_gridly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2028 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_harvest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_hubplanner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3668 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_hubspot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_insightly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1588 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_instagram.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      769 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_instatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_intercom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1181 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_ip2whois.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1404 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_iterable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3240 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_jira.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_k6_cloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1924 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_klarna.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1332 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_klaviyo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1134 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_kustomer_singer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_launchdarkly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      757 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_lemlist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3583 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_linkedin_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3010 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_linkedin_pages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1550 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_linnworks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1112 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_lokalise.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2746 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_mailchimp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1650 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_mailgun.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1473 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_mailjet_sms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1973 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_marketo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1829 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_metabase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4251 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_microsoft_teams.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6254 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_mixpanel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2588 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_monday.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4422 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_mongodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12234 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_mssql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_my_hours.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12863 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_mysql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2487 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_netsuite.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_notion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2251 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_nytimes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3007 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_okta.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      755 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_omnisend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2695 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_onesignal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3403 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_openweather.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10232 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_oracle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2764 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_orb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1327 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_orbit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1813 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_outreach.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1989 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_paypal_transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1749 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_paystack.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      715 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_pendo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_persistiq.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2551 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_pexels_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3240 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_pinterest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1959 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_pipedrive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3920 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_pocket.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      782 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_pokeapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2981 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_polygon_stock_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7554 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_postgres.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1624 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_posthog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_postmarkapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1468 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_prestashop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      630 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_public_apis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_punk_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_pypi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1814 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_qualaroo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3543 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_quickbooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1065 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_railz.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_recharge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_recreation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1160 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_recruitee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1500 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_recurly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2267 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_redshift.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      883 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_retently.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      840 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_rki_covid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      717 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_rss.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13850 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_s3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3785 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_salesforce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3520 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_salesforce_singer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3552 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_salesloft.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      792 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_sap_fieldglass.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_secoda.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1368 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_sendgrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_sendinblue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3353 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_senseforce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1964 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_sentry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3653 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_sftp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3477 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_sftp_bulk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3217 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_shopify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1135 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_shortio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4288 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_slack.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1255 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_smaily.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      776 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_smartengage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4183 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_smartsheets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2135 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_snapchat_marketing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4413 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_snowflake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2206 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_sonar_cloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      997 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_spacex_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3714 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_square.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2103 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_strava.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2529 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_stripe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2702 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_survey_sparrow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3738 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_surveymonkey.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_tempo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2981 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_the_guardian_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4470 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_tiktok_marketing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_todoist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2023 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_trello.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3853 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_trustpilot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1797 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_tvmaze_schedule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1662 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_twilio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      988 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_twilio_taskrouter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2178 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_twitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1789 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_typeform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1315 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_us_census.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_vantage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1084 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_webflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_whisky_hunter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2403 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_wikipedia_pageviews.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1581 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_woocommerce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2469 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_xero.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      586 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_xkcd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_yandex_metrica.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1447 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_younium.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      836 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_youtube_analytics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3567 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_zendesk_chat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3150 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_zendesk_sunshine.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2067 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_zendesk_support.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1787 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_zendesk_talk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1889 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_zenloop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3102 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_zoho_crm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      733 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_zoom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1706 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/source_zuora.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1050 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/sourcecreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/sourceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      801 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/sourcesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1598 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/streamconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      709 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/streamconfigurations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1778 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/streamproperties.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      469 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/workspacecreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1268 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/workspaceoauthcredentialsrequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      857 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/workspaceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      816 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/models/shared/workspacesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3591 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6839 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/sources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1982 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:10:11.896006 airbyte-api-0.3.0/src/airbyte/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6106 2023-04-27 19:10:01.000000 airbyte-api-0.3.0/src/airbyte/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:10:11.896006 airbyte-api-0.3.0/src/airbyte_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-04-27 19:10:11.000000 airbyte-api-0.3.0/src/airbyte_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13849 2023-04-27 19:10:11.000000 airbyte-api-0.3.0/src/airbyte_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:10:11.000000 airbyte-api-0.3.0/src/airbyte_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-27 19:10:11.000000 airbyte-api-0.3.0/src/airbyte_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 19:10:11.000000 airbyte-api-0.3.0/src/airbyte_api.egg-info/top_level.txt
```

### Comparing `airbyte-api-0.1.0/LICENSE.md` & `airbyte-api-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/PKG-INFO` & `airbyte-api-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,35 @@
-Metadata-Version: 2.1
-Name: airbyte-api
-Version: 0.1.0
-Summary: Python Client SDK for Airbyte API
-Home-page: UNKNOWN
-Author: Airbyte
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 <div align="center">
-    <picture>
         <img src="https://user-images.githubusercontent.com/68016351/222853569-b35cc448-6481-4cf2-a237-bd5da47e94fd.png" width="500">
-    </picture>
    <p>Programatically control Airbyte Cloud through an API.</p>
    <a href="https://reference.airbyte.com/reference/start"><img src="https://img.shields.io/static/v1?label=Docs&message=API Ref&color=000000&style=for-the-badge" /></a>
    <a href="https://github.com/airbytehq/airbyte-api-python-sdk/actions"><img src="https://img.shields.io/github/actions/workflow/status/airbytehq/airbyte-api-python-sdk/speakeasy_sdk_generation.yml?style=for-the-badge" /></a>
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge" /></a>
   <a href="https://github.com/airbytehq/airbyte-api-python-sdk/releases"><img src="https://img.shields.io/github/v/release/airbytehq/airbyte-api-python-sdk?sort=semver&style=for-the-badge" /></a>
 </div>
 
 ## Authentication
 
 Developers will need to create an API Key within your [Developer Portal](https://portal.airbyte.com/) to make API requests. You can use your existing Airbyte account to log in to the Developer Portal. Once you are in the Developer Portal, use the API Keys tab to create or remove API Keys. You can see a [walkthrough demo here](https://www.loom.com/share/7997a7c67cd642cc8d1c72ef0dfcc4bc)🎦
 
 The Developer Portal UI can also be used to help build your integration by showing information about network requests in the Requests tab. API usage information is also available to you in the Usage tab.
 
-***(Installation will not work until published to a package manager, please clone locally and run `pip install -e ../path/to/local/clone` to try out the artifact locally)***
-
 <!-- Start SDK Installation -->
 ## SDK Installation
 
 ```bash
 pip install airbyte-api
 ```
 <!-- End SDK Installation -->
 
 ## SDK Example Usage
 <!-- Start SDK Example Usage -->
 ```python
 import airbyte
-from airbyte.models import operations, shared
+from airbyte.models import shared
 
 s = airbyte.Airbyte(
     security=shared.Security(
         bearer_auth="Bearer YOUR_BEARER_TOKEN_HERE",
     ),
 )
 
@@ -121,74 +105,72 @@
     prefix="dolorem",
     schedule=shared.ConnectionScheduleCreate(
         cron_expression="corporis",
         schedule_type="manual",
     ),
     source_id="c5955907-aff1-4a3a-afa9-467739251aa5",
 )
-    
+
 res = s.connections.create_connection(req)
 
 if res.connection_response is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
 ## Available Resources and Operations
 
 
-### connections
+### [connections](docs/connections/README.md)
 
-* `create_connection` - Create a connection
-* `delete_connection` - Delete a Connection
-* `get_connection` - Get Connection details
-* `list_connections` - List connections
+* [create_connection](docs/connections/README.md#create_connection) - Create a connection
+* [delete_connection](docs/connections/README.md#delete_connection) - Delete a Connection
+* [get_connection](docs/connections/README.md#get_connection) - Get Connection details
+* [list_connections](docs/connections/README.md#list_connections) - List connections
 
-### destinations
+### [destinations](docs/destinations/README.md)
 
-* `create_destination` - Create a destination
-* `delete_destination` - Delete a Destination
-* `get_destination` - Get Destination details
-* `list_destinations` - List destinations
+* [create_destination](docs/destinations/README.md#create_destination) - Create a destination
+* [delete_destination](docs/destinations/README.md#delete_destination) - Delete a Destination
+* [get_destination](docs/destinations/README.md#get_destination) - Get Destination details
+* [list_destinations](docs/destinations/README.md#list_destinations) - List destinations
 
-### jobs
+### [jobs](docs/jobs/README.md)
 
-* `cancel_job` - Cancel a running Job
-* `create_job` - Trigger a sync or reset job of a connection
-* `get_job` - Get Job status and details
-* `list_jobs` - List Jobs by sync type
+* [cancel_job](docs/jobs/README.md#cancel_job) - Cancel a running Job
+* [create_job](docs/jobs/README.md#create_job) - Trigger a sync or reset job of a connection
+* [get_job](docs/jobs/README.md#get_job) - Get Job status and details
+* [list_jobs](docs/jobs/README.md#list_jobs) - List Jobs by sync type
 
-### sources
+### [sources](docs/sources/README.md)
 
-* `create_source` - Create a source
-* `delete_source` - Delete a Source
-* `get_source` - Get Source details
-* `initiate_o_auth` - Initiate OAuth for a source
-* `list_sources` - List sources
+* [create_source](docs/sources/README.md#create_source) - Create a source
+* [delete_source](docs/sources/README.md#delete_source) - Delete a Source
+* [get_source](docs/sources/README.md#get_source) - Get Source details
+* [initiate_o_auth](docs/sources/README.md#initiate_o_auth) - Initiate OAuth for a source
+* [list_sources](docs/sources/README.md#list_sources) - List sources
 
-### streams
+### [streams](docs/streams/README.md)
 
-* `get_stream_properties` - Get stream properties
+* [get_stream_properties](docs/streams/README.md#get_stream_properties) - Get stream properties
 
-### workspaces
+### [workspaces](docs/workspaces/README.md)
 
-* `create_or_update_workspace_o_auth_credentials` - Create OAuth override credentials for a workspace and source type.
-* `create_workspace` - Create a workspace
-* `get_workspace` - Get Workspace details
-* `list_workspaces` - List workspaces
+* [create_or_update_workspace_o_auth_credentials](docs/workspaces/README.md#create_or_update_workspace_o_auth_credentials) - Create OAuth override credentials for a workspace and source type.
+* [create_workspace](docs/workspaces/README.md#create_workspace) - Create a workspace
+* [get_workspace](docs/workspaces/README.md#get_workspace) - Get Workspace details
+* [list_workspaces](docs/workspaces/README.md#list_workspaces) - List workspaces
 <!-- End SDK Available Operations -->
 
 ### Maturity
 
 This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
 to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
 looking for the latest version.
 
 ### Contributions
 
 While we value open-source contributions to this SDK, this library is generated programmatically.
 Feel free to open a PR or a Github issue as a proof of concept and we'll do our best to include it in a future release !
 
 ### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
-
-
```

#### html2text {}

```diff
@@ -1,13 +1,9 @@
-Metadata-Version: 2.1 Name: airbyte-api Version: 0.1.0 Summary: Python Client
-SDK for Airbyte API Home-page: UNKNOWN Author: Airbyte License: UNKNOWN
-Platform: UNKNOWN Requires-Python: >=3.9 Description-Content-Type: text/
-markdown License-File: LICENSE.md
-  [https://user-images.githubusercontent.com/68016351/222853569-b35cc448-6481-
-                         4cf2-a237-bd5da47e94fd.png]
+ [https://user-images.githubusercontent.com/68016351/222853569-b35cc448-6481-
+                          4cf2-a237-bd5da47e94fd.png]
              Programatically control Airbyte Cloud through an API.
            [https://img.shields.io/static/v1?label=Docs&message=API
  Ref&color=000000&style=for-the-badge] [https://img.shields.io/github/actions/
                workflow/status/airbytehq/airbyte-api-python-sdk/
   speakeasy_sdk_generation.yml?style=for-the-badge] [https://img.shields.io/
 badge/License-MIT-blue.svg?style=for-the-badge] [https://img.shields.io/github/
   v/release/airbytehq/airbyte-api-python-sdk?sort=semver&style=for-the-badge]
@@ -15,53 +11,67 @@
 [Developer Portal](https://portal.airbyte.com/) to make API requests. You can
 use your existing Airbyte account to log in to the Developer Portal. Once you
 are in the Developer Portal, use the API Keys tab to create or remove API Keys.
 You can see a [walkthrough demo here](https://www.loom.com/share/
 7997a7c67cd642cc8d1c72ef0dfcc4bc)ð¦ The Developer Portal UI can also be used
 to help build your integration by showing information about network requests in
 the Requests tab. API usage information is also available to you in the Usage
-tab. ***(Installation will not work until published to a package manager,
-please clone locally and run `pip install -e ../path/to/local/clone` to try out
-the artifact locally)***  ## SDK Installation ```bash pip install airbyte-api
-```  ## SDK Example Usage  ```python import airbyte from airbyte.models import
-operations, shared s = airbyte.Airbyte( security=shared.Security
-( bearer_auth="Bearer YOUR_BEARER_TOKEN_HERE", ), ) req =
-shared.ConnectionCreateRequest( configurations=shared.StreamConfigurations
-( streams=[ shared.StreamConfiguration( cursor_field=[ "distinctio",
-"quibusdam", "unde", ], name="Johnnie Stamm", primary_key=[ [ "iure", "magnam",
-], [ "ipsa", "delectus", "tempora", "suscipit", ], [ "minus", "placeat", ], ],
+tab.  ## SDK Installation ```bash pip install airbyte-api ```  ## SDK Example
+Usage  ```python import airbyte from airbyte.models import shared s =
+airbyte.Airbyte( security=shared.Security( bearer_auth="Bearer
+YOUR_BEARER_TOKEN_HERE", ), ) req = shared.ConnectionCreateRequest
+( configurations=shared.StreamConfigurations( streams=
+[ shared.StreamConfiguration( cursor_field=[ "distinctio", "quibusdam", "unde",
+], name="Johnnie Stamm", primary_key=[ [ "iure", "magnam", ], [ "ipsa",
+"delectus", "tempora", "suscipit", ], [ "minus", "placeat", ], ],
 sync_mode="incremental_append", ), shared.StreamConfiguration( cursor_field=
 [ "excepturi", "nisi", ], name="Jake Bernier MD", primary_key=[
 [ "repellendus", "sapiente", ], ], sync_mode="incremental_deduped_history", ),
 shared.StreamConfiguration( cursor_field=[ "at", ], name="Emilio Krajcik",
 primary_key=[ [ "porro", "dolorum", "dicta", ], [ "officia", "occaecati",
 "fugit", ], ], sync_mode="incremental_append", ), ], ), data_residency="eu",
 destination_id="c816742c-b739-4205-9293-96fea7596eb1", name="Lela Orn",
 namespace_definition="source", namespace_format="${SOURCE_NAMESPACE}",
 prefix="dolorem", schedule=shared.ConnectionScheduleCreate
 ( cron_expression="corporis", schedule_type="manual", ), source_id="c5955907-
 aff1-4a3a-afa9-467739251aa5", ) res = s.connections.create_connection(req) if
 res.connection_response is not None: # handle response ```   ## Available
-Resources and Operations ### connections * `create_connection` - Create a
-connection * `delete_connection` - Delete a Connection * `get_connection` - Get
-Connection details * `list_connections` - List connections ### destinations *
-`create_destination` - Create a destination * `delete_destination` - Delete a
-Destination * `get_destination` - Get Destination details * `list_destinations`
-- List destinations ### jobs * `cancel_job` - Cancel a running Job *
-`create_job` - Trigger a sync or reset job of a connection * `get_job` - Get
-Job status and details * `list_jobs` - List Jobs by sync type ### sources *
-`create_source` - Create a source * `delete_source` - Delete a Source *
-`get_source` - Get Source details * `initiate_o_auth` - Initiate OAuth for a
-source * `list_sources` - List sources ### streams * `get_stream_properties` -
-Get stream properties ### workspaces *
-`create_or_update_workspace_o_auth_credentials` - Create OAuth override
-credentials for a workspace and source type. * `create_workspace` - Create a
-workspace * `get_workspace` - Get Workspace details * `list_workspaces` - List
-workspaces  ### Maturity This SDK is in beta, and there may be breaking changes
-between versions without a major version update. Therefore, we recommend
-pinning usage to a specific package version. This way, you can install the same
-version each time without breaking changes unless you are intentionally looking
-for the latest version. ### Contributions While we value open-source
-contributions to this SDK, this library is generated programmatically. Feel
-free to open a PR or a Github issue as a proof of concept and we'll do our best
-to include it in a future release ! ### SDK Created by [Speakeasy](https://
-docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
+Resources and Operations ### [connections](docs/connections/README.md) *
+[create_connection](docs/connections/README.md#create_connection) - Create a
+connection * [delete_connection](docs/connections/README.md#delete_connection)
+- Delete a Connection * [get_connection](docs/connections/
+README.md#get_connection) - Get Connection details * [list_connections](docs/
+connections/README.md#list_connections) - List connections ### [destinations]
+(docs/destinations/README.md) * [create_destination](docs/destinations/
+README.md#create_destination) - Create a destination * [delete_destination]
+(docs/destinations/README.md#delete_destination) - Delete a Destination *
+[get_destination](docs/destinations/README.md#get_destination) - Get
+Destination details * [list_destinations](docs/destinations/
+README.md#list_destinations) - List destinations ### [jobs](docs/jobs/
+README.md) * [cancel_job](docs/jobs/README.md#cancel_job) - Cancel a running
+Job * [create_job](docs/jobs/README.md#create_job) - Trigger a sync or reset
+job of a connection * [get_job](docs/jobs/README.md#get_job) - Get Job status
+and details * [list_jobs](docs/jobs/README.md#list_jobs) - List Jobs by sync
+type ### [sources](docs/sources/README.md) * [create_source](docs/sources/
+README.md#create_source) - Create a source * [delete_source](docs/sources/
+README.md#delete_source) - Delete a Source * [get_source](docs/sources/
+README.md#get_source) - Get Source details * [initiate_o_auth](docs/sources/
+README.md#initiate_o_auth) - Initiate OAuth for a source * [list_sources](docs/
+sources/README.md#list_sources) - List sources ### [streams](docs/streams/
+README.md) * [get_stream_properties](docs/streams/
+README.md#get_stream_properties) - Get stream properties ### [workspaces](docs/
+workspaces/README.md) * [create_or_update_workspace_o_auth_credentials](docs/
+workspaces/README.md#create_or_update_workspace_o_auth_credentials) - Create
+OAuth override credentials for a workspace and source type. *
+[create_workspace](docs/workspaces/README.md#create_workspace) - Create a
+workspace * [get_workspace](docs/workspaces/README.md#get_workspace) - Get
+Workspace details * [list_workspaces](docs/workspaces/
+README.md#list_workspaces) - List workspaces  ### Maturity This SDK is in beta,
+and there may be breaking changes between versions without a major version
+update. Therefore, we recommend pinning usage to a specific package version.
+This way, you can install the same version each time without breaking changes
+unless you are intentionally looking for the latest version. ### Contributions
+While we value open-source contributions to this SDK, this library is generated
+programmatically. Feel free to open a PR or a Github issue as a proof of
+concept and we'll do our best to include it in a future release ! ### SDK
+Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/
+client-sdks)
```

### Comparing `airbyte-api-0.1.0/README.md` & `airbyte-api-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,47 @@
+Metadata-Version: 2.1
+Name: airbyte-api
+Version: 0.3.0
+Summary: Python Client SDK for Airbyte API
+Home-page: UNKNOWN
+Author: Airbyte
+License: UNKNOWN
+Platform: UNKNOWN
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 <div align="center">
-    <picture>
         <img src="https://user-images.githubusercontent.com/68016351/222853569-b35cc448-6481-4cf2-a237-bd5da47e94fd.png" width="500">
-    </picture>
    <p>Programatically control Airbyte Cloud through an API.</p>
    <a href="https://reference.airbyte.com/reference/start"><img src="https://img.shields.io/static/v1?label=Docs&message=API Ref&color=000000&style=for-the-badge" /></a>
    <a href="https://github.com/airbytehq/airbyte-api-python-sdk/actions"><img src="https://img.shields.io/github/actions/workflow/status/airbytehq/airbyte-api-python-sdk/speakeasy_sdk_generation.yml?style=for-the-badge" /></a>
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge" /></a>
   <a href="https://github.com/airbytehq/airbyte-api-python-sdk/releases"><img src="https://img.shields.io/github/v/release/airbytehq/airbyte-api-python-sdk?sort=semver&style=for-the-badge" /></a>
 </div>
 
 ## Authentication
 
 Developers will need to create an API Key within your [Developer Portal](https://portal.airbyte.com/) to make API requests. You can use your existing Airbyte account to log in to the Developer Portal. Once you are in the Developer Portal, use the API Keys tab to create or remove API Keys. You can see a [walkthrough demo here](https://www.loom.com/share/7997a7c67cd642cc8d1c72ef0dfcc4bc)🎦
 
 The Developer Portal UI can also be used to help build your integration by showing information about network requests in the Requests tab. API usage information is also available to you in the Usage tab.
 
-***(Installation will not work until published to a package manager, please clone locally and run `pip install -e ../path/to/local/clone` to try out the artifact locally)***
-
 <!-- Start SDK Installation -->
 ## SDK Installation
 
 ```bash
 pip install airbyte-api
 ```
 <!-- End SDK Installation -->
 
 ## SDK Example Usage
 <!-- Start SDK Example Usage -->
 ```python
 import airbyte
-from airbyte.models import operations, shared
+from airbyte.models import shared
 
 s = airbyte.Airbyte(
     security=shared.Security(
         bearer_auth="Bearer YOUR_BEARER_TOKEN_HERE",
     ),
 )
 
@@ -109,72 +117,74 @@
     prefix="dolorem",
     schedule=shared.ConnectionScheduleCreate(
         cron_expression="corporis",
         schedule_type="manual",
     ),
     source_id="c5955907-aff1-4a3a-afa9-467739251aa5",
 )
-    
+
 res = s.connections.create_connection(req)
 
 if res.connection_response is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
 ## Available Resources and Operations
 
 
-### connections
+### [connections](docs/connections/README.md)
 
-* `create_connection` - Create a connection
-* `delete_connection` - Delete a Connection
-* `get_connection` - Get Connection details
-* `list_connections` - List connections
+* [create_connection](docs/connections/README.md#create_connection) - Create a connection
+* [delete_connection](docs/connections/README.md#delete_connection) - Delete a Connection
+* [get_connection](docs/connections/README.md#get_connection) - Get Connection details
+* [list_connections](docs/connections/README.md#list_connections) - List connections
 
-### destinations
+### [destinations](docs/destinations/README.md)
 
-* `create_destination` - Create a destination
-* `delete_destination` - Delete a Destination
-* `get_destination` - Get Destination details
-* `list_destinations` - List destinations
+* [create_destination](docs/destinations/README.md#create_destination) - Create a destination
+* [delete_destination](docs/destinations/README.md#delete_destination) - Delete a Destination
+* [get_destination](docs/destinations/README.md#get_destination) - Get Destination details
+* [list_destinations](docs/destinations/README.md#list_destinations) - List destinations
 
-### jobs
+### [jobs](docs/jobs/README.md)
 
-* `cancel_job` - Cancel a running Job
-* `create_job` - Trigger a sync or reset job of a connection
-* `get_job` - Get Job status and details
-* `list_jobs` - List Jobs by sync type
+* [cancel_job](docs/jobs/README.md#cancel_job) - Cancel a running Job
+* [create_job](docs/jobs/README.md#create_job) - Trigger a sync or reset job of a connection
+* [get_job](docs/jobs/README.md#get_job) - Get Job status and details
+* [list_jobs](docs/jobs/README.md#list_jobs) - List Jobs by sync type
 
-### sources
+### [sources](docs/sources/README.md)
 
-* `create_source` - Create a source
-* `delete_source` - Delete a Source
-* `get_source` - Get Source details
-* `initiate_o_auth` - Initiate OAuth for a source
-* `list_sources` - List sources
+* [create_source](docs/sources/README.md#create_source) - Create a source
+* [delete_source](docs/sources/README.md#delete_source) - Delete a Source
+* [get_source](docs/sources/README.md#get_source) - Get Source details
+* [initiate_o_auth](docs/sources/README.md#initiate_o_auth) - Initiate OAuth for a source
+* [list_sources](docs/sources/README.md#list_sources) - List sources
 
-### streams
+### [streams](docs/streams/README.md)
 
-* `get_stream_properties` - Get stream properties
+* [get_stream_properties](docs/streams/README.md#get_stream_properties) - Get stream properties
 
-### workspaces
+### [workspaces](docs/workspaces/README.md)
 
-* `create_or_update_workspace_o_auth_credentials` - Create OAuth override credentials for a workspace and source type.
-* `create_workspace` - Create a workspace
-* `get_workspace` - Get Workspace details
-* `list_workspaces` - List workspaces
+* [create_or_update_workspace_o_auth_credentials](docs/workspaces/README.md#create_or_update_workspace_o_auth_credentials) - Create OAuth override credentials for a workspace and source type.
+* [create_workspace](docs/workspaces/README.md#create_workspace) - Create a workspace
+* [get_workspace](docs/workspaces/README.md#get_workspace) - Get Workspace details
+* [list_workspaces](docs/workspaces/README.md#list_workspaces) - List workspaces
 <!-- End SDK Available Operations -->
 
 ### Maturity
 
 This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
 to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
 looking for the latest version.
 
 ### Contributions
 
 While we value open-source contributions to this SDK, this library is generated programmatically.
 Feel free to open a PR or a Github issue as a proof of concept and we'll do our best to include it in a future release !
 
 ### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
+
+
```

#### html2text {}

```diff
@@ -1,9 +1,13 @@
-  [https://user-images.githubusercontent.com/68016351/222853569-b35cc448-6481-
-                         4cf2-a237-bd5da47e94fd.png]
+Metadata-Version: 2.1 Name: airbyte-api Version: 0.3.0 Summary: Python Client
+SDK for Airbyte API Home-page: UNKNOWN Author: Airbyte License: UNKNOWN
+Platform: UNKNOWN Requires-Python: >=3.9 Description-Content-Type: text/
+markdown License-File: LICENSE.md
+ [https://user-images.githubusercontent.com/68016351/222853569-b35cc448-6481-
+                          4cf2-a237-bd5da47e94fd.png]
              Programatically control Airbyte Cloud through an API.
            [https://img.shields.io/static/v1?label=Docs&message=API
  Ref&color=000000&style=for-the-badge] [https://img.shields.io/github/actions/
                workflow/status/airbytehq/airbyte-api-python-sdk/
   speakeasy_sdk_generation.yml?style=for-the-badge] [https://img.shields.io/
 badge/License-MIT-blue.svg?style=for-the-badge] [https://img.shields.io/github/
   v/release/airbytehq/airbyte-api-python-sdk?sort=semver&style=for-the-badge]
@@ -11,53 +15,67 @@
 [Developer Portal](https://portal.airbyte.com/) to make API requests. You can
 use your existing Airbyte account to log in to the Developer Portal. Once you
 are in the Developer Portal, use the API Keys tab to create or remove API Keys.
 You can see a [walkthrough demo here](https://www.loom.com/share/
 7997a7c67cd642cc8d1c72ef0dfcc4bc)ð¦ The Developer Portal UI can also be used
 to help build your integration by showing information about network requests in
 the Requests tab. API usage information is also available to you in the Usage
-tab. ***(Installation will not work until published to a package manager,
-please clone locally and run `pip install -e ../path/to/local/clone` to try out
-the artifact locally)***  ## SDK Installation ```bash pip install airbyte-api
-```  ## SDK Example Usage  ```python import airbyte from airbyte.models import
-operations, shared s = airbyte.Airbyte( security=shared.Security
-( bearer_auth="Bearer YOUR_BEARER_TOKEN_HERE", ), ) req =
-shared.ConnectionCreateRequest( configurations=shared.StreamConfigurations
-( streams=[ shared.StreamConfiguration( cursor_field=[ "distinctio",
-"quibusdam", "unde", ], name="Johnnie Stamm", primary_key=[ [ "iure", "magnam",
-], [ "ipsa", "delectus", "tempora", "suscipit", ], [ "minus", "placeat", ], ],
+tab.  ## SDK Installation ```bash pip install airbyte-api ```  ## SDK Example
+Usage  ```python import airbyte from airbyte.models import shared s =
+airbyte.Airbyte( security=shared.Security( bearer_auth="Bearer
+YOUR_BEARER_TOKEN_HERE", ), ) req = shared.ConnectionCreateRequest
+( configurations=shared.StreamConfigurations( streams=
+[ shared.StreamConfiguration( cursor_field=[ "distinctio", "quibusdam", "unde",
+], name="Johnnie Stamm", primary_key=[ [ "iure", "magnam", ], [ "ipsa",
+"delectus", "tempora", "suscipit", ], [ "minus", "placeat", ], ],
 sync_mode="incremental_append", ), shared.StreamConfiguration( cursor_field=
 [ "excepturi", "nisi", ], name="Jake Bernier MD", primary_key=[
 [ "repellendus", "sapiente", ], ], sync_mode="incremental_deduped_history", ),
 shared.StreamConfiguration( cursor_field=[ "at", ], name="Emilio Krajcik",
 primary_key=[ [ "porro", "dolorum", "dicta", ], [ "officia", "occaecati",
 "fugit", ], ], sync_mode="incremental_append", ), ], ), data_residency="eu",
 destination_id="c816742c-b739-4205-9293-96fea7596eb1", name="Lela Orn",
 namespace_definition="source", namespace_format="${SOURCE_NAMESPACE}",
 prefix="dolorem", schedule=shared.ConnectionScheduleCreate
 ( cron_expression="corporis", schedule_type="manual", ), source_id="c5955907-
 aff1-4a3a-afa9-467739251aa5", ) res = s.connections.create_connection(req) if
 res.connection_response is not None: # handle response ```   ## Available
-Resources and Operations ### connections * `create_connection` - Create a
-connection * `delete_connection` - Delete a Connection * `get_connection` - Get
-Connection details * `list_connections` - List connections ### destinations *
-`create_destination` - Create a destination * `delete_destination` - Delete a
-Destination * `get_destination` - Get Destination details * `list_destinations`
-- List destinations ### jobs * `cancel_job` - Cancel a running Job *
-`create_job` - Trigger a sync or reset job of a connection * `get_job` - Get
-Job status and details * `list_jobs` - List Jobs by sync type ### sources *
-`create_source` - Create a source * `delete_source` - Delete a Source *
-`get_source` - Get Source details * `initiate_o_auth` - Initiate OAuth for a
-source * `list_sources` - List sources ### streams * `get_stream_properties` -
-Get stream properties ### workspaces *
-`create_or_update_workspace_o_auth_credentials` - Create OAuth override
-credentials for a workspace and source type. * `create_workspace` - Create a
-workspace * `get_workspace` - Get Workspace details * `list_workspaces` - List
-workspaces  ### Maturity This SDK is in beta, and there may be breaking changes
-between versions without a major version update. Therefore, we recommend
-pinning usage to a specific package version. This way, you can install the same
-version each time without breaking changes unless you are intentionally looking
-for the latest version. ### Contributions While we value open-source
-contributions to this SDK, this library is generated programmatically. Feel
-free to open a PR or a Github issue as a proof of concept and we'll do our best
-to include it in a future release ! ### SDK Created by [Speakeasy](https://
-docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
+Resources and Operations ### [connections](docs/connections/README.md) *
+[create_connection](docs/connections/README.md#create_connection) - Create a
+connection * [delete_connection](docs/connections/README.md#delete_connection)
+- Delete a Connection * [get_connection](docs/connections/
+README.md#get_connection) - Get Connection details * [list_connections](docs/
+connections/README.md#list_connections) - List connections ### [destinations]
+(docs/destinations/README.md) * [create_destination](docs/destinations/
+README.md#create_destination) - Create a destination * [delete_destination]
+(docs/destinations/README.md#delete_destination) - Delete a Destination *
+[get_destination](docs/destinations/README.md#get_destination) - Get
+Destination details * [list_destinations](docs/destinations/
+README.md#list_destinations) - List destinations ### [jobs](docs/jobs/
+README.md) * [cancel_job](docs/jobs/README.md#cancel_job) - Cancel a running
+Job * [create_job](docs/jobs/README.md#create_job) - Trigger a sync or reset
+job of a connection * [get_job](docs/jobs/README.md#get_job) - Get Job status
+and details * [list_jobs](docs/jobs/README.md#list_jobs) - List Jobs by sync
+type ### [sources](docs/sources/README.md) * [create_source](docs/sources/
+README.md#create_source) - Create a source * [delete_source](docs/sources/
+README.md#delete_source) - Delete a Source * [get_source](docs/sources/
+README.md#get_source) - Get Source details * [initiate_o_auth](docs/sources/
+README.md#initiate_o_auth) - Initiate OAuth for a source * [list_sources](docs/
+sources/README.md#list_sources) - List sources ### [streams](docs/streams/
+README.md) * [get_stream_properties](docs/streams/
+README.md#get_stream_properties) - Get stream properties ### [workspaces](docs/
+workspaces/README.md) * [create_or_update_workspace_o_auth_credentials](docs/
+workspaces/README.md#create_or_update_workspace_o_auth_credentials) - Create
+OAuth override credentials for a workspace and source type. *
+[create_workspace](docs/workspaces/README.md#create_workspace) - Create a
+workspace * [get_workspace](docs/workspaces/README.md#get_workspace) - Get
+Workspace details * [list_workspaces](docs/workspaces/
+README.md#list_workspaces) - List workspaces  ### Maturity This SDK is in beta,
+and there may be breaking changes between versions without a major version
+update. Therefore, we recommend pinning usage to a specific package version.
+This way, you can install the same version each time without breaking changes
+unless you are intentionally looking for the latest version. ### Contributions
+While we value open-source contributions to this SDK, this library is generated
+programmatically. Feel free to open a PR or a Github issue as a proof of
+concept and we'll do our best to include it in a future release ! ### SDK
+Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/
+client-sdks)
```

### Comparing `airbyte-api-0.1.0/setup.py` & `airbyte-api-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="airbyte-api",
-    version="0.1.0",
+    version="0.3.0",
     author="Airbyte",
     description="Python Client SDK for Airbyte API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
-        "certifi==2022.12.07",
+        "certifi==2022.12.7",
         "charset-normalizer==2.1.1",
         "dataclasses-json-speakeasy==0.5.8",
         "idna==3.3",
         "marshmallow==3.17.1",
         "marshmallow-enum==1.5.1",
         "mypy-extensions==0.4.3",
         "packaging==21.3",
```

### Comparing `airbyte-api-0.1.0/src/airbyte/connections.py` & `airbyte-api-0.3.0/src/airbyte/connections.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/destinations.py` & `airbyte-api-0.3.0/src/airbyte/destinations.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/jobs.py` & `airbyte-api-0.3.0/src/airbyte/jobs.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/__init__.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/canceljob.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/canceljob.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/createconnection.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/createconnection.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/createdestination.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/createdestination.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/createjob.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/createjob.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/createorupdateworkspaceoauthcredentials.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/createorupdateworkspaceoauthcredentials.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/createsource.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/createsource.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/createworkspace.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/createworkspace.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/deleteconnection.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/deleteconnection.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/deletedestination.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/deletedestination.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/deletesource.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/deletesource.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/getconnection.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/getconnection.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/getdestination.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/getdestination.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/getjob.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/getjob.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/getsource.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/getsource.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/getstreamproperties.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/getstreamproperties.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/getworkspace.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/getworkspace.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/listconnections.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/listconnections.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/listdestinations.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/listdestinations.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/listjobs.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/listjobs.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/listsources.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/listsources.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/operations/listworkspaces.py` & `airbyte-api-0.3.0/src/airbyte/models/operations/listworkspaces.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/__init__.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/connectioncreaterequest.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/connectioncreaterequest.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/connectionresponse.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/connectionresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/connectionschedulecreate.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/connectionschedulecreate.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/connectionscheduleresponse.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/connectionscheduleresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/connectionsresponse.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/connectionsresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_amazon_sqs.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_amazon_sqs.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_aws_datalake.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_aws_datalake.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_azure_blob_storage.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_bigquery.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_bigquery.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_bigquery_denormalized.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_bigquery_denormalized.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_cassandra.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_cassandra.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_clickhouse.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_clickhouse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_convex.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_convex.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_databend.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_databend.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_databricks.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_databricks.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_dynamodb.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_dynamodb.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_elasticsearch.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_firebolt.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_firebolt.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_firestore.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_firestore.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_gcs.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_gcs.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_google_sheets.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_google_sheets.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_keen.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_keen.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_kinesis.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_kinesis.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_mariadb_columnstore.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_mariadb_columnstore.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_meilisearch.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_meilisearch.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_mongodb.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_mongodb.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_mssql.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_mssql.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_mysql.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_mysql.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_oracle.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_oracle.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_postgres.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_postgres.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_pubsub.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_pubsub.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_pulsar.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_pulsar.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_rabbitmq.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_redis.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_redis.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_redshift.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_redshift.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_rockset.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_rockset.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_s3.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_s3.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_s3_glue.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_s3_glue.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_scylla.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_scylla.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_sftp_json.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_sftp_json.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_snowflake.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_snowflake.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destination_typesense.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destination_typesense.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destinationcreaterequest.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destinationcreaterequest.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destinationresponse.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destinationresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/destinationsresponse.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/destinationsresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/initiateoauthrequest.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/initiateoauthrequest.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/jobcreaterequest.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/jobcreaterequest.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/jobresponse.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/jobresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/jobsresponse.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/jobsresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_airtable.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_airtable.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_alloydb.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_alloydb.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_amazon_ads.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_amazon_ads.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_amazon_seller_partner.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_amazon_seller_partner.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_amazon_sqs.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_amazon_sqs.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_amplitude.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_amplitude.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_apify_dataset.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_apify_dataset.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_asana.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_asana.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_auth0.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_auth0.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_aws_cloudtrail.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_aws_cloudtrail.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_azure_blob_storage.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_azure_table.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_azure_table.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_bamboo_hr.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_bamboo_hr.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_bigcommerce.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_bigcommerce.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_bigquery.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_bigquery.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_bing_ads.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_bing_ads.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_braintree.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_braintree.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_braze.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_braze.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_chargebee.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_chargebee.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_chartmogul.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_chartmogul.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_clickhouse.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_clickhouse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_clickup_api.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_clickup_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_close_com.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_close_com.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_coda.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_coda.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_coin_api.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_coin_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_coinmarketcap.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_coinmarketcap.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_configcat.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_configcat.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_confluence.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_confluence.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_datascope.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_datascope.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_delighted.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_delighted.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_dixa.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_dixa.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_dockerhub.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_dockerhub.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_dremio.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_dremio.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_dynamodb.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_dynamodb.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_e2e_test_cloud.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_e2e_test_cloud.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_emailoctopus.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_emailoctopus.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_exchange_rates.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_exchange_rates.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_facebook_marketing.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_facebook_marketing.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_facebook_pages.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_facebook_pages.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_faker.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_faker.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_fauna.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_fauna.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_file_secure.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_file_secure.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_firebolt.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_firebolt.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_freshcaller.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_freshcaller.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_freshdesk.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_freshdesk.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_freshsales.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_freshsales.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_gcs.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_gcs.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_getlago.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_getlago.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_github.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_github.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_gitlab.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_gitlab.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_glassfrog.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_glassfrog.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_gnews.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_gnews.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_google_ads.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_google_ads.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_google_analytics_data_api.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_google_analytics_data_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_google_analytics_v4.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_google_analytics_v4.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_google_directory.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_google_directory.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_google_search_console.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_google_search_console.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_google_sheets.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_google_sheets.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_google_webfonts.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_google_webfonts.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_google_workspace_admin_reports.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_google_workspace_admin_reports.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_greenhouse.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_greenhouse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_gridly.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_gridly.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_harvest.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_harvest.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_hubplanner.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_hubplanner.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_hubspot.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_hubspot.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_insightly.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_insightly.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_instagram.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_instagram.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_instatus.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_instatus.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_intercom.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_intercom.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_ip2whois.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_ip2whois.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_iterable.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_iterable.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_jira.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_jira.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_k6_cloud.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_k6_cloud.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_klarna.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_klarna.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_klaviyo.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_klaviyo.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_kustomer_singer.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_kustomer_singer.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_launchdarkly.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_launchdarkly.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_lemlist.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_lemlist.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_linkedin_ads.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_linkedin_ads.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_linkedin_pages.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_linkedin_pages.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_linnworks.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_linnworks.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_lokalise.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_lokalise.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_mailchimp.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_mailchimp.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_mailgun.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_mailgun.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_mailjet_sms.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_mailjet_sms.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_marketo.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_marketo.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_metabase.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_metabase.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_microsoft_teams.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_microsoft_teams.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_mixpanel.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_mixpanel.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_monday.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_monday.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_mongodb.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_mongodb.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_mssql.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_mssql.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_my_hours.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_my_hours.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_mysql.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_mysql.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_netsuite.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_netsuite.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_notion.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_notion.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_nytimes.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_nytimes.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_okta.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_okta.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_omnisend.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_omnisend.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_onesignal.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_onesignal.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_openweather.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_openweather.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_oracle.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_oracle.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_orb.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_orb.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_orbit.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_orbit.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_outreach.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_outreach.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_paypal_transaction.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_paypal_transaction.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_paystack.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_paystack.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_pendo.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_pendo.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_persistiq.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_persistiq.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_pexels_api.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_pexels_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_pinterest.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_pinterest.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_pipedrive.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_pipedrive.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_pocket.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_pocket.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_pokeapi.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_pokeapi.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_polygon_stock_api.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_polygon_stock_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_postgres.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_postgres.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_posthog.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_posthog.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_postmarkapp.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_postmarkapp.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_prestashop.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_prestashop.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_public_apis.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_public_apis.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_punk_api.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_punk_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_pypi.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_pypi.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_qualaroo.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_qualaroo.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_quickbooks.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_quickbooks.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_railz.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_railz.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_recharge.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_recharge.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_recreation.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_recreation.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_recruitee.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_recruitee.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_recurly.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_recurly.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_redshift.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_redshift.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_retently.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_retently.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_rki_covid.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_rki_covid.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_rss.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_rss.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_s3.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_s3.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_salesforce.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_salesforce.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_salesforce_singer.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_salesforce_singer.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_salesloft.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_salesloft.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_sap_fieldglass.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_sap_fieldglass.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_secoda.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_secoda.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_sendgrid.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_sendgrid.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_sendinblue.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_sendinblue.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_senseforce.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_senseforce.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_sentry.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_sentry.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_sftp.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_sftp.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_sftp_bulk.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_sftp_bulk.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_shopify.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_shopify.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_shortio.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_shortio.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_slack.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_slack.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_smaily.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_smaily.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_smartengage.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_smartengage.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_smartsheets.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_smartsheets.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_snapchat_marketing.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_snapchat_marketing.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_snowflake.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_snowflake.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_sonar_cloud.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_sonar_cloud.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_spacex_api.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_spacex_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_square.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_square.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_strava.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_strava.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_stripe.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_stripe.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_survey_sparrow.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_survey_sparrow.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_surveymonkey.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_surveymonkey.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_tempo.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_tempo.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_the_guardian_api.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_the_guardian_api.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_tiktok_marketing.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_tiktok_marketing.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_todoist.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_todoist.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_trello.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_trello.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_trustpilot.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_trustpilot.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_tvmaze_schedule.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_tvmaze_schedule.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_twilio.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_twilio.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_twilio_taskrouter.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_twilio_taskrouter.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_twitter.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_twitter.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_typeform.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_typeform.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_us_census.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_us_census.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_vantage.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_vantage.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_webflow.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_webflow.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_whisky_hunter.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_whisky_hunter.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_wikipedia_pageviews.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_wikipedia_pageviews.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_woocommerce.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_woocommerce.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_xero.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_xero.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_xkcd.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_xkcd.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_yandex_metrica.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_yandex_metrica.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_younium.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_younium.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_youtube_analytics.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_youtube_analytics.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_zendesk_chat.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_zendesk_chat.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_zendesk_sunshine.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_zendesk_sunshine.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_zendesk_support.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_zendesk_support.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_zendesk_talk.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_zendesk_talk.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_zenloop.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_zenloop.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_zoho_crm.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_zoho_crm.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_zoom.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_zoom.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/source_zuora.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/source_zuora.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/sourcecreaterequest.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/sourcecreaterequest.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/sourceresponse.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/sourceresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/sourcesresponse.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/sourcesresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/streamconfiguration.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/streamconfiguration.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/streamconfigurations.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/streamconfigurations.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/streamproperties.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/streamproperties.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/workspaceoauthcredentialsrequest.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/workspaceoauthcredentialsrequest.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/workspaceresponse.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/workspaceresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/models/shared/workspacesresponse.py` & `airbyte-api-0.3.0/src/airbyte/models/shared/workspacesresponse.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/sdk.py` & `airbyte-api-0.3.0/src/airbyte/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     streams: Streams
     workspaces: Workspaces
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.1.0"
-    _gen_version: str = "2.20.1"
+    _sdk_version: str = "0.3.0"
+    _gen_version: str = "2.22.0"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `airbyte-api-0.1.0/src/airbyte/sources.py` & `airbyte-api-0.3.0/src/airbyte/sources.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/streams.py` & `airbyte-api-0.3.0/src/airbyte/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/utils/retries.py` & `airbyte-api-0.3.0/src/airbyte/utils/retries.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/utils/utils.py` & `airbyte-api-0.3.0/src/airbyte/utils/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte/workspaces.py` & `airbyte-api-0.3.0/src/airbyte/workspaces.py`

 * *Files identical despite different names*

### Comparing `airbyte-api-0.1.0/src/airbyte_api.egg-info/PKG-INFO` & `airbyte-api-0.3.0/src/airbyte_api.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 Metadata-Version: 2.1
 Name: airbyte-api
-Version: 0.1.0
+Version: 0.3.0
 Summary: Python Client SDK for Airbyte API
 Home-page: UNKNOWN
 Author: Airbyte
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 <div align="center">
-    <picture>
         <img src="https://user-images.githubusercontent.com/68016351/222853569-b35cc448-6481-4cf2-a237-bd5da47e94fd.png" width="500">
-    </picture>
    <p>Programatically control Airbyte Cloud through an API.</p>
    <a href="https://reference.airbyte.com/reference/start"><img src="https://img.shields.io/static/v1?label=Docs&message=API Ref&color=000000&style=for-the-badge" /></a>
    <a href="https://github.com/airbytehq/airbyte-api-python-sdk/actions"><img src="https://img.shields.io/github/actions/workflow/status/airbytehq/airbyte-api-python-sdk/speakeasy_sdk_generation.yml?style=for-the-badge" /></a>
   <a href="https://opensource.org/licenses/MIT"><img src="https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge" /></a>
   <a href="https://github.com/airbytehq/airbyte-api-python-sdk/releases"><img src="https://img.shields.io/github/v/release/airbytehq/airbyte-api-python-sdk?sort=semver&style=for-the-badge" /></a>
 </div>
 
 ## Authentication
 
 Developers will need to create an API Key within your [Developer Portal](https://portal.airbyte.com/) to make API requests. You can use your existing Airbyte account to log in to the Developer Portal. Once you are in the Developer Portal, use the API Keys tab to create or remove API Keys. You can see a [walkthrough demo here](https://www.loom.com/share/7997a7c67cd642cc8d1c72ef0dfcc4bc)🎦
 
 The Developer Portal UI can also be used to help build your integration by showing information about network requests in the Requests tab. API usage information is also available to you in the Usage tab.
 
-***(Installation will not work until published to a package manager, please clone locally and run `pip install -e ../path/to/local/clone` to try out the artifact locally)***
-
 <!-- Start SDK Installation -->
 ## SDK Installation
 
 ```bash
 pip install airbyte-api
 ```
 <!-- End SDK Installation -->
 
 ## SDK Example Usage
 <!-- Start SDK Example Usage -->
 ```python
 import airbyte
-from airbyte.models import operations, shared
+from airbyte.models import shared
 
 s = airbyte.Airbyte(
     security=shared.Security(
         bearer_auth="Bearer YOUR_BEARER_TOKEN_HERE",
     ),
 )
 
@@ -121,65 +117,65 @@
     prefix="dolorem",
     schedule=shared.ConnectionScheduleCreate(
         cron_expression="corporis",
         schedule_type="manual",
     ),
     source_id="c5955907-aff1-4a3a-afa9-467739251aa5",
 )
-    
+
 res = s.connections.create_connection(req)
 
 if res.connection_response is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
 ## Available Resources and Operations
 
 
-### connections
+### [connections](docs/connections/README.md)
 
-* `create_connection` - Create a connection
-* `delete_connection` - Delete a Connection
-* `get_connection` - Get Connection details
-* `list_connections` - List connections
+* [create_connection](docs/connections/README.md#create_connection) - Create a connection
+* [delete_connection](docs/connections/README.md#delete_connection) - Delete a Connection
+* [get_connection](docs/connections/README.md#get_connection) - Get Connection details
+* [list_connections](docs/connections/README.md#list_connections) - List connections
 
-### destinations
+### [destinations](docs/destinations/README.md)
 
-* `create_destination` - Create a destination
-* `delete_destination` - Delete a Destination
-* `get_destination` - Get Destination details
-* `list_destinations` - List destinations
+* [create_destination](docs/destinations/README.md#create_destination) - Create a destination
+* [delete_destination](docs/destinations/README.md#delete_destination) - Delete a Destination
+* [get_destination](docs/destinations/README.md#get_destination) - Get Destination details
+* [list_destinations](docs/destinations/README.md#list_destinations) - List destinations
 
-### jobs
+### [jobs](docs/jobs/README.md)
 
-* `cancel_job` - Cancel a running Job
-* `create_job` - Trigger a sync or reset job of a connection
-* `get_job` - Get Job status and details
-* `list_jobs` - List Jobs by sync type
+* [cancel_job](docs/jobs/README.md#cancel_job) - Cancel a running Job
+* [create_job](docs/jobs/README.md#create_job) - Trigger a sync or reset job of a connection
+* [get_job](docs/jobs/README.md#get_job) - Get Job status and details
+* [list_jobs](docs/jobs/README.md#list_jobs) - List Jobs by sync type
 
-### sources
+### [sources](docs/sources/README.md)
 
-* `create_source` - Create a source
-* `delete_source` - Delete a Source
-* `get_source` - Get Source details
-* `initiate_o_auth` - Initiate OAuth for a source
-* `list_sources` - List sources
+* [create_source](docs/sources/README.md#create_source) - Create a source
+* [delete_source](docs/sources/README.md#delete_source) - Delete a Source
+* [get_source](docs/sources/README.md#get_source) - Get Source details
+* [initiate_o_auth](docs/sources/README.md#initiate_o_auth) - Initiate OAuth for a source
+* [list_sources](docs/sources/README.md#list_sources) - List sources
 
-### streams
+### [streams](docs/streams/README.md)
 
-* `get_stream_properties` - Get stream properties
+* [get_stream_properties](docs/streams/README.md#get_stream_properties) - Get stream properties
 
-### workspaces
+### [workspaces](docs/workspaces/README.md)
 
-* `create_or_update_workspace_o_auth_credentials` - Create OAuth override credentials for a workspace and source type.
-* `create_workspace` - Create a workspace
-* `get_workspace` - Get Workspace details
-* `list_workspaces` - List workspaces
+* [create_or_update_workspace_o_auth_credentials](docs/workspaces/README.md#create_or_update_workspace_o_auth_credentials) - Create OAuth override credentials for a workspace and source type.
+* [create_workspace](docs/workspaces/README.md#create_workspace) - Create a workspace
+* [get_workspace](docs/workspaces/README.md#get_workspace) - Get Workspace details
+* [list_workspaces](docs/workspaces/README.md#list_workspaces) - List workspaces
 <!-- End SDK Available Operations -->
 
 ### Maturity
 
 This SDK is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
 to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
 looking for the latest version.
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: airbyte-api Version: 0.1.0 Summary: Python Client
+Metadata-Version: 2.1 Name: airbyte-api Version: 0.3.0 Summary: Python Client
 SDK for Airbyte API Home-page: UNKNOWN Author: Airbyte License: UNKNOWN
 Platform: UNKNOWN Requires-Python: >=3.9 Description-Content-Type: text/
 markdown License-File: LICENSE.md
-  [https://user-images.githubusercontent.com/68016351/222853569-b35cc448-6481-
-                         4cf2-a237-bd5da47e94fd.png]
+ [https://user-images.githubusercontent.com/68016351/222853569-b35cc448-6481-
+                          4cf2-a237-bd5da47e94fd.png]
              Programatically control Airbyte Cloud through an API.
            [https://img.shields.io/static/v1?label=Docs&message=API
  Ref&color=000000&style=for-the-badge] [https://img.shields.io/github/actions/
                workflow/status/airbytehq/airbyte-api-python-sdk/
   speakeasy_sdk_generation.yml?style=for-the-badge] [https://img.shields.io/
 badge/License-MIT-blue.svg?style=for-the-badge] [https://img.shields.io/github/
   v/release/airbytehq/airbyte-api-python-sdk?sort=semver&style=for-the-badge]
@@ -15,53 +15,67 @@
 [Developer Portal](https://portal.airbyte.com/) to make API requests. You can
 use your existing Airbyte account to log in to the Developer Portal. Once you
 are in the Developer Portal, use the API Keys tab to create or remove API Keys.
 You can see a [walkthrough demo here](https://www.loom.com/share/
 7997a7c67cd642cc8d1c72ef0dfcc4bc)ð¦ The Developer Portal UI can also be used
 to help build your integration by showing information about network requests in
 the Requests tab. API usage information is also available to you in the Usage
-tab. ***(Installation will not work until published to a package manager,
-please clone locally and run `pip install -e ../path/to/local/clone` to try out
-the artifact locally)***  ## SDK Installation ```bash pip install airbyte-api
-```  ## SDK Example Usage  ```python import airbyte from airbyte.models import
-operations, shared s = airbyte.Airbyte( security=shared.Security
-( bearer_auth="Bearer YOUR_BEARER_TOKEN_HERE", ), ) req =
-shared.ConnectionCreateRequest( configurations=shared.StreamConfigurations
-( streams=[ shared.StreamConfiguration( cursor_field=[ "distinctio",
-"quibusdam", "unde", ], name="Johnnie Stamm", primary_key=[ [ "iure", "magnam",
-], [ "ipsa", "delectus", "tempora", "suscipit", ], [ "minus", "placeat", ], ],
+tab.  ## SDK Installation ```bash pip install airbyte-api ```  ## SDK Example
+Usage  ```python import airbyte from airbyte.models import shared s =
+airbyte.Airbyte( security=shared.Security( bearer_auth="Bearer
+YOUR_BEARER_TOKEN_HERE", ), ) req = shared.ConnectionCreateRequest
+( configurations=shared.StreamConfigurations( streams=
+[ shared.StreamConfiguration( cursor_field=[ "distinctio", "quibusdam", "unde",
+], name="Johnnie Stamm", primary_key=[ [ "iure", "magnam", ], [ "ipsa",
+"delectus", "tempora", "suscipit", ], [ "minus", "placeat", ], ],
 sync_mode="incremental_append", ), shared.StreamConfiguration( cursor_field=
 [ "excepturi", "nisi", ], name="Jake Bernier MD", primary_key=[
 [ "repellendus", "sapiente", ], ], sync_mode="incremental_deduped_history", ),
 shared.StreamConfiguration( cursor_field=[ "at", ], name="Emilio Krajcik",
 primary_key=[ [ "porro", "dolorum", "dicta", ], [ "officia", "occaecati",
 "fugit", ], ], sync_mode="incremental_append", ), ], ), data_residency="eu",
 destination_id="c816742c-b739-4205-9293-96fea7596eb1", name="Lela Orn",
 namespace_definition="source", namespace_format="${SOURCE_NAMESPACE}",
 prefix="dolorem", schedule=shared.ConnectionScheduleCreate
 ( cron_expression="corporis", schedule_type="manual", ), source_id="c5955907-
 aff1-4a3a-afa9-467739251aa5", ) res = s.connections.create_connection(req) if
 res.connection_response is not None: # handle response ```   ## Available
-Resources and Operations ### connections * `create_connection` - Create a
-connection * `delete_connection` - Delete a Connection * `get_connection` - Get
-Connection details * `list_connections` - List connections ### destinations *
-`create_destination` - Create a destination * `delete_destination` - Delete a
-Destination * `get_destination` - Get Destination details * `list_destinations`
-- List destinations ### jobs * `cancel_job` - Cancel a running Job *
-`create_job` - Trigger a sync or reset job of a connection * `get_job` - Get
-Job status and details * `list_jobs` - List Jobs by sync type ### sources *
-`create_source` - Create a source * `delete_source` - Delete a Source *
-`get_source` - Get Source details * `initiate_o_auth` - Initiate OAuth for a
-source * `list_sources` - List sources ### streams * `get_stream_properties` -
-Get stream properties ### workspaces *
-`create_or_update_workspace_o_auth_credentials` - Create OAuth override
-credentials for a workspace and source type. * `create_workspace` - Create a
-workspace * `get_workspace` - Get Workspace details * `list_workspaces` - List
-workspaces  ### Maturity This SDK is in beta, and there may be breaking changes
-between versions without a major version update. Therefore, we recommend
-pinning usage to a specific package version. This way, you can install the same
-version each time without breaking changes unless you are intentionally looking
-for the latest version. ### Contributions While we value open-source
-contributions to this SDK, this library is generated programmatically. Feel
-free to open a PR or a Github issue as a proof of concept and we'll do our best
-to include it in a future release ! ### SDK Created by [Speakeasy](https://
-docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
+Resources and Operations ### [connections](docs/connections/README.md) *
+[create_connection](docs/connections/README.md#create_connection) - Create a
+connection * [delete_connection](docs/connections/README.md#delete_connection)
+- Delete a Connection * [get_connection](docs/connections/
+README.md#get_connection) - Get Connection details * [list_connections](docs/
+connections/README.md#list_connections) - List connections ### [destinations]
+(docs/destinations/README.md) * [create_destination](docs/destinations/
+README.md#create_destination) - Create a destination * [delete_destination]
+(docs/destinations/README.md#delete_destination) - Delete a Destination *
+[get_destination](docs/destinations/README.md#get_destination) - Get
+Destination details * [list_destinations](docs/destinations/
+README.md#list_destinations) - List destinations ### [jobs](docs/jobs/
+README.md) * [cancel_job](docs/jobs/README.md#cancel_job) - Cancel a running
+Job * [create_job](docs/jobs/README.md#create_job) - Trigger a sync or reset
+job of a connection * [get_job](docs/jobs/README.md#get_job) - Get Job status
+and details * [list_jobs](docs/jobs/README.md#list_jobs) - List Jobs by sync
+type ### [sources](docs/sources/README.md) * [create_source](docs/sources/
+README.md#create_source) - Create a source * [delete_source](docs/sources/
+README.md#delete_source) - Delete a Source * [get_source](docs/sources/
+README.md#get_source) - Get Source details * [initiate_o_auth](docs/sources/
+README.md#initiate_o_auth) - Initiate OAuth for a source * [list_sources](docs/
+sources/README.md#list_sources) - List sources ### [streams](docs/streams/
+README.md) * [get_stream_properties](docs/streams/
+README.md#get_stream_properties) - Get stream properties ### [workspaces](docs/
+workspaces/README.md) * [create_or_update_workspace_o_auth_credentials](docs/
+workspaces/README.md#create_or_update_workspace_o_auth_credentials) - Create
+OAuth override credentials for a workspace and source type. *
+[create_workspace](docs/workspaces/README.md#create_workspace) - Create a
+workspace * [get_workspace](docs/workspaces/README.md#get_workspace) - Get
+Workspace details * [list_workspaces](docs/workspaces/
+README.md#list_workspaces) - List workspaces  ### Maturity This SDK is in beta,
+and there may be breaking changes between versions without a major version
+update. Therefore, we recommend pinning usage to a specific package version.
+This way, you can install the same version each time without breaking changes
+unless you are intentionally looking for the latest version. ### Contributions
+While we value open-source contributions to this SDK, this library is generated
+programmatically. Feel free to open a PR or a Github issue as a proof of
+concept and we'll do our best to include it in a future release ! ### SDK
+Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/
+client-sdks)
```

### Comparing `airbyte-api-0.1.0/src/airbyte_api.egg-info/SOURCES.txt` & `airbyte-api-0.3.0/src/airbyte_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

