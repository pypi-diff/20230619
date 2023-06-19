# Comparing `tmp/trogon-0.4.0.tar.gz` & `tmp/trogon-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trogon-0.4.0.tar", max compression
+gzip compressed data, was "trogon-0.5.0.tar", max compression
```

## Comparing `trogon-0.4.0.tar` & `trogon-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3503 2023-05-25 14:54:56.303882 trogon-0.4.0/README.md
--rw-r--r--   0        0        0     1380 2023-05-25 18:42:46.362789 trogon-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       67 2023-05-20 10:29:22.256492 trogon-0.4.0/trogon/__init__.py
--rw-r--r--   0        0        0      123 2023-05-20 10:29:22.256748 trogon-0.4.0/trogon/constants.py
--rw-r--r--   0        0        0     1740 2023-05-25 15:45:10.256944 trogon-0.4.0/trogon/detect_run_string.py
--rw-r--r--   0        0        0     6423 2023-05-25 14:54:56.305164 trogon-0.4.0/trogon/introspect.py
--rw-r--r--   0        0        0     9544 2023-05-25 14:54:56.305692 trogon-0.4.0/trogon/run_command.py
--rw-r--r--   0        0        0    10894 2023-05-25 18:42:46.363337 trogon-0.4.0/trogon/trogon.py
--rw-r--r--   0        0        0     3859 2023-05-25 18:42:46.363629 trogon-0.4.0/trogon/trogon.scss
--rw-r--r--   0        0        0        0 2023-05-20 10:29:22.257716 trogon-0.4.0/trogon/widgets/__init__.py
--rw-r--r--   0        0        0     2829 2023-05-20 10:29:22.258043 trogon-0.4.0/trogon/widgets/about.py
--rw-r--r--   0        0        0     3874 2023-05-20 10:29:22.258321 trogon-0.4.0/trogon/widgets/command_info.py
--rw-r--r--   0        0        0     1811 2023-05-25 14:54:56.305972 trogon-0.4.0/trogon/widgets/command_tree.py
--rw-r--r--   0        0        0     8071 2023-05-25 18:42:46.363865 trogon-0.4.0/trogon/widgets/form.py
--rw-r--r--   0        0        0     2861 2023-05-20 10:29:22.258923 trogon-0.4.0/trogon/widgets/multiple_choice.py
--rw-r--r--   0        0        0    16782 2023-05-25 18:42:46.364210 trogon-0.4.0/trogon/widgets/parameter_controls.py
--rw-r--r--   0        0        0     4978 1970-01-01 00:00:00.000000 trogon-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3828 2023-06-19 08:58:27.787711 trogon-0.5.0/README.md
+-rw-r--r--   0        0        0     1380 2023-06-19 08:59:28.042822 trogon-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       67 2023-05-20 10:29:22.256492 trogon-0.5.0/trogon/__init__.py
+-rw-r--r--   0        0        0      123 2023-05-20 10:29:22.256748 trogon-0.5.0/trogon/constants.py
+-rw-r--r--   0        0        0     1740 2023-05-25 15:45:10.256944 trogon-0.5.0/trogon/detect_run_string.py
+-rw-r--r--   0        0        0     6423 2023-05-25 14:54:56.305164 trogon-0.5.0/trogon/introspect.py
+-rw-r--r--   0        0        0     9544 2023-05-25 14:54:56.305692 trogon-0.5.0/trogon/run_command.py
+-rw-r--r--   0        0        0    11141 2023-06-19 08:58:27.788019 trogon-0.5.0/trogon/trogon.py
+-rw-r--r--   0        0        0     3859 2023-05-25 18:42:46.363629 trogon-0.5.0/trogon/trogon.scss
+-rw-r--r--   0        0        0        0 2023-05-20 10:29:22.257716 trogon-0.5.0/trogon/widgets/__init__.py
+-rw-r--r--   0        0        0     2829 2023-05-20 10:29:22.258043 trogon-0.5.0/trogon/widgets/about.py
+-rw-r--r--   0        0        0     3930 2023-06-19 08:58:27.788578 trogon-0.5.0/trogon/widgets/command_info.py
+-rw-r--r--   0        0        0     1883 2023-06-19 08:58:27.788721 trogon-0.5.0/trogon/widgets/command_tree.py
+-rw-r--r--   0        0        0     8071 2023-05-25 18:42:46.363865 trogon-0.5.0/trogon/widgets/form.py
+-rw-r--r--   0        0        0     2861 2023-05-20 10:29:22.258923 trogon-0.5.0/trogon/widgets/multiple_choice.py
+-rw-r--r--   0        0        0    16765 2023-05-30 09:11:53.641476 trogon-0.5.0/trogon/widgets/parameter_controls.py
+-rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 trogon-0.5.0/PKG-INFO
```

### Comparing `trogon-0.4.0/README.md` & `trogon-0.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -98,10 +98,23 @@
     def cli():
         ...
     ```
 3. Your click app will have a new `tui` command available.
 
 See also the `examples` folder for two example apps.
 
+## Custom command name and custom help
+
+By default the command added will be called `tui` and the help text for it will be `Open Textual TUI.`
+
+You can customize one or both of these using the `help=` and `command=` parameters:
+
+```python
+@tui(command="ui", help="Open terminal UI")
+@click.group(...)
+def cli():
+    ...
+```
+
 ## Follow this project
 
 If this app interests you, you may want to join the Textual [Discord server](https://discord.gg/Enf6Z3qhVr) where you can talk to Textual developers / community.
```

