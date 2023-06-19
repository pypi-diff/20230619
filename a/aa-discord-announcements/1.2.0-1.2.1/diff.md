# Comparing `tmp/aa_discord_announcements-1.2.0.tar.gz` & `tmp/aa_discord_announcements-1.2.1.tar.gz`

## Comparing `aa_discord_announcements-1.2.0.tar` & `aa_discord_announcements-1.2.1.tar`

### file list

```diff
@@ -1,59 +1,60 @@
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/__init__.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/admin.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/app_settings.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/apps.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/auth_hooks.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/constants.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/forms.py
--rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/models.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/urls.py
--rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/views.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/helper/announcement_context.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/helper/discord_webhook.py
--rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/django.pot
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4621 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6061 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5383 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/migrations/0001_initial.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/migrations/__init__.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.css
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.min.css
--rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/base.html
--rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/index.html
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-css.html
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-js.html
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/copy-paste-text.html
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/partials/header/page-header.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templatetags/__init__.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/tests/__init__.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_access.py
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_ajax_calls.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_installed_modules.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_models.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_templatetags.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/aa_discord_announcements/tests/utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/LICENSE
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/README.md
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/__init__.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/admin.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/app_settings.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/apps.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/auth_hooks.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/constants.py
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/forms.py
+-rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/models.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/urls.py
+-rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/views.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/helper/announcement_context.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/helper/discord_webhook.py
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/django.pot
+-rw-r--r--   0        0        0     5096 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6792 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4905 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7878 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7064 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5383 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/migrations/0001_initial.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/migrations/0002_translation_updates.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/migrations/__init__.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.css
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.min.css
+-rw-r--r--   0        0        0     6636 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/base.html
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/index.html
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-css.html
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-js.html
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/copy-paste-text.html
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/partials/header/page-header.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templatetags/__init__.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/tests/__init__.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_access.py
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_ajax_calls.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_installed_modules.py
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_models.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/aa_discord_announcements/tests/utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/LICENSE
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/README.md
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 aa_discord_announcements-1.2.1/PKG-INFO
```

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/admin.py` & `aa_discord_announcements-1.2.1/aa_discord_announcements/admin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Settings for the admin backend
 """
 
 # Django
 from django.contrib import admin
+from django.utils.translation import gettext_lazy as _
 
 # AA Discord Announcements
 from aa_discord_announcements.models import PingTarget, Webhook
 
 
 @admin.register(PingTarget)
 class PingTargetAdmin(admin.ModelAdmin):
@@ -24,20 +25,22 @@
     )
 
     filter_horizontal = ("restricted_to_group",)
     readonly_fields = ("discord_id",)
     ordering = ("name",)
 
     @classmethod
-    @admin.display(description="Ping Target", ordering="name")
+    @admin.display(description=_("Group name"), ordering="name")
     def _name(cls, obj):
         return obj.name
 
     @classmethod
-    @admin.display(description="Restricted to", ordering="restricted_to_group__name")
+    @admin.display(
+        description=_("Group restrictions"), ordering="restricted_to_group__name"
+    )
     def _restricted_to_group(cls, obj):
         names = [x.name for x in obj.restricted_to_group.all().order_by("name")]
 
         if names:
             return ", ".join(names)
 
         return None
@@ -51,25 +54,27 @@
 
     list_display = ("_name", "_url", "_restricted_to_group", "notes", "is_enabled")
 
     filter_horizontal = ("restricted_to_group",)
     ordering = ("name",)
 
     @classmethod
-    @admin.display(description="Channel Name", ordering="name")
+    @admin.display(description=_("Discord channel"), ordering="name")
     def _name(cls, obj):
         return obj.name
 
     @classmethod
-    @admin.display(description="Webhook URL", ordering="url")
+    @admin.display(description=_("Webhook URL"), ordering="url")
     def _url(cls, obj):
         return obj.url
 
     @classmethod
-    @admin.display(description="Restricted to", ordering="restricted_to_group__name")
+    @admin.display(
+        description=_("Group restrictions"), ordering="restricted_to_group__name"
+    )
     def _restricted_to_group(cls, obj):
         names = [x.name for x in obj.restricted_to_group.all().order_by("name")]
 
         if names:
             return ", ".join(names)
 
         return None
```

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/auth_hooks.py` & `aa_discord_announcements-1.2.1/aa_discord_announcements/auth_hooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 """
 Hook into AA
 """
 
-# Django
-from django.utils.translation import gettext_lazy as _
-
 # Alliance Auth
 from allianceauth import hooks
 from allianceauth.services.hooks import MenuItemHook, UrlHook
 
 # AA Discord Announcements
 from aa_discord_announcements import __title__, urls
 
@@ -20,15 +17,15 @@
     This class ensures only authorized users will see the menu entry
     """
 
     def __init__(self):
         # setup menu entry for sidebar
         MenuItemHook.__init__(
             self,
-            _(__title__),
+            __title__,
             "far fa-bell fa-fw",
             "aa_discord_announcements:index",
             navactive=["aa_discord_announcements:"],
         )
 
     def render(self, request):
         """
```

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/models.py` & `aa_discord_announcements-1.2.1/aa_discord_announcements/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,28 +30,28 @@
     :type ping_target:
     :return:
     :rtype:
     """
 
     if not discord_service_installed():
         raise ValidationError(
-            _("You might want to install the Discord service first ...")
+            _("You might want to install the Discord service first …")
         )
 
     try:
         discord_group_info = DiscordUser.objects.group_to_role(group=ping_target)
     except HTTPError as http_error:
         raise ValidationError(
             _("Are you sure you have your Discord linked to your Alliance Auth?")
         ) from http_error
-    else:
-        if not discord_group_info:
-            raise ValidationError(_("This group has not been synced to Discord yet."))
 
-        return discord_group_info
+    if not discord_group_info:
+        raise ValidationError(_("This group has not been synced to Discord yet."))
+
+    return discord_group_info
 
 
 class General(models.Model):
     """
     Meta model for app permissions
     """
 
@@ -72,49 +72,54 @@
 
     # Discord group to ping
     name = models.OneToOneField(
         Group,
         related_name="discord_announcement_pingtarget",
         on_delete=models.CASCADE,
         unique=True,
+        verbose_name=_("Group name"),
         help_text=(
             _(
                 "Name of the Discord role to ping. "
                 "(Note: This must be an Auth group that is synced to Discord.)"
             )
         ),
     )
 
     # Discord group id
     discord_id = models.CharField(
         max_length=255,
         unique=True,
         blank=True,
+        verbose_name=_("Discord ID"),
         help_text=_("ID of the Discord role to ping"),
     )
 
     # Restrictions
     restricted_to_group = models.ManyToManyField(
         Group,
         blank=True,
         related_name="discord_announcement_pingtarget_required_groups",
-        help_text=_("Restrict ping rights to the following group(s) ..."),
+        verbose_name=_("Group restrictions"),
+        help_text=_("Restrict ping rights to the following group(s) …"),
     )
 
     # Notes
     notes = models.TextField(
         default="",
         blank=True,
+        verbose_name=_("Notes"),
         help_text=_("You can add notes about this configuration here if you want"),
     )
 
-    # Is this group active
+    # Is this group active?
     is_enabled = models.BooleanField(
         default=True,
         db_index=True,
+        verbose_name=_("Is enabled"),
         help_text=_("Whether this ping target is enabled or not"),
     )
 
     class Meta:  # pylint: disable=too-few-public-methods
         """
         DiscordPingTargets :: Meta
         """
@@ -156,48 +161,53 @@
     A Discord webhook
     """
 
     # Channel name
     name = models.CharField(
         max_length=255,
         unique=True,
+        verbose_name=_("Discord channel"),
         help_text=_("Name of the channel this webhook posts to"),
     )
 
     # Wehbook url
     url = models.CharField(
         max_length=255,
         unique=True,
+        verbose_name=_("Webhook URL"),
         help_text=(
             _(
                 "URL of this webhook, e.g. "
                 "https://discord.com/api/webhooks/123456/abcdef"
             )
         ),
     )
 
     # Restrictions
     restricted_to_group = models.ManyToManyField(
         Group,
         blank=True,
         related_name="discord_announcement_webhook_required_groups",
-        help_text=_("Restrict ping rights to the following group(s) ..."),
+        verbose_name=_("Group restrictions"),
+        help_text=_("Restrict ping rights to the following group(s) …"),
     )
 
     # Webhook notes
     notes = models.TextField(
         default="",
         blank=True,
+        verbose_name=_("Notes"),
         help_text=_("You can add notes about this webhook here if you want"),
     )
 
-    # Is it enabled
+    # Is it enabled?
     is_enabled = models.BooleanField(
         default=True,
         db_index=True,
+        verbose_name=_("Is enabled"),
         help_text=_("Whether this webhook is active or not"),
     )
 
     class Meta:  # pylint: disable=too-few-public-methods
         """
         Webhook :: Meta
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/urls.py` & `aa_discord_announcements-1.2.1/aa_discord_announcements/urls.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/views.py` & `aa_discord_announcements-1.2.1/aa_discord_announcements/views.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/helper/announcement_context.py` & `aa_discord_announcements-1.2.1/aa_discord_announcements/helper/announcement_context.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/helper/discord_webhook.py` & `aa_discord_announcements-1.2.1/aa_discord_announcements/helper/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/django.pot` & `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/django.pot`

 * *Files 8% similar despite different names*

```diff
@@ -4,138 +4,157 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-19 01:15+0200\n"
+"POT-Creation-Date: 2023-06-19 12:12+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: forms.py:20
-msgid "This field is mandatory"
+#: __init__.py:12 templates/aa_discord_announcements/base.html:5
+#: templates/aa_discord_announcements/base.html:8
+msgid "Discord Announcements"
+msgstr ""
+
+#: admin.py:32 models.py:79
+msgid "Group name"
 msgstr ""
 
