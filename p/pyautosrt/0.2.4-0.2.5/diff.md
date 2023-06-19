# Comparing `tmp/pyautosrt-0.2.4.tar.gz` & `tmp/pyautosrt-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyautosrt-0.2.4.tar", last modified: Sun Jun 18 20:11:44 2023, max compression
+gzip compressed data, was "pyautosrt-0.2.5.tar", last modified: Mon Jun 19 03:17:50 2023, max compression
```

## Comparing `pyautosrt-0.2.4.tar` & `pyautosrt-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 20:11:44.623683 pyautosrt-0.2.4/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 pyautosrt-0.2.4/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 pyautosrt-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2055 2023-06-18 20:11:44.624433 pyautosrt-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     3452 2023-04-24 17:27:22.000000 pyautosrt-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 20:11:44.565839 pyautosrt-0.2.4/pyautosrt/
--rw-rw-rw-   0        0        0   232104 2023-06-18 20:11:08.000000 pyautosrt-0.2.4/pyautosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 20:11:44.606454 pyautosrt-0.2.4/pyautosrt.egg-info/
--rw-rw-rw-   0        0        0     2055 2023-06-18 20:11:44.000000 pyautosrt-0.2.4/pyautosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-06-18 20:11:44.000000 pyautosrt-0.2.4/pyautosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 20:11:44.000000 pyautosrt-0.2.4/pyautosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-18 20:11:44.000000 pyautosrt-0.2.4/pyautosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      114 2023-06-18 20:11:44.000000 pyautosrt-0.2.4/pyautosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-18 20:11:44.000000 pyautosrt-0.2.4/pyautosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-18 20:11:44.626681 pyautosrt-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1850 2023-06-11 02:57:09.000000 pyautosrt-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 20:11:44.622185 pyautosrt-0.2.4/test/
--rw-rw-rw-   0        0        0    40142 2023-04-15 02:08:42.000000 pyautosrt-0.2.4/test/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:17:50.305583 pyautosrt-0.2.5/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 pyautosrt-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 pyautosrt-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2055 2023-06-19 03:17:50.306332 pyautosrt-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3452 2023-04-24 17:27:22.000000 pyautosrt-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 03:17:50.251640 pyautosrt-0.2.5/pyautosrt/
+-rw-rw-rw-   0        0        0   222764 2023-06-19 03:16:45.000000 pyautosrt-0.2.5/pyautosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:17:50.289101 pyautosrt-0.2.5/pyautosrt.egg-info/
+-rw-rw-rw-   0        0        0     2055 2023-06-19 03:17:49.000000 pyautosrt-0.2.5/pyautosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-06-19 03:17:50.000000 pyautosrt-0.2.5/pyautosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 03:17:49.000000 pyautosrt-0.2.5/pyautosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-19 03:17:49.000000 pyautosrt-0.2.5/pyautosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      114 2023-06-19 03:17:49.000000 pyautosrt-0.2.5/pyautosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-19 03:17:49.000000 pyautosrt-0.2.5/pyautosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-19 03:17:50.309333 pyautosrt-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1850 2023-06-11 02:57:09.000000 pyautosrt-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 03:17:50.304085 pyautosrt-0.2.5/test/
+-rw-rw-rw-   0        0        0    40142 2023-04-15 02:08:42.000000 pyautosrt-0.2.5/test/__init__.py
```

### Comparing `pyautosrt-0.2.4/LICENSE` & `pyautosrt-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.2.4/PKG-INFO` & `pyautosrt-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautosrt
-Version: 0.2.4
+Version: 0.2.5
 Summary: pyautosrt is a python based desktop app to generate subtitle and translated subtitle file
 Home-page: https://github.com/botbahlul/pyautosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `pyautosrt-0.2.4/README.md` & `pyautosrt-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.2.4/pyautosrt/__init__.py` & `pyautosrt-0.2.5/pyautosrt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,280 +37,15 @@
 import shlex
 
 #import warnings
 #warnings.filterwarnings("ignore", category=DeprecationWarning)
 #warnings.filterwarnings("ignore", category=RuntimeWarning)
 #sys.tracebacklimit = 0
 
