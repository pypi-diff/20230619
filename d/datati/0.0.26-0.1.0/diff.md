# Comparing `tmp/datati-0.0.26.tar.gz` & `tmp/datati-0.1.0.tar.gz`

## Comparing `datati-0.0.26.tar` & `datati-0.1.0.tar`

### file list

```diff
@@ -1,47 +1,50 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 datati-0.0.26/.idea/.gitignore
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 datati-0.0.26/.idea/datati.iml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 datati-0.0.26/.idea/misc.xml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 datati-0.0.26/.idea/modules.xml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 datati-0.0.26/.idea/other.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 datati-0.0.26/.idea/vcs.xml
--rw-r--r--   0        0        0     9599 2020-02-02 00:00:00.000000 datati-0.0.26/.idea/workspace.xml
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 datati-0.0.26/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 datati-0.0.26/src/.idea/.gitignore
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 datati-0.0.26/src/.idea/misc.xml
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 datati-0.0.26/src/.idea/modules.xml
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 datati-0.0.26/src/.idea/src.iml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 datati-0.0.26/src/.idea/vcs.xml
--rw-r--r--   0        0        0     4205 2020-02-02 00:00:00.000000 datati-0.0.26/src/.idea/workspace.xml
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 datati-0.0.26/src/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 datati-0.0.26/src/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     9309 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/LICENSE
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/__init__.py
--rw-r--r--   0        0        0     9442 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/dataset.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/pipeline.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/requirements.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/.idea/.gitignore
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/.idea/datati.iml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/.idea/misc.xml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/.idea/modules.xml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/.idea/vcs.xml
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/.idea/workspace.xml
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/.idea/scopes/datati.xml
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/encoding/__init__.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/encoding/quantization.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/models/README.md
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/models/__init__.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/models/binary.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/models/trees.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/models/modelers/__init__.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/models/modelers/filters.py
--rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/models/modelers/numeric.py
--rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 datati-0.0.26/src/datati/models/modelers/one_hot.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 datati-0.0.26/tests/test_modeler.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 datati-0.0.26/LICENSE
--rw-r--r--   0        0        0     8271 2020-02-02 00:00:00.000000 datati-0.0.26/README.md
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 datati-0.0.26/pyproject.toml
--rw-r--r--   0        0        0    10705 2020-02-02 00:00:00.000000 datati-0.0.26/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 datati-0.1.0/.idea/.gitignore
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 datati-0.1.0/.idea/datati.iml
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 datati-0.1.0/.idea/jupyter-settings.xml
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 datati-0.1.0/.idea/misc.xml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 datati-0.1.0/.idea/modules.xml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 datati-0.1.0/.idea/other.xml
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 datati-0.1.0/.idea/vcs.xml
+-rw-r--r--   0        0        0    11645 2020-02-02 00:00:00.000000 datati-0.1.0/.idea/workspace.xml
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 datati-0.1.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 datati-0.1.0/.idea/scopes/datati.xml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 datati-0.1.0/src/.idea/.gitignore
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 datati-0.1.0/src/.idea/jupyter-settings.xml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 datati-0.1.0/src/.idea/misc.xml
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 datati-0.1.0/src/.idea/modules.xml
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 datati-0.1.0/src/.idea/src.iml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 datati-0.1.0/src/.idea/vcs.xml
+-rw-r--r--   0        0        0     4298 2020-02-02 00:00:00.000000 datati-0.1.0/src/.idea/workspace.xml
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 datati-0.1.0/src/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 datati-0.1.0/src/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     9309 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/LICENSE
+-rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/__init__.py
+-rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/dataset.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/pipeline.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/requirements.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/.idea/.gitignore
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/.idea/datati.iml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/.idea/misc.xml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/.idea/modules.xml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/.idea/vcs.xml
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/.idea/workspace.xml
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/.idea/scopes/datati.xml
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/encoding/__init__.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/encoding/quantization.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/models/README.md
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/models/__init__.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/models/binary.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/models/trees.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/models/modelers/__init__.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/models/modelers/filters.py
+-rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/models/modelers/numeric.py
+-rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 datati-0.1.0/src/datati/models/modelers/one_hot.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 datati-0.1.0/tests/test_modeler.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 datati-0.1.0/LICENSE
+-rw-r--r--   0        0        0     8138 2020-02-02 00:00:00.000000 datati-0.1.0/README.md
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 datati-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 datati-0.1.0/PKG-INFO
```

