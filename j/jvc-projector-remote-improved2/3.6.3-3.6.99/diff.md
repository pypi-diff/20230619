# Comparing `tmp/jvc_projector_remote_improved2-3.6.3.tar.gz` & `tmp/jvc_projector_remote_improved2-3.6.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jvc_projector_remote_improved2-3.6.3.tar", last modified: Mon Jun 19 18:04:49 2023, max compression
+gzip compressed data, was "jvc_projector_remote_improved2-3.6.99.tar", last modified: Fri Jun  2 00:46:05 2023, max compression
```

## Comparing `jvc_projector_remote_improved2-3.6.3.tar` & `jvc_projector_remote_improved2-3.6.99.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:04:49.856130 jvc_projector_remote_improved2-3.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-19 18:04:38.000000 jvc_projector_remote_improved2-3.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-06-19 18:04:49.856130 jvc_projector_remote_improved2-3.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-06-19 18:04:38.000000 jvc_projector_remote_improved2-3.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:04:49.856130 jvc_projector_remote_improved2-3.6.3/jvc_projector/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-19 18:04:38.000000 jvc_projector_remote_improved2-3.6.3/jvc_projector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-06-19 18:04:38.000000 jvc_projector_remote_improved2-3.6.3/jvc_projector/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-06-19 18:04:38.000000 jvc_projector_remote_improved2-3.6.3/jvc_projector/jvc_projector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:04:49.856130 jvc_projector_remote_improved2-3.6.3/jvc_projector_remote_improved2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-06-19 18:04:49.000000 jvc_projector_remote_improved2-3.6.3/jvc_projector_remote_improved2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-19 18:04:49.000000 jvc_projector_remote_improved2-3.6.3/jvc_projector_remote_improved2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 18:04:49.000000 jvc_projector_remote_improved2-3.6.3/jvc_projector_remote_improved2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-19 18:04:49.000000 jvc_projector_remote_improved2-3.6.3/jvc_projector_remote_improved2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 18:04:49.856130 jvc_projector_remote_improved2-3.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-19 18:04:38.000000 jvc_projector_remote_improved2-3.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 18:04:49.856130 jvc_projector_remote_improved2-3.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 18:04:38.000000 jvc_projector_remote_improved2-3.6.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-19 18:04:38.000000 jvc_projector_remote_improved2-3.6.3/tests/testLowLatency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:46:05.123386 jvc_projector_remote_improved2-3.6.99/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-02 00:45:53.000000 jvc_projector_remote_improved2-3.6.99/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-06-02 00:46:05.123386 jvc_projector_remote_improved2-3.6.99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-06-02 00:45:53.000000 jvc_projector_remote_improved2-3.6.99/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:46:05.123386 jvc_projector_remote_improved2-3.6.99/jvc_projector/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-02 00:45:53.000000 jvc_projector_remote_improved2-3.6.99/jvc_projector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-06-02 00:45:53.000000 jvc_projector_remote_improved2-3.6.99/jvc_projector/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23096 2023-06-02 00:45:53.000000 jvc_projector_remote_improved2-3.6.99/jvc_projector/jvc_projector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:46:05.123386 jvc_projector_remote_improved2-3.6.99/jvc_projector_remote_improved2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-06-02 00:46:05.000000 jvc_projector_remote_improved2-3.6.99/jvc_projector_remote_improved2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-02 00:46:05.000000 jvc_projector_remote_improved2-3.6.99/jvc_projector_remote_improved2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 00:46:05.000000 jvc_projector_remote_improved2-3.6.99/jvc_projector_remote_improved2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-02 00:46:05.000000 jvc_projector_remote_improved2-3.6.99/jvc_projector_remote_improved2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 00:46:05.123386 jvc_projector_remote_improved2-3.6.99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-02 00:45:53.000000 jvc_projector_remote_improved2-3.6.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 00:46:05.123386 jvc_projector_remote_improved2-3.6.99/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 00:45:53.000000 jvc_projector_remote_improved2-3.6.99/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-02 00:45:53.000000 jvc_projector_remote_improved2-3.6.99/tests/testLowLatency.py
```

### Comparing `jvc_projector_remote_improved2-3.6.3/LICENSE` & `jvc_projector_remote_improved2-3.6.99/LICENSE`

 * *Files identical despite different names*

### Comparing `jvc_projector_remote_improved2-3.6.3/PKG-INFO` & `jvc_projector_remote_improved2-3.6.99/jvc_projector_remote_improved2.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jvc_projector_remote_improved2
-Version: 3.6.3
+Name: jvc-projector-remote-improved2
+Version: 3.6.99
 Summary: A package to control JVC projectors over IP
 Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -126,205 +126,134 @@
 # edit .env with values
 ```
 ## Supported Commands
 
 `$command,$parameter`
 example: "anamorphic,off"
 example: "anamorphic,d"
-example: "laser_mode,auto3"
+example: "laser_dim,auto3"
 
 It also supports using remote codes as ASCII [found here](https://support.jvc.com/consumer/support/documents/DILAremoteControlGuide.pdf) (Code A only)
 
 `jvc.emulate_remote("23")`
 
 ```
 Currently Supported Commands:
         anamorphic
         aperture
