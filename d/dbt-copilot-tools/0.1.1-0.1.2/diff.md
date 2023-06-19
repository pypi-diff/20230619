# Comparing `tmp/dbt_copilot_tools-0.1.1.tar.gz` & `tmp/dbt_copilot_tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_copilot_tools-0.1.1.tar", max compression
+gzip compressed data, was "dbt_copilot_tools-0.1.2.tar", max compression
```

## Comparing `dbt_copilot_tools-0.1.1.tar` & `dbt_copilot_tools-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1090 2023-06-16 11:05:25.987520 dbt_copilot_tools-0.1.1/LICENSE
--rw-r--r--   0        0        0     1209 2023-06-16 14:14:21.704068 dbt_copilot_tools-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-06-02 08:46:48.576039 dbt_copilot_tools-0.1.1/commands/__init__.py
--rwxr-xr-x   0        0        0     9980 2023-06-14 12:11:53.497780 dbt_copilot_tools-0.1.1/commands/bootstrap_cli.py
--rwxr-xr-x   0        0        0    11242 2023-06-15 11:49:38.161070 dbt_copilot_tools-0.1.1/commands/codebuild_cli.py
--rwxr-xr-x   0        0        0     8582 2023-06-15 16:41:34.056908 dbt_copilot_tools-0.1.1/commands/copilot_cli.py
--rwxr-xr-x   0        0        0    20889 2023-06-15 11:49:38.162560 dbt_copilot_tools-0.1.1/commands/dns_cli.py
--rw-r--r--   0        0        0     5902 2023-06-16 11:05:25.989196 dbt_copilot_tools-0.1.1/commands/utils.py
--rwxr-xr-x   0        0        0      656 2023-06-16 11:24:09.621662 dbt_copilot_tools-0.1.1/copilot_helper.py
--rw-r--r--   0        0        0     1149 2023-06-16 14:38:28.156185 dbt_copilot_tools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2188 1970-01-01 00:00:00.000000 dbt_copilot_tools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-16 11:05:25.987520 dbt_copilot_tools-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1209 2023-06-16 14:14:21.704068 dbt_copilot_tools-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 08:46:48.576039 dbt_copilot_tools-0.1.2/commands/__init__.py
+-rwxr-xr-x   0        0        0     9980 2023-06-14 12:11:53.497780 dbt_copilot_tools-0.1.2/commands/bootstrap_cli.py
+-rwxr-xr-x   0        0        0    11242 2023-06-15 11:49:38.161070 dbt_copilot_tools-0.1.2/commands/codebuild_cli.py
+-rwxr-xr-x   0        0        0     8582 2023-06-15 16:41:34.056908 dbt_copilot_tools-0.1.2/commands/copilot_cli.py
+-rwxr-xr-x   0        0        0    20700 2023-06-19 10:28:42.526261 dbt_copilot_tools-0.1.2/commands/dns_cli.py
+-rw-r--r--   0        0        0     5902 2023-06-16 11:05:25.989196 dbt_copilot_tools-0.1.2/commands/utils.py
+-rwxr-xr-x   0        0        0      656 2023-06-16 11:24:09.621662 dbt_copilot_tools-0.1.2/copilot_helper.py
+-rw-r--r--   0        0        0     1139 2023-06-19 14:04:34.232750 dbt_copilot_tools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2188 1970-01-01 00:00:00.000000 dbt_copilot_tools-0.1.2/PKG-INFO
```

### Comparing `dbt_copilot_tools-0.1.1/LICENSE` & `dbt_copilot_tools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.1/README.md` & `dbt_copilot_tools-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.1/commands/bootstrap_cli.py` & `dbt_copilot_tools-0.1.2/commands/bootstrap_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.1/commands/codebuild_cli.py` & `dbt_copilot_tools-0.1.2/commands/codebuild_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.1/commands/copilot_cli.py` & `dbt_copilot_tools-0.1.2/commands/copilot_cli.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.1/commands/dns_cli.py` & `dbt_copilot_tools-0.1.2/commands/dns_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import time
 
 import click
 import yaml
 
 from .utils import check_aws_conn
 from .utils import check_response
+from .utils import ensure_cwd_is_repo_root
 
 # To do
 # -----
 # Check user has logged into the aws accounts before scanning the accounts
 # When adding records from parent to subdomain, if ok, it then should remove them from parent domain
 # (run a test before removing)
 
@@ -172,18 +173,18 @@
                     },
                 ],
             },
         )
 
     check_response(response)
     click.echo(
-        click.style(f"{records['Name']}, Type: {records['Type']}", fg="white", bold=True) + 
-        click.style("Added.", fg="magenta")
-        )
-    return response['ChangeInfo']['Status']
+        click.style(f"{records['Name']}, Type: {records['Type']}", fg="white", bold=True)
+        + click.style("Added.", fg="magenta"),
+    )
+    return response["ChangeInfo"]["Status"]
 
 
 def check_for_records(client, parent_id, subdom, subdom_id):
     records_to_add = []
     response = client.list_resource_record_sets(
         HostedZoneId=parent_id,
     )
@@ -279,15 +280,18 @@
         hosted_zones[hz["Name"]] = hz
 
     # Check if base domain is valid
     if base_domain[-1] != ".":
         base_domain = base_domain + "."
 
     if base_domain not in hosted_zones:
