# Comparing `tmp/awsibox-0.7.8.tar.gz` & `tmp/awsibox-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsibox-0.7.8.tar", last modified: Tue Mar 28 09:46:08 2023, max compression
+gzip compressed data, was "awsibox-0.8.0.tar", last modified: Thu Apr 27 10:31:11 2023, max compression
```

## Comparing `awsibox-0.7.8.tar` & `awsibox-0.8.0.tar`

### file list

```diff
@@ -1,257 +1,281 @@
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.070088 awsibox-0.7.8/
--rw-r--r--   0 mello     (1000) mello     (1000)      771 2020-01-23 17:57:57.000000 awsibox-0.7.8/.gitignore
--rw-r--r--   0 mello     (1000) mello     (1000)      193 2023-01-02 14:06:20.000000 awsibox-0.7.8/MANIFEST.in
--rw-r--r--   0 mello     (1000) mello     (1000)     1014 2023-03-28 09:46:08.074087 awsibox-0.7.8/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      373 2022-03-14 08:29:15.000000 awsibox-0.7.8/README.md
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:07.958088 awsibox-0.7.8/awsibox/
--rw-r--r--   0 mello     (1000) mello     (1000)    17629 2023-02-09 13:28:49.000000 awsibox-0.7.8/awsibox/RP.py
--rw-r--r--   0 mello     (1000) mello     (1000)       39 2023-03-28 09:45:54.000000 awsibox-0.7.8/awsibox/__init__.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2251 2022-07-01 08:39:37.000000 awsibox-0.7.8/awsibox/args.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3755 2023-02-20 15:00:23.000000 awsibox-0.7.8/awsibox/autoscaling.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:07.938089 awsibox-0.7.8/awsibox/cfg/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:07.990088 awsibox-0.7.8/awsibox/cfg/BASE/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:07.990088 awsibox-0.7.8/awsibox/cfg/BASE/AGW/
--rw-r--r--   0 mello     (1000) mello     (1000)     1761 2023-01-10 10:29:21.000000 awsibox-0.7.8/awsibox/cfg/BASE/AGW/TYPE.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2490 2023-01-14 16:47:50.000000 awsibox-0.7.8/awsibox/cfg/BASE/AGW/infra-info.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:07.990088 awsibox-0.7.8/awsibox/cfg/BASE/CCH/
--rw-r--r--   0 mello     (1000) mello     (1000)      352 2022-06-20 10:24:01.000000 awsibox-0.7.8/awsibox/cfg/BASE/CCH/TYPE.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:07.990088 awsibox-0.7.8/awsibox/cfg/BASE/CLF/
--rw-r--r--   0 mello     (1000) mello     (1000)       79 2022-06-14 09:03:16.000000 awsibox-0.7.8/awsibox/cfg/BASE/CLF/TYPE.yml
--rw-r--r--   0 mello     (1000) mello     (1000)  7094944 2022-12-27 15:33:59.000000 awsibox-0.7.8/awsibox/cfg/BASE/CloudFormationResourceSpecification.json
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:07.994088 awsibox-0.7.8/awsibox/cfg/BASE/EC2/
--rw-r--r--   0 mello     (1000) mello     (1000)     3366 2023-02-10 08:49:27.000000 awsibox-0.7.8/awsibox/cfg/BASE/EC2/TYPE.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     4567 2023-02-20 13:13:58.000000 awsibox-0.7.8/awsibox/cfg/BASE/EC2/ecs-cluster.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:07.994088 awsibox-0.7.8/awsibox/cfg/BASE/ECR/
--rw-r--r--   0 mello     (1000) mello     (1000)      180 2022-07-19 10:19:56.000000 awsibox-0.7.8/awsibox/cfg/BASE/ECR/TYPE.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:07.994088 awsibox-0.7.8/awsibox/cfg/BASE/ECS/
--rw-r--r--   0 mello     (1000) mello     (1000)     2482 2023-03-28 09:34:39.000000 awsibox-0.7.8/awsibox/cfg/BASE/ECS/TYPE.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      832 2023-02-13 13:15:07.000000 awsibox-0.7.8/awsibox/cfg/BASE/ECS/buildkite.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      599 2023-02-13 15:29:26.000000 awsibox-0.7.8/awsibox/cfg/BASE/ECS/reserve-cpu.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:07.998088 awsibox-0.7.8/awsibox/cfg/BASE/LBD/
--rw-r--r--   0 mello     (1000) mello     (1000)      177 2023-02-13 10:23:42.000000 awsibox-0.7.8/awsibox/cfg/BASE/LBD/TYPE.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1234 2022-12-22 13:20:48.000000 awsibox-0.7.8/awsibox/cfg/BASE/LBD/stacks-ops.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:07.998088 awsibox-0.7.8/awsibox/cfg/BASE/RDS/
--rw-r--r--   0 mello     (1000) mello     (1000)      255 2022-06-14 10:32:06.000000 awsibox-0.7.8/awsibox/cfg/BASE/RDS/TYPE.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.002088 awsibox-0.7.8/awsibox/cfg/BASE/RES/
--rw-r--r--   0 mello     (1000) mello     (1000)      177 2023-02-13 10:23:42.000000 awsibox-0.7.8/awsibox/cfg/BASE/RES/TYPE.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      587 2023-02-13 16:19:35.000000 awsibox-0.7.8/awsibox/cfg/BASE/RES/res-base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1522 2022-11-22 10:13:54.000000 awsibox-0.7.8/awsibox/cfg/BASE/RES/res-ccr-lighthouse.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      859 2022-12-22 09:16:31.000000 awsibox-0.7.8/awsibox/cfg/BASE/RES/res-ccr-stack-replicator.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3519 2023-02-14 08:52:19.000000 awsibox-0.7.8/awsibox/cfg/BASE/RES/res-ecs-alb.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      138 2022-03-14 08:29:15.000000 awsibox-0.7.8/awsibox/cfg/BASE/RES/res-event-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      522 2023-01-25 11:33:09.000000 awsibox-0.7.8/awsibox/cfg/BASE/RES/res-extra-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      910 2022-03-14 08:29:15.000000 awsibox-0.7.8/awsibox/cfg/BASE/RES/res-iam-group-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     4694 2022-06-22 15:09:44.000000 awsibox-0.7.8/awsibox/cfg/BASE/RES/res-iam-policy-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       90 2022-06-28 10:42:48.000000 awsibox-0.7.8/awsibox/cfg/BASE/RES/res-iam-user-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       62 2022-07-01 09:53:12.000000 awsibox-0.7.8/awsibox/cfg/BASE/RES/res-lambda-layer-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      679 2022-11-10 08:23:57.000000 awsibox-0.7.8/awsibox/cfg/BASE/RES/res-latedge-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       29 2022-03-17 16:27:10.000000 awsibox-0.7.8/awsibox/cfg/BASE/RES/res-s3-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2157 2022-10-03 13:17:24.000000 awsibox-0.7.8/awsibox/cfg/BASE/RES/vpc.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.006088 awsibox-0.7.8/awsibox/cfg/BASE/TSK/
--rw-r--r--   0 mello     (1000) mello     (1000)     2485 2023-03-27 08:42:44.000000 awsibox-0.7.8/awsibox/cfg/BASE/TSK/TYPE.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.006088 awsibox-0.7.8/awsibox/cfg/BASE/apigateway/
--rw-r--r--   0 mello     (1000) mello     (1000)      147 2022-06-12 14:13:51.000000 awsibox-0.7.8/awsibox/cfg/BASE/apigateway/account.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      250 2022-06-29 10:50:58.000000 awsibox-0.7.8/awsibox/cfg/BASE/apigateway/deployment.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      788 2022-06-25 09:21:43.000000 awsibox-0.7.8/awsibox/cfg/BASE/apigateway/domain-name.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1257 2022-06-29 10:50:57.000000 awsibox-0.7.8/awsibox/cfg/BASE/apigateway/stage.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.006088 awsibox-0.7.8/awsibox/cfg/BASE/application-autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)     2937 2023-01-25 10:47:28.000000 awsibox-0.7.8/awsibox/cfg/BASE/application-autoscaling/scalabletarget.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2802 2023-02-20 15:00:37.000000 awsibox-0.7.8/awsibox/cfg/BASE/application-autoscaling/scalingpolicy.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.014088 awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)     2400 2023-02-15 10:01:39.000000 awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/autoscalinggroup.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      534 2022-03-14 08:29:15.000000 awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/capacity.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      459 2023-01-14 17:03:55.000000 awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/cloudwatch-agent.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1253 2022-03-14 08:29:15.000000 awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/ephemeral.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1357 2022-03-14 08:29:15.000000 awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/imageid-ec2.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1303 2022-03-14 08:29:15.000000 awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/imageid-ecs.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     5121 2023-03-16 17:01:49.000000 awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/launchtemplate.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2303 2022-03-14 08:29:15.000000 awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/mixed_instances.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2478 2023-02-20 15:00:34.000000 awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/scalingpolicy.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2484 2023-02-06 09:33:25.000000 awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/scheduledactions.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2917 2023-01-27 13:30:51.000000 awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/spot-asg.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2206 2022-10-17 06:40:39.000000 awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/spot-auto.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.014088 awsibox-0.7.8/awsibox/cfg/BASE/cloudformation/
--rw-r--r--   0 mello     (1000) mello     (1000)      637 2023-03-20 14:26:15.000000 awsibox-0.7.8/awsibox/cfg/BASE/cloudformation/custom-resource_light-house.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.018088 awsibox-0.7.8/awsibox/cfg/BASE/cloudfront/
--rw-r--r--   0 mello     (1000) mello     (1000)      123 2022-12-29 11:38:54.000000 awsibox-0.7.8/awsibox/cfg/BASE/cloudfront/base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1521 2022-12-29 11:38:54.000000 awsibox-0.7.8/awsibox/cfg/BASE/cloudfront/custom-errors.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3796 2023-01-27 10:47:14.000000 awsibox-0.7.8/awsibox/cfg/BASE/cloudfront/distribution.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1661 2023-02-09 13:18:01.000000 awsibox-0.7.8/awsibox/cfg/BASE/cloudfront/for-services.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      405 2023-02-13 10:31:43.000000 awsibox-0.7.8/awsibox/cfg/BASE/cloudfront/function.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      520 2022-07-12 16:27:54.000000 awsibox-0.7.8/awsibox/cfg/BASE/cloudfront/lambda-function-associations.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      243 2022-08-19 14:24:27.000000 awsibox-0.7.8/awsibox/cfg/BASE/cloudfront/origin-access-identity.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      495 2023-01-10 10:22:43.000000 awsibox-0.7.8/awsibox/cfg/BASE/cloudfront/origin-adhoc.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     5958 2022-11-14 09:14:53.000000 awsibox-0.7.8/awsibox/cfg/BASE/cloudfront/policy.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.018088 awsibox-0.7.8/awsibox/cfg/BASE/cloudwatch/
--rw-r--r--   0 mello     (1000) mello     (1000)     8653 2023-03-21 10:23:23.000000 awsibox-0.7.8/awsibox/cfg/BASE/cloudwatch/alarms.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      966 2022-10-26 15:45:08.000000 awsibox-0.7.8/awsibox/cfg/BASE/cloudwatch/log_group.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.022088 awsibox-0.7.8/awsibox/cfg/BASE/codedeploy/
--rw-r--r--   0 mello     (1000) mello     (1000)     1509 2023-02-20 11:28:59.000000 awsibox-0.7.8/awsibox/cfg/BASE/codedeploy/deployment-group.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1240 2023-03-27 09:31:00.000000 awsibox-0.7.8/awsibox/cfg/BASE/common.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.022088 awsibox-0.7.8/awsibox/cfg/BASE/crm/
--rw-r--r--   0 mello     (1000) mello     (1000)       86 2022-03-18 08:09:10.000000 awsibox-0.7.8/awsibox/cfg/BASE/crm/certificate-global.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1271 2023-01-27 09:08:33.000000 awsibox-0.7.8/awsibox/cfg/BASE/crm/certificate-regional.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      222 2023-01-27 09:09:29.000000 awsibox-0.7.8/awsibox/cfg/BASE/crm/certificate.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.022088 awsibox-0.7.8/awsibox/cfg/BASE/dynamodb/
--rw-r--r--   0 mello     (1000) mello     (1000)      579 2022-06-10 07:33:46.000000 awsibox-0.7.8/awsibox/cfg/BASE/dynamodb/table-credstash.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.022088 awsibox-0.7.8/awsibox/cfg/BASE/ec2/
--rw-r--r--   0 mello     (1000) mello     (1000)     1975 2022-07-12 09:52:04.000000 awsibox-0.7.8/awsibox/cfg/BASE/ec2/bottlerocket.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      282 2023-01-25 14:20:56.000000 awsibox-0.7.8/awsibox/cfg/BASE/ec2/securitygroup.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      254 2022-06-13 09:15:13.000000 awsibox-0.7.8/awsibox/cfg/BASE/ec2/vpc-endpoint.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.026088 awsibox-0.7.8/awsibox/cfg/BASE/ecr/
--rw-r--r--   0 mello     (1000) mello     (1000)     1405 2022-07-19 10:34:24.000000 awsibox-0.7.8/awsibox/cfg/BASE/ecr/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.030088 awsibox-0.7.8/awsibox/cfg/BASE/ecs/
--rw-r--r--   0 mello     (1000) mello     (1000)     2452 2022-03-14 08:29:15.000000 awsibox-0.7.8/awsibox/cfg/BASE/ecs/capacityprovider.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1390 2023-02-13 15:29:53.000000 awsibox-0.7.8/awsibox/cfg/BASE/ecs/daemon-reserver-cpu.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3116 2023-02-13 15:30:18.000000 awsibox-0.7.8/awsibox/cfg/BASE/ecs/ecs-and-cluster.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     5209 2023-03-28 09:41:11.000000 awsibox-0.7.8/awsibox/cfg/BASE/ecs/ecs-containerdefinition.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1518 2023-03-27 10:38:42.000000 awsibox-0.7.8/awsibox/cfg/BASE/ecs/ecs-fargate-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      703 2023-02-07 09:04:07.000000 awsibox-0.7.8/awsibox/cfg/BASE/ecs/ecs-scheduled.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3349 2023-03-28 09:34:37.000000 awsibox-0.7.8/awsibox/cfg/BASE/ecs/ecs-service.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      976 2023-02-10 09:53:32.000000 awsibox-0.7.8/awsibox/cfg/BASE/ecs/ecs-task.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1986 2023-02-10 09:53:53.000000 awsibox-0.7.8/awsibox/cfg/BASE/ecs/ecs-taskdefinition.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     6804 2023-03-27 13:11:01.000000 awsibox-0.7.8/awsibox/cfg/BASE/ecs/service-elasticloadbalancing.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.030088 awsibox-0.7.8/awsibox/cfg/BASE/efs/
--rw-r--r--   0 mello     (1000) mello     (1000)      378 2022-03-14 08:29:15.000000 awsibox-0.7.8/awsibox/cfg/BASE/efs/accesspoint.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      528 2022-06-25 09:57:09.000000 awsibox-0.7.8/awsibox/cfg/BASE/efs/filesystem.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      387 2023-02-07 09:03:42.000000 awsibox-0.7.8/awsibox/cfg/BASE/efs/volume.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.030088 awsibox-0.7.8/awsibox/cfg/BASE/elasticache/
--rw-r--r--   0 mello     (1000) mello     (1000)     4819 2023-01-30 15:06:16.000000 awsibox-0.7.8/awsibox/cfg/BASE/elasticache/cluster-and-replication-group.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      385 2023-01-27 09:05:31.000000 awsibox-0.7.8/awsibox/cfg/BASE/elasticache/subnet-group.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.034088 awsibox-0.7.8/awsibox/cfg/BASE/elasticloadbalancing/
--rw-r--r--   0 mello     (1000) mello     (1000)     1287 2022-10-04 11:01:08.000000 awsibox-0.7.8/awsibox/cfg/BASE/elasticloadbalancing/accountid.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      232 2023-01-16 12:50:27.000000 awsibox-0.7.8/awsibox/cfg/BASE/elasticloadbalancing/base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2246 2023-01-22 13:56:42.000000 awsibox-0.7.8/awsibox/cfg/BASE/elasticloadbalancing/certificate-adhoc.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2686 2023-01-27 14:09:52.000000 awsibox-0.7.8/awsibox/cfg/BASE/elasticloadbalancing/classic-loadbalancer.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1945 2022-03-18 08:09:10.000000 awsibox-0.7.8/awsibox/cfg/BASE/elasticloadbalancing/hostedzoneid.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     4622 2023-01-28 16:10:58.000000 awsibox-0.7.8/awsibox/cfg/BASE/elasticloadbalancing/listener.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      248 2023-02-09 13:17:41.000000 awsibox-0.7.8/awsibox/cfg/BASE/elasticloadbalancing/loadbalancer.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3463 2023-03-27 13:12:04.000000 awsibox-0.7.8/awsibox/cfg/BASE/elasticloadbalancing/targetgroup.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1563 2023-03-27 12:17:22.000000 awsibox-0.7.8/awsibox/cfg/BASE/elasticloadbalancing/v2-listener-rule.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2831 2023-01-22 13:19:21.000000 awsibox-0.7.8/awsibox/cfg/BASE/elasticloadbalancing/v2-loadbalancer.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.038088 awsibox-0.7.8/awsibox/cfg/BASE/events/
--rw-r--r--   0 mello     (1000) mello     (1000)     1765 2023-02-10 11:02:08.000000 awsibox-0.7.8/awsibox/cfg/BASE/events/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.042088 awsibox-0.7.8/awsibox/cfg/BASE/iam/
--rw-r--r--   0 mello     (1000) mello     (1000)      435 2022-06-23 13:31:57.000000 awsibox-0.7.8/awsibox/cfg/BASE/iam/ecs-exec.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2287 2023-01-31 13:29:59.000000 awsibox-0.7.8/awsibox/cfg/BASE/iam/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      143 2022-06-23 14:38:31.000000 awsibox-0.7.8/awsibox/cfg/BASE/iam/instance-profile.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3687 2022-06-22 15:39:41.000000 awsibox-0.7.8/awsibox/cfg/BASE/iam/managed-policy.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      939 2022-06-23 13:32:27.000000 awsibox-0.7.8/awsibox/cfg/BASE/iam/parameterstore.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1716 2023-02-14 11:22:05.000000 awsibox-0.7.8/awsibox/cfg/BASE/iam/policy-bucket-replica.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2019 2022-06-23 13:31:22.000000 awsibox-0.7.8/awsibox/cfg/BASE/iam/policy-update_stack.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      918 2022-06-27 15:51:08.000000 awsibox-0.7.8/awsibox/cfg/BASE/iam/role.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2731 2022-06-22 15:23:21.000000 awsibox-0.7.8/awsibox/cfg/BASE/iam/ssm.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.042088 awsibox-0.7.8/awsibox/cfg/BASE/kms/
--rw-r--r--   0 mello     (1000) mello     (1000)      684 2022-06-22 14:34:38.000000 awsibox-0.7.8/awsibox/cfg/BASE/kms/key-and-alias.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.046088 awsibox-0.7.8/awsibox/cfg/BASE/lambda/
--rw-r--r--   0 mello     (1000) mello     (1000)      140 2022-10-26 15:14:56.000000 awsibox-0.7.8/awsibox/cfg/BASE/lambda/base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      653 2022-06-23 13:30:44.000000 awsibox-0.7.8/awsibox/cfg/BASE/lambda/ccr-fargate-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1286 2022-07-01 09:10:53.000000 awsibox-0.7.8/awsibox/cfg/BASE/lambda/function.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2149 2023-01-31 08:25:55.000000 awsibox-0.7.8/awsibox/cfg/BASE/lambda/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      213 2022-07-01 10:02:27.000000 awsibox-0.7.8/awsibox/cfg/BASE/lambda/layer_permission.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       46 2022-08-18 09:38:23.000000 awsibox-0.7.8/awsibox/cfg/BASE/lambda/layers.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      938 2023-01-31 09:57:07.000000 awsibox-0.7.8/awsibox/cfg/BASE/lambda/permission.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1187 2022-10-26 14:50:09.000000 awsibox-0.7.8/awsibox/cfg/BASE/lambda/service_unavailable.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      586 2023-02-16 16:16:57.000000 awsibox-0.7.8/awsibox/cfg/BASE/lambda/version.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.046088 awsibox-0.7.8/awsibox/cfg/BASE/rds/
--rw-r--r--   0 mello     (1000) mello     (1000)     6506 2022-06-29 15:23:08.000000 awsibox-0.7.8/awsibox/cfg/BASE/rds/db-instance.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      370 2022-06-20 16:35:35.000000 awsibox-0.7.8/awsibox/cfg/BASE/rds/db-subnet-group.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.050088 awsibox-0.7.8/awsibox/cfg/BASE/res-base/
--rw-r--r--   0 mello     (1000) mello     (1000)      225 2022-03-14 08:29:15.000000 awsibox-0.7.8/awsibox/cfg/BASE/res-base/cloudwatch_alarm.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3715 2022-11-29 16:03:45.000000 awsibox-0.7.8/awsibox/cfg/BASE/res-base/ecs_draininstance.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1376 2022-10-26 14:50:09.000000 awsibox-0.7.8/awsibox/cfg/BASE/res-base/ecs_runtask.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2317 2022-06-22 15:26:44.000000 awsibox-0.7.8/awsibox/cfg/BASE/res-base/iam-managed-policy.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1939 2023-01-31 13:37:14.000000 awsibox-0.7.8/awsibox/cfg/BASE/res-base/role.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      672 2023-01-25 11:33:20.000000 awsibox-0.7.8/awsibox/cfg/BASE/res-base/securitygroup_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      374 2022-03-14 08:29:15.000000 awsibox-0.7.8/awsibox/cfg/BASE/res-base/servicediscovery.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.050088 awsibox-0.7.8/awsibox/cfg/BASE/res-elasticloadbalancing/
--rw-r--r--   0 mello     (1000) mello     (1000)      194 2022-10-25 07:55:45.000000 awsibox-0.7.8/awsibox/cfg/BASE/res-elasticloadbalancing/v2-listener.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.054088 awsibox-0.7.8/awsibox/cfg/BASE/res-event/
--rw-r--r--   0 mello     (1000) mello     (1000)     1323 2023-01-31 09:25:05.000000 awsibox-0.7.8/awsibox/cfg/BASE/res-event/cluster-autoscale.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2936 2023-01-31 09:28:04.000000 awsibox-0.7.8/awsibox/cfg/BASE/res-event/event_cw-alarm.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     6798 2023-01-31 09:45:06.000000 awsibox-0.7.8/awsibox/cfg/BASE/res-event/event_ec2.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3903 2023-01-31 09:27:03.000000 awsibox-0.7.8/awsibox/cfg/BASE/res-event/event_ecs-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1551 2023-01-31 09:16:14.000000 awsibox-0.7.8/awsibox/cfg/BASE/res-event/event_ecs.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1186 2023-01-31 09:29:46.000000 awsibox-0.7.8/awsibox/cfg/BASE/res-event/spot_advisor.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.054088 awsibox-0.7.8/awsibox/cfg/BASE/res-extra/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2022-11-28 15:30:15.000000 awsibox-0.7.8/awsibox/cfg/BASE/res-extra/asgnotificationr53.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1591 2022-06-22 15:50:36.000000 awsibox-0.7.8/awsibox/cfg/BASE/res-extra/cloudformation_stackset.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      428 2022-09-20 08:00:03.000000 awsibox-0.7.8/awsibox/cfg/BASE/res-extra/route53_resolver.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.054088 awsibox-0.7.8/awsibox/cfg/BASE/res-s3/
--rw-r--r--   0 mello     (1000) mello     (1000)      513 2023-02-13 16:05:49.000000 awsibox-0.7.8/awsibox/cfg/BASE/res-s3/logs.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.054088 awsibox-0.7.8/awsibox/cfg/BASE/route53/
--rw-r--r--   0 mello     (1000) mello     (1000)     1666 2022-06-20 10:21:54.000000 awsibox-0.7.8/awsibox/cfg/BASE/route53/hostedzones.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     7683 2023-03-27 13:23:40.000000 awsibox-0.7.8/awsibox/cfg/BASE/route53/recordset.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.058088 awsibox-0.7.8/awsibox/cfg/BASE/s3/
--rw-r--r--   0 mello     (1000) mello     (1000)     2780 2022-08-24 08:32:36.000000 awsibox-0.7.8/awsibox/cfg/BASE/s3/bucket-policy.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     8088 2023-03-15 14:07:12.000000 awsibox-0.7.8/awsibox/cfg/BASE/s3/bucket.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.058088 awsibox-0.7.8/awsibox/cfg/BASE/scheduler/
--rw-r--r--   0 mello     (1000) mello     (1000)     1487 2023-02-10 11:02:19.000000 awsibox-0.7.8/awsibox/cfg/BASE/scheduler/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.058088 awsibox-0.7.8/awsibox/cfg/BASE/sns/
--rw-r--r--   0 mello     (1000) mello     (1000)      442 2022-11-28 09:14:29.000000 awsibox-0.7.8/awsibox/cfg/BASE/sns/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      719 2022-11-28 15:53:51.000000 awsibox-0.7.8/awsibox/cfg/BASE/sns/subscription.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.058088 awsibox-0.7.8/awsibox/cfg/BASE/sqs/
--rw-r--r--   0 mello     (1000) mello     (1000)      493 2022-11-29 09:59:21.000000 awsibox-0.7.8/awsibox/cfg/BASE/sqs/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      978 2022-11-24 08:26:20.000000 awsibox-0.7.8/awsibox/cfg/BASE/sqs/queue-policy.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.058088 awsibox-0.7.8/awsibox/cfg/BASE/ssm/
--rw-r--r--   0 mello     (1000) mello     (1000)      312 2022-06-28 11:51:39.000000 awsibox-0.7.8/awsibox/cfg/BASE/ssm/parameter.yml
--rw-r--r--   0 mello     (1000) mello     (1000)    16236 2023-03-20 14:16:50.000000 awsibox-0.7.8/awsibox/cfg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1661 2023-03-20 14:25:03.000000 awsibox-0.7.8/awsibox/cloudformation.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2324 2023-01-17 08:49:47.000000 awsibox-0.7.8/awsibox/cloudfront.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1526 2023-01-11 14:11:23.000000 awsibox-0.7.8/awsibox/common.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1936 2022-12-25 15:46:26.000000 awsibox-0.7.8/awsibox/discover.py
--rw-r--r--   0 mello     (1000) mello     (1000)    13204 2023-02-09 13:53:52.000000 awsibox-0.7.8/awsibox/ec2.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2357 2022-07-19 10:35:48.000000 awsibox-0.7.8/awsibox/ecr.py
--rw-r--r--   0 mello     (1000) mello     (1000)      922 2023-02-09 16:43:35.000000 awsibox-0.7.8/awsibox/ecs.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2878 2022-07-16 08:44:32.000000 awsibox-0.7.8/awsibox/efs.py
--rw-r--r--   0 mello     (1000) mello     (1000)     5303 2023-02-08 17:22:02.000000 awsibox-0.7.8/awsibox/elasticloadbalancing.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2418 2023-01-31 09:55:00.000000 awsibox-0.7.8/awsibox/generate.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3304 2022-08-15 19:24:28.000000 awsibox-0.7.8/awsibox/iam.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2753 2023-01-30 15:49:45.000000 awsibox-0.7.8/awsibox/joker.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.066088 awsibox-0.7.8/awsibox/lambdas/
--rw-r--r--   0 mello     (1000) mello     (1000)     1687 2022-03-14 08:29:15.000000 awsibox-0.7.8/awsibox/lambdas/ASGSpot.code
--rw-r--r--   0 mello     (1000) mello     (1000)      812 2022-03-14 08:29:15.000000 awsibox-0.7.8/awsibox/lambdas/AtEdgeAddHeaders.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2759 2022-11-22 10:02:17.000000 awsibox-0.7.8/awsibox/lambdas/CCRLightHouse.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2115 2022-11-22 13:27:14.000000 awsibox-0.7.8/awsibox/lambdas/CloudWatchAlarmStateChange.code
--rw-r--r--   0 mello     (1000) mello     (1000)     1675 2022-11-22 13:26:46.000000 awsibox-0.7.8/awsibox/lambdas/CloudWatchRepeatedNotify.code
--rw-r--r--   0 mello     (1000) mello     (1000)      739 2022-03-14 08:29:15.000000 awsibox-0.7.8/awsibox/lambdas/EC2StartStopTagged.code
--rwxr-xr-x   0 mello     (1000) mello     (1000)     6507 2022-11-30 10:37:32.000000 awsibox-0.7.8/awsibox/lambdas/ECSClusterAutoscale.code
--rw-r--r--   0 mello     (1000) mello     (1000)     6697 2022-11-29 16:18:45.000000 awsibox-0.7.8/awsibox/lambdas/ECSDrainInstance.code
--rw-r--r--   0 mello     (1000) mello     (1000)     7111 2022-11-30 10:51:36.000000 awsibox-0.7.8/awsibox/lambdas/ECSDrainTasks.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2899 2022-11-22 15:41:37.000000 awsibox-0.7.8/awsibox/lambdas/ECSEventTaskStateChange.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2792 2022-11-30 13:18:45.000000 awsibox-0.7.8/awsibox/lambdas/ECSRunTask.code
--rw-r--r--   0 mello     (1000) mello     (1000)      987 2022-03-14 08:29:15.000000 awsibox-0.7.8/awsibox/lambdas/ECSUpdateDesiredCount.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2167 2022-03-14 08:29:15.000000 awsibox-0.7.8/awsibox/lambdas/ElasticSearchSnapShot.code
--rw-r--r--   0 mello     (1000) mello     (1000)     1267 2022-04-23 16:11:28.000000 awsibox-0.7.8/awsibox/lambdas/ManageService.code
--rw-r--r--   0 mello     (1000) mello     (1000)      547 2022-03-14 08:29:15.000000 awsibox-0.7.8/awsibox/lambdas/PaidApi.code
--rw-r--r--   0 mello     (1000) mello     (1000)      844 2022-03-14 08:29:15.000000 awsibox-0.7.8/awsibox/lambdas/Python37SSM.layer
--rw-r--r--   0 mello     (1000) mello     (1000)     3826 2022-11-30 13:32:53.000000 awsibox-0.7.8/awsibox/lambdas/R53RecordInstanceId.code
--rw-r--r--   0 mello     (1000) mello     (1000)     4360 2022-11-30 14:07:17.000000 awsibox-0.7.8/awsibox/lambdas/ServiceDiscovery.code
--rw-r--r--   0 mello     (1000) mello     (1000)      890 2022-11-30 13:39:06.000000 awsibox-0.7.8/awsibox/lambdas/ServiceUnavailable.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2126 2022-12-22 11:51:40.000000 awsibox-0.7.8/awsibox/lambdas/StacksOps.code
--rw-r--r--   0 mello     (1000) mello     (1000)     3383 2022-03-18 08:09:10.000000 awsibox-0.7.8/awsibox/mappings.py
--rw-r--r--   0 mello     (1000) mello     (1000)     5917 2022-06-21 15:07:51.000000 awsibox-0.7.8/awsibox/rds.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2760 2023-02-13 17:05:21.000000 awsibox-0.7.8/awsibox/s3.py
--rw-r--r--   0 mello     (1000) mello     (1000)    45373 2023-03-27 10:25:32.000000 awsibox-0.7.8/awsibox/shared.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.066088 awsibox-0.7.8/awsibox/user-data/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.070088 awsibox-0.7.8/awsibox/user-data/SCRIPTS/
--rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-02 14:06:20.000000 awsibox-0.7.8/awsibox/user-data/SCRIPTS/ELBCHECK.sh
--rw-r--r--   0 mello     (1000) mello     (1000)      685 2023-02-28 14:52:11.000000 awsibox-0.7.8/awsibox/user-data/SCRIPTS/END.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1467 2023-01-03 11:25:14.000000 awsibox-0.7.8/awsibox/user-data/SCRIPTS/INIT.sh
--rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-05 16:57:15.000000 awsibox-0.7.8/awsibox/user-data/SCRIPTS/PACKAGE.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1184 2023-01-02 14:06:20.000000 awsibox-0.7.8/awsibox/user-data/SCRIPTS/SERVICE.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1771 2023-01-03 16:26:40.000000 awsibox-0.7.8/awsibox/user-data/SCRIPTS/SETUP.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     2521 2023-01-03 11:24:26.000000 awsibox-0.7.8/awsibox/user-data/ecs-cluster.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     7975 2022-03-14 08:29:15.000000 awsibox-0.7.8/awsibox/waf.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:07.938089 awsibox-0.7.8/build/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:07.938089 awsibox-0.7.8/build/lib/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:07.950088 awsibox-0.7.8/build/lib/awsibox.egg-info/
--rw-r--r--   0 mello     (1000) mello     (1000)     1014 2023-03-28 09:46:07.000000 awsibox-0.7.8/build/lib/awsibox.egg-info/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)     7807 2023-03-28 09:46:07.000000 awsibox-0.7.8/build/lib/awsibox.egg-info/SOURCES.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-03-28 09:46:07.000000 awsibox-0.7.8/build/lib/awsibox.egg-info/dependency_links.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       44 2023-03-28 09:46:07.000000 awsibox-0.7.8/build/lib/awsibox.egg-info/requires.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        8 2023-03-28 09:46:07.000000 awsibox-0.7.8/build/lib/awsibox.egg-info/top_level.txt
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-03-28 09:46:08.070088 awsibox-0.7.8/scripts/
--rwxr-xr-x   0 mello     (1000) mello     (1000)     3157 2022-12-27 15:22:06.000000 awsibox-0.7.8/scripts/ibox_generate_templates.py
--rw-r--r--   0 mello     (1000) mello     (1000)      556 2023-03-28 09:46:08.074087 awsibox-0.7.8/setup.cfg
--rw-r--r--   0 mello     (1000) mello     (1000)      481 2022-05-04 14:53:59.000000 awsibox-0.7.8/setup.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.125942 awsibox-0.8.0/
+-rw-r--r--   0 mello     (1000) mello     (1000)      771 2020-01-23 17:57:57.000000 awsibox-0.8.0/.gitignore
+-rw-r--r--   0 mello     (1000) mello     (1000)      225 2023-04-27 09:19:18.000000 awsibox-0.8.0/MANIFEST.in
+-rw-r--r--   0 mello     (1000) mello     (1000)     1014 2023-04-27 10:31:11.129942 awsibox-0.8.0/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      373 2022-03-14 08:29:15.000000 awsibox-0.8.0/README.md
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.025940 awsibox-0.8.0/awsibox/
+-rw-r--r--   0 mello     (1000) mello     (1000)    17889 2023-04-27 10:00:09.000000 awsibox-0.8.0/awsibox/RP.py
+-rw-r--r--   0 mello     (1000) mello     (1000)       39 2023-04-27 10:30:14.000000 awsibox-0.8.0/awsibox/__init__.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2251 2022-07-01 08:39:37.000000 awsibox-0.8.0/awsibox/args.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3755 2023-02-20 15:00:23.000000 awsibox-0.8.0/awsibox/autoscaling.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.025940 awsibox-0.8.0/awsibox/aws/
+-rw-r--r--   0 mello     (1000) mello     (1000)  7094944 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/aws/CloudFormationResourceSpecification.json
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.009940 awsibox-0.8.0/awsibox/cfg/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.013940 awsibox-0.8.0/awsibox/cfg/ibox/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.057941 awsibox-0.8.0/awsibox/cfg/ibox/com/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.061941 awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)      534 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/capacity.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      459 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/cloudwatch-agent.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1253 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1357 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1303 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2303 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2934 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2206 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.061941 awsibox-0.8.0/awsibox/cfg/ibox/com/certificatemanager/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1222 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.061941 awsibox-0.8.0/awsibox/cfg/ibox/com/cloudformation/
+-rw-r--r--   0 mello     (1000) mello     (1000)      637 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/cloudformation/custom-resource_light-house.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.065941 awsibox-0.8.0/awsibox/cfg/ibox/com/cloudfront/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1521 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1687 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/cloudfront/for-services.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      121 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/cloudfront/i_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      495 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/cloudfront/origin-adhoc.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.065941 awsibox-0.8.0/awsibox/cfg/ibox/com/codedeploy/
+-rw-r--r--   0 mello     (1000) mello     (1000)      190 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/codedeploy/deployment-group.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1811 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/common.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.065941 awsibox-0.8.0/awsibox/cfg/ibox/com/dynamodb/
+-rw-r--r--   0 mello     (1000) mello     (1000)      579 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.065941 awsibox-0.8.0/awsibox/cfg/ibox/com/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1975 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ec2/bottlerocket.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      265 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ec2/securitygroup.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      672 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.069941 awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2452 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/capacityprovider.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1398 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1518 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/fargate-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3140 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      703 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     6819 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      977 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/task.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      399 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/taskdefinition-volume.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.069941 awsibox-0.8.0/awsibox/cfg/ibox/com/efs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      378 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/efs/accesspoint-app.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.073941 awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1287 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2246 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1945 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      365 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/i_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      251 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/loadbalancer.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      194 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/v2-listener.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.073941 awsibox-0.8.0/awsibox/cfg/ibox/com/events/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2892 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1340 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/events/cluster-autoscale.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     6914 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/events/ec2.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1581 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2584 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/events/ecs-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1570 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/events/ecs.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1203 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/events/spot_advisor.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.077941 awsibox-0.8.0/awsibox/cfg/ibox/com/iam/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5020 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/iam/managed-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1716 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/iam/policy-bucket-replica.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      435 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/iam/policy-ecs-exec.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      939 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2067 2023-04-27 10:06:22.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/iam/policy-update_stack.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1591 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1939 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/iam/roles.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.077941 awsibox-0.8.0/awsibox/cfg/ibox/com/kms/
+-rw-r--r--   0 mello     (1000) mello     (1000)      684 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.081941 awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/
+-rw-r--r--   0 mello     (1000) mello     (1000)      607 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3732 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1393 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      165 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/i_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       46 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/layers.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      935 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/py-packager.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1204 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/service-unavailable.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.081941 awsibox-0.8.0/awsibox/cfg/ibox/com/route53/
+-rw-r--r--   0 mello     (1000) mello     (1000)      428 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/route53/resolverendpoint-outbound.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.081941 awsibox-0.8.0/awsibox/cfg/ibox/com/s3/
+-rw-r--r--   0 mello     (1000) mello     (1000)      513 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/s3/bucket-log.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.081941 awsibox-0.8.0/awsibox/cfg/ibox/com/servicediscovery/
+-rw-r--r--   0 mello     (1000) mello     (1000)      374 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/servicediscovery/publicdnsnamespace-find.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.081941 awsibox-0.8.0/awsibox/cfg/ibox/com/sns/
+-rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      225 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/sns/cloudwatch-alarm.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.081941 awsibox-0.8.0/awsibox/cfg/ibox/com/ssm/
+-rw-r--r--   0 mello     (1000) mello     (1000)      312 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/com/ssm/parameter-user-password.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.013940 awsibox-0.8.0/awsibox/cfg/ibox/res/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.085941 awsibox-0.8.0/awsibox/cfg/ibox/res/apigateway/
+-rw-r--r--   0 mello     (1000) mello     (1000)      147 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/apigateway/accounts.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      250 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/apigateway/deployments.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      491 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/apigateway/domain-names.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1764 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/apigateway/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.085941 awsibox-0.8.0/awsibox/cfg/ibox/res/application-autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)      706 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2937 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2143 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.085941 awsibox-0.8.0/awsibox/cfg/ibox/res/autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2442 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3101 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5137 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1889 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.085941 awsibox-0.8.0/awsibox/cfg/ibox/res/certificatemanager/
+-rw-r--r--   0 mello     (1000) mello     (1000)      222 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/certificatemanager/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.089941 awsibox-0.8.0/awsibox/cfg/ibox/res/cloudfront/
+-rw-r--r--   0 mello     (1000) mello     (1000)     4759 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      243 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/cloudfront/origin-access-identities.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5958 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/cloudfront/policies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.089941 awsibox-0.8.0/awsibox/cfg/ibox/res/cloudwatch/
+-rw-r--r--   0 mello     (1000) mello     (1000)     7727 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/cloudwatch/alarms.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      955 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      966 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.089941 awsibox-0.8.0/awsibox/cfg/ibox/res/codedeploy/
+-rw-r--r--   0 mello     (1000) mello     (1000)      426 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/codedeploy/deployment-groups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1018 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.089941 awsibox-0.8.0/awsibox/cfg/ibox/res/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)      160 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/ec2/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      118 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/ec2/vpc-endpoints.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.093942 awsibox-0.8.0/awsibox/cfg/ibox/res/ecr/
+-rw-r--r--   0 mello     (1000) mello     (1000)      136 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/ecr/accounts.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1405 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/ecr/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.093942 awsibox-0.8.0/awsibox/cfg/ibox/res/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)     6608 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/ecs/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1964 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/ecs/services.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1986 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.093942 awsibox-0.8.0/awsibox/cfg/ibox/res/efs/
+-rw-r--r--   0 mello     (1000) mello     (1000)       68 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/efs/filesystems.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      561 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/efs/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.093942 awsibox-0.8.0/awsibox/cfg/ibox/res/elasticache/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5166 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/elasticache/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       69 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/elasticache/subnet-groups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.097942 awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/
+-rw-r--r--   0 mello     (1000) mello     (1000)     3972 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     4552 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/listeners.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1002 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2831 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2920 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.097942 awsibox-0.8.0/awsibox/cfg/ibox/res/events/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1765 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/events/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.097942 awsibox-0.8.0/awsibox/cfg/ibox/res/iam/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2287 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/iam/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      143 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/iam/instance-profiles.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3687 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/iam/managed-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      918 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/iam/roles.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.101942 awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1286 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/functions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2300 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      213 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/layer_permissions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      938 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/permissions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      586 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/versions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.101942 awsibox-0.8.0/awsibox/cfg/ibox/res/rds/
+-rw-r--r--   0 mello     (1000) mello     (1000)      393 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/rds/db-subnet-groups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     7723 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/rds/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.101942 awsibox-0.8.0/awsibox/cfg/ibox/res/route53/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1427 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/route53/hostedzones.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      357 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/route53/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     7683 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/route53/recordsets.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.101942 awsibox-0.8.0/awsibox/cfg/ibox/res/s3/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2808 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/s3/bucket-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     8101 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/s3/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.101942 awsibox-0.8.0/awsibox/cfg/ibox/res/scheduler/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1487 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/scheduler/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.105942 awsibox-0.8.0/awsibox/cfg/ibox/res/sns/
+-rw-r--r--   0 mello     (1000) mello     (1000)      397 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/sns/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      719 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/sns/subscriptions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.105942 awsibox-0.8.0/awsibox/cfg/ibox/res/sqs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      467 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/sqs/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      978 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/res/sqs/queue-policies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.013940 awsibox-0.8.0/awsibox/cfg/ibox/stacks/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.105942 awsibox-0.8.0/awsibox/cfg/ibox/stacks/agw/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1751 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/agw/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2612 2023-04-27 10:02:55.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/agw/infra-info.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.105942 awsibox-0.8.0/awsibox/cfg/ibox/stacks/cch/
+-rw-r--r--   0 mello     (1000) mello     (1000)      311 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/cch/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.105942 awsibox-0.8.0/awsibox/cfg/ibox/stacks/clf/
+-rw-r--r--   0 mello     (1000) mello     (1000)       89 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/clf/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.105942 awsibox-0.8.0/awsibox/cfg/ibox/stacks/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)     4591 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3433 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/ec2/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.109942 awsibox-0.8.0/awsibox/cfg/ibox/stacks/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      846 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/ecs/buildkite.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2510 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/ecs/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      621 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.109942 awsibox-0.8.0/awsibox/cfg/ibox/stacks/lbd/
+-rw-r--r--   0 mello     (1000) mello     (1000)      144 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/lbd/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1291 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.109942 awsibox-0.8.0/awsibox/cfg/ibox/stacks/rds/
+-rw-r--r--   0 mello     (1000) mello     (1000)      240 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/rds/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.113942 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/
+-rw-r--r--   0 mello     (1000) mello     (1000)      144 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      633 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1543 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      794 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3527 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      139 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-event-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      595 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-extra-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      910 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     4700 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      108 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-iam-user-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       67 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-lambda-layer-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      655 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       29 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-s3-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2157 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/vpc.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.113942 awsibox-0.8.0/awsibox/cfg/ibox/stacks/tsk/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2490 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/cfg/ibox/stacks/tsk/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)    16432 2023-04-27 10:25:15.000000 awsibox-0.8.0/awsibox/cfg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1661 2023-03-20 14:25:03.000000 awsibox-0.8.0/awsibox/cloudformation.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2324 2023-01-17 08:49:47.000000 awsibox-0.8.0/awsibox/cloudfront.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1685 2023-04-17 10:03:18.000000 awsibox-0.8.0/awsibox/common.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1867 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/discover.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    13204 2023-02-09 13:53:52.000000 awsibox-0.8.0/awsibox/ec2.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2402 2023-04-27 09:19:18.000000 awsibox-0.8.0/awsibox/ecr.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      922 2023-02-09 16:43:35.000000 awsibox-0.8.0/awsibox/ecs.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2878 2022-07-16 08:44:32.000000 awsibox-0.8.0/awsibox/efs.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     5303 2023-02-08 17:22:02.000000 awsibox-0.8.0/awsibox/elasticloadbalancing.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2418 2023-04-17 07:28:21.000000 awsibox-0.8.0/awsibox/generate.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3369 2023-04-14 07:54:55.000000 awsibox-0.8.0/awsibox/iam.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2784 2023-04-11 16:23:54.000000 awsibox-0.8.0/awsibox/joker.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.125942 awsibox-0.8.0/awsibox/lambdas/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1687 2022-03-14 08:29:15.000000 awsibox-0.8.0/awsibox/lambdas/ASGSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      812 2022-03-14 08:29:15.000000 awsibox-0.8.0/awsibox/lambdas/AtEdgeAddHeaders.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4293 2023-04-11 07:34:58.000000 awsibox-0.8.0/awsibox/lambdas/CCRFargateSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2759 2022-11-22 10:02:17.000000 awsibox-0.8.0/awsibox/lambdas/CCRLightHouse.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     3916 2023-04-11 07:35:07.000000 awsibox-0.8.0/awsibox/lambdas/CCRStackReplicator.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2115 2022-11-22 13:27:14.000000 awsibox-0.8.0/awsibox/lambdas/CloudWatchAlarmStateChange.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     1675 2022-11-22 13:26:46.000000 awsibox-0.8.0/awsibox/lambdas/CloudWatchRepeatedNotify.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      739 2022-03-14 08:29:15.000000 awsibox-0.8.0/awsibox/lambdas/EC2StartStopTagged.code
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     6507 2022-11-30 10:37:32.000000 awsibox-0.8.0/awsibox/lambdas/ECSClusterAutoscale.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     6697 2022-11-29 16:18:45.000000 awsibox-0.8.0/awsibox/lambdas/ECSDrainInstance.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     7111 2023-04-17 15:59:09.000000 awsibox-0.8.0/awsibox/lambdas/ECSDrainTasks.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2899 2022-11-22 15:41:37.000000 awsibox-0.8.0/awsibox/lambdas/ECSEventTaskStateChange.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4193 2023-04-12 09:41:12.000000 awsibox-0.8.0/awsibox/lambdas/ECSEventsSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     6177 2023-04-12 10:46:40.000000 awsibox-0.8.0/awsibox/lambdas/ECSRaiseASGAlarm.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2792 2022-11-30 13:18:45.000000 awsibox-0.8.0/awsibox/lambdas/ECSRunTask.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      987 2022-03-14 08:29:15.000000 awsibox-0.8.0/awsibox/lambdas/ECSUpdateDesiredCount.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2167 2022-03-14 08:29:15.000000 awsibox-0.8.0/awsibox/lambdas/ElasticSearchSnapShot.code
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     5132 2023-04-12 16:00:53.000000 awsibox-0.8.0/awsibox/lambdas/InfraInfo.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     1267 2022-04-23 16:11:28.000000 awsibox-0.8.0/awsibox/lambdas/ManageService.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      547 2022-03-14 08:29:15.000000 awsibox-0.8.0/awsibox/lambdas/PaidApi.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2724 2023-04-07 09:45:45.000000 awsibox-0.8.0/awsibox/lambdas/PyPackager.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      844 2022-03-14 08:29:15.000000 awsibox-0.8.0/awsibox/lambdas/Python37SSM.layer
+-rw-r--r--   0 mello     (1000) mello     (1000)     3826 2022-11-30 13:32:53.000000 awsibox-0.8.0/awsibox/lambdas/R53RecordInstanceId.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4360 2022-11-30 14:07:17.000000 awsibox-0.8.0/awsibox/lambdas/ServiceDiscovery.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      890 2022-11-30 13:39:06.000000 awsibox-0.8.0/awsibox/lambdas/ServiceUnavailable.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2126 2022-12-22 11:51:40.000000 awsibox-0.8.0/awsibox/lambdas/StacksOps.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     3383 2022-03-18 08:09:10.000000 awsibox-0.8.0/awsibox/mappings.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     5917 2022-06-21 15:07:51.000000 awsibox-0.8.0/awsibox/rds.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2760 2023-02-13 17:05:21.000000 awsibox-0.8.0/awsibox/s3.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    45456 2023-04-17 09:53:49.000000 awsibox-0.8.0/awsibox/shared.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.125942 awsibox-0.8.0/awsibox/user-data/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.125942 awsibox-0.8.0/awsibox/user-data/SCRIPTS/
+-rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-02 14:06:20.000000 awsibox-0.8.0/awsibox/user-data/SCRIPTS/ELBCHECK.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)      685 2023-02-28 14:52:11.000000 awsibox-0.8.0/awsibox/user-data/SCRIPTS/END.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1467 2023-01-03 11:25:14.000000 awsibox-0.8.0/awsibox/user-data/SCRIPTS/INIT.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-05 16:57:15.000000 awsibox-0.8.0/awsibox/user-data/SCRIPTS/PACKAGE.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1184 2023-01-02 14:06:20.000000 awsibox-0.8.0/awsibox/user-data/SCRIPTS/SERVICE.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1771 2023-01-03 16:26:40.000000 awsibox-0.8.0/awsibox/user-data/SCRIPTS/SETUP.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     2521 2023-01-03 11:24:26.000000 awsibox-0.8.0/awsibox/user-data/ecs-cluster.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     7975 2022-03-14 08:29:15.000000 awsibox-0.8.0/awsibox/waf.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.009940 awsibox-0.8.0/build/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.009940 awsibox-0.8.0/build/lib/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.017940 awsibox-0.8.0/build/lib/awsibox.egg-info/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1014 2023-04-27 10:31:10.000000 awsibox-0.8.0/build/lib/awsibox.egg-info/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)     8974 2023-04-27 10:31:10.000000 awsibox-0.8.0/build/lib/awsibox.egg-info/SOURCES.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-04-27 10:31:10.000000 awsibox-0.8.0/build/lib/awsibox.egg-info/dependency_links.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       44 2023-04-27 10:31:10.000000 awsibox-0.8.0/build/lib/awsibox.egg-info/requires.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        8 2023-04-27 10:31:10.000000 awsibox-0.8.0/build/lib/awsibox.egg-info/top_level.txt
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-04-27 10:31:11.125942 awsibox-0.8.0/scripts/
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     3177 2023-04-27 09:19:18.000000 awsibox-0.8.0/scripts/ibox_generate_templates.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      556 2023-04-27 10:31:11.129942 awsibox-0.8.0/setup.cfg
+-rw-r--r--   0 mello     (1000) mello     (1000)      506 2023-04-27 09:19:18.000000 awsibox-0.8.0/setup.py
```

### Comparing `awsibox-0.7.8/.gitignore` & `awsibox-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/PKG-INFO` & `awsibox-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsibox
-Version: 0.7.8
+Version: 0.8.0
 Summary: AWS Infrastructure in a Box
 Home-page: https://github.com/mello7tre/AwsIBox
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBox
         AwsIBox - **AWS** **I**nfrastructure in a **Box**
