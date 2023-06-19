# Comparing `tmp/sleepeeg-0.2.2.tar.gz` & `tmp/sleepeeg-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepeeg-0.2.2.tar", last modified: Wed Jun 14 08:25:44 2023, max compression
+gzip compressed data, was "sleepeeg-0.2.3.tar", last modified: Mon Jun 19 10:06:15 2023, max compression
```

## Comparing `sleepeeg-0.2.2.tar` & `sleepeeg-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 08:25:44.860960 sleepeeg-0.2.2/
--rw-rw-rw-   0        0        0     1088 2023-03-20 20:54:05.000000 sleepeeg-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     1728 2023-06-14 08:25:44.858964 sleepeeg-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2023-06-09 12:52:22.000000 sleepeeg-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 08:25:44.817077 sleepeeg-0.2.2/docs/
--rw-rw-rw-   0        0        0     2495 2023-06-06 06:12:53.000000 sleepeeg-0.2.2/docs/conf.py
--rw-rw-rw-   0        0        0      861 2023-06-14 08:23:24.000000 sleepeeg-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 08:25:44.860960 sleepeeg-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-14 08:25:44.840015 sleepeeg-0.2.2/sleepeeg/
--rw-rw-rw-   0        0        0    52073 2023-06-11 05:22:09.000000 sleepeeg-0.2.2/sleepeeg/base.py
--rw-rw-rw-   0        0        0     9820 2023-06-14 08:18:46.000000 sleepeeg-0.2.2/sleepeeg/dashboard.py
--rw-rw-rw-   0        0        0    34102 2023-06-11 07:01:30.000000 sleepeeg-0.2.2/sleepeeg/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:25:44.857968 sleepeeg-0.2.2/sleepeeg.egg-info/
--rw-rw-rw-   0        0        0     1728 2023-06-14 08:25:44.000000 sleepeeg-0.2.2/sleepeeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-06-14 08:25:44.000000 sleepeeg-0.2.2/sleepeeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 08:25:44.000000 sleepeeg-0.2.2/sleepeeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2023-06-14 08:25:44.000000 sleepeeg-0.2.2/sleepeeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-06-14 08:25:44.000000 sleepeeg-0.2.2/sleepeeg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 10:06:15.322218 sleepeeg-0.2.3/
+-rw-rw-rw-   0        0        0     1088 2023-03-20 20:54:05.000000 sleepeeg-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     1728 2023-06-19 10:06:15.322218 sleepeeg-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2023-06-09 12:52:22.000000 sleepeeg-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 10:06:15.292298 sleepeeg-0.2.3/docs/
+-rw-rw-rw-   0        0        0     2495 2023-06-06 06:12:53.000000 sleepeeg-0.2.3/docs/conf.py
+-rw-rw-rw-   0        0        0      861 2023-06-19 08:41:56.000000 sleepeeg-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-19 10:06:15.323215 sleepeeg-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-19 10:06:15.298281 sleepeeg-0.2.3/sleepeeg/
+-rw-rw-rw-   0        0        0    51888 2023-06-19 06:26:07.000000 sleepeeg-0.2.3/sleepeeg/base.py
+-rw-rw-rw-   0        0        0    12356 2023-06-19 09:06:55.000000 sleepeeg-0.2.3/sleepeeg/dashboard.py
+-rw-rw-rw-   0        0        0    34242 2023-06-19 06:53:17.000000 sleepeeg-0.2.3/sleepeeg/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-06-19 10:06:15.319225 sleepeeg-0.2.3/sleepeeg.egg-info/
+-rw-rw-rw-   0        0        0     1728 2023-06-19 10:06:15.000000 sleepeeg-0.2.3/sleepeeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-06-19 10:06:15.000000 sleepeeg-0.2.3/sleepeeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 10:06:15.000000 sleepeeg-0.2.3/sleepeeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      132 2023-06-19 10:06:15.000000 sleepeeg-0.2.3/sleepeeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2023-06-19 10:06:15.000000 sleepeeg-0.2.3/sleepeeg.egg-info/top_level.txt
```

### Comparing `sleepeeg-0.2.2/LICENSE` & `sleepeeg-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.2.2/PKG-INFO` & `sleepeeg-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepeeg
-Version: 0.2.2
+Version: 0.2.3
 Summary: Sleep EEG preprocessing and analysis
 Author-email: Gennadiy Belonosov <gennadiyb@mail.tau.ac.il>
 License: MIT
 Project-URL: Homepage, https://github.com/NirLab-TAU/sleepeeg
 Project-URL: Documentation, https://nirlab-tau.github.io/sleepeeg/
 Keywords: sleep,eeg
 Requires-Python: >=3.10
