# Comparing `tmp/simpleplayer-1.0.4.tar.gz` & `tmp/simpleplayer-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleplayer-1.0.4.tar", last modified: Mon Jun 19 07:07:06 2023, max compression
+gzip compressed data, was "simpleplayer-1.0.5.tar", last modified: Mon Jun 19 17:17:14 2023, max compression
```

## Comparing `simpleplayer-1.0.4.tar` & `simpleplayer-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-19 07:07:06.981432 simpleplayer-1.0.4/
--rw-r--r--   0 thowie     (501) staff       (20)     1067 2023-06-19 07:04:08.000000 simpleplayer-1.0.4/LICENSE
--rw-r--r--   0 thowie     (501) staff       (20)     3839 2023-06-19 07:07:06.981303 simpleplayer-1.0.4/PKG-INFO
--rw-r--r--   0 thowie     (501) staff       (20)     3481 2023-06-19 07:06:10.000000 simpleplayer-1.0.4/README.md
--rw-r--r--   0 thowie     (501) staff       (20)       38 2023-06-19 07:07:06.981482 simpleplayer-1.0.4/setup.cfg
--rw-r--r--   0 thowie     (501) staff       (20)      875 2023-06-19 06:02:52.000000 simpleplayer-1.0.4/setup.py
-drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-19 07:07:06.980338 simpleplayer-1.0.4/simpleplayer/
--rw-r--r--   0 thowie     (501) staff       (20)       69 2023-06-19 05:57:07.000000 simpleplayer-1.0.4/simpleplayer/__init__.py
--rw-r--r--   0 thowie     (501) staff       (20)     3139 2023-06-19 06:32:02.000000 simpleplayer-1.0.4/simpleplayer/simpleplayer.py
--rw-r--r--   0 thowie     (501) staff       (20)     1369 2023-06-19 06:32:22.000000 simpleplayer-1.0.4/simpleplayer/voicegen.py
-drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-19 07:07:06.981089 simpleplayer-1.0.4/simpleplayer.egg-info/
--rw-r--r--   0 thowie     (501) staff       (20)     3839 2023-06-19 07:07:06.000000 simpleplayer-1.0.4/simpleplayer.egg-info/PKG-INFO
--rw-r--r--   0 thowie     (501) staff       (20)      323 2023-06-19 07:07:06.000000 simpleplayer-1.0.4/simpleplayer.egg-info/SOURCES.txt
--rw-r--r--   0 thowie     (501) staff       (20)        1 2023-06-19 07:07:06.000000 simpleplayer-1.0.4/simpleplayer.egg-info/dependency_links.txt
--rw-r--r--   0 thowie     (501) staff       (20)      102 2023-06-19 07:07:06.000000 simpleplayer-1.0.4/simpleplayer.egg-info/entry_points.txt
--rw-r--r--   0 thowie     (501) staff       (20)       33 2023-06-19 07:07:06.000000 simpleplayer-1.0.4/simpleplayer.egg-info/requires.txt
--rw-r--r--   0 thowie     (501) staff       (20)       13 2023-06-19 07:07:06.000000 simpleplayer-1.0.4/simpleplayer.egg-info/top_level.txt
+drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-19 17:17:14.521428 simpleplayer-1.0.5/
+-rw-r--r--   0 thowie     (501) staff       (20)     1067 2023-06-19 07:04:08.000000 simpleplayer-1.0.5/LICENSE
+-rw-r--r--   0 thowie     (501) staff       (20)     3856 2023-06-19 17:17:14.521268 simpleplayer-1.0.5/PKG-INFO
+-rw-r--r--   0 thowie     (501) staff       (20)     3485 2023-06-19 17:02:11.000000 simpleplayer-1.0.5/README.md
+-rw-r--r--   0 thowie     (501) staff       (20)       38 2023-06-19 17:17:14.521498 simpleplayer-1.0.5/setup.cfg
+-rw-r--r--   0 thowie     (501) staff       (20)      895 2023-06-19 17:06:51.000000 simpleplayer-1.0.5/setup.py
+drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-19 17:17:14.519910 simpleplayer-1.0.5/simpleplayer/
+-rw-r--r--   0 thowie     (501) staff       (20)       69 2023-06-19 17:04:49.000000 simpleplayer-1.0.5/simpleplayer/__init__.py
+-rw-r--r--   0 thowie     (501) staff       (20)     3787 2023-06-19 17:16:53.000000 simpleplayer-1.0.5/simpleplayer/simpleplayer.py
+-rw-r--r--   0 thowie     (501) staff       (20)     1433 2023-06-19 16:42:57.000000 simpleplayer-1.0.5/simpleplayer/voicegen.py
+drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-19 17:17:14.520942 simpleplayer-1.0.5/simpleplayer.egg-info/
+-rw-r--r--   0 thowie     (501) staff       (20)     3856 2023-06-19 17:17:14.000000 simpleplayer-1.0.5/simpleplayer.egg-info/PKG-INFO
+-rw-r--r--   0 thowie     (501) staff       (20)      323 2023-06-19 17:17:14.000000 simpleplayer-1.0.5/simpleplayer.egg-info/SOURCES.txt
+-rw-r--r--   0 thowie     (501) staff       (20)        1 2023-06-19 17:17:14.000000 simpleplayer-1.0.5/simpleplayer.egg-info/dependency_links.txt
+-rw-r--r--   0 thowie     (501) staff       (20)      102 2023-06-19 17:17:14.000000 simpleplayer-1.0.5/simpleplayer.egg-info/entry_points.txt
+-rw-r--r--   0 thowie     (501) staff       (20)       33 2023-06-19 17:17:14.000000 simpleplayer-1.0.5/simpleplayer.egg-info/requires.txt
+-rw-r--r--   0 thowie     (501) staff       (20)       13 2023-06-19 17:17:14.000000 simpleplayer-1.0.5/simpleplayer.egg-info/top_level.txt
```

### Comparing `simpleplayer-1.0.4/LICENSE` & `simpleplayer-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleplayer-1.0.4/PKG-INFO` & `simpleplayer-1.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: simpleplayer
-Version: 1.0.4
+Version: 1.0.5
 Summary: Discover the pinnacle of audio elegance with this simple-player module, boasting a sophisticated blend of advanced features and seamless compatibility across multiple platforms.
 Author: TOWDIO
 Author-email: thowiestudio@gmail.com