### Comparing `datati-0.0.26/.idea/datati.iml` & `datati-0.1.0/.idea/datati.iml`

 * *Files identical despite different names*

### Comparing `datati-0.0.26/.idea/workspace.xml` & `datati-0.1.0/.idea/workspace.xml`

 * *Files 18% similar despite different names*

#### Comparing `datati-0.0.26/.idea/workspace.xml` & `datati-0.1.0/.idea/workspace.xml`

```diff
@@ -1,38 +1,53 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AnalysisUIOptions">
     <option name="ANALYZE_INJECTED_CODE" value="false"/>
+    <option name="SCOPE_TYPE" value="8"/>
+    <option name="CUSTOM_SCOPE_NAME" value="datati"/>
   </component>
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="ChangeListManager">
     <list default="true" id="5d0c4f20-94d7-4865-9ee8-18d354e82f5e" name="Changes" comment="">
-      <change beforePath="$PROJECT_DIR$/src/models/__init__.py" beforeDir="false"/>
-      <change beforePath="$PROJECT_DIR$/src/models/binary.py" beforeDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/datati/README.md" beforeDir="false" afterPath="$PROJECT_DIR$/src/datati/README.md" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/datati/dataset.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/datati/dataset.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/datati/encoding/quantization.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/datati/encoding/quantization.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/datati/models/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/datati/models/__init__.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/datati/models/binary.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/datati/models/binary.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/datati/models/modelers/filters.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/datati/models/modelers/filters.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/datati/models/modelers/numeric.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/datati/models/modelers/numeric.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/datati/models/modelers/one_hot.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/datati/models/modelers/one_hot.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/datati/models/trees.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/datati/models/trees.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/datati/pipeline.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/datati/pipeline.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
       <list>
         <option value="Python Script"/>
       </list>
     </option>
   </component>
   <component name="Git.Settings">
-    <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
+    <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$/src/datati"/>
   </component>
   <component name="MarkdownSettingsMigration">
     <option name="stateVersion" value="1"/>
   </component>
+  <component name="NamedScopeManager">
+    <order>
+      <scope name="datati"/>
+    </order>
+  </component>
   <component name="ProblemsViewState">
     <option name="selectedTabId" value="CurrentFile"/>
   </component>
   <component name="ProjectId" id="2NuHSfyDsmMWUI4R7dI3A8VXzfA"/>
   <component name="ProjectLevelVcsManager">
     <ConfirmationsSetting value="1" id="Add"/>
   </component>
@@ -41,31 +56,33 @@
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "WebServerToolWindowFactoryState": "true",
-    "last_opened_file_path": "/home/ms/di.onedrive/research/datasets/datati_pip/datati/src/datati",
+    "git-widget-placeholder": "dvl",
+    "last_opened_file_path": "/home/aslan/onedrive/research/datasets/datati_pip/datati",
     "node.js.detected.package.eslint": "true",
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)",
     "run.code.analysis.last.selected.profile": "pProject Default",
-    "settings.editor.selected.configurable": "preferences.pluginManager",
+    "settings.editor.selected.configurable": "editor.preferences.fonts.default",
+    "settings.editor.splitter.proportion": "0.153125",
     "vue.rearranger.settings.migration": "true"
   }
 }]]></component>
   <component name="RecentsManager">
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/src/datati"/>
       <recent name="$PROJECT_DIR$/src/datati/models/modelers"/>
     </key>
   </component>
-  <component name="RunManager" selected="Python.playground">
+  <component name="RunManager" selected="Python tests.Unittests">
     <configuration name="playground" type="PythonConfigurationType" factoryName="Python" nameIsGenerated="true">
       <module name="datati"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
@@ -81,14 +98,29 @@
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
+    <configuration name="Python tests for test_modeler.TestLoad" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+      <module name="datati"/>
+      <option name="INTERPRETER_OPTIONS" value=""/>
+      <option name="PARENT_ENVS" value="true"/>
+      <option name="SDK_HOME" value=""/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
+      <option name="IS_MODULE_SDK" value="true"/>
+      <option name="ADD_CONTENT_ROOTS" value="true"/>
+      <option name="ADD_SOURCE_ROOTS" value="true"/>
+      <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
+      <option name="_new_additionalArguments" value="&quot;&quot;"/>
+      <option name="_new_target" value="&quot;test_modeler.TestLoad&quot;"/>
+      <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
+      <method v="2"/>
+    </configuration>
     <configuration name="Unittests" type="tests" factoryName="Unittests">
       <module name="datati"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value="$USER_HOME$/.virtualenvs/datati/bin/python3.10"/>
       <option name="SDK_NAME" value="Python 3.10 (datati)"/>
       <option name="WORKING_DIRECTORY" value=""/>
@@ -101,81 +133,64 @@
       <option name="_new_target" value="&quot;$PROJECT_DIR$/tests/test_modeler.py&quot;"/>
       <option name="_new_targetType" value="&quot;PATH&quot;"/>
       <method v="2"/>
     </configuration>
     <list>
       <item itemvalue="Python.playground"/>
       <item itemvalue="Python tests.Unittests"/>
+      <item itemvalue="Python tests.Python tests for test_modeler.TestLoad"/>
     </list>
+    <recent_temporary>
+      <list>
+        <item itemvalue="Python tests.Python tests for test_modeler.TestLoad"/>
+      </list>
+    </recent_temporary>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="5d0c4f20-94d7-4865-9ee8-18d354e82f5e" name="Changes" comment=""/>
       <created>1680507049272</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1680507049272</updated>
       <workItem from="1680507054707" duration="11188000"/>
       <workItem from="1680610121474" duration="2774000"/>
       <workItem from="1681314129394" duration="9355000"/>
       <workItem from="1681397215597" duration="10607000"/>
       <workItem from="1681818046010" duration="7992000"/>
+      <workItem from="1686954883285" duration="103000"/>
+      <workItem from="1686955002695" duration="3013000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="UnknownFeatures">
     <option featureType="com.intellij.fileTypeFactory" implementationName="requirements.txt"/>
   </component>
   <component name="XDebuggerManager">
     <breakpoint-manager>
       <breakpoints>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/src/datati/dataset.py</url>
-          <line>201</line>
-          <option name="timeStamp" value="1"/>
-        </line-breakpoint>
-        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <condition expression="dtype.name != &quot;bool&quot;" language="Python"/>
-          <url>file://$PROJECT_DIR$/tests/test_modeler.py</url>
-          <line>71</line>
-          <option name="timeStamp" value="13"/>
-        </line-breakpoint>
-        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_modeler.py</url>
           <line>27</line>
           <option name="timeStamp" value="14"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <condition expression="target_feature is None" language="Python"/>
-          <url>file://$PROJECT_DIR$/src/datati/models/modelers/numeric.py</url>
-          <line>41</line>
-          <option name="timeStamp" value="27"/>
-        </line-breakpoint>
-        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/src/datati/models/modelers/numeric.py</url>
-          <line>117</line>
-          <option name="timeStamp" value="41"/>
-        </line-breakpoint>
-        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/src/datati/models/modelers/one_hot.py</url>
-          <line>115</line>
-          <option name="timeStamp" value="44"/>
-        </line-breakpoint>
-        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/src/datati/models/binary.py</url>
-          <line>1</line>
-          <option name="timeStamp" value="45"/>
+          <condition expression="not (dtype.name.startswith(&quot;int&quot;) or dtype.name.startswith(&quot;float&quot;))" language="Python"/>
+          <url>file://$PROJECT_DIR$/tests/test_modeler.py</url>
+          <line>45</line>
+          <option name="timeStamp" value="47"/>
         </line-breakpoint>
       </breakpoints>
     </breakpoint-manager>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
+    <SUITE FILE_PATH="coverage/datati$playground.coverage" NAME="playground Coverage Results" MODIFIED="1681817196395" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/src/datati"/>
     <SUITE FILE_PATH="coverage/datati$dataset.coverage" NAME="dataset Coverage Results" MODIFIED="1680507554073" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/src/datati"/>
     <SUITE FILE_PATH="coverage/datati$one_hot.coverage" NAME="one_hot Coverage Results" MODIFIED="1680511960642" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/src/datati/models/modelers"/>
-    <SUITE FILE_PATH="coverage/datati$Unittests.coverage" NAME="Unittests Coverage Results" MODIFIED="1681344763672" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY=""/>
-    <SUITE FILE_PATH="coverage/datati$playground.coverage" NAME="playground Coverage Results" MODIFIED="1681817196395" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/src/datati"/>
+    <SUITE FILE_PATH="coverage/datati$Unittests.coverage" NAME="Unittests Coverage Results" MODIFIED="1686957981763" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY=""/>
+    <SUITE FILE_PATH="coverage/datati$.coverage" NAME=" Coverage Results" MODIFIED="1686955381179" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/tests"/>
   </component>
 </project>
```

