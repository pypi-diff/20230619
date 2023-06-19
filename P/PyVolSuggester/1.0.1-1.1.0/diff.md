# Comparing `tmp/pyvolsuggester-1.0.1.tar.gz` & `tmp/pyvolsuggester-1.1.0.tar.gz`

## Comparing `pyvolsuggester-1.0.1.tar` & `pyvolsuggester-1.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.1/License.txt
--rw-r--r--   0        0        0     9989 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.1/README.md
--rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    12351 2020-02-02 00:00:00.000000 pyvolsuggester-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pyvolsuggester-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyvolsuggester-1.1.0/License.txt
+-rw-r--r--   0        0        0     9989 2020-02-02 00:00:00.000000 pyvolsuggester-1.1.0/README.md
+-rw-r--r--   0        0        0     8537 2020-02-02 00:00:00.000000 pyvolsuggester-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    12414 2020-02-02 00:00:00.000000 pyvolsuggester-1.1.0/PKG-INFO
```

### Comparing `pyvolsuggester-1.0.1/License.txt` & `pyvolsuggester-1.1.0/License.txt`

 * *Files identical despite different names*

### Comparing `pyvolsuggester-1.0.1/README.md` & `pyvolsuggester-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyvolsuggester-1.0.1/pyproject.toml` & `pyvolsuggester-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 name = "PyVolSuggester"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.1"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
+version = "1.1.0"  # Required ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Does audio feature extraction and suggest the feasible volumne for better feeling and experience."  # Optional ## --------------------------------------------------------------------------------------------------------------------------------------
 
 # This is an optional longer description of your project that represents
@@ -73,15 +73,15 @@
 #
 # For a list of valid classifiers, see https://pypi.org/classifiers/
 classifiers = [  # Optional ## --------------------------------------------------------------------------------------------------------------------------------------
   # How mature is this project? Common values are
   #   3 - Alpha
   #   4 - Beta
   #   5 - Production/Stable
-  "Development Status :: 3 - Alpha",
+  "Development Status :: 4 - Beta",
 
   # Indicate who your project is intended for
   "Intended Audience :: Developers",
   "Topic :: Software Development :: Build Tools",
 
   # Pick your license as you wish
   "License :: OSI Approved :: MIT License",
@@ -130,21 +130,21 @@
 # issues, where the source is hosted, where to say thanks to the package
 # maintainers, and where to support the project financially. The key is
 # what's used to render the link text on PyPI.
 [project.urls]  # Optional ## --------------------------------------------------------------------------------------------------------------------------------------
 "Homepage" = "https://github.com/akash-rajak/PyVolSuggester"
 "Bug Reports" = "https://github.com/akash-rajak/PyVolSuggester/issues"
 "Funding" = "https://donate.pypi.org"
-#"Say Thanks!" = "http://saythanks.io/to/example"
+"Say Thanks!" = "https://saythanks.io/to/aakashrajak02"
 "Source" = "https://github.com/akash-rajak/PyVolSuggester"
 
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
-#[project.scripts]  # Optional
-#sample = "sample:main"
+[project.scripts]  # Optional
+sample = "sample:Suggester"
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 #[tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 #package-data = {"sample" = ["*.dat"]}
```

### Comparing `pyvolsuggester-1.0.1/PKG-INFO` & `pyvolsuggester-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: PyVolSuggester
-Version: 1.0.1
+Version: 1.1.0
 Summary: Does audio feature extraction and suggest the feasible volumne for better feeling and experience.
 Project-URL: Homepage, https://github.com/akash-rajak/PyVolSuggester
 Project-URL: Bug Reports, https://github.com/akash-rajak/PyVolSuggester/issues
 Project-URL: Funding, https://donate.pypi.org
+Project-URL: Say Thanks!, https://saythanks.io/to/aakashrajak02
 Project-URL: Source, https://github.com/akash-rajak/PyVolSuggester
 Author-email: Akash Rajak <aakashrajak02@gmail.com>
 Maintainer-email: Akash Rajak <aakashrajak02@gmail.com>
 License: MIT License
         
         Copyright (c) [2023] [Akash Rajak]
         
@@ -27,15 +28,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: License.txt
 Keywords: RMS/Energy-spectogram,amplitude-wave,audio,audio-feature-extraction,chroma-feature,mel-frequency-cepstral-coefficients,mel-frequency-spectogram,spectogram,tempogram,volumne-suggester,zero-crossing-rate
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