-VERSION = "0.2.4"
-
-
-#======================================================== ffmpeg_progress_yield ========================================================#
-
-
-import re
-#import subprocess
-from typing import Any, Callable, Iterator, List, Optional, Union
-
-
-def to_ms(**kwargs: Union[float, int, str]) -> int:
-    hour = int(kwargs.get("hour", 0))
-    minute = int(kwargs.get("min", 0))
-    sec = int(kwargs.get("sec", 0))
-    ms = int(kwargs.get("ms", 0))
-
-    return (hour * 60 * 60 * 1000) + (minute * 60 * 1000) + (sec * 1000) + ms
-
-
-def _probe_duration(cmd: List[str]) -> Optional[int]:
-    '''
-    Get the duration via ffprobe from input media file
-    in case ffmpeg was run with loglevel=error.
-
-    Args:
-        cmd (List[str]): A list of command line elements, e.g. ["ffmpeg", "-i", ...]
-
-    Returns:
-        Optional[int]: The duration in milliseconds.
-    '''
-
-    def _get_file_name(cmd: List[str]) -> Optional[str]:
-        try:
-            idx = cmd.index("-i")
-            return cmd[idx + 1]
-        except ValueError:
-            return None
-
-    file_name = _get_file_name(cmd)
-    if file_name is None:
-        return None
-
-    try:
-        if sys.platform == "win32":
-            output = subprocess.check_output(
-                [
-                    "ffprobe",
-                    "-loglevel",
-                    "-1",
-                    "-hide_banner",
-                    "-show_entries",
-                    "format=duration",
-                    "-of",
-                    "default=noprint_wrappers=1:nokey=1",
-                    file_name,
-                ],
-                universal_newlines=True,
-                creationflags=subprocess.CREATE_NO_WINDOW,
-            )
-        else:
-            output = subprocess.check_output(
-                [
-                    "ffprobe",
-                    "-loglevel",
-                    "-1",
-                    "-hide_banner",
-                    "-show_entries",
-                    "format=duration",
-                    "-of",
-                    "default=noprint_wrappers=1:nokey=1",
-                    file_name,
-                ],
-                universal_newlines=True,
-            )
-
-        return int(float(output.strip()) * 1000)
-    except Exception:
-        # TODO: add logging
-        return None
-
-
-def _uses_error_loglevel(cmd: List[str]) -> bool:
-    try:
-        idx = cmd.index("-loglevel")
-        if cmd[idx + 1] == "error":
-            return True
-        else:
-            return False
-    except ValueError:
-        return False
-
-
-class FfmpegProgress:
-    DUR_REGEX = re.compile(
-        r"Duration: (?P<hour>\d{2}):(?P<min>\d{2}):(?P<sec>\d{2})\.(?P<ms>\d{2})"
-    )
-    TIME_REGEX = re.compile(
-        r"out_time=(?P<hour>\d{2}):(?P<min>\d{2}):(?P<sec>\d{2})\.(?P<ms>\d{2})"
-    )
-
-    def __init__(self, cmd: List[str], dry_run: bool = False) -> None:
-        '''Initialize the FfmpegProgress class.
-
-        Args:
-            cmd (List[str]): A list of command line elements, e.g. ["ffmpeg", "-i", ...]
-            dry_run (bool, optional): Only show what would be done. Defaults to False.
-        '''
-        self.cmd = cmd
-        self.stderr: Union[str, None] = None
-        self.dry_run = dry_run
-        self.process: Any = None
-        self.stderr_callback: Union[Callable[[str], None], None] = None
-        if sys.platform == "win32":
-            self.base_popen_kwargs = {
-                "stdin": subprocess.PIPE,  # Apply stdin isolation by creating separate pipe.
-                "stdout": subprocess.PIPE,
-                "stderr": subprocess.STDOUT,
-                "universal_newlines": False,
-                "shell": True,
-            }
-        else:
-            self.base_popen_kwargs = {
-                "stdin": subprocess.PIPE,  # Apply stdin isolation by creating separate pipe.
-                "stdout": subprocess.PIPE,
-                "stderr": subprocess.STDOUT,
-                "universal_newlines": False,
-            }
-
-    def set_stderr_callback(self, callback: Callable[[str], None]) -> None:
-        '''
-        Set a callback function to be called on stderr output.
-        The callback function must accept a single string argument.
-        Note that this is called on every line of stderr output, so it can be called a lot.
-        Also note that stdout/stderr are joined into one stream, so you might get stdout output in the callback.
-
-        Args:
-            callback (Callable[[str], None]): A callback function that accepts a single string argument.
-        '''
-        if not callable(callback) or len(callback.__code__.co_varnames) != 1:
-            raise ValueError(
-                "Callback must be a function that accepts only one argument"
-            )
-
-        self.stderr_callback = callback
-
-    def run_command_with_progress(
-        self, popen_kwargs=None, duration_override: Union[float, None] = None
-    ) -> Iterator[int]:
-        '''
-        Run an ffmpeg command, trying to capture the process output and calculate
-        the duration / progress.
-        Yields the progress in percent.
-
-        Args:
-            popen_kwargs (dict, optional): A dict to specify extra arguments to the popen call, e.g. { creationflags: CREATE_NO_WINDOW }
-            duration_override (float, optional): The duration in seconds. If not specified, it will be calculated from the ffmpeg output.
-
-        Raises:
-            RuntimeError: If the command fails, an exception is raised.
-
-        Yields:
-            Iterator[int]: A generator that yields the progress in percent.
-        '''
-        if self.dry_run:
-            return self.cmd
-
-        total_dur: Union[None, int] = None
-        if _uses_error_loglevel(self.cmd):
-            total_dur = _probe_duration(self.cmd)
-
-        cmd_with_progress = (
-            [self.cmd[0]] + ["-progress", "-", "-nostats"] + self.cmd[1:]
-        )
-
-        stderr = []
-        base_popen_kwargs = self.base_popen_kwargs.copy()
-        if popen_kwargs is not None:
-            base_popen_kwargs.update(popen_kwargs)
-
-        if sys.platform == "win32":
-            self.process = subprocess.Popen(
-                cmd_with_progress,
-                **base_popen_kwargs,
-                creationflags=subprocess.CREATE_NO_WINDOW,
-            )  # type: ignore
-        else:
-            self.process = subprocess.Popen(
-                cmd_with_progress,
-                **base_popen_kwargs,
-            )  # type: ignore
-
-        yield 0
-
-        while True:
-            if self.process.stdout is None:
-                continue
-
-            stderr_line = (
-                self.process.stdout.readline().decode("utf-8", errors="replace").strip()
-            )
-
-            if self.stderr_callback:
-                self.stderr_callback(stderr_line)
-
-            if stderr_line == '' and self.process.poll() is not None:
-                break
-
-            stderr.append(stderr_line.strip())
-
-            self.stderr = "\n".join(stderr)
-
-            if total_dur is None:
-                total_dur_match = self.DUR_REGEX.search(stderr_line)
-                if total_dur_match:
-                    total_dur = to_ms(**total_dur_match.groupdict())
-                    continue
-                elif duration_override is not None:
-                    # use the override (should apply in the first loop)
-                    total_dur = int(duration_override * 1000)
-                    continue
-
-            if total_dur:
-                progress_time = FfmpegProgress.TIME_REGEX.search(stderr_line)
-                if progress_time:
-                    elapsed_time = to_ms(**progress_time.groupdict())
-                    yield int(elapsed_time * 100/ total_dur)
-
-        if self.process is None or self.process.returncode != 0:
-            #print(self.process)
-            #print(self.process.returncode)
-            _pretty_stderr = "\n".join(stderr)
-            raise RuntimeError(f"Error running command {self.cmd}: {_pretty_stderr}")
-
-        yield 100
-        self.process = None
-
-    def quit_gracefully(self) -> None:
-        '''
-        Quit the ffmpeg process by sending 'q'
-
-        Raises:
-            RuntimeError: If no process is found.
-        '''
-        if self.process is None:
-            raise RuntimeError("No process found. Did you run the command?")
-
-        self.process.communicate(input=b"q")
-        self.process.kill()
-        self.process = None
-
-    def quit(self) -> None:
-        '''
-        Quit the ffmpeg process by sending SIGKILL.
-
-        Raises:
-            RuntimeError: If no process is found.
-        '''
-        if self.process is None:
-            raise RuntimeError("No process found. Did you run the command?")
-
-        self.process.kill()
-        self.process = None
-
-
-#=============================================================== autosrt ===============================================================#
+VERSION = "0.2.5"
 
 
 def stop_ffmpeg_windows(error_messages_callback=None):
     try:
         tasklist_output = subprocess.check_output(['tasklist'], creationflags=subprocess.CREATE_NO_WINDOW).decode('utf-8')
         ffmpeg_pid = None
         for line in tasklist_output.split('\n'):