### Comparing `datati-0.0.26/.idea/inspectionProfiles/Project_Default.xml` & `datati-0.1.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `datati-0.0.26/src/.idea/workspace.xml` & `datati-0.1.0/src/.idea/workspace.xml`

 * *Files 8% similar despite different names*

#### Comparing `datati-0.0.26/src/.idea/workspace.xml` & `datati-0.1.0/src/.idea/workspace.xml`

```diff
@@ -33,32 +33,35 @@
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent"><![CDATA[{
   "keyToString": {
     "RunOnceActivity.OpenProjectViewOnStart": "true",
     "RunOnceActivity.ShowReadmeOnStart": "true",
     "WebServerToolWindowFactoryState": "false",
+    "git-widget-placeholder": "dvl",
     "last_opened_file_path": "/home/aslan/onedrive/research/datasets/datati_pip/datati/src",
     "node.js.detected.package.eslint": "true",
     "node.js.detected.package.tslint": "true",
     "node.js.selected.package.eslint": "(autodetect)",
     "node.js.selected.package.tslint": "(autodetect)",
-    "settings.editor.selected.configurable": "com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable",
+    "nodejs_package_manager_path": "npm",
+    "settings.editor.selected.configurable": "preferences.general",
     "vue.rearranger.settings.migration": "true"
   }
 }]]></component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="ec93cc03-41e9-4a1f-ad90-cd7e92597ef7" name="Changes" comment=""/>
       <created>1682245150938</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1682245150938</updated>
       <workItem from="1682245152173" duration="5127000"/>
+      <workItem from="1686951522294" duration="1673000"/>
     </task>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="XDebuggerManager">
```

