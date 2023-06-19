# Comparing `tmp/emailalert-1.1.5.tar.gz` & `tmp/emailalert-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.1.5.tar", last modified: Mon Jun 19 10:00:09 2023, max compression
+gzip compressed data, was "emailalert-1.1.6.tar", last modified: Mon Jun 19 10:06:37 2023, max compression
```

## Comparing `emailalert-1.1.5.tar` & `emailalert-1.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 10:00:09.754229 emailalert-1.1.5/
--rw-rw-rw-   0        0        0      178 2023-06-19 10:00:09.752001 emailalert-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 10:00:09.704994 emailalert-1.1.5/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-19 10:00:09.000000 emailalert-1.1.5/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-19 10:00:09.000000 emailalert-1.1.5/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 10:00:09.000000 emailalert-1.1.5/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-19 10:00:09.000000 emailalert-1.1.5/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 10:00:09.743995 emailalert-1.1.5/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.1.5/sck/__init__.py
--rw-rw-rw-   0        0        0     3043 2023-06-19 10:00:04.000000 emailalert-1.1.5/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-19 10:00:09.756993 emailalert-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-19 10:00:01.000000 emailalert-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 10:06:37.431918 emailalert-1.1.6/
+-rw-rw-rw-   0        0        0      178 2023-06-19 10:06:37.427904 emailalert-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 10:06:37.386825 emailalert-1.1.6/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-19 10:06:37.000000 emailalert-1.1.6/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-19 10:06:37.000000 emailalert-1.1.6/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 10:06:37.000000 emailalert-1.1.6/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-19 10:06:37.000000 emailalert-1.1.6/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 10:06:37.419974 emailalert-1.1.6/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.1.6/sck/__init__.py
+-rw-rw-rw-   0        0        0     3013 2023-06-19 10:02:16.000000 emailalert-1.1.6/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 10:06:37.431918 emailalert-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-19 10:06:24.000000 emailalert-1.1.6/setup.py
```

### Comparing `emailalert-1.1.5/README.md` & `emailalert-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.1.5/sck/emailalert.py` & `emailalert-1.1.6/sck/emailalert.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,14 @@
             attachment.set_payload(file.read())
         encoders.encode_base64(attachment)
         attachment.add_header(
             "Content-Disposition",
             f"attachment; filename= {os.path.basename(file_path)}",
         )
         msg.attach(attachment)
-        os.remove(file_path)
         # use the shutil.move() function to move the file
         if os.path.exists('./backup/'+os.path.basename(file_path)):
             os.replace('./backup/'+os.path.basename(file_path), os.path.basename(file_path))
         shutil.move(os.path.basename(file_path), './backup/')
 
     # Connect to the SMTP server
     with smtplib.SMTP(smtp_server, smtp_port) as server:
```