-#: forms.py:41
-msgid "Discord Markdown"
+#: admin.py:38 admin.py:72 models.py:102 models.py:190
+msgid "Group restrictions"
 msgstr ""
 
-#: forms.py:48
-#, python-brace-format
-msgid "Hint: You can use {discord_markdown_link} to format the text."
+#: admin.py:61 models.py:168
+msgid "Discord channel"
+msgstr ""
+
+#: admin.py:66 models.py:176
+msgid "Webhook URL"
+msgstr ""
+
+#: forms.py:20
+msgid "This field is mandatory"
 msgstr ""
 
-#: forms.py:58
+#: forms.py:37
 msgid "Announcement Target"
 msgstr ""
 
-#: forms.py:60
+#: forms.py:39
 msgid "Who do you want to ping?"
 msgstr ""
 
-#: forms.py:64
+#: forms.py:43
 msgid "Announcement Channel"
 msgstr ""
 
-#: forms.py:66
+#: forms.py:45
 msgid "Select a channel to send the announcement to automatically."
 msgstr ""
 
-#: forms.py:70
+#: forms.py:49
 msgid "Announcement Text"
 msgstr ""
 
-#: forms.py:76
-msgid "Your announcement…"
+#: forms.py:55
+msgid "Your announcement …"
 msgstr ""
 
 #: models.py:37
-msgid "You might want to install the Discord service first ..."
+msgid "You might want to install the Discord service first …"
 msgstr ""
 
 #: models.py:44
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 
 #: models.py:48
 msgid "This group has not been synced to Discord yet."
 msgstr ""
 
-#: models.py:81
+#: models.py:82
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 
-#: models.py:92
+#: models.py:93
+msgid "Discord ID"
+msgstr ""
+
+#: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr ""
 
-#: models.py:100 models.py:183
-msgid "Restrict ping rights to the following group(s) ..."
+#: models.py:103 models.py:191
+msgid "Restrict ping rights to the following group(s) …"
 msgstr ""
 
-#: models.py:107
+#: models.py:110 models.py:198
+msgid "Notes"
+msgstr ""
+
+#: models.py:111
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 
-#: models.py:114
+#: models.py:118 models.py:206
+msgid "Is enabled"
+msgstr ""
+
+#: models.py:119
 msgid "Whether this ping target is enabled or not"
 msgstr ""
 
-#: models.py:122
+#: models.py:127
 msgid "Discord Ping Target"
 msgstr ""
 
-#: models.py:123
+#: models.py:128
 msgid "Discord Ping Targets"
 msgstr ""
 
-#: models.py:163
+#: models.py:169
 msgid "Name of the channel this webhook posts to"
 msgstr ""
 
-#: models.py:172
+#: models.py:179
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 
-#: models.py:190
+#: models.py:199
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 
-#: models.py:197
+#: models.py:207
 msgid "Whether this webhook is active or not"
 msgstr ""
 
-#: models.py:205
+#: models.py:215
 msgid "Webhook"
 msgstr ""
 
-#: models.py:206
+#: models.py:216
 msgid "Webhooks"
 msgstr ""
 
-#: models.py:222
+#: models.py:232
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
-msgid "Discord Announcements"
-msgstr ""
-
 #: templates/aa_discord_announcements/index.html:10
 msgid "Announcement Details"
 msgstr ""
 
 #: templates/aa_discord_announcements/index.html:21
 msgid "Formatted Announcement Text"
 msgstr ""
@@ -153,15 +172,15 @@
 msgstr ""
 
 #: templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
-msgid "No announcement created yet ..."
+msgid "No announcement created yet …"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/form/form.html:27
```

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,27 +7,27 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-discord-announcements/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16.4\n"
+"X-Generator: Weblate 4.18\n"
 
 msgid "Additionally configured announcement targets"
-msgstr "Zusätzlich konfigurierte Ping Ziele"
+msgstr "Zusätzlich konfigurierte Ankündigungsziele"
 
 msgid "Announcement Channel"
-msgstr "Kanal"
+msgstr "Ankündigungskanal"
 
 msgid "Announcement Details"
 msgstr "Ankündigung Details"
 
 msgid "Announcement Target"
-msgstr "Ping"
+msgstr "Ankündigungsziel"
 
 msgid "Announcement Text"
 msgstr "Ankündigungstext"
 
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 "Bist Du sicher das Du Deinen Discord Server mit Alliance Auth verbunden hast?"
@@ -35,24 +35,27 @@
 msgid "Copy Announcement Text"
 msgstr "Kopiere Ankündigungstext"
 
 msgid "Create Announcement"
 msgstr "Ankündigung erstellen"
 
 msgid "Discord Announcements"
-msgstr "Discord Ankündigungen"
+msgstr "Discord-Ankündigungen"
 
-msgid "Discord Markdown"
-msgstr "Discord Markdown"
+msgid "Discord ID"
+msgstr "Discord ID"
 
 msgid "Discord Ping Target"
-msgstr "Discord Ping Ziel"
+msgstr "Discord Pingziel"
 
 msgid "Discord Ping Targets"
-msgstr "Discord Ping Ziele"
+msgstr "Discord Pingziele"
+
+msgid "Discord channel"
+msgstr "Discord-Kanal"
 
 msgid "Don't Ping"
 msgstr "Kein Ping"
 
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
@@ -62,29 +65,34 @@
 
 msgid "Form invalid. Please check your input."
 msgstr "Formular ungültig. Bitte die Angaben prüfen."
 
 msgid "Formatted Announcement Text"
 msgstr "Formatierter Text der Ankündigung"
 
-msgid "Hint: You can use {discord_markdown_link} to format the text."
-msgstr ""
-"Hinweis: Du kannst {discord_markdown_link} nutzen um den Text zu formatieren."
+msgid "Group name"
+msgstr "Gruppenname"
+
+msgid "Group restrictions"
+msgstr "Gruppenbeschränkungen"
 
 msgid "ID of the Discord role to ping"
 msgstr "ID der Discord Rolle zum Pingen"
 
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 "Ungültige Webhook-URL. Die eingegebene Webhook-URL stimmt mit keinem "
 "bekannten Format für einen Discord-Webhook überein. Bitte überprüfe die "
 "Webhook-URL."
 
+msgid "Is enabled"
+msgstr "Ist aktiviert"
+
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement Text"
 msgstr ""
 "Pflichtangaben fehlen.<br>Um eine Ankündigung zu erstellen, müssen folgende "
 "Felder ausgefüllt sein:<br>» Ankündigungstext"
 
@@ -94,25 +102,28 @@
 msgstr ""
 "Name der Discord Rolle zum Pingen. (Hinweis: Dies muss eine Auth Gruppe sein "
 "die zu Discord synchronisiert wurde.)"
 
 msgid "Name of the channel this webhook posts to"
 msgstr "Name des Kanals in dem dieser Webhook postet"
 
-msgid "No announcement created yet ..."
+msgid "No announcement created yet …"
 msgstr "Noch keine Ankündigung erstellt …"
 
 msgid "No form data submitted."
 msgstr "Keine Formulardaten übermittelt."
 
 msgid "None, just format it for me"
 msgstr "Keiner, einfach nur den Text formatieren"
 
-msgid "Restrict ping rights to the following group(s) ..."
-msgstr "Beschränkt die Ping-Rechte auf die folgende(n) Gruppe(n) ..."
+msgid "Notes"
+msgstr "Notizen"
+
+msgid "Restrict ping rights to the following group(s) …"
+msgstr "Beschränkt die Ping-Rechte auf die folgende(n) Gruppe(n) …"
 
 msgid "Select a channel to send the announcement to automatically."
 msgstr "Wähle einen Kanal in dem die Ankündigung gesendet werden soll."
 
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr "Erfolg! Der Ankündigungstext wurde in die Zwischenablage kopiert."
 
@@ -126,19 +137,22 @@
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 "URL des Webhooks, z. B.: https://discord.com/api/webhooks/123456/abcdef"
 
 msgid "Webhook"
 msgstr "Webhook"
 
+msgid "Webhook URL"
+msgstr "Webhook URL"
+
 msgid "Webhooks"
 msgstr "Webhooks"
 
 msgid "Whether this ping target is enabled or not"
-msgstr "Ist dieses Ping Ziel aktiv oder nicht"
+msgstr "Ist dieses Pingziel aktiv oder nicht"
 
 msgid "Whether this webhook is active or not"
 msgstr "Ist dieser Webhook aktiv oder nicht"
 
 msgid "Who do you want to ping?"
 msgstr "Wen möchtest Du pingen?"
 
@@ -147,12 +161,12 @@
 "Wenn Du möchtest, kannst Du hier Anmerkungen zu dieser Konfiguration "
 "hinzufügen"
 
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 "Wenn Du möchtest, kannst Du hier Anmerkungen zu diesem Webhook hinzufügen"
 
-msgid "You might want to install the Discord service first ..."
+msgid "You might want to install the Discord service first …"
 msgstr "Du solltest zunächst den Discord Service installieren …"
 
-msgid "Your announcement…"
+msgid "Your announcement …"
 msgstr "Deine Ankündigung …"
```

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/de/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -2,151 +2,170 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-11 23:21+0200\n"
-"PO-Revision-Date: 2023-04-11 21:42+0000\n"
-"Last-Translator: \"H. Peter Pfeufer\" <info@ppfeufer.de>\n"
+"POT-Creation-Date: 2023-06-19 12:12+0200\n"
+"PO-Revision-Date: 2023-06-19 10:18+0000\n"
+"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: German <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-discord-announcements/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.16.4\n"
+"X-Generator: Weblate 4.18\n"
+
+#: __init__.py:12 templates/aa_discord_announcements/base.html:5
+#: templates/aa_discord_announcements/base.html:8
+msgid "Discord Announcements"
+msgstr "Discord-Ankündigungen"
+
+#: admin.py:32 models.py:79
+msgid "Group name"
+msgstr "Gruppenname"
+
+#: admin.py:38 admin.py:72 models.py:102 models.py:190
+msgid "Group restrictions"
+msgstr "Gruppenbeschränkungen"
+
+#: admin.py:61 models.py:168
+msgid "Discord channel"
+msgstr "Discord-Kanal"
+
+#: admin.py:66 models.py:176
+msgid "Webhook URL"
+msgstr "Webhook URL"
 
 #: forms.py:20
 msgid "This field is mandatory"
 msgstr "Dies ist ein Pflichtfeld"
 