-        aspect_ratio
-        color_mode
-        content_type
-        content_type_trans
         enhance
-        eshift_mode
-        get_model
-        get_software_version
+        eshift
         graphic_mode
-        hdr_data
-        hdr_level
-        hdr_processing
-        input_level
-        input_mode
+        input
         installation_mode
-        lamp_power
-        lamp_time
-        laser_mode
+        laser_dim
         laser_power
         low_latency
         mask
         menu
         motion_enhance
         picture_mode
         power
-        remote
-        source_status
-        theater_optimizer
 
 
 Currently Supported Parameters:
-AnamorphicModes
+anamorphic:
         off
         a
         b
         c
         d
-ApertureModes
+aperture:
         off
         auto1
         auto2
-AspectRatioModes
+aspect_ratio:
         zoom
         auto
         native
-ColorSpaceModes
-        auto
-        YCbCr444
-        YCbCr422
-        RGB
-ContentTypeTrans
-        sdr
-        hdr10_plus
-        hdr10
-        hlg
-ContentTypes
-        auto
-        sdr
-        hdr10_plus
-        hdr10
-        hlg
-EnhanceModes
+enhance:
         zero
         one
         two
         three
         four
         five
         six
         seven
         eight
         nine
         ten
-EshiftModes
+eshift:
         off
         on
-GraphicModeModes
+graphic_mode:
         standard
         hires1
         hires2
-HdrData
-        sdr
-        hdr
-        smpte
-        hybridlog
-        hdr10_plus
-        none
-HdrLevel
-        auto
-        min2
-        min1
-        zero
-        plus1
-        plus2
-HdrProcessing
-        hdr10_plus
-        static
-        frame_by_frame
-        scene_by_scene
-InputLevel
-        standard
-        enhanced
-        superwhite
-        auto
-InputModes
+input:
         hdmi1
         hdmi2
-InstallationModes
+installation_mode:
         mode1
         mode2
         mode3
         mode4
         mode5
         mode6
         mode7
         mode8
         mode9
         mode10
-LampPowerModes
-        normal
-        high
-LaserModes
+laser_dim:
         off
         auto1
         auto2
         auto3
-LaserPowerModes
+laser_power:
         low
         med
         high
-LowLatencyModes
+low_latency:
         off
         on
-MaskModes
+mask:
         on
         off
-MenuModes
+menu:
         menu
         up
         down
         back
         left
         right
         ok
-MotionEnhanceModes
+motion_enhance:
         off
         low
         high
-PictureModes
+picture_mode:
         film
         cinema
         natural
         hdr
-        thx
+        THX
         frame_adapt_hdr
+        frame_adapt_hdr2
+        frame_adapt_hdr3
+        filmmaker
         user1
         user2
         user3
         user4
         user5
         user6
         hlg
         hdr_plus
         pana_pq
