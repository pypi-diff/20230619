# Comparing `tmp/netbox_plugin_machine_tracking-0.0.4.tar.gz` & `tmp/netbox_plugin_machine_tracking-0.0.5.tar.gz`

## Comparing `netbox_plugin_machine_tracking-0.0.4.tar` & `netbox_plugin_machine_tracking-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/__init__.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/filtersets.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/forms.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/models.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/navigation.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/tables.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/template_content.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/urls.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/api/__init__.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/api/serializers.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/api/urls.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/api/views.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/migrations/0001_initial.py
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/migrations/0002_event_part_type.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/migrations/0003_alter_replacement_part_type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/migrations/__init__.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/templates/machine_tracking/device_panel.html
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/templates/machine_tracking/event.html
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/machine_tracking/templates/machine_tracking/replacement.html
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/LICENCE
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/README.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/__init__.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/filtersets.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/forms.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/models.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/navigation.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/tables.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/template_content.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/urls.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/api/__init__.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/api/serializers.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/api/urls.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/api/views.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/migrations/0001_initial.py
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/migrations/0002_event_part_type.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/migrations/0003_alter_replacement_part_type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/migrations/__init__.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/templates/machine_tracking/device_panel.html
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/templates/machine_tracking/event.html
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/machine_tracking/templates/machine_tracking/replacement.html
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/.gitignore
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/LICENCE
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/README.md
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 netbox_plugin_machine_tracking-0.0.5/PKG-INFO
```

### Comparing `netbox_plugin_machine_tracking-0.0.4/machine_tracking/filtersets.py` & `netbox_plugin_machine_tracking-0.0.5/machine_tracking/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.4/machine_tracking/forms.py` & `netbox_plugin_machine_tracking-0.0.5/machine_tracking/forms.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.4/machine_tracking/models.py` & `netbox_plugin_machine_tracking-0.0.5/machine_tracking/models.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.4/machine_tracking/tables.py` & `netbox_plugin_machine_tracking-0.0.5/machine_tracking/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.4/machine_tracking/template_content.py` & `netbox_plugin_machine_tracking-0.0.5/machine_tracking/template_content.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         avg_fail = timedelta(seconds=(duration_sum / (fail_count - 1)))
         avg_days = avg_fail.days
         return str(avg_days) + " days"
 
     def right_page(self):
         device = self.context['object']
         sixty_days_ago = timezone.now() - timedelta(days=60)
-        fail_events = Event.objects.filter(machine=device, new_state="failed", time__gte=sixty_days_ago)
+        fail_events = Event.objects.filter(machine=device, new_state__in=["failed","degraded"], time__gte=sixty_days_ago)
         fail_count = fail_events.count()
         fail_time = "N/A" if fail_count <= 1 else self._average_time(fail_count, fail_events)
 
         return self.render('machine_tracking/device_panel.html', extra_context={
             'fail_count': fail_count,
             'fail_time': fail_time,
         })
```

### Comparing `netbox_plugin_machine_tracking-0.0.4/machine_tracking/urls.py` & `netbox_plugin_machine_tracking-0.0.5/machine_tracking/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.4/machine_tracking/views.py` & `netbox_plugin_machine_tracking-0.0.5/machine_tracking/views.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.4/machine_tracking/api/serializers.py` & `netbox_plugin_machine_tracking-0.0.5/machine_tracking/api/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
         model = Event
         fields = (
             'id',
             'time',
             'ticket_no',
             'machine',
             'new_state',
+            'part_type',
             'event_details',
         )
 
 class ReplacementSerializer(NetBoxModelSerializer):
     class Meta:
         model = Replacement
         fields = (
```

### Comparing `netbox_plugin_machine_tracking-0.0.4/machine_tracking/api/views.py` & `netbox_plugin_machine_tracking-0.0.5/machine_tracking/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.4/machine_tracking/migrations/0001_initial.py` & `netbox_plugin_machine_tracking-0.0.5/machine_tracking/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.4/machine_tracking/templates/machine_tracking/device_panel.html` & `netbox_plugin_machine_tracking-0.0.5/machine_tracking/templates/machine_tracking/device_panel.html`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,14 @@
                 <tr>
                     <th scope="row">Average time between failures</th>
                     <td>
                         <span class="text-muted">{{ fail_time }}</span>
                     </td>
                 </tr>
                 <tr>
-                    <p scope="row"><a href="/plugins/machine-tracking/event/?machine={{object.id}}&new_state=failed">See failures</a></p>
+                    <p scope="row"><a href="/plugins/machine-tracking/event/?machine={{object.id}}&new_state=failed&new_state=degraded">See failures</a></p>
                 </tr>
                 </tbody>
             </table>
         </div>
     </div>
 </div>
```

### Comparing `netbox_plugin_machine_tracking-0.0.4/machine_tracking/templates/machine_tracking/event.html` & `netbox_plugin_machine_tracking-0.0.5/machine_tracking/templates/machine_tracking/event.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.4/machine_tracking/templates/machine_tracking/replacement.html` & `netbox_plugin_machine_tracking-0.0.5/machine_tracking/templates/machine_tracking/replacement.html`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.4/LICENCE` & `netbox_plugin_machine_tracking-0.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.4/README.md` & `netbox_plugin_machine_tracking-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `netbox_plugin_machine_tracking-0.0.4/pyproject.toml` & `netbox_plugin_machine_tracking-0.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netbox-plugin-machine-tracking"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Lisa Guo", email="lisguo@cisco.com" },
 ]
 description = "A Netbox plugin tracking failures and other state changes in devices."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -13,16 +13,20 @@
     "Operating System :: OS Independent",
 ]
 
 [tool.hatch.build]
 include = [
   "machine_tracking",
   "/templates",
+  "/api",
   "*.html",
 ]
 exclude = [
-  "*.pyc"
+  "*.pyc",
+  ".gitignore",
+  ".gitlab-ci.yml",
+  ".eggs",
 ]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `netbox_plugin_machine_tracking-0.0.4/PKG-INFO` & `netbox_plugin_machine_tracking-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-plugin-machine-tracking
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Netbox plugin tracking failures and other state changes in devices.
 Author-email: Lisa Guo <lisguo@cisco.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