### Comparing `datati-0.0.26/src/.idea/inspectionProfiles/Project_Default.xml` & `datati-0.1.0/src/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `datati-0.0.26/src/datati/.gitignore` & `datati-0.1.0/src/datati/.gitignore`

 * *Files identical despite different names*

### Comparing `datati-0.0.26/src/datati/LICENSE` & `datati-0.1.0/src/datati/LICENSE`

 * *Files identical despite different names*

### Comparing `datati-0.0.26/src/datati/README.md` & `datati-0.1.0/src/datati/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 # Datati: Modern (tabular) datasets require modern solutions
 
-> :warning: Warning, alpha version, everything brakes, only tested on Huggingface and single-output datasets for
-> now. :warning:
-
-
 __Dataset to model, in one go!__
 **datati** is a small library to streamline tabular dataset loading and preprocessing.
 The goal of this library is to minimize the boring boilerplate code that separates choosing a dataset to work on,
 and actually getting it ready to train a classification model .
 `datati` provides simple interfaces to load, preprocess, and encode a dataset for training your model of choice:
 ```python
 from datati.dataset import Dataset
@@ -25,17 +21,17 @@
 Then we use a `Modeler` object to map the initial `Dataset` into an encoding suitable for Decision Tree induction
 (`modeler.process(dataset)`).
 
 `datati` builds on top of the huggingface hub, providing an interface to integrate it with common preprocessing
 pipelines.
 
 # Quickstart
-`datati` is currently available on test-pypi:
+`datati` is currently available on pypi:
 ```shell
