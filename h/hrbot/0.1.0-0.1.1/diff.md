# Comparing `tmp/hrbot-0.1.0.tar.gz` & `tmp/hrbot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrbot-0.1.0.tar", max compression
+gzip compressed data, was "hrbot-0.1.1.tar", max compression
```

## Comparing `hrbot-0.1.0.tar` & `hrbot-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0      158 2023-06-15 08:01:29.191231 hrbot-0.1.0/hrbot/__init__.py
--rw-r--r--   0        0        0       31 2023-05-18 14:31:32.146814 hrbot-0.1.0/hrbot/bot/__init__.py
--rw-r--r--   0        0        0      988 2023-06-15 08:48:39.851385 hrbot-0.1.0/hrbot/bot/base.py
--rw-r--r--   0        0        0     3092 2023-06-14 10:31:36.453525 hrbot-0.1.0/hrbot/bot/bot.py
--rw-r--r--   0        0        0       59 2023-05-18 14:31:32.138854 hrbot-0.1.0/hrbot/dispatcher/__init__.py
--rw-r--r--   0        0        0     8581 2023-06-17 09:43:42.524896 hrbot-0.1.0/hrbot/dispatcher/__pycache__/dispatсher.cpython-311.pyc
--rw-r--r--   0        0        0     5690 2023-06-17 09:43:39.773391 hrbot-0.1.0/hrbot/dispatcher/dispatсher.py
--rw-r--r--   0        0        0     9399 2023-06-14 10:31:36.445953 hrbot-0.1.0/hrbot/dispatcher/filter.py
--rw-r--r--   0        0        0       30 2023-05-31 10:19:08.115326 hrbot-0.1.0/hrbot/dispatcher/fsm/__init__.py
--rw-r--r--   0        0        0     1972 2023-06-15 09:02:33.436860 hrbot-0.1.0/hrbot/dispatcher/fsm/state.py
--rw-r--r--   0        0        0     4675 2023-06-14 06:55:24.164338 hrbot-0.1.0/hrbot/dispatcher/fsm/storage.py
--rw-r--r--   0        0        0     1337 2023-06-14 07:07:30.601511 hrbot-0.1.0/hrbot/dispatcher/handler.py
--rw-r--r--   0        0        0      284 2023-06-11 09:43:38.740611 hrbot-0.1.0/hrbot/types/__init__.py
--rw-r--r--   0        0        0      432 2023-06-14 07:58:57.121193 hrbot-0.1.0/hrbot/types/handler.py
--rw-r--r--   0        0        0       31 2023-05-14 15:25:08.437975 hrbot-0.1.0/hrbot/types/hr.py
--rw-r--r--   0        0        0        0 2023-05-14 13:14:36.307325 hrbot-0.1.0/hrbot/utils/__init__.py
--rw-r--r--   0        0        0      494 2023-06-18 07:13:28.726074 hrbot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      962 2023-06-17 09:59:30.331030 hrbot-0.1.0/README.md
--rw-r--r--   0        0        0     1513 1970-01-01 00:00:00.000000 hrbot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      158 2023-06-15 08:01:29.191231 hrbot-0.1.1/hrbot/__init__.py
+-rw-r--r--   0        0        0       31 2023-05-18 14:31:32.146814 hrbot-0.1.1/hrbot/bot/__init__.py
+-rw-r--r--   0        0        0      988 2023-06-15 08:48:39.851385 hrbot-0.1.1/hrbot/bot/base.py
+-rw-r--r--   0        0        0     3138 2023-06-19 05:53:59.271960 hrbot-0.1.1/hrbot/bot/bot.py
+-rw-r--r--   0        0        0       59 2023-05-18 14:31:32.138854 hrbot-0.1.1/hrbot/dispatcher/__init__.py
+-rw-r--r--   0        0        0     8542 2023-06-19 03:04:48.395643 hrbot-0.1.1/hrbot/dispatcher/__pycache__/dispatсher.cpython-311.pyc
+-rw-r--r--   0        0        0     5652 2023-06-19 02:47:45.490439 hrbot-0.1.1/hrbot/dispatcher/dispatсher.py
+-rw-r--r--   0        0        0     9361 2023-06-19 02:47:45.478983 hrbot-0.1.1/hrbot/dispatcher/filter.py
+-rw-r--r--   0        0        0       30 2023-05-31 10:19:08.115326 hrbot-0.1.1/hrbot/dispatcher/fsm/__init__.py
+-rw-r--r--   0        0        0     1972 2023-06-15 09:02:33.436860 hrbot-0.1.1/hrbot/dispatcher/fsm/state.py
+-rw-r--r--   0        0        0     4675 2023-06-14 06:55:24.164338 hrbot-0.1.1/hrbot/dispatcher/fsm/storage.py
+-rw-r--r--   0        0        0     1337 2023-06-14 07:07:30.601511 hrbot-0.1.1/hrbot/dispatcher/handler.py
+-rw-r--r--   0        0        0      284 2023-06-11 09:43:38.740611 hrbot-0.1.1/hrbot/types/__init__.py
+-rw-r--r--   0        0        0      402 2023-06-19 02:47:45.500862 hrbot-0.1.1/hrbot/types/handler.py
+-rw-r--r--   0        0        0       31 2023-05-14 15:25:08.437975 hrbot-0.1.1/hrbot/types/hr.py
+-rw-r--r--   0        0        0        0 2023-05-14 13:14:36.307325 hrbot-0.1.1/hrbot/utils/__init__.py
+-rw-r--r--   0        0        0     1084 2023-06-18 13:15:36.011849 hrbot-0.1.1/LICENSE
+-rw-r--r--   0        0        0      459 2023-06-19 10:20:38.280823 hrbot-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1612 2023-06-19 07:04:11.369368 hrbot-0.1.1/README.md
+-rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 hrbot-0.1.1/PKG-INFO
```

### Comparing `hrbot-0.1.0/hrbot/bot/base.py` & `hrbot-0.1.1/hrbot/bot/base.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.0/hrbot/bot/bot.py` & `hrbot-0.1.1/hrbot/bot/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     @__event_handler
     async def on_start(self, session_metadata: SessionMetadata) -> None:
         """On a connection to the room being established.
 
         This may be called multiple times, since the connection may be dropped
         and reestablished.
         """