-#: forms.py:41
-msgid "Discord Markdown"
-msgstr "Discord Markdown"
-
-#: forms.py:48
-#, python-brace-format
-msgid "Hint: You can use {discord_markdown_link} to format the text."
-msgstr ""
-"Hinweis: Du kannst {discord_markdown_link} nutzen um den Text zu formatieren."
-
-#: forms.py:58
+#: forms.py:37
 msgid "Announcement Target"
-msgstr "Ping"
+msgstr "Ankündigungsziel"
 
-#: forms.py:60
+#: forms.py:39
 msgid "Who do you want to ping?"
 msgstr "Wen möchtest Du pingen?"
 
-#: forms.py:64
+#: forms.py:43
 msgid "Announcement Channel"
-msgstr "Kanal"
+msgstr "Ankündigungskanal"
 
-#: forms.py:66
+#: forms.py:45
 msgid "Select a channel to send the announcement to automatically."
 msgstr "Wähle einen Kanal in dem die Ankündigung gesendet werden soll."
 
-#: forms.py:70
+#: forms.py:49
 msgid "Announcement Text"
 msgstr "Ankündigungstext"
 
-#: forms.py:76
-msgid "Your announcement…"
+#: forms.py:55
+msgid "Your announcement …"
 msgstr "Deine Ankündigung …"
 
 #: models.py:37
-msgid "You might want to install the Discord service first ..."
+msgid "You might want to install the Discord service first …"
 msgstr "Du solltest zunächst den Discord Service installieren …"
 
 #: models.py:44
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 "Bist Du sicher das Du Deinen Discord Server mit Alliance Auth verbunden hast?"
 
 #: models.py:48
 msgid "This group has not been synced to Discord yet."
 msgstr "Diese Gruppe wurde bisher noch nicht zu Discord synchronisiert."
 
-#: models.py:81
+#: models.py:82
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 "Name der Discord Rolle zum Pingen. (Hinweis: Dies muss eine Auth Gruppe sein "
 "die zu Discord synchronisiert wurde.)"
 
-#: models.py:92
+#: models.py:93
+msgid "Discord ID"
+msgstr "Discord ID"
+
+#: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr "ID der Discord Rolle zum Pingen"
 
-#: models.py:100 models.py:183
-msgid "Restrict ping rights to the following group(s) ..."
-msgstr "Beschränkt die Ping-Rechte auf die folgende(n) Gruppe(n) ..."
+#: models.py:103 models.py:191
+msgid "Restrict ping rights to the following group(s) …"
+msgstr "Beschränkt die Ping-Rechte auf die folgende(n) Gruppe(n) …"
+
+#: models.py:110 models.py:198
+msgid "Notes"
+msgstr "Notizen"
 
-#: models.py:107
+#: models.py:111
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 "Wenn Du möchtest, kannst Du hier Anmerkungen zu dieser Konfiguration "
 "hinzufügen"
 
-#: models.py:114
+#: models.py:118 models.py:206
+msgid "Is enabled"
+msgstr "Ist aktiviert"
+
+#: models.py:119
 msgid "Whether this ping target is enabled or not"
-msgstr "Ist dieses Ping Ziel aktiv oder nicht"
+msgstr "Ist dieses Pingziel aktiv oder nicht"
 
-#: models.py:122
+#: models.py:127
 msgid "Discord Ping Target"
-msgstr "Discord Ping Ziel"
+msgstr "Discord Pingziel"
 
-#: models.py:123
+#: models.py:128
 msgid "Discord Ping Targets"
-msgstr "Discord Ping Ziele"
+msgstr "Discord Pingziele"
 
-#: models.py:163
+#: models.py:169
 msgid "Name of the channel this webhook posts to"
 msgstr "Name des Kanals in dem dieser Webhook postet"
 
-#: models.py:172
+#: models.py:179
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
-msgstr "URL des Webhooks, z. B.: https://discord.com/api/webhooks/123456/abcdef"
+msgstr ""
+"URL des Webhooks, z. B.: https://discord.com/api/webhooks/123456/abcdef"
 
-#: models.py:190
+#: models.py:199
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 "Wenn Du möchtest, kannst Du hier Anmerkungen zu diesem Webhook hinzufügen"
 
-#: models.py:197
+#: models.py:207
 msgid "Whether this webhook is active or not"
 msgstr "Ist dieser Webhook aktiv oder nicht"
 
-#: models.py:205
+#: models.py:215
 msgid "Webhook"
 msgstr "Webhook"
 
-#: models.py:206
+#: models.py:216
 msgid "Webhooks"
 msgstr "Webhooks"
 
-#: models.py:222
+#: models.py:232
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 "Ungültige Webhook-URL. Die eingegebene Webhook-URL stimmt mit keinem "
 "bekannten Format für einen Discord-Webhook überein. Bitte überprüfe die "
 "Webhook-URL."
 
-#: templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
-msgid "Discord Announcements"
-msgstr "Discord Ankündigungen"
-
 #: templates/aa_discord_announcements/index.html:10
 msgid "Announcement Details"
 msgstr "Ankündigung Details"
 
 #: templates/aa_discord_announcements/index.html:21
 msgid "Formatted Announcement Text"
 msgstr "Formatierter Text der Ankündigung"
@@ -168,15 +187,15 @@
 "Möglicherweise unterstützt Dein Browser diese Funktion nicht."
 
 #: templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr "Erfolg! Der Ankündigungstext wurde in die Zwischenablage kopiert."
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
-msgid "No announcement created yet ..."
+msgid "No announcement created yet …"
 msgstr "Noch keine Ankündigung erstellt …"
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr "Kopiere Ankündigungstext"
 
 #: templates/aa_discord_announcements/partials/form/form.html:27
@@ -189,15 +208,15 @@
 
 #: templates/aa_discord_announcements/partials/form/segments/announcement-targets.html:3
 msgid "Don't Ping"
 msgstr "Kein Ping"
 
 #: templates/aa_discord_announcements/partials/form/segments/announcement-targets.html:9
 msgid "Additionally configured announcement targets"
-msgstr "Zusätzlich konfigurierte Ping Ziele"
+msgstr "Zusätzlich konfigurierte Ankündigungsziele"
 
 #: views.py:154
 msgid "Form invalid. Please check your input."
 msgstr "Formular ungültig. Bitte die Angaben prüfen."
 
 #: views.py:156
 msgid "No form data submitted."
