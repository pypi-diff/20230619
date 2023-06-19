# Comparing `tmp/emailalert-1.1.4.tar.gz` & `tmp/emailalert-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.1.4.tar", last modified: Mon Jun 19 09:28:34 2023, max compression
+gzip compressed data, was "emailalert-1.1.5.tar", last modified: Mon Jun 19 10:00:09 2023, max compression
```

## Comparing `emailalert-1.1.4.tar` & `emailalert-1.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 09:28:34.082083 emailalert-1.1.4/
--rw-rw-rw-   0        0        0      178 2023-06-19 09:28:34.080048 emailalert-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 09:28:34.062050 emailalert-1.1.4/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-19 09:28:33.000000 emailalert-1.1.4/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-19 09:28:33.000000 emailalert-1.1.4/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 09:28:33.000000 emailalert-1.1.4/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-19 09:28:33.000000 emailalert-1.1.4/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 09:28:34.074051 emailalert-1.1.4/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.1.4/sck/__init__.py
--rw-rw-rw-   0        0        0     2467 2023-06-19 09:27:21.000000 emailalert-1.1.4/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-19 09:28:34.082083 emailalert-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-19 09:28:30.000000 emailalert-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 10:00:09.754229 emailalert-1.1.5/
+-rw-rw-rw-   0        0        0      178 2023-06-19 10:00:09.752001 emailalert-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 10:00:09.704994 emailalert-1.1.5/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-19 10:00:09.000000 emailalert-1.1.5/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-19 10:00:09.000000 emailalert-1.1.5/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 10:00:09.000000 emailalert-1.1.5/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-19 10:00:09.000000 emailalert-1.1.5/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 10:00:09.743995 emailalert-1.1.5/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.1.5/sck/__init__.py
+-rw-rw-rw-   0        0        0     3043 2023-06-19 10:00:04.000000 emailalert-1.1.5/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 10:00:09.756993 emailalert-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-19 10:00:01.000000 emailalert-1.1.5/setup.py
```

### Comparing `emailalert-1.1.4/README.md` & `emailalert-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.1.4/sck/emailalert.py` & `emailalert-1.1.5/sck/emailalert.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 import os
 import smtplib
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
 from email.mime.base import MIMEBase
 from email import encoders
+import shutil
 
 def get_files_in_folders(folder_paths):
     file_paths = []
     for folder_path in folder_paths:
         for root, dirs, files in os.walk(folder_path):
             for file in files:
                 file_paths.append(os.path.join(root, file))
     return file_paths
 
+def get_filenames_in_folders(folder_paths):
+    file_names = []
+    for folder_path in folder_paths:
+        for root, dirs, files in os.walk(folder_path):
+            for file_name in files:
+                file_names.append(file_name)
+    return file_names
+
 
 def send(recipients,subject,message, folder_paths):
     # Email details
     smtp_server = 'mrelay.noc.sony.co.jp'
     smtp_port = 25
     sender = 'SCK-H5BAREVOS-NGK-SYSADMIN@sony.com'
 
@@ -27,16 +36,19 @@
     msg['From'] = sender
     #msg['To'] = recipient
     msg['To'] = ', '.join(recipients)
 
     # Get all file paths in the folders
     attachment_paths = get_files_in_folders(folder_paths)
 
+    # Get all file names in the folders
+    attachment_file_names = get_filenames_in_folders(folder_paths)
+
     # Add the email body with the list of attached files
-    message += "\n".join(attachment_paths)
+    message += "\n\r".join(attachment_file_names)
     msg.attach(MIMEText(message, 'plain'))
 
     # Find files with the specified extension in the folder
     # attachment_paths = []
     # sendEmail = 0
     # for file_name in os.listdir(folder_path):
     #     if file_name.endswith(file_extension):
@@ -53,22 +65,23 @@
         encoders.encode_base64(attachment)
         attachment.add_header(
             "Content-Disposition",
             f"attachment; filename= {os.path.basename(file_path)}",
         )
         msg.attach(attachment)
         os.remove(file_path)
+        # use the shutil.move() function to move the file
+        if os.path.exists('./backup/'+os.path.basename(file_path)):
+            os.replace('./backup/'+os.path.basename(file_path), os.path.basename(file_path))
+        shutil.move(os.path.basename(file_path), './backup/')
 
     # Connect to the SMTP server
     with smtplib.SMTP(smtp_server, smtp_port) as server:
         try:    
             server.sendmail(sender, recipients, msg.as_string())
-
-            # remove the attached files from the target folder
-            os.remove("★"+csv_file_name)
             return 1
         except Exception as e:
             print('An error occurred:', str(e))
             return 0
         finally:
             # Disconnect from the SMTP server
             server.quit()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

