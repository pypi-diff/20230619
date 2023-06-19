# Comparing `tmp/emailalert-1.1.0.tar.gz` & `tmp/emailalert-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.1.0.tar", last modified: Mon Jun 19 01:58:41 2023, max compression
+gzip compressed data, was "emailalert-1.1.1.tar", last modified: Mon Jun 19 08:56:03 2023, max compression
```

## Comparing `emailalert-1.1.0.tar` & `emailalert-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 01:58:41.684465 emailalert-1.1.0/
--rw-rw-rw-   0        0        0      178 2023-06-19 01:58:41.682466 emailalert-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-06-15 05:04:18.000000 emailalert-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 01:58:41.644687 emailalert-1.1.0/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-19 01:58:41.000000 emailalert-1.1.0/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-19 01:58:41.000000 emailalert-1.1.0/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 01:58:41.000000 emailalert-1.1.0/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-19 01:58:41.000000 emailalert-1.1.0/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 01:58:41.675462 emailalert-1.1.0/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.1.0/sck/__init__.py
--rw-rw-rw-   0        0        0     2056 2023-06-19 01:56:58.000000 emailalert-1.1.0/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-19 01:58:41.685462 emailalert-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-19 01:57:35.000000 emailalert-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 08:56:03.502478 emailalert-1.1.1/
+-rw-rw-rw-   0        0        0      178 2023-06-19 08:56:03.499302 emailalert-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 08:56:03.462303 emailalert-1.1.1/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-19 08:56:03.000000 emailalert-1.1.1/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-19 08:56:03.000000 emailalert-1.1.1/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 08:56:03.000000 emailalert-1.1.1/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-19 08:56:03.000000 emailalert-1.1.1/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 08:56:03.494300 emailalert-1.1.1/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.1.1/sck/__init__.py
+-rw-rw-rw-   0        0        0     2574 2023-06-19 08:55:51.000000 emailalert-1.1.1/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 08:56:03.503555 emailalert-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-19 08:55:59.000000 emailalert-1.1.1/setup.py
```

### Comparing `emailalert-1.1.0/sck/emailalert.py` & `emailalert-1.1.1/sck/emailalert.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 import os
 import smtplib
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
 from email.mime.base import MIMEBase
 from email import encoders
 
-def send(recipients,subject,message, folder_path, file_extension):
+def get_files_in_folders(folder_paths):
+    file_paths = []
+    for folder_path in folder_paths:
+        for root, dirs, files in os.walk(folder_path):
+            for file in files:
+                file_paths.append(os.path.join(root, file))
+    return file_paths
+
+
+def send(recipients,subject,message, folder_paths):
     # Email details
     smtp_server = 'mrelay.noc.sony.co.jp'
     smtp_port = 25
     sender = 'SCK-H5BAREVOS-NGK-SYSADMIN@sony.com'
 
     # Create a MIME text object
     #msg = MIMEText(message)
@@ -26,29 +35,39 @@
     #     part = MIMEBase('application', 'octet-stream')
     #     part.set_payload(attachement.read())
     #     encoders.endoe_base64(part)
     #     part.add_header('Content-Disposition', f'attachement; filename={attachement}')
 
     #     msg.attach(part)
 
-    # Find files with the specified extension in the folder
-    attachment_paths = []
-    for file_name in os.listdir(folder_path):
-        if file_name.endswith(file_extension):
-            attachment_paths.append(os.path.join(folder_path, file_name))
-
-    # Attach multiple files
-    for attachment_path in attachment_paths:
-        with open(attachment_path, 'rb') as attachment:
-            part = MIMEBase('application', 'octet-stream')
-            part.set_payload(attachment.read())
-            encoders.encode_base64(part)
-            part.add_header('Content-Disposition', f'attachment; filename={attachment_path}')
+    
+    # Get all file paths in the folders
+    attachment_paths = get_files_in_folders(folder_paths)
 
-            msg.attach(part)
+    # Find files with the specified extension in the folder
+    # attachment_paths = []
+    # sendEmail = 0
+    # for file_name in os.listdir(folder_path):
+    #     if file_name.endswith(file_extension):
+    #         attachment_paths.append(os.path.join(folder_path, file_name))
+    #         sendEmail = 1
+    # if sendEmail==0:
+    #     return 0
+
+    # Attach the files to the email
+    for file_path in attachment_paths:
+        attachment = MIMEBase("application", "octet-stream")
+        with open(file_path, "rb") as file:
+            attachment.set_payload(file.read())
+        encoders.encode_base64(attachment)
+        attachment.add_header(
+            "Content-Disposition",
+            f"attachment; filename= {os.path.basename(file_path)}",
+        )
+        msg.attach(attachment)
 
     # Connect to the SMTP server
     with smtplib.SMTP(smtp_server, smtp_port) as server:
         try:    
             server.sendmail(sender, recipients, msg.as_string())
 
             return 1
```