```

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/es/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/es/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -2,141 +2,160 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-11 23:21+0200\n"
+"POT-Creation-Date: 2023-06-19 12:12+0200\n"
 "PO-Revision-Date: 2023-04-18 23:17+0000\n"
 "Last-Translator: \"H. Peter Pfeufer\" <info@ppfeufer.de>\n"
-"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-discord-announcements/es/>\n"
-"Language: es\n"
+"Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-discord-announcements/fr/>\n"
+"Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"Plural-Forms: nplurals=2; plural=n > 1;\n"
 "X-Generator: Weblate 4.16.4\n"
 
-#: forms.py:20
-msgid "This field is mandatory"
-msgstr "Este campo es obligatorio"
+#: __init__.py:12 templates/aa_discord_announcements/base.html:5
+#: templates/aa_discord_announcements/base.html:8
+msgid "Discord Announcements"
+msgstr ""
 
-#: forms.py:41
-msgid "Discord Markdown"
+#: admin.py:32 models.py:79
+msgid "Group name"
 msgstr ""
 
-#: forms.py:48
-#, python-brace-format
-msgid "Hint: You can use {discord_markdown_link} to format the text."
+#: admin.py:38 admin.py:72 models.py:102 models.py:190
+msgid "Group restrictions"
 msgstr ""
 
-#: forms.py:58
+#: admin.py:61 models.py:168
+msgid "Discord channel"
+msgstr ""
+
+#: admin.py:66 models.py:176
+msgid "Webhook URL"
+msgstr ""
+
+#: forms.py:20
+msgid "This field is mandatory"
+msgstr "Ce champ est obligatoire"
+
+#: forms.py:37
 msgid "Announcement Target"
 msgstr ""
 
-#: forms.py:60
+#: forms.py:39
 msgid "Who do you want to ping?"
 msgstr ""
 
-#: forms.py:64
+#: forms.py:43
 msgid "Announcement Channel"
 msgstr ""
 
-#: forms.py:66
+#: forms.py:45
 msgid "Select a channel to send the announcement to automatically."
 msgstr ""
 
-#: forms.py:70
+#: forms.py:49
 msgid "Announcement Text"
 msgstr ""
 
-#: forms.py:76
-msgid "Your announcement…"
+#: forms.py:55
+msgid "Your announcement …"
 msgstr ""
 
 #: models.py:37
-msgid "You might want to install the Discord service first ..."
+msgid "You might want to install the Discord service first …"
 msgstr ""
 
 #: models.py:44
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 
 #: models.py:48
 msgid "This group has not been synced to Discord yet."
 msgstr ""
 
-#: models.py:81
+#: models.py:82
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 
-#: models.py:92
+#: models.py:93
+msgid "Discord ID"
+msgstr ""
+
+#: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr ""
 
-#: models.py:100 models.py:183
-msgid "Restrict ping rights to the following group(s) ..."
+#: models.py:103 models.py:191
+msgid "Restrict ping rights to the following group(s) …"
 msgstr ""
 
-#: models.py:107
+#: models.py:110 models.py:198
+msgid "Notes"
+msgstr ""
+
+#: models.py:111
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 
-#: models.py:114
+#: models.py:118 models.py:206
+msgid "Is enabled"
+msgstr ""
+
+#: models.py:119
 msgid "Whether this ping target is enabled or not"
 msgstr ""
 
-#: models.py:122
+#: models.py:127
 msgid "Discord Ping Target"
 msgstr ""
 
-#: models.py:123
+#: models.py:128
 msgid "Discord Ping Targets"
 msgstr ""
 
-#: models.py:163
+#: models.py:169
 msgid "Name of the channel this webhook posts to"
 msgstr ""
 
-#: models.py:172
+#: models.py:179
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 
-#: models.py:190
+#: models.py:199
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 
-#: models.py:197
+#: models.py:207
 msgid "Whether this webhook is active or not"
 msgstr ""
 
-#: models.py:205
+#: models.py:215
 msgid "Webhook"
 msgstr ""
 
-#: models.py:206
+#: models.py:216
 msgid "Webhooks"
 msgstr ""
 
-#: models.py:222
+#: models.py:232
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
-msgid "Discord Announcements"
-msgstr ""
-
 #: templates/aa_discord_announcements/index.html:10
 msgid "Announcement Details"
 msgstr ""
 
 #: templates/aa_discord_announcements/index.html:21
 msgid "Formatted Announcement Text"
 msgstr ""
@@ -154,15 +173,15 @@
 msgstr ""
 
 #: templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
-msgid "No announcement created yet ..."
+msgid "No announcement created yet …"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/form/form.html:27
```

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/es/LC_MESSAGES/django.po`

 * *Files 13% similar despite different names*

```diff
@@ -2,141 +2,160 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-11 23:21+0200\n"
+"POT-Creation-Date: 2023-06-19 12:12+0200\n"
 "PO-Revision-Date: 2023-04-18 23:17+0000\n"
 "Last-Translator: \"H. Peter Pfeufer\" <info@ppfeufer.de>\n"
-"Language-Team: French <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-discord-announcements/fr/>\n"
-"Language: fr_FR\n"
+"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-discord-announcements/es/>\n"
+"Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.16.4\n"
 
-#: forms.py:20
-msgid "This field is mandatory"
-msgstr "Ce champ est obligatoire"
+#: __init__.py:12 templates/aa_discord_announcements/base.html:5
+#: templates/aa_discord_announcements/base.html:8
+msgid "Discord Announcements"
+msgstr ""
 
-#: forms.py:41
-msgid "Discord Markdown"
+#: admin.py:32 models.py:79
+msgid "Group name"
 msgstr ""
 
-#: forms.py:48
-#, python-brace-format
-msgid "Hint: You can use {discord_markdown_link} to format the text."
+#: admin.py:38 admin.py:72 models.py:102 models.py:190
+msgid "Group restrictions"
 msgstr ""
 
-#: forms.py:58
+#: admin.py:61 models.py:168
+msgid "Discord channel"
+msgstr ""
+
+#: admin.py:66 models.py:176
+msgid "Webhook URL"
+msgstr ""
+
+#: forms.py:20
+msgid "This field is mandatory"
+msgstr "Este campo es obligatorio"
+
+#: forms.py:37
 msgid "Announcement Target"
 msgstr ""
 
-#: forms.py:60
+#: forms.py:39
 msgid "Who do you want to ping?"
 msgstr ""
 
-#: forms.py:64
+#: forms.py:43
 msgid "Announcement Channel"
 msgstr ""
 
-#: forms.py:66
+#: forms.py:45
 msgid "Select a channel to send the announcement to automatically."
 msgstr ""
 
-#: forms.py:70
+#: forms.py:49
 msgid "Announcement Text"
 msgstr ""
 
-#: forms.py:76
-msgid "Your announcement…"
+#: forms.py:55
+msgid "Your announcement …"
 msgstr ""
 
 #: models.py:37
-msgid "You might want to install the Discord service first ..."
+msgid "You might want to install the Discord service first …"
 msgstr ""
 
 #: models.py:44
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 
 #: models.py:48
 msgid "This group has not been synced to Discord yet."
 msgstr ""
 
-#: models.py:81
+#: models.py:82
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 
-#: models.py:92
+#: models.py:93
+msgid "Discord ID"
+msgstr ""
+
+#: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr ""
 
-#: models.py:100 models.py:183
-msgid "Restrict ping rights to the following group(s) ..."
+#: models.py:103 models.py:191
+msgid "Restrict ping rights to the following group(s) …"
 msgstr ""
 
-#: models.py:107
+#: models.py:110 models.py:198
+msgid "Notes"
+msgstr ""
+
+#: models.py:111
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 
-#: models.py:114
+#: models.py:118 models.py:206
+msgid "Is enabled"
+msgstr ""
+
+#: models.py:119
 msgid "Whether this ping target is enabled or not"
 msgstr ""
 
-#: models.py:122
+#: models.py:127
 msgid "Discord Ping Target"
 msgstr ""
 
-#: models.py:123
+#: models.py:128
 msgid "Discord Ping Targets"
 msgstr ""
 
-#: models.py:163
+#: models.py:169
 msgid "Name of the channel this webhook posts to"
 msgstr ""
 
-#: models.py:172
+#: models.py:179
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 
-#: models.py:190
+#: models.py:199
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 
-#: models.py:197
+#: models.py:207
 msgid "Whether this webhook is active or not"
 msgstr ""
 
-#: models.py:205
+#: models.py:215
 msgid "Webhook"
 msgstr ""
 
-#: models.py:206
+#: models.py:216
 msgid "Webhooks"
 msgstr ""
 
-#: models.py:222
+#: models.py:232
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
-msgid "Discord Announcements"
-msgstr ""
-
 #: templates/aa_discord_announcements/index.html:10
 msgid "Announcement Details"
 msgstr ""
 
 #: templates/aa_discord_announcements/index.html:21
 msgid "Formatted Announcement Text"
 msgstr ""
@@ -154,15 +173,15 @@
 msgstr ""
 
 #: templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