```

### Comparing `sleepeeg-0.2.2/README.md` & `sleepeeg-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.2.2/docs/conf.py` & `sleepeeg-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.2.2/pyproject.toml` & `sleepeeg-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 exclude = ["notebooks"]  # empty by default
 
 [project]
 name = "sleepeeg"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
     {name = "Gennadiy Belonosov", email = "gennadiyb@mail.tau.ac.il"},
 ]
 description = "Sleep EEG preprocessing and analysis"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT"}
```

### Comparing `sleepeeg-0.2.2/sleepeeg/base.py` & `sleepeeg-0.2.3/sleepeeg/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,64 +83,63 @@
     """An instanse of :py:class:`mne:mne.io.Raw`.
     """
 
     @mne_raw.default
     def _read_mne_raw(self):
         if self.prec_pipe:
             return self.prec_pipe.mne_raw
-        else:
-            try:
-                return mne.io.read_raw(self.path_to_eeg)
-            except RuntimeError as err:
-                if "EGI epoch first/last samps" in str(err):
-                    import re
-                    from ast import literal_eval
-                    from itertools import chain
-                    import shutil
+        try:
+            return mne.io.read_raw(self.path_to_eeg)
+        except RuntimeError as err:
+            if "EGI epoch first/last samps" in str(err):
+                import re
+                from ast import literal_eval
+                from itertools import chain
+                import shutil
 