```

### Comparing `awsibox-0.7.8/awsibox/RP.py` & `awsibox-0.8.0/awsibox/RP.py`

 * *Files 14% similar despite different names*

```diff
@@ -85,37 +85,32 @@
 
         return RP_base_keys + [stacktype, envrole]
 
     RP_base_keys = _get_RP_base_keys()
 
     class Loader(yaml.Loader):
         def __init__(self, stream):
-            # This way for include relative to file with include statement
-            self._root_current = os.path.split(stream.name)[0]
-            # This way for include BASE relative on BASE dir
-            self._root_base = os.path.join(CFG_FILE_INT, "BASE")
-            # This way for include relative on BASE EXT dir
-            self._root_base_ext = os.path.join(CFG_FILE_EXT, "BASE")
+            #            # This way for include relative to file with include statement
+            #            self._root_current = os.path.split(stream.name)[0]
+            # This way for include relative on ibox dir
+            self._root_base = os.path.join(CFG_FILE_INT, cfg.IBOX_BRAND_DIR)
+            # This way for include relative on ibox EXT dir
+            self._root_base_ext = os.path.join(CFG_FILE_EXT, cfg.IBOX_BRAND_DIR)
             # This way for include relative on brand EXT dir
             self._root_brand_ext = os.path.join(CFG_FILE_EXT, brand)
 