-msgid "No announcement created yet ..."
+msgid "No announcement created yet …"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/form/form.html:27
```

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -2,141 +2,160 @@
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-11 23:21+0200\n"
+"POT-Creation-Date: 2023-06-19 12:12+0200\n"
 "PO-Revision-Date: 2023-04-18 23:17+0000\n"
 "Last-Translator: \"H. Peter Pfeufer\" <info@ppfeufer.de>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-discord-announcements/it/>\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-discord-announcements/it/>\n"
 "Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.16.4\n"
 
-#: forms.py:20
-msgid "This field is mandatory"
-msgstr "Questo campo è obbligatorio"
+#: __init__.py:12 templates/aa_discord_announcements/base.html:5
+#: templates/aa_discord_announcements/base.html:8
+msgid "Discord Announcements"
+msgstr ""
 
-#: forms.py:41
-msgid "Discord Markdown"
+#: admin.py:32 models.py:79
+msgid "Group name"
 msgstr ""
 
-#: forms.py:48
-#, python-brace-format
-msgid "Hint: You can use {discord_markdown_link} to format the text."
+#: admin.py:38 admin.py:72 models.py:102 models.py:190
+msgid "Group restrictions"
 msgstr ""
 
-#: forms.py:58
+#: admin.py:61 models.py:168
+msgid "Discord channel"
+msgstr ""
+
+#: admin.py:66 models.py:176
+msgid "Webhook URL"
+msgstr ""
+
+#: forms.py:20
+msgid "This field is mandatory"
+msgstr "Questo campo è obbligatorio"
+
+#: forms.py:37
 msgid "Announcement Target"
 msgstr ""
 
-#: forms.py:60
+#: forms.py:39
 msgid "Who do you want to ping?"
 msgstr ""
 
-#: forms.py:64
+#: forms.py:43
 msgid "Announcement Channel"
 msgstr ""
 
-#: forms.py:66
+#: forms.py:45
 msgid "Select a channel to send the announcement to automatically."
 msgstr ""
 
-#: forms.py:70
+#: forms.py:49
 msgid "Announcement Text"
 msgstr ""
 
-#: forms.py:76
-msgid "Your announcement…"
+#: forms.py:55
+msgid "Your announcement …"
 msgstr ""
 
 #: models.py:37
-msgid "You might want to install the Discord service first ..."
+msgid "You might want to install the Discord service first …"
 msgstr ""
 
 #: models.py:44
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 
 #: models.py:48
 msgid "This group has not been synced to Discord yet."
 msgstr ""
 
-#: models.py:81
+#: models.py:82
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 
-#: models.py:92
+#: models.py:93
+msgid "Discord ID"
+msgstr ""
+
+#: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr ""
 
-#: models.py:100 models.py:183
-msgid "Restrict ping rights to the following group(s) ..."
+#: models.py:103 models.py:191
+msgid "Restrict ping rights to the following group(s) …"
+msgstr ""
+
+#: models.py:110 models.py:198
+msgid "Notes"
 msgstr ""
 
-#: models.py:107
+#: models.py:111
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 
-#: models.py:114
+#: models.py:118 models.py:206
+msgid "Is enabled"
+msgstr ""
+
+#: models.py:119
 msgid "Whether this ping target is enabled or not"
 msgstr ""
 
-#: models.py:122
+#: models.py:127
 msgid "Discord Ping Target"
 msgstr ""
 
-#: models.py:123
+#: models.py:128
 msgid "Discord Ping Targets"
 msgstr ""
 
-#: models.py:163
+#: models.py:169
 msgid "Name of the channel this webhook posts to"
 msgstr ""
 
-#: models.py:172
+#: models.py:179
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 
-#: models.py:190
+#: models.py:199
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 
-#: models.py:197
+#: models.py:207
 msgid "Whether this webhook is active or not"
 msgstr ""
 
-#: models.py:205
+#: models.py:215
 msgid "Webhook"
 msgstr ""
 
-#: models.py:206
+#: models.py:216
 msgid "Webhooks"
 msgstr ""
 
-#: models.py:222
+#: models.py:232
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
-msgid "Discord Announcements"
-msgstr ""
-
 #: templates/aa_discord_announcements/index.html:10
 msgid "Announcement Details"
 msgstr ""
 
 #: templates/aa_discord_announcements/index.html:21
 msgid "Formatted Announcement Text"
 msgstr ""
@@ -154,15 +173,15 @@
 msgstr ""
 
 #: templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
-msgid "No announcement created yet ..."
+msgid "No announcement created yet …"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/form/form.html:27
```

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,139 +4,157 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-11 23:21+0200\n"
+"POT-Creation-Date: 2023-06-19 12:12+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: forms.py:20
-msgid "This field is mandatory"
+#: __init__.py:12 templates/aa_discord_announcements/base.html:5
+#: templates/aa_discord_announcements/base.html:8
+msgid "Discord Announcements"
+msgstr ""
+
+#: admin.py:32 models.py:79
+msgid "Group name"
 msgstr ""
 
-#: forms.py:41
-msgid "Discord Markdown"
+#: admin.py:38 admin.py:72 models.py:102 models.py:190
+msgid "Group restrictions"
 msgstr ""
 
-#: forms.py:48
-#, python-brace-format
-msgid "Hint: You can use {discord_markdown_link} to format the text."
+#: admin.py:61 models.py:168
+msgid "Discord channel"
+msgstr ""
+
+#: admin.py:66 models.py:176
+msgid "Webhook URL"
+msgstr ""
+
+#: forms.py:20
+msgid "This field is mandatory"
 msgstr ""
 
-#: forms.py:58
+#: forms.py:37
 msgid "Announcement Target"
 msgstr ""
 
-#: forms.py:60
+#: forms.py:39
 msgid "Who do you want to ping?"
 msgstr ""
 
-#: forms.py:64
+#: forms.py:43
 msgid "Announcement Channel"
 msgstr ""
 
-#: forms.py:66
+#: forms.py:45
 msgid "Select a channel to send the announcement to automatically."
 msgstr ""
 
-#: forms.py:70
+#: forms.py:49
 msgid "Announcement Text"
 msgstr ""
 
-#: forms.py:76
-msgid "Your announcement…"
+#: forms.py:55
+msgid "Your announcement …"
 msgstr ""
 
 #: models.py:37
-msgid "You might want to install the Discord service first ..."
+msgid "You might want to install the Discord service first …"
 msgstr ""
 
 #: models.py:44
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 
 #: models.py:48
 msgid "This group has not been synced to Discord yet."
 msgstr ""
 
-#: models.py:81
+#: models.py:82
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 
-#: models.py:92
+#: models.py:93
+msgid "Discord ID"
+msgstr ""
+
+#: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr ""
 
-#: models.py:100 models.py:183
-msgid "Restrict ping rights to the following group(s) ..."
+#: models.py:103 models.py:191
+msgid "Restrict ping rights to the following group(s) …"
 msgstr ""
 
-#: models.py:107
+#: models.py:110 models.py:198
+msgid "Notes"
+msgstr ""
+
+#: models.py:111
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 
-#: models.py:114
+#: models.py:118 models.py:206
+msgid "Is enabled"
+msgstr ""
+
+#: models.py:119
 msgid "Whether this ping target is enabled or not"
 msgstr ""
 
-#: models.py:122
+#: models.py:127
 msgid "Discord Ping Target"
 msgstr ""
 
-#: models.py:123
+#: models.py:128
 msgid "Discord Ping Targets"
 msgstr ""
 
-#: models.py:163
+#: models.py:169
 msgid "Name of the channel this webhook posts to"
 msgstr ""
 
-#: models.py:172
+#: models.py:179
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 
-#: models.py:190
+#: models.py:199
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 
-#: models.py:197
+#: models.py:207
 msgid "Whether this webhook is active or not"
 msgstr ""
 
-#: models.py:205
+#: models.py:215
 msgid "Webhook"
 msgstr ""
 
-#: models.py:206
+#: models.py:216
 msgid "Webhooks"
 msgstr ""
 
-#: models.py:222
+#: models.py:232
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
-msgid "Discord Announcements"
-msgstr ""
-
 #: templates/aa_discord_announcements/index.html:10
 msgid "Announcement Details"
 msgstr ""
 
 #: templates/aa_discord_announcements/index.html:21
 msgid "Formatted Announcement Text"
 msgstr ""
@@ -154,15 +172,15 @@
 msgstr ""
 
 #: templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
-msgid "No announcement created yet ..."
+msgid "No announcement created yet …"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/form/form.html:27
```

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -4,138 +4,158 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-11 23:21+0200\n"
+"POT-Creation-Date: 2023-06-19 12:12+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
-#: forms.py:20
-msgid "This field is mandatory"
+#: __init__.py:12 templates/aa_discord_announcements/base.html:5
+#: templates/aa_discord_announcements/base.html:8
+msgid "Discord Announcements"
+msgstr ""
+
+#: admin.py:32 models.py:79
+msgid "Group name"
 msgstr ""
 
-#: forms.py:41
-msgid "Discord Markdown"
+#: admin.py:38 admin.py:72 models.py:102 models.py:190
+msgid "Group restrictions"
 msgstr ""
 
-#: forms.py:48
-#, python-brace-format
-msgid "Hint: You can use {discord_markdown_link} to format the text."
+#: admin.py:61 models.py:168
+msgid "Discord channel"
+msgstr ""
+
+#: admin.py:66 models.py:176
+msgid "Webhook URL"
+msgstr ""
+
+#: forms.py:20
+msgid "This field is mandatory"
 msgstr ""
 
-#: forms.py:58
+#: forms.py:37
 msgid "Announcement Target"
 msgstr ""
 
-#: forms.py:60
+#: forms.py:39
 msgid "Who do you want to ping?"
 msgstr ""
 
-#: forms.py:64
+#: forms.py:43
 msgid "Announcement Channel"
 msgstr ""
 
-#: forms.py:66
+#: forms.py:45
 msgid "Select a channel to send the announcement to automatically."
 msgstr ""
 
-#: forms.py:70
+#: forms.py:49
 msgid "Announcement Text"
 msgstr ""
 
-#: forms.py:76
-msgid "Your announcement…"
+#: forms.py:55
+msgid "Your announcement …"
 msgstr ""
 
 #: models.py:37
-msgid "You might want to install the Discord service first ..."
+msgid "You might want to install the Discord service first …"
 msgstr ""
 
 #: models.py:44
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 
 #: models.py:48
 msgid "This group has not been synced to Discord yet."
 msgstr ""
 
-#: models.py:81
+#: models.py:82
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 
-#: models.py:92
+#: models.py:93
+msgid "Discord ID"
+msgstr ""
+
+#: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr ""
 
-#: models.py:100 models.py:183
-msgid "Restrict ping rights to the following group(s) ..."
+#: models.py:103 models.py:191
+msgid "Restrict ping rights to the following group(s) …"
 msgstr ""
 
-#: models.py:107
+#: models.py:110 models.py:198
+msgid "Notes"
+msgstr ""
+
+#: models.py:111
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 
-#: models.py:114
+#: models.py:118 models.py:206
+msgid "Is enabled"
+msgstr ""
+
+#: models.py:119
 msgid "Whether this ping target is enabled or not"
 msgstr ""
 
-#: models.py:122
+#: models.py:127
 msgid "Discord Ping Target"
 msgstr ""
 
-#: models.py:123
+#: models.py:128
 msgid "Discord Ping Targets"
 msgstr ""
 
-#: models.py:163
+#: models.py:169
 msgid "Name of the channel this webhook posts to"
 msgstr ""
 
-#: models.py:172
+#: models.py:179
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 
-#: models.py:190
+#: models.py:199
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 
-#: models.py:197
+#: models.py:207
 msgid "Whether this webhook is active or not"
 msgstr ""
 
-#: models.py:205
+#: models.py:215
 msgid "Webhook"
 msgstr ""
 
-#: models.py:206
+#: models.py:216
 msgid "Webhooks"
 msgstr ""
 
-#: models.py:222
+#: models.py:232
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
-msgid "Discord Announcements"
-msgstr ""
-
 #: templates/aa_discord_announcements/index.html:10
 msgid "Announcement Details"
 msgstr ""
 
 #: templates/aa_discord_announcements/index.html:21
 msgid "Formatted Announcement Text"
 msgstr ""
@@ -153,15 +173,15 @@
 msgstr ""
 
 #: templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
-msgid "No announcement created yet ..."
+msgid "No announcement created yet …"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/form/form.html:27
```

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-discord-announcements/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 4.16.4\n"
+"X-Generator: Weblate 4.18\n"
 
 msgid "Additionally configured announcement targets"
 msgstr "Дополнительно сконфигурированные цели объявлений"
 
 msgid "Announcement Channel"
 msgstr "Канал объявления"
 
