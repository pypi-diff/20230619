# Comparing `tmp/microdata_tools-0.0.1.tar.gz` & `tmp/microdata_tools-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microdata_tools-0.0.1.tar", max compression
+gzip compressed data, was "microdata_tools-0.1.0.tar", max compression
```

## Comparing `microdata_tools-0.0.1.tar` & `microdata_tools-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-16 08:44:10.266109 microdata_tools-0.0.1/LICENSE.md
--rw-r--r--   0        0        0     1416 2023-06-16 08:44:10.266109 microdata_tools-0.0.1/README.md
--rw-r--r--   0        0        0       91 2023-06-16 08:44:10.266109 microdata_tools-0.0.1/microdata_tools/__init__.py
--rw-r--r--   0        0        0     4610 2023-06-16 08:44:10.266109 microdata_tools-0.0.1/microdata_tools/_encrypt.py
--rw-r--r--   0        0        0       47 2023-06-16 08:44:10.266109 microdata_tools-0.0.1/microdata_tools/exceptions.py
--rw-r--r--   0        0        0     1262 2023-06-16 08:44:10.266109 microdata_tools-0.0.1/microdata_tools/package_dataset.py
--rw-r--r--   0        0        0      534 2023-06-16 08:44:10.266109 microdata_tools-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1982 1970-01-01 00:00:00.000000 microdata_tools-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/LICENSE.md
+-rw-r--r--   0        0        0     2203 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/README.md
+-rw-r--r--   0        0        0      176 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/microdata_tools/__init__.py
+-rw-r--r--   0        0        0     4008 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/microdata_tools/_decrypt.py
+-rw-r--r--   0        0        0     4235 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/microdata_tools/_encrypt.py
+-rw-r--r--   0        0        0      212 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/microdata_tools/_utils.py
+-rw-r--r--   0        0        0      141 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/microdata_tools/exceptions.py
+-rw-r--r--   0        0        0     1331 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/microdata_tools/package_dataset.py
+-rw-r--r--   0        0        0     2341 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/microdata_tools/unpackage_dataset.py
+-rw-r--r--   0        0        0      534 2023-06-19 12:08:45.713412 microdata_tools-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2769 1970-01-01 00:00:00.000000 microdata_tools-0.1.0/PKG-INFO
```

### Comparing `microdata_tools-0.0.1/LICENSE.md` & `microdata_tools-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `microdata_tools-0.0.1/README.md` & `microdata_tools-0.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -14,23 +14,40 @@
     MY_DATASET_NAME/
         MY_DATASET_NAME.csv
         MY_DATASET_NAME.json
 ```
 The CSV file is optional in some cases.
 
 ### Package dataset
-The `package_dataset()` function will encrypt and package your datset as a tar archive. The process is as follows:
+The `package_dataset()` function will encrypt and package your dataset as a tar archive. The process is as follows:
 
 1. Generate the symmetric key for a dataset.
 2. Encrypt the dataset data (CSV) using the symmetric key and store the encrypted file as `<DATASET_NAME>.csv.encr`
-3. Encrypt the symmetric key using the asymmetric rsa public key and store the encrypted file as `<DATASET_NAME>.symkey.encr`
+3. Encrypt the symmetric key using the asymmetric RSA public key `microdata_public_key.pem` 
+   and store the encrypted file as `<DATASET_NAME>.symkey.encr`
 4. Gather the encrypted CSV, encrypted symmetric key and metadata (JSON) file in one tar file.
 
+### Unpackage dataset
+The `unpackage_dataset()` function will untar and decrypt your dataset using the `microdata_private_key.pem`
+RSA private key.
+
+The packaged file has to have the `<DATASET_NAME>.tar` extension. Its contents should be as follows:
+
+```<DATASET_NAME>.json``` : Required medata file.
+
+```<DATASET_NAME>.csv.encr``` : Optional encrypted dataset file.
+
+```<DATASET_NAME>.symkey.encr``` : Optional encrypted file containing the symmetrical key used to decrypt the dataset file. Required if the `.csv.encr` file is present.
+
+Decryption uses the RSA private key located at ```RSA_KEY_DIR```.
+
+The packaged file is then stored in `output_dir/archive/unpackaged` after a successful run or `output_dir/archive/failed` after an unsuccessful run.
+
 ## Example
-Python script that uses a public RSA key named `microdata_public_key.pem` and packages a dataset:
+Python script that uses a RSA public key named `microdata_public_key.pem` and packages a dataset:
 ```py
 from pathlib import Path
 from microdata_tools import package_dataset
 
 RSA_KEYS_DIRECTORY = Path("tests/resources/rsa_keys")
 DATASET_DIRECTORY = Path("tests/resources/input/DATASET_1")
 OUTPUT_DIRECTORY = Path("tests/resources/output")
```

### Comparing `microdata_tools-0.0.1/microdata_tools/_encrypt.py` & `microdata_tools-0.1.0/microdata_tools/_encrypt.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,42 +7,35 @@
 from cryptography.fernet import Fernet
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import padding
 
 from microdata_tools.exceptions import ValidationException
+from microdata_tools._utils import check_exists
 
 logger = logging.getLogger()
 
 
 def _encrypt_dataset(rsa_keys_dir: Path, dataset_dir: Path, output_dir: Path) -> None:
     """
     Encrypts a dataset as follows:
         1. Generates the symmetric key for this dataset.
         2. Encrypts the dataset using the symmetric key.
-        3. Encrypts the symmetric key using the public rsa key.
+        3. Encrypts the symmetric key using the RSA public key.
     """
 
