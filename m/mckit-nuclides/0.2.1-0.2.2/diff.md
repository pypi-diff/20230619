# Comparing `tmp/mckit_nuclides-0.2.1.tar.gz` & `tmp/mckit_nuclides-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mckit_nuclides-0.2.1.tar", max compression
+gzip compressed data, was "mckit_nuclides-0.2.2.tar", max compression
```

## Comparing `mckit_nuclides-0.2.1.tar` & `mckit_nuclides-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2023-03-09 08:43:27.096242 mckit_nuclides-0.2.1/LICENSE
--rw-r--r--   0        0        0     3281 2023-03-09 08:43:27.096242 mckit_nuclides-0.2.1/README.rst
--rw-r--r--   0        0        0     8652 2023-03-09 08:43:46.496313 mckit_nuclides-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      716 2023-03-09 08:43:27.104242 mckit_nuclides-0.2.1/src/mckit_nuclides/__init__.py
--rw-r--r--   0        0        0     1575 2023-03-09 08:43:46.496313 mckit_nuclides-0.2.1/src/mckit_nuclides/abundance.py
--rw-r--r--   0        0        0    13595 2023-03-09 08:43:27.104242 mckit_nuclides-0.2.1/src/mckit_nuclides/data/elements.csv
--rw-r--r--   0        0        0   717942 2023-03-09 08:43:27.108242 mckit_nuclides-0.2.1/src/mckit_nuclides/data/nist_atomic_weights_and_element_compositions.txt
--rw-r--r--   0        0        0     3286 2023-03-09 08:43:46.496313 mckit_nuclides-0.2.1/src/mckit_nuclides/elements.py
--rw-r--r--   0        0        0     3118 2023-03-09 08:43:46.496313 mckit_nuclides-0.2.1/src/mckit_nuclides/nuclides.py
--rw-r--r--   0        0        0        0 2023-03-09 08:43:27.108242 mckit_nuclides-0.2.1/src/mckit_nuclides/py.typed
--rw-r--r--   0        0        0       20 2023-03-09 08:43:46.496313 mckit_nuclides-0.2.1/src/mckit_nuclides/utils/__init__.py
--rw-r--r--   0        0        0      657 2023-03-09 08:43:46.496313 mckit_nuclides-0.2.1/src/mckit_nuclides/utils/resource.py
--rw-r--r--   0        0        0     4552 1970-01-01 00:00:00.000000 mckit_nuclides-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-19 11:26:09.801151 mckit_nuclides-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3281 2023-06-19 11:26:09.801151 mckit_nuclides-0.2.2/README.rst
+-rw-r--r--   0        0        0    16503 2023-06-19 11:26:25.757158 mckit_nuclides-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      752 2023-06-19 11:26:25.757158 mckit_nuclides-0.2.2/src/mckit_nuclides/__init__.py
+-rw-r--r--   0        0        0     1647 2023-06-19 11:26:25.757158 mckit_nuclides-0.2.2/src/mckit_nuclides/abundance.py
+-rw-r--r--   0        0        0    13595 2023-06-19 11:26:09.813151 mckit_nuclides-0.2.2/src/mckit_nuclides/data/elements.csv
+-rw-r--r--   0        0        0   717942 2023-06-19 11:26:09.813151 mckit_nuclides-0.2.2/src/mckit_nuclides/data/nist_atomic_weights_and_element_compositions.txt
+-rw-r--r--   0        0        0     3255 2023-06-19 11:26:25.757158 mckit_nuclides-0.2.2/src/mckit_nuclides/elements.py
+-rw-r--r--   0        0        0     3113 2023-06-19 11:26:25.757158 mckit_nuclides-0.2.2/src/mckit_nuclides/nuclides.py
+-rw-r--r--   0        0        0        0 2023-06-19 11:26:09.813151 mckit_nuclides-0.2.2/src/mckit_nuclides/py.typed
+-rw-r--r--   0        0        0       20 2023-06-19 11:26:09.813151 mckit_nuclides-0.2.2/src/mckit_nuclides/utils/__init__.py
+-rw-r--r--   0        0        0      768 2023-06-19 11:26:25.757158 mckit_nuclides-0.2.2/src/mckit_nuclides/utils/resource.py
+-rw-r--r--   0        0        0     4504 1970-01-01 00:00:00.000000 mckit_nuclides-0.2.2/PKG-INFO
```

### Comparing `mckit_nuclides-0.2.1/LICENSE` & `mckit_nuclides-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mckit_nuclides-0.2.1/README.rst` & `mckit_nuclides-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `mckit_nuclides-0.2.1/src/mckit_nuclides/__init__.py` & `mckit_nuclides-0.2.2/src/mckit_nuclides/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """The `mckit_nuclides` package.
 
 Provides functionality to transfer meta information
 inserted to STP file component names as special tags
 to MCNP files generated from the STP with SuperMC.
 """
+from __future__ import annotations
+
 from importlib import metadata as _meta
 from importlib.metadata import PackageNotFoundError, version
 
 try:
     __version__ = version(__name__)
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
```

