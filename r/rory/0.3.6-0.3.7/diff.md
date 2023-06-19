# Comparing `tmp/rory-0.3.6.tar.gz` & `tmp/rory-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rory-0.3.6.tar", last modified: Fri Jul  1 19:00:38 2022, max compression
+gzip compressed data, was "rory-0.3.7.tar", last modified: Mon Jun 19 19:38:19 2023, max compression
```

## Comparing `rory-0.3.6.tar` & `rory-0.3.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 quintin   (1000) quintin   (1000)        0 2022-07-01 19:00:38.343806 rory-0.3.6/
--rw-r--r--   0 quintin   (1000) quintin   (1000)    18046 2022-05-29 18:39:16.000000 rory-0.3.6/LICENSE
--rw-r--r--   0 quintin   (1000) quintin   (1000)     1855 2022-07-01 19:00:38.343806 rory-0.3.6/PKG-INFO
--rw-r--r--   0 quintin   (1000) quintin   (1000)     1353 2022-05-29 18:39:16.000000 rory-0.3.6/README.md
-drwxr-xr-x   0 quintin   (1000) quintin   (1000)        0 2022-07-01 19:00:38.343806 rory-0.3.6/rory/
--rwxr-xr-x   0 quintin   (1000) quintin   (1000)     1960 2022-07-01 18:59:44.000000 rory-0.3.6/rory/__init__.py
--rw-r--r--   0 quintin   (1000) quintin   (1000)     5691 2022-06-21 04:16:44.000000 rory-0.3.6/rory/interactor.py
--rw-r--r--   0 quintin   (1000) quintin   (1000)    42824 2022-07-01 18:59:44.000000 rory-0.3.6/rory/interface.py
--rw-r--r--   0 quintin   (1000) quintin   (1000)    13536 2022-06-02 03:43:55.000000 rory-0.3.6/rory/midiinterface.py
--rw-r--r--   0 quintin   (1000) quintin   (1000)    10006 2022-07-01 18:59:44.000000 rory-0.3.6/rory/player.py
--rw-r--r--   0 quintin   (1000) quintin   (1000)     9844 2022-06-10 16:16:41.000000 rory-0.3.6/rory/structures.py
-drwxr-xr-x   0 quintin   (1000) quintin   (1000)        0 2022-07-01 19:00:38.343806 rory-0.3.6/rory.egg-info/
--rw-r--r--   0 quintin   (1000) quintin   (1000)     1855 2022-07-01 19:00:37.000000 rory-0.3.6/rory.egg-info/PKG-INFO
--rw-r--r--   0 quintin   (1000) quintin   (1000)      306 2022-07-01 19:00:38.000000 rory-0.3.6/rory.egg-info/SOURCES.txt
--rw-r--r--   0 quintin   (1000) quintin   (1000)        1 2022-07-01 19:00:38.000000 rory-0.3.6/rory.egg-info/dependency_links.txt
--rw-r--r--   0 quintin   (1000) quintin   (1000)       35 2022-07-01 19:00:38.000000 rory-0.3.6/rory.egg-info/entry_points.txt
--rw-r--r--   0 quintin   (1000) quintin   (1000)       24 2022-07-01 19:00:38.000000 rory-0.3.6/rory.egg-info/requires.txt
--rw-r--r--   0 quintin   (1000) quintin   (1000)        5 2022-07-01 19:00:38.000000 rory-0.3.6/rory.egg-info/top_level.txt
--rw-r--r--   0 quintin   (1000) quintin   (1000)       38 2022-07-01 19:00:38.343806 rory-0.3.6/setup.cfg
--rw-r--r--   0 quintin   (1000) quintin   (1000)      943 2022-05-29 18:39:16.000000 rory-0.3.6/setup.py
+drwxrwxr-x   0 pent      (1000) pent      (1000)        0 2023-06-19 19:38:19.280117 rory-0.3.7/
+-rw-rw-r--   0 pent      (1000) pent      (1000)    18046 2023-06-19 19:38:09.000000 rory-0.3.7/LICENSE
+-rw-rw-r--   0 pent      (1000) pent      (1000)     1699 2023-06-19 19:38:19.280117 rory-0.3.7/PKG-INFO
+-rw-rw-r--   0 pent      (1000) pent      (1000)     1204 2023-06-19 19:38:09.000000 rory-0.3.7/README.md
+drwxrwxr-x   0 pent      (1000) pent      (1000)        0 2023-06-19 19:38:19.276117 rory-0.3.7/rory/
+-rwxrwxr-x   0 pent      (1000) pent      (1000)     1949 2023-06-19 19:38:19.000000 rory-0.3.7/rory/__init__.py
+-rw-rw-r--   0 pent      (1000) pent      (1000)     5691 2023-06-19 19:38:19.000000 rory-0.3.7/rory/interactor.py
+-rw-rw-r--   0 pent      (1000) pent      (1000)    43564 2023-06-19 19:38:19.000000 rory-0.3.7/rory/interface.py
+-rw-rw-r--   0 pent      (1000) pent      (1000)    13500 2023-06-19 19:38:19.000000 rory-0.3.7/rory/midiinterface.py
+-rw-rw-r--   0 pent      (1000) pent      (1000)    11411 2023-06-19 19:38:19.000000 rory-0.3.7/rory/player.py
+-rw-rw-r--   0 pent      (1000) pent      (1000)    16188 2023-06-19 19:38:19.000000 rory-0.3.7/rory/structures.py
+drwxrwxr-x   0 pent      (1000) pent      (1000)        0 2023-06-19 19:38:19.280117 rory-0.3.7/rory.egg-info/
+-rw-rw-r--   0 pent      (1000) pent      (1000)     1699 2023-06-19 19:38:19.000000 rory-0.3.7/rory.egg-info/PKG-INFO
+-rw-rw-r--   0 pent      (1000) pent      (1000)      306 2023-06-19 19:38:19.000000 rory-0.3.7/rory.egg-info/SOURCES.txt
+-rw-rw-r--   0 pent      (1000) pent      (1000)        1 2023-06-19 19:38:19.000000 rory-0.3.7/rory.egg-info/dependency_links.txt
+-rw-rw-r--   0 pent      (1000) pent      (1000)       36 2023-06-19 19:38:19.000000 rory-0.3.7/rory.egg-info/entry_points.txt
+-rw-rw-r--   0 pent      (1000) pent      (1000)       24 2023-06-19 19:38:19.000000 rory-0.3.7/rory.egg-info/requires.txt
+-rw-rw-r--   0 pent      (1000) pent      (1000)        5 2023-06-19 19:38:19.000000 rory-0.3.7/rory.egg-info/top_level.txt
+-rw-rw-r--   0 pent      (1000) pent      (1000)       38 2023-06-19 19:38:19.280117 rory-0.3.7/setup.cfg
+-rw-rw-r--   0 pent      (1000) pent      (1000)      917 2023-06-19 19:38:09.000000 rory-0.3.7/setup.py
```

### Comparing `rory-0.3.6/LICENSE` & `rory-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rory-0.3.6/PKG-INFO` & `rory-0.3.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: rory
-Version: 0.3.6
+Version: 0.3.7
 Summary: Play along to MIDI files in console