@@ -396,15 +131,26 @@
 
 
 def check_file_type(file_path, error_messages_callback=None):
     try:
         if "\\" in file_path:
             file_path = file_path.replace("\\", "/")
 
-        ffprobe_cmd = ['ffprobe', '-v', '-1', '-loglevel', '-1', '-hide_banner', '-show_format', '-show_streams', '-print_format', 'json', file_path]
+        ffprobe_cmd = [
+                        'ffprobe',
+                        '-hide_banner',
+                        '-v', 'error',
+                        '-loglevel', 'error',
+                        '-show_format',
+                        '-show_streams',
+                        '-print_format',
+                        'json',
+                        file_path
+                      ]
+
         output = None
 
         if sys.platform == "win32":
             output = subprocess.check_output(ffprobe_cmd, stdin=open(os.devnull), stderr=subprocess.PIPE, creationflags=subprocess.CREATE_NO_WINDOW).decode('utf-8')
         else:
             output = subprocess.check_output(ffprobe_cmd, stdin=open(os.devnull), stderr=subprocess.PIPE).decode('utf-8')
 
@@ -1172,49 +918,43 @@
             if self.error_messages_callback:
                 self.error_messages_callback("ffmpeg: Executable not found on machine.")
             else:
                 print("ffmpeg: Executable not found on machine.")
                 raise Exception("Dependency not found: ffmpeg")
 
         ffmpeg_command = [
-                            "ffmpeg",
-                            "-hide_banner",
-                            "-loglevel", "-1",
-                            "-v", "-1",
-                            "-y",
-                            "-i", media_filepath,
-                            "-ac", str(self.channels),
-                            "-ar", str(self.rate),
-                            "-progress", "-", "-nostats",
+                            'ffmpeg',
+                            '-hide_banner',
+                            '-loglevel', 'error',
+                            '-v', 'error',
+                            '-y',
+                            '-i', media_filepath,
+                            '-ac', str(self.channels),
+                            '-ar', str(self.rate),
+                            '-progress', '-', '-nostats',
                             temp.name
                          ]
 
         try:
-            # RUNNING ffmpeg WITHOUT SHOWING PROGRESSS
-            #use_shell = True if os.name == "nt" else False
-            #subprocess.check_output(command, stdin=open(os.devnull), shell=use_shell)
-
             media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
             info = f"Converting '{media_file_display_name}' to a temporary WAV file"
             start_time = time.time()
 
-            '''
-            # RUNNING ffmpeg WITH PROGRESSS
-            ff = FfmpegProgress(ffmpeg_command)
-            percentage = 0
-            for progress in ff.run_command_with_progress():
-                percentage = progress
-                if self.progress_callback:
-                    self.progress_callback(info, media_file_display_name, percentage, start_time)
-            '''
-
-
-            # RUNNING ffmpeg_command WITHOUT ffmpeg_progress_yield
-            ffprobe_command = f'ffprobe -v -1 -loglevel -1 -hide_banner -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+            ffprobe_command = [
+                                'ffprobe',
+                                '-hide_banner',
+                                '-v', 'error',
+                                '-loglevel', 'error',
+                                '-show_entries',
+                                'format=duration',
+                                '-of', 'default=noprint_wrappers=1:nokey=1',
+                                media_filepath
+                              ]
 
+            ffprobe_process = None
             if sys.platform == "win32":
                 ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
                 ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
 
             total_duration = float(ffprobe_process.strip())
 
@@ -1258,19 +998,19 @@
                 self.error_messages_callback(f"WavConverter : {e}")
             else:
                 print(f"WavConverter : {e}")
             return
 
 # DEFINE progress_callback FUNCTION TO SHOW ffmpeg PROGRESS
 # IF WE'RE IN pysimplegui ENVIRONMENT WE CAN DO :