### Comparing `trogon-0.4.0/pyproject.toml` & `trogon-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trogon"
-version = "0.4.0"
+version = "0.5.0"
 description = "Automatically generate a Textual TUI for your Click CLI"
 authors = ["Darren Burns <darrenb900@gmail.com>"]
 readme = "README.md"
 packages = [{include = "trogon"}]
 license = "MIT"
 homepage = "https://github.com/Textualize/trogon"
 classifiers = [
```

### Comparing `trogon-0.4.0/trogon/detect_run_string.py` & `trogon-0.5.0/trogon/detect_run_string.py`

 * *Files identical despite different names*

### Comparing `trogon-0.4.0/trogon/introspect.py` & `trogon-0.5.0/trogon/introspect.py`

 * *Files identical despite different names*

### Comparing `trogon-0.4.0/trogon/run_command.py` & `trogon-0.5.0/trogon/run_command.py`

 * *Files identical despite different names*

### Comparing `trogon-0.4.0/trogon/trogon.py` & `trogon-0.5.0/trogon/trogon.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,34 +55,36 @@
         Binding(key="f1", action="about", description="About"),
     ]
 
     def __init__(
         self,
         cli: click.BaseCommand,
         click_app_name: str,
+        command_name: str,
         name: str | None = None,
         id: str | None = None,
         classes: str | None = None,
     ):
         super().__init__(name, id, classes)
         self.command_data = None
         self.cli = cli
         self.is_grouped_cli = isinstance(cli, click.Group)
         self.command_schemas = introspect_click_app(cli)
         self.click_app_name = click_app_name
+        self.command_name = command_name
 
         try:
             self.version = metadata.version(self.click_app_name)
         except Exception:
             self.version = None
 
         self.highlighter = ReprHighlighter()
 
     def compose(self) -> ComposeResult:
-        tree = CommandTree("Commands", self.command_schemas)
+        tree = CommandTree("Commands", self.command_schemas, self.command_name)
 
         title_parts = [Text(self.click_app_name, style="b")]
         if self.version:
             version_style = self.get_component_rich_style("version-string")
             title_parts.extend(["\n", (f"v{self.version}", version_style)])
 
         title = Text.assemble(*title_parts)
@@ -212,29 +214,31 @@
 
 class Trogon(App):
     CSS_PATH = Path(__file__).parent / "trogon.scss"
 
     def __init__(
         self,
         cli: click.Group,
-        app_name: str = None,
-        click_context: click.Context = None,
+        app_name: str | None = None,
+        command_name: str = "tui",
+        click_context: click.Context | None = None,
     ) -> None:
         super().__init__()
         self.cli = cli
         self.post_run_command: list[str] = []
         self.is_grouped_cli = isinstance(cli, click.Group)
         self.execute_on_exit = False
         if app_name is None and click_context is not None:
             self.app_name = detect_run_string()
         else:
             self.app_name = app_name
+        self.command_name = command_name
 
     def on_mount(self):
