# Comparing `tmp/emailalert-1.1.8.tar.gz` & `tmp/emailalert-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.1.8.tar", last modified: Mon Jun 19 10:16:43 2023, max compression
+gzip compressed data, was "emailalert-1.1.9.tar", last modified: Mon Jun 19 10:20:41 2023, max compression
```

## Comparing `emailalert-1.1.8.tar` & `emailalert-1.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 10:16:43.839416 emailalert-1.1.8/
--rw-rw-rw-   0        0        0      178 2023-06-19 10:16:43.836308 emailalert-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 10:16:43.803310 emailalert-1.1.8/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-19 10:16:43.000000 emailalert-1.1.8/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-19 10:16:43.000000 emailalert-1.1.8/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 10:16:43.000000 emailalert-1.1.8/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-19 10:16:43.000000 emailalert-1.1.8/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 10:16:43.828313 emailalert-1.1.8/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.1.8/sck/__init__.py
--rw-rw-rw-   0        0        0     2953 2023-06-19 10:16:29.000000 emailalert-1.1.8/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-19 10:16:43.840336 emailalert-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-19 10:16:39.000000 emailalert-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 10:20:41.340898 emailalert-1.1.9/
+-rw-rw-rw-   0        0        0      178 2023-06-19 10:20:41.338926 emailalert-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 10:20:41.296909 emailalert-1.1.9/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-19 10:20:41.000000 emailalert-1.1.9/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-19 10:20:41.000000 emailalert-1.1.9/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 10:20:41.000000 emailalert-1.1.9/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-19 10:20:41.000000 emailalert-1.1.9/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 10:20:41.331899 emailalert-1.1.9/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.1.9/sck/__init__.py
+-rw-rw-rw-   0        0        0     3093 2023-06-19 10:20:25.000000 emailalert-1.1.9/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 10:20:41.342306 emailalert-1.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-19 10:20:32.000000 emailalert-1.1.9/setup.py
```

### Comparing `emailalert-1.1.8/README.md` & `emailalert-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.1.8/sck/emailalert.py` & `emailalert-1.1.9/sck/emailalert.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,16 +65,17 @@
         encoders.encode_base64(attachment)
         attachment.add_header(
             "Content-Disposition",
             f"attachment; filename= {os.path.basename(file_path)}",
         )
         msg.attach(attachment)
         # Move the attached file to the backup folder
-        backup_folder = "backup/"
-        backup_file_path = os.path.join(backup_folder, os.path.basename(file_path))
+        backup_folder = "backup/"  # Relative path to the backup folder
+        current_dir = os.getcwd()  # Get the current working directory
+        backup_file_path = os.path.abspath(os.path.join(current_dir, backup_folder, os.path.basename(file_path)))
         shutil.move(file_path, backup_file_path)
 
     # Connect to the SMTP server
     with smtplib.SMTP(smtp_server, smtp_port) as server:
         try:    
             server.sendmail(sender, recipients, msg.as_string())
             return 1
```

