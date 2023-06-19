# Comparing `tmp/odoo_filter_addons-1.2.0rc1.tar.gz` & `tmp/odoo_filter_addons-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo_filter_addons-1.2.0rc1.tar", last modified: Fri Jun  9 08:43:08 2023, max compression
+gzip compressed data, was "odoo_filter_addons-1.2.1.tar", last modified: Mon Jun 19 07:55:50 2023, max compression
```

## Comparing `odoo_filter_addons-1.2.0rc1.tar` & `odoo_filter_addons-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:43:08.847087 odoo_filter_addons-1.2.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-09 08:43:08.847087 odoo_filter_addons-1.2.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-09 08:42:56.000000 odoo_filter_addons-1.2.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:43:08.847087 odoo_filter_addons-1.2.0rc1/odoo_filter_addons/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-09 08:42:56.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-06-09 08:42:56.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-09 08:42:56.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:43:08.847087 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-09 08:43:08.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-09 08:43:08.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 08:43:08.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-09 08:43:08.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-09 08:43:08.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 08:43:08.000000 odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-09 08:42:56.000000 odoo_filter_addons-1.2.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 08:43:08.847087 odoo_filter_addons-1.2.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 08:42:56.000000 odoo_filter_addons-1.2.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:55:50.505172 odoo_filter_addons-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-19 07:55:50.505172 odoo_filter_addons-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-19 07:55:40.000000 odoo_filter_addons-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:55:50.505172 odoo_filter_addons-1.2.1/odoo_filter_addons/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-19 07:55:40.000000 odoo_filter_addons-1.2.1/odoo_filter_addons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-06-19 07:55:40.000000 odoo_filter_addons-1.2.1/odoo_filter_addons/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-19 07:55:40.000000 odoo_filter_addons-1.2.1/odoo_filter_addons/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 07:55:50.505172 odoo_filter_addons-1.2.1/odoo_filter_addons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-19 07:55:50.000000 odoo_filter_addons-1.2.1/odoo_filter_addons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-19 07:55:50.000000 odoo_filter_addons-1.2.1/odoo_filter_addons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 07:55:50.000000 odoo_filter_addons-1.2.1/odoo_filter_addons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-19 07:55:50.000000 odoo_filter_addons-1.2.1/odoo_filter_addons.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-19 07:55:50.000000 odoo_filter_addons-1.2.1/odoo_filter_addons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-19 07:55:50.000000 odoo_filter_addons-1.2.1/odoo_filter_addons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-19 07:55:40.000000 odoo_filter_addons-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 07:55:50.505172 odoo_filter_addons-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-19 07:55:40.000000 odoo_filter_addons-1.2.1/setup.py
```

### Comparing `odoo_filter_addons-1.2.0rc1/PKG-INFO` & `odoo_filter_addons-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo_filter_addons
-Version: 1.2.0rc1
+Version: 1.2.1
 Summary: Simple utlity to filter odoo addons into a single directory
 Author-email: Pablo Esteban <pablo.esteban@forgeflow.com>
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Operating System :: POSIX
 Classifier: Framework :: Odoo
 Classifier: Programming Language :: Python :: 3