+License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Simple Player
 
 Discover the pinnacle of audio elegance with this `simpleplayer` module, boasting a sophisticated blend of advanced features and seamless compatibility across multiple platforms.
 
@@ -28,18 +29,18 @@
 You can also use the module directly from the terminal:
 ```
 simpleplayer path/to/your/audio/file.wav
 ```
 
 ## Usage
 
-Import the `AudioPlayer` class from the `simpleplayer` module:
+Import the `simpleplayer` class from the `simpleplayer` module:
 
 ```python
-from simpleplayer import AudioPlayer
+from simpleplayer import simpleplayer
 ```
 
 Create an instance of the AudioPlayer class, providing the filename of the audio file as a parameter:
 
 ```python
 player = AudioPlayer('path/to/your/audio/file.wav')
 ```
@@ -85,18 +86,18 @@
 <br>
 
 ## Example
 
 Here's an example that demonstrates the usage of the AudioPlayer module:
     
 ```python
-from simpleplayer import AudioPlayer
+from simpleplayer import simpleplayer
 
 # Create an instance of AudioPlayer
-player = AudioPlayer('path/to/your/audio/file.wav')
+player = simpleplayer('path/to/your/audio/file.wav')
 
 # Start playing the audio
 player.play()
 player.wait()
 
 # Perform actions or wait for the audio to finish
```

