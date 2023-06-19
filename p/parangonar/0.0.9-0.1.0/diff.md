# Comparing `tmp/parangonar-0.0.9.tar.gz` & `tmp/parangonar-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parangonar-0.0.9.tar", last modified: Mon Nov 21 13:51:08 2022, max compression
+gzip compressed data, was "parangonar-0.1.0.tar", last modified: Mon Jun 19 11:35:37 2023, max compression
```

## Comparing `parangonar-0.0.9.tar` & `parangonar-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-11-21 13:51:08.386329 parangonar-0.0.9/
--rw-rw-rw-   0        0        0    11630 2022-11-11 16:50:07.000000 parangonar-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     5801 2022-11-21 13:51:08.385332 parangonar-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     5340 2022-11-21 13:44:44.000000 parangonar-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2022-11-21 13:51:08.334467 parangonar-0.0.9/parangonar/
--rw-rw-rw-   0        0        0      525 2022-11-21 12:55:28.000000 parangonar-0.0.9/parangonar/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-21 13:51:08.367379 parangonar-0.0.9/parangonar/assets/
--rw-rw-rw-   0        0        0    20420 2022-10-04 17:33:45.000000 parangonar-0.0.9/parangonar/assets/mozart_k265_var1.match
-drwxrwxrwx   0        0        0        0 2022-11-21 13:51:08.370370 parangonar-0.0.9/parangonar/evaluate/
--rw-rw-rw-   0        0        0     7951 2022-11-21 13:46:33.000000 parangonar-0.0.9/parangonar/evaluate/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-21 13:51:08.382339 parangonar-0.0.9/parangonar/match/
--rw-rw-rw-   0        0        0      644 2022-11-21 11:53:39.000000 parangonar-0.0.9/parangonar/match/__init__.py
--rw-rw-rw-   0        0        0     4976 2022-11-18 10:41:29.000000 parangonar-0.0.9/parangonar/match/dtw.py
--rw-rw-rw-   0        0        0    19355 2022-11-21 13:12:14.000000 parangonar-0.0.9/parangonar/match/matchers.py
--rw-rw-rw-   0        0        0     6438 2022-11-18 13:06:13.000000 parangonar-0.0.9/parangonar/match/nwtw.py
--rw-rw-rw-   0        0        0    22443 2022-11-21 13:22:53.000000 parangonar-0.0.9/parangonar/match/preprocessors.py
-drwxrwxrwx   0        0        0        0 2022-11-21 13:51:08.365386 parangonar-0.0.9/parangonar.egg-info/
--rw-rw-rw-   0        0        0     5801 2022-11-21 13:51:08.000000 parangonar-0.0.9/parangonar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2022-11-21 13:51:08.000000 parangonar-0.0.9/parangonar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-21 13:51:08.000000 parangonar-0.0.9/parangonar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2022-11-21 13:51:08.000000 parangonar-0.0.9/parangonar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-11-21 13:51:08.000000 parangonar-0.0.9/parangonar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-21 13:51:08.387329 parangonar-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1870 2022-11-21 13:48:54.000000 parangonar-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:35:37.831336 parangonar-0.1.0/
+-rw-rw-rw-   0        0        0    11630 2022-11-11 16:50:08.000000 parangonar-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     5772 2023-06-19 11:35:37.830323 parangonar-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5311 2023-06-19 11:33:08.000000 parangonar-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 11:35:37.776367 parangonar-0.1.0/parangonar/
+-rw-rw-rw-   0        0        0      525 2022-12-05 09:58:42.000000 parangonar-0.1.0/parangonar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:35:37.804393 parangonar-0.1.0/parangonar/assets/
+-rw-rw-rw-   0        0        0    20420 2022-10-04 17:33:46.000000 parangonar-0.1.0/parangonar/assets/mozart_k265_var1.match
+drwxrwxrwx   0        0        0        0 2023-06-19 11:35:37.807389 parangonar-0.1.0/parangonar/evaluate/
+-rw-rw-rw-   0        0        0     7951 2023-06-19 11:28:40.000000 parangonar-0.1.0/parangonar/evaluate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:35:37.822343 parangonar-0.1.0/parangonar/match/
+-rw-rw-rw-   0        0        0      681 2023-06-19 11:28:40.000000 parangonar-0.1.0/parangonar/match/__init__.py
+-rw-rw-rw-   0        0        0     4976 2023-06-19 11:28:40.000000 parangonar-0.1.0/parangonar/match/dtw.py
+-rw-rw-rw-   0        0        0    19355 2023-06-19 11:33:08.000000 parangonar-0.1.0/parangonar/match/matchers.py
+-rw-rw-rw-   0        0        0     6438 2022-11-18 13:06:14.000000 parangonar-0.1.0/parangonar/match/nwtw.py
+-rw-rw-rw-   0        0        0    15788 2023-06-19 11:28:40.000000 parangonar-0.1.0/parangonar/match/preprocessors.py
+-rw-rw-rw-   0        0        0    12540 2023-06-19 11:28:40.000000 parangonar-0.1.0/parangonar/match/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:35:37.796319 parangonar-0.1.0/parangonar.egg-info/
+-rw-rw-rw-   0        0        0     5772 2023-06-19 11:35:37.000000 parangonar-0.1.0/parangonar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      503 2023-06-19 11:35:37.000000 parangonar-0.1.0/parangonar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 11:35:37.000000 parangonar-0.1.0/parangonar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-19 11:35:37.000000 parangonar-0.1.0/parangonar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-19 11:35:37.000000 parangonar-0.1.0/parangonar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-19 11:35:37.831336 parangonar-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1870 2023-06-19 11:33:08.000000 parangonar-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:35:37.827333 parangonar-0.1.0/tests/
+-rw-rw-rw-   0        0        0     1301 2022-11-18 13:22:30.000000 parangonar-0.1.0/tests/test_align.py
+-rw-rw-rw-   0        0        0     1015 2022-11-18 16:17:30.000000 parangonar-0.1.0/tests/test_note_align.py
```

### Comparing `parangonar-0.0.9/LICENSE` & `parangonar-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parangonar-0.0.9/PKG-INFO` & `parangonar-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,21 @@
-Metadata-Version: 2.1
-Name: parangonar
-Version: 0.0.9
-Summary: Symbolic music alignment
-Home-page: https://github.com/sildater/parangonar
-Author: Silvan Peter, Carlos Cancino-Chacón, Florian Henkel
-License: Apache 2.0
-Keywords: match alignment midi performance score
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
 Parangonar
 ==========
 
 **Parangonar** is a Python package for note alignment of symbolic music. 
 **Parangonar** uses [Partitura](https://github.com/CPJKU/partitura) as file I/O utility.
 Note alignments produced py **Parangonar** can be visualized using the 
 web tool [Parangonda](https://sildater.github.io/parangonada/)
 
 
 Installation
 ==========
 
 The easiest way to install the package is via `pip` from the [PyPI (Python
-Package Index)](https://pypi.python.org/pypi>):
+Package Index)](https://pypi.org/project/parangonar/>):
 ```shell
 pip install parangonar
 ```
 This will install the latest release of the package and will install all dependencies automatically.
 
 
 Quickstart
@@ -97,25 +82,26 @@
 ```
 
 File I/O for note alignments
 ==========
 
 ```python
 import partitura as pt
+import parangonar as pa
 
 # load note alignments of the asap dataset: 
 # https://github.com/CPJKU/asap-dataset/tree/note_alignments
 alignment = pt.io.importparangonada.load_alignment_from_ASAP(filename= 'path/to/note_alignment.tsv')
 
 # export a note alignment for visualization with parangonada:
 # https://sildater.github.io/parangonada/
-pt.io.exportparangonada.save_parangonada_csv(alignment, 
-                                            performance_data,
-                                            score_data
-                                            outdir="path/to/dir")
+pa.match.save_parangonada_csv(alignment, 
+                            performance_data,
+                            score_data,
+                            outdir="path/to/dir")
 
 # import a corrected note alignment from parangonada:
 # https://sildater.github.io/parangonada/
 alignment = pt.io.importparangonada.load_parangonada_alignment(filename= 'path/to/note_alignment.csv')
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `parangonar-0.0.9/README.md` & `parangonar-0.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,36 @@
+Metadata-Version: 2.1
+Name: parangonar
+Version: 0.1.0
+Summary: Symbolic music alignment
+Home-page: https://github.com/sildater/parangonar
+Author: Silvan Peter, Carlos Cancino-Chacón, Florian Henkel
+License: Apache 2.0
+Keywords: match alignment midi performance score
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
 Parangonar
 ==========
 
 **Parangonar** is a Python package for note alignment of symbolic music. 
 **Parangonar** uses [Partitura](https://github.com/CPJKU/partitura) as file I/O utility.
 Note alignments produced py **Parangonar** can be visualized using the 
 web tool [Parangonda](https://sildater.github.io/parangonada/)
 
 
 Installation
 ==========
 
 The easiest way to install the package is via `pip` from the [PyPI (Python
-Package Index)](https://pypi.python.org/pypi>):
+Package Index)](https://pypi.org/project/parangonar/>):
 ```shell
 pip install parangonar
 ```
 This will install the latest release of the package and will install all dependencies automatically.
 
 
 Quickstart
@@ -82,25 +97,26 @@
 ```
 
 File I/O for note alignments
 ==========
 
 ```python
 import partitura as pt
+import parangonar as pa
 
 # load note alignments of the asap dataset: 
 # https://github.com/CPJKU/asap-dataset/tree/note_alignments
 alignment = pt.io.importparangonada.load_alignment_from_ASAP(filename= 'path/to/note_alignment.tsv')
 
 # export a note alignment for visualization with parangonada:
 # https://sildater.github.io/parangonada/
-pt.io.exportparangonada.save_parangonada_csv(alignment, 
-                                            performance_data,
-                                            score_data
-                                            outdir="path/to/dir")
+pa.match.save_parangonada_csv(alignment, 
+                            performance_data,
+                            score_data,
+                            outdir="path/to/dir")
 
 # import a corrected note alignment from parangonada:
 # https://sildater.github.io/parangonada/
 alignment = pt.io.importparangonada.load_parangonada_alignment(filename= 'path/to/note_alignment.csv')
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `parangonar-0.0.9/parangonar/__init__.py` & `parangonar-0.1.0/parangonar/__init__.py`

 * *Files identical despite different names*

### Comparing `parangonar-0.0.9/parangonar/assets/mozart_k265_var1.match` & `parangonar-0.1.0/parangonar/assets/mozart_k265_var1.match`

 * *Files identical despite different names*

### Comparing `parangonar-0.0.9/parangonar/evaluate/__init__.py` & `parangonar-0.1.0/parangonar/evaluate/__init__.py`

 * *Files identical despite different names*

### Comparing `parangonar-0.0.9/parangonar/match/__init__.py` & `parangonar-0.1.0/parangonar/match/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 """
 
 
 from .dtw import DTW
 from .nwtw import NW_DTW, NW
 from .matchers import (AnchorPointNoteMatcher, 
                        AutomaticNoteMatcher)
-from .preprocessors import node_array
+from .utils import (node_array,
+                    save_parangonada_csv)
```

### Comparing `parangonar-0.0.9/parangonar/match/dtw.py` & `parangonar-0.1.0/parangonar/match/dtw.py`

 * *Files identical despite different names*

### Comparing `parangonar-0.0.9/parangonar/match/matchers.py` & `parangonar-0.1.0/parangonar/match/matchers.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,16 +311,16 @@
                  node_mender=mend_note_alignments,
                  symbolic_note_matcher=SequenceAugmentedGreedyMatcher(),
                  greedy_symbolic_note_matcher=SimplestGreedyMatcher(),
                  alignment_type="dtw",
                  SCORE_FINE_NODE_LENGTH=0.25,
                  s_time_div=16,
                  p_time_div=16,
-                 sfuzziness=0.5,
-                 pfuzziness=0.5,
+                 sfuzziness=4.0,
+                 pfuzziness=4.0,
                  window_size=1,
                  pfuzziness_relative_to_tempo=True,
                  shift_onsets=False,
                  cap_combinations=None):
 
         self.note_matcher = note_matcher(**matcher_kwargs)
         self.symbolic_note_matcher = symbolic_note_matcher
```

### Comparing `parangonar-0.0.9/parangonar/match/nwtw.py` & `parangonar-0.1.0/parangonar/match/nwtw.py`

 * *Files identical despite different names*

### Comparing `parangonar-0.0.9/parangonar/match/preprocessors.py` & `parangonar-0.1.0/parangonar/match/preprocessors.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,22 +3,15 @@
 """
 This module contains preprocessing methods
 """
 
 import numpy as np
 from scipy.interpolate import interp1d
 
-from partitura.utils.music import (compute_pianoroll, 
-                                   ensure_notearray)
-
-from partitura.musicanalysis.performance_codec import ( 
-                                    to_matched_score,
-                                    get_unique_onset_idxs
-                                    )
-
+from partitura.utils.music import (compute_pianoroll)
 
 from .dtw import DTW
 from .nwtw import NW_DTW, NW
 
 
 ################################### HELPERS ###################################
 
@@ -340,166 +333,7 @@
         if pnote_id not in used_perf_notes:
             #print("previously unused performance note: ", pnote_id, performance_alignment[pnote_id])
             alignment.append({'label': 'insertion', 'performance_id': pnote_id})
 
     return alignment, score_alignment, performance_alignment
 
 
-################################### ANCHOR POINT GENERAITON ###################################
-
-
-def node_array(part, 
-                ppart,
-                alignment,
-                tapping_noise=False,
-                node_interval=1, 
-                start_beat=None,
-                nodes_in_beats=True):
-    """
-    generates an array of nodes, corresponding score time point and 
-    performance time point tuples, spacing given by note_interval.
-    
-    Args:
-        part (partitura.Part): a part object
-        ppart (partitura.PerformedPart): a performedpart object
-        alignment (List(Dict)): an alignment
-
-    Returns:
-        np.ndarray: a minimal, aligned 
-            node note array.
-
-    """
-
-    ppart.sustain_pedal_threshold = 128
-
-    matched_score, snote_ids = to_matched_score(part, ppart, alignment)
-
-    # get unique onsets
-    nid_dict = dict((n.id, i) for i, n in enumerate(part.notes_tied))
-    matched_subset_idxs = np.array([nid_dict[nid] for nid in snote_ids])
-
-    part_note_array = ensure_notearray(part,
-                                        include_time_signature=True)
-
-    score_onsets = part_note_array[matched_subset_idxs]['onset_beat']
-    # changed from onset_beat
-    unique_onset_idxs = get_unique_onset_idxs(score_onsets)
-
-    smatched_score_onset = notewise_to_onsetwise(matched_score['onset'],
-                                                    unique_onset_idxs,
-                                                    aggregation_func=np.mean)
-    pmatched_score_onset = notewise_to_onsetwise(matched_score['p_onset'],
-                                                    unique_onset_idxs,
-                                                    aggregation_func=np.mean)
-    
-    if nodes_in_beats:
-        beat_times, sbeat_times = beat_times_from_matched_score(
-            smatched_score_onset, 
-            pmatched_score_onset,
-            tapping_noise=tapping_noise,
-            node_interval=node_interval,
-            start_beat=start_beat)
-    else: 
-        beat_times, sbeat_times = measure_times_from_matched_score(
-            smatched_score_onset, 
-            pmatched_score_onset, 
-            part, 
-            tapping_noise=tapping_noise,
-            measure_interval=node_interval,
-            start_measure=start_beat)
-
-    alignment_times = [*zip(sbeat_times, beat_times)]
-
-    return alignment_times
-
-
-def beat_times_from_matched_score(x, y,
-                                  tapping_noise=False,
-                                  node_interval=1.0,
-                                  start_beat=None):
-
-    beat_times_func = interp1d(x, y, kind="linear", fill_value="extrapolate")
-
-    min_beat = np.ceil(x.min())  # -node_interval
-    min_beat_original = min_beat
-    max_beat = np.floor(x.max())  # +node_interval
-
-    if start_beat is not None:
-        print("first node at ", start_beat, " first beat at ", min_beat)
-        min_beat = start_beat
-        
-    sbeat_times = np.arange(min_beat, max_beat, node_interval)
-    # prepend and append very low and high values to make sure every beat/beat annotation falls between two sbeat_times/beat_times
-    sbeat_times = np.append(np.append(min_beat_original-max(100, node_interval),sbeat_times),max_beat+max(100, node_interval))
-    beat_times = beat_times_func(sbeat_times)
-
-    if tapping_noise:
-        beat_times += np.random.normal(0.0, tapping_noise,
-                                       beat_times.shape)
-
-    return beat_times, sbeat_times
-
-
-def measure_times_from_matched_score(x, y, part, 
-                                  tapping_noise=False,
-                                  measure_interval=1,
-                                  start_measure=None):
-
-    beat_times_func = interp1d(x, y, kind="linear", fill_value="extrapolate")
-
-    measure_times_in_part = [part.beat_map(measure.start.t) for measure in part.iter_all(partitura.score.Measure)]
-    if start_measure is None:
-        start_measure=0
-    
-    smeasure_idx = np.arange(start_measure, len(measure_times_in_part), measure_interval, dtype = int)
-    smeasure_times = np.array(measure_times_in_part)[smeasure_idx]
-    # prepend and append very low and high values to make sure every beat/beat annotation falls between two sbeat_times/beat_times
-    smeasure_times = np.append(np.append(smeasure_times[0]-max(100, measure_interval),smeasure_times),smeasure_times[-1]+max(100, measure_interval))
-    pmeasure_times = beat_times_func(smeasure_times)
-
-    if tapping_noise:
-        pmeasure_times += np.random.normal(0.0, tapping_noise, pmeasure_times.shape)
-
-    return pmeasure_times, smeasure_times
-
-
-def notewise_to_onsetwise(notewise_inputs, 
-                          unique_onset_idxs, 
-                          aggregation_func=np.mean):
-    """Agregate onset times per score onset
-    """
-    
-    onsetwise_inputs = np.zeros(len(unique_onset_idxs),
-                                dtype=notewise_inputs.dtype)
-
-    for i, uix in enumerate(unique_onset_idxs):
-        onsetwise_inputs[i] = aggregation_func(notewise_inputs[uix])
-    return onsetwise_inputs
-
-
-def expand_grace_notes(note_array, backwards_time=0.2):
-    """
-    expand the duration of gracenotes in a note_array and reset their onset by a timespan called backwards_time
-    """
-    grace_note_onsets = np.unique(
-        note_array["onset_beat"][note_array["duration_beat"] == 0.0])
-    for gno in grace_note_onsets:
-        mask = np.all([note_array["duration_beat"] == 0.0,
-                       note_array["onset_beat"] == gno],
-                      axis=0)
-        number_of_grace_notes = mask.sum()
-        note_array["onset_beat"][mask] -= np.linspace(backwards_time,0.0, number_of_grace_notes+1)[:-1]
-        note_array["duration_beat"][mask] += backwards_time/(number_of_grace_notes)
-    return note_array
-
-
-def convert_grace_to_insertions(alignment):
-    """
-    relabel all ornament alignments as insertions
-    """
-    new_alignment = [al for al in alignment if al["label"] != "ornament"]
-    new_alignment_o = [al for al in alignment if al["label"] == "ornament"]
-    for al in new_alignment_o:
-        new_al = {'label': 'insertion', 'performance_id': al["performance_id"]}
-        new_alignment.append(new_al)
-    return new_alignment
-
```

### Comparing `parangonar-0.0.9/parangonar.egg-info/PKG-INFO` & `parangonar-0.1.0/parangonar.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parangonar
-Version: 0.0.9
+Version: 0.1.0
 Summary: Symbolic music alignment
 Home-page: https://github.com/sildater/parangonar
 Author: Silvan Peter, Carlos Cancino-Chacón, Florian Henkel
 License: Apache 2.0
 Keywords: match alignment midi performance score
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -22,15 +22,15 @@
 web tool [Parangonda](https://sildater.github.io/parangonada/)
 
 
 Installation
 ==========
 
 The easiest way to install the package is via `pip` from the [PyPI (Python
-Package Index)](https://pypi.python.org/pypi>):
+Package Index)](https://pypi.org/project/parangonar/>):
 ```shell
 pip install parangonar
 ```
 This will install the latest release of the package and will install all dependencies automatically.
 
 
 Quickstart
@@ -97,25 +97,26 @@
 ```
 
 File I/O for note alignments
 ==========
 
 ```python
 import partitura as pt
+import parangonar as pa
 
 # load note alignments of the asap dataset: 
 # https://github.com/CPJKU/asap-dataset/tree/note_alignments
 alignment = pt.io.importparangonada.load_alignment_from_ASAP(filename= 'path/to/note_alignment.tsv')
 
 # export a note alignment for visualization with parangonada:
 # https://sildater.github.io/parangonada/
-pt.io.exportparangonada.save_parangonada_csv(alignment, 
-                                            performance_data,
-                                            score_data
-                                            outdir="path/to/dir")
+pa.match.save_parangonada_csv(alignment, 
+                            performance_data,
+                            score_data,
+                            outdir="path/to/dir")
 
 # import a corrected note alignment from parangonada:
 # https://sildater.github.io/parangonada/
 alignment = pt.io.importparangonada.load_parangonada_alignment(filename= 'path/to/note_alignment.csv')
 ```
```

### Comparing `parangonar-0.0.9/setup.py` & `parangonar-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Package meta-data.
 NAME = 'parangonar'
 DESCRIPTION = 'Symbolic music alignment'
 KEYWORDS = 'match alignment midi performance score'
 URL = "https://github.com/sildater/parangonar"
 AUTHOR = 'Silvan Peter, Carlos Cancino-Chacón, Florian Henkel'
 REQUIRES_PYTHON = '>=3.7'
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'numpy',
     'scipy',
     'partitura>=1.1.0',
     'python-hiddenmarkov'
```