-pip install --extra-index-url https://test.pypi.org/simple/ datati
+pip install datati
 ```
 
 ## What datasets are available?
 `datati` allows you to load huggingface (`load_from="huggingface"`), or local (`load_from="local"`) datasets,
 whether they are `numpy.array`s, `pandas.DataFrame`s, or `pyarrow.ArrowDataset`s.
 
 I'm curating a list of datasets directly on Huggingface at [huggingface.co/mstz](https://huggingface.co/mstz).
```

### Comparing `datati-0.0.26/src/datati/dataset.py` & `datati-0.1.0/src/datati/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from __future__ import annotations
 import warnings
 
-from pandas import DataFrame, Series
-from pandas import Index
-from pandas._libs import lib
+from pandas import DataFrame
 
 warnings.simplefilter(action="ignore", category=UserWarning)
 
 import copy
-from typing import Optional, Dict, TypeVar, Sequence, Tuple, Literal, Callable, Hashable, Mapping
+from typing import Optional, Dict, TypeVar, Sequence, Tuple
 
 import numpy
 import pandas
 from pandas._typing import IgnoreRaise, Axes, Dtype
 from datasets.arrow_dataset import Dataset as ArrowDataset
 from datasets import load_dataset as load_huggingface_dataset
```

### Comparing `datati-0.0.26/src/datati/requirements.txt` & `datati-0.1.0/src/datati/requirements.txt`

 * *Files identical despite different names*

### Comparing `datati-0.0.26/src/datati/.idea/workspace.xml` & `datati-0.1.0/src/datati/.idea/workspace.xml`

 * *Files 3% similar despite different names*

#### Comparing `datati-0.0.26/src/datati/.idea/workspace.xml` & `datati-0.1.0/src/datati/.idea/workspace.xml`

```diff
@@ -36,15 +36,15 @@
     <option name="showLibraryContents" value="true"/>
   </component>
   <component name="PropertiesComponent">{
   &quot;keyToString&quot;: {
     &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
     &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
     &quot;WebServerToolWindowFactoryState&quot;: &quot;true&quot;,
-    &quot;last_opened_file_path&quot;: &quot;/home/ms/onedrive/research/datasets/datati_pip/datati/src/datati&quot;,
+    &quot;last_opened_file_path&quot;: &quot;/home/ms/onedrive/research/datasets/autotraino&quot;,
     &quot;run.code.analysis.last.selected.profile&quot;: &quot;pProject Default&quot;,
     &quot;settings.editor.selected.configurable&quot;: &quot;com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable&quot;
   }
 }</component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
@@ -53,12 +53,13 @@
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1681826051505</updated>
       <workItem from="1681826052713" duration="1280000"/>
       <workItem from="1681829033965" duration="5066000"/>
       <workItem from="1682065285700" duration="487000"/>
       <workItem from="1683127485089" duration="339000"/>
-      <workItem from="1683130306834" duration="2335000"/>
+      <workItem from="1683130306834" duration="5650000"/>
+      <workItem from="1684946685330" duration="31000"/>
     </task>
     <servers/>
   </component>
 </project>
