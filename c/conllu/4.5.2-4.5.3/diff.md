# Comparing `tmp/conllu-4.5.2.tar.gz` & `tmp/conllu-4.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conllu-4.5.2.tar", last modified: Fri Jul 29 07:54:00 2022, max compression
+gzip compressed data, was "conllu-4.5.3.tar", last modified: Mon Jun 19 12:37:38 2023, max compression
```

## Comparing `conllu-4.5.2.tar` & `conllu-4.5.3.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxr-xr-x   0 emilstenstrom  (1000) emilstenstrom  (1000)        0 2022-07-29 07:54:00.193440 conllu-4.5.2/
--rw-r--r--   0 emilstenstrom  (1000) emilstenstrom  (1000)     3218 2020-12-09 19:31:29.000000 conllu-4.5.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 emilstenstrom  (1000) emilstenstrom  (1000)     1082 2020-12-09 19:31:29.000000 conllu-4.5.2/LICENSE
--rw-r--r--   0 emilstenstrom  (1000) emilstenstrom  (1000)       61 2020-12-09 19:31:29.000000 conllu-4.5.2/MANIFEST.in
--rw-r--r--   0 emilstenstrom  (1000) emilstenstrom  (1000)    19591 2022-07-29 07:54:00.193440 conllu-4.5.2/PKG-INFO
--rw-r--r--   0 emilstenstrom  (1000) emilstenstrom  (1000)    19205 2022-06-06 12:29:25.000000 conllu-4.5.2/README.md
-drwxr-xr-x   0 emilstenstrom  (1000) emilstenstrom  (1000)        0 2022-07-29 07:54:00.193440 conllu-4.5.2/conllu/
--rw-r--r--   0 emilstenstrom  (1000) emilstenstrom  (1000)     2057 2022-07-13 17:01:57.000000 conllu-4.5.2/conllu/__init__.py
--rw-r--r--   0 emilstenstrom  (1000) emilstenstrom  (1000)       42 2020-12-09 19:31:29.000000 conllu-4.5.2/conllu/exceptions.py
--rw-r--r--   0 emilstenstrom  (1000) emilstenstrom  (1000)    13786 2022-07-12 20:29:17.000000 conllu-4.5.2/conllu/models.py
--rw-r--r--   0 emilstenstrom  (1000) emilstenstrom  (1000)     9318 2022-07-29 07:47:46.000000 conllu-4.5.2/conllu/parser.py
--rw-r--r--   0 emilstenstrom  (1000) emilstenstrom  (1000)        0 2020-12-09 19:31:29.000000 conllu-4.5.2/conllu/py.typed
--rw-r--r--   0 emilstenstrom  (1000) emilstenstrom  (1000)     1426 2022-07-12 15:01:41.000000 conllu-4.5.2/conllu/serializer.py
-drwxr-xr-x   0 emilstenstrom  (1000) emilstenstrom  (1000)        0 2022-07-29 07:54:00.193440 conllu-4.5.2/conllu.egg-info/
--rw-r--r--   0 emilstenstrom  (1000) emilstenstrom  (1000)    19591 2022-07-29 07:54:00.000000 conllu-4.5.2/conllu.egg-info/PKG-INFO
--rw-r--r--   0 emilstenstrom  (1000) emilstenstrom  (1000)      298 2022-07-29 07:54:00.000000 conllu-4.5.2/conllu.egg-info/SOURCES.txt
--rw-r--r--   0 emilstenstrom  (1000) emilstenstrom  (1000)        1 2022-07-29 07:54:00.000000 conllu-4.5.2/conllu.egg-info/dependency_links.txt
--rw-r--r--   0 emilstenstrom  (1000) emilstenstrom  (1000)        7 2022-07-29 07:54:00.000000 conllu-4.5.2/conllu.egg-info/top_level.txt
--rw-r--r--   0 emilstenstrom  (1000) emilstenstrom  (1000)      498 2022-07-29 07:54:00.193440 conllu-4.5.2/setup.cfg
--rw-r--r--   0 emilstenstrom  (1000) emilstenstrom  (1000)     1225 2022-07-29 07:49:44.000000 conllu-4.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:37:38.395475 conllu-4.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-19 12:37:29.000000 conllu-4.5.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-19 12:37:29.000000 conllu-4.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-19 12:37:29.000000 conllu-4.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19571 2023-06-19 12:37:38.395475 conllu-4.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18725 2023-06-19 12:37:29.000000 conllu-4.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:37:38.395475 conllu-4.5.3/conllu/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-19 12:37:29.000000 conllu-4.5.3/conllu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-19 12:37:29.000000 conllu-4.5.3/conllu/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-06-19 12:37:29.000000 conllu-4.5.3/conllu/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-06-19 12:37:29.000000 conllu-4.5.3/conllu/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:37:29.000000 conllu-4.5.3/conllu/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-19 12:37:29.000000 conllu-4.5.3/conllu/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:37:38.395475 conllu-4.5.3/conllu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19571 2023-06-19 12:37:38.000000 conllu-4.5.3/conllu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-19 12:37:38.000000 conllu-4.5.3/conllu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:37:38.000000 conllu-4.5.3/conllu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 12:37:38.000000 conllu-4.5.3/conllu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-19 12:37:38.395475 conllu-4.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-19 12:37:29.000000 conllu-4.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:37:38.395475 conllu-4.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-06-19 12:37:29.000000 conllu-4.5.3/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22382 2023-06-19 12:37:29.000000 conllu-4.5.3/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27449 2023-06-19 12:37:29.000000 conllu-4.5.3/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-19 12:37:29.000000 conllu-4.5.3/tests/test_readme.py
```

### Comparing `conllu-4.5.2/CODE_OF_CONDUCT.md` & `conllu-4.5.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `conllu-4.5.2/LICENSE` & `conllu-4.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `conllu-4.5.2/PKG-INFO` & `conllu-4.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: conllu
-Version: 4.5.2
+Version: 4.5.3
 Summary: CoNLL-U Parser parses a CoNLL-U formatted string into a nested python dictionary
 Home-page: https://github.com/EmilStenstrom/conllu/
 Author: Emil Stenström
 Author-email: emil@emilstenstrom.se
 License: MIT License
 Keywords: conllu,conll,conll-u,parser,nlp
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -497,9 +496,7 @@
     ```bash
     tox -e py36
     ```
 
 5. Make a pull request. Here's a [good guide on PRs from GitHub](https://help.github.com/articles/creating-a-pull-request-from-a-fork/).
 
 Thanks for helping conllu become a better library!