-            # try to find out if source file is in a subfolder
-            if self._root_base in self._root_current:
-                suffix = self._root_current.replace(self._root_base, "")
-            elif self._root_base_ext in self._root_current:
-                suffix = self._root_current.replace(self._root_base_ext, "")
-            else:
-                suffix = self._root_current.replace(self._root_brand_ext, "")
-
-            # self.root_current_suffix will be empty if source file is in root
-            self.root_current_suffix = os.path.basename(suffix)
-            if self.root_current_suffix.upper() in cfg.STACK_TYPES:
-                # set to empty even if UPPERCASE subfolders is in
-                # cfg.STACK_TYPES to not be searched for include files
-                self.root_current_suffix = ""
+            #            # find out suffix to use for file included withouth a path (no more used)
+            #            if self._root_base in self._root_current:
+            #                suffix = self._root_current.replace(self._root_base, "")
+            #            elif self._root_base_ext in self._root_current:
+            #                suffix = self._root_current.replace(self._root_base_ext, "")
+            #            else:
+            #                suffix = self._root_current.replace(self._root_brand_ext, "")
+            #
+            #            self.root_current_suffix = os.path.basename(suffix)
 
             self.stream = stream
             super(Loader, self).__init__(stream)
             Loader.add_constructor("!include", Loader.include)
             Loader.add_constructor("!exclude", Loader.exclude)
 
         def exclude(self, node):
@@ -134,18 +129,17 @@
 
                     # search for include in files in roots
                     for path in [
                         self._root_base,
                         self._root_base_ext,
                         self._root_brand_ext,
                     ]:
-                        if "/" not in filename and self.root_current_suffix:
-                            # for file in subfolder that include file without a path
-                            # search only in current subfolder
-                            path = os.path.join(path, self.root_current_suffix)
+                        #                        if "/" not in filename:
+                        #                            # for include without a path search only in current subfolder
+                        #                            path = os.path.join(path, self.root_current_suffix)
 
                         contents = self.extractFile(filename, path)
                         if contents:
                             result.append(contents)
                 return result
             else:
                 print("Error:: unrecognised node type in !include statement")
@@ -258,16 +252,16 @@
                         _process(m, w, RP)
             else:
                 RP = data
             return RP
 
         return _recurse(data)
 
-    def read_yaml(file_type, brand, base_dir, stacktype=""):
-        cfg_file = os.path.join(base_dir, brand, stacktype.upper(), f"{file_type}.yml")
+    def read_yaml(file_type, brand, base_dir, stacktype="", prefix=""):
+        cfg_file = os.path.join(base_dir, brand, prefix, stacktype, f"{file_type}.yml")
 
         try:
             with open(cfg_file, "r") as ymlfile:
                 cfg = yaml.load(ymlfile, Loader=Loader)
 
                 return cfg
         except IOError:
@@ -399,29 +393,41 @@
 
         return RP_tree, RP_map
 
     # End inner methods and begin of main code.
 
     # envrole type files must be read first
     yaml_role = [
-        read_yaml(envrole, "BASE", CFG_FILE_INT, stacktype),
-        read_yaml(envrole, "BASE", CFG_FILE_EXT, stacktype),
-        read_yaml(envrole, brand, CFG_FILE_EXT, stacktype),
+        read_yaml(envrole, cfg.IBOX_BRAND_DIR, CFG_FILE_INT, stacktype, cfg.STACKS_DIR),
+        read_yaml(envrole, cfg.IBOX_BRAND_DIR, CFG_FILE_EXT, stacktype, cfg.STACKS_DIR),
+        read_yaml(envrole, brand, CFG_FILE_EXT, stacktype, cfg.STACKS_DIR),
     ]
 
     yaml_cfg = {
         "common": [
-            read_yaml("common", "BASE", CFG_FILE_INT),
-            read_yaml("common", "BASE", CFG_FILE_EXT),
-            read_yaml("common", brand, CFG_FILE_EXT),
+            read_yaml("common", cfg.IBOX_BRAND_DIR, CFG_FILE_INT, prefix="com"),
+            read_yaml("common", cfg.IBOX_BRAND_DIR, CFG_FILE_EXT, prefix="com"),
+            read_yaml("common", brand, CFG_FILE_EXT, prefix="com"),
         ],
         "type": [
-            read_yaml("TYPE", "BASE", CFG_FILE_INT, stacktype),
-            read_yaml("TYPE", "BASE", CFG_FILE_EXT, stacktype),
-            read_yaml("TYPE", brand, CFG_FILE_EXT, stacktype),
+            read_yaml(
+                "i_type",
+                cfg.IBOX_BRAND_DIR,
+                CFG_FILE_INT,
+                stacktype,
+                cfg.STACKS_DIR,
+            ),
+            read_yaml(
+                "i_type",
+                cfg.IBOX_BRAND_DIR,
+                CFG_FILE_EXT,
+                stacktype,
+                cfg.STACKS_DIR,
+            ),
+            read_yaml("i_type", brand, CFG_FILE_EXT, stacktype, cfg.STACKS_DIR),
         ],
         "role": yaml_role,
     }
 
     cfg.RP_tree, cfg.RP_map = get_RP(yaml_cfg)
 
     if cfg.debug:
```

### Comparing `awsibox-0.7.8/awsibox/args.py` & `awsibox-0.8.0/awsibox/args.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/autoscaling.py` & `awsibox-0.8.0/awsibox/autoscaling.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/AGW/TYPE.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/stacks/agw/i_type.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 IBoxLoader: !include
-  - apigateway/stage.yml
-  - apigateway/deployment.yml
-  - cloudfront/for-services.yml
-  - lambda/base.yml
+  - res/apigateway/deployments.yml
+  - com/cloudfront/for-services.yml
+  - com/lambda/i_base.yml
 
 global:
   Output:
     - InvokeUrl:
         Value: Sub('https://${ApiGatewayRestApi}.execute-api.${AWS::Region}.amazonaws.com/%s' % cfg.ApiGatewayRestApi['Base']['Stage'])
   ApiGatewayRestApi:
     - Base:
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/AGW/infra-info.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/stacks/agw/infra-info.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 IBoxLoader:
+  - !include
+    - com/lambda/layers.yml
   - !exclude
-    - cloudfront/for-services.yml
+    - com/cloudfront/for-services.yml
 
 global:
   StackName: iif
   ApiGatewayRestApi:
     - Base:
         Description: 'Infrastracture Informations'
         Name: 'InfraInfo'
@@ -57,22 +59,26 @@
         Roles:
           - Ref('RoleLambdaInfraInfov1')
         PolicyDocument:
           Statement:
             - 1:
                 Action:
                   - 'cloudformation:DescribeStack*'
+                  - 'cloudformation:ListStacks'
                   - 'ecs:ListClusters'
                   - 'ecs:ListServices'
                   - 'ecs:DescribeServices'
                   - 'application-autoscaling:DescribeScalableTargets'
                 Effect: Allow
                 Resource: '*'
   Lambda:
     - InfraInfov1:
+        Architectures:
+          - arm64
         Code:
-          S3Bucket: Sub(cfg.BucketNameAppRepository)
-          S3Key: 'ibox-tools/infra-info/infra-info-01.zip'
+          ZipFile: InfraInfo
         Description: 'Infrastracture Informations'
-        MemorySize: 128
+        Layers:
+          - LambdaLayerVersionPythonArm64IboxStacksOps
+        MemorySize: 512
         Runtime: python3.9
         Timeout: 60
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/CloudFormationResourceSpecification.json` & `awsibox-0.8.0/awsibox/aws/CloudFormationResourceSpecification.json`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/EC2/TYPE.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/stacks/ec2/i_type.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 IBoxLoader: !include
-  - autoscaling/autoscalinggroup.yml
-  - elasticloadbalancing/loadbalancer.yml
-  - ec2/securitygroup.yml
-  - cloudwatch/alarms.yml
-  - cloudfront/for-services.yml
-  - iam/parameterstore.yml
-  - iam/instance-profile.yml
-  - sns/subscription.yml
-  - sqs/queue-policy.yml
-  - lambda/base.yml
-  - iam/role.yml
+  - res/autoscaling/autoscalinggroups.yml
+  - com/elasticloadbalancing/loadbalancer.yml
+  - com/ec2/securitygroup.yml
+  - res/cloudwatch/alarms.yml
+  - com/cloudfront/for-services.yml
+  - com/iam/policy-parameterstore.yml
+  - res/iam/instance-profiles.yml
+  - res/sns/subscriptions.yml
+  - res/sqs/queue-policies.yml
+  - com/lambda/i_base.yml
+  - res/iam/roles.yml
 
 global:
   Parameter:
     - UpdateMode:
         Description: 'How to update Instances'
         AllowedValues: ['none', 'Replace', 'Rolling']
         Default: 'none'
@@ -112,9 +112,9 @@
 stg: *cfg_dev 
 
 
 prd:
   #AutoScalingGroupBaseHealthCheckType: ELB
 
 IBoxLoaderAfter: !include
-  - autoscaling/spot-auto.yml
-  - autoscaling/cloudwatch-agent.yml
+  - com/autoscaling/spot-auto.yml
+  - com/autoscaling/cloudwatch-agent.yml
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/EC2/ecs-cluster.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 IBoxLoader: 
   - !exclude
-      - cloudfront/for-services.yml
-      - elasticloadbalancing/loadbalancer.yml
+      - com/cloudfront/for-services.yml
+      - com/elasticloadbalancing/loadbalancer.yml
   - !include
-      #- autoscaling/imageid-ecs.yml
-      - ecs/capacityprovider.yml
-      - ecs/daemon-reserver-cpu.yml
-      - ec2/bottlerocket.yml
+      #- com/autoscaling/imageid-ecs.yml
+      - com/ecs/capacityprovider.yml
+      - com/ecs/daemon-reserver-cpu.yml
+      - com/ec2/bottlerocket.yml
 
 global:
   StackName: ecs
   Parameter:
     - GPUInstance:
         Description: 'Install Coda and nvidia-docker2'
         AllowedValues: ['yes', 'no']
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/ECS/TYPE.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/stacks/ecs/i_type.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 IBoxLoader: !include
-  - autoscaling/capacity.yml
-  - application-autoscaling/scalingpolicy.yml
-  - application-autoscaling/scalabletarget.yml
-  - cloudwatch/alarms.yml
-  - ecs/ecs-task.yml
-  - ecs/ecs-service.yml
-  - ecs/service-elasticloadbalancing.yml
+  - com/autoscaling/capacity.yml
+  - res/application-autoscaling/scalingpolicies.yml
+  - res/application-autoscaling/scalabletargets.yml
+  - res/cloudwatch/alarms.yml
+  - com/ecs/task.yml
+  - res/ecs/services.yml
+  - com/ecs/service-elasticloadbalancing.yml
 
 global:
   ApplicationAutoScalingScalableTarget:
     - ECSService:
         ScheduledActions:
           - Down:
               Enabled: 'no'
@@ -74,9 +74,9 @@
     Up:
       Enabled: 'yes'
 
 stg: *cfg_dev
 
 
 IBoxLoaderAfter: !include [
-  #ecs-fargate-spot.yml,
+  #com/ecs/fargate-spot.yml,
 ]
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/ECS/buildkite.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/stacks/ecs/buildkite.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 IBoxLoader:
   - !exclude
-    - ecs/service-elasticloadbalancing.yml
-    - application-autoscaling/scalingpolicy.yml
+    - com/ecs/service-elasticloadbalancing.yml
+    - res/application-autoscaling/scalingpolicies.yml
   - !include
-    - iam/policy-update_stack.yml
+    - com/iam/policy-update_stack.yml
 
 global:
   StackName: bkt
   ApplicationAutoScalingScalingPolicy: IBOX_SKIP_FUNC
   Capacity:
     Desired: 3
     Max: 4
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/ECS/reserve-cpu.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 IBoxLoader: !exclude
-  - application-autoscaling/scalingpolicy.yml
-  - autoscaling/capacity.yml
-  - ecs/service-elasticloadbalancing.yml
-  - ec2/securitygroup.yml
-  - cloudwatch/alarms.yml
+  - res/application-autoscaling/scalingpolicies.yml
+  - com/autoscaling/capacity.yml
+  - com/ecs/service-elasticloadbalancing.yml
+  - com/ec2/securitygroup.yml
+  - res/cloudwatch/alarms.yml
 
 global:
   StackName: rsc
   ApplicationAutoScalingScalableTarget: IBOX_SKIP_FUNC
   ApplicationAutoScalingScalingPolicy: IBOX_SKIP_FUNC
   CloudWatchAlarm: IBOX_SKIP_FUNC
   ContainerDefinitions:
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/LBD/stacks-ops.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 IBoxLoader:
   - !include
-    - iam/policy-update_stack.yml
-    - lambda/layers.yml
+    - com/iam/policy-update_stack.yml
+    - com/lambda/layers.yml
 
 global:
   StackName: sss
   IAMPolicy:
     - UpdateStack:
         Roles:
           - Ref('RoleLambdaStacksOps')
@@ -23,20 +23,22 @@
                 Resource: '*'
             - KMSKey:
                 Action: 'kms:Decrypt'
                 Effect: Allow
                 Resource: get_expvalue('KeyParameterStore')
   Lambda:
     - StacksOps:
+        Architectures:
+          - arm64
         Code:
           ZipFile: str(IBOX_INDEXNAME)
         Description: 'Stacks Operations'
         Layers:
           - LambdaLayerVersionPython37SSM
-          - LambdaLayerVersionPythonIboxStacksOps
-          - LambdaLayerVersionPython39SlackClient
-        MemorySize: 128
+          - LambdaLayerVersionPythonArm64IboxStacksOps
+          - LambdaLayerVersionPythonArm64SlackClient
+        MemorySize: 512
         Runtime: python3.9
         Environment:
           Variables:
             - CloudFormationNotificationArn: get_expvalue('SNSTopicCloudFormationNotification')
         Timeout: 60
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/RES/res-ccr-lighthouse.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 IBoxLoader: !include
-  - lambda/layers.yml
+  - com/lambda/layers.yml
 
 global:
   StackName: r-ccr-lth
   Parameter:
     - EnvApp1Version:
         Description: EnvApp1Version used by Lambda
     - LightHouseTaskStackName:
@@ -33,19 +33,20 @@
             - 3:
                 Action:
                   - 'events:ListTargetsByRule'
                 Effect: Allow
                 Resource: '*'
   Lambda:
     - CCRLightHouse:
+        Architectures:
+          - arm64
         Export: True
         Code:
           ZipFile: str(IBOX_INDEXNAME)
         Description: 'Custom Resource for executing lighthouse-task'
         Layers:
           - LambdaLayerVersionPython39CRHelper
-        MemorySize: 128
         Runtime: python3.9
         Timeout: 300
         Environment:
           Variables:
             - LightHouseTaskStackName: Ref('LightHouseTaskStackName')
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/RES/res-ccr-stack-replicator.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             - 1:
                 Action:
                   - '*'
                 Effect: Allow
                 Resource: '*'
   Lambda:
     - CCRStackReplicator:
+        Architectures:
+          - arm64
         Export: True
         Code:
-          S3Bucket: Sub(cfg.BucketNameAppRepository)
-          S3Key: 'ibox-tools/stack-replicator/stack_replicator.zip'
+          ZipFile: str(IBOX_INDEXNAME)
         Description: 'Replicate Stacks'
-        MemorySize: 128
         Runtime: python3.9
         Timeout: 300
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/RES/res-ecs-alb.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 IBoxLoader: !include
-  - elasticloadbalancing/loadbalancer.yml
-  - cloudwatch/alarms.yml
+  - com/elasticloadbalancing/loadbalancer.yml
+  - res/cloudwatch/alarms.yml
 
 global:
   StackName: alb
   Parameter:
     - LoadBalancer:
         Description: 'Application Load Balancer to conditionally create - empty for default based on role - need to be already defined'
         AllowedValues: ['External', 'Internal', '']
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/RES/res-extra-01.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-extra-01.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 IBoxLoader: !include
-  - crm/certificate-global.yml
-  - crm/certificate-regional.yml
-  - cloudfront/policy.yml
-  - res-extra/cloudformation_stackset.yml
-  - elasticache/subnet-group.yml
-  - rds/db-subnet-group.yml
-  - apigateway/account.yml
-  - route53/recordset.yml
-  - efs/filesystem.yml
+  - com/certificatemanager/certificate-global.yml
+  - com/certificatemanager/certificate-regional.yml
+  - res/cloudfront/policies.yml
+  - com/iam/roles-cloudformation-stackset.yml
+  - res/elasticache/subnet-groups.yml
+  - res/rds/db-subnet-groups.yml
+  - res/apigateway/accounts.yml
+  - res/route53/recordsets.yml
+  - res/efs/filesystems.yml
 
 
 global:
   StackName: r-extra-01
   MappingClass:
     - AZones:
   EC2SecurityGroup:
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/RES/res-iam-group-01.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/RES/res-iam-policy-01.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 IBoxLoader: !include
-  - iam/managed-policy.yml
+  - res/iam/managed-policies.yml
 
 global:
   StackName: iam-p-01
   IAMManagedPolicy:
     - SSMParameterStoreBase:
         IBOX_ENABLED: True
     - LogRead:
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/RES/res-latedge-01.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml`

 * *Files 4% similar despite different names*