### Comparing `simpleplayer-1.0.4/README.md` & `simpleplayer-1.0.5/simpleplayer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: simpleplayer
+Version: 1.0.5
+Summary: Discover the pinnacle of audio elegance with this simple-player module, boasting a sophisticated blend of advanced features and seamless compatibility across multiple platforms.
+Author: TOWDIO
+Author-email: thowiestudio@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Simple Player
 
 Discover the pinnacle of audio elegance with this `simpleplayer` module, boasting a sophisticated blend of advanced features and seamless compatibility across multiple platforms.
 
 <br>
 
 ## Installation
@@ -19,18 +29,18 @@
 You can also use the module directly from the terminal:
 ```
 simpleplayer path/to/your/audio/file.wav
 ```
 
 ## Usage
 
-Import the `AudioPlayer` class from the `simpleplayer` module:
+Import the `simpleplayer` class from the `simpleplayer` module:
 
 ```python
-from simpleplayer import AudioPlayer
+from simpleplayer import simpleplayer
 ```
 
 Create an instance of the AudioPlayer class, providing the filename of the audio file as a parameter:
 
 ```python
 player = AudioPlayer('path/to/your/audio/file.wav')
 ```
@@ -76,18 +86,18 @@
 <br>
 
 ## Example
 
 Here's an example that demonstrates the usage of the AudioPlayer module:
     
 ```python
-from simpleplayer import AudioPlayer
+from simpleplayer import simpleplayer
 
 # Create an instance of AudioPlayer
-player = AudioPlayer('path/to/your/audio/file.wav')
+player = simpleplayer('path/to/your/audio/file.wav')
 
 # Start playing the audio
 player.play()
 player.wait()
 
 # Perform actions or wait for the audio to finish
```

### Comparing `simpleplayer-1.0.4/setup.py` & `simpleplayer-1.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of README.md file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='simpleplayer',
-    version='1.0.4',
+    version='1.0.5',
     description='Discover the pinnacle of audio elegance with this simple-player module, boasting a sophisticated blend of advanced features and seamless compatibility across multiple platforms.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='TOWDIO',
     author_email='thowiestudio@gmail.com',
     packages=['simpleplayer'],
     install_requires=[
@@ -20,9 +20,10 @@
         'gtts',
     ],
     entry_points={
         'console_scripts': [
             'simpleplayer = simpleplayer.simpleplayer:main',
             'voicegen = simpleplayer.voicegen:main',
         ],
-    }
+    },
+    license='MIT',
 )
```

### Comparing `simpleplayer-1.0.4/simpleplayer.egg-info/PKG-INFO` & `simpleplayer-1.0.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: simpleplayer
-Version: 1.0.4
-Summary: Discover the pinnacle of audio elegance with this simple-player module, boasting a sophisticated blend of advanced features and seamless compatibility across multiple platforms.
-Author: TOWDIO
-Author-email: thowiestudio@gmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Simple Player
 
 Discover the pinnacle of audio elegance with this `simpleplayer` module, boasting a sophisticated blend of advanced features and seamless compatibility across multiple platforms.
 
 <br>
 
 ## Installation
@@ -28,18 +19,18 @@
 You can also use the module directly from the terminal:
 ```
 simpleplayer path/to/your/audio/file.wav
 ```
 
 ## Usage
 
-Import the `AudioPlayer` class from the `simpleplayer` module:
+Import the `simpleplayer` class from the `simpleplayer` module:
 
 ```python
-from simpleplayer import AudioPlayer
+from simpleplayer import simpleplayer
 ```
 
 Create an instance of the AudioPlayer class, providing the filename of the audio file as a parameter:
 
 ```python
 player = AudioPlayer('path/to/your/audio/file.wav')
 ```
@@ -85,18 +76,18 @@
 <br>
 
 ## Example
 
 Here's an example that demonstrates the usage of the AudioPlayer module:
     
 ```python
-from simpleplayer import AudioPlayer
+from simpleplayer import simpleplayer
 
 # Create an instance of AudioPlayer
-player = AudioPlayer('path/to/your/audio/file.wav')
+player = simpleplayer('path/to/your/audio/file.wav')
 
 # Start playing the audio
 player.play()
 player.wait()
 
 # Perform actions or wait for the audio to finish
```