```

### Comparing `datati-0.0.26/src/datati/.idea/inspectionProfiles/Project_Default.xml` & `datati-0.1.0/src/datati/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `datati-0.0.26/src/datati/encoding/__init__.py` & `datati-0.1.0/src/datati/encoding/__init__.py`

 * *Files identical despite different names*

### Comparing `datati-0.0.26/src/datati/encoding/quantization.py` & `datati-0.1.0/src/datati/encoding/quantization.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Quantization measures to map sets of values to bins."""
 from __future__ import annotations
 
 import numpy
 
-from ..encoding import NumericBinner
+from encoding import NumericBinner
 
 
 class Quantiler(NumericBinner):
     """Quantization of numerical values into bins given by quantiles."""
     def __init__(self, n_quantiles: int = 4):
         super().__init__()
         self.n_quantiles = n_quantiles
```

### Comparing `datati-0.0.26/src/datati/models/README.md` & `datati-0.1.0/src/datati/models/README.md`

 * *Files identical despite different names*

### Comparing `datati-0.0.26/src/datati/models/__init__.py` & `datati-0.1.0/src/datati/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Model the given dataset for the desired model of choice by transforming its features."""
 
 from abc import abstractmethod, ABC
 
-from ..dataset import Dataset
+from dataset import Dataset
 
 
 class Modeler(ABC):
     """Process the given dataset for the model of choice."""
     def __init__(self):
         pass
```

### Comparing `datati-0.0.26/src/datati/models/binary.py` & `datati-0.1.0/src/datati/models/binary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Model the given dataset in a binary format by mapping all features to a 0-1 domain."""
 from typing import Optional, Dict
 
