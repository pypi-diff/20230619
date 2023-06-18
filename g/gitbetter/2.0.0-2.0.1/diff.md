# Comparing `tmp/gitbetter-2.0.0.tar.gz` & `tmp/gitbetter-2.0.1.tar.gz`

## Comparing `gitbetter-2.0.0.tar` & `gitbetter-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 gitbetter-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0    34198 2020-02-02 00:00:00.000000 gitbetter-2.0.0/docs/gitbetter.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-2.0.0/docs/index.html
--rw-r--r--   0        0        0   178440 2020-02-02 00:00:00.000000 gitbetter-2.0.0/docs/search.js
--rw-r--r--   0        0        0   592710 2020-02-02 00:00:00.000000 gitbetter-2.0.0/docs/gitbetter/git.html
--rw-r--r--   0        0        0   524054 2020-02-02 00:00:00.000000 gitbetter-2.0.0/docs/gitbetter/gitbetter.html
--rw-r--r--   0        0        0    58253 2020-02-02 00:00:00.000000 gitbetter-2.0.0/docs/gitbetter/parsers.html
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 gitbetter-2.0.0/src/gitbetter/__init__.py
--rw-r--r--   0        0        0    19360 2020-02-02 00:00:00.000000 gitbetter-2.0.0/src/gitbetter/git.py
--rw-r--r--   0        0        0    17224 2020-02-02 00:00:00.000000 gitbetter-2.0.0/src/gitbetter/gitbetter.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 gitbetter-2.0.0/src/gitbetter/parsers.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 gitbetter-2.0.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-2.0.0/LICENSE.txt
--rw-r--r--   0        0        0     6518 2020-02-02 00:00:00.000000 gitbetter-2.0.0/README.md
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 gitbetter-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 gitbetter-2.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0    34198 2020-02-02 00:00:00.000000 gitbetter-2.0.1/docs/gitbetter.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-2.0.1/docs/index.html
+-rw-r--r--   0        0        0   178440 2020-02-02 00:00:00.000000 gitbetter-2.0.1/docs/search.js
+-rw-r--r--   0        0        0   592728 2020-02-02 00:00:00.000000 gitbetter-2.0.1/docs/gitbetter/git.html
+-rw-r--r--   0        0        0   524054 2020-02-02 00:00:00.000000 gitbetter-2.0.1/docs/gitbetter/gitbetter.html
+-rw-r--r--   0        0        0    58253 2020-02-02 00:00:00.000000 gitbetter-2.0.1/docs/gitbetter/parsers.html
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 gitbetter-2.0.1/src/gitbetter/__init__.py
+-rw-r--r--   0        0        0    19366 2020-02-02 00:00:00.000000 gitbetter-2.0.1/src/gitbetter/git.py
+-rw-r--r--   0        0        0    17224 2020-02-02 00:00:00.000000 gitbetter-2.0.1/src/gitbetter/gitbetter.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 gitbetter-2.0.1/src/gitbetter/parsers.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 gitbetter-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-2.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     6518 2020-02-02 00:00:00.000000 gitbetter-2.0.1/README.md
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 gitbetter-2.0.1/PKG-INFO
```

### Comparing `gitbetter-2.0.0/CHANGELOG.md` & `gitbetter-2.0.1/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,48 @@
 # Changelog
 
+## v2.0.0 (2023-06-13)
+
+#### New Features
+
+* help command shows built in git commands and convenience commands separately
+* add commit_all()
+* add ignore() to Git
+* do_initcommit can take a list of files instead of only operating on all files
+* add all core git commands to gitbetter shell
+* initcommit() can accept a list of files
+* add owner and repo name properties
+* add all porcelain git commands
+#### Fixes
+
+* fix faulty import statement
+* replace backslashes with forward slashes in add_files if there are any
+#### Refactorings
+
+* do_push_new() will use current_branch property instead of needing branch name supplied
+* remove recursive options from shell parsers in favor of native wildcard usage
+* remove quote check from do_commitall
+* make origin_url a property
+* move shell parsers to separate file
+* change some convenience functions to use newly added core functions
+* change execute method name to git
+* update to revised Git functions
+* remove owner and name params from github cli functions
+#### Docs
+
+* update readme
+* update and improve docstrings
+#### Others
+
+* remove unused imports
+* remove unused arg from do_delete_gh_repo
+* add to ignore
+* update ignores
+
+
 ## v1.4.0 (2023-06-01)
 
 #### Refactorings
 
 * no longer necessary to specify the -f/--files flag before listing files when using the add command
 ## v1.3.0 (2023-05-30)