-        click.secho(f"The base domain: {base_domain} does not exist in your AWS domain account {response['HostedZones']}", fg='red')
+        click.secho(
+            f"The base domain: {base_domain} does not exist in your AWS domain account {response['HostedZones']}",
+            fg="red",
+        )
         exit()
 
     base_len = len(base_domain.split(".")) - 1
     parts = domain.split(".")
 
     for _ in range(len(parts) - 1):
         subdom = ".".join(parts) + "."
@@ -371,14 +375,16 @@
 @click.option("--svc", help="Service Name", required=True)
 @click.option("--env", help="Environment", required=True)
 def assign_domain(app, domain_profile, project_profile, svc, env):
     """Check R53 domain is pointing to the correct ECS Load Blanacer."""
     domain_session = check_aws_conn(domain_profile)
     project_session = check_aws_conn(project_profile)
 
+    ensure_cwd_is_repo_root()
+
     # Find the Load Balancer name.
     proj_client = project_session.client("ecs")
 
     response = proj_client.list_clusters()
     check_response(response)
     no_items = True
     for cluster_arn in response["clusterArns"]:
@@ -403,15 +409,14 @@
     no_items = True
     for service_arn in response["serviceArns"]:
         service_name = service_arn.split("/")[2]
         service_name_items = service_name.split("-")
         service_app = service_name_items[0]
         service_env = service_name_items[1]
         service_service = service_name_items[2]
-
         if service_app == app and service_env == env and service_service == svc:
             no_items = False
             break
 
     if no_items:
         click.echo(
             click.style("There are no services matching ", fg="red")
@@ -438,34 +443,28 @@
     )["TargetGroups"][0]["LoadBalancerArns"][0]
 
     response = elb_client.describe_load_balancers(LoadBalancerArns=[elb_arn])
     check_response(response)
     elb_name = response["LoadBalancers"][0]["DNSName"]
 
     # Find the domain name
-    response = elb_client.describe_listeners(LoadBalancerArn=[elb_arn][0])
-    check_response(response)
-    for listener in response["Listeners"]:
-        if listener["Protocol"] == "HTTPS":
-            acm_client = project_session.client("acm")
-            response = acm_client.describe_certificate(
-                CertificateArn=elb_client.describe_listener_certificates(ListenerArn=listener["ListenerArn"])[
-                    "Certificates"
-                ][0]["CertificateArn"],
-            )
-            check_response(response)
-            domain_name = response["Certificate"]["DomainName"]
+    with open(f"./copilot/{svc}/manifest.yml", "r") as fd:
+        conf = yaml.safe_load(fd)
+        if "environments" in conf:
+            for domain in conf["environments"].items():
+                if domain[0] == env:
+                    domain_name = domain[1]["http"]["alias"]
 
-    click.echo(
-        click.style("The Domain: ", fg="yellow")
-        + click.style(f"{domain_name}\n", fg="white", bold=True)
-        + click.style("has been assigned the Load Balancer: ", fg="yellow")
-        + click.style(f"{elb_name}\n", fg="white", bold=True)
-        + click.style("Checking to see if this is in R53", fg="yellow"),
-    )
+        click.echo(
+            click.style("The Domain: ", fg="yellow")
+            + click.style(f"{domain_name}\n", fg="white", bold=True)
+            + click.style("has been assigned the Load Balancer: ", fg="yellow")
+            + click.style(f"{elb_name}\n", fg="white", bold=True)
+            + click.style("Checking to see if this is in R53", fg="yellow"),
+        )
 
     domain_client = domain_session.client("route53")
     response = domain_client.list_hosted_zones_by_name()
     check_response(response)
 
     # Scan R53 Zone for matching domains and update records if needed.
     hosted_zones = {}
```

### Comparing `dbt_copilot_tools-0.1.1/commands/utils.py` & `dbt_copilot_tools-0.1.2/commands/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.1/copilot_helper.py` & `dbt_copilot_tools-0.1.2/copilot_helper.py`

 * *Files identical despite different names*

### Comparing `dbt_copilot_tools-0.1.1/pyproject.toml` & `dbt_copilot_tools-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.black]
 line-length = 119
 
 [tool.poetry]
 name = "dbt-copilot-tools"
-version = "0.1.1"
+version = "0.1.2"
 description = "Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot."
 authors = ["Department for Business and Trade Platform Team <sre-team@digital.trade.gov.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "commands" },
     { include = "copilot_helper.py" }
 ]
 
 [tool.poetry.scripts]
-dbt-copilot-tools-helper = "copilot_helper:cli"
+copilot-helper = "copilot_helper:cli"
 
 [tool.poetry.dependencies]
 Jinja2 = "3.1.2"
 PyYAML = "6.0"
 boto3 = "1.26.31"
 boto3-stubs = "1.26.148"
 botocore = "1.29.31"
```

### Comparing `dbt_copilot_tools-0.1.1/PKG-INFO` & `dbt_copilot_tools-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-copilot-tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: Set of tools to help transfer applications/services from GOV.UK PaaS to DBT PaaS augmenting AWS Copilot.
 License: MIT
 Author: Department for Business and Trade Platform Team
 Author-email: sre-team@digital.trade.gov.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

