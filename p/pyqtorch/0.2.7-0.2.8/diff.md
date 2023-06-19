# Comparing `tmp/pyqtorch-0.2.7.tar.gz` & `tmp/pyqtorch-0.2.8.tar.gz`

## Comparing `pyqtorch-0.2.7.tar` & `pyqtorch-0.2.8.tar`

### file list

```diff
@@ -1,82 +1,63 @@
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/CONTRIBUTING.md
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/README.md
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/mkdocs.yml
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/readthedocs.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/setup.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.github/workflows/run-tests-and-mypy.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/21836652c37a637f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/2602555962d0fc4c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/30645ad5f1f1dcfe
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/317d2f17a1075099
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/41d845d0f90a6417
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/617ac8c861e982f1
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/68cc7f39a1692629
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/71de32d0dc4ef210
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/7ab8961a5fd3e34a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/7b50e93d7b401d37
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/7e9bc91eb0e4bec7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/8446b77184378e13
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/8c22cf14dc3075f3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/8f831c3208d022cd
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/963472f7f566f99d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/9b70b475da072d2b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/a3b4cbbb65fe8420
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/aaa2c54c6449792b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/af9c8e117f709f43
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/c73abac16d830acc
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/ce5cb2c96a07a572
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/ce5dade58b1ccd69
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/d49ef2d71d47c091
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/df86f5c8bc05afc4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/e69f22aa2552f985
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/f6f6f60064e20f97
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.ruff_cache/content/f78c2e380fc669b7
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/CODE_OF_CONDUCT.md -> ../CODE_OF_CONDUCT.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
--rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/QAOA.ipynb
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/essentials.ipynb
--rw-r--r--   0        0        0   154246 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/fit_function.ipynb
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/index.md
--rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/deprecated/QAOA.ipynb
--rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/deprecated/bench.py
--rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/deprecated/fit_function.ipynb
--rw-r--r--   0        0        0    74062 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/deprecated/getting_started.ipynb
--rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/deprecated/ham_evol_comparison.ipynb
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/docs/deprecated/state_evolution.ipynb
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/ansatz.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/embedding.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/matrices.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/matrices_sparse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/converters/__init__.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/converters/store_ops.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/converters/to_qiskit.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/core/__init__.py
--rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/core/batched_operation.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/core/circuit.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/core/measurement.py
--rw-r--r--   0        0        0    22213 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/core/operation.py
--rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/core/utils.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/modules/__init__.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/modules/circuit.py
--rw-r--r--   0        0        0     7686 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/modules/hamevo.py
--rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/modules/parametric.py
--rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/modules/primitive.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyqtorch/modules/utils.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/tests/conftest.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/tests/test_batched_operations.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/tests/test_converters.py
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/tests/test_module_hamevo.py
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/tests/test_modules.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/tests/test_notebooks.py
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/tests/test_operations.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/tests/test_operations_hamevo.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/LICENSE
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 pyqtorch-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/README.md
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/mkdocs.yml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/publish.sh
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/readthedocs.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/setup.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/.github/workflows/run-tests-and-mypy.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/CODE_OF_CONDUCT.md -> ../CODE_OF_CONDUCT.md
+
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
+
+-rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/QAOA.ipynb
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/circuit.md
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/essentials.ipynb
+-rw-r--r--   0        0        0   154246 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/fit_function.ipynb
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/gate_composition.ipynb
+-rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/hamevo.md
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/index.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/matrices.md
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/parametric.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/primitive.md
+-rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/deprecated/QAOA.ipynb
+-rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/deprecated/bench.py
+-rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/deprecated/fit_function.ipynb
+-rw-r--r--   0        0        0    74062 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/deprecated/getting_started.ipynb
+-rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/deprecated/ham_evol_comparison.ipynb
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/deprecated/state_evolution.ipynb
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/ansatz.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/embedding.py
+-rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/matrices.py
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/matrices_sparse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/converters/__init__.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/converters/store_ops.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/converters/to_qiskit.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/core/__init__.py
+-rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/core/batched_operation.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/core/circuit.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/core/measurement.py
+-rw-r--r--   0        0        0    22213 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/core/operation.py
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/core/utils.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/modules/__init__.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/modules/abstract.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/modules/circuit.py
+-rw-r--r--   0        0        0    11650 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/modules/hamevo.py
+-rw-r--r--   0        0        0    14144 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/modules/parametric.py
+-rw-r--r--   0        0        0    11426 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/modules/primitive.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/modules/utils.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/tests/conftest.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/tests/test_batched_operations.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/tests/test_converters.py
+-rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/tests/test_module_hamevo.py
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/tests/test_modules.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/tests/test_notebooks.py
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/tests/test_operations.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/tests/test_operations_hamevo.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/LICENSE
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/PKG-INFO
```

