# Comparing `tmp/yeref-0.2.0.tar.gz` & `tmp/yeref-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.2.0.tar", last modified: Mon Jun 19 08:14:49 2023, max compression
+gzip compressed data, was "yeref-0.2.1.tar", last modified: Mon Jun 19 18:19:22 2023, max compression
```

## Comparing `yeref-0.2.0.tar` & `yeref-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-19 08:14:49.723598 yeref-0.2.0/
--rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-19 08:14:49.723859 yeref-0.2.0/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-19 08:14:49.725498 yeref-0.2.0/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1390 2023-06-19 08:14:37.000000 yeref-0.2.0/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-19 08:14:49.716182 yeref-0.2.0/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.0/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   557031 2023-06-18 12:52:19.000000 yeref-0.2.0/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   210926 2023-06-19 08:12:39.000000 yeref-0.2.0/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-19 08:14:49.722841 yeref-0.2.0/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-19 08:14:49.000000 yeref-0.2.0/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-19 08:14:49.000000 yeref-0.2.0/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-19 08:14:49.000000 yeref-0.2.0/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-19 08:14:49.000000 yeref-0.2.0/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-19 18:19:22.342320 yeref-0.2.1/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-19 18:19:22.342550 yeref-0.2.1/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-06-19 18:19:22.343498 yeref-0.2.1/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1391 2023-06-19 18:18:30.000000 yeref-0.2.1/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-19 18:19:22.334951 yeref-0.2.1/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.1/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   557022 2023-06-19 17:17:09.000000 yeref-0.2.1/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   210940 2023-06-19 18:18:21.000000 yeref-0.2.1/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-06-19 18:19:22.341692 yeref-0.2.1/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       84 2023-06-19 18:19:22.000000 yeref-0.2.1/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-06-19 18:19:22.000000 yeref-0.2.1/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-06-19 18:19:22.000000 yeref-0.2.1/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-06-19 18:19:22.000000 yeref-0.2.1/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.2.0/setup.py` & `yeref-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.2.0',
+      version='0.2.01',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.2.0/yeref/l_.py` & `yeref-0.2.1/yeref/l_.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
     'en': "☑️ No",
     'es': "☑️No",
     'fr': "☑️ Non",
     'zh': "☑️没有",
     'ar': "☑️ لا",
 }
 l_post_button = {
-    'ru': "✏️ 3. <b>Введи названия</b> для кнопок и <b>ссылки</b> в формате (одну или несколько; кликни на образец ниже, чтобы скопировать):\n\n<code>[🐳 Link | https://t.me/XXXXX]</code>\n\nили\n\n<code>[❤️ Like][💔 Foo]</code>\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
+    'ru': "✏️ 3. <b>Введи названия</b> для кнопок и <b>ссылки</b> в формате (одну или несколько; кликни на образец ниже, чтобы скопировать):\n\n<code>[🐳 Link | https://t.me/XXXXX]\n\n[❤️ Like][💔 Foo]</code>\n\n(<i>или нажми «➡️️/Next», чтобы пропустить этот шаг</i>)",
     'en': "✏️ 3. <b>Enter button names</b> and <b>links</b> in the format (one or more; click on the sample below to copy):\n\n[🐳 Link | https://t.me/XXXXX]\n\nor\n\n[❤️ Интересно][💔 Не пиши]\n\n( <i>or press &quot;➡️️/Next&quot; to skip this step</i> )",
     'es': "✏️ 3. <b>Ingrese los nombres de los botones</b> y <b>los enlaces</b> en el formato (uno o más; haga clic en la muestra a continuación para copiar):\n\n[🐳 Link | https://t.me/XXXXX]\n\ni\n\n[❤️ Интересно][💔 Не пиши]\n\n( <i>o presiona &quot;➡️️/Siguiente&quot; para omitir este paso</i> )",
     'fr': "✏️ 3. <b>Saisissez les noms des boutons</b> et <b>les liens</b> au format (un ou plusieurs ; cliquez sur l&#x27;exemple ci-dessous pour le copier) :\n\n[🐳 Link | https://t.me/XXXXX]\n\nor\n\n[❤️ Интересно][💔 Не пиши]\n\n( <i>ou appuyez sur &quot;➡️️/Suivant&quot; pour ignorer cette étape</i> )",
     'zh': "✏️ 3.<b>输入按钮名称</b>和<b>链接</b>格式（一个或多个；点击下方示例复制）：\n\n[🐳 Link | https://t.me/XXXXX]\n\nor\n\n[❤️ Интересно][💔 Не пиши]\n\n（<i>或按“➡️️/Next”跳过这一步</i>）",
     'ar': "✏️ 3. <b>أدخل أسماء الأزرار</b> <b>والارتباطات</b> بالتنسيق (واحد أو أكثر ؛ انقر على النموذج أدناه لنسخه):\n\n[🐳 Link | https://t.me/XXXXX]\n\ ولا\n\n[❤️ Интересно][💔 Не пиши]\n\n( <i>أو اضغط على &quot;➡️️ / التالي&quot; لتخطي هذه الخطوة</i> )",
 }
 l_post_button_urlinvalid = {
@@ -1322,15 +1322,15 @@
     'en': "✖️ Bot settings [<b>{0}</b>] successfully reset!",
     'es': "✖️ ¡La configuración del bot [<b>{0}</b>] se restableció correctamente!",
     'fr': "✖️ Les paramètres du bot [<b>{0}</b>] ont été réinitialisés avec succès !",
     'zh': "✖️ 机器人设置 [<b>{0}</b>] 成功重置！",
     'ar': "✖️ تم إعادة تعيين إعدادات البوت [<b>{0}</b>] بنجاح!",
 }
 l_cdeletetext = {
-    'ru': "🚫 Убрать привязку бота [<b>{0}</b>]?",
+    'ru': "🚫 <b>Убрать</b> привязку бота [<b>{0}</b>]?",
     'en': "🚫 Remove bot binding [<b>{0}</b>]?",
     'es': "🚫 ¿Eliminar el enlace del bot [<b>{0}</b>]?",
     'fr': "🚫 Supprimer la liaison du bot [<b>{0}</b>] ?",
     'zh': "🚫 删除机器人绑定 [<b>{0}</b>]？",
     'ar': "🚫 إزالة ربط البوت [<b>{0}</b>]؟",
 }
 l_cdeleteanswer = {
@@ -2532,15 +2532,15 @@
     'en': "✖️ Settings for [<b>{0}</b>] reset successfully!",
     'es': "✖️ ¡La configuración de [<b>{0}</b>] se restableció correctamente!",
     'fr': "✖️ Les paramètres de [<b>{0}</b>] ont été réinitialisés avec succès !",
     'zh': "✖️ [<b>{0}</b>] 的设置重置成功！",
     'ar': "✖️ تمت إعادة تعيين إعدادات [<b>{0}</b>] بنجاح!",
 }
 l_cdelete_text = {
-    'ru': "🚫 Убрать привязку бота к [<b>{0}</b>]?",
+    'ru': "🚫 <b>Убрать</b> привязку бота к [<b>{0}</b>]?",
     'en': "🚫 Remove bot binding to [<b>{0}</b>]?",
     'es': "🚫 ¿Eliminar la vinculación del bot a [<b>{0}</b>]?",
     'fr': "🚫 Supprimer la liaison du bot à [<b>{0}</b>] ?",
     'zh': "🚫 删除绑定到 [<b>{0}</b>] 的机器人？",
     'ar': "🚫 هل تريد إزالة ربط البوت بـ [<b>{0}</b>]؟",
 }
 l_cdelete_answer = {
```

### Comparing `yeref-0.2.0/yeref/yeref.py` & `yeref-0.2.1/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 🇬🇧🇨🇳🇦🇪🇪🇸🇷🇸🇫🇷
 """
 
 markupAdmin = types.ReplyKeyboardMarkup(keyboard=[
     [types.KeyboardButton(text='⬅️ Prev'), types.KeyboardButton(text='↩️ Menu'),
      types.KeyboardButton(text='➡️️ Next')]], resize_keyboard=True, selective=True, row_width=3)
 
-BOT_VARS_ = '{"BOT_PROMO": "#911", "BOT_CHANNEL": 0, "BOT_CHANNELTID": 0, "BOT_GROUP": 0, "BOT_GROUPTID": 0, "BOT_TZ": 0, "BOT_TZ": 0, "BOT_LZ": "en", "BOT_LC": "en"}'
+BOT_VARS_ = '{"BOT_PROMO": "#911", "BOT_CHANNEL": 0, "BOT_CHANNELTID": 0, "BOT_GROUP": 0, "BOT_GROUPTID": 0, "BOT_TZ": 0, "BOT_TZ": 0, "BOT_DT": "", "BOT_LZ": "en", "BOT_LC": "en"}'
 BOT_LSTS_ = '{"BOT_ADMINS": []}'
 USER_VARS_ = '{"USER_TEXT": "", "USER_EMAIL": "", "USER_PROMO": "", "USER_PHONE": "", "USER_GEO": "", "USER_UTM": "", "USER_ID": 0, "USER_DT": "", "USER_TZ": 0, "USER_LC": "en", "USER_ISADMIN": 0, "USER_ISPREMIUM": 0, "USER_BALL": 0, "USER_RAND": 0, "USER_QUIZ": 0, "USER_DICE": 0, "USER_PAY": 0, "DATE_TIME": 0}'
 USER_LSTS_ = '{"USER_UTMREF": []}'
 # endregion
 
 
 # region db
```

