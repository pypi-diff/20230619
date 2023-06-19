# Comparing `tmp/xtuples-0.0.7.tar.gz` & `tmp/xtuples-0.0.8.tar.gz`

## Comparing `xtuples-0.0.7.tar` & `xtuples-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    26953 2020-02-02 00:00:00.000000 xtuples-0.0.7/README.ipynb
--rw-r--r--   0        0        0     7004 2020-02-02 00:00:00.000000 xtuples-0.0.7/docs/index.html
--rw-r--r--   0        0        0    22834 2020-02-02 00:00:00.000000 xtuples-0.0.7/docs/json.html
--rw-r--r--   0        0        0   106349 2020-02-02 00:00:00.000000 xtuples-0.0.7/docs/xtuples.html
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 xtuples-0.0.7/src/xtuples/__about__.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 xtuples-0.0.7/src/xtuples/__init__.py
--rw-r--r--   0        0        0     5845 2020-02-02 00:00:00.000000 xtuples-0.0.7/src/xtuples/json.py
--rw-r--r--   0        0        0    21657 2020-02-02 00:00:00.000000 xtuples-0.0.7/src/xtuples/xtuples.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 xtuples-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 xtuples-0.0.7/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 xtuples-0.0.7/LICENSE.txt
--rw-r--r--   0        0        0    15119 2020-02-02 00:00:00.000000 xtuples-0.0.7/README.md
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 xtuples-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    15265 2020-02-02 00:00:00.000000 xtuples-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    28408 2020-02-02 00:00:00.000000 xtuples-0.0.8/README.ipynb
+-rw-r--r--   0        0        0     7004 2020-02-02 00:00:00.000000 xtuples-0.0.8/docs/index.html
+-rw-r--r--   0        0        0    22834 2020-02-02 00:00:00.000000 xtuples-0.0.8/docs/json.html
+-rw-r--r--   0        0        0   106349 2020-02-02 00:00:00.000000 xtuples-0.0.8/docs/xtuples.html
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 xtuples-0.0.8/src/xtuples/__about__.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 xtuples-0.0.8/src/xtuples/__init__.py
+-rw-r--r--   0        0        0     5845 2020-02-02 00:00:00.000000 xtuples-0.0.8/src/xtuples/json.py
+-rw-r--r--   0        0        0    21657 2020-02-02 00:00:00.000000 xtuples-0.0.8/src/xtuples/xtuples.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 xtuples-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 xtuples-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 xtuples-0.0.8/LICENSE.txt
+-rw-r--r--   0        0        0    15965 2020-02-02 00:00:00.000000 xtuples-0.0.8/README.md
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 xtuples-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    16081 2020-02-02 00:00:00.000000 xtuples-0.0.8/PKG-INFO
```

### Comparing `xtuples-0.0.7/README.ipynb` & `xtuples-0.0.8/README.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9945147679324895%*

 * *Differences: {"'cells'": "{16: {'source': {insert: [(0, 'Here, we pipe into but discard the output of print(), "*

 * *            'so we still get back out an iTuple of Ticker_Prices (even whilst print() would '*

 * *            "otherwise return None).\\n')], delete: [0]}}, 27: {'source': ['As such, iTuple "*

 * *            'creation time is fairly similar to that of a raw list, at least when amortised over '*

 * *            "long enough sequences (though is generally slower for shorter ones):']}, 31: "*

 * *            "{'execution_count':  […]*

```diff
@@ -190,15 +190,15 @@
         {
             "cell_type": "markdown",
             "metadata": {
                 "jp-MarkdownHeadingCollapsed": true,
                 "tags": []
             },
             "source": [
-                "Here, we pipe into but discard the output of print(), so we still get back out and iTuple of Ticker_Prices (even whilst print() would otherwise return None).\n",
+                "Here, we pipe into but discard the output of print(), so we still get back out an iTuple of Ticker_Prices (even whilst print() would otherwise return None).\n",
                 "\n",
                 "Let's say that we want to map the prices into some new currency:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
@@ -326,34 +326,91 @@
                 "#### Creation & Memory"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "As such, creation takes a fairly similar time to that of a raw list (a raw tuple would probably be faster):"
+                "As such, iTuple creation time is fairly similar to that of a raw list, at least when amortised over long enough sequences (though is generally slower for shorter ones):"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 31,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "1.85 \u00b5s \u00b1 26 ns per loop (mean \u00b1 std. dev. of 7 runs, 1,000,000 loops each)\n",
-                        "560 ns \u00b1 2.41 ns per loop (mean \u00b1 std. dev. of 7 runs, 1,000,000 loops each)\n"
+                        "1.83 \u00b5s \u00b1 33.2 ns per loop (mean \u00b1 std. dev. of 7 runs, 1,000,000 loops each)\n",
+                        "570 ns \u00b1 6.58 ns per loop (mean \u00b1 std. dev. of 7 runs, 1,000,000 loops each)\n"
                     ]
                 }
             ],
             "source": [
-                "%timeit xtuples.iTuple.range(100)\n",
-                "%timeit list(range(100))"
+                "%timeit xtuples.iTuple.range(10 ** 2)\n",
+                "%timeit list(range(10 ** 2))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 34,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "10.7 \u00b5s \u00b1 104 ns per loop (mean \u00b1 std. dev. of 7 runs, 100,000 loops each)\n",
+                        "7.87 \u00b5s \u00b1 102 ns per loop (mean \u00b1 std. dev. of 7 runs, 100,000 loops each)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "%timeit xtuples.iTuple.range(10 ** 3)\n",
+                "%timeit list(range(10 ** 3))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 33,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "110 \u00b5s \u00b1 627 ns per loop (mean \u00b1 std. dev. of 7 runs, 10,000 loops each)\n",
+                        "91.3 \u00b5s \u00b1 506 ns per loop (mean \u00b1 std. dev. of 7 runs, 10,000 loops each)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "%timeit xtuples.iTuple.range(10 ** 4)\n",
+                "%timeit list(range(10 ** 4))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 36,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "26.2 ms \u00b1 656 \u00b5s per loop (mean \u00b1 std. dev. of 7 runs, 10 loops each)\n",
+                        "24.6 ms \u00b1 717 \u00b5s per loop (mean \u00b1 std. dev. of 7 runs, 10 loops each)\n"
+                    ]
+                }
+            ],
+            "source": [
+                "%timeit xtuples.iTuple.range(10 ** 6)\n",
+                "%timeit list(range(10 ** 6))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Memory usage is very similar:"
```

### Comparing `xtuples-0.0.7/docs/index.html` & `xtuples-0.0.8/docs/index.html`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.7/docs/json.html` & `xtuples-0.0.8/docs/json.html`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.7/docs/xtuples.html` & `xtuples-0.0.8/docs/xtuples.html`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.7/src/xtuples/json.py` & `xtuples-0.0.8/src/xtuples/json.py`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.7/src/xtuples/xtuples.py` & `xtuples-0.0.8/src/xtuples/xtuples.py`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.7/.gitignore` & `xtuples-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.7/LICENSE.txt` & `xtuples-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.7/README.md` & `xtuples-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     .pipe(print, discard=True)
 )
 ```
 
     iTuple(Ticker_Price(ticker='IBM US Equity', price=100), Ticker_Price(ticker='AAPL US Equity', price=105), Ticker_Price(ticker='F US Equity', price=95))
     
 
-Here, we pipe into but discard the output of print(), so we still get back out and iTuple of Ticker_Prices (even whilst print() would otherwise return None).
+Here, we pipe into but discard the output of print(), so we still get back out an iTuple of Ticker_Prices (even whilst print() would otherwise return None).
 
 Let's say that we want to map the prices into some new currency:
 
 
 ```python
 def convert_price(ticker, price, fx):
     return price * fx