-    if not rsa_keys_dir.exists():
-        raise ValidationException(f"The RSA keys directory {rsa_keys_dir} has to exist")
-
-    if not dataset_dir.exists():
-        raise ValidationException(
-            f"The directory containing the dataset files to encrypt {dataset_dir} "
-            "has to exist."
-        )
+    check_exists(rsa_keys_dir)
+    check_exists(dataset_dir)
 
     if not output_dir.exists():
         os.makedirs(output_dir)
 
     public_key_location = rsa_keys_dir / "microdata_public_key.pem"
-
-    if not public_key_location.is_file():
-        raise ValidationException(f"Public key {public_key_location} not found")
+    check_exists(public_key_location)
 
     # Read public key from file
     with open(public_key_location, "rb") as key_file:
         public_key = serialization.load_pem_public_key(
             key_file.read(), backend=default_backend()
         )
 
@@ -104,16 +97,15 @@
     """
     Creates a tar file from encrypted dataset files.
     Removes the input directory after successful completion.
     :param input_dir: the input directory containing the dataset directory
     :param dataset_name: the name of the dataset
     """
 
-    if not input_dir.exists():
-        raise ValidationException(f"Input directory {input_dir} does not exist")
+    check_exists(input_dir)
 
     if len(list((input_dir / dataset_name).iterdir())) == 0:
         raise ValidationException(f"No files found in {input_dir / dataset_name}")
 
     tar_file_name = f"{dataset_name}.tar"
     full_tar_file_name = input_dir / tar_file_name
     files_to_tar = [
```

### Comparing `microdata_tools-0.0.1/microdata_tools/package_dataset.py` & `microdata_tools-0.1.0/microdata_tools/package_dataset.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,21 +10,25 @@
 
 def package_dataset(
     rsa_keys_dir: Path,
     dataset_dir: Path,
     output_dir: Path,
 ) -> None:
     """
-    Encrypt a dataset and tar the resulting files.
-    Only the CSV file will be encrypted.
+    Packages a dataset. It will encrypt and tar the dataset using
+    the provided RSA public key. Only the CSV file will be encrypted.
 
-    :param rsa_keys_dir: directory containing public key file microdata_public_key.pem
-    :param dataset_dir: directory containing the dataset files (CSV and JSON)
-    :param output_dir: directory to encrypt to
-    :return: None
+    :param rsa_keys_dir:
+        directory containing public key file microdata_public_key.pem
+    :param dataset_dir:
+        directory containing the dataset files (CSV and JSON)
+    :param output_dir:
+        output directory
+    :return:
+        None
     """
 
     dataset_name = dataset_dir.stem
     dataset_output_dir = output_dir / dataset_name
     csv_files = [file for file in dataset_dir.iterdir() if file.suffix == ".csv"]
 
     if len(csv_files) == 1:
```

### Comparing `microdata_tools-0.0.1/pyproject.toml` & `microdata_tools-0.1.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "microdata-tools"
-version = "0.0.1"
+version = "0.1.0"
 description = "Tools for the microdata.no platform"
 authors = ["microdata-developers"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "microdata_tools"}]
 
 [tool.poetry.dependencies]
```

### Comparing `microdata_tools-0.0.1/PKG-INFO` & `microdata_tools-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microdata-tools
-Version: 0.0.1
+Version: 0.1.0
 Summary: Tools for the microdata.no platform
 License: MIT
 Author: microdata-developers
 Requires-Python: >=3.7.2,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -30,23 +30,40 @@
     MY_DATASET_NAME/
         MY_DATASET_NAME.csv
         MY_DATASET_NAME.json
 ```
 The CSV file is optional in some cases.
 
 ### Package dataset
-The `package_dataset()` function will encrypt and package your datset as a tar archive. The process is as follows:
+The `package_dataset()` function will encrypt and package your dataset as a tar archive. The process is as follows:
 
 1. Generate the symmetric key for a dataset.
 2. Encrypt the dataset data (CSV) using the symmetric key and store the encrypted file as `<DATASET_NAME>.csv.encr`
-3. Encrypt the symmetric key using the asymmetric rsa public key and store the encrypted file as `<DATASET_NAME>.symkey.encr`
+3. Encrypt the symmetric key using the asymmetric RSA public key `microdata_public_key.pem` 
+   and store the encrypted file as `<DATASET_NAME>.symkey.encr`
 4. Gather the encrypted CSV, encrypted symmetric key and metadata (JSON) file in one tar file.
 
+### Unpackage dataset
+The `unpackage_dataset()` function will untar and decrypt your dataset using the `microdata_private_key.pem`
+RSA private key.
+
+The packaged file has to have the `<DATASET_NAME>.tar` extension. Its contents should be as follows:
+
+```<DATASET_NAME>.json``` : Required medata file.
+
+```<DATASET_NAME>.csv.encr``` : Optional encrypted dataset file.
+
+```<DATASET_NAME>.symkey.encr``` : Optional encrypted file containing the symmetrical key used to decrypt the dataset file. Required if the `.csv.encr` file is present.
+
+Decryption uses the RSA private key located at ```RSA_KEY_DIR```.
+
+The packaged file is then stored in `output_dir/archive/unpackaged` after a successful run or `output_dir/archive/failed` after an unsuccessful run.
+
 ## Example
-Python script that uses a public RSA key named `microdata_public_key.pem` and packages a dataset:
+Python script that uses a RSA public key named `microdata_public_key.pem` and packages a dataset:
 ```py
 from pathlib import Path
 from microdata_tools import package_dataset
 
 RSA_KEYS_DIRECTORY = Path("tests/resources/rsa_keys")
 DATASET_DIRECTORY = Path("tests/resources/input/DATASET_1")
 OUTPUT_DIRECTORY = Path("tests/resources/output")
```

