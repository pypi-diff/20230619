# Comparing `tmp/clear_skies_aws-1.5.7.tar.gz` & `tmp/clear_skies_aws-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear_skies_aws-1.5.7.tar", max compression
+gzip compressed data, was "clear_skies_aws-1.6.0.tar", max compression
```

## Comparing `clear_skies_aws-1.5.7.tar` & `clear_skies_aws-1.6.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1053 2022-01-16 00:26:29.571128 clear_skies_aws-1.5.7/LICENSE
--rw-r--r--   0        0        0     7780 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.7/README.md
--rw-r--r--   0        0        0      789 2023-06-16 09:57:16.506074 clear_skies_aws-1.5.7/pyproject.toml
--rw-r--r--   0        0        0       58 2023-05-23 15:29:15.831933 clear_skies_aws-1.5.7/src/clearskies_aws/__init__.py
--rw-r--r--   0        0        0     2141 2023-06-07 12:04:20.019789 clear_skies_aws-1.5.7/src/clearskies_aws/actions/__init__.py
--rw-r--r--   0        0        0     3357 2023-06-08 12:35:36.805017 clear_skies_aws-1.5.7/src/clearskies_aws/actions/action_aws.py
--rw-r--r--   0        0        0     4085 2023-06-07 00:11:48.817084 clear_skies_aws-1.5.7/src/clearskies_aws/actions/assume_role.py
--rw-r--r--   0        0        0     2450 2023-06-07 00:11:48.873084 clear_skies_aws-1.5.7/src/clearskies_aws/actions/assume_role_test.py
--rw-r--r--   0        0        0     6914 2023-06-08 12:07:05.650182 clear_skies_aws-1.5.7/src/clearskies_aws/actions/ses.py
--rw-r--r--   0        0        0     1630 2023-06-07 12:04:20.019789 clear_skies_aws-1.5.7/src/clearskies_aws/actions/ses_test.py
--rw-r--r--   0        0        0     2197 2023-06-08 12:06:42.106108 clear_skies_aws-1.5.7/src/clearskies_aws/actions/sns.py
--rw-r--r--   0        0        0     2194 2023-06-07 19:38:57.987774 clear_skies_aws-1.5.7/src/clearskies_aws/actions/sns_test.py
--rw-r--r--   0        0        0     2340 2023-06-08 12:07:13.458206 clear_skies_aws-1.5.7/src/clearskies_aws/actions/sqs.py
--rw-r--r--   0        0        0     2234 2023-06-06 22:38:31.426673 clear_skies_aws-1.5.7/src/clearskies_aws/actions/sqs_test.py
--rw-r--r--   0        0        0       83 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.7/src/clearskies_aws/backends/__init__.py
--rw-r--r--   0        0        0    29126 2023-05-17 10:18:33.296047 clear_skies_aws-1.5.7/src/clearskies_aws/backends/dynamo_db_backend.py
--rw-r--r--   0        0        0    13150 2023-04-27 10:33:09.319573 clear_skies_aws-1.5.7/src/clearskies_aws/backends/dynamo_db_backend_test.py
--rw-r--r--   0        0        0     2726 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.7/src/clearskies_aws/backends/sqs_backend.py
--rw-r--r--   0        0        0     1138 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.7/src/clearskies_aws/backends/sqs_backend_test.py
--rw-r--r--   0        0        0      325 2023-06-16 01:31:49.897322 clear_skies_aws-1.5.7/src/clearskies_aws/contexts/__init__.py
--rw-r--r--   0        0        0     1305 2023-03-26 13:26:58.707778 clear_skies_aws-1.5.7/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     1276 2023-03-26 13:26:58.707778 clear_skies_aws-1.5.7/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     1251 2023-03-26 13:26:58.707778 clear_skies_aws-1.5.7/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc
--rw-r--r--   0        0        0      506 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.7/src/clearskies_aws/contexts/cli.py
--rw-r--r--   0        0        0     1002 2023-03-26 13:26:58.703778 clear_skies_aws-1.5.7/src/clearskies_aws/contexts/lambda_api_gateway.py
--rw-r--r--   0        0        0      952 2023-03-26 13:26:58.703778 clear_skies_aws-1.5.7/src/clearskies_aws/contexts/lambda_elb.py
--rw-r--r--   0        0        0     1009 2023-03-26 13:26:58.703778 clear_skies_aws-1.5.7/src/clearskies_aws/contexts/lambda_http_gateway.py
--rw-r--r--   0        0        0     1183 2023-03-26 13:26:58.703778 clear_skies_aws-1.5.7/src/clearskies_aws/contexts/lambda_invocation.py
--rw-r--r--   0        0        0     1349 2023-06-16 09:57:05.034003 clear_skies_aws-1.5.7/src/clearskies_aws/contexts/lambda_sns.py
--rw-r--r--   0        0        0     1678 2023-04-04 23:13:02.122630 clear_skies_aws-1.5.7/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py
--rw-r--r--   0        0        0     1999 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.7/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py
--rw-r--r--   0        0        0       56 2023-03-26 13:26:58.711778 clear_skies_aws-1.5.7/src/clearskies_aws/di/__init__.py
--rw-r--r--   0        0        0      775 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.7/src/clearskies_aws/di/standard_dependencies.py
--rw-r--r--   0        0        0      267 2023-06-07 19:44:19.148834 clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/__init__.py
--rw-r--r--   0        0        0      943 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     3710 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     2761 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc
--rw-r--r--   0        0        0      901 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc
--rw-r--r--   0        0        0     2932 2023-03-26 13:26:58.711778 clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/lambda_api_gateway.py
--rw-r--r--   0        0        0     2845 2023-03-26 13:26:58.711778 clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py
--rw-r--r--   0        0        0      662 2023-03-26 13:26:58.711778 clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/lambda_elb.py
--rw-r--r--   0        0        0      692 2023-03-26 13:26:58.711778 clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/lambda_http_gateway.py
--rw-r--r--   0        0        0      715 2023-03-26 13:26:58.711778 clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/lambda_invocation.py
--rw-r--r--   0        0        0     2081 2023-06-16 01:36:39.962697 clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/lambda_sns.py
--rw-r--r--   0        0        0     2047 2023-03-26 15:10:17.430380 clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/lambda_sqs_standard.py
--rw-r--r--   0        0        0       22 2023-05-23 15:29:05.208303 clear_skies_aws-1.5.7/src/clearskies_aws/mocks/__init__.py
--rw-r--r--   0        0        0       21 2023-05-23 15:29:05.208303 clear_skies_aws-1.5.7/src/clearskies_aws/mocks/actions/__init__.py
--rw-r--r--   0        0        0      911 2023-05-23 15:29:05.208303 clear_skies_aws-1.5.7/src/clearskies_aws/mocks/actions/ses.py
--rw-r--r--   0        0        0      121 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.7/src/clearskies_aws/secrets/__init__.py
--rw-r--r--   0        0        0     1919 2023-05-19 13:30:13.392139 clear_skies_aws-1.5.7/src/clearskies_aws/secrets/additional_configs/__init__.py
--rw-r--r--   0        0        0     1082 2023-03-26 13:26:58.719778 clear_skies_aws-1.5.7/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py
--rw-r--r--   0        0        0     3467 2023-05-19 13:34:03.783513 clear_skies_aws-1.5.7/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py
--rw-r--r--   0        0        0     3776 2023-03-26 13:26:58.719778 clear_skies_aws-1.5.7/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py
--rw-r--r--   0        0        0     6444 2023-03-26 13:26:58.719778 clear_skies_aws-1.5.7/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py
--rw-r--r--   0        0        0     1655 2023-04-14 14:57:45.726909 clear_skies_aws-1.5.7/src/clearskies_aws/secrets/parameter_store.py
--rw-r--r--   0        0        0      761 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.7/src/clearskies_aws/secrets/parameter_store_test.py
--rw-r--r--   0        0        0     2898 2023-04-14 14:57:45.758909 clear_skies_aws-1.5.7/src/clearskies_aws/secrets/secrets_manager.py
--rw-r--r--   0        0        0      786 2023-03-26 13:26:58.715778 clear_skies_aws-1.5.7/src/clearskies_aws/secrets/secrets_manager_test.py
--rw-r--r--   0        0        0     8579 1970-01-01 00:00:00.000000 clear_skies_aws-1.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1053 2022-01-16 00:26:29.571128 clear_skies_aws-1.6.0/LICENSE
+-rw-r--r--   0        0        0     7780 2023-03-26 15:10:17.430380 clear_skies_aws-1.6.0/README.md
+-rw-r--r--   0        0        0      789 2023-06-19 12:50:27.923247 clear_skies_aws-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0       58 2023-05-23 15:29:15.831933 clear_skies_aws-1.6.0/src/clearskies_aws/__init__.py
+-rw-r--r--   0        0        0     2141 2023-06-07 12:04:20.019789 clear_skies_aws-1.6.0/src/clearskies_aws/actions/__init__.py
+-rw-r--r--   0        0        0     3357 2023-06-08 12:35:36.805017 clear_skies_aws-1.6.0/src/clearskies_aws/actions/action_aws.py
+-rw-r--r--   0        0        0     4085 2023-06-07 00:11:48.817084 clear_skies_aws-1.6.0/src/clearskies_aws/actions/assume_role.py
+-rw-r--r--   0        0        0     2450 2023-06-07 00:11:48.873084 clear_skies_aws-1.6.0/src/clearskies_aws/actions/assume_role_test.py
+-rw-r--r--   0        0        0     6914 2023-06-08 12:07:05.650182 clear_skies_aws-1.6.0/src/clearskies_aws/actions/ses.py
+-rw-r--r--   0        0        0     1630 2023-06-07 12:04:20.019789 clear_skies_aws-1.6.0/src/clearskies_aws/actions/ses_test.py
+-rw-r--r--   0        0        0     2197 2023-06-08 12:06:42.106108 clear_skies_aws-1.6.0/src/clearskies_aws/actions/sns.py
+-rw-r--r--   0        0        0     2194 2023-06-07 19:38:57.987774 clear_skies_aws-1.6.0/src/clearskies_aws/actions/sns_test.py
+-rw-r--r--   0        0        0     2340 2023-06-08 12:07:13.458206 clear_skies_aws-1.6.0/src/clearskies_aws/actions/sqs.py
+-rw-r--r--   0        0        0     2234 2023-06-06 22:38:31.426673 clear_skies_aws-1.6.0/src/clearskies_aws/actions/sqs_test.py
+-rw-r--r--   0        0        0       83 2023-03-26 15:10:17.430380 clear_skies_aws-1.6.0/src/clearskies_aws/backends/__init__.py
+-rw-r--r--   0        0        0    29126 2023-05-17 10:18:33.296047 clear_skies_aws-1.6.0/src/clearskies_aws/backends/dynamo_db_backend.py
+-rw-r--r--   0        0        0    13150 2023-04-27 10:33:09.319573 clear_skies_aws-1.6.0/src/clearskies_aws/backends/dynamo_db_backend_test.py
+-rw-r--r--   0        0        0     2726 2023-03-26 15:10:17.430380 clear_skies_aws-1.6.0/src/clearskies_aws/backends/sqs_backend.py
+-rw-r--r--   0        0        0     1138 2023-03-26 15:10:17.430380 clear_skies_aws-1.6.0/src/clearskies_aws/backends/sqs_backend_test.py
+-rw-r--r--   0        0        0      325 2023-06-16 01:31:49.897322 clear_skies_aws-1.6.0/src/clearskies_aws/contexts/__init__.py
+-rw-r--r--   0        0        0     1305 2023-03-26 13:26:58.707778 clear_skies_aws-1.6.0/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     1276 2023-03-26 13:26:58.707778 clear_skies_aws-1.6.0/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     1251 2023-03-26 13:26:58.707778 clear_skies_aws-1.6.0/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc
+-rw-r--r--   0        0        0      506 2023-03-26 15:10:17.430380 clear_skies_aws-1.6.0/src/clearskies_aws/contexts/cli.py
+-rw-r--r--   0        0        0     1002 2023-03-26 13:26:58.703778 clear_skies_aws-1.6.0/src/clearskies_aws/contexts/lambda_api_gateway.py
+-rw-r--r--   0        0        0      952 2023-03-26 13:26:58.703778 clear_skies_aws-1.6.0/src/clearskies_aws/contexts/lambda_elb.py
+-rw-r--r--   0        0        0     1009 2023-03-26 13:26:58.703778 clear_skies_aws-1.6.0/src/clearskies_aws/contexts/lambda_http_gateway.py
+-rw-r--r--   0        0        0     1183 2023-03-26 13:26:58.703778 clear_skies_aws-1.6.0/src/clearskies_aws/contexts/lambda_invocation.py
+-rw-r--r--   0        0        0     1317 2023-06-19 12:47:47.710621 clear_skies_aws-1.6.0/src/clearskies_aws/contexts/lambda_sns.py
+-rw-r--r--   0        0        0     1685 2023-06-19 12:49:55.399120 clear_skies_aws-1.6.0/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py
+-rw-r--r--   0        0        0     1999 2023-03-26 15:10:17.430380 clear_skies_aws-1.6.0/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py
+-rw-r--r--   0        0        0       56 2023-03-26 13:26:58.711778 clear_skies_aws-1.6.0/src/clearskies_aws/di/__init__.py
+-rw-r--r--   0        0        0      775 2023-03-26 15:10:17.430380 clear_skies_aws-1.6.0/src/clearskies_aws/di/standard_dependencies.py
+-rw-r--r--   0        0        0      267 2023-06-07 19:44:19.148834 clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/__init__.py
+-rw-r--r--   0        0        0      943 2023-03-26 13:26:58.715778 clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     3710 2023-03-26 13:26:58.715778 clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     2761 2023-03-26 13:26:58.715778 clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc
+-rw-r--r--   0        0        0      901 2023-03-26 13:26:58.715778 clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc
+-rw-r--r--   0        0        0     3065 2023-06-19 12:48:55.506886 clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/lambda_api_gateway.py
+-rw-r--r--   0        0        0     2845 2023-03-26 13:26:58.711778 clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py
+-rw-r--r--   0        0        0      662 2023-03-26 13:26:58.711778 clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/lambda_elb.py
+-rw-r--r--   0        0        0      692 2023-03-26 13:26:58.711778 clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/lambda_http_gateway.py
+-rw-r--r--   0        0        0      715 2023-03-26 13:26:58.711778 clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/lambda_invocation.py
+-rw-r--r--   0        0        0     2163 2023-06-19 12:49:21.822989 clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/lambda_sns.py
+-rw-r--r--   0        0        0     2082 2023-06-19 12:50:01.219143 clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/lambda_sqs_standard.py
+-rw-r--r--   0        0        0       22 2023-05-23 15:29:05.208303 clear_skies_aws-1.6.0/src/clearskies_aws/mocks/__init__.py
+-rw-r--r--   0        0        0       21 2023-05-23 15:29:05.208303 clear_skies_aws-1.6.0/src/clearskies_aws/mocks/actions/__init__.py
+-rw-r--r--   0        0        0      911 2023-05-23 15:29:05.208303 clear_skies_aws-1.6.0/src/clearskies_aws/mocks/actions/ses.py
+-rw-r--r--   0        0        0      121 2023-03-26 13:26:58.715778 clear_skies_aws-1.6.0/src/clearskies_aws/secrets/__init__.py
+-rw-r--r--   0        0        0     1919 2023-05-19 13:30:13.392139 clear_skies_aws-1.6.0/src/clearskies_aws/secrets/additional_configs/__init__.py
+-rw-r--r--   0        0        0     1082 2023-03-26 13:26:58.719778 clear_skies_aws-1.6.0/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py
+-rw-r--r--   0        0        0     3467 2023-05-19 13:34:03.783513 clear_skies_aws-1.6.0/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py
+-rw-r--r--   0        0        0     3776 2023-03-26 13:26:58.719778 clear_skies_aws-1.6.0/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py
+-rw-r--r--   0        0        0     6444 2023-03-26 13:26:58.719778 clear_skies_aws-1.6.0/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py
+-rw-r--r--   0        0        0     1655 2023-04-14 14:57:45.726909 clear_skies_aws-1.6.0/src/clearskies_aws/secrets/parameter_store.py
+-rw-r--r--   0        0        0      761 2023-03-26 13:26:58.715778 clear_skies_aws-1.6.0/src/clearskies_aws/secrets/parameter_store_test.py
+-rw-r--r--   0        0        0     2898 2023-04-14 14:57:45.758909 clear_skies_aws-1.6.0/src/clearskies_aws/secrets/secrets_manager.py
+-rw-r--r--   0        0        0      786 2023-03-26 13:26:58.715778 clear_skies_aws-1.6.0/src/clearskies_aws/secrets/secrets_manager_test.py
+-rw-r--r--   0        0        0     8579 1970-01-01 00:00:00.000000 clear_skies_aws-1.6.0/PKG-INFO
```

### Comparing `clear_skies_aws-1.5.7/LICENSE` & `clear_skies_aws-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/README.md` & `clear_skies_aws-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/pyproject.toml` & `clear_skies_aws-1.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "clear-skies-aws"
-version = "1.5.7"
+version = "1.6.0"
 description = "clearskies bindings for working in AWS"
 authors = [
     "Conor Mancone <cmancone@gmail.com>",
     "tnijboer"
 ]
 repository = "https://github.com/cmancone/clearskies-aws"
 license = "MIT"