-        filmmaker
-        frame_adapt_hdr2
-        frame_adapt_hdr3
-PowerModes
-        off
-        on
-PowerStates
-        standby
-        on
-        cooling
-        reserved
-        emergency
-SourceStatuses
-        logo
-        no_signal
-        signal
-TheaterOptimizer
+power:
         off
         on
 ```
 
 ### Adding new commands
 
 All commands are stored in Enums within `commands.py` so simply adding them to that file in the proper Enum will automatically propagate to code. Add them using [this guide](http://pro.jvc.com/pro/attributes/PRESENT/manual/2018_ILA-FPJ_Ext_Command_List_v1.2.pdf) as a reference.
```

### Comparing `jvc_projector_remote_improved2-3.6.3/README.md` & `jvc_projector_remote_improved2-3.6.99/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: jvc_projector_remote_improved2
+Version: 3.6.99
+Summary: A package to control JVC projectors over IP
+Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
+Author: iloveicedgreentea
+Classifier: Programming Language :: Python :: 3.9
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # JVC Projector Python Library
 
 This implements new features, improvements, and optimizations inspired by https://github.com/bezmi/jvc_projector. This was made with NZ models in mind. Almost every function will work with NX models but I do not guarantee operability for them.
 
 This is designed to work with my Home Assistant plugin: https://github.com/iloveicedgreentea/jvc_homeassistant
 
 ## Installation
@@ -114,205 +126,134 @@
 # edit .env with values
 ```
 ## Supported Commands
 
 `$command,$parameter`
 example: "anamorphic,off"
 example: "anamorphic,d"
-example: "laser_mode,auto3"
+example: "laser_dim,auto3"
 
 It also supports using remote codes as ASCII [found here](https://support.jvc.com/consumer/support/documents/DILAremoteControlGuide.pdf) (Code A only)
 
 `jvc.emulate_remote("23")`
 
 ```
 Currently Supported Commands:
         anamorphic
         aperture
-        aspect_ratio
-        color_mode
-        content_type
-        content_type_trans
         enhance
-        eshift_mode
-        get_model
-        get_software_version
+        eshift
         graphic_mode
-        hdr_data
-        hdr_level
-        hdr_processing
-        input_level
-        input_mode
+        input
         installation_mode
-        lamp_power
-        lamp_time
-        laser_mode
+        laser_dim
         laser_power
         low_latency
         mask
         menu
         motion_enhance
         picture_mode
         power
-        remote
-        source_status
-        theater_optimizer
 
 
 Currently Supported Parameters:
-AnamorphicModes
+anamorphic:
         off
         a
         b
         c
         d
-ApertureModes
+aperture:
         off
         auto1
         auto2
-AspectRatioModes
+aspect_ratio:
         zoom
         auto
         native
-ColorSpaceModes
-        auto
-        YCbCr444
-        YCbCr422
-        RGB
-ContentTypeTrans
-        sdr
-        hdr10_plus
-        hdr10
-        hlg
-ContentTypes
-        auto
-        sdr
-        hdr10_plus
-        hdr10
-        hlg
-EnhanceModes
+enhance:
         zero
         one
         two
         three
         four
         five
         six
         seven
         eight
         nine
         ten
-EshiftModes
+eshift:
         off
         on
-GraphicModeModes
+graphic_mode:
         standard
         hires1
         hires2
-HdrData
-        sdr
-        hdr
-        smpte
-        hybridlog
-        hdr10_plus
-        none
-HdrLevel
-        auto
-        min2
-        min1
-        zero
-        plus1
-        plus2
-HdrProcessing
-        hdr10_plus
-        static
-        frame_by_frame
-        scene_by_scene
-InputLevel
-        standard
-        enhanced
-        superwhite
-        auto
-InputModes
+input:
         hdmi1
         hdmi2
-InstallationModes
+installation_mode:
         mode1
         mode2
         mode3
         mode4
         mode5
         mode6
         mode7
         mode8
         mode9
         mode10
-LampPowerModes
-        normal
-        high
-LaserModes
+laser_dim:
         off
         auto1
         auto2
         auto3
-LaserPowerModes
+laser_power:
         low
         med
         high
-LowLatencyModes
+low_latency:
         off
         on
-MaskModes
+mask:
         on
         off
-MenuModes
+menu:
         menu
         up
         down
         back
         left
         right
         ok
-MotionEnhanceModes
+motion_enhance:
         off
         low
         high
