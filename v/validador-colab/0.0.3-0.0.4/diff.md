# Comparing `tmp/validador_colab-0.0.3.tar.gz` & `tmp/validador_colab-0.0.4.tar.gz`

## Comparing `validador_colab-0.0.3.tar` & `validador_colab-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 validador_colab-0.0.3/main.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 validador_colab-0.0.3/requirements.txt
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/core/__init__.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/core/entities/__init__.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/core/entities/colab_counter.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/core/entities/natural_one.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/core/entities/sakura.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/core/entities/smarket_counter.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/core/entities/validation_detail.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/core/errors/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/core/errors/divergent_data.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/core/errors/no_data_found.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/core/repositories/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/core/repositories/colab_counters.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/core/repositories/smarket_analytics.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/core/usecases/__init__.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/core/usecases/colab_service.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/core/usecases/smarket_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/infra/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/infra/configs/__init__.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/infra/configs/configs.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/infra/database/__init__.py
--rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/infra/database/postgres.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/infra/database/postgres_controle.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/infra/repositories/__init__.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/infra/repositories/colab_counters_repository.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/infra/repositories/smarket_analytics_repository.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/infra/routes/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/infra/routes/daily_conf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/infra/utils/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/loop/__init__.py
--rw-r--r--   0        0        0    13853 2020-02-02 00:00:00.000000 validador_colab-0.0.3/validador_colab/loop/first_block.py
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 validador_colab-0.0.3/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.3/README.md
--rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 validador_colab-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 validador_colab-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 validador_colab-0.0.4/main.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 validador_colab-0.0.4/requirements.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/entities/__init__.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/entities/colab_counter.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/entities/natural_one.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/entities/sakura.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/entities/smarket_counter.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/entities/validation_detail.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/errors/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/errors/divergent_data.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/errors/no_data_found.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/repositories/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/repositories/colab_counters.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/repositories/smarket_analytics.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/usecases/__init__.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/usecases/colab_service.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/core/usecases/smarket_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/configs/__init__.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/configs/configs.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/database/__init__.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/database/postgres.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/database/postgres_controle.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/repositories/__init__.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/repositories/colab_counters_repository.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/repositories/smarket_analytics_repository.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/routes/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/routes/daily_conf.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/infra/utils/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/loop/__init__.py
+-rw-r--r--   0        0        0    13853 2020-02-02 00:00:00.000000 validador_colab-0.0.4/validador_colab/loop/first_block.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 validador_colab-0.0.4/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.4/README.md
+-rw-r--r--   0        0        0     4180 2020-02-02 00:00:00.000000 validador_colab-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 validador_colab-0.0.4/PKG-INFO
```

### Comparing `validador_colab-0.0.3/main.py` & `validador_colab-0.0.4/main.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.3/requirements.txt` & `validador_colab-0.0.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.3/validador_colab/core/entities/natural_one.py` & `validador_colab-0.0.4/validador_colab/core/entities/natural_one.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.3/validador_colab/core/entities/sakura.py` & `validador_colab-0.0.4/validador_colab/core/entities/sakura.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.3/validador_colab/core/usecases/colab_service.py` & `validador_colab-0.0.4/validador_colab/core/usecases/colab_service.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.3/validador_colab/core/usecases/smarket_service.py` & `validador_colab-0.0.4/validador_colab/core/usecases/smarket_service.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.3/validador_colab/infra/configs/configs.py` & `validador_colab-0.0.4/validador_colab/infra/configs/configs.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.3/validador_colab/infra/database/postgres.py` & `validador_colab-0.0.4/validador_colab/infra/database/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         pool_smarket = pool.QueuePool(
             self.getconn_smarket, max_overflow=0, pool_size=2)
         self.conn_colab = pool_colab.connect()
         self.conn_smarket = pool_smarket.connect()
         self.cursor_colab = self.conn_colab.cursor()
         self.cursor_smarket = self.conn_smarket.cursor()
 
-    def get(self, mode: str, sql: str) -> list[tuple]:
+    def get(self, mode: str, sql: str):
 
         values = [()]
 
         if mode.upper() == 'COLAB':
             self.cursor_colab.execute(sql)
             try:
                 values = self.cursor_colab.fetchall()
```

### Comparing `validador_colab-0.0.3/validador_colab/infra/database/postgres_controle.py` & `validador_colab-0.0.4/validador_colab/infra/database/postgres_controle.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.3/validador_colab/infra/repositories/colab_counters_repository.py` & `validador_colab-0.0.4/validador_colab/infra/repositories/colab_counters_repository.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.3/validador_colab/infra/repositories/smarket_analytics_repository.py` & `validador_colab-0.0.4/validador_colab/infra/repositories/smarket_analytics_repository.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.3/validador_colab/infra/routes/daily_conf.py` & `validador_colab-0.0.4/validador_colab/infra/routes/daily_conf.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.3/validador_colab/loop/first_block.py` & `validador_colab-0.0.4/validador_colab/loop/first_block.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.3/.gitignore` & `validador_colab-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.3/pyproject.toml` & `validador_colab-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "validador-colab"
 description = 'Validador colab é uma ferramenta para validar os dados diarios incrementáis nas tabelas de fato do colab e no Analytics'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
-version = "0.0.3"
+version = "0.0.4"
 keywords = []
 authors = [
   { name = "Davi Amaral de Araujo", email = "davi@smarketsolutions.com.br" },
 ]
 
 classifiers = [
   "Development Status :: 4 - Beta",
```

### Comparing `validador_colab-0.0.3/PKG-INFO` & `validador_colab-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validador-colab
-Version: 0.0.3
+Version: 0.0.4
 Summary: Validador colab é uma ferramenta para validar os dados diarios incrementáis nas tabelas de fato do colab e no Analytics
 Project-URL: Documentation, https://github.com/unknown/validador-colab#readme
 Project-URL: Issues, https://github.com/unknown/validador-colab/issues
 Project-URL: Source, https://github.com/unknown/validador-colab
 Author-email: Davi Amaral de Araujo <davi@smarketsolutions.com.br>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

