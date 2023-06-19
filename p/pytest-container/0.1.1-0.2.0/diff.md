# Comparing `tmp/pytest_container-0.1.1.tar.gz` & `tmp/pytest_container-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_container-0.1.1.tar", max compression
+gzip compressed data, was "pytest_container-0.2.0.tar", max compression
```

## Comparing `pytest_container-0.1.1.tar` & `pytest_container-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    26529 2021-10-08 13:15:14.394542 pytest_container-0.1.1/LICENSE
--rw-r--r--   0        0        0     3098 2023-03-21 07:57:20.813678 pytest_container-0.1.1/README.rst
--rw-r--r--   0        0        0     1812 2023-03-21 07:57:20.814678 pytest_container-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      885 2023-03-13 13:25:07.886901 pytest_container-0.1.1/pytest_container/__init__.py
--rw-r--r--   0        0        0    10071 2023-03-13 13:24:53.195912 pytest_container-0.1.1/pytest_container/build.py
--rw-r--r--   0        0        0    35796 2023-03-20 08:57:48.682447 pytest_container-0.1.1/pytest_container/container.py
--rw-r--r--   0        0        0     5306 2023-02-15 14:43:16.942510 pytest_container-0.1.1/pytest_container/helpers.py
--rw-r--r--   0        0        0     8810 2023-03-15 10:13:40.486872 pytest_container-0.1.1/pytest_container/inspect.py
--rw-r--r--   0        0        0      362 2023-02-15 14:43:01.064514 pytest_container-0.1.1/pytest_container/logging.py
--rw-r--r--   0        0        0     6114 2023-03-13 13:25:07.890901 pytest_container-0.1.1/pytest_container/plugin.py
--rw-r--r--   0        0        0     7870 2023-03-20 08:58:06.665440 pytest_container-0.1.1/pytest_container/pod.py
--rw-r--r--   0        0        0    20073 2023-03-20 16:18:28.260007 pytest_container-0.1.1/pytest_container/runtime.py
--rw-r--r--   0        0        0     4768 1970-01-01 00:00:00.000000 pytest_container-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    26529 2023-04-18 07:11:49.372516 pytest_container-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3098 2023-04-18 07:11:49.372516 pytest_container-0.2.0/README.rst
+-rw-r--r--   0        0        0     1858 2023-06-19 07:54:35.365666 pytest_container-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      885 2023-04-18 07:11:49.373516 pytest_container-0.2.0/pytest_container/__init__.py
+-rw-r--r--   0        0        0    10071 2023-04-18 07:11:49.373516 pytest_container-0.2.0/pytest_container/build.py
+-rw-r--r--   0        0        0    36915 2023-06-14 09:57:59.292310 pytest_container-0.2.0/pytest_container/container.py
+-rw-r--r--   0        0        0     5306 2023-04-18 07:11:49.373516 pytest_container-0.2.0/pytest_container/helpers.py
+-rw-r--r--   0        0        0     8928 2023-06-14 09:57:59.293310 pytest_container-0.2.0/pytest_container/inspect.py
+-rw-r--r--   0        0        0      362 2023-04-18 07:11:49.373516 pytest_container-0.2.0/pytest_container/logging.py
+-rw-r--r--   0        0        0     7426 2023-06-14 12:10:05.835567 pytest_container-0.2.0/pytest_container/plugin.py
+-rw-r--r--   0        0        0     7950 2023-06-14 09:57:59.293310 pytest_container-0.2.0/pytest_container/pod.py
+-rw-r--r--   0        0        0    21340 2023-06-12 15:47:12.592839 pytest_container-0.2.0/pytest_container/runtime.py
+-rw-r--r--   0        0        0     4567 1970-01-01 00:00:00.000000 pytest_container-0.2.0/PKG-INFO
```

### Comparing `pytest_container-0.1.1/LICENSE` & `pytest_container-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_container-0.1.1/README.rst` & `pytest_container-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest_container-0.1.1/pyproject.toml` & `pytest_container-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest_container"
-version = "0.1.1"
+version = "0.2.0"
 description = "Pytest fixtures for writing container based tests"
 authors = ["Dan Čermák <dcermak@suse.com>"]
 homepage = "https://dcermak.github.io/pytest_container/"
 repository = "https://github.com/dcermak/pytest_container/"
 readme = "README.rst"
 license = "LGPL-2.1-or-later"
 classifiers = [
@@ -15,14 +15,15 @@
     "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Quality Assurance",
     "Topic :: Software Development :: Testing"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.6.2,<4.0"
 pytest = ">= 3.10"
```

### Comparing `pytest_container-0.1.1/pytest_container/__init__.py` & `pytest_container-0.2.0/pytest_container/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_container-0.1.1/pytest_container/build.py` & `pytest_container-0.2.0/pytest_container/build.py`

 * *Files identical despite different names*

### Comparing `pytest_container-0.1.1/pytest_container/container.py` & `pytest_container-0.2.0/pytest_container/container.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import itertools
 import operator
 import os
 import socket
 import sys
 import tempfile
 import time
+import warnings
 from abc import ABC
 from abc import abstractmethod
 from dataclasses import dataclass
 from dataclasses import field
 from datetime import datetime
 from datetime import timedelta
 from hashlib import md5
@@ -94,39 +95,14 @@
             PortForwarding(
                 container_port=port.container_port,
                 protocol=port.protocol,
                 host_port=port_num,
             )
         )
         sockets.append(sock)
