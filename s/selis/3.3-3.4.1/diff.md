# Comparing `tmp/selis-3.3.tar.gz` & `tmp/selis-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selis-3.3.tar", last modified: Mon Jun 19 05:08:36 2023, max compression
+gzip compressed data, was "selis-3.4.1.tar", last modified: Mon Jun 19 14:44:42 2023, max compression
```

## Comparing `selis-3.3.tar` & `selis-3.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-19 05:08:36.984958 selis-3.3/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-19 05:08:36.984845 selis-3.3/PKG-INFO
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-19 05:08:36.983659 selis-3.3/selis/
--rw-r--r--   0 client     (501) staff       (20)        0 2023-06-17 14:59:11.000000 selis-3.3/selis/__init__.py
--rw-r--r--   0 client     (501) staff       (20)     3862 2023-06-19 05:07:34.000000 selis-3.3/selis/client.py
--rw-r--r--   0 client     (501) staff       (20)      786 2023-06-19 05:07:04.000000 selis-3.3/selis/computerinfo.py
--rw-r--r--   0 client     (501) staff       (20)     1149 2023-06-19 05:07:57.000000 selis-3.3/selis/selis.py
--rw-r--r--   0 client     (501) staff       (20)      289 2023-06-19 05:01:26.000000 selis-3.3/selis/utils.py
-drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-19 05:08:36.984633 selis-3.3/selis.egg-info/
--rw-r--r--   0 client     (501) staff       (20)      128 2023-06-19 05:08:36.000000 selis-3.3/selis.egg-info/PKG-INFO
--rw-r--r--   0 client     (501) staff       (20)      270 2023-06-19 05:08:36.000000 selis-3.3/selis.egg-info/SOURCES.txt
--rw-r--r--   0 client     (501) staff       (20)        1 2023-06-19 05:08:36.000000 selis-3.3/selis.egg-info/dependency_links.txt
--rw-r--r--   0 client     (501) staff       (20)       44 2023-06-19 05:08:36.000000 selis-3.3/selis.egg-info/entry_points.txt
--rw-r--r--   0 client     (501) staff       (20)       24 2023-06-19 05:08:36.000000 selis-3.3/selis.egg-info/requires.txt
--rw-r--r--   0 client     (501) staff       (20)        6 2023-06-19 05:08:36.000000 selis-3.3/selis.egg-info/top_level.txt
--rw-r--r--   0 client     (501) staff       (20)       38 2023-06-19 05:08:36.985000 selis-3.3/setup.cfg
--rw-r--r--   0 client     (501) staff       (20)      279 2023-06-19 05:08:14.000000 selis-3.3/setup.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-19 14:44:42.118849 selis-3.4.1/
+-rw-r--r--   0 client     (501) staff       (20)      130 2023-06-19 14:44:42.118737 selis-3.4.1/PKG-INFO
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-19 14:44:42.117672 selis-3.4.1/selis/
+-rw-r--r--   0 client     (501) staff       (20)        0 2023-06-17 14:59:11.000000 selis-3.4.1/selis/__init__.py
+-rw-r--r--   0 client     (501) staff       (20)     3903 2023-06-19 14:43:38.000000 selis-3.4.1/selis/client.py
+-rw-r--r--   0 client     (501) staff       (20)      786 2023-06-19 14:43:51.000000 selis-3.4.1/selis/computerinfo.py
+-rw-r--r--   0 client     (501) staff       (20)     1134 2023-06-19 14:40:34.000000 selis-3.4.1/selis/selis.py
+-rw-r--r--   0 client     (501) staff       (20)      410 2023-06-19 14:43:43.000000 selis-3.4.1/selis/utils.py
+drwxr-xr-x   0 client     (501) staff       (20)        0 2023-06-19 14:44:42.118569 selis-3.4.1/selis.egg-info/
+-rw-r--r--   0 client     (501) staff       (20)      130 2023-06-19 14:44:42.000000 selis-3.4.1/selis.egg-info/PKG-INFO
+-rw-r--r--   0 client     (501) staff       (20)      270 2023-06-19 14:44:42.000000 selis-3.4.1/selis.egg-info/SOURCES.txt
+-rw-r--r--   0 client     (501) staff       (20)        1 2023-06-19 14:44:42.000000 selis-3.4.1/selis.egg-info/dependency_links.txt
+-rw-r--r--   0 client     (501) staff       (20)       44 2023-06-19 14:44:42.000000 selis-3.4.1/selis.egg-info/entry_points.txt
+-rw-r--r--   0 client     (501) staff       (20)       24 2023-06-19 14:44:42.000000 selis-3.4.1/selis.egg-info/requires.txt
+-rw-r--r--   0 client     (501) staff       (20)        6 2023-06-19 14:44:42.000000 selis-3.4.1/selis.egg-info/top_level.txt
+-rw-r--r--   0 client     (501) staff       (20)       38 2023-06-19 14:44:42.118889 selis-3.4.1/setup.cfg
+-rw-r--r--   0 client     (501) staff       (20)      281 2023-06-19 14:44:31.000000 selis-3.4.1/setup.py
```

### Comparing `selis-3.3/selis/client.py` & `selis-3.4.1/selis/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import socket
 import threading
 import sys
