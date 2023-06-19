# Comparing `tmp/tsdf-0.2.0.tar.gz` & `tmp/tsdf-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsdf-0.2.0.tar", max compression
+gzip compressed data, was "tsdf-0.3.0.tar", max compression
```

## Comparing `tsdf-0.2.0.tar` & `tsdf-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0      619 2022-12-21 12:44:30.653600 tsdf-0.2.0/LICENSE
--rw-r--r--   0        0        0     1294 2023-03-08 10:05:00.337823 tsdf-0.2.0/README.md
--rw-r--r--   0        0        0     1231 2023-04-26 13:13:43.004410 tsdf-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      375 2023-04-26 11:56:37.830492 tsdf-0.2.0/src/tsdf/__init__.py
--rw-r--r--   0        0        0      996 2023-04-26 11:56:37.831018 tsdf-0.2.0/src/tsdf/constants.py
--rw-r--r--   0        0        0     5785 2023-04-26 11:56:37.831667 tsdf-0.2.0/src/tsdf/io.py
--rw-r--r--   0        0        0     6459 2023-04-26 11:56:37.832124 tsdf-0.2.0/src/tsdf/io_metadata.py
--rw-r--r--   0        0        0     1834 2023-04-26 11:56:37.832479 tsdf-0.2.0/src/tsdf/numpy_utils.py
--rw-r--r--   0        0        0     2369 2023-04-26 11:56:37.833034 tsdf-0.2.0/src/tsdf/tsdf_metadata.py
--rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 tsdf-0.2.0/setup.py
--rw-r--r--   0        0        0     2469 1970-01-01 00:00:00.000000 tsdf-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0      619 2022-12-21 12:44:30.653600 tsdf-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1421 2023-05-24 09:40:28.932574 tsdf-0.3.0/README.md
+-rw-r--r--   0        0        0     1231 2023-05-24 09:42:37.396194 tsdf-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      375 2023-04-26 11:56:37.830492 tsdf-0.3.0/src/tsdf/__init__.py
+-rw-r--r--   0        0        0      996 2023-06-19 09:02:10.958613 tsdf-0.3.0/src/tsdf/constants.py
+-rw-r--r--   0        0        0     8201 2023-05-24 09:40:28.935308 tsdf-0.3.0/src/tsdf/io.py
+-rw-r--r--   0        0        0     6459 2023-04-26 11:56:37.832124 tsdf-0.3.0/src/tsdf/io_metadata.py
+-rw-r--r--   0        0        0     1834 2023-04-26 11:56:37.832479 tsdf-0.3.0/src/tsdf/numpy_utils.py
+-rw-r--r--   0        0        0     2370 2023-05-24 09:40:28.935752 tsdf-0.3.0/src/tsdf/tsdf_metadata.py
+-rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 tsdf-0.3.0/setup.py
+-rw-r--r--   0        0        0     2575 1970-01-01 00:00:00.000000 tsdf-0.3.0/PKG-INFO
```

### Comparing `tsdf-0.2.0/LICENSE` & `tsdf-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tsdf-0.2.0/README.md` & `tsdf-0.3.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 
 ![Python package](https://github.com/biomarkersparkinson/tsdf/workflows/Python%20package/badge.svg)
+[![PyPI](https://img.shields.io/pypi/v/tsdf.svg)](https://pypi.python.org/pypi/tsdf/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7867900.svg)](https://doi.org/10.5281/zenodo.7867900)
 
 # tsdf
 
 A package to load [TSDF data](https://arxiv.org/abs/2211.11294) into Python
 
 ## Installation
 
-Download or clone the content of [our repository](https://github.com/biomarkersParkinson/tsdf) and install using `poetry` or `pip`.
-
-### Using `poetry` (recommended)
-
-```bash
-poetry install
-```
-
 ### Using `pip`
 
+The package is available in PyPi. It can be installed using:
+
 ```bash
 $ pip install tsdf
 ```
 
 ## Usage
 
-- TODO
+See our [extended tutorials](https://biomarkersparkinson.github.io/tsdf/).
 
 ## Development
 
 ### Running tests
 
 ```bash
 poetry install
```

### Comparing `tsdf-0.2.0/pyproject.toml` & `tsdf-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "tsdf"
-version = "0.2.0"
+version = "0.3.0"
 description = "A Python library that provides methods for encoding and decoding TSDF (Time Series Data Format) data, which allows you to easily create, manipulate and serialize TSDF files in your Python code."
-authors = ["Pablo Rodríguez <p.rodriguez-sanchez@esciencecenter.nl>",
-            "Peter Kok <p.kok@esciencecenter.nl>",
+authors = ["Peter Kok <p.kok@esciencecenter.nl>",
+            "Pablo Rodríguez <p.rodriguez-sanchez@esciencecenter.nl>",
             "Vedran Kasalica <v.kaslica@esciencecenter.nl>"]
 license = "Apache-2.0"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
```

### Comparing `tsdf-0.2.0/src/tsdf/constants.py` & `tsdf-0.3.0/src/tsdf/constants.py`

 * *Files identical despite different names*

### Comparing `tsdf-0.2.0/src/tsdf/io.py` & `tsdf-0.3.0/src/tsdf/io_metadata.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,182 +1,183 @@
 import json
 import os
-import sys
 from typing import Any, Dict, List
-import numpy as np
-from tsdf import io_metadata
-from tsdf.numpy_utils import (
-    data_type_numpy_to_tsdf,
-    data_type_tsdf_to_numpy,
-    bits_numpy_to_tsdf,
-    bytes_tsdf_to_numpy,
-    endianness_numpy_to_tsdf,
-    endianness_tsdf_to_numpy,
-    rows_numpy_to_tsdf,
-)
-from tsdf.tsdf_metadata import TSDFMetadata
 
+from tsdf import constants
+from tsdf.tsdf_metadata import (
+    TSDFMetadataFieldError,
+    TSDFMetadata,
+    TSDFMetadataFieldValueError,
+)
 
-def load_metadata_file(file) -> Dict[str, TSDFMetadata]:
-    """Loads a TSDF metadata file, returns a dictionary
 
-    Reference: https://arxiv.org/abs/2211.11294
+def read_data(data: Any, source_path: str) -> Dict[str, TSDFMetadata]:
     """
-
-    # The data is isomorphic to a JSON
-    data = json.load(file)
-
-    abs_path = os.path.realpath(file.name)
-
-    # Parse the data and verify that it complies with TSDF requirements
-    return io_metadata.read_data(data, abs_path)
-
-
-def load_metadata_from_path(path: str) -> Dict[str, TSDFMetadata]:
-    """Loads a TSDF metadata file, returns a dictionary
-
-    Reference: https://arxiv.org/abs/2211.11294
+    Function used to parse the JSON object containing TSDF metadata. It returns a
+    list of TSDFMetadata objects, where each object describes formatting of a binary file.
     """
-    # The data is isomorphic to a JSON
-    with open(path, "r") as file:
-        data = json.load(file)
-
-    abs_path = os.path.realpath(path)
-    # Parse the data and verify that it complies with TSDF requirements
-    return io_metadata.read_data(data, abs_path)
 
+    # Check if the version is supported
+    version = data["metadata_version"]
+    if not version in constants.SUPPORTED_TSDF_VERSIONS:
+        raise TSDFMetadataFieldValueError(f"TSDF file version {version} not supported.")
+
+    defined_properties: Dict[str, Any] = {}
+    return _read_struct(data, defined_properties.copy(), source_path, version)
 
-def load_metadata_string(json_str) -> Dict[str, TSDFMetadata]:
-    """Loads a TSDF metadata string, returns a dictionary
 
-    Reference: https://arxiv.org/abs/2211.11294
+def _read_struct(
+    data: Any, defined_properties: Dict[str, Any], source_path, version: str
+) -> Dict[str, TSDFMetadata]:
     """
+    Recursive method used to parse the TSDF metadata in a hierarchical
+    order (from the root towards the leaves).
+    """
+    all_streams: Dict[str, TSDFMetadata] = {}
+    remaining_data = {}
+    leaf: bool = True
+
+    # 1) Map all the values provided at the current level of the TSDF structure.
+    for key, value in data.items():
+        if is_mandatory_type(key, version):
+            defined_properties[key] = value
+        elif not _contains_file_name(value):
+            defined_properties[key] = value
+        else:
+            leaf = False
+            remaining_data[key] = value
+
+    # 2) If the current element is a leaf in the structure, convert it into a TSDFMetadata object.
+    if leaf:
+        try:
+            bin_file_name = defined_properties["file_name"]
+            path = os.path.split(source_path)
+            file_dir = os.path.join(path[0])
+            meta_file_name = path[1]
+            all_streams[bin_file_name] = TSDFMetadata(
+                defined_properties, file_dir, meta_file_name
+            )
+        except TSDFMetadataFieldError as exc:
+            raise TSDFMetadataFieldError(
+                "A property 'file_name' is missing in the TSDF metadata file."
+            ) from exc
+
+    # 3) If the current element is not a leaf, `remaining_data`` will contain lower
+    # levels of the TSDF structure.
+    # Extend the mapping recursively with values provided at those levels.
+    for key, value in remaining_data.items():
+        if _is_a_list(value):
+            for each_value in value:
+                all_streams = all_streams | _read_struct(
+                    each_value, defined_properties.copy(), source_path, version
+                )
+        else:
+            all_streams = all_streams | _read_struct(
+                value, defined_properties.copy(), source_path, version
+            )
 
-    # The data is isomorphic to a JSON
-    data = json.loads(json_str)
-
-    # Parse the data and verify that it complies with TSDF requirements
-    return io_metadata.read_data(data, "")
-
-
-def load_binary_from_metadata(metadata_dir: str, metadata: TSDFMetadata) -> np.ndarray:
-    """Use metadata properties to load and return numpy array from a binary file"""
-    bin_path = os.path.join(metadata_dir, metadata.file_name)
-    return load_binary_file(
-        bin_path,
-        metadata.data_type,
-        metadata.bits,
-        metadata.endianness,
-        metadata.rows,
-        len(metadata.channels),
-    )
+    return all_streams
 
 
-def load_binary_file(
-    bin_file_path: str,
-    data_type: str,
-    n_bits: int,
-    endianness: str,
-    n_rows: int,
-    n_columns: int,
-) -> np.ndarray:
-    """Use provided parameters to load and return a numpy array from a binary file"""
+def is_mandatory_type(key: str, version: str) -> bool:
+    """
+    Function returns True if the field that corresponds to the
+    key is mandatory for the given TSDF version, otherwise it returns False.
+    """
+    return True if key in constants.MANDATORY_TSDF_KEYS[version] else False
 
-    s_endianness = endianness_tsdf_to_numpy(endianness)
-    s_type = data_type_tsdf_to_numpy(data_type)
-    s_n_bytes = bytes_tsdf_to_numpy(n_bits)
-    format_string = "".join([s_endianness, s_type, s_n_bytes])
 
-    # Load the data and reshape
-    with open(bin_file_path, "rb") as fid:
-        values = np.fromfile(fid, dtype=format_string)
-        if n_columns > 1:
-            values = values.reshape((-1, n_columns))
+def _contains_file_name(data: Any) -> bool:
+    """
+    Function return True if the data contains the "file_name" key,
+    and thus, represents nested data elements.
+    Otherwise it returns False.
+    """
 
-    # Check whether the number of rows matches the metadata
-    if values.shape[0] != n_rows:
-        raise Exception("Number of rows doesn't match file length.")
+    if isinstance(data, list):
+        for elem in data:
+            if _contains_file_name(elem):
+                return True
 
-    return values
+    if not isinstance(data, dict):
+        return False
 
+    for key, value in data.items():
+        if key == "file_name":
+            return True
+        if _contains_file_name(value):
+            return True
+    return False
 
-def get_metadata_from_ndarray(data: np.ndarray) -> Dict[str, Any]:
-    """Retrieve metadata information encoded in the NumPy array."""
 
-    metadata = {
-        "data_type": data_type_numpy_to_tsdf(data),
-        "bits": bits_numpy_to_tsdf(data),
-        "endianness": endianness_numpy_to_tsdf(data),
-        "rows": rows_numpy_to_tsdf(data),
-    }
-    return metadata
+def _is_a_list(value) -> bool:
+    """Function returns True if the value is a list, otherwise it returns False."""
+    return isinstance(value, list)
 
 
-def write_binary_file(
-    file_dir: str, file_name: str, data: np.ndarray, metadata: dict
-) -> TSDFMetadata:
-    """Save binary file based on the provided NumPy array."""
-    path = os.path.join(file_dir, file_name)
-    data.tofile(path)
-    metadata.update(get_metadata_from_ndarray(data))
-    metadata.update({"file_name": file_name})
-
-    return TSDFMetadata(metadata, file_dir)
+def check_tsdf_mandatory_fields(dictionary: Dict[str, Any]) -> None:
+    """
+    Verifies that all the mandatory properties for TSDF metadata are provided,
+    and are in the right format.
+    """
+    version_key = "metadata_version"
+    if not version_key in dictionary.keys():
+        raise TSDFMetadataFieldError(f"TSDF structure is missing key '{version_key}'")
+
+    version = dictionary[version_key]
+    for key in constants.MANDATORY_TSDF_KEYS[version]:
+        if not key in dictionary.keys():
+            raise TSDFMetadataFieldError(f"TSDF structure is missing key '{key}'")
+    units = "units"
+    channels = "channels"
+    if len(dictionary[units]) != len(dictionary[channels]):
+        raise TSDFMetadataFieldValueError(
+            f"TSDF structure requires equal number of {units} and {channels}"
+        )
 
+    for key, value in dictionary.items():
+        _check_tsdf_property_format(key, value, version)
 
-def write_metadata(metadatas: List[TSDFMetadata], file_name: str) -> None:
-    """Combine and save the TSDF metadata objects as a json file."""
-    if len(metadatas) == 0:
-        raise Exception(
-            "Metadata cannot be saved, as the list of TSDFMetadata objects is empty."
-        )
 
-    if len(metadatas) == 1:
-        meta = metadatas[0]
-        write_to_file(meta.get_plain_tsdf_dict_copy(), meta.file_dir_path, file_name)
+def _check_tsdf_property_format(key: str, value, version: str) -> None:
+    """
+    Function checks whether the value of the mandatory TSDF field specified by the key
+    is of the expected data format.\\
+    `Note: If the key is not mandatory the function does not perform any checks.`
+    """
+    if not is_mandatory_type(key, version):
         return
 
-    # Ensure that the metadata files can be combined
-    io_metadata.confirm_dir_of_metadata(metadatas)
+    index = constants.MANDATORY_TSDF_KEYS[version].index(key)
+    type_name = constants.MANDATORY_TSDF_KEYS_VALUES[version][index]
 
-    plain_meta = [meta.get_plain_tsdf_dict_copy() for meta in metadatas]
-    overlap = extract_dict_overlap(plain_meta)
-    if not overlap:
-        raise Exception(
-            "Metadata files mist have at least one common field. Otherwise, they should be stored separtely."
+    if not isinstance(value, constants.KEY_VALUE_TYPES[type_name]):
+        raise TSDFMetadataFieldValueError(
+            f"The given value for {key} is not in the expected ({type_name}) format."
         )
 
-    overlap["sensors"] = optimise_dict_structure_rec(plain_meta)
-    write_to_file(overlap, metadatas[0].file_dir_path, file_name)
-
 
-def extract_dict_overlap(metadatas: List[Dict[str, Any]]) -> Dict[str, Any]:
-    """Extract the fields that are the same for all the metadata files.
-    A new dict is created and the fields are removed from the original dictionaries."""
-    meta_overlap: Dict[str, Any] = {}
-
-    init_metadata = metadatas[0]
-    for key, value in init_metadata.items():
-        key_in_all = True
-        for curr_meta in metadatas[1:]:
-            if key not in curr_meta.keys() or curr_meta[key] != value:
-                key_in_all = False
-        if key_in_all:
-            meta_overlap[key] = value
-    for key, _ in meta_overlap.items():
-        for meta_dict in metadatas:
-            meta_dict.pop(key)
-
-    return meta_overlap
-
-
-def optimise_dict_structure_rec(
-    metadatas: List[Dict[str, Any]]
-) -> List[Dict[str, Any]]:
-    """TODO: A recursive call that should optimise the structure of the TSDF metadata, by grouping the common values."""
-    return metadatas
-
-
-def write_to_file(dict: Dict[str, Any], dir_path: str, file_name: str) -> None:
-    path = os.path.join(dir_path, file_name)
-    with open(path, "w") as convert_file:
-        convert_file.write(json.dumps(dict))
+def get_file_metadata_at_index(
+    metadata: Dict[str, TSDFMetadata], index: int
+) -> TSDFMetadata:
+    """Returns the metadata object at the position defined by the index."""
+    for _key, value in metadata.items():
+        if index == 0:
+            return value
+        index -= 1
+    raise IndexError("The index is out of range.")
+
+
+def confirm_dir_of_metadata(metadatas: List[TSDFMetadata]) -> None:
+    """The method is used to confirm whether all the metadata files are expected in the same directory."""
+    metadata_iter = iter(metadatas)
+    init_metadata = next(metadata_iter)
+
+    for curr_metadata in metadata_iter:
+        if init_metadata.file_dir_path != curr_metadata.file_dir_path:
+            raise Exception(
+                "Metadata files have to be in the same folder to be combined."
+            )
+        if init_metadata.file_name == curr_metadata.file_name:
+            raise Exception(
+                "Two metadata objects cannot reference the same binary file (file_name)."
+            )
```

### Comparing `tsdf-0.2.0/src/tsdf/numpy_utils.py` & `tsdf-0.3.0/src/tsdf/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `tsdf-0.2.0/src/tsdf/tsdf_metadata.py` & `tsdf-0.3.0/src/tsdf/tsdf_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 
 class TSDFMetadataFieldValueError(Exception):
     "Raised when a TSDFMetadata field is wrongly annotated."
     pass
 
 
+
 class TSDFMetadata:
     """Structure that provides metadata needed for reading a data stream."""
 
     metadata_version: str
     study_id: str
     subject_id: str
     device_id: str
```

### Comparing `tsdf-0.2.0/setup.py` & `tsdf-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,19 +15,19 @@
  'mkdocs-jupyter>=0.22.0,<0.23.0',
  'mkdocs>=1.4.2,<2.0.0',
  'mypy>=1.0.1,<2.0.0',
  'numpy>=1.24.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'tsdf',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': 'A Python library that provides methods for encoding and decoding TSDF (Time Series Data Format) data, which allows you to easily create, manipulate and serialize TSDF files in your Python code.',
-    'long_description': '\n![Python package](https://github.com/biomarkersparkinson/tsdf/workflows/Python%20package/badge.svg)\n\n# tsdf\n\nA package to load [TSDF data](https://arxiv.org/abs/2211.11294) into Python\n\n## Installation\n\nDownload or clone the content of [our repository](https://github.com/biomarkersParkinson/tsdf) and install using `poetry` or `pip`.\n\n### Using `poetry` (recommended)\n\n```bash\npoetry install\n```\n\n### Using `pip`\n\n```bash\n$ pip install tsdf\n```\n\n## Usage\n\n- TODO\n\n## Development\n\n### Running tests\n\n```bash\npoetry install\npoetry run pytest\n```\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\nThis package was created by Pablo Rodríguez, Peter Kok and Vedran Kasalica. It is licensed under the terms of the Apache License 2.0 license.\n\n## Credits\n\n- The [TSDF data format](https://arxiv.org/abs/2211.11294) was created by Kasper Claes, Valentina Ticcinelli, Reham Badawy, Yordan P. Raykov, Luc J.W. Evers, Max A. Little.\n- This package was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
-    'author': 'Pablo Rodríguez',
-    'author_email': 'p.rodriguez-sanchez@esciencecenter.nl',
+    'long_description': '\n![Python package](https://github.com/biomarkersparkinson/tsdf/workflows/Python%20package/badge.svg)\n[![PyPI](https://img.shields.io/pypi/v/tsdf.svg)](https://pypi.python.org/pypi/tsdf/)\n[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7867900.svg)](https://doi.org/10.5281/zenodo.7867900)\n\n# tsdf\n\nA package to load [TSDF data](https://arxiv.org/abs/2211.11294) into Python\n\n## Installation\n\n### Using `pip`\n\nThe package is available in PyPi. It can be installed using:\n\n```bash\n$ pip install tsdf\n```\n\n## Usage\n\nSee our [extended tutorials](https://biomarkersparkinson.github.io/tsdf/).\n\n## Development\n\n### Running tests\n\n```bash\npoetry install\npoetry run pytest\n```\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\nThis package was created by Pablo Rodríguez, Peter Kok and Vedran Kasalica. It is licensed under the terms of the Apache License 2.0 license.\n\n## Credits\n\n- The [TSDF data format](https://arxiv.org/abs/2211.11294) was created by Kasper Claes, Valentina Ticcinelli, Reham Badawy, Yordan P. Raykov, Luc J.W. Evers, Max A. Little.\n- This package was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
+    'author': 'Peter Kok',
+    'author_email': 'p.kok@esciencecenter.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/biomarkersParkinson/tsdf',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
```

### Comparing `tsdf-0.2.0/PKG-INFO` & `tsdf-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tsdf
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python library that provides methods for encoding and decoding TSDF (Time Series Data Format) data, which allows you to easily create, manipulate and serialize TSDF files in your Python code.
 Home-page: https://github.com/biomarkersParkinson/tsdf
 License: Apache-2.0
 Keywords: Time Series Data Format (TSDF),binary data,digital sensors
-Author: Pablo Rodríguez
-Author-email: p.rodriguez-sanchez@esciencecenter.nl
+Author: Peter Kok
+Author-email: p.kok@esciencecenter.nl
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -21,38 +21,34 @@
 Requires-Dist: mypy (>=1.0.1,<2.0.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Project-URL: Repository, https://github.com/biomarkersParkinson/tsdf
 Description-Content-Type: text/markdown
 
 
 ![Python package](https://github.com/biomarkersparkinson/tsdf/workflows/Python%20package/badge.svg)
+[![PyPI](https://img.shields.io/pypi/v/tsdf.svg)](https://pypi.python.org/pypi/tsdf/)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7867900.svg)](https://doi.org/10.5281/zenodo.7867900)
 
 # tsdf
 
 A package to load [TSDF data](https://arxiv.org/abs/2211.11294) into Python
 
 ## Installation
 
-Download or clone the content of [our repository](https://github.com/biomarkersParkinson/tsdf) and install using `poetry` or `pip`.
-
-### Using `poetry` (recommended)
-
-```bash
-poetry install
-```
-
 ### Using `pip`
 
+The package is available in PyPi. It can be installed using:
+
 ```bash
 $ pip install tsdf
 ```
 
 ## Usage
 
-- TODO
+See our [extended tutorials](https://biomarkersparkinson.github.io/tsdf/).
 
 ## Development
 
 ### Running tests
 
 ```bash
 poetry install
```

