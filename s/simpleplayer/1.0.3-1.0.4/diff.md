# Comparing `tmp/simpleplayer-1.0.3.tar.gz` & `tmp/simpleplayer-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleplayer-1.0.3.tar", last modified: Mon Jun 19 05:05:20 2023, max compression
+gzip compressed data, was "simpleplayer-1.0.4.tar", last modified: Mon Jun 19 07:07:06 2023, max compression
```

## Comparing `simpleplayer-1.0.3.tar` & `simpleplayer-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-19 05:05:20.431295 simpleplayer-1.0.3/
--rw-r--r--   0 thowie     (501) staff       (20)     4058 2023-06-19 05:05:20.431134 simpleplayer-1.0.3/PKG-INFO
--rw-r--r--   0 thowie     (501) staff       (20)     3722 2023-06-19 04:24:30.000000 simpleplayer-1.0.3/README.md
--rw-r--r--   0 thowie     (501) staff       (20)       38 2023-06-19 05:05:20.431359 simpleplayer-1.0.3/setup.cfg
--rw-r--r--   0 thowie     (501) staff       (20)      808 2023-06-19 05:04:21.000000 simpleplayer-1.0.3/setup.py
-drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-19 05:05:20.429867 simpleplayer-1.0.3/simpleplayer/
--rw-r--r--   0 thowie     (501) staff       (20)       38 2023-06-18 12:06:16.000000 simpleplayer-1.0.3/simpleplayer/__init__.py
--rw-r--r--   0 thowie     (501) staff       (20)     2742 2023-06-19 04:22:31.000000 simpleplayer-1.0.3/simpleplayer/simpleplayer.py
-drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-19 05:05:20.430870 simpleplayer-1.0.3/simpleplayer.egg-info/
--rw-r--r--   0 thowie     (501) staff       (20)     4058 2023-06-19 05:05:20.000000 simpleplayer-1.0.3/simpleplayer.egg-info/PKG-INFO
--rw-r--r--   0 thowie     (501) staff       (20)      290 2023-06-19 05:05:20.000000 simpleplayer-1.0.3/simpleplayer.egg-info/SOURCES.txt
--rw-r--r--   0 thowie     (501) staff       (20)        1 2023-06-19 05:05:20.000000 simpleplayer-1.0.3/simpleplayer.egg-info/dependency_links.txt
--rw-r--r--   0 thowie     (501) staff       (20)       64 2023-06-19 05:05:20.000000 simpleplayer-1.0.3/simpleplayer.egg-info/entry_points.txt
--rw-r--r--   0 thowie     (501) staff       (20)       28 2023-06-19 05:05:20.000000 simpleplayer-1.0.3/simpleplayer.egg-info/requires.txt
--rw-r--r--   0 thowie     (501) staff       (20)       13 2023-06-19 05:05:20.000000 simpleplayer-1.0.3/simpleplayer.egg-info/top_level.txt
+drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-19 07:07:06.981432 simpleplayer-1.0.4/
+-rw-r--r--   0 thowie     (501) staff       (20)     1067 2023-06-19 07:04:08.000000 simpleplayer-1.0.4/LICENSE
+-rw-r--r--   0 thowie     (501) staff       (20)     3839 2023-06-19 07:07:06.981303 simpleplayer-1.0.4/PKG-INFO
+-rw-r--r--   0 thowie     (501) staff       (20)     3481 2023-06-19 07:06:10.000000 simpleplayer-1.0.4/README.md
+-rw-r--r--   0 thowie     (501) staff       (20)       38 2023-06-19 07:07:06.981482 simpleplayer-1.0.4/setup.cfg
+-rw-r--r--   0 thowie     (501) staff       (20)      875 2023-06-19 06:02:52.000000 simpleplayer-1.0.4/setup.py
+drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-19 07:07:06.980338 simpleplayer-1.0.4/simpleplayer/
+-rw-r--r--   0 thowie     (501) staff       (20)       69 2023-06-19 05:57:07.000000 simpleplayer-1.0.4/simpleplayer/__init__.py
+-rw-r--r--   0 thowie     (501) staff       (20)     3139 2023-06-19 06:32:02.000000 simpleplayer-1.0.4/simpleplayer/simpleplayer.py
+-rw-r--r--   0 thowie     (501) staff       (20)     1369 2023-06-19 06:32:22.000000 simpleplayer-1.0.4/simpleplayer/voicegen.py
+drwxr-xr-x   0 thowie     (501) staff       (20)        0 2023-06-19 07:07:06.981089 simpleplayer-1.0.4/simpleplayer.egg-info/
+-rw-r--r--   0 thowie     (501) staff       (20)     3839 2023-06-19 07:07:06.000000 simpleplayer-1.0.4/simpleplayer.egg-info/PKG-INFO
+-rw-r--r--   0 thowie     (501) staff       (20)      323 2023-06-19 07:07:06.000000 simpleplayer-1.0.4/simpleplayer.egg-info/SOURCES.txt
+-rw-r--r--   0 thowie     (501) staff       (20)        1 2023-06-19 07:07:06.000000 simpleplayer-1.0.4/simpleplayer.egg-info/dependency_links.txt
+-rw-r--r--   0 thowie     (501) staff       (20)      102 2023-06-19 07:07:06.000000 simpleplayer-1.0.4/simpleplayer.egg-info/entry_points.txt
+-rw-r--r--   0 thowie     (501) staff       (20)       33 2023-06-19 07:07:06.000000 simpleplayer-1.0.4/simpleplayer.egg-info/requires.txt
+-rw-r--r--   0 thowie     (501) staff       (20)       13 2023-06-19 07:07:06.000000 simpleplayer-1.0.4/simpleplayer.egg-info/top_level.txt
```

### Comparing `simpleplayer-1.0.3/PKG-INFO` & `simpleplayer-1.0.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,10 @@
-Metadata-Version: 2.1
-Name: simpleplayer
-Version: 1.0.3
-Summary: Discover the pinnacle of audio elegance with this simple-player module, boasting a sophisticated blend of advanced features and seamless compatibility across multiple platforms.
-Author: TOWDIO
-Author-email: thowiestudio@gmail.com
-Description-Content-Type: text/markdown
-
 # Simple Player
 