@@ -37,23 +37,26 @@
 
 msgid "Create Announcement"
 msgstr "Создать объявление"
 
 msgid "Discord Announcements"
 msgstr "Объявления Discord"
 
-msgid "Discord Markdown"
-msgstr "Форматирование для Discord"
+msgid "Discord ID"
+msgstr "Идентификатор Discord"
 
 msgid "Discord Ping Target"
 msgstr "Цель пинга Discrod"
 
 msgid "Discord Ping Targets"
 msgstr "Цели пинга Discord"
 
+msgid "Discord channel"
+msgstr "Канал Discord"
+
 msgid "Don't Ping"
 msgstr "Не пингуй"
 
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
@@ -62,29 +65,33 @@
 
 msgid "Form invalid. Please check your input."
 msgstr "Форма некорректна. Проверьте введенные данные."
 
 msgid "Formatted Announcement Text"
 msgstr "Отформатированный текст объявления"
 
-msgid "Hint: You can use {discord_markdown_link} to format the text."
-msgstr ""
-"Подсказка: Вы можете использовать {discord_markdown_link} для форматирования "
-"текста."
+msgid "Group name"
+msgstr "Название группы"
+
+msgid "Group restrictions"
+msgstr "Ограничения групп"
 
 msgid "ID of the Discord role to ping"
 msgstr "ID роли Discord для пинга"
 
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 "Некорректный URL вебхука. Введенный URL не совпадает с известными форматами "
 "вебхуков Discord. Пожалуйста, проверьте URL."
 
+msgid "Is enabled"
+msgstr "Разрешен"
+
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement Text"
 msgstr ""
 "Отсутствует необходимая информация. <br>Для создания объявления необходимо "
 "заполнить следующие поля:<br>» Текст объявления"
 
@@ -94,25 +101,28 @@
 msgstr ""
 "Имя роли Discord для пинга. (Примечание: Это должна быть синхронизированная "
 "с Discord группа Auth.)"
 
 msgid "Name of the channel this webhook posts to"
 msgstr "Название канала, в который вебхук отправляет сообщения"
 
-msgid "No announcement created yet ..."
-msgstr "Объявлений нет..."
+msgid "No announcement created yet …"
+msgstr "Объявлений нет …"
 
 msgid "No form data submitted."
 msgstr "Данные формы не отправлены."
 
 msgid "None, just format it for me"
 msgstr "Нет, только отформатируй"
 
-msgid "Restrict ping rights to the following group(s) ..."
-msgstr "Разрешить пинговать следующим группам..."
+msgid "Notes"
+msgstr "Примечания"
+
+msgid "Restrict ping rights to the following group(s) …"
+msgstr "Разрешить пинговать следующим группам …"
 
 msgid "Select a channel to send the announcement to automatically."
 msgstr "Выберите канал для автоматической отправки объявлений."
 
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr "Успех! Объявление скопировано в буфер обмена."
 
@@ -126,14 +136,17 @@
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 "URL этого вебхука, например https://discord.com/api/webhooks/123456/abcdef"
 
 msgid "Webhook"
 msgstr "Вебхук"
 
+msgid "Webhook URL"
+msgstr "Вебхук URL"
+
 msgid "Webhooks"
 msgstr "Вебхуки"
 
 msgid "Whether this ping target is enabled or not"
 msgstr "Разрешена или нет цель пинга"
 
 msgid "Whether this webhook is active or not"
@@ -144,12 +157,12 @@
 
 msgid "You can add notes about this configuration here if you want"
 msgstr "Здесь Вы можете добавить примечания для этой конфигурации"
 
 msgid "You can add notes about this webhook here if you want"
 msgstr "Здесь Вы можете добавить примечания для этого вебхука"
 
-msgid "You might want to install the Discord service first ..."
-msgstr "Возможно, Вам следует сначала установить сервис Discord..."
+msgid "You might want to install the Discord service first …"
+msgstr "Возможно, Вам следует сначала установить сервис Discord …"
 
-msgid "Your announcement…"
-msgstr "Ваше объявление…"
+msgid "Your announcement …"
+msgstr "Ваше объявление …"
```

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -3,149 +3,166 @@
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
 # Nikolay <nick.postnikov@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-11 23:21+0200\n"
-"PO-Revision-Date: 2023-04-20 21:50+0000\n"
-"Last-Translator: Nikolay <nick.postnikov@gmail.com>\n"
+"POT-Creation-Date: 2023-06-19 12:12+0200\n"
+"PO-Revision-Date: 2023-06-19 10:18+0000\n"
+"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-discord-announcements/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 4.16.4\n"
+"X-Generator: Weblate 4.18\n"
+
+#: __init__.py:12 templates/aa_discord_announcements/base.html:5
+#: templates/aa_discord_announcements/base.html:8
+msgid "Discord Announcements"
+msgstr "Объявления Discord"
+
+#: admin.py:32 models.py:79
+msgid "Group name"
+msgstr "Название группы"
+
+#: admin.py:38 admin.py:72 models.py:102 models.py:190
+msgid "Group restrictions"
+msgstr "Ограничения групп"
+
+#: admin.py:61 models.py:168
+msgid "Discord channel"
+msgstr "Канал Discord"
+
+#: admin.py:66 models.py:176
+msgid "Webhook URL"
+msgstr "Вебхук URL"
 
 #: forms.py:20
 msgid "This field is mandatory"
 msgstr "Обязательное поле"
 
-#: forms.py:41
-msgid "Discord Markdown"
-msgstr "Форматирование для Discord"
-
-#: forms.py:48
-#, python-brace-format
-msgid "Hint: You can use {discord_markdown_link} to format the text."
-msgstr ""
-"Подсказка: Вы можете использовать {discord_markdown_link} для форматирования "
-"текста."
-
-#: forms.py:58
+#: forms.py:37
 msgid "Announcement Target"
 msgstr "Цель объявления"
 
-#: forms.py:60
+#: forms.py:39
 msgid "Who do you want to ping?"
 msgstr "Кого Вы хотите пинговать?"
 
-#: forms.py:64
+#: forms.py:43
 msgid "Announcement Channel"
 msgstr "Канал объявления"
 
-#: forms.py:66
+#: forms.py:45
 msgid "Select a channel to send the announcement to automatically."
 msgstr "Выберите канал для автоматической отправки объявлений."
 
-#: forms.py:70
+#: forms.py:49
 msgid "Announcement Text"
 msgstr "Текст объявления"
 
-#: forms.py:76
-msgid "Your announcement…"
-msgstr "Ваше объявление…"
+#: forms.py:55
+msgid "Your announcement …"
+msgstr "Ваше объявление …"
 
 #: models.py:37
-msgid "You might want to install the Discord service first ..."
-msgstr "Возможно, Вам следует сначала установить сервис Discord..."
+msgid "You might want to install the Discord service first …"
+msgstr "Возможно, Вам следует сначала установить сервис Discord …"
 
 #: models.py:44
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "Вы уверены, что Ваш Discord связан с Вашим Alliance Auth?"
 
 #: models.py:48
 msgid "This group has not been synced to Discord yet."
 msgstr "Эта группа не была синхронизирована с Discord."
 
-#: models.py:81
+#: models.py:82
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 "Имя роли Discord для пинга. (Примечание: Это должна быть синхронизированная "
 "с Discord группа Auth.)"
 
-#: models.py:92
+#: models.py:93
+msgid "Discord ID"
+msgstr "Идентификатор Discord"
+
+#: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr "ID роли Discord для пинга"
 
-#: models.py:100 models.py:183
-msgid "Restrict ping rights to the following group(s) ..."
-msgstr "Разрешить пинговать следующим группам..."
+#: models.py:103 models.py:191
+msgid "Restrict ping rights to the following group(s) …"
+msgstr "Разрешить пинговать следующим группам …"
+
+#: models.py:110 models.py:198
+msgid "Notes"
+msgstr "Примечания"
 
-#: models.py:107
+#: models.py:111
 msgid "You can add notes about this configuration here if you want"
 msgstr "Здесь Вы можете добавить примечания для этой конфигурации"
 
-#: models.py:114
+#: models.py:118 models.py:206
+msgid "Is enabled"
+msgstr "Разрешен"
+
+#: models.py:119
 msgid "Whether this ping target is enabled or not"
 msgstr "Разрешена или нет цель пинга"
 
-#: models.py:122
+#: models.py:127
 msgid "Discord Ping Target"
 msgstr "Цель пинга Discrod"
 
-#: models.py:123
+#: models.py:128
 msgid "Discord Ping Targets"
 msgstr "Цели пинга Discord"
 
-#: models.py:163
+#: models.py:169
 msgid "Name of the channel this webhook posts to"
 msgstr "Название канала, в который вебхук отправляет сообщения"
 
-#: models.py:172
+#: models.py:179
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 "URL этого вебхука, например https://discord.com/api/webhooks/123456/abcdef"
 
-#: models.py:190
+#: models.py:199
 msgid "You can add notes about this webhook here if you want"
 msgstr "Здесь Вы можете добавить примечания для этого вебхука"
 
-#: models.py:197
+#: models.py:207
 msgid "Whether this webhook is active or not"
 msgstr "Активен или нет вебхук"
 
-#: models.py:205
+#: models.py:215
 msgid "Webhook"
 msgstr "Вебхук"
 
-#: models.py:206
+#: models.py:216
 msgid "Webhooks"
 msgstr "Вебхуки"
 
-#: models.py:222
+#: models.py:232
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 "Некорректный URL вебхука. Введенный URL не совпадает с известными форматами "
 "вебхуков Discord. Пожалуйста, проверьте URL."
 
-#: templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
-msgid "Discord Announcements"
-msgstr "Объявления Discord"
-
 #: templates/aa_discord_announcements/index.html:10
 msgid "Announcement Details"
 msgstr "Детали объявления"
 
 #: templates/aa_discord_announcements/index.html:21
 msgid "Formatted Announcement Text"
 msgstr "Отформатированный текст объявления"
@@ -167,16 +184,16 @@
 "не предоставляет такую функциональность."
 
 #: templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr "Успех! Объявление скопировано в буфер обмена."
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
-msgid "No announcement created yet ..."
-msgstr "Объявлений нет..."
+msgid "No announcement created yet …"
+msgstr "Объявлений нет …"
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr "Скопировать текст объявления"
 
 #: templates/aa_discord_announcements/partials/form/form.html:27
 msgid "Create Announcement"
```

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/uk/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/uk/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,18 @@
 "apps/aa-discord-announcements/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 4.16.4\n"