### Comparing `mckit_nuclides-0.2.1/src/mckit_nuclides/abundance.py` & `mckit_nuclides-0.2.2/src/mckit_nuclides/abundance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """Methods to change nuclide abundance in compositions."""
-from typing import Generator, Iterable, Tuple
+from __future__ import annotations
 
-import pandas as pd
+from typing import TYPE_CHECKING, Generator, Iterable
 
 from mckit_nuclides.nuclides import NUCLIDES_TABLE
 
+if TYPE_CHECKING:
+    import pandas as pd
+
 
 def convert_to_atomic_fraction(
-    composition: pd.DataFrame, fraction_column: str = "fraction"
+    composition: pd.DataFrame,
+    fraction_column: str = "fraction",
 ) -> pd.DataFrame:
     """Change fractions by mass to fractions by atoms.
 
     Args:
         composition: DataFrame indexed by MultipleIndex (atomic_number, mass_number)
         fraction_column: name of column presenting fraction
 
@@ -21,16 +25,16 @@
     composition[fraction_column] /= (
         NUCLIDES_TABLE.loc[composition.index, ["nuclide_mass"]].to_numpy().flatten()
     )
     return composition
 
 
 def expand_natural_presence(
-    zaf: Iterable[Tuple[int, int, float]]
-) -> Generator[Tuple[int, int, float], None, None]:
+    zaf: Iterable[tuple[int, int, float]],
+) -> Generator[tuple[int, int, float], None, None]:
     """Convert sequence of nuclide-fraction specification with natural presence.
 
     Substitute a sequence of nuclides when mass number is specified as 0.
     This means natural presence.
 
     Args:
         zaf: sequence of atomic number, mass number and fraction
@@ -39,10 +43,10 @@
         atomic number, mass_number, and corrected atomic fraction
     """  # DAR401
     for z, a, f in zaf:
         if a != 0:
             yield z, a, f
         else:
             isotopic_compositions: pd.Series = NUCLIDES_TABLE.loc[z].isotopic_composition
-            isotopic_compositions = isotopic_compositions[0 < isotopic_compositions]
+            isotopic_compositions = isotopic_compositions[isotopic_compositions > 0]
             for _a, _ic in isotopic_compositions.items():
                 yield z, _a, f * _ic
```

### Comparing `mckit_nuclides-0.2.1/src/mckit_nuclides/data/elements.csv` & `mckit_nuclides-0.2.2/src/mckit_nuclides/data/elements.csv`

 * *Files identical despite different names*

### Comparing `mckit_nuclides-0.2.1/src/mckit_nuclides/data/nist_atomic_weights_and_element_compositions.txt` & `mckit_nuclides-0.2.2/src/mckit_nuclides/data/nist_atomic_weights_and_element_compositions.txt`

 * *Files identical despite different names*

### Comparing `mckit_nuclides-0.2.1/src/mckit_nuclides/elements.py` & `mckit_nuclides-0.2.2/src/mckit_nuclides/elements.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Module `elements` provides access to information on chemical element level."""
 from __future__ import annotations
 
-from typing import Optional, Union, cast
+from typing import Union, cast
 
 import pandas as pd
 
 from mckit_nuclides.utils.resource import path_resolver
 
 TableValue = Union[int, str, float, None]
 
 