-The `AudioPlayer` module allows you to play audio files using the `soundfile` and `sounddevice` libraries.
+Discover the pinnacle of audio elegance with this `simpleplayer` module, boasting a sophisticated blend of advanced features and seamless compatibility across multiple platforms.
 
 <br>
 
 ## Installation
 
 You can install the module using pip:
 
@@ -110,76 +102,62 @@
 
 ```
 
 Remember to replace 'path/to/your/audio/file.wav' with the actual path to your audio file.
 
 <br>
 
-## Simple Player Example
+## [Simple Player Example](https://raw.githubusercontent.com/tantowijh/simple-player-python/main/example.py)
+
+<br>
+<br>
+
+
+# Voice Generator
+
+The `voicegen` module allows you to convert text to speech and save it as an audio file using the `gtts` library.
+
+To use the `voicegen` module, you need to follow these steps:
+
+1. Import the `voicegen` class from the `voicegen` module:
+
+    ```python
+    from simpleplayer import voicegen
+    ```
+2. Create an instance of the voicegen class, providing the text, filename, and an optional language parameter:
+
+    ```python
+    voicegen(text, filename, lang='en')
+    ```
+    Replace text with the text you want to convert to speech, filename with the desired name of the output audio file, and lang with the language code (default is 'en').
+
+3. If the internet connection is available, the text will be converted into speech and saved as an MP3 file with the specified filename.
+
+<br>
+
+Example usage:
 
 ```python