+        self.id = session_metadata.user_id
+
         print(
             f'{_bcolors.WARNING}Bot started in room: '
             f'{_bcolors.FAIL}{session_metadata.room_info.room_name}{_bcolors.ENDC}'
         )
         if self._detailed_start_message:
             print(
                 f'{_bcolors.WARNING}user_id:             {_bcolors.FAIL}{session_metadata.user_id}{_bcolors.ENDC}\n'
```

### Comparing `hrbot-0.1.0/hrbot/dispatcher/__pycache__/dispatсher.cpython-311.pyc` & `hrbot-0.1.1/hrbot/dispatcher/__pycache__/dispatсher.cpython-311.pyc`

 * *Files 11% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x4b808d64 (Sat Jun 17 09:43:39 2023 UTC)
-files sz: 5690
+moddate:  0xd1c18f64 (Mon Jun 19 02:47:45 2023 UTC)
+files sz: 5652
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640264036c026d035a036d
@@ -89,46 +89,46 @@
       ('Optional',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 18
          flags     : 0
          code
-            0x970065005a0164005a02640184005a0364026402640265046a05000000
-            000000000065046a06000000000000000064026402640364049c08640565
-            046a070000000000000000640665046a080000000000000000640765046a
-            08000000000000000064086509650a190000000000000000006409650965
-            0b19000000000000000000640a6509650a19000000000000000000640b65
-            09650a19000000000000000000640c6509650b1900000000000000000066
-            10640d84065a0c64026402640265046a05000000000000000065046a0600
-            0000000000000064026402640364049c08640565046a0700000000000000
-            00640665046a080000000000000000640765046a08000000000000000064
-            086509650a1900000000000000000064096509650b190000000000000000
-            00640a6509650a19000000000000000000640b6509650a19000000000000
-            000000640c6509650b190000000000000000006610640e84065a0d640264
-            02640264026403640f9c05640565046a070000000000000000641065046a
-            080000000000000000641165046a070000000000000000640b6509650a19
-            000000000000000000640c6509650b19000000000000000000660a641284
-            065a0e6402640264026402640364139c05640565046a0700000000000000
-            00641465046a0f0000000000000000641165046a07000000000000000064
-            0b6509650a19000000000000000000640c6509650b190000000000000000
-            00660a641584065a1064026402640364169c03640565046a070000000000
-            000000640b6509650a19000000000000000000640c6509650b1900000000
-            00000000006606641784065a1164026402640364169c03640565046a0700
-            00000000000000640b6509650a19000000000000000000640c6509650b19
-            0000000000000000006606641884065a126402640264026402640364199c
-            05641a65046a070000000000000000641165046a07000000000000000064
-            1b65046a130000000000000000640b6509650a1900000000000000000064
-            0c6509650b19000000000000000000660a641c84065a1464026402640264
-            03641d9c04641e6509650a19000000000000000000640665046a08000000
-            0000000000641f65096515650a1900000000000000000019000000000000
-            000000640c6509650b190000000000000000006608642084065a16640264
-            026402640364219c04640565046a070000000000000000642265046a1700
-            00000000000000640b6509650a19000000000000000000640c6509650b19
-            0000000000000000006608642384065a1864025300
+            0x970065005a0164005a02640184005a03640264026402640365046a0500
+            0000000000000064026402640464059c08640665046a0600000000000000
+            00640765046a070000000000000000640865046a07000000000000000064
+            096508650919000000000000000000640a6508650a190000000000000000
+            00640b6508650919000000000000000000640c6508650919000000000000
+            000000640d6508650a190000000000000000006610640e84065a0b640264
+            026402640365046a05000000000000000064026402640464059c08640665
+            046a060000000000000000640765046a070000000000000000640865046a
+            07000000000000000064096508650919000000000000000000640a650865
+            0a19000000000000000000640b6508650919000000000000000000640c65
+            08650919000000000000000000640d6508650a1900000000000000000066
+            10640f84065a0c6402640264026402640464109c05640665046a06000000
+            0000000000641165046a070000000000000000641265046a060000000000
+            000000640c6508650919000000000000000000640d6508650a1900000000
+            0000000000660a641384065a0d6402640264026402640464149c05640665
+            046a060000000000000000641565046a0e0000000000000000641265046a
+            060000000000000000640c6508650919000000000000000000640d650865
+            0a19000000000000000000660a641684065a0f64026402640464179c0364
+            0665046a060000000000000000640c650865091900000000000000000064
+            0d6508650a190000000000000000006606641884065a1064026402640464
+            179c03640665046a060000000000000000640c6508650919000000000000
+            000000640d6508650a190000000000000000006606641984065a11640264
+            02640264026404641a9c05641b65046a060000000000000000641265046a
+            060000000000000000641c65046a120000000000000000640c6508650919
+            000000000000000000640d6508650a19000000000000000000660a641d84
+            065a136402640264026404641e9c04641f65086509190000000000000000
+            00640765046a070000000000000000642065086514650919000000000000
+            00000019000000000000000000640d6508650a1900000000000000000066
+            08642184065a15640264026402640464229c04640665046a060000000000
+            000000642365046a160000000000000000640c6508650919000000000000
+            000000640d6508650a190000000000000000006608642484065a17640253
+            00
           10           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DispatcherEvents')
                        8 STORE_NAME               2 (__qualname__)
          
           11          10 LOAD_CONST               1 (<code object on_start, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 11>)
@@ -137,418 +137,416 @@
          
           22          16 LOAD_CONST               2 (None)
          
           23          18 LOAD_CONST               2 (None)
          
           24          20 LOAD_CONST               2 (None)
          
-          25          22 LOAD_NAME                4 (handler)
-                      24 LOAD_ATTR                5 (PrefixDefaultValue)
+          25          22 LOAD_CONST               3 ('/.!$#')
          
-          26          34 LOAD_NAME                4 (handler)
-                      36 LOAD_ATTR                6 (CaseIgnoreDefaultValue)
+          26          24 LOAD_NAME                4 (handler)
+                      26 LOAD_ATTR                5 (CaseIgnoreDefaultValue)
          
-          27          46 LOAD_CONST               2 (None)
+          27          36 LOAD_CONST               2 (None)
          
-          28          48 LOAD_CONST               2 (None)
+          28          38 LOAD_CONST               2 (None)
          
-          29          50 LOAD_CONST               3 (False)
+          29          40 LOAD_CONST               4 (False)
          
-          19          52 LOAD_CONST               4 (('user', 'message', 'command', 'prefix', 'case_ignore', 'regex', 'state', 'go_on'))
-                      54 BUILD_CONST_KEY_MAP      8
-                      56 LOAD_CONST               5 ('user')
+          19          42 LOAD_CONST               5 (('user', 'message', 'command', 'prefix', 'case_ignore', 'regex', 'state', 'go_on'))
+                      44 BUILD_CONST_KEY_MAP      8
+                      46 LOAD_CONST               6 ('user')
          
-          22          58 LOAD_NAME                4 (handler)
-                      60 LOAD_ATTR                7 (User)
+          22          48 LOAD_NAME                4 (handler)
+                      50 LOAD_ATTR                6 (User)
          
-          19          70 LOAD_CONST               6 ('message')
+          19          60 LOAD_CONST               7 ('message')
          
-          23          72 LOAD_NAME                4 (handler)
-                      74 LOAD_ATTR                8 (Message)
+          23          62 LOAD_NAME                4 (handler)
+                      64 LOAD_ATTR                7 (Message)
          
-          19          84 LOAD_CONST               7 ('command')
+          19          74 LOAD_CONST               8 ('command')
          
-          24          86 LOAD_NAME                4 (handler)
-                      88 LOAD_ATTR                8 (Message)
+          24          76 LOAD_NAME                4 (handler)
+                      78 LOAD_ATTR                7 (Message)
          
-          19          98 LOAD_CONST               8 ('prefix')
+          19          88 LOAD_CONST               9 ('prefix')
          
-          25         100 LOAD_NAME                9 (Optional)
-                     102 LOAD_NAME               10 (str)
-                     104 BINARY_SUBSCR
+          25          90 LOAD_NAME                8 (Optional)
+                      92 LOAD_NAME                9 (str)
+                      94 BINARY_SUBSCR
          
-          19         114 LOAD_CONST               9 ('case_ignore')
+          19         104 LOAD_CONST              10 ('case_ignore')
          
-          26         116 LOAD_NAME                9 (Optional)
-                     118 LOAD_NAME               11 (bool)
-                     120 BINARY_SUBSCR
+          26         106 LOAD_NAME                8 (Optional)
+                     108 LOAD_NAME               10 (bool)
+                     110 BINARY_SUBSCR
          
-          19         130 LOAD_CONST              10 ('regex')
+          19         120 LOAD_CONST              11 ('regex')
          
-          27         132 LOAD_NAME                9 (Optional)
-                     134 LOAD_NAME               10 (str)
-                     136 BINARY_SUBSCR
+          27         122 LOAD_NAME                8 (Optional)
+                     124 LOAD_NAME                9 (str)
+                     126 BINARY_SUBSCR
          
-          19         146 LOAD_CONST              11 ('state')
+          19         136 LOAD_CONST              12 ('state')
          
-          28         148 LOAD_NAME                9 (Optional)
-                     150 LOAD_NAME               10 (str)
-                     152 BINARY_SUBSCR
+          28         138 LOAD_NAME                8 (Optional)
+                     140 LOAD_NAME                9 (str)
+                     142 BINARY_SUBSCR
          
-          19         162 LOAD_CONST              12 ('go_on')
+          19         152 LOAD_CONST              13 ('go_on')
          
-          29         164 LOAD_NAME                9 (Optional)
-                     166 LOAD_NAME               11 (bool)
-                     168 BINARY_SUBSCR
+          29         154 LOAD_NAME                8 (Optional)
+                     156 LOAD_NAME               10 (bool)
+                     158 BINARY_SUBSCR
          
-          19         178 BUILD_TUPLE             16
-                     180 LOAD_CONST              13 (<code object on_chat, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 19>)
-                     182 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     184 STORE_NAME              12 (on_chat)
+          19         168 BUILD_TUPLE             16
+                     170 LOAD_CONST              14 (<code object on_chat, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 19>)
+                     172 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     174 STORE_NAME              11 (on_chat)
          
-          38         186 LOAD_CONST               2 (None)
+          38         176 LOAD_CONST               2 (None)
          
-          39         188 LOAD_CONST               2 (None)
+          39         178 LOAD_CONST               2 (None)
          
-          40         190 LOAD_CONST               2 (None)
+          40         180 LOAD_CONST               2 (None)
          
-          41         192 LOAD_NAME                4 (handler)
-                     194 LOAD_ATTR                5 (PrefixDefaultValue)
+          41         182 LOAD_CONST               3 ('/.!$#')
          
-          42         204 LOAD_NAME                4 (handler)
-                     206 LOAD_ATTR                6 (CaseIgnoreDefaultValue)
+          42         184 LOAD_NAME                4 (handler)
+                     186 LOAD_ATTR                5 (CaseIgnoreDefaultValue)
          
-          43         216 LOAD_CONST               2 (None)
+          43         196 LOAD_CONST               2 (None)
          
-          44         218 LOAD_CONST               2 (None)
+          44         198 LOAD_CONST               2 (None)
          
-          45         220 LOAD_CONST               3 (False)
+          45         200 LOAD_CONST               4 (False)
          
-          35         222 LOAD_CONST               4 (('user', 'message', 'command', 'prefix', 'case_ignore', 'regex', 'state', 'go_on'))
-                     224 BUILD_CONST_KEY_MAP      8
-                     226 LOAD_CONST               5 ('user')
+          35         202 LOAD_CONST               5 (('user', 'message', 'command', 'prefix', 'case_ignore', 'regex', 'state', 'go_on'))
+                     204 BUILD_CONST_KEY_MAP      8
+                     206 LOAD_CONST               6 ('user')
          
-          38         228 LOAD_NAME                4 (handler)
-                     230 LOAD_ATTR                7 (User)
+          38         208 LOAD_NAME                4 (handler)
+                     210 LOAD_ATTR                6 (User)
          
-          35         240 LOAD_CONST               6 ('message')
+          35         220 LOAD_CONST               7 ('message')
          
-          39         242 LOAD_NAME                4 (handler)
-                     244 LOAD_ATTR                8 (Message)
+          39         222 LOAD_NAME                4 (handler)
+                     224 LOAD_ATTR                7 (Message)
          
-          35         254 LOAD_CONST               7 ('command')
+          35         234 LOAD_CONST               8 ('command')
          
-          40         256 LOAD_NAME                4 (handler)
-                     258 LOAD_ATTR                8 (Message)
+          40         236 LOAD_NAME                4 (handler)
+                     238 LOAD_ATTR                7 (Message)
          
-          35         268 LOAD_CONST               8 ('prefix')
+          35         248 LOAD_CONST               9 ('prefix')
          
-          41         270 LOAD_NAME                9 (Optional)
-                     272 LOAD_NAME               10 (str)
-                     274 BINARY_SUBSCR
+          41         250 LOAD_NAME                8 (Optional)
+                     252 LOAD_NAME                9 (str)
+                     254 BINARY_SUBSCR
          
-          35         284 LOAD_CONST               9 ('case_ignore')
+          35         264 LOAD_CONST              10 ('case_ignore')
          
-          42         286 LOAD_NAME                9 (Optional)
-                     288 LOAD_NAME               11 (bool)
-                     290 BINARY_SUBSCR
+          42         266 LOAD_NAME                8 (Optional)
+                     268 LOAD_NAME               10 (bool)
+                     270 BINARY_SUBSCR
          
-          35         300 LOAD_CONST              10 ('regex')
+          35         280 LOAD_CONST              11 ('regex')
          
-          43         302 LOAD_NAME                9 (Optional)
-                     304 LOAD_NAME               10 (str)
-                     306 BINARY_SUBSCR
+          43         282 LOAD_NAME                8 (Optional)
+                     284 LOAD_NAME                9 (str)
+                     286 BINARY_SUBSCR
          
-          35         316 LOAD_CONST              11 ('state')
+          35         296 LOAD_CONST              12 ('state')
          
-          44         318 LOAD_NAME                9 (Optional)
-                     320 LOAD_NAME               10 (str)
-                     322 BINARY_SUBSCR
+          44         298 LOAD_NAME                8 (Optional)
+                     300 LOAD_NAME                9 (str)
+                     302 BINARY_SUBSCR
          
-          35         332 LOAD_CONST              12 ('go_on')
+          35         312 LOAD_CONST              13 ('go_on')
          
-          45         334 LOAD_NAME                9 (Optional)
-                     336 LOAD_NAME               11 (bool)
-                     338 BINARY_SUBSCR
+          45         314 LOAD_NAME                8 (Optional)
+                     316 LOAD_NAME               10 (bool)
+                     318 BINARY_SUBSCR
          
-          35         348 BUILD_TUPLE             16
-                     350 LOAD_CONST              14 (<code object on_whisper, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 35>)
-                     352 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     354 STORE_NAME              13 (on_whisper)
+          35         328 BUILD_TUPLE             16
+                     330 LOAD_CONST              15 (<code object on_whisper, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 35>)
+                     332 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     334 STORE_NAME              12 (on_whisper)
          
-          54         356 LOAD_CONST               2 (None)
+          54         336 LOAD_CONST               2 (None)
          
-          55         358 LOAD_CONST               2 (None)
+          55         338 LOAD_CONST               2 (None)
          
-          56         360 LOAD_CONST               2 (None)
+          56         340 LOAD_CONST               2 (None)
          
-          57         362 LOAD_CONST               2 (None)
+          57         342 LOAD_CONST               2 (None)
          
-          58         364 LOAD_CONST               3 (False)
+          58         344 LOAD_CONST               4 (False)
          
-          51         366 LOAD_CONST              15 (('user', 'emote_id', 'receiver', 'state', 'go_on'))
-                     368 BUILD_CONST_KEY_MAP      5
-                     370 LOAD_CONST               5 ('user')
+          51         346 LOAD_CONST              16 (('user', 'emote_id', 'receiver', 'state', 'go_on'))
+                     348 BUILD_CONST_KEY_MAP      5
+                     350 LOAD_CONST               6 ('user')
          
-          54         372 LOAD_NAME                4 (handler)
-                     374 LOAD_ATTR                7 (User)
+          54         352 LOAD_NAME                4 (handler)
+                     354 LOAD_ATTR                6 (User)
          
-          51         384 LOAD_CONST              16 ('emote_id')
+          51         364 LOAD_CONST              17 ('emote_id')
          
-          55         386 LOAD_NAME                4 (handler)
-                     388 LOAD_ATTR                8 (Message)
+          55         366 LOAD_NAME                4 (handler)
+                     368 LOAD_ATTR                7 (Message)
          
-          51         398 LOAD_CONST              17 ('receiver')
+          51         378 LOAD_CONST              18 ('receiver')
          
-          56         400 LOAD_NAME                4 (handler)
-                     402 LOAD_ATTR                7 (User)
+          56         380 LOAD_NAME                4 (handler)
+                     382 LOAD_ATTR                6 (User)
          
-          51         412 LOAD_CONST              11 ('state')
+          51         392 LOAD_CONST              12 ('state')
          
-          57         414 LOAD_NAME                9 (Optional)
-                     416 LOAD_NAME               10 (str)
-                     418 BINARY_SUBSCR
+          57         394 LOAD_NAME                8 (Optional)
+                     396 LOAD_NAME                9 (str)
+                     398 BINARY_SUBSCR
          
-          51         428 LOAD_CONST              12 ('go_on')
+          51         408 LOAD_CONST              13 ('go_on')
          
-          58         430 LOAD_NAME                9 (Optional)
-                     432 LOAD_NAME               11 (bool)
-                     434 BINARY_SUBSCR
+          58         410 LOAD_NAME                8 (Optional)
+                     412 LOAD_NAME               10 (bool)
+                     414 BINARY_SUBSCR
          
-          51         444 BUILD_TUPLE             10
-                     446 LOAD_CONST              18 (<code object on_emote, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 51>)
-                     448 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     450 STORE_NAME              14 (on_emote)
+          51         424 BUILD_TUPLE             10
+                     426 LOAD_CONST              19 (<code object on_emote, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 51>)
+                     428 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     430 STORE_NAME              13 (on_emote)
          
-          66         452 LOAD_CONST               2 (None)
+          66         432 LOAD_CONST               2 (None)
          
-          67         454 LOAD_CONST               2 (None)
+          67         434 LOAD_CONST               2 (None)
          
-          68         456 LOAD_CONST               2 (None)
+          68         436 LOAD_CONST               2 (None)
          
-          69         458 LOAD_CONST               2 (None)
+          69         438 LOAD_CONST               2 (None)
          
-          70         460 LOAD_CONST               3 (False)
+          70         440 LOAD_CONST               4 (False)
          
-          64         462 LOAD_CONST              19 (('user', 'reaction', 'receiver', 'state', 'go_on'))
-                     464 BUILD_CONST_KEY_MAP      5
-                     466 LOAD_CONST               5 ('user')
+          64         442 LOAD_CONST              20 (('user', 'reaction', 'receiver', 'state', 'go_on'))
+                     444 BUILD_CONST_KEY_MAP      5
+                     446 LOAD_CONST               6 ('user')
          
-          66         468 LOAD_NAME                4 (handler)
-                     470 LOAD_ATTR                7 (User)
+          66         448 LOAD_NAME                4 (handler)
+                     450 LOAD_ATTR                6 (User)
          
-          64         480 LOAD_CONST              20 ('reaction')
+          64         460 LOAD_CONST              21 ('reaction')
          
-          67         482 LOAD_NAME                4 (handler)
-                     484 LOAD_ATTR               15 (Reaction)
+          67         462 LOAD_NAME                4 (handler)
+                     464 LOAD_ATTR               14 (Reaction)
          
-          64         494 LOAD_CONST              17 ('receiver')
+          64         474 LOAD_CONST              18 ('receiver')
          
-          68         496 LOAD_NAME                4 (handler)
-                     498 LOAD_ATTR                7 (User)
+          68         476 LOAD_NAME                4 (handler)
+                     478 LOAD_ATTR                6 (User)
          
-          64         508 LOAD_CONST              11 ('state')
+          64         488 LOAD_CONST              12 ('state')
          
-          69         510 LOAD_NAME                9 (Optional)
-                     512 LOAD_NAME               10 (str)
-                     514 BINARY_SUBSCR
+          69         490 LOAD_NAME                8 (Optional)
+                     492 LOAD_NAME                9 (str)
+                     494 BINARY_SUBSCR
          
-          64         524 LOAD_CONST              12 ('go_on')
+          64         504 LOAD_CONST              13 ('go_on')
          
-          70         526 LOAD_NAME                9 (Optional)
-                     528 LOAD_NAME               11 (bool)
-                     530 BINARY_SUBSCR
+          70         506 LOAD_NAME                8 (Optional)
+                     508 LOAD_NAME               10 (bool)
+                     510 BINARY_SUBSCR
          
-          64         540 BUILD_TUPLE             10
-                     542 LOAD_CONST              21 (<code object on_reaction, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 64>)
-                     544 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     546 STORE_NAME              16 (on_reaction)
+          64         520 BUILD_TUPLE             10
+                     522 LOAD_CONST              22 (<code object on_reaction, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 64>)
+                     524 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     526 STORE_NAME              15 (on_reaction)
          
-          79         548 LOAD_CONST               2 (None)
+          79         528 LOAD_CONST               2 (None)
          
-          80         550 LOAD_CONST               2 (None)
+          80         530 LOAD_CONST               2 (None)
          
-          81         552 LOAD_CONST               3 (False)
+          81         532 LOAD_CONST               4 (False)
          
-          76         554 LOAD_CONST              22 (('user', 'state', 'go_on'))
-                     556 BUILD_CONST_KEY_MAP      3
-                     558 LOAD_CONST               5 ('user')
+          76         534 LOAD_CONST              23 (('user', 'state', 'go_on'))
+                     536 BUILD_CONST_KEY_MAP      3
+                     538 LOAD_CONST               6 ('user')
          
-          79         560 LOAD_NAME                4 (handler)
-                     562 LOAD_ATTR                7 (User)
+          79         540 LOAD_NAME                4 (handler)
+                     542 LOAD_ATTR                6 (User)
          
-          76         572 LOAD_CONST              11 ('state')
+          76         552 LOAD_CONST              12 ('state')
          
-          80         574 LOAD_NAME                9 (Optional)
-                     576 LOAD_NAME               10 (str)
-                     578 BINARY_SUBSCR
+          80         554 LOAD_NAME                8 (Optional)
+                     556 LOAD_NAME                9 (str)
+                     558 BINARY_SUBSCR
          
-          76         588 LOAD_CONST              12 ('go_on')
+          76         568 LOAD_CONST              13 ('go_on')
          
-          81         590 LOAD_NAME                9 (Optional)
-                     592 LOAD_NAME               11 (bool)
-                     594 BINARY_SUBSCR
+          81         570 LOAD_NAME                8 (Optional)
+                     572 LOAD_NAME               10 (bool)
+                     574 BINARY_SUBSCR
          
-          76         604 BUILD_TUPLE              6
-                     606 LOAD_CONST              23 (<code object on_user_join, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 76>)
-                     608 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     610 STORE_NAME              17 (on_user_join)
+          76         584 BUILD_TUPLE              6
+                     586 LOAD_CONST              24 (<code object on_user_join, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 76>)
+                     588 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     590 STORE_NAME              16 (on_user_join)
          
-          90         612 LOAD_CONST               2 (None)
+          90         592 LOAD_CONST               2 (None)
          
-          91         614 LOAD_CONST               2 (None)
+          91         594 LOAD_CONST               2 (None)
          
-          92         616 LOAD_CONST               3 (False)
+          92         596 LOAD_CONST               4 (False)
          
-          87         618 LOAD_CONST              22 (('user', 'state', 'go_on'))
-                     620 BUILD_CONST_KEY_MAP      3
-                     622 LOAD_CONST               5 ('user')
+          87         598 LOAD_CONST              23 (('user', 'state', 'go_on'))
+                     600 BUILD_CONST_KEY_MAP      3
+                     602 LOAD_CONST               6 ('user')
          
-          90         624 LOAD_NAME                4 (handler)
-                     626 LOAD_ATTR                7 (User)
+          90         604 LOAD_NAME                4 (handler)
+                     606 LOAD_ATTR                6 (User)
          
-          87         636 LOAD_CONST              11 ('state')
+          87         616 LOAD_CONST              12 ('state')
          
-          91         638 LOAD_NAME                9 (Optional)
-                     640 LOAD_NAME               10 (str)
-                     642 BINARY_SUBSCR
+          91         618 LOAD_NAME                8 (Optional)
+                     620 LOAD_NAME                9 (str)
+                     622 BINARY_SUBSCR
          
-          87         652 LOAD_CONST              12 ('go_on')
+          87         632 LOAD_CONST              13 ('go_on')
          
-          92         654 LOAD_NAME                9 (Optional)
-                     656 LOAD_NAME               11 (bool)
-                     658 BINARY_SUBSCR
+          92         634 LOAD_NAME                8 (Optional)
+                     636 LOAD_NAME               10 (bool)
+                     638 BINARY_SUBSCR
          
-          87         668 BUILD_TUPLE              6
-                     670 LOAD_CONST              24 (<code object on_user_leave, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 87>)
-                     672 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     674 STORE_NAME              18 (on_user_leave)
+          87         648 BUILD_TUPLE              6
+                     650 LOAD_CONST              25 (<code object on_user_leave, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 87>)
+                     652 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     654 STORE_NAME              17 (on_user_leave)
          
-         100         676 LOAD_CONST               2 (None)
+         100         656 LOAD_CONST               2 (None)
          
-         101         678 LOAD_CONST               2 (None)
+         101         658 LOAD_CONST               2 (None)
          
-         102         680 LOAD_CONST               2 (None)
+         102         660 LOAD_CONST               2 (None)
          
-         103         682 LOAD_CONST               2 (None)
+         103         662 LOAD_CONST               2 (None)
          
-         104         684 LOAD_CONST               3 (False)
+         104         664 LOAD_CONST               4 (False)
          
-          98         686 LOAD_CONST              25 (('sender', 'receiver', 'tip', 'state', 'go_on'))
-                     688 BUILD_CONST_KEY_MAP      5
-                     690 LOAD_CONST              26 ('sender')
+          98         666 LOAD_CONST              26 (('sender', 'receiver', 'tip', 'state', 'go_on'))
+                     668 BUILD_CONST_KEY_MAP      5
+                     670 LOAD_CONST              27 ('sender')
          
-         100         692 LOAD_NAME                4 (handler)
-                     694 LOAD_ATTR                7 (User)
+         100         672 LOAD_NAME                4 (handler)
+                     674 LOAD_ATTR                6 (User)
          
-          98         704 LOAD_CONST              17 ('receiver')
+          98         684 LOAD_CONST              18 ('receiver')
          
-         101         706 LOAD_NAME                4 (handler)
-                     708 LOAD_ATTR                7 (User)
+         101         686 LOAD_NAME                4 (handler)
+                     688 LOAD_ATTR                6 (User)
          
-          98         718 LOAD_CONST              27 ('tip')
+          98         698 LOAD_CONST              28 ('tip')
          
-         102         720 LOAD_NAME                4 (handler)
-                     722 LOAD_ATTR               19 (Tip)
+         102         700 LOAD_NAME                4 (handler)
+                     702 LOAD_ATTR               18 (Tip)
          
-          98         732 LOAD_CONST              11 ('state')
+          98         712 LOAD_CONST              12 ('state')
          
-         103         734 LOAD_NAME                9 (Optional)
-                     736 LOAD_NAME               10 (str)
-                     738 BINARY_SUBSCR
+         103         714 LOAD_NAME                8 (Optional)
+                     716 LOAD_NAME                9 (str)
+                     718 BINARY_SUBSCR
          
-          98         748 LOAD_CONST              12 ('go_on')
+          98         728 LOAD_CONST              13 ('go_on')
          
-         104         750 LOAD_NAME                9 (Optional)
-                     752 LOAD_NAME               11 (bool)
-                     754 BINARY_SUBSCR
+         104         730 LOAD_NAME                8 (Optional)
+                     732 LOAD_NAME               10 (bool)
+                     734 BINARY_SUBSCR
          
-          98         764 BUILD_TUPLE             10
-                     766 LOAD_CONST              28 (<code object on_tip, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 98>)
-                     768 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     770 STORE_NAME              20 (on_tip)
+          98         744 BUILD_TUPLE             10
+                     746 LOAD_CONST              29 (<code object on_tip, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 98>)
+                     748 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     750 STORE_NAME              19 (on_tip)
          
-         112         772 LOAD_CONST               2 (None)
+         112         752 LOAD_CONST               2 (None)
          
-         113         774 LOAD_CONST               2 (None)
+         113         754 LOAD_CONST               2 (None)
          
-         114         776 LOAD_CONST               2 (None)
+         114         756 LOAD_CONST               2 (None)
          
-         115         778 LOAD_CONST               3 (False)
+         115         758 LOAD_CONST               4 (False)
          
-         110         780 LOAD_CONST              29 (('sender_id', 'message', 'tags', 'go_on'))
-                     782 BUILD_CONST_KEY_MAP      4
-                     784 LOAD_CONST              30 ('sender_id')
+         110         760 LOAD_CONST              30 (('sender_id', 'message', 'tags', 'go_on'))
+                     762 BUILD_CONST_KEY_MAP      4
+                     764 LOAD_CONST              31 ('sender_id')
          
-         112         786 LOAD_NAME                9 (Optional)
-                     788 LOAD_NAME               10 (str)
-                     790 BINARY_SUBSCR
+         112         766 LOAD_NAME                8 (Optional)
+                     768 LOAD_NAME                9 (str)
+                     770 BINARY_SUBSCR
          
-         110         800 LOAD_CONST               6 ('message')
+         110         780 LOAD_CONST               7 ('message')
          
-         113         802 LOAD_NAME                4 (handler)
-                     804 LOAD_ATTR                8 (Message)
+         113         782 LOAD_NAME                4 (handler)
+                     784 LOAD_ATTR                7 (Message)
          
-         110         814 LOAD_CONST              31 ('tags')
+         110         794 LOAD_CONST              32 ('tags')
          
-         114         816 LOAD_NAME                9 (Optional)
-                     818 LOAD_NAME               21 (set)
-                     820 LOAD_NAME               10 (str)
-                     822 BINARY_SUBSCR
-                     832 BINARY_SUBSCR
+         114         796 LOAD_NAME                8 (Optional)
+                     798 LOAD_NAME               20 (set)
+                     800 LOAD_NAME                9 (str)
+                     802 BINARY_SUBSCR
+                     812 BINARY_SUBSCR
          
-         110         842 LOAD_CONST              12 ('go_on')
+         110         822 LOAD_CONST              13 ('go_on')
          
-         115         844 LOAD_NAME                9 (Optional)
-                     846 LOAD_NAME               11 (bool)
-                     848 BINARY_SUBSCR
+         115         824 LOAD_NAME                8 (Optional)
+                     826 LOAD_NAME               10 (bool)
+                     828 BINARY_SUBSCR
          
-         110         858 BUILD_TUPLE              8
-                     860 LOAD_CONST              32 (<code object on_channel, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 110>)
-                     862 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     864 STORE_NAME              22 (on_channel)
+         110         838 BUILD_TUPLE              8
+                     840 LOAD_CONST              33 (<code object on_channel, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 110>)
+                     842 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     844 STORE_NAME              21 (on_channel)
          
-         123         866 LOAD_CONST               2 (None)
+         123         846 LOAD_CONST               2 (None)
          
-         124         868 LOAD_CONST               2 (None)
+         124         848 LOAD_CONST               2 (None)
          
-         125         870 LOAD_CONST               2 (None)
+         125         850 LOAD_CONST               2 (None)
          
-         126         872 LOAD_CONST               3 (False)
+         126         852 LOAD_CONST               4 (False)
          
-         121         874 LOAD_CONST              33 (('user', 'destination', 'state', 'go_on'))
-                     876 BUILD_CONST_KEY_MAP      4
-                     878 LOAD_CONST               5 ('user')
+         121         854 LOAD_CONST              34 (('user', 'destination', 'state', 'go_on'))
+                     856 BUILD_CONST_KEY_MAP      4
+                     858 LOAD_CONST               6 ('user')
          
-         123         880 LOAD_NAME                4 (handler)
-                     882 LOAD_ATTR                7 (User)
+         123         860 LOAD_NAME                4 (handler)
+                     862 LOAD_ATTR                6 (User)
          
-         121         892 LOAD_CONST              34 ('destination')
+         121         872 LOAD_CONST              35 ('destination')
          
-         124         894 LOAD_NAME                4 (handler)
-                     896 LOAD_ATTR               23 (Destination)
+         124         874 LOAD_NAME                4 (handler)
+                     876 LOAD_ATTR               22 (Destination)
          
-         121         906 LOAD_CONST              11 ('state')
+         121         886 LOAD_CONST              12 ('state')
          
-         125         908 LOAD_NAME                9 (Optional)
-                     910 LOAD_NAME               10 (str)
-                     912 BINARY_SUBSCR
+         125         888 LOAD_NAME                8 (Optional)
+                     890 LOAD_NAME                9 (str)
+                     892 BINARY_SUBSCR
          
-         121         922 LOAD_CONST              12 ('go_on')
+         121         902 LOAD_CONST              13 ('go_on')
          
-         126         924 LOAD_NAME                9 (Optional)
-                     926 LOAD_NAME               11 (bool)
-                     928 BINARY_SUBSCR
+         126         904 LOAD_NAME                8 (Optional)
+                     906 LOAD_NAME               10 (bool)
+                     908 BINARY_SUBSCR
          
-         121         938 BUILD_TUPLE              8
-                     940 LOAD_CONST              35 (<code object on_user_move, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 121>)
-                     942 MAKE_FUNCTION            6 (kwdefaults, annotations)
-                     944 STORE_NAME              24 (on_user_move)
-                     946 LOAD_CONST               2 (None)
-                     948 RETURN_VALUE
+         121         918 BUILD_TUPLE              8
+                     920 LOAD_CONST              36 (<code object on_user_move, file "C:\pythonProject\HighRise\NewBotLibrary\hrbot\hrbot\dispatcher\dispatсher.py", line 121>)
+                     922 MAKE_FUNCTION            6 (kwdefaults, annotations)
+                     924 STORE_NAME              23 (on_user_move)
+                     926 LOAD_CONST               2 (None)
+                     928 RETURN_VALUE
          consts
             'DispatcherEvents'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
@@ -565,14 +563,15 @@
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       'on_start'
                firstlineno 11
                lnotab 0x0206
             None
+            '/.!$#'
             False
             ('user', 'message', 'command', 'prefix', 'case_ignore', 'regex', 'state', 'go_on')
             'user'
             'message'
             'command'
             'prefix'
             'case_ignore'
@@ -778,25 +777,25 @@
                varnames   ('user', 'destination', 'state', 'go_on', 'custom_filter', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
                name       'on_user_move'
                firstlineno 121
                lnotab 0x0209
-         names      ('__name__', '__module__', '__qualname__', 'on_start', 'handler', 'PrefixDefaultValue', 'CaseIgnoreDefaultValue', 'User', 'Message', 'Optional', 'str', 'bool', 'on_chat', 'on_whisper', 'on_emote', 'Reaction', 'on_reaction', 'on_user_join', 'on_user_leave', 'Tip', 'on_tip', 'set', 'on_channel', 'Destination', 'on_user_move')
+         names      ('__name__', '__module__', '__qualname__', 'on_start', 'handler', 'CaseIgnoreDefaultValue', 'User', 'Message', 'Optional', 'str', 'bool', 'on_chat', 'on_whisper', 'on_emote', 'Reaction', 'on_reaction', 'on_user_join', 'on_user_leave', 'Tip', 'on_tip', 'set', 'on_channel', 'Destination', 'on_user_move')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\pythonProject\\HighRise\\NewBotLibrary\\hrbot\\hrbot\\dispatcher\\dispatсher.py'
          name       'DispatcherEvents'
          firstlineno 10
          lnotab
-            0x0a01060b0201020102010c010c010201020102f606030cfd02040cfc02
+            0x0a01060b02010201020102010c010201020102f606030cfd02040cfc02
             050cfb02060efa02070ef902080ef802090ef7020a0ef608130201020102
-            010c010c010201020102f606030cfd02040cfc02050cfb02060efa02070e
+            0102010c010201020102f606030cfd02040cfc02050cfb02060efa02070e
             f902080ef802090ef7020a0ef60813020102010201020102f906030cfd02
             040cfc02050cfb02060efa02070ef9080f020102010201020102fa06020c
             fe02030cfd02040cfc02050efb02060efa080f0201020102fb06030cfd02
             040efc02050efb080e0201020102fb06030cfd02040efc02050efb080d02
             0102010201020102fa06020cfe02030cfd02040cfc02050efb02060efa08
             0e02010201020102fb06020efe02030cfd02041afc02050efb080d020102
             01020102fb06020cfe02030cfd02040efc02050efb
```

### Comparing `hrbot-0.1.0/hrbot/dispatcher/dispatсher.py` & `hrbot-0.1.1/hrbot/dispatcher/dispatсher.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     def on_chat(
             self,
             *custom_filter,
             user: handler.User = None,
             message: handler.Message = None,
             command: handler.Message = None,
-            prefix: Optional[str] = handler.PrefixDefaultValue,
+            prefix: Optional[str] = '/.!$#',
             case_ignore: Optional[bool] = handler.CaseIgnoreDefaultValue,
             regex: Optional[str] = None,
             state: Optional[str] = None,
             go_on: Optional[bool] = False,
             **kwargs
     ):
         """On a received room-wide chat."""
