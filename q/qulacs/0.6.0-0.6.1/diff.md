# Comparing `tmp/qulacs-0.6.0.tar.gz` & `tmp/qulacs-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qulacs-0.6.0.tar", last modified: Thu Apr 13 06:42:32 2023, max compression
+gzip compressed data, was "qulacs-0.6.1.tar", last modified: Mon Jun 19 06:38:52 2023, max compression
```

## Comparing `qulacs-0.6.0.tar` & `qulacs-0.6.1.tar`

### file list

```diff
@@ -1,435 +1,450 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.288308 qulacs-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-13 06:41:58.000000 qulacs-0.6.0/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.208310 qulacs-0.6.0/.devcontainer/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.216309 qulacs-0.6.0/.devcontainer/cpu/
--rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-04-13 06:41:58.000000 qulacs-0.6.0/.devcontainer/cpu/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)     2394 2023-04-13 06:41:58.000000 qulacs-0.6.0/.devcontainer/cpu/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.216309 qulacs-0.6.0/.devcontainer/gpu/
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-04-13 06:41:58.000000 qulacs-0.6.0/.devcontainer/gpu/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (122)     2766 2023-04-13 06:41:58.000000 qulacs-0.6.0/.devcontainer/gpu/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.208310 qulacs-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.216309 qulacs-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-04-13 06:41:58.000000 qulacs-0.6.0/.github/workflows/ci_macos.yml
--rw-r--r--   0 runner    (1001) docker     (122)     9050 2023-04-13 06:41:58.000000 qulacs-0.6.0/.github/workflows/ci_ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-04-13 06:41:58.000000 qulacs-0.6.0/.github/workflows/ci_windows.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-04-13 06:41:58.000000 qulacs-0.6.0/.github/workflows/wheel.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-04-13 06:41:58.000000 qulacs-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-04-13 06:41:58.000000 qulacs-0.6.0/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.216309 qulacs-0.6.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-04-13 06:41:58.000000 qulacs-0.6.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (122)    17144 2023-04-13 06:41:58.000000 qulacs-0.6.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2572 2023-04-13 06:41:58.000000 qulacs-0.6.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-04-13 06:41:58.000000 qulacs-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    13054 2023-04-13 06:42:32.288308 qulacs-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11068 2023-04-13 06:41:58.000000 qulacs-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    11431 2023-04-13 06:41:58.000000 qulacs-0.6.0/README_MPI.md
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-13 06:41:58.000000 qulacs-0.6.0/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.220309 qulacs-0.6.0/benchmark/
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/AdaptiveGate.py
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4799 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/bench_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/benchmark2.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/causalconetest.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.220309 qulacs-0.6.0/benchmark/circuits/
--rw-r--r--   0 runner    (1001) docker     (122)      238 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/circuits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3156 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/circuits/quantumvolume.py
--rw-r--r--   0 runner    (1001) docker     (122)     5764 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/circuits/qulacsbench.py
--rw-r--r--   0 runner    (1001) docker     (122)     4625 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/libcppsim_benchmark.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    17638 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/libcsim_benchmark.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/merge_circuit.py
--rw-r--r--   0 runner    (1001) docker     (122)     5914 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/test_qulacs_1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1219 2023-04-13 06:41:58.000000 qulacs-0.6.0/benchmark/test_qulacs_2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.220309 qulacs-0.6.0/cmake_script/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.220309 qulacs-0.6.0/cmake_script/FetchContent/
--rw-r--r--   0 runner    (1001) docker     (122)      831 2023-04-13 06:41:58.000000 qulacs-0.6.0/cmake_script/FetchContent/CMakeLists.cmake.in
--rw-r--r--   0 runner    (1001) docker     (122)    38023 2023-04-13 06:41:58.000000 qulacs-0.6.0/cmake_script/FetchContent.cmake
--rw-r--r--   0 runner    (1001) docker     (122)     1475 2023-04-13 06:41:58.000000 qulacs-0.6.0/cmake_script/FindAVX2.cmake
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-04-13 06:41:58.000000 qulacs-0.6.0/cmake_script/FindSVE.cmake
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.220309 qulacs-0.6.0/doc/
--rw-r--r--   0 runner    (1001) docker     (122)     1935 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.220309 qulacs-0.6.0/doc/en/
--rw-r--r--   0 runner    (1001) docker     (122)      639 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.224309 qulacs-0.6.0/doc/en/source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.208310 qulacs-0.6.0/doc/en/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.224309 qulacs-0.6.0/doc/en/source/_static/images/
--rw-r--r--   0 runner    (1001) docker     (122)     7067 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_static/images/dojo.png
--rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_static/images/github.png
--rw-r--r--   0 runner    (1001) docker     (122)    54241 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_static/images/logo-c-h.png
--rw-r--r--   0 runner    (1001) docker     (122)     2627 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_static/images/slack.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.224309 qulacs-0.6.0/doc/en/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.224309 qulacs-0.6.0/doc/en/source/_templates/autoapi/
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      215 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/macros.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.224309 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/attribute.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2213 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/class.rst
--rw-r--r--   0 runner    (1001) docker     (122)      852 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/data.rst
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/exception.rst
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/function.rst
--rw-r--r--   0 runner    (1001) docker     (122)      704 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/method.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/module.rst
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/package.rst
--rw-r--r--   0 runner    (1001) docker     (122)      338 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/autoapi/python/property.rst
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/_templates/footer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.228309 qulacs-0.6.0/doc/en/source/apply/
--rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/apply/0_overview.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)   162833 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/apply/5.2_qcl.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    30093 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/apply/6.2_vqe.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    55651 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/apply/6.3_ssvqe.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.228309 qulacs-0.6.0/doc/en/source/apply/img/
--rw-r--r--   0 runner    (1001) docker     (122)    59895 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/apply/img/QCL.png
--rw-r--r--   0 runner    (1001) docker     (122)     3953 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.228309 qulacs-0.6.0/doc/en/source/guide/
--rw-r--r--   0 runner    (1001) docker     (122)   151517 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/guide/2.0_python_advanced.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     2132 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.228309 qulacs-0.6.0/doc/en/source/intro/
--rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/intro/0_about.md
--rw-r--r--   0 runner    (1001) docker     (122)     3799 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/intro/1_install.md
--rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/intro/2_faq.md
--rw-r--r--   0 runner    (1001) docker     (122)     2856 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/intro/3_usage.md
--rw-r--r--   0 runner    (1001) docker     (122)    27329 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/intro/4.1_python_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    25763 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/intro/4.2_cpp_tutorial.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.228309 qulacs-0.6.0/doc/en/source/write/
--rw-r--r--   0 runner    (1001) docker     (122)     2574 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/en/source/write/0_readme.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.228309 qulacs-0.6.0/doc/ja/
--rw-r--r--   0 runner    (1001) docker     (122)      639 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.228309 qulacs-0.6.0/doc/ja/source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.208310 qulacs-0.6.0/doc/ja/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.232309 qulacs-0.6.0/doc/ja/source/_static/images/
--rw-r--r--   0 runner    (1001) docker     (122)     7067 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_static/images/dojo.png
--rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_static/images/github.png
--rw-r--r--   0 runner    (1001) docker     (122)    54241 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_static/images/logo-c-h.png
--rw-r--r--   0 runner    (1001) docker     (122)     2627 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_static/images/slack.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.232309 qulacs-0.6.0/doc/ja/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.232309 qulacs-0.6.0/doc/ja/source/_templates/autoapi/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      215 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/macros.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.232309 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/attribute.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2213 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/class.rst
--rw-r--r--   0 runner    (1001) docker     (122)      852 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/data.rst
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/exception.rst
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/function.rst
--rw-r--r--   0 runner    (1001) docker     (122)      704 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/method.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/module.rst
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/package.rst
--rw-r--r--   0 runner    (1001) docker     (122)      338 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/property.rst
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (122)     4006 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.232309 qulacs-0.6.0/doc/ja/source/guide/
--rw-r--r--   0 runner    (1001) docker     (122)    75211 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/guide/2.0_python_advanced.md
--rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/index.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.232309 qulacs-0.6.0/doc/ja/source/intro/
--rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/intro/0_about.md
--rw-r--r--   0 runner    (1001) docker     (122)     3799 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/intro/1_install.md
--rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/intro/2_faq.md
--rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/intro/3_usage.md
--rw-r--r--   0 runner    (1001) docker     (122)    14702 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/intro/4.1_python_tutorial.md
--rw-r--r--   0 runner    (1001) docker     (122)    26305 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/ja/source/intro/4.2_cpp_tutorial.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.236309 qulacs-0.6.0/doc/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)     5920 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/scripts/customdoxygen.css
--rw-r--r--   0 runner    (1001) docker     (122)    10217 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/scripts/doxy-boot.js
--rw-r--r--   0 runner    (1001) docker     (122)      710 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/scripts/footer.html
--rw-r--r--   0 runner    (1001) docker     (122)     3325 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/scripts/header.html
--rw-r--r--   0 runner    (1001) docker     (122)     7954 2023-04-13 06:41:58.000000 qulacs-0.6.0/doc/scripts/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     2456 2023-04-13 06:41:58.000000 qulacs-0.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.212309 qulacs-0.6.0/pysrc/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.236309 qulacs-0.6.0/pysrc/qulacs/
--rw-r--r--   0 runner    (1001) docker     (122)      315 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32351 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-13 06:42:32.000000 qulacs-0.6.0/pysrc/qulacs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.240309 qulacs-0.6.0/pysrc/qulacs/circuit/
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      765 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/circuit/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/circuit/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/circuit.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.240309 qulacs-0.6.0/pysrc/qulacs/converter/
--rw-r--r--   0 runner    (1001) docker     (122)      234 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13118 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/converter/qasm_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.240309 qulacs-0.6.0/pysrc/qulacs/gate/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/gate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10832 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/gate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/gate/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     6526 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/gate.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.240309 qulacs-0.6.0/pysrc/qulacs/observable/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/observable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      771 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/observable/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/observable/_get_matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/observable/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/observable.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.240309 qulacs-0.6.0/pysrc/qulacs/quantum_operator/
--rw-r--r--   0 runner    (1001) docker     (122)       42 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/quantum_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/quantum_operator/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/quantum_operator/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      452 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/quantum_operator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.240309 qulacs-0.6.0/pysrc/qulacs/state/
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2068 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/state/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/state/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     1451 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/state.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.240309 qulacs-0.6.0/pysrc/qulacs/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/utils/conversions_openfermion.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.240309 qulacs-0.6.0/pysrc/qulacs/vistest/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/vistest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1344 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/vistest/test_vis.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.244309 qulacs-0.6.0/pysrc/qulacs/visualizer/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/visualizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-04-13 06:41:58.000000 qulacs-0.6.0/pysrc/qulacs/visualizer/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.236309 qulacs-0.6.0/pysrc/qulacs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    13054 2023-04-13 06:42:32.000000 qulacs-0.6.0/pysrc/qulacs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    11697 2023-04-13 06:42:32.000000 qulacs-0.6.0/pysrc/qulacs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 06:42:32.000000 qulacs-0.6.0/pysrc/qulacs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 06:42:31.000000 qulacs-0.6.0/pysrc/qulacs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-04-13 06:42:32.000000 qulacs-0.6.0/pysrc/qulacs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-13 06:42:32.000000 qulacs-0.6.0/pysrc/qulacs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.244309 qulacs-0.6.0/python/
--rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-04-13 06:41:58.000000 qulacs-0.6.0/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)    71886 2023-04-13 06:41:58.000000 qulacs-0.6.0/python/cppsim_wrapper.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.244309 qulacs-0.6.0/python/stub-test/
--rw-r--r--   0 runner    (1001) docker     (122)     1448 2023-04-13 06:41:58.000000 qulacs-0.6.0/python/stub-test/generate_mypy_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.244309 qulacs-0.6.0/python/test/
--rw-r--r--   0 runner    (1001) docker     (122)    52480 2023-04-13 06:41:58.000000 qulacs-0.6.0/python/test/test_qulacs.py
--rw-r--r--   0 runner    (1001) docker     (122)    36446 2023-04-13 06:41:58.000000 qulacs-0.6.0/python/test/test_qulacs_multicpu.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.248309 qulacs-0.6.0/script/
--rwxr-xr-x   0 runner    (1001) docker     (122)      303 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_clang.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      691 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_gcc.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      440 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_gcc_with_gpu.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      441 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_gcc_with_memory_sanitizer.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      122 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_mpicc.sh
--rw-r--r--   0 runner    (1001) docker     (122)      300 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_msvc_2015.bat
--rw-r--r--   0 runner    (1001) docker     (122)      301 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_msvc_2015_with_gpu.bat
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_msvc_2017.bat
--rw-r--r--   0 runner    (1001) docker     (122)      301 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_msvc_2017_with_gpu.bat
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_msvc_2019.bat
--rw-r--r--   0 runner    (1001) docker     (122)      295 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/build_msvc_2019_with_gpu.bat
--rwxr-xr-x   0 runner    (1001) docker     (122)      127 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/clean.sh
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/download_wheel.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      318 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/fix_wheel_osx.sh
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/generate_msvc_project_2015.bat
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/generate_msvc_project_2015_with_gpu.bat
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/generate_msvc_project_2017.bat
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/generate_msvc_project_2017_with_gpu.bat
--rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/generate_msvc_project_2019.bat
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/generate_msvc_project_2019_with_gpu.bat
--rwxr-xr-x   0 runner    (1001) docker     (122)      436 2023-04-13 06:41:58.000000 qulacs-0.6.0/script/update_stubs.sh
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 06:42:32.288308 qulacs-0.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5235 2023-04-13 06:41:58.000000 qulacs-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.248309 qulacs-0.6.0/src/
--rw-r--r--   0 runner    (1001) docker     (122)      319 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.256309 qulacs-0.6.0/src/cppsim/
--rw-r--r--   0 runner    (1001) docker     (122)      636 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)    20392 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/circuit.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    22387 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/circuit.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      507 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/circuit_builder.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7895 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/circuit_optimizer.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2751 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/circuit_optimizer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     9609 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/exception.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5100 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    10490 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    32399 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_factory.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    19238 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_factory.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    24644 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_general.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    13445 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5783 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     6483 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_matrix_diagonal.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6184 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_matrix_diagonal.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5044 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_matrix_sparse.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5835 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_matrix_sparse.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    20532 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_merge.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6478 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_merge.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5541 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_named_npair.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_named_one.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    16353 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_named_one.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7977 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_named_pauli.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     8986 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_named_two.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    23274 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_noisy_evolution.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    12950 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_noisy_evolution.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_reflect.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2858 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_reversible.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2368 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/gate_to_gqo.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    34378 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/general_quantum_operator.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    14623 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/general_quantum_operator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    14140 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/matrix_decomposition.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7033 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/noisesimulator.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3925 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/noisesimulator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    13716 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/observable.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5966 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/observable.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    14801 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/pauli_operator.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    10673 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/pauli_operator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      830 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/qubit_info.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7181 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/qubit_info.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     2374 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/simulator.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2795 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/simulator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3506 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/state.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    34493 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/state.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5116 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/state_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    16629 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/state_dm.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/state_gpu.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    15703 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/state_gpu.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      913 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/type.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    10550 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/utility.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8184 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/cppsim/utility.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.268308 qulacs-0.6.0/src/csim/
--rw-r--r--   0 runner    (1001) docker     (122)      908 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7145 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/MPIutil.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2336 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/MPIutil.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1107 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/constant.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/constant.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/init_ops.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/init_ops_fill.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3960 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/init_ops_random.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      661 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/memory_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/memory_ops.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/memory_ops_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/memory_ops_dm.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4584 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/stat_ops.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/stat_ops.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    10432 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/stat_ops_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1639 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/stat_ops_dm.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    30440 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/stat_ops_expectation_value.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/stat_ops_probability.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4800 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/stat_ops_transition_amplitude.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/type.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    60932 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     7802 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_control_multi_target_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    14209 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_control_multi_target_single.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5740 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_control_single_target_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    19452 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_control_single_target_single.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2762 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    34691 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3689 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_dm.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    82604 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_matrix_dense_double.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2387 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_matrix_dense_double_eigen.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7071 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_matrix_dense_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6882 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_matrix_dense_multi_eigen.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    17967 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_matrix_dense_single.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3749 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_matrix_diagonal_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    10516 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_matrix_diagonal_single.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_matrix_phase_single.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    12326 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_CNOT.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     7080 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_CZ.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    12677 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_FusedSWAP.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     9614 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_H.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    11477 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_SWAP.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5205 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_X.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     9384 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_Y.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3953 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_Z.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3194 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_projection.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2548 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_named_state.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    16633 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_pauli_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_pauli_single.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2922 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_qft.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      705 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_reflection.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/update_ops_reversible_boolean.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5153 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/utility.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5405 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/csim/utility.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.272308 qulacs-0.6.0/src/gpusim/
--rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     6204 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/memory_ops.cu
--rw-r--r--   0 runner    (1001) docker     (122)      917 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/memory_ops.h
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/memory_ops_device_functions.h
--rw-r--r--   0 runner    (1001) docker     (122)    52450 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/stat_ops.cu
--rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/stat_ops.h
--rw-r--r--   0 runner    (1001) docker     (122)     2709 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/stat_ops_device_functions.h
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/test.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8162 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/update_ops_cuda.h
--rw-r--r--   0 runner    (1001) docker     (122)     5285 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/update_ops_cuda_device_functions.h
--rw-r--r--   0 runner    (1001) docker     (122)    69614 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/update_ops_multi.cu
--rw-r--r--   0 runner    (1001) docker     (122)    21139 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/update_ops_named.cu
--rw-r--r--   0 runner    (1001) docker     (122)    15186 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/update_ops_single.cu
--rw-r--r--   0 runner    (1001) docker     (122)    24389 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/util.cu
--rw-r--r--   0 runner    (1001) docker     (122)     2806 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/util.cuh
--rw-r--r--   0 runner    (1001) docker     (122)     2201 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/util.h
--rw-r--r--   0 runner    (1001) docker     (122)      517 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/util_common.h
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/util_export.h
--rw-r--r--   0 runner    (1001) docker     (122)     2713 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/util_func.h
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/util_type.h
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/gpusim/util_type_internal.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.276308 qulacs-0.6.0/src/vqcsim/
--rw-r--r--   0 runner    (1001) docker     (122)      372 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1910 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/GradCalculator.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      408 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/GradCalculator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      730 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/boolean_formula.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     8079 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/causalcone_simulator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1353 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/differential.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      788 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/differential.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/loss_function.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      547 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/loss_function.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     3015 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/optimizer.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    13788 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/parametric_circuit.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3267 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/parametric_circuit.hpp
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/parametric_circuit_builder.hpp
--rw-r--r--   0 runner    (1001) docker     (122)    10288 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/parametric_gate.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4677 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/parametric_gate_factory.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      823 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/parametric_gate_factory.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     1020 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/parametric_simulator.cpp
--rw-r--r--   0 runner    (1001) docker     (122)      603 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/parametric_simulator.hpp
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/parser.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     4262 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/problem.hpp
--rw-r--r--   0 runner    (1001) docker     (122)     5367 2023-04-13 06:41:58.000000 qulacs-0.6.0/src/vqcsim/solver.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.276308 qulacs-0.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.280308 qulacs-0.6.0/test/cppsim/
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)      450 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/H2.txt
--rw-r--r--   0 runner    (1001) docker     (122)      274 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/main.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_KAK.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    30583 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_circuit.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    32800 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_circuit_multicpu.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     9942 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_circuit_optimize_light.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    55264 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_gate.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    29782 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_gate_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    57226 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_gate_multicpu.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    21214 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_hamiltonian.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5465 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_hamiltonian_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    15636 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_hamiltonian_multicpu.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_mpiutil_multicpu.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    12025 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_noise_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5334 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_noisesimulator.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    20963 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_noisyevolution.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6242 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_pauli_operator.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2973 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_simulator.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    11552 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_state.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    11267 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_state_dm.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5685 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/cppsim/test_state_multicpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.284308 qulacs-0.6.0/test/csim/
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)      274 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/main.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1206 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_memory.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_omputil.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    26768 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_stat.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    10235 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_update_control.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     5793 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_update_dense.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3594 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_update_dense_double.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3458 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_update_diagonal.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6761 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_update_diagonal_multi.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    13376 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_update_named.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     6955 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/csim/test_update_pauli.cpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.288308 qulacs-0.6.0/test/gpusim/
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/H2.txt
--rw-r--r--   0 runner    (1001) docker     (122)    33345 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_circuit.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     9054 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_compat_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     2249 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_func_memory.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    47172 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_gate.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     9409 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_hamiltonian.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    43543 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_state.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8633 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_update_control.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    15382 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_update_dense.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     3689 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_update_diagonal.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    10371 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_update_named.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     8491 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_update_pauli.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/gpusim/test_util.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.288308 qulacs-0.6.0/test/util/
--rw-r--r--   0 runner    (1001) docker     (122)    13090 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/util/util.hpp
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 06:42:32.288308 qulacs-0.6.0/test/vqcsim/
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/vqcsim/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)      274 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/vqcsim/main.cpp
--rw-r--r--   0 runner    (1001) docker     (122)    15642 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/vqcsim/test.cpp
--rw-r--r--   0 runner    (1001) docker     (122)     4767 2023-04-13 06:41:58.000000 qulacs-0.6.0/test/vqcsim/test_backprop.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.780336 qulacs-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-06-19 06:38:18.000000 qulacs-0.6.1/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.720335 qulacs-0.6.1/.devcontainer/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.728335 qulacs-0.6.1/.devcontainer/cpu/
+-rw-r--r--   0 runner    (1001) docker     (122)     1015 2023-06-19 06:38:18.000000 qulacs-0.6.1/.devcontainer/cpu/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)     2612 2023-06-19 06:38:18.000000 qulacs-0.6.1/.devcontainer/cpu/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.728335 qulacs-0.6.1/.devcontainer/gpu/
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-06-19 06:38:18.000000 qulacs-0.6.1/.devcontainer/gpu/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (122)     2994 2023-06-19 06:38:18.000000 qulacs-0.6.1/.devcontainer/gpu/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.720335 qulacs-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.728335 qulacs-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-06-19 06:38:18.000000 qulacs-0.6.1/.github/workflows/ci_macos.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     8777 2023-06-19 06:38:18.000000 qulacs-0.6.1/.github/workflows/ci_ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-06-19 06:38:18.000000 qulacs-0.6.1/.github/workflows/ci_windows.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3934 2023-06-19 06:38:18.000000 qulacs-0.6.1/.github/workflows/wheel.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-06-19 06:38:18.000000 qulacs-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-06-19 06:38:18.000000 qulacs-0.6.1/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.728335 qulacs-0.6.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (122)     1956 2023-06-19 06:38:18.000000 qulacs-0.6.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (122)    16675 2023-06-19 06:38:18.000000 qulacs-0.6.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2572 2023-06-19 06:38:18.000000 qulacs-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-06-19 06:38:18.000000 qulacs-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    13054 2023-06-19 06:38:52.780336 qulacs-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    11068 2023-06-19 06:38:18.000000 qulacs-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11431 2023-06-19 06:38:18.000000 qulacs-0.6.1/README_MPI.md
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-19 06:38:18.000000 qulacs-0.6.1/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.732335 qulacs-0.6.1/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (122)      564 2023-06-19 06:38:18.000000 qulacs-0.6.1/benchmark/AdaptiveGate.py
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-06-19 06:38:18.000000 qulacs-0.6.1/benchmark/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-06-19 06:38:18.000000 qulacs-0.6.1/benchmark/bench_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-06-19 06:38:18.000000 qulacs-0.6.1/benchmark/benchmark2.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-06-19 06:38:18.000000 qulacs-0.6.1/benchmark/causalconetest.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.732335 qulacs-0.6.1/benchmark/circuits/
+-rw-r--r--   0 runner    (1001) docker     (122)      239 2023-06-19 06:38:18.000000 qulacs-0.6.1/benchmark/circuits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3445 2023-06-19 06:38:18.000000 qulacs-0.6.1/benchmark/circuits/quantumvolume.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6270 2023-06-19 06:38:18.000000 qulacs-0.6.1/benchmark/circuits/qulacsbench.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4625 2023-06-19 06:38:18.000000 qulacs-0.6.1/benchmark/libcppsim_benchmark.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    17638 2023-06-19 06:38:18.000000 qulacs-0.6.1/benchmark/libcsim_benchmark.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-06-19 06:38:18.000000 qulacs-0.6.1/benchmark/merge_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6060 2023-06-19 06:38:18.000000 qulacs-0.6.1/benchmark/test_qulacs_1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1345 2023-06-19 06:38:18.000000 qulacs-0.6.1/benchmark/test_qulacs_2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.732335 qulacs-0.6.1/cmake_script/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.732335 qulacs-0.6.1/cmake_script/FetchContent/
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-06-19 06:38:18.000000 qulacs-0.6.1/cmake_script/FetchContent/CMakeLists.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (122)    38023 2023-06-19 06:38:18.000000 qulacs-0.6.1/cmake_script/FetchContent.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)     1475 2023-06-19 06:38:18.000000 qulacs-0.6.1/cmake_script/FindAVX2.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-06-19 06:38:18.000000 qulacs-0.6.1/cmake_script/FindSVE.cmake
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-19 06:38:18.000000 qulacs-0.6.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.732335 qulacs-0.6.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (122)     1935 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.732335 qulacs-0.6.1/doc/en/
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.732335 qulacs-0.6.1/doc/en/source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.724335 qulacs-0.6.1/doc/en/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.732335 qulacs-0.6.1/doc/en/source/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (122)     7067 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/_static/images/dojo.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/_static/images/github.png
+-rw-r--r--   0 runner    (1001) docker     (122)    54241 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/_static/images/logo-c-h.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2627 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/_static/images/slack.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.732335 qulacs-0.6.1/doc/en/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.732335 qulacs-0.6.1/doc/en/source/_templates/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/_templates/autoapi/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/_templates/autoapi/macros.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.732335 qulacs-0.6.1/doc/en/source/_templates/autoapi/python/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/_templates/autoapi/python/attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2213 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/_templates/autoapi/python/class.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/_templates/autoapi/python/data.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/_templates/autoapi/python/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/_templates/autoapi/python/function.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/_templates/autoapi/python/method.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/_templates/autoapi/python/module.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/_templates/autoapi/python/package.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      338 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/_templates/autoapi/python/property.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/_templates/footer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.736335 qulacs-0.6.1/doc/en/source/apply/
+-rw-r--r--   0 runner    (1001) docker     (122)     1143 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/apply/0_overview.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)   162833 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/apply/5.2_qcl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    30093 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/apply/6.2_vqe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    55651 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/apply/6.3_ssvqe.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.736335 qulacs-0.6.1/doc/en/source/apply/img/
+-rw-r--r--   0 runner    (1001) docker     (122)    59895 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/apply/img/QCL.png
+-rw-r--r--   0 runner    (1001) docker     (122)     3953 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.736335 qulacs-0.6.1/doc/en/source/guide/
+-rw-r--r--   0 runner    (1001) docker     (122)   156635 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/guide/2.0_python_advanced.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)     2132 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.736335 qulacs-0.6.1/doc/en/source/intro/
+-rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/intro/0_about.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3799 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/intro/1_install.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/intro/2_faq.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2856 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/intro/3_usage.md
+-rw-r--r--   0 runner    (1001) docker     (122)    27329 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/intro/4.1_python_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)    25763 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/intro/4.2_cpp_tutorial.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.736335 qulacs-0.6.1/doc/en/source/write/
+-rw-r--r--   0 runner    (1001) docker     (122)     2574 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/en/source/write/0_readme.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.736335 qulacs-0.6.1/doc/ja/
+-rw-r--r--   0 runner    (1001) docker     (122)      639 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.736335 qulacs-0.6.1/doc/ja/source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.724335 qulacs-0.6.1/doc/ja/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.736335 qulacs-0.6.1/doc/ja/source/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (122)     7067 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/_static/images/dojo.png
+-rw-r--r--   0 runner    (1001) docker     (122)     4268 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/_static/images/github.png
+-rw-r--r--   0 runner    (1001) docker     (122)    54241 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/_static/images/logo-c-h.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2627 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/_static/images/slack.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.736335 qulacs-0.6.1/doc/ja/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.736335 qulacs-0.6.1/doc/ja/source/_templates/autoapi/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/_templates/autoapi/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/_templates/autoapi/macros.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.740335 qulacs-0.6.1/doc/ja/source/_templates/autoapi/python/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/_templates/autoapi/python/attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2213 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/_templates/autoapi/python/class.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      852 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/_templates/autoapi/python/data.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/_templates/autoapi/python/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/_templates/autoapi/python/function.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/_templates/autoapi/python/method.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/_templates/autoapi/python/module.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/_templates/autoapi/python/package.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      338 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/_templates/autoapi/python/property.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3966 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.740335 qulacs-0.6.1/doc/ja/source/guide/
+-rw-r--r--   0 runner    (1001) docker     (122)    77805 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/guide/2.0_python_advanced.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/index.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.740335 qulacs-0.6.1/doc/ja/source/intro/
+-rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/intro/0_about.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3799 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/intro/1_install.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2017 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/intro/2_faq.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/intro/3_usage.md
+-rw-r--r--   0 runner    (1001) docker     (122)    14702 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/intro/4.1_python_tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (122)    26305 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/ja/source/intro/4.2_cpp_tutorial.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.740335 qulacs-0.6.1/doc/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)     5920 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/scripts/customdoxygen.css
+-rw-r--r--   0 runner    (1001) docker     (122)    10217 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/scripts/doxy-boot.js
+-rw-r--r--   0 runner    (1001) docker     (122)      710 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/scripts/footer.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3325 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/scripts/header.html
+-rw-r--r--   0 runner    (1001) docker     (122)     7954 2023-06-19 06:38:18.000000 qulacs-0.6.1/doc/scripts/index.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2740 2023-06-19 06:38:18.000000 qulacs-0.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.724335 qulacs-0.6.1/pysrc/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.740335 qulacs-0.6.1/pysrc/qulacs/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32506 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-19 06:38:52.000000 qulacs-0.6.1/pysrc/qulacs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.744336 qulacs-0.6.1/pysrc/qulacs/circuit/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/circuit/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/circuit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      444 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/circuit.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.744336 qulacs-0.6.1/pysrc/qulacs/converter/
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13126 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/converter/qasm_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.744336 qulacs-0.6.1/pysrc/qulacs/gate/
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/gate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10986 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/gate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/gate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     6763 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/gate.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.744336 qulacs-0.6.1/pysrc/qulacs/observable/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/observable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/observable/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/observable/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/observable.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.744336 qulacs-0.6.1/pysrc/qulacs/quantum_operator/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/quantum_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/quantum_operator/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/quantum_operator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      474 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/quantum_operator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.744336 qulacs-0.6.1/pysrc/qulacs/state/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2175 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/state/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/state/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/state.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.744336 qulacs-0.6.1/pysrc/qulacs/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1473 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/utils/conversions_openfermion.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.744336 qulacs-0.6.1/pysrc/qulacs/vistest/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/vistest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1311 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/vistest/test_vis.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.744336 qulacs-0.6.1/pysrc/qulacs/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/visualizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3068 2023-06-19 06:38:18.000000 qulacs-0.6.1/pysrc/qulacs/visualizer/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.740335 qulacs-0.6.1/pysrc/qulacs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    13054 2023-06-19 06:38:52.000000 qulacs-0.6.1/pysrc/qulacs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    12202 2023-06-19 06:38:52.000000 qulacs-0.6.1/pysrc/qulacs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 06:38:52.000000 qulacs-0.6.1/pysrc/qulacs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 06:38:52.000000 qulacs-0.6.1/pysrc/qulacs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-06-19 06:38:52.000000 qulacs-0.6.1/pysrc/qulacs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-19 06:38:52.000000 qulacs-0.6.1/pysrc/qulacs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.744336 qulacs-0.6.1/python/
+-rw-r--r--   0 runner    (1001) docker     (122)     3010 2023-06-19 06:38:18.000000 qulacs-0.6.1/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    72023 2023-06-19 06:38:18.000000 qulacs-0.6.1/python/cppsim_wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.744336 qulacs-0.6.1/python/stub-test/
+-rw-r--r--   0 runner    (1001) docker     (122)     1448 2023-06-19 06:38:18.000000 qulacs-0.6.1/python/stub-test/generate_mypy_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.744336 qulacs-0.6.1/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:18.000000 qulacs-0.6.1/python/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.744336 qulacs-0.6.1/python/tests/multi_cpu/
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-06-19 06:38:18.000000 qulacs-0.6.1/python/tests/multi_cpu/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2122 2023-06-19 06:38:18.000000 qulacs-0.6.1/python/tests/multi_cpu/test_state_multi_cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.748335 qulacs-0.6.1/python/tests/single_cpu/
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-06-19 06:38:18.000000 qulacs-0.6.1/python/tests/single_cpu/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      876 2023-06-19 06:38:18.000000 qulacs-0.6.1/python/tests/single_cpu/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6064 2023-06-19 06:38:18.000000 qulacs-0.6.1/python/tests/single_cpu/test_density_matrix_handling.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12303 2023-06-19 06:38:18.000000 qulacs-0.6.1/python/tests/single_cpu/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4464 2023-06-19 06:38:18.000000 qulacs-0.6.1/python/tests/single_cpu/test_noise_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1698 2023-06-19 06:38:18.000000 qulacs-0.6.1/python/tests/single_cpu/test_observable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2883 2023-06-19 06:38:18.000000 qulacs-0.6.1/python/tests/single_cpu/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17686 2023-06-19 06:38:18.000000 qulacs-0.6.1/python/tests/single_cpu/test_pointer_handling.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3137 2023-06-19 06:38:18.000000 qulacs-0.6.1/python/tests/single_cpu/test_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1071 2023-06-19 06:38:18.000000 qulacs-0.6.1/python/tests/single_cpu/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-06-19 06:38:18.000000 qulacs-0.6.1/python/tests/single_cpu/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.748335 qulacs-0.6.1/script/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      303 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/build_clang.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      691 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/build_gcc.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      440 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/build_gcc_with_gpu.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      441 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/build_gcc_with_memory_sanitizer.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      122 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/build_mpicc.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      300 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/build_msvc_2015.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      301 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/build_msvc_2015_with_gpu.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/build_msvc_2017.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      301 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/build_msvc_2017_with_gpu.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/build_msvc_2019.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/build_msvc_2019_with_gpu.bat
+-rwxr-xr-x   0 runner    (1001) docker     (122)      127 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/clean.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/download_wheel.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      318 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/fix_wheel_osx.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      141 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/format.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/generate_msvc_project_2015.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/generate_msvc_project_2015_with_gpu.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/generate_msvc_project_2017.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/generate_msvc_project_2017_with_gpu.bat
+-rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/generate_msvc_project_2019.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/generate_msvc_project_2019_with_gpu.bat
+-rwxr-xr-x   0 runner    (1001) docker     (122)      512 2023-06-19 06:38:18.000000 qulacs-0.6.1/script/update_stubs.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-19 06:38:52.780336 qulacs-0.6.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5242 2023-06-19 06:38:18.000000 qulacs-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.752335 qulacs-0.6.1/src/
+-rw-r--r--   0 runner    (1001) docker     (122)      319 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.756336 qulacs-0.6.1/src/cppsim/
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    20392 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/circuit.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    22387 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/circuit.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/circuit_builder.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7895 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/circuit_optimizer.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2751 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/circuit_optimizer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9609 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/exception.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5100 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10490 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    32399 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_factory.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    19238 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_factory.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    24644 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_general.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13445 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5783 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6483 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_matrix_diagonal.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6184 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_matrix_diagonal.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5044 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_matrix_sparse.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5835 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_matrix_sparse.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    20532 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_merge.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6478 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_merge.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5541 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_named_npair.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_named_one.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    16353 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_named_one.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7977 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_named_pauli.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8986 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_named_two.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    23274 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_noisy_evolution.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    12950 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_noisy_evolution.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_reflect.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2858 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_reversible.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2368 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/gate_to_gqo.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    36921 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/general_quantum_operator.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14781 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/general_quantum_operator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14140 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/matrix_decomposition.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7033 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/noisesimulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3925 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/noisesimulator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13716 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/observable.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5966 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/observable.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14801 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/pauli_operator.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10673 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/pauli_operator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/qubit_info.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7181 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/qubit_info.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2374 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/simulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2795 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/simulator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3506 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/state.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    34493 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/state.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5116 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/state_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    16629 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/state_dm.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/state_gpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    15703 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/state_gpu.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1001 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/type.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10550 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/utility.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8184 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/cppsim/utility.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.764336 qulacs-0.6.1/src/csim/
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7145 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/MPIutil.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2336 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/MPIutil.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1107 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/constant.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1439 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/constant.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/init_ops.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/init_ops_fill.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3960 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/init_ops_random.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      661 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/memory_ops.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/memory_ops.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/memory_ops_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/memory_ops_dm.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4584 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/stat_ops.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/stat_ops.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10432 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/stat_ops_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1639 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/stat_ops_dm.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    30440 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/stat_ops_expectation_value.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3355 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/stat_ops_probability.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4800 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/stat_ops_transition_amplitude.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/type.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    60932 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7802 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_control_multi_target_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    14209 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_control_multi_target_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5740 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_control_single_target_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    19452 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_control_single_target_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2762 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    34691 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3689 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_dm.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    82604 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_matrix_dense_double.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2387 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_matrix_dense_double_eigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7071 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_matrix_dense_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6882 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_matrix_dense_multi_eigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    17967 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_matrix_dense_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3749 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_matrix_diagonal_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10516 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_matrix_diagonal_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_matrix_phase_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_named.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    12326 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_named_CNOT.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     7080 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_named_CZ.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    12677 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_named_FusedSWAP.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9614 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_named_H.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11477 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_named_SWAP.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5205 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_named_X.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9384 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_named_Y.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3953 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_named_Z.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3194 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_named_projection.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2548 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_named_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    16633 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_pauli_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3876 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_pauli_single.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2922 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_qft.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      705 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_reflection.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/update_ops_reversible_boolean.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5153 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/utility.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5405 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/csim/utility.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.768336 qulacs-0.6.1/src/gpusim/
+-rw-r--r--   0 runner    (1001) docker     (122)     1144 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     6130 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/memory_ops.cu
+-rw-r--r--   0 runner    (1001) docker     (122)      917 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/memory_ops.h
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/memory_ops_device_functions.h
+-rw-r--r--   0 runner    (1001) docker     (122)    52450 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/stat_ops.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     3692 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/stat_ops.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2709 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/stat_ops_device_functions.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8162 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/update_ops_cuda.h
+-rw-r--r--   0 runner    (1001) docker     (122)     5285 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/update_ops_cuda_device_functions.h
+-rw-r--r--   0 runner    (1001) docker     (122)    69614 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/update_ops_multi.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    21139 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/update_ops_named.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    15186 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/update_ops_single.cu
+-rw-r--r--   0 runner    (1001) docker     (122)    24452 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/util.cu
+-rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/util.cuh
+-rw-r--r--   0 runner    (1001) docker     (122)     2201 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/util.h
+-rw-r--r--   0 runner    (1001) docker     (122)      517 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/util_common.h
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/util_export.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2713 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/util_func.h
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/util_type.h
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/gpusim/util_type_internal.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.772336 qulacs-0.6.1/src/vqcsim/
+-rw-r--r--   0 runner    (1001) docker     (122)      372 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1910 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/GradCalculator.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      408 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/GradCalculator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/boolean_formula.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8079 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/causalcone_simulator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1353 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/differential.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      788 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/differential.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/loss_function.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      547 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/loss_function.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3015 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/optimizer.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13788 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/parametric_circuit.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3267 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/parametric_circuit.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/parametric_circuit_builder.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10288 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/parametric_gate.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4677 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/parametric_gate_factory.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      823 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/parametric_gate_factory.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1020 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/parametric_simulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)      603 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/parametric_simulator.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/parser.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4262 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/problem.hpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5367 2023-06-19 06:38:18.000000 qulacs-0.6.1/src/vqcsim/solver.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.772336 qulacs-0.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.776336 qulacs-0.6.1/test/cppsim/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      450 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/H2.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/test_KAK.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    30583 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/test_circuit.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    32800 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/test_circuit_multicpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9942 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/test_circuit_optimize_light.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    55264 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/test_gate.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    29782 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/test_gate_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    57226 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/test_gate_multicpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    23845 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/test_hamiltonian.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5465 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/test_hamiltonian_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    15636 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/test_hamiltonian_multicpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5357 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/test_mpiutil_multicpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    12025 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/test_noise_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5334 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/test_noisesimulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    20764 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/test_noisyevolution.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6242 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/test_pauli_operator.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2973 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/test_simulator.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11552 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/test_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    11267 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/test_state_dm.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5685 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/cppsim/test_state_multicpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.776336 qulacs-0.6.1/test/csim/
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/csim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/csim/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1206 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/csim/test_memory.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/csim/test_omputil.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    26768 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/csim/test_stat.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10235 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/csim/test_update_control.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     5793 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/csim/test_update_dense.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3594 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/csim/test_update_dense_double.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3458 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/csim/test_update_diagonal.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6761 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/csim/test_update_diagonal_multi.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    13376 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/csim/test_update_named.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     6955 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/csim/test_update_pauli.cpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.780336 qulacs-0.6.1/test/gpusim/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/gpusim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/gpusim/H2.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    33345 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/gpusim/test_circuit.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9054 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/gpusim/test_compat_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     2249 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/gpusim/test_func_memory.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    47172 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/gpusim/test_gate.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     9409 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/gpusim/test_hamiltonian.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    43543 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/gpusim/test_state.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8633 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/gpusim/test_update_control.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    15382 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/gpusim/test_update_dense.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     3689 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/gpusim/test_update_diagonal.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    10371 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/gpusim/test_update_named.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     8491 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/gpusim/test_update_pauli.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/gpusim/test_util.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.780336 qulacs-0.6.1/test/util/
+-rw-r--r--   0 runner    (1001) docker     (122)    13090 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/util/util.hpp
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 06:38:52.780336 qulacs-0.6.1/test/vqcsim/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/vqcsim/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      274 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/vqcsim/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)    15642 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/vqcsim/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (122)     4767 2023-06-19 06:38:18.000000 qulacs-0.6.1/test/vqcsim/test_backprop.cpp
```

### Comparing `qulacs-0.6.0/.devcontainer/cpu/Dockerfile` & `qulacs-0.6.1/.devcontainer/cpu/Dockerfile`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/.devcontainer/cpu/devcontainer.json` & `qulacs-0.6.1/.devcontainer/gpu/devcontainer.json`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,73 @@
 // For format details, see https://aka.ms/devcontainer.json. For config options, see the README at:
 // https://github.com/microsoft/vscode-dev-containers/tree/v0.209.6/containers/cpp
 {
-	"name": "CPU Environment",
+	"name": "GPU(CUDA) Environment",
 	"build": {
 		"dockerfile": "Dockerfile",
 	},
 	"runArgs": [
 		"--cap-add=SYS_PTRACE",
 		"--security-opt",
-		"seccomp=unconfined"
+		"seccomp=unconfined",
+		"--gpus",
+		"all"
 	],
 	// Set *default* container specific settings.json values on container create.
 	"customizations": {
 		"vscode": {
 			"settings": {
-				"python.linting.enabled": true,
-				"python.linting.pylintEnabled": false,
-				"python.linting.flake8Enabled": true,
-				"python.formatting.provider": "black",
 				"editor.formatOnSave": true,
 				"editor.codeActionsOnSave": {
 					"source.organizeImports": true
 				},
-				"editor.defaultFormatter": "xaver.clang-format",
+				"[python]": {
+					"editor.defaultFormatter": "ms-python.black-formatter"
+				},
+				"python.linting.enabled": true,
+				"python.linting.pylintEnabled": false,
+				"python.linting.flake8Enabled": true,
+				"python.formatting.provider": "none", // use ms-python.black-formatter
 				"python.linting.mypyEnabled": true,
 				"python.terminal.activateEnvironment": false,
+				"[cpp]": {
+					"editor.defaultFormatter": "xaver.clang-format"
+				},
 				// CAVEAT: you need to restart after building qulacs to take effect.
 				"C_Cpp.default.includePath": [
 					"include",
 					"/usr/local/include/python3.9"
+				],
+				// To highlight GPU code in VSCode.
+				"C_Cpp.default.defines": [
+					"_USE_GPU"
 				]
 			},
 			// Add the IDs of extensions you want installed when the container is created.
 			"extensions": [
 				"ms-vscode.cpptools",
 				"ms-vscode.cmake-tools",
 				"ms-python.python",
 				"ms-python.vscode-pylance",
+				"ms-python.black-formatter",
+				"ms-python.isort",
+				"ms-python.flake8",
 				"xaver.clang-format"
 			]
 		}
 	},
-
+	"features": {
+		"ghcr.io/devcontainers/features/common-utils:2": {
+			// Following settings create a user whose uid and gid are the same as the host ones.
+			"username": "automatic",
+			"uid": "automatic",
+			"gid": "automatic",
+			"installZsh": true
+		},
+	},
 	// Required by `mounts`.
 	// c.f. https://code.visualstudio.com/remote/advancedcontainers/improve-performance#_use-a-targeted-named-volume
 	"workspaceMount": "source=${localWorkspaceFolder},target=/workspaces/qulacs,type=bind,consistency=cached",
 	"workspaceFolder": "/workspaces/qulacs",
 	"mounts": [
 		"source=${localWorkspaceFolderBasename}-build,target=${containerWorkspaceFolder}/build,type=volume"
 	],
```

### Comparing `qulacs-0.6.0/.devcontainer/gpu/Dockerfile` & `qulacs-0.6.1/.devcontainer/gpu/Dockerfile`

 * *Files 17% similar despite different names*

```diff
@@ -25,9 +25,11 @@
     pandoc \
     python3 \
     python3-distutils \
     python3-pip \
     wget \
     && apt-get autoremove -y && apt-get clean -y && rm -rf /var/lib/apt/lists/*
 
+RUN ln -s /usr/bin/python3 /usr/bin/python
+
 RUN pip install -U pip \
     && pip install black flake8 openfermion mypy pybind11-stubgen
```

### Comparing `qulacs-0.6.0/.devcontainer/gpu/devcontainer.json` & `qulacs-0.6.1/.devcontainer/cpu/devcontainer.json`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,58 @@
 // For format details, see https://aka.ms/devcontainer.json. For config options, see the README at:
 // https://github.com/microsoft/vscode-dev-containers/tree/v0.209.6/containers/cpp
 {
-	"name": "GPU(CUDA) Environment",
+	"name": "CPU Environment",
 	"build": {
 		"dockerfile": "Dockerfile",
 	},
 	"runArgs": [
 		"--cap-add=SYS_PTRACE",
 		"--security-opt",
-		"seccomp=unconfined",
-		"--gpus",
-		"all"
+		"seccomp=unconfined"
 	],
 	// Set *default* container specific settings.json values on container create.
 	"customizations": {
 		"vscode": {
 			"settings": {
-				"python.linting.enabled": true,
-				"python.linting.pylintEnabled": false,
-				"python.linting.flake8Enabled": true,
-				"python.formatting.provider": "black",
 				"editor.formatOnSave": true,
 				"editor.codeActionsOnSave": {
 					"source.organizeImports": true
 				},
-				"editor.defaultFormatter": "xaver.clang-format",
+				"[python]": {
+					"editor.defaultFormatter": "ms-python.black-formatter"
+				},
+				"python.linting.enabled": true,
+				"python.linting.pylintEnabled": false,
+				"python.linting.flake8Enabled": true,
+				"python.formatting.provider": "none", // use ms-python.black-formatter
 				"python.linting.mypyEnabled": true,
 				"python.terminal.activateEnvironment": false,
+				"[cpp]": {
+					"editor.defaultFormatter": "xaver.clang-format"
+				},
 				// CAVEAT: you need to restart after building qulacs to take effect.
 				"C_Cpp.default.includePath": [
 					"include",
 					"/usr/local/include/python3.9"
-				],
-				// To highlight GPU code in VSCode.
-				"C_Cpp.default.defines": ["_USE_GPU"]
+				]
 			},
 			// Add the IDs of extensions you want installed when the container is created.
 			"extensions": [
 				"ms-vscode.cpptools",
 				"ms-vscode.cmake-tools",
 				"ms-python.python",
 				"ms-python.vscode-pylance",
+				"ms-python.black-formatter",
+				"ms-python.isort",
+				"ms-python.flake8",
 				"xaver.clang-format"
 			]
 		}
 	},
-
-	"features": {
-		"ghcr.io/devcontainers/features/common-utils:2": {
-			// Following settings create a user whose uid and gid are the same as the host ones.
-			"username": "automatic",
-			"uid": "automatic",
-			"gid": "automatic",
-			"installZsh": true
-		},
-	},
-
 	// Required by `mounts`.
 	// c.f. https://code.visualstudio.com/remote/advancedcontainers/improve-performance#_use-a-targeted-named-volume
 	"workspaceMount": "source=${localWorkspaceFolder},target=/workspaces/qulacs,type=bind,consistency=cached",
 	"workspaceFolder": "/workspaces/qulacs",
 	"mounts": [
 		"source=${localWorkspaceFolderBasename}-build,target=${containerWorkspaceFolder}/build,type=volume"
 	],
```

### Comparing `qulacs-0.6.0/.github/workflows/ci_macos.yml` & `qulacs-0.6.1/.github/workflows/ci_macos.yml`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/.github/workflows/ci_ubuntu.yml` & `qulacs-0.6.1/.github/workflows/ci_ubuntu.yml`

 * *Files 23% similar despite different names*

```diff
@@ -55,15 +55,15 @@
           sudo make install
 
       - name: Install qulacs for Ubuntu
         run: ./script/build_gcc.sh
 
       - name: Install qulacs Python module
         run: pip install .[ci]
-      
+
       - name: Check stubs
         run: |
           ./script/update_stubs.sh
           diff=$(git diff)
           echo -n "$diff"
           # Without `-n`, `echo -n "$diff" | wc -l` is 1 even if `"$diff" is empty.`
           test $(echo -n "$diff" | wc -l) -eq 0
@@ -203,46 +203,54 @@
           file ../bin/vqcsim_test
           QEMU_CPU="max,sve512=on" qemu-aarch64 ../bin/vqcsim_test
           QEMU_CPU="max,sve256=on" qemu-aarch64 ../bin/vqcsim_test
 
   format:
     name: Format with clang-format
     runs-on: "ubuntu-20.04"
-    container:
-      image: ghcr.io/qulacs-osaka/qulacs-ubuntu-clang-format:latest
     steps:
-      # This job is running on a docker container.
-      # We can't use actions/checkout because Node.js is not installed on the container.
-      # Therefore, we use `git clone` instead of actions/checkout.
-      - name: clone /qulacs (pull_request)
-        if: ${{ github.event_name == 'pull_request' }}
-        env:
-          # We use $REPOSITORY to support PR from the forked repository of Qulacs/qulacs.
-          REPOSITORY: ${{ github.event.pull_request.head.repo.full_name }}
-        run: |
-          cd /
-          git clone -b "${GITHUB_HEAD_REF#refs/*/}" https://github.com/$REPOSITORY
+      - uses: actions/checkout@v3
 
