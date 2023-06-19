# Comparing `tmp/autosrt-1.3.9.tar.gz` & `tmp/autosrt-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.3.9.tar", last modified: Wed Jun  7 20:06:20 2023, max compression
+gzip compressed data, was "autosrt-1.4.1.tar", last modified: Mon Jun 19 08:17:42 2023, max compression
```

## Comparing `autosrt-1.3.9.tar` & `autosrt-1.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 20:06:20.641807 autosrt-1.3.9/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.3.9/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.3.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2018 2023-06-07 20:06:20.641807 autosrt-1.3.9/PKG-INFO
--rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.3.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 20:06:20.603597 autosrt-1.3.9/autosrt/
--rw-rw-rw-   0        0        0   115678 2023-06-07 20:05:48.000000 autosrt-1.3.9/autosrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 20:06:20.626822 autosrt-1.3.9/autosrt.egg-info/
--rw-rw-rw-   0        0        0     2018 2023-06-07 20:06:20.000000 autosrt-1.3.9/autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-06-07 20:06:20.000000 autosrt-1.3.9/autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 20:06:20.000000 autosrt-1.3.9/autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-07 20:06:20.000000 autosrt-1.3.9/autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2023-06-07 20:06:20.000000 autosrt-1.3.9/autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-07 20:06:20.000000 autosrt-1.3.9/autosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-07 20:06:20.645555 autosrt-1.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 20:06:20.638810 autosrt-1.3.9/test/
--rw-rw-rw-   0        0        0     7435 2023-06-06 20:34:53.000000 autosrt-1.3.9/test/test1.py
--rw-rw-rw-   0        0        0     4481 2023-06-06 20:37:56.000000 autosrt-1.3.9/test/test2.py
--rw-rw-rw-   0        0        0     9938 2023-06-06 20:52:44.000000 autosrt-1.3.9/test/test3.py
--rw-rw-rw-   0        0        0    68819 2023-05-09 15:49:36.000000 autosrt-1.3.9/test/test4.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:17:42.376718 autosrt-1.4.1/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.4.1/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2018 2023-06-19 08:17:42.377467 autosrt-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 08:17:42.287563 autosrt-1.4.1/autosrt/
+-rw-rw-rw-   0        0        0   156840 2023-06-19 08:16:44.000000 autosrt-1.4.1/autosrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:17:42.323528 autosrt-1.4.1/autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2018 2023-06-19 08:17:41.000000 autosrt-1.4.1/autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-06-19 08:17:42.000000 autosrt-1.4.1/autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 08:17:41.000000 autosrt-1.4.1/autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-19 08:17:41.000000 autosrt-1.4.1/autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-06-19 08:17:41.000000 autosrt-1.4.1/autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-19 08:17:41.000000 autosrt-1.4.1/autosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-19 08:17:42.380467 autosrt-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:17:42.375220 autosrt-1.4.1/test/
+-rw-rw-rw-   0        0        0     7435 2023-06-06 20:34:53.000000 autosrt-1.4.1/test/test1.py
+-rw-rw-rw-   0        0        0     4481 2023-06-06 20:37:56.000000 autosrt-1.4.1/test/test2.py
+-rw-rw-rw-   0        0        0     9938 2023-06-06 20:52:44.000000 autosrt-1.4.1/test/test3.py
+-rw-rw-rw-   0        0        0    68818 2023-06-16 20:05:01.000000 autosrt-1.4.1/test/test4.py
```

### Comparing `autosrt-1.3.9/LICENSE` & `autosrt-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.9/PKG-INFO` & `autosrt-1.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.3.9
+Version: 1.4.1
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.3.9/README.md` & `autosrt-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.9/autosrt/__init__.py` & `autosrt-1.4.1/autosrt/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -23,15 +23,282 @@
 from glob import glob, escape
 import time
 from datetime import datetime, timedelta
 from pathlib import Path
 import shlex
 import shutil
 
-VERSION = "1.3.9"
+
+VERSION = "1.4.1"
+
+
+#======================================================== ffmpeg_progress_yield ========================================================#
+
+
+import re
+import subprocess
+from typing import Any, Callable, Iterator, List, Optional, Union
+
+
+def to_ms(**kwargs: Union[float, int, str]) -> int:
+    hour = int(kwargs.get("hour", 0))
+    minute = int(kwargs.get("min", 0))
+    sec = int(kwargs.get("sec", 0))
+    ms = int(kwargs.get("ms", 0))
+
+    return (hour * 60 * 60 * 1000) + (minute * 60 * 1000) + (sec * 1000) + ms
+
+
+def _probe_duration(cmd: List[str]) -> Optional[int]:
+    '''
+    Get the duration via ffprobe from input media file
+    in case ffmpeg was run with loglevel=error.
+
+    Args:
+        cmd (List[str]): A list of command line elements, e.g. ["ffmpeg", "-i", ...]
+
+    Returns:
+        Optional[int]: The duration in milliseconds.
+    '''
+
+    def _get_file_name(cmd: List[str]) -> Optional[str]:
+        try:
+            idx = cmd.index("-i")
+            return cmd[idx + 1]
+        except ValueError:
+            return None
+
+    file_name = _get_file_name(cmd)
+    if file_name is None:
+        return None
+
+    try:
+        if sys.platform == "win32":
+            output = subprocess.check_output(
+                [
+                    "ffprobe",
+                    "-loglevel",
+                    "-1",
+                    "-hide_banner",
+                    "-show_entries",
+                    "format=duration",
+                    "-of",
+                    "default=noprint_wrappers=1:nokey=1",
+                    file_name,
+                ],
+                universal_newlines=True,
+                creationflags=subprocess.CREATE_NO_WINDOW,
+            )
+        else:
+            output = subprocess.check_output(
+                [
+                    "ffprobe",
+                    "-loglevel",
+                    "-1",
+                    "-hide_banner",
+                    "-show_entries",
+                    "format=duration",
+                    "-of",
+                    "default=noprint_wrappers=1:nokey=1",
+                    file_name,
+                ],
+                universal_newlines=True,
+            )
+
+        return int(float(output.strip()) * 1000)
+    except Exception:
+        # TODO: add logging
+        return None
+
+
+def _uses_error_loglevel(cmd: List[str]) -> bool:
+    try:
+        idx = cmd.index("-loglevel")
+        if cmd[idx + 1] == "error":
+            return True
+        else:
+            return False
+    except ValueError:
+        return False
+
+
+class FfmpegProgress:
+    DUR_REGEX = re.compile(
+        r"Duration: (?P<hour>\d{2}):(?P<min>\d{2}):(?P<sec>\d{2})\.(?P<ms>\d{2})"
+    )
+    TIME_REGEX = re.compile(
+        r"out_time=(?P<hour>\d{2}):(?P<min>\d{2}):(?P<sec>\d{2})\.(?P<ms>\d{2})"
+    )
+
+    def __init__(self, cmd: List[str], dry_run: bool = False) -> None:
+        '''Initialize the FfmpegProgress class.
+
+        Args:
+            cmd (List[str]): A list of command line elements, e.g. ["ffmpeg", "-i", ...]
+            dry_run (bool, optional): Only show what would be done. Defaults to False.
+        '''
+        self.cmd = cmd
+        self.stderr: Union[str, None] = None
+        self.dry_run = dry_run
+        self.process: Any = None
+        self.stderr_callback: Union[Callable[[str], None], None] = None
+        if sys.platform == "win32":
+            self.base_popen_kwargs = {
+                "stdin": subprocess.PIPE,  # Apply stdin isolation by creating separate pipe.
+                "stdout": subprocess.PIPE,
+                "stderr": subprocess.STDOUT,
+                "universal_newlines": False,
+                "shell": True,
+            }
+        else:
+            self.base_popen_kwargs = {
+                "stdin": subprocess.PIPE,  # Apply stdin isolation by creating separate pipe.
+                "stdout": subprocess.PIPE,
+                "stderr": subprocess.STDOUT,
+                "universal_newlines": False,
+            }
+
+    def set_stderr_callback(self, callback: Callable[[str], None]) -> None:
+        '''
+        Set a callback function to be called on stderr output.
+        The callback function must accept a single string argument.
+        Note that this is called on every line of stderr output, so it can be called a lot.
+        Also note that stdout/stderr are joined into one stream, so you might get stdout output in the callback.
+
+        Args:
+            callback (Callable[[str], None]): A callback function that accepts a single string argument.
+        '''
+        if not callable(callback) or len(callback.__code__.co_varnames) != 1:
+            raise ValueError(
+                "Callback must be a function that accepts only one argument"
+            )
+
+        self.stderr_callback = callback
+
+    def run_command_with_progress(
+        self, popen_kwargs=None, duration_override: Union[float, None] = None
+    ) -> Iterator[int]:
+        '''
+        Run an ffmpeg command, trying to capture the process output and calculate
+        the duration / progress.
+        Yields the progress in percent.
+
+        Args:
+            popen_kwargs (dict, optional): A dict to specify extra arguments to the popen call, e.g. { creationflags: CREATE_NO_WINDOW }
+            duration_override (float, optional): The duration in seconds. If not specified, it will be calculated from the ffmpeg output.
+
+        Raises:
+            RuntimeError: If the command fails, an exception is raised.
+
+        Yields:
+            Iterator[int]: A generator that yields the progress in percent.
+        '''
+        if self.dry_run:
+            return self.cmd
+
+        total_dur: Union[None, int] = None
+        if _uses_error_loglevel(self.cmd):
+            total_dur = _probe_duration(self.cmd)
+
+        cmd_with_progress = (
+            [self.cmd[0]] + ["-progress", "-", "-nostats"] + self.cmd[1:]
+        )
+
+        stderr = []
+        base_popen_kwargs = self.base_popen_kwargs.copy()
+        if popen_kwargs is not None:
+            base_popen_kwargs.update(popen_kwargs)
+
+        if sys.platform == "win32":
+            self.process = subprocess.Popen(
+                cmd_with_progress,
+                **base_popen_kwargs,
+                creationflags=subprocess.CREATE_NO_WINDOW,
+            )  # type: ignore
+        else:
+            self.process = subprocess.Popen(
+                cmd_with_progress,
+                **base_popen_kwargs,
+            )  # type: ignore
+
+        yield 0
+
+        while True:
+            if self.process.stdout is None:
+                continue
+
+            stderr_line = (
+                self.process.stdout.readline().decode("utf-8", errors="replace").strip()
+            )
+
+            if self.stderr_callback:
+                self.stderr_callback(stderr_line)
+
+            if stderr_line == '' and self.process.poll() is not None:
+                break
+
+            stderr.append(stderr_line.strip())
+
+            self.stderr = "\n".join(stderr)
+
+            if total_dur is None:
+                total_dur_match = self.DUR_REGEX.search(stderr_line)
+                if total_dur_match:
+                    total_dur = to_ms(**total_dur_match.groupdict())
+                    continue
+                elif duration_override is not None:
+                    # use the override (should apply in the first loop)
+                    total_dur = int(duration_override * 1000)
+                    continue
+
+            if total_dur:
+                progress_time = FfmpegProgress.TIME_REGEX.search(stderr_line)
+                if progress_time:
+                    elapsed_time = to_ms(**progress_time.groupdict())
+                    yield int(elapsed_time * 100/ total_dur)
+
+        if self.process is None or self.process.returncode != 0:
+            #print(self.process)
+            #print(self.process.returncode)
+            _pretty_stderr = "\n".join(stderr)
+            raise RuntimeError(f"Error running command {self.cmd}: {_pretty_stderr}")
+
+        yield 100
+        self.process = None
+
+    def quit_gracefully(self) -> None:
+        '''
+        Quit the ffmpeg process by sending 'q'
+
+        Raises:
+            RuntimeError: If no process is found.
+        '''
+        if self.process is None:
+            raise RuntimeError("No process found. Did you run the command?")
+
+        self.process.communicate(input=b"q")
+        self.process.kill()
+        self.process = None
+
+    def quit(self) -> None:
+        '''
+        Quit the ffmpeg process by sending SIGKILL.
+
+        Raises:
+            RuntimeError: If no process is found.
+        '''
+        if self.process is None:
+            raise RuntimeError("No process found. Did you run the command?")
+
+        self.process.kill()
+        self.process = None
+
+
+#=======================================================================================================================================#
+
 
 def stop_ffmpeg_windows(error_messages_callback=None):
     try:
         tasklist_output = subprocess.check_output(['tasklist'], creationflags=subprocess.CREATE_NO_WINDOW).decode('utf-8')
         ffmpeg_pid = None
         for line in tasklist_output.split('\n'):
             if "ffmpeg" in line:
@@ -113,28 +380,42 @@
         else:
             print(e)
         return
 
 
 def check_file_type(media_filepath, error_messages_callback=None):
     try:
-        ffprobe_cmd = ['ffprobe', '-v', 'error', '-show_format', '-show_streams', '-print_format', 'json', media_filepath]
+        ffprobe_cmd = [
+                        'ffprobe',
+                        '-hide_banner',
+                        '-loglevel', 'error',
+                        '-v', 'error',
+                        '-show_format',
+                        '-show_streams',
+                        '-print_format',
+                        'json',
+                        media_filepath
+                      ]
+
         output = None
+
         if sys.platform == "win32":
-            output = subprocess.check_output(ffprobe_cmd, creationflags=subprocess.CREATE_NO_WINDOW).decode('utf-8')
+            output = subprocess.check_output(ffprobe_cmd, stdin=open(os.devnull), stderr=subprocess.PIPE, creationflags=subprocess.CREATE_NO_WINDOW).decode('utf-8')
         else:
-            output = subprocess.check_output(ffprobe_cmd).decode('utf-8')
+            output = subprocess.check_output(ffprobe_cmd, stdin=open(os.devnull), stderr=subprocess.PIPE).decode('utf-8')
+
         data = json.loads(output)
 
         if 'streams' in data:
             for stream in data['streams']:
                 if 'codec_type' in stream and stream['codec_type'] == 'audio':
                     return 'audio'
                 elif 'codec_type' in stream and stream['codec_type'] == 'video':
                     return 'video'
+
     except (subprocess.CalledProcessError, json.JSONDecodeError):
         pass
 
     except Exception as e:
         if error_messages_callback:
             error_messages_callback(e)
         else:
@@ -886,64 +1167,73 @@
             if self.error_messages_callback:
                 self.error_messages_callback("ffmpeg: Executable not found on machine.")
             else:
                 print("ffmpeg: Executable not found on machine.")
                 raise Exception("Dependency not found: ffmpeg")
 
         ffmpeg_command = [
-                            "ffmpeg",
-                            "-y",
-                            "-i", media_filepath,
-                            "-ac", str(self.channels),
-                            "-ar", str(self.rate),
-                            "-loglevel", "error",
-                            "-hide_banner",
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
-            '''
-            # RUNNING ffmpeg WITH PROGRESSS
-            ff = FfmpegProgress(command)
-            percentage = 0
-            for progress in ff.run_command_with_progress():
-                percentage = progress
-                if self.progress_callback:
-                    self.progress_callback(media_filepath, percentage)
-            temp.close()
-            '''
+            media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
+            info = f"Converting '{media_file_display_name}' to a temporary WAV file"
+            start_time = time.time()
+
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
 
-            ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+            ffprobe_process = None
             if sys.platform == "win32":
-                ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+                ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
-                ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+                ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
 
-            total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
+            total_duration = float(ffprobe_process.strip())
 
+            process = None
             if sys.platform == "win32":
-                process = subprocess.Popen(ffmpeg_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+                process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
-                process = subprocess.Popen(ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+                process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+            while True:
+                if process.stdout is None:
+                    continue
+
+                stderr_line = (process.stdout.readline().decode("utf-8", errors="replace").strip())
+ 
+                if stderr_line == '' and process.poll() is not None:
+                    break
+
+                if "out_time=" in stderr_line:
+                    time_str = stderr_line.split('time=')[1].split()[0]
+                    current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
 
-            for line in process.stdout:
-                if "time=" in line:
-                    #print(line)
-                    time_str = line.split("time=")[1].split()[0]
-                    #print("time_str = %s" %time_str)
-                    current_duration = sum(float(x) * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
-                    #print("current_duration = %s" %current_duration)
                     if current_duration>0:
-                        percentage = int(current_duration*100/total_duration)
+                        percentage = int(current_duration*100/(int(float(total_duration))*1000))
                         if self.progress_callback:
-                            self.progress_callback(media_filepath, percentage)
+                            self.progress_callback(info, media_file_display_name, percentage, start_time)
 
             temp.close()
 
             return temp.name, self.rate
 
         except KeyboardInterrupt:
             if self.error_messages_callback:
@@ -956,14 +1246,34 @@
             if self.error_messages_callback:
                 self.error_messages_callback(e)
             else:
                 print(e)
             return
 
 
+# DEFINE progress_callback FUNCTION TO SHOW ffmpeg PROGRESS
+# IF WE'RE IN pysimplegui ENVIRONMENT WE CAN DO :
+#def show_progress(info, media_file_display_name, percentage, start_time):
+    #global main_window
+    #main_window.write_event_value('-UPDATE-PROGRESS-', percentage) AND HANDLE THAT EVENT IN pysimplegui MAIN LOOP
+# IF WE'RE IN console ENVIRONMENT WE CAN DO :
+#def show_progress(info, media_file_display_name, percentage, start_time):
+    #global pbar
+    #pbar.update(percentage)
+
+# DEFINE error_messages_callback FUNCTION TO SHOW ERROR MESSAGES
+# IF WE'RE IN pysimplegui ENVIRONMENT WE CAN DO :
+#def show_error_messages(messages):
+    #global main_window
+    #main_window.write_event_value('-EXCEPTION-', messages) AND HANDLE THAT EVENT IN pysimplegui MAIN LOOP
+# IF WE'RE IN console ENVIRONMENT WE CAN DO :
+#def show_error_messages(messages):
+    #print(messages)
+
+
 class SpeechRegionFinder:
     @staticmethod
     def percentile(arr, percent):
         arr = sorted(arr)
         k = (len(arr) - 1) * percent
         f = math.floor(k)
         c = math.ceil(k)
@@ -1037,24 +1347,32 @@
             if "\\" in self.wav_filepath:
                 self.wav_filepath = self.wav_filepath.replace("\\", "/")
 
             start, end = region
             start = max(0, start - self.include_before)
             end += self.include_after
             temp = tempfile.NamedTemporaryFile(suffix='.flac', delete=False)
+
             command = [
-                        "ffmpeg",
-                        "-ss", str(start),
-                        "-t", str(end - start),
-                        "-y",
-                        "-i", self.wav_filepath,
-                        "-loglevel", "error",
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
-            subprocess.check_output(command, stdin=open(os.devnull))
+
+            if sys.platform == "win32":
+                subprocess.check_output(command, stdin=open(os.devnull), creationflags=subprocess.CREATE_NO_WINDOW)
+            else:
+                subprocess.check_output(command, stdin=open(os.devnull))
+
             content = temp.read()
             temp.close()
             return content
 
         except KeyboardInterrupt:
             if self.error_messages_callback:
                 self.error_messages_callback("Cancelling all tasks")
@@ -1352,25 +1670,33 @@
             self._timed_subtitles.append(self.get_timed_subtitles(media_filepath, subtitle_stream_index+1))
             subtitle_data.append((index, language, self.get_timed_subtitles(media_filepath, subtitle_stream_index+1)))
 
         self._number_of_streams = len(subtitle_data)
         return subtitle_data
 
     def get_subtitle_streams(self, media_filepath):
+
         ffprobe_cmd = [
                         'ffprobe',
-                        '-v', 'quiet',
+                        '-hide_banner',
+                        '-v', 'error',
+                        '-loglevel', 'error',
                         '-print_format', 'json',
                         '-show_entries', 'stream=index:stream_tags=language',
                         '-select_streams', 's',
                         media_filepath
                       ]
 
         try:
-            result = subprocess.run(ffprobe_cmd, capture_output=True, text=True)
+            result = None
+            if sys.platform == "win32":
+                result = subprocess.run(ffprobe_cmd, stdin=open(os.devnull), capture_output=True, text=True, creationflags=subprocess.CREATE_NO_WINDOW)
+            else:
+                result = subprocess.run(ffprobe_cmd, stdin=open(os.devnull), capture_output=True, text=True)
+
             output = result.stdout
 
             streams = json.loads(output)['streams']
 
             subtitle_streams = []
             empty_stream_exists = False
 
@@ -1400,56 +1726,64 @@
             if self.error_messages_callback:
                 self.error_messages_callback(e)
             else:
                 print(e)
             return None
 
     def get_timed_subtitles(self, media_filepath, subtitle_stream_index):
+
         ffmpeg_cmd = [
                         'ffmpeg',
+                        '-hide_banner',
+                        '-loglevel', 'error',
+                        '-v', 'error',
                         '-i', media_filepath,
                         '-map', f'0:s:{subtitle_stream_index-1}',
                         '-f', 'srt',
                         '-'
                      ]
 
         try:
-            result = subprocess.run(ffmpeg_cmd, capture_output=True, text=True)
+            result = None
+            if sys.platform == "win32":
+                result = subprocess.run(ffmpeg_cmd, stdin=open(os.devnull), capture_output=True, text=True, creationflags=subprocess.CREATE_NO_WINDOW)
+            else:
+                result = subprocess.run(ffmpeg_cmd, stdin=open(os.devnull), capture_output=True, text=True)
+
             output = result.stdout
-			#print(output)
 
             timed_subtitles = []
             subtitle_data = []
             lines = output.strip().split('\n')
             #print(lines)
             subtitles = []
-            subtitle = None
+            subtitles = None
             subtitle_blocks = []
             block = []
             for line in lines:
                 if line.strip() == '':
                     subtitle_blocks.append(block)
                     block = []
                 else:
                     block.append(line.strip())
             subtitle_blocks.append(block)
 
-            # Parse each subtitle block and store as tuple in timed_subtitles list
+            # Parse each subtitles block and store as tuple in timed_subtitles list
             for block in subtitle_blocks:
                 if block:
-                    # Extract start and end times from subtitle block
+                    # Extract start and end times from subtitles block
                     start_time_str, end_time_str = block[1].split(' --> ')
                     time_format = '%H:%M:%S,%f'
                     start_time_time_delta = datetime.strptime(start_time_str, time_format) - datetime.strptime('00:00:00,000', time_format)
                     start_time_total_seconds = start_time_time_delta.total_seconds()
                     end_time_time_delta = datetime.strptime(end_time_str, time_format) - datetime.strptime('00:00:00,000', time_format)
                     end_time_total_seconds = end_time_time_delta.total_seconds()
-                    # Extract subtitle text from subtitle block
-                    subtitle = ' '.join(block[2:])
-                    timed_subtitles.append(((start_time_total_seconds, end_time_total_seconds), subtitle))
+                    # Extract subtitles text from subtitles block
+                    subtitles = ' '.join(block[2:])
+                    timed_subtitles.append(((start_time_total_seconds, end_time_total_seconds), subtitles))
             return timed_subtitles
 
         except FileNotFoundError:
             if self.error_messages_callback:
                 msg = 'ffmpeg not found. Make sure it is installed and added to the system PATH.'
                 self.error_messages_callback(msg)
             else:
@@ -1514,17 +1848,16 @@
     def ffmpeg_check():
         if MediaSubtitleRenderer.which("ffmpeg"):
             return "ffmpeg"
         if MediaSubtitleRenderer.which("ffmpeg.exe"):
             return "ffmpeg.exe"
         return None
 
-    def __init__(self, subtitle_path=None, language="eng", output_path=None, progress_callback=None, error_messages_callback=None):
+    def __init__(self, subtitle_path=None, output_path=None, progress_callback=None, error_messages_callback=None):
         self.subtitle_path = subtitle_path
-        self.language = language
         self.output_path = output_path
         self.progress_callback = progress_callback
         self.error_messages_callback = error_messages_callback
 
     def __call__(self, media_filepath):
         if "\\" in media_filepath:
             media_filepath = media_filepath.replace("\\", "/")
@@ -1545,53 +1878,77 @@
             if self.error_messages_callback:
                 self.error_messages_callback("ffmpeg: Executable not found on machine.")
             else:
                 print("ffmpeg: Executable not found on machine.")
                 raise Exception("Dependency not found: ffmpeg")
 
         try:
+            scale_switch = "'trunc(iw/2)*2'\:'trunc(ih/2)*2'"
             ffmpeg_command = [
-                                "ffmpeg",
-                                "-y",
-                                "-i", media_filepath,
-                                "-sub_charenc", "UTF-8",
-                                "-i", self.subtitle_path,
-                                "-c:v", "copy",
-                                "-c:a", "copy",
-                                "-scodec", "mov_text",
-                                "-metadata:s:s:0",
-                                f"language={shlex.quote(self.language)}",
-                                "-f", "mp4",
-                                "-y", self.output_path
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
+                                self.output_path
                              ]
 
-            ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+            media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
+            info = f"Rendering subtitles file into '{media_file_display_name}'"
+            start_time = time.time()
+
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
+
+            ffprobe_process = None
             if sys.platform == "win32":
-                ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+                ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
-                ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+                ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
 
-            total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
+            total_duration = float(ffprobe_process.strip())
 
+            process = None
             if sys.platform == "win32":
-                process = subprocess.Popen(ffmpeg_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+                process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
-                process = subprocess.Popen(ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+                process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+            while True:
+                if process.stdout is None:
+                    continue
+
+                stderr_line = (process.stdout.readline().decode("utf-8", errors="replace").strip())
+ 
+                if stderr_line == '' and process.poll() is not None:
+                    break
+
+                if "out_time=" in stderr_line:
+                    time_str = stderr_line.split('time=')[1].split()[0]
+                    current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
 
-            for line in process.stdout:
-                if "time=" in line:
-                    #print(line)
-                    time_str = line.split("time=")[1].split()[0]
-                    #print("time_str = %s" %time_str)
-                    current_duration = sum(float(x) * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
-                    #print("current_duration = %s" %current_duration)
                     if current_duration>0:
-                        percentage = int(current_duration*100/total_duration)
+                        percentage = int(current_duration*100/(int(float(total_duration))*1000))
                         if self.progress_callback:
-                            self.progress_callback(media_filepath, percentage)
+                            self.progress_callback(info, media_file_display_name, percentage, start_time)
 
             if os.path.isfile(self.output_path):
                 return self.output_path
             else:
                 return None
 
         except KeyboardInterrupt:
@@ -1608,16 +1965,16 @@
                 print(e)
             return
 
 
 class MediaSubtitleEmbedder:
     @staticmethod
     def which(program):
-        def is_exe(media_filepath):
-            return os.path.isfile(media_filepath) and os.access(media_filepath, os.X_OK)
+        def is_exe(file_path):
+            return os.path.isfile(file_path) and os.access(file_path, os.X_OK)
         fpath, _ = os.path.split(program)
         if fpath:
             if is_exe(program):
                 return program
         else:
             for path in os.environ["PATH"].split(os.pathsep):
                 path = path.strip('"')
@@ -1630,39 +1987,42 @@
     def ffmpeg_check():
         if MediaSubtitleEmbedder.which("ffmpeg"):
             return "ffmpeg"
         if MediaSubtitleEmbedder.which("ffmpeg.exe"):
             return "ffmpeg.exe"
         return None
 
-    def __init__(self, subtitle_path=None, language="eng", output_path=None, progress_callback=None, error_messages_callback=None):
+    def __init__(self, subtitle_path=None, language=None, output_path=None, progress_callback=None, error_messages_callback=None):
         self.subtitle_path = subtitle_path
         self.language = language
         self.output_path = output_path
         self.progress_callback = progress_callback
         self.error_messages_callback = error_messages_callback
 
     def get_existing_subtitle_language(self, media_filepath):
         # Run ffprobe to get stream information
         if "\\" in media_filepath:
             media_filepath = media_filepath.replace("\\", "/")
 
         command = [
                     'ffprobe',
-                    '-v', 'quiet',
+                    '-hide_banner',
+                    '-v', 'error',
+                    '-loglevel', 'error',
                     '-of', 'json',
                     '-show_entries',
                     'format:stream',
                     media_filepath
                   ]
 
+        output = None
         if sys.platform == "win32":
-            output = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, universal_newlines=True)
+            output = subprocess.run(command, stdin=open(os.devnull), stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
         else:
-            output = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True)
+            output = subprocess.run(command, stdin=open(os.devnull), stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True)
 
         metadata = json.loads(output.stdout)
         streams = metadata['streams']
 
         # Find the subtitle stream with language metadata
         subtitle_languages = []
         for stream in streams:
@@ -1708,63 +2068,78 @@
 
             else:
                 # Determine the next available subtitle index
                 next_index = len(existing_languages)
 
                 ffmpeg_command = [
                                     'ffmpeg',
+                                    '-hide_banner',
+                                    '-loglevel', 'error',
+                                    '-v', 'error',
                                     '-y',
                                     '-i', media_filepath,
                                     '-sub_charenc', 'UTF-8',
                                     '-i', self.subtitle_path,
                                     '-c:v', 'copy',
                                     '-c:a', 'copy',
                                     '-scodec', 'mov_text',
                                     '-metadata:s:s:' + str(next_index), f'language={shlex.quote(self.language)}',
                                     '-map', '0',
                                     '-map', '1',
+                                    '-progress', '-', '-nostats',
                                     self.output_path
                                  ]
 
+                subtitle_file_display_name = os.path.basename(self.subtitle_path).split('/')[-1]
+                media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
+                info = f"Embedding '{self.language}' subtitles file '{subtitle_file_display_name}' into '{media_file_display_name}'"
+                start_time = time.time()
+
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
 
-                '''
-                # USING ffmpeg_progress_yield MODULE
-                ff = FfmpegProgress(ffmpeg_command)
-                percentage = 0
-                for progress in ff.run_command_with_progress():
-                    percentage = progress
-                    if self.progress_callback:
-                        self.progress_callback(media_filepath, percentage)
-                '''
-
-                # WITHOUT USING ffmpeg_progress_yield MODULE
-                ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
+                ffprobe_process = None
                 if sys.platform == "win32":
-                    ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+                    ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
                 else:
-                    ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+                    ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
 
-                total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
+                total_duration = float(ffprobe_process.strip())
 
+                process = None
                 if sys.platform == "win32":
-                    process = subprocess.Popen(ffmpeg_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+                    process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
                 else:
-                    process = subprocess.Popen(ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+                    process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+                while True:
+                    if process.stdout is None:
+                        continue
+
+                    stderr_line = (process.stdout.readline().decode("utf-8", errors="replace").strip())
+ 
+                    if stderr_line == '' and process.poll() is not None:
+                        break
+
+                    if "out_time=" in stderr_line:
+                        time_str = stderr_line.split('time=')[1].split()[0]
+                        current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
 
-                for line in process.stdout:
-                    if "time=" in line:
-                        #print(line)
-                        time_str = line.split("time=")[1].split()[0]
-                        #print("time_str = %s" %time_str)
-                        current_duration = sum(float(x) * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
-                        #print("current_duration = %s" %current_duration)
                         if current_duration>0:
-                            percentage = int(current_duration*100/total_duration)
+                            percentage = int(current_duration*100/(int(float(total_duration))*1000))
                             if self.progress_callback:
-                                self.progress_callback(media_filepath, percentage)
+                                self.progress_callback(info, media_file_display_name, percentage, start_time)
 
                 if os.path.isfile(self.output_path):
                     return self.output_path
                 else:
                     return None
 
                 if os.path.isfile(self.output_path):
@@ -1783,52 +2158,188 @@
             if self.error_messages_callback:
                 self.error_messages_callback(e)
             else:
                 print(e)
             return
 
 
+class MediaSubtitleRemover:
+    @staticmethod
+    def which(program):
+        def is_exe(media_filepath):
+            return os.path.isfile(media_filepath) and os.access(media_filepath, os.X_OK)
+        fpath, _ = os.path.split(program)
+        if fpath:
+            if is_exe(program):
+                return program
+        else:
+            for path in os.environ["PATH"].split(os.pathsep):
+                path = path.strip('"')
+                exe_file = os.path.join(path, program)
+                if is_exe(exe_file):
+                    return exe_file
+        return None
+
+    @staticmethod
+    def ffmpeg_check():
+        if MediaSubtitleRemover.which("ffmpeg"):
+            return "ffmpeg"
+        if MediaSubtitleRemover.which("ffmpeg.exe"):
+            return "ffmpeg.exe"
+        return None
+
+    def __init__(self, output_path=None, progress_callback=None, error_messages_callback=None):
+        self.output_path = output_path
+        self.progress_callback = progress_callback
+        self.error_messages_callback = error_messages_callback
+
+    def __call__(self, media_filepath):
+        if "\\" in media_filepath:
+            media_filepath = media_filepath.replace("\\", "/")
+
+        if "\\" in self.output_path:
+            self.output_path = self.output_path.replace("\\", "/")
+
+        if not os.path.isfile(media_filepath):
+            if self.error_messages_callback:
+                self.error_messages_callback("The given file does not exist: {0}".format(media_filepath))
+            else:
+                print("The given file does not exist: {0}".format(media_filepath))
+                raise Exception("Invalid file: {0}".format(media_filepath))
+        if not self.ffmpeg_check():
+            if self.error_messages_callback:
+                self.error_messages_callback("ffmpeg: Executable not found on machine.")
+            else:
+                print("ffmpeg: Executable not found on machine.")
+                raise Exception("Dependency not found: ffmpeg")
+
+        try:
+            ffmpeg_command = [
+                                'ffmpeg',
+                                '-hide_banner',
+                                '-loglevel', 'error',
+                                '-v', 'error',
+                                '-y',
+                                '-i', media_filepath,
+                                '-c', 'copy',
+                                '-sn',
+                                '-progress', '-', '-nostats',
+                                self.output_path
+                             ]
+
+            media_file_display_name = os.path.basename(media_filepath).split('/')[-1]
+            info = f"Removing subtitles streams from '{media_file_display_name}'"
+            start_time = time.time()
+
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
+
+            ffprobe_process = None
+            if sys.platform == "win32":
+                ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
+            else:
+                ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
+
+            total_duration = float(ffprobe_process.strip())
+
+            process = None
+            if sys.platform == "win32":
+                process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
+            else:
+                process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+            while True:
+                if process.stdout is None:
+                    continue
+
+                stderr_line = (process.stdout.readline().decode("utf-8", errors="replace").strip())
+ 
+                if stderr_line == '' and process.poll() is not None:
+                    break
+
+                if "out_time=" in stderr_line:
+                    time_str = stderr_line.split('time=')[1].split()[0]
+                    current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
+
+                    if current_duration>0:
+                        percentage = int(current_duration*100/(int(float(total_duration))*1000))
+                        if self.progress_callback:
+                            self.progress_callback(info, media_file_display_name, percentage, start_time)
+
+            if os.path.isfile(self.output_path):
+                return self.output_path
+            else:
+                return None
+
+            if os.path.isfile(self.output_path):
+                return self.output_path
+            else:
+                return None
+
+        except KeyboardInterrupt:
+            if self.error_messages_callback:
+                self.error_messages_callback("Cancelling all tasks")
+            else:
+                print("Cancelling all tasks")
+            return
+
+        except Exception as e:
+            if self.error_messages_callback:
+                self.error_messages_callback(e)
+            else:
+                print(e)
+            return
+
+
 class SRTFileReader:
     def __init__(self, srt_file_path, error_messages_callback=None):
         self.timed_subtitles = self(srt_file_path)
         self.error_messages_callback = error_messages_callback
 
     @staticmethod
     def __call__(srt_file_path):
         try:
             """
-            Read SRT formatted subtitle file and return subtitles as list of tuples
+            Read SRT formatted subtitles file and return subtitles as list of tuples
             """
             timed_subtitles = []
             with open(srt_file_path, 'r') as srt_file:
                 lines = srt_file.readlines()
-                # Split the subtitle file into subtitle blocks
+                # Split the subtitles file into subtitles blocks
                 subtitle_blocks = []
                 block = []
                 for line in lines:
                     if line.strip() == '':
                         subtitle_blocks.append(block)
                         block = []
                     else:
                         block.append(line.strip())
                 subtitle_blocks.append(block)
 
-                # Parse each subtitle block and store as tuple in timed_subtitles list
+                # Parse each subtitles block and store as tuple in timed_subtitles list
                 for block in subtitle_blocks:
                     if block:
-                        # Extract start and end times from subtitle block
+                        # Extract start and end times from subtitles block
                         start_time_str, end_time_str = block[1].split(' --> ')
                         time_format = '%H:%M:%S,%f'
                         start_time_time_delta = datetime.strptime(start_time_str, time_format) - datetime.strptime('00:00:00,000', time_format)
                         start_time_total_seconds = start_time_time_delta.total_seconds()
                         end_time_time_delta = datetime.strptime(end_time_str, time_format) - datetime.strptime('00:00:00,000', time_format)
                         end_time_total_seconds = end_time_time_delta.total_seconds()
-                        # Extract subtitle text from subtitle block
-                        subtitle = ' '.join(block[2:])
-                        timed_subtitles.append(((start_time_total_seconds, end_time_total_seconds), subtitle))
+                        # Extract subtitles text from subtitles block
+                        subtitles = ' '.join(block[2:])
+                        timed_subtitles.append(((start_time_total_seconds, end_time_total_seconds), subtitles))
                 return timed_subtitles
 
         except KeyboardInterrupt:
             if self.error_messages_callback:
                 self.error_messages_callback("Cancelling all tasks")
             else:
                 print("Cancelling all tasks")
@@ -1844,23 +2355,30 @@
 
 def has_subtitles(media_filepath, error_messages_callback=None):
     try:
         if "\\" in media_filepath:
             media_filepath = media_filepath.replace("\\", "/")
 
         ffmpeg_cmd = [
-            "ffmpeg",
-            "-y",
-            "-i", media_filepath,
-            "-map", "0:s:0",
-            "-f", "srt",
-            "-"
-        ]
+                        'ffmpeg',
+                        '-hide_banner',
+                        '-v', 'error',
+                        '-loglevel', 'error',
+                        '-y',
+                        '-i', media_filepath,
+                        '-map', '0:s:0',
+                        '-f', 'srt',
+                        '-'
+                     ]
 
-        result = subprocess.run(ffmpeg_cmd, capture_output=True, text=True)
+        result = None
+        if sys.platform == "win32":
+            result = subprocess.run(ffmpeg_cmd, stdin=open(os.devnull), capture_output=True, text=True, creationflags=subprocess.CREATE_NO_WINDOW)
+        else:
+            result = subprocess.run(ffmpeg_cmd, stdin=open(os.devnull), capture_output=True, text=True)
 
         if result.stdout:
             return True  # Subtitles detected
         else:
             return False  # No subtitles detected
 
     except Exception as e:
@@ -1871,72 +2389,109 @@
         return False
 
 
 def get_existing_subtitle_language(media_path):
     # Run ffprobe to get stream information
     command = [
                 'ffprobe',
-                '-v', 'quiet',
+                '-hide_banner',
+                '-v', 'error',
+                '-loglevel', 'error',
                 '-of', 'json',
                 '-show_entries',
                 'format:stream',
                 media_path
-    ]
+              ]
+
+    output = None
+    if sys.platform == "win32":
+        output = subprocess.run(command, stdin=open(os.devnull), stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
+    else:
+        output = subprocess.run(command, stdin=open(os.devnull), stdout=subprocess.PIPE, stderr=subprocess.PIPE, universal_newlines=True)
 
-    output = subprocess.run(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, universal_newlines=True)
     metadata = json.loads(output.stdout)
     streams = metadata['streams']
 
-    # Find the subtitle stream with language metadata
+    # Find the subtitles stream with language metadata
     subtitle_languages = []
     for stream in streams:
-        if stream['codec_type'] == 'subtitle' and 'tags' in stream and 'language' in stream['tags']:
+        if stream['codec_type'] == 'subtitles' and 'tags' in stream and 'language' in stream['tags']:
             language = stream['tags']['language']
             subtitle_languages.append(language)
 
     return subtitle_languages
 
 
 def render_subtitle_to_media(media_filepath, media_type, media_ext, subtitle_path, output_path, error_messages_callback=None):
-
     try:
         if "\\" in media_filepath:
             media_filepath = media_filepath.replace("\\", "/")
 
         if "\\" in subtitle_path:
             subtitle_path = subtitle_path.replace("\\", "/")
 
         if "\\" in output_path:
             output_path = output_path.replace("\\", "/")
 
-        ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
-        ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-        total_duration = float(ffprobe_process.stdout.read().decode().strip())
+        scale_switch = "'trunc(iw/2)*2':'trunc(ih/2)*2'"
+        ffmpeg_command = [
+                            'ffmpeg',
+                            '-y',
+                            '-i', media_filepath,
+                            '-vf', f'subtitles={shlex.quote(self.subtitle_path)},scale={scale_switch}',
+                            '-c:v', 'libx264',
+                            '-crf', '23',
+                            '-preset', 'medium',
+                            '-c:a', 'copy',
+                            self.output_path
+                         ]
+
+        ffprobe_command = [
+                            'ffprobe',
+                            '-hide_banner',
+                            '-v', 'error',
+                            '-loglevel', 'error',
+                            '-show_entries',
+                            'format=duration',
+                            '-of', 'default=noprint_wrappers=1:nokey=1',
+                            media_filepath
+                          ]
+
+        ffprobe_process = None
+        if sys.platform == "win32":
+            ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
+        else:
+            ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
 
-        ffmpeg_command = f'ffmpeg -y -i "{media_filepath}" -vf "subtitles={shlex.quote(subtitle_path)}" "{output_path}"'
+        total_duration = float(ffprobe_process.strip())
 
-        widgets = [f"Rendering subtitles into {media_type} : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+        widgets = [f"Rendering '{language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
         pbar = ProgressBar(widgets=widgets, maxval=100).start()
         percentage = 0
 
+        process = None
         if sys.platform == "win32":
-            process = subprocess.Popen(ffmpeg_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+            process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
         else:
-            process = subprocess.Popen(ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+            process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+        while True:
+            if process.stdout is None:
+                continue
+
+            stderr_line = (process.stdout.readline().decode("utf-8", errors="replace").strip())
+ 
+            if stderr_line == '' and process.poll() is not None:
+                break
 
-        for line in process.stdout:
-            if "time=" in line:
-                #print(line)
-                time_str = line.split("time=")[1].split()[0]
-                #print("time_str = %s" %time_str)
-                current_duration = sum(float(x) * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
-                #print("current_duration = %s" %current_duration)
+            if "out_time=" in stderr_line:
+                time_str = stderr_line.split('time=')[1].split()[0]
+                current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
                 if current_duration>0:
-                    percentage = int(current_duration*100/total_duration)
-                    #print("percentage = {}%".format(percentage))
+                    percentage = int(current_duration*100/(int(float(total_duration))*1000))
                     pbar.update(percentage)
         pbar.finish()
         return output_path
 
     except Exception as e:
         if error_messages_callback:
             error_messages_callback(e)
@@ -1954,105 +2509,212 @@
             subtitle_path = subtitle_path.replace("\\", "/")
 
         if "\\" in output_path:
             output_path = output_path.replace("\\", "/")
 
         existing_languages = get_existing_subtitle_language(media_filepath)
         if language_code in existing_languages:
-            #print(f"'{language_code}' subtitle stream already existed in {media_filepath}")
+            #print(f"'{language_code}' subtitles stream already existed in {media_filepath}")
             return
 
         else:
-            # Determine the next available subtitle index
+            # Determine the next available subtitles index
             next_index = len(existing_languages)
 
-            ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
-            if sys.platform == "win32":
-                ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-            else:
-                ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-
-            total_duration = float(ffprobe_process.stdout.read().decode('utf-8').strip())
-
             ffmpeg_command = [
                                 'ffmpeg',
+                                '-hide_banner',
+                                '-loglevel', 'error',
+                                '-v', 'error',
                                 '-y',
                                 '-i', media_filepath,
                                 '-sub_charenc', 'UTF-8',
                                 '-i', subtitle_path,
                                 '-c:v', 'copy',
                                 '-c:a', 'copy',
                                 '-scodec', 'mov_text',
                                 '-metadata:s:s:' + str(next_index), f'language={shlex.quote(language_code)}',
                                 '-map', '0',
                                 '-map', '1',
                                 output_path
                              ]
 
-            widgets = [f"Embedding \'{language_code}\' subtitles into {media_type}     : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+            ffprobe_command = [
+                                'ffprobe',
+                                '-hide_banner',
+                                '-v', 'error',
+                                '-loglevel', 'error',
+                                '-show_entries',
+                                'format=duration',
+                                '-of', 'default=noprint_wrappers=1:nokey=1',
+                                media_filepath
+                             ]
+
+            ffprobe_process = None
+            if sys.platform == "win32":
+                ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
+            else:
+                ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
+
+            total_duration = float(ffprobe_process.strip())
+
+            widgets = [f"Embedding '{language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
             pbar = ProgressBar(widgets=widgets, maxval=100).start()
             percentage = 0
 
+            process = None
             if sys.platform == "win32":
-                process = subprocess.Popen(ffmpeg_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+                process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
             else:
-                process = subprocess.Popen(ffmpeg_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True)
+                process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
 
-            for line in process.stdout:
-                if "time=" in line:
-                    #print(line)
-                    time_str = line.split("time=")[1].split()[0]
-                    #print("time_str = %s" %time_str)
-                    current_duration = sum(float(x) * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
-                    #print("current_duration = %s" %current_duration)
+            while True:
+                if process.stdout is None:
+                    continue
+
+                stderr_line = (process.stdout.readline().decode("utf-8", errors="replace").strip())
+ 
+                if stderr_line == '' and process.poll() is not None:
+                    break
+
+                if "out_time=" in stderr_line:
+                    time_str = stderr_line.split('time=')[1].split()[0]
+                    current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
                     if current_duration>0:
-                        percentage = int(current_duration*100/total_duration)
-                        #print("percentage = {}%".format(percentage))
+                        percentage = int(current_duration*100/(int(float(total_duration))*1000))
                         pbar.update(percentage)
             pbar.finish()
+
             return output_path
+
         return
 
     except Exception as e:
         if error_messages_callback:
             error_messages_callback(e)
         else:
             print(e)
         return None
 
 
-def show_progress(media_filepath, progress):
+def remove_subtitles_from_media(media_filepath, output_path, progress_callback=None, error_messages_callback=None):
+    try:
+        if "\\" in media_filepath:
+            media_filepath = media_filepath.replace("\\", "/")
+
+        if "\\" in output_path:
+            output_path = output_path.replace("\\", "/")
+
+        ffmpeg_command = [
+                            'ffmpeg',
+                            '-hide_banner',
+                            '-loglevel', 'error',
+                            '-v', 'error',
+                            '-y',
+                            '-i', media_filepath,
+                            '-c', 'copy',
+                            '-sn',
+                            '-progress', '-', '-nostats',
+                            self.output_path
+                         ]
+
+        ffprobe_command = [
+                            'ffprobe',
+                            '-hide_banner',
+                            '-v', 'error',
+                            '-loglevel', 'error',
+                            '-show_entries',
+                            'format=duration',
+                            '-of', 'default=noprint_wrappers=1:nokey=1',
+                            media_filepath
+                          ]
+
+        ffprobe_process = None
+        if sys.platform == "win32":
+            ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
+        else:
+            ffprobe_process = subprocess.check_output(ffprobe_command, stdin=open(os.devnull), universal_newlines=True)
+
+        total_duration = float(ffprobe_process.strip())
+
+        widgets = ["Removing subtitles streams from file    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+        pbar = ProgressBar(widgets=widgets, maxval=100).start()
+        percentage = 0
+
+        process = None
+        if sys.platform == "win32":
+            process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, shell=True, creationflags=subprocess.CREATE_NO_WINDOW)
+        else:
+            process = subprocess.Popen(ffmpeg_command, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+
+        while True:
+            if process.stdout is None:
+                continue
+
+            stderr_line = (process.stdout.readline().decode("utf-8", errors="replace").strip())
+ 
+            if stderr_line == '' and process.poll() is not None:
+                break
+
+            if "out_time=" in stderr_line:
+                time_str = stderr_line.split('time=')[1].split()[0]
+                current_duration = sum(float(x) * 1000 * 60 ** i for i, x in enumerate(reversed(time_str.split(":"))))
+                if current_duration>0:
+                    percentage = int(current_duration*100/(int(float(total_duration))*1000))
+                    pbar.update(percentage)
+        pbar.finish()
+
+        return output_path
+
+    except KeyboardInterrupt:
+        if error_messages_callback:
+            error_messages_callback("Cancelling all tasks")
+        else:
+            print("Cancelling all tasks")
+        return
+
+    except Exception as e:
+        if error_messages_callback:
+            error_messages_callback(e)
+        else:
+            print(e)
+        return
+
+
+def show_progress(info, media_file_display_name, progress, start_time):
     global pbar
     pbar.update(progress)
 
 
 def show_error_messages(messages):
     print(messages)
 
 
 def main():
-    global pbar, pbar2
+    global pbar
 
     if sys.platform == "win32":
         stop_ffmpeg_windows(error_messages_callback=show_error_messages)
     else:
         stop_ffmpeg_linux(error_messages_callback=show_error_messages)
 
     remove_temp_files("flac", error_messages_callback=show_error_messages)
     remove_temp_files("wav", error_messages_callback=show_error_messages)
 
     parser = argparse.ArgumentParser()
-    parser.add_argument('source_path', help="Path to the video or audio files to generate subtitles files (use wildcard for multiple files or separate them with a space character e.g. \"file 1.mp4\" \"file 2.mp4\")", nargs='*')
-    parser.add_argument('-S', '--src-language', help="Language code of the audio language spoken in video/audio source_path", default="en")
+    parser.add_argument('source_path', help="Path to the media files to generate subtitles files (use wildcard for multiple files or separate them with a space character e.g. \"file 1.mp4\" \"file 2.mp4\")", nargs='*')
+    parser.add_argument('-S', '--src-language', help="Language code of the audio language spoken in media file source_path", default="en")
     parser.add_argument('-D', '--dst-language', help="Desired translation language code for the subtitles", default=None)
     parser.add_argument('-ll', '--list-languages', help="List all supported languages", action='store_true')
-    parser.add_argument('-F', '--format', help="Desired subtitle format", default="srt")
-    parser.add_argument('-lf', '--list-formats', help="List all supported subtitle formats", action='store_true')
+    parser.add_argument('-F', '--format', help="Desired subtitles file format", default="srt")
+    parser.add_argument('-lf', '--list-formats', help="List all supported subtitles file formats", action='store_true')
     parser.add_argument('-C', '--concurrency', help="Number of concurrent API requests to make", type=int, default=10)
-    parser.add_argument('-e', '--embed', help="Boolean value (True or False) for embed subtitle file into video file", type=bool, default=False)
+    parser.add_argument('-es', '--embed-src', help="Boolean value (True or False) for embedding original language subtitles file into media file", type=bool, default=False)
+    parser.add_argument('-ed', '--embed-dst', help="Boolean value (True or False) for embedding translated subtitles file into media file", type=bool, default=False)
+    parser.add_argument('-fr', '--force-recognize', help="Boolean value (True or False) for re-recognize media file event if it's already has subtitles stream", type=bool, default=False)
     parser.add_argument('-v', '--version', action='version', version=VERSION)
 
     args = parser.parse_args()
 
     language = Language()
 
     if args.list_languages:
@@ -2077,32 +2739,27 @@
             do_translate = True
         else:
             do_translate = False
     else:
         do_translate = False
 
     if args.list_formats:
-        print("List of supported subtitle formats:")
+        print("List of supported subtitles formats:")
         for subtitle_format in SubtitleFormatter.supported_formats:
             print("{format}".format(format=subtitle_format))
         return 0
 
     if args.format not in SubtitleFormatter.supported_formats:
         print("Subtitle format is not supported. Run with --list-formats to see all supported formats.")
         return 1
 
     if not args.source_path:
         parser.print_help(sys.stderr)
         return 1
 
-    if str(args.embed) == "true":
-        args.embed = True
-    if str(args.embed) == "false":
-        args.embed = False
-
     completed_tasks = 0
     media_filepaths = []
     arg_filepaths = []
     invalid_media_filepaths = []
     not_exist_filepaths = []
     argpath = None
     media_type = None
@@ -2153,15 +2810,15 @@
                     media_type = None
             else:
                 not_exist_filepaths.append(argpath)
                 media_type = None
 
         if invalid_media_filepaths:
             for invalid_media_filepath in invalid_media_filepaths:
-                msg = "{} is not valid video or audio files".format(invalid_media_filepath)
+                msg = "{} is not valid media files".format(invalid_media_filepath)
                 print(msg)
 
     #print("not_exist_filepaths = %s" %(not_exist_filepaths))
 
     if not_exist_filepaths:
         if (not "*" in str(args_source_path)) and (not "?" in str(args_source_path)):
             for not_exist_filepath in not_exist_filepaths:
@@ -2187,168 +2844,334 @@
 
     subtitle_format = args.format
 
     #print("media_filepaths = {}".format(media_filepaths))
 
     removed_media_filepaths = []
 
-    print("CHECKING EXISTING SUBTITLES STREAMS")
-    print("===================================")
+    if args.force_recognize == False:
 
-    if do_translate == False:
+        print("CHECKING EXISTING SUBTITLES STREAMS")
+        print("===================================")
 
-        for media_filepath in media_filepaths:
-            ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
-            print("Checking %s" %media_filepath)
+        # CHECKING ffmpeg_src_language_code SUBTITLES STREAM ONLY, IF EXISTS WE PRINT IT AND EXTRACT IT
+        if do_translate == False:
 
-            subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
-            subtitle_streams_data = subtitle_stream_parser(media_filepath)
+            for media_filepath in media_filepaths:
 
-            if subtitle_streams_data and subtitle_streams_data != []:
+                ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
 
-                src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
-
-                if ffmpeg_src_language_code in subtitle_stream_parser.languages():
-                    print("Is '%s' subtitle stream exist          : Yes" %(ffmpeg_src_language_code.center(3)))
-                    subtitle_stream_regions = []
-                    subtitle_stream_transcripts = []
-                    for entry in src_subtitle_stream_timed_subtitles:
-                        subtitle_stream_regions.append(entry[0])
-                        subtitle_stream_transcripts.append(entry[1])
-                    base, ext = os.path.splitext(media_filepath)
-                    src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=args.src_language, format=subtitle_format)
-                    writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
-                    print(f"Extracting '{ffmpeg_src_language_code}'subtitle stream as      : {src_subtitle_filepath}")
-                    writer.write(src_subtitle_filepath)
-                    removed_media_filepaths.append(media_filepath)
+                print("Checking %s" %media_filepath)
 
-                else:
-                    print("Is '%s' subtitle stream exist          : No" %(ffmpeg_src_language_code.center(3)))
+                subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
+                subtitle_streams_data = subtitle_stream_parser(media_filepath)
 
-        print("")
+                if subtitle_streams_data and subtitle_streams_data != []:
 
-        if removed_media_filepaths:
-            for removed_media_filepath in removed_media_filepaths:
-                media_filepaths.remove(removed_media_filepath)
+                    src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
 
-        if not media_filepaths:
-            print("Nothing else to do, exiting")
-            sys.exit(0)
+                    if ffmpeg_src_language_code in subtitle_stream_parser.languages():
+                        print("Is '%s' subtitles stream exist         : Yes" %(ffmpeg_src_language_code.center(3)))
 
-    elif do_translate == True:
+                        subtitle_stream_regions = []
+                        subtitle_stream_transcripts = []
+                        for entry in src_subtitle_stream_timed_subtitles:
+                            subtitle_stream_regions.append(entry[0])
+                            subtitle_stream_transcripts.append(entry[1])
 
-        for media_filepath in media_filepaths:
-            ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
-            print("Checking %s" %media_filepath)
+                        base, ext = os.path.splitext(media_filepath)
+                        src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=args.src_language, format=subtitle_format)
 
-            subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
-            subtitle_streams_data = subtitle_stream_parser(media_filepath)
+                        print(f"Extracting '{ffmpeg_src_language_code}'subtitles stream as     : {src_subtitle_filepath}")
 
-            if subtitle_streams_data and subtitle_streams_data != []:
+                        writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
+                        writer.write(src_subtitle_filepath)
 
-                src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
-
-                if ffmpeg_src_language_code in subtitle_stream_parser.languages():
-                    print("Is '%s' subtitle stream exist          : Yes" %(ffmpeg_src_language_code.center(3)))
-                    subtitle_stream_regions = []
-                    subtitle_stream_transcripts = []
-                    for entry in src_subtitle_stream_timed_subtitles:
-                        subtitle_stream_regions.append(entry[0])
-                        subtitle_stream_transcripts.append(entry[1])
-                    base, ext = os.path.splitext(media_filepath)
-                    src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=args.src_language, format=subtitle_format)
-                    writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
-                    print(f"Extracting '{ffmpeg_src_language_code}'subtitle stream as      : {src_subtitle_filepath}")
-                    writer.write(src_subtitle_filepath)
+                        # no translate process as instructed in command arguments
 
-                else:
-                    print("Is '%s' subtitle stream exist          : No" %(ffmpeg_src_language_code.center(3)))
+                        # if args.embed_src is True we can't embed it because dst subtitles stream already exist
+                        if args.embed_src == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
+                            print(f"No need to embed '{ffmpeg_src_language_code}' subtitles stream because it's already existed")
 
-        for media_filepath in media_filepaths:
-            ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
-            print("Checking %s" %media_filepath)
+                        # remove media_filepath from transcribe proceed_list because all needed srt files already saved
+                        if args.force_recognize == False:
+                            if media_filepath not in removed_media_filepaths:
+                                removed_media_filepaths.append(media_filepath)
 
-            subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
-            subtitle_streams_data = subtitle_stream_parser(media_filepath)
+                    else:
+                        print("Is '%s' subtitles stream exist         : No" %(ffmpeg_src_language_code.center(3)))
 
-            if subtitle_streams_data and subtitle_streams_data != []:
+                print("")
 
-                src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
-                dst_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_dst_language_code)
-
-                if ffmpeg_dst_language_code in subtitle_stream_parser.languages():
-                    print("Is '%s' subtitle stream exist          : Yes" %(ffmpeg_dst_language_code.center(3)))
-                    subtitle_stream_regions = []
-                    subtitle_stream_transcripts = []
-                    for entry in dst_subtitle_stream_timed_subtitles:
-                        subtitle_stream_regions.append(entry[0])
-                        subtitle_stream_transcripts.append(entry[1])
-                    base, ext = os.path.splitext(media_filepath)
-                    dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=args.dst_language, format=subtitle_format)
-                    writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
-                    print(f"Extracting '{ffmpeg_dst_language_code}'subtitle stream as      : {dst_subtitle_filepath}")
-                    writer.write(dst_subtitle_filepath)
-                    removed_media_filepaths.append(media_filepath)
+            if removed_media_filepaths:
+                for removed_media_filepath in removed_media_filepaths:
+                    media_filepaths.remove(removed_media_filepath)
 
-                else:
-                    print("Is '%s' subtitle stream exist          : No" %(ffmpeg_dst_language_code.center(3)))
+            if not media_filepaths:
+                transcribe_end_time = time.time()
+                transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
+                transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
+                transcribe_elapsed_time_str = str(transcribe_elapsed_time_seconds)
+                hour, minute, second = transcribe_elapsed_time_str.split(":")
+                msg = "Total running time                      : %s:%s:%s" %(hour.zfill(2), minute, second)
+                print(msg)
+                sys.exit(0)
 
-                    if src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
-                        prompt = "Translating from %s to %s   : " %(args.src_language.center(8), args.dst_language.center(8))
-                        widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
-                        pbar = ProgressBar(widgets=widgets, maxval=len(src_subtitle_stream_timed_subtitles)).start()
-
-                        transcript_translator = SentenceTranslator(src=args.src_language, dst=args.dst_language, error_messages_callback=show_error_messages)
-
-                        translated_subtitle_stream_transcripts = []
-                        for i, translated_subtitle_stream_transcript in enumerate(pool.imap(transcript_translator, subtitle_stream_transcripts)):
-                            translated_subtitle_stream_transcripts.append(translated_subtitle_stream_transcript)
-                            pbar.update(i)
-                        pbar.finish()
+        # CHECKING ffmpeg_src_language_code AND ffmpeg_dst_language_code SUBTITLES STREAMS, IF EXISTS WE PRINT IT AND EXTRACT IT
+        # IF ONE OF THEM (ffmpeg_src_language_code OR ffmpeg_dst_language_code) NOT EXIST, WE TRANSLATE IT AND THEN EMBED IT
+        elif do_translate == True:
+
+            for media_filepath in media_filepaths:
+
+                ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
+                ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
+
+                subtitle_stream_parser = SubtitleStreamParser(error_messages_callback=show_error_messages)
+                subtitle_streams_data = subtitle_stream_parser(media_filepath)
+
+                print("Checking %s" %media_filepath)
+
+                if subtitle_streams_data and subtitle_streams_data != []:
+
+                    src_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_src_language_code)
+                    dst_subtitle_stream_timed_subtitles = subtitle_stream_parser.timed_subtitles_of_language(ffmpeg_dst_language_code)
+
+                    # ffmpeg_src_language_code subtitles stream exist, we print it and extract it
+                    if ffmpeg_src_language_code in subtitle_stream_parser.languages():
+                        print("Is '%s' subtitles stream exist         : Yes" %(ffmpeg_src_language_code.center(3)))
+
+                        subtitle_stream_regions = []
+                        subtitle_stream_transcripts = []
+                        for entry in src_subtitle_stream_timed_subtitles:
+                            subtitle_stream_regions.append(entry[0])
+                            subtitle_stream_transcripts.append(entry[1])
 
                         base, ext = os.path.splitext(media_filepath)
-                        dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=args.dst_language, format=subtitle_format)
-                        translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
-                        translation_writer.write(dst_subtitle_filepath)
-                        print("Translated subtitles file saved as      : {}" .format(dst_subtitle_filepath))
-                        removed_media_filepaths.append(media_filepath)
+                        src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=args.src_language, format=subtitle_format)
+
+                        print(f"Extracting '{ffmpeg_src_language_code}'subtitles stream as     : {src_subtitle_filepath}")
+
+                        writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
+                        writer.write(src_subtitle_filepath)
+
+                    # ffmpeg_src_language_code subtitles stream not exist, just print it
+                    else:
+                        print("Is '%s' subtitles stream exist         : No" %(ffmpeg_src_language_code.center(3)))
+
+                    # ffmpeg_dst_language_code subtitles stream exist, so we print it and extract it
+                    if ffmpeg_dst_language_code in subtitle_stream_parser.languages():
+                        print("Is '%s' subtitles stream exist         : Yes" %(ffmpeg_dst_language_code.center(3)))
+
+                        subtitle_stream_regions = []
+                        subtitle_stream_transcripts = []
+                        for entry in dst_subtitle_stream_timed_subtitles:
+                            subtitle_stream_regions.append(entry[0])
+                            subtitle_stream_transcripts.append(entry[1])
 
-                    if args.embed and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
                         base, ext = os.path.splitext(media_filepath)
-                        tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
-                        embedded_media_filepath = "{base}.embedded.{format}".format(base=base, format=ext[1:])
-                        ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
+                        dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=args.dst_language, format=subtitle_format)
 
-                        widgets = [f"Embedding \'{ffmpeg_dst_language_code}\' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-                        pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                        result = subtitle_embedder(media_filepath)
-                        pbar.finish()
+                        print(f"Extracting '{ffmpeg_dst_language_code}'subtitles stream as     : {dst_subtitle_filepath}")
 
-                        if os.path.isfile(tmp_embedded_media_filepath_1):
-                            shutil.copy(tmp_embedded_media_filepath_1, embedded_media_filepath)
-                        if os.path.isfile(embedded_media_filepath):
-                            print("Subtitle embedded {} file saved as   : {}".format(media_type, embedded_media_filepath))
+                        writer = SubtitleWriter(subtitle_stream_regions, subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
+                        writer.write(dst_subtitle_filepath)
+
+                    # ffmpeg_dst_language_code subtitles stream not exist, just print it
+                    else:
+                        print("Is '%s' subtitles stream exist         : No" %(ffmpeg_dst_language_code.center(3)))
 
-        print("")
+                    # ffmpeg_src_language_code subtitles stream = not exist,
+                    # ffmpeg_dst_language_code subtitles stream = exist
+                    # so we translate it from 'args.dst_language' to 'args.src_language'
+                    if ffmpeg_dst_language_code in subtitle_stream_parser.languages() and ffmpeg_src_language_code not in subtitle_stream_parser.languages():
+
+                        if dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
+                            prompt = "Translating from %s to %s   : " %(args.dst_language.center(8), args.src_language.center(8))
+                            widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
+                            pbar = ProgressBar(widgets=widgets, maxval=len(dst_subtitle_stream_timed_subtitles)).start()
+
+                            transcript_translator = SentenceTranslator(src=args.dst_language, dst=args.src_language, error_messages_callback=show_error_messages)
+
+                            translated_subtitle_stream_transcripts = []
+                            for i, translated_subtitle_stream_transcript in enumerate(pool.imap(transcript_translator, subtitle_stream_transcripts)):
+                                translated_subtitle_stream_transcripts.append(translated_subtitle_stream_transcript)
+                                pbar.update(i)
+                            pbar.finish()
 
-        if removed_media_filepaths:
-            for removed_media_filepath in removed_media_filepaths:
-                if removed_media_filepath in media_filepaths:
-                    media_filepaths.remove(removed_media_filepath)
+                            base, ext = os.path.splitext(media_filepath)
+                            src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=args.src_language, format=subtitle_format)
+
+                            translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
+                            translation_writer.write(src_subtitle_filepath)
+
+                            print("Translated subtitles file saved as      : {}" .format(src_subtitle_filepath))
+
+                            # remove media_filepath from transcribe proceed_list because all needed srt files already saved
+                            if args.force_recognize == False:
+                                if media_filepath not in removed_media_filepaths:
+                                    removed_media_filepaths.append(media_filepath)
+
+                            # if args.embed_src is True then we embed the translated srt into media_filepath
+                            if args.embed_src == True and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
+
+                                ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
+
+                                base, ext = os.path.splitext(media_filepath)
+                                src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+                                embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+
+                                widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                                pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                                subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                                src_tmp_output = subtitle_embedder(media_filepath)
+                                pbar.finish()
+
+                                if os.path.isfile(src_tmp_output):
+                                    shutil.copy(src_tmp_output, embedded_media_filepath)
+                                    os.remove(src_tmp_output)
+
+                                if os.path.isfile(embedded_media_filepath):
+                                    print("Subtitle embedded {} file saved as   : {}".format(media_type, embedded_media_filepath))
+
+                            # if args.embed_dst is True we can't embed it because dst subtitles stream already exist
+                            if args.embed_dst == True and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
+                                print(f"No need to embed '{ffmpeg_dst_language_code}' subtitles stream because it's already existed")
+
+                    # ffmpeg_src_language_code subtitles stream = exist,
+                    # ffmpeg_dst_language_code subtitles stream = not exist
+                    # so we translate it from 'args.src_language' to 'args.dst_language'
+                    elif ffmpeg_dst_language_code not in subtitle_stream_parser.languages() and ffmpeg_src_language_code in subtitle_stream_parser.languages():
+
+                        if src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
+                            prompt = "Translating from %s to %s   : " %(args.src_language.center(8), args.dst_language.center(8))
+                            widgets = [prompt, Percentage(), ' ', Bar(), ' ', ETA()]
+                            pbar = ProgressBar(widgets=widgets, maxval=len(src_subtitle_stream_timed_subtitles)).start()
+
+                            transcript_translator = SentenceTranslator(src=args.src_language, dst=args.dst_language, error_messages_callback=show_error_messages)
+
+                            translated_subtitle_stream_transcripts = []
+                            for i, translated_subtitle_stream_transcript in enumerate(pool.imap(transcript_translator, subtitle_stream_transcripts)):
+                                translated_subtitle_stream_transcripts.append(translated_subtitle_stream_transcript)
+                                pbar.update(i)
+                            pbar.finish()
+
+                            base, ext = os.path.splitext(media_filepath)
+                            dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=args.dst_language, format=subtitle_format)
+
+                            translation_writer = SubtitleWriter(subtitle_stream_regions, translated_subtitle_stream_transcripts, subtitle_format, error_messages_callback=show_error_messages)
+                            translation_writer.write(dst_subtitle_filepath)
+
+                            print("Translated subtitles file saved as      : {}" .format(dst_subtitle_filepath))
+
+                            # remove media_filepath from transcribe proceed_list because all needed srt files already saved
+                            if args.force_recognize == False:
+                                if media_filepath not in removed_media_filepaths:
+                                    removed_media_filepaths.append(media_filepath)
+
+                            # if args.embed_src is True we can't embed it because dst subtitles stream already exist
+                            if args.embed_src == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
+                                print(f"No need to embed '{ffmpeg_src_language_code}' subtitles stream because it's already existed")
+
+                            # if args.embed_dst is True then we embed that translated srt into media_filepath
+                            if args.embed_dst == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
+
+                                ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
+
+                                base, ext = os.path.splitext(media_filepath)
+                                dst_tmp_embedded_media_filepath = "{base}.{dst}.tmp.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
+                                embedded_media_filepath = "{base}.{dst}.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
+
+                                widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                                pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                                subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                                dst_tmp_output = subtitle_embedder(media_filepath)
+                                pbar.finish()
+
+                                if os.path.isfile(dst_tmp_output):
+                                    shutil.copy(dst_tmp_output, embedded_media_filepath)
+                                    os.remove(dst_tmp_output)
+
+                                if os.path.isfile(embedded_media_filepath):
+                                    print("Subtitle embedded {} file saved as   : {}".format(media_type, embedded_media_filepath))
+
+                    # ffmpeg_dst_language_code subtitles stream = exist
+                    # ffmpeg_src_language_code subtitles stream = exist
+                    # remove media_filepath from proceed list
+                    elif ffmpeg_dst_language_code in subtitle_stream_parser.languages() and ffmpeg_src_language_code in subtitle_stream_parser.languages():
+
+                        # remove media_filepath from transcribe proceed_list because all needed srt files already saved
+                        if args.force_recognize == False:
+                            if media_filepath not in removed_media_filepaths:
+                                removed_media_filepaths.append(media_filepath)
+
+                        # no need to translate becouse both languages subtitles files already saved
+
+                        # if args.embed_src is True we can't embed it because dst subtitles stream already exist
+                        if args.embed_src == True and src_subtitle_stream_timed_subtitles and src_subtitle_stream_timed_subtitles != []:
+                            print(f"No need to embed '{ffmpeg_src_language_code}' subtitles stream because it's already existed")
+
+                        # if args.embed_dst is True we can't embed it because dst subtitles stream already exist
+                        if args.embed_dst == True and dst_subtitle_stream_timed_subtitles and dst_subtitle_stream_timed_subtitles != []:
+                            print(f"No need to embed '{ffmpeg_dst_language_code}' subtitles stream because it's already existed")
+
+                print("")
+
+            # modifying  media_filepaths list as transcribe proceed_list (if args.force_recognize is false)
+            if removed_media_filepaths:
+                for removed_media_filepath in removed_media_filepaths:
+                    if removed_media_filepath in media_filepaths:
+                        media_filepaths.remove(removed_media_filepath)
+
+            # nothing to process
+            if not media_filepaths:
+                transcribe_end_time = time.time()
+                transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
+                transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
+                transcribe_elapsed_time_str = str(transcribe_elapsed_time_seconds)
+                hour, minute, second = transcribe_elapsed_time_str.split(":")
+                msg = "Total running time                      : %s:%s:%s" %(hour.zfill(2), minute, second)
+                print(msg)
+                sys.exit(0)
+
+
+    print("PERFORMING SPEECH RECOGNITION FOR MEDIA FILES THAT HAVE NO SUBTITLES STREAMS OR FORCED TO BE RE-RECOGNIZED")
+    print("=========================================================================================================")
+
+    proceed_list = []
+    # if args.force_recognize is true then we need to remove subtitles streams and save it as new media file to proceed with transcribe
+    if args.force_recognize == True:
+        for media_filepath in media_filepaths:
+            base, ext = os.path.splitext(media_filepath)
+            tmp_subtitle_removed_media_filepath = "{base}.tmp.subtitles.removed.media_filepath.{format}".format(base=base, format=ext[1:])
+            subtitle_removed_media_filepath = "{base}.force.recognize.{format}".format(base=base, format=ext[1:])
+
+            #src_tmp_output = remove_subtitles_from_media(media_filepath, tmp_subtitle_removed_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+
+            widgets = ["Removing subtitles streams from file    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+            pbar = ProgressBar(widgets=widgets, maxval=100).start()
+            subtitle_remover = MediaSubtitleRemover(output_path=tmp_subtitle_removed_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+            tmp_output = subtitle_remover(media_filepath)
+            pbar.finish()
 
-        if not media_filepaths:
-            print("Nothing else to do, exiting")
-            sys.exit(0)
+            if os.path.isfile(tmp_output):
+                shutil.copy(tmp_output, subtitle_removed_media_filepath)
+                os.remove(tmp_output)
 
+                proceed_list.append(subtitle_removed_media_filepath)
 
-    print("PERFORMING SPEECH RECOGNITION FOR MEDIA FILES THAT HAVE NO SUBTITLE STREAMS")
-    print("===========================================================================")
+            print("Subtitle removed {} file saved as    : {}".format(media_type, subtitle_removed_media_filepath))
+            print("")
 
-    for media_filepath in media_filepaths:
+    # if args.force_recognize is false then we just use modified media_filepaths list
+    else:
+        proceed_list = media_filepaths
+
+
+    # START THE TRANSCRIBE PROCESS
+    for media_filepath in proceed_list:
         print("Processing {}".format(media_filepath))
 
         try:
             widgets = ["Converting to a temporary WAV file      : ", Percentage(), ' ', Bar(), ' ', ETA()]
             pbar = ProgressBar(widgets=widgets, maxval=100).start()
             wav_converter = WavConverter(progress_callback=show_progress, error_messages_callback=show_error_messages)
             wav_filepath, sample_rate = wav_converter(media_filepath)
@@ -2378,15 +3201,15 @@
                 pbar.finish()
 
                 base, ext = os.path.splitext(media_filepath)
                 src_subtitle_filepath = "{base}.{src}.{format}".format(base=base, src=args.src_language, format=subtitle_format)
                 writer = SubtitleWriter(regions, transcripts, subtitle_format, error_messages_callback=show_error_messages)
                 writer.write(src_subtitle_filepath)
 
-                if do_translate:
+                if do_translate == True:
                     # CONCURRENT TRANSLATION USING class SentenceTranslator(object)
                     # NO NEED TO TRANSLATE ALL transcript IN transcripts
                     # BECAUSE SOME region IN regions MAY JUST HAVE transcript WITH EMPTY STRING
                     # JUST TRANSLATE ALREADY CREATED subtitles ENTRIES FROM timed_subtitles
                     timed_subtitles = writer.timed_subtitles
                     created_regions = []
                     created_subtitles = []
@@ -2407,90 +3230,144 @@
                     pbar.finish()
 
                     base, ext = os.path.splitext(media_filepath)
                     dst_subtitle_filepath = "{base}.{dst}.{format}".format(base=base, dst=args.dst_language, format=subtitle_format)
                     translation_writer = SubtitleWriter(created_regions, translated_subtitles, subtitle_format, error_messages_callback=show_error_messages)
                     translation_writer.write(dst_subtitle_filepath)
 
-                if do_translate:
+                if do_translate == True:
                     print("Original subtitles file saved as        : {}".format(src_subtitle_filepath))
                     print("Translated subtitles file saved as      : {}" .format(dst_subtitle_filepath))
                 else:
                     print("Subtitles file saved as                 : {}".format(src_subtitle_filepath))
 
-                if args.embed:
-                    base, ext = os.path.splitext(media_filepath)
-                    tmp_embedded_media_filepath_1 = "{base}.embedded1.{format}".format(base=base, format=ext[1:])
-                    tmp_embedded_media_filepath_2 = "{base}.embedded2.{format}".format(base=base, format=ext[1:])
-                    tmp_embedded_media_filepath_3 = "{base}.embedded3.{format}".format(base=base, format=ext[1:])
-                    embedded_media_filepath = "{base}.embedded.{format}".format(base=base, format=ext[1:])
 
-                    if do_translate:
+                # EMBEDDING SUBTITLES FILE
+                embedded_media_filepath = None
+                if do_translate == False:
+
+                    if args.embed_src == True:
+
+                        ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
+
+                        base, ext = os.path.splitext(media_filepath)
+                        src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+                        embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+
+                        widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                        pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                        src_tmp_output = subtitle_embedder(media_filepath)
+                        pbar.finish()
+
+                        if os.path.isfile(src_tmp_output):
+                            shutil.copy(src_tmp_output, embedded_media_filepath)
+                            os.remove(src_tmp_output)
+                            print("Subtitle embedded {} file saved as   : {}".format(media_type, embedded_media_filepath))
+
+                elif do_translate == True:
+
+                    if args.embed_src == True and args.embed_dst == True:
+
                         ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
                         ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
 
+                        base, ext = os.path.splitext(media_filepath)
+                        src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+                        src_dst_tmp_embedded_media_filepath = "{base}.{src}.{dst}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, dst=ffmpeg_dst_language_code, format=ext[1:])
+                        embedded_media_filepath = "{base}.{src}.{dst}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, dst=ffmpeg_dst_language_code, format=ext[1:])
+
                         '''
                         # USING FUNCTION
-                        result = embed_subtitle_to_media(media_filepath, media_type, src_subtitle_filepath, ffmpeg_src_language_code, tmp_embedded_media_filepath_1)
-                        if os.path.isfile(tmp_embedded_media_filepath_1) and os.path.isfile(dst_subtitle_filepath):
-                            result = embed_subtitle_to_media(tmp_embedded_media_filepath_1, media_type, dst_subtitle_filepath, ffmpeg_dst_language_code, tmp_embedded_media_filepath_2)
-                        else:
-                            result = embed_subtitle_to_media(media_filepath, media_type, dst_subtitle_filepath, ffmpeg_dst_language_code, tmp_embedded_media_filepath_2)
+                        src_tmp_output = embed_subtitle_to_media(media_filepath, media_type, src_subtitle_filepath, ffmpeg_src_language_code, src_tmp_embedded_media_filepath)
+                        if os.path.isfile(src_tmp_output) and os.path.isfile(dst_subtitle_filepath):
+                            src_dst_tmp_output = embed_subtitle_to_media(src_tmp_embedded_media_filepath, media_type, dst_subtitle_filepath, ffmpeg_dst_language_code, src_dst_tmp_embedded_media_filepath)
                         '''
 
+
                         # USING CLASS
-                        widgets = [f"Embedding \'{ffmpeg_src_language_code}\' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                        widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                         pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                        result = subtitle_embedder(media_filepath)
+                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                        src_tmp_output = subtitle_embedder(media_filepath)
                         pbar.finish()
 
-                        if os.path.isfile(tmp_embedded_media_filepath_1) and os.path.isfile(dst_subtitle_filepath):
-                            widgets = [f"Embedding \'{ffmpeg_dst_language_code}\' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                        if os.path.isfile(src_tmp_output) and os.path.isfile(dst_subtitle_filepath):
+                            widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                             pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_2, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                            result = subtitle_embedder(tmp_embedded_media_filepath_1)
-                            pbar.finish()
-                        elif (not os.path.isfile(tmp_embedded_media_filepath_1)) and os.path.isfile(dst_subtitle_filepath):
-                            widgets = [f"Embedding \'{ffmpeg_dst_language_code}\' subtitles into {media_type}     : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
-                            pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=tmp_embedded_media_filepath_2, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                            result = subtitle_embedder(media_filepath)
+                            subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=src_dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                            src_dst_tmp_output = subtitle_embedder(src_tmp_output)
                             pbar.finish()
 
-                        if os.path.isfile(tmp_embedded_media_filepath_2):
-                            shutil.copy(tmp_embedded_media_filepath_2, embedded_media_filepath)
 
-                        if os.path.isfile(tmp_embedded_media_filepath_1):
-                            os.remove(tmp_embedded_media_filepath_1)
-                        if os.path.isfile(tmp_embedded_media_filepath_2):
-                            os.remove(tmp_embedded_media_filepath_2)
+                        if os.path.isfile(src_dst_tmp_output):
+                            shutil.copy(src_dst_tmp_output, embedded_media_filepath)
+                            print("Subtitle embedded {} file saved as   : {}".format(media_type, embedded_media_filepath))
+                        else:
+                            print("Unknown error!")
+
+                        if os.path.isfile(src_dst_tmp_output):
+                            os.remove(src_dst_tmp_output)
+                        if os.path.isfile(src_tmp_output):
+                            os.remove(src_tmp_output)
+
+                    elif args.embed_src == True and args.embed_dst == False:
 
-                    else:
                         ffmpeg_src_language_code = language.ffmpeg_code_of_code[args.src_language]
 
-                        #result = embed_subtitle_to_media(media_filepath, media_type, src_subtitle_filepath, ffmpeg_src_language_code, tmp_embedded_media_filepath_1)
+                        base, ext = os.path.splitext(media_filepath)
+                        src_tmp_embedded_media_filepath = "{base}.{src}.tmp.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
+                        embedded_media_filepath = "{base}.{src}.embedded.{format}".format(base=base, src=ffmpeg_src_language_code, format=ext[1:])
 
-                        widgets = [f"Embedding \'{ffmpeg_src_language_code}\' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                        widgets = [f"Embedding '{ffmpeg_src_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                         pbar = ProgressBar(widgets=widgets, maxval=100).start()
-                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=tmp_embedded_media_filepath_1, progress_callback=show_progress, error_messages_callback=show_error_messages)
-                        result = subtitle_embedder(media_filepath)
+                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=src_subtitle_filepath, language=ffmpeg_src_language_code, output_path=src_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                        src_tmp_output = subtitle_embedder(media_filepath)
                         pbar.finish()
 
-                        if tmp_embedded_media_filepath_1:
-                            shutil.copy(tmp_embedded_media_filepath_1, embedded_media_filepath)
-                            os.remove(tmp_embedded_media_filepath_1)
-
-                    if os.path.isfile(embedded_media_filepath):
-                        print("Subtitle embedded {} file saved as   : {}".format(media_type, embedded_media_filepath))
-
-                if not args.embed:
-                    completed_tasks += 1
-                elif args.embed:
-                    if embedded_media_filepath and os.path.isfile(embedded_media_filepath):
+                        if os.path.isfile(src_tmp_output):
+                            shutil.copy(src_tmp_output, embedded_media_filepath)
+                            os.remove(src_tmp_embedded_media_filepath)
+                            print("Subtitle embedded {} file saved as   : {}".format(media_type, embedded_media_filepath))
+                        else:
+                            print("Unknown error!")
+
+                    elif args.embed_src == False and args.embed_dst == True:
+
+                        ffmpeg_dst_language_code = language.ffmpeg_code_of_code[args.dst_language]
+
+                        base, ext = os.path.splitext(media_filepath)
+                        dst_tmp_embedded_media_filepath = "{base}.{dst}.tmp.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
+                        embedded_media_filepath = "{base}.{dst}.embedded.{format}".format(base=base, dst=ffmpeg_dst_language_code, format=ext[1:])
+
+                        widgets = [f"Embedding '{ffmpeg_dst_language_code}' subtitles into {media_type}    : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
+                        pbar = ProgressBar(widgets=widgets, maxval=100).start()
+                        subtitle_embedder = MediaSubtitleEmbedder(subtitle_path=dst_subtitle_filepath, language=ffmpeg_dst_language_code, output_path=dst_tmp_embedded_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                        dst_tmp_output = subtitle_embedder(media_filepath)
+                        pbar.finish()
+
+                        if os.path.isfile(dst_tmp_output):
+                            shutil.copy(dst_tmp_output, embedded_media_filepath)
+                            os.remove(dst_tmp_output)
+                            print("Subtitle embedded {} file saved as   : {}".format(media_type, embedded_media_filepath))
+                        else:
+                            print("Unknown error!")
+
+                if do_translate == False:
+                    if args.embed_src == True:
+                        if embedded_media_filepath and os.path.isfile(embedded_media_filepath):
+                            completed_tasks += 1
+                    else:
+                        completed_tasks += 1
+
+                elif do_translate == True:
+                    if args.embed_src == True or args.embed_dst == True:
+                        if embedded_media_filepath and os.path.isfile(embedded_media_filepath):
+                            completed_tasks += 1
+                    else:
                         completed_tasks += 1
 
                 print('')
                 if len(media_filepaths)>0 and completed_tasks == len(media_filepaths):
                     transcribe_end_time = time.time()
                     transcribe_elapsed_time = transcribe_end_time - transcribe_start_time
                     transcribe_elapsed_time_seconds = timedelta(seconds=int(transcribe_elapsed_time))
@@ -2512,15 +3389,15 @@
                 stop_ffmpeg_linux(error_messages_callback=show_error_messages)
 
             remove_temp_files("flac")
             remove_temp_files("wav")
             return 1
 
         except Exception as e:
-            if not KeyboardInterrupt in e:
+            if not KeyboardInterrupt in str(e):
                 pbar.finish()
                 pool.terminate()
                 pool.close()
                 pool.join()
                 print(e)
 
                 if sys.platform == "win32":
```

### Comparing `autosrt-1.3.9/autosrt.egg-info/PKG-INFO` & `autosrt-1.4.1/autosrt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.3.9
+Version: 1.4.1
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.3.9/setup.py` & `autosrt-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.9/test/test1.py` & `autosrt-1.4.1/test/test1.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.9/test/test2.py` & `autosrt-1.4.1/test/test2.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.9/test/test3.py` & `autosrt-1.4.1/test/test3.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.9/test/test4.py` & `autosrt-1.4.1/test/test4.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
         )
 
         stderr = []
         base_popen_kwargs = self.base_popen_kwargs.copy()
         if popen_kwargs is not None:
             base_popen_kwargs.update(popen_kwargs)
 
-        if sys.platform == "wind32":
+        if sys.platform == "win32":
             self.process = subprocess.Popen(
                 cmd_with_progress,
                 **base_popen_kwargs,
                 creationflags=subprocess.CREATE_NO_WINDOW,
             )  # type: ignore
         else:
             self.process = subprocess.Popen(
```