-import time
-from test import AudioPlayer
+from simpleplayer import voicegen
+
+# Generate the voice
+voicegen("Hello, world!", "output")
+```
+This will generate an audio file named output.mp3 containing the speech for the text "Hello, world!".
 
-class AudioMenu:
-    def __init__(self):
-        self.player = None
-
-    def display_menu(self):
-        print("1. Load audio file")
-        print("2. Play audio")
-        print("3. Pause audio")
-        print("4. Resume audio")
-        print("5. Stop audio")
-        print("6. Exit")
-
-    def run(self):
-        while True:
-            self.display_menu()
-            choice = input("Enter your choice: ")
-
-            if choice == "1":
-                filename = input("Enter the audio file path: ")
-                self.player = AudioPlayer(filename)
-                print("Audio file loaded.")
-
-            elif choice == "2":
-                if self.player is not None:
-                    self.player.play()
-                    print("Audio playback started.")
-                else:
-                    print("No audio file loaded.")
-
-            elif choice == "3":
-                if self.player is not None:
-                    self.player.pause()
-                    print("Audio playback paused.")
-                else:
-                    print("No audio file loaded.")
-
-            elif choice == "4":
-                if self.player is not None:
-                    self.player.resume()
-                    print("Audio playback resumed.")
-                else:
-                    print("No audio file loaded.")
-
-            elif choice == "5":
-                if self.player is not None:
-                    self.player.stop()
-                    print("Audio playback stopped.")
-                    self.player = None
-                else:
-                    print("No audio file loaded.")
-
-            elif choice == "6":
-                break
-
-            else:
-                print("Invalid choice. Please try again.")
-
-            time.sleep(1)  # Add a small delay to allow time for audio operations to take effect
-
-# Create an instance of AudioMenu and run the menu
-menu = AudioMenu()
-menu.run()
+<br>
+
+## Terminal Usage
+You can also use the voicegen module directly from the terminal:
+```
+voicegen "Hello, world!" output
 ```
+
+Replace "Hello, world!" with the desired text and output with the desired filename (without the file extension). The generated audio file will be saved as output.mp3 in the current directory.
+
+Note: Ensure that you have a stable internet connection to use the voicegen module successfully.
+
+<br>
+<br>
+
+# LICENSE
+This project is licensed under the [MIT License](LICENSE) - see the LICENSE file for details.
```

### Comparing `simpleplayer-1.0.3/setup.py` & `simpleplayer-1.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 
 # Read the contents of README.md file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='simpleplayer',
-    version='1.0.3',
+    version='1.0.4',
     description='Discover the pinnacle of audio elegance with this simple-player module, boasting a sophisticated blend of advanced features and seamless compatibility across multiple platforms.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='TOWDIO',
     author_email='thowiestudio@gmail.com',
     packages=['simpleplayer'],
     install_requires=[
         'soundfile',
         'sounddevice',
         'numpy',
+        'gtts',
     ],
     entry_points={
         'console_scripts': [
             'simpleplayer = simpleplayer.simpleplayer:main',
+            'voicegen = simpleplayer.voicegen:main',
         ],
     }
-
-)
+)
```

### Comparing `simpleplayer-1.0.3/simpleplayer/simpleplayer.py` & `simpleplayer-1.0.4/simpleplayer/simpleplayer.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,22 +64,31 @@
             self.paused = False
 
     def wait(self) -> None:
         seconds = int(self.duration)
         time.sleep(seconds)
 
 def main():
-    # Ensure a filename is provided as a command-line argument
-    if len(sys.argv) < 2:
-        print("Please provide the filename of the audio file.")
-        return
+    try:
+        # Ensure a filename is provided as a command-line argument
+        if len(sys.argv) < 2 or sys.argv[1] == "--help":
+            print("\n"*3)
+            print("Simple Player\n")
+            print("Usage  : simpleplayer <filename>\n")
+            print("Example: simpleplayer 'path/to/file audio.wav'\n")
+            print("         simpleplayer --help   (to show this help message)")
+            print("\n"*3)
+            sys.exit(0)
 
-    # Extract the filename from command-line arguments
-    filename = sys.argv[1]
+        # Extract the filename from command-line arguments
+        filename = sys.argv[1]
 
-    # Create an instance of AudioPlayer and play the audio
-    player = AudioPlayer(filename)
-    player.play()
-    player.wait()
+        # Create an instance of AudioPlayer and play the audio
+        player = AudioPlayer(filename)
+        player.play()
+        player.wait()
+    except KeyboardInterrupt:
+        print("\nInterrupted by user")
+        sys.exit(0)
 
 if __name__ == '__main__':
     main()
```

