# Comparing `tmp/pulumi_auto_deploy-0.0.3.tar.gz` & `tmp/pulumi_auto_deploy-0.0.3a1687127619.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_auto_deploy-0.0.3.tar", last modified: Sun Jun 18 22:47:04 2023, max compression
+gzip compressed data, was "dist/pulumi_auto_deploy-0.0.3a1687127619.tar", last modified: Sun Jun 18 22:35:46 2023, max compression
```

## Comparing `pulumi_auto_deploy-0.0.3.tar` & `pulumi_auto_deploy-0.0.3a1687127619.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:47:04.427745 pulumi_auto_deploy-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-18 22:47:04.427745 pulumi_auto_deploy-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-18 22:47:04.000000 pulumi_auto_deploy-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:47:04.427745 pulumi_auto_deploy-0.0.3/pulumi_auto_deploy/
--rw-------   0 runner    (1001) docker     (123)      654 2023-06-18 22:47:04.000000 pulumi_auto_deploy-0.0.3/pulumi_auto_deploy/__init__.py
--rw-------   0 runner    (1001) docker     (123)     8047 2023-06-18 22:47:04.000000 pulumi_auto_deploy-0.0.3/pulumi_auto_deploy/_utilities.py
--rw-------   0 runner    (1001) docker     (123)     8953 2023-06-18 22:47:04.000000 pulumi_auto_deploy-0.0.3/pulumi_auto_deploy/auto_deployer.py
--rw-------   0 runner    (1001) docker     (123)     2731 2023-06-18 22:47:04.000000 pulumi_auto_deploy-0.0.3/pulumi_auto_deploy/provider.py
--rw-------   0 runner    (1001) docker     (123)       48 2023-06-18 22:47:04.000000 pulumi_auto_deploy-0.0.3/pulumi_auto_deploy/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)        0 2023-06-18 22:47:04.000000 pulumi_auto_deploy-0.0.3/pulumi_auto_deploy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:47:04.427745 pulumi_auto_deploy-0.0.3/pulumi_auto_deploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-18 22:47:04.000000 pulumi_auto_deploy-0.0.3/pulumi_auto_deploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-18 22:47:04.000000 pulumi_auto_deploy-0.0.3/pulumi_auto_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 22:47:04.000000 pulumi_auto_deploy-0.0.3/pulumi_auto_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 22:47:04.000000 pulumi_auto_deploy-0.0.3/pulumi_auto_deploy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-18 22:47:04.000000 pulumi_auto_deploy-0.0.3/pulumi_auto_deploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 22:47:04.000000 pulumi_auto_deploy-0.0.3/pulumi_auto_deploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 22:47:04.427745 pulumi_auto_deploy-0.0.3/setup.cfg
--rw-------   0 runner    (1001) docker     (123)     1825 2023-06-18 22:47:04.000000 pulumi_auto_deploy-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:35:46.000000 pulumi_auto_deploy-0.0.3a1687127619/
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-18 22:35:46.000000 pulumi_auto_deploy-0.0.3a1687127619/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-18 22:35:46.000000 pulumi_auto_deploy-0.0.3a1687127619/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:35:46.000000 pulumi_auto_deploy-0.0.3a1687127619/pulumi_auto_deploy/
+-rw-------   0 runner    (1001) docker     (123)      654 2023-06-18 22:35:46.000000 pulumi_auto_deploy-0.0.3a1687127619/pulumi_auto_deploy/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     8047 2023-06-18 22:35:46.000000 pulumi_auto_deploy-0.0.3a1687127619/pulumi_auto_deploy/_utilities.py
+-rw-------   0 runner    (1001) docker     (123)     8953 2023-06-18 22:35:46.000000 pulumi_auto_deploy-0.0.3a1687127619/pulumi_auto_deploy/auto_deployer.py
+-rw-------   0 runner    (1001) docker     (123)     2731 2023-06-18 22:35:46.000000 pulumi_auto_deploy-0.0.3a1687127619/pulumi_auto_deploy/provider.py
+-rw-------   0 runner    (1001) docker     (123)       48 2023-06-18 22:35:46.000000 pulumi_auto_deploy-0.0.3a1687127619/pulumi_auto_deploy/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (123)        0 2023-06-18 22:35:46.000000 pulumi_auto_deploy-0.0.3a1687127619/pulumi_auto_deploy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 22:35:46.000000 pulumi_auto_deploy-0.0.3a1687127619/pulumi_auto_deploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-18 22:35:46.000000 pulumi_auto_deploy-0.0.3a1687127619/pulumi_auto_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-18 22:35:46.000000 pulumi_auto_deploy-0.0.3a1687127619/pulumi_auto_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 22:35:46.000000 pulumi_auto_deploy-0.0.3a1687127619/pulumi_auto_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 22:35:46.000000 pulumi_auto_deploy-0.0.3a1687127619/pulumi_auto_deploy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-18 22:35:46.000000 pulumi_auto_deploy-0.0.3a1687127619/pulumi_auto_deploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 22:35:46.000000 pulumi_auto_deploy-0.0.3a1687127619/pulumi_auto_deploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 22:35:46.000000 pulumi_auto_deploy-0.0.3a1687127619/setup.cfg
+-rw-------   0 runner    (1001) docker     (123)     1862 2023-06-18 22:35:46.000000 pulumi_auto_deploy-0.0.3a1687127619/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pulumi_auto_deploy-0.0.3/PKG-INFO` & `pulumi_auto_deploy-0.0.3a1687127619/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: pulumi_auto_deploy
-Version: 0.0.3
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # Pulumi Auto Deploy
 
 [![Slack](https://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Fauto-deploy.svg)](https://www.npmjs.com/package/@pulumi/auto-deploy)
 [![Python version](https://badge.fury.io/py/pulumi-auto-deploy.svg)](https://pypi.org/project/pulumi-auto-deploy)
 [![NuGet version](https://badge.fury.io/nu/pulumi.auto-deploy.svg)](https://badge.fury.io/nu/pulumi.auto-deploy)
 [![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-auto-deploy/sdk/go/auto-deploy)](https://pkg.go.dev/github.com/pulumi/pulumi-auto-deploy/sdk/go)
@@ -111,9 +101,8 @@
 
     $ go get github.com/pulumi/pulumi-auto-deploy/sdk/go
 
 ### .NET
 
 To use from .NET, install using `dotnet add package`:
 
-    $ dotnet add package Pulumi.AutoDeploy
-
+    $ dotnet add package Pulumi.AutoDeploy
```

### Comparing `pulumi_auto_deploy-0.0.3/README.md` & `pulumi_auto_deploy-0.0.3a1687127619/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,108 +1,117 @@
-# Pulumi Auto Deploy
-
-[![Slack](https://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
-[![NPM version](https://badge.fury.io/js/%40pulumi%2Fauto-deploy.svg)](https://www.npmjs.com/package/@pulumi/auto-deploy)
-[![Python version](https://badge.fury.io/py/pulumi-auto-deploy.svg)](https://pypi.org/project/pulumi-auto-deploy)
-[![NuGet version](https://badge.fury.io/nu/pulumi.auto-deploy.svg)](https://badge.fury.io/nu/pulumi.auto-deploy)
-[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-auto-deploy/sdk/go/auto-deploy)](https://pkg.go.dev/github.com/pulumi/pulumi-auto-deploy/sdk/go)
-[![License](https://img.shields.io/npm/l/%40pulumi%2Fauto-deploy.svg)](https://github.com/pulumi/pulumi-auto-deploy/blob/main/LICENSE)
-
-A Pulumi Component for configuring automated updates of dependent stacks using [Pulumi Deployments](https://www.pulumi.com/docs/pulumi-cloud/deployments/). It lets you simply express dependencies between stacks, and takes care of creating and updating the necessary Deployment Webhooks under the hood. Each stack that you configure must have [Deployment Settings](https://www.pulumi.com/docs/pulumi-cloud/deployments/reference/#deployment-settings).
-
-```ts
-import * as autodeploy from "@pulumi/auto-deploy";
-import * as pulumi from "@pulumi/pulumi";
-
-/**
- *
- * The following example configures automatic deployment of stacks with the following dependency graph:
-    a
-    ├── b
-    │   ├── d
-    │   ├── e
-    │   └── f
-    └── c
- * Whenever a node in the graph is updated, 
- * all downstream nodes will be automatically updated via a webhook triggering Pulumi Deployments.
- */
-
-
-const organization = pulumi.getOrganization();
-const project = "dependency-example"
-
-export const f = new autodeploy.AutoDeployer("auto-deployer-f", {
-    organization,
-    project,
-    stack: "f",
-    downstreamRefs: [],
-});
-
-export const e = new autodeploy.AutoDeployer("auto-deployer-e", {
-    organization,
-    project,
-    stack: "e",
-    downstreamRefs: [],
-});
-
-export const d = new autodeploy.AutoDeployer("auto-deployer-d", {
-    organization,
-    project,
-    stack: "d",
-    downstreamRefs: [],
-});
-
-export const c = new autodeploy.AutoDeployer("auto-deployer-c", {
-    organization,
-    project,
-    stack: "c",
-    downstreamRefs: [],
-});
-
-export const b = new autodeploy.AutoDeployer("auto-deployer-b", {
-    organization,
-    project,
-    stack: "b",
-    downstreamRefs: [d.ref, e.ref, f.ref],
-
-});
-
-export const a = new autodeploy.AutoDeployer("auto-deployer-a", {
-    organization,
-    project,
-    stack: "a",
-    downstreamRefs: [b.ref, c.ref],
-});
-
-```
-
-## Installing
-
-This package is available in many languages in the standard packaging formats.
-
-### Node.js (Java/TypeScript)
-
-To use from JavaScript or TypeScript in Node.js, install using either `npm`:
-
-    $ npm install @pulumi/auto-deploy
-
-or `yarn`:
-
-    $ yarn add @pulumi/auto-deploy
-
-### Python
-
-To use from Python, install using `pip`:
-
-    $ pip install pulumi-auto-deploy
-
-### Go
-
-To use from Go, use `go get` to grab the latest version of the library
-
-    $ go get github.com/pulumi/pulumi-auto-deploy/sdk/go
-
-### .NET
-
-To use from .NET, install using `dotnet add package`:
-
-    $ dotnet add package Pulumi.AutoDeploy
+Metadata-Version: 2.1
+Name: pulumi_auto_deploy
+Version: 0.0.3a1687127619
+Summary: UNKNOWN
+Home-page: UNKNOWN
+License: UNKNOWN
+Description: # Pulumi Auto Deploy
+        
+        [![Slack](https://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
+        [![NPM version](https://badge.fury.io/js/%40pulumi%2Fauto-deploy.svg)](https://www.npmjs.com/package/@pulumi/auto-deploy)
+        [![Python version](https://badge.fury.io/py/pulumi-auto-deploy.svg)](https://pypi.org/project/pulumi-auto-deploy)
+        [![NuGet version](https://badge.fury.io/nu/pulumi.auto-deploy.svg)](https://badge.fury.io/nu/pulumi.auto-deploy)
+        [![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-auto-deploy/sdk/go/auto-deploy)](https://pkg.go.dev/github.com/pulumi/pulumi-auto-deploy/sdk/go)
+        [![License](https://img.shields.io/npm/l/%40pulumi%2Fauto-deploy.svg)](https://github.com/pulumi/pulumi-auto-deploy/blob/main/LICENSE)
+        
+        A Pulumi Component for configuring automated updates of dependent stacks using [Pulumi Deployments](https://www.pulumi.com/docs/pulumi-cloud/deployments/). It lets you simply express dependencies between stacks, and takes care of creating and updating the necessary Deployment Webhooks under the hood. Each stack that you configure must have [Deployment Settings](https://www.pulumi.com/docs/pulumi-cloud/deployments/reference/#deployment-settings).
+        
+        ```ts
+        import * as autodeploy from "@pulumi/auto-deploy";
+        import * as pulumi from "@pulumi/pulumi";
+        
+        /**
+         *
+         * The following example configures automatic deployment of stacks with the following dependency graph:
+            a
+            ├── b
+            │   ├── d
+            │   ├── e
+            │   └── f
+            └── c
+         * Whenever a node in the graph is updated, 
+         * all downstream nodes will be automatically updated via a webhook triggering Pulumi Deployments.
+         */
+        
+        
+        const organization = pulumi.getOrganization();
+        const project = "dependency-example"
+        
+        export const f = new autodeploy.AutoDeployer("auto-deployer-f", {
+            organization,
+            project,
+            stack: "f",
+            downstreamRefs: [],
+        });
+        
+        export const e = new autodeploy.AutoDeployer("auto-deployer-e", {
+            organization,
+            project,
+            stack: "e",
+            downstreamRefs: [],
+        });
+        
+        export const d = new autodeploy.AutoDeployer("auto-deployer-d", {
+            organization,
+            project,
+            stack: "d",
+            downstreamRefs: [],
+        });
+        
+        export const c = new autodeploy.AutoDeployer("auto-deployer-c", {
+            organization,
+            project,
+            stack: "c",
+            downstreamRefs: [],
+        });
+        
+        export const b = new autodeploy.AutoDeployer("auto-deployer-b", {
+            organization,
+            project,
+            stack: "b",
+            downstreamRefs: [d.ref, e.ref, f.ref],
+        
+        });
+        
+        export const a = new autodeploy.AutoDeployer("auto-deployer-a", {
+            organization,
+            project,
+            stack: "a",
+            downstreamRefs: [b.ref, c.ref],
+        });
+        
+        ```
+        
+        ## Installing
+        
+        This package is available in many languages in the standard packaging formats.
+        
+        ### Node.js (Java/TypeScript)
+        
+        To use from JavaScript or TypeScript in Node.js, install using either `npm`:
+        
+            $ npm install @pulumi/auto-deploy
+        
+        or `yarn`:
+        
+            $ yarn add @pulumi/auto-deploy
+        
+        ### Python
+        
+        To use from Python, install using `pip`:
+        
+            $ pip install pulumi-auto-deploy
+        
+        ### Go
+        
+        To use from Go, use `go get` to grab the latest version of the library
+        
+            $ go get github.com/pulumi/pulumi-auto-deploy/sdk/go
+        
+        ### .NET
+        
+        To use from .NET, install using `dotnet add package`:
+        
+            $ dotnet add package Pulumi.AutoDeploy
+Platform: UNKNOWN
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
```

### Comparing `pulumi_auto_deploy-0.0.3/pulumi_auto_deploy/__init__.py` & `pulumi_auto_deploy-0.0.3a1687127619/pulumi_auto_deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_auto_deploy-0.0.3/pulumi_auto_deploy/_utilities.py` & `pulumi_auto_deploy-0.0.3a1687127619/pulumi_auto_deploy/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_auto_deploy-0.0.3/pulumi_auto_deploy/auto_deployer.py` & `pulumi_auto_deploy-0.0.3a1687127619/pulumi_auto_deploy/auto_deployer.py`

 * *Files identical despite different names*

### Comparing `pulumi_auto_deploy-0.0.3/pulumi_auto_deploy/provider.py` & `pulumi_auto_deploy-0.0.3a1687127619/pulumi_auto_deploy/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_auto_deploy-0.0.3/pulumi_auto_deploy.egg-info/PKG-INFO` & `pulumi_auto_deploy-0.0.3a1687127619/pulumi_auto_deploy.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,119 +1,117 @@
 Metadata-Version: 2.1
 Name: pulumi-auto-deploy
-Version: 0.0.3
+Version: 0.0.3a1687127619
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
+Description: # Pulumi Auto Deploy
+        
+        [![Slack](https://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
+        [![NPM version](https://badge.fury.io/js/%40pulumi%2Fauto-deploy.svg)](https://www.npmjs.com/package/@pulumi/auto-deploy)
+        [![Python version](https://badge.fury.io/py/pulumi-auto-deploy.svg)](https://pypi.org/project/pulumi-auto-deploy)
+        [![NuGet version](https://badge.fury.io/nu/pulumi.auto-deploy.svg)](https://badge.fury.io/nu/pulumi.auto-deploy)
+        [![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-auto-deploy/sdk/go/auto-deploy)](https://pkg.go.dev/github.com/pulumi/pulumi-auto-deploy/sdk/go)
+        [![License](https://img.shields.io/npm/l/%40pulumi%2Fauto-deploy.svg)](https://github.com/pulumi/pulumi-auto-deploy/blob/main/LICENSE)
+        
+        A Pulumi Component for configuring automated updates of dependent stacks using [Pulumi Deployments](https://www.pulumi.com/docs/pulumi-cloud/deployments/). It lets you simply express dependencies between stacks, and takes care of creating and updating the necessary Deployment Webhooks under the hood. Each stack that you configure must have [Deployment Settings](https://www.pulumi.com/docs/pulumi-cloud/deployments/reference/#deployment-settings).
+        
+        ```ts
+        import * as autodeploy from "@pulumi/auto-deploy";
+        import * as pulumi from "@pulumi/pulumi";
+        
+        /**
+         *
+         * The following example configures automatic deployment of stacks with the following dependency graph:
+            a
+            ├── b
+            │   ├── d
+            │   ├── e
+            │   └── f
+            └── c
+         * Whenever a node in the graph is updated, 
+         * all downstream nodes will be automatically updated via a webhook triggering Pulumi Deployments.
+         */
+        
+        
+        const organization = pulumi.getOrganization();
+        const project = "dependency-example"
+        
+        export const f = new autodeploy.AutoDeployer("auto-deployer-f", {
+            organization,
+            project,
+            stack: "f",
+            downstreamRefs: [],
+        });
+        
+        export const e = new autodeploy.AutoDeployer("auto-deployer-e", {
+            organization,
+            project,
+            stack: "e",
+            downstreamRefs: [],
+        });
+        
+        export const d = new autodeploy.AutoDeployer("auto-deployer-d", {
+            organization,
+            project,
+            stack: "d",
+            downstreamRefs: [],
+        });
+        
+        export const c = new autodeploy.AutoDeployer("auto-deployer-c", {
+            organization,
+            project,
+            stack: "c",
+            downstreamRefs: [],
+        });
+        
+        export const b = new autodeploy.AutoDeployer("auto-deployer-b", {
+            organization,
+            project,
+            stack: "b",
+            downstreamRefs: [d.ref, e.ref, f.ref],
+        
+        });
+        
+        export const a = new autodeploy.AutoDeployer("auto-deployer-a", {
+            organization,
+            project,
+            stack: "a",
+            downstreamRefs: [b.ref, c.ref],
+        });
+        
+        ```
+        
+        ## Installing
+        
+        This package is available in many languages in the standard packaging formats.
+        
+        ### Node.js (Java/TypeScript)
+        
+        To use from JavaScript or TypeScript in Node.js, install using either `npm`:
+        
+            $ npm install @pulumi/auto-deploy
+        
+        or `yarn`:
+        
+            $ yarn add @pulumi/auto-deploy
+        
+        ### Python
+        
+        To use from Python, install using `pip`:
+        
+            $ pip install pulumi-auto-deploy
+        
+        ### Go
+        
+        To use from Go, use `go get` to grab the latest version of the library
+        
+            $ go get github.com/pulumi/pulumi-auto-deploy/sdk/go
+        
+        ### .NET
+        
+        To use from .NET, install using `dotnet add package`:
+        
+            $ dotnet add package Pulumi.AutoDeploy
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-
-# Pulumi Auto Deploy
-
-[![Slack](https://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
-[![NPM version](https://badge.fury.io/js/%40pulumi%2Fauto-deploy.svg)](https://www.npmjs.com/package/@pulumi/auto-deploy)
-[![Python version](https://badge.fury.io/py/pulumi-auto-deploy.svg)](https://pypi.org/project/pulumi-auto-deploy)
-[![NuGet version](https://badge.fury.io/nu/pulumi.auto-deploy.svg)](https://badge.fury.io/nu/pulumi.auto-deploy)
-[![PkgGoDev](https://pkg.go.dev/badge/github.com/pulumi/pulumi-auto-deploy/sdk/go/auto-deploy)](https://pkg.go.dev/github.com/pulumi/pulumi-auto-deploy/sdk/go)
-[![License](https://img.shields.io/npm/l/%40pulumi%2Fauto-deploy.svg)](https://github.com/pulumi/pulumi-auto-deploy/blob/main/LICENSE)
-
-A Pulumi Component for configuring automated updates of dependent stacks using [Pulumi Deployments](https://www.pulumi.com/docs/pulumi-cloud/deployments/). It lets you simply express dependencies between stacks, and takes care of creating and updating the necessary Deployment Webhooks under the hood. Each stack that you configure must have [Deployment Settings](https://www.pulumi.com/docs/pulumi-cloud/deployments/reference/#deployment-settings).
-
-```ts
-import * as autodeploy from "@pulumi/auto-deploy";
-import * as pulumi from "@pulumi/pulumi";
-
-/**
- *
- * The following example configures automatic deployment of stacks with the following dependency graph:
-    a
-    ├── b
-    │   ├── d
-    │   ├── e
-    │   └── f
-    └── c
- * Whenever a node in the graph is updated, 
- * all downstream nodes will be automatically updated via a webhook triggering Pulumi Deployments.
- */
-
-
-const organization = pulumi.getOrganization();
-const project = "dependency-example"
-
-export const f = new autodeploy.AutoDeployer("auto-deployer-f", {
-    organization,
-    project,
-    stack: "f",
-    downstreamRefs: [],
-});
-
-export const e = new autodeploy.AutoDeployer("auto-deployer-e", {
-    organization,
-    project,
-    stack: "e",
-    downstreamRefs: [],
-});
-
-export const d = new autodeploy.AutoDeployer("auto-deployer-d", {
-    organization,
-    project,
-    stack: "d",
-    downstreamRefs: [],
-});
-
-export const c = new autodeploy.AutoDeployer("auto-deployer-c", {
-    organization,
-    project,
-    stack: "c",
-    downstreamRefs: [],
-});
-
-export const b = new autodeploy.AutoDeployer("auto-deployer-b", {
-    organization,
-    project,
-    stack: "b",
-    downstreamRefs: [d.ref, e.ref, f.ref],
-
-});
-
-export const a = new autodeploy.AutoDeployer("auto-deployer-a", {
-    organization,
-    project,
-    stack: "a",
-    downstreamRefs: [b.ref, c.ref],
-});
-
-```
-
-## Installing
-
-This package is available in many languages in the standard packaging formats.
-
-### Node.js (Java/TypeScript)
-
-To use from JavaScript or TypeScript in Node.js, install using either `npm`:
-
-    $ npm install @pulumi/auto-deploy
-
-or `yarn`:
-
-    $ yarn add @pulumi/auto-deploy
-
-### Python
-
-To use from Python, install using `pip`:
-
-    $ pip install pulumi-auto-deploy
-
-### Go
-
-To use from Go, use `go get` to grab the latest version of the library
-
-    $ go get github.com/pulumi/pulumi-auto-deploy/sdk/go
-
-### .NET
-
-To use from .NET, install using `dotnet add package`:
-
-    $ dotnet add package Pulumi.AutoDeploy
-
```

### Comparing `pulumi_auto_deploy-0.0.3/setup.py` & `pulumi_auto_deploy-0.0.3a1687127619/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.3"
-PLUGIN_VERSION = "0.0.3"
+VERSION = "0.0.3a1687127619"
+PLUGIN_VERSION = "0.0.3-alpha.1687127619+ecdcfa6b"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'auto-deploy', PLUGIN_VERSION])
         except OSError as error:
```