@@ -34,15 +34,15 @@
 
     def on_whisper(
             self,
             *custom_filter,
             user: handler.User = None,
             message: handler.Message = None,
             command: handler.Message = None,
-            prefix: Optional[str] = handler.PrefixDefaultValue,
+            prefix: Optional[str] = '/.!$#',
             case_ignore: Optional[bool] = handler.CaseIgnoreDefaultValue,
             regex: Optional[str] = None,
             state: Optional[str] = None,
             go_on: Optional[bool] = False,
             **kwargs
     ):
         """On a received room whisper."""
```

### Comparing `hrbot-0.1.0/hrbot/dispatcher/filter.py` & `hrbot-0.1.1/hrbot/dispatcher/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         *args, **kwargs
 ) -> bool:
     if not await Check.state(user, handler_filter): return False
     if not await Check.compare_two_value(handler_filter.data.user, user): return False
     if not await Check.compare_two_value(handler_filter.data.message,
                                          message, handler_filter.data.case_ignore): return False
     if not await Check.command(handler_filter.data.command,
-                               handler_filter.data.prefix if handler_filter.data.prefix else handler.PrefixDefaultValue,
+                               handler_filter.data.prefix if handler_filter.data.prefix else '/.!$#',
                                message, handler_filter.data.case_ignore): return False
     if not await Check.regex(handler_filter.data.regex, message): return False
     for filter_func in handler_filter.custom_filters:
         if callable(filter_func) and not await Check.func(message, filter_func):
             return False
     return True
 
