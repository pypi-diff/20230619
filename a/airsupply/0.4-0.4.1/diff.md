# Comparing `tmp/airsupply-0.4.tar.gz` & `tmp/airsupply-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airsupply-0.4.tar", max compression
+gzip compressed data, was "airsupply-0.4.1.tar", max compression
```

## Comparing `airsupply-0.4.tar` & `airsupply-0.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2020-01-24 03:52:19.000000 airsupply-0.4/airsupply/__init__.py
--rw-r--r--   0        0        0       30 2020-01-24 03:52:44.000000 airsupply-0.4/airsupply/__main__.py
--rw-r--r--   0        0        0      369 2020-01-29 08:19:41.000000 airsupply-0.4/airsupply/apk.py
--rw-r--r--   0        0        0     2042 2023-06-18 18:04:25.108912 airsupply-0.4/airsupply/cli.py
--rw-r--r--   0        0        0     6987 2023-06-18 20:13:03.097247 airsupply-0.4/airsupply/html.jinja2
--rw-r--r--   0        0        0     3822 2023-06-18 20:46:16.489617 airsupply-0.4/airsupply/ipa.py
--rw-r--r--   0        0        0     1673 2021-05-11 18:41:16.178945 airsupply-0.4/airsupply/ipa_manifest.jinja2
--rw-r--r--   0        0        0      987 2023-06-18 20:40:42.782744 airsupply-0.4/airsupply/local.py
--rw-r--r--   0        0        0     5746 2023-06-18 18:35:47.415996 airsupply-0.4/airsupply/push.py
--rw-r--r--   0        0        0     1441 2023-06-18 20:40:55.247744 airsupply-0.4/airsupply/s3.py
--rw-r--r--   0        0        0      166 2020-01-29 08:19:41.000000 airsupply-0.4/airsupply/templates.py
--rw-r--r--   0        0        0      497 2023-06-18 20:46:34.081842 airsupply-0.4/pyproject.toml
--rw-r--r--   0        0        0      723 1970-01-01 00:00:00.000000 airsupply-0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-01-24 03:52:19.000000 airsupply-0.4.1/airsupply/__init__.py
+-rw-r--r--   0        0        0       30 2020-01-24 03:52:44.000000 airsupply-0.4.1/airsupply/__main__.py
+-rw-r--r--   0        0        0      369 2020-01-29 08:19:41.000000 airsupply-0.4.1/airsupply/apk.py
+-rw-r--r--   0        0        0     2042 2023-06-18 18:04:25.108912 airsupply-0.4.1/airsupply/cli.py
+-rw-r--r--   0        0        0     8343 2023-06-19 01:27:09.183060 airsupply-0.4.1/airsupply/html.jinja2
+-rw-r--r--   0        0        0     3822 2023-06-18 20:46:16.489617 airsupply-0.4.1/airsupply/ipa.py
+-rw-r--r--   0        0        0     1673 2021-05-11 18:41:16.178945 airsupply-0.4.1/airsupply/ipa_manifest.jinja2
+-rw-r--r--   0        0        0      987 2023-06-18 20:40:42.782744 airsupply-0.4.1/airsupply/local.py
+-rw-r--r--   0        0        0     5746 2023-06-18 23:56:47.595306 airsupply-0.4.1/airsupply/push.py
+-rw-r--r--   0        0        0     1441 2023-06-18 20:40:55.247744 airsupply-0.4.1/airsupply/s3.py
+-rw-r--r--   0        0        0      166 2020-01-29 08:19:41.000000 airsupply-0.4.1/airsupply/templates.py
+-rw-r--r--   0        0        0      499 2023-06-19 01:28:01.830490 airsupply-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 airsupply-0.4.1/PKG-INFO
```

### Comparing `airsupply-0.4/airsupply/cli.py` & `airsupply-0.4.1/airsupply/cli.py`

 * *Files identical despite different names*

### Comparing `airsupply-0.4/airsupply/html.jinja2` & `airsupply-0.4.1/airsupply/html.jinja2`

 * *Files 13% similar despite different names*

```diff
@@ -103,14 +103,15 @@
     </option>
     {% endfor %}
   </select>
 {% for pkg in packages %}
   <div
     id="pkg-{{ loop.index }}"
     class="package"
+    data-fragment="{{ pkg.app_id }}:{{ pkg.version_code }}"
     data-title="{{ pkg.display_name }} v{{ pkg.version_name }} ({{ pkg.version_code }})"
     data-type="{{ pkg.package_type }}"
   >
     <h1>{{ pkg.display_name }}</h1>
     <h2>{{ pkg.version_name }} ({{ pkg.version_code }})</h2>
     {% if pkg.image_url %}
     <img class="app-icon" src="{{ pkg.image_url | safe }}">
@@ -127,14 +128,17 @@
     <a
       href="{{ pkg.download_url | safe }}"
       class="btn"
     >
       Download
     </a>
     <p class="comment">
+      <a class="copy-link-btn" href="#{{ pkg.app_id }}:{{ pkg.version_code }}">Copy Permalink</a>
+    </p>
+    <p class="comment">
       {% set os = 'Android' if pkg.package_type == 'apk' else 'WatchOS' if pkg.platform == 'watchos' else 'iOS' %}
       {% if pkg.minimum_os_version is defined %}
       This app requires <b>{{ os }} {{ pkg.minimum_os_version }}</b> or higher.
       {% else %}
       This app requires <b>{{ os }}</b>.
       {% endif %}
     </p>
@@ -197,69 +201,110 @@
   window.addEventListener('keydown', function (e) {
     if (modal.style.display === 'none') return;
     if (e.key === 'Escape') {
       modal.style.display = 'none';
     }
   });
 