```

### Comparing `odoo_filter_addons-1.2.0rc1/README.md` & `odoo_filter_addons-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `odoo_filter_addons-1.2.0rc1/odoo_filter_addons/main.py` & `odoo_filter_addons-1.2.1/odoo_filter_addons/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,34 +27,55 @@
 
 def print_header(msg, sym):
     print("{}\n{}".format(sym*len(msg), msg))
 
 def load_yml(path, expand=False):
     if path.with_suffix(".yml").is_file():
         path = path.with_suffix(".yml")
-        suffix = ".yml"
     elif path.with_suffix(".yaml").is_file():
         path = path.with_suffix(".yaml")
-        suffix = ".yaml"
     else:
         raise UserException("YAML file {}.y[a]ml not found".format(path))
 
     with open(path, "r") as f:
         if expand and path.with_suffix(".env").is_file():
             env = dotenv_values(path.with_suffix(".env"))
             templated = Template(f.read()).substitute(env)
             yml = yaml.safe_load(StringIO(templated).read())
         else:
             yml = yaml.safe_load(f.read())
-    return yml, suffix
+    return yml
 
 def dump_yml(path, yml):
     with open(path, "w") as f:
         f.write(yaml.safe_dump(yml))
 
+# Remove targets from repositories, as they cause issues with gitaggregator>=3.0.0
+# https://github.com/acsone/git-aggregator/pull/55
+def remove_targets(repos):
+    for repo in repos.values():
+        if repo.get("target"):
+            del repo["target"]
+    return repos
+
+# Update remote URLs to use GitLab access token
+def update_remotes(repos):
+    try:
+        token = os.environ["CI_JOB_TOKEN"]
+        host = os.environ["CI_SERVER_HOST"]
+    except KeyError as e:
+        raise UserException("Unset environment variable {}".format(e))
+    gitlab_url = "https://gitlab-ci-token:{}@{}/{{}}".format(token, host)
+    for repo in repos.values():
+        for name, url in repo["remotes"].items():
+            if "git@gitlab.com:" in url:
+                project = url.split(":")[1]
+                repo["remotes"][name] = gitlab_url.format(project)
+    return repos
+
 #####################################################################
 
 def is_module(path):
     path = Path(path)
     return path.is_dir() and (path/"__manifest__.py").is_file()
 
 def filter_repo(tmp_path, rname, repo, modules):
@@ -97,15 +118,16 @@
         if not repo:
             raise UserException("addons.yml entry {} not found in repos.yml".format(rname))
         repo_message = filter_repo(tmp_path, rname, repo, modules)
         messages.append(repo_message)
     print_header("Finished filtering", '*')
     # Commit changes, if any, and push them to remote if specified
     if not release:
-        print("No changes, nothing commited")
+        git("restore", "--staged", ".")
+        print("Release disabled, nothing commited")
     elif filter(None, messages) and git["diff", "--staged", "--quiet"] & TF(1):
         messages = [f"[AUTO] {__package__} {__version__}"] + messages
         message = "\n".join(messages)
         git("commit", "-m", message)
         print("Changes commited")
         if push:
             if git["rev-parse", "@{u}"] & TF:
@@ -117,72 +139,57 @@
                 git("push", "origin", "HEAD:{}".format(branch))
             else:
                 raise UserException("addons.yml entry {} not found in repos.yml".format(rname))
             print("Commit pushed to remote")
     else:
         print("No changes, nothing commited")
 
-# Update remote URLs to use GitLab access token
-def update_ci_urls(repos):
-    try:
-        token = os.environ["CI_JOB_TOKEN"]
-        host = os.environ["CI_SERVER_HOST"]
-    except KeyError as e:
-        raise UserException("Unset environment variable {}".format(e))
-    gitlab_url = "https://gitlab-ci-token:{}@{}/{{}}".format(token, host)
-    for repo in repos.values():
-        for name, url in repo["remotes"].items():
-            if "git@gitlab.com:" in url:
-                project = url.split(":")[1]
-                repo["remotes"][name] = gitlab_url.format(project)
-    return repos
-
 @contextmanager
 def set_argv(new_argv):
     old_argv = sys.argv
     sys.argv = new_argv
     try:
         yield
     finally:
         sys.argv = old_argv
 
 # Create a git repo if not present and aggregate addon repositories
-def initialize_repos(output_path, input_path, tmp_path, repos_suffix):
-    os.chdir(tmp_path)
+def initialize_repos(output_path, tmp_path, repos):
     if not output_path.is_dir():
         print("Initializing git repository in '{}'".format(output_path))
         Path(output_path).mkdir(parents=True, exist_ok=True)
     git("-C", output_path, "init")
 
-    repos_path = (input_path/"repos").with_suffix(repos_suffix)
-    new_argv = ["gitaggregate", "-c", str(repos_path)]
-    if (input_path/"repos.env").is_file():
-        new_argv += ["-e", "--env-file", str(input_path/"repos.env")]
+    os.chdir(tmp_path)
+    dump_yml("repos.yml", repos)
+
+    new_argv = ["gitaggregate", "-c", "repos.yml"]
     with set_argv(new_argv):
         gitaggregate()
-    print("Writing gitaggregate output to '{}'".format(tmp_path))
+    print("gitaggregate output written to '{}'".format(tmp_path))
 
 #####################################################################
 
 # API entry point
-def main(input_path=None, output_path=None, clean=True, release=False, push=False, gitlab_ci=False):
+def api_main(input_path=None, output_path=None, clean=True, release=False, push=False, gitlab_ci=False):
     input_path = Path(input_path).resolve() if input_path else Path.cwd()
     output_path = Path(output_path).resolve() if output_path else Path.cwd()
     tmp_path = Path(mkdtemp())
 
     print("Loading configuration files from '{}'".format(input_path))
-    repos, repos_suffix = load_yml(input_path/"repos", True)
-    addons, addons_suffix = load_yml(input_path/"addons")
+    repos = load_yml(input_path/"repos", True)
+    addons = load_yml(input_path/"addons")
+
+    repos = remove_targets(repos)
     if gitlab_ci:
-        repos = update_ci_urls(repos)
-        dump_yml("repos.yml", update_ci_urls(repos))
+        repos = update_remotes(repos)
 
     try:
         print("Filtering addons to '{}'".format(output_path))
-        initialize_repos(output_path, input_path, tmp_path, repos_suffix)
+        initialize_repos(output_path, tmp_path, repos)
         filter_repos(output_path, tmp_path, repos, addons, release, push, gitlab_ci)
     except Exception as e:
         if clean:
             rmtree(tmp_path)
         raise e
     if clean:
         print("Cleaning up intermediate output")
@@ -197,15 +204,15 @@
 @click.option("-r", "--release/--no-release", is_flag=True, default=False, help="Create a relase commit if any changes are made.")
 @click.option("-p", "--push/--no-push", is_flag=True, default=False, help="Push to remote repo if any changes are commited.")
 @click.option("-g", "--gitlab-ci", is_flag=True, default=False, help="Update client addon repository in GitLab CI.")
 def cli_main(input_path, output_path, clean, release, push, gitlab_ci):
     import sys
     import traceback
     try:
-        main(input_path, output_path, clean, release, push, gitlab_ci)
+        api_main(input_path, output_path, clean, release, push, gitlab_ci)
         sys.exit(0)
     except UserException as e:
         print("User error:", e)
     except yaml.YAMLError as e:
         print("Invalid YAML content:", e)
     except ProcessExecutionError as e:
         print("Process execution error:", e)
```