-
-
```

### Comparing `conllu-4.5.2/README.md` & `conllu-4.5.3/conllu.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,480 +1,502 @@
-# CoNLL-U Parser
-
-**CoNLL-U Parser** parses a [CoNLL-U formatted](http://universaldependencies.org/format.html) string into a nested python dictionary. CoNLL-U is often the output of natural language processing tasks.
-
-## Why should you use conllu?
-
-- It's simple. ~300 lines of code.
-- It has no dependencies
-- Full typing support so your editor can do autocompletion
-- Nice set of tests with CI setup: [![Build](https://github.com/EmilStenstrom/conllu/workflows/Run%20tests%20for%20all%20supported%20python%20versions/badge.svg)](https://github.com/EmilStenstrom/conllu/actions?query=workflow%3A%22Run+tests+for+all+supported+python+versions%22)
-- It has 100% test branch coverage (and has undergone [mutation testing](https://github.com/boxed/mutmut/))
-- It has [![lots of downloads](http://pepy.tech/badge/conllu)](http://pepy.tech/project/conllu)
-
-## Installation
-
-Note: As of conllu 4.0, Python 3.6 is required to install conllu. See [Notes on updating from 3.0 to 4.0](#notes-on-updating-from-30-to-40)
-
-```bash
-pip install conllu
-```
-
-Or, if you are using [conda](https://conda.io/docs/):
-
-```bash
-conda install -c conda-forge conllu
-```
-
-## Notes on updating from 3.0 to 4.0
-
-Conllu version 4.0 drops support for Python 2 and all versions of earlier than Python 3.6. If you need support for older versions of python, you can always pin your install to an old version of conllu. You can install it with `pip install conllu==3.1.1`.
-
-## Notes on updating from 2.0 to 3.0
-
-The Universal dependencies 2.0 release changed two of the field names from xpostag -> xpos and upostag -> upos. Version 3.0 of conllu handles this by aliasing the previous names to the new names. This means you can use xpos/upos or xpostag/upostag, they will both return the same thing. This does change the public API slightly, so I've upped the major version to 3.0, but I've taken care to ensure you most likely DO NOT have to update your code when you update to 3.0.
-
-## Notes on updating from 0.1 to 1.0
-
-I don't like breaking backwards compatibility, but to be able to add new features I felt I had to. This means that updating from 0.1 to 1.0 *might* require code changes. Here's a guide on [how to upgrade to 1.0
-](https://github.com/EmilStenstrom/conllu/wiki/Migrating-from-0.1-to-1.0).
-
-## Example usage
-
-At the top level, conllu provides two methods, `parse` and `parse_tree`. The first one parses sentences and returns a flat list. The other returns a nested tree structure. Let's go through them one by one.
-
-## Use parse() to parse into a list of sentences
-
-```python
->>> from conllu import parse
->>> 
->>> data = """
-... # text = The quick brown fox jumps over the lazy dog.
-... 1   The     the    DET    DT   Definite=Def|PronType=Art   4   det     _   _
-... 2   quick   quick  ADJ    JJ   Degree=Pos                  4   amod    _   _
-... 3   brown   brown  ADJ    JJ   Degree=Pos                  4   amod    _   _
-... 4   fox     fox    NOUN   NN   Number=Sing                 5   nsubj   _   _
-... 5   jumps   jump   VERB   VBZ  Mood=Ind|Number=Sing|Person=3|Tense=Pres|VerbForm=Fin   0   root    _   _
-... 6   over    over   ADP    IN   _                           9   case    _   _
-... 7   the     the    DET    DT   Definite=Def|PronType=Art   9   det     _   _
-... 8   lazy    lazy   ADJ    JJ   Degree=Pos                  9   amod    _   _
-... 9   dog     dog    NOUN   NN   Number=Sing                 5   nmod    _   SpaceAfter=No
-... 10  .       .      PUNCT  .    _                           5   punct   _   _
-...
-... """
-```
-
-Now you have the data in a variable called `data`. Let's parse it:
-
-```python
->>> sentences = parse(data)
->>> sentences
-[TokenList<The, quick, brown, fox, jumps, over, the, lazy, dog, ., metadata={text: "The quick brown fox jumps over the lazy dog."}>]
-```
-
-<blockquote>
-
-**Advanced usage**: If you have many sentences (say over a megabyte) to parse at once, you can avoid loading them into memory at once by using `parse_incr()` instead of `parse`. It takes an opened file, and returns a generator instead of the list directly, so you need to either iterate over it, or call list() to get the TokenLists out. Here's how you would use it:
-
-```python
-from io import open
-from conllu import parse_incr
-
-data_file = open("huge_file.conllu", "r", encoding="utf-8")
-for tokenlist in parse_incr(data_file):
-    print(tokenlist)
-```
-
-For most files, `parse` works fine.
-</blockquote>
-
-Since one CoNLL-U file usually contains multiple sentences, `parse()` always returns a list of sentences. Each sentence is represented by a TokenList.
-
-```python
->>> sentence = sentences[0]
->>> sentence
-TokenList<The, quick, brown, fox, jumps, over, the, lazy, dog, ., metadata={text: "The quick brown fox jumps over the lazy dog."}>
-```
-
-The TokenList supports indexing, so you can get the first token, represented by an ordered dictionary, like this:
-
-```python
->>> token = sentence[0]
->>> token
-{'id': 1,
-     'form': 'The',
-     'lemma': 'the',
-     ...}
->>> token["form"]
-'The'
-```
-
-### New in conllu 2.0: `filter()` a TokenList
-
-```python
->>> sentence = sentences[0]
->>> sentence
-TokenList<The, quick, brown, fox, jumps, over, the, lazy, dog, ., metadata={text: "The quick brown fox jumps over the lazy dog."}>
->>> sentence.filter(form="quick")
-TokenList<quick>
-```
-
-By using `filter(field1__field2=value)` you can filter based on subelements further down in a parsed token.
-
-```python
->>> sentence.filter(feats__Degree="Pos")
-TokenList<quick, brown, lazy>
-```
-
-Filters can also be chained (meaning you can do `sentence.filter(...).filter(...)`), and filtering on multiple properties at the same time (`sentence.filter(field1=value1, field2=value2)`) means that ALL properties must match.
-
-#### New in conllu 4.3: `filter()` a TokenList by lambda
-
-You can also filter using a lambda function as value. This is useful if you, for instance, would like to filter out only tokens with integer ID:s:
-
-```python
->>> from conllu.models import TokenList, Token
->>> sentence2 = TokenList([
-...    Token(id=(1, "-", 2), form="It's"),
-...    Token(id=1, form="It"),
-...    Token(id=2, form="is"),
-... ])
->>> sentence2
-TokenList<It's, It, is>
->>> sentence2.filter(id=lambda x: type(x) is int)
-TokenList<It, is>
-```
-
-### Writing data back to a TokenList
-
-If you want to change your CoNLL-U file, there are a couple of convenience methods to know about.
-
-You can add a new token by simply appending a dictionary with the fields you want to a TokenList:
-
-```python
->>> sentence3 = TokenList([
-...    {"id": 1, "form": "Lazy"},
-...    {"id": 2, "form": "fox"},
-... ])
->>> sentence3
-TokenList<Lazy, fox>
->>> sentence3.append({"id": 3, "form": "box"})
->>> sentence3
-TokenList<Lazy, fox, box>
-```
-
-Changing a sentence just means indexing into it, and setting a value to what you want:
-
-```python
->>> sentence4 = TokenList([
-...    {"id": 1, "form": "Lazy"},
-...    {"id": 2, "form": "fox"},
-... ])
->>> sentence4[1]["form"] = "crocodile"
->>> sentence4
-TokenList<Lazy, crocodile>
->>> sentence4[1] = {"id": 2, "form": "elephant"}
->>> sentence4
-TokenList<Lazy, elephant>
-```
-
-If you omit a field when passing in a dict, conllu will fill in a "_" for those values.
-
-```python
->>> sentences = parse("1  The")
->>> sentences[0].append({"id": 2})
->>> sentences[0]
-TokenList<The, _>
-```
-
-### Parse metadata from a CoNLL-U file
-
-Each sentence can also have metadata in the form of comments before the sentence starts. This is available in a property on the TokenList called `metadata`.
-
-```python
->>> sentence.metadata
-{'text': 'The quick brown fox jumps over the lazy dog.'}
-```
-
-### Turn a TokenList back into CoNLL-U
-
-If you ever want to get your CoNLL-U formated text back (maybe after changing something?), use the `serialize()` method:
-
-```python
->>> print(sentence.serialize())
-# text = The quick brown fox jumps over the lazy dog.
-1   The     the     DET    DT   Definite=Def|PronType=Art   4   det    _   _
-2   quick   quick   ADJ    JJ   Degree=Pos                  4   amod   _   _
-3   brown   brown   ADJ    JJ   Degree=Pos                  4   amod   _   _
-4   fox     fox     NOUN   NN   Number=Sing                 5   nsubj  _   _
-5   jumps   jump    VERB   VBZ  Mood=Ind|Number=Sing|Person=3|Tense=Pres|VerbForm=Fin   0   root   _   _
-6   over    over    ADP    IN   _                           9   case   _   _
-7   the     the     DET    DT   Definite=Def|PronType=Art   9   det    _   _
-8   lazy    lazy    ADJ    JJ   Degree=Pos                  9   amod   _   _
-9   dog     dog     NOUN   NN   Number=Sing                 5   nmod   _   SpaceAfter=No
-10  .       .       PUNCT  .    _                           5   punct  _   _
-```
-
-### Turn a TokenList into a TokenTree (see below)
-
-You can also convert a TokenList to a TokenTree by using `to_tree`:
-
-```python
->>> sentence.to_tree()
-TokenTree<token={id=5, form=jumps}, children=[...]>
-```
-
-That's it!
-
-## Use parse_tree() to parse into a list of dependency trees
-
-Sometimes you're interested in the tree structure that hides in the `head` column of a CoNLL-U file. When this is the case, use `parse_tree` to get a nested structure representing the sentence.
-
-```python
->>> from conllu import parse_tree
->>> sentences = parse_tree(data)
->>> sentences
-[TokenTree<...>]
-```
-
-<blockquote>
-
-**Advanced usage**: If you have many sentences (say over a megabyte) to parse at once, you can avoid loading them into memory at once by using `parse_tree_incr()` instead of `parse_tree`. It takes an opened file, and returns a generator instead of the list directly, so you need to either iterate over it, or call list() to get the TokenTrees out. Here's how you would use it:
-
-```python
-from io import open
-from conllu import parse_tree_incr
-
-data_file = open("huge_file.conllu", "r", encoding="utf-8")
-for tokentree in parse_tree_incr(data_file):
-    print(tokentree)
-```
-
-</blockquote>
-
-Since one CoNLL-U file usually contains multiple sentences, `parse_tree()` always returns a list of sentences. Each sentence is represented by a TokenTree.
-
-```python
->>> root = sentences[0]
->>> root
-TokenTree<token={id=5, form=jumps}, children=[...]>
-```
-
-To quickly visualize the tree structure you can call `print_tree` on a TokenTree.
-
-```python
->>> root.print_tree()
-(deprel:root) form:jumps lemma:jump upos:VERB [5]
-    (deprel:nsubj) form:fox lemma:fox upos:NOUN [4]
-        (deprel:det) form:The lemma:the upos:DET [1]
-        (deprel:amod) form:quick lemma:quick upos:ADJ [2]
-        (deprel:amod) form:brown lemma:brown upos:ADJ [3]
-    (deprel:nmod) form:dog lemma:dog upos:NOUN [9]
-        (deprel:case) form:over lemma:over upos:ADP [6]
-        (deprel:det) form:the lemma:the upos:DET [7]
-        (deprel:amod) form:lazy lemma:lazy upos:ADJ [8]
-    (deprel:punct) form:. lemma:. upos:PUNCT [10]
-```
-
-To access the token corresponding to the current node in the tree, use `token`:
-
-```python
->>> root.token
-{
-    'id': 5,
-    'form': 'jumps',
-    'lemma': 'jump',
-    ...
-}
-```
-
-To start walking down the children of the current node, use the children attribute:
-
-```python
->>> children = root.children
->>> children
-[
-    TokenTree<token={id=4, form=fox}, children=[...]>,
-    TokenTree<token={id=9, form=dog}, children=[...]>,
-    TokenTree<token={id=10, form=.}, children=None>
-]
-```
-
-Just like with `parse()`, if a sentence has metadata it is available in a property on the TokenTree root called `metadata`.
-
-```python
->>> root.metadata
-{'text': 'The quick brown fox jumps over the lazy dog.'}
-```
-
-If you ever want to get your CoNLL-U formated text back (maybe after changing something?), use the `serialize()` method:
-
-```python
->>> print(root.serialize())
-# text = The quick brown fox jumps over the lazy dog.
-1   The     the    DET    DT   Definite=Def|PronType=Art   4   det     _   _
-2   quick   quick  ADJ    JJ   Degree=Pos                  4   amod    _   _
-...
-```
-
-If you want to write it back to a file, you can use something like this:
-
-```python
->>> from conllu import parse_tree
->>> sentences = parse_tree(data)
->>> 
->>> # Make some change to sentences here
->>> 
->>> with open('file-to-write-to', 'w') as f:
-...     f.writelines([sentence.serialize() + "\n" for sentence in sentences])
-```
-
-## Customizing parsing to handle strange variations of CoNLL-U
-
-Far from all CoNLL-U files found in the wild follow the CoNLL-U format specification. CoNLL-U tries to parse even files that are malformed according to the specification, but sometimes that doesn't work. For those situations you can change how conllu parses your files.
-
-A normal CoNLL-U file consists of a specific set of fields (id, form, lemma, and so on...). Let's walk through how to parse a custom format using the three options `fields`, `field_parsers`, `metadata_parsers`. Here's the custom format we'll use.
-
-```python
->>> data = """
-... # tagset = TAG1|TAG2|TAG3|TAG4
-... # sentence-123
-... 1   My       TAG1|TAG2
-... 2   custom   TAG3
-... 3   format   TAG4
-...
-... """
-```
-
-Now, let's parse this with the the default settings, and look specifically at the first token to see how it was parsed.
-
-```python
->>> sentences = parse(data)
->>> sentences[0][0]
-{'id': 1, 'form': 'My', 'lemma': 'TAG1|TAG2'}
-```
-
-The parser has assumed (incorrectly) that the third field must the the default ´lemma´ field and parsed it as such. Let's customize this so the parser gets the name right, by setting the `fields` parameter when calling parse.
-
-```python
->>> sentences = parse(data, fields=["id", "form", "tag"])
->>> sentences[0][0]
-{'id': 1, 'form': 'My', 'tag': 'TAG1|TAG2'}
-```
-
-The only difference is that you now get the correct field name back when parsing. Now let's say you want those two tags returned as a list instead of as a string. This can be done using the `field_parsers` argument.
-
-```python
->>> split_func = lambda line, i: line[i].split("|")
->>> sentences = parse(data, fields=["id", "form", "tag"], field_parsers={"tag": split_func})
->>> sentences[0][0]
-{'id': 1, 'form': 'My', 'tag': ['TAG1', 'TAG2']}
-```
-
-That's much better! `field_parsers` specifies a mapping from a field name, to a function that can parse that field. In our case, we specify that the field with custom logic is `"tag"` and that the function to handle it is `split_func`. Each field_parser gets sent two parameters:
-
-* `line`: The whole list of values from this line, split on whitespace. The reason you get the full line is so you can merge several tokens into one using a field_parser if you want.
-* `i`: The current location in the line where you currently are. Most often, you'll use `line[i]` to get the current value.
-
-In our case, we return `line[i].split("|")`, which returns a list like we want.
-
-Let's look at the metadata in this example.
-
-```text
-# tagset = TAG1|TAG2|TAG3|TAG4
-# sentence-123
-```
-
-None of these values are valid in CoNLL-U, but since the first line follows the key-value format of other (valid) fields, conllu will parse it anyway:
-
-```python
->>> sentences = parse(data)
->>> sentences[0].metadata
-{'tagset': 'TAG1|TAG2|TAG3|TAG4'}
-```
-
-Let's return this as a list using the `metadata_parsers` parameter.
-
-```python
->>> sentences = parse(data, metadata_parsers={"tagset": lambda key, value: (key, value.split("|"))})
->>> sentences[0].metadata
-{'tagset': ['TAG1', 'TAG2', 'TAG3', 'TAG4']}
-```
-
-A metadata parser behaves similarily to a field parser, but since most comments you'll see will be of the form "key = value" these values will be parsed and cleaned first, and then sent to your custom metadata_parser. Here we just take the value, and split it on "|", and return a list back. And lo and behold, we get what we wanted!
-
-Now, let's deal with the "sentence-123" comment. Specifying another metadata_parser won't work, because this is an ID that will be different for each sentence. Instead, let's use a special metadata parser, called `__fallback__`.
-
-```python
->>> sentences = parse(data, metadata_parsers={
-...    "tagset": lambda key, value: (key, value.split("|")),
-...    "__fallback__": lambda key, value: ("sentence-id", key)
-... })
->>> sentences[0].metadata
-{
-    'tagset': ['TAG1', 'TAG2', 'TAG3', 'TAG4'],
-    'sentence-id': 'sentence-123'
-}
-```
-
-Just what we wanted! `__fallback__` gets called any time none of the other metadata_parsers match, and just like the others, it gets sent the key and value of the current line. In our case, the line contains no "=" to split on, so key will be "sentence-123" and value will be empty. We can return whatever we want here, but let's just say we want to call this field "sentence-id" so we return that as the key, and "sentence-123" as our value.
-
-Finally, consider an even trickier case.
-
-```python
->>> data = """
-... # id=1-document_id=36:1047-span=1
-... 1   My       TAG1|TAG2
-... 2   custom   TAG3
-... 3   format   TAG4
-...
-... """
-```
-
-This is actually three different comments, but somehow they are separated by "-" instead of on their own lines. To handle this, we get to use the ability of a metadata_parser to return multiple matches from a single line.
-
-```python
->>> sentences = parse(data, metadata_parsers={
-...    "__fallback__": lambda key, value: [pair.split("=") for pair in (key + "=" + value).split("-")]
-... })
->>> sentences[0].metadata
-{
-    'id': '1',
-    'document_id': '36:1047',
-    'span': '1'
-}
-```
-
-Our fallback parser returns a **list** of matches, one per pair of metadata comments we find. The `key + "=" + value` trick is needed since by default conllu assumes that this is a valid comment, so `key` is "id" and `value` is everything after the first "=", `1-document_id=36:1047-span=1` (note the missing "id=" in the beginning). We need to add it back before splitting on "-".
-
-And that's it! Using these tricks you should be able to parse all the strange files you stumble into.
-
-## Develop locally and run the tests
-
-1. Make a fork of the repository to your own GitHub account.
-
-2. Clone the repository locally on your computer:
-    ```bash
-    git clone git@github.com:YOURUSERNAME/conllu.git conllu
-    cd conllu
-    ```
-
-3. Install the library used for running the tests:
-    ```bash
-    pip install tox
-    ```
-
-4. Now you can run the tests:
-    ```bash
-    tox
-    ```
-    This runs tox across all supported versions of Python, and also runs checks for code-coverage, syntax errors, and how imports are sorted.
-
-4. (Alternative) If you just have one version of python installed, and don't want to go through the hassle of installing multiple version of python (hint: Install pyenv and pyenv-tox), **it's fine to run tox with just one version of python**:
-
-    ```bash
-    tox -e py36
-    ```
-
-5. Make a pull request. Here's a [good guide on PRs from GitHub](https://help.github.com/articles/creating-a-pull-request-from-a-fork/).
-
-Thanks for helping conllu become a better library!
+Metadata-Version: 2.1
+Name: conllu
+Version: 4.5.3
+Summary: CoNLL-U Parser parses a CoNLL-U formatted string into a nested python dictionary
+Home-page: https://github.com/EmilStenstrom/conllu/
+Author: Emil Stenström
+Author-email: emil@emilstenstrom.se
+License: MIT License
+Keywords: conllu,conll,conll-u,parser,nlp
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# CoNLL-U Parser
+
+**CoNLL-U Parser** parses a [CoNLL-U formatted](http://universaldependencies.org/format.html) string into a nested python dictionary. CoNLL-U is often the output of natural language processing tasks.
+
+## Why should you use conllu?
+
+- It's simple. ~300 lines of code.
+- It has no dependencies
+- Full typing support so your editor can do autocompletion
+- Nice set of tests with CI setup: [![Build](https://github.com/EmilStenstrom/conllu/workflows/Run%20tests%20for%20all%20supported%20python%20versions/badge.svg)](https://github.com/EmilStenstrom/conllu/actions?query=workflow%3A%22Run+tests+for+all+supported+python+versions%22)
+- It has 100% test branch coverage (and has undergone [mutation testing](https://github.com/boxed/mutmut/))
+- It has [![lots of downloads](http://pepy.tech/badge/conllu)](http://pepy.tech/project/conllu)
+
+## Installation
+
+Note: As of conllu 4.0, Python 3.6 is required to install conllu. See [Notes on updating from 3.0 to 4.0](#notes-on-updating-from-30-to-40)
+
+```bash
+pip install conllu
+```
+
+Or, if you are using [conda](https://conda.io/docs/):
+
+```bash
+conda install -c conda-forge conllu
+```
+
+## Notes on updating from 3.0 to 4.0
+
+Conllu version 4.0 drops support for Python 2 and all versions of earlier than Python 3.6. If you need support for older versions of python, you can always pin your install to an old version of conllu. You can install it with `pip install conllu==3.1.1`.
+
+## Notes on updating from 2.0 to 3.0
+
+The Universal dependencies 2.0 release changed two of the field names from xpostag -> xpos and upostag -> upos. Version 3.0 of conllu handles this by aliasing the previous names to the new names. This means you can use xpos/upos or xpostag/upostag, they will both return the same thing. This does change the public API slightly, so I've upped the major version to 3.0, but I've taken care to ensure you most likely DO NOT have to update your code when you update to 3.0.
+
+## Notes on updating from 0.1 to 1.0
+
+I don't like breaking backwards compatibility, but to be able to add new features I felt I had to. This means that updating from 0.1 to 1.0 *might* require code changes. Here's a guide on [how to upgrade to 1.0
+](https://github.com/EmilStenstrom/conllu/wiki/Migrating-from-0.1-to-1.0).
+
+## Example usage
+
+At the top level, conllu provides two methods, `parse` and `parse_tree`. The first one parses sentences and returns a flat list. The other returns a nested tree structure. Let's go through them one by one.
+
+## Use parse() to parse into a list of sentences
+
+```python
+>>> from conllu import parse
+>>> 
+>>> data = """
+... # text = The quick brown fox jumps over the lazy dog.
+... 1   The     the    DET    DT   Definite=Def|PronType=Art   4   det     _   _
+... 2   quick   quick  ADJ    JJ   Degree=Pos                  4   amod    _   _
+... 3   brown   brown  ADJ    JJ   Degree=Pos                  4   amod    _   _
+... 4   fox     fox    NOUN   NN   Number=Sing                 5   nsubj   _   _
+... 5   jumps   jump   VERB   VBZ  Mood=Ind|Number=Sing|Person=3|Tense=Pres|VerbForm=Fin   0   root    _   _
+... 6   over    over   ADP    IN   _                           9   case    _   _
+... 7   the     the    DET    DT   Definite=Def|PronType=Art   9   det     _   _
+... 8   lazy    lazy   ADJ    JJ   Degree=Pos                  9   amod    _   _
+... 9   dog     dog    NOUN   NN   Number=Sing                 5   nmod    _   SpaceAfter=No
+... 10  .       .      PUNCT  .    _                           5   punct   _   _
+...
+... """
+```
+
+Now you have the data in a variable called `data`. Let's parse it:
+
+```python
+>>> sentences = parse(data)
+>>> sentences
+[TokenList<The, quick, brown, fox, jumps, over, the, lazy, dog, ., metadata={text: "The quick brown fox jumps over the lazy dog."}>]
+```
+
+<blockquote>
+
+**Advanced usage**: If you have many sentences (say over a megabyte) to parse at once, you can avoid loading them into memory at once by using `parse_incr()` instead of `parse`. It takes an opened file, and returns a generator instead of the list directly, so you need to either iterate over it, or call list() to get the TokenLists out. Here's how you would use it:
+
+```python
+from io import open
+from conllu import parse_incr
+
+data_file = open("huge_file.conllu", "r", encoding="utf-8")
+for tokenlist in parse_incr(data_file):
+    print(tokenlist)
+```
+
+For most files, `parse` works fine.
+</blockquote>
+
+Since one CoNLL-U file usually contains multiple sentences, `parse()` always returns a list of sentences. Each sentence is represented by a TokenList.
+
+```python
+>>> sentence = sentences[0]
+>>> sentence
+TokenList<The, quick, brown, fox, jumps, over, the, lazy, dog, ., metadata={text: "The quick brown fox jumps over the lazy dog."}>
+```
+
+The TokenList supports indexing, so you can get the first token, represented by an ordered dictionary, like this:
+
+```python
+>>> token = sentence[0]
+>>> token
+{'id': 1,
+     'form': 'The',
+     'lemma': 'the',
+     ...}
+>>> token["form"]
+'The'
+```
+
+### New in conllu 2.0: `filter()` a TokenList
+
+```python
+>>> sentence = sentences[0]
+>>> sentence
+TokenList<The, quick, brown, fox, jumps, over, the, lazy, dog, ., metadata={text: "The quick brown fox jumps over the lazy dog."}>
+>>> sentence.filter(form="quick")
+TokenList<quick>
+```
+
+By using `filter(field1__field2=value)` you can filter based on subelements further down in a parsed token.
+
+```python
+>>> sentence.filter(feats__Degree="Pos")
+TokenList<quick, brown, lazy>
+```
+
+Filters can also be chained (meaning you can do `sentence.filter(...).filter(...)`), and filtering on multiple properties at the same time (`sentence.filter(field1=value1, field2=value2)`) means that ALL properties must match.
+
+#### New in conllu 4.3: `filter()` a TokenList by lambda
+
+You can also filter using a lambda function as value. This is useful if you, for instance, would like to filter out only tokens with integer ID:s:
+
+```python
+>>> from conllu.models import TokenList, Token
+>>> sentence2 = TokenList([
+...    Token(id=(1, "-", 2), form="It's"),
+...    Token(id=1, form="It"),
+...    Token(id=2, form="is"),
+... ])
+>>> sentence2
+TokenList<It's, It, is>
+>>> sentence2.filter(id=lambda x: type(x) is int)
+TokenList<It, is>
+```
+
+### Writing data back to a TokenList
+
+If you want to change your CoNLL-U file, there are a couple of convenience methods to know about.
+
+You can add a new token by simply appending a dictionary with the fields you want to a TokenList:
+
+```python
+>>> sentence3 = TokenList([
+...    {"id": 1, "form": "Lazy"},
+...    {"id": 2, "form": "fox"},
+... ])
+>>> sentence3
+TokenList<Lazy, fox>
+>>> sentence3.append({"id": 3, "form": "box"})
+>>> sentence3
+TokenList<Lazy, fox, box>
+```
+
+Changing a sentence just means indexing into it, and setting a value to what you want:
+
+```python
+>>> sentence4 = TokenList([
+...    {"id": 1, "form": "Lazy"},
+...    {"id": 2, "form": "fox"},
+... ])
+>>> sentence4[1]["form"] = "crocodile"
+>>> sentence4
+TokenList<Lazy, crocodile>
+>>> sentence4[1] = {"id": 2, "form": "elephant"}
+>>> sentence4
+TokenList<Lazy, elephant>
+```
+
+If you omit a field when passing in a dict, conllu will fill in a "_" for those values.
+
+```python
+>>> sentences = parse("1  The")
+>>> sentences[0].append({"id": 2})
+>>> sentences[0]
+TokenList<The, _>
+```
+
+### Parse metadata from a CoNLL-U file
+
+Each sentence can also have metadata in the form of comments before the sentence starts. This is available in a property on the TokenList called `metadata`.
+
+```python
+>>> sentence.metadata
+{'text': 'The quick brown fox jumps over the lazy dog.'}
+```
+
+### Turn a TokenList back into CoNLL-U
+
+If you ever want to get your CoNLL-U formated text back (maybe after changing something?), use the `serialize()` method:
+
+```python
+>>> print(sentence.serialize())
+# text = The quick brown fox jumps over the lazy dog.
+1   The     the     DET    DT   Definite=Def|PronType=Art   4   det    _   _
+2   quick   quick   ADJ    JJ   Degree=Pos                  4   amod   _   _
+3   brown   brown   ADJ    JJ   Degree=Pos                  4   amod   _   _
+4   fox     fox     NOUN   NN   Number=Sing                 5   nsubj  _   _
+5   jumps   jump    VERB   VBZ  Mood=Ind|Number=Sing|Person=3|Tense=Pres|VerbForm=Fin   0   root   _   _
+6   over    over    ADP    IN   _                           9   case   _   _
+7   the     the     DET    DT   Definite=Def|PronType=Art   9   det    _   _
+8   lazy    lazy    ADJ    JJ   Degree=Pos                  9   amod   _   _
+9   dog     dog     NOUN   NN   Number=Sing                 5   nmod   _   SpaceAfter=No
+10  .       .       PUNCT  .    _                           5   punct  _   _
+```
+
+### Turn a TokenList into a TokenTree (see below)
+
+You can also convert a TokenList to a TokenTree by using `to_tree`:
+
+```python
+>>> sentence.to_tree()
+TokenTree<token={id=5, form=jumps}, children=[...]>
+```
+
+That's it!
+
+## Use parse_tree() to parse into a list of dependency trees
+
+Sometimes you're interested in the tree structure that hides in the `head` column of a CoNLL-U file. When this is the case, use `parse_tree` to get a nested structure representing the sentence.
+
+```python
+>>> from conllu import parse_tree
+>>> sentences = parse_tree(data)
+>>> sentences
+[TokenTree<...>]
+```
+
+<blockquote>
+
+**Advanced usage**: If you have many sentences (say over a megabyte) to parse at once, you can avoid loading them into memory at once by using `parse_tree_incr()` instead of `parse_tree`. It takes an opened file, and returns a generator instead of the list directly, so you need to either iterate over it, or call list() to get the TokenTrees out. Here's how you would use it:
+
+```python
+from io import open
+from conllu import parse_tree_incr
+
+data_file = open("huge_file.conllu", "r", encoding="utf-8")
+for tokentree in parse_tree_incr(data_file):
+    print(tokentree)
+```
+
+</blockquote>
+
+Since one CoNLL-U file usually contains multiple sentences, `parse_tree()` always returns a list of sentences. Each sentence is represented by a TokenTree.
+
+```python
+>>> root = sentences[0]
+>>> root
+TokenTree<token={id=5, form=jumps}, children=[...]>
+```
+
+To quickly visualize the tree structure you can call `print_tree` on a TokenTree.
+
+```python
+>>> root.print_tree()
+(deprel:root) form:jumps lemma:jump upos:VERB [5]
+    (deprel:nsubj) form:fox lemma:fox upos:NOUN [4]
+        (deprel:det) form:The lemma:the upos:DET [1]
+        (deprel:amod) form:quick lemma:quick upos:ADJ [2]
+        (deprel:amod) form:brown lemma:brown upos:ADJ [3]
+    (deprel:nmod) form:dog lemma:dog upos:NOUN [9]
+        (deprel:case) form:over lemma:over upos:ADP [6]
+        (deprel:det) form:the lemma:the upos:DET [7]
+        (deprel:amod) form:lazy lemma:lazy upos:ADJ [8]
+    (deprel:punct) form:. lemma:. upos:PUNCT [10]
+```
+
+To access the token corresponding to the current node in the tree, use `token`:
+
+```python
+>>> root.token
+{
+    'id': 5,
+    'form': 'jumps',
+    'lemma': 'jump',
+    ...
+}
+```
+
+To start walking down the children of the current node, use the children attribute:
+
+```python
+>>> children = root.children
+>>> children
+[
+    TokenTree<token={id=4, form=fox}, children=[...]>,
+    TokenTree<token={id=9, form=dog}, children=[...]>,
+    TokenTree<token={id=10, form=.}, children=None>
+]
+```
+
+Just like with `parse()`, if a sentence has metadata it is available in a property on the TokenTree root called `metadata`.
+
+```python
+>>> root.metadata
+{'text': 'The quick brown fox jumps over the lazy dog.'}
+```
+
+If you ever want to get your CoNLL-U formated text back (maybe after changing something?), use the `serialize()` method:
+
+```python
+>>> print(root.serialize())
+# text = The quick brown fox jumps over the lazy dog.
+1   The     the    DET    DT   Definite=Def|PronType=Art   4   det     _   _
+2   quick   quick  ADJ    JJ   Degree=Pos                  4   amod    _   _
+...
+```
+
+If you want to write it back to a file, you can use something like this:
+
+```python
+>>> from conllu import parse_tree
+>>> sentences = parse_tree(data)
+>>> 
+>>> # Make some change to sentences here
+>>> 
+>>> with open('file-to-write-to', 'w') as f:
+...     f.writelines([sentence.serialize() + "\n" for sentence in sentences])
+```
+
+## Customizing parsing to handle strange variations of CoNLL-U
+
+Far from all CoNLL-U files found in the wild follow the CoNLL-U format specification. CoNLL-U tries to parse even files that are malformed according to the specification, but sometimes that doesn't work. For those situations you can change how conllu parses your files.
+
+A normal CoNLL-U file consists of a specific set of fields (id, form, lemma, and so on...). Let's walk through how to parse a custom format using the three options `fields`, `field_parsers`, `metadata_parsers`. Here's the custom format we'll use.
+
+```python
+>>> data = """
+... # tagset = TAG1|TAG2|TAG3|TAG4
+... # sentence-123
+... 1   My       TAG1|TAG2
+... 2   custom   TAG3
+... 3   format   TAG4
+...
+... """
+```
+
+Now, let's parse this with the the default settings, and look specifically at the first token to see how it was parsed.
+
+```python
+>>> sentences = parse(data)
+>>> sentences[0][0]
+{'id': 1, 'form': 'My', 'lemma': 'TAG1|TAG2'}
+```
+
+The parser has assumed (incorrectly) that the third field must the the default ´lemma´ field and parsed it as such. Let's customize this so the parser gets the name right, by setting the `fields` parameter when calling parse.
+
+```python
+>>> sentences = parse(data, fields=["id", "form", "tag"])
+>>> sentences[0][0]
+{'id': 1, 'form': 'My', 'tag': 'TAG1|TAG2'}
+```
+
+The only difference is that you now get the correct field name back when parsing. Now let's say you want those two tags returned as a list instead of as a string. This can be done using the `field_parsers` argument.
+
+```python
+>>> split_func = lambda line, i: line[i].split("|")
+>>> sentences = parse(data, fields=["id", "form", "tag"], field_parsers={"tag": split_func})
+>>> sentences[0][0]
+{'id': 1, 'form': 'My', 'tag': ['TAG1', 'TAG2']}
+```
+
+That's much better! `field_parsers` specifies a mapping from a field name, to a function that can parse that field. In our case, we specify that the field with custom logic is `"tag"` and that the function to handle it is `split_func`. Each field_parser gets sent two parameters:
+
+* `line`: The whole list of values from this line, split on whitespace. The reason you get the full line is so you can merge several tokens into one using a field_parser if you want.
+* `i`: The current location in the line where you currently are. Most often, you'll use `line[i]` to get the current value.
+
+In our case, we return `line[i].split("|")`, which returns a list like we want.
+
+Let's look at the metadata in this example.
+
+```text
+# tagset = TAG1|TAG2|TAG3|TAG4
+# sentence-123
+```
+
+None of these values are valid in CoNLL-U, but since the first line follows the key-value format of other (valid) fields, conllu will parse it anyway:
+
+```python
+>>> sentences = parse(data)
+>>> sentences[0].metadata
+{'tagset': 'TAG1|TAG2|TAG3|TAG4'}
+```
+
+Let's return this as a list using the `metadata_parsers` parameter.
+
+```python
+>>> sentences = parse(data, metadata_parsers={"tagset": lambda key, value: (key, value.split("|"))})
+>>> sentences[0].metadata
+{'tagset': ['TAG1', 'TAG2', 'TAG3', 'TAG4']}
+```
+
+A metadata parser behaves similarily to a field parser, but since most comments you'll see will be of the form "key = value" these values will be parsed and cleaned first, and then sent to your custom metadata_parser. Here we just take the value, and split it on "|", and return a list back. And lo and behold, we get what we wanted!
+
+Now, let's deal with the "sentence-123" comment. Specifying another metadata_parser won't work, because this is an ID that will be different for each sentence. Instead, let's use a special metadata parser, called `__fallback__`.
+
+```python
+>>> sentences = parse(data, metadata_parsers={
+...    "tagset": lambda key, value: (key, value.split("|")),
+...    "__fallback__": lambda key, value: ("sentence-id", key)
+... })
+>>> sentences[0].metadata
+{
+    'tagset': ['TAG1', 'TAG2', 'TAG3', 'TAG4'],
+    'sentence-id': 'sentence-123'
+}
+```
+
+Just what we wanted! `__fallback__` gets called any time none of the other metadata_parsers match, and just like the others, it gets sent the key and value of the current line. In our case, the line contains no "=" to split on, so key will be "sentence-123" and value will be empty. We can return whatever we want here, but let's just say we want to call this field "sentence-id" so we return that as the key, and "sentence-123" as our value.
+
+Finally, consider an even trickier case.
+
+```python
+>>> data = """
+... # id=1-document_id=36:1047-span=1
+... 1   My       TAG1|TAG2
+... 2   custom   TAG3
+... 3   format   TAG4
+...
+... """
+```
+
+This is actually three different comments, but somehow they are separated by "-" instead of on their own lines. To handle this, we get to use the ability of a metadata_parser to return multiple matches from a single line.
+
+```python
+>>> sentences = parse(data, metadata_parsers={
+...    "__fallback__": lambda key, value: [pair.split("=") for pair in (key + "=" + value).split("-")]
+... })
+>>> sentences[0].metadata
+{
+    'id': '1',
+    'document_id': '36:1047',
+    'span': '1'
+}
+```
+
+Our fallback parser returns a **list** of matches, one per pair of metadata comments we find. The `key + "=" + value` trick is needed since by default conllu assumes that this is a valid comment, so `key` is "id" and `value` is everything after the first "=", `1-document_id=36:1047-span=1` (note the missing "id=" in the beginning). We need to add it back before splitting on "-".
+
+And that's it! Using these tricks you should be able to parse all the strange files you stumble into.
+
+## Develop locally and run the tests
+
+1. Make a fork of the repository to your own GitHub account.
+
+2. Clone the repository locally on your computer:
+    ```bash
+    git clone git@github.com:YOURUSERNAME/conllu.git conllu
+    cd conllu
+    ```
+
+3. Install the library used for running the tests:
+    ```bash
+    pip install tox
+    ```
+
+4. Now you can run the tests:
+    ```bash
+    tox
+    ```
+    This runs tox across all supported versions of Python, and also runs checks for code-coverage, syntax errors, and how imports are sorted.
+
+4. (Alternative) If you just have one version of python installed, and don't want to go through the hassle of installing multiple version of python (hint: Install pyenv and pyenv-tox), **it's fine to run tox with just one version of python**:
+
+    ```bash
+    tox -e py36
+    ```
+
+5. Make a pull request. Here's a [good guide on PRs from GitHub](https://help.github.com/articles/creating-a-pull-request-from-a-fork/).
+
+Thanks for helping conllu become a better library!
```

### Comparing `conllu-4.5.2/conllu/models.py` & `conllu-4.5.3/conllu/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,387 +1,387 @@
-import typing as T
-from collections import defaultdict
-from collections.abc import Mapping
-
-from conllu.exceptions import ParseException
-from conllu.serializer import serialize
-
-DEFAULT_EXCLUDE_FIELDS = ('id', 'deprel', 'xpos', 'feats', 'head', 'deps', 'misc')
-
-if T.TYPE_CHECKING:
-    class SupportsIndex(T.Protocol):
-        def __index__(self) -> int:
-            pass
-
-    class SupportsNext(T.Protocol):
-        def __next__(self) -> int:
-            pass
-
-class Metadata(dict):
-    pass
-
-class Token(dict):
-    MAPPING = {
-        "upostag": "upos",
-        "xpostag": "xpos",
-        "upos": "upostag",
-        "xpos": "xpostag",
-    }
-
-    def get(self, key: str, default: T.Optional[T.Any] = None) -> T.Any:
-        if key not in self and key in self.MAPPING:
-            key = self.MAPPING[key]
-
-        return super(Token, self).get(key, default)
-
-    def __missing__(self, key: str) -> T.Any:
-        if key in self.MAPPING:
-            return self.get(self.MAPPING[key])
-
-        raise KeyError("'" + key + "'")
-
-    def __str__(self) -> str:
-        if 'form' in self:
-            return self['form']
-
-        if 'id' in self:
-            return f"id={self['id']}"
-
-        return ''
-
-class TokenList(T.List[Token]):
-    def __init__(
-        self,
-        tokens: T.Iterable[Token] = None,
-        metadata: Metadata = None,
-        default_fields: T.Optional[T.Iterable[str]] = None,
-    ):
-        tokens = tokens or []
-
-        if not isinstance(tokens, list):
-            raise ParseException("Can't create TokenList, tokens is not a list.")
-
-        if len(tokens) > 0 and not isinstance(tokens[0], Token):
-            tokens = [Token(token) for token in tokens]
-
-        super(TokenList, self).__init__(tokens)
-
-        self.metadata = metadata or Metadata()
-        self.default_fields = default_fields
-
-    def __repr__(self) -> str:
-        tokens = ', '.join(str(token) for token in self)
-        if not self.metadata:
-            return f'TokenList<{tokens}>'
-        else:
-            metadata = ', '.join(f"{key}: \"{value}\"" for key, value in self.metadata.items())
-            return f'TokenList<{tokens}, metadata={{{metadata}}}>'
-
-    def __eq__(self, other: T.Any) -> bool:
-        if not isinstance(other, TokenList):
-            other = TokenList(other)
-
-        return super(TokenList, self).__eq__(other) and self.metadata == other.metadata
-
-    def __ne__(self, other: T.Any) -> bool:
-        return not self == other
-
-    def clear(self) -> None:
-        super(TokenList, self).clear()
-        self.metadata = Metadata()
-        self.default_fields = None
-
-    def copy(self) -> 'TokenList':
-        tokens_copy = super().copy()
-        return TokenList(tokens_copy, self.metadata, self.default_fields)
-
-    def extend(self, iterable: T.Union['TokenList', T.Iterable[Token]]) -> None:
-        if not isinstance(iterable, TokenList):
-            iterable = TokenList(iterable)
-
-        super(TokenList, self).extend(iterable)
-
-        self.metadata.update(iterable.metadata)
-
-    def _dict_to_token_and_set_defaults(self, token: T.Union[dict, Token]) -> Token:
-        if not isinstance(token, Token):
-            token = Token(token)
-
-        if self.default_fields:
-            for field in self.default_fields:
-                if field not in token:
-                    token[field] = "_"
-
-        return token
-
-    def append(self, token: T.Union[dict, Token]) -> None:
-        token = self._dict_to_token_and_set_defaults(token)
-        super(TokenList, self).append(token)
-
-    def insert(self, i: 'SupportsIndex', token: T.Union[dict, Token]) -> None:
-        token = self._dict_to_token_and_set_defaults(token)
-        super(TokenList, self).insert(i, token)
-
-    @T.overload
-    def __setitem__(self, key: 'SupportsIndex', tokens: T.Union[dict, Token]) -> None: ...  # noqa, pragma: no cover
-
-    @T.overload
-    def __setitem__(self, key: slice, tokens: T.Union[T.Iterable[T.Union[dict, Token]], 'TokenList']) -> None: ...  # noqa, pragma: no cover
-
-    def __setitem__(self, key, tokens):  # noqa: F811
-        if isinstance(key, slice):
-            tokens = [self._dict_to_token_and_set_defaults(token) for token in tokens]
-            super(TokenList, self).__setitem__(key, tokens)
-        else:
-            token = tokens
-            token = self._dict_to_token_and_set_defaults(token)
-            super(TokenList, self).__setitem__(key, token)
-
-    def serialize(self) -> str:
-        return serialize(self)
-
-    @staticmethod
-    def head_to_token(sentence: 'TokenList') -> T.Dict[int, T.List[Token]]:
-        if not sentence:
-            raise ParseException("Can't parse tree, need a tokenlist as input.")
-
-        if "head" not in sentence[0]:
-            raise ParseException("Can't parse tree, missing 'head' field.")
-
-        head_indexed = defaultdict(list)
-        for token in sentence:
-            # Filter out range and decimal ID:s before building tree
-            if "id" in token and not isinstance(token["id"], int):
-                continue
-
-            # Filter out tokens with negative head, they are sometimes used to
-            # specify tokens which should not be included in tree
-            # Also filter out those that have no head, just exclude them from the tree.
-            if (token.get("head") is None) or token["head"] < 0:
-                continue
-
-            head_indexed[token["head"]].append(token)
-
-        if len(head_indexed[0]) == 0:
-            raise ParseException("Found no head node, can't build tree")
-
-        return head_indexed
-
-    def to_tree(self) -> 'TokenTree':
-        def _create_tree(head_to_token_mapping: T.Dict[int, T.List[Token]], id_: int = 0) -> T.List['TokenTree']:
-            return [
-                TokenTree(child, _create_tree(head_to_token_mapping, child["id"]))
-                for child in head_to_token_mapping[id_]
-            ]
-
-        head_indexed = self.head_to_token(self)
-        if len(head_indexed[0]) > 1:
-            # Introduce fake root node that multiple root nodes can have a single parent
-            head_indexed[-1] = [Token(
-                [("id", 0), ("form", "_"), ("deprel", "root")]
-            )]
-            root = _create_tree(head_indexed, -1)[0]
-        else:
-            root = _create_tree(head_indexed, 0)[0]
-
-        root.set_metadata(self.metadata)
-        return root
-
-    def filter(self, **kwargs: T.Any) -> 'TokenList':
-        tokens: T.Iterable[Token] = self.copy()
-
-        for query, value in kwargs.items():
-            filtered_tokens = []
-            for token in tokens:
-                if callable(value) and value(traverse_dict(token, query)) is True:
-                    filtered_tokens.append(token)
-                else:
-                    if traverse_dict(token, query) == value:
-                        filtered_tokens.append(token)
-
-            tokens = filtered_tokens
-
-        return TokenList(tokens)
-
-
-_T = T.TypeVar("_T")
-def traverse_dict(obj: T.Mapping[str, _T], query: str) -> T.Optional[_T]:
-    """
-        Get elements inside a nested dict, based on a dict query. The query is defined by a
-        string separated by '__'. traverse_dict(foo, 'a__b__c') is roughly equivalent to foo[a][b][c] but
-        will short circuit to return None if something on the query is None.
-    """
-    query_split = query.split('__')
-
-    cur_obj: T.Optional[T.Union[_T, T.Mapping[str, _T]]] = obj
-    for name in query_split:
-        assert isinstance(cur_obj, Mapping)  # help mypy
-        cur_obj = cur_obj.get(name, None)
-        if cur_obj is None:
-            return None
-    assert not isinstance(cur_obj, Mapping)  # help mypy
-    return cur_obj
-
-
-class TokenTree(object):
-    token: Token
-    children: T.List['TokenTree']
-    metadata: T.Optional[Metadata]
-
-    def __init__(self, token: Token, children: T.List['TokenTree'], metadata: T.Optional[Metadata] = None):
-        self.token = token
-        self.children = children
-        self.metadata = metadata
-
-    def set_metadata(self, metadata: T.Optional[Metadata]) -> None:
-        self.metadata = metadata
-
-    def __repr__(self) -> str:
-        return 'TokenTree<' + \
-            'token={id=' + str(self.token['id']) + ', form=' + str(self.token['form']) + '}, ' + \
-            'children=' + ('[...]' if self.children else 'None') + \
-            '>'
-
-    def __eq__(self, other: T.Any) -> bool:
-        if isinstance(other, TokenTree):
-            return self.token == other.token and self.children == other.children \
-                and self.metadata == other.metadata
-        return False
-
-    def serialize(self) -> str:
-        if not self.token or "id" not in self.token:
-            raise ParseException("Could not serialize tree, missing 'id' field.")
-
-        def flatten_tree(root_token: TokenTree, token_list: T.List[Token] = []) -> T.List[Token]:
-            token_list.append(root_token.token)
-
-            for child_token in root_token.children:
-                flatten_tree(child_token, token_list)
-
-            return token_list
-
-        tokens = flatten_tree(self)
-        tokens = sorted(tokens, key=lambda t: t['id'])
-        tokenlist = TokenList(tokens, self.metadata)
-
-        return serialize(tokenlist)
-
-    def print_tree(self, depth: int = 0, indent: int = 4,
-                   exclude_fields: T.Sequence[str] = DEFAULT_EXCLUDE_FIELDS) -> None:
-        if not self.token:
-            raise ParseException("Can't print, token is None.")
-
-        if "deprel" not in self.token or "id" not in self.token:
-            raise ParseException("Can't print, token is missing either the id or deprel fields.")
-
-        relevant_data = self.token.copy()
-        for key in exclude_fields:
-            if key in relevant_data:
-                del relevant_data[key]
-
-        node_repr = ' '.join([
-            '{key}:{value}'.format(key=key, value=value)
-            for key, value in relevant_data.items()
-        ])
-
-        print(' ' * indent * depth + '(deprel:{deprel}) {node_repr} [{idx}]'.format(
-            deprel=self.token['deprel'],
-            node_repr=node_repr,
-            idx=self.token['id'],
-        ))
-        for child in self.children:
-            child.print_tree(depth=depth + 1, indent=indent, exclude_fields=exclude_fields)
-
-class SentenceList(T.List[TokenList]):
-    def __init__(
-        self,
-        sentences: T.Iterable[TokenList] = None,
-        metadata: Metadata = None,
-    ):
-        sentences = sentences or []
-
-        if hasattr(sentences, "__next__"):
-            sentences = list(sentences)
-
-        if not isinstance(sentences, list):
-            raise ParseException("Can't create SentenceList, sentences is not a list.")
-
-        super(SentenceList, self).__init__(sentences)
-
-        self.metadata = metadata or Metadata()
-
-    def __repr__(self) -> str:
-        sentences = ', '.join(str(sentence) for sentence in self)
-        if not self.metadata:
-            return f'[{sentences}]'
-        else:
-            metadata = ', '.join(f"{key}: \"{value}\"" for key, value in self.metadata.items())
-            return f'SentenceList<{sentences}, metadata={{{metadata}}}>'
-
-    def __eq__(self, other: T.Any) -> bool:
-        if not isinstance(other, SentenceList):
-            other = SentenceList(other)
-
-        return super(SentenceList, self).__eq__(other) and self.metadata == other.metadata
-
-    def __ne__(self, other: T.Any) -> bool:
-        return not self == other
-
-    @T.overload
-    def __getitem__(self, key: 'SupportsIndex') -> TokenList: ...  # noqa, pragma: no cover
-
-    @T.overload
-    def __getitem__(self, key: slice) -> "SentenceList": ...  # noqa, pragma: no cover
-
-    def __getitem__(self, key):  # noqa: F811
-        if isinstance(key, slice):
-            return SentenceList(
-                sentences=super(SentenceList, self).__getitem__(key),
-                metadata=self.metadata
-            )
-        else:
-            return super(SentenceList, self).__getitem__(key)
-
-    def clear(self) -> None:
-        super(SentenceList, self).clear()
-        self.metadata = Metadata()
-
-    def copy(self) -> 'SentenceList':
-        sentences_copy = super().copy()
-        return SentenceList(sentences_copy, self.metadata)
-
-    def extend(self, iterable: T.Union['SentenceList', T.Iterable[TokenList], None]) -> None:
-        if not isinstance(iterable, SentenceList):
-            iterable = SentenceList(iterable)
-
-        super(SentenceList, self).extend(iterable)
-
-        self.metadata.update(iterable.metadata)
-
-
-class SentenceGenerator(T.Iterable[TokenList]):
-    def __init__(
-        self,
-        sentences: T.Iterator[TokenList],
-        metadata: Metadata = None,
-    ):
-        if isinstance(sentences, T.List):
-            sentences = iter(sentences)
-
-        if not isinstance(sentences, T.Iterator):
-            raise ParseException("Can't create SentenceGenerator, sentences is not an iterator.")
-
-        self.sentences = sentences
-        self.metadata = metadata or Metadata()
-
-    def __iter__(self) -> T.Iterator[TokenList]:
-        return self.sentences.__iter__()
-
-    def __next__(self) -> TokenList:
-        return self.sentences.__next__()
-
-    def __repr__(self) -> str:
-        if not self.metadata:
-            return f'SentenceGenerator<{id(self)}>'
-        else:
-            metadata = ', '.join(f"{key}: \"{value}\"" for key, value in self.metadata.items())
-            return f'SentenceGenerator<{id(self)}, metadata={{{metadata}}}>'
+import typing as T
+from collections import defaultdict
+from collections.abc import Mapping
+
+from conllu.exceptions import ParseException
+from conllu.serializer import serialize
+
+DEFAULT_EXCLUDE_FIELDS = ('id', 'deprel', 'xpos', 'feats', 'head', 'deps', 'misc')
+
+if T.TYPE_CHECKING:
+    class SupportsIndex(T.Protocol):
+        def __index__(self) -> int:
+            pass
+
+    class SupportsNext(T.Protocol):
+        def __next__(self) -> int:
+            pass
+
+class Metadata(dict):
+    pass
+
+class Token(dict):
+    MAPPING = {
+        "upostag": "upos",
+        "xpostag": "xpos",
+        "upos": "upostag",
+        "xpos": "xpostag",
+    }
+
+    def get(self, key: str, default: T.Optional[T.Any] = None) -> T.Any:
+        if key not in self and key in self.MAPPING:
+            key = self.MAPPING[key]
+
+        return super(Token, self).get(key, default)
+
+    def __missing__(self, key: str) -> T.Any:
+        if key in self.MAPPING:
+            return self.get(self.MAPPING[key])
+
+        raise KeyError("'" + key + "'")
+
+    def __str__(self) -> str:
+        if 'form' in self:
+            return self['form']
+
+        if 'id' in self:
+            return f"id={self['id']}"
+
+        return ''
+
+class TokenList(T.List[Token]):
+    def __init__(
+        self,
+        tokens: T.Optional[T.Iterable[Token]] = None,
+        metadata: T.Optional[Metadata] = None,
+        default_fields: T.Optional[T.Iterable[str]] = None,
+    ):
+        tokens = tokens or []
+
+        if not isinstance(tokens, list):
+            raise ParseException("Can't create TokenList, tokens is not a list.")
+
+        if len(tokens) > 0 and not isinstance(tokens[0], Token):
+            tokens = [Token(token) for token in tokens]
+
+        super(TokenList, self).__init__(tokens)
+
+        self.metadata = metadata or Metadata()
+        self.default_fields = default_fields
+
+    def __repr__(self) -> str:
+        tokens = ', '.join(str(token) for token in self)
+        if not self.metadata:
+            return f'TokenList<{tokens}>'
+        else:
+            metadata = ', '.join(f"{key}: \"{value}\"" for key, value in self.metadata.items())
+            return f'TokenList<{tokens}, metadata={{{metadata}}}>'
+
+    def __eq__(self, other: T.Any) -> bool:
+        if not isinstance(other, TokenList):
+            other = TokenList(other)
+
+        return super(TokenList, self).__eq__(other) and self.metadata == other.metadata
+
+    def __ne__(self, other: T.Any) -> bool:
+        return not self == other
+
+    def clear(self) -> None:
+        super(TokenList, self).clear()
+        self.metadata = Metadata()
+        self.default_fields = None
+
+    def copy(self) -> 'TokenList':
+        tokens_copy = super().copy()
+        return TokenList(tokens_copy, self.metadata, self.default_fields)
+
+    def extend(self, iterable: T.Union['TokenList', T.Iterable[Token]]) -> None:
+        if not isinstance(iterable, TokenList):
+            iterable = TokenList(iterable)
+
+        super(TokenList, self).extend(iterable)
+
+        self.metadata.update(iterable.metadata)
+
+    def _dict_to_token_and_set_defaults(self, token: T.Union[dict, Token]) -> Token:
+        if not isinstance(token, Token):
+            token = Token(token)
+
+        if self.default_fields:
+            for field in self.default_fields:
+                if field not in token:
+                    token[field] = "_"
+
+        return token
+
+    def append(self, token: T.Union[dict, Token]) -> None:
+        token = self._dict_to_token_and_set_defaults(token)
+        super(TokenList, self).append(token)
+
+    def insert(self, i: 'SupportsIndex', token: T.Union[dict, Token]) -> None:
+        token = self._dict_to_token_and_set_defaults(token)
+        super(TokenList, self).insert(i, token)
+
+    @T.overload
+    def __setitem__(self, key: 'SupportsIndex', tokens: T.Union[dict, Token]) -> None: ...  # noqa, pragma: no cover
+
+    @T.overload
+    def __setitem__(self, key: slice, tokens: T.Union[T.Iterable[T.Union[dict, Token]], 'TokenList']) -> None: ...  # noqa, pragma: no cover
+
+    def __setitem__(self, key, tokens):  # noqa: F811
+        if isinstance(key, slice):
+            tokens = [self._dict_to_token_and_set_defaults(token) for token in tokens]
+            super(TokenList, self).__setitem__(key, tokens)
+        else:
+            token = tokens
+            token = self._dict_to_token_and_set_defaults(token)
+            super(TokenList, self).__setitem__(key, token)
+
+    def serialize(self) -> str:
+        return serialize(self)
+
+    @staticmethod
+    def head_to_token(sentence: 'TokenList') -> T.Dict[int, T.List[Token]]:
+        if not sentence:
+            raise ParseException("Can't parse tree, need a tokenlist as input.")
+
+        if "head" not in sentence[0]:
+            raise ParseException("Can't parse tree, missing 'head' field.")
+
+        head_indexed = defaultdict(list)
+        for token in sentence:
+            # Filter out range and decimal ID:s before building tree
+            if "id" in token and not isinstance(token["id"], int):
+                continue
+
+            # Filter out tokens with negative head, they are sometimes used to
+            # specify tokens which should not be included in tree
+            # Also filter out those that have no head, just exclude them from the tree.
+            if (token.get("head") is None) or token["head"] < 0:
+                continue
+
+            head_indexed[token["head"]].append(token)
+
+        if len(head_indexed[0]) == 0:
+            raise ParseException("Found no head node, can't build tree")
+
+        return head_indexed
+
+    def to_tree(self) -> 'TokenTree':
+        def _create_tree(head_to_token_mapping: T.Dict[int, T.List[Token]], id_: int = 0) -> T.List['TokenTree']:
+            return [
+                TokenTree(child, _create_tree(head_to_token_mapping, child["id"]))
+                for child in head_to_token_mapping[id_]
+            ]
+
+        head_indexed = self.head_to_token(self)
+        if len(head_indexed[0]) > 1:
+            # Introduce fake root node that multiple root nodes can have a single parent
+            head_indexed[-1] = [Token(
+                [("id", 0), ("form", "_"), ("deprel", "root")]
+            )]
+            root = _create_tree(head_indexed, -1)[0]
+        else:
+            root = _create_tree(head_indexed, 0)[0]
+
+        root.set_metadata(self.metadata)
+        return root
+
+    def filter(self, **kwargs: T.Any) -> 'TokenList':
+        tokens: T.Iterable[Token] = self.copy()
+
+        for query, value in kwargs.items():
+            filtered_tokens = []
+            for token in tokens:
+                if callable(value) and value(traverse_dict(token, query)) is True:
+                    filtered_tokens.append(token)
+                else:
+                    if traverse_dict(token, query) == value:
+                        filtered_tokens.append(token)
+
+            tokens = filtered_tokens
+
+        return TokenList(tokens)
+
+
+_T = T.TypeVar("_T")
+def traverse_dict(obj: T.Mapping[str, _T], query: str) -> T.Optional[_T]:
+    """
+        Get elements inside a nested dict, based on a dict query. The query is defined by a
+        string separated by '__'. traverse_dict(foo, 'a__b__c') is roughly equivalent to foo[a][b][c] but
+        will short circuit to return None if something on the query is None.
+    """
+    query_split = query.split('__')
+
+    cur_obj: T.Optional[T.Union[_T, T.Mapping[str, _T]]] = obj
+    for name in query_split:
+        assert isinstance(cur_obj, Mapping)  # help mypy
+        cur_obj = cur_obj.get(name, None)
+        if cur_obj is None:
+            return None
+    assert not isinstance(cur_obj, Mapping)  # help mypy
+    return cur_obj
+
+
+class TokenTree(object):
+    token: Token
+    children: T.List['TokenTree']
+    metadata: T.Optional[Metadata]
+
+    def __init__(self, token: Token, children: T.List['TokenTree'], metadata: T.Optional[Metadata] = None):
+        self.token = token
+        self.children = children
+        self.metadata = metadata
+
+    def set_metadata(self, metadata: T.Optional[Metadata]) -> None:
+        self.metadata = metadata
+
+    def __repr__(self) -> str:
+        return 'TokenTree<' + \
+            'token={id=' + str(self.token['id']) + ', form=' + str(self.token['form']) + '}, ' + \
+            'children=' + ('[...]' if self.children else 'None') + \
+            '>'
+
+    def __eq__(self, other: T.Any) -> bool:
+        if isinstance(other, TokenTree):
+            return self.token == other.token and self.children == other.children \
+                and self.metadata == other.metadata
+        return False
+
+    def serialize(self) -> str:
+        if not self.token or "id" not in self.token:
+            raise ParseException("Could not serialize tree, missing 'id' field.")
+
+        def flatten_tree(root_token: TokenTree, token_list: T.List[Token] = []) -> T.List[Token]:
+            token_list.append(root_token.token)
+
+            for child_token in root_token.children:
+                flatten_tree(child_token, token_list)
+
+            return token_list
+
+        tokens = flatten_tree(self)
+        tokens = sorted(tokens, key=lambda t: t['id'])
+        tokenlist = TokenList(tokens, self.metadata)
+
+        return serialize(tokenlist)
+
+    def print_tree(self, depth: int = 0, indent: int = 4,
+                   exclude_fields: T.Sequence[str] = DEFAULT_EXCLUDE_FIELDS) -> None:
+        if not self.token:
+            raise ParseException("Can't print, token is None.")
+
+        if "deprel" not in self.token or "id" not in self.token:
+            raise ParseException("Can't print, token is missing either the id or deprel fields.")
+
+        relevant_data = self.token.copy()
+        for key in exclude_fields:
+            if key in relevant_data:
+                del relevant_data[key]
+
+        node_repr = ' '.join([
+            '{key}:{value}'.format(key=key, value=value)
+            for key, value in relevant_data.items()
+        ])
+
+        print(' ' * indent * depth + '(deprel:{deprel}) {node_repr} [{idx}]'.format(
+            deprel=self.token['deprel'],
+            node_repr=node_repr,
+            idx=self.token['id'],
+        ))
+        for child in self.children:
+            child.print_tree(depth=depth + 1, indent=indent, exclude_fields=exclude_fields)
+
+class SentenceList(T.List[TokenList]):
+    def __init__(
+        self,
+        sentences: T.Optional[T.Iterable[TokenList]] = None,
+        metadata: T.Optional[Metadata] = None,
+    ):
+        sentences = sentences or []
+
+        if hasattr(sentences, "__next__"):
+            sentences = list(sentences)
+
+        if not isinstance(sentences, list):
+            raise ParseException("Can't create SentenceList, sentences is not a list.")
+
+        super(SentenceList, self).__init__(sentences)
+
+        self.metadata = metadata or Metadata()
+
+    def __repr__(self) -> str:
+        sentences = ', '.join(str(sentence) for sentence in self)
+        if not self.metadata:
+            return f'[{sentences}]'
+        else:
+            metadata = ', '.join(f"{key}: \"{value}\"" for key, value in self.metadata.items())
+            return f'SentenceList<{sentences}, metadata={{{metadata}}}>'
+
+    def __eq__(self, other: T.Any) -> bool:
+        if not isinstance(other, SentenceList):
+            other = SentenceList(other)
+
+        return super(SentenceList, self).__eq__(other) and self.metadata == other.metadata
+
+    def __ne__(self, other: T.Any) -> bool:
+        return not self == other
+
+    @T.overload
+    def __getitem__(self, key: 'SupportsIndex') -> TokenList: ...  # noqa, pragma: no cover
+
+    @T.overload
+    def __getitem__(self, key: slice) -> "SentenceList": ...  # noqa, pragma: no cover
+
+    def __getitem__(self, key):  # noqa: F811
+        if isinstance(key, slice):
+            return SentenceList(
+                sentences=super(SentenceList, self).__getitem__(key),
+                metadata=self.metadata
+            )
+        else:
+            return super(SentenceList, self).__getitem__(key)
+
+    def clear(self) -> None:
+        super(SentenceList, self).clear()
+        self.metadata = Metadata()
+
+    def copy(self) -> 'SentenceList':
+        sentences_copy = super().copy()
+        return SentenceList(sentences_copy, self.metadata)
+
+    def extend(self, iterable: T.Union['SentenceList', T.Iterable[TokenList]]) -> None:
+        if not isinstance(iterable, SentenceList):
+            iterable = SentenceList(iterable)
+
+        super(SentenceList, self).extend(iterable)
+
+        self.metadata.update(iterable.metadata)
+
+
+class SentenceGenerator(T.Iterable[TokenList]):
+    def __init__(
+        self,
+        sentences: T.Iterator[TokenList],
+        metadata: T.Optional[Metadata] = None,
+    ):
+        if isinstance(sentences, T.List):
+            sentences = iter(sentences)
+
+        if not isinstance(sentences, T.Iterator):
+            raise ParseException("Can't create SentenceGenerator, sentences is not an iterator.")
+
+        self.sentences = sentences
+        self.metadata = metadata or Metadata()
+
+    def __iter__(self) -> T.Iterator[TokenList]:
+        return self.sentences.__iter__()
+
+    def __next__(self) -> TokenList:
+        return self.sentences.__next__()
+
+    def __repr__(self) -> str:
+        if not self.metadata:
+            return f'SentenceGenerator<{id(self)}>'
+        else:
+            metadata = ', '.join(f"{key}: \"{value}\"" for key, value in self.metadata.items())
+            return f'SentenceGenerator<{id(self)}, metadata={{{metadata}}}>'
```

### Comparing `conllu-4.5.2/conllu/parser.py` & `conllu-4.5.3/conllu/parser.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,259 +1,259 @@
-import re
-import typing as T
-
-from conllu.exceptions import ParseException
-from conllu.models import Metadata, Token, TokenList
-
-_IdType = T.Union[int, T.Tuple[int, str, int]]
-_FieldParserType = T.Callable[[T.List[str], int], T.Any]
-_MetadataParserType = T.Callable[[str, T.Optional[str]], T.Any]
-
-DEFAULT_FIELDS = ('id', 'form', 'lemma', 'upos', 'xpos', 'feats', 'head', 'deprel', 'deps', 'misc')
-DEFAULT_FIELD_PARSERS: T.Dict[str, _FieldParserType] = {
-    "id": lambda line, i: parse_id_value(line[i]),
-    "xpos": lambda line, i: parse_nullable_value(line[i]),
-    "feats": lambda line, i: parse_dict_value(line[i]),
-    "head": lambda line, i: parse_int_value(line[i]),
-    "deps": lambda line, i: parse_paired_list_value(line[i]),
-    "misc": lambda line, i: parse_dict_value(line[i]),
-}
-DEFAULT_METADATA_PARSERS: T.Dict[str, _MetadataParserType] = {
-    "newpar": lambda key, value: (key, value),
-    "newdoc": lambda key, value: (key, value),
-}
-
-def parse_conllu_plus_fields(in_file: T.TextIO,
-                             metadata_parsers: T.Optional[T.Dict[str, _MetadataParserType]] = None
-                             ) -> T.Optional[T.Sequence[str]]:
-    pos = in_file.tell()
-
-    # Get first line
-    try:
-        first_sentence = next(parse_sentences(in_file))
-        first_line = first_sentence.split("\n")[0]
-    except StopIteration:
-        first_line = ""
-
-    # parse_sentences moves to file cursor, so reset it here
-    in_file.seek(pos)
-
-    if not first_line.startswith("#"):
-        return None
-
-    tokenlist = parse_token_and_metadata(first_line, metadata_parsers=metadata_parsers)
-    metadata = tokenlist.metadata
-
-    fields = None
-    if "global.columns" in metadata and metadata["global.columns"]:
-        fields = [value.lower() for value in metadata["global.columns"].split(" ")]
-
-    return fields
-
-def parse_sentences(in_file: T.TextIO) -> T.Iterator[str]:
-    buf: T.List[str] = []
-    for line in in_file:
-        if line.strip() == "":
-            if not buf:
-                continue
-            yield "".join(buf).rstrip()
-            buf = []
-        else:
-            buf.append(line)
-    if buf:
-        yield "".join(buf).rstrip()
-
-def parse_token_and_metadata(data: str, fields: T.Optional[T.Sequence[str]] = None,
-                             field_parsers: T.Optional[T.Dict[str, _FieldParserType]] = None,
-                             metadata_parsers: T.Optional[T.Dict[str, _MetadataParserType]] = None
-                             ) -> TokenList:
-
-    if not data:
-        raise ParseException("Can't create TokenList, no data sent to constructor.")
-
-    fields = fields or DEFAULT_FIELDS
-
-    if not field_parsers:
-        field_parsers = DEFAULT_FIELD_PARSERS.copy()
-    elif sorted(field_parsers.keys()) != sorted(fields):
-        new_field_parsers = DEFAULT_FIELD_PARSERS.copy()
-        new_field_parsers.update(field_parsers)
-        field_parsers = new_field_parsers
-
-    tokens = []
-    metadata = Metadata()
-
-    for line in data.split('\n'):
-        line = line.strip()
-
-        if not line:
-            continue
-
-        if line.startswith('#'):
-            pairs = parse_comment_line(line, metadata_parsers=metadata_parsers)
-            for key, value in pairs:
-                metadata[key] = value
-        else:
-            tokens.append(parse_line(line, fields, field_parsers))
-
-    return TokenList(tokens, metadata, default_fields=fields)
-
-def parse_line(line: str,
-               fields: T.Sequence[str], field_parsers: T.Optional[T.Dict[str, _FieldParserType]] = None
-               ) -> Token:
-    # Be backwards compatible if people called parse_line without field_parsers before
-    field_parsers = field_parsers or DEFAULT_FIELD_PARSERS
-
-    # Support xpostag/upostag as aliases for xpos/upos (both ways)
-    if "xpostag" not in field_parsers and "xpos" in field_parsers:
-        field_parsers["xpostag"] = field_parsers["xpos"]
-    if "xpos" not in field_parsers and "xpostag" in field_parsers:
-        field_parsers["xpos"] = field_parsers["xpostag"]
-
-    if "upostag" not in field_parsers and "upos" in field_parsers:
-        field_parsers["upostag"] = field_parsers["upos"]
-    if "upos" not in field_parsers and "upostag" in field_parsers:
-        field_parsers["upos"] = field_parsers["upostag"]
-
-    line_split = re.split(r"\t| {2,}", line)
-
-    if len(line_split) == 1:
-        raise ParseException("Invalid line format, line must contain either tabs or two spaces.")
-
-    data = Token()
-
-    for i, field in enumerate(fields):
-        # Allow parsing CoNNL-U files with fewer columns
-        if i >= len(line_split):
-            break
-
-        if field in field_parsers:
-            try:
-                value = field_parsers[field](line_split, i)
-            except ParseException as e:
-                raise ParseException("Failed parsing field '{}': ".format(field) + str(e))
-
-        else:
-            value = line_split[i]
-
-        data[str(field)] = value
-
-    return data
-
-def parse_comment_line(line: str,
-                       metadata_parsers: T.Optional[T.Dict[str, _MetadataParserType]] = None
-                       ) -> T.List[T.Tuple[str, T.Optional[str]]]:
-    line = line.strip()
-
-    if line[0] != '#':
-        raise ParseException("Invalid comment format, comment must start with '#'")
-
-    key, value = parse_pair_value(line[1:])
-
-    if not metadata_parsers:
-        metadata_parsers = DEFAULT_METADATA_PARSERS.copy()
-    else:
-        new_metadata_parsers = DEFAULT_METADATA_PARSERS.copy()
-        new_metadata_parsers.update(metadata_parsers)
-        metadata_parsers = new_metadata_parsers
-
-    custom_result = None
-    if key in metadata_parsers:
-        custom_result = metadata_parsers[key](key, value)
-    elif "__fallback__" in metadata_parsers:
-        custom_result = metadata_parsers["__fallback__"](key, value)
-
-    # Allow returning pair instead of list of pairs from metadata parsers
-    if custom_result:
-        if isinstance(custom_result, tuple):
-            key, value = custom_result
-            return [(str(key), value)]
-        return [(str(key), value) for key, value in custom_result]
-
-    if not key or not value:
-        # Lines without value are invalid by default
-        return []
-
-    return [(str(key), value)]
-
-def parse_pair_value(value: str) -> T.Tuple[str, T.Optional[str]]:
-    key_maybe_value = value.split('=', 1)
-    key = key_maybe_value[0].strip()
-    value_new = None if len(key_maybe_value) == 1 else key_maybe_value[1].strip()
-
-    return key, value_new
-
-
-INTEGER = re.compile(r"0|(\-?[1-9][0-9]*)")
-
-def parse_int_value(value: str) -> T.Optional[int]:
-    if value == '_':
-        return None
-
-    if re.fullmatch(INTEGER, value):
-        return int(value)
-    else:
-        raise ParseException("'{}' is not a valid value for parse_int_value.".format(value))
-
-
-ID_SINGLE = re.compile(r"(?:0|[1-9][0-9]*)")
-ID_RANGE = re.compile(r"[1-9][0-9]*\-[1-9][0-9]*")
-ID_DOT_ID = re.compile(r"[0-9][0-9]*\.[1-9][0-9]*")
-
-def parse_id_value(value: str) -> T.Optional[_IdType]:
-    if not value or value == '_':
-        return None
-
-    if re.fullmatch(ID_SINGLE, value):
-        return int(value)
-
-    elif re.fullmatch(ID_RANGE, value):
-        from_str, to_str = value.split("-")
-        from_, to = int(from_str), int(to_str)
-        if to >= from_:
-            return (int(from_), "-", int(to))
-
-    elif re.fullmatch(ID_DOT_ID, value):
-        return (int(value.split(".")[0]), ".", int(value.split(".")[1]))
-
-    raise ParseException("'{}' is not a valid ID.".format(value))
-
-
-ANY_ID = re.compile(ID_SINGLE.pattern + "|" + ID_RANGE.pattern + "|" + ID_DOT_ID.pattern)
-DEPS_RE = re.compile("(" + ANY_ID.pattern + r")(:[^\d:_\-|][^:|]*)+")
-MULTI_DEPS_PATTERN = re.compile(r"{}(\|{})*".format(DEPS_RE.pattern, DEPS_RE.pattern))
-
-def parse_paired_list_value(value: str) -> T.Union[T.Optional[str], T.List[T.Tuple[str, T.Optional[_IdType]]]]:
-    if re.fullmatch(MULTI_DEPS_PATTERN, value):
-        return [
-            (part.split(":", 1)[1], parse_id_value(part.split(":")[0]))
-            for part in value.split("|")
-        ]
-
-    return parse_nullable_value(value)
-
-def parse_dict_value(value: str) -> T.Optional[T.Dict[str, T.Optional[str]]]:
-    if parse_nullable_value(value) is None:
-        return None
-
-    return {
-        part.split("=")[0]: parse_nullable_value(part.split("=")[1]) if "=" in part else ""
-        for part in value.split("|") if parse_nullable_value(part.split("=")[0]) is not None
-    }
-
-def parse_nullable_value(value: str) -> T.Optional[str]:
-    if not value or value == "_":
-        return None
-
-    return value
-
-# DEPRECATED: Mantain old paths until next major version
-def serialize(tokenlist: TokenList) -> str:
-    from conllu.serializer import serialize as new_serialize
-    return new_serialize(tokenlist)
-
-def serialize_field(field: T.Any) -> str:
-    from conllu.serializer import serialize_field as new_serialize_field
-    return new_serialize_field(field)
-
-def head_to_token(sentence: TokenList) -> T.Dict[int, T.List[Token]]:
-    return TokenList.head_to_token(sentence)
+import re
+import typing as T
+
+from conllu.exceptions import ParseException
+from conllu.models import Metadata, Token, TokenList
+
+_IdType = T.Union[int, T.Tuple[int, str, int]]
+_FieldParserType = T.Callable[[T.List[str], int], T.Any]
+_MetadataParserType = T.Callable[[str, T.Optional[str]], T.Any]
+
+DEFAULT_FIELDS = ('id', 'form', 'lemma', 'upos', 'xpos', 'feats', 'head', 'deprel', 'deps', 'misc')
+DEFAULT_FIELD_PARSERS: T.Dict[str, _FieldParserType] = {
+    "id": lambda line, i: parse_id_value(line[i]),
+    "xpos": lambda line, i: parse_nullable_value(line[i]),
+    "feats": lambda line, i: parse_dict_value(line[i]),
+    "head": lambda line, i: parse_int_value(line[i]),
+    "deps": lambda line, i: parse_paired_list_value(line[i]),
+    "misc": lambda line, i: parse_dict_value(line[i]),
+}
+DEFAULT_METADATA_PARSERS: T.Dict[str, _MetadataParserType] = {
+    "newpar": lambda key, value: (key, value),
+    "newdoc": lambda key, value: (key, value),
+}
+
+def parse_conllu_plus_fields(in_file: T.TextIO,
+                             metadata_parsers: T.Optional[T.Dict[str, _MetadataParserType]] = None
+                             ) -> T.Optional[T.Sequence[str]]:
+    pos = in_file.tell()
+
+    # Get first line
+    try:
+        first_sentence = next(parse_sentences(in_file))
+        first_line = first_sentence.split("\n")[0]
+    except StopIteration:
+        first_line = ""
+
+    # parse_sentences moves to file cursor, so reset it here
+    in_file.seek(pos)
+
+    if not first_line.startswith("#"):
+        return None
+
+    tokenlist = parse_token_and_metadata(first_line, metadata_parsers=metadata_parsers)
+    metadata = tokenlist.metadata
+
+    fields = None
+    if "global.columns" in metadata and metadata["global.columns"]:
+        fields = [value.lower() for value in metadata["global.columns"].split(" ")]
+
+    return fields
+
+def parse_sentences(in_file: T.TextIO) -> T.Iterator[str]:
+    buf: T.List[str] = []
+    for line in in_file:
+        if line.strip() == "":
+            if not buf:
+                continue
+            yield "".join(buf).rstrip()
+            buf = []
+        else:
+            buf.append(line)
+    if buf:
+        yield "".join(buf).rstrip()
+
+def parse_token_and_metadata(data: str, fields: T.Optional[T.Sequence[str]] = None,
+                             field_parsers: T.Optional[T.Dict[str, _FieldParserType]] = None,
+                             metadata_parsers: T.Optional[T.Dict[str, _MetadataParserType]] = None
+                             ) -> TokenList:
+
+    if not data:
+        raise ParseException("Can't create TokenList, no data sent to constructor.")
+
+    fields = fields or DEFAULT_FIELDS
+
+    if not field_parsers:
+        field_parsers = DEFAULT_FIELD_PARSERS.copy()
+    elif sorted(field_parsers.keys()) != sorted(fields):
+        new_field_parsers = DEFAULT_FIELD_PARSERS.copy()
+        new_field_parsers.update(field_parsers)
+        field_parsers = new_field_parsers
+
+    tokens = []
+    metadata = Metadata()
+
+    for line in data.split('\n'):
+        line = line.strip()
+
+        if not line:
+            continue
+
+        if line.startswith('#'):
+            pairs = parse_comment_line(line, metadata_parsers=metadata_parsers)
+            for key, value in pairs:
+                metadata[key] = value
+        else:
+            tokens.append(parse_line(line, fields, field_parsers))
+
+    return TokenList(tokens, metadata, default_fields=fields)
+
+def parse_line(line: str,
+               fields: T.Sequence[str], field_parsers: T.Optional[T.Dict[str, _FieldParserType]] = None
+               ) -> Token:
+    # Be backwards compatible if people called parse_line without field_parsers before
+    field_parsers = field_parsers or DEFAULT_FIELD_PARSERS
+
+    # Support xpostag/upostag as aliases for xpos/upos (both ways)
+    if "xpostag" not in field_parsers and "xpos" in field_parsers:
+        field_parsers["xpostag"] = field_parsers["xpos"]
+    if "xpos" not in field_parsers and "xpostag" in field_parsers:
+        field_parsers["xpos"] = field_parsers["xpostag"]
+
+    if "upostag" not in field_parsers and "upos" in field_parsers:
+        field_parsers["upostag"] = field_parsers["upos"]
+    if "upos" not in field_parsers and "upostag" in field_parsers:
+        field_parsers["upos"] = field_parsers["upostag"]
+
+    line_split = re.split(r"\t| {2,}", line)
+
+    if len(line_split) == 1:
+        raise ParseException("Invalid line format, line must contain either tabs or two spaces.")
+
+    data = Token()
+
+    for i, field in enumerate(fields):
+        # Allow parsing CoNNL-U files with fewer columns
+        if i >= len(line_split):
+            break
+
+        if field in field_parsers:
+            try:
+                value = field_parsers[field](line_split, i)
+            except ParseException as e:
+                raise ParseException("Failed parsing field '{}': ".format(field) + str(e))
+
+        else:
+            value = line_split[i]
+
+        data[str(field)] = value
+
+    return data
+
+def parse_comment_line(line: str,
+                       metadata_parsers: T.Optional[T.Dict[str, _MetadataParserType]] = None
+                       ) -> T.List[T.Tuple[str, T.Optional[str]]]:
+    line = line.strip()
+
+    if line[0] != '#':
+        raise ParseException("Invalid comment format, comment must start with '#'")
+
+    key, value = parse_pair_value(line[1:])
+
+    if not metadata_parsers:
+        metadata_parsers = DEFAULT_METADATA_PARSERS.copy()
+    else:
+        new_metadata_parsers = DEFAULT_METADATA_PARSERS.copy()
+        new_metadata_parsers.update(metadata_parsers)
+        metadata_parsers = new_metadata_parsers
+
+    custom_result = None
+    if key in metadata_parsers:
+        custom_result = metadata_parsers[key](key, value)
+    elif "__fallback__" in metadata_parsers:
+        custom_result = metadata_parsers["__fallback__"](key, value)
+
+    # Allow returning pair instead of list of pairs from metadata parsers
+    if custom_result:
+        if isinstance(custom_result, tuple):
+            key, value = custom_result
+            return [(str(key), value)]
+        return [(str(key), value) for key, value in custom_result]
+
+    if not key or not value:
+        # Lines without value are invalid by default
+        return []
+
+    return [(str(key), value)]
+
+def parse_pair_value(value: str) -> T.Tuple[str, T.Optional[str]]:
+    key_maybe_value = value.split('=', 1)
+    key = key_maybe_value[0].strip()
+    value_new = None if len(key_maybe_value) == 1 else key_maybe_value[1].strip()
+
+    return key, value_new
+
+
+INTEGER = re.compile(r"0|(\-?[1-9][0-9]*)")
+
+def parse_int_value(value: str) -> T.Optional[int]:
+    if value == '_':
+        return None
+
+    if re.fullmatch(INTEGER, value):
+        return int(value)
+    else:
+        raise ParseException("'{}' is not a valid value for parse_int_value.".format(value))
+
+
+ID_SINGLE = re.compile(r"(?:0|[1-9][0-9]*)")
+ID_RANGE = re.compile(r"[1-9][0-9]*\-[1-9][0-9]*")
+ID_DOT_ID = re.compile(r"[0-9][0-9]*\.[1-9][0-9]*")
+
+def parse_id_value(value: str) -> T.Optional[_IdType]:
+    if not value or value == '_':
+        return None
+
+    if re.fullmatch(ID_SINGLE, value):
+        return int(value)
+
+    elif re.fullmatch(ID_RANGE, value):
+        from_str, to_str = value.split("-")
+        from_, to = int(from_str), int(to_str)
+        if to >= from_:
+            return (int(from_), "-", int(to))
+
+    elif re.fullmatch(ID_DOT_ID, value):
+        return (int(value.split(".")[0]), ".", int(value.split(".")[1]))
+
+    raise ParseException("'{}' is not a valid ID.".format(value))
+
+
+ANY_ID = re.compile(ID_SINGLE.pattern + "|" + ID_RANGE.pattern + "|" + ID_DOT_ID.pattern)
+DEPS_RE = re.compile("(" + ANY_ID.pattern + r")(:[^\d:_\-|][^:|]*)+")
+MULTI_DEPS_PATTERN = re.compile(r"{}(\|{})*".format(DEPS_RE.pattern, DEPS_RE.pattern))
+
+def parse_paired_list_value(value: str) -> T.Union[T.Optional[str], T.List[T.Tuple[str, T.Optional[_IdType]]]]:
+    if re.fullmatch(MULTI_DEPS_PATTERN, value):
+        return [
+            (part.split(":", 1)[1], parse_id_value(part.split(":")[0]))
+            for part in value.split("|")
+        ]
+
+    return parse_nullable_value(value)
+
+def parse_dict_value(value: str) -> T.Optional[T.Dict[str, T.Optional[str]]]:
+    if parse_nullable_value(value) is None:
+        return None
+
+    return {
+        part.split("=")[0]: parse_nullable_value(part.split("=")[1]) if "=" in part else ""
+        for part in value.split("|") if parse_nullable_value(part.split("=")[0]) is not None
+    }
+
+def parse_nullable_value(value: str) -> T.Optional[str]:
+    if not value or value == "_":
+        return None
+
+    return value
+
+# DEPRECATED: Mantain old paths until next major version
+def serialize(tokenlist: TokenList) -> str:
+    from conllu.serializer import serialize as new_serialize
+    return new_serialize(tokenlist)
+
+def serialize_field(field: T.Any) -> str:
+    from conllu.serializer import serialize_field as new_serialize_field
+    return new_serialize_field(field)
+
+def head_to_token(sentence: TokenList) -> T.Dict[int, T.List[Token]]:
+    return TokenList.head_to_token(sentence)
```

### Comparing `conllu-4.5.2/conllu.egg-info/PKG-INFO` & `conllu-4.5.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: conllu
-Version: 4.5.2
-Summary: CoNLL-U Parser parses a CoNLL-U formatted string into a nested python dictionary
-Home-page: https://github.com/EmilStenstrom/conllu/
-Author: Emil Stenström
-Author-email: emil@emilstenstrom.se
-License: MIT License
-Keywords: conllu,conll,conll-u,parser,nlp
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CoNLL-U Parser
 
 **CoNLL-U Parser** parses a [CoNLL-U formatted](http://universaldependencies.org/format.html) string into a nested python dictionary. CoNLL-U is often the output of natural language processing tasks.
 
 ## Why should you use conllu?
 
 - It's simple. ~300 lines of code.
@@ -497,9 +474,7 @@
     ```bash
     tox -e py36
     ```
 
 5. Make a pull request. Here's a [good guide on PRs from GitHub](https://help.github.com/articles/creating-a-pull-request-from-a-fork/).
 
 Thanks for helping conllu become a better library!
-
-
```

### Comparing `conllu-4.5.2/setup.py` & `conllu-4.5.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import os
-
-from setuptools import setup  # type: ignore
-
-VERSION = '4.5.2'
-
-with open(os.path.join(os.path.dirname(__file__), 'README.md')) as f:
-    description = f.read()
-
-setup(
-    name='conllu',
-    packages=["conllu"],
-    python_requires=">=3.6",
-    package_data={
-        "": ["py.typed"]
-    },
-    version=VERSION,
-    license='MIT License',
-    description='CoNLL-U Parser parses a CoNLL-U formatted string into a nested python dictionary',
-    long_description=description,
-    long_description_content_type="text/markdown",
-    author=u'Emil Stenström',
-    author_email="emil@emilstenstrom.se",
-    url='https://github.com/EmilStenstrom/conllu/',
-    keywords=['conllu', 'conll', 'conll-u', 'parser', 'nlp'],
-    classifiers=[
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Operating System :: OS Independent",
-    ],
-)
+import os
+
+from setuptools import setup  # type: ignore
+
+VERSION = '4.5.3'
+
+with open(os.path.join(os.path.dirname(__file__), 'README.md')) as f:
+    description = f.read()
+
+setup(
+    name='conllu',
+    packages=["conllu"],
+    python_requires=">=3.6",
+    package_data={
+        "": ["py.typed"]
+    },
+    version=VERSION,
+    license='MIT License',
+    description='CoNLL-U Parser parses a CoNLL-U formatted string into a nested python dictionary',
+    long_description=description,
+    long_description_content_type="text/markdown",
+    author=u'Emil Stenström',
+    author_email="emil@emilstenstrom.se",
+    url='https://github.com/EmilStenstrom/conllu/',
+    keywords=['conllu', 'conll', 'conll-u', 'parser', 'nlp'],
+    classifiers=[
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Operating System :: OS Independent",
+    ],
+)
```

