# Comparing `tmp/slap_cli-1.9.4.tar.gz` & `tmp/slap_cli-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slap_cli-1.9.4.tar", max compression
+gzip compressed data, was "slap_cli-1.9.5.tar", max compression
```

## Comparing `slap_cli-1.9.4.tar` & `slap_cli-1.9.5.tar`

### file list

```diff
@@ -1,61 +1,62 @@
--rw-r--r--   0        0        0     1002 2023-01-29 11:43:11.729548 slap_cli-1.9.4/LICENSE
--rw-r--r--   0        0        0     4981 2023-05-19 08:33:39.581819 slap_cli-1.9.4/pyproject.toml
--rw-r--r--   0        0        0       98 2023-05-19 08:33:39.581819 slap_cli-1.9.4/src/slap/__init__.py
--rw-r--r--   0        0        0      122 2023-05-15 14:08:15.856560 slap_cli-1.9.4/src/slap/__main__.py
--rw-r--r--   0        0        0    12213 2023-05-15 15:51:24.022394 slap_cli-1.9.4/src/slap/application.py
--rw-r--r--   0        0        0     9163 2023-02-09 13:39:04.453992 slap_cli-1.9.4/src/slap/changelog.py
--rw-r--r--   0        0        0     3353 2023-01-29 11:43:11.729548 slap_cli-1.9.4/src/slap/check.py
--rw-r--r--   0        0        0     2533 2023-05-15 15:02:36.078985 slap_cli-1.9.4/src/slap/configuration.py
--rw-r--r--   0        0        0     5337 2023-05-15 13:54:26.739024 slap_cli-1.9.4/src/slap/ext/application/add.py
--rw-r--r--   0        0        0    27292 2023-05-15 16:43:58.997086 slap_cli-1.9.4/src/slap/ext/application/changelog.py
--rw-r--r--   0        0        0     6330 2023-05-15 14:28:58.852972 slap_cli-1.9.4/src/slap/ext/application/check.py
--rw-r--r--   0        0        0     3177 2023-05-15 14:02:47.957819 slap_cli-1.9.4/src/slap/ext/application/info.py
--rw-r--r--   0        0        0     4911 2023-05-19 08:24:24.059256 slap_cli-1.9.4/src/slap/ext/application/init.py
--rw-r--r--   0        0        0    14309 2023-05-15 14:29:33.968869 slap_cli-1.9.4/src/slap/ext/application/install.py
--rw-r--r--   0        0        0     5982 2023-05-15 14:16:35.467350 slap_cli-1.9.4/src/slap/ext/application/link.py
--rw-r--r--   0        0        0     4230 2023-05-15 14:29:48.828826 slap_cli-1.9.4/src/slap/ext/application/publish.py
--rw-r--r--   0        0        0    21667 2023-05-15 14:33:39.328295 slap_cli-1.9.4/src/slap/ext/application/release.py
--rw-r--r--   0        0        0     3243 2023-05-15 14:30:47.388698 slap_cli-1.9.4/src/slap/ext/application/report.py
--rw-r--r--   0        0        0     3555 2023-05-15 14:59:30.475460 slap_cli-1.9.4/src/slap/ext/application/run.py
--rw-r--r--   0        0        0     7789 2023-05-15 14:29:06.756949 slap_cli-1.9.4/src/slap/ext/application/test.py
--rw-r--r--   0        0        0    19880 2023-05-15 14:20:06.182817 slap_cli-1.9.4/src/slap/ext/application/venv.py
--rw-r--r--   0        0        0     2075 2023-01-29 11:43:11.729548 slap_cli-1.9.4/src/slap/ext/checks/changelog.py
--rw-r--r--   0        0        0     2215 2023-01-29 11:43:11.729548 slap_cli-1.9.4/src/slap/ext/checks/general.py
--rw-r--r--   0        0        0     6060 2023-01-29 11:43:11.729548 slap_cli-1.9.4/src/slap/ext/checks/poetry.py
--rw-r--r--   0        0        0     2815 2023-05-15 14:08:26.480527 slap_cli-1.9.4/src/slap/ext/checks/release.py
--rw-r--r--   0        0        0     8491 2023-01-29 11:43:11.729548 slap_cli-1.9.4/src/slap/ext/project_handlers/base.py
--rw-r--r--   0        0        0     3799 2023-01-29 11:43:11.729548 slap_cli-1.9.4/src/slap/ext/project_handlers/flit.py
--rw-r--r--   0        0        0     6462 2023-05-15 13:23:04.316661 slap_cli-1.9.4/src/slap/ext/project_handlers/poetry.py
--rw-r--r--   0        0        0     5751 2023-01-29 11:43:11.729548 slap_cli-1.9.4/src/slap/ext/project_handlers/setuptools.py
--rw-r--r--   0        0        0     1208 2023-01-29 11:43:11.729548 slap_cli-1.9.4/src/slap/ext/release/changelog.py
--rw-r--r--   0        0        0     2046 2023-01-29 11:43:11.729548 slap_cli-1.9.4/src/slap/ext/release/source_code_version.py
--rw-r--r--   0        0        0    16205 2023-05-15 13:23:04.316661 slap_cli-1.9.4/src/slap/ext/repository_ci/github_actions.py
--rw-r--r--   0        0        0     4065 2023-01-29 11:43:11.729548 slap_cli-1.9.4/src/slap/ext/repository_handlers/default.py
--rw-r--r--   0        0        0     4479 2023-02-20 12:50:15.737708 slap_cli-1.9.4/src/slap/ext/repository_hosts/github.py
--rw-r--r--   0        0        0     1357 2023-01-29 11:43:11.729548 slap_cli-1.9.4/src/slap/ext/version_incrementing_rule.py
--rw-r--r--   0        0        0    10869 2023-01-29 11:43:11.729548 slap_cli-1.9.4/src/slap/install/installer.py
--rw-r--r--   0        0        0     8308 2023-05-15 13:52:59.875225 slap_cli-1.9.4/src/slap/plugins.py
--rw-r--r--   0        0        0     8623 2023-05-15 15:05:38.122588 slap_cli-1.9.4/src/slap/project.py
--rw-r--r--   0        0        0        0 2023-01-29 11:43:11.729548 slap_cli-1.9.4/src/slap/py.typed
--rw-r--r--   0        0        0    14965 2023-05-15 13:23:04.316661 slap_cli-1.9.4/src/slap/python/dependency.py
--rw-r--r--   0        0        0     9711 2023-01-29 11:43:11.733548 slap_cli-1.9.4/src/slap/python/environment.py
--rw-r--r--   0        0        0     6833 2023-01-29 11:43:11.733548 slap_cli-1.9.4/src/slap/python/pep508.py
--rw-r--r--   0        0        0     2535 2023-01-29 11:43:11.733548 slap_cli-1.9.4/src/slap/release.py
--rw-r--r--   0        0        0     5629 2023-05-15 15:05:54.734548 slap_cli-1.9.4/src/slap/repository.py
--rw-r--r--   0        0        0     1091 2023-05-15 13:23:04.316661 slap_cli-1.9.4/src/slap/templates/github/.github/workflows/changelog.yaml
--rw-r--r--   0        0        0      972 2023-05-15 13:23:04.316661 slap_cli-1.9.4/src/slap/templates/github/.github/workflows/python.yaml
--rw-r--r--   0        0        0      246 2023-05-15 13:23:04.316661 slap_cli-1.9.4/src/slap/templates/poetry/.flake8
--rw-r--r--   0        0        0       78 2023-05-15 13:23:04.316661 slap_cli-1.9.4/src/slap/templates/poetry/.gitignore
--rw-r--r--   0        0        0        0 2023-05-15 13:23:04.316661 slap_cli-1.9.4/src/slap/templates/poetry/LICENSE
--rw-r--r--   0        0        0        9 2023-05-15 13:23:04.316661 slap_cli-1.9.4/src/slap/templates/poetry/README.md
--rw-r--r--   0        0        0     1472 2023-05-19 08:33:11.881692 slap_cli-1.9.4/src/slap/templates/poetry/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-15 13:23:04.320661 slap_cli-1.9.4/src/slap/templates/poetry/src/{path}/__init__.py
--rw-r--r--   0        0        0        0 2023-05-15 13:23:04.320661 slap_cli-1.9.4/src/slap/templates/poetry/src/{path}/py.typed
--rw-r--r--   0        0        0       67 2023-05-15 13:23:04.320661 slap_cli-1.9.4/src/slap/templates/poetry/tests/test_import.py
--rw-r--r--   0        0        0     1847 2023-01-29 11:43:11.733548 slap_cli-1.9.4/src/slap/util/cleo.py
--rw-r--r--   0        0        0     4309 2023-01-29 11:43:11.733548 slap_cli-1.9.4/src/slap/util/external/licenses.py
--rw-r--r--   0        0        0     2172 2023-01-29 11:43:11.733548 slap_cli-1.9.4/src/slap/util/external/pypi_classifiers.py
--rw-r--r--   0        0        0      418 2023-01-29 11:43:11.733548 slap_cli-1.9.4/src/slap/util/pygments.py
--rw-r--r--   0        0        0     2113 2023-01-29 11:43:11.733548 slap_cli-1.9.4/src/slap/util/toml_file.py
--rw-r--r--   0        0        0     7363 2023-01-29 11:43:11.733548 slap_cli-1.9.4/src/slap/util/vcs.py
--rw-r--r--   0        0        0     1450 1970-01-01 00:00:00.000000 slap_cli-1.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-01-29 11:43:11.729548 slap_cli-1.9.5/LICENSE
+-rw-r--r--   0        0        0     4981 2023-06-19 15:04:44.343754 slap_cli-1.9.5/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-06-19 15:04:44.347754 slap_cli-1.9.5/src/slap/__init__.py
+-rw-r--r--   0        0        0      122 2023-05-15 14:08:15.856560 slap_cli-1.9.5/src/slap/__main__.py
+-rw-r--r--   0        0        0    12941 2023-06-19 14:59:50.401440 slap_cli-1.9.5/src/slap/application.py
+-rw-r--r--   0        0        0     9163 2023-02-09 13:39:04.453992 slap_cli-1.9.5/src/slap/changelog.py
+-rw-r--r--   0        0        0     3353 2023-01-29 11:43:11.729548 slap_cli-1.9.5/src/slap/check.py
+-rw-r--r--   0        0        0     2533 2023-05-15 15:02:36.078985 slap_cli-1.9.5/src/slap/configuration.py
+-rw-r--r--   0        0        0     5337 2023-05-15 13:54:26.739024 slap_cli-1.9.5/src/slap/ext/application/add.py
+-rw-r--r--   0        0        0    27292 2023-05-15 16:43:58.997086 slap_cli-1.9.5/src/slap/ext/application/changelog.py
+-rw-r--r--   0        0        0     6330 2023-05-15 14:28:58.852972 slap_cli-1.9.5/src/slap/ext/application/check.py
+-rw-r--r--   0        0        0     3177 2023-05-15 14:02:47.957819 slap_cli-1.9.5/src/slap/ext/application/info.py
+-rw-r--r--   0        0        0     4911 2023-05-19 08:24:24.059256 slap_cli-1.9.5/src/slap/ext/application/init.py
+-rw-r--r--   0        0        0    13604 2023-06-19 15:03:13.515086 slap_cli-1.9.5/src/slap/ext/application/install.py
+-rw-r--r--   0        0        0     5982 2023-05-15 14:16:35.467350 slap_cli-1.9.5/src/slap/ext/application/link.py
+-rw-r--r--   0        0        0     4230 2023-05-15 14:29:48.828826 slap_cli-1.9.5/src/slap/ext/application/publish.py
+-rw-r--r--   0        0        0    21667 2023-05-15 14:33:39.328295 slap_cli-1.9.5/src/slap/ext/application/release.py
+-rw-r--r--   0        0        0     3243 2023-05-15 14:30:47.388698 slap_cli-1.9.5/src/slap/ext/application/report.py
+-rw-r--r--   0        0        0     3555 2023-05-15 14:59:30.475460 slap_cli-1.9.5/src/slap/ext/application/run.py
+-rw-r--r--   0        0        0     8129 2023-06-19 15:03:08.063044 slap_cli-1.9.5/src/slap/ext/application/test.py
+-rw-r--r--   0        0        0    19880 2023-05-15 14:20:06.182817 slap_cli-1.9.5/src/slap/ext/application/venv.py
+-rw-r--r--   0        0        0     2075 2023-01-29 11:43:11.729548 slap_cli-1.9.5/src/slap/ext/checks/changelog.py
+-rw-r--r--   0        0        0     2215 2023-01-29 11:43:11.729548 slap_cli-1.9.5/src/slap/ext/checks/general.py
+-rw-r--r--   0        0        0     6060 2023-01-29 11:43:11.729548 slap_cli-1.9.5/src/slap/ext/checks/poetry.py
+-rw-r--r--   0        0        0     2815 2023-05-15 14:08:26.480527 slap_cli-1.9.5/src/slap/ext/checks/release.py
+-rw-r--r--   0        0        0     8491 2023-01-29 11:43:11.729548 slap_cli-1.9.5/src/slap/ext/project_handlers/base.py
+-rw-r--r--   0        0        0     3799 2023-01-29 11:43:11.729548 slap_cli-1.9.5/src/slap/ext/project_handlers/flit.py
+-rw-r--r--   0        0        0     6462 2023-05-15 13:23:04.316661 slap_cli-1.9.5/src/slap/ext/project_handlers/poetry.py
+-rw-r--r--   0        0        0     5751 2023-01-29 11:43:11.729548 slap_cli-1.9.5/src/slap/ext/project_handlers/setuptools.py
+-rw-r--r--   0        0        0     1208 2023-01-29 11:43:11.729548 slap_cli-1.9.5/src/slap/ext/release/changelog.py
+-rw-r--r--   0        0        0     2046 2023-01-29 11:43:11.729548 slap_cli-1.9.5/src/slap/ext/release/source_code_version.py
+-rw-r--r--   0        0        0    16205 2023-05-15 13:23:04.316661 slap_cli-1.9.5/src/slap/ext/repository_ci/github_actions.py
+-rw-r--r--   0        0        0     4065 2023-01-29 11:43:11.729548 slap_cli-1.9.5/src/slap/ext/repository_handlers/default.py
+-rw-r--r--   0        0        0     4479 2023-02-20 12:50:15.737708 slap_cli-1.9.5/src/slap/ext/repository_hosts/github.py
+-rw-r--r--   0        0        0     1357 2023-01-29 11:43:11.729548 slap_cli-1.9.5/src/slap/ext/version_incrementing_rule.py
+-rw-r--r--   0        0        0    10869 2023-01-29 11:43:11.729548 slap_cli-1.9.5/src/slap/install/installer.py
+-rw-r--r--   0        0        0     8308 2023-05-15 13:52:59.875225 slap_cli-1.9.5/src/slap/plugins.py
+-rw-r--r--   0        0        0     8623 2023-05-15 15:05:38.122588 slap_cli-1.9.5/src/slap/project.py
+-rw-r--r--   0        0        0        0 2023-01-29 11:43:11.729548 slap_cli-1.9.5/src/slap/py.typed
+-rw-r--r--   0        0        0    14965 2023-05-15 13:23:04.316661 slap_cli-1.9.5/src/slap/python/dependency.py
+-rw-r--r--   0        0        0     9711 2023-01-29 11:43:11.733548 slap_cli-1.9.5/src/slap/python/environment.py
+-rw-r--r--   0        0        0     6833 2023-01-29 11:43:11.733548 slap_cli-1.9.5/src/slap/python/pep508.py
+-rw-r--r--   0        0        0     2535 2023-01-29 11:43:11.733548 slap_cli-1.9.5/src/slap/release.py
+-rw-r--r--   0        0        0     5629 2023-05-15 15:05:54.734548 slap_cli-1.9.5/src/slap/repository.py
+-rw-r--r--   0        0        0     1091 2023-05-15 13:23:04.316661 slap_cli-1.9.5/src/slap/templates/github/.github/workflows/changelog.yaml
+-rw-r--r--   0        0        0      972 2023-05-15 13:23:04.316661 slap_cli-1.9.5/src/slap/templates/github/.github/workflows/python.yaml
+-rw-r--r--   0        0        0      246 2023-05-15 13:23:04.316661 slap_cli-1.9.5/src/slap/templates/poetry/.flake8
+-rw-r--r--   0        0        0       78 2023-05-15 13:23:04.316661 slap_cli-1.9.5/src/slap/templates/poetry/.gitignore
+-rw-r--r--   0        0        0        0 2023-05-15 13:23:04.316661 slap_cli-1.9.5/src/slap/templates/poetry/LICENSE
+-rw-r--r--   0        0        0        9 2023-05-15 13:23:04.316661 slap_cli-1.9.5/src/slap/templates/poetry/README.md
+-rw-r--r--   0        0        0     1472 2023-05-19 08:33:11.881692 slap_cli-1.9.5/src/slap/templates/poetry/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-15 13:23:04.320661 slap_cli-1.9.5/src/slap/templates/poetry/src/{path}/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:23:04.320661 slap_cli-1.9.5/src/slap/templates/poetry/src/{path}/py.typed
+-rw-r--r--   0        0        0       67 2023-05-15 13:23:04.320661 slap_cli-1.9.5/src/slap/templates/poetry/tests/test_import.py
+-rw-r--r--   0        0        0     1847 2023-01-29 11:43:11.733548 slap_cli-1.9.5/src/slap/util/cleo.py
+-rw-r--r--   0        0        0     4309 2023-01-29 11:43:11.733548 slap_cli-1.9.5/src/slap/util/external/licenses.py
+-rw-r--r--   0        0        0     2172 2023-01-29 11:43:11.733548 slap_cli-1.9.5/src/slap/util/external/pypi_classifiers.py
+-rw-r--r--   0        0        0      418 2023-01-29 11:43:11.733548 slap_cli-1.9.5/src/slap/util/pygments.py
+-rw-r--r--   0        0        0      114 2023-06-19 14:59:51.061445 slap_cli-1.9.5/src/slap/util/strings.py
+-rw-r--r--   0        0        0     2113 2023-01-29 11:43:11.733548 slap_cli-1.9.5/src/slap/util/toml_file.py
+-rw-r--r--   0        0        0     7363 2023-01-29 11:43:11.733548 slap_cli-1.9.5/src/slap/util/vcs.py
+-rw-r--r--   0        0        0     1450 1970-01-01 00:00:00.000000 slap_cli-1.9.5/PKG-INFO
```

### Comparing `slap_cli-1.9.4/LICENSE` & `slap_cli-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/pyproject.toml` & `slap_cli-1.9.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "slap-cli"
-version = "1.9.4"
+version = "1.9.5"
 description = "Slap is a command-line utility for developing Python applications."
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 packages = [{ include = "slap", from = "src" }]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Console",
```

### Comparing `slap_cli-1.9.4/src/slap/application.py` & `slap_cli-1.9.5/src/slap/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from cleo.application import Application as BaseCleoApplication  # type: ignore[import]
 from cleo.commands.command import Command as _BaseCommand  # type: ignore[import]
 from cleo.helpers import argument, option  # type: ignore[import]
 from cleo.io.io import IO  # type: ignore[import]
 from databind.core.settings import Alias
 
 from slap import __version__