-        # port_added = True
-
-        #     if not socket.has_ipv6 or (
-        #         socket.has_dualstack_ipv6()
-        #         and port.protocol == NetworkProtocol.TCP
-        #     ):
-        #         add_port()
-        #         break
-        #     else:
-        #         try:
-        #             sock2 = socket.socket(
-        #                 family=socket.AF_INET6, type=port.protocol.SOCK_CONST
-        #             )
-        #             sock2.bind(("", port_num))
-        #         except OSError:
-        #             sock.close()
-        #         else:
-        #             add_port()
-        #             sockets.append(sock2)
-        #             break
-
-        # if not port_added:
-        #     raise RuntimeError(
-        #         f"Failed to find a free port for {port}, giving up after {retries} retries."
-        #     )
 
     for sock in sockets:
         sock.close()
 
     assert len(port_forwards) == len(finished_forwards)
     return finished_forwards
 
@@ -645,18 +621,21 @@
 
     base: Union[Container, "DerivedContainer", str] = ""
 
     #: The :file:`Containerfile` that is used to build this container derived
     #: from :py:attr:`base`.
     containerfile: str = ""
 
-    #: An optional image format when building images with :command:`buildah`.
-    #: This attribute can be used to instruct :command:`buildah` to build images
-    #: in the ``docker`` format, instead of the default (``oci``).
-    #: This attribute is ignored by :command:`docker`.
+    #: An optional image format when building images with :command:`buildah`. It
+    #: is ignored when the container runtime is :command:`docker`.
+    #: The ``oci`` image format is used by default. If the image format is
+    #: ``None`` and the base image has a ``HEALTHCHECK`` defined, then the
+    #: ``docker`` image format will be used instead.
+    #: Specifying an image format disables the auto-detection and uses the
+    #: supplied value.
     image_format: Optional[ImageFormat] = None
 
     #: Additional build tags/names that should be added to the container once it
     #: has been built
     add_build_tags: List[str] = field(default_factory=list)
 
     def __post_init__(self) -> None:
@@ -717,25 +696,53 @@
                 _logger.debug(
                     "Writing containerfile to %s: %s",
                     containerfile_path,
                     containerfile_contents,
                 )
                 containerfile.write(containerfile_contents)
 
-            image_format_args: List[str] = []
-            if (
-                self.image_format is not None
-                and "buildah" in runtime.build_command
-            ):
-                image_format_args = ["--format", str(self.image_format)]
+            cmd = runtime.build_command
+            if "buildah" in runtime.build_command:
+                if self.image_format is not None:
+                    cmd += ["--format", str(self.image_format)]
+                else:
+                    assert (
+                        "podman" in runtime.runner_binary
+                    ), "The runner for buildah should be podman"
+
+                    if not runtime.supports_healthcheck_inherit_from_base:
+                        warnings.warn(
+                            UserWarning(
+                                "Runtime does not support inheriting HEALTHCHECK "
+                                "from base images, image format auto-detection "
+                                "will *not* work!"
+                            )
+                        )
+
+                    # if the parent image has a healthcheck defined, then we
+                    # have to use the docker image format, so that the
+                    # healthcheck is in newly build image as well
+                    elif (
+                        "<nil>"
+                        != check_output(
+                            [
+                                runtime.runner_binary,
+                                "inspect",
+                                "-f",
+                                "{{.HealthCheck}}",
+                                from_id,
+                            ]
+                        )
+                        .decode()
+                        .strip()
+                    ):
+                        cmd += ["--format", str(ImageFormat.DOCKER)]
 