```diff
@@ -15,12 +15,11 @@
         Environment: IBOX_SKIP
     - AtEdgeAddHeaders:
         IBOX_ENABLED: False
         Code:
           ZipFile: str(IBOX_INDEXNAME)
         AtEdge: True
         Description: 'Lambda@Edge add Headers'
-        MemorySize: 128
         Runtime: python3.9
         Timeout: 10
         Version: True
         CacheControl: 31536000
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/RES/vpc.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/stacks/res/vpc.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/TSK/TYPE.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/stacks/tsk/i_type.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 IBoxLoader: !include
-  - ecs/ecs-task.yml
-  - lambda/permission.yml
+  - com/ecs/task.yml
+  - res/lambda/permissions.yml
 
 global:
   Condition:
     - EnableExecuteCommand: Equals(True, False)
       # Need to create a "dummy" Condition for tasks that do not use EventsRuleECSRunTask, where there is the "right" one
     - ECSTasksLaunchOnFargate: Equals(True, True)
   ECSTaskDefinition:
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/apigateway/stage.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/apigateway/ibox_base.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,44 @@
-Stage: &stage
-  IBOX_LINKED_OBJ:
-    Key: ApiGatewayDeployment
-    Type: Base
-    For: ["A", "B"]
-    Conf:
-      IBOX_RESNAME: ApiGatewayDeployment.IBOX_INDEXNAME
-      IBOX_LINKED_OBJ_NAME: IBOX_INDEXNAME.IBOX_LINKED_OBJ_FOR
-      IBOX_LINKED_OBJ_INDEX: IBOX_INDEXNAME
-  IBOX_PARAMETER:
-    - Deployment.IBOX_INDEXNAME.Description:
-        Description: str(f"Deployment{IBOX_INDEXNAME} Description")
-        Default: str(IBOX_INDEXNAME)
-    - Deployment.IBOX_INDEXNAME:
-        Description: str(f"Deployment{IBOX_INDEXNAME} - change between A/B " "to trigger new deploy")
-        AllowedValues: ["A", "B"]
-        Default: "A"
-  IBOX_CONDITION:
-    - Deployment.IBOX_INDEXNAME.A:
-        get_condition("", "equals", "A", f"Deployment{IBOX_INDEXNAME}", nomap=True)
-    - Deployment.IBOX_INDEXNAME.B:
-        get_condition("", "equals", "B", f"Deployment{IBOX_INDEXNAME}", nomap=True)
-  IBOX_OUTPUT:
-    - Deployment.IBOX_INDEXNAME:
-        Value: Ref(f"Deployment{IBOX_INDEXNAME}")
-  DeploymentId: If(
-    f"Deployment{IBOX_INDEXNAME}A", Ref(f"ApiGatewayDeployment{IBOX_INDEXNAME}A"), Ref(f"ApiGatewayDeployment{IBOX_INDEXNAME}B"))
-  RestApiId: Ref("ApiGatewayRestApi")
-  StageName: str(IBOX_INDEXNAME)
-
-
 global:
+  ApiGatewayDomainName:
+    - IBOX_BASE:
+        IBOX_ENABLED: False
+        IBOX_LINKED_OBJ:
+          Key: Route53RecordSet
+          Type: ApiGatewayDomainName.IBOX_INDEXNAME
+          Conf:
+            IBOX_RESNAME: RecordSet.IBOX_RESNAME
+        IBOX_OUTPUT:
+          - _:
+              Value: Ref(IBOX_RESNAME)
+              Export: Export(IBOX_RESNAME)
+
   ApiGatewayStage:
-    - IBOX_BASE: *stage
+    - IBOX_BASE:
+        IBOX_LINKED_OBJ:
+          Key: ApiGatewayDeployment
+          Type: Base
+          For: ["A", "B"]
+          Conf:
+            IBOX_RESNAME: ApiGatewayDeployment.IBOX_INDEXNAME
+            IBOX_LINKED_OBJ_NAME: IBOX_INDEXNAME.IBOX_LINKED_OBJ_FOR
+            IBOX_LINKED_OBJ_INDEX: IBOX_INDEXNAME
+        IBOX_PARAMETER:
+          - Deployment.IBOX_INDEXNAME.Description:
+              Description: str(f"Deployment{IBOX_INDEXNAME} Description")
+              Default: str(IBOX_INDEXNAME)
+          - Deployment.IBOX_INDEXNAME:
+              Description: str(f"Deployment{IBOX_INDEXNAME} - change between A/B " "to trigger new deploy")
+              AllowedValues: ["A", "B"]
+              Default: "A"
+        IBOX_CONDITION:
+          - Deployment.IBOX_INDEXNAME.A:
+              get_condition("", "equals", "A", f"Deployment{IBOX_INDEXNAME}", nomap=True)
+          - Deployment.IBOX_INDEXNAME.B:
+              get_condition("", "equals", "B", f"Deployment{IBOX_INDEXNAME}", nomap=True)
+        IBOX_OUTPUT:
+          - Deployment.IBOX_INDEXNAME:
+              Value: Ref(f"Deployment{IBOX_INDEXNAME}")
+        DeploymentId: If(
+          f"Deployment{IBOX_INDEXNAME}A", Ref(f"ApiGatewayDeployment{IBOX_INDEXNAME}A"), Ref(f"ApiGatewayDeployment{IBOX_INDEXNAME}B"))
+        RestApiId: Ref("ApiGatewayRestApi")
+        StageName: str(IBOX_INDEXNAME)
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/application-autoscaling/scalabletarget.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/application-autoscaling/scalingpolicy.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,79 +1,63 @@
 Tracking: &tracking
   Condition: IBOX_RESNAME
   IBOX_PARAMETER:
-    - _TargetTrackingScalingPolicyConfigurationTargetValue:
+    - _TargetTrackingConfigurationTargetValue:
         Description: '0 to disable - empty for mapped value'
   IBOX_CONDITION:
     - _:
-        get_condition('', 'not_equals', '0', f'{IBOX_RESNAME}TargetTrackingScalingPolicyConfigurationTargetValue')
+        get_condition('', 'not_equals', '0', f'{IBOX_RESNAME}TargetTrackingConfigurationTargetValue')
+  EstimatedInstanceWarmup: 120
   PolicyType: TargetTrackingScaling
 
 Step: &step
+  AdjustmentType: ChangeInCapacity
+  EstimatedInstanceWarmup: 600
   PolicyType: StepScaling
-  StepScalingPolicyConfiguration:
-    AdjustmentType: ChangeInCapacity
-    MetricAggregationType: Average
-
+             
 global:
-  ApplicationAutoScalingScalingPolicy:
-    - IBOX_BASE:
-        PolicyName: IBOX_RESNAME
-        ScalingTargetId: Ref('ApplicationAutoScalingScalableTargetECSService')
-        TargetTrackingScalingPolicyConfiguration:
-          PredefinedMetricSpecification.IBOX_PCO:
-            IBOX_OUTPUT:
-              - _:
-                  Value: PredefinedMetricType= ${PredefinedMetricSpecificationPredefinedMetricType} ,TargetValue= ${TargetValue}
-          CustomizedMetricSpecification.IBOX_PCO:
-            IBOX_OUTPUT:
-              - _:
-                  Value: MetricName= ${CustomizedMetricSpecificationMetricName} ,Statistic= ${CustomizedMetricSpecificationStatistic} ,TargetValue= ${TargetValue}
+  AutoScalingScalingPolicy:
     - Cpu:
         <<: *tracking
         IBOX_ENABLED: False
-        TargetTrackingScalingPolicyConfiguration:
+        TargetTrackingConfiguration:
           PredefinedMetricSpecification:
-            PredefinedMetricType: 'ECSServiceAverageCPUUtilization'
-          ScaleInCooldown: 60
-          ScaleOutCooldown: 60
-          TargetValue: 80
+            PredefinedMetricType: 'ASGAverageCPUUtilization'
+          TargetValue: 70
     - Custom:
         <<: *tracking
         IBOX_ENABLED: False
-        TargetTrackingScalingPolicyConfiguration:
+        TargetTrackingConfiguration:
           CustomizedMetricSpecification:
             Dimensions: []
-            Namespace: 'AWS/ECS'
-            Statistic.IBOX_AUTO_P: {}
+            Namespace: 'AWS/EC2'
+            Statistic.IBOX_AUTO_P: {} 
     - Down:
         <<: *step
         IBOX_ENABLED: False
-        StepScalingPolicyConfiguration:
-          StepAdjustments:
-            - 0:
-                MetricIntervalLowerBound: -10
-                MetricIntervalUpperBound: 0
-                ScalingAdjustment: -1
-            - 1:
-                MetricIntervalLowerBound: -20
-                MetricIntervalUpperBound: -10
-                ScalingAdjustment: -2
-            - 2:
-                MetricIntervalUpperBound: -20
-                ScalingAdjustment: -2
+        StepAdjustments:
+          - 0:
+              MetricIntervalLowerBound: -10
+              MetricIntervalUpperBound: 0
+              ScalingAdjustment: -1
+          - 1:
+              MetricIntervalLowerBound: -20
+              MetricIntervalUpperBound: -10
+              ScalingAdjustment: -2
+          - 2:
+              MetricIntervalUpperBound: -20
+              ScalingAdjustment: -2
     - Up:
         <<: *step
         IBOX_ENABLED: False
-        StepScalingPolicyConfiguration:
-          StepAdjustments:
-            - 0:
-                MetricIntervalLowerBound: 0
-                MetricIntervalUpperBound: 10
-                ScalingAdjustment: 1
-            - 1:
-                MetricIntervalLowerBound: 10
-                MetricIntervalUpperBound: 20
-                ScalingAdjustment: 2
-            - 2:
-                MetricIntervalLowerBound: 20
-                ScalingAdjustment: 2
+        StepAdjustments:
+          - 0:
+              MetricIntervalLowerBound: 0
+              MetricIntervalUpperBound: 10
+              ScalingAdjustment: 1
+          - 1:
+              MetricIntervalLowerBound: 10
+              MetricIntervalUpperBound: 20
+              ScalingAdjustment: 2
+          - 2:
+              MetricIntervalLowerBound: 20
+              ScalingAdjustment: 2
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/autoscalinggroup.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 IBoxLoader: !include
-  - capacity.yml
-  #- imageid-ec2.yml
-  - launchtemplate.yml
-  - scalingpolicy.yml
-  - scheduledactions.yml
+  - com/autoscaling/capacity.yml
+  #- com/autoscaling/imageid-ec2.yml
+  - res/autoscaling/launchtemplates.yml
+  - res/autoscaling/scalingpolicies.yml
 
 global:
   AutoScalingGroup:
     - Base:
         IBOX_TITLE: AutoScalingGroup
         AvailabilityZones: GetAZs()
         DesiredCapacity: get_endvalue('CapacityDesired')
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/capacity.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/capacity.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/ephemeral.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/imageid-ec2.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/imageid-ecs.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/launchtemplate.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 IBoxLoader: !include [
-  #ephemeral.yml,
+  #com/autoscaling/ephemeral.yml,
 ]
 
 global:
   LaunchTemplate:
     - Data:
         IBOX_PARAMETER:
           - DoNotSignal:
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/mixed_instances.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/scheduledactions.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,21 @@
 global:
+  AutoScalingScalingPolicy:
+    - IBOX_BASE:
+        AutoScalingGroupName: Ref('AutoScalingGroup')
+        TargetTrackingConfiguration:
+          PredefinedMetricSpecification.IBOX_PCO:
+            IBOX_OUTPUT:
+              - _:
+                  Value: PredefinedMetricType= ${PredefinedMetricSpecificationPredefinedMetricType} ,TargetValue= ${TargetValue}
+          CustomizedMetricSpecification.IBOX_PCO:
+            IBOX_OUTPUT:
+              - _:
+                  Value: MetricName= ${CustomizedMetricSpecificationMetricName} ,Statistic= ${CustomizedMetricSpecificationStatistic} ,TargetValue= ${TargetValue}
+
   AutoScalingScheduledAction:
     - IBOX_BASE:
         IBOX_PARAMETER:
           - _DesiredSize:
               Description: 'k to keep current value - empty for mapped value'
           - _MinSize:
               Description: 'k to keep current value - empty for mapped value'
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/spot-asg.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml`

 * *Files 3% similar despite different names*

```diff
@@ -55,19 +55,20 @@
           Statement:
             - 1:
                 Action: 'autoscaling:SetDesiredCapacity'
                 Effect: Allow
                 Resource: Sub('arn:aws:autoscaling:*:*:autoScalingGroup:*:autoScalingGroupName/${AutoScalingGroup}')
   Lambda:
     - ASGSpot:
+        Architectures:
+          - arm64
         Condition: SpotASG
         Code:
           ZipFile: str(IBOX_INDEXNAME)
         Description: 'Rebalance Spot and OnDeman AutoScalingGroup'
-        MemorySize: 128
         ReservedConcurrentExecutions: 1
         Runtime: python3.9
         Timeout: 60
         Environment:
           Variables:
             - ASGOnDemand: Ref('AutoScalingGroup')
             - ASGSpot: Ref('AutoScalingGroupSpot')
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/autoscaling/spot-auto.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/cloudformation/custom-resource_light-house.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/cloudformation/custom-resource_light-house.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/cloudfront/custom-errors.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/cloudfront/distribution.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml`

 * *Files 17% similar despite different names*

```diff
@@ -73,7 +73,35 @@
             Value: ${WebACLId}
           WebACLId: none
         LogEnabled.IBOX_AUTO_PO:
           Description: 'Empty for mapped value'
           AllowedValues: ['', 'yes', 'no']
           CONDITION: get_condition('', 'equals', 'yes', f'{IBOX_RESNAME}LogEnabled')
         LogEnabled: 'no'
+
+  CloudFrontFunction:
+    - IBOX_BASE:
+        IBOX_OUTPUT:
+          - _:
+              Value: GetAtt(IBOX_RESNAME, "FunctionARN")
+              Export: Export(IBOX_RESNAME)
+        AutoPublish: True
+        FunctionCode: Join("", import_lambda(IBOX_INDEXNAME))
+        FunctionConfig:
+          Comment: str(IBOX_INDEXNAME)
+          Runtime: cloudfront-js-1.0
+        Name: str(IBOX_INDEXNAME)
+
+  CloudFrontLambdaFunctionAssociation:
+    - IBOX_BASE:
+        IBOX_PARAMETER:
+          - _LambdaFunctionARN:
+              Description: LambdaAtEdge Version Arn - empty for mapped value - none to disable
+        IBOX_CONDITION:
+          - _LambdaFunctionARN:
+              get_condition('', 'not_equals', 'none', f'{IBOX_RESNAME}LambdaFunctionARN')
+        IBOX_OUTPUT:
+          - _LambdaFunctionARN:
+              Value: ${LambdaFunctionARN}
+        Condition: IBOX_RESNAME.LambdaFunctionARN
+        EventType: viewer-request
+        LambdaFunctionARN: none
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/cloudfront/for-services.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/cloudfront/for-services.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 IBoxLoader: !include
-  - cloudfront/base.yml
-  - route53/recordset.yml
+  - com/cloudfront/i_base.yml
+  - res/route53/recordsets.yml
 
 global:
   CloudFrontDistribution:
     - IBOX_BASE:
         IBOX_LINKED_OBJ:
           Route53RecordSet:
             Key: Route53RecordSet
@@ -32,9 +32,9 @@
                 DomainName: get_endvalue('CloudFrontDistributionBaseDistributionConfigDefaultCacheBehaviorTargetOriginId')
                 Id: get_endvalue('CloudFrontDistributionBaseDistributionConfigDefaultCacheBehaviorTargetOriginId')
         DnsSuffix.IBOX_AUTO_PO:
           Description: 'Useful to create duplicate stack that use CloudFront; change Aliases and DefaultOriginDomainName'
 
 
 IBoxLoaderAfter: !include [
-  #origin-adhoc.yml,
+  #com/cloudfront/origin-adhoc.yml,
 ]
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/cloudfront/policy.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/cloudfront/policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/cloudwatch/alarms.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/cloudwatch/alarms.yml`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,16 @@
   Threshold: '50'
   TreatMissingData: 'notBreaching'
   Namespace: 'AWS/ELB'
 
 ASGSpot: &asgspot
   Condition: SpotASG
   AlarmActions: [Ref('SNSTopicASGSpot')]
-  Period: Ref('AWS::NoValue')
+  Dimensions: IBOX_SKIP
+  Period: IBOX_SKIP
   Metrics: &asgspotmetrics
     - Expression:
     - MinOnDemand:
         ReturnData: false
         Id: m1
         MetricStat:
           Metric:
@@ -83,25 +84,14 @@
               - ASGOnDemand:
                   Name: AutoScalingGroupName
                   Value: Ref('AutoScalingGroupSpot')
             MetricName: GroupInServiceInstances
           Stat: Average
           Period: 60
 
-DiskUsed: &diskused
-  EvaluationPeriods: 3
-  MetricName: 'root_disk_used_percent'
-  Statistic: 'Maximum'
-  Namespace: 'CWAgent'
-  Unit: Percent
-  Dimensions:
-    - RootDisk:
-        Name: AutoScalingGroupName
-        Value: Ref('AutoScalingGroup')
-
 EC2: &ec2
   Dimensions:
     - Autoscaling:
         Name: AutoScalingGroupName
         Value: Ref('AutoScalingGroup')
   Namespace: 'AWS/EC2'
 
@@ -122,34 +112,14 @@
   Statistic: 'Average'
   Namespace: ''
   Unit: Percent
 
 
 global:
   CloudWatchAlarm:
