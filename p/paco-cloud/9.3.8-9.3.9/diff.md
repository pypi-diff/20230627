# Comparing `tmp/paco-cloud-9.3.8.tar.gz` & `tmp/paco-cloud-9.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/paco-cloud-9.3.8.tar", last modified: Sat Apr 10 00:45:22 2021, max compression
+gzip compressed data, was "dist/paco-cloud-9.3.9.tar", last modified: Mon Apr 19 20:20:18 2021, max compression
```

## Comparing `paco-cloud-9.3.8.tar` & `paco-cloud-9.3.9.tar`

### file list

```diff
@@ -1,335 +1,335 @@
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/
--rw-r--r--   0 klindsay   (501) staff       (20)    35248 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/CHANGELOG.md
--rw-r--r--   0 klindsay   (501) staff       (20)      183 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/MANIFEST.in
--rw-r--r--   0 klindsay   (501) staff       (20)    47228 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/PKG-INFO
--rw-r--r--   0 klindsay   (501) staff       (20)     1669 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/README.md
--rw-r--r--   0 klindsay   (501) staff       (20)       38 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/setup.cfg
--rw-r--r--   0 klindsay   (501) staff       (20)     2170 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/setup.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/
--rw-r--r--   0 klindsay   (501) staff       (20)       65 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/__init__.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/adapters/
--rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/adapters/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1352 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/adapters/monitoring.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/application/
--rw-r--r--   0 klindsay   (501) staff       (20)     2319 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/application/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)     9282 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/application/app_engine.py
--rw-r--r--   0 klindsay   (501) staff       (20)    82461 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/application/ec2_launch_manager.py
--rw-r--r--   0 klindsay   (501) staff       (20)     6212 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/application/ec2lm_commands.py
--rw-r--r--   0 klindsay   (501) staff       (20)     3938 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/application/res_engine.py
--rw-r--r--   0 klindsay   (501) staff       (20)      316 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/application/reseng_acm.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2183 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/application/reseng_apigatewayrestapi.py
--rw-r--r--   0 klindsay   (501) staff       (20)     6489 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/application/reseng_asg.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1234 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/application/reseng_cloudfront.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1977 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/application/reseng_codedeployapplication.py
--rw-r--r--   0 klindsay   (501) staff       (20)      633 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/application/reseng_cognito.py
--rw-r--r--   0 klindsay   (501) staff       (20)      353 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/application/reseng_dashboard.py
--rw-r--r--   0 klindsay   (501) staff       (20)    54691 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/application/reseng_deploymentpipeline.py
--rw-r--r--   0 klindsay   (501) staff       (20)      340 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/application/reseng_dynamodb.py
--rw-r--r--   0 klindsay   (501) staff       (20)      330 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/application/reseng_ebs.py
--rw-r--r--   0 klindsay   (501) staff       (20)      577 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/application/reseng_ec2.py
--rw-r--r--   0 klindsay   (501) staff       (20)      602 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/application/reseng_ecrrepository.py
--rw-r--r--   0 klindsay   (501) staff       (20)      345 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/application/reseng_ecscluster.py
--rw-r--r--   0 klindsay   (501) staff       (20)     5180 2021-04-10 00:45:21.000000 paco-cloud-9.3.8/src/paco/application/reseng_ecsservices.py
--rw-r--r--   0 klindsay   (501) staff       (20)      414 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/application/reseng_efs.py
--rw-r--r--   0 klindsay   (501) staff       (20)      345 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/application/reseng_eip.py
--rw-r--r--   0 klindsay   (501) staff       (20)      396 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/application/reseng_elasticacheredis.py
--rw-r--r--   0 klindsay   (501) staff       (20)      861 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/application/reseng_elasticsearch.py
--rw-r--r--   0 klindsay   (501) staff       (20)      506 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/application/reseng_eventsrule.py
--rw-r--r--   0 klindsay   (501) staff       (20)     5324 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/application/reseng_iamuser.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2946 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/application/reseng_iotanalyticspipeline.py
--rw-r--r--   0 klindsay   (501) staff       (20)      339 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/application/reseng_iotpolicy.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2748 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/application/reseng_iottopicrule.py
--rw-r--r--   0 klindsay   (501) staff       (20)     4483 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/application/reseng_lambda.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1099 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/application/reseng_lb.py
--rw-r--r--   0 klindsay   (501) staff       (20)      363 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/application/reseng_pinpointapplication.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2051 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/application/reseng_rds.py
--rw-r--r--   0 klindsay   (501) staff       (20)      775 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/application/reseng_s3bucket.py
--rw-r--r--   0 klindsay   (501) staff       (20)      426 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/application/reseng_snstopic.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/acm/
--rw-r--r--   0 klindsay   (501) staff       (20)     7855 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/acm/ACM.py
--rw-r--r--   0 klindsay   (501) staff       (20)       43 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/acm/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)      201 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/acm/aws_helpers.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/awslambda/
--rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/awslambda/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)     3070 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/awslambda/code.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/ecs/
--rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/ecs/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)    11575 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/ecs/capacityprovider.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/iam/
--rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/iam/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2927 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/iam/user.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/iot/
--rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/iot/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)     3644 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/iot/iotpolicy.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/ssm/
--rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/ssm/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2494 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/aws_api/ssm/document.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/
--rw-r--r--   0 klindsay   (501) staff       (20)     3002 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)    24030 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/apigateway.py
--rw-r--r--   0 klindsay   (501) staff       (20)    34922 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/asg.py
--rw-r--r--   0 klindsay   (501) staff       (20)     7709 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/backup.py
--rw-r--r--   0 klindsay   (501) staff       (20)    23582 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/cftemplates.py
--rw-r--r--   0 klindsay   (501) staff       (20)    18768 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/cloudfront.py
--rw-r--r--   0 klindsay   (501) staff       (20)     4673 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/cloudtrail.py
--rw-r--r--   0 klindsay   (501) staff       (20)    22958 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/codebuild.py
--rw-r--r--   0 klindsay   (501) staff       (20)     9074 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/codecommit.py
--rw-r--r--   0 klindsay   (501) staff       (20)    13045 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/codedeploy.py
--rw-r--r--   0 klindsay   (501) staff       (20)     5111 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/codedeployapplication.py
--rw-r--r--   0 klindsay   (501) staff       (20)    52738 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/codepipeline.py
--rw-r--r--   0 klindsay   (501) staff       (20)    15220 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/cognito.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2039 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/config.py
--rw-r--r--   0 klindsay   (501) staff       (20)    19666 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/cw_alarms.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2085 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/dashboard.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1442 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/dynamodb.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1316 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/ebs.py
--rw-r--r--   0 klindsay   (501) staff       (20)     4481 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/ecr.py
--rw-r--r--   0 klindsay   (501) staff       (20)    34527 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/ecs.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2352 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/efs.py
--rw-r--r--   0 klindsay   (501) staff       (20)     3185 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/eip.py
--rw-r--r--   0 klindsay   (501) staff       (20)     4246 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/elasticache.py
--rw-r--r--   0 klindsay   (501) staff       (20)     4411 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/elasticsearch.py
--rw-r--r--   0 klindsay   (501) staff       (20)     5521 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/eventsrule.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1219 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/example_template.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2830 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/iam_managed_policies.py
--rw-r--r--   0 klindsay   (501) staff       (20)    12125 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/iam_roles.py
--rw-r--r--   0 klindsay   (501) staff       (20)      939 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/iam_sl_roles.py
--rw-r--r--   0 klindsay   (501) staff       (20)    16777 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/iam_user_account_delegates.py
--rw-r--r--   0 klindsay   (501) staff       (20)     7747 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/iam_users.py
--rw-r--r--   0 klindsay   (501) staff       (20)     4475 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/iamuser.py
--rw-r--r--   0 klindsay   (501) staff       (20)    11937 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/iotanalyticspipeline.py
--rw-r--r--   0 klindsay   (501) staff       (20)     3636 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/iottopicrule.py
--rw-r--r--   0 klindsay   (501) staff       (20)     7743 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/kms.py
--rw-r--r--   0 klindsay   (501) staff       (20)    27062 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/lambda_function.py
--rw-r--r--   0 klindsay   (501) staff       (20)    20030 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/lb.py
--rw-r--r--   0 klindsay   (501) staff       (20)     7861 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/loggroups.py
--rw-r--r--   0 klindsay   (501) staff       (20)    10984 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/nat_gateway.py
--rw-r--r--   0 klindsay   (501) staff       (20)     4609 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/notification_rules.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2260 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/pinpointapplication.py
--rw-r--r--   0 klindsay   (501) staff       (20)    34046 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/rds.py
--rw-r--r--   0 klindsay   (501) staff       (20)     4998 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/route53.py
--rw-r--r--   0 klindsay   (501) staff       (20)     4481 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/route53_hostedzone.py
--rw-r--r--   0 klindsay   (501) staff       (20)     4675 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/route53_recordset.py
--rw-r--r--   0 klindsay   (501) staff       (20)     4289 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/route53healthcheck.py
--rw-r--r--   0 klindsay   (501) staff       (20)    10779 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/s3.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2983 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/secrets_manager.py
--rw-r--r--   0 klindsay   (501) staff       (20)     8280 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/security_groups.py
--rw-r--r--   0 klindsay   (501) staff       (20)    12198 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/segment.py
--rw-r--r--   0 klindsay   (501) staff       (20)     5703 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/sns.py
--rw-r--r--   0 klindsay   (501) staff       (20)     6245 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/snstopics.py
--rw-r--r--   0 klindsay   (501) staff       (20)      672 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/ssmdocument.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/tests/
--rw-r--r--   0 klindsay   (501) staff       (20)     2417 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/tests/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1087 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/tests/test_asg.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1484 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/tests/test_cftemplates.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1800 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/tests/test_codecommit.py
--rw-r--r--   0 klindsay   (501) staff       (20)      741 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/tests/test_ecs.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1050 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/tests/test_efs.py
--rw-r--r--   0 klindsay   (501) staff       (20)     5835 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/tests/test_iam_managed_policies.py
--rw-r--r--   0 klindsay   (501) staff       (20)     7071 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/tests/test_iam_roles.py
--rw-r--r--   0 klindsay   (501) staff       (20)     4173 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/vpc.py
--rw-r--r--   0 klindsay   (501) staff       (20)     3037 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cftemplates/vpc_peering.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/
--rw-r--r--   0 klindsay   (501) staff       (20)     1029 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/cli.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1246 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/cmd_delete.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1987 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/cmd_describe.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2889 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/cmd_init.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2865 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/cmd_lambda.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1361 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/cmd_provision.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1077 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/cmd_set.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1218 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/cmd_shell.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1055 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/cmd_validate.py
--rw-r--r--   0 klindsay   (501) staff       (20)     3659 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/cookiecutter_test.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/
--rw-r--r--   0 klindsay   (501) staff       (20)      132 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1008 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/accounts.pt
--rw-r--r--   0 klindsay   (501) staff       (20)     3351 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/env.pt
--rw-r--r--   0 klindsay   (501) staff       (20)     8138 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/globalresources.pt
--rw-r--r--   0 klindsay   (501) staff       (20)     3327 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/html.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1106 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/iam.pt
--rw-r--r--   0 klindsay   (501) staff       (20)     1001 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/index.pt
--rw-r--r--   0 klindsay   (501) staff       (20)    16751 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/jsonoutput.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1866 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/layout-html.pt
--rw-r--r--   0 klindsay   (501) staff       (20)      366 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/layout-spa.pt
--rw-r--r--   0 klindsay   (501) staff       (20)     5061 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/monitoring.pt
--rw-r--r--   0 klindsay   (501) staff       (20)     3758 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/netenvs.pt
--rw-r--r--   0 klindsay   (501) staff       (20)     1991 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/res-ASG.pt
--rw-r--r--   0 klindsay   (501) staff       (20)     2512 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/res-base.pt
--rw-r--r--   0 klindsay   (501) staff       (20)       39 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/res-empty.pt
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/static/
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/static/assets/
--rw-r--r--   0 klindsay   (501) staff       (20)     1232 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/static/assets/main.js
--rw-r--r--   0 klindsay   (501) staff       (20)     7797 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/static/assets/normalize.css
--rw-r--r--   0 klindsay   (501) staff       (20)     3612 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/static/assets/paco.css
--rw-r--r--   0 klindsay   (501) staff       (20)     6989 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/static/assets/skeleton.css
--rw-r--r--   0 klindsay   (501) staff       (20)      766 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/display/static/favicon.ico
--rw-r--r--   0 klindsay   (501) staff       (20)    13711 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/helpers.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/tests/
--rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/commands/tests/__init__.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/config/
--rw-r--r--   0 klindsay   (501) staff       (20)       58 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/config/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)     6608 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/config/aws_credentials.py
--rw-r--r--   0 klindsay   (501) staff       (20)      825 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/config/config_processor.py
--rw-r--r--   0 klindsay   (501) staff       (20)      130 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/config/interfaces.py
--rw-r--r--   0 klindsay   (501) staff       (20)     5595 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/config/paco_buckets.py
--rw-r--r--   0 klindsay   (501) staff       (20)    27173 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/config/paco_context.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/config/tests/
--rw-r--r--   0 klindsay   (501) staff       (20)      195 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/config/tests/test_aim_context.py
--rw-r--r--   0 klindsay   (501) staff       (20)      482 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/config/tests/test_cfg_network_environment.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/controllers/
--rw-r--r--   0 klindsay   (501) staff       (20)     1351 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/controllers/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1221 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/controllers/controllers.py
--rw-r--r--   0 klindsay   (501) staff       (20)    10859 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/controllers/ctl_account.py
--rw-r--r--   0 klindsay   (501) staff       (20)     7522 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/controllers/ctl_cloudtrail.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2146 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/controllers/ctl_cloudwatch.py
--rw-r--r--   0 klindsay   (501) staff       (20)     5738 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/controllers/ctl_codecommit.py
--rw-r--r--   0 klindsay   (501) staff       (20)     7438 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/controllers/ctl_config.py
--rw-r--r--   0 klindsay   (501) staff       (20)     4164 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/controllers/ctl_ec2.py
--rw-r--r--   0 klindsay   (501) staff       (20)    32589 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/controllers/ctl_iam.py
--rw-r--r--   0 klindsay   (501) staff       (20)    11558 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/controllers/ctl_network_environment.py
--rw-r--r--   0 klindsay   (501) staff       (20)    12283 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/controllers/ctl_project.py
--rw-r--r--   0 klindsay   (501) staff       (20)     5925 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/controllers/ctl_route53.py
--rw-r--r--   0 klindsay   (501) staff       (20)    13896 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/controllers/ctl_s3.py
--rw-r--r--   0 klindsay   (501) staff       (20)     6419 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/controllers/ctl_sns.py
--rw-r--r--   0 klindsay   (501) staff       (20)     3636 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/controllers/ctl_snstopics.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2729 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/controllers/ctl_ssm.py
--rw-r--r--   0 klindsay   (501) staff       (20)     3432 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/controllers/mixins.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/
--rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/__init__.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/
--rw-r--r--   0 klindsay   (501) staff       (20)      809 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)      663 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/cookiecutter.json
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/accounts/
--rw-r--r--   0 klindsay   (501) staff       (20)      315 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/accounts/master.yaml
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/monitor/
--rw-r--r--   0 klindsay   (501) staff       (20)     6768 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml
--rw-r--r--   0 klindsay   (501) staff       (20)     2498 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/monitor/Logging.yaml
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/dashboards/
--rw-r--r--   0 klindsay   (501) staff       (20)    10823 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/dashboards/complete-dashboard.json
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/webapp/
--rw-r--r--   0 klindsay   (501) staff       (20)      685 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/webapp/get_rds_dsn.sh
--rw-r--r--   0 klindsay   (501) staff       (20)      324 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/webapp/saas_wsgi.conf
--rw-r--r--   0 klindsay   (501) staff       (20)    26116 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml
--rw-r--r--   0 klindsay   (501) staff       (20)        4 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/paco-project-version.txt
--rw-r--r--   0 klindsay   (501) staff       (20)      210 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/project.yaml
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/resource/
--rw-r--r--   0 klindsay   (501) staff       (20)      405 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/resource/cloudtrail.yaml
--rw-r--r--   0 klindsay   (501) staff       (20)      462 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/resource/codecommit.yaml
--rw-r--r--   0 klindsay   (501) staff       (20)      760 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/resource/ec2.yaml
--rw-r--r--   0 klindsay   (501) staff       (20)      462 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/resource/iam.yaml
--rw-r--r--   0 klindsay   (501) staff       (20)      176 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/resource/route53.yaml
--rw-r--r--   0 klindsay   (501) staff       (20)      379 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/resource/snstopics.yaml
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/
--rw-r--r--   0 klindsay   (501) staff       (20)      582 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)      536 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/cookiecutter.json
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/accounts/
--rw-r--r--   0 klindsay   (501) staff       (20)      289 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/accounts/master.yaml
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/monitor/
--rw-r--r--   0 klindsay   (501) staff       (20)     1220 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/netenv/
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/netenv/pypi-config/
--rw-r--r--   0 klindsay   (501) staff       (20)      322 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/netenv/pypi-config/cfn-auto-reloader.conf
--rw-r--r--   0 klindsay   (501) staff       (20)      124 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/netenv/pypi-config/cfn-hup.conf
--rw-r--r--   0 klindsay   (501) staff       (20)      251 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/netenv/pypi-config/htpasswd.txt
--rw-r--r--   0 klindsay   (501) staff       (20)      558 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/netenv/pypi-config/pypiserver.service
--rw-r--r--   0 klindsay   (501) staff       (20)    16157 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml
--rw-r--r--   0 klindsay   (501) staff       (20)        4 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/paco-project-version.txt
--rw-r--r--   0 klindsay   (501) staff       (20)      210 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/project.yaml
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/resource/
--rw-r--r--   0 klindsay   (501) staff       (20)      173 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/resource/ec2.yaml
--rw-r--r--   0 klindsay   (501) staff       (20)      249 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/resource/snstopics.yaml
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/
--rw-r--r--   0 klindsay   (501) staff       (20)      687 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)      523 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/cookiecutter.json
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/accounts/
--rw-r--r--   0 klindsay   (501) staff       (20)      289 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/accounts/master.yaml
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/monitor/
--rw-r--r--   0 klindsay   (501) staff       (20)      777 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/netenv/
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/netenv/lambda_code/
--rw-r--r--   0 klindsay   (501) staff       (20)     1484 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/netenv/lambda_code/s3_replicator.py
--rw-r--r--   0 klindsay   (501) staff       (20)     4262 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml
--rw-r--r--   0 klindsay   (501) staff       (20)        3 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/paco-project-version.txt
--rw-r--r--   0 klindsay   (501) staff       (20)      169 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/project.yaml
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/resource/
--rw-r--r--   0 klindsay   (501) staff       (20)      243 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/resource/snstopics.yaml
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/simplewebapp/
--rw-r--r--   0 klindsay   (501) staff       (20)      534 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/simplewebapp/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)      516 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/simplewebapp/cookiecutter.json
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/accounts/
--rw-r--r--   0 klindsay   (501) staff       (20)      288 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/accounts/master.yaml
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/monitor/
--rw-r--r--   0 klindsay   (501) staff       (20)     5255 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml
--rw-r--r--   0 klindsay   (501) staff       (20)     1889 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/monitor/Logging.yaml
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/netenv/
--rw-r--r--   0 klindsay   (501) staff       (20)     5597 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml
--rw-r--r--   0 klindsay   (501) staff       (20)        3 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/paco-project-version.txt
--rw-r--r--   0 klindsay   (501) staff       (20)      129 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/project.yaml
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/
--rw-r--r--   0 klindsay   (501) staff       (20)      582 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)      516 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/cookiecutter.json
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/accounts/
--rw-r--r--   0 klindsay   (501) staff       (20)      289 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/accounts/master.yaml
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/monitor/
--rw-r--r--   0 klindsay   (501) staff       (20)     1576 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml
--rw-r--r--   0 klindsay   (501) staff       (20)       56 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/monitor/Logging.yaml
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/netenv/
--rw-r--r--   0 klindsay   (501) staff       (20)     6881 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml
--rw-r--r--   0 klindsay   (501) staff       (20)        3 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/paco-project-version.txt
--rw-r--r--   0 klindsay   (501) staff       (20)      210 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/project.yaml
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/resource/
--rw-r--r--   0 klindsay   (501) staff       (20)      145 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/resource/ec2.yaml
--rw-r--r--   0 klindsay   (501) staff       (20)      136 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/resource/route53.yaml
--rw-r--r--   0 klindsay   (501) staff       (20)      312 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/resource/snstopics.yaml
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/core/
--rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/core/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)     4248 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/core/exception.py
--rw-r--r--   0 klindsay   (501) staff       (20)      423 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/core/log.py
--rw-r--r--   0 klindsay   (501) staff       (20)     1872 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/core/yaml.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/doc/
--rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/doc/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)    50903 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/doc/docschema.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/extend/
--rw-r--r--   0 klindsay   (501) staff       (20)     8262 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/extend/__init__.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/stack/
--rw-r--r--   0 klindsay   (501) staff       (20)      291 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/stack/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2530 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/stack/botostack.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/stack/botostacks/
--rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/stack/botostacks/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)     3001 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/stack/botostacks/acm.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2320 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/stack/botostacks/iotpolicy.py
--rw-r--r--   0 klindsay   (501) staff       (20)      479 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/stack/interfaces.py
--rw-r--r--   0 klindsay   (501) staff       (20)    68940 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/stack/stack.py
--rw-r--r--   0 klindsay   (501) staff       (20)    11750 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/stack/stack_group.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/stack_grps/
--rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/stack_grps/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)      763 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/stack_grps/grp_account.py
--rw-r--r--   0 klindsay   (501) staff       (20)      968 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/stack_grps/grp_application.py
--rw-r--r--   0 klindsay   (501) staff       (20)     3125 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/stack_grps/grp_backup.py
--rw-r--r--   0 klindsay   (501) staff       (20)     4977 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/stack_grps/grp_codecommit.py
--rw-r--r--   0 klindsay   (501) staff       (20)     7451 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/stack_grps/grp_network.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2205 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/stack_grps/grp_route53.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2147 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/stack_grps/grp_secretsmanager.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/tests/
--rw-r--r--   0 klindsay   (501) staff       (20)      850 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/tests/__init__.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/utils/
--rw-r--r--   0 klindsay   (501) staff       (20)     7458 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/utils/__init__.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2388 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/utils/cache.py
--rw-r--r--   0 klindsay   (501) staff       (20)     2153 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco/utils/zip.py
-drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco_cloud.egg-info/
--rw-r--r--   0 klindsay   (501) staff       (20)    47228 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco_cloud.egg-info/PKG-INFO
--rw-r--r--   0 klindsay   (501) staff       (20)    12534 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 klindsay   (501) staff       (20)        1 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 klindsay   (501) staff       (20)       99 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco_cloud.egg-info/entry_points.txt
--rw-r--r--   0 klindsay   (501) staff       (20)        1 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco_cloud.egg-info/not-zip-safe
--rw-r--r--   0 klindsay   (501) staff       (20)      241 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco_cloud.egg-info/requires.txt
--rw-r--r--   0 klindsay   (501) staff       (20)        5 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/src/paco_cloud.egg-info/top_level.txt
--rw-r--r--   0 klindsay   (501) staff       (20)        6 2021-04-10 00:45:22.000000 paco-cloud-9.3.8/version.txt
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/
+-rw-r--r--   0 klindsay   (501) staff       (20)    35521 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/CHANGELOG.md
+-rw-r--r--   0 klindsay   (501) staff       (20)      183 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/MANIFEST.in
+-rw-r--r--   0 klindsay   (501) staff       (20)    47597 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/PKG-INFO
+-rw-r--r--   0 klindsay   (501) staff       (20)     1669 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/README.md
+-rw-r--r--   0 klindsay   (501) staff       (20)       38 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/setup.cfg
+-rw-r--r--   0 klindsay   (501) staff       (20)     2170 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/setup.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/
+-rw-r--r--   0 klindsay   (501) staff       (20)       65 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/__init__.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/adapters/
+-rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/adapters/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1352 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/adapters/monitoring.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/application/
+-rw-r--r--   0 klindsay   (501) staff       (20)     2319 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     9282 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/app_engine.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    82649 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/ec2_launch_manager.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     6212 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/ec2lm_commands.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     3938 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/res_engine.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      316 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_acm.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2183 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_apigatewayrestapi.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     6489 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_asg.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1234 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_cloudfront.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1977 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_codedeployapplication.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      633 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_cognito.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      353 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_dashboard.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    55586 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_deploymentpipeline.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      340 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_dynamodb.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      330 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_ebs.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      577 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_ec2.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      602 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_ecrrepository.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      345 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_ecscluster.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     5180 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_ecsservices.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      414 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_efs.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      345 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_eip.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      396 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_elasticacheredis.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      861 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_elasticsearch.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      506 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_eventsrule.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     5324 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_iamuser.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2946 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_iotanalyticspipeline.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      339 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_iotpolicy.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2748 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_iottopicrule.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     4483 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_lambda.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1099 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_lb.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      363 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_pinpointapplication.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2051 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_rds.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      775 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_s3bucket.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      426 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/application/reseng_snstopic.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/aws_api/
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/aws_api/acm/
+-rw-r--r--   0 klindsay   (501) staff       (20)     7855 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/aws_api/acm/ACM.py
+-rw-r--r--   0 klindsay   (501) staff       (20)       43 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/aws_api/acm/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      201 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/aws_api/acm/aws_helpers.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/aws_api/awslambda/
+-rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/aws_api/awslambda/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     3070 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/aws_api/awslambda/code.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/aws_api/ecs/
+-rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/aws_api/ecs/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    11575 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/aws_api/ecs/capacityprovider.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/aws_api/iam/
+-rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/aws_api/iam/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2927 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/aws_api/iam/user.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/aws_api/iot/
+-rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/aws_api/iot/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     3644 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/aws_api/iot/iotpolicy.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/aws_api/ssm/
+-rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/aws_api/ssm/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2494 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/aws_api/ssm/document.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cftemplates/
+-rw-r--r--   0 klindsay   (501) staff       (20)     3002 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    24030 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/apigateway.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    34922 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/asg.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     7709 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/backup.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    23582 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/cftemplates.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    18768 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/cloudfront.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     4673 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/cloudtrail.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    22958 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/codebuild.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     9074 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/codecommit.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    13045 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/codedeploy.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     5111 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/codedeployapplication.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    52738 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/codepipeline.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    15220 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/cognito.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2039 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/config.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    19700 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/cw_alarms.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2085 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/dashboard.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1442 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/dynamodb.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1316 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/ebs.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     4481 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/ecr.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    35726 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/ecs.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2352 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/efs.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     3185 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/eip.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     4246 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/elasticache.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     4411 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/elasticsearch.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     5521 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/eventsrule.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1219 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/example_template.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2830 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/iam_managed_policies.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    12125 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/iam_roles.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      939 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/iam_sl_roles.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    16777 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/iam_user_account_delegates.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     7747 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/iam_users.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     4475 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/iamuser.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    11937 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/iotanalyticspipeline.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     3636 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/iottopicrule.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     7743 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/kms.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    27062 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/lambda_function.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    20030 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/lb.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     7861 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/loggroups.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    10984 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/nat_gateway.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     4609 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/notification_rules.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2260 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/pinpointapplication.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    34046 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/rds.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     4998 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/route53.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     4481 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/route53_hostedzone.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     4675 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/route53_recordset.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     4289 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/route53healthcheck.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    10779 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/s3.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2983 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/secrets_manager.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     8280 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/security_groups.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    12198 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/segment.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     5703 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/sns.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     6245 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/snstopics.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      672 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/ssmdocument.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cftemplates/tests/
+-rw-r--r--   0 klindsay   (501) staff       (20)     2417 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/tests/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1087 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/tests/test_asg.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1484 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/tests/test_cftemplates.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1800 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/tests/test_codecommit.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      741 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/tests/test_ecs.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1050 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/tests/test_efs.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     5835 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/tests/test_iam_managed_policies.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     7071 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/tests/test_iam_roles.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     4173 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/vpc.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     3037 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cftemplates/vpc_peering.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/commands/
+-rw-r--r--   0 klindsay   (501) staff       (20)     1029 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/cli.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1246 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/cmd_delete.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1987 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/cmd_describe.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2889 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/cmd_init.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2865 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/cmd_lambda.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1361 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/cmd_provision.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1077 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/cmd_set.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1218 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/cmd_shell.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1055 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/cmd_validate.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     3659 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/cookiecutter_test.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/commands/display/
+-rw-r--r--   0 klindsay   (501) staff       (20)      132 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1008 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/accounts.pt
+-rw-r--r--   0 klindsay   (501) staff       (20)     3351 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/env.pt
+-rw-r--r--   0 klindsay   (501) staff       (20)     8138 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/globalresources.pt
+-rw-r--r--   0 klindsay   (501) staff       (20)     3327 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/html.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1106 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/iam.pt
+-rw-r--r--   0 klindsay   (501) staff       (20)     1001 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/index.pt
+-rw-r--r--   0 klindsay   (501) staff       (20)    16751 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/jsonoutput.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1866 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/layout-html.pt
+-rw-r--r--   0 klindsay   (501) staff       (20)      366 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/layout-spa.pt
+-rw-r--r--   0 klindsay   (501) staff       (20)     5061 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/monitoring.pt
+-rw-r--r--   0 klindsay   (501) staff       (20)     3758 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/netenvs.pt
+-rw-r--r--   0 klindsay   (501) staff       (20)     1991 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/res-ASG.pt
+-rw-r--r--   0 klindsay   (501) staff       (20)     2512 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/res-base.pt
+-rw-r--r--   0 klindsay   (501) staff       (20)       39 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/res-empty.pt
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/commands/display/static/
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/commands/display/static/assets/
+-rw-r--r--   0 klindsay   (501) staff       (20)     1232 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/static/assets/main.js
+-rw-r--r--   0 klindsay   (501) staff       (20)     7797 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/static/assets/normalize.css
+-rw-r--r--   0 klindsay   (501) staff       (20)     3612 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/static/assets/paco.css
+-rw-r--r--   0 klindsay   (501) staff       (20)     6989 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/static/assets/skeleton.css
+-rw-r--r--   0 klindsay   (501) staff       (20)      766 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/display/static/favicon.ico
+-rw-r--r--   0 klindsay   (501) staff       (20)    13711 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/helpers.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/commands/tests/
+-rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/commands/tests/__init__.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/config/
+-rw-r--r--   0 klindsay   (501) staff       (20)       58 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/config/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     6608 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/config/aws_credentials.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      825 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/config/config_processor.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      130 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/config/interfaces.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     5595 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/config/paco_buckets.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    27173 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/config/paco_context.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/config/tests/
+-rw-r--r--   0 klindsay   (501) staff       (20)      195 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/config/tests/test_aim_context.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      482 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/config/tests/test_cfg_network_environment.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/controllers/
+-rw-r--r--   0 klindsay   (501) staff       (20)     1351 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/controllers/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1221 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/controllers/controllers.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    10859 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/controllers/ctl_account.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     7522 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/controllers/ctl_cloudtrail.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2146 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/controllers/ctl_cloudwatch.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     5738 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/controllers/ctl_codecommit.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     7438 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/controllers/ctl_config.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     4164 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/controllers/ctl_ec2.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    32589 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/controllers/ctl_iam.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    11558 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/controllers/ctl_network_environment.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    12283 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/controllers/ctl_project.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     5925 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/controllers/ctl_route53.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    13896 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/controllers/ctl_s3.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     6419 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/controllers/ctl_sns.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     3636 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/controllers/ctl_snstopics.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2729 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/controllers/ctl_ssm.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     3432 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/controllers/mixins.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/
+-rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/__init__.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/
+-rw-r--r--   0 klindsay   (501) staff       (20)      809 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      663 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/cookiecutter.json
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/accounts/
+-rw-r--r--   0 klindsay   (501) staff       (20)      315 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/accounts/master.yaml
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/monitor/
+-rw-r--r--   0 klindsay   (501) staff       (20)     6768 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml
+-rw-r--r--   0 klindsay   (501) staff       (20)     2498 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/monitor/Logging.yaml
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/dashboards/
+-rw-r--r--   0 klindsay   (501) staff       (20)    10823 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/dashboards/complete-dashboard.json
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/webapp/
+-rw-r--r--   0 klindsay   (501) staff       (20)      685 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/webapp/get_rds_dsn.sh
+-rw-r--r--   0 klindsay   (501) staff       (20)      324 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/webapp/saas_wsgi.conf
+-rw-r--r--   0 klindsay   (501) staff       (20)    26116 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml
+-rw-r--r--   0 klindsay   (501) staff       (20)        4 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/paco-project-version.txt
+-rw-r--r--   0 klindsay   (501) staff       (20)      210 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/project.yaml
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/resource/
+-rw-r--r--   0 klindsay   (501) staff       (20)      405 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/resource/cloudtrail.yaml
+-rw-r--r--   0 klindsay   (501) staff       (20)      462 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/resource/codecommit.yaml
+-rw-r--r--   0 klindsay   (501) staff       (20)      760 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/resource/ec2.yaml
+-rw-r--r--   0 klindsay   (501) staff       (20)      462 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/resource/iam.yaml
+-rw-r--r--   0 klindsay   (501) staff       (20)      176 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/resource/route53.yaml
+-rw-r--r--   0 klindsay   (501) staff       (20)      379 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/resource/snstopics.yaml
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/
+-rw-r--r--   0 klindsay   (501) staff       (20)      582 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      536 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/cookiecutter.json
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/accounts/
+-rw-r--r--   0 klindsay   (501) staff       (20)      289 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/accounts/master.yaml
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/monitor/
+-rw-r--r--   0 klindsay   (501) staff       (20)     1220 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/netenv/
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/netenv/pypi-config/
+-rw-r--r--   0 klindsay   (501) staff       (20)      322 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/netenv/pypi-config/cfn-auto-reloader.conf
+-rw-r--r--   0 klindsay   (501) staff       (20)      124 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/netenv/pypi-config/cfn-hup.conf
+-rw-r--r--   0 klindsay   (501) staff       (20)      251 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/netenv/pypi-config/htpasswd.txt
+-rw-r--r--   0 klindsay   (501) staff       (20)      558 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/netenv/pypi-config/pypiserver.service
+-rw-r--r--   0 klindsay   (501) staff       (20)    16157 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml
+-rw-r--r--   0 klindsay   (501) staff       (20)        4 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/paco-project-version.txt
+-rw-r--r--   0 klindsay   (501) staff       (20)      210 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/project.yaml
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/resource/
+-rw-r--r--   0 klindsay   (501) staff       (20)      173 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/resource/ec2.yaml
+-rw-r--r--   0 klindsay   (501) staff       (20)      249 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/resource/snstopics.yaml
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/
+-rw-r--r--   0 klindsay   (501) staff       (20)      687 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      523 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/cookiecutter.json
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/accounts/
+-rw-r--r--   0 klindsay   (501) staff       (20)      289 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/accounts/master.yaml
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/monitor/
+-rw-r--r--   0 klindsay   (501) staff       (20)      777 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/netenv/
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/netenv/lambda_code/
+-rw-r--r--   0 klindsay   (501) staff       (20)     1484 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/netenv/lambda_code/s3_replicator.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     4262 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml
+-rw-r--r--   0 klindsay   (501) staff       (20)        3 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/paco-project-version.txt
+-rw-r--r--   0 klindsay   (501) staff       (20)      169 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/project.yaml
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/resource/
+-rw-r--r--   0 klindsay   (501) staff       (20)      243 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/resource/snstopics.yaml
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/simplewebapp/
+-rw-r--r--   0 klindsay   (501) staff       (20)      534 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/simplewebapp/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      516 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/simplewebapp/cookiecutter.json
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/accounts/
+-rw-r--r--   0 klindsay   (501) staff       (20)      288 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/accounts/master.yaml
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/monitor/
+-rw-r--r--   0 klindsay   (501) staff       (20)     5255 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml
+-rw-r--r--   0 klindsay   (501) staff       (20)     1889 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/monitor/Logging.yaml
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/netenv/
+-rw-r--r--   0 klindsay   (501) staff       (20)     5597 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml
+-rw-r--r--   0 klindsay   (501) staff       (20)        3 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/paco-project-version.txt
+-rw-r--r--   0 klindsay   (501) staff       (20)      129 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/project.yaml
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/
+-rw-r--r--   0 klindsay   (501) staff       (20)      582 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      516 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/cookiecutter.json
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/accounts/
+-rw-r--r--   0 klindsay   (501) staff       (20)      289 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/accounts/master.yaml
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/monitor/
+-rw-r--r--   0 klindsay   (501) staff       (20)     1576 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml
+-rw-r--r--   0 klindsay   (501) staff       (20)       56 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/monitor/Logging.yaml
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/netenv/
+-rw-r--r--   0 klindsay   (501) staff       (20)     6881 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml
+-rw-r--r--   0 klindsay   (501) staff       (20)        3 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/paco-project-version.txt
+-rw-r--r--   0 klindsay   (501) staff       (20)      210 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/project.yaml
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/resource/
+-rw-r--r--   0 klindsay   (501) staff       (20)      145 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/resource/ec2.yaml
+-rw-r--r--   0 klindsay   (501) staff       (20)      136 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/resource/route53.yaml
+-rw-r--r--   0 klindsay   (501) staff       (20)      312 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/resource/snstopics.yaml
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/core/
+-rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/core/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     4248 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/core/exception.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      423 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/core/log.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     1872 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/core/yaml.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/doc/
+-rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/doc/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    50903 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/doc/docschema.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/extend/
+-rw-r--r--   0 klindsay   (501) staff       (20)     8262 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/extend/__init__.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/stack/
+-rw-r--r--   0 klindsay   (501) staff       (20)      291 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/stack/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2530 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/stack/botostack.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/stack/botostacks/
+-rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/stack/botostacks/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     3001 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/stack/botostacks/acm.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2320 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/stack/botostacks/iotpolicy.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      479 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/stack/interfaces.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    68940 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/stack/stack.py
+-rw-r--r--   0 klindsay   (501) staff       (20)    11750 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/stack/stack_group.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/stack_grps/
+-rw-r--r--   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/stack_grps/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      763 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/stack_grps/grp_account.py
+-rw-r--r--   0 klindsay   (501) staff       (20)      968 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/stack_grps/grp_application.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     3125 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/stack_grps/grp_backup.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     4977 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/stack_grps/grp_codecommit.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     7451 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/stack_grps/grp_network.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2205 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/stack_grps/grp_route53.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2147 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/stack_grps/grp_secretsmanager.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/tests/
+-rw-r--r--   0 klindsay   (501) staff       (20)      850 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/tests/__init__.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco/utils/
+-rw-r--r--   0 klindsay   (501) staff       (20)     7458 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/utils/__init__.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2388 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/utils/cache.py
+-rw-r--r--   0 klindsay   (501) staff       (20)     2153 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/src/paco/utils/zip.py
+drwxr-xr-x   0 klindsay   (501) staff       (20)        0 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco_cloud.egg-info/
+-rw-r--r--   0 klindsay   (501) staff       (20)    47597 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 klindsay   (501) staff       (20)    12534 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 klindsay   (501) staff       (20)        1 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 klindsay   (501) staff       (20)       99 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 klindsay   (501) staff       (20)        1 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 klindsay   (501) staff       (20)      241 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco_cloud.egg-info/requires.txt
+-rw-r--r--   0 klindsay   (501) staff       (20)        5 2021-04-19 20:20:18.000000 paco-cloud-9.3.9/src/paco_cloud.egg-info/top_level.txt
+-rw-r--r--   0 klindsay   (501) staff       (20)        6 2021-04-19 20:20:17.000000 paco-cloud-9.3.9/version.txt
```

### Comparing `paco-cloud-9.3.8/CHANGELOG.md` & `paco-cloud-9.3.9/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 Changelog for Paco
 ==================
 