```

### Comparing `gitbetter-2.0.0/docs/gitbetter.html` & `gitbetter-2.0.1/docs/gitbetter.html`

 * *Files identical despite different names*

### Comparing `gitbetter-2.0.0/docs/search.js` & `gitbetter-2.0.1/docs/search.js`

 * *Files identical despite different names*

### Comparing `gitbetter-2.0.0/docs/gitbetter/git.html` & `gitbetter-2.0.1/docs/gitbetter/git.html`

 * *Files 0% similar despite different names*

```diff
@@ -738,15 +738,15 @@
 </span><span id="L-379"><a href="#L-379"><span class="linenos">379</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit changes to the previous commit.</span>
 </span><span id="L-380"><a href="#L-380"><span class="linenos">380</span></a>
 </span><span id="L-381"><a href="#L-381"><span class="linenos">381</span></a><span class="sd">        If `files` is `None`, all files will be staged.</span>
 </span><span id="L-382"><a href="#L-382"><span class="linenos">382</span></a>
 </span><span id="L-383"><a href="#L-383"><span class="linenos">383</span></a><span class="sd">        &gt;&gt;&gt; git add {files} or git add .</span>
 </span><span id="L-384"><a href="#L-384"><span class="linenos">384</span></a><span class="sd">        &gt;&gt;&gt; git commit --amend --no-edit</span>
 </span><span id="L-385"><a href="#L-385"><span class="linenos">385</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="L-386"><a href="#L-386"><span class="linenos">386</span></a>        <span class="k">return</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="k">if</span> <span class="n">files</span> <span class="k">else</span> <span class="bp">self</span><span class="o">.</span><span class="n">add_all</span><span class="p">())</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="L-386"><a href="#L-386"><span class="linenos">386</span></a>        <span class="k">return</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">add_files</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="k">if</span> <span class="n">files</span> <span class="k">else</span> <span class="bp">self</span><span class="o">.</span><span class="n">add_all</span><span class="p">())</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
 </span><span id="L-387"><a href="#L-387"><span class="linenos">387</span></a>
 </span><span id="L-388"><a href="#L-388"><span class="linenos">388</span></a>    <span class="k">def</span> <span class="nf">commit_all</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
 </span><span id="L-389"><a href="#L-389"><span class="linenos">389</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with `message`.</span>
 </span><span id="L-390"><a href="#L-390"><span class="linenos">390</span></a><span class="sd">        &gt;&gt;&gt; git add .</span>
 </span><span id="L-391"><a href="#L-391"><span class="linenos">391</span></a><span class="sd">        &gt;&gt;&gt; git commit -m \&quot;{message}\&quot; &quot;&quot;&quot;</span>
 </span><span id="L-392"><a href="#L-392"><span class="linenos">392</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add_all</span><span class="p">()</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
 </span><span id="L-393"><a href="#L-393"><span class="linenos">393</span></a>
@@ -1274,15 +1274,15 @@
 </span><span id="Git-380"><a href="#Git-380"><span class="linenos">380</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit changes to the previous commit.</span>
 </span><span id="Git-381"><a href="#Git-381"><span class="linenos">381</span></a>
 </span><span id="Git-382"><a href="#Git-382"><span class="linenos">382</span></a><span class="sd">        If `files` is `None`, all files will be staged.</span>
 </span><span id="Git-383"><a href="#Git-383"><span class="linenos">383</span></a>
 </span><span id="Git-384"><a href="#Git-384"><span class="linenos">384</span></a><span class="sd">        &gt;&gt;&gt; git add {files} or git add .</span>
 </span><span id="Git-385"><a href="#Git-385"><span class="linenos">385</span></a><span class="sd">        &gt;&gt;&gt; git commit --amend --no-edit</span>
 </span><span id="Git-386"><a href="#Git-386"><span class="linenos">386</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Git-387"><a href="#Git-387"><span class="linenos">387</span></a>        <span class="k">return</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="k">if</span> <span class="n">files</span> <span class="k">else</span> <span class="bp">self</span><span class="o">.</span><span class="n">add_all</span><span class="p">())</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="Git-387"><a href="#Git-387"><span class="linenos">387</span></a>        <span class="k">return</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">add_files</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="k">if</span> <span class="n">files</span> <span class="k">else</span> <span class="bp">self</span><span class="o">.</span><span class="n">add_all</span><span class="p">())</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
 </span><span id="Git-388"><a href="#Git-388"><span class="linenos">388</span></a>
 </span><span id="Git-389"><a href="#Git-389"><span class="linenos">389</span></a>    <span class="k">def</span> <span class="nf">commit_all</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">str</span> <span class="o">|</span> <span class="nb">int</span><span class="p">:</span>
 </span><span id="Git-390"><a href="#Git-390"><span class="linenos">390</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with `message`.</span>
 </span><span id="Git-391"><a href="#Git-391"><span class="linenos">391</span></a><span class="sd">        &gt;&gt;&gt; git add .</span>
 </span><span id="Git-392"><a href="#Git-392"><span class="linenos">392</span></a><span class="sd">        &gt;&gt;&gt; git commit -m \&quot;{message}\&quot; &quot;&quot;&quot;</span>
 </span><span id="Git-393"><a href="#Git-393"><span class="linenos">393</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">add_all</span><span class="p">()</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
 </span><span id="Git-394"><a href="#Git-394"><span class="linenos">394</span></a>