-    - IBOX_BASE:
-        IBOX_ENABLED: False
-        IBOX_PARAMETER:
-          - _EvaluationPeriods:
-              Description: 'Number of periods for alarm evaluation - 0 to disable - empty for mapped value'
-              AllowedValues: ['', '0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
-          - _Threshold:
-              Description: 'Threshold for alarm triggering - empty for mapped value'
-              AllowedValues: ['', '10', '15', '20', '25', '30', '35', '40', '45', '50',
-                              '55', '60', '65', '70', '75', '80', '85', '90', '95', '100']
-        IBOX_CONDITION:
-          - _:
-              get_condition('', 'not_equals', '0', f'{IBOX_RESNAME}EvaluationPeriods')
-        IBOX_OUTPUT:
-          - _:
-              Value: Period= ${Period} ,EvaluationPeriods= ${EvaluationPeriods} ,Threshold= ${Threshold}
-        Condition: IBOX_RESNAME
-        ActionsEnabled: true
-        Period: 60
-        Dimensions: {}
     - EC2CPUHigh:
         <<: [*cpu, *ec2]
         AlarmActions: [Ref('AutoScalingScalingPolicyUp')]
         AlarmDescription: 'Alarm if CPU too High'
         ComparisonOperator: 'GreaterThanThreshold'
         Threshold: '60'
     - EC2CPULow:
@@ -245,17 +215,25 @@
           Expression:
             ReturnData: true
             Expression: m1 - m2 + m3 - m4
             Id: e1
             Label: OnDemandInExcess
         Threshold: -1
     - DiskUsed:
-        <<: *diskused
         ComparisonOperator: GreaterThanOrEqualToThreshold
+        Dimensions:
+          - RootDisk:
+              Name: AutoScalingGroupName
+              Value: Ref('AutoScalingGroup')
+        EvaluationPeriods: 3
+        MetricName: 'root_disk_used_percent'
+        Namespace: 'CWAgent'
+        Statistic: 'Maximum'
         Threshold: '80'
+        Unit: Percent
     - SQSQueueDeadLetter:
         IBOX_PARAMETER:
           - _Threshold:
               AllowedValues: ['', '1', '2', '3', '4', '5', '6', '7', '8', '9', '10']
               AlarmActions: [get_expvalue('SNSTopicCloudWatchAlarm')]
         AlarmActions: [get_expvalue('SNSTopicCloudWatchAlarm')]
         EvaluationPeriods: 1
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/cloudwatch/log_group.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/codedeploy/deployment-group.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/ibox_base.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,68 @@
 global:
-  Parameter:
-    - UpdateMode:
-        AllowedValues: ['none', 'Replace', 'Rolling', 'CodeDeploy']
-  Condition:
-    - DeployRevision:
-        Equals(Ref("UpdateMode"), "CodeDeploy")
-  CodeDeployDeploymentGroup:
+  LambdaPermission:
     - IBOX_BASE:
-        Ec2TagFilters:
-          - IBOX_IF:
-            - DeployRevision
-            - IBOX_IFVALUE
-            - Ref('AWS::NoValue')
-          - EnvStackName:
-              Key: EnvStackName
-              Type: KEY_AND_VALUE
-              Value: Ref("AWS::StackName")
-        Deployment:
-          IBOX_IF:
-            - DeployRevision
-            - IBOX_IFVALUE
-            - Ref('AWS::NoValue')
-          Revision:
-            RevisionType: S3
-            S3Location:
-              Bucket: Sub(cfg.BucketNameAppRepository)
-              BundleType: tgz
-              Key: Join('', [
-                  get_endvalue(f"{IBOX_RESNAME}ApplicationName"), "/", get_endvalue(f"{IBOX_RESNAME}ApplicationName"), "-",
-                  Sub(getattr(cfg, f'{IBOX_CURNAME}Suffix')),
-                ])
-        DeploymentGroupName: get_subvalue("${AWS::StackName}.${EnvRole}-${1M}", f"{IBOX_RESNAME}ApplicationName")
-        ServiceRoleArn: get_expvalue("RoleCodeDeploy", "")
-  - Test01:
-      IBOX_ENABLED: False
-      ApplicationName: "name.of.a.git.repo"
-      Deployment:
-        Revision:
-          S3Location:
-            # equals to:
-            # Key: Sub("name.of.a.git.repo/name.of.a.git.repo-${EnvApp1Version}.tar.gz")
-            KeySuffix: Sub("${EnvApp1Version}.tar.gz")
+        Action: "lambda:InvokeFunction"
+
+  Lambda:
+    - IBOX_BASE:
+        IBOX_LINKED_OBJ:
+          Role:
+            Key: IAMRole
+            Type: Lambda
+            Conf:
+              IBOX_RESNAME: Role.IBOX_RESNAME
+          LogGroup:
+            Key: LogsLogGroup
+            Type: Lambda
+            Conf:
+              IBOX_LINKED_OBJ_NAME: IBOX_RESNAME
+        IBOX_OUTPUT:
+          - _:
+              IBOX_ENABLED_IF: get_endvalue(f"{IBOX_RESNAME}Export") == True
+              Value: GetAtt(IBOX_RESNAME, "Arn")
+              Export: Export(IBOX_RESNAME)
+        Code:
+          ZipFile.IBOX_CODE_KEY: Join("", import_lambda(get_endvalue(f"{IBOX_RESNAME}CodeZipFile")))
+          S3Key.IBOX_AUTO_PO:
+            Description: str(f"S3Key Name for lambda {IBOX_INDEXNAME} Code")
+        Export: False
+        Layers.IBOX_CUSTOM_OBJ:
+          IBOX_PARAMETER:
+            - _:
+                Description: str(IBOX_RESNAME)
+          IBOX_OUTPUT:
+            - _:
+                Value: get_endvalue(IBOX_RESNAME)
+          Value: get_endvalue(IBOX_RESNAME)
+        LogGroupCreate: "yes"
+        Handler: "index.lambda_handler"
+        MemorySize.IBOX_AUTO_PO: {}
+        MemorySize: 128
+        Role: GetAtt(f"RoleLambda{IBOX_INDEXNAME}", "Arn")
+        FunctionName: Sub("${AWS::StackName}-${EnvRole}-%s" % IBOX_INDEXNAME)
+        Environment:
+          Variables.IBOX_PCO:
+            IBOX_PARAMETER:
+              - EnvServiceRestartTime:
+                  Description: 'Use to force service restart - can use: $(date +%F_%T)'
+          Variables:
+            - Env: Ref('EnvShort')
+            - EnvRole: Ref('EnvRole')
+            - IBox_EnvServiceRestartTime: Ref("EnvServiceRestartTime")
+
+  LambdaLayerVersion:
+    - IBOX_BASE:
+        IBOX_LINKED_OBJ:
+          Key: LambdaLayerVersionPermission
+          Type: Base
+          Conf:
+            IBOX_RESNAME: LambdaLayerPermission.IBOX_INDEXNAME
+            IBOX_LINKED_OBJ_NAME: IBOX_RESNAME
+        IBOX_OUTPUT:
+          - _:
+              Value: Ref(IBOX_RESNAME)
+        # Uncomment to retain previous layerversion
+        #UpdateReplacePolicy: Retain
+        Content:
+          S3Key.IBOX_AUTO_PO:
+            Description: str(f"S3Key Name for lambda {IBOX_INDEXNAME} Content")
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/crm/certificate-regional.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-IBoxLoader: !include [
-  crm/certificate.yml,
-]
-
 global:
   CertificateManagerCertificate:
     - LoadBalancerExternal:
         IBOX_ENABLED: False
         DomainName: Sub('*.%s' % cfg.HostedZoneNameRegionEnv)
         DomainValidationOptions:
           - Region:
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/dynamodb/table-credstash.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/ec2/bottlerocket.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/ec2/bottlerocket.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/ecr/ibox_base.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/ecr/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/ecs/capacityprovider.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/capacityprovider.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/ecs/daemon-reserver-cpu.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 IBoxLoader:
   - !exclude
-    - iam/ecs-exec.yml
+    - com/iam/policy-ecs-exec.yml
   - !include
-    - ecs/ecs-task.yml
-    - ecs/ecs-service.yml
+    - com/ecs/task.yml
+    - res/ecs/services.yml
 
 global:
   Parameter:
     - DaemonReserveCpu:
         Description: 'Empty for mapped value'
         AllowedValues: ['', 'yes', 'no']
   Condition:
@@ -25,15 +25,15 @@
         Cpu: 512
         Image: 'busybox'
         LogConfiguration: IBOX_SKIP_FUNC
         Memory: 32
   EC2SecurityGroup:
     - EcsService:
         IBOX_ENABLED: False
-  # Included yaml ecs/ecs-task.yml have changed ParameterStore Roles to RoleTask, need to restore it.
+  # Included yaml ecs/task.yml have changed ParameterStore Roles to RoleTask, need to restore it.
   IAMPolicy:
     - ParameterStore:
         Roles:
           - Ref('RoleInstance')
   LogDriver: none
   LogsLogGroup: IBOX_SKIP_FUNC
   IAMRole:
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/ecs/ecs-and-cluster.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 IBoxLoader:
   - !exclude
-      - ecs/daemon-reserver-cpu.yml
-      - elasticloadbalancing/loadbalancer.yml
+      - com/ecs/daemon-reserver-cpu.yml
+      - com/elasticloadbalancing/loadbalancer.yml
   - !include
-      - EC2/TYPE.yml
-      - EC2/ecs-cluster.yml
+      - stacks/ec2/i_type.yml
+      - stacks/ec2/ecs-cluster.yml
 
 global:
   IBOX_LAUNCH_TEMPLATE_NO_SG_EXTRA: True
   IBOX_ROLE_EX: ecs-cluster
   Output:
     - StackType:
         Value: ec2 ecs
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/ecs/ecs-fargate-spot.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/fargate-spot.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/ecs/ecs-scheduled.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/ecs/ecs-task.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/task.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-IBoxLoader: !include [
-  ecs-taskdefinition.yml,
-  ecs-containerdefinition.yml,
-  iam/parameterstore.yml,
-  iam/ecs-exec.yml,
-  ec2/securitygroup.yml,
-]
+IBoxLoader: !include
+  - res/ecs/taskdefinitions.yml
+  - com/iam/policy-parameterstore.yml
+  - com/iam/policy-ecs-exec.yml
+  - com/ec2/securitygroup.yml
+
 
 global:
   Parameter:
     - ClusterStack:
         Description: 'Cluster Stack Name used to launch service on - empty for default based on env/role'
     - DockerLabelLastUpdate:
         Description: 'Use to force redeploy - can use: $(date +%F_%T)'
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/ecs/ecs-taskdefinition.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/ecs/service-elasticloadbalancing.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 IBoxLoader: !include
-  - elasticloadbalancing/base.yml
-  - elasticloadbalancing/v2-listener-rule.yml
-  - cloudfront/for-services.yml
-  - res-elasticloadbalancing/v2-listener.yml
+  - com/elasticloadbalancing/i_base.yml
+  - res/elasticloadbalancing/v2-listener-rules.yml
+  - com/cloudfront/for-services.yml
+  - com/elasticloadbalancing/v2-listener.yml
 
 global:
   Parameter:
     - LoadBalancer:
         Description: "Comma delimited list of enabled LoadBalancerApplication - empty for mapped value - none to disable"
         AllowedValues: ["", "none", "External", "Internal", "External,Internal"]
   Condition:
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/efs/filesystem.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/efs/ibox_base.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,19 @@
-Base: &base
-  IBOX_OUTPUT:
-    - _:
-        Condition: IBOX_RESNAME
-        Value: Ref(IBOX_RESNAME)
-        Export: Export(IBOX_RESNAME)
-  IBOX_LINKED_OBJ:
-    Key: Route53RecordSet
-    Type: EFS
-    Conf:
-      IBOX_RESNAME: RecordSetEFS.IBOX_INDEXNAME
-      IBOX_LINKED_OBJ_NAME: IBOX_RESNAME
-      IBOX_LINKED_OBJ_INDEX: IBOX_INDEXNAME
-  Condition: IBOX_RESNAME
-  Enabled: 'no'
-  Encrypted: false
-  PerformanceMode: generalPurpose
-
-
 global:
   EFSFileSystem:
-    - IBOX_BASE: *base
-    - EcsCluster:
-        Name: EcsCluster
+    - IBOX_BASE:
+        IBOX_OUTPUT:
+          - _:
+              Condition: IBOX_RESNAME
+              Value: Ref(IBOX_RESNAME)
+              Export: Export(IBOX_RESNAME)
+        IBOX_LINKED_OBJ:
+          Key: Route53RecordSet
+          Type: EFS
+          Conf:
+            IBOX_RESNAME: RecordSetEFS.IBOX_INDEXNAME
+            IBOX_LINKED_OBJ_NAME: IBOX_RESNAME
+            IBOX_LINKED_OBJ_INDEX: IBOX_INDEXNAME
+        Condition: IBOX_RESNAME
+        Enabled: 'no'
+        Encrypted: false
+        PerformanceMode: generalPurpose
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/elasticache/cluster-and-replication-group.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/elasticache/ibox_base.yml`

 * *Files 4% similar despite different names*

```diff
@@ -98,7 +98,17 @@
         <<: [*base, *cluster]
         IBOX_TITLE: ElastiCacheCacheCluster
   
   ElastiCacheReplicationGroup:
     - IBOX_BASE:
         <<: [*base, *replication-group, *cluster]
         IBOX_TITLE: ElastiCacheReplicationGroup
+
+  ElastiCacheSubnetGroup:
+    - IBOX_BASE:
+        IBOX_RESNAME: CacheSubnetGroup.IBOX_INDEXNAME
+        IBOX_OUTPUT:
+          - _:
+              Value: Ref(IBOX_RESNAME)
+              Export: Export(IBOX_RESNAME)
+        Description: Sub("${EnvShort}-%s" % IBOX_INDEXNAME)
+        SubnetIds: Split(",", ImportValue(f"Subnets{IBOX_INDEXNAME}"))
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/elasticloadbalancing/accountid.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/elasticloadbalancing/certificate-adhoc.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/elasticloadbalancing/classic-loadbalancer.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml`

 * *Files 20% similar despite different names*

```diff
@@ -58,7 +58,39 @@
           - GetAtt('SecurityGroupLoadBalancer', 'GroupId')
     - External:
         Scheme: 'internet-facing'
         Subnets: Split(',', get_expvalue('SubnetsPublic'))
     - Internal:
         Scheme: 'internal'
         Subnets: Split(',', get_expvalue('SubnetsPrivate'))
+
+  ElasticLoadBalancingV2Listener:
+    - IBOX_BASE:
+        Access: Public
+        Port.IBOX_AUTO_PO: {}
+
+  ElasticLoadBalancingV2ListenerRule:
+    - IBOX_BASE:
+        Conditions:
+          - IBOX_BASE:
+              Values.IBOX_CUSTOM_OBJ:
+                Value.IBOX_PCO:
+                  IBOX_PARAMETER:
+                    - IBOX_REFNAME.Values.IBOX_RESNAME:
+                        Description: "Empty for mapped value"
+                  IBOX_OUTPUT:
+                    - IBOX_REFNAME.Values.IBOX_RESNAME:
+                        Value: get_endvalue(f"{IBOX_REFNAME}Values{IBOX_RESNAME}")
+                Value: get_endvalue(f"{IBOX_REFNAME}Values{IBOX_RESNAME}")
+        Priority.IBOX_AUTO_PO: {}
+
+  ElasticLoadBalancingV2TargetGroup:
+    - IBOX_BASE:
+        IBOX_OUTPUT:
+          - _HealthCheck:
+              Value: >-
+                Path= ${HealthCheckPath} ,Interval= ${HealthCheckIntervalSeconds} ,Timeout= ${HealthCheckTimeoutSeconds} ,Healthy= ${HealthyThresholdCount} ,Unhealthy= ${UnhealthyThresholdCount}
+        HealthCheckIntervalSeconds: Ref('AWS::NoValue')
+        HealthCheckPath: Ref('AWS::NoValue')
+        HealthCheckTimeoutSeconds: Ref('AWS::NoValue')
+        HealthyThresholdCount: Ref('AWS::NoValue')
+        UnhealthyThresholdCount: Ref('AWS::NoValue')
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/elasticloadbalancing/hostedzoneid.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/elasticloadbalancing/listener.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/listeners.yml`

 * *Files 1% similar despite different names*

```diff
@@ -42,17 +42,14 @@
           MessageBody: "404 Not Found\n"
           StatusCode: '404'
         Type: 'fixed-response' 
 
 
 global:
   ElasticLoadBalancingV2Listener:
-    - IBOX_BASE:
-        Access: Public
-        Port.IBOX_AUTO_PO: {}
     - EC2HttpInternal:
         IBOX_ENABLED: False
         <<: *http
         DefaultActions:
           - TG:
               Type: forward
               TargetGroupArn: Ref('ElasticLoadBalancingV2TargetGroupEC2LoadBalancerApplicationInternal')
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/elasticloadbalancing/targetgroup.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml`

 * *Files 14% similar despite different names*

```diff
@@ -22,24 +22,14 @@
         Key: 'stickiness.enabled'
         Value: If(f'{IBOX_MAPNAME}TargetGroupAttributesCookieDurationValue', 'true', 'false')
   Protocol: HTTP
   VpcId: get_expvalue('VpcId')
 
 global:
   ElasticLoadBalancingV2TargetGroup:
-    - IBOX_BASE:
-        IBOX_OUTPUT:
-          - _HealthCheck:
-              Value: >-
-                Path= ${HealthCheckPath} ,Interval= ${HealthCheckIntervalSeconds} ,Timeout= ${HealthCheckTimeoutSeconds} ,Healthy= ${HealthyThresholdCount} ,Unhealthy= ${UnhealthyThresholdCount}
-        HealthCheckIntervalSeconds: Ref('AWS::NoValue')
-        HealthCheckPath: Ref('AWS::NoValue')
-        HealthCheckTimeoutSeconds: Ref('AWS::NoValue')
-        HealthyThresholdCount: Ref('AWS::NoValue')
-        UnhealthyThresholdCount: Ref('AWS::NoValue')
     - EC2LoadBalancerApplicationExternal:
         IBOX_ENABLED: False
         <<: *base
         Port: 80
     - EC2LoadBalancerApplicationInternal:
         IBOX_ENABLED: False
         <<: *base
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/elasticloadbalancing/v2-listener-rule.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/iam/ibox_base.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,69 @@
-Base: &base
-  IBOX_ENABLED: False
-  IBOX_RESNAME: Listener.IBOX_INDEXNAME
-  Conditions:
-    - Host:
-        Field: host-header
-        Values:
-          - 1: Sub('*${EnvRole}.*')
-
 global:
-  ElasticLoadBalancingV2ListenerRule:
+  IAMManagedPolicy:
     - IBOX_BASE:
-        Conditions:
-          - IBOX_BASE:
-              Values.IBOX_CUSTOM_OBJ:
-                Value.IBOX_PCO:
-                  IBOX_PARAMETER:
-                    - IBOX_REFNAME.Values.IBOX_RESNAME:
-                        Description: "Empty for mapped value"
-                  IBOX_OUTPUT:
-                    - IBOX_REFNAME.Values.IBOX_RESNAME:
-                        Value: get_endvalue(f"{IBOX_REFNAME}Values{IBOX_RESNAME}")
-                Value: get_endvalue(f"{IBOX_REFNAME}Values{IBOX_RESNAME}")
-        Priority.IBOX_AUTO_PO: {}
-    - HttpsExternalRules1:
-        <<: *base
-        Actions:
-          - 1:
-              Type: forward
-              TargetGroupArn: Ref("TargetGroupExternal")
-        ListenerArn: get_expvalue("ListenerHttpsDefaultExternal", "LoadBalancerApplicationStack")
-    - HttpExternalRules1:
-        <<: *base
-        Actions:
-          - 1:
-              Type: forward
-              TargetGroupArn: Ref("TargetGroupExternal")
-        ListenerArn: get_expvalue("ListenerHttpDefaultExternal", "LoadBalancerApplicationStack")
-    - HttpInternalRules1:
-        <<: *base
-        Actions:
-          - 1:
-              Type: forward
-              TargetGroupArn: Ref("TargetGroupInternal")
-        ListenerArn: get_expvalue("ListenerHttpDefaultInternal", "LoadBalancerApplicationStack")
+        IBOX_RESNAME: IAMPolicy.IBOX_INDEXNAME
+        IBOX_OUTPUT:
+          - _:
+              IBOX_ENABLED_IF: get_endvalue(f"{IBOX_MAPNAME}Export") == True
+              Value: Ref(IBOX_RESNAME)
+              Export: Export(IBOX_RESNAME)
+        Export: True
+        PolicyDocument:
+          Statement:
+            - IBOX_LIST: {}
+          Version: "2012-10-17"
+  IAMRole:
+    - IBOX_BASE:
+        IBOX_RESNAME: Role.IBOX_INDEXNAME
+        IBOX_OUTPUT:
+          - _:
+              IBOX_ENABLED_IF: get_endvalue(f"{IBOX_MAPNAME}Export") == True
+              Value: GetAtt(IBOX_RESNAME, "Arn")
+              Export: Export(IBOX_RESNAME)
+        Export: False
+        AssumeRolePolicyDocument:
+          Statement:
+            - IBOX_LIST:
+            - 1:
+                Action: 'sts:AssumeRole'
+                Effect: Allow
+                Principal:
+                  Service:
+                    - get_endvalue(f"{IBOX_MAPNAME}Principal")
+        Path: "/"
+  IAMPolicy:
+    - IBOX_BASE:
+        IBOX_OUTPUT:
+          - _:
+              IBOX_ENABLED_IF: get_endvalue(f"{IBOX_MAPNAME}Export") == True
+              Value: Ref(IBOX_RESNAME)
+              Export: Export(IBOX_RESNAME)
+        Export: False
+        PolicyName: IBOX_INDEXNAME
+        PolicyDocument:
+          Statement:
+            - IBOX_LIST: {}
+          Version: "2012-10-17"
+  IAMUser:
+    - IBOX_BASE:
+        IBOX_LINKED_OBJ:
+          Key: SSMParameter
+          Type: UserPasswordBase
+          Conf:
+            IBOX_RESNAME: SSMParameterPassword.IBOX_INDEXNAME
+            IBOX_LINKED_OBJ_NAME: IBOX_RESNAME
+            IBOX_LINKED_OBJ_INDEX: IBOX_INDEXNAME
+        IBOX_PARAMETER:
+          - PasswordBase.IBOX_INDEXNAME:
+              Description: "Base Password, must be changed at first login"
+              NoEcho: True
+        IBOX_CONDITION:
+          - _:
+              get_condition("", "equals", "yes", f"{IBOX_RESNAME}Enabled")
+          - _RoleAccount:
+              get_condition("", "not_equals", "none", f"{IBOX_RESNAME}RoleAccount")
+        Condition: IBOX_RESNAME
+        UserName: str(IBOX_REMAPNAME)
+        LoginProfile:
+          Password: GetAtt(f"SSMParameterPassword{IBOX_INDEXNAME}", "Value")
+          PasswordResetRequired: True
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/elasticloadbalancing/v2-loadbalancer.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/events/ibox_base.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/events/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/iam/managed-policy.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/iam/managed-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/iam/parameterstore.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/iam/policy-bucket-replica.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/iam/policy-bucket-replica.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/iam/policy-update_stack.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/iam/policy-update_stack.yml`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,18 @@
                   - 'sns:*'
                   - 'cloudwatch:*'
                   - 'autoscaling:*'
                   - 'route53:*'
                   - 'codedeploy:*'
                   - 'acm:*'
                   - 'cloudformation:DescribeStack*'
-                  - 'cloudformation:GetTemplate*'
+                  - 'cloudformation:ListStacks'
                   - 'cloudformation:ListStackResources'
                   - 'cloudformation:ListExports'
+                  - 'cloudformation:GetTemplate*'
                   - 'cloudformation:UpdateStack'
                   - 'cloudformation:CancelUpdateStack'
                   - 'cloudformation:ValidateTemplate'
                   - 'cloudfront:*'
                   - 'lambda:*'
                   - 'events:*'
                   - 'elasticfilesystem:*'
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/iam/role.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/iam/roles.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/kms/key-and-alias.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/lambda/ccr-fargate-spot.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 global:
   Lambda:
     - CCRFargateSpot:
+        Architectures:
+          - arm64
         Export: True
         Code:
-          S3Bucket: Sub(cfg.BucketNameAppRepository)
-          S3Key: Sub('ibox-tools/ccr-fargate-spot/ccr-fargate-spot.zip')
+          ZipFile: str(IBOX_INDEXNAME)
         Description: 'CCR invoked by stack using Fargate Spot'
         Runtime: python3.9
         Timeout: 60
   IAMPolicy:
     - LambdaCCRFargateSpot:
         Roles:
           - Ref('RoleLambdaCCRFargateSpot')
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/lambda/function.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/functions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/lambda/permission.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/permissions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/lambda/service_unavailable.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/service-unavailable.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 global:
   Output:
     - LambdaServiceUnavailableArn:
         Value: GetAtt('LambdaServiceUnavailable', 'Arn')
         Export: Export('LambdaServiceUnavailableArn')
   Lambda:
     - ServiceUnavailable:
+        Architectures:
+          - arm64
         Code:
           ZipFile: str(IBOX_INDEXNAME)
         Description: 'Lambda to serve resource-unavailable pages'
-        MemorySize: 128
         Runtime: python3.9
         Timeout: 65
         Environment:
           Variables:
             - RCode: 503
             - Bucket: Sub(cfg.BucketNameAppData)
   LambdaPermission:
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/lambda/version.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/lambda/versions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/rds/db-instance.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/rds/ibox_base.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,145 +1,152 @@
-# Here i use IBOX_MAPNAME in place of IBOX_RESNAME because current resource name IBOX_RESNAME is simply DBInstance.
-# Instead i want to have a code that permit to create multiple rds resources in the same stack.
-Base: &base
-  IBOX_ENABLED: False
-  IBOX_LINKED_OBJ:
-    Key: Route53RecordSet
-    Conf:
-      IBOX_RESNAME: RecordSet
-      IBOX_LINKED_OBJ_NAME: IBOX_RESNAME
-    Type: RDS
-    For: ["External", "Internal"]
-  IBOX_PARAMETER:
-    - IBOX_MAPNAME.AllocatedStorage:
-        Description: 'Storage Size in GB - empty for mapped value'
-    - IBOX_MAPNAME.MaxAllocatedStorage:
-        Description: 'Max Storage Size in GB (Enable Storage Autoscaling)- empty for mapped value - 0 to disable'
-    - IBOX_MAPNAME.DBInstanceClass:
-        Description: 'Instance Type - empty for mapped value'
-        AllowedValues: [
-          '', 'db.m3.medium', 'db.m3.large', 'db.m3.xlarge', 'db.m3.2xlarge',
-          'db.m4.large', 'db.m4.xlarge', 'db.m4.2xlarge', 'db.m4.4xlarge', 'db.m4.10xlarge',
-          'db.m5.large', 'db.m5.xlarge', 'db.m5.2xlarge', 'db.m5.4xlarge', 'db.m5.12xlarge',
-          'db.r3.large', 'db.r3.xlarge', 'db.r3.2xlarge', 'db.r3.4xlarge', 'db.r3.8xlarge',
-          'db.r5.large', 'db.r5.xlarge', 'db.r5.2xlarge', 'db.r5.4xlarge', 'db.r5.12xlarge',
-          'db.t2.micro', 'db.t2.small', 'db.t2.medium', 'db.t2.large',
-          'db.t3.micro', 'db.t3.small', 'db.t3.medium', 'db.t3.large']
-    - IBOX_MAPNAME.DBName:
-        Description: 'Empty for mapped value'
-    - IBOX_MAPNAME.DBSnapshotIdentifier:
-        Description: 'DB snapshot used to restore the DB instance - "none" for not using one - empty for mapped value'
-    - IBOX_MAPNAME.DeletionProtection:
-        Description: 'empty for mapped value'
-        AllowedValues: ['', 'true', 'false']
-    - IBOX_MAPNAME.SourceDBInstanceIdentifier:
-        Description: 'ID of the source DB instance to create ReadReplica - "none" for not using one - empty for mapped value'
-    - IBOX_MAPNAME.Engine:
-        Description: 'Engine - empty for mapped value'
-        AllowedValues: [
-          '', 'mysql', 'mariadb', 'oracle-se1', 'oracle-se2', 'oracle-se', 'oracle-ee',
-          'sqlserver-ee', 'sqlserver-se', 'sqlserver-ex', 'sqlserver-web', 'postgres', 'aurora'
-        ]
-    - IBOX_MAPNAME.EngineVersion:
-        Description: 'Engine Version - empty for mapped value'
-    - IBOX_MAPNAME.MasterUsername:
-        Description: 'Username - empty for mapped value'
-    - IBOX_MAPNAME.MasterUserPassword:
-        Description: 'Password - empty for mapped value'
-        NoEcho: true
-    - IBOX_MAPNAME.MonitoringInterval:
-        Description: 'The interval, in seconds, for Enhanced Monitoring metrics - empty for mapped value - 0 to disable'
-        AllowedValues: ['', '0', '1', '5', '10', '15', '30', '60']
-    - IBOX_MAPNAME.MultiAZ:
-        Description: 'Use multiple Availability Zone - empty for mapped value'
-        AllowedValues: ['', 'true', 'false']
-    - IBOX_MAPNAME.PerformanceInsights:
-        Description: 'The amount of time, in days, to retain Performance Insights data - empty for mapped value - 0 to disable'
-    - IBOX_MAPNAME.StorageType:
-        Description: 'empty for mapped value'
-        AllowedValues: ['', 'standard', 'gp2']
-  IBOX_CONDITION:
-    - IBOX_MAPNAME.DBSnapshotIdentifier:
-        get_condition('', 'not_equals', 'none', f'{IBOX_MAPNAME}DBSnapshotIdentifier')
-    - IBOX_MAPNAME.SourceDBInstanceIdentifier:
-        get_condition('', 'not_equals', 'none', f'{IBOX_MAPNAME}SourceDBInstanceIdentifier')
-    - IBOX_MAPNAME.DBInstanceSkipProperties:
-        Or(Condition(f'{IBOX_MAPNAME}DBSnapshotIdentifier'), Condition(f'{IBOX_MAPNAME}SourceDBInstanceIdentifier'))
-    - IBOX_MAPNAME.MonitoringInterval:
-        get_condition('', 'not_equals', '0', f'{IBOX_MAPNAME}MonitoringInterval')
-    - IBOX_MAPNAME.PerformanceInsights:
-        get_condition('', 'not_equals', '0', f'{IBOX_MAPNAME}PerformanceInsights')
-    - IBOX_MAPNAME.StorageAutoScaling:
-        get_condition('', 'not_equals', '0', f'{IBOX_MAPNAME}MaxAllocatedStorage')
-  IBOX_OUTPUT:
-    - IBOX_MAPNAME.AllocatedStorage:
-        Value: ${AllocatedStorage}
-    - IBOX_MAPNAME.MaxAllocatedStorage:
-        Value: ${MaxAllocatedStorage}
-    - IBOX_MAPNAME.DBInstanceClass:
-        Value: ${DBInstanceClass}
-    - IBOX_MAPNAME.DBName:
-        Value: ${DBName}
-    - IBOX_MAPNAME.DBSnapshotIdentifier:
-        Value: ${DBSnapshotIdentifier}
-    - IBOX_MAPNAME.DeletionProtection:
-        Value: ${DeletionProtection}
-    - IBOX_MAPNAME.Engine:
-        Value: ${Engine}
-    - IBOX_MAPNAME.EngineVersion:
-        Value: ${EngineVersion}
-    - IBOX_MAPNAME.MasterUsername:
-        Value: ${MasterUsername}
-    - IBOX_MAPNAME.MonitoringInterval:
-        Value: ${MonitoringInterval}
-    - IBOX_MAPNAME.MultiAZ:
-        Value: ${MultiAZ}
-    - IBOX_MAPNAME.PerformanceInsightsRetentionPeriod:
-        Value: ${PerformanceInsightsRetentionPeriod}
-    - IBOX_MAPNAME.PubliclyAccessible:
-        Value: ${PubliclyAccessible}
-    - IBOX_MAPNAME.SourceDBInstanceIdentifier:
-        Value: ${SourceDBInstanceIdentifier}
-    - IBOX_MAPNAME.StorageType:
-        Value: ${StorageType}
-  AllocatedStorage: 50
-  AllowMajorVersionUpgrade: true
-  DBInstanceClass: db.t3.micro
-  DBName: dbname
-  DBParameterGroupName: Ref('DBParameterGroup1')
-  DBSnapshotIdentifier: none
-  DeletionProtection: false
-  EnablePerformanceInsights:
-    If(f'{IBOX_MAPNAME}PerformanceInsights', True, False)
-  MasterUsername: masterusername
-  MasterUserPassword: masteruserpassword
-  MaxAllocatedStorage: 0
-  MaxAllocatedStorage.IBOX_CODE:
-    If(f'{IBOX_MAPNAME}StorageAutoScaling', get_endvalue(f'{IBOX_MAPNAME}MaxAllocatedStorage'), Ref('AWS::NoValue'))
-  MonitoringInterval: 0
-  MonitoringRoleArn: If(f'{IBOX_MAPNAME}MonitoringInterval', get_expvalue('RoleRDSEnhancedMonitoring'), Ref('AWS::NoValue'))
-  MultiAZ: false
-  PerformanceInsights: 0
-  PerformanceInsightsRetentionPeriod:
-    If(f'{IBOX_MAPNAME}PerformanceInsights', get_endvalue(f'{IBOX_MAPNAME}PerformanceInsights'), Ref('AWS::NoValue'))
-  SourceDBInstanceIdentifier: none
-  StorageType: gp2
-  VPCSecurityGroups:
-    - Ref(f'SecurityGroup{IBOX_MAPNAME}')
-
 Mysql: &mysql
-  <<: *base
   Engine: mysql
   EngineVersion: '5.7'
 
 MysqlInternal:
-  <<: [*base, *mysql]
+  <<: *mysql
   PubliclyAccessible: false
   DBSubnetGroupName: get_expvalue('DBSubnetGroupPrivate')
 MysqlExternal:
-  <<: [*base, *mysql]
+  <<: *mysql
   PubliclyAccessible: true
   DBSubnetGroupName: get_expvalue('DBSubnetGroupPublic')
 
 global:
   RDSDBInstance:
-    - IBOX_BASE: *base
+    # Here i use IBOX_MAPNAME in place of IBOX_RESNAME because current resource name IBOX_RESNAME is simply DBInstance.
+    # Instead i want to have a code that permit to create multiple rds resources in the same stack.
+    - IBOX_BASE:
+        IBOX_ENABLED: False
+        IBOX_LINKED_OBJ:
+          Key: Route53RecordSet
+          Conf:
+            IBOX_RESNAME: RecordSet
+            IBOX_LINKED_OBJ_NAME: IBOX_RESNAME
+          Type: RDS
+          For: ["External", "Internal"]
+        IBOX_PARAMETER:
+          - IBOX_MAPNAME.AllocatedStorage:
+              Description: 'Storage Size in GB - empty for mapped value'
+          - IBOX_MAPNAME.MaxAllocatedStorage:
+              Description: 'Max Storage Size in GB (Enable Storage Autoscaling)- empty for mapped value - 0 to disable'
+          - IBOX_MAPNAME.DBInstanceClass:
+              Description: 'Instance Type - empty for mapped value'
+              AllowedValues: [
+                '', 'db.m3.medium', 'db.m3.large', 'db.m3.xlarge', 'db.m3.2xlarge',
+                'db.m4.large', 'db.m4.xlarge', 'db.m4.2xlarge', 'db.m4.4xlarge', 'db.m4.10xlarge',
+                'db.m5.large', 'db.m5.xlarge', 'db.m5.2xlarge', 'db.m5.4xlarge', 'db.m5.12xlarge',
+                'db.r3.large', 'db.r3.xlarge', 'db.r3.2xlarge', 'db.r3.4xlarge', 'db.r3.8xlarge',
+                'db.r5.large', 'db.r5.xlarge', 'db.r5.2xlarge', 'db.r5.4xlarge', 'db.r5.12xlarge',
+                'db.t2.micro', 'db.t2.small', 'db.t2.medium', 'db.t2.large',
+                'db.t3.micro', 'db.t3.small', 'db.t3.medium', 'db.t3.large']
+          - IBOX_MAPNAME.DBName:
+              Description: 'Empty for mapped value'
+          - IBOX_MAPNAME.DBSnapshotIdentifier:
+              Description: 'DB snapshot used to restore the DB instance - "none" for not using one - empty for mapped value'
+          - IBOX_MAPNAME.DeletionProtection:
+              Description: 'empty for mapped value'
+              AllowedValues: ['', 'true', 'false']
+          - IBOX_MAPNAME.SourceDBInstanceIdentifier:
+              Description: 'ID of the source DB instance to create ReadReplica - "none" for not using one - empty for mapped value'
+          - IBOX_MAPNAME.Engine:
+              Description: 'Engine - empty for mapped value'
+              AllowedValues: [
+                '', 'mysql', 'mariadb', 'oracle-se1', 'oracle-se2', 'oracle-se', 'oracle-ee',
+                'sqlserver-ee', 'sqlserver-se', 'sqlserver-ex', 'sqlserver-web', 'postgres', 'aurora'
+              ]
+          - IBOX_MAPNAME.EngineVersion:
+              Description: 'Engine Version - empty for mapped value'
+          - IBOX_MAPNAME.MasterUsername:
+              Description: 'Username - empty for mapped value'
+          - IBOX_MAPNAME.MasterUserPassword:
+              Description: 'Password - empty for mapped value'
+              NoEcho: true
+          - IBOX_MAPNAME.MonitoringInterval:
+              Description: 'The interval, in seconds, for Enhanced Monitoring metrics - empty for mapped value - 0 to disable'
+              AllowedValues: ['', '0', '1', '5', '10', '15', '30', '60']
+          - IBOX_MAPNAME.MultiAZ:
+              Description: 'Use multiple Availability Zone - empty for mapped value'
+              AllowedValues: ['', 'true', 'false']
+          - IBOX_MAPNAME.PerformanceInsights:
+              Description: 'The amount of time, in days, to retain Performance Insights data - empty for mapped value - 0 to disable'
+          - IBOX_MAPNAME.StorageType:
+              Description: 'empty for mapped value'
+              AllowedValues: ['', 'standard', 'io1', 'gp2', 'gp3']
+          - IBOX_MAPNAME.StorageThroughput:
+              Description: 'empty for mapped value'
+        IBOX_CONDITION:
+          - IBOX_MAPNAME.DBSnapshotIdentifier:
+              get_condition('', 'not_equals', 'none', f'{IBOX_MAPNAME}DBSnapshotIdentifier')
+          - IBOX_MAPNAME.SourceDBInstanceIdentifier:
+              get_condition('', 'not_equals', 'none', f'{IBOX_MAPNAME}SourceDBInstanceIdentifier')
+          - IBOX_MAPNAME.DBInstanceSkipProperties:
+              Or(Condition(f'{IBOX_MAPNAME}DBSnapshotIdentifier'), Condition(f'{IBOX_MAPNAME}SourceDBInstanceIdentifier'))
+          - IBOX_MAPNAME.MonitoringInterval:
+              get_condition('', 'not_equals', '0', f'{IBOX_MAPNAME}MonitoringInterval')
+          - IBOX_MAPNAME.PerformanceInsights:
+              get_condition('', 'not_equals', '0', f'{IBOX_MAPNAME}PerformanceInsights')
+          - IBOX_MAPNAME.StorageAutoScaling:
+              get_condition('', 'not_equals', '0', f'{IBOX_MAPNAME}MaxAllocatedStorage')
+          - IBOX_MAPNAME.StorageThroughput:
+              get_condition('', 'not_equals', '0', f'{IBOX_MAPNAME}StorageThroughput')
+        IBOX_OUTPUT:
+          - IBOX_MAPNAME.AllocatedStorage:
+              Value: ${AllocatedStorage}
+          - IBOX_MAPNAME.MaxAllocatedStorage:
+              Value: ${MaxAllocatedStorage}
+          - IBOX_MAPNAME.DBInstanceClass:
+              Value: ${DBInstanceClass}
+          - IBOX_MAPNAME.DBName:
+              Value: ${DBName}
+          - IBOX_MAPNAME.DBSnapshotIdentifier:
+              Value: ${DBSnapshotIdentifier}
+          - IBOX_MAPNAME.DeletionProtection:
+              Value: ${DeletionProtection}
+          - IBOX_MAPNAME.Engine:
+              Value: ${Engine}
+          - IBOX_MAPNAME.EngineVersion:
+              Value: ${EngineVersion}
+          - IBOX_MAPNAME.MasterUsername:
+              Value: ${MasterUsername}
+          - IBOX_MAPNAME.MonitoringInterval:
+              Value: ${MonitoringInterval}
+          - IBOX_MAPNAME.MultiAZ:
+              Value: ${MultiAZ}
+          - IBOX_MAPNAME.PerformanceInsightsRetentionPeriod:
+              Value: ${PerformanceInsightsRetentionPeriod}
+          - IBOX_MAPNAME.PubliclyAccessible:
+              Value: ${PubliclyAccessible}
+          - IBOX_MAPNAME.SourceDBInstanceIdentifier:
+              Value: ${SourceDBInstanceIdentifier}
+          - IBOX_MAPNAME.StorageType:
+              Value: ${StorageType}
+          - IBOX_MAPNAME.StorageThroughput:
+              Value: ${StorageThroughput}
+        AllocatedStorage: 50
+        AllowMajorVersionUpgrade: true
+        DBInstanceClass: db.t3.micro
+        DBName: dbname
+        DBParameterGroupName: Ref('DBParameterGroup1')
+        DBSnapshotIdentifier: none
+        DeletionProtection: false
+        EnablePerformanceInsights:
+          If(f'{IBOX_MAPNAME}PerformanceInsights', True, False)
+        MasterUsername: masterusername
+        MasterUserPassword: masteruserpassword
+        MaxAllocatedStorage: 0
+        MaxAllocatedStorage.IBOX_CODE:
+          If(f'{IBOX_MAPNAME}StorageAutoScaling', get_endvalue(f'{IBOX_MAPNAME}MaxAllocatedStorage'), Ref('AWS::NoValue'))
+        MonitoringInterval: 0
+        MonitoringRoleArn: If(f'{IBOX_MAPNAME}MonitoringInterval', get_expvalue('RoleRDSEnhancedMonitoring'), Ref('AWS::NoValue'))
+        MultiAZ: false
+        PerformanceInsights: 0
+        PerformanceInsightsRetentionPeriod:
+          If(f'{IBOX_MAPNAME}PerformanceInsights', get_endvalue(f'{IBOX_MAPNAME}PerformanceInsights'), Ref('AWS::NoValue'))
+        SourceDBInstanceIdentifier: none
+        StorageThroughput.IBOX_CODE:
+          If(f'{IBOX_MAPNAME}StorageThroughput', get_endvalue(f'{IBOX_MAPNAME}StorageThroughput'), Ref('AWS::NoValue'))
+        StorageThroughput: 0
+        StorageType: gp3
+        VPCSecurityGroups:
+          - Ref(f'SecurityGroup{IBOX_MAPNAME}')
+
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/res-base/ecs_draininstance.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml`

 * *Files 0% similar despite different names*

```diff
@@ -44,21 +44,22 @@
 
 global:
   Lambda:
     - ECSDrainInstance:
         IBOX_LINKED_OBJ:
           Role:
             Conf: *policies_lambda_ecs_drain_instance
+        Architectures:
+          - arm64
         Code:
           ZipFile: str(IBOX_INDEXNAME)
         Description: 'Gracefully drain ECS tasks from EC2 instances before the instances are terminated by autoscaling.'
         Environment:
           Variables:
             - SQSQueue: Ref("SQSQueueECSDrainInstance")
-        MemorySize: 128
         Runtime: python3.9
         Timeout: 29
   LambdaEventSourceMapping:
     - ECSDrainInstance:
         DependsOn: 'RoleLambdaECSDrainInstance'
         BatchSize: 1
         EventSourceArn: GetAtt('SQSQueueECSDrainInstance', 'Arn')
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/res-base/ecs_runtask.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml`

 * *Files 3% similar despite different names*

```diff
@@ -32,13 +32,14 @@
         Value: Ref('RoleLambdaECSRunTask')
         Export: Export('RoleLambdaECSRunTask')
   Lambda:
     - ECSRunTask:
         IBOX_LINKED_OBJ:
           Role:
             Conf: *policies_iamrole_lamba_ecs_runtask
+        Architectures:
+          - arm64
         Code:
           ZipFile: str(IBOX_INDEXNAME)
         Description: 'Run ECS Task'
-        MemorySize: 128
         Runtime: python3.9
         Timeout: 60
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/res-base/role.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/iam/roles.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/res-base/securitygroup_base.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/res-event/cluster-autoscale.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/events/cluster-autoscale.yml`

 * *Files 3% similar despite different names*

```diff
@@ -7,19 +7,20 @@
        ScheduleExpression: 'cron(*/2 * * * ? *)'
        Targets:
          - Lambda0:
              Arn: GetAtt('LambdaECSClusterAutoscale', 'Arn')
              Id: 'TargetFunction-01'
   Lambda:
     - ECSClusterAutoscale:
+        Architectures:
+          - arm64
         Code:
           ZipFile: str(IBOX_INDEXNAME)
         Export: True
         Description: 'Lambda to automatically reduce and ECS Cluster'
-        MemorySize: 128
         Runtime: python3.9
         Timeout: 65
   IAMPolicy:
     - LambdaECSClusterAutoscale:
         Roles:
           - Ref('RoleLambdaECSClusterAutoscale')
         PolicyDocument:
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/res-event/event_cw-alarm.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 IBoxLoader:
   - !include
-    - lambda/layers.yml
+    - com/lambda/layers.yml
 
 global:
   EventsRule:
     - CloudWatchRepeatedNotify:
         IBOX_SOURCE_OBJ: EventsRuleTargetLambda
         Description: 'Schedule check for alarms in ALARM state and notify'
         State: 'DISABLED'
@@ -35,29 +35,27 @@
     - CloudWatchRepeatedNotify:
         Architectures: ['arm64']
         Description: 'CloudWatch Repeated Notify'
         Code:
           ZipFile: str(IBOX_INDEXNAME)
         Layers:
           - LambdaLayerVersionPython37SSM
-        MemorySize: 128
         Runtime: python3.9
         Timeout: 30
         Environment:
           Variables:
             - SNSTopic: get_expvalue('SNSTopicCloudWatchAlarm')
     - CloudWatchAlarmStateChange:
         IBOX_ENABLED: False
         Architectures: ['arm64']
         Description: 'CloudWatch Alarm State change to Alarm'
         Code:
           ZipFile: str(IBOX_INDEXNAME)
         Layers:
           - LambdaLayerVersionPython37SSM
-        MemorySize: 128
         Runtime: python3.9
         Timeout: 30
   IAMPolicy:
     - LambdaCloudWatchRepeatedNotify:
         Roles:
           - Ref('RoleLambdaCloudWatchRepeatedNotify')
         PolicyDocument:
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/res-event/event_ec2.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/events/ec2.yml`

 * *Files 4% similar despite different names*

```diff
@@ -51,54 +51,60 @@
             - aws.ec2
         Targets:
           - LambdaECSDrainTasks:
               Arn: GetAtt('LambdaECSDrainTasks', 'Arn')
               Id: 'TargetFunction-01'
   Lambda:
     - EC2StartStopTagged:
+        Architectures:
+          - arm64
         Code:
           ZipFile: str(IBOX_INDEXNAME)
         Description: 'Start and Stop EC2 Tagged Instances'
-        MemorySize: 128
         Runtime: python3.9
         Timeout: 10
         Environment:
           Variables:
             - TagName: 'AutoStartStop'
     - ECSDrainTasks:
+        Architectures:
+          - arm64
         Code:
           ZipFile: str(IBOX_INDEXNAME)
         Description: 'Drain and stop Tasks from ECS container spot instances scheduled for termination'
-        MemorySize: 128
         Runtime: python3.9
         Timeout: 300
     - ServiceDiscovery:
+        Architectures:
+          - arm64
         Code:
           ZipFile: str(IBOX_INDEXNAME)
         Description: 'ServiceDiscovery'
-        MemorySize: 128
-        Runtime: python3.9
-        Timeout: 30
         Environment:
           Variables:
             - NameSpaceID: get_expvalue('ServiceDiscoveryPublicDnsNamespaceId')
             - PublicDnsNamespaceName: Sub(f'find.{cfg.HostedZoneNameEnv}')
             - HostedZoneId: get_expvalue('HostedZoneIdEnv')
+        MemorySize: 256
+        Runtime: python3.9
+        Timeout: 30
     - R53RecordInstanceId:
+        Architectures:
+          - arm64
         Code:
           ZipFile: str(IBOX_INDEXNAME)
         Description: 'R53 Record InstanceId Automatic Creation'
-        MemorySize: 128
-        Runtime: python3.9
-        Timeout: 30
         Environment:
           Variables:
             - HostedZoneName: get_endvalue('HostedZoneNamePrivate')
             - HostedZoneId: get_expvalue('HostedZoneIdPrivate')
             - Topic: Ref('SNSTopicASGNotificationR53')
+        MemorySize: 256
+        Runtime: python3.9
+        Timeout: 30
   LambdaPermission:
     - EC2StartStopTaggedEventsRuleEC2StartTagged:
         FunctionName: GetAtt('LambdaEC2StartStopTagged', 'Arn')
         Principal: events.amazonaws.com
         SourceArn: GetAtt("EventsRuleEC2StartTagged", 'Arn')
     - EC2StartStopTaggedEventsRuleEC2StopTagged:
         FunctionName: GetAtt('LambdaEC2StartStopTagged', 'Arn')
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/res-event/event_ecs-spot.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/events/ecs-spot.yml`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,9 @@
-IBoxLoader:
-  - !include
-    - lambda/layers.yml
-
 global:
   EventsRule:
-    - ECSEventServiceFailure:
-        IBOX_SOURCE_OBJ: EventsRuleTargetLambda
-        Description: 'ECSEventsSpot Lambda Trigger for Cpu and Memory Failure'
-        State: 'DISABLED'
-        EventPattern:
-          detail:
-            eventType:
-              - ERROR
-            eventName:
-              - SERVICE_TASK_PLACEMENT_FAILURE
-            reason:
-              - 'RESOURCE:MEMORY'
-              - 'RESOURCE:CPU'
-          detail-type:
-            - ECS Service Action
-          source:
-            - aws.ecs
-        Targets:
-          - Lambda0:
-              Arn: GetAtt('LambdaECSEventsSpot', 'Arn')
-              Id: TargetFunction-01
     - ECSEventsSpot:
         IBOX_SOURCE_OBJ: EventsRuleTargetLambda
         Description: 'ECSEventsSpot Lambda Trigger for Task Spot RUNNING'
         State: 'DISABLED'
         EventPattern:
           detail:
             capacityProviderName:
@@ -85,41 +60,27 @@
             - aws.ecs
         Targets:
           - Lambda0:
               Arn: GetAtt('LambdaECSEventsSpot', 'Arn')
               Id: TargetFunction-01
   Lambda:
     - ECSEventsSpot:
+        Architectures:
+          - arm64
         Description: 'ECSEventsSpot'
         Code:
-          S3Bucket: Sub(cfg.BucketNameAppRepository)
-          S3Key: ibox-tools/ecs-events/master-444dd76.zip
-        Layers:
-          - LambdaLayerVersionPython37SSM
-        MemorySize: 128
+          ZipFile: str(IBOX_INDEXNAME)
         Runtime: python3.9
         Timeout: 30
-        Environment:
-          Variables:
-            - SNSTopic: get_expvalue('SNSTopicCloudWatchAlarm')
   IAMPolicy:
     - LambdaECSEventsSpot:
         Roles:
           - Ref('RoleLambdaECSEventsSpot')
         PolicyDocument:
           Statement:
             - 1:
                 Action:
                   - 'ecs:DescribeContainerInstances'
                   - 'ecs:DescribeServices'
                   - 'ecs:UpdateService'
-                  - 'cloudwatch:SetAlarmState'
-                  - 'cloudwatch:DisableAlarmActions'
-                  - 'cloudwatch:EnableAlarmActions'
-                  - 'events:PutRule'
-                  - 'events:DeleteRule'
-                  - 'events:PutTargets'
-                  - 'events:RemoveTargets'
-                  - 'lambda:AddPermission'
-                  - 'lambda:RemovePermission'
                 Effect: Allow
                 Resource: '*'
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/res-event/event_ecs.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/events/ecs.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 IBoxLoader:
   - !include
-    - lambda/layers.yml
-    #- res-event/event_ecs-spot.yml
+    - com/lambda/layers.yml
+    #- com/events/ecs-spot.yml
 
 global:
   EventsRule:
     - ECSEventTaskStateChange:
         IBOX_SOURCE_OBJ: EventsRuleTargetLambda
         Description: 'ECSEvents Lambda Trigger for Task STOPPED'
         State: 'DISABLED'
@@ -23,21 +23,22 @@
             - aws.ecs
         Targets:
           - Lambda0:
               Arn: GetAtt('LambdaECSEventTaskStateChange', 'Arn')
               Id: TargetFunction-01
   Lambda:
     - ECSEventTaskStateChange:
+        Architectures:
+          - arm64
         Description: 'ECSEventTaskStateChange'
         Code:
           ZipFile: str(IBOX_INDEXNAME)
         Layers:
           - LambdaLayerVersionPython37SSM
-          - LambdaLayerVersionPython39SlackClient
-        MemorySize: 128
+          - LambdaLayerVersionPythonArm64SlackClient
         Runtime: python3.9
         Timeout: 30
         Environment:
           Variables:
             - SNSTopic: get_expvalue('SNSTopicCloudWatchAlarm')
   IAMPolicy:
     - LambdaECSEventTaskStateChange:
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/res-event/spot_advisor.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/events/spot_advisor.yml`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,20 @@
        ScheduleExpression: 'cron(16 * * * ? *)'
        Targets:
          - Lambda0:
              Arn: GetAtt('LambdaSpotAdvisor', 'Arn')
              Id: 'TargetFunction-01'
   Lambda:
     - SpotAdvisor:
+        Architectures:
+          - arm64
         Code:
           S3Bucket: Sub(cfg.BucketNameAppRepository)
           S3Key: ibox-tools/spot-advisor/spot-advisor.zip
         Description: 'Advise if ASG is using a spot instance type with a high frequency of interruption'
-        MemorySize: 128
         Runtime: python3.9
         Timeout: 300
         Environment:
           Variables:
             - SNSTopic: get_expvalue('SNSTopicCloudWatchAlarm')
   IAMPolicy:
     - LambdaSpotAdvisor:
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/res-extra/asgnotificationr53.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/res-extra/cloudformation_stackset.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/res-s3/logs.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/com/s3/bucket-log.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/route53/hostedzones.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/route53/hostedzones.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Base: &base
-  IBOX_RESNAME: HostedZone.IBOX_INDEXNAME
-  Enabled: 'no'
-  Id: none
-  IBOX_OUTPUT:
-    - HostedZoneName.IBOX_INDEXNAME:
-        Condition: None
-        Value: get_endvalue(f"Route53{IBOX_RESNAME}Name")
-
 Public: &public
   IBOX_PARAMETER:
     - Route53.IBOX_RESNAME.Enabled:
         Description: 'Create Zone - can be created in only one Region - empty for default based on mapping'
     - Route53.IBOX_RESNAME.Id:
         Description: 'Id of Zone - required in all Regions where zone is not created - empty for default based on mapping'
   IBOX_CONDITION:
@@ -29,15 +20,14 @@
         Condition: None
         Value: Ref(IBOX_RESNAME)
         Export: Export(f"HostedZoneId{IBOX_INDEXNAME}")
 
 
 global:
   Route53HostedZone:
-    - IBOX_BASE: *base
     - Env:
         <<: *public
         HostedZoneConfig:
           Comment: Sub('${EnvShort} public zone')
         Name: Sub(cfg.HostedZoneNameEnv)
     - EnvExtra1:
         <<: *public
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/route53/recordset.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/route53/recordsets.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/s3/bucket-policy.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/s3/bucket-policies.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 global:
   S3BucketPolicy:
     - Base:
+        IBOX_ENABLED: False
         PolicyDocument:
           Statement:
             - IBOX_LIST:
             - Base:
                 Action:
                   - "s3:GetBucketLocation"
                 Effect: Allow
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/s3/bucket.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/s3/ibox_base.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 IBoxLoader: !include
-  - bucket-policy.yml
-  - iam/policy-bucket-replica.yml
+  - res/s3/bucket-policies.yml
+  - com/iam/policy-bucket-replica.yml
 
 global:
   S3Bucket:
     - IBOX_BASE:
         IBOX_TITLE: Bucket.IBOX_INDEXNAME
         IBOX_CUSTOM_OBJ:
           - PolicyStatementCloudFrontOriginAccessIdentityPrincipal:
```

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/scheduler/ibox_base.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/scheduler/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/sns/subscription.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/sns/subscriptions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg/BASE/sqs/queue-policy.yml` & `awsibox-0.8.0/awsibox/cfg/ibox/res/sqs/queue-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cfg.py` & `awsibox-0.8.0/awsibox/cfg.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,27 +11,30 @@
 Conditions = {}
 Mappings = {}
 Resources = {}
 Outputs = {}
 
 OBJS = {}
 
-PATH_INT = os.path.join(os.path.dirname(os.path.realpath(__file__)), "cfg")
+APP_DIR = os.path.dirname(os.path.realpath(__file__))
+
+PATH_INT = os.path.join(APP_DIR, "cfg")
 PATH_INT = os.path.normpath(PATH_INT)
 
 PATH_EXT = os.path.join(cwd, "cfg")
 PATH_EXT = os.path.normpath(PATH_EXT)
 
+IBOX_BRAND_DIR = "ibox"
+STACKS_DIR = "stacks"
+
 STACK_TYPES = [
     "agw",
-    "alb",
     "cch",
     "clf",
     "ec2",
-    "ecr",
     "ecs",
     "rds",
     "res",
     "tsk",
     "lbd",
 ]
 
@@ -533,14 +536,16 @@
         "func": ("servicediscovery", "Service"),
     },
     "SchedulerSchedule": {
         "module": "joker",
         "func": ("scheduler", "Schedule"),
         "dep": ["SecurityGroups"],
     },