@@ -118,15 +118,15 @@
         *args, **kwargs
 ) -> bool:
     if not await Check.state(user, handler_filter): return False
     if not await Check.compare_two_value(handler_filter.data.user, user): return False
     if not await Check.compare_two_value(handler_filter.data.message,
                                          message, handler_filter.data.case_ignore): return False
     if not await Check.command(handler_filter.data.command,
-                               handler_filter.data.prefix if handler_filter.data.prefix else handler.PrefixDefaultValue,
+                               handler_filter.data.prefix if handler_filter.data.prefix else '/.!$#',
                                message, handler_filter.data.case_ignore): return False
     if not await Check.regex(handler_filter.data.regex, message): return False
     for filter_func in handler_filter.custom_filters:
         if callable(filter_func) and not await Check.func(message, filter_func):
             return False
     return True
```

### Comparing `hrbot-0.1.0/hrbot/dispatcher/fsm/state.py` & `hrbot-0.1.1/hrbot/dispatcher/fsm/state.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.0/hrbot/dispatcher/fsm/storage.py` & `hrbot-0.1.1/hrbot/dispatcher/fsm/storage.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.0/hrbot/dispatcher/handler.py` & `hrbot-0.1.1/hrbot/dispatcher/handler.py`

 * *Files identical despite different names*

### Comparing `hrbot-0.1.0/README.md` & `hrbot-0.1.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,50 @@
-# The hrbot
-The hrbot is a wrapper on top of the [HighRise Python Bot SDK](https://github.com/pocketzworld/python-bot-sdk) that makes it easy to create bots in [HighRise](https://highrise.game/).
 
-Install the library:
-```shell
-pip install hrbot
-```
-
-Example:
-```python
+# The hrbot  
+The hrbot is a wrapper on top of the [HighRise Python Bot SDK](https://github.com/pocketzworld/python-bot-sdk) that makes it easy to create bots in [HighRise](https://highrise.game/).  
+  
+Install the library:  
+```shell  
+pip install hrbot  
+```  
+# Features:  
+- Quick and easy creation of an unlimited number of handlers for any event  
+- FSM (finite state machine). Available storage in memory and Redis  
+- Large number of available conditions in handlers  
+# Unreleased features:
+- Web API support
+- Spam blocking bypass. Allows you to send an unlimited number of identical messages
+# Example:  
+```python  
 from hrbot import Bot, Dispatcher  
-from hrbot.types.hr import *
-
-dp = Dispatcher()
-bot = Bot(
-    api_key='',
-    room_id='',
-    dispatcher=dp
-)
-
-@dp.on_user_join()
-async def user_join(user: User):
-    await bot.highrise.chat(f'Hi, {user.username}')
-
-@dp.on_chat(command='help', case_ignore=True, prefix='!')
-async def help_command(user: User, message: str):
-    await bot.highrise.chat('some text')
-
-@dp.on_chat()
-async def echo(user: User, message: str):
+from hrbot.types.hr import User  
+  
+dp = Dispatcher()  
+bot = Bot(  
+    api_key='',  
+    room_id='',  
+    dispatcher=dp  
+)  
+  
+@dp.on_user_join()  
+async def user_join(user: User):  
+    """Triggers when a player joins a room"""  
+    await bot.highrise.chat(f'Hi, {user.username}')  
+  
+@dp.on_user_leave()  
+async def user_leave(user: User):  
+    """Triggers when a player leaves the room"""  
+    await bot.highrise.chat(f'Goodbye, {user.username}')  
+  
+@dp.on_chat(command='help', case_ignore=True, prefix='.!')  
+async def help_command(user: User, message: str):  
+    """Works for .help and !help messages. Not case-sensitive"""  
+    await bot.highrise.chat("Some text for help command")  
+  
+@dp.on_chat()  
+async def echo(user: User, message: str):  
+    """Works for all chat messages"""  
     await bot.highrise.chat(message)
-
-@dp.on_user_leave()
-async def user_leave(user: User):
-    await bot.highrise.chat(f'Goodbye, {user.username}')
-
-if __name__ == '__main__':
-    bot.start()
+  
+if __name__ == '__main__':  
+    bot.start()  
 ```
```

### Comparing `hrbot-0.1.0/PKG-INFO` & `hrbot-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,66 @@
 Metadata-Version: 2.1
 Name: hrbot
-Version: 0.1.0
+Version: 0.1.1
 Summary: The hrbot is a wrapper on top of the HighRise Python Bot SDK that makes it easy to create bots in HighRise.
 License: MIT
 Author: MuoDosta
 Author-email: MuoDostaWork@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: highrise-bot-sdk (==23.1.0b12)
-Requires-Dist: redis (>=4.5.5,<5.0.0)
+Requires-Dist: redis (==4.5.5)
 Description-Content-Type: text/markdown
 
-# The hrbot
-The hrbot is a wrapper on top of the [HighRise Python Bot SDK](https://github.com/pocketzworld/python-bot-sdk) that makes it easy to create bots in [HighRise](https://highrise.game/).
 
-Install the library:
-```shell
-pip install hrbot
-```
-
-Example:
-```python
+# The hrbot  
+The hrbot is a wrapper on top of the [HighRise Python Bot SDK](https://github.com/pocketzworld/python-bot-sdk) that makes it easy to create bots in [HighRise](https://highrise.game/).  
+  
+Install the library:  
+```shell  
+pip install hrbot  
+```  
+# Features:  
+- Quick and easy creation of an unlimited number of handlers for any event  
+- FSM (finite state machine). Available storage in memory and Redis  
+- Large number of available conditions in handlers  
+# Unreleased features:
+- Web API support
+- Spam blocking bypass. Allows you to send an unlimited number of identical messages
+# Example:  
+```python  
 from hrbot import Bot, Dispatcher  
-from hrbot.types.hr import *
-
-dp = Dispatcher()
-bot = Bot(
-    api_key='',
-    room_id='',
-    dispatcher=dp
-)
-
-@dp.on_user_join()
-async def user_join(user: User):
-    await bot.highrise.chat(f'Hi, {user.username}')
-
-@dp.on_chat(command='help', case_ignore=True, prefix='!')
-async def help_command(user: User, message: str):
-    await bot.highrise.chat('some text')
-
-@dp.on_chat()
-async def echo(user: User, message: str):
+from hrbot.types.hr import User  
+  
+dp = Dispatcher()  
+bot = Bot(  
+    api_key='',  
+    room_id='',  
+    dispatcher=dp  
+)  
+  
+@dp.on_user_join()  
+async def user_join(user: User):  
+    """Triggers when a player joins a room"""  
+    await bot.highrise.chat(f'Hi, {user.username}')  
+  
+@dp.on_user_leave()  
+async def user_leave(user: User):  
+    """Triggers when a player leaves the room"""  
+    await bot.highrise.chat(f'Goodbye, {user.username}')  
+  
+@dp.on_chat(command='help', case_ignore=True, prefix='.!')  
+async def help_command(user: User, message: str):  
+    """Works for .help and !help messages. Not case-sensitive"""  
+    await bot.highrise.chat("Some text for help command")  
+  
+@dp.on_chat()  
+async def echo(user: User, message: str):  
+    """Works for all chat messages"""  
     await bot.highrise.chat(message)
-
-@dp.on_user_leave()
-async def user_leave(user: User):
-    await bot.highrise.chat(f'Goodbye, {user.username}')
-
-if __name__ == '__main__':
-    bot.start()
+  
+if __name__ == '__main__':  
+    bot.start()  
 ```
```