-from ..dataset import Dataset
-from ..encoding import Binner
-from ..models.modelers.one_hot import BinaryBoolModeler
+from dataset import Dataset
+from encoding import Binner
+from models.modelers.one_hot import BinaryBoolModeler
 
 
 class CorelsModeler(BinaryBoolModeler):
     def __init__(self, binner: Optional[Binner | Dict[str, Binner]] = None):
         """
         Args:
             binner: Optional binner to bin features. Either a unique binner, which will be applied to all features,
```

### Comparing `datati-0.0.26/src/datati/models/trees.py` & `datati-0.1.0/src/datati/models/trees.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 
-from ..dataset import Dataset
-from ..models import Modeler
-from ..models.modelers.numeric import TargetModeler, BoolToIntModeler
-from ..models.modelers.one_hot import OneHotModeler
-from ..pipeline import Pipeline
+from dataset import Dataset
+from models import Modeler
+from models.modelers.numeric import TargetModeler, BoolToIntModeler
+from models.modelers.one_hot import OneHotModeler
+from pipeline import Pipeline
 
 
 class ContinuousTreeModeler(Modeler):
     """Model data as continuous, mapping boolean features to 0/1, and categorical features to target encoders."""
     def __init__(self):
         super().__init__()
         self.pipeline = Pipeline(TargetModeler(), BoolToIntModeler(guess_booleans=True))
```

### Comparing `datati-0.0.26/src/datati/models/modelers/filters.py` & `datati-0.1.0/src/datati/models/modelers/filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from ...dataset import Dataset
-from .. import Modeler
+from dataset import Dataset
+from models import Modeler
 
 
 class ContinuousModeler(Modeler):
     """Filter out all non-continuous features."""
     def __init__(self):
         super().__init__()
```

### Comparing `datati-0.0.26/src/datati/models/modelers/numeric.py` & `datati-0.1.0/src/datati/models/modelers/numeric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import copy
 from typing import List, Optional, Dict
 
 import numpy
 import pandas
 
-from ...dataset import Dataset
-from ...encoding.quantization import Quantiler
-from ...encoding import Binner, NumericBinner
-from .. import Modeler
+from dataset import Dataset
+from encoding.quantization import Quantiler
+from encoding import Binner, NumericBinner
+from models import Modeler
 
 
 class TargetModeler(Modeler):
     """Map all categorical features with target encoding.
     Attributes:
         encoding_map: Dictionary category => encoding.
     """
@@ -41,17 +41,17 @@
         # only use n - 1 encodings since the last one can be inferred from the other ones
         unique_target_values = dataset_copy[target_feature].unique()[:-1]
 
         for categorical_feature in categorical_features:
             feature_values = dataset_copy[categorical_feature]
             unique_feature_values = feature_values.unique()
             values_per_categorical_feature.append(unique_feature_values)
-            target_counts_per_category = numpy.array(
-                [numpy.array([dataset_copy[(dataset_copy[categorical_feature] == value)
-                                             & (dataset_copy[target_feature] == target_value)].shape[0]
+            target_counts_per_category = numpy.array([
+                                            numpy.array([dataset_copy[(dataset_copy[categorical_feature] == value)
+                                                                      & (dataset_copy[target_feature] == target_value)].shape[0]
                               for target_value in unique_target_values])
                  for value in unique_feature_values])
             encoded_feature = (target_counts_per_category / nr_records)
             self.encoding_map[categorical_feature] = {feature_value: encoded_feature_value
                                                       for feature_value, encoded_feature_value in zip(unique_feature_values, encoded_feature)}
 
         for categorical_feature, unique_feature_values in zip(categorical_features, values_per_categorical_feature):
@@ -60,15 +60,15 @@
             # dataframe values must be hashable, hence need to first split numpy array, then create the encoded dataframe
             encoded_df = list()
             for target_index, target_value in enumerate(unique_target_values):
                 # encoded_df = [self.encoding_map[categorical_feature][x] for x in dataset_copy[categorical_feature].values]
                 encoded_feature = dataset_copy[categorical_feature].apply(lambda x:
                                                                           self.encoding_map[categorical_feature][x][target_index])
                 encoded_df.append(pandas.DataFrame(encoded_feature))
-            encoded_df = pandas.concat(encoded_df, axis="columns")
+            encoded_df = pandas.concat(encoded_df, axis="columns").astype("float64")
             encoded_df.columns = [f"{categorical_feature}{feature_name_separator}{target_value}"
                                   for target_value in unique_target_values]
             preceding_df = dataset_copy[list(dataset_copy.columns)[:position]]
             following_df = dataset_copy[list(dataset_copy.columns)[position + 1:]]
             dataset_copy = pandas.concat((preceding_df, encoded_df, following_df),
                                            axis="columns")
         dataset_copy = Dataset(dataset_copy)
@@ -96,14 +96,16 @@
         """
         dataset_copy = copy.deepcopy(dataset)
         features_to_ignore = kwargs.get("features_to_ignore", [dataset_copy.target_feature])
         bins_are_categories = kwargs.get("bins_are_categories", True)
         features = [f for f in dataset_copy.columns if f not in features_to_ignore]
         if self.binners is None:
             self.binners = {f: Quantiler(n_quantiles=4) for f in dataset_copy.columns}
+        elif isinstance(self.binners, Binner):
+            self.binners = {f: copy.deepcopy(self.binners) for f in dataset_copy.columns}
 
         for feature in features:
             if isinstance(self.binners[feature], NumericBinner)\
                     and not (dataset_copy.dtypes[feature].name.startswith("int")
                              or dataset_copy.dtypes[feature].name.startswith("float")):
                 continue
```

### Comparing `datati-0.0.26/src/datati/models/modelers/one_hot.py` & `datati-0.1.0/src/datati/models/modelers/one_hot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import copy
 from functools import partial
 from typing import Dict
 
 import numpy
 import pandas
 
-from ...encoding import Binner
+from encoding import Binner
 