@@ -3469,15 +3469,15 @@
 </span><span id="Git.amend-380"><a href="#Git.amend-380"><span class="linenos">380</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit changes to the previous commit.</span>
 </span><span id="Git.amend-381"><a href="#Git.amend-381"><span class="linenos">381</span></a>
 </span><span id="Git.amend-382"><a href="#Git.amend-382"><span class="linenos">382</span></a><span class="sd">        If `files` is `None`, all files will be staged.</span>
 </span><span id="Git.amend-383"><a href="#Git.amend-383"><span class="linenos">383</span></a>
 </span><span id="Git.amend-384"><a href="#Git.amend-384"><span class="linenos">384</span></a><span class="sd">        &gt;&gt;&gt; git add {files} or git add .</span>
 </span><span id="Git.amend-385"><a href="#Git.amend-385"><span class="linenos">385</span></a><span class="sd">        &gt;&gt;&gt; git commit --amend --no-edit</span>
 </span><span id="Git.amend-386"><a href="#Git.amend-386"><span class="linenos">386</span></a><span class="sd">        &quot;&quot;&quot;</span>
-</span><span id="Git.amend-387"><a href="#Git.amend-387"><span class="linenos">387</span></a>        <span class="k">return</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="k">if</span> <span class="n">files</span> <span class="k">else</span> <span class="bp">self</span><span class="o">.</span><span class="n">add_all</span><span class="p">())</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="Git.amend-387"><a href="#Git.amend-387"><span class="linenos">387</span></a>        <span class="k">return</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">add_files</span><span class="p">(</span><span class="n">files</span><span class="p">)</span> <span class="k">if</span> <span class="n">files</span> <span class="k">else</span> <span class="bp">self</span><span class="o">.</span><span class="n">add_all</span><span class="p">())</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit changes to the previous commit.</p>
 
 <p>If <code>files</code> is <code>None</code>, all files will be staged.</p>
```

#### html2text {}

```diff
@@ -494,16 +494,16 @@
 379        """Stage and commit changes to the previous commit.
 380
 381        If `files` is `None`, all files will be staged.
 382
 383        >>> git add {files} or git add .
 384        >>> git commit --amend --no-edit
 385        """
-386        return (self.add(files) if files else self.add_all()) + self.commit
-("--amend --no-edit")  # type: ignore
+386        return (self.add_files(files) if files else self.add_all()) +
+self.commit("--amend --no-edit")  # type: ignore
 387
 388    def commit_all(self, message: str) -> str | int:
 389        """Stage and commit all files with `message`.
 390        >>> git add .
 391        >>> git commit -m \"{message}\" """
 392        return self.add_all() + self.commit(f'-m "{message}"')  # type:
 ignore
@@ -1043,16 +1043,16 @@
 380        """Stage and commit changes to the previous commit.
 381
 382        If `files` is `None`, all files will be staged.
 383
 384        >>> git add {files} or git add .
 385        >>> git commit --amend --no-edit
 386        """
-387        return (self.add(files) if files else self.add_all()) + self.commit
-("--amend --no-edit")  # type: ignore
+387        return (self.add_files(files) if files else self.add_all()) +
+self.commit("--amend --no-edit")  # type: ignore
 388
 389    def commit_all(self, message: str) -> str | int:
 390        """Stage and commit all files with `message`.
 391        >>> git add .
 392        >>> git commit -m \"{message}\" """
 393        return self.add_all() + self.commit(f'-m "{message}"')  # type:
 ignore