### Comparing `odoo_filter_addons-1.2.0rc1/odoo_filter_addons.egg-info/PKG-INFO` & `odoo_filter_addons-1.2.1/odoo_filter_addons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-filter-addons
-Version: 1.2.0rc1
+Version: 1.2.1
 Summary: Simple utlity to filter odoo addons into a single directory
 Author-email: Pablo Esteban <pablo.esteban@forgeflow.com>
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Operating System :: POSIX
 Classifier: Framework :: Odoo
 Classifier: Programming Language :: Python :: 3
```

### Comparing `odoo_filter_addons-1.2.0rc1/pyproject.toml` & `odoo_filter_addons-1.2.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 classifiers = [
     "Intended Audience :: Developers",
     "Topic :: Utilities",
     "Operating System :: POSIX",
     "Framework :: Odoo",
     "Programming Language :: Python :: 3"
 ]
+
 requires-python = ">=3"
-# Pin git-aggregator to 2.1.0 to prevent weird bug when using 'target' in repos.yml
-# TODO: pin other packages as well to prevent future issues
-dependencies= ["pyyaml", "click", "python-dotenv", "plumbum", "git-aggregator==2.1.0"]
+# Ensure git-aggregator>=3.0.0 to prevent branch divergence issues with recent git versions
+# https://github.com/acsone/git-aggregator/pull/64
+dependencies= ["pyyaml", "click", "python-dotenv", "plumbum", "git-aggregator>=3.0.0"]
 dynamic = ["version"]
 
 [project.scripts]
 odoo_filter_addons = "odoo_filter_addons.main:cli_main"
 
 [build-system]
 requires = ["setuptools"]
```