-      - name: clone /qulacs (push)
-        if: ${{ github.event_name == 'push' }}
-        run: |
-          cd /
-          git clone -b "${GITHUB_REF#refs/*/}" https://github.com/${GITHUB_REPOSITORY}
+      - run: sudo apt install clang-format=1:10.0-50~exp1
 
       - name: format
-        run: qulacs_format
+        run: |
+          ./script/format.sh
 
       - name: Compare diff
         run: |
-          cd /qulacs
           diff=$(git diff)
           echo -n "$diff"
           # Without `-n`, `echo -n "$diff" | wc -l` is 1 even if `"$diff" is empty.`
           test $(echo -n "$diff" | wc -l) -eq 0
 
+  python-format:
+    name: Format with Python formatters
+    runs-on: "ubuntu-20.04"
+    strategy:
+      matrix:
+        python-version: ["3.10"]
+
+    steps:
+      - uses: actions/checkout@v3
+
+      - name: Setup Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: ${{ matrix.python-version }}
+          architecture: x64
+
+      - name: Install formatters
+        run: pip install black isort
+
+      - name: Check format
+        run: |
+          black . --check --diff
+          isort . --check --diff
+
   mpicc-build:
     name: MPICC build
     strategy:
       matrix:
         python-version: ["3.7.5"]
     runs-on: "ubuntu-20.04"
     env:
@@ -303,11 +311,11 @@
           make coverage
           make pythontest
 
       - name: Test in Ubuntu
         run: |
           pip install pytest
           mpirun -n 2 bin/cppsim_test --gtest_filter="*multicpu*"
-          mpirun -n 2 pytest python/test/test_qulacs_multicpu.py
+          mpirun -n 2 pytest python/tests/multi_cpu
 
       - name: Upload coverage to codecov
         uses: codecov/codecov-action@v3
```

### Comparing `qulacs-0.6.0/.github/workflows/ci_windows.yml` & `qulacs-0.6.1/.github/workflows/ci_windows.yml`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/.github/workflows/wheel.yml` & `qulacs-0.6.1/.github/workflows/wheel.yml`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/.gitignore` & `qulacs-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/.vscode/tasks.json` & `qulacs-0.6.1/.vscode/tasks.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9708333333333333%*

 * *Differences: {"'tasks'": "{6: {'command': 'script/format.sh'}, insert: [(7, OrderedDict([('label', 'python "*

 * *            "format'), ('type', 'shell'), ('command', 'black . && isort .')]))]}"}*

```diff
@@ -39,19 +39,24 @@
             "dependsOn": [
                 "build gcc"
             ],
             "label": "install",
             "type": "shell"
         },
         {
-            "command": "find ./src ./test ./benchmark ./python -regex '.*\\.\\(cu\\|cuh\\|cpp\\|h\\|hpp\\)' -exec clang-format -style=file -i {} \\;",
+            "command": "script/format.sh",
             "label": "format",
             "type": "shell"
         },
         {
+            "command": "black . && isort .",
+            "label": "python format",
+            "type": "shell"
+        },
+        {
             "command": "script/update_stubs.sh",
             "dependsOn": [
                 "install"
             ],
             "label": "update stub",
             "problemMatcher": [
                 "$gcc"
```

### Comparing `qulacs-0.6.0/CMakeLists.txt` & `qulacs-0.6.1/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -140,30 +140,14 @@
     INSTALL_COMMAND
       ${CMAKE_COMMAND} -E copy_directory ${EIGEN_BUILD_DIR}/src/eigen/Eigen ${EIGEN_INCLUDE_DIR}/Eigen
       && ${CMAKE_COMMAND} -E copy_directory ${EIGEN_BUILD_DIR}/src/eigen/unsupported ${EIGEN_INCLUDE_DIR}/unsupported
     TEST_COMMAND ""
 )
 include_directories(SYSTEM ${EIGEN_INCLUDE_DIR})
 
-# Cereal
-set(CEREAL_BUILD_DIR   ${CMAKE_BINARY_DIR}/cereal)
-set(CEREAL_INSTALL_DIR ${CMAKE_SOURCE_DIR}/include)
-set(CEREAL_INCLUDE_DIR ${CEREAL_INSTALL_DIR})
-ExternalProject_Add(
-    Cereal
-    URL https://github.com/USCiLab/cereal/archive/v1.3.0.tar.gz
-    PREFIX ${CEREAL_BUILD_DIR}
-    CONFIGURE_COMMAND ""
-    BUILD_COMMAND ""
-    INSTALL_COMMAND
-      ${CMAKE_COMMAND} -E copy_directory ${CEREAL_BUILD_DIR}/src/Cereal/include ${CEREAL_INCLUDE_DIR}
-    TEST_COMMAND ""
-)
-include_directories(SYSTEM ${CEREAL_INCLUDE_DIR})
-
 # Google test
 if(USE_TEST)
 	FetchContent_Declare(
 		googletest_fetch
 		GIT_REPOSITORY https://github.com/google/googletest
 		GIT_TAG release-1.12.1
 	)
