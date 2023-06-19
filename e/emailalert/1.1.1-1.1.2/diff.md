# Comparing `tmp/emailalert-1.1.1.tar.gz` & `tmp/emailalert-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.1.1.tar", last modified: Mon Jun 19 08:56:03 2023, max compression
+gzip compressed data, was "emailalert-1.1.2.tar", last modified: Mon Jun 19 09:07:53 2023, max compression
```

## Comparing `emailalert-1.1.1.tar` & `emailalert-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 08:56:03.502478 emailalert-1.1.1/
--rw-rw-rw-   0        0        0      178 2023-06-19 08:56:03.499302 emailalert-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 08:56:03.462303 emailalert-1.1.1/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-19 08:56:03.000000 emailalert-1.1.1/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-19 08:56:03.000000 emailalert-1.1.1/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 08:56:03.000000 emailalert-1.1.1/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-19 08:56:03.000000 emailalert-1.1.1/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 08:56:03.494300 emailalert-1.1.1/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.1.1/sck/__init__.py
--rw-rw-rw-   0        0        0     2574 2023-06-19 08:55:51.000000 emailalert-1.1.1/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-19 08:56:03.503555 emailalert-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-19 08:55:59.000000 emailalert-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:07:53.143760 emailalert-1.1.2/
+-rw-rw-rw-   0        0        0      178 2023-06-19 09:07:53.139676 emailalert-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 09:07:53.072120 emailalert-1.1.2/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-19 09:07:52.000000 emailalert-1.1.2/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-19 09:07:52.000000 emailalert-1.1.2/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 09:07:52.000000 emailalert-1.1.2/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-19 09:07:52.000000 emailalert-1.1.2/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 09:07:53.129879 emailalert-1.1.2/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.1.2/sck/__init__.py
+-rw-rw-rw-   0        0        0     2712 2023-06-19 09:07:30.000000 emailalert-1.1.2/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 09:07:53.145658 emailalert-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-19 09:07:47.000000 emailalert-1.1.2/setup.py
```

### Comparing `emailalert-1.1.1/README.md` & `emailalert-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.1.1/sck/emailalert.py` & `emailalert-1.1.2/sck/emailalert.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,20 +60,23 @@
             attachment.set_payload(file.read())
         encoders.encode_base64(attachment)
         attachment.add_header(
             "Content-Disposition",
             f"attachment; filename= {os.path.basename(file_path)}",
         )
         msg.attach(attachment)
+        os.remove(file_path)
 
     # Connect to the SMTP server
     with smtplib.SMTP(smtp_server, smtp_port) as server:
         try:    
             server.sendmail(sender, recipients, msg.as_string())
 
+            # remove the attached files from the target folder
+            os.remove("★"+csv_file_name)
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
-us-ascii
+utf-8
```