```

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/actions/__init__.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/actions/action_aws.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/actions/action_aws.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/actions/assume_role.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/actions/assume_role.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/actions/assume_role_test.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/actions/assume_role_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/actions/ses.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/actions/ses.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/actions/ses_test.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/actions/ses_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/actions/sns.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/actions/sns.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/actions/sns_test.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/actions/sns_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/actions/sqs.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/actions/sqs.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/actions/sqs_test.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/actions/sqs_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/backends/dynamo_db_backend.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/backends/dynamo_db_backend.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/backends/dynamo_db_backend_test.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/backends/dynamo_db_backend_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/backends/sqs_backend.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/backends/sqs_backend.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/backends/sqs_backend_test.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/backends/sqs_backend_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.6.0/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.6.0/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc` & `clear_skies_aws-1.6.0/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/contexts/lambda_api_gateway.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/contexts/lambda_api_gateway.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/contexts/lambda_elb.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/contexts/lambda_elb.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/contexts/lambda_http_gateway.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/contexts/lambda_http_gateway.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/contexts/lambda_invocation.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/contexts/lambda_invocation.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/contexts/lambda_sns.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/contexts/lambda_sns.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         }
 
     def __call__(self, event, context):
         if self.handler is None:
             raise ValueError("Cannot execute LambdaSnsEvent context without first configuring it")
 
         try:
-            return self.handler(LambdaSnsInputOutput(event['Records'][0]['Sns']['Message'], context))
+            return self.handler(LambdaSnsInputOutput(event, context))
         except Exception as e:
             print('Failed message ' + event['Records'][0]['Sns']['MessageId'] + '. Error error: ' + str(e))
             raise e
 
 def lambda_sns(
     application,
     di_class=StandardDependencies,
```

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     def __call__(self, event, context):
         if self.handler is None:
             raise ValueError("Cannot execute LambdaELB context without first configuring it")
 
         item_failures = []
         for record in event['Records']:
             try:
-                self.handler(LambdaSqsStandardInputOutput(record['body'], context))
+                self.handler(LambdaSqsStandardInputOutput(record['body'], event, context))
             except Exception as e:
                 print('Failed message ' + record['messageId'] + ' being returned for retry.  Error error: ' + str(e))
                 item_failures.append({'itemIdentifier': record['messageId']})
 
         if item_failures:
             return {
                 "batchItemFailures": item_failures,
```

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/di/standard_dependencies.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/di/standard_dependencies.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc` & `clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc` & `clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/lambda_api_gateway.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/lambda_api_gateway.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,7 +83,13 @@
         return self._request_headers[header_name.lower()]
 
     def get_query_parameter(self, key):
         return self._query_parameters[key] if key in self._query_parameters else []
 
     def get_query_parameters(self):
         return self._query_parameters
+
+    def context_specifics(self):
+        return {
+            "event": self._event,
+            "context": self._context,
+        }
```

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/lambda_elb.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/lambda_elb.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/lambda_http_gateway.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/lambda_http_gateway.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/lambda_invocation.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/lambda_invocation.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/lambda_sns.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/lambda_sns.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from .lambda_api_gateway import LambdaAPIGateway
 from clearskies.handlers.exceptions import ClientError
 import json
 class LambdaSns(LambdaAPIGateway):
-    def __init__(self, record, context):
+    def __init__(self, event, context):
+        self._event = event
+        self._context = context
+        record = event['Records'][0]['Sns']['Message']
         try:
             self._record = json.loads(record)
         except json.JSONDecodeError as e:
             raise ClientError("The message from AWS was not a serialized JSON string.  The lambda_sns context for clearskies only accepts serialized JSON")
-        self._context = context
 
     def respond(self, body, status_code=200):
         pass
 
     def get_body(self):
         return self._record
```

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/input_outputs/lambda_sqs_standard.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/input_outputs/lambda_sqs_standard.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .lambda_api_gateway import LambdaAPIGateway
 from clearskies.handlers.exceptions import ClientError
 import json
 class LambdaSqsStandard(LambdaAPIGateway):
-    def __init__(self, record, context):
+    def __init__(self, record, event, context):
         self._record = record
         self._context = context
+        self._event = event
 
     def respond(self, body, status_code=200):
         pass
 
     def get_body(self):
         return self._record
```

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/mocks/actions/ses.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/mocks/actions/ses.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/secrets/additional_configs/__init__.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/secrets/additional_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/secrets/parameter_store.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/secrets/parameter_store.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/secrets/parameter_store_test.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/secrets/parameter_store_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/secrets/secrets_manager.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/secrets/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/src/clearskies_aws/secrets/secrets_manager_test.py` & `clear_skies_aws-1.6.0/src/clearskies_aws/secrets/secrets_manager_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.5.7/PKG-INFO` & `clear_skies_aws-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-aws
-Version: 1.5.7
+Version: 1.6.0
 Summary: clearskies bindings for working in AWS
 Home-page: https://github.com/cmancone/clearskies-aws
 License: MIT
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