-#def show_progress(percentage):
+#def show_progress(info, media_file_display_name, percentage, start_time):
     #global main_window
     #main_window.write_event_value('-UPDATE-PROGRESS-', percentage) AND HANDLE THAT EVENT IN pysimplegui MAIN LOOP
 # IF WE'RE IN console ENVIRONMENT WE CAN DO :
-#def show_progress(percentage):
+#def show_progress(info, media_file_display_name, percentage, start_time):
     #global pbar
     #pbar.update(percentage)
 
 # DEFINE error_messages_callback FUNCTION TO SHOW ERROR MESSAGES
 # IF WE'RE IN pysimplegui ENVIRONMENT WE CAN DO :
 #def show_error_messages(messages):
     #global main_window
@@ -1354,29 +1094,32 @@
             if "\\" in self.wav_filepath:
                 self.wav_filepath = self.wav_filepath.replace("\\", "/")
 
             start, end = region
             start = max(0, start - self.include_before)
             end += self.include_after
             temp = tempfile.NamedTemporaryFile(suffix='.flac', delete=False)
+
             command = [
-                        "ffmpeg",
-                        "-hide_banner",
-                        "-loglevel", "-1",
-                        "-v", "-1",
-                        "-ss", str(start),
-                        "-t", str(end - start),
-                        "-y",
-                        "-i", self.wav_filepath,
+                        'ffmpeg',
+                        '-hide_banner',
+                        '-loglevel', 'error',
+                        '-v', 'error',
+                        '-ss', str(start),
+                        '-t', str(end - start),
+                        '-y',
+                        '-i', self.wav_filepath,
                         temp.name
                       ]
+
             if sys.platform == "win32":
                 subprocess.check_output(command, stdin=open(os.devnull), creationflags=subprocess.CREATE_NO_WINDOW)
             else:
                 subprocess.check_output(command, stdin=open(os.devnull))
+
             content = temp.read()
             temp.close()
             return content
 
         except KeyboardInterrupt:
             if self.error_messages_callback:
                 self.error_messages_callback("Cancelling all tasks")
@@ -1730,19 +1473,20 @@
             self._timed_subtitles.append(self.get_timed_subtitles(media_filepath, subtitle_stream_index+1))
             subtitle_data.append((index, language, self.get_timed_subtitles(media_filepath, subtitle_stream_index+1)))
 
         self._number_of_streams = len(subtitle_data)
         return subtitle_data
 
     def get_subtitle_streams(self, media_filepath):
+
         ffprobe_cmd = [
                         'ffprobe',
                         '-hide_banner',
-                        '-v', '-1',
-                        '-loglevel', '-1',
+                        '-v', 'error',
+                        '-loglevel', 'error',
                         '-print_format', 'json',
                         '-show_entries', 'stream=index:stream_tags=language',
                         '-select_streams', 's',
                         media_filepath
                       ]
 
         try:
@@ -1785,19 +1529,20 @@
             if self.error_messages_callback:
                 self.error_messages_callback(e)
             else:
                 print(e)
             return None
 
     def get_timed_subtitles(self, media_filepath, subtitle_stream_index):
+
         ffmpeg_cmd = [
                         'ffmpeg',
                         '-hide_banner',
-                        '-loglevel', '-1',
-                        '-v', '-1',
+                        '-loglevel', 'error',
+                        '-v', 'error',
                         '-i', media_filepath,
                         '-map', f'0:s:{subtitle_stream_index-1}',
                         '-f', 'srt',
                         '-'
                      ]
 
         try:
@@ -1952,54 +1697,52 @@
             else:
                 print("ffmpeg: Executable not found on machine.")
                 raise Exception("Dependency not found: ffmpeg")
 
         try:
             scale_switch = "'trunc(iw/2)*2'\:'trunc(ih/2)*2'"
             ffmpeg_command = [
-                                "ffmpeg",
-                                "-hide_banner",
-                                "-loglevel", "-1",
-                                "-v", "-1",
-                                "-y",
-                                "-i", media_filepath,
-                                "-vf", f"subtitles={shlex.quote(subtitle_path_str)},scale={scale_switch}",
-                                "-c:v", "libx264",
-                                "-crf", "23",
-                                "-preset", "medium",
-                                "-c:a", "copy",
-                                "-progress", "-", "-nostats",
+                                'ffmpeg',
+                                '-hide_banner',
+                                '-loglevel', 'error',
+                                '-v', 'error',
+                                '-y',
+                                '-i', media_filepath,
+                                '-vf', f'subtitles={shlex.quote(subtitle_path_str)},scale={scale_switch}',
+                                '-c:v', 'libx264',
+                                '-crf', '23',
+                                '-preset', 'medium',
+                                '-c:a', 'copy',
+                                '-progress', '-', '-nostats',
                                 self.output_path
                              ]
 
             media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
             info = f"Rendering subtitles file into '{media_file_display_name}'"
             start_time = time.time()
 
-            '''
-            # RUNNING ffmpeg WITH ffmpeg_progress_yield
-            ff = FfmpegProgress(ffmpeg_command)
-            percentage = 0
-            for progress in ff.run_command_with_progress():
-                percentage = progress
-                if self.progress_callback:
-                    self.progress_callback(info, media_file_display_name, percentage, start_time)
-            '''
-
-            # RUNNING ffmpeg_command WITHOUT ffmpeg_progress_yield
-            ffprobe_command = f'ffprobe -v -1 -loglevel -1 -hide_banner -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+            ffprobe_command = [
+                                'ffprobe',
+                                '-hide_banner',
+                                '-v', 'error',
+                                '-loglevel', 'error',
+                                '-show_entries',
+                                'format=duration',
+                                '-of', 'default=noprint_wrappers=1:nokey=1',
+                                media_filepath
+                              ]
 
+            ffprobe_process = None
             if sys.platform == "win32":
                 ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
                 ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
 
             total_duration = float(ffprobe_process.strip())
 
-
             process = None
             if sys.platform == "win32":
                 process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
                 process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
 
             while True:
@@ -2076,16 +1819,16 @@
         # Run ffprobe to get stream information
         if "\\" in media_filepath:
             media_filepath = media_filepath.replace("\\", "/")
 
         command = [
                     'ffprobe',
                     '-hide_banner',
-                    '-v', '-1',
-                    '-loglevel', '-1',
+                    '-v', 'error',
+                    '-loglevel', 'error',
                     '-of', 'json',
                     '-show_entries',
                     'format:stream',
                     media_filepath
                   ]
 
         output = None
@@ -2143,16 +1886,16 @@
             else:
                 # Determine the next available subtitle index
                 next_index = len(existing_languages)
 
                 ffmpeg_command = [
                                     'ffmpeg',
                                     '-hide_banner',
-                                    '-loglevel', '-1',
-                                    '-v', '-1',
+                                    '-loglevel', 'error',
+                                    '-v', 'error',
                                     '-y',
                                     '-i', media_filepath,
                                     '-sub_charenc', 'UTF-8',
                                     '-i', self.subtitle_path,
                                     '-c:v', 'copy',
                                     '-c:a', 'copy',
                                     '-scodec', 'mov_text',
@@ -2164,35 +1907,33 @@
                                  ]
 
                 subtitle_file_display_name = os.path.basename(self.subtitle_path).split('/')[-1]
                 media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
                 info = f"Embedding '{self.language}' subtitles file '{subtitle_file_display_name}' into '{media_file_display_name}'"
                 start_time = time.time()
 
-                '''
-                # USING ffmpeg_progress_yield MODULE
-                ff = FfmpegProgress(ffmpeg_command)
-                percentage = 0
-                for progress in ff.run_command_with_progress():
-                    percentage = progress
-                    if self.progress_callback:
-                        self.progress_callback(info, media_file_display_name, percentage, start_time)
-                '''
-
-                # RUNNING ffmpeg_command WITHOUT ffmpeg_progress_yield
-                ffprobe_command = f'ffprobe -v -1 -loglevel -1 -hide_banner -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+                ffprobe_command = [
+                                    'ffprobe',
+                                    '-hide_banner',
+                                    '-v', 'error',
+                                    '-loglevel', 'error',
+                                    '-show_entries',
+                                    'format=duration',
+                                    '-of', 'default=noprint_wrappers=1:nokey=1',
+                                    media_filepath
+                                  ]
 