-from ...dataset import Dataset
-from .. import Modeler
-from ..modelers.numeric import BinModeler, IntToBoolModeler
-from ...pipeline import Pipeline
+from dataset import Dataset
+from models import Modeler
+from models.modelers.numeric import BinModeler, IntToBoolModeler
+from pipeline import Pipeline
 
 
 class BinaryBoolModeler(Modeler):
     """Transform the given dataset into a binary one by:
         - binning its numerical features;
         - create a one-hot encoding of such bins.
 
     Attributes:
         one_hot_encoding_dictionary: Dictionary mapping each feature and value to the position in the one-hot space.
         bins_encoding_dictionary: Dictionary mapping each bin to its elements.
         base_binners: The base binner used to create a binner for each feature.
         fit_binners: Binners fit to each feature.
     """
-    def __init__(self, binner: Binner | Dict[str, Binner]):
+    def __init__(self, binner: Dict[str, Binner]):
         """
         Args:
             binner: Base Binner. A copy of such binner will be fit on each feature to bin.
         """
         super().__init__()
         self.one_hot_encoding_dictionary = dict()
         self.bins_encoding_dictionary = dict()
```

### Comparing `datati-0.0.26/tests/test_modeler.py` & `datati-0.1.0/tests/test_modeler.py`

 * *Files identical despite different names*

### Comparing `datati-0.0.26/LICENSE` & `datati-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datati-0.0.26/README.md` & `datati-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 # Datati: Modern (tabular) datasets require modern solutions
- 
-> :warning: Warning, alpha version, everything brakes, only tested on Huggingface and single-output datasets for
-> now. :warning:
-
 
 __Dataset to model, in one go!__
 **datati** is a small library to streamline tabular dataset loading and preprocessing.
 The goal of this library is to minimize the boring boilerplate code that separates choosing a dataset to work on,
 and actually getting it ready to train a classification model .
 `datati` provides simple interfaces to load, preprocess, and encode a dataset for training your model of choice:
 ```python
```

### Comparing `datati-0.0.26/pyproject.toml` & `datati-0.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "datati"
-version = "0.0.26"
+version = "0.1.0"
 authors = [
-  { name="Mattia Setzu", email="mattia.setzu@di.unipi.it" },
+  { name="Mattia Setzu", email="mattia.setzu@unipi.it" },
 ]
 description = "Download and preprocess your dataset from any source, all in one place."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Operating System :: OS Independent",
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers"
 ]
 dependencies = [
     "aiohttp == 3.8.4",
     "aiosignal == 1.3.1",
     "async-timeout == 4.0.2",
     "attrs == 23.1.0",
```

### Comparing `datati-0.0.26/PKG-INFO` & `datati-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: datati
-Version: 0.0.26
+Version: 0.1.0
 Summary: Download and preprocess your dataset from any source, all in one place.
 Project-URL: Homepage, https://github.com/msetzu/datati
 Project-URL: Bug Tracker, https://github.com/msetzu/datati/issues
-Author-email: Mattia Setzu <mattia.setzu@di.unipi.it>
+Author-email: Mattia Setzu <mattia.setzu@unipi.it>
 License-File: LICENSE
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: aiosignal==1.3.1
@@ -66,18 +66,14 @@
 Requires-Dist: webencodings==0.5.1
 Requires-Dist: xxhash==3.2.0
 Requires-Dist: yarl==1.8.2
 Requires-Dist: zipp==3.15.0
 Description-Content-Type: text/markdown
 
 # Datati: Modern (tabular) datasets require modern solutions
- 
-> :warning: Warning, alpha version, everything brakes, only tested on Huggingface and single-output datasets for
-> now. :warning:
-
 
 __Dataset to model, in one go!__
 **datati** is a small library to streamline tabular dataset loading and preprocessing.
 The goal of this library is to minimize the boring boilerplate code that separates choosing a dataset to work on,
 and actually getting it ready to train a classification model .
 `datati` provides simple interfaces to load, preprocess, and encode a dataset for training your model of choice:
 ```python
```