+from slap.util.strings import split_by_commata
 
 if t.TYPE_CHECKING:
     from nr.util.functional import Once
 
     from slap.configuration import Configuration
     from slap.project import Project
     from slap.repository import Repository
@@ -257,25 +258,38 @@
         self.load_plugins()
 
     def run(self) -> None:
         """Loads and activates application plugins and then invokes the CLI."""
 
         self.cleo.run()
 
-    def get_target_projects(self) -> list[Project]:
+    def get_target_projects(self, only_projects: str | t.Sequence[str] | None = None) -> list[Project]:
         """
         Returns the list of projects that should be dealt with when executing a command. When there is a main project,
         only the main project will be returned. When in the repository root, all projects will be returned.
         """
 
+        if isinstance(only_projects, str):
+            only_projects = split_by_commata(only_projects)
+
+        if only_projects is not None:
+            projects: list[Project] = []
+            for only_project in only_projects:
+                project_path = Path(only_project).resolve()
+                matching_projects = [p for p in self.repository.projects() if p.directory.resolve() == project_path]
+                if not matching_projects:
+                    raise ValueError(f'error: "{only_project}" does not point to a project')
+                projects += matching_projects
+            return projects
+
         main = self.main_project()
         if main:
             return [main]
         if self._directory == self.repository.directory:
-            return self.repository.projects()
+            return self.repository.get_projects_ordered()
         return []
 
 
 def find_repository(directory: Path) -> Repository:
     """
     Finds the repository for the given directory. This will search for the closest parent directory that contains a
     `slap.toml` configuration file. If no such file exists, but we're in a Git directory, and the given *directory*
```

### Comparing `slap_cli-1.9.4/src/slap/changelog.py` & `slap_cli-1.9.5/src/slap/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/check.py` & `slap_cli-1.9.5/src/slap/check.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/configuration.py` & `slap_cli-1.9.5/src/slap/configuration.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/application/add.py` & `slap_cli-1.9.5/src/slap/ext/application/add.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/application/changelog.py` & `slap_cli-1.9.5/src/slap/ext/application/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/application/check.py` & `slap_cli-1.9.5/src/slap/ext/application/check.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/application/info.py` & `slap_cli-1.9.5/src/slap/ext/application/info.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/application/init.py` & `slap_cli-1.9.5/src/slap/ext/application/init.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/application/install.py` & `slap_cli-1.9.5/src/slap/ext/application/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -299,31 +299,15 @@
                 return False
 
         return True
 
     def _get_projects_to_install(self) -> list[Project]:
         """Return the list of Slap projects to install."""
 
-        if only_project := self.option("only"):
-            project_path = Path(only_project).resolve()
-            projects = [p for p in self.app.repository.projects() if p.directory.resolve() == project_path]
-            if not projects:
-                self.line_error(f'error: "{only_project}" does not point to a project', "error")
-                return []
-            assert len(projects) == 1, projects
-            return projects
-
-        else:
-            main_project = self.app.main_project()
-            if main_project:
-                return [main_project]
-            if not self.app.repository.projects:
-                self.line_error("error: no projects found")
-                return []
-            return self.app.repository.get_projects_ordered()
+        return self.app.get_target_projects(self.option("only"))
 
     def _get_extras_to_install(self) -> set[str]:
         """Return a set of the extras that should be installed."""
 
         extras = set(map(str.strip, (self.option("extras") or self.option("only-extras") or "").split(",")))
         extras.discard("")
```

### Comparing `slap_cli-1.9.4/src/slap/ext/application/link.py` & `slap_cli-1.9.5/src/slap/ext/application/link.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/application/publish.py` & `slap_cli-1.9.5/src/slap/ext/application/publish.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/application/release.py` & `slap_cli-1.9.5/src/slap/ext/application/release.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/application/report.py` & `slap_cli-1.9.5/src/slap/ext/application/report.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/application/run.py` & `slap_cli-1.9.5/src/slap/ext/application/run.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/application/test.py` & `slap_cli-1.9.5/src/slap/ext/application/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,23 +111,28 @@
       <fg=dark_gray>mypy | Success: no issues found in 12 source files
       pytest | ===================================== test session starts ======================================
       pytest | platform linux -- Python 3.10.2, pytest-6.2.5, py-1.11.0, pluggy-1.0.0
       ...</fg>
     """
 
     app: Application