+"X-Generator: Weblate 4.17\n"
+
+msgid "Announcement Text"
+msgstr "Текст оголошення"
 
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "Ви впевнені, що ваш Discord пов'язаний з вашим Alliance Auth?"
 
 msgid "Discord Markdown"
 msgstr "Discord markdown"
 
@@ -60,16 +63,19 @@
 
 msgid "No form data submitted."
 msgstr "Не подано жодних даних."
 
 msgid "None, just format it for me"
 msgstr "Ні, просто відформатуйте для мене"
 
-msgid "Restrict ping rights to the following group(s) ..."
-msgstr "Обмежити права на пінг для наступних груп ..."
+msgid "Restrict ping rights to the following group(s) …"
+msgstr "Обмежити права на пінг для наступних груп …"
+
+msgid "Select a channel to send the announcement to automatically."
+msgstr "Виберіть канал для автоматичного відправлення оголошення."
 
 msgid "This group has not been synced to Discord yet."
 msgstr "Цю групу ще не синхронізовано з Discord."
 
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
@@ -90,9 +96,12 @@
 
 msgid "You can add notes about this configuration here if you want"
 msgstr "Ви можете додати примітки про цю конфігурацію тут, якщо хочете"
 
 msgid "You can add notes about this webhook here if you want"
 msgstr "Ви можете додати примітки про цей вебхук тут, якщо хочете"
 
-msgid "You might want to install the Discord service first ..."
-msgstr "Можливо, ви захочете спочатку встановити службу Discord ..."
+msgid "You might want to install the Discord service first …"
+msgstr "Можливо, ви захочете спочатку встановити службу Discord …"
+
+msgid "Your announcement…"
+msgstr "Ваше оголошення…"
```

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/uk/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/uk/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,153 +1,177 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Kristof <kristof@teh.ninja>, 2023.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
+# "Andrii M." <elfleg0las88@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-19 01:15+0200\n"
-"PO-Revision-Date: 2023-04-20 21:50+0000\n"
-"Last-Translator: \"H. Peter Pfeufer\" <info@ppfeufer.de>\n"
-"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-discord-announcements/uk/>\n"
+"POT-Creation-Date: 2023-06-19 12:12+0200\n"
+"PO-Revision-Date: 2023-06-14 17:18+0000\n"
+"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-discord-announcements/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 4.16.4\n"
+"X-Generator: Weblate 4.17\n"
 
-#: forms.py:20
-msgid "This field is mandatory"
+#: __init__.py:12 templates/aa_discord_announcements/base.html:5
+#: templates/aa_discord_announcements/base.html:8
+msgid "Discord Announcements"
 msgstr ""
 
-#: forms.py:41
-msgid "Discord Markdown"
-msgstr "Discord markdown"
+#: admin.py:32 models.py:79
+msgid "Group name"
+msgstr ""
+
+#: admin.py:38 admin.py:72 models.py:102 models.py:190
+msgid "Group restrictions"
+msgstr ""
+
+#: admin.py:61 models.py:168
+msgid "Discord channel"
+msgstr ""
 
-#: forms.py:48
-#, python-brace-format
-msgid "Hint: You can use {discord_markdown_link} to format the text."
+#: admin.py:66 models.py:176
+#, fuzzy
+#| msgid "Webhook"
+msgid "Webhook URL"
+msgstr "Веб-хук"
+
+#: forms.py:20
+msgid "This field is mandatory"
 msgstr ""
-"Підказка: Ви можете використовувати {discord_markdown_link} для форматування "
-"тексту."
 
-#: forms.py:58
+#: forms.py:37
 msgid "Announcement Target"
 msgstr ""
 
-#: forms.py:60
+#: forms.py:39
 msgid "Who do you want to ping?"
 msgstr "Кого ви хочете пінгувати?"
 
-#: forms.py:64
+#: forms.py:43
 msgid "Announcement Channel"
 msgstr ""
 
-#: forms.py:66
+#: forms.py:45
 msgid "Select a channel to send the announcement to automatically."
-msgstr ""
+msgstr "Виберіть канал для автоматичного відправлення оголошення."
 
-#: forms.py:70
+#: forms.py:49
 msgid "Announcement Text"
-msgstr ""
+msgstr "Текст оголошення"
 
-#: forms.py:76
-msgid "Your announcement…"
-msgstr ""
+#: forms.py:55
+#, fuzzy
+#| msgid "Your announcement…"
+msgid "Your announcement …"
+msgstr "Ваше оголошення…"
 
 #: models.py:37
-msgid "You might want to install the Discord service first ..."
-msgstr "Можливо, ви захочете спочатку встановити службу Discord ..."
+msgid "You might want to install the Discord service first …"
+msgstr "Можливо, ви захочете спочатку встановити службу Discord …"
 
 #: models.py:44
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "Ви впевнені, що ваш Discord пов'язаний з вашим Alliance Auth?"
 
 #: models.py:48
 msgid "This group has not been synced to Discord yet."
 msgstr "Цю групу ще не синхронізовано з Discord."
 
-#: models.py:81
+#: models.py:82
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 "Ім'я ролі Discord, яку потрібно пінгувати. (Примітка: це має бути група "
 "Auth, яка синхронізована з Discord.)"
 
-#: models.py:92
+#: models.py:93
+#, fuzzy
+#| msgid "Discord Markdown"
+msgid "Discord ID"
+msgstr "Discord markdown"
+
+#: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr "Ідентифікатор ролі Discord для пінгування"
 
-#: models.py:100 models.py:183
-msgid "Restrict ping rights to the following group(s) ..."
-msgstr "Обмежити права на пінг для наступних груп ..."
+#: models.py:103 models.py:191
+msgid "Restrict ping rights to the following group(s) …"
+msgstr "Обмежити права на пінг для наступних груп …"
+
+#: models.py:110 models.py:198
+msgid "Notes"
+msgstr ""
 
-#: models.py:107
+#: models.py:111
 msgid "You can add notes about this configuration here if you want"
 msgstr "Ви можете додати примітки про цю конфігурацію тут, якщо хочете"
 
-#: models.py:114
+#: models.py:118 models.py:206
+msgid "Is enabled"
+msgstr ""
+
+#: models.py:119
 msgid "Whether this ping target is enabled or not"
 msgstr ""
 
-#: models.py:122
+#: models.py:127
 msgid "Discord Ping Target"
 msgstr "Ціль для пінгу в Discord"
 
-#: models.py:123
+#: models.py:128
 msgid "Discord Ping Targets"
 msgstr "Цілі для пінгу в Discord"
 
-#: models.py:163
+#: models.py:169
 msgid "Name of the channel this webhook posts to"
 msgstr "Назва каналу, на який публікується цей веб-хук"
 
-#: models.py:172
+#: models.py:179
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
-"URL-адреса цього веб-хука, наприклад, https://discord.com/api/webhooks/"
-"123456/abcdef"
+"URL-адреса цього веб-хука, наприклад, https://discord.com/api/"
+"webhooks/123456/abcdef"
 
-#: models.py:190
+#: models.py:199
 msgid "You can add notes about this webhook here if you want"
 msgstr "Ви можете додати примітки про цей вебхук тут, якщо хочете"
 
-#: models.py:197
+#: models.py:207
 msgid "Whether this webhook is active or not"
 msgstr "Активний цей вебхук чи ні"
 
-#: models.py:205
+#: models.py:215
 msgid "Webhook"
 msgstr "Веб-хук"
 
-#: models.py:206
+#: models.py:216
 msgid "Webhooks"
 msgstr "Веб-хуки"
 
-#: models.py:222
+#: models.py:232
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 "Неправильна URL-адреса веб-хука. Введена вами URL-адреса веб-хука не "
 "відповідає жодному з відомих форматів веб-хуків Discord. Будь ласка, "
 "перевірте URL-адресу веб-хука."
 
-#: templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
-msgid "Discord Announcements"
-msgstr ""
-
 #: templates/aa_discord_announcements/index.html:10
 msgid "Announcement Details"
 msgstr ""
 
 #: templates/aa_discord_announcements/index.html:21
 msgid "Formatted Announcement Text"
 msgstr ""
@@ -165,15 +189,15 @@
 msgstr ""
 
 #: templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
-msgid "No announcement created yet ..."
+msgid "No announcement created yet …"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/form/form.html:27
```

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_discord_announcements-1.2.1/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -4,139 +4,158 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-11 23:21+0200\n"
+"POT-Creation-Date: 2023-06-19 12:12+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
-#: forms.py:20
-msgid "This field is mandatory"
+#: __init__.py:12 templates/aa_discord_announcements/base.html:5
+#: templates/aa_discord_announcements/base.html:8
+msgid "Discord Announcements"
+msgstr ""
+
+#: admin.py:32 models.py:79
+msgid "Group name"
 msgstr ""
 