@@ -1723,16 +1723,16 @@
 380        """Stage and commit changes to the previous commit.
 381
 382        If `files` is `None`, all files will be staged.
 383
 384        >>> git add {files} or git add .
 385        >>> git commit --amend --no-edit
 386        """
-387        return (self.add(files) if files else self.add_all()) + self.commit
-("--amend --no-edit")  # type: ignore
+387        return (self.add_files(files) if files else self.add_all()) +
+self.commit("--amend --no-edit")  # type: ignore
 Stage and commit changes to the previous commit.
 If files is None, all files will be staged.
 >>> git add {files} or git add .
 >>> git commit --amend --no-edit
 ⁰
 def commit_all(self, message: str) -> str | int: View Source
 389    def commit_all(self, message: str) -> str | int:
```

### Comparing `gitbetter-2.0.0/docs/gitbetter/gitbetter.html` & `gitbetter-2.0.1/docs/gitbetter/gitbetter.html`

 * *Files identical despite different names*

### Comparing `gitbetter-2.0.0/docs/gitbetter/parsers.html` & `gitbetter-2.0.1/docs/gitbetter/parsers.html`

 * *Files identical despite different names*

### Comparing `gitbetter-2.0.0/src/gitbetter/git.py` & `gitbetter-2.0.1/src/gitbetter/git.py`

 * *Files 0% similar despite different names*

```diff
@@ -379,15 +379,15 @@
         """Stage and commit changes to the previous commit.
 
         If `files` is `None`, all files will be staged.
 
         >>> git add {files} or git add .
         >>> git commit --amend --no-edit
         """
-        return (self.add(files) if files else self.add_all()) + self.commit("--amend --no-edit")  # type: ignore
+        return (self.add_files(files) if files else self.add_all()) + self.commit("--amend --no-edit")  # type: ignore
 
     def commit_all(self, message: str) -> str | int:
         """Stage and commit all files with `message`.
         >>> git add .
         >>> git commit -m \"{message}\" """
         return self.add_all() + self.commit(f'-m "{message}"')  # type: ignore
```

### Comparing `gitbetter-2.0.0/src/gitbetter/gitbetter.py` & `gitbetter-2.0.1/src/gitbetter/gitbetter.py`

 * *Files identical despite different names*

### Comparing `gitbetter-2.0.0/src/gitbetter/parsers.py` & `gitbetter-2.0.1/src/gitbetter/parsers.py`

 * *Files identical despite different names*

### Comparing `gitbetter-2.0.0/LICENSE.txt` & `gitbetter-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitbetter-2.0.0/README.md` & `gitbetter-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `gitbetter-2.0.0/pyproject.toml` & `gitbetter-2.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6769 7462 6574 7465 7222 0d0a 6465   "gitbetter"..de
 00000070: 7363 7269 7074 696f 6e20 3d20 2243 7573  scription = "Cus
 00000080: 746f 6d20 6769 7420 7368 656c 6c20 746f  tom git shell to
 00000090: 2074 7970 6520 6c65 7373 2061 6e64 2063   type less and c
 000000a0: 6f6d 6d69 7420 6d6f 7265 2e22 0d0a 7665  ommit more."..ve
-000000b0: 7273 696f 6e20 3d20 2232 2e30 2e30 220d  rsion = "2.0.0".
+000000b0: 7273 696f 6e20 3d20 2232 2e30 2e31 220d  rsion = "2.0.1".
 000000c0: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
 000000d0: 203d 2022 3e3d 332e 3130 220d 0a64 6570   = ">=3.10"..dep
 000000e0: 656e 6465 6e63 6965 7320 3d20 5b22 6172  endencies = ["ar
 000000f0: 6773 6865 6c6c 222c 2022 7061 7468 6965  gshell", "pathie
 00000100: 7222 2c20 2270 7974 6573 7422 5d0d 0a72  r", "pytest"]..r
 00000110: 6561 646d 6520 3d20 2252 4541 444d 452e  eadme = "README.
 00000120: 6d64 220d 0a6b 6579 776f 7264 7320 3d20  md"..keywords =
```

### Comparing `gitbetter-2.0.0/PKG-INFO` & `gitbetter-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitbetter
-Version: 2.0.0
+Version: 2.0.1
 Summary: Custom git shell to type less and commit more.
 Project-URL: Homepage, https://github.com/matt-manes/gitbetter
 Project-URL: Documentation, https://github.com/matt-manes/gitbetter/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/gitbetter/tree/main/src/gitbetter
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: cli,commit,git,shell,terminal
```

