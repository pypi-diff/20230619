# Comparing `tmp/emailalert-1.1.2.tar.gz` & `tmp/emailalert-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailalert-1.1.2.tar", last modified: Mon Jun 19 09:07:53 2023, max compression
+gzip compressed data, was "emailalert-1.1.3.tar", last modified: Mon Jun 19 09:23:15 2023, max compression
```

## Comparing `emailalert-1.1.2.tar` & `emailalert-1.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 09:07:53.143760 emailalert-1.1.2/
--rw-rw-rw-   0        0        0      178 2023-06-19 09:07:53.139676 emailalert-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 09:07:53.072120 emailalert-1.1.2/emailalert.egg-info/
--rw-rw-rw-   0        0        0      178 2023-06-19 09:07:52.000000 emailalert-1.1.2/emailalert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-19 09:07:52.000000 emailalert-1.1.2/emailalert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 09:07:52.000000 emailalert-1.1.2/emailalert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-19 09:07:52.000000 emailalert-1.1.2/emailalert.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-19 09:07:53.129879 emailalert-1.1.2/sck/
--rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.1.2/sck/__init__.py
--rw-rw-rw-   0        0        0     2712 2023-06-19 09:07:30.000000 emailalert-1.1.2/sck/emailalert.py
--rw-rw-rw-   0        0        0       42 2023-06-19 09:07:53.145658 emailalert-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      253 2023-06-19 09:07:47.000000 emailalert-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 09:23:15.049704 emailalert-1.1.3/
+-rw-rw-rw-   0        0        0      178 2023-06-19 09:23:15.046593 emailalert-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-19 02:19:42.000000 emailalert-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-19 09:23:15.009639 emailalert-1.1.3/emailalert.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-06-19 09:23:14.000000 emailalert-1.1.3/emailalert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-19 09:23:14.000000 emailalert-1.1.3/emailalert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 09:23:14.000000 emailalert-1.1.3/emailalert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-19 09:23:14.000000 emailalert-1.1.3/emailalert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 09:23:15.040589 emailalert-1.1.3/sck/
+-rw-rw-rw-   0        0        0        0 2023-06-15 05:04:18.000000 emailalert-1.1.3/sck/__init__.py
+-rw-rw-rw-   0        0        0     2814 2023-06-19 09:22:59.000000 emailalert-1.1.3/sck/emailalert.py
+-rw-rw-rw-   0        0        0       42 2023-06-19 09:23:15.050593 emailalert-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      253 2023-06-19 09:23:06.000000 emailalert-1.1.3/setup.py
```

### Comparing `emailalert-1.1.2/README.md` & `emailalert-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `emailalert-1.1.2/sck/emailalert.py` & `emailalert-1.1.3/sck/emailalert.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     #msg = MIMEText(message)
     msg = MIMEMultipart()
     msg['Subject'] = subject
     msg['From'] = sender
     #msg['To'] = recipient
     msg['To'] = ', '.join(recipients)
 
+    # Add the email body with the list of attached files
+    message += "\n".join(attachment_paths)
     msg.attach(MIMEText(message, 'plain'))
 
     # Attach the file
     # with open(attachment, 'rb') as attachement:
     #     part = MIMEBase('application', 'octet-stream')
     #     part.set_payload(attachement.read())
     #     encoders.endoe_base64(part)
```