+    "SSOPermissionSet": {"module": "joker", "func": ("sso", "PermissionSet")},
+    "SSOAssignment": {"module": "joker", "func": ("sso", "Assignment")},
     "SQSQueue": {"module": "joker", "func": ("sqs", "Queue")},
     "SQSQueuePolicy": {
         "module": "joker",
         "func": ("sqs", "QueuePolicy"),
         "dep": ["SNSSubscription"],
     },
     "SNSSubscription": {"module": "joker", "func": ("sns", "SubscriptionResource")},
```

### Comparing `awsibox-0.7.8/awsibox/cloudformation.py` & `awsibox-0.8.0/awsibox/cloudformation.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/cloudfront.py` & `awsibox-0.8.0/awsibox/cloudfront.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/common.py` & `awsibox-0.8.0/awsibox/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import json
 import logging
 from pprint import pprint, pformat
 from pathlib import PurePath
 from troposphere import validators
 from troposphere.autoscaling import Tags as asgTags
 import troposphere.ssm as ssm
+import troposphere.sso as sso
 
 from troposphere import (
     And,
     AWSHelperFn,
     AWSObject,
     AWSProperty,
     PropsDictType,
@@ -43,14 +44,16 @@
 from . import cfg
 
 from .cfg import (
     MAX_SECURITY_GROUPS,
     SECURITY_GROUPS_DEFAULT,
 )
 
+# Temporary fix for https://github.com/cloudtools/troposphere/issues/2146
+sso.PermissionSet.props["InlinePolicy"] = (str, False)
 
 # Temporary fix for https://github.com/cloudtools/troposphere/issues/1474
 def my_one_of(class_name, properties, property, conditionals):
     if properties.get(property) not in conditionals and not isinstance(
         properties.get(property), If
     ):
         raise ValueError(
```

### Comparing `awsibox-0.7.8/awsibox/discover.py` & `awsibox-0.8.0/awsibox/discover.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,47 @@
 import sys
 import os
 import mmap
 
 from . import cfg
 
 
-def get_brands():
-    brand_int = os.listdir(cfg.PATH_INT)
-    brand_ext = os.listdir(cfg.PATH_EXT)
-
-    brands = set(brand_int + brand_ext)
-
-    brands.remove("BASE")
-
-    return brands
-
-
 def build_discover_map(brand, stacktypes, envroles):
     if not stacktypes and not envroles:
         # include all roles in all stacktypes
         stacktypes = cfg.STACK_TYPES
 
     roles = []
 
-    path_int = os.path.join(cfg.PATH_INT, brand)
-    path_ext = os.path.join(cfg.PATH_EXT, brand)
+    path_int = os.path.join(cfg.PATH_INT, brand, cfg.STACKS_DIR)
+    path_ext = os.path.join(cfg.PATH_EXT, brand, cfg.STACKS_DIR)
 
     for n in [path_int, path_ext]:
         for root, directories, filenames in os.walk(n, topdown=True):
             try:
                 directories.remove("UNUSED")
             except Exception:
                 pass
             for filename in filenames:
-                root_dir = os.path.basename(root)
-                stacktype = root_dir.lower()
+                stacktype = os.path.basename(root)
                 role = os.path.splitext(os.path.basename(filename))[0]
                 if (
-                    root_dir.isupper()
-                    and not filename.startswith(".")
-                    and not filename == "TYPE.yml"
+                    not filename.startswith(".")
+                    and not filename == "i_type.yml"
                     and (stacktype in stacktypes or role in envroles)
                 ):
                     roles.append((stacktype, role))
 
-    if brand == "BASE":
+    if brand == cfg.IBOX_BRAND_DIR:
+        # add all roles found in ibox conf to all other brands
         for n in ext_brands:
-            add_to_map(n, roles)
+            if n != cfg.IBOX_BRAND_DIR:
+                add_to_map(n, roles)
     else:
+        # add roles to brand
         add_to_map(brand, roles)
 
 
 def add_to_map(brand, roles):
     global discover_map
 
     try:
@@ -65,16 +55,14 @@
     global ext_brands
 
     discover_map = {}
 
     if brands:
         ext_brands = list(brands)
     else:
-        ext_brands = get_brands()
-        brands = list(ext_brands)
-
-    brands.append("BASE")
+        ext_brands = os.listdir(cfg.PATH_EXT)
 
-    for brand in brands:
+    # cycle on external brands + ibox one
+    for brand in set(ext_brands + [cfg.IBOX_BRAND_DIR]):
         build_discover_map(brand, stacktypes, envroles)
 
     return discover_map
```

### Comparing `awsibox-0.7.8/awsibox/ec2.py` & `awsibox-0.8.0/awsibox/ec2.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/ecr.py` & `awsibox-0.8.0/awsibox/ecr.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,16 @@
 
 # ##########################################
 # ### END STACK META CLASSES AND METHODS ###
 # ##########################################
 
 
 def ECR_Repositories(key):
+    if not getattr(cfg, key):
+        return
     PolicyStatementAccounts = []
     for n, v in cfg.EcrAccount.items():
         mapname = f"EcrAccount{n}Id"  # Ex. EcrAccountPrdId
         # conditions
         add_obj(get_condition(mapname, "not_equals", "none"))
 
         if "Pull" in v["Policy"]:
```

### Comparing `awsibox-0.7.8/awsibox/ecs.py` & `awsibox-0.8.0/awsibox/ecs.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/efs.py` & `awsibox-0.8.0/awsibox/efs.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/elasticloadbalancing.py` & `awsibox-0.8.0/awsibox/elasticloadbalancing.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/generate.py` & `awsibox-0.8.0/awsibox/generate.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/iam.py` & `awsibox-0.8.0/awsibox/iam.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,14 +83,16 @@
         r_GroupAdd = iam.UserToGroupAddition(resname, GroupName=n, Users=Users)
 
         add_obj([r_GroupAdd])
 
 
 def IAM_Groups(key):
     for n, v in getattr(cfg, key).items():
+        if not v.get("IBOX_ENABLED", True):
+            continue
         resname = f"{key}{n}"  # Ex. IAMGroupBase
 
         # conditions
         add_obj(get_condition(resname, "equals", "yes", f"{resname}Enabled"))
 
         ManagedPolicyArns = []
         for m in v["ManagedPolicyArns"]:
```

### Comparing `awsibox-0.7.8/awsibox/joker.py` & `awsibox-0.8.0/awsibox/joker.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,23 +42,15 @@
             RP_to_cfg(source_obj_conf, prefix=mapname, mappedvalues=cfg.mappedvalues)
             v = merge_dict(v, source_obj_conf)
             # Uncomment to use old method: auto_get_props
             # auto_get_props(obj, mapname=source_obj, indexname=n)
             # #reset obj title, if changed by IBOX_TITLE key
             # obj.title = resname
 
-        # populate obj
-        auto_get_props(
-            obj,
-            mapname=mapname,
-            indexname=n,
-            linked_obj_name=linked_obj_name,
-            linked_obj_index=linked_obj_index,
-        )
-
+        # autocreate condition
         if v.get("Create"):
             add_obj(
                 Parameter(
                     f"{resname}Create",
                     Description=f"Create {resname}",
                     AllowedValues=["", "yes", "no"],
                 )
@@ -71,8 +63,17 @@
                         Condition=resname,
                         Value=Ref(v.get("IBOX_TITLE", resname)),
                     )
                 )
                 if not hasattr(obj, "Condition"):
                     obj.Condition = resname
 
+        # populate obj
+        auto_get_props(
+            obj,
+            mapname=mapname,
+            indexname=n,
+            linked_obj_name=linked_obj_name,
+            linked_obj_index=linked_obj_index,
+        )
+
         add_obj(obj)
```

### Comparing `awsibox-0.7.8/awsibox/lambdas/ASGSpot.code` & `awsibox-0.8.0/awsibox/lambdas/ASGSpot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/lambdas/AtEdgeAddHeaders.code` & `awsibox-0.8.0/awsibox/lambdas/AtEdgeAddHeaders.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/lambdas/CCRLightHouse.code` & `awsibox-0.8.0/awsibox/lambdas/CCRLightHouse.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/lambdas/CloudWatchAlarmStateChange.code` & `awsibox-0.8.0/awsibox/lambdas/CloudWatchAlarmStateChange.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/lambdas/CloudWatchRepeatedNotify.code` & `awsibox-0.8.0/awsibox/lambdas/CloudWatchRepeatedNotify.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/lambdas/EC2StartStopTagged.code` & `awsibox-0.8.0/awsibox/lambdas/EC2StartStopTagged.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/lambdas/ECSClusterAutoscale.code` & `awsibox-0.8.0/awsibox/lambdas/ECSClusterAutoscale.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/lambdas/ECSDrainInstance.code` & `awsibox-0.8.0/awsibox/lambdas/ECSDrainInstance.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/lambdas/ECSDrainTasks.code` & `awsibox-0.8.0/awsibox/lambdas/ECSDrainTasks.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/lambdas/ECSEventTaskStateChange.code` & `awsibox-0.8.0/awsibox/lambdas/ECSEventTaskStateChange.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/lambdas/ECSRunTask.code` & `awsibox-0.8.0/awsibox/lambdas/ECSRunTask.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/lambdas/ECSUpdateDesiredCount.code` & `awsibox-0.8.0/awsibox/lambdas/ECSUpdateDesiredCount.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/lambdas/ElasticSearchSnapShot.code` & `awsibox-0.8.0/awsibox/lambdas/ElasticSearchSnapShot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/lambdas/ManageService.code` & `awsibox-0.8.0/awsibox/lambdas/ManageService.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/lambdas/PaidApi.code` & `awsibox-0.8.0/awsibox/lambdas/PaidApi.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/lambdas/Python37SSM.layer` & `awsibox-0.8.0/awsibox/lambdas/Python37SSM.layer`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/lambdas/R53RecordInstanceId.code` & `awsibox-0.8.0/awsibox/lambdas/R53RecordInstanceId.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/lambdas/ServiceDiscovery.code` & `awsibox-0.8.0/awsibox/lambdas/ServiceDiscovery.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/lambdas/ServiceUnavailable.code` & `awsibox-0.8.0/awsibox/lambdas/ServiceUnavailable.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/lambdas/StacksOps.code` & `awsibox-0.8.0/awsibox/lambdas/StacksOps.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/mappings.py` & `awsibox-0.8.0/awsibox/mappings.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/rds.py` & `awsibox-0.8.0/awsibox/rds.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/s3.py` & `awsibox-0.8.0/awsibox/s3.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/shared.py` & `awsibox-0.8.0/awsibox/shared.py`

 * *Files 1% similar despite different names*

```diff
@@ -699,16 +699,19 @@
                 except Exception as e:
                     # logging.warning(f"Resource with missing properties: {obj_propname}\n\t\t{e}")
                     prop_obj = None
             elif prop_class.__name__ == "dict":
                 prop_obj = get_dictvalue(key[obj_propname])
             elif prop_class.__name__ == "Tags":
                 prop_obj = _get_obj_tags()
-            elif prop_class.__name__ == "str" and obj_propname == "LifecyclePolicyText":
-                # str but can be represented as dict Ex. ECR LifecyclePolicyText
+            elif prop_class.__name__ == "str" and obj_propname in [
+                "LifecyclePolicyText",
+                "InlinePolicy",
+            ]:
+                # str but can be represented as dict Ex. ECR LifecyclePolicyText, SSO InlinePolicy
                 prop_obj = json.dumps(get_dictvalue(key[obj_propname]))
 
             return prop_obj
 
         # obj_propname is are Tropo Tags
         elif (
             isinstance(prop_class, tuple)
```

### Comparing `awsibox-0.7.8/awsibox/user-data/SCRIPTS/ELBCHECK.sh` & `awsibox-0.8.0/awsibox/user-data/SCRIPTS/ELBCHECK.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/user-data/SCRIPTS/END.sh` & `awsibox-0.8.0/awsibox/user-data/SCRIPTS/END.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/user-data/SCRIPTS/INIT.sh` & `awsibox-0.8.0/awsibox/user-data/SCRIPTS/INIT.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/user-data/SCRIPTS/PACKAGE.sh` & `awsibox-0.8.0/awsibox/user-data/SCRIPTS/PACKAGE.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/user-data/SCRIPTS/SERVICE.sh` & `awsibox-0.8.0/awsibox/user-data/SCRIPTS/SERVICE.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/user-data/SCRIPTS/SETUP.sh` & `awsibox-0.8.0/awsibox/user-data/SCRIPTS/SETUP.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/user-data/ecs-cluster.sh` & `awsibox-0.8.0/awsibox/user-data/ecs-cluster.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/awsibox/waf.py` & `awsibox-0.8.0/awsibox/waf.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.7.8/build/lib/awsibox.egg-info/PKG-INFO` & `awsibox-0.8.0/build/lib/awsibox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsibox
-Version: 0.7.8
+Version: 0.8.0
 Summary: AWS Infrastructure in a Box
 Home-page: https://github.com/mello7tre/AwsIBox
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Description: # AwsIBox
         AwsIBox - **AWS** **I**nfrastructure in a **Box**
```

### Comparing `awsibox-0.7.8/build/lib/awsibox.egg-info/SOURCES.txt` & `awsibox-0.8.0/build/lib/awsibox.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -26,173 +26,184 @@
 awsibox/iam.py
 awsibox/joker.py
 awsibox/mappings.py
 awsibox/rds.py
 awsibox/s3.py
 awsibox/shared.py
 awsibox/waf.py
-awsibox/cfg/BASE/CloudFormationResourceSpecification.json
-awsibox/cfg/BASE/common.yml
-awsibox/cfg/BASE/AGW/TYPE.yml
-awsibox/cfg/BASE/AGW/infra-info.yml
-awsibox/cfg/BASE/CCH/TYPE.yml
-awsibox/cfg/BASE/CLF/TYPE.yml
-awsibox/cfg/BASE/EC2/TYPE.yml
-awsibox/cfg/BASE/EC2/ecs-cluster.yml
-awsibox/cfg/BASE/ECR/TYPE.yml
-awsibox/cfg/BASE/ECS/TYPE.yml
-awsibox/cfg/BASE/ECS/buildkite.yml
-awsibox/cfg/BASE/ECS/reserve-cpu.yml
-awsibox/cfg/BASE/LBD/TYPE.yml
-awsibox/cfg/BASE/LBD/stacks-ops.yml
-awsibox/cfg/BASE/RDS/TYPE.yml
-awsibox/cfg/BASE/RES/TYPE.yml
-awsibox/cfg/BASE/RES/res-base.yml
-awsibox/cfg/BASE/RES/res-ccr-lighthouse.yml
-awsibox/cfg/BASE/RES/res-ccr-stack-replicator.yml
-awsibox/cfg/BASE/RES/res-ecs-alb.yml
-awsibox/cfg/BASE/RES/res-event-01.yml
-awsibox/cfg/BASE/RES/res-extra-01.yml
-awsibox/cfg/BASE/RES/res-iam-group-01.yml
-awsibox/cfg/BASE/RES/res-iam-policy-01.yml
-awsibox/cfg/BASE/RES/res-iam-user-01.yml
-awsibox/cfg/BASE/RES/res-lambda-layer-01.yml
-awsibox/cfg/BASE/RES/res-latedge-01.yml
-awsibox/cfg/BASE/RES/res-s3-01.yml
-awsibox/cfg/BASE/RES/vpc.yml
-awsibox/cfg/BASE/TSK/TYPE.yml
-awsibox/cfg/BASE/apigateway/account.yml
-awsibox/cfg/BASE/apigateway/deployment.yml
-awsibox/cfg/BASE/apigateway/domain-name.yml
-awsibox/cfg/BASE/apigateway/stage.yml
-awsibox/cfg/BASE/application-autoscaling/scalabletarget.yml
-awsibox/cfg/BASE/application-autoscaling/scalingpolicy.yml
-awsibox/cfg/BASE/autoscaling/autoscalinggroup.yml
-awsibox/cfg/BASE/autoscaling/capacity.yml
-awsibox/cfg/BASE/autoscaling/cloudwatch-agent.yml
-awsibox/cfg/BASE/autoscaling/ephemeral.yml
-awsibox/cfg/BASE/autoscaling/imageid-ec2.yml
-awsibox/cfg/BASE/autoscaling/imageid-ecs.yml
-awsibox/cfg/BASE/autoscaling/launchtemplate.yml
-awsibox/cfg/BASE/autoscaling/mixed_instances.yml
-awsibox/cfg/BASE/autoscaling/scalingpolicy.yml
-awsibox/cfg/BASE/autoscaling/scheduledactions.yml
-awsibox/cfg/BASE/autoscaling/spot-asg.yml
-awsibox/cfg/BASE/autoscaling/spot-auto.yml
-awsibox/cfg/BASE/cloudformation/custom-resource_light-house.yml
-awsibox/cfg/BASE/cloudfront/base.yml
-awsibox/cfg/BASE/cloudfront/custom-errors.yml
-awsibox/cfg/BASE/cloudfront/distribution.yml
-awsibox/cfg/BASE/cloudfront/for-services.yml
-awsibox/cfg/BASE/cloudfront/function.yml
-awsibox/cfg/BASE/cloudfront/lambda-function-associations.yml
-awsibox/cfg/BASE/cloudfront/origin-access-identity.yml
-awsibox/cfg/BASE/cloudfront/origin-adhoc.yml
-awsibox/cfg/BASE/cloudfront/policy.yml
-awsibox/cfg/BASE/cloudwatch/alarms.yml
-awsibox/cfg/BASE/cloudwatch/log_group.yml
-awsibox/cfg/BASE/codedeploy/deployment-group.yml
-awsibox/cfg/BASE/crm/certificate-global.yml
-awsibox/cfg/BASE/crm/certificate-regional.yml
-awsibox/cfg/BASE/crm/certificate.yml
-awsibox/cfg/BASE/dynamodb/table-credstash.yml
-awsibox/cfg/BASE/ec2/bottlerocket.yml
-awsibox/cfg/BASE/ec2/securitygroup.yml
-awsibox/cfg/BASE/ec2/vpc-endpoint.yml
-awsibox/cfg/BASE/ecr/ibox_base.yml
-awsibox/cfg/BASE/ecs/capacityprovider.yml
-awsibox/cfg/BASE/ecs/daemon-reserver-cpu.yml
-awsibox/cfg/BASE/ecs/ecs-and-cluster.yml
-awsibox/cfg/BASE/ecs/ecs-containerdefinition.yml
-awsibox/cfg/BASE/ecs/ecs-fargate-spot.yml
-awsibox/cfg/BASE/ecs/ecs-scheduled.yml
-awsibox/cfg/BASE/ecs/ecs-service.yml
-awsibox/cfg/BASE/ecs/ecs-task.yml
-awsibox/cfg/BASE/ecs/ecs-taskdefinition.yml
-awsibox/cfg/BASE/ecs/service-elasticloadbalancing.yml
-awsibox/cfg/BASE/efs/accesspoint.yml
-awsibox/cfg/BASE/efs/filesystem.yml
-awsibox/cfg/BASE/efs/volume.yml
-awsibox/cfg/BASE/elasticache/cluster-and-replication-group.yml
-awsibox/cfg/BASE/elasticache/subnet-group.yml
-awsibox/cfg/BASE/elasticloadbalancing/accountid.yml
-awsibox/cfg/BASE/elasticloadbalancing/base.yml
-awsibox/cfg/BASE/elasticloadbalancing/certificate-adhoc.yml
-awsibox/cfg/BASE/elasticloadbalancing/classic-loadbalancer.yml
-awsibox/cfg/BASE/elasticloadbalancing/hostedzoneid.yml
-awsibox/cfg/BASE/elasticloadbalancing/listener.yml
-awsibox/cfg/BASE/elasticloadbalancing/loadbalancer.yml
-awsibox/cfg/BASE/elasticloadbalancing/targetgroup.yml
-awsibox/cfg/BASE/elasticloadbalancing/v2-listener-rule.yml
-awsibox/cfg/BASE/elasticloadbalancing/v2-loadbalancer.yml
-awsibox/cfg/BASE/events/ibox_base.yml
-awsibox/cfg/BASE/iam/ecs-exec.yml
-awsibox/cfg/BASE/iam/ibox_base.yml
-awsibox/cfg/BASE/iam/instance-profile.yml
-awsibox/cfg/BASE/iam/managed-policy.yml
-awsibox/cfg/BASE/iam/parameterstore.yml
-awsibox/cfg/BASE/iam/policy-bucket-replica.yml
-awsibox/cfg/BASE/iam/policy-update_stack.yml
-awsibox/cfg/BASE/iam/role.yml
-awsibox/cfg/BASE/iam/ssm.yml
-awsibox/cfg/BASE/kms/key-and-alias.yml
-awsibox/cfg/BASE/lambda/base.yml
-awsibox/cfg/BASE/lambda/ccr-fargate-spot.yml
-awsibox/cfg/BASE/lambda/function.yml
-awsibox/cfg/BASE/lambda/ibox_base.yml
-awsibox/cfg/BASE/lambda/layer_permission.yml
-awsibox/cfg/BASE/lambda/layers.yml
-awsibox/cfg/BASE/lambda/permission.yml
-awsibox/cfg/BASE/lambda/service_unavailable.yml
-awsibox/cfg/BASE/lambda/version.yml
-awsibox/cfg/BASE/rds/db-instance.yml
-awsibox/cfg/BASE/rds/db-subnet-group.yml
-awsibox/cfg/BASE/res-base/cloudwatch_alarm.yml
-awsibox/cfg/BASE/res-base/ecs_draininstance.yml
-awsibox/cfg/BASE/res-base/ecs_runtask.yml
-awsibox/cfg/BASE/res-base/iam-managed-policy.yml
-awsibox/cfg/BASE/res-base/role.yml
-awsibox/cfg/BASE/res-base/securitygroup_base.yml
-awsibox/cfg/BASE/res-base/servicediscovery.yml
-awsibox/cfg/BASE/res-elasticloadbalancing/v2-listener.yml
-awsibox/cfg/BASE/res-event/cluster-autoscale.yml
-awsibox/cfg/BASE/res-event/event_cw-alarm.yml
-awsibox/cfg/BASE/res-event/event_ec2.yml
-awsibox/cfg/BASE/res-event/event_ecs-spot.yml
-awsibox/cfg/BASE/res-event/event_ecs.yml
-awsibox/cfg/BASE/res-event/spot_advisor.yml
-awsibox/cfg/BASE/res-extra/asgnotificationr53.yml
-awsibox/cfg/BASE/res-extra/cloudformation_stackset.yml
-awsibox/cfg/BASE/res-extra/route53_resolver.yml
-awsibox/cfg/BASE/res-s3/logs.yml
-awsibox/cfg/BASE/route53/hostedzones.yml
-awsibox/cfg/BASE/route53/recordset.yml
-awsibox/cfg/BASE/s3/bucket-policy.yml
-awsibox/cfg/BASE/s3/bucket.yml
-awsibox/cfg/BASE/scheduler/ibox_base.yml
-awsibox/cfg/BASE/sns/ibox_base.yml
-awsibox/cfg/BASE/sns/subscription.yml
-awsibox/cfg/BASE/sqs/ibox_base.yml
-awsibox/cfg/BASE/sqs/queue-policy.yml
-awsibox/cfg/BASE/ssm/parameter.yml
+awsibox/aws/CloudFormationResourceSpecification.json
+awsibox/cfg/ibox/com/common.yml
+awsibox/cfg/ibox/com/autoscaling/capacity.yml
+awsibox/cfg/ibox/com/autoscaling/cloudwatch-agent.yml
+awsibox/cfg/ibox/com/autoscaling/ephemeral.yml
+awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml
+awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml
+awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml
+awsibox/cfg/ibox/com/autoscaling/spot-asg.yml
+awsibox/cfg/ibox/com/autoscaling/spot-auto.yml
+awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml
+awsibox/cfg/ibox/com/cloudformation/custom-resource_light-house.yml
+awsibox/cfg/ibox/com/cloudfront/custom-errors.yml
+awsibox/cfg/ibox/com/cloudfront/for-services.yml
+awsibox/cfg/ibox/com/cloudfront/i_base.yml
+awsibox/cfg/ibox/com/cloudfront/origin-adhoc.yml
+awsibox/cfg/ibox/com/codedeploy/deployment-group.yml
+awsibox/cfg/ibox/com/dynamodb/table-credstash.yml
+awsibox/cfg/ibox/com/ec2/bottlerocket.yml
+awsibox/cfg/ibox/com/ec2/securitygroup.yml
+awsibox/cfg/ibox/com/ec2/securitygroups-base.yml
+awsibox/cfg/ibox/com/ecs/capacityprovider.yml
+awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml
+awsibox/cfg/ibox/com/ecs/fargate-spot.yml
+awsibox/cfg/ibox/com/ecs/service-and-cluster.yml
+awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml
+awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml
+awsibox/cfg/ibox/com/ecs/task.yml
+awsibox/cfg/ibox/com/ecs/taskdefinition-volume.yml
+awsibox/cfg/ibox/com/efs/accesspoint-app.yml
+awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml
+awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml
+awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml
+awsibox/cfg/ibox/com/elasticloadbalancing/i_base.yml
+awsibox/cfg/ibox/com/elasticloadbalancing/loadbalancer.yml
+awsibox/cfg/ibox/com/elasticloadbalancing/v2-listener.yml
+awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml
+awsibox/cfg/ibox/com/events/cluster-autoscale.yml
+awsibox/cfg/ibox/com/events/ec2.yml
+awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml
+awsibox/cfg/ibox/com/events/ecs-spot.yml
+awsibox/cfg/ibox/com/events/ecs.yml
+awsibox/cfg/ibox/com/events/spot_advisor.yml
+awsibox/cfg/ibox/com/iam/managed-policies.yml
+awsibox/cfg/ibox/com/iam/policy-bucket-replica.yml
+awsibox/cfg/ibox/com/iam/policy-ecs-exec.yml
+awsibox/cfg/ibox/com/iam/policy-parameterstore.yml
+awsibox/cfg/ibox/com/iam/policy-update_stack.yml
+awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml
+awsibox/cfg/ibox/com/iam/roles.yml
+awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml
+awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml
+awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml
+awsibox/cfg/ibox/com/lambda/ecs-runtask.yml
+awsibox/cfg/ibox/com/lambda/i_base.yml
+awsibox/cfg/ibox/com/lambda/layers.yml
+awsibox/cfg/ibox/com/lambda/py-packager.yml
+awsibox/cfg/ibox/com/lambda/service-unavailable.yml
+awsibox/cfg/ibox/com/route53/resolverendpoint-outbound.yml
+awsibox/cfg/ibox/com/s3/bucket-log.yml
+awsibox/cfg/ibox/com/servicediscovery/publicdnsnamespace-find.yml
+awsibox/cfg/ibox/com/sns/asgnotificationr53.yml
+awsibox/cfg/ibox/com/sns/cloudwatch-alarm.yml
+awsibox/cfg/ibox/com/ssm/parameter-user-password.yml
+awsibox/cfg/ibox/res/apigateway/accounts.yml
+awsibox/cfg/ibox/res/apigateway/deployments.yml
+awsibox/cfg/ibox/res/apigateway/domain-names.yml
+awsibox/cfg/ibox/res/apigateway/ibox_base.yml
+awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml
+awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml
+awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml
+awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml
+awsibox/cfg/ibox/res/autoscaling/ibox_base.yml
+awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml
+awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml
+awsibox/cfg/ibox/res/certificatemanager/ibox_base.yml
+awsibox/cfg/ibox/res/cloudfront/ibox_base.yml
+awsibox/cfg/ibox/res/cloudfront/origin-access-identities.yml
+awsibox/cfg/ibox/res/cloudfront/policies.yml
+awsibox/cfg/ibox/res/cloudwatch/alarms.yml
+awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml
+awsibox/cfg/ibox/res/cloudwatch/log_groups.yml
+awsibox/cfg/ibox/res/codedeploy/deployment-groups.yml
+awsibox/cfg/ibox/res/codedeploy/ibox_base.yml
+awsibox/cfg/ibox/res/ec2/ibox_base.yml
+awsibox/cfg/ibox/res/ec2/vpc-endpoints.yml
+awsibox/cfg/ibox/res/ecr/accounts.yml
+awsibox/cfg/ibox/res/ecr/ibox_base.yml
+awsibox/cfg/ibox/res/ecs/ibox_base.yml
+awsibox/cfg/ibox/res/ecs/services.yml
+awsibox/cfg/ibox/res/ecs/taskdefinitions.yml
+awsibox/cfg/ibox/res/efs/filesystems.yml
+awsibox/cfg/ibox/res/efs/ibox_base.yml
+awsibox/cfg/ibox/res/elasticache/ibox_base.yml
+awsibox/cfg/ibox/res/elasticache/subnet-groups.yml
+awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml
+awsibox/cfg/ibox/res/elasticloadbalancing/listeners.yml
+awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml
+awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml
+awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml
+awsibox/cfg/ibox/res/events/ibox_base.yml
+awsibox/cfg/ibox/res/iam/ibox_base.yml
+awsibox/cfg/ibox/res/iam/instance-profiles.yml
+awsibox/cfg/ibox/res/iam/managed-policies.yml
+awsibox/cfg/ibox/res/iam/roles.yml
+awsibox/cfg/ibox/res/lambda/functions.yml
+awsibox/cfg/ibox/res/lambda/ibox_base.yml
+awsibox/cfg/ibox/res/lambda/layer_permissions.yml
+awsibox/cfg/ibox/res/lambda/permissions.yml
+awsibox/cfg/ibox/res/lambda/versions.yml
+awsibox/cfg/ibox/res/rds/db-subnet-groups.yml
+awsibox/cfg/ibox/res/rds/ibox_base.yml
+awsibox/cfg/ibox/res/route53/hostedzones.yml
+awsibox/cfg/ibox/res/route53/ibox_base.yml
+awsibox/cfg/ibox/res/route53/recordsets.yml
+awsibox/cfg/ibox/res/s3/bucket-policies.yml
+awsibox/cfg/ibox/res/s3/ibox_base.yml
+awsibox/cfg/ibox/res/scheduler/ibox_base.yml
+awsibox/cfg/ibox/res/sns/ibox_base.yml
+awsibox/cfg/ibox/res/sns/subscriptions.yml
+awsibox/cfg/ibox/res/sqs/ibox_base.yml
+awsibox/cfg/ibox/res/sqs/queue-policies.yml
+awsibox/cfg/ibox/stacks/agw/i_type.yml
+awsibox/cfg/ibox/stacks/agw/infra-info.yml
+awsibox/cfg/ibox/stacks/cch/i_type.yml
+awsibox/cfg/ibox/stacks/clf/i_type.yml
+awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml
+awsibox/cfg/ibox/stacks/ec2/i_type.yml
+awsibox/cfg/ibox/stacks/ecs/buildkite.yml
+awsibox/cfg/ibox/stacks/ecs/i_type.yml
+awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml
+awsibox/cfg/ibox/stacks/lbd/i_type.yml
+awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml
+awsibox/cfg/ibox/stacks/rds/i_type.yml
+awsibox/cfg/ibox/stacks/res/i_type.yml
+awsibox/cfg/ibox/stacks/res/res-base.yml
+awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml
+awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml
+awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml
+awsibox/cfg/ibox/stacks/res/res-event-01.yml
+awsibox/cfg/ibox/stacks/res/res-extra-01.yml
+awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml
+awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml
+awsibox/cfg/ibox/stacks/res/res-iam-user-01.yml
+awsibox/cfg/ibox/stacks/res/res-lambda-layer-01.yml
+awsibox/cfg/ibox/stacks/res/res-latedge-01.yml
+awsibox/cfg/ibox/stacks/res/res-s3-01.yml
+awsibox/cfg/ibox/stacks/res/vpc.yml
+awsibox/cfg/ibox/stacks/tsk/i_type.yml
 awsibox/lambdas/ASGSpot.code
 awsibox/lambdas/AtEdgeAddHeaders.code
+awsibox/lambdas/CCRFargateSpot.code
 awsibox/lambdas/CCRLightHouse.code
+awsibox/lambdas/CCRStackReplicator.code
 awsibox/lambdas/CloudWatchAlarmStateChange.code
 awsibox/lambdas/CloudWatchRepeatedNotify.code
 awsibox/lambdas/EC2StartStopTagged.code
 awsibox/lambdas/ECSClusterAutoscale.code
 awsibox/lambdas/ECSDrainInstance.code
 awsibox/lambdas/ECSDrainTasks.code
 awsibox/lambdas/ECSEventTaskStateChange.code
+awsibox/lambdas/ECSEventsSpot.code
+awsibox/lambdas/ECSRaiseASGAlarm.code
 awsibox/lambdas/ECSRunTask.code
 awsibox/lambdas/ECSUpdateDesiredCount.code
 awsibox/lambdas/ElasticSearchSnapShot.code
+awsibox/lambdas/InfraInfo.code
 awsibox/lambdas/ManageService.code
 awsibox/lambdas/PaidApi.code
+awsibox/lambdas/PyPackager.code
 awsibox/lambdas/Python37SSM.layer
 awsibox/lambdas/R53RecordInstanceId.code
 awsibox/lambdas/ServiceDiscovery.code
 awsibox/lambdas/ServiceUnavailable.code
 awsibox/lambdas/StacksOps.code
 awsibox/user-data/ecs-cluster.sh
 awsibox/user-data/SCRIPTS/ELBCHECK.sh
```

### Comparing `awsibox-0.7.8/scripts/ibox_generate_templates.py` & `awsibox-0.8.0/scripts/ibox_generate_templates.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,16 +79,19 @@
             except Exception as e:
                 print(f"{role} generated an exception: {e}")
                 print_exc()
                 break
         for future in future_to_role:
             future.cancel()
 
+
 # read CloudFormationResourceSpecification to get CloudFormation Resources Properties
-with open(f"{cfg.PATH_INT}/BASE/CloudFormationResourceSpecification.json", "r") as cfm_res_spec_json:
+with open(
+    os.path.join(cfg.APP_DIR, "aws", "CloudFormationResourceSpecification.json"), "r"
+) as cfm_res_spec_json:
     cfg.cfm_res_spec = json.load(cfm_res_spec_json)
 
 if args.action == "view":
     discover_map = discover.discover([args.Brand], [args.EnvRole], [])
 
     cfg.brand = args.Brand
     try:
```

### Comparing `awsibox-0.7.8/setup.cfg` & `awsibox-0.8.0/setup.cfg`

 * *Files identical despite different names*

