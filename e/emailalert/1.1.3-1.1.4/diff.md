# Comparing `tmp/emailalert-1.1.3.tar.gz` & `tmp/emailalert-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.1.3.tar", last modified: Mon Jun 19 09:23:15 2023, max compression
+gzip compressed data, was "emailalert-1.1.4.tar", last modified: Mon Jun 19 09:28:34 2023, max compression
```

## Comparing `emailalert-1.1.3.tar` & `emailalert-1.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 09:23:15.049704 emailalert-1.1.3/
--rw-rw-rw-   0        0        0      178 2023-06-19 09:23:15.046593 emailalert-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 09:23:15.009639 emailalert-1.1.3/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-19 09:23:14.000000 emailalert-1.1.3/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-19 09:23:14.000000 emailalert-1.1.3/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 09:23:14.000000 emailalert-1.1.3/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-19 09:23:14.000000 emailalert-1.1.3/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 09:23:15.040589 emailalert-1.1.3/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.1.3/sck/__init__.py
--rw-rw-rw-   0        0        0     2814 2023-06-19 09:22:59.000000 emailalert-1.1.3/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-19 09:23:15.050593 emailalert-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-19 09:23:06.000000 emailalert-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:28:34.082083 emailalert-1.1.4/
+-rw-rw-rw-   0        0        0      178 2023-06-19 09:28:34.080048 emailalert-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 09:28:34.062050 emailalert-1.1.4/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-19 09:28:33.000000 emailalert-1.1.4/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-19 09:28:33.000000 emailalert-1.1.4/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 09:28:33.000000 emailalert-1.1.4/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-19 09:28:33.000000 emailalert-1.1.4/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 09:28:34.074051 emailalert-1.1.4/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.1.4/sck/__init__.py
+-rw-rw-rw-   0        0        0     2467 2023-06-19 09:27:21.000000 emailalert-1.1.4/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 09:28:34.082083 emailalert-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-19 09:28:30.000000 emailalert-1.1.4/setup.py
```

### Comparing `emailalert-1.1.3/README.md` & `emailalert-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.1.3/sck/emailalert.py` & `emailalert-1.1.4/sck/emailalert.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,31 +24,21 @@
     #msg = MIMEText(message)
     msg = MIMEMultipart()
     msg['Subject'] = subject
     msg['From'] = sender
     #msg['To'] = recipient
     msg['To'] = ', '.join(recipients)
 
+    # Get all file paths in the folders
+    attachment_paths = get_files_in_folders(folder_paths)
+
     # Add the email body with the list of attached files
     message += "\n".join(attachment_paths)
     msg.attach(MIMEText(message, 'plain'))
 
-    # Attach the file
-    # with open(attachment, 'rb') as attachement:
-    #     part = MIMEBase('application', 'octet-stream')
-    #     part.set_payload(attachement.read())
-    #     encoders.endoe_base64(part)
-    #     part.add_header('Content-Disposition', f'attachement; filename={attachement}')
-
-    #     msg.attach(part)
-
-    
-    # Get all file paths in the folders
-    attachment_paths = get_files_in_folders(folder_paths)
-
     # Find files with the specified extension in the folder
     # attachment_paths = []
     # sendEmail = 0
     # for file_name in os.listdir(folder_path):
     #     if file_name.endswith(file_extension):
     #         attachment_paths.append(os.path.join(folder_path, file_name))
     #         sendEmail = 1
```