-import webbrowser
 import getpass
 
 from selis.computerinfo import ComputerInfo
-from selis.utils import convert_color, guide_to_exit
+from selis.utils import convert_color, guide_to_exit, clear_screen, open_url
 
 
 class ChatClient:
     def __init__(self, ip, port, nickname):
         self.connection = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         try:
             self.connection.connect((ip, port))
@@ -29,31 +28,27 @@
         self.send_message(msg)
 
 
     def send_message(self, message):
         self.connection.send(message.encode())
 
 
-    def open_url(self, url):
-        webbrowser.open(url)
-
-
     def process_receiving_message(self):
         while True:
             try:
                 response = self.connection.recv(1024).decode()
 
                 if not response and self.connection:
                     print(convert_color("[-] Sever is not opening", style="FAIL"))
                     guide_to_exit()
                     break
 
                 elif "admin/open-url" in response:
                     url = response.split(" ")[1]
-                    self.open_url(url)
+                    open_url(url)
 
                 elif response == "admin/close-server":
                     print(convert_color("[-] Admin closes the server", style="FAIL"))
                     guide_to_exit()
                     self.connection.close()
                     sys.exit(0)
 
@@ -64,28 +59,31 @@
                 print(convert_color("[-] Connection is closed", style="FAIL"))
                 self.connection.close()
                 break
 
 
     def process_admin_mode(self):
         password = getpass.getpass(convert_color("[*] Admin's Password: \n>> ", style="ENDC"))
-        msg = "check-admin/" + password
+        msg = "check-admin/" + self.nickname + "/" + password
         self.send_message(msg)
 
 
     def process_sending_message(self):
         try:
             while True:
                 content = input()
 
                 if content == "/exit":
                     self.send_message(f"client/exit {self.nickname}")
                     self.connection.close()
                     break
 
+                elif content == "/clear":
+                    clear_screen()
+
                 elif content == "/ls":
                     self.send_message(content)
 
                 elif content == "/admin-mode":
                     self.process_admin_mode()
 
                 elif content == "/close-server":
```

### Comparing `selis-3.3/selis/computerinfo.py` & `selis-3.4.1/selis/computerinfo.py`

 * *Files identical despite different names*

### Comparing `selis-3.3/selis/selis.py` & `selis-3.4.1/selis/selis.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import sys
 
 from optparse import OptionParser
-from selis.client import ChatClient
+from selis.selis import ChatClient
 
 
 def return_arguments():
     parser = OptionParser()
-    parser.add_option("-v", "--version", dest="version", action="store_true", help="Show version then exit")
-    parser.add_option("-p", "--port", dest="port", help="Connect to sever through this port")
-    parser.add_option("-n", "--nickname", dest="nickname", help="Choose your name or a nickname")
+    parser.add_option("-v", "--version", dest="version", action="store_true", help="show version and exit")
+    parser.add_option("-p", "--port", dest="port", help="connect to sever through this port")
+    parser.add_option("-n", "--nickname", dest="nickname", help="choose a nickname")
     (options, arguments) = parser.parse_args()
 
     if options.version:
         print("selis 2.7")
         sys.exit()
         
     return_error(parser, options)
```