@@ -493,14 +477,16 @@
     file(GLOB_RECURSE ALL_CXX_SOURCE_FILES
         ${CMAKE_CURRENT_SOURCE_DIR}/benchmark/*.[ch]pp
 		${CMAKE_CURRENT_SOURCE_DIR}/benchmark/*.[ch]
         ${CMAKE_CURRENT_SOURCE_DIR}/src/*.[ch]pp
         ${CMAKE_CURRENT_SOURCE_DIR}/src/*.[ch]
         ${CMAKE_CURRENT_SOURCE_DIR}/test/*.[ch]pp
         ${CMAKE_CURRENT_SOURCE_DIR}/test/*.[ch]
+        ${CMAKE_CURRENT_SOURCE_DIR}/python/*.[ch]pp
+        ${CMAKE_CURRENT_SOURCE_DIR}/python/*.[ch]
     )
     add_custom_target(
         format
         COMMAND clang-format
 		-style=file
         -i
         ${ALL_CXX_SOURCE_FILES}
@@ -517,14 +503,13 @@
 # python binding
 if(USE_PYTHON)
 	add_custom_target(python
 		DEPENDS qulacs_core
 	)
 	add_custom_target(pythontest
 		DEPENDS qulacs_core
-		COMMAND python ${CMAKE_CURRENT_SOURCE_DIR}/python/test/test_qulacs.py
+		COMMAND pytest -v -s ${CMAKE_CURRENT_SOURCE_DIR}/python/tests
 	)
 endif()
 
 #dependency setting for ExternalProject
-add_dependencies(qulacs_core Cereal)
 add_dependencies(qulacs_core eigen)
```

### Comparing `qulacs-0.6.0/CONTRIBUTING.md` & `qulacs-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/LICENSE` & `qulacs-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/PKG-INFO` & `qulacs-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qulacs
-Version: 0.6.0
+Version: 0.6.1
 Summary: Quantum circuit simulator for research
 Author-email: QunaSys <qulacs@qunasys.com>
 License: MIT License
         
         Copyright (c) 2018 Qulacs Authors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `qulacs-0.6.0/README.md` & `qulacs-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/README_MPI.md` & `qulacs-0.6.1/README_MPI.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/benchmark/AdaptiveGate.py` & `qulacs-0.6.1/benchmark/AdaptiveGate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from qulacs import QuantumState
-from qulacs.gate import Adaptive,X
+from qulacs.gate import Adaptive, X
 
 # OLD
 adaptive = Adaptive(X(0), lambda a: (a[2] == 1))
 s = QuantumState(1)
 s.set_computational_basis(0)
 s.set_classical_value(2, 1)
 adaptive.update_quantum_state(s)
 print(s)
 s.set_classical_value(2, 0)
 adaptive.update_quantum_state(s)
 print(s)
 
 # NEW
-adaptive = Adaptive(X(0), lambda a,b: (a[b] == 1),2)
+adaptive = Adaptive(X(0), lambda a, b: (a[b] == 1), 2)
 s = QuantumState(1)
 s.set_computational_basis(0)
 s.set_classical_value(2, 1)
 adaptive.update_quantum_state(s)
 print(s)
 s.set_classical_value(2, 0)
 adaptive.update_quantum_state(s)
```

### Comparing `qulacs-0.6.0/benchmark/bench_circuit.py` & `qulacs-0.6.1/benchmark/bench_circuit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,130 +1,167 @@
-from qulacs import QuantumCircuit, QuantumState
-from qulacs.circuit import QuantumCircuitOptimizer as QCO
-
-from argparse import ArgumentParser
-import numpy as np
 import random
 import time
-from mpi4py import MPI
+from argparse import ArgumentParser
 
+import numpy as np
 from circuits import get_circuit
+from mpi4py import MPI
+
+from qulacs import QuantumCircuit, QuantumState
+from qulacs.circuit import QuantumCircuitOptimizer as QCO
+
 
 def get_option():
     argparser = ArgumentParser()
-    argparser.add_argument('-n', '--nqubits', type = int,
-            default = 10, help = 'Number of qubits (default 10)')
-    argparser.add_argument('-d', '--depth', type = int,
-            default = 10, help = 'Number of Depth (default 10)')
-    argparser.add_argument('-o', '--opt', type = int,
-            default = -1, help = 'Enable QuantumCircuitOptimizer: 99 is to use optmize_light(), 0-6 is to use optimize(). (default no-use)')
-    #argparser.add_argument('-f', '--fused', type = int,
+    argparser.add_argument(
+        "-n", "--nqubits", type=int, default=10, help="Number of qubits (default 10)"
+    )
+    argparser.add_argument(
+        "-d", "--depth", type=int, default=10, help="Number of Depth (default 10)"
+    )
+    argparser.add_argument(
+        "-o",
+        "--opt",
+        type=int,
+        default=-1,
+        help="Enable QuantumCircuitOptimizer: 99 is to use optmize_light(), 0-6 is to use optimize(). (default no-use)",
+    )
+    # argparser.add_argument('-f', '--fused', type = int,
     #        default = -1, help = 'Enable QuantumCircuitOptimizer: 0 is not to use, 1-2 is to use Fused-swap opt')
-    argparser.add_argument('-v', '--verbose',
-            action='store_true',
-            help='Verbose switch, Output circuit infomations')
-    argparser.add_argument('-s', '--seed', type = int,
-            default = -1, help = 'Random Seed')
-    argparser.add_argument('-t', '--circuit', type = str,
-            default = "quantumvolume", help = 'Specify the Quantum Circuit name: "quantumvolume" or "qulacsbench" can be chosen.')
-    argparser.add_argument('-c', '--check', action = 'store_true', help = 'Check each values of the state vector between with and without multi-cpu')
+    argparser.add_argument(
+        "-v",
+        "--verbose",
+        action="store_true",
+        help="Verbose switch, Output circuit infomations",
+    )
+    argparser.add_argument("-s", "--seed", type=int, default=-1, help="Random Seed")
+    argparser.add_argument(
+        "-t",
+        "--circuit",
+        type=str,
+        default="quantumvolume",
+        help='Specify the Quantum Circuit name: "quantumvolume" or "qulacsbench" can be chosen.',
+    )
+    argparser.add_argument(
+        "-c",
+        "--check",
+        action="store_true",
+        help="Check each values of the state vector between with and without multi-cpu",
+    )
     return argparser.parse_args()
 
+
 tStart = time.perf_counter()
 
+
 def elapsed():
     global tStart
     tNow = time.perf_counter()
     elap = tNow - tStart
     tStart = tNow
     return f"elapsed_time= {elap:.6f}"
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     mpicomm = MPI.COMM_WORLD
     mpirank = mpicomm.Get_rank()
     mpisize = mpicomm.Get_size()
 
     args = get_option()
     n = args.nqubits
     num_global_qubits = int(np.log2(mpisize))
 
     st = QuantumState(n, use_multi_cpu=True)
     if args.circuit == "quantumvolume":
-        assert n - num_global_qubits >= num_global_qubits * 2, "ERROR: number of local qubits is too small"
+        assert (
+            n - num_global_qubits >= num_global_qubits * 2
+        ), "ERROR: number of local qubits is too small"
     elif args.circuit == "qulacsbench":
-        assert n - num_global_qubits >= num_global_qubits, "ERROR: number of local qubits is too small"
+        assert (
+            n - num_global_qubits >= num_global_qubits
+        ), "ERROR: number of local qubits is too small"
     else:
         assert False, "ERROR: " + args.circuit + " is not supported"
 
     if args.check:
         st_ref = QuantumState(n)
 
     if args.seed >= 0:
         seed = args.seed
         random.seed(seed)
-        rng = np.random.default_rng(seed = seed)
+        rng = np.random.default_rng(seed=seed)
     else:
         seed = random.randint(0, 9999)
-        seed = mpicomm.bcast(seed, root = 0)
+        seed = mpicomm.bcast(seed, root=0)
         random.seed(seed)
         np.random.seed(seed)
-        rng = np.random.default_rng(seed = seed)
+        rng = np.random.default_rng(seed=seed)
 
     # make a quantum circuit
-    circuit = get_circuit(args.circuit,
-            nqubits = args.nqubits,
-            global_nqubits = num_global_qubits,
-            #global_nqubits = 0 if args.fused >= 0 else num_global_qubits,
-            depth = args.depth,
-            verbose = (args.verbose and (mpirank == 0)),
-            random_gen = rng)
+    circuit = get_circuit(
+        args.circuit,
+        nqubits=args.nqubits,
+        global_nqubits=num_global_qubits,
+        # global_nqubits = 0 if args.fused >= 0 else num_global_qubits,
+        depth=args.depth,
+        verbose=(args.verbose and (mpirank == 0)),
+        random_gen=rng,
+    )
 
     if args.check:
         circuit_ref = circuit.copy()
     if args.opt == 99:
-        #if args.fused == -1:
-            QCO().optimize_light(circuit)
-        #else:
-        #    QCO().optimize_light(circuit, args.fused)
+        # if args.fused == -1:
+        QCO().optimize_light(circuit)
+    # else:
+    #    QCO().optimize_light(circuit, args.fused)
     elif args.opt >= 0:
-        #if args.fused == -1:
-            QCO().optimize(circuit, args.opt)
-        #else:
-        #    QCO().optimize(circuit, args.opt, args.fused)
+        # if args.fused == -1:
+        QCO().optimize(circuit, args.opt)
+    # else:
+    #    QCO().optimize(circuit, args.opt, args.fused)
 
     if mpirank == 0:
-        print("# A quantum circuit was created. ", args.circuit,
-                f"nqubits= {args.nqubits} depth= {args.depth}",
-        #        "optimize =", (args.opt, args.fused), elapsed())
-                "optimize=", args.opt, elapsed())
+        print(
+            "# A quantum circuit was created. ",
+            args.circuit,
+            f"nqubits= {args.nqubits} depth= {args.depth}",
+            #        "optimize =", (args.opt, args.fused), elapsed())
+            "optimize=",
+            args.opt,
+            elapsed(),
+        )
         print(circuit)
 
     # update the state vector
     circuit.update_quantum_state(st)
     mpicomm.barrier()
-    if mpirank == 0: print("# The state vector has been updated.", elapsed())
+    if mpirank == 0:
+        print("# The state vector has been updated.", elapsed())
 
     # Check that the result is the same as if it were not distributed
     if args.check:
-        if mpirank == 0: print("# check ", end="")
+        if mpirank == 0:
+            print("# check ", end="")
         circuit_ref.update_quantum_state(st_ref, seed)
         vec = st.get_vector()
         vec_ref = st_ref.get_vector()
         offs = 0
         if st.get_device_name() == "multi-cpu":
             offs = ((1 << args.nqubits) // mpisize) * mpirank
-        if np.allclose(vec, vec_ref[offs:offs + len(vec)]):
-            if mpirank == 0: print("OK!", elapsed())
+        if np.allclose(vec, vec_ref[offs : offs + len(vec)]):
+            if mpirank == 0:
+                print("OK!", elapsed())
         else:
             print("# check NG! rank=", mpirank)
             print("# vec    =", vec)
-            print("# vec_ref=", vec_ref[offs:offs + len(vec)])
+            print("# vec_ref=", vec_ref[offs : offs + len(vec)])
             exit()
 
     # sampling using the state vector
     samples = st.sampling(10, seed)
     if mpirank == 0:
         print(f"# sampling results(seed= {seed}) {samples}", elapsed())
         print()
 
     del st
-#EOF
+# EOF
```

### Comparing `qulacs-0.6.0/benchmark/causalconetest.cpp` & `qulacs-0.6.1/benchmark/causalconetest.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/benchmark/circuits/quantumvolume.py` & `qulacs-0.6.1/benchmark/circuits/quantumvolume.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """
 build a QuantumVolume Circuit with parameter
 """
 
-from qulacs import QuantumCircuit
 import numpy as np
 
+from qulacs import QuantumCircuit
+
+
 def simple_swap(p, q, array):
     tmp = array[p]
     array[p] = array[q]
     array[q] = tmp
 
+
 def local_swap(p, q, done_ug, qubit_table):
     simple_swap(p, q, done_ug)
     simple_swap(p, q, qubit_table)
-    #simple_swap(p, q, master_table)
+    # simple_swap(p, q, master_table)
+
 
 def block_swap(p, q, bs, done_ug, qubit_table):
     for t in range(bs):
         simple_swap(p + t, q + t, qubit_table)
-        #simple_swap(p + t, q + t, master_table)
+        # simple_swap(p + t, q + t, master_table)
+
 
 def build_circuit(nqubits, global_nqubits=0, depth=10, verbose=False, random_gen=""):
     use_fusedswap = True if global_nqubits > 0 else False
     local_nqubits = nqubits - global_nqubits
     if random_gen == "":
         rng = np.random.default_rng()
     else:
@@ -31,22 +36,26 @@
     circuit = QuantumCircuit(nqubits)
     perm_0 = list(range(nqubits))
     seed = rng.integers(10000)
 
     for d in range(depth):
         qubit_table = list(range(nqubits))
         perm = rng.permutation(perm_0)
-        pend_pair=[]
-        done_ug = [0]*nqubits
+        pend_pair = []
+        done_ug = [0] * nqubits
 
         # add random_unitary_gate for local_nqubits, first
-        for w in range(nqubits//2):
+        for w in range(nqubits // 2):
             physical_qubits = [int(perm[2 * w]), int(perm[2 * w + 1])]
-            if physical_qubits[0] < local_nqubits and physical_qubits[1] < local_nqubits:
-                if verbose: print("#1: circuit.add_random_unitary_gate(",physical_qubits,")")
+            if (
+                physical_qubits[0] < local_nqubits
+                and physical_qubits[1] < local_nqubits
+            ):
+                if verbose:
+                    print("#1: circuit.add_random_unitary_gate(", physical_qubits, ")")
                 circuit.add_random_unitary_gate(physical_qubits, seed)
                 seed += 1
                 done_ug[physical_qubits[0]] = 1
                 done_ug[physical_qubits[1]] = 1
             else:
                 pend_pair.append(physical_qubits)
 
@@ -55,29 +64,42 @@
         for s in range(global_nqubits):
             if done_ug[work_qubit + s] == 0:
                 for t in range(work_qubit):
                     if done_ug[work_qubit - t - 1] == 1:
                         p = work_qubit + s
                         q = work_qubit - t - 1
                         local_swap(p, q, done_ug, qubit_table)
-                        if verbose: print("#2: circuit.add_SWAP_gate(", p, ", ", q, ")")
+                        if verbose:
+                            print("#2: circuit.add_SWAP_gate(", p, ", ", q, ")")
                         circuit.add_SWAP_gate(p, q)
                         break
 
-        if verbose: print("#3 block_swap(", work_qubit,", ", local_nqubits,", ", global_nqubits, ")")
+        if verbose:
+            print(
+                "#3 block_swap(",
+                work_qubit,
+                ", ",
+                local_nqubits,
+                ", ",
+                global_nqubits,
+                ")",
+            )
         if global_nqubits > 0:
             block_swap(work_qubit, local_nqubits, global_nqubits, done_ug, qubit_table)
             circuit.add_FusedSWAP_gate(work_qubit, local_nqubits, global_nqubits)
-        if verbose: print("#: qubit_table=", qubit_table)
+        if verbose:
+            print("#: qubit_table=", qubit_table)
 
         # add random_unitary_gate for qubits that were originally outside.
         for pair in pend_pair:
             unitary_pair = [qubit_table.index(pair[0]), qubit_table.index(pair[1])]
-            if verbose: print("#4: circuit.add_random_unitary_gate(", unitary_pair, ")")
+            if verbose:
+                print("#4: circuit.add_random_unitary_gate(", unitary_pair, ")")
             circuit.add_random_unitary_gate(unitary_pair, seed)
             seed += 1
             done_ug[unitary_pair[0]] = 1
             done_ug[unitary_pair[1]] = 1
 
-    if verbose: print("circuit=",circuit)
+    if verbose:
+        print("circuit=", circuit)
 
     return circuit
```

### Comparing `qulacs-0.6.0/benchmark/circuits/qulacsbench.py` & `qulacs-0.6.1/benchmark/circuits/qulacsbench.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,114 +1,160 @@
 """
 build a Qulacs benchmark Circuit with parameter
 """
 
-from qulacs import QuantumCircuit
 import numpy as np
 
+from qulacs import QuantumCircuit
+
+
 def get_act_idx(i, local_qc, global_qc):
     if swapped:
         if i >= local_qc:
             return i - global_qc
         elif i >= local_qc - global_qc:
             return i + global_qc
         else:
             return i
     else:
         return i
 
+
 def first_rotation(circuit, nqubits, global_qc):
     global swapped
     local_qc = nqubits - global_qc
 
-    local_qubit_list = list(filter(lambda i: get_act_idx(i, local_qc, global_qc) <  local_qc, range(nqubits)))
-    global_qubit_list = list(filter(lambda i: get_act_idx(i, local_qc, global_qc) >= local_qc, range(nqubits)))
+    local_qubit_list = list(
+        filter(lambda i: get_act_idx(i, local_qc, global_qc) < local_qc, range(nqubits))
+    )
+    global_qubit_list = list(
+        filter(
+            lambda i: get_act_idx(i, local_qc, global_qc) >= local_qc, range(nqubits)
+        )
+    )
 
     for k in local_qubit_list:
         k_phy = get_act_idx(k, local_qc, global_qc)
-        if _print_debug and mpirank == 0: print('RX/RZ {} ({})'.format(k, k_phy))
+        if _print_debug and mpirank == 0:
+            print("RX/RZ {} ({})".format(k, k_phy))
         circuit.add_RX_gate(k_phy, np.random.rand())
         circuit.add_RZ_gate(k_phy, np.random.rand())
 
     if global_qc > 0:
-        if _print_debug and mpirank == 0: print('FusedSWAP {} {} {}'.format(local_qc - global_qc, local_qc, global_qc))
+        if _print_debug and mpirank == 0:
+            print(
+                "FusedSWAP {} {} {}".format(local_qc - global_qc, local_qc, global_qc)
+            )
         circuit.add_FusedSWAP_gate(local_qc - global_qc, local_qc, global_qc)
         swapped = not swapped
 
     for k in global_qubit_list:
         k_phy = get_act_idx(k, local_qc, global_qc)
-        if _print_debug and mpirank == 0: print('RX/RZ {} ({})'.format(k, k_phy))
+        if _print_debug and mpirank == 0:
+            print("RX/RZ {} ({})".format(k, k_phy))
         circuit.add_RX_gate(k_phy, np.random.rand())
         circuit.add_RZ_gate(k_phy, np.random.rand())
 
+
 def mid_rotation(circuit, nqubits, global_qc):
     global swapped
     local_qc = nqubits - global_qc
 
-    local_qubit_list = list(filter(lambda i: get_act_idx(i, local_qc, global_qc) <  local_qc, range(nqubits)))
-    global_qubit_list = list(filter(lambda i: get_act_idx(i, local_qc, global_qc) >= local_qc, range(nqubits)))
+    local_qubit_list = list(
+        filter(lambda i: get_act_idx(i, local_qc, global_qc) < local_qc, range(nqubits))
+    )
+    global_qubit_list = list(
+        filter(
+            lambda i: get_act_idx(i, local_qc, global_qc) >= local_qc, range(nqubits)
+        )
+    )
 
     for k in local_qubit_list:
         k_phy = get_act_idx(k, local_qc, global_qc)
-        if _print_debug and mpirank == 0: print('RZ/RX/RZ {} ({})'.format(k, k_phy))
+        if _print_debug and mpirank == 0:
+            print("RZ/RX/RZ {} ({})".format(k, k_phy))
         circuit.add_RZ_gate(k_phy, np.random.rand())
         circuit.add_RX_gate(k_phy, np.random.rand())
         circuit.add_RZ_gate(k_phy, np.random.rand())
 
     if global_qc > 0:
-        if _print_debug and mpirank == 0: print('FusedSWAP {} {} {}'.format(local_qc - global_qc, local_qc, global_qc))
+        if _print_debug and mpirank == 0:
+            print(
+                "FusedSWAP {} {} {}".format(local_qc - global_qc, local_qc, global_qc)
+            )
         circuit.add_FusedSWAP_gate(local_qc - global_qc, local_qc, global_qc)
         swapped = not swapped
 
     for k in global_qubit_list:
         k_phy = get_act_idx(k, local_qc, global_qc)
-        if _print_debug and mpirank == 0: print('RZ/RX/RZ {} ({})'.format(k, k_phy))
+        if _print_debug and mpirank == 0:
+            print("RZ/RX/RZ {} ({})".format(k, k_phy))
         circuit.add_RZ_gate(k_phy, np.random.rand())
         circuit.add_RX_gate(k_phy, np.random.rand())
         circuit.add_RZ_gate(k_phy, np.random.rand())
 
+
 def last_rotation(circuit, nqubits, global_qc):
     global swapped
     local_qc = nqubits - global_qc
 
-    local_qubit_list = list(filter(lambda i: get_act_idx(i, local_qc, global_qc) <  local_qc, range(nqubits)))
-    global_qubit_list = list(filter(lambda i: get_act_idx(i, local_qc, global_qc) >= local_qc, range(nqubits)))
+    local_qubit_list = list(
+        filter(lambda i: get_act_idx(i, local_qc, global_qc) < local_qc, range(nqubits))
+    )
+    global_qubit_list = list(
+        filter(
+            lambda i: get_act_idx(i, local_qc, global_qc) >= local_qc, range(nqubits)
+        )
+    )
 
     for k in local_qubit_list:
         k_phy = get_act_idx(k, local_qc, global_qc)
-        if _print_debug and mpirank == 0: print('RZ/RX {} ({})'.format(k, k_phy))
+        if _print_debug and mpirank == 0:
+            print("RZ/RX {} ({})".format(k, k_phy))
         circuit.add_RZ_gate(k_phy, np.random.rand())
         circuit.add_RX_gate(k_phy, np.random.rand())
 
     if global_qc > 0:
-        if _print_debug and mpirank == 0: print('FusedSWAP {} {} {}'.format(local_qc - global_qc, local_qc, global_qc))
+        if _print_debug and mpirank == 0:
+            print(
+                "FusedSWAP {} {} {}".format(local_qc - global_qc, local_qc, global_qc)
+            )
         circuit.add_FusedSWAP_gate(local_qc - global_qc, local_qc, global_qc)
         swapped = not swapped
 
     for k in global_qubit_list:
         k_phy = get_act_idx(k, local_qc, global_qc)
-        if _print_debug and mpirank == 0: print('RZ/RX {} ({})'.format(k, k_phy))
+        if _print_debug and mpirank == 0:
+            print("RZ/RX {} ({})".format(k, k_phy))
         circuit.add_RZ_gate(k_phy, np.random.rand())
         circuit.add_RX_gate(k_phy, np.random.rand())
 
+
 def entangler(circuit, nqubits, pairs, global_qc):
     global swapped
     local_qc = nqubits - global_qc
 
     for a, b in pairs:
         if global_qc > 0 and get_act_idx(b, local_qc, global_qc) >= local_qc:
-            if _print_debug and mpirank == 0: print('FusedSWAP {} {} {}'.format(local_qc - global_qc, local_qc, global_qc))
+            if _print_debug and mpirank == 0:
+                print(
+                    "FusedSWAP {} {} {}".format(
+                        local_qc - global_qc, local_qc, global_qc
+                    )
+                )
             circuit.add_FusedSWAP_gate(local_qc - global_qc, local_qc, global_qc)
             swapped = not swapped
 
         a_phy = get_act_idx(a, local_qc, global_qc)
         b_phy = get_act_idx(b, local_qc, global_qc)
-        if _print_debug and mpirank == 0: print('CNOT {} {} ({} {})'.format(a, b, a_phy, b_phy))
+        if _print_debug and mpirank == 0:
+            print("CNOT {} {} ({} {})".format(a, b, a_phy, b_phy))
         circuit.add_CNOT_gate(a_phy, b_phy)
 
+
 def build_circuit(nqubits, global_nqubits, depth=9, verbose=False, random_gen=""):
     use_fusedswap = True if global_nqubits > 0 else False
     local_nqubits = nqubits - global_nqubits
     if random_gen == "":
         rng = np.random.default_rng()
     else:
         rng = random_gen
@@ -131,14 +177,17 @@
     for k in range(depth):
         mid_rotation(circuit, nqubits, global_qc)
         entangler(circuit, nqubits, pairs, global_qc)
     last_rotation(circuit, nqubits, global_qc)
 
     # recover if needed
     if use_fusedswap and swapped:
-        if _print_debug and mpirank == 0: print('FusedSWAP {} {} {}'.format(local_qc - global_qc, local_qc, global_qc))
+        if _print_debug and mpirank == 0:
+            print(
+                "FusedSWAP {} {} {}".format(local_qc - global_qc, local_qc, global_qc)
+            )
         circuit.add_FusedSWAP_gate(local_qc - global_qc, local_qc, global_qc)
         swapped = not swapped
 
     assert swapped is False
 
     return circuit
```

### Comparing `qulacs-0.6.0/benchmark/libcppsim_benchmark.cpp` & `qulacs-0.6.1/benchmark/libcppsim_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/benchmark/libcsim_benchmark.cpp` & `qulacs-0.6.1/benchmark/libcsim_benchmark.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/benchmark/test_qulacs_1.py` & `qulacs-0.6.1/benchmark/test_qulacs_1.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,153 +1,198 @@
 import numpy as np
+import pytest
 from scipy.sparse import csr_matrix
+
 from qulacs import QuantumCircuit, QuantumState
-from qulacs.gate import X, T, H, CNOT, TOFFOLI, DenseMatrix, PauliRotation, SparseMatrix, DiagonalMatrix, ReversibleBoolean
+from qulacs.gate import (
+    CNOT,
+    TOFFOLI,
+    DenseMatrix,
+    DiagonalMatrix,
+    H,
+    PauliRotation,
+    ReversibleBoolean,
+    SparseMatrix,
+    T,
+    X,
+)
 
-import pytest
+nqubits_list = range(4, 26)
 
-nqubits_list = range(4,26)
 
 def bench_gate(benchmark, nqubits, g):
     st = QuantumState(nqubits)
     benchmark(g.update_quantum_state, st)
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_X(benchmark, nqubits):
     benchmark.group = "X"
     bench_gate(benchmark, nqubits, X(3))
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_CNOT(benchmark, nqubits):
     benchmark.group = "CNOT"
     bench_gate(benchmark, nqubits, CNOT(2, 3))
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_TOFFOLI(benchmark, nqubits):
     benchmark.group = "TOFFOLI"
     bench_gate(benchmark, nqubits, TOFFOLI(1, 2, 3))
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_CCCNOT(benchmark, nqubits):
     benchmark.group = "CCCNOT"
-    g = DenseMatrix([3], [[0,1],[1,0]])
-    g.add_control_qubit(2,1)
-    g.add_control_qubit(1,1)
-    g.add_control_qubit(0,1)
+    g = DenseMatrix([3], [[0, 1], [1, 0]])
+    g.add_control_qubit(2, 1)
+    g.add_control_qubit(1, 1)
+    g.add_control_qubit(0, 1)
     bench_gate(benchmark, nqubits, g)
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Dense1Q(benchmark, nqubits):
     benchmark.group = "DenseMatrix1Q"
     bench_gate(benchmark, nqubits, DenseMatrix([3], np.eye(2)))
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Dense2Q(benchmark, nqubits):
     benchmark.group = "DenseMatrix2Q"
-    bench_gate(benchmark, nqubits, DenseMatrix([2,3], np.eye(4)))
+    bench_gate(benchmark, nqubits, DenseMatrix([2, 3], np.eye(4)))
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Dense3Q(benchmark, nqubits):
     benchmark.group = "DenseMatrix3Q"
-    bench_gate(benchmark, nqubits, DenseMatrix([1,2,3], np.eye(8)))
+    bench_gate(benchmark, nqubits, DenseMatrix([1, 2, 3], np.eye(8)))
+
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Dense4Q(benchmark, nqubits):
     benchmark.group = "DenseMatrix4Q"
-    bench_gate(benchmark, nqubits, DenseMatrix([0,1,2,3], np.eye(16)))
+    bench_gate(benchmark, nqubits, DenseMatrix([0, 1, 2, 3], np.eye(16)))
+
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Diagonal1QSp(benchmark, nqubits):
     benchmark.group = "DiagonalMatrix1QSp"
     bench_gate(benchmark, nqubits, DiagonalMatrix([0], np.ones(2)))
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Diagonal1Q(benchmark, nqubits):
     benchmark.group = "DiagonalMatrix1Q"
     bench_gate(benchmark, nqubits, DiagonalMatrix([3], np.ones(2)))
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Diagonal2Q(benchmark, nqubits):
     benchmark.group = "DiagonalMatrix2Q"
-    bench_gate(benchmark, nqubits, DiagonalMatrix([2,3], np.ones(4)))
+    bench_gate(benchmark, nqubits, DiagonalMatrix([2, 3], np.ones(4)))
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Diagonal3Q(benchmark, nqubits):
     benchmark.group = "DiagonalMatrix3Q"
-    bench_gate(benchmark, nqubits, DiagonalMatrix([1,2,3], np.ones(8)))
+    bench_gate(benchmark, nqubits, DiagonalMatrix([1, 2, 3], np.ones(8)))
+
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Diagonal4Q(benchmark, nqubits):
     benchmark.group = "DiagonalMatrix4Q"
-    bench_gate(benchmark, nqubits, DiagonalMatrix([0,1,2,3], np.ones(16)))
+    bench_gate(benchmark, nqubits, DiagonalMatrix([0, 1, 2, 3], np.ones(16)))
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Sparse1Q(benchmark, nqubits):
     benchmark.group = "SparseMatrix1Q"
-    sparse_matrix = csr_matrix(([1], ([0],[0])), shape=(2,2), dtype=complex)
+    sparse_matrix = csr_matrix(([1], ([0], [0])), shape=(2, 2), dtype=complex)
     bench_gate(benchmark, nqubits, SparseMatrix([3], sparse_matrix))
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Sparse2Q(benchmark, nqubits):
     benchmark.group = "SparseMatrix2Q"
-    sparse_matrix = csr_matrix(([1], ([0],[0])), shape=(4,4), dtype=complex)
-    bench_gate(benchmark, nqubits, SparseMatrix([2,3], sparse_matrix))
+    sparse_matrix = csr_matrix(([1], ([0], [0])), shape=(4, 4), dtype=complex)
+    bench_gate(benchmark, nqubits, SparseMatrix([2, 3], sparse_matrix))
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Sparse3Q(benchmark, nqubits):
     benchmark.group = "SparseMatrix3Q"
-    sparse_matrix = csr_matrix(([1], ([0],[0])), shape=(8,8), dtype=complex)
-    bench_gate(benchmark, nqubits, SparseMatrix([1,2,3], sparse_matrix))
+    sparse_matrix = csr_matrix(([1], ([0], [0])), shape=(8, 8), dtype=complex)
+    bench_gate(benchmark, nqubits, SparseMatrix([1, 2, 3], sparse_matrix))
+
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Sparse4Q(benchmark, nqubits):
     benchmark.group = "SparseMatrix4Q"
-    sparse_matrix = csr_matrix(([1], ([0],[0])), shape=(16,16), dtype=complex)
-    bench_gate(benchmark, nqubits, SparseMatrix([0,1,2,3], sparse_matrix))
+    sparse_matrix = csr_matrix(([1], ([0], [0])), shape=(16, 16), dtype=complex)
+    bench_gate(benchmark, nqubits, SparseMatrix([0, 1, 2, 3], sparse_matrix))
+
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Permutation1Q(benchmark, nqubits):
     benchmark.group = "Permutation1Q"
+
     def rev(index, dim):
-        return (index+1)%dim
+        return (index + 1) % dim
+
     bench_gate(benchmark, nqubits, ReversibleBoolean([3], rev))
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Permutation2Q(benchmark, nqubits):
     benchmark.group = "Permutation2Q"
+
     def rev(index, dim):
-        return (index+1)%dim
-    bench_gate(benchmark, nqubits, ReversibleBoolean([2,3], rev))
+        return (index + 1) % dim
+
+    bench_gate(benchmark, nqubits, ReversibleBoolean([2, 3], rev))
+
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Permutation3Q(benchmark, nqubits):
     benchmark.group = "Permutation3Q"
+
     def rev(index, dim):
-        return (index+1)%dim
-    bench_gate(benchmark, nqubits, ReversibleBoolean([1,2,3], rev))
+        return (index + 1) % dim
+
+    bench_gate(benchmark, nqubits, ReversibleBoolean([1, 2, 3], rev))
+
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Permutation4Q(benchmark, nqubits):
     benchmark.group = "Permutation4Q"
+
     def rev(index, dim):
-        return (index+1)%dim
-    bench_gate(benchmark, nqubits, ReversibleBoolean([0,1,2,3], rev))
+        return (index + 1) % dim
+
+    bench_gate(benchmark, nqubits, ReversibleBoolean([0, 1, 2, 3], rev))
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_PauliRotation1Q(benchmark, nqubits):
     benchmark.group = "PauliRotation1Q"
     bench_gate(benchmark, nqubits, PauliRotation([3], [1], 0.1))
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_PauliRotation2Q(benchmark, nqubits):
     benchmark.group = "PauliRotation2Q"
-    bench_gate(benchmark, nqubits, PauliRotation([2,3], [1,1], 0.1))
+    bench_gate(benchmark, nqubits, PauliRotation([2, 3], [1, 1], 0.1))
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_PauliRotation3Q(benchmark, nqubits):
     benchmark.group = "PauliRotation3Q"
-    bench_gate(benchmark, nqubits, PauliRotation([1,2,3], [1,1,1], 0.1))
+    bench_gate(benchmark, nqubits, PauliRotation([1, 2, 3], [1, 1, 1], 0.1))
+
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_PauliRotation4Q(benchmark, nqubits):
     benchmark.group = "PauliRotation4Q"
-    bench_gate(benchmark, nqubits, PauliRotation([0,1,2,3], [1,1,1,1], 0.1))
+    bench_gate(benchmark, nqubits, PauliRotation([0, 1, 2, 3], [1, 1, 1, 1], 0.1))
```

### Comparing `qulacs-0.6.0/benchmark/test_qulacs_2.py` & `qulacs-0.6.1/benchmark/test_qulacs_2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,57 @@
 import numpy as np
+import pytest
 from scipy.sparse import csr_matrix
+
 from qulacs import QuantumCircuit, QuantumState
-from qulacs.gate import DenseMatrix, CPTP, Probabilistic, Instrument, Measurement
+from qulacs.gate import (
+    CPTP,
+    DenseMatrix,
+    Instrument,
+    Measurement,
+    Probabilistic,
+)
 
-import pytest
+nqubits_list = range(4, 26)
 
-nqubits_list = range(4,26)
 
 def bench_gate(benchmark, nqubits, g):
     st = QuantumState(nqubits)
     benchmark(g.update_quantum_state, st)
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Dense1Q(benchmark, nqubits):
     benchmark.group = "DenseMatrix1Q"
     bench_gate(benchmark, nqubits, DenseMatrix([3], np.eye(2)))
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_CPTP1Q(benchmark, nqubits):
     benchmark.group = "CPTP1Q"
-    g = DenseMatrix([3,], np.eye(2)/np.sqrt(2))
-    cptp = CPTP([g,g])
+    g = DenseMatrix(
+        [
+            3,
+        ],
+        np.eye(2) / np.sqrt(2),
+    )
+    cptp = CPTP([g, g])
     bench_gate(benchmark, nqubits, cptp)
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Instrument1Q(benchmark, nqubits):
     benchmark.group = "Instrument1Q"
     bench_gate(benchmark, nqubits, Measurement(3, 0))
 
-@pytest.mark.parametrize('nqubits', nqubits_list)
+
+@pytest.mark.parametrize("nqubits", nqubits_list)
 def test_Probabilistic1Q(benchmark, nqubits):
     benchmark.group = "Probabilistic1Q"
-    g = DenseMatrix([3,], np.eye(2)/np.sqrt(2))
-    gate = Probabilistic([0.5, 0.5], [g,g])
+    g = DenseMatrix(
+        [
+            3,
+        ],
+        np.eye(2) / np.sqrt(2),
+    )
+    gate = Probabilistic([0.5, 0.5], [g, g])
     bench_gate(benchmark, nqubits, gate)
-
```

### Comparing `qulacs-0.6.0/cmake_script/FetchContent/CMakeLists.cmake.in` & `qulacs-0.6.1/cmake_script/FetchContent/CMakeLists.cmake.in`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/cmake_script/FetchContent.cmake` & `qulacs-0.6.1/cmake_script/FetchContent.cmake`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/cmake_script/FindAVX2.cmake` & `qulacs-0.6.1/cmake_script/FindAVX2.cmake`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/cmake_script/FindSVE.cmake` & `qulacs-0.6.1/cmake_script/FindSVE.cmake`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/.gitignore` & `qulacs-0.6.1/doc/.gitignore`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/Makefile` & `qulacs-0.6.1/doc/en/Makefile`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/make.bat` & `qulacs-0.6.1/doc/en/make.bat`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/_static/images/dojo.png` & `qulacs-0.6.1/doc/en/source/_static/images/dojo.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/_static/images/github.png` & `qulacs-0.6.1/doc/en/source/_static/images/github.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/_static/images/logo-c-h.png` & `qulacs-0.6.1/doc/en/source/_static/images/logo-c-h.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/_static/images/slack.png` & `qulacs-0.6.1/doc/en/source/_static/images/slack.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/_templates/autoapi/python/class.rst` & `qulacs-0.6.1/doc/en/source/_templates/autoapi/python/class.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/_templates/autoapi/python/data.rst` & `qulacs-0.6.1/doc/en/source/_templates/autoapi/python/data.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/_templates/autoapi/python/function.rst` & `qulacs-0.6.1/doc/en/source/_templates/autoapi/python/function.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/_templates/autoapi/python/method.rst` & `qulacs-0.6.1/doc/en/source/_templates/autoapi/python/method.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/_templates/autoapi/python/module.rst` & `qulacs-0.6.1/doc/en/source/_templates/autoapi/python/module.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/apply/0_overview.ipynb` & `qulacs-0.6.1/doc/en/source/apply/0_overview.ipynb`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/apply/5.2_qcl.ipynb` & `qulacs-0.6.1/doc/en/source/apply/5.2_qcl.ipynb`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/apply/6.2_vqe.ipynb` & `qulacs-0.6.1/doc/en/source/apply/6.2_vqe.ipynb`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/apply/6.3_ssvqe.ipynb` & `qulacs-0.6.1/doc/en/source/apply/6.3_ssvqe.ipynb`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/apply/img/QCL.png` & `qulacs-0.6.1/doc/en/source/apply/img/QCL.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/conf.py` & `qulacs-0.6.1/doc/en/source/conf.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 import qulacs
 
 project = "Qulacs"
 
 language = "en"
 locale_dirs = ["locale/"]
 
@@ -91,16 +93,14 @@
 
 # Tell sphinx what the pygments highlight language should be.
 # highlight_language = 'cpp'
 
 #
 
 # on_rtd is whether we are on readthedocs.org, this line of code grabbed from docs.readthedocs.org
-import os
-
 on_rtd = os.environ.get("READTHEDOCS", None) == "True"
 
 if not on_rtd:  # only import and set the theme if we're building docs locally
     import sphinx_rtd_theme
 
     html_theme = "sphinx_rtd_theme"
     html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
```

### Comparing `qulacs-0.6.0/doc/en/source/guide/2.0_python_advanced.ipynb` & `qulacs-0.6.1/doc/en/source/guide/2.0_python_advanced.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9796352155727156%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 1: {'attachments': OrderedDict()}, 3: "*

 * *            "{'execution_count': 1}, 4: {'attachments': OrderedDict()}, 6: {'attachments': "*

 * *            "OrderedDict()}, 12: {'attachments': OrderedDict()}, 14: {'attachments': "*

 * *            "OrderedDict()}, 16: {'attachments': OrderedDict()}, 18: {'attachments': "*

 * *            "OrderedDict()}, 20: {'attachments': OrderedDict()}, 22: {'attachments': "*

 * *            "OrderedDict()}, 24: {'attachments': OrderedDict()}, 26:  […]*

```diff
@@ -1,19 +1,21 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Qulacs Python Advanced Guide\n",
                 "\n",
                 "This chapter is for those who are familiar with the terminology of quantum information and want fine tuning for numerical calculations. For more information on terminology, please see the textbook **Quantum Computation and Quantum Information** by M.A. Nielsen et al.."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Quantum States\n",
                 "This class allocates and manages $2^n$ complex arrays on the CPU/GPU with the precision of complex128."
             ]
         },
@@ -24,15 +26,15 @@
             "source": [
                 "### Create and Destroy\n",
                 "Necessary memory is secured at the time of instance creation and released when the instance is destroyed, but you can explicitly destroy it to release the memory with `del`."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         " *** Quantum State ***\n",
@@ -52,14 +54,15 @@
                 "n = 2\n",
                 "state = QuantumState(n)\n",
                 "print(state)\n",
                 "del state"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Transform between quantum state and numpy array\n",
                 "Transformation between quantum state and numpy array can be realized by `get_vector` or `load` function. In principle, it is not checked whether the norm is saved.\n",
                 "While `get_vector` returns all the element as an array, `get_amplitude` can be used to quickly get a single element."
             ]
@@ -87,14 +90,15 @@
                 "print(vec)\n",
                 "state.load([0,1,2,3])\n",
                 "print(state.get_vector())\n",
                 "print(state.get_amplitude(2))"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Copy quantum states\n",
                 "Quantum states can generate new instances of the same state by `copy`. By giving a quantum state to the load function, it is possible to copy a quantum vector of another quantum state without allocating a new area in the existing quantum state. This allows you to reuse the already allocated space. You can use the `allocate_buffer` function if you want to allocate a state vector of the same size as the quantum state you already have and without copying the state."
             ]
         },
@@ -177,14 +181,15 @@
                 "\n",
                 "# load\n",
                 "with open('state.pickle', 'rb') as f:\n",
                 "    state = pickle.load(f)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Initialization of quantum state\n",
                 "The following is an function initializing a quantum state to a specific state."
             ]
         },
@@ -221,14 +226,15 @@
                 "# Initialize to random pure state with Haar measure using argument value as seed\n",
                 "# If no value is specified, the time function is used as a seed. Pseudo random number uses xorshift.\n",
                 "state.set_Haar_random_state(0)\n",
                 "print(state.get_vector())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Check quantum state\n",
                 "The following example is a list of functions to check quantum state information without changing the quantum state."
             ]
         },
@@ -296,14 +302,15 @@
                 "\n",
                 "# Get a character string indicating whether the state vector is on CPU or GPU\n",
                 "dev_type = state.get_device_name()\n",
                 "print(\"device\", dev_type)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Deformation of quantum state\n",
                 "The following functions modify a quantum state."
             ]
         },
@@ -365,14 +372,15 @@
                 "print(\"sq_norm\", squared_norm)\n",
                 "state.normalize(squared_norm)\n",
                 "print(\"normalized\", state.get_vector())\n",
                 "print(\"sq_norm\", state.get_squared_norm())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Opetation on classic registers\n",
                 "Quantum states have classical registers as integer arrays with variable length. The classical register is used to write the result of the Instrument operation or to describe a gate that executes conditions as the result of the classical register. The value of a classic register that has not yet been written is 0. The classical register is copied at the same time when the quantum state is copied by the `copy` and `load` functions."
             ]
         },
@@ -397,14 +405,15 @@
                 "state.set_classical_value(position, 20)\n",
                 "# Get the value of the `position`-th register\n",
                 "obtained = state.get_classical_value(position)\n",
                 "print(obtained)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Calculation between quantum states\n",
                 "The inner product and tensor product between quantum states can be obtained by `inner_product` and `tensor_product` respectively."
             ]
         },
@@ -445,14 +454,15 @@
                 "\n",
                 "# Calculation of tensor product\n",
                 "tensor_product_state = tensor_product(state_ket1, state_ket2)\n",
                 "print(tensor_product_state.get_vector())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Swap and delete qubits\n",
                 "You can swap indices of a qubit with `permutate_qubit()`.\n",
                 "You can get a projection onto a specified qubit with `drop_qubit()`."
             ]
@@ -505,14 +515,15 @@
                 "state0 = drop_qubit(state, [1], [0])\n",
                 "print(\"projection to 0:\", state0.get_vector()) # projection: qubit 1 is 0\n",
                 "state1 = drop_qubit(state, [1], [1])\n",
                 "print(\"projection to 1:\", state1.get_vector()) # projection: qubit 1 is 1"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Calculate partial trace\n",
                 "With `partial_trace()`, you can obtain a partial trace of a given qubit of a given quantum state as a density matrix.\n",
                 "The indices of the converted qubits are reassigned based on the order of the qubits before conversion."
             ]
@@ -568,45 +579,49 @@
                 "print(dm_state.get_matrix())\n",
                 "\n",
                 "trace = partial_trace(dm_state, [1])\n",
                 "print(trace.get_matrix())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Calculation using GPU\n",
                 "When Qulacs is installed from qulacs-gpu package, `QuantumStateGpu` is available. Except the different class name, the usage is the same as `QuantumState`."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "```python\n",
                 "from qulacs import QuantumStateGpu\n",
                 "state = QuantumStateGpu(2)\n",
                 "print(state)\n",
                 "# print(state.get_device_name())\n",
                 "# gpu\n",
                 "```"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Though the usage is the same as `QuantumState`, there are two aspects to keep in mind:\n",
                 "\n",
                 "* The `get_vector` function takes a long time because it requires copying between the GPU and CPU. This function should be avoided whenever possible.\n",
                 "* `inner_product` between CPU / GPU states cannot be calculated. It is possible to `load` a state vector between the GPU and CPU state vectors, but it is time consuming and should be avoided."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## DensityMatrix\n",
                 "\n",
                 "`DensityMatrix` is a class to hold a quantum state as a density matrix. While `StateVector` can hold a pure state, `DensityMatrix` can also hold a mixed state, or probabilistic mixture of multiple states.\n",
                 "Use the density matrix $\\sum_i p_i\\ket{\\psi_i}\\bra{\\psi_i}$ when each state is $\\ket{\\psi_i}$ with probability $p_i$.\n",
@@ -643,14 +658,15 @@
                 "n = 2\n",
                 "state = DensityMatrix(n)\n",
                 "print(state)\n",
                 "del state"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Conversion between quantum states and numpy array\n",
                 "You can convert quantum states and numpy array mutually with `get_matrix` and `load`.\n",
                 "If the array is 1-dimensional, it is converted from a state vector to a density matrix, and if it is 2-dimensional, it is read as a density matrix.\n",
                 "Basically, whether the norm is conserved or not is not checked."
@@ -689,14 +705,15 @@
                 "state.load([0,1,2,3])\n",
                 "print(state.get_matrix())\n",
                 "state.load([[0,1,2,3], [1,2,3,4], [2,3,4,5], [3,4,5,6]])\n",
                 "print(state.get_matrix())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Copy between quantum states\n",
                 "A quantum state can be instantiated by `copy` to create a new instance of itself.\n",
                 "Also, by giving a quantum state to the `load` function, you can copy the quantum vector or density matrix of another quantum state without allocating new space in the existing quantum state.\n",
                 "This allows you to reuse the space you have already allocated. If you want to allocate a density matrix of the same size as the quantum state you already have, but do not need to copy the state, you can use the `allocate_buffer` function."
@@ -793,14 +810,15 @@
                 "\n",
                 "# load\n",
                 "with open('state.pickle', 'rb') as f:\n",
                 "    state = pickle.load(f)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Initialize quantum states\n",
                 "The following example shows functions to initialize a quantum state to a specific pure state."
             ]
         },
@@ -851,14 +869,15 @@
                 "# If you do not give the seed, `time` function is used for seed.\n",
                 "# Xorshift is used for psuedo random.\n",
                 "state.set_Haar_random_state(0)\n",
                 "print(state.get_matrix())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Check quantum states\n",
                 "The following example shows functions to check information of quantum states without changing the states."
             ]
         },
@@ -1008,14 +1027,15 @@
                 "print(\"sq_norm\", squared_norm)\n",
                 "state.normalize(squared_norm)\n",
                 "print(\"normalized\", state.get_matrix())\n",
                 "print(\"sq_norm\", state.get_squared_norm())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Operation on classical registers\n",
                 "`DensityMatrix` also has classical registers as integer arrays with variable length."
             ]
         },
@@ -1092,14 +1112,15 @@
                 "p = 1 / 2\n",
                 "q = 1 / 2\n",
                 "c = make_mixture(p, a, q, b)\n",
                 "print(c.get_matrix())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Quantum gates\n",
                 "\n",
                 "### Types of quantum gate\n",
                 "Quantum gates are divided into two types: special gates and general gates. In Qulacs, quantum gates are not limited to unitary operators, and the operation of updating an arbitrary quantum state, such as Instrument and CPTP-map, is also called a gate.\n",
@@ -1198,14 +1219,113 @@
                 "gate_json = o_gate.to_json()\n",
                 "\n",
                 "r_gate = gate.from_json(gate_json)\n",
                 "print(r_gate)"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "A new instance of the same quantum gate as itself can be created with the `copy` function."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 1,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        " *** gate info *** \n",
+                        " * gate name : X\n",
+                        " * target    : \n",
+                        " 2 : commute X     \n",
+                        " * control   : \n",
+                        " * Pauli     : yes\n",
+                        " * Clifford  : yes\n",
+                        " * Gaussian  : no\n",
+                        " * Parametric: no\n",
+                        " * Diagonal  : no\n",
+                        "\n",
+                        " *** gate info *** \n",
+                        " * gate name : X\n",
+                        " * target    : \n",
+                        " 2 : commute X     \n",
+                        " * control   : \n",
+                        " * Pauli     : yes\n",
+                        " * Clifford  : yes\n",
+                        " * Gaussian  : no\n",
+                        " * Parametric: no\n",
+                        " * Diagonal  : no\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "import numpy as np\n",
+                "from qulacs.gate import X\n",
+                "\n",
+                "n = 2\n",
+                "initial_gate = X(n)\n",
+                "print(initial_gate)\n",
+                "\n",
+                "copied_gate = initial_gate.copy()\n",
+                "print(copied_gate)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "The `update_quantum_state` function is used to change the quantum state by a quantum gate.\n",
+                "For example, to make the H-gate act on the 0-th qubit, write the following code."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        " *** Quantum State ***\n",
+                        " * Qubit Count : 2\n",
+                        " * Dimension   : 4\n",
+                        " * State vector : \n",
+                        "(0.707107,0)\n",
+                        "(0.707107,0)\n",
+                        "       (0,0)\n",
+                        "       (0,0)\n",
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "import qulacs\n",
+                "from qulacs.gate import H\n",
+                "\n",
+                "n = 2\n",
+                "quantum_state = qulacs.QuantumState(n)\n",
+                "\n",
+                "quantum_state.set_zero_state()\n",
+                "\n",
+                "hadamard_gate = H(0)\n",
+                "\n",
+                "hadamard_gate.update_quantum_state(quantum_state)\n",
+                "\n",
+                "print(quantum_state)"
+            ]
+        },
+        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Special gate\n",
                 "The special gates are listed below.\n",
                 "\n",
                 "#### 1 qubit gate\n",
@@ -1243,14 +1363,15 @@
                 "from qulacs.gate import P0, P1 # Projection to 0,1 (not normalized)\n",
                 "target = 3\n",
                 "gate = T(target)\n",
                 "print(gate)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "`Identity` does not update the quantum state, but when it is included into the quantum circuit, it is counted as a gate that consumes 1 step.\n",
                 "\n",
                 "#### 1 qubit rotating gate\n",
                 "Take the index of the target bit as the first argument and the rotation angle as the second argument."
@@ -1288,14 +1409,15 @@
                 "angle = 0.1\n",
                 "gate = RX(target, angle)\n",
                 "print(gate)\n",
                 "print(gate.get_matrix())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The definition of rotating operation is $R_X(\\theta) = \\exp(i\\frac{\\theta}{2} X)$\u3067\u3059\u3002\n",
                 "\n",
                 "#### IBMQ basis gate\n",
                 " IBMQ basis gate is a gate based on the virtual-Z decomposition defined by IBMQ's OpenQASM."
@@ -1329,14 +1451,15 @@
             ],
             "source": [
                 "from qulacs.gate import U1,U2,U3\n",
                 "print(U3(0, 0.1, 0.2, 0.3))"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Definitions are:\n",
                 "\n",
                 "* $U_1(\\lambda) = R_Z(\\lambda)$\n",
                 "* $U_2(\\phi, \\lambda) = R_Z(\\phi+\\frac{\\pi}{2}) R_X(\\frac{\\pi}{2}) R_Z(\\lambda-\\frac{\\pi}{2})$\n",
@@ -1380,14 +1503,15 @@
                 "gate = CNOT(control, target)\n",
                 "print(gate)\n",
                 "gate = CZ(control, target)\n",
                 "gate = SWAP(target, target2)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Multi-bit Pauli operation\n",
                 "Multi-bit Pauli operations define a gate with arguments as a list of target qubits and a list of Pauli operators. Since the update speed of an $n$-qubit Pauli operation has the same order as the update cost of a 1-qubit Pauli operation, Pauli's tensor product should be defined as the gate in this form. In the Pauli operator specification, 1, 2, and 3 correspond to X, Y, and Z, respectively."
             ]
         },
@@ -1430,14 +1554,15 @@
                 "pauli_index = [1,3,1] # 1:X , 2:Y, 3:Z\n",
                 "gate = Pauli(target_list, pauli_index) # = X_0 Z_3 X_5\n",
                 "print(gate)\n",
                 "print(gate.get_matrix())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Multi-bit Pauli rotating operation\n",
                 "Multi-bit Pauli rotating operation rotates multi-bit Pauli operator. The multi-bit Pauli rotation becomes heavy calculation when the gate matrix is calculated greedily, but it can be updated efficiently if it is defined in this form."
             ]
         },
@@ -1474,14 +1599,15 @@
                 "angle = 0.5\n",
                 "gate = PauliRotation(target_list, pauli_index, angle) # = exp(i angle/2 X_0 Z_3 X_5)\n",
                 "print(gate)\n",
                 "print(gate.get_matrix().shape)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Reversible circuit\n",
                 "Reversible circuit performs permutation operation between basis by giving a bijective function to a total number of $2^n$ index. This is equivalent to the gate matrix being a permutation matrix. Please note that it will not work properly unless the given function is bijective."
             ]
         },
@@ -1522,14 +1648,15 @@
                 "state.load(np.arange(2**3))\n",
                 "print(state.get_vector())\n",
                 "gate.update_quantum_state(state)\n",
                 "print(state.get_vector())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The above code moves the elements of the vector down one by one in the subspace of the qubit of interest (the bottom element moves to the top).\n",
                 "### State reflection\n",
                 "This gate is $(I-2\\ket{a}\\bra{a})$, which is defined with the quantum state $\\ket{a}$ as an argument. This corresponds to the operation of reflecting based on the quantum state $\\ket{a}$. This gate appears in Grover search. The number of qubits on which this gate operates must match the number of qubits in the quantum state given as an argument."
             ]
@@ -1563,14 +1690,15 @@
                 "print(\"axis\", axis.get_vector())\n",
                 "print(\"reflected\", state.get_vector())\n",
                 "gate.update_quantum_state(state)\n",
                 "print(\"two reflection\", state.get_vector())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### General gate\n",
                 "This is a quantum gate with a gate matrix.\n",
                 "\n",
                 "### Dense matrix gate\n",
@@ -1629,14 +1757,15 @@
                 "\n",
                 "# 2-qubit gate\n",
                 "gate = DenseMatrix([0,1], [[1,0,0,0],[0,1,0,0],[0,0,0,1],[0,0,1,0]])\n",
                 "print(gate)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Sparse matrix gate\n",
                 "A gate defined based on a sparse matrix. If the elements are sparse enough, they can be updated faster than a dense matrix. Define sparse matrices using scipy's `csc_matrix`."
             ]
         },
@@ -1683,14 +1812,15 @@
                 "qs = QuantumState(2)\n",
                 "qs.load([1,2,3,4])\n",
                 "gate.update_quantum_state(qs)\n",
                 "print(qs.get_vector())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Add control bit\n",
                 "General gates can add a control qubit using the `add_control_qubit` function. You can also specify whether the target qubit has an effect when control qubit is 0 or 1."
             ]
         },
@@ -1743,14 +1873,15 @@
                 "print(state.get_vector())\n",
                 "\n",
                 "x_mat_gate.update_quantum_state(state)\n",
                 "print(state.get_vector())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Operation to create a new gate from multiple gates\n",
                 "### Gate product\n",
                 "Combine successively the operating quantum gates to create a new single quantum gate. This reduces access to quantum states."
             ]
@@ -1798,14 +1929,15 @@
                 "# Create the new gate by combining gates\n",
                 "# The gate in the first augement is applied first\n",
                 "x_and_ry_gate = merge(x_gate, ry_gate)\n",
                 "print(x_and_ry_gate)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Gate sum\n",
                 "You can add multiple gates to create a new gate. This is useful for making the projection of the Pauli operator $P$ onto the +1 eigenvalue space such as $(I + P) / 2$."
             ]
         },
@@ -1870,14 +2002,15 @@
                 "proj_00_plus_11 = merge(gate_ii_zz, gate_ii_xx)\n",
                 "# ((|00>+|11>)(<00|+<11|))/2 = (II + ZZ)(II + XX)/4\n",
                 "proj_00_plus_11.multiply_scalar(0.25)\n",
                 "print(proj_00_plus_11)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Random unitary\n",
                 "Use the `RandomUnitary` function to sample a random unitary matrix with the Haar measure and generate a dense matrix gate."
             ]
         },
@@ -1914,14 +2047,15 @@
                 "from qulacs.gate import RandomUnitary\n",
                 "target_list = [2,3]\n",
                 "gate = RandomUnitary(target_list)\n",
                 "print(gate)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Stochastic operation\n",
                 "Using the `Probabilistic` function, create the stochastic operation by giving multiple gate operations and probability distribution. If the sum of the given probability distributions is less than 1, `Identity` will operate with a probability less than 1."
             ]
         },
@@ -1968,14 +2102,15 @@
                 "state = QuantumState(2)\n",
                 "for _ in range(10):\n",
                 "    gate.update_quantum_state(state)\n",
                 "    print(state.get_vector())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "`BitFlipNoise`, `DephasingNoise`, `IndependentXZNoise`, `DepolarizingNoise`, and `TwoQubitDepolarizingNoise` gates are defined as stochastic gates. `Probabilistic` instances are generated by entering the error probabilities."
             ]
         },
         {
@@ -2015,14 +2150,15 @@
                 "state = QuantumState(2)\n",
                 "for _ in range(10):\n",
                 "    gate.update_quantum_state(state)\n",
                 "    print(state.get_vector())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Noisy evolution\n",
                 "There are two gates, `NoisyEvolution` and `NoisyEvolution_fast`, that interact from the environment and are attenuated by time evolution.\n",
                 "They can be used by the following steps\n",
                 "\n",
@@ -3090,14 +3226,15 @@
                 "   H(1).update_quantum_state(state)\n",
                 "   gate.update_quantum_state(state)\n",
                 "   exp += observable.get_expectation_value(state) / n_samples\n",
                 "   print(f\"[{k}] exp: {exp}\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### CPTP mapping\n",
                 "`CPTP` is created by giving a list of Claus operators that satisfy the completeness."
             ]
         },
@@ -3141,14 +3278,15 @@
                 "    state.set_zero_state()\n",
                 "    merge(H(0),H(1)).update_quantum_state(state)\n",
                 "    gate.update_quantum_state(state)\n",
                 "    print(state.get_vector())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The `AmplitudeDampingNoise` gate is defined as CPTP-map."
             ]
         },
         {
@@ -3180,14 +3318,15 @@
                 "target = 0\n",
                 "damping_rate = 0.1\n",
                 "AmplitudeDampingNoise(target, damping_rate) \n",
                 "#K_0: [[1,0],[0,sqrt(1-p)]], K_1: [[0,sqrt(p)], [0,0]]"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Instrument\n",
                 "Instrument is an operation to get the index of the Claus operator that acts randomly in addition to the general CPTP-map operation. For example, measurement on the Z basis is equivalent to applying a CPTP-map consisting of `P0` and `P1` and knowing which one has acted. In cppsim, this is achieved in the `Instrument` function, by specifying the information of the CPTP-map and the address of the classic register in which the index of the operated Claus operator is written."
             ]
         },
@@ -3234,14 +3373,15 @@
                 "    merge(H(0),H(1)).update_quantum_state(state)\n",
                 "    gate.update_quantum_state(state)\n",
                 "    result = state.get_classical_value(classical_pos)\n",
                 "    print(index, format(result,\"b\").zfill(2), state.get_vector())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Note that `Measurement` gate is defined as Instrument."
             ]
         },
         {
@@ -3253,14 +3393,15 @@
                 "from qulacs.gate import Measurement\n",
                 "target = 0\n",
                 "classical_pos = 0\n",
                 "gate = Measurement(target, classical_pos)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Adaptive operation\n",
                 "This is a gate that uses a function that returns a Boolean value with variable-length list of classical register values as an argument, and determines whether to perform an operation according to the conditions obtained from the classical register. Conditions can be written as python functions. A python function must be a function that takes a list of type `int` as an argument and returns a bool type value."
             ]
         },
@@ -3301,14 +3442,15 @@
                 "# func returns True, so X operates\n",
                 "state.set_classical_value(0,1)\n",
                 "gate.update_quantum_state(state)\n",
                 "print(state.get_vector())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Operator\n",
                 "\n",
                 "### Pauli operator\n",
                 "Observables are represented as linear combinations of Pauli operators with real coefficients. `PauliOperator` class is a class that expresses each term with the coefficient added to the $n$-qubit Pauli operator. Unlike gates, operator cannot update quantum states.\n",
@@ -3354,14 +3496,15 @@
                 "pauli_str = [s[i] for i in pauli_id_list]\n",
                 "terms_str = [item[0]+str(item[1]) for item in zip(pauli_str,index_list)]\n",
                 "full_str = str(coef) + \" \" + \" \".join(terms_str)\n",
                 "print(full_str)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Expected value of Pauli operator\n",
                 "You can evaluate the expected value and transition moment of the Pauli operator for one state."
             ]
         },
@@ -3398,14 +3541,15 @@
                 "bra = QuantumState(n)\n",
                 "bra.set_Haar_random_state()\n",
                 "value = pauli.get_transition_amplitude(bra, state)\n",
                 "print(\"transition\", value)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### General linear operators\n",
                 "The linear operator `GeneralQuantumOperator` is represented by a linear combination of the Pauli operators with a complex coefficient. `PauliOperator` with coefficient can be added as a term with `add_operator`."
             ]
         },
@@ -3460,15 +3604,14 @@
                 "bra = QuantumState(n)\n",
                 "bra.set_Haar_random_state()\n",
                 "value = operator.get_transition_amplitude(bra, state)\n",
                 "print(\"transition\", value)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Store linear operators\n",
                 "`GeneralQuantumOperator` can be converted to/from JSON string."
             ]
         },
@@ -3497,14 +3640,15 @@
                 "print(\"original:\", o_operator)\n",
                 "\n",
                 "r_operator = quantum_operator.from_json(operator_json)\n",
                 "print(\"restored:\", r_operator)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Generation of observables using OpenFermion\n",
                 "`OpenFermion` is a tool that gives Hamiltonian to be solved by chemical calculation in the form of Pauli operator. The output of this tool can be read in the form of a file or a string and can be used in the form of an operator."
             ]
         },
@@ -3547,22 +3691,24 @@
                 "operator = create_quantum_operator_from_openfermion_text(open_fermion_text)\n",
                 "print(operator.get_term_count())\n",
                 "print(operator.get_qubit_count())\n",
                 "# In the case of create_quantum_operator_from_openfermion_file, specify the path of the file where the above is written in the argument."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Hermite operator / observable\n",
                 "The Hermite operator is represented by a real linear combination of the Pauli operators. Equivalent to the `GeneralQuatnumOperator` class, except that eigenvalues and expected values are guaranteed to be real."
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "The function to read and process from an external file is possible by replacing the `quantum_operator` with the `observable`, and using functions such as `create_observable_from_openfermion_file` `create_observable_from_openfermion_text` `create_split_observable`.\n",
                 "\n",
                 "#### Separates operators into diagonal and off-diagonal terms\n",
                 "When reading an operator from a file, you can separate it into diagonal and off-diagonal components with the `create_split_observable` function."
@@ -3582,14 +3728,15 @@
                 "operator = create_observable_from_openfermion_file(\"./H2.txt\")\n",
                 "diag, nondiag = create_split_observable(\"./H2.txt\")\n",
                 "print(operator.get_term_count(), diag.get_term_count(), nondiag.get_term_count())\n",
                 "print(operator.get_qubit_count(), diag.get_qubit_count(), nondiag.get_qubit_count())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "#### Compute ground state\n",
                 "You can compute a ground state of the operator by power method, Arnoldi method or Lanczos method. After computation, the corresponding ground state is assigned to `state` in the argument.\n",
                 "\n",
                 "##### Power method"
@@ -3609,14 +3756,15 @@
                 "state = QuantumState(n)\n",
                 "state.set_Haar_random_state()\n",
                 "value = operator.solve_ground_state_eigenvalue_by_power_method(state, 50)\n",
                 "print(value)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "##### Arnoldi method"
             ]
         },
         {
@@ -3633,14 +3781,15 @@
                 "state = QuantumState(n)\n",
                 "state.set_Haar_random_state()\n",
                 "value = operator.solve_ground_state_eigenvalue_by_arnoldi_method(state, 50)\n",
                 "print(value)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "##### Lanczos method"
             ]
         },
         {
@@ -3657,14 +3806,15 @@
                 "state = QuantumState(n)\n",
                 "state.set_Haar_random_state()\n",
                 "value = operator.solve_ground_state_eigenvalue_by_lanczos_method(state, 50)\n",
                 "print(value)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Apply to a quantum state\n",
                 "An operator can be applied to a quantum state."
             ]
         },
@@ -3684,14 +3834,15 @@
                 "result = QuantumState(n)\n",
                 "work_state = QuantumState(n)\n",
                 "operator.apply_to_state(work_state, state, result)\n",
                 "print(result)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Quantum Circuits\n",
                 "\n",
                 "### Structure of a quantum circuit\n",
                 "A quantum circuit is represented as a set of quantum gates. For example, a quantum circuit can be configured as follows."
@@ -3731,14 +3882,72 @@
                 "# Operate quantum circuit to state\n",
                 "circuit.update_quantum_state(state)\n",
                 "\n",
                 "print(state.get_vector())"
             ]
         },
         {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "### Further operations on a quantum circuit\n",
+                "You can add gates at specific positions to a quantum circuit and perform operations such as ```copy``` and ```merge_circuit```. Here is the code that summarizes these operations."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "qubit count = 3\n",
+                        "gate count = 3\n",
+                        "[ 0.+0.j -1.-0.j  0.+0.j -0.-0.j  0.+0.j -0.-0.j  0.+0.j -0.-0.j]\n"
+                    ]
+                }
+            ],
+            "source": [
+                "from qulacs import QuantumCircuit, QuantumState\n",
+                "from qulacs.gate import H, Z\n",
+                "\n",
+                "n = 3\n",
+                "state = QuantumState(n)\n",
+                "state.set_zero_state()\n",
+                "\n",
+                "circuit = QuantumCircuit(n)\n",
+                "\n",
+                "circuit.add_gate(Z(0))\n",
+                "\n",
+                "# add a gate at the specified position\n",
+                "for i in range(n):\n",
+                "    circuit.add_gate(H(i), i)\n",
+                "\n",
+                "circuit.remove_gate(1)\n",
+                "\n",
+                "print(f\"qubit count = {circuit.get_qubit_count()}\")\n",
+                "\n",
+                "print(f\"gate count = {circuit.get_gate_count()}\")\n",
+                "\n",
+                "# get a deep copy of a quantum circuit.\n",
+                "copy_circuit = circuit.copy()\n",
+                "\n",
+                "# merge the gates of the provided quantum circuit as arguments\n",
+                "# modifying the merged side does not affect the side that has been merged\n",
+                "circuit.merge_circuit(copy_circuit)\n",
+                "\n",
+                "circuit.update_quantum_state(state)\n",
+                "print(state.get_vector())"
+            ]
+        },
+        {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Calculation and optimization of depth of quantum circuits\n",
                 "By combining quantum gates into a single quantum gate, the number of quantum gates and the time required for numerical calculations can be reduced. (Of course, if the number of target qubits increases, or if a quantum gate with a dedicated function is synthesized into a quantum gate without a dedicated function, the total calculation time may not decrease. It depends.)\n",
                 "\n",
                 "The code below uses the `optimize` function to repeat the greedy synthesis of the quantum gate of the quantum circuit until the target qubit becomes three."
@@ -3778,14 +3987,15 @@
                 "opt.optimize(circuit, max_block_size)\n",
                 "\n",
                 "# Calculate the depth (depth=1\u3078)\n",
                 "print(circuit.calculate_depth())"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "###  Debugging quantum circuits\n",
                 "When print a quantum circuit, statistical information about the gates included in the quantum circuit will be displayed."
             ]
         },
@@ -3820,15 +4030,14 @@
                 "    for i in range(n):\n",
                 "        circuit.add_H_gate(i)\n",
                 "\n",
                 "print(circuit)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Store QuantumCircuit\n",
                 "`QuantumCircuit` can be converted to/from JSON string.\n",
                 "If it has unsupported gates, the conversion fails with an error."
             ]
@@ -3877,15 +4086,14 @@
                 "print(o_circuit)\n",
                 "\n",
                 "r_circuit = circuit.from_json(circuit_json)\n",
                 "print(r_circuit)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Quantum circuits can be stored to files in pickle format."
             ]
         },
         {
@@ -3908,14 +4116,15 @@
                 "\n",
                 "# load\n",
                 "with open('circuit.pickle', 'rb') as f:\n",
                 "    circuit = pickle.load(f)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Parametric Quantum Circuits\n",
                 "Defining a quantum circuit as a `ParametricQuantumCircuit` class enables some functions that are useful for optimizing quantum circuits using variational methods, in addition to the usual functions of the `QuantumCircuit` class.\n",
                 "\n",
                 "### Application examples of parametric quantum circuits\n",
@@ -4025,14 +4234,15 @@
                 "\n",
                 "# output state and circuit info\n",
                 "print(state)\n",
                 "print(circuit)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Compute a gradient of parametric quantum circuit\n",
                 "You can compute a gradient of parametric circuit by `GradCalculator` or `ParametricQuantumCircuit.backprop()`.\n",
                 "\n",
                 "- In `GradCalculator`, compute a gradient by calculating expected value with `CausalConeSimulator`.\n",
@@ -4073,15 +4283,14 @@
                 "# \u7b2c\u4e09\u5f15\u6570\u306b\u56de\u8ee2\u89d2\u3092\u6307\u5b9a\u3059\u308b\u3053\u3068\u3082\u53ef\u80fd\n",
                 "print(gcalc.calculate_grad(circuit, observable, theta))\n",
                 "# Backprop\u3092\u4f7f\u3063\u3066\u6c42\u3081\u305f\u5834\u5408\n",
                 "print(circuit.backprop(observable))"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### Store parametric quantum circuits\n",
                 "\n",
                 "Parametric quantum circuits can be converted to/from JSON string.\n",
                 "If it has unsupported gates, the conversion fails with an error."
@@ -4137,15 +4346,14 @@
                 "print(o_circuit)\n",
                 "\n",
                 "r_circuit = circuit.from_json(circuit_json)\n",
                 "print(r_circuit)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Parametric quantum circuits can be converted to files in pickle format."
             ]
         },
         {
@@ -4168,14 +4376,15 @@
                 "\n",
                 "# load\n",
                 "with open('circuit.pickle', 'rb') as f:\n",
                 "    circuit = pickle.load(f)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Simulator\n",
                 "### `QuantumCircuitSimulator`\n",
                 "You can manage a circuit and quantum states together. It has a buffer for quantum state to swap the state to use."
             ]
@@ -4293,14 +4502,15 @@
                 "# \u91cf\u5b50\u72b6\u614b\u3092\u30b3\u30d4\u30fc\uff08\u73fe\u72b6\u614b->\u30d0\u30c3\u30d5\u30a1\uff09\n",
                 "sim.copy_state_to_buffer()\n",
                 "sim.simulate()\n",
                 "print(state)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### `NoiseSimulator`\n",
                 "The `NoiseSimulator` allows you to run your circuit in a simulated noise environment.\n",
                 "\n",
                 "To set up noise, you should add a gate to the circuit using `add_noise_gate()`.\n",
@@ -4364,14 +4574,15 @@
                 "state.set_Haar_random_state()\n",
                 "sim = NoiseSimulator(circuit, state)\n",
                 "sim.execute(100)\n",
                 "print(state)"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "### `CausalConeSimulator`\n",
                 "`CausalConeSimulator` allows you to extract the gates associated with a given observable by traversing the circuit in reverse.\n",
                 "Only the extracted gates can be applied to obtain the expected value of the physical quantity.\n",
                 "\n",
@@ -4418,15 +4629,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "version": "3.9.16"
         },
         "vscode": {
             "interpreter": {
                 "hash": "949777d72b0d2535278d3dc13498b2535136f6dfe0678499012e853ee9abcab1"
             }
         }
     },
```

### Comparing `qulacs-0.6.0/doc/en/source/index.md` & `qulacs-0.6.1/doc/en/source/index.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/intro/0_about.md` & `qulacs-0.6.1/doc/en/source/intro/0_about.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/intro/1_install.md` & `qulacs-0.6.1/doc/en/source/intro/1_install.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/intro/2_faq.md` & `qulacs-0.6.1/doc/en/source/intro/2_faq.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/intro/3_usage.md` & `qulacs-0.6.1/doc/en/source/intro/3_usage.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/intro/4.1_python_tutorial.ipynb` & `qulacs-0.6.1/doc/en/source/intro/4.1_python_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/intro/4.2_cpp_tutorial.md` & `qulacs-0.6.1/doc/en/source/intro/4.2_cpp_tutorial.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/en/source/write/0_readme.md` & `qulacs-0.6.1/doc/en/source/write/0_readme.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/ja/Makefile` & `qulacs-0.6.1/doc/ja/Makefile`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/ja/make.bat` & `qulacs-0.6.1/doc/ja/make.bat`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/ja/source/_static/images/dojo.png` & `qulacs-0.6.1/doc/ja/source/_static/images/dojo.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/ja/source/_static/images/github.png` & `qulacs-0.6.1/doc/ja/source/_static/images/github.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/ja/source/_static/images/logo-c-h.png` & `qulacs-0.6.1/doc/ja/source/_static/images/logo-c-h.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/ja/source/_static/images/slack.png` & `qulacs-0.6.1/doc/ja/source/_static/images/slack.png`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/class.rst` & `qulacs-0.6.1/doc/ja/source/_templates/autoapi/python/class.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/data.rst` & `qulacs-0.6.1/doc/ja/source/_templates/autoapi/python/data.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/function.rst` & `qulacs-0.6.1/doc/ja/source/_templates/autoapi/python/function.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/method.rst` & `qulacs-0.6.1/doc/ja/source/_templates/autoapi/python/method.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/ja/source/_templates/autoapi/python/module.rst` & `qulacs-0.6.1/doc/ja/source/_templates/autoapi/python/module.rst`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/ja/source/conf.py` & `qulacs-0.6.1/doc/ja/source/conf.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,77 +1,76 @@
+import os
+
 import qulacs
 
 project = "Qulacs"
 
-language = 'ja'
-locale_dirs = ['locale/']
+language = "ja"
+locale_dirs = ["locale/"]
 
 # The `extensions` list should already be in here from `sphinx-quickstart`
 extensions = [
     # there may be others here already, e.g. 'sphinx.ext.mathjax'
-    'breathe',
-    'exhale',
-    'myst_parser',
-    'nbsphinx',
-    'sphinx.ext.mathjax',
-    'sphinx_copybutton',
-    'sphinx.ext.napoleon',
-    'sphinx.ext.autodoc',
-    'sphinx.ext.graphviz',
-    'sphinx.ext.inheritance_diagram',
-    'autoapi.extension',
+    "breathe",
+    "exhale",
+    "myst_parser",
+    "nbsphinx",
+    "sphinx.ext.mathjax",
+    "sphinx_copybutton",
+    "sphinx.ext.napoleon",
+    "sphinx.ext.autodoc",
+    "sphinx.ext.graphviz",
+    "sphinx.ext.inheritance_diagram",
+    "autoapi.extension",
 ]
 
-exclude_patterns = ['_build', '**.ipynb_checkpoints']
+exclude_patterns = ["_build", "**.ipynb_checkpoints"]
 nbsphinx_allow_errors = True
 myst_enable_extensions = [
     "dollarmath",
 ]
 
 
 # source files for shpinx
 source_suffix = {
-    '.rst': 'restructuredtext',
-    '.txt': 'markdown',
-    '.md': 'markdown',
+    ".rst": "restructuredtext",
+    ".txt": "markdown",
+    ".md": "markdown",
 }
 
 # Setup the breathe extension
-breathe_projects = {
-    "Docs": "./xml"
-}
+breathe_projects = {"Docs": "./xml"}
 
 breathe_default_project = "Docs"
 
 # Setup the exhale extension
 exhale_args = {
     # These arguments are required
-    "containmentFolder":     "./api",
-    "rootFileName":          "cpp_library_root.rst",
-    "rootFileTitle":         "C++ APIリファレンス",
-    "doxygenStripFromPath":  "..",
+    "containmentFolder": "./api",
+    "rootFileName": "cpp_library_root.rst",
+    "rootFileTitle": "C++ APIリファレンス",
+    "doxygenStripFromPath": "..",
     # Suggested optional arguments
-    "createTreeView":        True,
+    "createTreeView": True,
     # TIP: if using the sphinx-bootstrap-theme, you need
     # "treeViewIsBootstrap": True,
     "exhaleExecutesDoxygen": True,
-    "exhaleDoxygenStdin": \
-        "INPUT = ../../../src/cppsim ../../../src/vqcsim \n \
+    "exhaleDoxygenStdin": "INPUT = ../../../src/cppsim ../../../src/vqcsim \n \
         OUTPUT_LANGUAGE = Japanese-en \n \
         FILE_PATTERNS          = *.hpp \n \
         WARN_IF_UNDOCUMENTED   = NO \n \
         ENABLE_PREPROCESSING   = YES \n \
         MACRO_EXPANSION        = YES \n \
         PREDEFINED             += __attribute__(x)= \n \
         PREDEFINED             += DllExport= \n \
         GENERATE_LEGEND        = YES \n \
         GRAPHICAL_HIERARCHY    = YES \n \
         CLASS_GRAPH            = YES \n \
         HIDE_UNDOC_RELATIONS   = YES\n \
-        CLASS_DIAGRAMS         = YES\n"
+        CLASS_DIAGRAMS         = YES\n",
 }
 
 autoapi_type = "python"
 autoapi_keep_files = True
 autoapi_root = "pyRef"
 # The order of `autoapi_file_patterns`` specifies the order of preference for reading files.
 # So, we give priority to `*.pyi`.
@@ -87,51 +86,50 @@
     "undoc-members",
     "show-inheritance",
     "show-module-summary",
     "imported-members",
 ]
 
 # Tell sphinx what the primary language being documented is.
-#primary_domain = 'cpp'
+# primary_domain = 'cpp'
 
 # Tell sphinx what the pygments highlight language should be.
-#highlight_language = 'cpp'
+# highlight_language = 'cpp'
 
 #
 
 # on_rtd is whether we are on readthedocs.org, this line of code grabbed from docs.readthedocs.org
-import os
-
-on_rtd = os.environ.get('READTHEDOCS', None) == 'True'
+on_rtd = os.environ.get("READTHEDOCS", None) == "True"
 
 if not on_rtd:  # only import and set the theme if we're building docs locally
     import sphinx_rtd_theme
-    html_theme = 'sphinx_rtd_theme'
+
+    html_theme = "sphinx_rtd_theme"
     html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
 
 
 html_theme_options = {
     # 'canonical_url': '',
     # 'analytics_id': 'UA-XXXXXXX-1',  #  Provided by Google in your dashboard
-    'logo_only': False,
+    "logo_only": False,
     # 'display_version': True,
-    'prev_next_buttons_location': 'bottom',
-    'style_external_links': False,
+    "prev_next_buttons_location": "bottom",
+    "style_external_links": False,
     # 'vcs_pageview_mode': '',
-    'style_nav_header_background': '#004659',
+    "style_nav_header_background": "#004659",
     # Toc options
-    'collapse_navigation': True,
-    'sticky_navigation': True,
-    'navigation_depth': 2,
-    'includehidden': True,
-    'titles_only': False
+    "collapse_navigation": True,
+    "sticky_navigation": True,
+    "navigation_depth": 2,
+    "includehidden": True,
+    "titles_only": False,
 }
 
 templates_path = ["_templates"]
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
-copyright = '2018 Qulacs Authors'
+copyright = "2018 Qulacs Authors"
 
 # `version` is only used for local build.
 # On Read the Docs, the latest version is `latest`` and the specific version
 # is the Git tag name.
 version = qulacs._version.__version__
```

### Comparing `qulacs-0.6.0/doc/ja/source/guide/2.0_python_advanced.md` & `qulacs-0.6.1/doc/ja/source/guide/2.0_python_advanced.md`

 * *Files 2% similar despite different names*

```diff
@@ -884,14 +884,86 @@
  * Pauli     : yes
  * Clifford  : yes
  * Gaussian  : no
  * Parametric: no
  * Diagonal  : no
 ```
 
+量子ゲートは`copy`関数で自身と同じインスタンスを新たに生成できます。
+```python
+import numpy as np
+from qulacs.gate import X
+
+# Xゲートを生成する
+n = 2
+initial_gate = X(n)
+print(initial_gate)
+
+# ゲートをコピーする
+copied_gate = initial_gate.copy()
+print(copied_gate)
+```
+```
+ *** gate info *** 
+ * gate name : X
+ * target    : 
+ 2 : commute X     
+ * control   : 
+ * Pauli     : yes
+ * Clifford  : yes
+ * Gaussian  : no
+ * Parametric: no
+ * Diagonal  : no
+
+ *** gate info *** 
+ * gate name : X
+ * target    : 
+ 2 : commute X     
+ * control   : 
+ * Pauli     : yes
+ * Clifford  : yes
+ * Gaussian  : no
+ * Parametric: no
+ * Diagonal  : no
+
+```
+
+量子ゲートによって量子状態を変更するには`update_quantum_state`関数を用います。
+例えば、Hゲートを0-th qubitに作用させるには以下のようなコードを書きます。
+```python
+import qulacs
+from qulacs.gate import H
+
+n = 2
+quantum_state = qulacs.QuantumState(n)
+
+# |00>に初期化する
+quantum_state.set_zero_state()
+
+# Hゲートを生成する
+hadamard_gate = H(0)
+
+# Hゲートを作用させる
+hadamard_gate.update_quantum_state(quantum_state)
+
+# 量子状態を表示する
+print(quantum_state)
+```
+
+```
+ *** Quantum State ***
+ * Qubit Count : 2
+ * Dimension   : 4
+ * State vector : 
+(0.707107,0)
+(0.707107,0)
+       (0,0)
+       (0,0)
+```
+
 ### 特殊ゲート
 
 下記に特殊ゲートを列挙します。
 
 #### 1量子ビットゲート
 
 第一引数に対象ビットの添え字を取ります。
@@ -2008,14 +2080,58 @@
 ```
 
 ```
 [ 0.35355339+0.j -0.35355339-0.j -0.35355339-0.j  0.35355339+0.j
  -0.35355339-0.j  0.35355339+0.j  0.35355339+0.j -0.35355339-0.j]
 ```
 
+### 量子回路のさらなる操作
+量子回路に対して指定位置にゲートを追加したり、```copy```や```merge_circuit```などの操作も行うことが出来る。以下にそれらをまとめたコードを記載する。
+```python
+from qulacs import QuantumCircuit, QuantumState
+from qulacs.gate import H, Z
+
+n = 3
+state = QuantumState(n)
+state.set_zero_state()
+
+circuit = QuantumCircuit(n)
+
+circuit.add_gate(Z(0))
+
+# ゲートは回路の指定した位置に追加できる
+for i in range(n):
+    circuit.add_gate(H(i), i)
+
+# 指定した位置のゲートを削除する
+circuit.remove_gate(1)
+
+# qubitの個数を得る
+print(f"qubit count = {circuit.get_qubit_count()}")
+
+# gateの個数を得る
+print(f"gate count = {circuit.get_gate_count()}")
+
+# 量子回路のディープコピーを行う
+copy_circuit = circuit.copy()
+
+# 引数で与えた量子回路のゲートをマージする
+# マージした側を変更してもマージされた側に変更はない
+circuit.merge_circuit(copy_circuit)
+
+circuit.update_quantum_state(state)
+print(state.get_vector())
+
+```
+```
+qubit count = 3
+gate count = 3
+[ 0.+0.j -1.-0.j  0.+0.j -0.-0.j  0.+0.j -0.-0.j  0.+0.j -0.-0.j]s
+```
+
 ### 量子回路のdepthの計算と最適化
 
 量子ゲートをまとめて一つの量子ゲートとすることで、量子ゲートの数を減らすことができ、数値計算の時間を短縮できることがあります。
 （もちろん、対象となる量子ビットの数が増える場合や、専用関数を持つ量子ゲートを合成して専用関数を持たない量子ゲートにしてしまった場合は、トータルで計算時間が減少するかは状況に依ります。）
 
 下記のコードでは `optimize` 関数を用いて、量子回路の量子ゲートをターゲットとなる量子ビットが3つになるまで貪欲法で合成を繰り返します。
```

### Comparing `qulacs-0.6.0/doc/ja/source/index.md` & `qulacs-0.6.1/doc/ja/source/index.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/ja/source/intro/0_about.md` & `qulacs-0.6.1/doc/ja/source/intro/0_about.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/ja/source/intro/1_install.md` & `qulacs-0.6.1/doc/ja/source/intro/1_install.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/ja/source/intro/2_faq.md` & `qulacs-0.6.1/doc/ja/source/intro/2_faq.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/ja/source/intro/3_usage.md` & `qulacs-0.6.1/doc/ja/source/intro/3_usage.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/ja/source/intro/4.1_python_tutorial.md` & `qulacs-0.6.1/doc/ja/source/intro/4.1_python_tutorial.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/ja/source/intro/4.2_cpp_tutorial.md` & `qulacs-0.6.1/doc/ja/source/intro/4.2_cpp_tutorial.md`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/scripts/customdoxygen.css` & `qulacs-0.6.1/doc/scripts/customdoxygen.css`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/scripts/doxy-boot.js` & `qulacs-0.6.1/doc/scripts/doxy-boot.js`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/scripts/footer.html` & `qulacs-0.6.1/doc/scripts/footer.html`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/scripts/header.html` & `qulacs-0.6.1/doc/scripts/header.html`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/doc/scripts/index.html` & `qulacs-0.6.1/doc/scripts/index.html`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/pyproject.toml` & `qulacs-0.6.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -36,27 +36,33 @@
 [project.urls]
 homepage = "http://www.qulacs.org"
 
 [project.optional-dependencies]
 dev = [
     "black",
     "flake8",
-    "openfermion",
+    "isort",
     "mypy",
-    "pybind11-stubgen"
+    "pybind11-stubgen",
+    "openfermion",
+    "pytest"
 ]
 
 test = [
     "openfermion"
 ]
 
 ci = [
-    "openfermion",
+    "black",
+    "flake8",
+    "isort",
     "mypy",
-    "pybind11-stubgen"
+    "pybind11-stubgen",
+    "openfermion",
+    "pytest"
 ]
 
 doc = [
     "sphinx == 4.5.0",
     "sphinx-rtd-theme == 1.0.*",
     "breathe == 4.33.*",
     "exhale == 0.3.*",
@@ -69,16 +75,16 @@
 
 [tool.setuptools]
 include-package-data = true
 zip-safe = false
 
 [tool.cibuildwheel]
 build-verbosity = "1"
-test-command = "python {project}/python/test/test_qulacs.py"
-test-requires = "numpy scipy openfermion"
+test-command = "pytest -v -s {project}/python/tests"
+test-requires = "pytest numpy scipy openfermion"
 
 [tool.cibuildwheel.linux]
 environment = { QULACS_OPT_FLAGS = "-mtune=haswell -mfpmath=both" }
 before-build = """\
 yum install wget -y && \
 wget -q https://boostorg.jfrog.io/artifactory/main/release/1.76.0/source/boost_1_76_0.tar.gz && \
 tar -zxf boost_1_76_0.tar.gz && \
@@ -93,7 +99,16 @@
 [tool.cibuildwheel.macos]
 before-build = """\
 brew upgrade && brew install -f boost && \
 brew link boost && rm -rf {project}/build\
 """
 archs = ["x86_64", "arm64"]
 repair-wheel-command = "delocate-listdeps {wheel} && script/fix_wheel_osx.sh {wheel} {dest_dir} && delocate-listdeps {wheel}"
+
+[tool.isort]
+default_section = "THIRDPARTY"
+ensure_newline_before_comments = true
+force_grid_wrap = 0
+force_single_line = false
+include_trailing_comma = true
+multi_line_output = 3
+use_parentheses = true
```

### Comparing `qulacs-0.6.0/pysrc/qulacs/__init__.pyi` & `qulacs-0.6.1/pysrc/qulacs/__init__.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """cppsim python interface"""
 from __future__ import annotations
-import qulacs_core
+
 import typing
+
 import numpy
-_Shape = typing.Tuple[int, ...]
+import qulacs_core
+import scipy.sparse
 
 __all__ = [
     "CausalConeSimulator",
     "ClsNoisyEvolution",
     "ClsNoisyEvolution_fast",
     "ClsOneControlOneTargetGate",
     "ClsOneQubitGate",
@@ -41,1034 +43,1128 @@
     "StateVector",
     "check_build_for_mpi",
     "circuit",
     "gate",
     "observable",
     "quantum_operator",
     "state",
-    "to_general_quantum_operator"
+    "to_general_quantum_operator",
 ]
 
-
-class CausalConeSimulator():
-    def __init__(self, arg0: ParametricQuantumCircuit, arg1: Observable) -> None: 
+class CausalConeSimulator:
+    def __init__(self, arg0: ParametricQuantumCircuit, arg1: Observable) -> None:
         """
         Constructor
         """
-    def build(self) -> None: 
+    def build(self) -> None:
         """
         Build
         """
-    def get_circuit_list(self) -> typing.List[typing.List[ParametricQuantumCircuit]]: 
+    def get_circuit_list(self) -> typing.List[typing.List[ParametricQuantumCircuit]]:
         """
         Return circuit_list
         """
-    def get_coef_list(self) -> typing.List[complex]: 
+    def get_coef_list(self) -> typing.List[complex]:
         """
         Return coef_list
         """
-    def get_expectation_value(self) -> complex: 
+    def get_expectation_value(self) -> complex:
         """
         Return expectation_value
         """
-    def get_pauli_operator_list(self) -> typing.List[typing.List[PauliOperator]]: 
+    def get_pauli_operator_list(self) -> typing.List[typing.List[PauliOperator]]:
         """
         Return pauli_operator_list
         """
     pass
-class QuantumGateBase():
+
+class QuantumGateBase:
     def __str__(self) -> str: ...
-    def copy(self) -> QuantumGateBase: 
+    def copy(self) -> QuantumGateBase:
         """
         Create copied instance
         """
-    def get_control_index_list(self) -> typing.List[int]: 
+    def get_control_index_list(self) -> typing.List[int]:
         """
         Get control qubit index list
         """
-    def get_control_index_value_list(self) -> typing.List[typing.Tuple[int, int]]: 
+    def get_control_index_value_list(self) -> typing.List[typing.Tuple[int, int]]:
         """
         Get control qubit pair index value list
         """
-    def get_control_value_list(self) -> typing.List[int]: 
+    def get_control_value_list(self) -> typing.List[int]:
         """
         Get control qubit value list
         """
-    def get_inverse(self) -> QuantumGateBase: 
+    def get_inverse(self) -> QuantumGateBase:
         """
         get inverse gate
         """
-    def get_matrix(self) -> numpy.ndarray[numpy.complex128, _Shape[m, n]]: 
+    def get_matrix(self) -> numpy.ndarray:
         """
         Get gate matrix
         """
-    def get_name(self) -> str: 
+    def get_name(self) -> str:
         """
         Get gate name
         """
-    def get_target_index_list(self) -> typing.List[int]: 
+    def get_target_index_list(self) -> typing.List[int]:
         """
         Get target qubit index list
         """
-    def is_Clifford(self) -> bool: 
+    def is_Clifford(self) -> bool:
         """
         Check this gate is element of Clifford group
         """
-    def is_Gaussian(self) -> bool: 
+    def is_Gaussian(self) -> bool:
         """
         Check this gate is element of Gaussian group
         """
-    def is_Pauli(self) -> bool: 
+    def is_Pauli(self) -> bool:
         """
         Check this gate is element of Pauli group
         """
-    def is_commute(self, gate: QuantumGateBase) -> bool: 
+    def is_commute(self, gate: QuantumGateBase) -> bool:
         """
         Check this gate commutes with a given gate
         """
-    def is_diagonal(self) -> bool: 
+    def is_diagonal(self) -> bool:
         """
         Check the gate matrix is diagonal
         """
-    def is_parametric(self) -> bool: 
+    def is_parametric(self) -> bool:
         """
         Check this gate is parametric gate
         """
-    def to_json(self) -> str: 
+    def to_json(self) -> str:
         """
         to json string
         """
-    def to_string(self) -> str: 
+    def to_string(self) -> str:
         """
         to string
         """
-    def update_quantum_state(self, state: QuantumStateBase) -> None: 
+    def update_quantum_state(self, state: QuantumStateBase) -> None:
         """
         Update quantum state
         """
     pass
+
 class ClsNoisyEvolution_fast(QuantumGateBase):
     pass
+
 class ClsOneControlOneTargetGate(QuantumGateBase):
     pass
+
 class ClsOneQubitGate(QuantumGateBase):
     pass
+
 class ClsOneQubitRotationGate(QuantumGateBase):
     pass
+
 class ClsPauliGate(QuantumGateBase):
     pass
+
 class ClsPauliRotationGate(QuantumGateBase):
     pass
+
 class ClsReversibleBooleanGate(QuantumGateBase):
     pass
+
 class ClsStateReflectionGate(QuantumGateBase):
     pass
+
 class ClsTwoQubitGate(QuantumGateBase):
     pass
-class QuantumStateBase():
+
+class QuantumStateBase:
     pass
-class GeneralQuantumOperator():
+
+class GeneralQuantumOperator:
     def __IADD__(self, arg0: PauliOperator) -> GeneralQuantumOperator: ...
     @typing.overload
     def __IMUL__(self, arg0: PauliOperator) -> GeneralQuantumOperator: ...
     @typing.overload
     def __IMUL__(self, arg0: complex) -> GeneralQuantumOperator: ...
     def __ISUB__(self, arg0: PauliOperator) -> GeneralQuantumOperator: ...
     @typing.overload
     def __add__(self, arg0: GeneralQuantumOperator) -> GeneralQuantumOperator: ...
     @typing.overload
     def __add__(self, arg0: PauliOperator) -> GeneralQuantumOperator: ...
     def __iadd__(self, arg0: GeneralQuantumOperator) -> GeneralQuantumOperator: ...
     def __imul__(self, arg0: GeneralQuantumOperator) -> GeneralQuantumOperator: ...
-    def __init__(self, qubit_count: int) -> None: 
+    def __init__(self, qubit_count: int) -> None:
         """
         Constructor
         """
     def __isub__(self, arg0: GeneralQuantumOperator) -> GeneralQuantumOperator: ...
     @typing.overload
     def __mul__(self, arg0: GeneralQuantumOperator) -> GeneralQuantumOperator: ...
     @typing.overload
     def __mul__(self, arg0: PauliOperator) -> GeneralQuantumOperator: ...
     @typing.overload
     def __mul__(self, arg0: complex) -> GeneralQuantumOperator: ...
-    def __str__(self) -> str: 
+    def __str__(self) -> str:
         """
         to string
         """
     @typing.overload
     def __sub__(self, arg0: GeneralQuantumOperator) -> GeneralQuantumOperator: ...
     @typing.overload
     def __sub__(self, arg0: PauliOperator) -> GeneralQuantumOperator: ...
     @typing.overload
-    def add_operator(self, coef: complex, pauli_string: str) -> None: 
+    def add_operator(self, pauli_operator: PauliOperator) -> None:
         """
         Add Pauli operator
         """
     @typing.overload
-    def add_operator(self, pauli_operator: PauliOperator) -> None: ...
-    def add_operator_copy(self, pauli_operator: PauliOperator) -> None: 
+    def add_operator(self, coef: complex, pauli_string: str) -> None: ...
+    def add_operator_copy(self, pauli_operator: PauliOperator) -> None:
         """
         Add Pauli operator
         """
-    def add_operator_move(self, pauli_operator: PauliOperator) -> None: 
+    def add_operator_move(self, pauli_operator: PauliOperator) -> None:
         """
         Add Pauli operator
         """
     @typing.overload
-    def apply_to_state(self, state_to_be_multiplied: QuantumStateBase, dst_state: QuantumStateBase) -> None: 
+    def apply_to_state(
+        self,
+        work_state: QuantumStateBase,
+        state_to_be_multiplied: QuantumStateBase,
+        dst_state: QuantumStateBase,
+    ) -> None:
         """
         Apply observable to `state_to_be_multiplied`. The result is stored into `dst_state`.
         """
     @typing.overload
-    def apply_to_state(self, work_state: QuantumStateBase, state_to_be_multiplied: QuantumStateBase, dst_state: QuantumStateBase) -> None: ...
-    def copy(self) -> GeneralQuantumOperator: 
+    def apply_to_state(
+        self, state_to_be_multiplied: QuantumStateBase, dst_state: QuantumStateBase
+    ) -> None: ...
+    def copy(self) -> GeneralQuantumOperator:
         """
         Create copied instance of General Quantum operator class
         """
-    def get_expectation_value(self, state: QuantumStateBase) -> complex: 
+    def get_expectation_value(self, state: QuantumStateBase) -> complex:
         """
         Get expectation value
         """
-    def get_expectation_value_single_thread(self, state: QuantumStateBase) -> complex: 
+    def get_expectation_value_single_thread(self, state: QuantumStateBase) -> complex:
         """
         Get expectation value
         """
-    def get_qubit_count(self) -> int: 
+    def get_matrix(self) -> scipy.sparse.csr_matrix[numpy.complex128]:
+        """
+        Get the Hermitian matrix representation of the observable
+        """
+    def get_qubit_count(self) -> int:
         """
         Get qubit count
         """
-    def get_state_dim(self) -> int: 
+    def get_state_dim(self) -> int:
         """
         Get state dimension
         """
-    def get_term(self, index: int) -> PauliOperator: 
+    def get_term(self, index: int) -> PauliOperator:
         """
         Get Pauli term
         """
-    def get_term_count(self) -> int: 
+    def get_term_count(self) -> int:
         """
         Get count of Pauli terms
         """
-    def get_transition_amplitude(self, state_bra: QuantumStateBase, state_ket: QuantumStateBase) -> complex: 
+    def get_transition_amplitude(
+        self, state_bra: QuantumStateBase, state_ket: QuantumStateBase
+    ) -> complex:
         """
         Get transition amplitude
         """
-    def is_hermitian(self) -> bool: 
+    def is_hermitian(self) -> bool:
         """
         Get is Herimitian
         """
-    def to_json(self) -> str: 
+    def to_json(self) -> str:
         """
         to json string
         """
     pass
-class GradCalculator():
+
+class GradCalculator:
     def __init__(self) -> None: ...
     @typing.overload
-    def calculate_grad(self, parametric_circuit: ParametricQuantumCircuit, observable: Observable) -> typing.List[complex]: 
+    def calculate_grad(
+        self, parametric_circuit: ParametricQuantumCircuit, observable: Observable
+    ) -> typing.List[complex]:
         """
         Calculate Grad
         """
     @typing.overload
-    def calculate_grad(self, parametric_circuit: ParametricQuantumCircuit, observable: Observable, angles_of_gates: typing.List[float]) -> typing.List[complex]: ...
+    def calculate_grad(
+        self,
+        parametric_circuit: ParametricQuantumCircuit,
+        observable: Observable,
+        angles_of_gates: typing.List[float],
+    ) -> typing.List[complex]: ...
     pass
-class NoiseSimulator():
-    def __init__(self, arg0: QuantumCircuit, arg1: QuantumState) -> None: 
+
+class NoiseSimulator:
+    def __init__(self, arg0: QuantumCircuit, arg1: QuantumState) -> None:
         """
         Constructor
         """
-    def execute(self, arg0: int) -> typing.List[int]: 
+    def execute(self, arg0: int) -> typing.List[int]:
         """
         Sampling & Return result [array]
         """
-    def execute_and_get_result(self, arg0: int) -> SimulationResult: 
+    def execute_and_get_result(self, arg0: int) -> SimulationResult:
         """
         Simulate & Return ressult [array of (state, frequency)]
         """
     pass
+
 class Observable(GeneralQuantumOperator):
-    def __init__(self, qubit_count: int) -> None: 
+    def __init__(self, qubit_count: int) -> None:
         """
         Constructor
         """
-    def __str__(self) -> str: 
+    def __str__(self) -> str:
         """
         to string
         """
     @typing.overload
-    def add_operator(self, coef: complex, string: str) -> None: 
+    def add_operator(self, pauli_operator: PauliOperator) -> None:
         """
         Add Pauli operator
         """
     @typing.overload
-    def add_operator(self, pauli_operator: PauliOperator) -> None: ...
-    def add_operator_copy(self, pauli_operator: PauliOperator) -> None: 
+    def add_operator(self, coef: complex, string: str) -> None: ...
+    def add_operator_copy(self, pauli_operator: PauliOperator) -> None:
         """
         Add Pauli operator
         """
-    def add_operator_move(self, pauli_operator: PauliOperator) -> None: 
+    def add_operator_move(self, pauli_operator: PauliOperator) -> None:
         """
         Add Pauli operator
         """
     @typing.overload
-    def add_random_operator(self, operator_count: int) -> None: 
+    def add_random_operator(self, operator_count: int) -> None:
         """
         Add random pauli operator
         """
     @typing.overload
     def add_random_operator(self, operator_count: int, seed: int) -> None: ...
-    def apply_to_state(self, work_state: QuantumStateBase, state_to_be_multiplied: QuantumStateBase, dst_state: QuantumStateBase) -> None: 
+    def apply_to_state(
+        self,
+        work_state: QuantumStateBase,
+        state_to_be_multiplied: QuantumStateBase,
+        dst_state: QuantumStateBase,
+    ) -> None:
         """
         Apply observable to `state_to_be_multiplied`. The result is stored into `dst_state`.
         """
-    def get_expectation_value(self, state: QuantumStateBase) -> float: 
+    def get_expectation_value(self, state: QuantumStateBase) -> float:
         """
         Get expectation value
         """
-    def get_expectation_value_single_thread(self, state: QuantumStateBase) -> float: 
+    def get_expectation_value_single_thread(self, state: QuantumStateBase) -> float:
         """
         Get expectation value
         """
-    def get_qubit_count(self) -> int: 
+    def get_qubit_count(self) -> int:
         """
         Get qubit count
         """
-    def get_state_dim(self) -> int: 
+    def get_state_dim(self) -> int:
         """
         Get state dimension
         """
-    def get_term(self, index: int) -> PauliOperator: 
+    def get_term(self, index: int) -> PauliOperator:
         """
         Get Pauli term
         """
-    def get_term_count(self) -> int: 
+    def get_term_count(self) -> int:
         """
         Get count of Pauli terms
         """
-    def get_transition_amplitude(self, state_bra: QuantumStateBase, state_ket: QuantumStateBase) -> complex: 
+    def get_transition_amplitude(
+        self, state_bra: QuantumStateBase, state_ket: QuantumStateBase
+    ) -> complex:
         """
         Get transition amplitude
         """
-    def solve_ground_state_eigenvalue_by_arnoldi_method(self, state: QuantumStateBase, iter_count: int, mu: complex = 0.0) -> complex: 
+    def solve_ground_state_eigenvalue_by_arnoldi_method(
+        self, state: QuantumStateBase, iter_count: int, mu: complex = 0.0
+    ) -> complex:
         """
         Compute ground state eigenvalue by arnoldi method
         """
-    def solve_ground_state_eigenvalue_by_lanczos_method(self, state: QuantumStateBase, iter_count: int, mu: complex = 0.0) -> complex: 
+    def solve_ground_state_eigenvalue_by_lanczos_method(
+        self, state: QuantumStateBase, iter_count: int, mu: complex = 0.0
+    ) -> complex:
         """
         Compute ground state eigenvalue by lanczos method
         """
-    def solve_ground_state_eigenvalue_by_power_method(self, state: QuantumStateBase, iter_count: int, mu: complex = 0.0) -> complex: 
+    def solve_ground_state_eigenvalue_by_power_method(
+        self, state: QuantumStateBase, iter_count: int, mu: complex = 0.0
+    ) -> complex:
         """
         Compute ground state eigenvalue by power method
         """
     pass
-class QuantumCircuit():
+
+class QuantumCircuit:
     def __getstate__(self) -> str: ...
-    def __init__(self, qubit_count: int) -> None: 
+    def __init__(self, qubit_count: int) -> None:
         """
         Constructor
         """
     def __setstate__(self, arg0: str) -> None: ...
-    def __str__(self) -> str: 
+    def __str__(self) -> str:
         """
         to string
         """
-    def add_CNOT_gate(self, control: int, target: int) -> None: 
+    def add_CNOT_gate(self, control: int, target: int) -> None:
         """
         Add CNOT gate
         """
-    def add_CZ_gate(self, control: int, target: int) -> None: 
+    def add_CZ_gate(self, control: int, target: int) -> None:
         """
         Add CNOT gate
         """
-    def add_FusedSWAP_gate(self, target1: int, target2: int, block_size: int) -> None: 
+    def add_FusedSWAP_gate(self, target1: int, target2: int, block_size: int) -> None:
         """
         Add FusedSWAP gate
         """
-    def add_H_gate(self, index: int) -> None: 
+    def add_H_gate(self, index: int) -> None:
         """
         Add Hadamard gate
         """
-    def add_P0_gate(self, index: int) -> None: 
+    def add_P0_gate(self, index: int) -> None:
         """
         Add projection gate to |0> subspace
         """
-    def add_P1_gate(self, index: int) -> None: 
+    def add_P1_gate(self, index: int) -> None:
         """
         Add projection gate to |1> subspace
         """
-    def add_RX_gate(self, index: int, angle: float) -> None: 
+    def add_RX_gate(self, index: int, angle: float) -> None:
         """
         Add Pauli-X rotation gate
         """
-    def add_RY_gate(self, index: int, angle: float) -> None: 
+    def add_RY_gate(self, index: int, angle: float) -> None:
         """
         Add Pauli-Y rotation gate
         """
-    def add_RZ_gate(self, index: int, angle: float) -> None: 
+    def add_RZ_gate(self, index: int, angle: float) -> None:
         """
         Add Pauli-Z rotation gate
         """
-    def add_RotInvX_gate(self, index: int, angle: float) -> None: 
+    def add_RotInvX_gate(self, index: int, angle: float) -> None:
         """
         Add Pauli-X rotation gate
         """
-    def add_RotInvY_gate(self, index: int, angle: float) -> None: 
+    def add_RotInvY_gate(self, index: int, angle: float) -> None:
         """
         Add Pauli-Y rotation gate
         """
-    def add_RotInvZ_gate(self, index: int, angle: float) -> None: 
+    def add_RotInvZ_gate(self, index: int, angle: float) -> None:
         """
         Add Pauli-Z rotation gate
         """
-    def add_RotX_gate(self, index: int, angle: float) -> None: 
+    def add_RotX_gate(self, index: int, angle: float) -> None:
         """
         Add Pauli-X rotation gate
         """
-    def add_RotY_gate(self, index: int, angle: float) -> None: 
+    def add_RotY_gate(self, index: int, angle: float) -> None:
         """
         Add Pauli-Y rotation gate
         """
-    def add_RotZ_gate(self, index: int, angle: float) -> None: 
+    def add_RotZ_gate(self, index: int, angle: float) -> None:
         """
         Add Pauli-Z rotation gate
         """
-    def add_SWAP_gate(self, target1: int, target2: int) -> None: 
+    def add_SWAP_gate(self, target1: int, target2: int) -> None:
         """
         Add SWAP gate
         """
-    def add_S_gate(self, index: int) -> None: 
+    def add_S_gate(self, index: int) -> None:
         """
         Add pi/4 phase gate
         """
-    def add_Sdag_gate(self, index: int) -> None: 
+    def add_Sdag_gate(self, index: int) -> None:
         """
         Add adjoint of pi/4 phsae gate
         """
-    def add_T_gate(self, index: int) -> None: 
+    def add_T_gate(self, index: int) -> None:
         """
         Add pi/8 phase gate
         """
-    def add_Tdag_gate(self, index: int) -> None: 
+    def add_Tdag_gate(self, index: int) -> None:
         """
         Add adjoint of pi/8 phase gate
         """
-    def add_U1_gate(self, index: int, lambda_: float) -> None: 
+    def add_U1_gate(self, index: int, lambda_: float) -> None:
         """
         Add QASM U1 gate
         """
-    def add_U2_gate(self, index: int, phi: float, lambda_: float) -> None: 
+    def add_U2_gate(self, index: int, phi: float, lambda_: float) -> None:
         """
         Add QASM U2 gate
         """
-    def add_U3_gate(self, index: int, theta: float, phi: float, lambda_: float) -> None: 
+    def add_U3_gate(self, index: int, theta: float, phi: float, lambda_: float) -> None:
         """
         Add QASM U3 gate
         """
-    def add_X_gate(self, index: int) -> None: 
+    def add_X_gate(self, index: int) -> None:
         """
         Add Pauli-X gate
         """
-    def add_Y_gate(self, index: int) -> None: 
+    def add_Y_gate(self, index: int) -> None:
         """
         Add Pauli-Y gate
         """
-    def add_Z_gate(self, index: int) -> None: 
+    def add_Z_gate(self, index: int) -> None:
         """
         Add Pauli-Z gate
         """
     @typing.overload
-    def add_dense_matrix_gate(self, index: int, matrix: numpy.ndarray[numpy.complex128, _Shape[m, n]]) -> None: 
+    def add_dense_matrix_gate(self, index: int, matrix: numpy.ndarray) -> None:
         """
         Add dense matrix gate
         """
     @typing.overload
-    def add_dense_matrix_gate(self, index_list: typing.List[int], matrix: numpy.ndarray[numpy.complex128, _Shape[m, n]]) -> None: ...
-    def add_diagonal_observable_rotation_gate(self, observable: Observable, angle: float) -> None: 
+    def add_dense_matrix_gate(
+        self, index_list: typing.List[int], matrix: numpy.ndarray
+    ) -> None: ...
+    def add_diagonal_observable_rotation_gate(
+        self, observable: Observable, angle: float
+    ) -> None:
         """
         Add diagonal observable rotation gate
         """
     @typing.overload
-    def add_gate(self, gate: QuantumGateBase) -> None: 
+    def add_gate(self, gate: QuantumGateBase) -> None:
         """
         Add gate with copy
         """
     @typing.overload
     def add_gate(self, gate: QuantumGateBase, position: int) -> None: ...
     @typing.overload
-    def add_multi_Pauli_gate(self, index_list: typing.List[int], pauli_ids: typing.List[int]) -> None: 
+    def add_multi_Pauli_gate(
+        self, index_list: typing.List[int], pauli_ids: typing.List[int]
+    ) -> None:
         """
         Add multi-qubit Pauli gate
         """
     @typing.overload
     def add_multi_Pauli_gate(self, pauli: PauliOperator) -> None: ...
     @typing.overload
-    def add_multi_Pauli_rotation_gate(self, index_list: typing.List[int], pauli_ids: typing.List[int], angle: float) -> None: 
+    def add_multi_Pauli_rotation_gate(
+        self, index_list: typing.List[int], pauli_ids: typing.List[int], angle: float
+    ) -> None:
         """
         Add multi-qubit Pauli rotation gate
         """
     @typing.overload
     def add_multi_Pauli_rotation_gate(self, pauli: PauliOperator) -> None: ...
-    def add_noise_gate(self, gate: QuantumGateBase, NoiseType: str, NoiseProbability: float) -> None: 
+    def add_noise_gate(
+        self, gate: QuantumGateBase, NoiseType: str, NoiseProbability: float
+    ) -> None:
         """
         Add noise gate with copy
         """
-    def add_observable_rotation_gate(self, observable: Observable, angle: float, repeat: int) -> None: 
+    def add_observable_rotation_gate(
+        self, observable: Observable, angle: float, repeat: int
+    ) -> None:
         """
         Add observable rotation gate
         """
     @typing.overload
-    def add_random_unitary_gate(self, index_list: typing.List[int]) -> None: 
+    def add_random_unitary_gate(self, index_list: typing.List[int]) -> None:
         """
         Add random unitary gate
         """
     @typing.overload
-    def add_random_unitary_gate(self, index_list: typing.List[int], seed: int) -> None: ...
-    def add_sqrtX_gate(self, index: int) -> None: 
+    def add_random_unitary_gate(
+        self, index_list: typing.List[int], seed: int
+    ) -> None: ...
+    def add_sqrtX_gate(self, index: int) -> None:
         """
         Add pi/4 Pauli-X rotation gate
         """
-    def add_sqrtXdag_gate(self, index: int) -> None: 
+    def add_sqrtXdag_gate(self, index: int) -> None:
         """
         Add adjoint of pi/4 Pauli-X rotation gate
         """
-    def add_sqrtY_gate(self, index: int) -> None: 
+    def add_sqrtY_gate(self, index: int) -> None:
         """
         Add pi/4 Pauli-Y rotation gate
         """
-    def add_sqrtYdag_gate(self, index: int) -> None: 
+    def add_sqrtYdag_gate(self, index: int) -> None:
         """
         Add adjoint of pi/4 Pauli-Y rotation gate
         """
-    def calculate_depth(self) -> int: 
+    def calculate_depth(self) -> int:
         """
         Calculate depth of circuit
         """
-    def copy(self) -> QuantumCircuit: 
+    def copy(self) -> QuantumCircuit:
         """
         Create copied instance
         """
-    def get_gate(self, position: int) -> QuantumGateBase: 
+    def get_gate(self, position: int) -> QuantumGateBase:
         """
         Get gate instance
         """
-    def get_gate_count(self) -> int: 
+    def get_gate_count(self) -> int:
         """
         Get gate count
         """
-    def get_inverse(self) -> QuantumCircuit: 
+    def get_inverse(self) -> QuantumCircuit:
         """
         get inverse circuit
         """
-    def get_qubit_count(self) -> int: 
+    def get_qubit_count(self) -> int:
         """
         Get qubit count
         """
     def merge_circuit(self, circuit: QuantumCircuit) -> None: ...
-    def remove_gate(self, position: int) -> None: 
+    def remove_gate(self, position: int) -> None:
         """
         Remove gate
         """
     def to_json(self) -> str: ...
-    def to_string(self) -> str: 
+    def to_string(self) -> str:
         """
         Get string representation
         """
     @typing.overload
-    def update_quantum_state(self, state: QuantumStateBase) -> None: 
+    def update_quantum_state(self, state: QuantumStateBase) -> None:
         """
         Update quantum state
         """
     @typing.overload
-    def update_quantum_state(self, state: QuantumStateBase, start: int, end: int) -> None: ...
+    def update_quantum_state(
+        self, state: QuantumStateBase, start: int, end: int
+    ) -> None: ...
     pass
-class PauliOperator():
+
+class PauliOperator:
     def __IMUL__(self, arg0: complex) -> PauliOperator: ...
     def __imul__(self, arg0: PauliOperator) -> PauliOperator: ...
     @typing.overload
-    def __init__(self, coef: complex) -> None: 
+    def __init__(self, coef: complex) -> None:
         """
         Constructor
         """
     @typing.overload
     def __init__(self, pauli_string: str, coef: complex) -> None: ...
     @typing.overload
     def __mul__(self, arg0: PauliOperator) -> PauliOperator: ...
     @typing.overload
     def __mul__(self, arg0: complex) -> PauliOperator: ...
-    def add_single_Pauli(self, index: int, pauli_type: int) -> None: 
+    def add_single_Pauli(self, index: int, pauli_type: int) -> None:
         """
         Add Pauli operator to this term
         """
-    def change_coef(self, new_coef: complex) -> None: 
+    def change_coef(self, new_coef: complex) -> None:
         """
         Change coefficient
         """
-    def copy(self) -> PauliOperator: 
+    def copy(self) -> PauliOperator:
         """
         Create copied instance of Pauli operator class
         """
-    def get_coef(self) -> complex: 
+    def get_coef(self) -> complex:
         """
         Get coefficient of Pauli term
         """
-    def get_expectation_value(self, state: QuantumStateBase) -> complex: 
+    def get_expectation_value(self, state: QuantumStateBase) -> complex:
         """
         Get expectation value
         """
-    def get_expectation_value_single_thread(self, state: QuantumStateBase) -> complex: 
+    def get_expectation_value_single_thread(self, state: QuantumStateBase) -> complex:
         """
         Get expectation value
         """
-    def get_index_list(self) -> typing.List[int]: 
+    def get_index_list(self) -> typing.List[int]:
         """
         Get list of target qubit indices
         """
-    def get_pauli_id_list(self) -> typing.List[int]: 
+    def get_pauli_id_list(self) -> typing.List[int]:
         """
         Get list of Pauli IDs (I,X,Y,Z) = (0,1,2,3)
         """
-    def get_pauli_string(self) -> str: 
+    def get_pauli_string(self) -> str:
         """
         Get pauli string
         """
-    def get_transition_amplitude(self, state_bra: QuantumStateBase, state_ket: QuantumStateBase) -> complex: 
+    def get_transition_amplitude(
+        self, state_bra: QuantumStateBase, state_ket: QuantumStateBase
+    ) -> complex:
         """
         Get transition amplitude
         """
     pass
+
 class ParametricQuantumCircuit(QuantumCircuit):
     def __getstate__(self) -> str: ...
-    def __init__(self, qubit_count: int) -> None: 
+    def __init__(self, qubit_count: int) -> None:
         """
         Constructor
         """
     def __setstate__(self, arg0: str) -> None: ...
-    def __str__(self) -> str: 
+    def __str__(self) -> str:
         """
         to string
         """
     @typing.overload
-    def add_gate(self, gate: QuantumGateBase) -> None: 
+    def add_gate(self, gate: QuantumGateBase) -> None:
         """
         Add gate
         """
     @typing.overload
     def add_gate(self, gate: QuantumGateBase, position: int) -> None: ...
-    def add_parametric_RX_gate(self, index: int, angle: float) -> None: 
+    def add_parametric_RX_gate(self, index: int, angle: float) -> None:
         """
         Add parametric Pauli-X rotation gate
         """
-    def add_parametric_RY_gate(self, index: int, angle: float) -> None: 
+    def add_parametric_RY_gate(self, index: int, angle: float) -> None:
         """
         Add parametric Pauli-Y rotation gate
         """
-    def add_parametric_RZ_gate(self, index: int, angle: float) -> None: 
+    def add_parametric_RZ_gate(self, index: int, angle: float) -> None:
         """
         Add parametric Pauli-Z rotation gate
         """
     @typing.overload
-    def add_parametric_gate(self, gate: QuantumGate_SingleParameter) -> None: 
+    def add_parametric_gate(self, gate: QuantumGate_SingleParameter) -> None:
         """
         Add parametric gate
         """
     @typing.overload
-    def add_parametric_gate(self, gate: QuantumGate_SingleParameter, position: int) -> None: ...
-    def add_parametric_multi_Pauli_rotation_gate(self, index_list: typing.List[int], pauli_ids: typing.List[int], angle: float) -> None: 
+    def add_parametric_gate(
+        self, gate: QuantumGate_SingleParameter, position: int
+    ) -> None: ...
+    def add_parametric_multi_Pauli_rotation_gate(
+        self, index_list: typing.List[int], pauli_ids: typing.List[int], angle: float
+    ) -> None:
         """
         Add parametric multi-qubit Pauli rotation gate
         """
-    def backprop(self, obs: GeneralQuantumOperator) -> typing.List[float]: 
+    def backprop(self, obs: GeneralQuantumOperator) -> typing.List[float]:
         """
         Do backprop
         """
-    def backprop_inner_product(self, state: QuantumState) -> typing.List[float]: 
+    def backprop_inner_product(self, state: QuantumState) -> typing.List[float]:
         """
         Do backprop with innder product
         """
-    def copy(self) -> ParametricQuantumCircuit: 
+    def copy(self) -> ParametricQuantumCircuit:
         """
         Create copied instance
         """
-    def get_parameter(self, index: int) -> float: 
+    def get_parameter(self, index: int) -> float:
         """
         Get parameter
         """
-    def get_parameter_count(self) -> int: 
+    def get_parameter_count(self) -> int:
         """
         Get parameter count
         """
-    def get_parametric_gate_position(self, index: int) -> int: 
+    def get_parametric_gate_position(self, index: int) -> int:
         """
         Get parametric gate position
         """
-    def merge_circuit(self, circuit: ParametricQuantumCircuit) -> None: 
+    def merge_circuit(self, circuit: ParametricQuantumCircuit) -> None:
         """
         Merge another ParametricQuantumCircuit
         """
-    def remove_gate(self, position: int) -> None: 
+    def remove_gate(self, position: int) -> None:
         """
         Remove gate
         """
-    def set_parameter(self, index: int, parameter: float) -> None: 
+    def set_parameter(self, index: int, parameter: float) -> None:
         """
         Set parameter
         """
     pass
-class QuantumCircuitSimulator():
-    def __init__(self, circuit: QuantumCircuit, state: QuantumStateBase) -> None: 
+
+class QuantumCircuitSimulator:
+    def __init__(self, circuit: QuantumCircuit, state: QuantumStateBase) -> None:
         """
         Constructor
         """
-    def copy_state_from_buffer(self) -> None: 
+    def copy_state_from_buffer(self) -> None:
         """
         Copy buffer to state
         """
-    def copy_state_to_buffer(self) -> None: 
+    def copy_state_to_buffer(self) -> None:
         """
         Copy state to buffer
         """
-    def get_expectation_value(self, observable: Observable) -> complex: 
+    def get_expectation_value(self, observable: Observable) -> complex:
         """
         Get expectation value
         """
-    def get_gate_count(self) -> int: 
+    def get_gate_count(self) -> int:
         """
         Get gate count
         """
     @typing.overload
-    def initialize_random_state(self) -> None: 
+    def initialize_random_state(self) -> None:
         """
         Initialize state with random pure state
         """
     @typing.overload
     def initialize_random_state(self, seed: int) -> None: ...
-    def initialize_state(self, arg0: int) -> None: 
+    def initialize_state(self, arg0: int) -> None:
         """
         Initialize state
         """
-    def simulate(self) -> None: 
+    def simulate(self) -> None:
         """
         Simulate circuit
         """
-    def simulate_range(self, start: int, end: int) -> None: 
+    def simulate_range(self, start: int, end: int) -> None:
         """
         Simulate circuit
         """
-    def swap_state_and_buffer(self) -> None: 
+    def swap_state_and_buffer(self) -> None:
         """
         Swap state and buffer
         """
     pass
+
 class ClsNoisyEvolution(QuantumGateBase):
     pass
+
 class QuantumGateDiagonalMatrix(QuantumGateBase):
     pass
+
 class QuantumGateMatrix(QuantumGateBase):
-    def add_control_qubit(self, index: int, control_value: int) -> None: 
+    def add_control_qubit(self, index: int, control_value: int) -> None:
         """
         Add control qubit
         """
-    def multiply_scalar(self, value: complex) -> None: 
+    def multiply_scalar(self, value: complex) -> None:
         """
         Multiply scalar value to gate matrix
         """
     pass
+
 class QuantumGateSparseMatrix(QuantumGateBase):
     pass
+
 class QuantumGate_Adaptive(QuantumGateBase):
     pass
+
 class QuantumGate_CP(QuantumGateBase):
-    def get_gate_list(self) -> typing.List[QuantumGateBase]: 
+    def get_gate_list(self) -> typing.List[QuantumGateBase]:
         """
         get_gate_list
         """
     pass
+
 class QuantumGate_CPTP(QuantumGateBase):
     """
     QuantumGate_Instrument
     """
-    def get_gate_list(self) -> typing.List[QuantumGateBase]: 
+
+    def get_gate_list(self) -> typing.List[QuantumGateBase]:
         """
         get_gate_list
         """
     pass
+
 class QuantumGate_Probabilistic(QuantumGateBase):
     """
     QuantumGate_ProbabilisticInstrument
     """
-    def get_cumulative_distribution(self) -> typing.List[float]: 
+
+    def get_cumulative_distribution(self) -> typing.List[float]:
         """
         get_cumulative_distribution
         """
-    def get_distribution(self) -> typing.List[float]: 
+    def get_distribution(self) -> typing.List[float]:
         """
         get_distribution
         """
-    def get_gate_list(self) -> typing.List[QuantumGateBase]: 
+    def get_gate_list(self) -> typing.List[QuantumGateBase]:
         """
         get_gate_list
         """
-    def optimize_ProbablisticGate(self) -> None: 
+    def optimize_ProbablisticGate(self) -> None:
         """
         optimize_ProbablisticGate
         """
     pass
+
 class QuantumGate_SingleParameter(QuantumGateBase):
-    def copy(self) -> QuantumGate_SingleParameter: 
+    def copy(self) -> QuantumGate_SingleParameter:
         """
         Create copied instance
         """
-    def get_parameter_value(self) -> float: 
+    def get_parameter_value(self) -> float:
         """
         Get parameter value
         """
-    def set_parameter_value(self, value: float) -> None: 
+    def set_parameter_value(self, value: float) -> None:
         """
         Set parameter value
         """
     pass
+
 class QuantumState(QuantumStateBase):
     def __getstate__(self) -> str: ...
     @typing.overload
-    def __init__(self, qubit_count: int) -> None: 
+    def __init__(self, qubit_count: int) -> None:
         """
         Constructor
         """
     @typing.overload
     def __init__(self, qubit_count: int, use_multi_cpu: bool) -> None: ...
     def __setstate__(self, arg0: str) -> None: ...
-    def __str__(self) -> str: 
+    def __str__(self) -> str:
         """
         to string
         """
-    def add_state(self, state: QuantumStateBase) -> None: 
+    def add_state(self, state: QuantumStateBase) -> None:
         """
         Add state vector to this state
         """
-    def allocate_buffer(self) -> QuantumState: 
+    def allocate_buffer(self) -> QuantumState:
         """
         Allocate buffer with the same size
         """
-    def copy(self) -> QuantumState: 
+    def copy(self) -> QuantumState:
         """
         Create copied instance
         """
-    def get_amplitude(self, comp_basis: int) -> complex: 
+    def get_amplitude(self, comp_basis: int) -> complex:
         """
         Get Amplitude of a specified computational basis
         """
-    def get_classical_value(self, index: int) -> int: 
+    def get_classical_value(self, index: int) -> int:
         """
         Get classical value
         """
-    def get_device_name(self) -> str: 
+    def get_device_name(self) -> str:
         """
         Get allocated device name
         """
-    def get_entropy(self) -> float: 
+    def get_entropy(self) -> float:
         """
         Get entropy
         """
-    def get_marginal_probability(self, measured_values: typing.List[int]) -> float: 
+    def get_marginal_probability(self, measured_values: typing.List[int]) -> float:
         """
         Get merginal probability for measured values
         """
-    def get_qubit_count(self) -> int: 
+    def get_qubit_count(self) -> int:
         """
         Get qubit count
         """
-    def get_squared_norm(self) -> float: 
+    def get_squared_norm(self) -> float:
         """
         Get squared norm
         """
-    def get_vector(self) -> numpy.ndarray[numpy.complex128, _Shape[m, 1]]: 
+    def get_vector(self) -> numpy.ndarray:
         """
         Get state vector
         """
-    def get_zero_probability(self, index: int) -> float: 
+    def get_zero_probability(self, index: int) -> float:
         """
         Get probability with which we obtain 0 when we measure a qubit
         """
     @typing.overload
-    def load(self, state: QuantumStateBase) -> None: 
+    def load(self, state: QuantumStateBase) -> None:
         """
         Load quantum state vector
         """
     @typing.overload
     def load(self, state: typing.List[complex]) -> None: ...
-    def multiply_coef(self, coef: complex) -> None: 
+    def multiply_coef(self, coef: complex) -> None:
         """
         Multiply coefficient to this state
         """
-    def multiply_elementwise_function(self, func: typing.Callable[[int], complex]) -> None: 
+    def multiply_elementwise_function(
+        self, func: typing.Callable[[int], complex]
+    ) -> None:
         """
         Multiply elementwise function
         """
-    def normalize(self, squared_norm: float) -> None: 
+    def normalize(self, squared_norm: float) -> None:
         """
         Normalize quantum state
         """
     @typing.overload
-    def sampling(self, sampling_count: int) -> typing.List[int]: 
+    def sampling(self, sampling_count: int) -> typing.List[int]:
         """
         Sampling measurement results
         """
     @typing.overload
     def sampling(self, sampling_count: int, random_seed: int) -> typing.List[int]: ...
     @typing.overload
-    def set_Haar_random_state(self) -> None: 
+    def set_Haar_random_state(self) -> None:
         """
         Set Haar random state
         """
     @typing.overload
     def set_Haar_random_state(self, seed: int) -> None: ...
-    def set_classical_value(self, index: int, value: int) -> None: 
+    def set_classical_value(self, index: int, value: int) -> None:
         """
         Set classical value
         """
-    def set_computational_basis(self, comp_basis: int) -> None: 
+    def set_computational_basis(self, comp_basis: int) -> None:
         """
         Set state to computational basis
         """
-    def set_zero_state(self) -> None: 
+    def set_zero_state(self) -> None:
         """
         Set state to |0>
         """
-    def to_json(self) -> str: 
+    def to_json(self) -> str:
         """
         to json string
         """
-    def to_string(self) -> str: 
+    def to_string(self) -> str:
         """
         to string
         """
     pass
+
 class DensityMatrix(QuantumStateBase):
     def __getstate__(self) -> str: ...
-    def __init__(self, qubit_count: int) -> None: 
+    def __init__(self, qubit_count: int) -> None:
         """
         Constructor
         """
     def __setstate__(self, arg0: str) -> None: ...
-    def __str__(self) -> str: 
+    def __str__(self) -> str:
         """
         to string
         """
-    def add_state(self, state: QuantumStateBase) -> None: 
+    def add_state(self, state: QuantumStateBase) -> None:
         """
         Add state vector to this state
         """
-    def allocate_buffer(self) -> DensityMatrix: 
+    def allocate_buffer(self) -> DensityMatrix:
         """
         Allocate buffer with the same size
         """
-    def copy(self) -> DensityMatrix: 
+    def copy(self) -> DensityMatrix:
         """
         Create copied insntace
         """
-    def get_classical_value(self, index: int) -> int: 
+    def get_classical_value(self, index: int) -> int:
         """
         Get classical value
         """
-    def get_device_name(self) -> str: 
+    def get_device_name(self) -> str:
         """
         Get allocated device name
         """
-    def get_entropy(self) -> float: 
+    def get_entropy(self) -> float:
         """
         Get entropy
         """
-    def get_marginal_probability(self, measured_values: typing.List[int]) -> float: 
+    def get_marginal_probability(self, measured_values: typing.List[int]) -> float:
         """
         Get merginal probability for measured values
         """
-    def get_matrix(self) -> numpy.ndarray[numpy.complex128, _Shape[m, n]]: 
+    def get_matrix(self) -> numpy.ndarray:
         """
         Get density matrix
         """
-    def get_qubit_count(self) -> int: 
+    def get_qubit_count(self) -> int:
         """
         Get qubit count
         """
-    def get_squared_norm(self) -> float: 
+    def get_squared_norm(self) -> float:
         """
         Get squared norm
         """
-    def get_zero_probability(self, index: int) -> float: 
+    def get_zero_probability(self, index: int) -> float:
         """
         Get probability with which we obtain 0 when we measure a qubit
         """
     @typing.overload
-    def load(self, state: QuantumStateBase) -> None: 
+    def load(self, state: QuantumStateBase) -> None:
         """
         Load quantum state vector or density matrix
         """
     @typing.overload
-    def load(self, state: numpy.ndarray[numpy.complex128, _Shape[m, n]]) -> None: ...
-    @typing.overload
     def load(self, state: typing.List[complex]) -> None: ...
-    def multiply_coef(self, coef: complex) -> None: 
+    @typing.overload
+    def load(self, state: numpy.ndarray) -> None: ...
+    def multiply_coef(self, coef: complex) -> None:
         """
         Multiply coefficient to this state
         """
-    def normalize(self, squared_norm: float) -> None: 
+    def normalize(self, squared_norm: float) -> None:
         """
         Normalize quantum state
         """
     @typing.overload
-    def sampling(self, sampling_count: int) -> typing.List[int]: 
+    def sampling(self, sampling_count: int) -> typing.List[int]:
         """
         Sampling measurement results
         """
     @typing.overload
     def sampling(self, sampling_count: int, random_seed: int) -> typing.List[int]: ...
     @typing.overload
-    def set_Haar_random_state(self) -> None: 
+    def set_Haar_random_state(self) -> None:
         """
         Set Haar random state
         """
     @typing.overload
     def set_Haar_random_state(self, seed: int) -> None: ...
-    def set_classical_value(self, index: int, value: int) -> None: 
+    def set_classical_value(self, index: int, value: int) -> None:
         """
         Set classical value
         """
-    def set_computational_basis(self, comp_basis: int) -> None: 
+    def set_computational_basis(self, comp_basis: int) -> None:
         """
         Set state to computational basis
         """
-    def set_zero_state(self) -> None: 
+    def set_zero_state(self) -> None:
         """
         Set state to |0>
         """
-    def to_json(self) -> str: 
+    def to_json(self) -> str:
         """
         to json string
         """
-    def to_string(self) -> str: 
+    def to_string(self) -> str:
         """
         to string
         """
     pass
-class SimulationResult():
-    def get_count(self) -> int: 
+
+class SimulationResult:
+    def get_count(self) -> int:
         """
         get state count
         """
-    def get_frequency(self, arg0: int) -> int: 
+    def get_frequency(self, arg0: int) -> int:
         """
         get state frequency
         """
-    def get_state(self, arg0: int) -> QuantumState: 
+    def get_state(self, arg0: int) -> QuantumState:
         """
         get state
         """
     pass
+
 def StateVector(arg0: int) -> QuantumState:
     """
     StateVector
     """
+
 def check_build_for_mpi() -> bool:
     pass
-def to_general_quantum_operator(gate: QuantumGateBase, qubits: int, tol: float) -> GeneralQuantumOperator:
+
+def to_general_quantum_operator(
+    gate: QuantumGateBase, qubits: int, tol: float
+) -> GeneralQuantumOperator:
     pass
```

### Comparing `qulacs-0.6.0/pysrc/qulacs/circuit/__init__.pyi` & `qulacs-0.6.1/pysrc/qulacs/circuit/__init__.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from __future__ import annotations
-import qulacs_core.circuit
+
 import typing
-import qulacs_core
 
-__all__ = [
-    "QuantumCircuitOptimizer",
-    "from_json"
-]
+import qulacs_core
+import qulacs_core.circuit
 
+__all__ = ["QuantumCircuitOptimizer", "from_json"]
 
-class QuantumCircuitOptimizer():
-    def __init__(self) -> None: 
+class QuantumCircuitOptimizer:
+    def __init__(self) -> None:
         """
         Constructor
         """
-    def merge_all(self, circuit: qulacs_core.QuantumCircuit) -> qulacs_core.QuantumGateMatrix: ...
-    def optimize(self, circuit: qulacs_core.QuantumCircuit, block_size: int) -> None: 
+    def merge_all(
+        self, circuit: qulacs_core.QuantumCircuit
+    ) -> qulacs_core.QuantumGateMatrix: ...
+    def optimize(self, circuit: qulacs_core.QuantumCircuit, block_size: int) -> None:
         """
         Optimize quantum circuit
         """
-    def optimize_light(self, circuit: qulacs_core.QuantumCircuit) -> None: 
+    def optimize_light(self, circuit: qulacs_core.QuantumCircuit) -> None:
         """
         Optimize quantum circuit with light method
         """
     pass
+
 def from_json(arg0: str) -> qulacs_core.QuantumCircuit:
     """
     from json string
     """
```

### Comparing `qulacs-0.6.0/pysrc/qulacs/converter/qasm_converter.py` & `qulacs-0.6.1/pysrc/qulacs/converter/qasm_converter.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,20 +2,27 @@
 import typing
 from cmath import phase
 from logging import NullHandler, getLogger
 from typing import List
 
 import numpy as np
 import qulacs_core
+
 from qulacs import QuantumCircuit
 from qulacs.gate import DenseMatrix, Identity
 
 logger = getLogger(__name__)
 logger.addHandler(NullHandler())
 
+FIXED_POINT_PATTERN = r"[+-]?\d+(?:\.\d*)?|\.\d+"
+FLOATING_POINT_PATTERN = r"[eE][-+]?\d+"
+GENERAL_NUMBER_PATTERN = (
+    rf"(?:{FIXED_POINT_PATTERN})(?:{FLOATING_POINT_PATTERN})?"  # noqa
+)
+
 
 def convert_qulacs_circuit_to_QASM(cir: QuantumCircuit) -> typing.List[str]:
     # convert qulacs Quantum Circuit to QASM List[str].
     # This method uses extended QASM for serializing Density Matrix.
     # This serializes almost all gate type defined in qelib1.inc,
     # except for sqrtY gate.
     # CAVEAT: this function currently does not accept leading zero notation like
@@ -187,74 +194,64 @@
             cir.add_T_gate(mapping[int(ary[0])])
         elif instr[0:4] == "tdgq":
             matchobj = re.match(r"tdgq\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_Tdag_gate(mapping[int(ary[0])])
         elif instr[0:2] == "rx":
-            matchobj = re.match(
-                r"rx\((\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?\)q\[(\d+)\];", instr
-            )
+            matchobj = re.match(rf"rx\(({GENERAL_NUMBER_PATTERN})\)q\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_RX_gate(mapping[int(ary[1])], -float(ary[0]))
         elif instr[0:2] == "ry":
-            matchobj = re.match(
-                r"ry\((\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?\)q\[(\d+)\];", instr
-            )
+            matchobj = re.match(rf"ry\(({GENERAL_NUMBER_PATTERN})\)q\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_RY_gate(mapping[int(ary[1])], -float(ary[0]))
         elif instr[0:2] == "rz":
-            matchobj = re.match(
-                r"rz\((\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?\)q\[(\d+)\];", instr
-            )
+            matchobj = re.match(rf"rz\(({GENERAL_NUMBER_PATTERN})\)q\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_RZ_gate(mapping[int(ary[1])], -float(ary[0]))
         elif instr[0:1] == "p":
-            matchobj = re.match(
-                r"p\((\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?\)q\[(\d+)\];", instr
-            )
+            matchobj = re.match(rf"p\({GENERAL_NUMBER_PATTERN}\)q\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_U1_gate(mapping[int(ary[1])], float(ary[0]))
         elif instr[0:2] == "u1":
-            matchobj = re.match(
-                r"u1\((\d+(\.\d*)?|\.\d+)([eE][-+]?\d+\)?)q[(\d+)];", instr
-            )
+            matchobj = re.match(rf"u1\(({GENERAL_NUMBER_PATTERN})\)q[(\d+)];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_U1_gate(mapping[int(ary[1])], float(ary[0]))
         elif instr[0:2] == "u2":
             matchobj = re.match(
-                r"u2\((\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?,"
-                + r"(\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?\)q\[(\d+)\];",
+                rf"u2\({GENERAL_NUMBER_PATTERN}),"
+                + rf"({GENERAL_NUMBER_PATTERN}\)q\[(\d+)\];",
                 instr,
             )
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_U2_gate(mapping[int(ary[2])], float(ary[0]), float(ary[1]))
         elif instr[0:2] == "u3":
             matchobj = re.match(
-                r"u3\((\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?,"
-                + r"(\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?,"
-                + r"(\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?\)q\[(\d+)\];",
+                rf"u3\(({GENERAL_NUMBER_PATTERN}),"
+                + rf"({GENERAL_NUMBER_PATTERN}),"
+                + rf"({GENERAL_NUMBER_PATTERN})\)q\[(\d+)\];",
                 instr,
             )
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_U3_gate(
                 mapping[int(ary[3])], float(ary[0]), float(ary[1]), float(ary[2])
             )
         elif instr[0:1] == "u":
             matchobj = re.match(
-                r"u\((\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?,"
-                + r"(\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?,"
-                + r"(\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?\)q\[(\d+)\];",
+                rf"u\(({GENERAL_NUMBER_PATTERN}),"
+                + rf"({GENERAL_NUMBER_PATTERN}),"
+                + rf"({GENERAL_NUMBER_PATTERN})\)q\[(\d+)\];",
                 instr,
             )
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_U3_gate(
                 mapping[int(ary[3])], float(ary[0]), float(ary[1]), float(ary[2])
             )
@@ -265,14 +262,15 @@
             cir.add_sqrtX_gate(mapping[int(ary[0])])
         elif instr[0:5] == "sxdgq":
             matchobj = re.match(r"sxdgq\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_sqrtXdag_gate(mapping[int(ary[0])])
         elif instr[0:11] == "densematrix":
+            # Matches all matrix elements and qubit indexes
             deary = re.findall(r"[+-]?\d+(?:\.\d+)?(?:[eE][+-]?\d+)?", instr)
             target_qubit_count = int(deary[0])
             control_qubit_count = int(deary[1])
 
             gate_mat = np.zeros(
                 (2**target_qubit_count, 2**target_qubit_count), dtype="complex"
             )
```

### Comparing `qulacs-0.6.0/pysrc/qulacs/gate/__init__.pyi` & `qulacs-0.6.1/pysrc/qulacs/gate/__init__.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
-import qulacs_core.gate
+
 import typing
+
 import numpy
 import qulacs_core
+import qulacs_core.gate
 import scipy.sparse
-_Shape = typing.Tuple[int, ...]
 
 __all__ = [
     "Adaptive",
     "AmplitudeDampingNoise",
     "BitFlipNoise",
     "CNOT",
     "CP",
@@ -66,289 +67,419 @@
     "add",
     "from_json",
     "merge",
     "sqrtX",
     "sqrtXdag",
     "sqrtY",
     "sqrtYdag",
-    "to_matrix_gate"
+    "to_matrix_gate",
 ]
 
-
 @typing.overload
-def Adaptive(gate: qulacs_core.QuantumGateBase, condition: typing.Callable[[typing.List[int], int], bool], id: int) -> qulacs_core.QuantumGateBase:
+def Adaptive(
+    gate: qulacs_core.QuantumGateBase,
+    condition: typing.Callable[[typing.List[int]], bool],
+) -> qulacs_core.QuantumGateBase:
     """
     Create adaptive gate
     """
+
 @typing.overload
-def Adaptive(gate: qulacs_core.QuantumGateBase, condition: typing.Callable[[typing.List[int]], bool]) -> qulacs_core.QuantumGateBase:
+def Adaptive(
+    gate: qulacs_core.QuantumGateBase,
+    condition: typing.Callable[[typing.List[int], int], bool],
+    id: int,
+) -> qulacs_core.QuantumGateBase:
     pass
+
 def AmplitudeDampingNoise(index: int, prob: float) -> qulacs_core.QuantumGate_CPTP:
     """
     Create amplitude damping noise
     """
+
 def BitFlipNoise(index: int, prob: float) -> qulacs_core.QuantumGate_Probabilistic:
     """
     Create bit-flip noise
     """
+
 def CNOT(control: int, target: int) -> qulacs_core.ClsOneControlOneTargetGate:
     """
     Create CNOT gate
     """
-def CP(kraus_list: typing.List[qulacs_core.QuantumGateBase], state_normalize: bool, probability_normalize: bool, assign_zero_if_not_matched: bool) -> qulacs_core.QuantumGateBase:
+
+def CP(
+    kraus_list: typing.List[qulacs_core.QuantumGateBase],
+    state_normalize: bool,
+    probability_normalize: bool,
+    assign_zero_if_not_matched: bool,
+) -> qulacs_core.QuantumGateBase:
     """
     Create completely-positive map
     """
-def CPTP(kraus_list: typing.List[qulacs_core.QuantumGateBase]) -> qulacs_core.QuantumGateBase:
+
+def CPTP(
+    kraus_list: typing.List[qulacs_core.QuantumGateBase],
+) -> qulacs_core.QuantumGateBase:
     """
     Create completely-positive trace preserving map
     """
+
 def CZ(control: int, target: int) -> qulacs_core.ClsOneControlOneTargetGate:
     """
     Create CZ gate
     """
+
 @typing.overload
-def DenseMatrix(index: int, matrix: numpy.ndarray[numpy.complex128, _Shape[m, n]]) -> qulacs_core.QuantumGateMatrix:
+def DenseMatrix(index: int, matrix: numpy.ndarray) -> qulacs_core.QuantumGateMatrix:
     """
     Create dense matrix gate
     """
+
 @typing.overload
-def DenseMatrix(index_list: typing.List[int], matrix: numpy.ndarray[numpy.complex128, _Shape[m, n]]) -> qulacs_core.QuantumGateMatrix:
+def DenseMatrix(
+    index_list: typing.List[int], matrix: numpy.ndarray
+) -> qulacs_core.QuantumGateMatrix:
     pass
+
 def DephasingNoise(index: int, prob: float) -> qulacs_core.QuantumGate_Probabilistic:
     """
     Create dephasing noise
     """
+
 def DepolarizingNoise(index: int, prob: float) -> qulacs_core.QuantumGate_Probabilistic:
     """
     Create depolarizing noise
     """
-def DiagonalMatrix(index_list: typing.List[int], diagonal_element: numpy.ndarray[numpy.complex128, _Shape[m, 1]]) -> qulacs_core.QuantumGateDiagonalMatrix:
+
+def DiagonalMatrix(
+    index_list: typing.List[int], diagonal_element: numpy.ndarray
+) -> qulacs_core.QuantumGateDiagonalMatrix:
     """
     Create diagonal matrix gate
     """
+
 def FREDKIN(control: int, target1: int, target2: int) -> qulacs_core.QuantumGateMatrix:
     """
     Create FREDKIN gate
     """
+
 def FusedSWAP(target1: int, target2: int, block_size: int) -> ClsNpairQubitGate:
     """
     Create FusedSWAP gate
     """
+
 def H(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create Hadamard gate
     """
+
 def Identity(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create identity gate
     """
-def IndependentXZNoise(index: int, prob: float) -> qulacs_core.QuantumGate_Probabilistic:
+
+def IndependentXZNoise(
+    index: int, prob: float
+) -> qulacs_core.QuantumGate_Probabilistic:
     """
     Create independent XZ noise
     """
-def Instrument(kraus_list: typing.List[qulacs_core.QuantumGateBase], register: int) -> qulacs_core.QuantumGateBase:
+
+def Instrument(
+    kraus_list: typing.List[qulacs_core.QuantumGateBase], register: int
+) -> qulacs_core.QuantumGateBase:
     """
     Create instruments
     """
+
 def Measurement(index: int, register: int) -> qulacs_core.QuantumGate_CPTP:
     """
     Create measurement gate
     """
-def NoisyEvolution(hamiltonian: qulacs_core.Observable, c_ops: typing.List[qulacs_core.GeneralQuantumOperator], time: float, dt: float) -> qulacs_core.ClsNoisyEvolution:
+
+def NoisyEvolution(
+    hamiltonian: qulacs_core.Observable,
+    c_ops: typing.List[qulacs_core.GeneralQuantumOperator],
+    time: float,
+    dt: float,
+) -> qulacs_core.ClsNoisyEvolution:
     """
     Create noisy evolution
     """
-def NoisyEvolution_fast(hamiltonian: qulacs_core.Observable, c_ops: typing.List[qulacs_core.GeneralQuantumOperator], time: float) -> qulacs_core.ClsNoisyEvolution_fast:
+
+def NoisyEvolution_fast(
+    hamiltonian: qulacs_core.Observable,
+    c_ops: typing.List[qulacs_core.GeneralQuantumOperator],
+    time: float,
+) -> qulacs_core.ClsNoisyEvolution_fast:
     """
     Create noisy evolution fast version
     """
+
 def P0(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create projection gate to |0> subspace
     """
+
 def P1(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create projection gate to |1> subspace
     """
-def ParametricPauliRotation(index_list: typing.List[int], pauli_ids: typing.List[int], angle: float) -> qulacs_core.QuantumGate_SingleParameter:
+
+def ParametricPauliRotation(
+    index_list: typing.List[int], pauli_ids: typing.List[int], angle: float
+) -> qulacs_core.QuantumGate_SingleParameter:
     """
     Create parametric multi-qubit Pauli rotation gate
     """
+
 def ParametricRX(index: int, angle: float) -> qulacs_core.QuantumGate_SingleParameter:
     """
     Create parametric Pauli-X rotation gate
     """
+
 def ParametricRY(index: int, angle: float) -> qulacs_core.QuantumGate_SingleParameter:
     """
     Create parametric Pauli-Y rotation gate
     """
+
 def ParametricRZ(index: int, angle: float) -> qulacs_core.QuantumGate_SingleParameter:
     """
     Create parametric Pauli-Z rotation gate
     """
-def Pauli(index_list: typing.List[int], pauli_ids: typing.List[int]) -> qulacs_core.ClsPauliGate:
+
+def Pauli(
+    index_list: typing.List[int], pauli_ids: typing.List[int]
+) -> qulacs_core.ClsPauliGate:
     """
     Create multi-qubit Pauli gate
     """
-def PauliRotation(index_list: typing.List[int], pauli_ids: typing.List[int], angle: float) -> qulacs_core.ClsPauliRotationGate:
+
+def PauliRotation(
+    index_list: typing.List[int], pauli_ids: typing.List[int], angle: float
+) -> qulacs_core.ClsPauliRotationGate:
     """
     Create multi-qubit Pauli rotation
     """
-def Probabilistic(prob_list: typing.List[float], gate_list: typing.List[qulacs_core.QuantumGateBase]) -> qulacs_core.QuantumGateBase:
+
+def Probabilistic(
+    prob_list: typing.List[float], gate_list: typing.List[qulacs_core.QuantumGateBase]
+) -> qulacs_core.QuantumGateBase:
     """
     Create probabilistic gate
     """
-def ProbabilisticInstrument(prob_list: typing.List[float], gate_list: typing.List[qulacs_core.QuantumGateBase], register: int) -> qulacs_core.QuantumGateBase:
+
+def ProbabilisticInstrument(
+    prob_list: typing.List[float],
+    gate_list: typing.List[qulacs_core.QuantumGateBase],
+    register: int,
+) -> qulacs_core.QuantumGateBase:
     """
     Create probabilistic instrument gate
     """
+
 def RX(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate:
     """
     Create Pauli-X rotation gate
     """
+
 def RY(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate:
     """
     Create Pauli-Y rotation gate
     """
+
 def RZ(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate:
     """
     Create Pauli-Z rotation gate
     """
+
 @typing.overload
 def RandomUnitary(index_list: typing.List[int]) -> qulacs_core.QuantumGateMatrix:
     """
     Create random unitary gate
     """
+
 @typing.overload
-def RandomUnitary(index_list: typing.List[int], seed: int) -> qulacs_core.QuantumGateMatrix:
+def RandomUnitary(
+    index_list: typing.List[int], seed: int
+) -> qulacs_core.QuantumGateMatrix:
     pass
-def ReversibleBoolean(index_list: typing.List[int], func: typing.Callable[[int, int], int]) -> qulacs_core.ClsReversibleBooleanGate:
+
+def ReversibleBoolean(
+    index_list: typing.List[int], func: typing.Callable[[int, int], int]
+) -> qulacs_core.ClsReversibleBooleanGate:
     """
     Create reversible boolean gate
     """
+
 def RotInvX(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate:
     """
     Create Pauli-X rotation gate
     """
+
 def RotInvY(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate:
     """
     Create Pauli-Y rotation gate
     """
+
 def RotInvZ(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate:
     """
     Create Pauli-Z rotation gate
     """
+
 def RotX(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate:
     """
     Create Pauli-X rotation gate
     """
+
 def RotY(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate:
     """
     Create Pauli-Y rotation gate
     """
+
 def RotZ(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate:
     """
     Create Pauli-Z rotation gate
     """
+
 def S(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create pi/4-phase gate
     """
+
 def SWAP(target1: int, target2: int) -> qulacs_core.ClsTwoQubitGate:
     """
     Create SWAP gate
     """
+
 def Sdag(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create adjoint of pi/4-phase gate
     """
-def SparseMatrix(index_list: typing.List[int], matrix: scipy.sparse.csc_matrix[numpy.complex128]) -> qulacs_core.QuantumGateSparseMatrix:
+
+def SparseMatrix(
+    index_list: typing.List[int], matrix: scipy.sparse.csc_matrix[numpy.complex128]
+) -> qulacs_core.QuantumGateSparseMatrix:
     """
     Create sparse matrix gate
     """
-def StateReflection(state: qulacs_core.QuantumState) -> qulacs_core.ClsStateReflectionGate:
+
+def StateReflection(
+    state: qulacs_core.QuantumState,
+) -> qulacs_core.ClsStateReflectionGate:
     """
     Create state reflection gate
     """
+
 def T(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create pi/8-phase gate
     """
+
 def TOFFOLI(control1: int, control2: int, target: int) -> qulacs_core.QuantumGateMatrix:
     """
     Create TOFFOLI gate
     """
+
 def Tdag(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create adjoint of pi/8-phase gate
     """
-def TwoQubitDepolarizingNoise(index1: int, index2: int, prob: float) -> qulacs_core.QuantumGate_Probabilistic:
+
+def TwoQubitDepolarizingNoise(
+    index1: int, index2: int, prob: float
+) -> qulacs_core.QuantumGate_Probabilistic:
     """
     Create two-qubit depolarizing noise
     """
+
 def U1(index: int, lambda_: float) -> qulacs_core.QuantumGateMatrix:
     """
     Create QASM U1 gate
     """
+
 def U2(index: int, phi: float, lambda_: float) -> qulacs_core.QuantumGateMatrix:
     """
     Create QASM U2 gate
     """
-def U3(index: int, theta: float, phi: float, lambda_: float) -> qulacs_core.QuantumGateMatrix:
+
+def U3(
+    index: int, theta: float, phi: float, lambda_: float
+) -> qulacs_core.QuantumGateMatrix:
     """
     Create QASM U3 gate
     """
+
 def X(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create Pauli-X gate
     """
+
 def Y(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create Pauli-Y gate
     """
+
 def Z(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create Pauli-Z gate
     """
+
 @typing.overload
-def add(gate1: qulacs_core.QuantumGateBase, gate2: qulacs_core.QuantumGateBase) -> qulacs_core.QuantumGateMatrix:
+def add(
+    gate1: qulacs_core.QuantumGateBase, gate2: qulacs_core.QuantumGateBase
+) -> qulacs_core.QuantumGateMatrix:
     """
     Add quantum gate matrices
 
     Add quantum gate matrices
     """
+
 @typing.overload
-def add(gate_list: typing.List[qulacs_core.QuantumGateBase]) -> qulacs_core.QuantumGateMatrix:
+def add(
+    gate_list: typing.List[qulacs_core.QuantumGateBase],
+) -> qulacs_core.QuantumGateMatrix:
     pass
+
 def from_json(arg0: str) -> qulacs_core.QuantumGateBase:
     """
     from json string
     """
+
 @typing.overload
-def merge(gate1: qulacs_core.QuantumGateBase, gate2: qulacs_core.QuantumGateBase) -> qulacs_core.QuantumGateMatrix:
+def merge(
+    gate1: qulacs_core.QuantumGateBase, gate2: qulacs_core.QuantumGateBase
+) -> qulacs_core.QuantumGateMatrix:
     """
     Merge two quantum gate or gate list
     """
+
 @typing.overload
-def merge(gate_list: typing.List[qulacs_core.QuantumGateBase]) -> qulacs_core.QuantumGateMatrix:
+def merge(
+    gate_list: typing.List[qulacs_core.QuantumGateBase],
+) -> qulacs_core.QuantumGateMatrix:
     pass
+
 def sqrtX(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create pi/4 Pauli-X rotation gate
     """
+
 def sqrtXdag(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create adjoint of pi/4 Pauli-X rotation gate
     """
+
 def sqrtY(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create pi/4 Pauli-Y rotation gate
     """
+
 def sqrtYdag(index: int) -> qulacs_core.ClsOneQubitGate:
     """
     Create adjoint of pi/4 Pauli-Y rotation gate
     """
+
 def to_matrix_gate(gate: qulacs_core.QuantumGateBase) -> qulacs_core.QuantumGateMatrix:
     """
     Convert named gate to matrix gate
     """
```

### Comparing `qulacs-0.6.0/pysrc/qulacs/gate.pyi` & `qulacs-0.6.1/pysrc/qulacs/gate.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,86 +1,161 @@
-from typing import Callable, List
+from typing import Callable, List, overload
 
-from typing import overload
 import numpy
 import qulacs_core
 import scipy.sparse
 
 @overload
-def Adaptive(gate: qulacs_core.QuantumGateBase, condition: Callable[[List[int]],bool]) -> qulacs_core.QuantumGateBase: ...
-@overload
-def Adaptive(gate: qulacs_core.QuantumGateBase, condition: Callable[[List[int],int],bool], id: int) -> qulacs_core.QuantumGateBase: ...
+def Adaptive(
+    gate: qulacs_core.QuantumGateBase, condition: Callable[[List[int]], bool]
+) -> qulacs_core.QuantumGateBase: ...
+@overload
+def Adaptive(
+    gate: qulacs_core.QuantumGateBase,
+    condition: Callable[[List[int], int], bool],
+    id: int,
+) -> qulacs_core.QuantumGateBase: ...
 def AmplitudeDampingNoise(index: int, prob: float) -> qulacs_core.QuantumGate_CPTP: ...
 def BitFlipNoise(index: int, prob: float) -> qulacs_core.QuantumGate_Probabilistic: ...
 def CNOT(control: int, target: int) -> qulacs_core.ClsOneControlOneTargetGate: ...
-def CP(kraus_list: List[qulacs_core.QuantumGateBase], state_normalize: bool, probability_normalize: bool, assign_zero_if_not_matched: bool) -> qulacs_core.QuantumGateBase: ...
-def CPTP(kraus_list: List[qulacs_core.QuantumGateBase]) -> qulacs_core.QuantumGateBase: ...
+def CP(
+    kraus_list: List[qulacs_core.QuantumGateBase],
+    state_normalize: bool,
+    probability_normalize: bool,
+    assign_zero_if_not_matched: bool,
+) -> qulacs_core.QuantumGateBase: ...
+def CPTP(
+    kraus_list: List[qulacs_core.QuantumGateBase],
+) -> qulacs_core.QuantumGateBase: ...
 def CZ(control: int, target: int) -> qulacs_core.ClsOneControlOneTargetGate: ...
 @overload
-def DenseMatrix(index: int, matrix: numpy.ndarray[numpy.complex128[m,n]]) -> qulacs_core.QuantumGateMatrix: ...
-@overload
-def DenseMatrix(index_list: List[int], matrix: numpy.ndarray[numpy.complex128[m,n]]) -> qulacs_core.QuantumGateMatrix: ...
-def DephasingNoise(index: int, prob: float) -> qulacs_core.QuantumGate_Probabilistic: ...
-def DepolarizingNoise(index: int, prob: float) -> qulacs_core.QuantumGate_Probabilistic: ...
-def DiagonalMatrix(index_list: List[int], diagonal_element: numpy.ndarray[numpy.complex128[m,1]]) -> qulacs_core.QuantumGateDiagonalMatrix: ...
-def FREDKIN(control: int, target1: int, target2: int) -> qulacs_core.QuantumGateMatrix: ...
+def DenseMatrix(
+    index: int, matrix: numpy.ndarray[numpy.complex128[m, n]]
+) -> qulacs_core.QuantumGateMatrix: ...
+@overload
+def DenseMatrix(
+    index_list: List[int], matrix: numpy.ndarray[numpy.complex128[m, n]]
+) -> qulacs_core.QuantumGateMatrix: ...
+def DephasingNoise(
+    index: int, prob: float
+) -> qulacs_core.QuantumGate_Probabilistic: ...
+def DepolarizingNoise(
+    index: int, prob: float
+) -> qulacs_core.QuantumGate_Probabilistic: ...
+def DiagonalMatrix(
+    index_list: List[int], diagonal_element: numpy.ndarray[numpy.complex128[m, 1]]
+) -> qulacs_core.QuantumGateDiagonalMatrix: ...
+def FREDKIN(
+    control: int, target1: int, target2: int
+) -> qulacs_core.QuantumGateMatrix: ...
 def FusedSWAP(target1: int, target2: int, block_size: int) -> ClsNpairQubitGate: ...
 def H(index: int) -> qulacs_core.ClsOneQubitGate: ...
 def Identity(index: int) -> qulacs_core.ClsOneQubitGate: ...
-def IndependentXZNoise(index: int, prob: float) -> qulacs_core.QuantumGate_Probabilistic: ...
-def Instrument(kraus_list: List[qulacs_core.QuantumGateBase], register: int) -> qulacs_core.QuantumGateBase: ...
+def IndependentXZNoise(
+    index: int, prob: float
+) -> qulacs_core.QuantumGate_Probabilistic: ...
+def Instrument(
+    kraus_list: List[qulacs_core.QuantumGateBase], register: int
+) -> qulacs_core.QuantumGateBase: ...
 def Measurement(index: int, register: int) -> qulacs_core.QuantumGate_CPTP: ...
-def NoisyEvolution(hamiltonian: qulacs_core.Observable, c_ops: List[qulacs_core.GeneralQuantumOperator], time: float, dt: float) -> qulacs_core.ClsNoisyEvolution: ...
-def NoisyEvolution_fast(hamiltonian: qulacs_core.Observable, c_ops: List[qulacs_core.GeneralQuantumOperator], time: float) -> qulacs_core.ClsNoisyEvolution_fast: ...
+def NoisyEvolution(
+    hamiltonian: qulacs_core.Observable,
+    c_ops: List[qulacs_core.GeneralQuantumOperator],
+    time: float,
+    dt: float,
+) -> qulacs_core.ClsNoisyEvolution: ...
+def NoisyEvolution_fast(
+    hamiltonian: qulacs_core.Observable,
+    c_ops: List[qulacs_core.GeneralQuantumOperator],
+    time: float,
+) -> qulacs_core.ClsNoisyEvolution_fast: ...
 def P0(index: int) -> qulacs_core.ClsOneQubitGate: ...
 def P1(index: int) -> qulacs_core.ClsOneQubitGate: ...
-def ParametricPauliRotation(index_list: List[int], pauli_ids: List[int], angle: float) -> qulacs_core.QuantumGate_SingleParameter: ...
-def ParametricRX(index: int, angle: float) -> qulacs_core.QuantumGate_SingleParameter: ...
-def ParametricRY(index: int, angle: float) -> qulacs_core.QuantumGate_SingleParameter: ...
-def ParametricRZ(index: int, angle: float) -> qulacs_core.QuantumGate_SingleParameter: ...
+def ParametricPauliRotation(
+    index_list: List[int], pauli_ids: List[int], angle: float
+) -> qulacs_core.QuantumGate_SingleParameter: ...
+def ParametricRX(
+    index: int, angle: float
+) -> qulacs_core.QuantumGate_SingleParameter: ...
+def ParametricRY(
+    index: int, angle: float
+) -> qulacs_core.QuantumGate_SingleParameter: ...
+def ParametricRZ(
+    index: int, angle: float
+) -> qulacs_core.QuantumGate_SingleParameter: ...
 def Pauli(index_list: List[int], pauli_ids: List[int]) -> qulacs_core.ClsPauliGate: ...
-def PauliRotation(index_list: List[int], pauli_ids: List[int], angle: float) -> qulacs_core.ClsPauliRotationGate: ...
-def Probabilistic(prob_list: List[float], gate_list: List[qulacs_core.QuantumGateBase]) -> qulacs_core.QuantumGateBase: ...
-def ProbabilisticInstrument(prob_list: List[float], gate_list: List[qulacs_core.QuantumGateBase], register: int) -> qulacs_core.QuantumGateBase: ...
+def PauliRotation(
+    index_list: List[int], pauli_ids: List[int], angle: float
+) -> qulacs_core.ClsPauliRotationGate: ...
+def Probabilistic(
+    prob_list: List[float], gate_list: List[qulacs_core.QuantumGateBase]
+) -> qulacs_core.QuantumGateBase: ...
+def ProbabilisticInstrument(
+    prob_list: List[float], gate_list: List[qulacs_core.QuantumGateBase], register: int
+) -> qulacs_core.QuantumGateBase: ...
 def RX(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate: ...
 def RY(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate: ...
 def RZ(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate: ...
 @overload
 def RandomUnitary(index_list: List[int]) -> qulacs_core.QuantumGateMatrix: ...
 @overload
-def RandomUnitary(index_list: List[int], seed: int) -> qulacs_core.QuantumGateMatrix: ...
-def ReversibleBoolean(index_list: List[int], func: Callable[[int,int],int]) -> qulacs_core.ClsReversibleBooleanGate: ...
+def RandomUnitary(
+    index_list: List[int], seed: int
+) -> qulacs_core.QuantumGateMatrix: ...
+def ReversibleBoolean(
+    index_list: List[int], func: Callable[[int, int], int]
+) -> qulacs_core.ClsReversibleBooleanGate: ...
 def RotInvX(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate: ...
 def RotInvY(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate: ...
 def RotInvZ(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate: ...
 def RotX(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate: ...
 def RotY(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate: ...
 def RotZ(index: int, angle: float) -> qulacs_core.ClsOneQubitRotationGate: ...
 def S(index: int) -> qulacs_core.ClsOneQubitGate: ...
 def SWAP(target1: int, target2: int) -> qulacs_core.ClsTwoQubitGate: ...
 def Sdag(index: int) -> qulacs_core.ClsOneQubitGate: ...
-def SparseMatrix(index_list: List[int], matrix: scipy.sparse.csc_matrix[numpy.complex128]) -> qulacs_core.QuantumGateSparseMatrix: ...
-def StateReflection(state: qulacs_core.QuantumState) -> qulacs_core.ClsStateReflectionGate: ...
+def SparseMatrix(
+    index_list: List[int], matrix: scipy.sparse.csc_matrix[numpy.complex128]
+) -> qulacs_core.QuantumGateSparseMatrix: ...
+def StateReflection(
+    state: qulacs_core.QuantumState,
+) -> qulacs_core.ClsStateReflectionGate: ...
 def T(index: int) -> qulacs_core.ClsOneQubitGate: ...
-def TOFFOLI(control1: int, control2: int, target: int) -> qulacs_core.QuantumGateMatrix: ...
+def TOFFOLI(
+    control1: int, control2: int, target: int
+) -> qulacs_core.QuantumGateMatrix: ...
 def Tdag(index: int) -> qulacs_core.ClsOneQubitGate: ...
-def TwoQubitDepolarizingNoise(index1: int, index2: int, prob: float) -> qulacs_core.QuantumGate_Probabilistic: ...
+def TwoQubitDepolarizingNoise(
+    index1: int, index2: int, prob: float
+) -> qulacs_core.QuantumGate_Probabilistic: ...
 def U1(index: int, lambda_: float) -> qulacs_core.QuantumGateMatrix: ...
 def U2(index: int, phi: float, lambda_: float) -> qulacs_core.QuantumGateMatrix: ...
-def U3(index: int, theta: float, phi: float, lambda_: float) -> qulacs_core.QuantumGateMatrix: ...
+def U3(
+    index: int, theta: float, phi: float, lambda_: float
+) -> qulacs_core.QuantumGateMatrix: ...
 def X(index: int) -> qulacs_core.ClsOneQubitGate: ...
 def Y(index: int) -> qulacs_core.ClsOneQubitGate: ...
 def Z(index: int) -> qulacs_core.ClsOneQubitGate: ...
 @overload
-def add(gate1: qulacs_core.QuantumGateBase, gate2: qulacs_core.QuantumGateBase) -> qulacs_core.QuantumGateMatrix: ...
-@overload
-def add(gate_list: List[qulacs_core.QuantumGateBase]) -> qulacs_core.QuantumGateMatrix: ...
+def add(
+    gate1: qulacs_core.QuantumGateBase, gate2: qulacs_core.QuantumGateBase
+) -> qulacs_core.QuantumGateMatrix: ...
+@overload
+def add(
+    gate_list: List[qulacs_core.QuantumGateBase],
+) -> qulacs_core.QuantumGateMatrix: ...
 def from_json(arg0: str) -> qulacs_core.QuantumGateBase: ...
 @overload
-def merge(gate1: qulacs_core.QuantumGateBase, gate2: qulacs_core.QuantumGateBase) -> qulacs_core.QuantumGateMatrix: ...
-@overload
-def merge(gate_list: List[qulacs_core.QuantumGateBase]) -> qulacs_core.QuantumGateMatrix: ...
+def merge(
+    gate1: qulacs_core.QuantumGateBase, gate2: qulacs_core.QuantumGateBase
+) -> qulacs_core.QuantumGateMatrix: ...
+@overload
+def merge(
+    gate_list: List[qulacs_core.QuantumGateBase],
+) -> qulacs_core.QuantumGateMatrix: ...
 def sqrtX(index: int) -> qulacs_core.ClsOneQubitGate: ...
 def sqrtXdag(index: int) -> qulacs_core.ClsOneQubitGate: ...
 def sqrtY(index: int) -> qulacs_core.ClsOneQubitGate: ...
 def sqrtYdag(index: int) -> qulacs_core.ClsOneQubitGate: ...
-def to_matrix_gate(gate: qulacs_core.QuantumGateBase) -> qulacs_core.QuantumGateMatrix: ...
+def to_matrix_gate(
+    gate: qulacs_core.QuantumGateBase,
+) -> qulacs_core.QuantumGateMatrix: ...
```

### Comparing `qulacs-0.6.0/pysrc/qulacs/observable/__init__.pyi` & `qulacs-0.6.1/pysrc/qulacs/observable/__init__.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 from __future__ import annotations
-import qulacs_core.observable
+
 import typing
+
 import qulacs_core
+import qulacs_core.observable
 
 __all__ = [
     "create_observable_from_openfermion_file",
     "create_observable_from_openfermion_text",
     "create_split_observable",
-    "from_json"
+    "from_json",
 ]
 
-
 def create_observable_from_openfermion_file(file_path: str) -> qulacs_core.Observable:
     """
     Create GeneralQuantumOperator from openfermion file
     """
+
 def create_observable_from_openfermion_text(text: str) -> qulacs_core.Observable:
     """
     Create GeneralQuantumOperator from openfermion text
     """
-def create_split_observable(arg0: str) -> typing.Tuple[qulacs_core.Observable, qulacs_core.Observable]:
+
+def create_split_observable(
+    arg0: str,
+) -> typing.Tuple[qulacs_core.Observable, qulacs_core.Observable]:
     pass
+
 def from_json(json: str) -> qulacs_core.Observable:
     """
     from json string
     """
```

### Comparing `qulacs-0.6.0/pysrc/qulacs/quantum_operator/__init__.pyi` & `qulacs-0.6.1/pysrc/qulacs/quantum_operator/__init__.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 from __future__ import annotations
-import qulacs_core.quantum_operator
+
 import typing
+
 import qulacs_core
+import qulacs_core.quantum_operator
 
 __all__ = [
     "create_quantum_operator_from_openfermion_file",
     "create_quantum_operator_from_openfermion_text",
     "create_split_quantum_operator",
-    "from_json"
+    "from_json",
 ]
 
-
-def create_quantum_operator_from_openfermion_file(arg0: str) -> qulacs_core.GeneralQuantumOperator:
+def create_quantum_operator_from_openfermion_file(
+    arg0: str,
+) -> qulacs_core.GeneralQuantumOperator:
     pass
-def create_quantum_operator_from_openfermion_text(arg0: str) -> qulacs_core.GeneralQuantumOperator:
+
+def create_quantum_operator_from_openfermion_text(
+    arg0: str,
+) -> qulacs_core.GeneralQuantumOperator:
     pass
-def create_split_quantum_operator(arg0: str) -> typing.Tuple[qulacs_core.GeneralQuantumOperator, qulacs_core.GeneralQuantumOperator]:
+
+def create_split_quantum_operator(
+    arg0: str,
+) -> typing.Tuple[
+    qulacs_core.GeneralQuantumOperator, qulacs_core.GeneralQuantumOperator
+]:
     pass
+
 def from_json(json: str) -> qulacs_core.GeneralQuantumOperator:
     """
     from json string
     """
```

### Comparing `qulacs-0.6.0/pysrc/qulacs/state/__init__.pyi` & `qulacs-0.6.1/pysrc/qulacs/state/__init__.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,100 @@
 from __future__ import annotations
-import qulacs_core.state
+
 import typing
+
 import qulacs_core
+import qulacs_core.state
 
 __all__ = [
     "drop_qubit",
     "from_json",
     "inner_product",
     "make_mixture",
     "make_superposition",
     "partial_trace",
     "permutate_qubit",
-    "tensor_product"
+    "tensor_product",
 ]
 
-
-def drop_qubit(state: qulacs_core.QuantumState, target: typing.List[int], projection: typing.List[int]) -> qulacs_core.QuantumState:
+def drop_qubit(
+    state: qulacs_core.QuantumState,
+    target: typing.List[int],
+    projection: typing.List[int],
+) -> qulacs_core.QuantumState:
     """
     Drop qubits from state
     """
+
 def from_json(json: str) -> qulacs_core.QuantumStateBase:
     """
     from json string
     """
-def inner_product(state_bra: qulacs_core.QuantumState, state_ket: qulacs_core.QuantumState) -> complex:
+
+def inner_product(
+    state_bra: qulacs_core.QuantumState, state_ket: qulacs_core.QuantumState
+) -> complex:
     """
     Get inner product
     """
-def make_mixture(prob1: complex, state1: qulacs_core.QuantumStateBase, prob2: complex, state2: qulacs_core.QuantumStateBase) -> qulacs_core.DensityMatrix:
+
+def make_mixture(
+    prob1: complex,
+    state1: qulacs_core.QuantumStateBase,
+    prob2: complex,
+    state2: qulacs_core.QuantumStateBase,
+) -> qulacs_core.DensityMatrix:
     """
     Create a mixed state
     """
-def make_superposition(coef1: complex, state1: qulacs_core.QuantumState, coef2: complex, state2: qulacs_core.QuantumState) -> qulacs_core.QuantumState:
+
+def make_superposition(
+    coef1: complex,
+    state1: qulacs_core.QuantumState,
+    coef2: complex,
+    state2: qulacs_core.QuantumState,
+) -> qulacs_core.QuantumState:
     """
     Create superposition of states
     """
+
 @typing.overload
-def partial_trace(state: qulacs_core.DensityMatrix, target_traceout: typing.List[int]) -> qulacs_core.DensityMatrix:
+def partial_trace(
+    state: qulacs_core.QuantumState, target_traceout: typing.List[int]
+) -> qulacs_core.DensityMatrix:
     """
     Take partial trace
     """
+
 @typing.overload
-def partial_trace(state: qulacs_core.QuantumState, target_traceout: typing.List[int]) -> qulacs_core.DensityMatrix:
+def partial_trace(
+    state: qulacs_core.DensityMatrix, target_traceout: typing.List[int]
+) -> qulacs_core.DensityMatrix:
     pass
+
 @typing.overload
-def permutate_qubit(state: qulacs_core.DensityMatrix, qubit_order: typing.List[int]) -> qulacs_core.DensityMatrix:
+def permutate_qubit(
+    state: qulacs_core.QuantumState, qubit_order: typing.List[int]
+) -> qulacs_core.QuantumState:
     """
     Permutate qubits from state
     """
+
 @typing.overload
-def permutate_qubit(state: qulacs_core.QuantumState, qubit_order: typing.List[int]) -> qulacs_core.QuantumState:
+def permutate_qubit(
+    state: qulacs_core.DensityMatrix, qubit_order: typing.List[int]
+) -> qulacs_core.DensityMatrix:
     pass
+
 @typing.overload
-def tensor_product(state_left: qulacs_core.DensityMatrix, state_right: qulacs_core.DensityMatrix) -> qulacs_core.DensityMatrix:
+def tensor_product(
+    state_left: qulacs_core.QuantumState, state_right: qulacs_core.QuantumState
+) -> qulacs_core.QuantumState:
     """
     Get tensor product of states
     """
+
 @typing.overload
-def tensor_product(state_left: qulacs_core.QuantumState, state_right: qulacs_core.QuantumState) -> qulacs_core.QuantumState:
+def tensor_product(
+    state_left: qulacs_core.DensityMatrix, state_right: qulacs_core.DensityMatrix
+) -> qulacs_core.DensityMatrix:
     pass
```

### Comparing `qulacs-0.6.0/pysrc/qulacs/state.pyi` & `qulacs-0.6.1/pysrc/qulacs/state.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,47 @@
-from typing import List
+from typing import List, overload
 
-from typing import overload
 import qulacs_core
 
-def drop_qubit(state: qulacs_core.QuantumState, target: List[int], projection: List[int]) -> qulacs_core.QuantumState: ...
+def drop_qubit(
+    state: qulacs_core.QuantumState, target: List[int], projection: List[int]
+) -> qulacs_core.QuantumState: ...
 def from_json(json: str) -> qulacs_core.QuantumStateBase: ...
-def inner_product(state_bra: qulacs_core.QuantumState, state_ket: qulacs_core.QuantumState) -> complex: ...
-def make_mixture(prob1: complex, state1: qulacs_core.QuantumStateBase, prob2: complex, state2: qulacs_core.QuantumStateBase) -> qulacs_core.DensityMatrix: ...
-def make_superposition(coef1: complex, state1: qulacs_core.QuantumState, coef2: complex, state2: qulacs_core.QuantumState) -> qulacs_core.QuantumState: ...
-@overload
-def partial_trace(state: qulacs_core.QuantumState, target_traceout: List[int]) -> qulacs_core.DensityMatrix: ...
-@overload
-def partial_trace(state: qulacs_core.DensityMatrix, target_traceout: List[int]) -> qulacs_core.DensityMatrix: ...
-@overload
-def permutate_qubit(state: qulacs_core.QuantumState, qubit_order: List[int]) -> qulacs_core.QuantumState: ...
-@overload
-def permutate_qubit(state: qulacs_core.DensityMatrix, qubit_order: List[int]) -> qulacs_core.DensityMatrix: ...
-@overload
-def tensor_product(state_left: qulacs_core.QuantumState, state_right: qulacs_core.QuantumState) -> qulacs_core.QuantumState: ...
-@overload
-def tensor_product(state_left: qulacs_core.DensityMatrix, state_right: qulacs_core.DensityMatrix) -> qulacs_core.DensityMatrix: ...
+def inner_product(
+    state_bra: qulacs_core.QuantumState, state_ket: qulacs_core.QuantumState
+) -> complex: ...
+def make_mixture(
+    prob1: complex,
+    state1: qulacs_core.QuantumStateBase,
+    prob2: complex,
+    state2: qulacs_core.QuantumStateBase,
+) -> qulacs_core.DensityMatrix: ...
+def make_superposition(
+    coef1: complex,
+    state1: qulacs_core.QuantumState,
+    coef2: complex,
+    state2: qulacs_core.QuantumState,
+) -> qulacs_core.QuantumState: ...
+@overload
+def partial_trace(
+    state: qulacs_core.QuantumState, target_traceout: List[int]
+) -> qulacs_core.DensityMatrix: ...
+@overload
+def partial_trace(
+    state: qulacs_core.DensityMatrix, target_traceout: List[int]
+) -> qulacs_core.DensityMatrix: ...
+@overload
+def permutate_qubit(
+    state: qulacs_core.QuantumState, qubit_order: List[int]
+) -> qulacs_core.QuantumState: ...
+@overload
+def permutate_qubit(
+    state: qulacs_core.DensityMatrix, qubit_order: List[int]
+) -> qulacs_core.DensityMatrix: ...
+@overload
+def tensor_product(
+    state_left: qulacs_core.QuantumState, state_right: qulacs_core.QuantumState
+) -> qulacs_core.QuantumState: ...
+@overload
+def tensor_product(
+    state_left: qulacs_core.DensityMatrix, state_right: qulacs_core.DensityMatrix
+) -> qulacs_core.DensityMatrix: ...
```

### Comparing `qulacs-0.6.0/pysrc/qulacs/utils/conversions_openfermion.py` & `qulacs-0.6.1/pysrc/qulacs/utils/conversions_openfermion.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-
-from qulacs_core import GeneralQuantumOperator
 import numpy as np
+from qulacs_core import GeneralQuantumOperator
 
 
 def convert_openfermion_op(openfermion_op, n_qubits=None):
     """convert_openfermion_op
     Args:
         openfermion_op (:class:`openfermion.ops.QubitOperator`)
         n_qubit (:class:`int`):
@@ -15,18 +14,18 @@
     if n_qubits is None:
         _n_qubits = _count_qubit_in_qubit_operator(openfermion_op)
     else:
         _n_qubits = n_qubits
     res = GeneralQuantumOperator(_n_qubits)
     for pauli_product in openfermion_op.terms:
         coef = float(np.real(openfermion_op.terms[pauli_product]))
-        pauli_string = ''
+        pauli_string = ""
         for pauli_operator in pauli_product:
-            pauli_string += pauli_operator[1] + ' ' + str(pauli_operator[0])
-            pauli_string += ' '
+            pauli_string += pauli_operator[1] + " " + str(pauli_operator[0])
+            pauli_string += " "
         res.add_operator(coef, pauli_string[:-1])
     return res
 
 
 def _count_qubit_in_qubit_operator(op):
     """_count_qubit_in_qubit_operator
     counts minimal number of qubits required to represent a given QubitOperator
@@ -36,8 +35,8 @@
         :class: `int`
     """
     n_qubits = 0
     for pauli_product in op.terms:
         for pauli_operator in pauli_product:
             if n_qubits < pauli_operator[0]:
                 n_qubits = pauli_operator[0]
-    return n_qubits+1
+    return n_qubits + 1
```

### Comparing `qulacs-0.6.0/pysrc/qulacs/vistest/test_vis.py` & `qulacs-0.6.1/pysrc/qulacs/vistest/test_vis.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-import numpy as np
-from qulacs import Observable, QuantumState
-from qulacs.gate import to_matrix_gate, X,Y,Z, CNOT, H, RX, RY
-from qulacs.visualizer import show_blochsphere,show_amplitude,show_probability
-
-
+from qulacs import QuantumState
+from qulacs.gate import CNOT, RY, H, X, Z
+from qulacs.visualizer import (
+    show_amplitude,
+    show_blochsphere,
+    show_probability,
+)
 
 
 def test_amp_pro():
     """適当な量子状態をつくって、棒グラフを表示するテスト用関数。"""
     n = 3
     state = QuantumState(n)
-    #state.set_Haar_random_state()
+    # state.set_Haar_random_state()
     show_amplitude(state)
     show_probability(state)
     X(0).update_quantum_state(state)
     show_amplitude(state)
     show_probability(state)
     H(0).update_quantum_state(state)
     show_amplitude(state)
```

### Comparing `qulacs-0.6.0/pysrc/qulacs/visualizer/visualizer.py` & `qulacs-0.6.1/pysrc/qulacs/visualizer/visualizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 """回路のグラフ化をできます。量子状態の棒グラフ、縮約した後の玉表示"""
-import numpy as np
 import matplotlib.pyplot as plt
-from mpl_toolkits.mplot3d import Axes3D
-from qulacs import Observable, QuantumState
+import numpy as np
 
-import matplotlib.colors
+from qulacs import Observable, QuantumState
 
 # bar(x, y, color=["red", "blue", "green", "pink", "orange"], width=0.5)
 
+
 def cmp_to_color(z):
     """複素数を受け取って、色を返す"""
     arg_rad = np.angle(z)
 
-    color=(np.cos(arg_rad)*0.5+0.5,np.cos(arg_rad+np.pi*0.667)*0.5+0.5,np.cos(arg_rad+np.pi*1.333)*0.5+0.5 )
+    color = (
+        np.cos(arg_rad) * 0.5 + 0.5,
+        np.cos(arg_rad + np.pi * 0.667) * 0.5 + 0.5,
+        np.cos(arg_rad + np.pi * 1.333) * 0.5 + 0.5,
+    )
     return color
 
+
 def show_amplitude(state):
     """純粋状態量子状態を受け取って、棒グラフを表示する"""
     n_qubit = state.get_qubit_count()
-    aaa=state.get_vector()
-    bits=[]
-    ys=[]
-    colors=[]
+    aaa = state.get_vector()
+    bits = []
+    ys = []
+    colors = []
     for i in range(2**n_qubit):
         print(aaa[i])
-        moziretu='{:b}'.format(i)
-        while len(moziretu)<n_qubit:
-            moziretu="0"+moziretu
+        moziretu = "{:b}".format(i)
+        while len(moziretu) < n_qubit:
+            moziretu = "0" + moziretu
         bits.append(moziretu)
 
         ys.append(abs(aaa[i]))
-        colors.append(cmp_to_color(aaa[i]))    
-    plt.bar(bits,ys,color=colors)
+        colors.append(cmp_to_color(aaa[i]))
+    plt.bar(bits, ys, color=colors)
     plt.show()
 
 
 def show_blochsphere(state, bit):
     """ブロッホ球の表示をします"""
     n_qubit = state.get_qubit_count()
     observableX = Observable(n_qubit)
@@ -66,27 +70,26 @@
     ax.set_zlabel("Z-axis")
     plt.show()
 
 
 def show_probability(state):
     """量子状態を受け取って、　出現確率の棒グラフを表示します。"""
     n_qubit = state.get_qubit_count()
-    bits=[]
-    ys=np.zeros(2**n_qubit)
+    bits = []
+    ys = np.zeros(2**n_qubit)
     for i in range(2**n_qubit):
-        moziretu='{:b}'.format(i)
-        while len(moziretu)<n_qubit:
-            moziretu="0"+moziretu
+        moziretu = "{:b}".format(i)
+        while len(moziretu) < n_qubit:
+            moziretu = "0" + moziretu
         bits.append(moziretu)
 
-    if isinstance(state,QuantumState):
-        aaa=state.get_vector()
+    if isinstance(state, QuantumState):
+        aaa = state.get_vector()
         for i in range(2**n_qubit):
-            ys[i]+=abs(aaa[i])**2
+            ys[i] += abs(aaa[i]) ** 2
     else:
-        aaa=state.get_matrix()
+        aaa = state.get_matrix()
         for h in range(len(aaa)):
             for i in range(2**n_qubit):
-                ys[i]+=abs(aaa[h][i])**2
-    plt.bar(bits,ys)
+                ys[i] += abs(aaa[h][i]) ** 2
+    plt.bar(bits, ys)
     plt.show()
-
```

### Comparing `qulacs-0.6.0/pysrc/qulacs.egg-info/PKG-INFO` & `qulacs-0.6.1/pysrc/qulacs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qulacs
-Version: 0.6.0
+Version: 0.6.1
 Summary: Quantum circuit simulator for research
 Author-email: QunaSys <qulacs@qunasys.com>
 License: MIT License
         
         Copyright (c) 2018 Qulacs Authors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `qulacs-0.6.0/pysrc/qulacs.egg-info/SOURCES.txt` & `qulacs-0.6.1/pysrc/qulacs.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 .readthedocs.yaml
 CMakeLists.txt
 CONTRIBUTING.md
 LICENSE
 README.md
 README_MPI.md
 _config.yml
+codecov.yml
 pyproject.toml
+setup.cfg
 setup.py
 .devcontainer/cpu/Dockerfile
 .devcontainer/cpu/devcontainer.json
 .devcontainer/gpu/Dockerfile
 .devcontainer/gpu/devcontainer.json
 .github/workflows/ci_macos.yml
 .github/workflows/ci_ubuntu.yml
@@ -123,15 +125,14 @@
 pysrc/qulacs/converter/__init__.py
 pysrc/qulacs/converter/qasm_converter.py
 pysrc/qulacs/gate/__init__.py
 pysrc/qulacs/gate/__init__.pyi
 pysrc/qulacs/gate/py.typed
 pysrc/qulacs/observable/__init__.py
 pysrc/qulacs/observable/__init__.pyi
-pysrc/qulacs/observable/_get_matrix.py
 pysrc/qulacs/observable/py.typed
 pysrc/qulacs/quantum_operator/__init__.py
 pysrc/qulacs/quantum_operator/__init__.pyi
 pysrc/qulacs/quantum_operator/py.typed
 pysrc/qulacs/state/__init__.py
 pysrc/qulacs/state/__init__.pyi
 pysrc/qulacs/state/py.typed
@@ -140,30 +141,43 @@
 pysrc/qulacs/vistest/__init__.py
 pysrc/qulacs/vistest/test_vis.py
 pysrc/qulacs/visualizer/__init__.py
 pysrc/qulacs/visualizer/visualizer.py
 python/CMakeLists.txt
 python/cppsim_wrapper.cpp
 python/stub-test/generate_mypy_tester.py
-python/test/test_qulacs.py
-python/test/test_qulacs_multicpu.py
+python/tests/__init__.py
+python/tests/multi_cpu/conftest.py
+python/tests/multi_cpu/test_state_multi_cpu.py
+python/tests/single_cpu/conftest.py
+python/tests/single_cpu/test_circuit.py
+python/tests/single_cpu/test_density_matrix_handling.py
+python/tests/single_cpu/test_json.py
+python/tests/single_cpu/test_noise_simulator.py
+python/tests/single_cpu/test_observable.py
+python/tests/single_cpu/test_pickle.py
+python/tests/single_cpu/test_pointer_handling.py
+python/tests/single_cpu/test_qasm.py
+python/tests/single_cpu/test_state.py
+python/tests/single_cpu/test_utils.py
 script/build_clang.sh
 script/build_gcc.sh
 script/build_gcc_with_gpu.sh
 script/build_gcc_with_memory_sanitizer.sh
 script/build_mpicc.sh
 script/build_msvc_2015.bat
 script/build_msvc_2015_with_gpu.bat
 script/build_msvc_2017.bat
 script/build_msvc_2017_with_gpu.bat
 script/build_msvc_2019.bat
 script/build_msvc_2019_with_gpu.bat
 script/clean.sh
 script/download_wheel.sh
 script/fix_wheel_osx.sh
+script/format.sh
 script/generate_msvc_project_2015.bat
 script/generate_msvc_project_2015_with_gpu.bat
 script/generate_msvc_project_2017.bat
 script/generate_msvc_project_2017_with_gpu.bat
 script/generate_msvc_project_2019.bat
 script/generate_msvc_project_2019_with_gpu.bat
 script/update_stubs.sh
```

### Comparing `qulacs-0.6.0/python/CMakeLists.txt` & `qulacs-0.6.1/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/python/cppsim_wrapper.cpp` & `qulacs-0.6.1/python/cppsim_wrapper.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,16 @@
             "Get is Herimitian")
         .def("get_qubit_count", &GeneralQuantumOperator::get_qubit_count,
             "Get qubit count")
         .def("get_state_dim", &GeneralQuantumOperator::get_state_dim,
             "Get state dimension")
         .def("get_term_count", &GeneralQuantumOperator::get_term_count,
             "Get count of Pauli terms")
+        .def("get_matrix", &GeneralQuantumOperator::get_matrix,
+            "Get the Hermitian matrix representation of the observable")
         .def("apply_to_state",
             py::overload_cast<QuantumStateBase*, const QuantumStateBase&,
                 QuantumStateBase*>(
                 &GeneralQuantumOperator::apply_to_state, py::const_),
             "Apply observable to `state_to_be_multiplied`. The result is "
             "stored into `dst_state`.",
             py::arg("work_state"), py::arg("state_to_be_multiplied"),
```

### Comparing `qulacs-0.6.0/python/stub-test/generate_mypy_tester.py` & `qulacs-0.6.1/python/stub-test/generate_mypy_tester.py`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/script/build_gcc.sh` & `qulacs-0.6.1/script/build_gcc.sh`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/script/download_wheel.sh` & `qulacs-0.6.1/script/download_wheel.sh`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/setup.py` & `qulacs-0.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,15 @@
         )
 
     def _generate_args(self, ext):
         # Following directories are created by cmake automatically.
         # Directory to output archive file.
         archive_dir = os.path.join(os.getcwd(), "lib")
         # Directory to output .so file generated by pybind.
-        extdir = os.path.abspath(os.path.dirname(
-            self.get_ext_fullpath(ext.name)))
+        extdir = os.path.abspath(os.path.dirname(self.get_ext_fullpath(ext.name)))
         # Directory to output test binaries.
         bindir = os.path.join(os.getcwd(), "bin")
         cmake_args = [
             "-DCMAKE_ARCHIVE_OUTPUT_DIRECTORY=" + archive_dir,
             "-DCMAKE_LIBRARY_OUTPUT_DIRECTORY=" + extdir,
             "-DCMAKE_RUNTIME_OUTPUT_DIRECTORY=" + bindir,
             "-DPYTHON_EXECUTABLE=" + sys.executable,
@@ -94,20 +93,18 @@
         ]
 
         cfg = "Debug" if self.debug else "Release"
         build_args = ["--config", cfg]
 
         if platform.system() == "Windows":
             cmake_args += [
-                "-DCMAKE_LIBRARY_OUTPUT_DIRECTORY_{}={}".format(
-                    cfg.upper(), extdir),
-                "-DCMAKE_RUNTIME_OUTPUT_DIRECTORY_{}={}".format(
-                    cfg.upper(), extdir),
+                "-DCMAKE_LIBRARY_OUTPUT_DIRECTORY_{}={}".format(cfg.upper(), extdir),
+                "-DCMAKE_RUNTIME_OUTPUT_DIRECTORY_{}={}".format(cfg.upper(), extdir),
             ]
-            if sys.maxsize > 2 ** 32:
+            if sys.maxsize > 2**32:
                 cmake_args += ["-A", "x64"]
             build_args += ["--", "/m"]
         else:
             # In macOS, gcc/g++ is aliased to clang/clang++.
             gcc = os.getenv("C_COMPILER", "gcc")
             gxx = os.getenv("CXX_COMPILER", "g++")
             if gcc is None or gxx is None:
@@ -121,18 +118,21 @@
             cmake_args += ["-DCMAKE_BUILD_TYPE=" + cfg]
 
             if gcc == "mpicc":
                 cmake_args += ["-DUSE_MPI:STR=Yes"]
 
             if platform.system() == "Darwin":
                 # This is for building Python package on GitHub Actions, whose architecture is x86_64.
-                # Without specifying the architecture explicitly, binaries for arm64 is built for x86_64 while cibuildwheel intends to build for arm64.
+                # Without specifying the architecture explicitly,
+                # binaries for arm64 is built for x86_64 while cibuildwheel intends to build for arm64.
                 archs = re.findall(r"-arch (\S+)", os.environ.get("ARCHFLAGS", ""))
                 if len(archs) > 0:
-                    cmake_args += ["-DCMAKE_OSX_ARCHITECTURES={}".format(";".join(archs))]
+                    cmake_args += [
+                        "-DCMAKE_OSX_ARCHITECTURES={}".format(";".join(archs))
+                    ]
 
             n_cpus = os.cpu_count()
             build_args += ["--", f"-j{n_cpus}"]
 
         return build_args, cmake_args
```

### Comparing `qulacs-0.6.0/src/cppsim/CMakeLists.txt` & `qulacs-0.6.1/src/cppsim/CMakeLists.txt`

 * *Files 21% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 
 add_library(cppsim_static STATIC ${CPPSIM_SRC})
 add_library(cppsim_shared SHARED ${CPPSIM_SRC})
 target_link_libraries(cppsim_static csim_static)
 target_link_libraries(cppsim_shared csim_static)
 add_dependencies(cppsim_static eigen)
 add_dependencies(cppsim_shared eigen)
-add_dependencies(cppsim_static Cereal)
-add_dependencies(cppsim_shared Cereal)
 
 if (USE_GPU)
     target_link_libraries(cppsim_static gpusim_static)
     target_link_libraries(cppsim_shared gpusim_static)
 endif()
 
 set_target_properties(cppsim_shared PROPERTIES EXCLUDE_FROM_ALL TRUE)
```

### Comparing `qulacs-0.6.0/src/cppsim/circuit.cpp` & `qulacs-0.6.1/src/cppsim/circuit.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/circuit.hpp` & `qulacs-0.6.1/src/cppsim/circuit.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/circuit_optimizer.cpp` & `qulacs-0.6.1/src/cppsim/circuit_optimizer.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/circuit_optimizer.hpp` & `qulacs-0.6.1/src/cppsim/circuit_optimizer.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/exception.hpp` & `qulacs-0.6.1/src/cppsim/exception.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate.cpp` & `qulacs-0.6.1/src/cppsim/gate.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate.hpp` & `qulacs-0.6.1/src/cppsim/gate.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_factory.cpp` & `qulacs-0.6.1/src/cppsim/gate_factory.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_factory.hpp` & `qulacs-0.6.1/src/cppsim/gate_factory.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_general.hpp` & `qulacs-0.6.1/src/cppsim/gate_general.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_matrix.cpp` & `qulacs-0.6.1/src/cppsim/gate_matrix.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_matrix.hpp` & `qulacs-0.6.1/src/cppsim/gate_matrix.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_matrix_diagonal.cpp` & `qulacs-0.6.1/src/cppsim/gate_matrix_diagonal.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_matrix_diagonal.hpp` & `qulacs-0.6.1/src/cppsim/gate_matrix_diagonal.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_matrix_sparse.cpp` & `qulacs-0.6.1/src/cppsim/gate_matrix_sparse.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_matrix_sparse.hpp` & `qulacs-0.6.1/src/cppsim/gate_matrix_sparse.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_merge.cpp` & `qulacs-0.6.1/src/cppsim/gate_merge.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_merge.hpp` & `qulacs-0.6.1/src/cppsim/gate_merge.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_named_npair.hpp` & `qulacs-0.6.1/src/cppsim/gate_named_npair.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_named_one.cpp` & `qulacs-0.6.1/src/cppsim/gate_named_one.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_named_one.hpp` & `qulacs-0.6.1/src/cppsim/gate_named_one.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_named_pauli.hpp` & `qulacs-0.6.1/src/cppsim/gate_named_pauli.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_named_two.hpp` & `qulacs-0.6.1/src/cppsim/gate_named_two.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_noisy_evolution.cpp` & `qulacs-0.6.1/src/cppsim/gate_noisy_evolution.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_noisy_evolution.hpp` & `qulacs-0.6.1/src/cppsim/gate_noisy_evolution.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_reflect.hpp` & `qulacs-0.6.1/src/cppsim/gate_reflect.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_reversible.hpp` & `qulacs-0.6.1/src/cppsim/gate_reversible.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/gate_to_gqo.hpp` & `qulacs-0.6.1/src/cppsim/gate_to_gqo.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/general_quantum_operator.cpp` & `qulacs-0.6.1/src/cppsim/general_quantum_operator.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #include <csim/stat_ops.hpp>
 #include <csim/update_ops.hpp>
 #include <csim/update_ops_dm.hpp>
 #include <csim/utility.hpp>
 #include <cstring>
 #include <fstream>
 #include <numeric>
+#include <unsupported/Eigen/KroneckerProduct>
 
 #include "exception.hpp"
 #include "gate_factory.hpp"
 #include "pauli_operator.hpp"
 #include "state.hpp"
 #include "type.hpp"
 #include "utility.hpp"
@@ -445,14 +446,76 @@
     auto quantum_operator = new GeneralQuantumOperator(_qubit_count);
     for (auto pauli : this->_operator_list) {
         quantum_operator->add_operator_copy(pauli);
     }
     return quantum_operator;
 }
 
+SparseComplexMatrixRowMajor _tensor_product(
+    const std::vector<SparseComplexMatrixRowMajor>& _obs) {
+    std::vector<SparseComplexMatrixRowMajor> obs(_obs);
+    int sz = obs.size();
+    while (sz != 1) {
+        if (sz % 2 == 0) {
+            for (int i = 0; i < sz; i += 2) {
+                obs[i >> 1] =
+                    Eigen::kroneckerProduct(obs[i], obs[i + 1]).eval();
+            }
+            sz >>= 1;
+        } else {
+            obs[sz - 2] =
+                Eigen::kroneckerProduct(obs[sz - 2], obs[sz - 1]).eval();
+            sz--;
+        }
+    }
+    return obs[0];
+}
+
+SparseComplexMatrixRowMajor GeneralQuantumOperator::get_matrix() const {
+    SparseComplexMatrixRowMajor sigma_x(2, 2), sigma_y(2, 2), sigma_z(2, 2),
+        sigma_i(2, 2);
+    sigma_x.insert(0, 1) = 1.0, sigma_x.insert(1, 0) = 1.0;
+    sigma_y.insert(0, 1) = -1.0i, sigma_y.insert(1, 0) = 1.0i;
+    sigma_z.insert(0, 0) = 1.0, sigma_z.insert(1, 1) = -1.0;
+    sigma_i.insert(0, 0) = 1.0, sigma_i.insert(1, 1) = 1.0;
+    std::vector<SparseComplexMatrixRowMajor> pauli_matrix_list = {
+        sigma_i, sigma_x, sigma_y, sigma_z};
+
+    int n_terms = this->get_term_count();
+    int n_qubits = this->get_qubit_count();
+    SparseComplexMatrixRowMajor hamiltonian_matrix(
+        1 << n_qubits, 1 << n_qubits);
+    hamiltonian_matrix.setZero();
+#ifdef _OPENMP
+#pragma omp declare reduction(+ : SparseComplexMatrixRowMajor : omp_out += \
+                                      omp_in) initializer(omp_priv = omp_orig)
+#pragma omp parallel for reduction(+ : hamiltonian_matrix)
+#endif
+    for (int i = 0; i < n_terms; i++) {
+        auto const pauli = this->get_term(i);
+        auto const pauli_id_list = pauli->get_pauli_id_list();
+        auto const pauli_target_list = pauli->get_index_list();
+
+        std::vector<SparseComplexMatrixRowMajor>
+            init_hamiltonian_pauli_matrix_list(
+                n_qubits, sigma_i);  // initialize matrix_list I
+        for (int j = 0; j < (int)pauli_target_list.size(); j++) {
+            init_hamiltonian_pauli_matrix_list[pauli_target_list[j]] =
+                pauli_matrix_list[pauli_id_list[j]];  // ex) [X,X,I,I]
+        }
+        std::reverse(init_hamiltonian_pauli_matrix_list.begin(),
+            init_hamiltonian_pauli_matrix_list.end());
+        hamiltonian_matrix +=
+            pauli->get_coef() *
+            _tensor_product(init_hamiltonian_pauli_matrix_list);
+    }
+    hamiltonian_matrix.prune(CPPCTYPE(0, 0));
+    return hamiltonian_matrix;
+}
+
 GeneralQuantumOperator* GeneralQuantumOperator::get_dagger() const {
     auto quantum_operator = new GeneralQuantumOperator(_qubit_count);
     for (auto pauli : this->_operator_list) {
         quantum_operator->add_operator(
             std::conj(pauli->get_coef()), pauli->get_pauli_string());
     }
     return quantum_operator;
```

### Comparing `qulacs-0.6.0/src/cppsim/general_quantum_operator.hpp` & `qulacs-0.6.1/src/cppsim/general_quantum_operator.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -267,14 +267,16 @@
      * @param [in] dst_state 結果を格納する状態
      */
     void apply_to_state_single_thread(
         QuantumStateBase* state, QuantumStateBase* dst_state) const;
 
     virtual GeneralQuantumOperator* copy() const;
 
+    SparseComplexMatrixRowMajor get_matrix() const;
+
     /**
      * \~japanese-en
      * ptreeに変換する
      *
      * @return ptree
      */
     virtual boost::property_tree::ptree to_ptree() const;
@@ -379,7 +381,10 @@
  */
 DllExport GeneralQuantumOperator* from_ptree(
     const boost::property_tree::ptree& pt);
 }  // namespace quantum_operator
 
 bool check_Pauli_operator(const GeneralQuantumOperator* quantum_operator,
     const PauliOperator* pauli_operator);