-    tests: list[Test]
     requires_venv: t.ClassVar[bool] = False
 
     name = "test"
     arguments = [
         argument("test", "One or more tests to run (runs all if none are specified)", optional=True, multiple=True),
     ]
     options = VenvAwareCommand.options + [
         option(
+            "--only",
+            description="Only run the tests for the projects in the given subdirectory. Multiple directories can be "
+            "specified by delimiting them with a comma.",
+            flag=False,
+        ),
+        option(
             "--no-line-prefix",
             "-s",
             description="Do not prefix output from the test commands with the test name (default if a single argument "
             "for <info>test</info> is specified).",
         ),
         option(
             "--list",
@@ -144,22 +149,27 @@
     ]
 
     # Hack to set a default value for the flag.
     next(opt for opt in options if opt.name == "no-line-prefix")._default = NotSet.Value  # type: ignore[assignment]
 
     def load_configuration(self, app: Application) -> None:
         self.app = app
-        self.tests = []
-        for project in app.get_target_projects():
-            for test_name, command in project.raw_config().get("test", {}).items():
-                self.tests.append(Test(project, test_name, command))
 
     def activate(self, app: Application, config: None) -> None:
         app.cleo.add(self)
 
+    @property
+    def tests(self) -> list[Test]:
+        tests = []
+        projects = self.app.get_target_projects(self.option("only"))
+        for project in projects:
+            for test_name, command in project.raw_config().get("test", {}).items():
+                tests.append(Test(project, test_name, command))
+        return tests
+
     def _select_tests(self, name: str) -> set[Test]:
         result = set()
         for test in self.tests:
             use_test = (
                 self.app.repository.is_monorepo
                 and (name == test.id or (name.startswith(":") and test.name == name[1:]) or (test.project.id == name))
                 or not self.app.repository.is_monorepo
```

### Comparing `slap_cli-1.9.4/src/slap/ext/application/venv.py` & `slap_cli-1.9.5/src/slap/ext/application/venv.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/checks/changelog.py` & `slap_cli-1.9.5/src/slap/ext/checks/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/checks/general.py` & `slap_cli-1.9.5/src/slap/ext/checks/general.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/checks/poetry.py` & `slap_cli-1.9.5/src/slap/ext/checks/poetry.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/checks/release.py` & `slap_cli-1.9.5/src/slap/ext/checks/release.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/project_handlers/base.py` & `slap_cli-1.9.5/src/slap/ext/project_handlers/base.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/project_handlers/flit.py` & `slap_cli-1.9.5/src/slap/ext/project_handlers/flit.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/project_handlers/poetry.py` & `slap_cli-1.9.5/src/slap/ext/project_handlers/poetry.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/project_handlers/setuptools.py` & `slap_cli-1.9.5/src/slap/ext/project_handlers/setuptools.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/release/changelog.py` & `slap_cli-1.9.5/src/slap/ext/release/changelog.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/release/source_code_version.py` & `slap_cli-1.9.5/src/slap/ext/release/source_code_version.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/repository_ci/github_actions.py` & `slap_cli-1.9.5/src/slap/ext/repository_ci/github_actions.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/repository_handlers/default.py` & `slap_cli-1.9.5/src/slap/ext/repository_handlers/default.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/repository_hosts/github.py` & `slap_cli-1.9.5/src/slap/ext/repository_hosts/github.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/ext/version_incrementing_rule.py` & `slap_cli-1.9.5/src/slap/ext/version_incrementing_rule.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/install/installer.py` & `slap_cli-1.9.5/src/slap/install/installer.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/plugins.py` & `slap_cli-1.9.5/src/slap/plugins.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/project.py` & `slap_cli-1.9.5/src/slap/project.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/python/dependency.py` & `slap_cli-1.9.5/src/slap/python/dependency.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/python/environment.py` & `slap_cli-1.9.5/src/slap/python/environment.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/python/pep508.py` & `slap_cli-1.9.5/src/slap/python/pep508.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/release.py` & `slap_cli-1.9.5/src/slap/release.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/repository.py` & `slap_cli-1.9.5/src/slap/repository.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/templates/github/.github/workflows/changelog.yaml` & `slap_cli-1.9.5/src/slap/templates/github/.github/workflows/changelog.yaml`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/templates/github/.github/workflows/python.yaml` & `slap_cli-1.9.5/src/slap/templates/github/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/templates/poetry/pyproject.toml` & `slap_cli-1.9.5/src/slap/templates/poetry/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/util/cleo.py` & `slap_cli-1.9.5/src/slap/util/cleo.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/util/external/licenses.py` & `slap_cli-1.9.5/src/slap/util/external/licenses.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/util/external/pypi_classifiers.py` & `slap_cli-1.9.5/src/slap/util/external/pypi_classifiers.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/util/toml_file.py` & `slap_cli-1.9.5/src/slap/util/toml_file.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/src/slap/util/vcs.py` & `slap_cli-1.9.5/src/slap/util/vcs.py`

 * *Files identical despite different names*

### Comparing `slap_cli-1.9.4/PKG-INFO` & `slap_cli-1.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slap-cli
-Version: 1.9.4
+Version: 1.9.5
 Summary: Slap is a command-line utility for developing Python applications.
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