@@ -144,24 +144,54 @@
 
 ### iTuple
 
 For instance, iTuple is a relatively minimal wrapper around the built in tuple.
 
 #### Creation & Memory
 
-As such, creation takes a fairly similar time to that of a raw list (a raw tuple would probably be faster):
+As such, iTuple creation time is fairly similar to that of a raw list, at least when amortised over long enough sequences (though is generally slower for shorter ones):
 
 
 ```python
-%timeit xtuples.iTuple.range(100)
-%timeit list(range(100))
+%timeit xtuples.iTuple.range(10 ** 2)
+%timeit list(range(10 ** 2))
 ```
 
-    1.85 µs ± 26 ns per loop (mean ± std. dev. of 7 runs, 1,000,000 loops each)
-    560 ns ± 2.41 ns per loop (mean ± std. dev. of 7 runs, 1,000,000 loops each)
+    1.83 µs ± 33.2 ns per loop (mean ± std. dev. of 7 runs, 1,000,000 loops each)
+    570 ns ± 6.58 ns per loop (mean ± std. dev. of 7 runs, 1,000,000 loops each)
+    
+
+
+```python
+%timeit xtuples.iTuple.range(10 ** 3)
+%timeit list(range(10 ** 3))
+```
+
+    10.7 µs ± 104 ns per loop (mean ± std. dev. of 7 runs, 100,000 loops each)
+    7.87 µs ± 102 ns per loop (mean ± std. dev. of 7 runs, 100,000 loops each)
+    
+
+
+```python
+%timeit xtuples.iTuple.range(10 ** 4)
+%timeit list(range(10 ** 4))
+```
+
+    110 µs ± 627 ns per loop (mean ± std. dev. of 7 runs, 10,000 loops each)
+    91.3 µs ± 506 ns per loop (mean ± std. dev. of 7 runs, 10,000 loops each)
+    
+
+
+```python
+%timeit xtuples.iTuple.range(10 ** 6)
+%timeit list(range(10 ** 6))
+```
+
+    26.2 ms ± 656 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
+    24.6 ms ± 717 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
     
 
 Memory usage is very similar:
 
 
 ```python
 memory = {}
```