-  var defaultPackageId = null;
+  window.addEventListener('hashchange', function (e) {
+    if (!window.location.hash) return;
+
+    for (var i = 0 ; i < packages.length ; ++i) {
+      var pkg = packages[i];
+      if (window.location.hash === '#' + pkg.dataset.fragment) {
+        return selectPackageById(pkg.id);
+      }
+    }
+    // if nothing matched then just clear the hash
+    window.location.fragment = '';
+  });
+
+  var activePackageId = null;
   for (var i = 0 ; i < packages.length ; ++i) {
     var pkg = packages[i];
     var isPackageInstallable = (
       (OS === 'android' && pkg.dataset.type === 'apk')
       || (OS === 'ios' && pkg.dataset.type === 'ipa')
     );
     if (!isPackageInstallable) {
       var installBtn = pkg.querySelector('.install-btn');
       installBtn.classList.add('disabled');
     }
-    else if (defaultPackageId === null) {
-      defaultPackageId = pkg.id;
+    else if (activePackageId === null) {
+      activePackageId = pkg.id;
     }
 
     var qrBtn = pkg.querySelector('.show-qr-btn');
     qrBtn.addEventListener('click', function () {
       modal.style.display = 'block';
-      qrcode.makeCode(window.location.href);
-    });
+      qrcode.makeCode(permalinkWithFragment(this.dataset.fragment));
+    }.bind(pkg));
+
+    var copyBtn = pkg.querySelector('.copy-link-btn');
+    copyBtn.addEventListener('click', function (e) {
+      e.preventDefault();
+
+      const type = "text/plain";
+      const text = permalinkWithFragment(this.dataset.fragment);
+      const blob = new Blob([text], { type });
+      const data = [new ClipboardItem({ [type]: blob })];
+
+      navigator.clipboard.write(data).then(
+        function () {},
+        function () {
+          alert('Failed to copy to clipboard.');
+        },
+      );
+    }.bind(pkg));
   }
 
   // if a fragment is set then search for that item first
   if (window.location.hash) {
     for (var i = 0 ; i < packages.length ; ++i) {
       var pkg = packages[i];
-      if (window.location.hash === '#' + pkg.id) {
-        defaultPackageId = pkg.id;
+      if (window.location.hash === '#' + pkg.dataset.fragment) {
+        activePackageId = pkg.id;
       }
     }
   }
   // if we still don't have an initial package then use the first
-  if (!defaultPackageId) {
-    defaultPackageId = packages[0].id;
+  if (!activePackageId) {
+    activePackageId = packages[0].id;
   }
 
   // mark the default package as selected
-  for (var i = 0 ; i < select.options.length ; ++i) {
-    var opt = select.options[i];
-    opt.selected = opt.value === defaultPackageId;
-  }
-  selectPackageById(defaultPackageId);
+  selectPackageById(activePackageId);
 
   function selectPackageById(id) {
+    activePackageId = id;
+
+    for (var i = 0 ; i < select.options.length ; ++i) {
+      var opt = select.options[i];
+      opt.selected = opt.value === id;
+    }
+
     for (var i = 0 ; i < packages.length ; ++i) {
       var pkg = packages[i];
       if (pkg.id === id) {
         document.title = pkg.dataset.title;
-        window.location.hash = '#' + pkg.id;
         pkg.classList.remove('hidden');
       }
       else {
         pkg.classList.add('hidden');
       }
     }
+    // clear out the selected hash
+    if (window.location.hash) {
+      window.location.hash = '';
+    }
+  }
+
+  function permalinkWithFragment(fragment) {
+    var url = window.location.href.split('#', 1)[0];
+    return url + '#' + fragment;
   }
   </script>
 </body>
 </html>
 <!--
 created at: {{ created_at }}
 updated at: {{ updated_at }}
```

#### html2text {}

```diff
@@ -4,14 +4,15 @@
 { pkg.version_code }})
 {% endfor %}
  {% for pkg in packages %}
 ****** {{ pkg.display_name }} ******
 ***** {{ pkg.version_name }} ({{ pkg.version_code }}) *****
 {% if pkg.image_url %} [{{ pkg.image_url | safe }}] {% endif %} Install  Show
 QR  Download
+Copy_Permalink
 {% set os = 'Android' if pkg.package_type == 'apk' else 'WatchOS' if
 pkg.platform == 'watchos' else 'iOS' %} {% if pkg.minimum_os_version is defined
 %} This app requires {{ os }} {{ pkg.minimum_os_version }} or higher. {% else
 %} This app requires {{ os }}. {% endif %}
 {{ pkg.app_id }}
 {% endfor %}
 ×
```

### Comparing `airsupply-0.4/airsupply/ipa.py` & `airsupply-0.4.1/airsupply/ipa.py`

 * *Files identical despite different names*

### Comparing `airsupply-0.4/airsupply/ipa_manifest.jinja2` & `airsupply-0.4.1/airsupply/ipa_manifest.jinja2`

 * *Files identical despite different names*

### Comparing `airsupply-0.4/airsupply/local.py` & `airsupply-0.4.1/airsupply/local.py`

 * *Files identical despite different names*

### Comparing `airsupply-0.4/airsupply/push.py` & `airsupply-0.4.1/airsupply/push.py`

 * *Files identical despite different names*

### Comparing `airsupply-0.4/airsupply/s3.py` & `airsupply-0.4.1/airsupply/s3.py`

 * *Files identical despite different names*

### Comparing `airsupply-0.4/PKG-INFO` & `airsupply-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airsupply
-Version: 0.4
+Version: 0.4.1
 Summary: Manage OTA distribution for IPA and APK files.
 License: MIT
 Author: Michael Merickel
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

