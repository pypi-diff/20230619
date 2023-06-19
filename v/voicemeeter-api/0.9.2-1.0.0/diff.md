# Comparing `tmp/voicemeeter-api-0.9.2.tar.gz` & `tmp/voicemeeter-api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter-api-0.9.2.tar", max compression
+gzip compressed data, was "voicemeeter-api-1.0.0.tar", max compression
```

## Comparing `voicemeeter-api-0.9.2.tar` & `voicemeeter-api-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter-api-0.9.2/LICENSE
--rw-r--r--   0        0        0      680 2022-10-26 14:27:23.997841 voicemeeter-api-0.9.2/pyproject.toml
--rw-r--r--   0        0        0    14994 2022-10-18 18:16:01.000112 voicemeeter-api-0.9.2/README.md
--rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter-api-0.9.2/voicemeeterlib/__init__.py
--rw-r--r--   0        0        0     8094 2022-10-16 16:28:43.116181 voicemeeter-api-0.9.2/voicemeeterlib/bus.py
--rw-r--r--   0        0        0     3590 2022-08-08 13:33:38.443073 voicemeeter-api-0.9.2/voicemeeterlib/cbindings.py
--rw-r--r--   0        0        0     1249 2022-07-22 14:05:44.167922 voicemeeter-api-0.9.2/voicemeeterlib/command.py
--rw-r--r--   0        0        0     5547 2022-09-28 22:57:08.807371 voicemeeter-api-0.9.2/voicemeeterlib/config.py
--rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter-api-0.9.2/voicemeeterlib/device.py
--rw-r--r--   0        0        0      251 2022-07-07 14:44:58.387087 voicemeeter-api-0.9.2/voicemeeterlib/error.py
--rw-r--r--   0        0        0     2044 2022-10-06 16:39:46.744854 voicemeeter-api-0.9.2/voicemeeterlib/event.py
--rw-r--r--   0        0        0     7525 2022-09-28 22:53:54.781804 voicemeeter-api-0.9.2/voicemeeterlib/factory.py
--rw-r--r--   0        0        0      988 2022-07-07 14:44:58.388087 voicemeeter-api-0.9.2/voicemeeterlib/inst.py
--rw-r--r--   0        0        0     1140 2022-10-11 11:49:25.582533 voicemeeter-api-0.9.2/voicemeeterlib/iremote.py
--rw-r--r--   0        0        0     2302 2022-08-08 13:33:38.445073 voicemeeter-api-0.9.2/voicemeeterlib/kinds.py
--rw-r--r--   0        0        0     1091 2022-10-16 16:37:25.001225 voicemeeter-api-0.9.2/voicemeeterlib/macrobutton.py
--rw-r--r--   0        0        0     1126 2022-10-11 11:06:58.539729 voicemeeter-api-0.9.2/voicemeeterlib/meta.py
--rw-r--r--   0        0        0     6192 2022-09-28 23:00:10.867422 voicemeeter-api-0.9.2/voicemeeterlib/misc.py
--rw-r--r--   0        0        0     1972 2022-07-22 14:04:26.664193 voicemeeter-api-0.9.2/voicemeeterlib/recorder.py
--rw-r--r--   0        0        0     9860 2022-10-04 13:06:59.524105 voicemeeter-api-0.9.2/voicemeeterlib/remote.py
--rw-r--r--   0        0        0    11421 2022-10-27 07:42:21.310552 voicemeeter-api-0.9.2/voicemeeterlib/strip.py
--rw-r--r--   0        0        0     1389 2022-09-29 10:29:54.452484 voicemeeter-api-0.9.2/voicemeeterlib/subject.py
--rw-r--r--   0        0        0     2025 2022-10-04 12:36:39.540193 voicemeeter-api-0.9.2/voicemeeterlib/updater.py
--rw-r--r--   0        0        0     1971 2022-08-08 13:33:38.447073 voicemeeter-api-0.9.2/voicemeeterlib/util.py
--rw-r--r--   0        0        0     4470 2022-08-08 13:33:38.448073 voicemeeter-api-0.9.2/voicemeeterlib/vban.py
--rw-r--r--   0        0        0    15735 2022-10-27 07:51:58.969961 voicemeeter-api-0.9.2/setup.py
--rw-r--r--   0        0        0    14900 2022-10-27 07:51:58.970961 voicemeeter-api-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter-api-1.0.0/LICENSE
+-rw-r--r--   0        0        0      835 2023-06-19 19:13:47.663268 voicemeeter-api-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    14994 2022-10-18 18:16:01.000112 voicemeeter-api-1.0.0/README.md
+-rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter-api-1.0.0/voicemeeterlib/__init__.py
+-rw-r--r--   0        0        0     8094 2022-10-16 16:28:43.116181 voicemeeter-api-1.0.0/voicemeeterlib/bus.py
+-rw-r--r--   0        0        0     3590 2022-08-08 13:33:38.443073 voicemeeter-api-1.0.0/voicemeeterlib/cbindings.py
+-rw-r--r--   0        0        0     1249 2022-07-22 14:05:44.167922 voicemeeter-api-1.0.0/voicemeeterlib/command.py
+-rw-r--r--   0        0        0     5547 2022-09-28 22:57:08.807371 voicemeeter-api-1.0.0/voicemeeterlib/config.py
+-rw-r--r--   0        0        0     1748 2022-07-07 14:44:58.387087 voicemeeter-api-1.0.0/voicemeeterlib/device.py
+-rw-r--r--   0        0        0      251 2022-07-07 14:44:58.387087 voicemeeter-api-1.0.0/voicemeeterlib/error.py
+-rw-r--r--   0        0        0     2044 2022-10-06 16:39:46.744854 voicemeeter-api-1.0.0/voicemeeterlib/event.py
+-rw-r--r--   0        0        0     7525 2023-06-19 18:13:07.464008 voicemeeter-api-1.0.0/voicemeeterlib/factory.py
+-rw-r--r--   0        0        0      988 2022-07-07 14:44:58.388087 voicemeeter-api-1.0.0/voicemeeterlib/inst.py
+-rw-r--r--   0        0        0     1140 2022-10-11 11:49:25.582533 voicemeeter-api-1.0.0/voicemeeterlib/iremote.py
+-rw-r--r--   0        0        0     2302 2022-08-08 13:33:38.445073 voicemeeter-api-1.0.0/voicemeeterlib/kinds.py
+-rw-r--r--   0        0        0     1091 2022-10-16 16:37:25.001225 voicemeeter-api-1.0.0/voicemeeterlib/macrobutton.py
+-rw-r--r--   0        0        0     1126 2022-10-11 11:06:58.539729 voicemeeter-api-1.0.0/voicemeeterlib/meta.py
+-rw-r--r--   0        0        0     6192 2022-09-28 23:00:10.867422 voicemeeter-api-1.0.0/voicemeeterlib/misc.py
+-rw-r--r--   0        0        0     1972 2022-07-22 14:04:26.664193 voicemeeter-api-1.0.0/voicemeeterlib/recorder.py
+-rw-r--r--   0        0        0     9860 2023-06-19 18:13:07.485347 voicemeeter-api-1.0.0/voicemeeterlib/remote.py
+-rw-r--r--   0        0        0    11421 2022-10-27 07:42:21.310552 voicemeeter-api-1.0.0/voicemeeterlib/strip.py
+-rw-r--r--   0        0        0     1389 2022-09-29 10:29:54.452484 voicemeeter-api-1.0.0/voicemeeterlib/subject.py
+-rw-r--r--   0        0        0     2025 2022-10-04 12:36:39.540193 voicemeeter-api-1.0.0/voicemeeterlib/updater.py
+-rw-r--r--   0        0        0     1971 2022-08-08 13:33:38.447073 voicemeeter-api-1.0.0/voicemeeterlib/util.py
+-rw-r--r--   0        0        0     4470 2022-08-08 13:33:38.448073 voicemeeter-api-1.0.0/voicemeeterlib/vban.py
+-rw-r--r--   0        0        0    16024 2023-06-19 19:14:33.802225 voicemeeter-api-1.0.0/setup.py
+-rw-r--r--   0        0        0    14900 2023-06-19 19:14:33.803230 voicemeeter-api-1.0.0/PKG-INFO
```

### Comparing `voicemeeter-api-0.9.2/LICENSE` & `voicemeeter-api-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/README.md` & `voicemeeter-api-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/bus.py` & `voicemeeter-api-1.0.0/voicemeeterlib/bus.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/cbindings.py` & `voicemeeter-api-1.0.0/voicemeeterlib/cbindings.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/command.py` & `voicemeeter-api-1.0.0/voicemeeterlib/command.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/config.py` & `voicemeeter-api-1.0.0/voicemeeterlib/config.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/device.py` & `voicemeeter-api-1.0.0/voicemeeterlib/device.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/event.py` & `voicemeeter-api-1.0.0/voicemeeterlib/event.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/factory.py` & `voicemeeter-api-1.0.0/voicemeeterlib/factory.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/inst.py` & `voicemeeter-api-1.0.0/voicemeeterlib/inst.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/iremote.py` & `voicemeeter-api-1.0.0/voicemeeterlib/iremote.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/kinds.py` & `voicemeeter-api-1.0.0/voicemeeterlib/kinds.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/macrobutton.py` & `voicemeeter-api-1.0.0/voicemeeterlib/macrobutton.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/meta.py` & `voicemeeter-api-1.0.0/voicemeeterlib/meta.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/misc.py` & `voicemeeter-api-1.0.0/voicemeeterlib/misc.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/recorder.py` & `voicemeeter-api-1.0.0/voicemeeterlib/recorder.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/remote.py` & `voicemeeter-api-1.0.0/voicemeeterlib/remote.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/strip.py` & `voicemeeter-api-1.0.0/voicemeeterlib/strip.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/subject.py` & `voicemeeter-api-1.0.0/voicemeeterlib/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/updater.py` & `voicemeeter-api-1.0.0/voicemeeterlib/updater.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/util.py` & `voicemeeter-api-1.0.0/voicemeeterlib/util.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/voicemeeterlib/vban.py` & `voicemeeter-api-1.0.0/voicemeeterlib/vban.py`

 * *Files identical despite different names*

### Comparing `voicemeeter-api-0.9.2/setup.py` & `voicemeeter-api-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,33 @@
 
 package_data = \
 {'': ['*']}
 
 extras_require = \
 {':python_version < "3.11"': ['tomli>=2.0.1,<3.0.0']}
 