-PictureModes
+picture_mode:
         film
         cinema
         natural
         hdr
-        thx
+        THX
         frame_adapt_hdr
+        frame_adapt_hdr2
+        frame_adapt_hdr3
+        filmmaker
         user1
         user2
         user3
         user4
         user5
         user6
         hlg
         hdr_plus
         pana_pq
-        filmmaker
-        frame_adapt_hdr2
-        frame_adapt_hdr3
-PowerModes
-        off
-        on
-PowerStates
-        standby
-        on
-        cooling
-        reserved
-        emergency
-SourceStatuses
-        logo
-        no_signal
-        signal
-TheaterOptimizer
+power:
         off
         on
 ```
 
 ### Adding new commands
 
 All commands are stored in Enums within `commands.py` so simply adding them to that file in the proper Enum will automatically propagate to code. Add them using [this guide](http://pro.jvc.com/pro/attributes/PRESENT/manual/2018_ILA-FPJ_Ext_Command_List_v1.2.pdf) as a reference.
```

### Comparing `jvc_projector_remote_improved2-3.6.3/jvc_projector/commands.py` & `jvc_projector_remote_improved2-3.6.99/jvc_projector/commands.py`

 * *Files identical despite different names*

### Comparing `jvc_projector_remote_improved2-3.6.3/jvc_projector/jvc_projector.py` & `jvc_projector_remote_improved2-3.6.99/jvc_projector/jvc_projector.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,40 +221,33 @@
             (
                 ack or error message: str,
                 success flag: bool
             )
         """
         # Check commands
         self.logger.debug("Command_type: %s", command_type)
-        self.logger.debug("Send command: %s is of type %s", send_command, type(send_command))
+        self.logger.debug("Send command: %s", send_command)
         self.logger.debug("Send ack: %s", ack)
         if command_type == Header.reference.value:
             return self._do_command(send_command, ack, command_type)
 
         if isinstance(send_command, list):
             # check emulate remote first
-            if "remote" in send_command[0]:
-                try:
-                    _, value = send_command[0].split(",")
-                    return self.emulate_remote(value)
-                except ValueError:
-                    return f"No value for command provided {send_command}", False
-                
+            if send_command[0] == "remote":
+                return self.emulate_remote(send_command[1])
             for cmd in send_command:
                 cons_command, ack = self._construct_command(cmd, command_type)
                 if not ack:
                     return cons_command, ack
                 # need a delay otherwise it kills connection
                 time.sleep(0.1)
                 return self._do_command(cons_command, ack.value, command_type)
 
+        # legacy since HA seems to always use a list
         else:
-            str_cmd = send_command.split(",")
-            if "remote" in str_cmd[0]:
-                return self.emulate_remote(str_cmd[1])
             try:
                 cons_command, ack = self._construct_command(send_command, command_type)
             except TypeError:
                 cons_command = send_command
 
             if not ack:
                 return cons_command, ack
```

### Comparing `jvc_projector_remote_improved2-3.6.3/jvc_projector_remote_improved2.egg-info/PKG-INFO` & `jvc_projector_remote_improved2-3.6.99/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: jvc-projector-remote-improved2
-Version: 3.6.3
-Summary: A package to control JVC projectors over IP
-Home-page: https://github.com/iloveicedgreentea/jvc_projector_improved
-Author: iloveicedgreentea
-Classifier: Programming Language :: Python :: 3.9
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # JVC Projector Python Library
 
 This implements new features, improvements, and optimizations inspired by https://github.com/bezmi/jvc_projector. This was made with NZ models in mind. Almost every function will work with NX models but I do not guarantee operability for them.
 
 This is designed to work with my Home Assistant plugin: https://github.com/iloveicedgreentea/jvc_homeassistant
 
 ## Installation
@@ -126,205 +114,134 @@
 # edit .env with values
 ```
 ## Supported Commands
 
 `$command,$parameter`
 example: "anamorphic,off"
 example: "anamorphic,d"
-example: "laser_mode,auto3"
+example: "laser_dim,auto3"
 
 It also supports using remote codes as ASCII [found here](https://support.jvc.com/consumer/support/documents/DILAremoteControlGuide.pdf) (Code A only)
 
 `jvc.emulate_remote("23")`
 
 ```
 Currently Supported Commands:
         anamorphic
         aperture
-        aspect_ratio
-        color_mode
-        content_type
-        content_type_trans
         enhance
-        eshift_mode
-        get_model
-        get_software_version
+        eshift
         graphic_mode
-        hdr_data
-        hdr_level
-        hdr_processing
-        input_level
-        input_mode
+        input
         installation_mode
-        lamp_power
-        lamp_time
-        laser_mode
+        laser_dim
         laser_power
         low_latency
         mask
         menu
         motion_enhance
         picture_mode
         power
-        remote
-        source_status
-        theater_optimizer
 
 
 Currently Supported Parameters:
-AnamorphicModes
+anamorphic:
         off
         a
         b
         c
         d
-ApertureModes
+aperture:
         off
         auto1
         auto2
-AspectRatioModes
+aspect_ratio:
         zoom
         auto
         native
-ColorSpaceModes
-        auto
-        YCbCr444
-        YCbCr422
-        RGB
-ContentTypeTrans
-        sdr
-        hdr10_plus
-        hdr10
-        hlg
-ContentTypes
-        auto
-        sdr
-        hdr10_plus
-        hdr10
-        hlg
-EnhanceModes
+enhance:
         zero
         one
         two
         three
         four
         five
         six
         seven
         eight
         nine
         ten
-EshiftModes
+eshift:
         off
         on
-GraphicModeModes
+graphic_mode:
         standard
         hires1
         hires2
-HdrData
-        sdr
-        hdr
-        smpte
-        hybridlog
-        hdr10_plus
-        none
-HdrLevel
-        auto
-        min2
-        min1
-        zero
-        plus1
-        plus2
-HdrProcessing
-        hdr10_plus
-        static
-        frame_by_frame
-        scene_by_scene
-InputLevel
-        standard
-        enhanced
-        superwhite
-        auto
-InputModes
+input:
         hdmi1
         hdmi2
-InstallationModes
+installation_mode:
         mode1
         mode2
         mode3
         mode4
         mode5
         mode6
         mode7
         mode8
         mode9
         mode10
-LampPowerModes
-        normal
-        high
-LaserModes
+laser_dim:
         off
         auto1
         auto2
         auto3
-LaserPowerModes
+laser_power:
         low
         med
         high
-LowLatencyModes
+low_latency:
         off
         on
-MaskModes
+mask:
         on
         off
-MenuModes
+menu:
         menu
         up
         down
         back
         left
         right
         ok
-MotionEnhanceModes
+motion_enhance:
         off
         low
         high
-PictureModes
+picture_mode:
         film
         cinema
         natural
         hdr
-        thx
+        THX
         frame_adapt_hdr
+        frame_adapt_hdr2
+        frame_adapt_hdr3
+        filmmaker
         user1
         user2
         user3
         user4
         user5
         user6
         hlg
         hdr_plus
         pana_pq
-        filmmaker
-        frame_adapt_hdr2
-        frame_adapt_hdr3
-PowerModes
-        off
-        on
-PowerStates
-        standby
-        on
-        cooling
-        reserved
-        emergency
-SourceStatuses
-        logo
-        no_signal
-        signal
-TheaterOptimizer
+power:
         off
         on
 ```
 
 ### Adding new commands
 
 All commands are stored in Enums within `commands.py` so simply adding them to that file in the proper Enum will automatically propagate to code. Add them using [this guide](http://pro.jvc.com/pro/attributes/PRESENT/manual/2018_ILA-FPJ_Ext_Command_List_v1.2.pdf) as a reference.
```

### Comparing `jvc_projector_remote_improved2-3.6.3/setup.py` & `jvc_projector_remote_improved2-3.6.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jvc_projector_remote_improved2",
-    version="3.6.3",
+    version="3.6.99",
     author="iloveicedgreentea",
     description="A package to control JVC projectors over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/jvc_projector_improved",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `jvc_projector_remote_improved2-3.6.3/tests/testLowLatency.py` & `jvc_projector_remote_improved2-3.6.99/tests/testLowLatency.py`

 * *Files identical despite different names*