-#: forms.py:41
-msgid "Discord Markdown"
+#: admin.py:38 admin.py:72 models.py:102 models.py:190
+msgid "Group restrictions"
 msgstr ""
 
-#: forms.py:48
-#, python-brace-format
-msgid "Hint: You can use {discord_markdown_link} to format the text."
+#: admin.py:61 models.py:168
+msgid "Discord channel"
+msgstr ""
+
+#: admin.py:66 models.py:176
+msgid "Webhook URL"
+msgstr ""
+
+#: forms.py:20
+msgid "This field is mandatory"
 msgstr ""
 
-#: forms.py:58
+#: forms.py:37
 msgid "Announcement Target"
 msgstr ""
 
-#: forms.py:60
+#: forms.py:39
 msgid "Who do you want to ping?"
 msgstr ""
 
-#: forms.py:64
+#: forms.py:43
 msgid "Announcement Channel"
 msgstr ""
 
-#: forms.py:66
+#: forms.py:45
 msgid "Select a channel to send the announcement to automatically."
 msgstr ""
 
-#: forms.py:70
+#: forms.py:49
 msgid "Announcement Text"
 msgstr ""
 
-#: forms.py:76
-msgid "Your announcement…"
+#: forms.py:55
+msgid "Your announcement …"
 msgstr ""
 
 #: models.py:37
-msgid "You might want to install the Discord service first ..."
+msgid "You might want to install the Discord service first …"
 msgstr ""
 
 #: models.py:44
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 
 #: models.py:48
 msgid "This group has not been synced to Discord yet."
 msgstr ""
 
-#: models.py:81
+#: models.py:82
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 
-#: models.py:92
+#: models.py:93
+msgid "Discord ID"
+msgstr ""
+
+#: models.py:94
 msgid "ID of the Discord role to ping"
 msgstr ""
 
-#: models.py:100 models.py:183
-msgid "Restrict ping rights to the following group(s) ..."
+#: models.py:103 models.py:191
+msgid "Restrict ping rights to the following group(s) …"
 msgstr ""
 
-#: models.py:107
+#: models.py:110 models.py:198
+msgid "Notes"
+msgstr ""
+
+#: models.py:111
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 
-#: models.py:114
+#: models.py:118 models.py:206
+msgid "Is enabled"
+msgstr ""
+
+#: models.py:119
 msgid "Whether this ping target is enabled or not"
 msgstr ""
 
-#: models.py:122
+#: models.py:127
 msgid "Discord Ping Target"
 msgstr ""
 
-#: models.py:123
+#: models.py:128
 msgid "Discord Ping Targets"
 msgstr ""
 
-#: models.py:163
+#: models.py:169
 msgid "Name of the channel this webhook posts to"
 msgstr ""
 
-#: models.py:172
+#: models.py:179
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 
-#: models.py:190
+#: models.py:199
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 
-#: models.py:197
+#: models.py:207
 msgid "Whether this webhook is active or not"
 msgstr ""
 
-#: models.py:205
+#: models.py:215
 msgid "Webhook"
 msgstr ""
 
-#: models.py:206
+#: models.py:216
 msgid "Webhooks"
 msgstr ""
 
-#: models.py:222
+#: models.py:232
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: templates/aa_discord_announcements/base.html:5
-#: templates/aa_discord_announcements/base.html:8
-msgid "Discord Announcements"
-msgstr ""
-
 #: templates/aa_discord_announcements/index.html:10
 msgid "Announcement Details"
 msgstr ""
 
 #: templates/aa_discord_announcements/index.html:21
 msgid "Formatted Announcement Text"
 msgstr ""
@@ -154,15 +173,15 @@
 msgstr ""
 
 #: templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:5
-msgid "No announcement created yet ..."
+msgid "No announcement created yet …"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/announcement/announcement.html:22
 msgid "Copy Announcement Text"
 msgstr ""
 
 #: templates/aa_discord_announcements/partials/form/form.html:27
```

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/migrations/0001_initial.py` & `aa_discord_announcements-1.2.1/aa_discord_announcements/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js` & `aa_discord_announcements-1.2.1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js` & `aa_discord_announcements-1.2.1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/index.html` & `aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/index.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html` & `aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load i18n %}
 
 <div class="aa-discord-announcements-no-announcement">
     <p>
-        {% translate "No announcement created yet ..." %}
+        {% translate "No announcement created yet …" %}
     </p>
 </div>
 
 <div class="aa-discord-announcements-announcement" style="display: none;">
     <div class="aa-discord-announcements-announcement-text"></div>
 
     <div class="aa-discord-announcements-announcement-copyresult"></div>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html` & `aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html` & `aa_discord_announcements-1.2.1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py` & `aa_discord_announcements-1.2.1/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_access.py` & `aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_ajax_calls.py` & `aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_ajax_calls.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_auth_hooks.py` & `aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_installed_modules.py` & `aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_installed_modules.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_models.py` & `aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,15 @@
 
         # when
         with self.assertRaises(ValidationError):
             announcement_target.clean()
 
         with self.assertRaisesMessage(
             ValidationError,
-            expected_message=(
-                "You might want to install the Discord service first ..."
-            ),
+            expected_message="You might want to install the Discord service first …",
         ):
             announcement_target.clean()
 
     def test_should_raise_validation_error_on_save(self):
         """
         Test should raise validation error on save
         :return:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/tests/test_templatetags.py` & `aa_discord_announcements-1.2.1/aa_discord_announcements/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/aa_discord_announcements/tests/utils.py` & `aa_discord_announcements-1.2.1/aa_discord_announcements/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/LICENSE` & `aa_discord_announcements-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/README.md` & `aa_discord_announcements-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.2.0/pyproject.toml` & `aa_discord_announcements-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aa-discord-announcements"
-version = "1.2.0"
+version = "1.2.1"
 description = "Discord Announcements via Alliance Auth. Write announcements and manage who can write announcements on your corporation or alliance Discord through Alliance Auth."
 readme = "README.md"
 license = "GPL-3.0"
 requires-python = "~=3.8"
 authors = [
     { name = "Peter Pfeufer", email = "develop@ppfeufer.de" },
 ]
```

### Comparing `aa_discord_announcements-1.2.0/PKG-INFO` & `aa_discord_announcements-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-discord-announcements
-Version: 1.2.0
+Version: 1.2.1
 Summary: Discord Announcements via Alliance Auth. Write announcements and manage who can write announcements on your corporation or alliance Discord through Alliance Auth.
 Project-URL: Homepage, https://github.com/ppfeufer/aa-discord-announcements
 Project-URL: Documentation, https://github.com/ppfeufer/aa-discord-announcements/blob/master/README.md
 Project-URL: Source, https://github.com/ppfeufer/aa-discord-announcements.git
 Project-URL: Changelog, https://github.com/ppfeufer/aa-discord-announcements/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://github.com/ppfeufer/aa-discord-announcements/issues
 Author-email: Peter Pfeufer <develop@ppfeufer.de>
```