-Home-page: https://github.com/quintinfsmith/rory
+Home-page: https://burnsomni.net/git/rory
 Author: Quintin Smith
 Author-email: smith.quintin@protonmail.com
 License: GPL-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Rory
 Learn Piano using MIDI files and a MIDI Keyboard<br/>
-[![Travis (.com)](https://img.shields.io/travis/com/quintinfsmith/rory?style=flat-square)](https://travis-ci.com/github/quintinfsmith/rory)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/rory?style=flat-square)](https://pypi.org/project/rory/)
 [![PyPI](https://img.shields.io/pypi/v/rory?style=flat-square)](https://pypi.org/project/rory/)
-[![GitHub](https://img.shields.io/github/license/quintinfsmith/rory?style=flat-square)](https://github.com/quintinfsmith/rory/blob/master/LICENSE)
+[![PyPI - License](https://img.shields.io/pypi/l/rory?style=flat-square)](https://burnsomni.net/project/rory/?branch=master&path=LICENSE)
 
 <img src="https://raw.githubusercontent.com/quintinfsmith/rory/master/res/sample.svg" />
 
 ## Installation
 ```bash
 pip install rory
 ```
```

### Comparing `rory-0.3.6/README.md` & `rory-0.3.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Rory
 Learn Piano using MIDI files and a MIDI Keyboard<br/>
-[![Travis (.com)](https://img.shields.io/travis/com/quintinfsmith/rory?style=flat-square)](https://travis-ci.com/github/quintinfsmith/rory)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/rory?style=flat-square)](https://pypi.org/project/rory/)
 [![PyPI](https://img.shields.io/pypi/v/rory?style=flat-square)](https://pypi.org/project/rory/)
-[![GitHub](https://img.shields.io/github/license/quintinfsmith/rory?style=flat-square)](https://github.com/quintinfsmith/rory/blob/master/LICENSE)
+[![PyPI - License](https://img.shields.io/pypi/l/rory?style=flat-square)](https://burnsomni.net/project/rory/?branch=master&path=LICENSE)
 
 <img src="https://raw.githubusercontent.com/quintinfsmith/rory/master/res/sample.svg" />
 
 ## Installation
 ```bash
 pip install rory
 ```
```

### Comparing `rory-0.3.6/rory/__init__.py` & `rory-0.3.7/rory/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python3
 # coding=utf-8
 """
 Usage:
     rory path/to/midi.midi
 """
 
-__version__ = "0.3.6"
+__version__ = "0.3.7"
 __license__ = "GPL-2.0"
 __author__ = "Quintin Smith"
 __email__ = "smith.quintin@protonmail.com"
-__url__ = "https://github.com/quintinfsmith/rory"
+__url__ = "https://burnsomni.net/git/rory"
 
 def main():
     import sys
     import time
     import os
     from apres import InvalidMIDIFile
-    from rory.interface import RoryStage, TerminalTooNarrow
+    from .interface import RoryStage, TerminalTooNarrow
     options = {
         "-t": ("transpose", int),
         "-m": ('numode', int)
     }
 
     arguments = sys.argv[1:]
     kwargs = {}
```

### Comparing `rory-0.3.6/rory/interactor.py` & `rory-0.3.7/rory/interactor.py`

 * *Files identical despite different names*

### Comparing `rory-0.3.6/rory/interface.py` & `rory-0.3.7/rory/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import time
 import os
 from typing import Final
 from abc import ABC
 import wrecked
 from wrecked import get_terminal_size
 from apres import MIDI
-from rory.player import Player
-from rory.interactor import Interactor
+from .player import Player
+from .interactor import Interactor
 
 class TerminalTooNarrow(Exception):
     '''Error thrown when the minimum width required isn't available'''
 
 class RoryStage:
     '''Interface to Run the MidiPlayer'''
     KILL = 1
@@ -656,14 +656,26 @@
 
         interactor.assign_context_sequence(
             RoryStage.CONTEXT_PLAYER,
             self.CONTROL_SET_RANGE,
             self.flag_new_range
         )
 
+        interactor.assign_context_sequence(
+            RoryStage.CONTEXT_PLAYER,
+            'v',
+            self.screengrab
+        )
+
+
+    def screengrab(self):
+        ansi_string = wrecked.get_current_ansi_string()
+        with open("SCREENER", "w") as fp:
+            fp.write(ansi_string)
+
     def __init__(self, rorystage: RoryStage, **kwargs):
         self.player = Player(**kwargs)
         self.nu_mode = kwargs.get('numode', False)
 
         super().__init__(rorystage)
 
         self.active_midi = MIDI.load(kwargs['path'])
@@ -681,26 +693,30 @@
         self.visible_note_rects = {}
         self.visible_note_rects_lines = {}
         self.pressed_note_rects = {}
 
         self.rect_position_display = self.rect_background.new_rect()
         self.rect_position_display.bold()
         self.rect_position_display.underline()
-        self.rect_position_display.set_bg_color(wrecked.BLACK)
+        #self.rect_position_display.set_bg_color(wrecked.BLACK)
+        self.rect_position_display.unset_bg_color()
         self.rect_position_display.set_fg_color(wrecked.WHITE)
         #self.rect_chord_names = self.rect_background.new_rect()
         #self.rect_chord_names.bold()
         #self.rect_chord_names.underline()
         #self.rect_chord_names.set_bg_color(wrecked.BLACK)
         #self.rect_chord_names.set_fg_color(wrecked.WHITE)
 
-        self.rect_background.set_bg_color(wrecked.BLACK)
+        #self.rect_background.set_bg_color(wrecked.BLACK)
+        self.rect_background.unset_bg_color()
         self.rect_background.set_fg_color(wrecked.BRIGHTBLACK)
-        self.rect_loop_start.set_bg_color(wrecked.BLACK)
-        self.rect_loop_end.set_bg_color(wrecked.BLACK)
+        #self.rect_loop_start.set_bg_color(wrecked.BLACK)
+        self.rect_loop_start.unset_bg_color()
+        #self.rect_loop_end.set_bg_color(wrecked.BLACK)
+        self.rect_loop_end.unset_bg_color()
         self.rect_loop_start.set_fg_color(wrecked.BRIGHTWHITE)
         self.rect_loop_end.set_fg_color(wrecked.BRIGHTWHITE)
 
         self.active_row_position = 8
 
         self.FLAG_BACKGROUND = True
         self.last_rendered_pressed = None
@@ -856,15 +872,16 @@
                         note_rect.set_character(0, 0, self.NOTELIST[message.note % 12])
 
                     if message.note % 12 in self.SHARPS:
                         note_rect.set_bg_color(color)
                         note_rect.set_fg_color(wrecked.BLACK)
                     else:
                         note_rect.set_fg_color(color)
-                        note_rect.set_bg_color(wrecked.BLACK)
+                        #note_rect.set_bg_color(wrecked.BLACK)
+                        note_rect.unset_bg_color()
 
                 note_rect.move(x, y)
 
             # Draw Measure Lines
             if position in midi_interface.beat_map and _y != self.active_row_position:
                 line_char = self.CHARS['measureline']
                 if position in midi_interface.measure_map:
@@ -879,15 +896,16 @@
 
                     try:
                         line_rect = self.visible_note_rects_lines[(position, x)]
                     except KeyError:
                         line_rect = self.layer_visible_notes.new_rect()
                         line_rect.set_character(0, 0, line_char)
                         line_rect.set_fg_color(wrecked.BRIGHTBLACK)
-                        line_rect.set_bg_color(wrecked.BLACK)
+                        #line_rect.set_bg_color(wrecked.BLACK)
+                        line_rect.unset_bg_color()
                         self.visible_note_rects_lines[(position, x)] = line_rect
                     line_rect.move(x, y)
 
 
             if position == self.player.loop[0]:
                 self.rect_loop_start.enable()
                 if _y != self.active_row_position:
@@ -935,14 +953,16 @@
             line_char = self.CHARS['activeline_beat']
         else:
             line_char = self.CHARS['activeline']
 
         for x in range(self.rect_active_row_line.width):
             self.rect_active_row_line.set_character(x, 0, line_char)
 
+        #self.rect_active_row_line.set_bg_color(wrecked.BLACK)
+        self.rect_active_row_line.unset_bg_color()
         if not self.metronome_state:
             self.rect_active_row_line.set_fg_color(wrecked.BRIGHTBLACK)
         else:
             self.rect_active_row_line.set_fg_color(wrecked.YELLOW)
 
 
 
@@ -1019,15 +1039,16 @@
         active_state = midi_interface.get_state(song_position)
 
         for note in pressed_notes:
             x = self.__get_displayed_key_position(note)
 
             note_rect = self.layer_active_notes.new_rect()
             note_rect.set_character(0, 0, self.CHARS['keyboard_pressed'])
-            note_rect.set_bg_color(wrecked.BLACK)
+            #note_rect.set_bg_color(wrecked.BLACK)
+            note_rect.unset_bg_color()
             note_rect.move(x, 1)
             self.pressed_note_rects[note] = note_rect
 
             if note in player.need_to_release:
                 if note in active_state:
                     note_rect.set_fg_color(wrecked.YELLOW)
                 else:
```

### Comparing `rory-0.3.6/rory/midiinterface.py` & `rory-0.3.7/rory/midiinterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''Plays MIDILike Objects'''
 from apres import NoteOn, NoteOff, TimeSignature, SetTempo
-from rory.structures import Grouping
+from .structures import Grouping
 
 class MIDIInterface:
     '''Layer between Player and the MIDI input file'''
     notelist = 'CCDDEFFGGAAB'
 
     def __handle_kwargs(self, kwargs):
         self.transpose = kwargs.get('transpose', 0)
@@ -18,15 +18,14 @@
         current_numerator = 4
         beat_size = self.midi.ppqn
         active_notes = {}
         min_note = 128
         max_note = 0
         for tick, event in self.midi.get_all_events():
             tick_diff = tick - running_beat_count[1]
-
             current_beat = int(running_beat_count[0] + (tick_diff // beat_size))
             while len(beats) <= current_beat:
                 beats.append([[], beat_size, None, current_numerator, None])
 
             if self.is_note_on(event):
                 active_notes[(event.channel, event.note)] = (
                     current_beat,
@@ -121,15 +120,14 @@
         beat_count = 0
         for measure in list(grouping):
             self.measure_map.append(len(self.state_map))
             for _beat_index, beat in enumerate(list(measure)):
                 if beat.is_open():
                     continue
 
-  #              beat.reduce()
                 beat.flatten()
 
                 self.beat_map[len(self.state_map)] = beat_count
                 self.inv_beat_map[beat_count] = len(self.state_map)
 
                 i = len(self.state_map)
                 for group in list(beat):
```

### Comparing `rory-0.3.6/rory/player.py` & `rory-0.3.7/rory/player.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 '''Plays MIDILike Objects'''
 import threading
 import time
 import os
 import pyinotify
 
 from apres import MIDI, MIDIController, MIDIEvent, NoteOn, NoteOff
-from rory.midiinterface import MIDIInterface
+from .midiinterface import MIDIInterface
 
 class Player:
     '''Plays MIDILike Objects'''
 
     def kill(self):
         ''''Shutdown the player'''
         self.is_active = False
-        self.midi_controller.close()
+        self.controller_manager.close()
 
     def next_state(self):
         '''Change the song position to the next state with notes.'''
         new_position = self.song_position + 1
         while new_position <= self.loop[1] \
         and not self.midi_interface.get_state(new_position, self.ignored_channels):
             new_position += 1
@@ -62,25 +62,26 @@
         self.current_tempo = self.midi_interface.get_tempo_at_tick(tick)
 
     def set_measure(self, measure):
         position = self.midi_interface.get_first_position_in_measure(measure)
         self.set_state(position)
 
     def reinit_midi_interface(self, **kwargs):
-        self.active_midi = MIDI(self.active_midi.path)
+        self.active_midi = MIDI.load(self.active_path)
         self.midi_interface = MIDIInterface(self.active_midi, **kwargs)
         self.clear_loop()
         self.song_position = -1
         self.next_state()
 
     def get_transpose(self):
         return self.midi_interface.transpose
 
     def __init__(self, **kwargs):
-        self.active_midi = MIDI.load(kwargs['path'])
+        self.active_path = kwargs.get('path', '')
+        self.active_midi = MIDI.load(self.active_path)
         self.current_tempo = 120
 
         self.is_active = True
         self.register = 0
         self.flag_negative_register = False
         self.loop = [0, 0]
         self.note_range = (21, 109)
@@ -97,18 +98,15 @@
 
         self.next_state()
 
 
         self.flag_range_input = False
         self._new_range = None
 
-        if 'controller_path' in kwargs:
-            self.midi_controller = RoryController(self, kwargs['controller_path'])
-        else:
-            self.midi_controller = RoryController(self)
+        self.controller_manager = ControllerManager(self)
 
     def get_register(self):
         if self.flag_negative_register:
             self.register *= -1
 
         output = self.register
         self.register = 0
@@ -118,15 +116,15 @@
     def set_note_range(self, lower, upper):
         self.note_range = (lower, upper)
         self.flag_range_input = False
         self._new_range = None
 
     def get_pressed_notes(self):
         ''' Get the notes that the midi device has held down '''
-        notes = self.midi_controller.pressed.copy()
+        notes = self.controller_manager.get_pressed()
         if self.flag_range_input:
             if len(notes):
                 lower = min(notes)
                 upper = max(notes)
                 if self._new_range is None:
                     self._new_range = (lower, upper)
                 else:
@@ -210,38 +208,86 @@
 
     def jump_to_register_position(self):
         '''Set the song position to the value of the input register'''
         self.set_state(self.get_register())
 
 
 class RoryController(MIDIController):
-    def __init__(self, player, path = ""):
-        self.player = player
+    def __init__(self, channel, device_index, controller_manager):
+        super().__init__(channel, device_index)
+        self.controller_manager = controller_manager
 
-        if not path:
-            for filename in os.listdir("/dev/"):
-                if "midi" in filename:
-                    path = "/dev/%s" % filename
-                    break
+    def hook_NoteOn(self, event):
+        if event.velocity == 0:
+            self.release_note(event.note)
+        else:
+            self.press_note(event.note)
 
-        super().__init__(path)
+    def hook_NoteOff(self, event):
+        self.release_note(event.note)
+
+    def press_note(self, note):
+        '''Press a Midi Note'''
+        self.controller_manager.press_note(note)
+
+    def release_note(self, note):
+        '''Release a Midi Note'''
+        self.controller_manager.release_note(note)
+
+class ControllerManager:
+    def __init__(self, player):
+        self.player = player
 
         self.pressed = set()
+        self.state_check_ticket = 0
+        self.processing_ticket = 0
+
+        channel = 0
+        device_index = 0
+        self.controller = None
+        self.active_key = None
+        for filename in os.listdir("/dev/snd/"):
+            if "midi" in filename:
+                device_index = int(filename[filename.rfind("D") + 1])
+                channel = int(filename[filename.rfind("C") + 1])
+                self.new_controller(channel, device_index)
+                break
 
         self.watch_manager = pyinotify.WatchManager()
-        notifier = pyinotify.ThreadedNotifier(self.watch_manager, TaskHandler(self))
-        notifier.daemon = True
-        notifier.start()
+        self.notifier = pyinotify.ThreadedNotifier(self.watch_manager, TaskHandler(self))
+        self.notifier.daemon = True
+        self.notifier.start()
         self.watch_manager.add_watch(
-            "/dev/",
+            "/dev/snd/",
             pyinotify.IN_CREATE | pyinotify.IN_DELETE
         )
 
-        self.state_check_ticket = 0
-        self.processing_ticket = 0
+    def get_pressed(self):
+        return self.pressed.copy()
+
+    def close(self):
+        self.disconnect_current()
+        self.notifier.stop()
+
+    def press_note(self, note):
+        '''Press a Midi Note'''
+        self.pressed.add(note)
+        self.do_state_check()
+
+    def release_note(self, note):
+        '''Release a Midi Note'''
+        try:
+            self.pressed.remove(note)
+        except KeyError:
+            pass
+        try:
+            self.player.need_to_release.remove(note)
+        except KeyError:
+            pass
+        self.do_state_check()
 
     def do_state_check(self):
         ''' Ticketed wrapper for player's do_state_check '''
         my_ticket = self.state_check_ticket
         self.state_check_ticket += 1
 
         while my_ticket != self.processing_ticket:
@@ -251,62 +297,55 @@
         if my_ticket == self.state_check_ticket - 1:
             self.player.do_state_check()
         else:
             pass
 
         self.processing_ticket += 1
 
-    def hook_NoteOn(self, event):
-        if event.velocity == 0:
-            self.release_note(event.note)
-        else:
-            self.press_note(event.note)
+    def new_controller(self, channel, device_id):
+        if self.controller is not None:
+            self.controller.close()
 
-    def hook_NoteOff(self, event):
-        self.release_note(event.note)
+        self.player.need_to_release = set()
+        self.controller = RoryController(channel, device_id, self)
+        thread = threading.Thread(target=self.controller.listen)
+        thread.start()
+        self.active_key = (channel, device_id)
+
+    def disconnect_current(self):
+        if self.controller is None:
+            return
 
-    def press_note(self, note):
-        '''Press a Midi Note'''
-        self.pressed.add(note)
-        self.do_state_check()
+        self.controller.close()
+        self.controller = None
+
+    def get_active_key(self):
+        return self.active_key
+
+    def is_connected(self):
+        return self.controller is not None
 
-    def release_note(self, note):
-        '''Release a Midi Note'''
-        try:
-            self.pressed.remove(note)
-        except KeyError:
-            pass
-        try:
-            self.player.need_to_release.remove(note)
-        except KeyError:
-            pass
-        self.do_state_check()
 
-    def connect(self, path):
-        self.player.need_to_release = set()
-        try:
-            super().connect(path)
-            # Automatically start listening for input on connect
-            input_thread = threading.Thread(
-                target=self.listen
-            )
-            input_thread.start()
-        except FileNotFoundError:
-            pass
 
 class TaskHandler(pyinotify.ProcessEvent):
     '''Event hooks to connect/disconnect from newly made midi device'''
-    def __init__(self, controller):
-        self.controller = controller
+    def __init__(self, controller_manager):
+        self.controller_manager = controller_manager
         super().__init__()
 
     def process_IN_CREATE(self, event):
         '''Hook to connect when midi device is plugged in'''
         if event.name[0:4] == 'midi':
             time.sleep(.5)
-            self.controller.connect(event.pathname)
+            channel = int(event.name[event.name.rfind("C") + 1])
+            device_id = int(event.name[event.name.rfind("D") + 1])
+            self.controller_manager.new_controller(channel, device_id)
 
     def process_IN_DELETE(self, event):
         '''Hook to disconnect when midi device is unplugged'''
-        if self.controller.midipath == event.pathname:
-            self.controller.disconnect()
+        if 'midi' in event.name:
+            channel = event.name[event.name.rfind("C") + 1]
+            device_id = event.name[event.name.rfind("D") + 1]
+            active_key = self.controller_manager.get_active_key()
+            if active_key == (channel, device_id):
+                self.controller_manager.disconnect_current()
```

### Comparing `rory-0.3.6/rory.egg-info/PKG-INFO` & `rory-0.3.7/rory.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: rory
-Version: 0.3.6
+Version: 0.3.7
 Summary: Play along to MIDI files in console
-Home-page: https://github.com/quintinfsmith/rory
+Home-page: https://burnsomni.net/git/rory
 Author: Quintin Smith
 Author-email: smith.quintin@protonmail.com
 License: GPL-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Rory
 Learn Piano using MIDI files and a MIDI Keyboard<br/>
-[![Travis (.com)](https://img.shields.io/travis/com/quintinfsmith/rory?style=flat-square)](https://travis-ci.com/github/quintinfsmith/rory)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/rory?style=flat-square)](https://pypi.org/project/rory/)
 [![PyPI](https://img.shields.io/pypi/v/rory?style=flat-square)](https://pypi.org/project/rory/)
-[![GitHub](https://img.shields.io/github/license/quintinfsmith/rory?style=flat-square)](https://github.com/quintinfsmith/rory/blob/master/LICENSE)
+[![PyPI - License](https://img.shields.io/pypi/l/rory?style=flat-square)](https://burnsomni.net/project/rory/?branch=master&path=LICENSE)
 
 <img src="https://raw.githubusercontent.com/quintinfsmith/rory/master/res/sample.svg" />
 
 ## Installation
 ```bash
 pip install rory
 ```
```

### Comparing `rory-0.3.6/setup.py` & `rory-0.3.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import setuptools
-from rory import __version__, __author__, __email__, __url__, __license__
+from src import __version__, __author__, __email__, __url__, __license__
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rory",
     version=__version__,
@@ -14,15 +14,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     license=__license__,
     keywords=[],
     python_requires="~=3.7",
     py_modules=["rory"],
     entry_points={ "console_scripts": ["rory = rory:main"] },
-    url="https://github.com/quintinfsmith/rory",
-    packages=setuptools.find_packages(),
+    url="https://burnsomni.net/git/rory",
+    packages=['rory'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Operating System :: POSIX :: Linux",
     ]
 )
```