### Comparing `pyqtorch-0.2.7/.pre-commit-config.yaml` & `pyqtorch-0.2.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/CODE_OF_CONDUCT.md` & `pyqtorch-0.2.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/CONTRIBUTING.md` & `pyqtorch-0.2.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/mkdocs.yml` & `pyqtorch-0.2.8/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,20 @@
       - How to Contribute: CONTRIBUTING.md
       - Code of Conduct: CODE_OF_CONDUCT.md
   - Overview:
       - Essentials : essentials.ipynb
   - Tutorials:
       - Fitting a function: fit_function.ipynb
       - QAOA : QAOA.ipynb
+  - Documentation:
+    - Modules:
+        - Circuit : circuit.md
+        - Matrices : matrices.md
+        - Parametric : parametric.md
+        - Primitive : primitive.md
 
 
 theme:
   name: material
   features:
   - content.code.annotate
   - navigation.indexes
```

### Comparing `pyqtorch-0.2.7/.github/workflows/run-tests-and-mypy.yml` & `pyqtorch-0.2.8/.github/workflows/run-tests-and-mypy.yml`

 * *Files 1% similar despite different names*

```diff
@@ -38,8 +38,8 @@
 
         - name: Lint
           run: |
             python -m hatch -e tests run pre-commit run --all-files
 
         - name: Perform unit tests
           run: |
-            python -m hatch -e tests run pytest
+            python -m hatch -e tests run pytest -n auto
```

### Comparing `pyqtorch-0.2.7/docs/QAOA.ipynb` & `pyqtorch-0.2.8/docs/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/docs/essentials.ipynb` & `pyqtorch-0.2.8/docs/essentials.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/docs/fit_function.ipynb` & `pyqtorch-0.2.8/docs/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/docs/deprecated/QAOA.ipynb` & `pyqtorch-0.2.8/docs/deprecated/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/docs/deprecated/bench.py` & `pyqtorch-0.2.8/docs/deprecated/bench.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/docs/deprecated/fit_function.ipynb` & `pyqtorch-0.2.8/docs/deprecated/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/docs/deprecated/getting_started.ipynb` & `pyqtorch-0.2.8/docs/deprecated/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/docs/deprecated/ham_evol_comparison.ipynb` & `pyqtorch-0.2.8/docs/deprecated/ham_evol_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/docs/deprecated/state_evolution.ipynb` & `pyqtorch-0.2.8/docs/deprecated/state_evolution.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/pyqtorch/__init__.py` & `pyqtorch-0.2.8/pyqtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/pyqtorch/ansatz.py` & `pyqtorch-0.2.8/pyqtorch/ansatz.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/pyqtorch/embedding.py` & `pyqtorch-0.2.8/pyqtorch/embedding.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/pyqtorch/matrices_sparse.py` & `pyqtorch-0.2.8/pyqtorch/matrices_sparse.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/pyqtorch/converters/store_ops.py` & `pyqtorch-0.2.8/pyqtorch/converters/store_ops.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/pyqtorch/converters/to_qiskit.py` & `pyqtorch-0.2.8/pyqtorch/converters/to_qiskit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/pyqtorch/core/__init__.py` & `pyqtorch-0.2.8/pyqtorch/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/pyqtorch/core/batched_operation.py` & `pyqtorch-0.2.8/pyqtorch/core/batched_operation.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/pyqtorch/core/circuit.py` & `pyqtorch-0.2.8/pyqtorch/core/circuit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/pyqtorch/core/measurement.py` & `pyqtorch-0.2.8/pyqtorch/core/measurement.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/pyqtorch/core/operation.py` & `pyqtorch-0.2.8/pyqtorch/core/operation.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/pyqtorch/core/utils.py` & `pyqtorch-0.2.8/pyqtorch/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,23 +16,25 @@
 from string import ascii_letters as ABC
 from typing import Any
 
 import numpy as np
 import torch
 from numpy.typing import NDArray
 
+torch.set_default_dtype(torch.float64)
+
 ABC_ARRAY: NDArray = np.array(list(ABC))
 
 
 IMAT = torch.eye(2, dtype=torch.cdouble)
 XMAT = torch.tensor([[0, 1], [1, 0]], dtype=torch.cdouble)
 YMAT = torch.tensor([[0, -1j], [1j, 0]], dtype=torch.cdouble)
 ZMAT = torch.tensor([[1, 0], [0, -1]], dtype=torch.cdouble)
 SMAT = torch.tensor([[1, 0], [0, 1j]], dtype=torch.cdouble)
-TMAT = torch.tensor([[1, 0], [0, torch.exp(torch.tensor(1j) * torch.pi / 4)]], dtype=torch.cdouble)
+TMAT = torch.tensor([[1, 0], [0, torch.exp(torch.tensor(1.0j * torch.pi / 4))]])
 SWAPMAT = torch.tensor(
     [[1, 0, 0, 0], [0, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, 1]], dtype=torch.cdouble
 )
 HMAT = 1 / torch.sqrt(torch.tensor(2)) * torch.tensor([[1, 1], [1, -1]], dtype=torch.cdouble)
 
 
 OPERATIONS_DICT = {
@@ -43,15 +45,20 @@
     "S": SMAT,
     "T": TMAT,
     "H": HMAT,
     "SWAP": SWAPMAT,
 }
 
 