+9.3.9 (2021-04-19)
+------------------
+
+### Added
+
+- Added logging to SSM instance EC2LM update run commands.
+- Added docker-exec command to ECS ScriptManager script.
+
+### Changed
+
+- Improved ECR Deploy Script to tag the destination image with the same tags as the source.
+
 9.3.8 (2021-04-09)
 ------------------
 
 ### Fixed
 
 - Fixed release phase script name in the ECR deploy script.
```

### Comparing `paco-cloud-9.3.8/PKG-INFO` & `paco-cloud-9.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paco-cloud
-Version: 9.3.8
+Version: 9.3.9
 Summary: Paco: Prescribed automation for cloud orchestration
 Home-page: https://github.com/waterbear-cloud/paco
 Author: Waterbear Cloud
 Author-email: hello@waterbear.cloud
 License: UNKNOWN
 Description: # Paco: Prescribed automation for cloud orchestration
         
@@ -40,14 +40,26 @@
         
         Paco is created by Kevin Lindsay and Kevin Teague for [Waterbear Cloud](https://waterbear.cloud).
         
         
         Changelog for Paco
         ==================
         
+        9.3.9 (2021-04-19)
+        ------------------
+        
+        ### Added
+        
+        - Added logging to SSM instance EC2LM update run commands.
+        - Added docker-exec command to ECS ScriptManager script.
+        
+        ### Changed
+        
+        - Improved ECR Deploy Script to tag the destination image with the same tags as the source.
+        
         9.3.8 (2021-04-09)
         ------------------
         
         ### Fixed
         
         - Fixed release phase script name in the ECR deploy script.
```

### Comparing `paco-cloud-9.3.8/README.md` & `paco-cloud-9.3.9/README.md`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/setup.py` & `paco-cloud-9.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     ],
     keywords=['AWS','Waterbear','Cloud','Infrastructure as Code', 'CloudFormation'],
     install_requires=[
-        'paco.models >= 7.8.7',
+        'paco.models >= 7.8.8',
         'boto3 >= 1.16.48',
         'click',
         'cookiecutter',
         'Setuptools',
         'tldextract',
         'pexpect',
         'troposphere >= 2.6.3',
```

### Comparing `paco-cloud-9.3.8/src/paco/adapters/monitoring.py` & `paco-cloud-9.3.9/src/paco/adapters/monitoring.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/__init__.py` & `paco-cloud-9.3.9/src/paco/application/__init__.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/app_engine.py` & `paco-cloud-9.3.9/src/paco/application/app_engine.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/ec2_launch_manager.py` & `paco-cloud-9.3.9/src/paco/application/ec2_launch_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1516,15 +1516,15 @@
                     {
                         "action": "aws:runShellScript",
                         "name": "updateEC2LMInstance",
                         "inputs": {
                             "runCommand": [
                                 '#!/bin/bash',
                                 f'. {self.paco_base_path}/EC2Manager/ec2lm_functions.bash',
-                                'ec2lm_launch_bundles ' + '{{CacheId}}',
+                                'ec2lm_launch_bundles ' + '{{CacheId}}' + '>>/var/log/paco/ec2lm.log',
                             ]
                         }
                     }
                 ]
             }
             ssm_doc.content = json.dumps(content)
             ssm_doc.document_type = 'Command'