+
+SparseComplexMatrixRowMajor _tensor_product(
+    const std::vector<SparseComplexMatrixRowMajor>& _obs);
```

### Comparing `qulacs-0.6.0/src/cppsim/matrix_decomposition.hpp` & `qulacs-0.6.1/src/cppsim/matrix_decomposition.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/noisesimulator.cpp` & `qulacs-0.6.1/src/cppsim/noisesimulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/noisesimulator.hpp` & `qulacs-0.6.1/src/cppsim/noisesimulator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/observable.cpp` & `qulacs-0.6.1/src/cppsim/observable.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/observable.hpp` & `qulacs-0.6.1/src/cppsim/observable.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/pauli_operator.cpp` & `qulacs-0.6.1/src/cppsim/pauli_operator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/pauli_operator.hpp` & `qulacs-0.6.1/src/cppsim/pauli_operator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/qubit_info.cpp` & `qulacs-0.6.1/src/cppsim/qubit_info.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/qubit_info.hpp` & `qulacs-0.6.1/src/cppsim/qubit_info.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/simulator.cpp` & `qulacs-0.6.1/src/cppsim/simulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/simulator.hpp` & `qulacs-0.6.1/src/cppsim/simulator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/state.cpp` & `qulacs-0.6.1/src/cppsim/state.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/state.hpp` & `qulacs-0.6.1/src/cppsim/state.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/state_dm.cpp` & `qulacs-0.6.1/src/cppsim/state_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/state_dm.hpp` & `qulacs-0.6.1/src/cppsim/state_dm.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/state_gpu.cpp` & `qulacs-0.6.1/src/cppsim/state_gpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/state_gpu.hpp` & `qulacs-0.6.1/src/cppsim/state_gpu.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/type.hpp` & `qulacs-0.6.1/src/cppsim/type.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 using ComplexVector = Eigen::VectorXcd;
 
 // In order to use matrix raw-data without reordering, we use RowMajor as
 // default.
 using ComplexMatrix =
     Eigen::Matrix<CPPCTYPE, Eigen::Dynamic, Eigen::Dynamic, Eigen::RowMajor>;
 using SparseComplexMatrix = Eigen::SparseMatrix<CPPCTYPE>;