-            cmd = (
-                runtime.build_command
-                + image_format_args
-                + (extra_build_args or [])
+            cmd += (
+                (extra_build_args or [])
                 + (
                     functools.reduce(
                         operator.add,
                         (["-t", tag] for tag in self.add_build_tags),
                     )
                     if self.add_build_tags
                     else []
@@ -771,14 +778,18 @@
     #: any ports that are exposed by this container
     forwarded_ports: List[PortForwarding]
 
     _container_runtime: OciRuntimeBase
 
     @property
     def inspect(self) -> ContainerInspect:
+        """Inspect the launched container and return the result of
+        :command:`$runtime inspect $ctr_id`.
+
+        """
         return self._container_runtime.inspect_container(self.container_id)
 
 
 def container_to_pytest_param(
     container: ContainerBase,
     marks: Optional[Union[Collection[MarkDecorator], MarkDecorator]] = None,
 ) -> ParameterSet:
@@ -865,22 +876,32 @@
         # __exit__()
         lock = FileLock(
             Path(tempfile.gettempdir()) / self.container.filelock_filename
         )
         _logger.debug(
             "Locking container preparation via file %s", lock.lock_file
         )
-        lock.acquire()
 
         def release_lock() -> None:
             _logger.debug("Releasing lock %s", lock.lock_file)
             lock.release()
             os.unlink(lock.lock_file)
 
-        self.container.prepare_container(self.rootdir, self.extra_build_args)
+        # Container preparation can fail, but then we would never release the
+        # lock as release_lock is not yet in self._stack. However, we do not
+        # want to add it into the exitstack for most containers either, as they
+        # should get unlocked right after preparation.
+        try:
+            lock.acquire()
+            self.container.prepare_container(
+                self.rootdir, self.extra_build_args
+            )
+        except:
+            release_lock()
+            raise
 
         # ordinary containers are only locked during the build,
         # singleton containers are unlocked after everything
         if not self.container.singleton:
             release_lock()
         else:
             self._stack.callback(release_lock)
```

### Comparing `pytest_container-0.1.1/pytest_container/helpers.py` & `pytest_container-0.2.0/pytest_container/helpers.py`

 * *Files identical despite different names*

### Comparing `pytest_container-0.1.1/pytest_container/inspect.py` & `pytest_container-0.2.0/pytest_container/inspect.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""This module contains the class definitions that represent the output of
+:command:`$runtime inspect $ctr_id`.
+
+"""
 import enum
 import socket
 from dataclasses import dataclass
 from dataclasses import field
 from datetime import timedelta
 from typing import Dict
 from typing import List
@@ -143,15 +147,15 @@
 _DEFAULT_INTERVAL = timedelta(seconds=30)
 _DEFAULT_TIMEOUT = timedelta(seconds=30)
 _DEFAULT_RETRIES = 3
 
 
 @dataclass(frozen=True)
 class HealthCheck:
-    """The HEALTCHECK of a container image."""
+    """The HEALTHCHECK of a container image."""
 
     #: startup period of the container during which healthcheck failures will
     #: not count towards the failure count
     start_period: timedelta = field(default=_DEFAULT_START_PERIOD)
 
     #: healthcheck command is run every interval
     interval: timedelta = field(default=_DEFAULT_INTERVAL)
```

### Comparing `pytest_container-0.1.1/pytest_container/plugin.py` & `pytest_container-0.2.0/pytest_container/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """The plugin module contains all fixtures that are provided by
 ``pytest_container``.
 
 """
 import sys
+from subprocess import PIPE
+from subprocess import run
 from typing import Callable
 from typing import Generator
 
 from pytest_container.container import container_from_pytest_param
 from pytest_container.container import ContainerData
 from pytest_container.container import ContainerLauncher
 from pytest_container.helpers import get_extra_build_args
@@ -34,14 +36,32 @@
     """pytest fixture that returns the currently selected container runtime
     according to the rules outlined :ref:`here <runtime selection rules>`.
 
     """
     return get_selected_runtime()
 
 
+def _log_container_logs(
+    container_id: str, ctr_runtime: OciRuntimeBase
+) -> None:
+    # don't die if logging fails for some reason
+    # pylint: disable=subprocess-run-check
+    logs_call = run(
+        [ctr_runtime.runner_binary, "logs", container_id],
+        stdout=PIPE,
+        stderr=PIPE,
+    )
+    if logs_call.returncode == 0:
+        _logger.debug(
+            "logs from container %s: %s",
+            container_id,
+            logs_call.stdout.decode(),
+        )
+
+
 def _create_auto_container_fixture(
     scope: Literal["session", "function"]
 ) -> Callable[
     [SubRequest, OciRuntimeBase, Config], Generator[ContainerData, None, None]
 ]:
     def fixture(
         request: SubRequest,
@@ -82,16 +102,26 @@
         with ContainerLauncher(
             container=launch_data,
             container_runtime=container_runtime,
             rootdir=pytestconfig.rootpath,
             extra_build_args=get_extra_build_args(pytestconfig),
             extra_run_args=get_extra_run_args(pytestconfig) + add_labels,
         ) as launcher:
-            launcher.launch_container()
-            yield launcher.container_data
+            # we want to ensure that the container's logs are saved at "all
+            # cost", especially when the container fails to launch for some
+            # reason
+            try:
+                launcher.launch_container()
+                container_data = launcher.container_data
+                yield container_data
+            finally:
+                if launcher._container_id:
+                    _log_container_logs(
+                        launcher._container_id, container_runtime
+                    )
 
     return pytest.fixture(scope=scope)(fixture)
 
 
 def _create_auto_pod_fixture(
     scope: Literal["session", "function"]
 ) -> Callable[
@@ -112,16 +142,24 @@
         with PodLauncher(
             pod,
             rootdir=pytestconfig.rootpath,
             extra_build_args=get_extra_build_args(pytestconfig),
             extra_run_args=get_extra_run_args(pytestconfig),
             extra_pod_create_args=get_extra_pod_create_args(pytestconfig),
         ) as launcher:
-            launcher.launch_pod()
-            yield launcher.pod_data
+            try:
+                launcher.launch_pod()
+                pod_data = launcher.pod_data
+                yield pod_data
+            finally:
+                for ctr_launcher in launcher._launchers:
+                    if ctr_launcher._container_id:
+                        _log_container_logs(
+                            ctr_launcher._container_id, container_runtime
+                        )
 
     return pytest.fixture(scope=scope)(fixture)
 
 
 #: This fixture parametrizes the test function once for each container image
 #: defined in the module level variable ``CONTAINER_IMAGES`` of the current test
 #: module and yield an instance of
```

### Comparing `pytest_container-0.1.1/pytest_container/pod.py` & `pytest_container-0.2.0/pytest_container/pod.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,14 +200,15 @@
     ) -> None:
         self._stack.close()
         self._pod_id = None
         self._infra_container_id = None
 
     @property
     def pod_data(self) -> PodData:
+        """Returns the :py:class:`PodData` corresponding to this podman pod."""
         if not self._pod_id or not self._infra_container_id:
             raise RuntimeError("Pod has not been created")
 
         return PodData(
             pod=self.pod,
             container_data=[
                 launcher.container_data for launcher in self._launchers
```

### Comparing `pytest_container-0.1.1/pytest_container/runtime.py` & `pytest_container-0.2.0/pytest_container/runtime.py`

 * *Files 7% similar despite different names*

```diff
@@ -220,14 +220,22 @@
     def inspect_container(self, container_id: str) -> ContainerInspect:
         """Inspect the container with the provided ``container_id`` and return
         the parsed output from the container runtime as an instance of
         :py:class:`~pytest_container.inspect.ContainerInspect`.
 
         """
 
+    @property
+    @abstractmethod
+    def supports_healthcheck_inherit_from_base(self) -> bool:
+        """Indicates whether the container runtime supports that derived images
+        will inherit the healthcheck from the base image.
+
+        """
+
 
 class OciRuntimeBase(_OciRuntimeBase, OciRuntimeABC, ToParamMixin):
     """Base class of the Container Runtimes."""
 
     def __post_init__(self) -> None:
         if not self.build_command or not self.runner_binary:
             raise ValueError(
@@ -397,20 +405,33 @@
 
 LOCALHOST = testinfra.host.get_host("local://")
 
 
 def _get_podman_version(version_stdout: str) -> Version:
     if version_stdout[:15] != "podman version ":
         raise RuntimeError(
-            f"Could not decode the podman version from {version_stdout}"
+            f"Could not decode the podman version from '{version_stdout}'"
         )
 
     return Version.parse(version_stdout[15:])
 
 
+def _get_buildah_version() -> Version:
+    version_stdout = LOCALHOST.run_expect([0], "buildah --version").stdout
+    BUILD_VERSION_BEGIN = "buildah version "
+    if version_stdout[:16] != BUILD_VERSION_BEGIN:
+        raise RuntimeError(
+            f"Could not decode the buildah version from '{version_stdout}'"
+        )
+
+    return Version.parse(
+        version_stdout.replace(BUILD_VERSION_BEGIN, "").split(" ")[0]
+    )
+
+
 class PodmanRuntime(OciRuntimeBase):
     """The container runtime using :command:`podman` for running containers and
     :command:`buildah` for building containers.
 
     """
 
     _runtime_functional = (
@@ -448,14 +469,24 @@
     @cached_property
     def version(self) -> Version:
         """Returns the version of podman installed on the system"""
         return _get_podman_version(
             LOCALHOST.run_expect([0], "podman --version").stdout
         )
 
+    @cached_property
+    def supports_healthcheck_inherit_from_base(self) -> bool:
+        # - buildah supports inheriting HEALTHCHECK since 1.25.0
+        #   https://github.com/containers/buildah/blob/main/CHANGELOG.md#v1250-2022-03-25
+        # - podman 4.1.0 bundles buildah >= 1.25.0
+        #   https://github.com/containers/podman/blob/main/RELEASE_NOTES.md#misc-8
+        return self.version >= Version(
+            4, 1, 0
+        ) and _get_buildah_version() >= Version(1, 25, 0)
+
     def inspect_container(self, container_id: str) -> ContainerInspect:
         inspect = self._get_container_inspect(container_id)
 
         Conf = inspect["Config"]
         healthcheck = None
         if "Healthcheck" in Conf:
             healthcheck = HealthCheck.from_container_inspect(
@@ -532,14 +563,18 @@
     @cached_property
     def version(self) -> Version:
         """Returns the version of docker installed on this system"""
         return _get_docker_version(
             LOCALHOST.run_expect([0], "docker --version").stdout
         )
 
+    @property
+    def supports_healthcheck_inherit_from_base(self) -> bool:
+        return True
+
     def inspect_container(self, container_id: str) -> ContainerInspect:
         inspect = self._get_container_inspect(container_id)
 
         Conf = inspect["Config"]
         if Conf.get("Env"):
             env = dict([env.split("=", maxsplit=1) for env in Conf["Env"]])
         else:
```

### Comparing `pytest_container-0.1.1/PKG-INFO` & `pytest_container-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-container
-Version: 0.1.1
+Version: 0.2.0
 Summary: Pytest fixtures for writing container based tests
 Home-page: https://dcermak.github.io/pytest_container/
 License: LGPL-2.1-or-later
 Author: Dan Čermák
 Author-email: dcermak@suse.com
 Requires-Python: >=3.6.2,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -15,19 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Requires-Dist: cached-property (>=1.5,<2.0) ; python_version < "3.8"
 Requires-Dist: dataclasses (>=0.8) ; python_version < "3.7"
 Requires-Dist: filelock (>=3.4,<4.0)
 Requires-Dist: pytest (>=3.10)
 Requires-Dist: pytest-testinfra (>=6.4.0)
```