@@ -1829,14 +1829,15 @@
                 dest_account_id = self.paco_ctx.get_ref(dest_env.network.aws_account+".id")
 
                 dest_ecr_obj = get_model_obj_from_ref(repository.dest_repo, self.paco_ctx.project)
                 ecr_deploy_script += ECR_DEPLOY_SCRIPT_CONFIG.format(
                     ecr_deploy_name=ecr_deploy_name,
                     source_repo_name=source_ecr_obj.repository_name,
                     source_repo_domain=f'{source_account_id}.dkr.ecr.{source_env.region}.amazonaws.com',
+                    source_repo_account_id=source_account_id,
                     idx=repo_idx,
                     source_tag=repository.source_tag,
                     dest_repo_name=dest_ecr_obj.repository_name,
                     dest_repo_domain=f'{dest_account_id}.dkr.ecr.{dest_env.region}.amazonaws.com',
                     dest_tag=repository.dest_tag,
                     release_phase=repository.release_phase
                 )
@@ -1941,28 +1942,29 @@
 {script_name}_PATH="{scripts[script_name]['path']}"
 {script_name}_MODE="{scripts[script_name]['mode']}"
 """
             idx += 1
 
         launch_script += f"""
 function run_launch_bundle() {{
+    echo "EC2LM: ScriptManager: Installing scripts"
     ec2lm_install_package jq
     for NAME in ${{SCRIPTS[@]}}
     do
         SCRIPT_PATH_VAR=${{NAME}}_PATH
         SCRIPT_DATA_VAR=${{NAME}}_DATA
         SCRIPT_MODE_VAR=${{NAME}}_MODE
 
         SCRIPT_PATH=${{!SCRIPT_PATH_VAR}}
         SCRIPT_DATA=${{!SCRIPT_DATA_VAR}}
         SCRIPT_MODE=${{!SCRIPT_MODE_VAR}}
         if [ -e "${{SCRIPT_PATH}}" ] ; then
-            echo "Updating script: ${{SCRIPT_PATH}}"
+            echo "EC2LM: ScriptManager: Updating script: ${{SCRIPT_PATH}}"
         else
-            echo "Creating script: ${{SCRIPT_PATH}}"
+            echo "EC2LM: ScriptManager: Creating script: ${{SCRIPT_PATH}}"
         fi
         echo ${{SCRIPT_DATA}} | base64 -d >${{SCRIPT_PATH}}
         chmod ${{SCRIPT_MODE}} ${{SCRIPT_PATH}}
     done
 }}
 
 function disable_launch_bundle() {{
```

### Comparing `paco-cloud-9.3.8/src/paco/application/ec2lm_commands.py` & `paco-cloud-9.3.9/src/paco/application/ec2lm_commands.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/res_engine.py` & `paco-cloud-9.3.9/src/paco/application/res_engine.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/reseng_apigatewayrestapi.py` & `paco-cloud-9.3.9/src/paco/application/reseng_apigatewayrestapi.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/reseng_asg.py` & `paco-cloud-9.3.9/src/paco/application/reseng_asg.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/reseng_cloudfront.py` & `paco-cloud-9.3.9/src/paco/application/reseng_cloudfront.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/reseng_codedeployapplication.py` & `paco-cloud-9.3.9/src/paco/application/reseng_codedeployapplication.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/reseng_cognito.py` & `paco-cloud-9.3.9/src/paco/application/reseng_cognito.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/reseng_deploymentpipeline.py` & `paco-cloud-9.3.9/src/paco/application/reseng_deploymentpipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 """
 
 ECR_DEPLOY_SCRIPT_CONFIG = """
 
 {ecr_deploy_name}_SOURCE_REPO_NAME_{idx}='{source_repo_name}'
 {ecr_deploy_name}_SOURCE_REPO_DOMAIN_{idx}='{source_repo_domain}'
 {ecr_deploy_name}_SOURCE_REPO_URI_{idx}="${{{ecr_deploy_name}_SOURCE_REPO_DOMAIN_{idx}}}/"
+{ecr_deploy_name}_SOURCE_REPO_ACCOUNT_{idx}="{source_repo_account_id}"
 {ecr_deploy_name}_SOURCE_TAG_{idx}='{source_tag}'
 {ecr_deploy_name}_DEST_REPO_NAME_{idx}='{dest_repo_name}'
 {ecr_deploy_name}_DEST_REPO_DOMAIN_{idx}='{dest_repo_domain}'
 {ecr_deploy_name}_DEST_REPO_URI_{idx}="${{{ecr_deploy_name}_DEST_REPO_DOMAIN_{idx}}}/"
 {ecr_deploy_name}_DEST_TAG_{idx}='{dest_tag}'
 {ecr_deploy_name}_RELEASE_PHASE_{idx}=$(echo "{release_phase}" | tr '[:upper:]' '[:lower:]')
 
@@ -168,24 +169,35 @@
     echo "Pushing to Destination"
 
     for (( J=0; J<${!ECR_DEPLOY_LEN}; J++ ))
     do
         SOURCE_REPO_NAME=${ECR_DEPLOY_LIST[$I]}_SOURCE_REPO_NAME_$J
         SOURCE_REPO_DOMAIN=${ECR_DEPLOY_LIST[$I]}_SOURCE_REPO_DOMAIN_$J
         SOURCE_REPO_URI=${ECR_DEPLOY_LIST[$I]}_SOURCE_REPO_URI_$J
+        SOURCE_REPO_ACCOUNT=${ECR_DEPLOY_LIST[$I]}_SOURCE_REPO_ACCOUNT_$J
         SOURCE_DEPLOY_TAG=${ECR_DEPLOY_LIST[$I]}_SOURCE_TAG_$J
         if [ "${OVERRIDE_SOURCE_DEPLOY_TAG}" != "" ] ; then
             SOURCE_DEPLOY_TAG="OVERRIDE_SOURCE_DEPLOY_TAG"
         fi
 
         DEST_REPO_NAME=${ECR_DEPLOY_LIST[$I]}_DEST_REPO_NAME_$J
         DEST_REPO_DOMAIN=${ECR_DEPLOY_LIST[$I]}_DEST_REPO_DOMAIN_$J
         DEST_DEPLOY_TAG=${ECR_DEPLOY_LIST[$I]}_DEST_TAG_$J
         DEST_REPO_URI=${ECR_DEPLOY_LIST[$I]}_DEST_REPO_URI_$J
 
+        JQ_QUERY=".imageDetails[] | select(.imageTags != null) | select(.imageTags | contains([\\\"${!SOURCE_DEPLOY_TAG}\\\"])) | .imageTags | join(\\\" \\\")"
+        SOURCE_REPO_TAGS=$(aws ecr describe-images --registry-id ${!SOURCE_REPO_ACCOUNT} --repository-name ${!SOURCE_REPO_NAME} | jq -c "${JQ_QUERY}" | tr -d '"')
+        for SOURCE_TAG in $(echo $SOURCE_REPO_TAGS)
+        do
+            if [ "$SOURCE_TAG" == "${!DEST_DEPLOY_TAG}" ] ; then
+               continue
+            fi
+            run_command "" "docker tag ${!SOURCE_REPO_URI}${!SOURCE_REPO_NAME}:${!SOURCE_DEPLOY_TAG} ${!DEST_REPO_URI}${!DEST_REPO_NAME}:${SOURCE_TAG}"
+            ec2lm_async_run "" "docker push ${!DEST_REPO_URI}${!DEST_REPO_NAME}:${SOURCE_TAG}"
+        done
         run_command "" "docker tag ${!SOURCE_REPO_URI}${!SOURCE_REPO_NAME}:${!SOURCE_DEPLOY_TAG} ${!DEST_REPO_URI}${!DEST_REPO_NAME}:${!DEST_DEPLOY_TAG}"
         ec2lm_async_run "" "docker push ${!DEST_REPO_URI}${!DEST_REPO_NAME}:${!DEST_DEPLOY_TAG}"
     done
     ec2lm_async_run_wait
 done
 """
```

### Comparing `paco-cloud-9.3.8/src/paco/application/reseng_ec2.py` & `paco-cloud-9.3.9/src/paco/application/reseng_ec2.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/reseng_ecrrepository.py` & `paco-cloud-9.3.9/src/paco/application/reseng_ecrrepository.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/reseng_ecsservices.py` & `paco-cloud-9.3.9/src/paco/application/reseng_ecsservices.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/reseng_elasticsearch.py` & `paco-cloud-9.3.9/src/paco/application/reseng_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/reseng_iamuser.py` & `paco-cloud-9.3.9/src/paco/application/reseng_iamuser.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/reseng_iotanalyticspipeline.py` & `paco-cloud-9.3.9/src/paco/application/reseng_iotanalyticspipeline.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/reseng_iottopicrule.py` & `paco-cloud-9.3.9/src/paco/application/reseng_iottopicrule.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/reseng_lambda.py` & `paco-cloud-9.3.9/src/paco/application/reseng_lambda.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/reseng_lb.py` & `paco-cloud-9.3.9/src/paco/application/reseng_lb.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/reseng_rds.py` & `paco-cloud-9.3.9/src/paco/application/reseng_rds.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/application/reseng_s3bucket.py` & `paco-cloud-9.3.9/src/paco/application/reseng_s3bucket.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/aws_api/acm/ACM.py` & `paco-cloud-9.3.9/src/paco/aws_api/acm/ACM.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/aws_api/awslambda/code.py` & `paco-cloud-9.3.9/src/paco/aws_api/awslambda/code.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/aws_api/ecs/capacityprovider.py` & `paco-cloud-9.3.9/src/paco/aws_api/ecs/capacityprovider.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/aws_api/iam/user.py` & `paco-cloud-9.3.9/src/paco/aws_api/iam/user.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/aws_api/iot/iotpolicy.py` & `paco-cloud-9.3.9/src/paco/aws_api/iot/iotpolicy.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/aws_api/ssm/document.py` & `paco-cloud-9.3.9/src/paco/aws_api/ssm/document.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/__init__.py` & `paco-cloud-9.3.9/src/paco/cftemplates/__init__.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/apigateway.py` & `paco-cloud-9.3.9/src/paco/cftemplates/apigateway.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/asg.py` & `paco-cloud-9.3.9/src/paco/cftemplates/asg.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/backup.py` & `paco-cloud-9.3.9/src/paco/cftemplates/backup.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/cftemplates.py` & `paco-cloud-9.3.9/src/paco/cftemplates/cftemplates.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/cloudfront.py` & `paco-cloud-9.3.9/src/paco/cftemplates/cloudfront.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/cloudtrail.py` & `paco-cloud-9.3.9/src/paco/cftemplates/cloudtrail.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/codebuild.py` & `paco-cloud-9.3.9/src/paco/cftemplates/codebuild.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/codecommit.py` & `paco-cloud-9.3.9/src/paco/cftemplates/codecommit.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/codedeploy.py` & `paco-cloud-9.3.9/src/paco/cftemplates/codedeploy.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/codedeployapplication.py` & `paco-cloud-9.3.9/src/paco/cftemplates/codedeployapplication.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/codepipeline.py` & `paco-cloud-9.3.9/src/paco/cftemplates/codepipeline.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/cognito.py` & `paco-cloud-9.3.9/src/paco/cftemplates/cognito.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/config.py` & `paco-cloud-9.3.9/src/paco/cftemplates/config.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/cw_alarms.py` & `paco-cloud-9.3.9/src/paco/cftemplates/cw_alarms.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,16 @@
     def set_alarm_actions_to_cfn_export(self, alarm, cfn_export_dict):
         "Sets the AlarmActions, OKActions and InsufficientDataActions for a Troposphere dict"
         alarm_action_list = []
         alarm_parent = get_parent_by_interface(alarm, schemas.IResource)
         alarm_account = alarm_parent.get_account()
         if alarm_account.name not in self.paco_ctx.project['resource']['sns'].computed.keys() or \
             alarm.region_name not in self.paco_ctx.project['resource']['sns'].computed[alarm_account.name].keys():
-                raise MissingSNSTopcis(f'Could not find SNS topics for account "{alarm_account.name}" in region "{alarm.region_name}"')
+                message = f'Could not find SNS topics for account "{alarm_account.name}" in region "{alarm.region_name}"'
+                raise MissingSNSTopcis(message)
         notification_groups = self.paco_ctx.project['resource']['sns'].computed[alarm_account.name][alarm.region_name]
         for alarm_action in alarm.get_alarm_actions_paco_refs(notification_groups):
             # Create parameter
             param_name = 'AlarmAction{}'.format(utils.md5sum(str_data=alarm_action))
             if param_name in self.alarm_action_param_map.keys():
                 alarm_action_param = self.alarm_action_param_map[param_name]
             else:
```

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/dashboard.py` & `paco-cloud-9.3.9/src/paco/cftemplates/dashboard.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/dynamodb.py` & `paco-cloud-9.3.9/src/paco/cftemplates/dynamodb.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/ebs.py` & `paco-cloud-9.3.9/src/paco/cftemplates/ebs.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/ecr.py` & `paco-cloud-9.3.9/src/paco/cftemplates/ecr.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/ecs.py` & `paco-cloud-9.3.9/src/paco/cftemplates/ecs.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,24 +64,24 @@
     LIST_CACHE=${SERVICE_LIST_CACHE}".data"
     if [ ! -e ${LIST_CACHE} ] ; then
 	aws ecs list-services --cluster ${CLUSTER_ARN} --query 'serviceArns[]' --output text >${LIST_CACHE}
     fi
     for SERVICE_ARN in $(cat ${LIST_CACHE})
     do
         if [ "$LIST_TYPE" == ""  ] ; then
-            SERVICE=$(echo "$SERVICE_ARN" | awk -F '/' '{print $3}' | awk -F '-' '{print $10}' | awk -F 'Service' '{print $2}' | tr '[:upper:]' '[:lower:]')
+            SERVICE=$(echo "$SERVICE_ARN" | awk -F '/' '{print $3}' | awk -F '-' '{print $11}' | awk -F 'Service' '{print $2}' | tr '[:upper:]' '[:lower:]')
         elif [ "$LIST_TYPE" == "full" ] ; then
             SERVICE=$(echo "$SERVICE_ARN" | awk -F '/' '{print $3}')
         elif [ "$LIST_TYPE" == "arns" ] ; then
             SERVICE="${SERVICE_ARN}"
 	elif [ "$LIST_TYPE" == "lookup" ] ; then
-	    SERVICE=$(echo "$SERVICE_ARN" | awk -F '/' '{print $3}' | awk -F '-' '{print $10}' | awk -F 'Service' '{print $2}' | tr '[:upper:]' '[:lower:]')
+	    SERVICE=$(echo "$SERVICE_ARN" | awk -F '/' '{print $3}' | awk -F '-' '{print $11}' | awk -F 'Service' '{print $2}' | tr '[:upper:]' '[:lower:]')
 	    if [ "$SERVICE" == "$2" ] ; then
-		echo "$SERVICE_ARN" | awk -F '/' '{print $3}'
-		return
+		    echo "$SERVICE_ARN" | awk -F '/' '{print $3}'
+		    return
 	    fi
         else
             echo "error: unknown list type: ${LIST_TYPE}"
             exit 1
         fi
         echo "${SERVICE}"
     done
@@ -89,26 +89,29 @@
 
 function list_tasks() {
     SERVICE_NAME_ARG=$(echo $1 | tr '[:upper:]' '[:lower:]')
     LIST_TYPE="$2"
 
     for SERVICE in $(list_services full)
     do
+        SHORT_SERVICE_NAME=$(echo $SERVICE | awk -F '-' '{print $11}' | awk -F 'Service' '{print $2}' | tr '[:upper:]' '[:lower:]')
+        if [ "${SHORT_SERVICE_NAME}" != "${SERVICE_NAME_ARG}" ] ; then
+            continue
+        fi
         #echo "aws ecs list-tasks --cluster ${CLUSTER_ARN} --service-name ${SERVICE} --query 'taskArns[]' --output text"
         for TASK_ARN in $(aws ecs list-tasks --cluster ${CLUSTER_ARN} --service-name ${SERVICE} --query 'taskArns[]' --output text)
         do
             if [ "$LIST_TYPE" == "arns" ] ; then
                 echo "$TASK_ARN"
             else
                 TASK=$(echo $TASK_ARN | awk -F'/' '{print $3}')
                 CONTAINER_INSTANCE_ARN=$(aws ecs describe-tasks --cluster ${CLUSTER_ARN} --tasks ${TASK} --query 'tasks[0].containerInstanceArn' --output text)
                 INSTANCE_ID=$(aws ecs describe-container-instances --cluster ${CLUSTER} --container-instances ${CONTAINER_INSTANCE_ARN} --query 'containerInstances[0].ec2InstanceId' --output text)
                 IP_ADDRESS=$(aws ec2 describe-instances --instance-ids ${INSTANCE_ID} --query 'Reservations[0].Instances[0].PrivateIpAddress' --output text)
                 DOCKER_TASK=$(aws ecs describe-tasks --cluster ${CLUSTER} --tasks ${TASK} --query 'tasks[0].containers[0].runtimeId' --output text)
-                SHORT_SERVICE_NAME=$(echo $SERVICE | awk -F '-' '{print $10}' | awk -F 'Service' '{print $2}' | tr '[:upper:]' '[:lower:]')
                 echo -e "${SHORT_SERVICE_NAME}	${IP_ADDRESS}	${DOCKER_TASK}"
             fi
         done
     done
 
 }
 
@@ -126,23 +129,137 @@
 	    restart_service $SERVICE
 	done
     else
         restart_service $(list_services lookup $SERVICE)
     fi
 }
 
+SSH_IP="NULL"
+SSH_DOCKER_TASK="NULL"
+function ssh_get_ip() {
+    SERVICE_NAME_ARG=$(echo $1 | tr '[:upper:]' '[:lower:]')
+    TASK_ARG="NULL"
+    if [ $# -eq 2 ] ; then
+        TASK_ARG=$2
+    fi
+
+    SERVICE_OPTION=""
+    SERVICE=""
+    for SERVICE_ARN in $(list_services arns)
+    do
+        SERVICE=$(echo "$SERVICE_ARN" |  awk -F '/' '{print $3}')
+        SERVICE_OPTION=$(echo "$SERVICE" | awk -F '-' '{print $11}' | awk -F 'Service' '{print $2}' | tr '[:upper:]' '[:lower:]')
+        if [ "$SERVICE_OPTION" == "$SERVICE_NAME_ARG" ] ; then
+            break
+        fi
+        SERVICE_OPTION=""
+    done
+
+    if [ "$SERVICE_OPTION" == "" ] ; then
+        echo "error: '${SERVICE_NAME_ARG}' was not found."
+        echo
+        usage
+    fi
+
+    SERVICE_ARN="${ARN_PREFIX}:service/${CLUSTER}/${SERVICE}"
+
+    TASK_IDX=0
+    NUM_TASKS=$(aws ecs list-tasks --cluster ${CLUSTER_ARN} --service-name ${SERVICE} --query 'length(taskArns)')
+    if [ $NUM_TASKS -gt 1 ] ; then
+        if [ "$TASK_ARG" == "NULL" ] ; then
+            echo "More than one task is running for '${SERVICE_NAME_ARG}'. Please specify a Task Id."
+            echo "       Task Id                         ""     Start Time"
+        fi
+        IDX=0
+        for TASK_ARN in $(list-tasks ${SERVICE} arns) #$(aws ecs list-tasks --cluster ${CLUSTER_ARN} --service-name ${SERVICE} --query 'taskArns[]' --output text)
+        do
+            IDX=$(($IDX+1))
+            TASK=$(echo $TASK_ARN | awk -F'/' '{print $3}')
+            if [ "$TASK_ARG" == "$TASK" ] ; then
+                break
+            fi
+            if [ "$TASK_ARG" == "NULL" ] ; then
+                TASK_STARTED_AT=$(aws ecs describe-tasks --cluster ${CLUSTER} --tasks ${TASK} --query 'tasks[0].startedAt' --output text)
+                echo "    ${IDX}) ${TASK}     "$(date -d @${TASK_STARTED_AT})
+            fi
+        done
+        while :
+        do
+            if [ "$TASK_ARG" == "$TASK" ] ; then
+                # break if the users Task argument was found
+                break
+            elif [ "$TASK_ARG" != "NULL" ] ; then
+                # Unable to find the users Task
+                echo "error: '${TASK_ARG}' task is not running"
+                exit 1
+            fi
+            read -p "Select a task: [1-$IDX]: " TASK_IDX
+            if [ $TASK_IDX -ge 1 -a $TASK_IDX -le $NUM_TASKS ] ; then
+                # Array is 0 based so decrement by 1
+                TASK_IDX=$(($TASK_IDX-1))
+                break
+            fi
+            echo "error: '$TASK_IDX' must be an integer between 1 and $NUM_TASKS"
+            echo
+        done
+    fi
+
+    TASK=$(aws ecs list-tasks --cluster ${CLUSTER_ARN} --service-name ${SERVICE} --query "taskArns[$TASK_IDX]" --output text | awk -F'/' '{print $3}')
+    CONTAINER_INSTANCE_ARN=$(aws ecs describe-tasks --cluster ${CLUSTER_ARN} --tasks ${TASK} --query 'tasks[0].containerInstanceArn' --output text)
+    INSTANCE_ID=$(aws ecs describe-container-instances --cluster ${CLUSTER} --container-instances ${CONTAINER_INSTANCE_ARN} --query 'containerInstances[0].ec2InstanceId' --output text)
+    IP_ADDRESS=$(aws ec2 describe-instances --instance-ids ${INSTANCE_ID} --query 'Reservations[0].Instances[0].PrivateIpAddress' --output text)
+    DOCKER_TASK=$(aws ecs describe-tasks --cluster ${CLUSTER} --tasks ${TASK} --query 'tasks[0].containers[0].runtimeId' --output text)
+    export SSH_DOCKER_TASK=${DOCKER_TASK}
+    export SSH_IP=${IP_ADDRESS}
+}
+
+function ssh_service() {
+    SERVICE_NAME_ARG=$(echo $1 | tr '[:upper:]' '[:lower:]')
+    TASK_ARG="NULL"
+    if [ $# -eq 2 ] ; then
+        TASK_ARG=$2
+    fi
+
+
+    ssh_get_ip $SERVICE_NAME_ARG $TASK_ARG
+
+    echo
+    echo "ecs-ssh: ${SERVICE_NAME_ARG}: SSH to ${IP_ADDRESS} for docker task id ${DOCKER_TASK}"
+
+    ssh ${SSH_IP}
+}
+
+function docker_exec()
+{
+    SERVICE_NAME_ARG=$(echo $1 | tr '[:upper:]' '[:lower:]')
+    DOCKER_COMMAND="$2"
+    TASK_ARG="NULL"
+    if [ $# -eq 3 ] ; then
+        TASK_ARG=$3
+    fi
+
+    ssh_get_ip $SERVICE_NAME_ARG $TASK_ARG
+
+    SSH_COMMAND="docker exec -it ${SSH_DOCKER_TASK} ${DOCKER_COMMAND}"
+
+    echo "connecting: ssh -t $SSH_IP '${SSH_COMMAND}'"
+    ssh -t ${SSH_IP} "${SSH_COMMAND}"
+}
+
 #function usage() {
 #    echo "$0 <service_name> [task_id]"
 #    echo
 #    echo "Service names:"
 #    list_services
 #    echo
 #    exit 1
 #}
 
+
+
 COMMAND=$1
 shift
 
 
 case ${COMMAND} in
     list-services)
 	    list_services $1
@@ -153,96 +270,24 @@
         exit 0
         ;;
     list-tasks)
         list_tasks $1
         exit 0
         ;;
     ssh)
+        ssh_service $*
+        ;;
+    docker-exec)
+        docker_exec $*
         ;;
     *)
         usage
         ;;
 esac
 
-TASK_ARG="NULL"
-if [ $# -eq 2 ] ; then
-    TASK_ARG=$2
-fi
-
-SERVICE_NAME_ARG=$(echo $1 | tr '[:upper:]' '[:lower:]')
-
-SERVICE_OPTION=""
-SERVICE=""
-for SERVICE_ARN in $(list_services arns)
-do
-    SERVICE=$(echo "$SERVICE_ARN" |  awk -F '/' '{print $3}')
-    SERVICE_OPTION=$(echo "$SERVICE" | awk -F '-' '{print $10}' | awk -F 'Service' '{print $2}' | tr '[:upper:]' '[:lower:]')
-    if [ "$SERVICE_OPTION" == "$SERVICE_NAME_ARG" ] ; then
-        break
-    fi
-    SERVICE_OPTION=""
-done
-
-if [ "$SERVICE_OPTION" == "" ] ; then
-    echo "error: '${SERVICE_NAME_ARG}' was not found."
-    echo
-    usage
-fi
-
-SERVICE_ARN="${ARN_PREFIX}:service/${CLUSTER}/${SERVICE}"
-
-TASK_IDX=0
-NUM_TASKS=$(aws ecs list-tasks --cluster ${CLUSTER_ARN} --service-name ${SERVICE} --query 'length(taskArns)')
-if [ $NUM_TASKS -gt 1 ] ; then
-    if [ "$TASK_ARG" == "NULL" ] ; then
-        echo "More than one task is running for '${SERVICE_NAME_ARG}'. Please specify a Task Id."
-        echo "       Task Id                         ""     Start Time"
-    fi
-    IDX=0
-    for TASK_ARN in $(list-tasks ${SERVICE} arns) #$(aws ecs list-tasks --cluster ${CLUSTER_ARN} --service-name ${SERVICE} --query 'taskArns[]' --output text)
-    do
-        IDX=$(($IDX+1))
-        TASK=$(echo $TASK_ARN | awk -F'/' '{print $3}')
-        if [ "$TASK_ARG" == "$TASK" ] ; then
-            break
-        fi
-        if [ "$TASK_ARG" == "NULL" ] ; then
-            TASK_STARTED_AT=$(aws ecs describe-tasks --cluster ${CLUSTER} --tasks ${TASK} --query 'tasks[0].startedAt' --output text)
-            echo "    ${IDX}) ${TASK}     "$(date -d @${TASK_STARTED_AT})
-        fi
-    done
-    while :
-    do
-        if [ "$TASK_ARG" == "$TASK" ] ; then
-            # break if the users Task argument was found
-            break
-        elif [ "$TASK_ARG" != "NULL" ] ; then
-            # Unable to find the users Task
-            echo "error: '${TASK_ARG}' task is not running"
-            exit 1
-        fi
-        read -p "Select a task: [1-$IDX]: " TASK_IDX
-        if [ $TASK_IDX -ge 1 -a $TASK_IDX -le $NUM_TASKS ] ; then
-            # Array is 0 based so decrement by 1
-            TASK_IDX=$(($TASK_IDX-1))
-            break
-        fi
-        echo "error: '$TASK_IDX' must be an integer between 1 and $NUM_TASKS"
-        echo
-    done
-fi
-
-TASK=$(aws ecs list-tasks --cluster ${CLUSTER_ARN} --service-name ${SERVICE} --query "taskArns[$TASK_IDX]" --output text | awk -F'/' '{print $3}')
-CONTAINER_INSTANCE_ARN=$(aws ecs describe-tasks --cluster ${CLUSTER_ARN} --tasks ${TASK} --query 'tasks[0].containerInstanceArn' --output text)
-INSTANCE_ID=$(aws ecs describe-container-instances --cluster ${CLUSTER} --container-instances ${CONTAINER_INSTANCE_ARN} --query 'containerInstances[0].ec2InstanceId' --output text)
-IP_ADDRESS=$(aws ec2 describe-instances --instance-ids ${INSTANCE_ID} --query 'Reservations[0].Instances[0].PrivateIpAddress' --output text)
-DOCKER_TASK=$(aws ecs describe-tasks --cluster ${CLUSTER} --tasks ${TASK} --query 'tasks[0].containers[0].runtimeId' --output text)
-echo
-echo "ecs-ssh: ${SERVICE_NAME_ARG}: SSH to ${IP_ADDRESS} for docker task id ${DOCKER_TASK}"
-ssh ${IP_ADDRESS}
 """
 
 class ECSCluster(StackTemplate):
     def __init__(self, stack, paco_ctx):
         ecs_cluster = stack.resource
         super().__init__(stack, paco_ctx)
         self.set_aws_name('ECSCluster', self.resource_group_name, self.resource.name)
```

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/efs.py` & `paco-cloud-9.3.9/src/paco/cftemplates/efs.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/eip.py` & `paco-cloud-9.3.9/src/paco/cftemplates/eip.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/elasticache.py` & `paco-cloud-9.3.9/src/paco/cftemplates/elasticache.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/elasticsearch.py` & `paco-cloud-9.3.9/src/paco/cftemplates/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/eventsrule.py` & `paco-cloud-9.3.9/src/paco/cftemplates/eventsrule.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/example_template.py` & `paco-cloud-9.3.9/src/paco/cftemplates/example_template.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/iam_managed_policies.py` & `paco-cloud-9.3.9/src/paco/cftemplates/iam_managed_policies.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/iam_roles.py` & `paco-cloud-9.3.9/src/paco/cftemplates/iam_roles.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/iam_sl_roles.py` & `paco-cloud-9.3.9/src/paco/cftemplates/iam_sl_roles.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/iam_user_account_delegates.py` & `paco-cloud-9.3.9/src/paco/cftemplates/iam_user_account_delegates.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/iam_users.py` & `paco-cloud-9.3.9/src/paco/cftemplates/iam_users.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/iamuser.py` & `paco-cloud-9.3.9/src/paco/cftemplates/iamuser.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/iotanalyticspipeline.py` & `paco-cloud-9.3.9/src/paco/cftemplates/iotanalyticspipeline.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/iottopicrule.py` & `paco-cloud-9.3.9/src/paco/cftemplates/iottopicrule.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/kms.py` & `paco-cloud-9.3.9/src/paco/cftemplates/kms.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/lambda_function.py` & `paco-cloud-9.3.9/src/paco/cftemplates/lambda_function.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/lb.py` & `paco-cloud-9.3.9/src/paco/cftemplates/lb.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/loggroups.py` & `paco-cloud-9.3.9/src/paco/cftemplates/loggroups.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/nat_gateway.py` & `paco-cloud-9.3.9/src/paco/cftemplates/nat_gateway.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/notification_rules.py` & `paco-cloud-9.3.9/src/paco/cftemplates/notification_rules.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/pinpointapplication.py` & `paco-cloud-9.3.9/src/paco/cftemplates/pinpointapplication.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/rds.py` & `paco-cloud-9.3.9/src/paco/cftemplates/rds.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/route53.py` & `paco-cloud-9.3.9/src/paco/cftemplates/route53.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/route53_hostedzone.py` & `paco-cloud-9.3.9/src/paco/cftemplates/route53_hostedzone.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/route53_recordset.py` & `paco-cloud-9.3.9/src/paco/cftemplates/route53_recordset.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/route53healthcheck.py` & `paco-cloud-9.3.9/src/paco/cftemplates/route53healthcheck.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/s3.py` & `paco-cloud-9.3.9/src/paco/cftemplates/s3.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/secrets_manager.py` & `paco-cloud-9.3.9/src/paco/cftemplates/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/security_groups.py` & `paco-cloud-9.3.9/src/paco/cftemplates/security_groups.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/segment.py` & `paco-cloud-9.3.9/src/paco/cftemplates/segment.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/sns.py` & `paco-cloud-9.3.9/src/paco/cftemplates/sns.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/snstopics.py` & `paco-cloud-9.3.9/src/paco/cftemplates/snstopics.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/ssmdocument.py` & `paco-cloud-9.3.9/src/paco/cftemplates/ssmdocument.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/tests/__init__.py` & `paco-cloud-9.3.9/src/paco/cftemplates/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/tests/test_asg.py` & `paco-cloud-9.3.9/src/paco/cftemplates/tests/test_asg.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/tests/test_cftemplates.py` & `paco-cloud-9.3.9/src/paco/cftemplates/tests/test_cftemplates.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/tests/test_codecommit.py` & `paco-cloud-9.3.9/src/paco/cftemplates/tests/test_codecommit.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/tests/test_ecs.py` & `paco-cloud-9.3.9/src/paco/cftemplates/tests/test_ecs.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/tests/test_efs.py` & `paco-cloud-9.3.9/src/paco/cftemplates/tests/test_efs.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/tests/test_iam_managed_policies.py` & `paco-cloud-9.3.9/src/paco/cftemplates/tests/test_iam_managed_policies.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/tests/test_iam_roles.py` & `paco-cloud-9.3.9/src/paco/cftemplates/tests/test_iam_roles.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/vpc.py` & `paco-cloud-9.3.9/src/paco/cftemplates/vpc.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cftemplates/vpc_peering.py` & `paco-cloud-9.3.9/src/paco/cftemplates/vpc_peering.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/cli.py` & `paco-cloud-9.3.9/src/paco/commands/cli.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/cmd_delete.py` & `paco-cloud-9.3.9/src/paco/commands/cmd_delete.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/cmd_describe.py` & `paco-cloud-9.3.9/src/paco/commands/cmd_describe.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/cmd_init.py` & `paco-cloud-9.3.9/src/paco/commands/cmd_init.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/cmd_lambda.py` & `paco-cloud-9.3.9/src/paco/commands/cmd_lambda.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/cmd_provision.py` & `paco-cloud-9.3.9/src/paco/commands/cmd_provision.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/cmd_set.py` & `paco-cloud-9.3.9/src/paco/commands/cmd_set.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/cmd_shell.py` & `paco-cloud-9.3.9/src/paco/commands/cmd_shell.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/cmd_validate.py` & `paco-cloud-9.3.9/src/paco/commands/cmd_validate.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/cookiecutter_test.py` & `paco-cloud-9.3.9/src/paco/commands/cookiecutter_test.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/display/accounts.pt` & `paco-cloud-9.3.9/src/paco/commands/display/accounts.pt`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/display/env.pt` & `paco-cloud-9.3.9/src/paco/commands/display/env.pt`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/display/globalresources.pt` & `paco-cloud-9.3.9/src/paco/commands/display/globalresources.pt`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/display/html.py` & `paco-cloud-9.3.9/src/paco/commands/display/html.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/display/iam.pt` & `paco-cloud-9.3.9/src/paco/commands/display/iam.pt`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/display/index.pt` & `paco-cloud-9.3.9/src/paco/commands/display/index.pt`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/display/jsonoutput.py` & `paco-cloud-9.3.9/src/paco/commands/display/jsonoutput.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/display/layout-html.pt` & `paco-cloud-9.3.9/src/paco/commands/display/layout-html.pt`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/display/monitoring.pt` & `paco-cloud-9.3.9/src/paco/commands/display/monitoring.pt`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/display/netenvs.pt` & `paco-cloud-9.3.9/src/paco/commands/display/netenvs.pt`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/display/res-ASG.pt` & `paco-cloud-9.3.9/src/paco/commands/display/res-ASG.pt`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/display/res-base.pt` & `paco-cloud-9.3.9/src/paco/commands/display/res-base.pt`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/display/static/assets/main.js` & `paco-cloud-9.3.9/src/paco/commands/display/static/assets/main.js`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/display/static/assets/normalize.css` & `paco-cloud-9.3.9/src/paco/commands/display/static/assets/normalize.css`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/display/static/assets/paco.css` & `paco-cloud-9.3.9/src/paco/commands/display/static/assets/paco.css`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/display/static/assets/skeleton.css` & `paco-cloud-9.3.9/src/paco/commands/display/static/assets/skeleton.css`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/display/static/favicon.ico` & `paco-cloud-9.3.9/src/paco/commands/display/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/commands/helpers.py` & `paco-cloud-9.3.9/src/paco/commands/helpers.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/config/aws_credentials.py` & `paco-cloud-9.3.9/src/paco/config/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/config/config_processor.py` & `paco-cloud-9.3.9/src/paco/config/config_processor.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/config/paco_buckets.py` & `paco-cloud-9.3.9/src/paco/config/paco_buckets.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/config/paco_context.py` & `paco-cloud-9.3.9/src/paco/config/paco_context.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/controllers/__init__.py` & `paco-cloud-9.3.9/src/paco/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/controllers/controllers.py` & `paco-cloud-9.3.9/src/paco/controllers/controllers.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/controllers/ctl_account.py` & `paco-cloud-9.3.9/src/paco/controllers/ctl_account.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/controllers/ctl_cloudtrail.py` & `paco-cloud-9.3.9/src/paco/controllers/ctl_cloudtrail.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/controllers/ctl_cloudwatch.py` & `paco-cloud-9.3.9/src/paco/controllers/ctl_cloudwatch.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/controllers/ctl_codecommit.py` & `paco-cloud-9.3.9/src/paco/controllers/ctl_codecommit.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/controllers/ctl_config.py` & `paco-cloud-9.3.9/src/paco/controllers/ctl_config.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/controllers/ctl_ec2.py` & `paco-cloud-9.3.9/src/paco/controllers/ctl_ec2.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/controllers/ctl_iam.py` & `paco-cloud-9.3.9/src/paco/controllers/ctl_iam.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/controllers/ctl_network_environment.py` & `paco-cloud-9.3.9/src/paco/controllers/ctl_network_environment.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/controllers/ctl_project.py` & `paco-cloud-9.3.9/src/paco/controllers/ctl_project.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/controllers/ctl_route53.py` & `paco-cloud-9.3.9/src/paco/controllers/ctl_route53.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/controllers/ctl_s3.py` & `paco-cloud-9.3.9/src/paco/controllers/ctl_s3.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/controllers/ctl_sns.py` & `paco-cloud-9.3.9/src/paco/controllers/ctl_sns.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/controllers/ctl_snstopics.py` & `paco-cloud-9.3.9/src/paco/controllers/ctl_snstopics.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/controllers/ctl_ssm.py` & `paco-cloud-9.3.9/src/paco/controllers/ctl_ssm.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/controllers/mixins.py` & `paco-cloud-9.3.9/src/paco/controllers/mixins.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/__init__.py` & `paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/__init__.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/cookiecutter.json` & `paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml` & `paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/monitor/Logging.yaml` & `paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/monitor/Logging.yaml`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/dashboards/complete-dashboard.json` & `paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/dashboards/complete-dashboard.json`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/webapp/get_rds_dsn.sh` & `paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/webapp/get_rds_dsn.sh`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml` & `paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/resource/ec2.yaml` & `paco-cloud-9.3.9/src/paco/cookiecutters/managedwebappcicd/{{cookiecutter.project_name}}/resource/ec2.yaml`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/__init__.py` & `paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/__init__.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/cookiecutter.json` & `paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml` & `paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/netenv/pypi-config/pypiserver.service` & `paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/netenv/pypi-config/pypiserver.service`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml` & `paco-cloud-9.3.9/src/paco/cookiecutters/privatepypi/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/__init__.py` & `paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/cookiecutter.json` & `paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml` & `paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/netenv/lambda_code/s3_replicator.py` & `paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/netenv/lambda_code/s3_replicator.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml` & `paco-cloud-9.3.9/src/paco/cookiecutters/s3lambda/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/simplewebapp/__init__.py` & `paco-cloud-9.3.9/src/paco/cookiecutters/simplewebapp/__init__.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/simplewebapp/cookiecutter.json` & `paco-cloud-9.3.9/src/paco/cookiecutters/simplewebapp/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml` & `paco-cloud-9.3.9/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/monitor/Logging.yaml` & `paco-cloud-9.3.9/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/monitor/Logging.yaml`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml` & `paco-cloud-9.3.9/src/paco/cookiecutters/simplewebapp/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/__init__.py` & `paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/__init__.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/cookiecutter.json` & `paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml` & `paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/monitor/AlarmSets.yaml`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml` & `paco-cloud-9.3.9/src/paco/cookiecutters/wordpresssingletier/{{cookiecutter.project_name}}/netenv/{{cookiecutter.network_environment_name}}.yaml`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/core/exception.py` & `paco-cloud-9.3.9/src/paco/core/exception.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/core/yaml.py` & `paco-cloud-9.3.9/src/paco/core/yaml.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/doc/docschema.py` & `paco-cloud-9.3.9/src/paco/doc/docschema.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/extend/__init__.py` & `paco-cloud-9.3.9/src/paco/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/stack/botostack.py` & `paco-cloud-9.3.9/src/paco/stack/botostack.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/stack/botostacks/acm.py` & `paco-cloud-9.3.9/src/paco/stack/botostacks/acm.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/stack/botostacks/iotpolicy.py` & `paco-cloud-9.3.9/src/paco/stack/botostacks/iotpolicy.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/stack/stack.py` & `paco-cloud-9.3.9/src/paco/stack/stack.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/stack/stack_group.py` & `paco-cloud-9.3.9/src/paco/stack/stack_group.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/stack_grps/grp_account.py` & `paco-cloud-9.3.9/src/paco/stack_grps/grp_account.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/stack_grps/grp_application.py` & `paco-cloud-9.3.9/src/paco/stack_grps/grp_application.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/stack_grps/grp_backup.py` & `paco-cloud-9.3.9/src/paco/stack_grps/grp_backup.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/stack_grps/grp_codecommit.py` & `paco-cloud-9.3.9/src/paco/stack_grps/grp_codecommit.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/stack_grps/grp_network.py` & `paco-cloud-9.3.9/src/paco/stack_grps/grp_network.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/stack_grps/grp_route53.py` & `paco-cloud-9.3.9/src/paco/stack_grps/grp_route53.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/stack_grps/grp_secretsmanager.py` & `paco-cloud-9.3.9/src/paco/stack_grps/grp_secretsmanager.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/tests/__init__.py` & `paco-cloud-9.3.9/src/paco/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/utils/__init__.py` & `paco-cloud-9.3.9/src/paco/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/utils/cache.py` & `paco-cloud-9.3.9/src/paco/utils/cache.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco/utils/zip.py` & `paco-cloud-9.3.9/src/paco/utils/zip.py`

 * *Files identical despite different names*

### Comparing `paco-cloud-9.3.8/src/paco_cloud.egg-info/PKG-INFO` & `paco-cloud-9.3.9/src/paco_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paco-cloud
-Version: 9.3.8
+Version: 9.3.9
 Summary: Paco: Prescribed automation for cloud orchestration
 Home-page: https://github.com/waterbear-cloud/paco
 Author: Waterbear Cloud
 Author-email: hello@waterbear.cloud
 License: UNKNOWN
 Description: # Paco: Prescribed automation for cloud orchestration
         
@@ -40,14 +40,26 @@
         
         Paco is created by Kevin Lindsay and Kevin Teague for [Waterbear Cloud](https://waterbear.cloud).
         
         
         Changelog for Paco
         ==================
         
+        9.3.9 (2021-04-19)
+        ------------------
+        
+        ### Added
+        
+        - Added logging to SSM instance EC2LM update run commands.
+        - Added docker-exec command to ECS ScriptManager script.
+        
+        ### Changed
+        
+        - Improved ECR Deploy Script to tag the destination image with the same tags as the source.
+        
         9.3.8 (2021-04-09)
         ------------------
         
         ### Fixed
         
         - Fixed release phase script name in the ECR deploy script.
```

### Comparing `paco-cloud-9.3.8/src/paco_cloud.egg-info/SOURCES.txt` & `paco-cloud-9.3.9/src/paco_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