-def _opt_float(x: Optional[str]) -> Optional[float]:
+def _opt_float(x: str | None) -> float | None:
     return float(x) if x else None
 
 
 def _load_elements() -> pd.DataFrame:
     converters = {
         "atomic_number": int,
         "symbol": str,
@@ -49,15 +49,15 @@
 
     Args:
         element: element by chemical symbol
 
     Returns:
         int: Z - the atomic number for the element.
     """
-    return cast(int, ELEMENTS_TABLE.at[element, "atomic_number"])
+    return cast(int, ELEMENTS_TABLE.loc[element, "atomic_number"])
 
 
 z = atomic_number
 """Synonym to atomic_number."""
 
 
 def symbol(_atomic_number: int) -> str:
@@ -79,20 +79,19 @@
         z_or_symbol: define either by atomic number or symbol
         column: column name in ELEMENTS_TABLE
 
     Returns:
         The column value for the given element.
     """
     if isinstance(z_or_symbol, int):
-        column_value: TableValue = ELEMENTS_TABLE.iat[
-            z_or_symbol - 1, ELEMENTS_TABLE.columns.get_loc(column)
-        ]
-    else:
-        column_value = ELEMENTS_TABLE.loc[z_or_symbol, [column]].item()
-    return column_value
+        return cast(
+            TableValue,
+            ELEMENTS_TABLE.iloc[z_or_symbol - 1, ELEMENTS_TABLE.columns.get_loc(column)],
+        )
+    return cast(TableValue, ELEMENTS_TABLE.loc[z_or_symbol, [column]].item())
 
 
 def atomic_mass(z_or_symbol: int | str) -> float:
     """Get standard atomic mass for and Element by atomic number.
 
     Args:
         z_or_symbol: define either by atomic number or symbol
```

### Comparing `mckit_nuclides-0.2.1/src/mckit_nuclides/nuclides.py` & `mckit_nuclides-0.2.2/src/mckit_nuclides/nuclides.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Information on nuclides: masses, natural presence and more."""
 from __future__ import annotations
 
-from typing import Any, Dict, Final, List, Tuple, cast
+from typing import Any, Final, cast
 
 import pandas as pd
 
 from mckit_nuclides.elements import TableValue, z
 from mckit_nuclides.utils.resource import path_resolver
 
 _TYPES: Final = {
     "atomic_number": int,
     "mass_number": int,
     "relative_atomic_mass": float,
     "isotopic_composition": float,
 }
 
 
-def _split_line(_line: str) -> Tuple[str, Any]:
+def _split_line(_line: str) -> tuple[str, Any]:
     _label, _value = map(str.strip, _line.split("="))  # type: str, str
     _label = _label.lower().replace(" ", "_")
     value_type = _TYPES.get(_label, None)
     if value_type is not None:
         if _value:
             # drop uncertainties, so far, there's no use cases for them
             _value = _value.split("(", 1)[0]
@@ -32,38 +32,39 @@
 
 def _load_tables() -> pd.DataFrame:
     collector = _load_nist_file()
     symbols = ["H" if x in ["D", "T"] else x for x in collector["atomic_symbol"]]
     collector["atomic_symbol"] = symbols
     nuclides_table = pd.DataFrame.from_dict(collector)
     nuclides_table = nuclides_table.set_index(
-        ["atomic_number", "mass_number"], verify_integrity=True
+        ["atomic_number", "mass_number"],
+        verify_integrity=True,
     )
     nuclides_table.index.name = "atom_and_mass_numbers"
     nuclides_table = nuclides_table.rename(
         columns={"atomic_symbol": "symbol", "relative_atomic_mass": "nuclide_mass"},
     )
 
     return nuclides_table
 
 
-def _load_nist_file() -> Dict[str, List[Any]]:
-    collector: Dict[str, List[Any]] = {
+def _load_nist_file() -> dict[str, list[Any]]:
+    collector: dict[str, list[Any]] = {
         "atomic_number": [],
         "atomic_symbol": [],
         "mass_number": [],
         "relative_atomic_mass": [],
         "isotopic_composition": [],
     }
     path = path_resolver("mckit_nuclides")("data/nist_atomic_weights_and_element_compositions.txt")
     with path.open(encoding="utf-8") as fid:
         for line in fid.readlines():
-            line = line.strip()
-            if line and not line.startswith("#"):
-                label, value = _split_line(line)
+            _line = line.strip()
+            if _line and not _line.startswith("#"):
+                label, value = _split_line(_line)
                 dst = collector.get(label, None)
                 if dst is not None:
                     dst.append(value)
     return collector
 
 
 NUCLIDES_TABLE = _load_tables()
@@ -78,15 +79,15 @@
         column: name of column to extract value from
 
     Returns:
         Value of a column for a given nuclide.
     """
     if isinstance(z_or_symbol, str):
         z_or_symbol = z(z_or_symbol)
-    return cast(TableValue, NUCLIDES_TABLE.at[(z_or_symbol, mass_number), column])
+    return cast(TableValue, NUCLIDES_TABLE.loc[(z_or_symbol, mass_number), column])
 
 
 def get_nuclide_mass(z_or_symbol: int | str, mass_number: int) -> float:
     """Retrieve mass of a nuclide by atomic and mass numbers, a.u.
 
     Args:
         z_or_symbol: Z or symbol of a nuclide
```

### Comparing `mckit_nuclides-0.2.1/PKG-INFO` & `mckit_nuclides-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: mckit-nuclides
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python tools to work with elements and isotopes
 Home-page: https://github.com/MC-kit/mckit-nuclides
 License: MIT
 Keywords: element,nuclide,isotope,abundance
 Author: dvp
 Author-email: dmitri_portnov@yahoo.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: importlib-resources (>=5.12.0) ; python_version == "3.8"
 Requires-Dist: numpy (>=1.24.2)
 Requires-Dist: openpyxl (>=3.0.9)
-Requires-Dist: pandas (>=1.4.1)
+Requires-Dist: pandas (>=2.0.0)
 Project-URL: Changelog, https://github.com/MC-kit/mckit-nuclides/releases
 Project-URL: Repository, https://github.com/MC-kit/mckit-nuclides
 Description-Content-Type: text/x-rst
 
 ==============================================================================
 *mckit-nuclides*: tables with information on elements and nuclides
 ==============================================================================
```