-                    logger.warning(
-                        "Fixing epochs.xml from the .mff, original file is saved as epochs_old.xml"
+                logger.warning(
+                    "Fixing epochs.xml from the .mff, original file is saved as epochs_old.xml"
+                )
+                values = chain.from_iterable(
+                    zip(
+                        range(-1000, -6000, -1000),
+                        range(1000, 6000, 1000),
                     )
-                    values = chain.from_iterable(
-                        zip(
-                            range(-1000, -6000, -1000),
-                            range(1000, 6000, 1000),
-                        )
-                    )
-                    shutil.copyfile(
-                        self.path_to_eeg / "epochs.xml",
-                        self.path_to_eeg / "epochs_old.xml",
+                )
+                shutil.copyfile(
+                    self.path_to_eeg / "epochs.xml",
+                    self.path_to_eeg / "epochs_old.xml",
+                )
+                for value in values:
+                    operation = (
+                        f"subtract {abs(value)} from"
+                        if value < 0
+                        else f"add {abs(value)} to"
                     )
-                    for value in values:
-                        logger.info(
-                            "Trying to {} the last 'endTime' tag",
-                            f"subtract {abs(value)} from"
-                            if value < 0
-                            else f"add {abs(value)} to",
+                    logger.info(f"Trying to {operation} the last 'endTime' tag")
+                    with open(self.path_to_eeg / "epochs.xml", "r+") as epochs_f:
+                        orig_xml = epochs_f.read()
+                        matches = re.findall(r"<endTime>(\d+)<\/endTime>", orig_xml)
+                        new_xml = orig_xml.replace(
+                            matches[-1], str(literal_eval(matches[-1]) + value)
                         )
-                        with open(self.path_to_eeg / "epochs.xml", "r+") as epochs_f:
-                            orig_xml = epochs_f.read()
-                            matches = re.findall(r"<endTime>(\d+)<\/endTime>", orig_xml)
-                            new_xml = orig_xml.replace(
-                                matches[-1], str(literal_eval(matches[-1]) + value)
-                            )
-                            epochs_f.seek(0)
-                            epochs_f.write(new_xml)
-                            epochs_f.truncate()
-                        try:
-                            return mne.io.read_raw(self.path_to_eeg)
-                        except:
-                            with open(self.path_to_eeg / "epochs.xml", "w") as epochs_f:
-                                epochs_f.write(orig_xml)
+                        epochs_f.seek(0)
+                        epochs_f.write(new_xml)
+                        epochs_f.truncate()
+                    try:
+                        return mne.io.read_raw(self.path_to_eeg)
+                    except:
+                        with open(self.path_to_eeg / "epochs.xml", "w") as epochs_f:
+                            epochs_f.write(orig_xml)
 
-                else:
-                    raise
-            except Exception as err:
-                print(f"Unexpected {err=}, {type(err)=}")
+            else:
                 raise
+        except Exception as err:
+            print(f"Unexpected {err=}, {type(err)=}")
+            raise
 
     @property
     def sf(self):
         """A wrapper for :py:class:`raw.info["sfreq"] <mne:mne.Info>`.
 
         Returns:
             float: sampling frequency
```

### Comparing `sleepeeg-0.2.2/sleepeeg/dashboard.py` & `sleepeeg-0.2.3/sleepeeg/dashboard.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,259 @@
 import os
+import time
+from collections.abc import Iterable, Sequence
+
 import numpy as np
-from collections.abc import Iterable
+import matplotlib.pyplot as plt
+from mne import pick_types
+from mne.io.pick import _picks_to_idx
+
+from .pipeline import CleaningPipe, SpectralPipe
 
 
-def get_min_max_psds(psds, picks):
+def _init_s_pipe(prec_pipe, path_to_hypnogram, hypno_freq):
+    if path_to_hypnogram is None:
+        s_pipe = SpectralPipe(
+            prec_pipe=prec_pipe,
+        )
+        s_pipe.hypno = np.zeros(s_pipe.mne_raw.n_times)
+        s_pipe.hypno_freq = s_pipe.sf
+        s_pipe._BaseHypnoPipe__upsample_hypno()
+        sleep_stages = {"All": 0}
+    else:
+        s_pipe = SpectralPipe(
+            prec_pipe=prec_pipe,
+            path_to_hypno=path_to_hypnogram,
+            hypno_freq=hypno_freq,
+        )
+        sleep_stages = {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4}
+    return s_pipe, sleep_stages
+
+
+def _get_min_max_psds(psds, picks):
     max_psd = None
     min_psd = None
     for spectrum in psds.values():
         data = 10 * np.log10(10**12 * spectrum.copy().pick(picks)._data)
         data[data == -np.inf] = np.nan
         max_psd = (
             np.nanmax(data) if max_psd is None or max_psd < np.nanmax(data) else max_psd
         )
         min_psd = (
             np.nanmin(data) if min_psd is None or min_psd > np.nanmin(data) else min_psd
         )
     return min_psd, max_psd
 
 
+def _filter(pipe, sfreq, fmin, fmax):
+    if sfreq is None or sfreq >= pipe.sf:
+        sfreq = pipe.sf
+    else:
+        pipe.resample(sfreq=sfreq, n_jobs=-1)
+
+    notch_freqs = np.arange(50, int(pipe.sf / 2), 50)
+    hp = pipe.mne_raw.info["highpass"]
+    lp = pipe.mne_raw.info["lowpass"]
+    if fmin is None or fmin <= hp:
+        fmin = hp
+    else:
+        pipe.filter(l_freq=fmin, h_freq=None, n_jobs=-1)
+    if fmax is None or fmax >= lp:
+        fmax = lp
+    else:
+        pipe.filter(l_freq=None, h_freq=fmax, n_jobs=-1)
+
+    if fmax > 50:
+        pipe.notch(freqs=notch_freqs, n_jobs=-1)
+    else:
+        notch_freqs = None
+
+    return sfreq, fmin, fmax, notch_freqs
+
+
+def _hypno_psd(
+    s_pipe,
+    sleep_stages,
+    ref_channels,
+    hypno_psd_pick,
+    ax_hypno,
+    ax_psd,
+    min_psd,
+    max_psd,
+):
+    s_pipe.compute_psds_per_stage(
+        sleep_stages=sleep_stages,
+        reference=ref_channels,
+        method="welch",
+        fmin=0,
+        fmax=25,
+        save=False,
+        picks="eeg",
+        reject_by_annotation=True,
+        n_jobs=-1,
+        verbose=False,
+        n_fft=2048,
+        n_per_seg=768,
+        n_overlap=512,
+        window="hamming",
+    )
+
+    if min_psd is None and max_psd is None:
+        min_psd, max_psd = _get_min_max_psds(s_pipe.psds, hypno_psd_pick)
+
+    win_sec = s_pipe.mne_raw.n_times / s_pipe.sf / 900
+    s_pipe.plot_hypnospectrogram(
+        picks=hypno_psd_pick,
+        win_sec=win_sec,
+        freq_range=(0, 25),
+        cmap="Spectral_r",
+        overlap=True,
+        axis=ax_hypno,
+    )
+    r = max_psd - min_psd
+    s_pipe.plot_psds(
+        picks=hypno_psd_pick,
+        psd_range=(min_psd - 0.1 * r, max_psd + 0.1 * r),
+        freq_range=(0, 25),
+        dB=True,
+        xscale="linear",
+        axis=ax_psd,
+        legend_args=dict(loc="upper right", fontsize="medium"),
+    )
+    return min_psd, max_psd
+
+
+def _topo(s_pipe, ref_channels, sleep_stages, topo_axes, topo_lims):
+    if len(sleep_stages) == 1:
+        stages = ["All"] * 4
+        topo_axes[0, 0].set_title(f"Alpha (8-12 Hz)")
+        topo_axes[0, 1].set_title(f"SMR (12-15 Hz)")
+        topo_axes[1, 0].set_title(f"Delta (0.5-4 Hz)")
+        topo_axes[1, 1].set_title(f"Theta (4-8 Hz)")
+    else:
+        stages = ["Wake", "N2", "N3", "REM"]
+        topo_axes[0, 0].set_title(f"{stages[0]}, Alpha (8-12 Hz)")
+        topo_axes[0, 1].set_title(f"{stages[1]}, SMR (12-15 Hz)")
+        topo_axes[1, 0].set_title(f"{stages[2]}, Delta (0.5-4 Hz)")
+        topo_axes[1, 1].set_title(f"{stages[3]}, Theta (4-8 Hz)")
+
+    if ref_channels != "average":
+        s_pipe.compute_psds_per_stage(
+            sleep_stages=sleep_stages,
+            reference="average",
+            method="welch",
+            fmin=0,
+            fmax=25,
+            save=False,
+            picks="eeg",
+            reject_by_annotation=True,
+            n_jobs=-1,
+            verbose=False,
+            n_fft=2048,
+            n_per_seg=2048,
+            n_overlap=1024,
+            window="hamming",
+        )
+
+    s_pipe.plot_topomap(
+        stage=stages[0],
+        band={"Alpha": (8, 12)},
+        dB=False,
+        axis=topo_axes[0, 0],
+        topomap_args=dict(cmap="plasma", vlim=topo_lims[0]),
+        cbar_args=None,
+    )
+
+    s_pipe.plot_topomap(
+        stage=stages[1],
+        band={"SMR": (12, 15)},
+        dB=False,
+        axis=topo_axes[0, 1],
+        topomap_args=dict(cmap="plasma", vlim=topo_lims[1]),
+        cbar_args=None,
+    )
+
+    s_pipe.plot_topomap(
+        stage=stages[2],
+        band={"Delta": (0.5, 4)},
+        dB=False,
+        axis=topo_axes[1, 0],
+        topomap_args=dict(cmap="plasma", vlim=topo_lims[2]),
+        cbar_args=None,
+    )
+
+    s_pipe.plot_topomap(
+        stage=stages[3],
+        band={"Theta": (4, 8)},
+        dB=False,
+        axis=topo_axes[1, 1],
+        topomap_args=dict(cmap="plasma", vlim=topo_lims[3]),
+        cbar_args=None,
+    )
+
+
 def create_dashboard(
     subject_code: str | os.PathLike,
-    path_to_mff: str | os.PathLike,
-    resampling_freq: float,
-    path_to_hypnogram: str | os.PathLike,
-    hypno_freq: float,
+    path_to_eeg: str | os.PathLike,
+    path_to_hypnogram: str | os.PathLike | None,
+    hypno_freq: float | None,
     path_to_bad_channels: str | os.PathLike,
     path_to_annotations: str | os.PathLike,
-    bandpass_filter_freqs: Iterable[float | None],
-    reference: str,
     output_dir: str | os.PathLike,
-    sleep_stages: dict = {"Wake": 0, "N1": 1, "N2/3": (2, 3), "REM": 4},
+    reference: str,
+    resampling_freq: float | None = None,
+    bandpass_filter_freqs: Iterable[float | None] = None,
+    hypno_psd_pick: Iterable[str] | str = ["E101"],
     path_to_ica_fif: str | os.PathLike = None,
     save_fif: bool = False,
+    topomap_cbar_limits: Sequence[tuple[float, float]] | None = None,
 ):
     """Applies cleaning, runs psd analyses and plots them on the dashboard.
 
     Args:
         subject_code: Subject code
-        path_to_mff: Path to the raw mff file
+        path_to_eeg: Path to the raw mff file
         resampling_freq: New frequency in Hz
         path_to_hypnogram: Path to the hypnogram yasa-style hypnogram
         hypno_freq: Sampling rate of the hypnogram in Hz.
         path_to_bad_channels: Path to bad_channels.txt saved by plot() method.
         path_to_annotations: Path to annotations saved by plot() method.
         bandpass_filter_freqs: Lower and upper bounds of the filter.
         reference: Reference to apply. Can be "mastoids", "average" or "VREF".
         output_dir: Directory to save the dashboard image in.
         sleep_stages: Mapping between stage names and indices in hypnogram.
             Defaults to {"Wake": 0, "N1": 1, "N2/3": (2, 3), "REM": 4}.
         path_to_ica_fif: Path to ica components file. Defaults to None.
         save_fif: Whether to save cleaned fif. Defaults to False.
     """
-    from sleepeeg.pipeline import CleaningPipe, SpectralPipe
-    import matplotlib.pyplot as plt
-    import time
-    from mne.io.pick import _picks_to_idx
-    from mne import pick_types
-
-    if reference == "mastoids":
-        ref_channels = ["E94", "E190"]
-    elif reference == "average":
-        ref_channels = "average"
-    elif reference == "VREF":
-        ref_channels = ["VREF"]
+
+    if bandpass_filter_freqs is None:
+        bandpass_filter_freqs = [None, None]
+    if topomap_cbar_limits is None:
+        topomap_cbar_limits = [(None, None)] * 4
+        is_adaptive_topo = True
+    else:
+        is_adaptive_topo = False
+
+    if isinstance(reference, str):
+        if reference.lower() == "mastoids":
+            reference = "Mastoids"
+            ref_channels = ["E94", "E190"]
+        elif reference.lower() == "average":
+            reference = "Average"
+            ref_channels = "average"
+        elif reference.lower() == "vref":
+            reference = "VREF"
+            ref_channels = ["VREF"]
+        else:
+            raise ValueError(
+                f"reference should be either 'average', 'VREF' or 'mastoids'"
+            )
+    else:
+        raise TypeError(f"reference type should be str, but got {type(reference)}")
 
     fig = plt.figure(layout="constrained", figsize=(1600 / 96, 1200 / 96), dpi=96)
     gs = fig.add_gridspec(5, 4)
     info_subfig = fig.add_subfigure(gs[0:2, 0:2])
     topo_subfig = fig.add_subfigure(gs[0:2, 2:4])
     info_axes = info_subfig.subplots(1, 2)
     topo_axes = topo_subfig.subplots(2, 2)
@@ -76,68 +263,43 @@
     gs_s_aft = spectrum_after.add_gridspec(3, 1)
     hypno_before = spectrum_before.add_subplot(gs_s_bef[0:1])
     hypno_after = spectrum_after.add_subplot(gs_s_aft[0:1])
     psd_before = spectrum_before.add_subplot(gs_s_bef[1:3])
     psd_after = spectrum_after.add_subplot(gs_s_aft[1:3])
 
     fig.suptitle(f"Dashboard <{subject_code}>")
-    spectrum_before.suptitle("Spectra after filtering")
-    spectrum_after.suptitle("Spectra after removing bad channels & epochs")
-
-    pipe = CleaningPipe(path_to_eeg=path_to_mff, output_dir=output_dir)
-    # pipe.mne_raw.load_data()
-    pipe.resample(sfreq=resampling_freq, n_jobs=-1)
-    pipe.filter(
-        l_freq=bandpass_filter_freqs[0], h_freq=bandpass_filter_freqs[1], n_jobs=-1
-    )
-    notch_freqs = np.arange(50, int(pipe.sf / 2), 50)
-    pipe.notch(freqs=notch_freqs, n_jobs=-1)
-    pipe.set_eeg_reference(ref_channels=ref_channels)
-    s_pipe = SpectralPipe(
-        prec_pipe=pipe,
-        path_to_hypno=path_to_hypnogram,
-        hypno_freq=hypno_freq,
+    pick = (
+        hypno_psd_pick
+        if isinstance(hypno_psd_pick, str)
+        else ", ".join(str(x) for x in hypno_psd_pick)
+    )
+    spectrum_before.suptitle(f"Spectra after filtering ({pick})")
+    spectrum_after.suptitle(f"Spectra after removing bad channels & epochs ({pick})")
+
+    pipe = CleaningPipe(path_to_eeg=path_to_eeg, output_dir=output_dir)
+
+    sfreq, fmin, fmax, notch_freqs = _filter(
+        pipe,
+        resampling_freq,
+        bandpass_filter_freqs[0],
+        bandpass_filter_freqs[1],
     )
 
-    s_pipe.compute_psds_per_stage(
-        sleep_stages=sleep_stages,
-        reference=ref_channels,
-        method="welch",
-        fmin=0,
-        fmax=25,
-        save=False,
-        picks="eeg",
-        reject_by_annotation=True,
-        n_jobs=-1,
-        verbose=False,
-        n_fft=2048,
-        n_per_seg=768,
-        n_overlap=512,
-        window="hamming",
-    )
+    pipe.set_eeg_reference(ref_channels=ref_channels)
 
-    win_sec = s_pipe.mne_raw.n_times / s_pipe.sf / 900
-    s_pipe.plot_hypnospectrogram(
-        picks=["E101"],
-        win_sec=win_sec,
-        freq_range=(0, 25),
-        cmap="Spectral_r",
-        overlap=True,
-        axis=hypno_before,
-    )
-    min_psd, max_psd = get_min_max_psds(s_pipe.psds, ["E101"])
-    r = max_psd - min_psd
-    s_pipe.plot_psds(
-        picks=["E101"],
-        psd_range=(min_psd - 0.1 * r, max_psd + 0.1 * r),
-        freq_range=(0, 25),
-        dB=True,
-        xscale="linear",
-        axis=psd_before,
-        legend_args=dict(loc="upper right", fontsize="medium"),
+    s_pipe, sleep_stages = _init_s_pipe(pipe, path_to_hypnogram, hypno_freq)
+    min_psd, max_psd = _hypno_psd(
+        s_pipe,
+        sleep_stages,
+        ref_channels,
+        hypno_psd_pick,
+        hypno_before,
+        psd_before,
+        min_psd=None,
+        max_psd=None,
     )
 
     pipe.read_bad_channels(path=path_to_bad_channels)
     bads = pipe.mne_raw.info["bads"]
     pipe.interpolate_bads(reset_bads=True)
     pipe.read_annotations(path=path_to_annotations)
 
@@ -146,15 +308,15 @@
         from sleepeeg.pipeline import ICAPipe
 
         is_ica = True
         pipe = ICAPipe(prec_pipe=pipe, path_to_ica=path_to_ica_fif)
         pipe.apply()
 
     if save_fif:
-        pipe.save_raw(fname="dashboard_cleaned_raw.fif")
+        pipe.save_raw(fname="dashboard_cleaned_raw.fif", overwrite=True)
 
     interpolated = _picks_to_idx(pipe.mne_raw.info, bads)
     pipe.plot_sensors(
         legend=["", "", "", "", "", "", "Interpolated", ""],
         axes=info_axes[0],
         legend_args=dict(loc="lower left", bbox_to_anchor=(-0.1, 0), fontsize="small"),
         ch_groups=[[], [], [], [], [], [], interpolated, []],
@@ -175,124 +337,44 @@
     interpolated_channels_percent = round(
         100 * len(interpolated) / len(pick_types(pipe.mne_raw.info, eeg=True)), 2
     )
 
     textstr = "\n\n".join(
         (
             f"Recording duration: {recording_time}",
-            f"Sampling frequency: {resampling_freq} Hz",
+            f"Sampling frequency: {sfreq} Hz",
             f"Bad epochs: {bad_epochs_percent}%",
             f"Interpolated channels: {interpolated_channels_percent}%",
             f"EEG reference: {reference}",
-            f"Band-pass filter: [{bandpass_filter_freqs[0]}, {bandpass_filter_freqs[1]}] Hz",
-            f"Notch filter: {set(notch_freqs)} Hz",
+            f"Band-pass filter: [{round(fmin, 2)}, {round(fmax, 2)}] Hz",
+            f"Notch filter: {set(notch_freqs) if notch_freqs else notch_freqs} Hz",
             f"ICA performed: {'Yes' if is_ica else 'No'}",
+            f"Adaptive topomaps: {'Yes' if is_adaptive_topo else 'No'}",
         )
     )
     info_axes[1].set_axis_off()
     info_axes[1].text(
         0,
         0.5,
         textstr,
         transform=info_axes[1].transAxes,
         fontsize="large",
         verticalalignment="center",
         horizontalalignment="left",
     )
 
-    s_pipe = SpectralPipe(
-        prec_pipe=pipe,
-        path_to_hypno=path_to_hypnogram,
-        hypno_freq=hypno_freq,
-    )
+    s_pipe, sleep_stages = _init_s_pipe(pipe, path_to_hypnogram, hypno_freq)
 
-    s_pipe.compute_psds_per_stage(
-        sleep_stages=sleep_stages,
-        reference=ref_channels,
-        method="welch",
-        fmin=0,
-        fmax=25,
-        save=False,
-        picks="eeg",
-        reject_by_annotation=True,
-        n_jobs=-1,
-        verbose=False,
-        n_fft=2048,
-        n_per_seg=768,
-        n_overlap=512,
-        window="hamming",
+    _hypno_psd(
+        s_pipe,
+        sleep_stages,
+        ref_channels,
+        hypno_psd_pick,
+        hypno_after,
+        psd_after,
+        min_psd,
+        max_psd,
     )
 
-    s_pipe.plot_hypnospectrogram(
-        picks=["E101"],
-        win_sec=win_sec,
-        freq_range=(0, 25),
-        cmap="Spectral_r",
-        overlap=True,
-        axis=hypno_after,
-    )
-
-    s_pipe.plot_psds(
-        picks=["E101"],
-        psd_range=(min_psd - 0.1 * r, max_psd + 0.1 * r),
-        freq_range=(0, 25),
-        dB=True,
-        xscale="linear",
-        axis=psd_after,
-        legend_args=dict(loc="upper right", fontsize="medium"),
-    )
-    if ref_channels != "average":
-        s_pipe.compute_psds_per_stage(
-            sleep_stages=sleep_stages,
-            reference="average",
-            method="welch",
-            fmin=0,
-            fmax=25,
-            save=False,
-            picks="eeg",
-            reject_by_annotation=True,
-            n_jobs=-1,
-            verbose=False,
-            n_fft=2048,
-            n_per_seg=2048,
-            n_overlap=1024,
-            window="hamming",
-        )
-    topo_axes[0, 0].set_title("Wake, Alpha (8-12 Hz)")
-    s_pipe.plot_topomap(
-        stage="Wake",
-        band={"Alpha": (8, 12)},
-        dB=False,
-        axis=topo_axes[0, 0],
-        topomap_args=dict(cmap="plasma"),
-        cbar_args=None,
-    )
-
-    topo_axes[0, 1].set_title("N2, SMR (12-15 Hz)")
-    s_pipe.plot_topomap(
-        stage="N2",
-        band={"SMR": (12, 15)},
-        dB=False,
-        axis=topo_axes[0, 1],
-        topomap_args=dict(cmap="plasma"),
-        cbar_args=None,
-    )
-    topo_axes[1, 0].set_title("N3, Delta (0.5-4 Hz)")
-    s_pipe.plot_topomap(
-        stage="N3",
-        band={"Delta": (0.5, 4)},
-        dB=False,
-        axis=topo_axes[1, 0],
-        topomap_args=dict(cmap="plasma"),
-        cbar_args=None,
-    )
-    topo_axes[1, 1].set_title("REM, Theta (4-8 Hz)")
-    s_pipe.plot_topomap(
-        stage="REM",
-        band={"Theta": (4, 8)},
-        dB=False,
-        axis=topo_axes[1, 1],
-        topomap_args=dict(cmap="plasma"),
-        cbar_args=None,
-    )
+    _topo(s_pipe, ref_channels, sleep_stages, topo_axes, topomap_cbar_limits)
 
     fig.savefig(f"{output_dir}/dashboard_{subject_code}.png")
```

### Comparing `sleepeeg-0.2.2/sleepeeg/pipeline.py` & `sleepeeg-0.2.3/sleepeeg/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,18 +75,21 @@
     @logger_wraps()
     def notch(self, freqs: str | Iterable[float] = "50s", **notch_kwargs):
         """A wrapper for :py:meth:`mne:mne.io.Raw.notch_filter`.
 
         Args:
             **notch_kwargs: Arguments passed to :py:meth:`mne:mne.io.Raw.notch_filter`.
         """
-        if freqs == "50s":
-            freqs = np.arange(50, int(self.sf / 2), 50)
-        elif freqs == "60s":
-            freqs = np.arange(50, int(self.sf / 2), 50)
+        if isinstance(freqs, str):
+            if freqs == "50s":
+                freqs = np.arange(50, int(self.sf / 2), 50)
+            elif freqs == "60s":
+                freqs = np.arange(50, int(self.sf / 2), 50)
+            else:
+                raise ValueError(f"Unsupported frequency: {freqs}")
         self.mne_raw.load_data().notch_filter(freqs=freqs, **notch_kwargs)
 
     def read_bad_channels(self, path: str | None = None):
         """Imports bad channels from file to mne raw object.
 
         Args:
             path: Path to the txt file with bad channel name per row. Defaults to None.
```

### Comparing `sleepeeg-0.2.2/sleepeeg.egg-info/PKG-INFO` & `sleepeeg-0.2.3/sleepeeg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepeeg
-Version: 0.2.2
+Version: 0.2.3
 Summary: Sleep EEG preprocessing and analysis
 Author-email: Gennadiy Belonosov <gennadiyb@mail.tau.ac.il>
 License: MIT
 Project-URL: Homepage, https://github.com/NirLab-TAU/sleepeeg
 Project-URL: Documentation, https://nirlab-tau.github.io/sleepeeg/
 Keywords: sleep,eeg
 Requires-Python: >=3.10
```