+using SparseComplexMatrixRowMajor =
+    Eigen::SparseMatrix<CPPCTYPE, Eigen::RowMajor>;
 
 #ifdef __GNUC__
 
 #if __GNUC__ >= 8
 using namespace std::complex_literals;
 #endif
 #endif
```

### Comparing `qulacs-0.6.0/src/cppsim/utility.cpp` & `qulacs-0.6.1/src/cppsim/utility.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/cppsim/utility.hpp` & `qulacs-0.6.1/src/cppsim/utility.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/CMakeLists.txt` & `qulacs-0.6.1/src/csim/CMakeLists.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 
 add_library(csim_static STATIC ${CSIM_SRC})
 add_library(csim_shared SHARED ${CSIM_SRC})
 #target_link_libraries(csim_static eigen)
 #target_link_libraries(csim_shared eigen)
 add_dependencies(csim_static eigen)
 add_dependencies(csim_shared eigen)
-add_dependencies(csim_static Cereal)
-add_dependencies(csim_shared Cereal)
 
 if (MSVC)
     set_target_properties(csim_static PROPERTIES LINKER_LANGUAGE CXX)
     set_target_properties(csim_shared PROPERTIES LINKER_LANGUAGE CXX)
 endif()
 
 set_target_properties(csim_shared PROPERTIES EXCLUDE_FROM_ALL TRUE)