### Comparing `xtuples-0.0.7/pyproject.toml` & `xtuples-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xtuples-0.0.7/PKG-INFO` & `xtuples-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtuples
-Version: 0.0.7
+Version: 0.0.8
 Project-URL: Documentation, https://tomjrwilliams.github.io/xtuples/
 Project-URL: Issues, https://github.com/tomjrwilliams/xtuples/issues
 Project-URL: Source, https://github.com/tomjrwilliams/xtuples
 Author-email: Tom Williams <tomjrw@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -101,15 +101,15 @@
     .pipe(print, discard=True)
 )
 ```
 
     iTuple(Ticker_Price(ticker='IBM US Equity', price=100), Ticker_Price(ticker='AAPL US Equity', price=105), Ticker_Price(ticker='F US Equity', price=95))
     
 
-Here, we pipe into but discard the output of print(), so we still get back out and iTuple of Ticker_Prices (even whilst print() would otherwise return None).
+Here, we pipe into but discard the output of print(), so we still get back out an iTuple of Ticker_Prices (even whilst print() would otherwise return None).
 
 Let's say that we want to map the prices into some new currency:
 
 
 ```python
 def convert_price(ticker, price, fx):
     return price * fx
@@ -161,24 +161,54 @@
 
 ### iTuple
 
 For instance, iTuple is a relatively minimal wrapper around the built in tuple.
 
 #### Creation & Memory
 
-As such, creation takes a fairly similar time to that of a raw list (a raw tuple would probably be faster):
+As such, iTuple creation time is fairly similar to that of a raw list, at least when amortised over long enough sequences (though is generally slower for shorter ones):
 
 
 ```python
-%timeit xtuples.iTuple.range(100)
-%timeit list(range(100))
+%timeit xtuples.iTuple.range(10 ** 2)
+%timeit list(range(10 ** 2))
 ```
 
-    1.85 µs ± 26 ns per loop (mean ± std. dev. of 7 runs, 1,000,000 loops each)
-    560 ns ± 2.41 ns per loop (mean ± std. dev. of 7 runs, 1,000,000 loops each)
+    1.83 µs ± 33.2 ns per loop (mean ± std. dev. of 7 runs, 1,000,000 loops each)
+    570 ns ± 6.58 ns per loop (mean ± std. dev. of 7 runs, 1,000,000 loops each)
+    
+
+
+```python
+%timeit xtuples.iTuple.range(10 ** 3)
+%timeit list(range(10 ** 3))
+```
+
+    10.7 µs ± 104 ns per loop (mean ± std. dev. of 7 runs, 100,000 loops each)
+    7.87 µs ± 102 ns per loop (mean ± std. dev. of 7 runs, 100,000 loops each)
+    
+
+
+```python
+%timeit xtuples.iTuple.range(10 ** 4)
+%timeit list(range(10 ** 4))
+```
+
+    110 µs ± 627 ns per loop (mean ± std. dev. of 7 runs, 10,000 loops each)
+    91.3 µs ± 506 ns per loop (mean ± std. dev. of 7 runs, 10,000 loops each)
+    
+
+
+```python
+%timeit xtuples.iTuple.range(10 ** 6)
+%timeit list(range(10 ** 6))
+```
+
+    26.2 ms ± 656 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
+    24.6 ms ± 717 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
     
 
 Memory usage is very similar:
 
 
 ```python
 memory = {}
```