+                ffprobe_process = None
                 if sys.platform == "win32":
                     ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
                 else:
                     ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
 
                 total_duration = float(ffprobe_process.strip())
 
-
                 process = None
                 if sys.platform == "win32":
                     process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
                 else:
                     process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
 
                 while True:
@@ -2288,42 +2029,40 @@
                 print("ffmpeg: Executable not found on machine.")
                 raise Exception("Dependency not found: ffmpeg")
 
         try:
             ffmpeg_command = [
                                 'ffmpeg',
                                 '-hide_banner',
-                                '-loglevel', '-1',
-                                '-v', '-1',
+                                '-loglevel', 'error',
+                                '-v', 'error',
                                 '-y',
                                 '-i', media_filepath,
                                 '-c', 'copy',
                                 '-sn',
                                 '-progress', '-', '-nostats',
                                 self.output_path
                              ]
 
             media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
             info = f"Removing subtitle streams from '{media_file_display_name}'"
             start_time = time.time()
 
-            '''
-            # USING ffmpeg_progress_yield MODULE
-            ff = FfmpegProgress(ffmpeg_command)
-            percentage = 0
-            for progress in ff.run_command_with_progress():
-                percentage = progress
-                if self.progress_callback:
-                    self.progress_callback(info, media_file_display_name, percentage, start_time)
-            '''
-
-
-            # RUNNING ffmpeg_command WITHOUT ffmpeg_progress_yield
-            ffprobe_command = f'ffprobe -v -1 -loglevel -1 -hide_banner -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+            ffprobe_command = [
+                                'ffprobe',
+                                '-hide_banner',
+                                '-v', 'error',
+                                '-loglevel', 'error',
+                                '-show_entries',
+                                'format=duration',
+                                '-of', 'default=noprint_wrappers=1:nokey=1',
+                                media_filepath
+                              ]
 
+            ffprobe_process = None
             if sys.platform == "win32":
                 ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
                 ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
 
             total_duration = float(ffprobe_process.strip())
 
@@ -2575,16 +2314,16 @@
 def record_streaming_windows(hls_url, media_filepath, error_messages_callback=None):
     global not_recording, main_window
 
     try:
         ffmpeg_cmd = [
                         'ffmpeg',
                         '-hide_banner',
-                        '-loglevel', '-1',
-                        '-v', '-1',
+                        '-loglevel', 'error',
+                        '-v', 'error',
                         '-y',
                         '-i', hls_url,
                         '-movflags', '+frag_keyframe+separate_moof+omit_tfhd_offset+empty_moov',
                         '-fflags', 'nobuffer',
                         media_filepath
                      ]
 
@@ -2621,16 +2360,16 @@
 def record_streaming_linux(url, output_file, error_messages_callback=None):
     global recognizing, ffmpeg_start_run_time, first_streaming_duration_recorded, main_window
 
     #ffmpeg_cmd = ['ffmpeg', '-y', '-i', url, '-c', 'copy', '-bsf:a', 'aac_adtstoasc', '-f', 'mp4', output_file]
     ffmpeg_cmd = [
                     'ffmpeg',
                     '-hide_banner',
-                    '-loglevel', '-1',
-                    '-v', '-1',
+                    '-loglevel', 'error',
+                    '-v', 'error',
                     '-y',
                     '-i', f'{url}',
                     '-movflags',
                     '+frag_keyframe+separate_moof+omit_tfhd_offset+empty_moov',
                     '-fflags',
                     'nobuffer',
                     f'{output_file}'
```

### Comparing `pyautosrt-0.2.4/pyautosrt.egg-info/PKG-INFO` & `pyautosrt-0.2.5/pyautosrt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyautosrt
-Version: 0.2.4
+Version: 0.2.5
 Summary: pyautosrt is a python based desktop app to generate subtitle and translated subtitle file
 Home-page: https://github.com/botbahlul/pyautosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `pyautosrt-0.2.4/setup.py` & `pyautosrt-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `pyautosrt-0.2.4/test/__init__.py` & `pyautosrt-0.2.5/test/__init__.py`

 * *Files identical despite different names*