```

### Comparing `qulacs-0.6.0/src/csim/MPIutil.cpp` & `qulacs-0.6.1/src/csim/MPIutil.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/MPIutil.hpp` & `qulacs-0.6.1/src/csim/MPIutil.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/constant.cpp` & `qulacs-0.6.1/src/csim/constant.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/constant.hpp` & `qulacs-0.6.1/src/csim/constant.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/init_ops.hpp` & `qulacs-0.6.1/src/csim/init_ops.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/init_ops_fill.cpp` & `qulacs-0.6.1/src/csim/init_ops_fill.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/init_ops_random.cpp` & `qulacs-0.6.1/src/csim/init_ops_random.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/memory_ops.cpp` & `qulacs-0.6.1/src/csim/memory_ops.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/memory_ops_dm.cpp` & `qulacs-0.6.1/src/csim/memory_ops_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/memory_ops_dm.hpp` & `qulacs-0.6.1/src/csim/memory_ops_dm.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/stat_ops.cpp` & `qulacs-0.6.1/src/csim/stat_ops.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/stat_ops.hpp` & `qulacs-0.6.1/src/csim/stat_ops.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/stat_ops_dm.cpp` & `qulacs-0.6.1/src/csim/stat_ops_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/stat_ops_dm.hpp` & `qulacs-0.6.1/src/csim/stat_ops_dm.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/stat_ops_expectation_value.cpp` & `qulacs-0.6.1/src/csim/stat_ops_expectation_value.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/stat_ops_probability.cpp` & `qulacs-0.6.1/src/csim/stat_ops_probability.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/stat_ops_transition_amplitude.cpp` & `qulacs-0.6.1/src/csim/stat_ops_transition_amplitude.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/type.hpp` & `qulacs-0.6.1/src/csim/type.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops.hpp` & `qulacs-0.6.1/src/csim/update_ops.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_control_multi_target_multi.cpp` & `qulacs-0.6.1/src/csim/update_ops_control_multi_target_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_control_multi_target_single.cpp` & `qulacs-0.6.1/src/csim/update_ops_control_multi_target_single.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_control_single_target_multi.cpp` & `qulacs-0.6.1/src/csim/update_ops_control_single_target_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_control_single_target_single.cpp` & `qulacs-0.6.1/src/csim/update_ops_control_single_target_single.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_cpp.hpp` & `qulacs-0.6.1/src/csim/update_ops_cpp.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_dm.cpp` & `qulacs-0.6.1/src/csim/update_ops_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_dm.hpp` & `qulacs-0.6.1/src/csim/update_ops_dm.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_matrix_dense_double.cpp` & `qulacs-0.6.1/src/csim/update_ops_matrix_dense_double.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_matrix_dense_double_eigen.cpp` & `qulacs-0.6.1/src/csim/update_ops_matrix_dense_double_eigen.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_matrix_dense_multi.cpp` & `qulacs-0.6.1/src/csim/update_ops_matrix_dense_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_matrix_dense_multi_eigen.cpp` & `qulacs-0.6.1/src/csim/update_ops_matrix_dense_multi_eigen.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_matrix_dense_single.cpp` & `qulacs-0.6.1/src/csim/update_ops_matrix_dense_single.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_matrix_diagonal_multi.cpp` & `qulacs-0.6.1/src/csim/update_ops_matrix_diagonal_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_matrix_diagonal_single.cpp` & `qulacs-0.6.1/src/csim/update_ops_matrix_diagonal_single.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_matrix_phase_single.cpp` & `qulacs-0.6.1/src/csim/update_ops_matrix_phase_single.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_named.cpp` & `qulacs-0.6.1/src/csim/update_ops_named.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_named_CNOT.cpp` & `qulacs-0.6.1/src/csim/update_ops_named_CNOT.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_named_CZ.cpp` & `qulacs-0.6.1/src/csim/update_ops_named_CZ.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_named_FusedSWAP.cpp` & `qulacs-0.6.1/src/csim/update_ops_named_FusedSWAP.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_named_H.cpp` & `qulacs-0.6.1/src/csim/update_ops_named_H.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_named_SWAP.cpp` & `qulacs-0.6.1/src/csim/update_ops_named_SWAP.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_named_X.cpp` & `qulacs-0.6.1/src/csim/update_ops_named_X.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_named_Y.cpp` & `qulacs-0.6.1/src/csim/update_ops_named_Y.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_named_Z.cpp` & `qulacs-0.6.1/src/csim/update_ops_named_Z.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_named_projection.cpp` & `qulacs-0.6.1/src/csim/update_ops_named_projection.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_named_state.cpp` & `qulacs-0.6.1/src/csim/update_ops_named_state.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_pauli_multi.cpp` & `qulacs-0.6.1/src/csim/update_ops_pauli_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_pauli_single.cpp` & `qulacs-0.6.1/src/csim/update_ops_pauli_single.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_qft.cpp` & `qulacs-0.6.1/src/csim/update_ops_qft.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_reflection.cpp` & `qulacs-0.6.1/src/csim/update_ops_reflection.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/update_ops_reversible_boolean.cpp` & `qulacs-0.6.1/src/csim/update_ops_reversible_boolean.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/utility.cpp` & `qulacs-0.6.1/src/csim/utility.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/csim/utility.hpp` & `qulacs-0.6.1/src/csim/utility.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/gpusim/CMakeLists.txt` & `qulacs-0.6.1/src/gpusim/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/gpusim/memory_ops.cu` & `qulacs-0.6.1/src/gpusim/memory_ops.cu`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,16 @@
 }
 
 __host__ void* allocate_quantum_state_host(
     ITYPE dim, unsigned int device_number) {
     int current_device = get_current_device();
     if (device_number != current_device) cudaSetDevice(device_number);
     GTYPE* state_gpu;
-    checkCudaErrors(cudaMalloc((void**)&state_gpu, dim * sizeof(GTYPE)));
+    checkCudaErrors(cudaMalloc((void**)&state_gpu, dim * sizeof(GTYPE)),
+        __FILE__, __LINE__);
     void* psi_gpu = reinterpret_cast<void*>(state_gpu);
     return psi_gpu;
 }
 
 __host__ void initialize_quantum_state_host(
     void* state, ITYPE dim, void* stream, unsigned int device_number) {
     int current_device = get_current_device();
@@ -73,16 +74,14 @@
 
     unsigned int block = dim <= 1024 ? dim : 1024;
     unsigned int grid = dim / block;
     init_qstate<<<grid, block, 0, *cuda_stream>>>(state_gpu, dim);
 
     checkCudaErrors(cudaStreamSynchronize(*cuda_stream), __FILE__, __LINE__);
     checkCudaErrors(cudaGetLastError(), __FILE__, __LINE__);
-    state = reinterpret_cast<void*>(state_gpu);
-    // stream = reinterpret_cast<void*>(cuda_stream);
 }
 
 __host__ void release_quantum_state_host(
     void* state, unsigned int device_number) {
     int current_device = get_current_device();
     if (device_number != current_device) cudaSetDevice(device_number);
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
```

