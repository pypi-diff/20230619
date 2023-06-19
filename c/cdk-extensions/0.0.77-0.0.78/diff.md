# Comparing `tmp/cdk-extensions-0.0.77.tar.gz` & `tmp/cdk-extensions-0.0.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-extensions-0.0.77.tar", last modified: Mon Jun 19 03:55:40 2023, max compression
+gzip compressed data, was "cdk-extensions-0.0.78.tar", last modified: Mon Jun 19 06:04:22 2023, max compression
```

## Comparing `cdk-extensions-0.0.77.tar` & `cdk-extensions-0.0.78.tar`

### file list

```diff
@@ -1,67 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.014815 cdk-extensions-0.0.77/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-19 03:55:40.014815 cdk-extensions-0.0.77/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 03:55:40.014815 cdk-extensions-0.0.77/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:39.998815 cdk-extensions-0.0.77/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.002815 cdk-extensions-0.0.77/src/cdk_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.002815 cdk-extensions-0.0.77/src/cdk_extensions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.006815 cdk-extensions-0.0.77/src/cdk_extensions/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/_jsii/bin/init-aws.sh
--rw-r--r--   0 runner    (1001) docker     (123)  1608680 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/_jsii/cdk-extensions@0.0.77.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.006815 cdk-extensions-0.0.77/src/cdk_extensions/aps/
--rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/aps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.006815 cdk-extensions-0.0.77/src/cdk_extensions/asserts/
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/asserts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.006815 cdk-extensions-0.0.77/src/cdk_extensions/athena/
--rw-r--r--   0 runner    (1001) docker     (123)   100087 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/athena/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.006815 cdk-extensions-0.0.77/src/cdk_extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.006815 cdk-extensions-0.0.77/src/cdk_extensions/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)   702338 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/ec2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.010815 cdk-extensions-0.0.77/src/cdk_extensions/ec2_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)   278700 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/ec2_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.010815 cdk-extensions-0.0.77/src/cdk_extensions/eks_patterns/
--rw-r--r--   0 runner    (1001) docker     (123)    95753 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/eks_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.010815 cdk-extensions-0.0.77/src/cdk_extensions/glue/
--rw-r--r--   0 runner    (1001) docker     (123)   507583 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/glue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.010815 cdk-extensions-0.0.77/src/cdk_extensions/glue_tables/
--rw-r--r--   0 runner    (1001) docker     (123)   140852 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/glue_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.010815 cdk-extensions-0.0.77/src/cdk_extensions/k8s_aws/
--rw-r--r--   0 runner    (1001) docker     (123)   692407 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/k8s_aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.010815 cdk-extensions-0.0.77/src/cdk_extensions/k8s_fargate/
--rw-r--r--   0 runner    (1001) docker     (123)    26236 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/k8s_fargate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.014815 cdk-extensions-0.0.77/src/cdk_extensions/kinesis_firehose/
--rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/kinesis_firehose/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.014815 cdk-extensions-0.0.77/src/cdk_extensions/lambda_/
--rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/lambda_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.014815 cdk-extensions-0.0.77/src/cdk_extensions/networkmanager/
--rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/networkmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.014815 cdk-extensions-0.0.77/src/cdk_extensions/ram/
--rw-r--r--   0 runner    (1001) docker     (123)    42369 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/ram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.014815 cdk-extensions-0.0.77/src/cdk_extensions/ram_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/ram_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.014815 cdk-extensions-0.0.77/src/cdk_extensions/rds/
--rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/rds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.014815 cdk-extensions-0.0.77/src/cdk_extensions/resourcegroups/
--rw-r--r--   0 runner    (1001) docker     (123)    39153 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/resourcegroups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.014815 cdk-extensions-0.0.77/src/cdk_extensions/route53/
--rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/route53/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.014815 cdk-extensions-0.0.77/src/cdk_extensions/s3_buckets/
--rw-r--r--   0 runner    (1001) docker     (123)   215415 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/s3_buckets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.014815 cdk-extensions-0.0.77/src/cdk_extensions/sso/
--rw-r--r--   0 runner    (1001) docker     (123)   130481 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/sso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.014815 cdk-extensions-0.0.77/src/cdk_extensions/stacks/
--rw-r--r--   0 runner    (1001) docker     (123)    58263 2023-06-19 03:55:25.000000 cdk-extensions-0.0.77/src/cdk_extensions/stacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:55:40.002815 cdk-extensions-0.0.77/src/cdk_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-19 03:55:39.000000 cdk-extensions-0.0.77/src/cdk_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-19 03:55:39.000000 cdk-extensions-0.0.77/src/cdk_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 03:55:39.000000 cdk-extensions-0.0.77/src/cdk_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-19 03:55:39.000000 cdk-extensions-0.0.77/src/cdk_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-19 03:55:39.000000 cdk-extensions-0.0.77/src/cdk_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.754397 cdk-extensions-0.0.78/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-19 06:04:22.754397 cdk-extensions-0.0.78/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 06:04:22.754397 cdk-extensions-0.0.78/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.738397 cdk-extensions-0.0.78/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.742397 cdk-extensions-0.0.78/src/cdk_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.742397 cdk-extensions-0.0.78/src/cdk_extensions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.746397 cdk-extensions-0.0.78/src/cdk_extensions/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/_jsii/bin/init-aws.sh
+-rw-r--r--   0 runner    (1001) docker     (123)  1745493 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/_jsii/cdk-extensions@0.0.78.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.746397 cdk-extensions-0.0.78/src/cdk_extensions/alerting/
+-rw-r--r--   0 runner    (1001) docker     (123)   277602 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/alerting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.746397 cdk-extensions-0.0.78/src/cdk_extensions/aps/
+-rw-r--r--   0 runner    (1001) docker     (123)   277230 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/aps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.746397 cdk-extensions-0.0.78/src/cdk_extensions/asserts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/asserts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.746397 cdk-extensions-0.0.78/src/cdk_extensions/athena/
+-rw-r--r--   0 runner    (1001) docker     (123)   100087 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/athena/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.746397 cdk-extensions-0.0.78/src/cdk_extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)    20196 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.746397 cdk-extensions-0.0.78/src/cdk_extensions/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)   702338 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/ec2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.746397 cdk-extensions-0.0.78/src/cdk_extensions/ec2_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)   278700 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/ec2_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.750397 cdk-extensions-0.0.78/src/cdk_extensions/eks_patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)    95753 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/eks_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.750397 cdk-extensions-0.0.78/src/cdk_extensions/glue/
+-rw-r--r--   0 runner    (1001) docker     (123)   507583 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/glue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.750397 cdk-extensions-0.0.78/src/cdk_extensions/glue_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)   140852 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/glue_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.750397 cdk-extensions-0.0.78/src/cdk_extensions/k8s_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)   692407 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/k8s_aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.750397 cdk-extensions-0.0.78/src/cdk_extensions/k8s_fargate/
+-rw-r--r--   0 runner    (1001) docker     (123)    26236 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/k8s_fargate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.750397 cdk-extensions-0.0.78/src/cdk_extensions/kinesis_firehose/
+-rw-r--r--   0 runner    (1001) docker     (123)   271406 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/kinesis_firehose/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.750397 cdk-extensions-0.0.78/src/cdk_extensions/lambda_/
+-rw-r--r--   0 runner    (1001) docker     (123)    22981 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/lambda_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.750397 cdk-extensions-0.0.78/src/cdk_extensions/networkmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/networkmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.750397 cdk-extensions-0.0.78/src/cdk_extensions/ram/
+-rw-r--r--   0 runner    (1001) docker     (123)    42369 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/ram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.750397 cdk-extensions-0.0.78/src/cdk_extensions/ram_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/ram_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.754397 cdk-extensions-0.0.78/src/cdk_extensions/rds/
+-rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/rds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.754397 cdk-extensions-0.0.78/src/cdk_extensions/resourcegroups/
+-rw-r--r--   0 runner    (1001) docker     (123)    39153 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/resourcegroups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.754397 cdk-extensions-0.0.78/src/cdk_extensions/route53/
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/route53/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.754397 cdk-extensions-0.0.78/src/cdk_extensions/s3_buckets/
+-rw-r--r--   0 runner    (1001) docker     (123)   215415 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/s3_buckets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.754397 cdk-extensions-0.0.78/src/cdk_extensions/sso/
+-rw-r--r--   0 runner    (1001) docker     (123)   130481 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/sso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.754397 cdk-extensions-0.0.78/src/cdk_extensions/stacks/
+-rw-r--r--   0 runner    (1001) docker     (123)    58263 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/stacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.754397 cdk-extensions-0.0.78/src/cdk_extensions/stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (123)    16540 2023-06-19 06:04:06.000000 cdk-extensions-0.0.78/src/cdk_extensions/stepfunctions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 06:04:22.742397 cdk-extensions-0.0.78/src/cdk_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-06-19 06:04:22.000000 cdk-extensions-0.0.78/src/cdk_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-19 06:04:22.000000 cdk-extensions-0.0.78/src/cdk_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 06:04:22.000000 cdk-extensions-0.0.78/src/cdk_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-19 06:04:22.000000 cdk-extensions-0.0.78/src/cdk_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-19 06:04:22.000000 cdk-extensions-0.0.78/src/cdk_extensions.egg-info/top_level.txt
```

### Comparing `cdk-extensions-0.0.77/LICENSE` & `cdk-extensions-0.0.78/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/PKG-INFO` & `cdk-extensions-0.0.78/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.77
+Version: 0.0.78
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.77/README.md` & `cdk-extensions-0.0.78/README.md`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/setup.py` & `cdk-extensions-0.0.78/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-extensions",
-    "version": "0.0.77",
+    "version": "0.0.78",
     "description": "cdk-extensions",
     "license": "Apache-2.0",
     "url": "https://github.com/vibe-io/cdk-extensions.git",
     "long_description_content_type": "text/markdown",
     "author": "Kevin Lucas<kevinluc08@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -19,14 +19,15 @@
     },
     "package_dir": {
         "": "src"
     },
     "packages": [
         "cdk_extensions",
         "cdk_extensions._jsii",
+        "cdk_extensions.alerting",
         "cdk_extensions.aps",
         "cdk_extensions.asserts",
         "cdk_extensions.athena",
         "cdk_extensions.core",
         "cdk_extensions.ec2",
         "cdk_extensions.ec2_patterns",
         "cdk_extensions.eks_patterns",
@@ -40,19 +41,20 @@
         "cdk_extensions.ram",
         "cdk_extensions.ram_resources",
         "cdk_extensions.rds",
         "cdk_extensions.resourcegroups",
         "cdk_extensions.route53",
         "cdk_extensions.s3_buckets",
         "cdk_extensions.sso",
-        "cdk_extensions.stacks"
+        "cdk_extensions.stacks",
+        "cdk_extensions.stepfunctions"
     ],
     "package_data": {
         "cdk_extensions._jsii": [
-            "cdk-extensions@0.0.77.jsii.tgz"
+            "cdk-extensions@0.0.78.jsii.tgz"
         ],
         "cdk_extensions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 import typing_extensions
 
 from typeguard import check_type
 
 from ._jsii import *
 
 __all__ = [
+    "alerting",
     "aps",
     "asserts",
     "athena",
     "core",
     "ec2",
     "ec2_patterns",
     "eks_patterns",
@@ -124,19 +125,21 @@
     "ram_resources",
     "rds",
     "resourcegroups",
     "route53",
     "s3_buckets",
     "sso",
     "stacks",
+    "stepfunctions",
 ]
 
 publication.publish()
 
 # Loading modules to ensure their types are registered with the jsii runtime library
+from . import alerting
 from . import aps
 from . import asserts
 from . import athena
 from . import core
 from . import ec2
 from . import ec2_patterns
 from . import eks_patterns
@@ -151,7 +154,8 @@
 from . import ram_resources
 from . import rds
 from . import resourcegroups
 from . import route53
 from . import s3_buckets
 from . import sso
 from . import stacks
+from . import stepfunctions
```

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/aps/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/aps/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/asserts/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/asserts/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/athena/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/core/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/ec2/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/ec2_patterns/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/ec2_patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/eks_patterns/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/eks_patterns/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/glue/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/glue/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/glue_tables/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/glue_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/k8s_aws/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/k8s_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/k8s_fargate/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/k8s_fargate/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/kinesis_firehose/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/kinesis_firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/lambda_/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/networkmanager/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/networkmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/ram/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/ram/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/ram_resources/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/ram_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/rds/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/rds/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/resourcegroups/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/resourcegroups/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/route53/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/s3_buckets/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/s3_buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/sso/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/sso/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions/stacks/__init__.py` & `cdk-extensions-0.0.78/src/cdk_extensions/stacks/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions.egg-info/PKG-INFO` & `cdk-extensions-0.0.78/src/cdk_extensions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-extensions
-Version: 0.0.77
+Version: 0.0.78
 Summary: cdk-extensions
 Home-page: https://github.com/vibe-io/cdk-extensions.git
 Author: Kevin Lucas<kevinluc08@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/vibe-io/cdk-extensions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-extensions-0.0.77/src/cdk_extensions.egg-info/SOURCES.txt` & `cdk-extensions-0.0.78/src/cdk_extensions.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 src/cdk_extensions/py.typed
 src/cdk_extensions.egg-info/PKG-INFO
 src/cdk_extensions.egg-info/SOURCES.txt
 src/cdk_extensions.egg-info/dependency_links.txt
 src/cdk_extensions.egg-info/requires.txt
 src/cdk_extensions.egg-info/top_level.txt
 src/cdk_extensions/_jsii/__init__.py
-src/cdk_extensions/_jsii/cdk-extensions@0.0.77.jsii.tgz
+src/cdk_extensions/_jsii/cdk-extensions@0.0.78.jsii.tgz
 src/cdk_extensions/_jsii/bin/init-aws.sh
+src/cdk_extensions/alerting/__init__.py
 src/cdk_extensions/aps/__init__.py
 src/cdk_extensions/asserts/__init__.py
 src/cdk_extensions/athena/__init__.py
 src/cdk_extensions/core/__init__.py
 src/cdk_extensions/ec2/__init__.py
 src/cdk_extensions/ec2_patterns/__init__.py
 src/cdk_extensions/eks_patterns/__init__.py
@@ -30,8 +31,9 @@
 src/cdk_extensions/ram/__init__.py
 src/cdk_extensions/ram_resources/__init__.py
 src/cdk_extensions/rds/__init__.py
 src/cdk_extensions/resourcegroups/__init__.py
 src/cdk_extensions/route53/__init__.py
 src/cdk_extensions/s3_buckets/__init__.py
 src/cdk_extensions/sso/__init__.py
-src/cdk_extensions/stacks/__init__.py
+src/cdk_extensions/stacks/__init__.py
+src/cdk_extensions/stepfunctions/__init__.py
```