+entry_points = \
+{'console_scripts': ['dsl = scripts:ex_dsl',
+                     'midi = scripts:ex_midi',
+                     'obs = scripts:ex_obs',
+                     'observer = scripts:ex_observer',
+                     'test = scripts:test']}
+
 setup_kwargs = {
     'name': 'voicemeeter-api',
-    'version': '0.9.2',
+    'version': '1.0.0',
     'description': 'A Python wrapper for the Voiceemeter API',
     'long_description': '[![PyPI version](https://badge.fury.io/py/voicemeeter-api.svg)](https://badge.fury.io/py/voicemeeter-api)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/onyx-and-iris/voicemeeter-api-python/blob/dev/LICENSE)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)\n![Tests Status](./tests/basic.svg?dummy=8484744)\n![Tests Status](./tests/banana.svg?dummy=8484744)\n![Tests Status](./tests/potato.svg?dummy=8484744)\n\n# Python Wrapper for Voicemeeter API\n\nThis package offers a Python interface for the Voicemeeter Remote C API.\n\nFor an outline of past/future changes refer to: [CHANGELOG](CHANGELOG.md)\n\n## Tested against\n\n-   Basic 1.0.8.4\n-   Banana 2.0.6.4\n-   Potato 3.0.2.4\n\n## Requirements\n\n-   [Voicemeeter](https://voicemeeter.com/)\n-   Python 3.10 or greater\n\n## Installation\n\n`pip install voicemeeter-api`\n\n## `Use`\n\nSimplest use case, use a context manager to request a Remote class of a kind.\n\nLogin and logout are handled for you in this scenario.\n\n#### `__main__.py`\n\n```python\nimport voicemeeterlib\n\n\nclass ManyThings:\n    def __init__(self, vm):\n        self.vm = vm\n\n    def things(self):\n        self.vm.strip[0].label = "podmic"\n        self.vm.strip[0].mute = True\n        print(\n            f"strip 0 ({self.vm.strip[0].label}) mute has been set to {self.vm.strip[0].mute}"\n        )\n\n    def other_things(self):\n        self.vm.bus[3].gain = -6.3\n        self.vm.bus[4].eq = True\n        info = (\n            f"bus 3 gain has been set to {self.vm.bus[3].gain}",\n            f"bus 4 eq has been set to {self.vm.bus[4].eq}",\n        )\n        print("\\n".join(info))\n\n\ndef main():\n    with voicemeeterlib.api(kind_id) as vm:\n        do = ManyThings(vm)\n        do.things()\n        do.other_things()\n\n        # set many parameters at once\n        vm.apply(\n            {\n                "strip-2": {"A1": True, "B1": True, "gain": -6.0},\n                "bus-2": {"mute": True},\n                "button-0": {"state": True},\n                "vban-in-0": {"on": True},\n                "vban-out-1": {"name": "streamname"},\n            }\n        )\n\n\nif __name__ == "__main__":\n    kind_id = "banana"\n\n    main()\n```\n\nOtherwise you must remember to call `vm.login()`, `vm.logout()` at the start/end of your code.\n\n## `kind_id`\n\nPass the kind of Voicemeeter as an argument. kind_id may be:\n\n-   `basic`\n-   `banana`\n-   `potato`\n\n## `Available commands`\n\n### Strip\n\nThe following properties are available.\n\n-   `mono`: boolean\n-   `solo`: boolean\n-   `mute`: boolean\n-   `gain`: float, from -60.0 to 12.0\n-   `comp`: float, from 0.0 to 10.0\n-   `gate`: float, from 0.0 to 10.0\n-   `audibility`: float, from 0.0 to 10.0\n-   `limit`: int, from -40 to 12\n-   `A1 - A5`, `B1 - B3`: boolean\n-   `label`: string\n-   `mc`: boolean\n-   `k`: int, from 0 to 4\n-   `bass`: float, from -12.0 to 12.0\n-   `mid`: float, from -12.0 to 12.0\n-   `treble`: float, from -12.0 to 12.0\n-   `reverb`: float, from 0.0 to 10.0\n-   `delay`: float, from 0.0 to 10.0\n-   `fx1`: float, from 0.0 to 10.0\n-   `fx2`: float, from 0.0 to 10.0\n-   `pan_x`: float, from -0.5 to 0.5\n-   `pan_y`: float, from 0.0 to 1.0\n-   `color_x`: float, from -0.5 to 0.5\n-   `color_y`: float, from 0.0 to 1.0\n-   `fx_x`: float, from -0.5 to 0.5\n-   `fx_y`: float, from 0.0 to 1.0\n-   `postreverb`: boolean\n-   `postdelay`: boolean\n-   `postfx1`: boolean\n-   `postfx2`: boolean\n\nexample:\n\n```python\nvm.strip[3].gain = 3.7\nprint(vm.strip[0].label)\n```\n\nThe following methods are available.\n\n-   `appgain(name, value)`: string, float, from 0.0 to 1.0\n\nSet the gain in db by value for the app matching name.\n\n-   `appmute(name, value)`: string, bool\n\nSet mute state as value for the app matching name.\n\nexample:\n\n```python\nvm.strip[5].appmute("Spotify", True)\nvm.strip[5].appgain("Spotify", 0.5)\n```\n\n##### Gainlayers\n\n-   `gain`: float, from -60.0 to 12.0\n\nexample:\n\n```python\nvm.strip[3].gainlayer[3].gain = 3.7\n```\n\nGainlayers are defined for potato version only.\n\n##### Levels\n\nThe following properties are available.\n\n-   `prefader`\n-   `postfader`\n-   `postmute`\n\nexample:\n\n```python\nprint(vm.strip[3].levels.prefader)\n```\n\nLevel properties will return -200.0 if no audio detected.\n\n### Bus\n\nThe following properties are available.\n\n-   `mono`: boolean\n-   `eq`: boolean\n-   `eq_ab`: boolean\n-   `mute`: boolean\n-   `sel`: boolean\n-   `gain`: float, from -60.0 to 12.0\n-   `label`: string\n-   `returnreverb`: float, from 0.0 to 10.0\n-   `returndelay`: float, from 0.0 to 10.0\n-   `returnfx1`: float, from 0.0 to 10.0\n-   `returnfx2`: float, from 0.0 to 10.0\n-   `monitor`: boolean\n\nexample:\n\n```python\nvm.bus[3].gain = 3.7\nprint(vm.bus[0].label)\n\nvm.bus[4].mono = True\n```\n\n##### Modes\n\nThe following properties are available.\n\n-   `normal`: boolean\n-   `amix`: boolean\n-   `bmix`: boolean\n-   `composite`: boolean\n-   `tvmix`: boolean\n-   `upmix21`: boolean\n-   `upmix41`: boolean\n-   `upmix61`: boolean\n-   `centeronly`: boolean\n-   `lfeonly`: boolean\n-   `rearonly`: boolean\n\nThe following methods are available.\n\n-   `get()`: Returns the current bus mode\n\nexample:\n\n```python\nvm.bus[4].mode.amix = True\n\nprint(vm.bus[2].mode.get())\n```\n\n##### Levels\n\nThe following properties are available.\n\n-   `all`\n\nexample:\n\n```python\nprint(vm.bus[0].levels.all)\n```\n\n`levels.all` will return -200.0 if no audio detected.\n\n### Strip | Bus\n\nThe following methods are available.\n\n-   `fadeto(amount, time)`: float, int\n-   `fadeby(amount, time)`: float, int\n\nModify gain to or by the selected amount in db over a time interval in ms.\n\nexample:\n\n```python\nvm.strip[0].fadeto(-10.3, 1000)\nvm.bus[3].fadeby(-5.6, 500)\n```\n\n#### Strip.Device | Bus.Device\n\nThe following properties are available\n\n-   `name`: str\n-   `sr`: int\n-   `wdm`: str\n-   `ks`: str\n-   `mme`: str\n-   `asio`: str\n\nexample:\n\n```python\nprint(vm.strip[0].device.name)\nvm.bus[0].device.asio = "Audient USB Audio ASIO Driver"\n```\n\nstrip|bus device parameters are defined for physical channels only.\n\nname, sr are read only. wdm, ks, mme, asio are write only.\n\n### Macrobuttons\n\nThe following properties are available.\n\n-   `state`: boolean\n-   `stateonly`: boolean\n-   `trigger`: boolean\n\nexample:\n\n```python\nvm.button[37].state = True\nvm.button[55].trigger = False\n```\n\n### Recorder\n\nThe following methods are available\n\n-   `play()`\n-   `stop()`\n-   `pause()`\n-   `record()`\n-   `ff()`\n-   `rew()`\n-   `load(<filepath>)`: string\n\nThe following properties are available\n\n-   `loop`: boolean\n-   `A1 - A5`: boolean\n-   `B1 - A3`: boolean\n\nexample:\n\n```python\nvm.recorder.play()\nvm.recorder.stop()\n\n# Enable loop play\nvm.recorder.loop = True\n\n# Disable recorder out channel B2\nvm.recorder.B2 = False\n\n# filepath as raw string\nvm.recorder.load(r\'C:\\music\\mytune.mp3\')\n```\n\nRecorder properties are defined as write only.\n\n### VBAN\n\n-   `vm.vban.enable()` `vm.vban.disable()` Turn VBAN on or off\n\n##### Instream | Outstream\n\nThe following properties are available.\n\n-   `on`: boolean\n-   `name`: string\n-   `ip`: string\n-   `port`: int, range from 1024 to 65535\n-   `sr`: int, (11025, 16000, 22050, 24000, 32000, 44100, 48000, 64000, 88200, 96000)\n-   `channel`: int, from 1 to 8\n-   `bit`: int, 16 or 24\n-   `quality`: int, from 0 to 4\n-   `route`: int, from 0 to 8\n\n`SR`, `channel` and `bit` are defined as:\n\n-   readonly for instreams.\n-   read and write for outstreams.\n\nexample:\n\n```python\n# turn VBAN on\nvm.vban.enable()\n\n# turn on vban instream 0\nvm.vban.instream[0].on = True\n\n# set bit property for outstream 3 to 24\nvm.vban.outstream[3].bit = 24\n```\n\n### Command\n\nCertain \'special\' commands are defined by the API as performing actions rather than setting values.\n\nThe following methods are available:\n\n-   `show()` : Bring Voiceemeter GUI to the front\n-   `shutdown()` : Shuts down the GUI\n-   `restart()` : Restart the audio engine\n-   `reset()`: Applies the `reset` config. (phys strip B1, virt strip A1, gains, comp, gate 0.0, mute, mono, solo, eq false)\n\nThe following properties are available.\n\n-   `showvbanchat`: boolean\n-   `lock`: boolean\n\nexample:\n\n```python\nvm.command.restart()\nvm.command.showvbanchat = True\n```\n\n`showvbanchat` and `lock` are write only.\n\n### Device\n\n-   `ins` `outs` : Returns the number of input/output devices\n-   `input(i)` `output(i)` : Returns a dict of device properties for device[i]\n\nexample:\n\n```python\nimport voicemeeterlib\nwith voicemeeterlib.api(kind_id) as vm:\n    for i in range(vm.device.ins):\n        print(vm.device.input(i))\n```\n\n### FX\n\nThe following properties are available:\n\n-   `reverb`: boolean\n-   `reverb_ab`: boolean\n-   `delay`: boolean\n-   `delay_ab`: boolean\n\nexample:\n\n```python\nvm.fx.reverb_ab = True\n```\n\n### Patch\n\nThe following properties are available:\n\n-   `postfadercomposite`: boolean\n-   `postfxinsert`: boolean\n\nexample:\n\n```python\nvm.patch.postfxinsert = False\n```\n\n##### asio[i]\n\n-   `get()`: int\n-   `set(patch_in)`: int, valid range determined by connected device.\n\nexample:\n\n```python\nvm.patch.asio[3].set(4)\n```\n\ni, from 0 to 10\n\n##### A2[i] - A5[i]\n\n-   `get()`: int\n-   `set(patch_out)`: int, valid range determined by connected device.\n\nexample:\n\n```python\nvm.patch.A3[5].set(3)\n```\n\ni, from 0 to 8.\n\n##### composite[i]\n\n-   `get()`: int\n-   `set(channel)`: int, from 0 up to number of channels depending on version.\n\nexample:\n\n```python\nvm.patch.composite[7].set(4)\n```\n\ni, from 0 to 8.\n\n##### insert[i]\n\n-   `on`: boolean\n\nexample:\n\n```python\nvm.patch.insert[18].on = True\n```\n\ni, from 0 up to number of channels depending on version.\n\n### Option\n\nThe following properties are available:\n\n-   `sr`: int\n-   `asiosr`: boolean\n-   `monitoronsel`: boolean\n\nexample:\n\n```python\nvm.option.sr = 48000\n```\n\nThe following methods are available:\n\n-   `buffer(driver, buffer)` : Set buffer size for particular audio driver.\n\nexample:\n\n```python\nvm.option.buffer("wdm", 512)\n```\n\ndriver defined as one of ("mme", "wdm", "ks", "asio")\n\nbuffer, from 128 to 2048\n\n##### delay[i]\n\n-   `get()`: int\n-   `set(delay)`: int, from 0 to 500\n\nexample:\n\n```python\nvm.option.delay[4].set(30)\n```\n\ni, from 0 up to 4.\n\n### Midi\n\nThe following properties are available:\n\n-   `channel`: int, returns the midi channel\n-   `current`: int, returns the current (or most recently pressed) key\n\nThe following methods are available:\n\n-   `get(key)`: int, returns most recent velocity value for a key\n\nexample:\n\n```python\nprint(vm.midi.get(12))\n```\n\nget() may return None if no value for requested key in midi cache\n\n### Multiple parameters\n\n-   `apply`\n    Set many strip/bus/macrobutton/vban parameters at once, for example:\n\n```python\nvm.apply(\n    {\n        "strip-2": {"A1": True, "B1": True, "gain": -6.0},\n        "bus-2": {"mute": True},\n        "button-0": {"state": True},\n        "vban-in-0": {"on": True},\n        "vban-out-1": {"name": "streamname"},\n    }\n)\n```\n\nOr for each class you may do:\n\n```python\nvm.strip[0].apply(mute: True, gain: 3.2, A1: True)\nvm.vban.outstream[0].apply(on: True, name: \'streamname\', bit: 24)\n```\n\n## Config Files\n\n`vm.apply_config(<configname>)`\n\nYou may load config files in TOML format.\nThree example configs have been included with the package. Remember to save\ncurrent settings before loading a user config. To set one you may do:\n\n```python\nimport voicemeeterlib\nwith voicemeeterlib.api(\'banana\') as vm:\n    vm.apply_config(\'example\')\n```\n\nwill load a user config file at configs/banana/example.toml for Voicemeeter Banana.\n\n## Events\n\nLevel updates are considered high volume, by default they are NOT listened for. Use subs keyword arg to initialize event updates.\n\nexample:\n\n```python\nimport voicemeeterlib\n# Set updates to occur every 50ms\n# Listen for level updates but disable midi updates\nwith voicemeeterlib.api(\'banana\', ratelimit=0.05, subs={"ldirty": True, "midi": False}) as vm:\n    ...\n```\n\n#### `vm.subject`\n\nUse the Subject class to register an app as event observer.\n\nThe following methods are available:\n\n-   `add`: registers an app as an event observer\n-   `remove`: deregisters an app as an event observer\n\nexample:\n\n```python\n# register an app to receive updates\nclass App():\n    def __init__(self, vm):\n        vm.subject.add(self)\n        ...\n```\n\n#### `vm.event`\n\nUse the event class to toggle updates as necessary.\n\nThe following properties are available:\n\n-   `pdirty`: boolean\n-   `mdirty`: boolean\n-   `midi`: boolean\n-   `ldirty`: boolean\n\nexample:\n\n```python\nvm.event.ldirty = True\n\nvm.event.pdirty = False\n```\n\nOr add, remove a list of events.\n\nThe following methods are available:\n\n-   `add()`\n-   `remove()`\n-   `get()`\n\nexample:\n\n```python\nvm.event.remove(["pdirty", "mdirty", "midi"])\n\n# get a list of currently subscribed\nprint(vm.event.get())\n```\n\n## Remote class\n\n`voicemeeterlib.api(kind_id: str)`\n\nYou may pass the following optional keyword arguments:\n\n-   `sync`: boolean=False, force the getters to wait for dirty parameters to clear. For most cases leave this as False.\n-   `ratelimit`: float=0.033, how often to check for updates in ms.\n-   `subs`: dict={"pdirty": True, "mdirty": True, "midi": True, "ldirty": False}, initialize which event updates to listen for.\n    -   `pdirty`: parameter updates\n    -   `mdirty`: macrobutton updates\n    -   `midi`: midi updates\n    -   `ldirty`: level updates\n\nAccess to lower level Getters and Setters are provided with these functions:\n\n-   `vm.get(param, is_string=False)`: For getting the value of any parameter. Set string to True if getting a property value expected to return a string.\n-   `vm.set(param, value)`: For setting the value of any parameter.\n\nAccess to lower level polling functions are provided with these functions:\n\n-   `vm.pdirty()`: Returns True if a parameter has been updated.\n-   `vm.mdirty()`: Returns True if a macrobutton has been updated.\n-   `vm.ldirty()`: Returns True if a level has been updated.\n\nexample:\n\n```python\nvm.get(\'Strip[2].Mute\')\nvm.set(\'Strip[4].Label\', \'stripname\')\nvm.set(\'Strip[0].Gain\', -3.6)\n```\n\n### Run tests\n\nTo run all tests:\n\n```\npytest -v\n```\n\n### Official Documentation\n\n-   [Voicemeeter Remote C API](https://github.com/onyx-and-iris/Voicemeeter-SDK/blob/main/VoicemeeterRemoteAPI.pdf)\n',
     'author': 'onyx-and-iris',
     'author_email': 'code@onyxandiris.online',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/onyx-and-iris/voicemeeter-api-python',
     'packages': packages,
     'package_data': package_data,
     'extras_require': extras_require,
+    'entry_points': entry_points,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `voicemeeter-api-0.9.2/PKG-INFO` & `voicemeeter-api-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicemeeter-api
-Version: 0.9.2
+Version: 1.0.0
 Summary: A Python wrapper for the Voiceemeter API
 Home-page: https://github.com/onyx-and-iris/voicemeeter-api-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