### Comparing `qulacs-0.6.0/src/gpusim/memory_ops.h` & `qulacs-0.6.1/src/gpusim/memory_ops.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/gpusim/memory_ops_device_functions.h` & `qulacs-0.6.1/src/gpusim/memory_ops_device_functions.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/gpusim/stat_ops.cu` & `qulacs-0.6.1/src/gpusim/stat_ops.cu`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/gpusim/stat_ops.h` & `qulacs-0.6.1/src/gpusim/stat_ops.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/gpusim/stat_ops_device_functions.h` & `qulacs-0.6.1/src/gpusim/stat_ops_device_functions.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/gpusim/test.cpp` & `qulacs-0.6.1/src/gpusim/test.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/gpusim/update_ops_cuda.h` & `qulacs-0.6.1/src/gpusim/update_ops_cuda.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/gpusim/update_ops_cuda_device_functions.h` & `qulacs-0.6.1/src/gpusim/update_ops_cuda_device_functions.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/gpusim/update_ops_multi.cu` & `qulacs-0.6.1/src/gpusim/update_ops_multi.cu`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/gpusim/update_ops_named.cu` & `qulacs-0.6.1/src/gpusim/update_ops_named.cu`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/gpusim/update_ops_single.cu` & `qulacs-0.6.1/src/gpusim/update_ops_single.cu`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/gpusim/util.cu` & `qulacs-0.6.1/src/gpusim/util.cu`

 * *Files 1% similar despite different names*