-def _apply_gate(state: torch.Tensor, mat: torch.Tensor, qubits: Any, N_qubits: int) -> torch.Tensor:
+def _apply_gate(
+    state: torch.Tensor,
+    mat: torch.Tensor,
+    qubits: Any,
+    N_qubits: int,
+) -> torch.Tensor:
     """
     Apply a gate represented by its matrix `mat` to the quantum state
     `state`
 
     Inputs:
     - state (torch.Tensor): input state of shape [2] * N_qubits + [batch_size]
     - mat (torch.Tensor): the matrix representing the gate
```

### Comparing `pyqtorch-0.2.7/tests/conftest.py` & `pyqtorch-0.2.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/tests/test_batched_operations.py` & `pyqtorch-0.2.8/tests/test_batched_operations.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/tests/test_converters.py` & `pyqtorch-0.2.8/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/tests/test_module_hamevo.py` & `pyqtorch-0.2.8/tests/test_module_hamevo.py`

 * *Files 18% similar despite different names*

```diff
@@ -150,7 +150,36 @@
     psi_ham = hamiltonian_evolution(H_batch, t_evo, psi_0)
 
     # assert torch.allclose(psi_rk4, psi_eig)
     # assert torch.allclose(psi_rk4, psi_eig)
     # assert torch.allclose(psi_eig, psi_exp)
     tensors = [psi_rk4, psi_eig, psi_exp, psi_ham]
     assert all(torch.allclose(tensors[i], tensors[0]) for i in range(1, len(tensors)))
+
+
+@pytest.mark.parametrize(
+    "ham_evo_type, ham_evo_class",
+    [
+        (pyq.HamEvoType.RK4, pyq.HamEvo),
+        (pyq.HamEvoType.EIG, pyq.HamEvoEig),
+        (pyq.HamEvoType.EXP, pyq.HamEvoExp),
+        ("rk4", pyq.HamEvo),
+        ("eig", pyq.HamEvoEig),
+        ("exp", pyq.HamEvoExp),
+    ],
+)
+def test_hamiltonianevolution_with_types(
+    ham_evo_type: pyq.HamEvoType, ham_evo_class: torch.nn.Module
+) -> None:
+    n_qubits = 4
+    H = Hamiltonian(1)
+    t_evo = torch.tensor([torch.pi / 4], dtype=torch.cdouble)
+
+    hamevo = pyq.HamiltonianEvolution(range(n_qubits), n_qubits, hamevo_type=ham_evo_type)
+    ham_evo_instance = hamevo.get_hamevo_instance(H, t_evo)
+    assert isinstance(ham_evo_instance, ham_evo_class)
+
+    psi = pyq.uniform_state(n_qubits)
+    psi_star = hamevo(H, t_evo, psi)
+    result = overlap(psi_star, psi)
+    result = result if isinstance(result, float) else result[0]
+    assert isclose(result, 0.5)
```

### Comparing `pyqtorch-0.2.7/tests/test_notebooks.py` & `pyqtorch-0.2.8/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/tests/test_operations.py` & `pyqtorch-0.2.8/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/tests/test_operations_hamevo.py` & `pyqtorch-0.2.8/tests/test_operations_hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/LICENSE` & `pyqtorch-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.7/pyproject.toml` & `pyqtorch-0.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     { name = "Aleksander Wennersteen", email = "aleksander.wennersteen@pasqal.com" },
     { name = "Mario Dagrada", email = "mario.dagrada@pasqal.com" },
     { name = "Dominik Seitz", email = "dominik.seitz@pasqal.com" },
     { name = "Niklas Heim", email = "niklas.heim@pasqal.com" },
 ]
 requires-python = ">=3.8.1,<3.11"
 license = {text = "Proprietary"}
-version = "0.2.7"
+version = "0.2.8"
 classifiers=[
     "License :: Other/Proprietary License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `pyqtorch-0.2.7/PKG-INFO` & `pyqtorch-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqtorch
-Version: 0.2.7
+Version: 0.2.8
 Summary: An efficient, large-scale emulator designed for quantum machine learning, seamlessly integrated with a PyTorch backend. Please refer to https://pyqtorch.readthedocs.io/en/latest/ for setup and usage info, along with the full documentation.
 Author-email: Slimane Thabet <slimane.thabet@pasqal.com>, Aleksander Wennersteen <aleksander.wennersteen@pasqal.com>, Mario Dagrada <mario.dagrada@pasqal.com>, Dominik Seitz <dominik.seitz@pasqal.com>, Niklas Heim <niklas.heim@pasqal.com>
 License: Proprietary
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