-        self.push_screen(CommandBuilder(self.cli, self.app_name))
+        self.push_screen(CommandBuilder(self.cli, self.app_name, self.command_name))
 
     @on(Button.Pressed, "#home-exec-button")
     def on_button_pressed(self):
         self.execute_on_exit = True
         self.exit()
 
     def run(
@@ -281,24 +285,24 @@
 
         Args:
             url: The URL to visit.
         """
         open_url(url)
 
 
-def tui(name: str | None = None):
+def tui(name: str | None = None, command: str = "tui", help: str = "Open Textual TUI."):
     def decorator(app: click.Group | click.Command):
         @click.pass_context
         def wrapped_tui(ctx, *args, **kwargs):
-            Trogon(app, app_name=name, click_context=ctx).run()
+            Trogon(app, app_name=name, command_name=command, click_context=ctx).run()
 
         if isinstance(app, click.Group):
-            app.command(name="tui", help="Open Textual TUI.")(wrapped_tui)
+            app.command(name=command, help=help)(wrapped_tui)
         else:
             new_group = click.Group()
             new_group.add_command(app)
-            new_group.command(name="tui", help="Open Textual TUI.")(wrapped_tui)
+            new_group.command(name=command, help=help)(wrapped_tui)
             return new_group
 
         return app
 
     return decorator
```

### Comparing `trogon-0.4.0/trogon/trogon.scss` & `trogon-0.5.0/trogon/trogon.scss`

 * *Files identical despite different names*

### Comparing `trogon-0.4.0/trogon/widgets/about.py` & `trogon-0.5.0/trogon/widgets/about.py`

 * *Files identical despite different names*

### Comparing `trogon-0.4.0/trogon/widgets/command_info.py` & `trogon-0.5.0/trogon/widgets/command_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -86,17 +86,19 @@
                     Tab("Description", id="command-info-text"),
                     Tab("Metadata", id="command-info-metadata"),
                     classes="command-info-tabs",
                 )
                 tabs.focus()
                 yield tabs
 
-            command_info = self.command_schema.docstring
-            if command_info:
-                command_info = command_info.strip()
+            command_info = (
+                self.command_schema.docstring.strip()
+                if self.command_schema.docstring
+                else "No description available"
+            )
 
             with ContentSwitcher(
                 initial="command-info-text", id="command-info-switcher"
             ):
                 yield Static(
                     command_info, id="command-info-text", classes="command-info-text"
                 )
```

### Comparing `trogon-0.4.0/trogon/widgets/command_tree.py` & `trogon-0.5.0/trogon/widgets/command_tree.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,35 +7,36 @@
 
 from trogon.introspect import CommandSchema, CommandName
 
 
 class CommandTree(Tree[CommandSchema]):
     COMPONENT_CLASSES = {"group"}
 
-    def __init__(self, label: TextType, cli_metadata: dict[CommandName, CommandSchema]):
+    def __init__(self, label: TextType, cli_metadata: dict[CommandName, CommandSchema], command_name: str):
         super().__init__(label)
         self.show_root = False
         self.guide_depth = 2
         self.show_guides = False
         self.cli_metadata = cli_metadata
+        self.command_name = command_name
 
     def render_label(
         self, node: TreeNode[TreeDataType], base_style: Style, style: Style
     ) -> Text:
         label = node._label.copy()
         label.stylize(style)
         return label
 
     def on_mount(self):
         def build_tree(
             data: dict[CommandName, CommandSchema], node: TreeNode
         ) -> TreeNode:
             data = {key: data[key] for key in sorted(data)}
             for cmd_name, cmd_data in data.items():
-                if cmd_name == "tui":
+                if cmd_name == self.command_name:
                     continue
                 if cmd_data.subcommands:
                     label = Text(cmd_name)
                     if cmd_data.is_group:
                         group_style = self.get_component_rich_style("group")
                         label.stylize(group_style)
                         label.append(" ")
```

### Comparing `trogon-0.4.0/trogon/widgets/form.py` & `trogon-0.5.0/trogon/widgets/form.py`

 * *Files identical despite different names*

### Comparing `trogon-0.4.0/trogon/widgets/multiple_choice.py` & `trogon-0.5.0/trogon/widgets/multiple_choice.py`

 * *Files identical despite different names*

### Comparing `trogon-0.4.0/trogon/widgets/parameter_controls.py` & `trogon-0.5.0/trogon/widgets/parameter_controls.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
         Args:
             filter_query: The string to filter on.
 
         Returns:
             True if the filter matched (and the widget is visible).
         """
-        help_text = getattr(self.schema, "help", "")
+        help_text = getattr(self.schema, "help", "") or ""
         if not filter_query:
             should_be_visible = True
             self.display = should_be_visible
         else:
             name = self.schema.name
             if isinstance(name, str):
                 # Argument names are strings, there's only one name
@@ -81,15 +81,15 @@
                 should_be_visible = name_contains_query
             else:
                 # Option names are lists since they can have multiple names (e.g. -v and --verbose)
                 name_contains_query = any(
                     filter_query in name.casefold() for name in self.schema.name
                 )
                 help_contains_query = (
-                    filter_query in getattr(self.schema, "help", "").casefold()
+                    filter_query in help_text.casefold()
                 )
                 should_be_visible = name_contains_query or help_contains_query
 
             self.display = should_be_visible
 
         # Update the highlighting of the help text
         if help_text:
```

### Comparing `trogon-0.4.0/PKG-INFO` & `trogon-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trogon
-Version: 0.4.0
+Version: 0.5.0
 Summary: Automatically generate a Textual TUI for your Click CLI
 Home-page: https://github.com/Textualize/trogon
 License: MIT
 Author: Darren Burns
 Author-email: darrenb900@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -133,11 +133,24 @@
     def cli():
         ...
     ```
 3. Your click app will have a new `tui` command available.
 
 See also the `examples` folder for two example apps.
 
+## Custom command name and custom help
+
+By default the command added will be called `tui` and the help text for it will be `Open Textual TUI.`
+
+You can customize one or both of these using the `help=` and `command=` parameters:
+
+```python
+@tui(command="ui", help="Open terminal UI")
+@click.group(...)
+def cli():
+    ...
+```
+
 ## Follow this project
 
 If this app interests you, you may want to join the Textual [Discord server](https://discord.gg/Enf6Z3qhVr) where you can talk to Textual developers / community.
```