```diff
@@ -165,17 +165,18 @@
 
 void print_quantum_state_host(
     void* state, ITYPE dim, unsigned int device_number) {
     int current_device = get_current_device();
     if (device_number != current_device) cudaSetDevice(device_number);
     GTYPE* state_gpu = reinterpret_cast<GTYPE*>(state);
     CPPCTYPE* state_cpu = (CPPCTYPE*)malloc(sizeof(CPPCTYPE) * dim);
-    checkCudaErrors(cudaDeviceSynchronize());
-    checkCudaErrors(cudaMemcpy(
-        state_cpu, state_gpu, dim * sizeof(CPPCTYPE), cudaMemcpyDeviceToHost));
+    checkCudaErrors(cudaDeviceSynchronize(), __FILE__, __LINE__);
+    checkCudaErrors(cudaMemcpy(state_cpu, state_gpu, dim * sizeof(CPPCTYPE),
+                        cudaMemcpyDeviceToHost),
+        __FILE__, __LINE__);
     for (int i = 0; i < dim; ++i) {
         std::cout << i << " : " << state_cpu[i].real() << "+i"
                   << state_cpu[i].imag() << '\n';
     }
     std::cout << '\n';
     free(state_cpu);
     state = reinterpret_cast<void*>(state);
```

### Comparing `qulacs-0.6.0/src/gpusim/util.cuh` & `qulacs-0.6.1/src/gpusim/util.cuh`

 * *Files 8% similar despite different names*

```diff
@@ -24,42 +24,35 @@
     if (error != cudaSuccess) {
         printf("Error: %s:%d, ", filename.c_str(), line);
         printf("code: %d, reason: %s\n", error, cudaGetErrorString(error));
         exit(1);
     }
 }
 
-inline void checkCudaErrors(const cudaError error) {
-    if (error != cudaSuccess) {
-        printf("Error: %s:%d, ", __FILE__, __LINE__);
-        printf("code: %d, reason: %s\n", error, cudaGetErrorString(error));
-        exit(1);
-    }
-}
 /*
 //inline void memcpy_quantum_state_HostToDevice(CPPCTYPE* state_cpu, GTYPE*
 state_gpu, ITYPE dim){ inline void memcpy_quantum_state_HostToDevice(CPPCTYPE*
 state_cpu, GTYPE* state_gpu, ITYPE dim, void* stream, UINT device_number){
         cudaStream_t* cuda_stream = reinterpret_cast<cudaStream_t*>(stream);
         int current_device = get_current_device();
         if (device_number != current_device) cudaSetDevice(device_number);
 
-        checkCudaErrors(cudaMalloc((void**)&state_gpu, dim * sizeof(CPPCTYPE)));
-        checkCudaErrors(cudaMemcpyAsync(state_gpu, state_cpu, dim *
+        checkCudaErrors(cudaMalloc((void**)&state_gpu, dim * sizeof(CPPCTYPE)),
+__FILE__, __LINE__); checkCudaErrors(cudaMemcpyAsync(state_gpu, state_cpu, dim *
 sizeof(CPPCTYPE), cudaMemcpyHostToDevice, *cuda_stream), __FILE__, __LINE__);
 }
 
 inline void memcpy_quantum_state_HostToDevice(CPPCTYPE* state_cpu, GTYPE*
 state_gpu, ITYPE dim, void* stream, unsigned int device_number){ cudaStream_t*
 cuda_stream = reinterpret_cast<cudaStream_t*>(stream); int current_device =
 get_current_device(); if (device_number != current_device)
 cudaSetDevice(device_number);
 
-        checkCudaErrors(cudaMalloc((void**)&state_gpu, dim * sizeof(CPPCTYPE)));
-        checkCudaErrors(cudaMemcpyAsync(state_gpu, state_cpu, dim *
+        checkCudaErrors(cudaMalloc((void**)&state_gpu, dim * sizeof(CPPCTYPE)),
+__FILE__, __LINE__); checkCudaErrors(cudaMemcpyAsync(state_gpu, state_cpu, dim *
 sizeof(CPPCTYPE), cudaMemcpyHostToDevice, *cuda_stream), __FILE__, __LINE__);
 }
 */
 inline void __cudaSafeCall(cudaError err, const char* file, const int line) {
 #ifdef CUDA_ERROR_CHECK
     if (cudaSuccess != err) {
         fprintf(stderr, "cudaSafeCall() failed at %s:%i : %s\n", file, line,
```

### Comparing `qulacs-0.6.0/src/gpusim/util.h` & `qulacs-0.6.1/src/gpusim/util.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/gpusim/util_common.h` & `qulacs-0.6.1/src/gpusim/util_common.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/gpusim/util_func.h` & `qulacs-0.6.1/src/gpusim/util_func.h`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/vqcsim/GradCalculator.cpp` & `qulacs-0.6.1/src/vqcsim/GradCalculator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/vqcsim/boolean_formula.hpp` & `qulacs-0.6.1/src/vqcsim/boolean_formula.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/vqcsim/causalcone_simulator.hpp` & `qulacs-0.6.1/src/vqcsim/causalcone_simulator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/vqcsim/differential.cpp` & `qulacs-0.6.1/src/vqcsim/differential.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/vqcsim/differential.hpp` & `qulacs-0.6.1/src/vqcsim/differential.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/vqcsim/loss_function.cpp` & `qulacs-0.6.1/src/vqcsim/loss_function.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/vqcsim/loss_function.hpp` & `qulacs-0.6.1/src/vqcsim/loss_function.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/vqcsim/optimizer.hpp` & `qulacs-0.6.1/src/vqcsim/optimizer.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/vqcsim/parametric_circuit.cpp` & `qulacs-0.6.1/src/vqcsim/parametric_circuit.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/vqcsim/parametric_circuit.hpp` & `qulacs-0.6.1/src/vqcsim/parametric_circuit.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/vqcsim/parametric_gate.hpp` & `qulacs-0.6.1/src/vqcsim/parametric_gate.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/vqcsim/parametric_gate_factory.cpp` & `qulacs-0.6.1/src/vqcsim/parametric_gate_factory.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/vqcsim/parametric_gate_factory.hpp` & `qulacs-0.6.1/src/vqcsim/parametric_gate_factory.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/vqcsim/parametric_simulator.cpp` & `qulacs-0.6.1/src/vqcsim/parametric_simulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/vqcsim/parametric_simulator.hpp` & `qulacs-0.6.1/src/vqcsim/parametric_simulator.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/vqcsim/problem.hpp` & `qulacs-0.6.1/src/vqcsim/problem.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/src/vqcsim/solver.hpp` & `qulacs-0.6.1/src/vqcsim/solver.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/cppsim/test_KAK.cpp` & `qulacs-0.6.1/test/cppsim/test_KAK.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/cppsim/test_circuit.cpp` & `qulacs-0.6.1/test/cppsim/test_circuit.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/cppsim/test_circuit_multicpu.cpp` & `qulacs-0.6.1/test/cppsim/test_circuit_multicpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/cppsim/test_circuit_optimize_light.cpp` & `qulacs-0.6.1/test/cppsim/test_circuit_optimize_light.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/cppsim/test_gate.cpp` & `qulacs-0.6.1/test/cppsim/test_gate.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/cppsim/test_gate_dm.cpp` & `qulacs-0.6.1/test/cppsim/test_gate_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/cppsim/test_gate_multicpu.cpp` & `qulacs-0.6.1/test/cppsim/test_gate_multicpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/cppsim/test_hamiltonian.cpp` & `qulacs-0.6.1/test/cppsim/test_hamiltonian.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -174,14 +174,73 @@
     ASSERT_NEAR(test_res.real(), res.real(), eps);
     ASSERT_NEAR(test_res.imag(), 0, eps);
     ASSERT_NEAR(res.imag(), 0, eps);
 
     delete observable;
 }
 
+TEST(ObservableTest, CheckGetMatrix) {
+    const std::string text =
+        "(-0.8126100000000005+0j) [] +\n"
+        "(0.04532175+0j) [X0 Z1 X2] +\n"
+        "(0.04532175+0j) [X0 Z1 X2 Z3] +\n"
+        "(0.04532175+0j) [Y0 Z1 Y2] +\n"
+        "(0.04532175+0j) [Y0 Z1 Y2 Z3] +\n"
+        "(0.17120100000000002+0j) [Z0] +\n"
+        "(0.17120100000000002+0j) [Z0 Z1] +\n"
+        "(0.165868+0j) [Z0 Z1 Z2] +\n"
+        "(0.165868+0j) [Z0 Z1 Z2 Z3] +\n"
+        "(0.12054625+0j) [Z0 Z2] +\n"
+        "(0.12054625+0j) [Z0 Z2 Z3] +\n"
+        "(0.16862325+0j) [Z1] +\n"
+        "(-0.22279649999999998+0j) [Z1 Z2 Z3] +\n"
+        "(0.17434925+0j) [Z1 Z3] +\n"
+        "(-0.22279649999999998+0j) [Z2]";
+
+    Observable* observable;
+    observable = observable::create_observable_from_openfermion_text(text);
+    ASSERT_NE(observable, (Observable*)NULL);
+    UINT qubit_count = observable->get_qubit_count();
+
+    SparseComplexMatrixRowMajor result = observable->get_matrix(),
+                                expected(16, 16);
+
+    expected.insert(0, 0) = CPPCTYPE(-4.163336342344337e-16, 0.0);
+    expected.insert(1, 1) = CPPCTYPE(-1.8304610000000006, 0.0);
+    expected.insert(1, 4) = CPPCTYPE(0.181287, 0.0);
+    expected.insert(2, 2) = CPPCTYPE(-1.2462260000000005, 0.0);
+    expected.insert(3, 3) = CPPCTYPE(-1.0649390000000005, 0.0);
+    expected.insert(3, 6) = CPPCTYPE(-0.181287, 0.0);
+    expected.insert(4, 1) = CPPCTYPE(0.181287, 0.0);
+    expected.insert(4, 4) = CPPCTYPE(-0.25447100000000045, 0.0);
+    expected.insert(5, 5) = CPPCTYPE(0.20638199999999932, 0.0);
+    expected.insert(6, 3) = CPPCTYPE(-0.181287, 0.0);
+    expected.insert(6, 6) = CPPCTYPE(-1.0649390000000005, 0.0);
+    expected.insert(7, 7) = CPPCTYPE(-1.2462260000000005, 0.0);
+    expected.insert(8, 8) = CPPCTYPE(-0.4759340000000004, 0.0);
+    expected.insert(9, 9) = CPPCTYPE(-1.1607380000000005, 0.0);
+    expected.insert(10, 10) = CPPCTYPE(-1.2524770000000005, 0.0);
+    expected.insert(11, 11) = CPPCTYPE(-1.2524770000000005, 0.0);
+    expected.insert(12, 12) = CPPCTYPE(-0.4759340000000005, 0.0);
+    expected.insert(13, 13) = CPPCTYPE(-1.1607380000000007, 0.0);
+    expected.insert(14, 14) = CPPCTYPE(-0.3612910000000006, 0.0);
+    expected.insert(15, 15) = CPPCTYPE(-0.3612910000000006, 0.0);
+
+    for (int i = 0; i < result.rows(); ++i) {
+        for (int j = 0; j < result.cols(); ++j) {
+            ASSERT_NEAR(result.coeffRef(i, j).real(),
+                expected.coeffRef(i, j).real(), eps);
+            ASSERT_NEAR(result.coeffRef(i, j).imag(),
+                expected.coeffRef(i, j).imag(), eps);
+        }
+    }
+
+    delete observable;
+}
+
 /*
 
 TEST(ObservableTest, CheckParsedObservableFromOpenFermionFile) {
     auto func = [](const std::string path,
         const QuantumStateBase* state) -> CPPCTYPE {
         std::ifstream ifs;
         ifs.open(path);
```

### Comparing `qulacs-0.6.0/test/cppsim/test_hamiltonian_dm.cpp` & `qulacs-0.6.1/test/cppsim/test_hamiltonian_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/cppsim/test_hamiltonian_multicpu.cpp` & `qulacs-0.6.1/test/cppsim/test_hamiltonian_multicpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/cppsim/test_mpiutil_multicpu.cpp` & `qulacs-0.6.1/test/cppsim/test_mpiutil_multicpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/cppsim/test_noise_dm.cpp` & `qulacs-0.6.1/test/cppsim/test_noise_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/cppsim/test_noisesimulator.cpp` & `qulacs-0.6.1/test/cppsim/test_noisesimulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/cppsim/test_noisyevolution.cpp` & `qulacs-0.6.1/test/cppsim/test_noisyevolution.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -305,16 +305,15 @@
     double time = 2.;
     double decay_rate_z = 0.2;
     double decay_rate_p = 0.6;
     double decay_rate_m = 0.1;
     double hamiltonian_energy = 1.;
     double ref = -0.3135191750739427;  // generated by qutip
     UINT n = 2;
-    UINT n_samples =
-        250;  // 以前は150だったが、テストに落ちることが多すぎたので増やした
+    UINT n_samples = 400;
 
     Observable observable(n);
     observable.add_operator(1, "X 0");
     // create hamiltonian and collapse operator
     Observable hamiltonian(n);
     hamiltonian.add_operator(hamiltonian_energy, "Z 0 Z 1");
     std::vector<GeneralQuantumOperator*> c_ops;
@@ -345,28 +344,27 @@
         h1->update_quantum_state(&state);
         delete h0;
         delete h1;
         circuit.update_quantum_state(&state);
         exp += observable.get_expectation_value(&state).real() / n_samples;
     }
     std::cout << "NoisyEvolution: " << exp << " ref: " << ref << std::endl;
-    ASSERT_NEAR(exp, ref,
-        .2);  // 以前は0.1だったが、テストに落ちることが多すぎたので増やした
+    ASSERT_NEAR(exp, ref, .1);
 }
 
 TEST(NoisyEvolutionTest_fast, tekitouu) {
     // 2 qubit dephasing dynamics with ZZ interaction
     double time = 0.8;
     double dt = 0.1;
     double decay_rate_z = 0.2;
     double decay_rate_p = 0.6;
     double decay_rate_m = 0.1;
     double hamiltonian_energy = 1.;
     UINT n = 2;
-    UINT n_samples = 200;
+    UINT n_samples = 1000;
 
     Observable observable(n);
     observable.add_operator(1, "X 0");
     // create hamiltonian and collapse operator
     Observable hamiltonian(n);
     hamiltonian.add_operator(hamiltonian_energy, "Z 0 Z 1");
     hamiltonian.add_operator(0.5, "X 0");
```

### Comparing `qulacs-0.6.0/test/cppsim/test_pauli_operator.cpp` & `qulacs-0.6.1/test/cppsim/test_pauli_operator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/cppsim/test_simulator.cpp` & `qulacs-0.6.1/test/cppsim/test_simulator.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/cppsim/test_state.cpp` & `qulacs-0.6.1/test/cppsim/test_state.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/cppsim/test_state_dm.cpp` & `qulacs-0.6.1/test/cppsim/test_state_dm.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/cppsim/test_state_multicpu.cpp` & `qulacs-0.6.1/test/cppsim/test_state_multicpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/csim/test_memory.cpp` & `qulacs-0.6.1/test/csim/test_memory.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/csim/test_omputil.cpp` & `qulacs-0.6.1/test/csim/test_omputil.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/csim/test_stat.cpp` & `qulacs-0.6.1/test/csim/test_stat.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/csim/test_update_control.cpp` & `qulacs-0.6.1/test/csim/test_update_control.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/csim/test_update_dense.cpp` & `qulacs-0.6.1/test/csim/test_update_dense.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/csim/test_update_dense_double.cpp` & `qulacs-0.6.1/test/csim/test_update_dense_double.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/csim/test_update_diagonal.cpp` & `qulacs-0.6.1/test/csim/test_update_diagonal.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/csim/test_update_diagonal_multi.cpp` & `qulacs-0.6.1/test/csim/test_update_diagonal_multi.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/csim/test_update_named.cpp` & `qulacs-0.6.1/test/csim/test_update_named.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/csim/test_update_pauli.cpp` & `qulacs-0.6.1/test/csim/test_update_pauli.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/gpusim/test_circuit.cpp` & `qulacs-0.6.1/test/gpusim/test_circuit.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/gpusim/test_compat_cpu.cpp` & `qulacs-0.6.1/test/gpusim/test_compat_cpu.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/gpusim/test_func_memory.cpp` & `qulacs-0.6.1/test/gpusim/test_func_memory.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/gpusim/test_gate.cpp` & `qulacs-0.6.1/test/gpusim/test_gate.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/gpusim/test_hamiltonian.cpp` & `qulacs-0.6.1/test/gpusim/test_hamiltonian.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/gpusim/test_state.cpp` & `qulacs-0.6.1/test/gpusim/test_state.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/gpusim/test_update_control.cpp` & `qulacs-0.6.1/test/gpusim/test_update_control.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/gpusim/test_update_dense.cpp` & `qulacs-0.6.1/test/gpusim/test_update_dense.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/gpusim/test_update_diagonal.cpp` & `qulacs-0.6.1/test/gpusim/test_update_diagonal.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/gpusim/test_update_named.cpp` & `qulacs-0.6.1/test/gpusim/test_update_named.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/gpusim/test_update_pauli.cpp` & `qulacs-0.6.1/test/gpusim/test_update_pauli.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/gpusim/test_util.hpp` & `qulacs-0.6.1/test/gpusim/test_util.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/util/util.hpp` & `qulacs-0.6.1/test/util/util.hpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/vqcsim/test.cpp` & `qulacs-0.6.1/test/vqcsim/test.cpp`

 * *Files identical despite different names*

### Comparing `qulacs-0.6.0/test/vqcsim/test_backprop.cpp` & `qulacs-0.6.1/test/vqcsim/test_backprop.cpp`

 * *Files identical despite different names*

