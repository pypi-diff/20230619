# Comparing `tmp/nonebot_plugin_al-0.3.0.tar.gz` & `tmp/nonebot_plugin_al-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_al-0.3.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_al-0.3.1.tar", max compression
```

## Comparing `nonebot_plugin_al-0.3.0.tar` & `nonebot_plugin_al-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/LICENSE
--rw-r--r--   0        0        0     3645 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/README.md
--rw-r--r--   0        0        0     6475 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/nonebot_plugin_al/__init__.py
--rw-r--r--   0        0        0    69693 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/nonebot_plugin_al/api.py
--rw-r--r--   0        0        0     3348 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/nonebot_plugin_al/bili.py
--rw-r--r--   0        0        0    69109 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/nonebot_plugin_al/data/eq.json
--rw-r--r--   0        0        0    41850 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/nonebot_plugin_al/data/ship.json
--rw-r--r--   0        0        0    10152 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/nonebot_plugin_al/draw.py
--rw-r--r--   0        0        0     7529 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/nonebot_plugin_al/name.py
--rw-r--r--   0        0        0    13339 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/nonebot_plugin_al/send_message.py
--rw-r--r--   0        0        0     5832 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/nonebot_plugin_al/utils.py
--rw-r--r--   0        0        0     1003 2023-06-19 05:10:24.525377 nonebot_plugin_al-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4733 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-19 16:16:50.043033 nonebot_plugin_al-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3793 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/README.md
+-rw-r--r--   0        0        0     6478 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/nonebot_plugin_al/__init__.py
+-rw-r--r--   0        0        0    69751 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/nonebot_plugin_al/api.py
+-rw-r--r--   0        0        0     3348 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/nonebot_plugin_al/bili.py
+-rw-r--r--   0        0        0    69109 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/nonebot_plugin_al/data/eq.json
+-rw-r--r--   0        0        0    41850 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/nonebot_plugin_al/data/ship.json
+-rw-r--r--   0        0        0    10152 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/nonebot_plugin_al/draw.py
+-rw-r--r--   0        0        0     7427 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/nonebot_plugin_al/name.py
+-rw-r--r--   0        0        0    13372 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/nonebot_plugin_al/send_message.py
+-rw-r--r--   0        0        0     5995 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/nonebot_plugin_al/utils.py
+-rw-r--r--   0        0        0     1028 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.3.1/PKG-INFO
```

### Comparing `nonebot_plugin_al-0.3.0/LICENSE` & `nonebot_plugin_al-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.0/README.md` & `nonebot_plugin_al-0.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 ## 功能
 
 1、b站wiki井号榜一图流
 
 2、舰船装备图鉴
 
-3、(50%完成)移植大部分[blhx](https://github.com/Gaylone/blhx_wiki)（原hoshino改项目）的大部分功能
+3、(70%完成)移植大部分[blhx](https://github.com/Gaylone/blhx_wiki)（原hoshino改项目）的大部分功能
 
 
 ## 安装
 
 以下命令选其一即可
 
 ```sh
@@ -54,15 +54,18 @@
 ```
 ```sh
 git clone https://github.com/Agnes4m/nonebot_plugin_AL.git
 ```
 
 ## 资源包
 
-本项的图片资源基本都来源于本地，具体在项目的ship_html/images文件夹里，大小在2.7G左右，项目在[api](https://github.com/AzurAPI/azurapi-js-setup) 打包下载，将下载来的项目里的images文件夹放入本项目的ship_html里面，这点十分重要，blhx_wiki功能90%依赖这个资源包，请自行留意它的更新
+本项的图片资源基本都来源于本地，具体在项目的images文件夹里，大小在3.5G左右，项目在[api](https://github.com/AzurAPI/azurapi-js-setup) 打包下载，将下载来的项目里的images文件夹放入bot目录下`data/al/ship_html`里面，也就是说路径为`data/al/ship_html/images/`这点十分重要，blhx_wiki功能90%依赖这个资源包，请自行留意它的更新
+
+百度云盘：链接：https://pan.baidu.com/s/1ppLW3rkygLovXIG_Y58Qrg?pwd=57uk 
+提取码：57uk
 
 ## 指令
 
 ### 【总】碧蓝帮助 | 碧蓝指令
 
 - 1、碧蓝+['强度榜','装备榜','金部件榜','萌新榜','兵器榜','专武榜',
         '兑换榜','研发榜','改造榜','跨队榜','pt榜','氪金榜','打捞主线榜','打捞作战榜']
```

#### html2text {}

```diff
@@ -1,22 +1,25 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
 # nonebot_plugin_al 0.3.0 __â¨Nonebot & ç¢§èèªçº¿æ»ç¥â¨__ [GitHub_stars]
            [GitHub_issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
 ## åè½ 1ãbç«wikiäºå·æ¦ä¸å¾æµ 2ãè°è¹è£å¤å¾é´ 3ã
-(50%å®æ)ç§»æ¤å¤§é¨å[blhx](https://github.com/Gaylone/
+(70%å®æ)ç§»æ¤å¤§é¨å[blhx](https://github.com/Gaylone/
 blhx_wiki)ï¼åhoshinoæ¹é¡¹ç®ï¼çå¤§é¨ååè½ ## å®è£
 ä»¥ä¸å½ä»¤éå¶ä¸å³å¯ ```sh nb plugin install nonebot_plugin_al ``` ```sh
 pip install nonebot_plugin_al ``` ```sh git clone https://github.com/Agnes4m/
 nonebot_plugin_AL.git ``` ## èµæºå
-æ¬é¡¹çå¾çèµæºåºæ¬é½æ¥æºäºæ¬å°ï¼å·ä½å¨é¡¹ç®çship_html/
-imagesæä»¶å¤¹éï¼å¤§å°å¨2.7Gå·¦å³ï¼é¡¹ç®å¨[api](https://github.com/
-AzurAPI/azurapi-js-setup)
-æåä¸è½½ï¼å°ä¸è½½æ¥çé¡¹ç®éçimagesæä»¶å¤¹æ¾å¥æ¬é¡¹ç®çship_htmléé¢ï¼è¿ç¹ååéè¦ï¼blhx_wikiåè½90%ä¾èµè¿ä¸ªèµæºåï¼è¯·èªè¡çæå®çæ´æ°
-## æä»¤ ### ãæ»ãç¢§èå¸®å© | ç¢§èæä»¤ - 1ãç¢§è+
+æ¬é¡¹çå¾çèµæºåºæ¬é½æ¥æºäºæ¬å°ï¼å·ä½å¨é¡¹ç®çimagesæä»¶å¤¹éï¼å¤§å°å¨3.5Gå·¦å³ï¼é¡¹ç®å¨
+[api](https://github.com/AzurAPI/azurapi-js-setup)
+æåä¸è½½ï¼å°ä¸è½½æ¥çé¡¹ç®éçimagesæä»¶å¤¹æ¾å¥botç®å½ä¸`data/
+al/ship_html`éé¢ï¼ä¹å°±æ¯è¯´è·¯å¾ä¸º`data/al/ship_html/images/
+`è¿ç¹ååéè¦ï¼blhx_wikiåè½90%ä¾èµè¿ä¸ªèµæºåï¼è¯·èªè¡çæå®çæ´æ°
+ç¾åº¦äºçï¼é¾æ¥ï¼https://pan.baidu.com/s/
+1ppLW3rkygLovXIG_Y58Qrg?pwd=57uk æåç ï¼57uk ## æä»¤ ###
+ãæ»ãç¢§èå¸®å© | ç¢§èæä»¤ - 1ãç¢§è+
 ['å¼ºåº¦æ¦','è£å¤æ¦','éé¨ä»¶æ¦','èæ°æ¦','åµå¨æ¦','ä¸æ­¦æ¦',
 'åæ¢æ¦','ç åæ¦','æ¹é æ¦','è·¨éæ¦','ptæ¦','æ°ªéæ¦','ææä¸»çº¿æ¦','ææä½ææ¦']
 - 2ãç¢§èè§è²ãè§è²åç§°ã - 3ãç¢§èè£å¤ãè£å¤åç§°ã ###
 ãblhx_wikiãï¼é¤äºæ¥è¹ï¼å¶ä»ä¸ç¨ç©ºæ ¼ï¼ 0.å¸®å©ä¿¡æ¯
 å½ä»¤ç¤ºèï¼blhx å¸®å© 1.æ ¹æ®è¹åæ¥è°è¹ä¿¡æ¯ å½ä»¤ç¤ºèï¼ blhx
 é¿é¨ 2.æ ¹æ®è¹ååç®è¤åæ¥è¯¢ç®è¤ç«ç» å½ä»¤ç¤ºèï¼blhx
 å£è·¯ææ¯ Luxury_Handle å½ä»¤ç¤ºèï¼blhx é¿é¨ å¾¡ççè¾æ¯è¢
```

### Comparing `nonebot_plugin_al-0.3.0/nonebot_plugin_al/__init__.py` & `nonebot_plugin_al-0.3.1/nonebot_plugin_al/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 try:
     import ujson as json
 except:
     import json
 
 
 from .bili import jinghao,get_data, get_ship_msg
-from .send_message import *
+from .send_message import blhx
 
 
 __version__ = "0.3"
 __plugin_meta__ = PluginMetadata(
     name="碧蓝航线攻略",
     description='碧蓝航线井号榜等等攻略',
     usage="""
```

### Comparing `nonebot_plugin_al-0.3.0/nonebot_plugin_al/api.py` & `nonebot_plugin_al-0.3.1/nonebot_plugin_al/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1164,15 +1164,16 @@
 参数：无
 返回值：字符串
 说明：该方法随机返回游戏加载图像的随机文件名
 """
 
 
 def get_random_gallery():
-    files = [f for f in Path(DATA_PATH, 'ship_html', 'images', 'gallery').resolve().iterdir() if f.is_file()]
+    gallery_path = Path(DATA_PATH, 'ship_html', 'images', 'gallery').resolve()
+    files = [f.relative_to(gallery_path) for f in gallery_path.iterdir() if f.is_file()]
     rfile = random.choice(files)
     return str(rfile)
 
 
 """
 方法名：get_pve_recommendation
 参数列表：无
```

### Comparing `nonebot_plugin_al-0.3.0/nonebot_plugin_al/bili.py` & `nonebot_plugin_al-0.3.1/nonebot_plugin_al/bili.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.0/nonebot_plugin_al/data/eq.json` & `nonebot_plugin_al-0.3.1/nonebot_plugin_al/data/eq.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.0/nonebot_plugin_al/data/ship.json` & `nonebot_plugin_al-0.3.1/nonebot_plugin_al/data/ship.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.0/nonebot_plugin_al/draw.py` & `nonebot_plugin_al-0.3.1/nonebot_plugin_al/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.0/nonebot_plugin_al/name.py` & `nonebot_plugin_al-0.3.1/nonebot_plugin_al/name.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from pathlib import Path
 
+BOT_PATH = Path.cwd()
 DATA_PATH = Path().joinpath('data/al')
 PATH = str(DATA_PATH.joinpath('azurapi_data'))
 BACK_PATH = DATA_PATH.joinpath('azurapi_data_bak')
+DATA_PATH_STR = str(DATA_PATH)
 SAVE_PATH = DATA_PATH
 MAIN_URL = "https://ghproxy.com/https://raw.githubusercontent.com/AzurAPI"    ##https://raw.fastgit.org可以根据需要配置不同代理，结合网络情况自行修改
 SHIP_LIST = f"{MAIN_URL}/azurapi-js-setup/master/ships.json"
 CHAPTER_LIST = f"{MAIN_URL}/azurapi-js-setup/master/chapters.json"
 EQUIPMENT_LIST = f"{MAIN_URL}/azurapi-js-setup/master/equipments.json"
 VERSION_INFO = f"{MAIN_URL}/azurapi-js-setup/master/version-info.json"
 MEMORIES_INFO = f"{MAIN_URL}/azurapi-js-setup/master/memories.json"
@@ -62,38 +64,35 @@
 args: null
 return: 返回整数，0表示成功，其他数字表示失败
 
 初始化名称文件，在执行脚本更新之后应该执行一次这个方法。
 对于已经在名字系统里面存在的船只，不做任何处理；对于新加入的船，会进行添加。
 '''
 async def UpdateName():
-    PATH = str(DATA_PATH)
     ships = {}
 
     # 判断文件是否存在，不存在的话就不进行读取
     try:
-        async with aiofiles.open(PATH + '/azurapi_data/names.json', 'r', encoding='utf-8') as fp:
+        async with aiofiles.open(DATA_PATH_STR + '/azurapi_data/names.json', 'r', encoding='utf-8') as fp:
             load_dict = await fp.read()
             ships = json.loads(load_dict)
-            ships = json.loads(ships)
     except:
         pass
 
-    async with aiofiles.open(PATH + '/azurapi_data/ships.json', 'r', encoding='utf-8') as fp:
+    async with aiofiles.open(DATA_PATH_STR + '/azurapi_data/ships.json', 'r', encoding='utf-8') as fp:
         load_dict = await fp.read()
         data = json.loads(load_dict)
-        data = json.loads(data) # 别删除
 
     for item in data:
         if item['id'] in ships.keys():
             continue
         ships[item['id']] = [item['names']['cn'], item['names']['jp'], item['names']['kr'], item['names']['en']]
 
     # print(ships)
-    async with aiofiles.open(PATH + '/azurapi_data/names.json', 'w', encoding='utf-8') as fp:
+    async with aiofiles.open(DATA_PATH_STR + '/azurapi_data/names.json', 'w', encoding='utf-8') as fp:
         # json.dump(ships, fp, indent=2, ensure_ascii=False)
         await fp.write(json.dumps(ships, indent=2, ensure_ascii=False))
 
     return 0
 
 
 '''
@@ -104,24 +103,23 @@
 return: 返回整数，0表示成功，其他数字表示失败
 
 为舰船上传新的别名，在调用这个方法的时候用该特别注意权限控制
 '''
 ERR_NAMEALREADYEXISTS = -1
 async def AddName(id: str, nickname: str):
 
-    async with aiofiles.open(PATH + '/azurapi_data/names.json', 'r', encoding='utf-8') as fp:
+    async with aiofiles.open(DATA_PATH_STR + '/azurapi_data/names.json', 'r', encoding='utf-8') as fp:
         load_dict = await fp.read()
         data = json.loads(load_dict)
-        data = json.loads(data)
 
     if nickname in data[str(id)]:
         return ERR_NAMEALREADYEXISTS
     data[id].append(nickname)
 
-    async with aiofiles.open(PATH + '/azurapi_data/names.json', 'w', encoding='utf-8') as fp:
+    async with aiofiles.open(DATA_PATH_STR + '/azurapi_data/names.json', 'w', encoding='utf-8') as fp:
         await fp.write(json.dumps(data, indent=2, ensure_ascii=False))
 
     return 0
 
 
 '''
 function: DelName
@@ -131,25 +129,24 @@
 return: 返回整数，0表示成功，其他数字表示失败
 
 为舰船删除已有的别名，在调用这个方法的时候用该特别注意权限控制
 '''
 ERR_NICKNAMENOTFOUND = -1
 async def DelName(id: str, nickname: str):
 
-    async with aiofiles.open(PATH + '/azurapi_data/names.json', 'r', encoding='utf-8') as fp:
+    async with aiofiles.open(DATA_PATH_STR + '/azurapi_data/names.json', 'r', encoding='utf-8') as fp:
         load_dict = await fp.read()
         data = json.loads(load_dict)
-        data = json.loads(data)
 
     try:
         data[id].remove(nickname)
     except:
         return ERR_NICKNAMENOTFOUND
 
-    async with aiofiles.open(PATH + '/azurapi_data/names.json', 'w', encoding='utf-8') as fp:
+    async with aiofiles.open(DATA_PATH_STR + '/azurapi_data/names.json', 'w', encoding='utf-8') as fp:
         await fp.write(json.dumps(data, indent=2, ensure_ascii=False))
 
     return 0
 
 
 '''
 function: GetStandredNameByNickname
@@ -160,18 +157,17 @@
     如果没有查找到船只，返回ERR_SHIPNOTFOUND整数值，该值为-1
 
 根据船只的标准名或者别名，查找船只的id和标准名
 '''
 ERR_SHIPNOTFOUND = -1
 async def GetIDByNickname(nickname: str):
 
-    async with aiofiles.open(PATH + '/azurapi_data/names.json', 'r', encoding='utf-8') as fp:
+    async with aiofiles.open(DATA_PATH_STR + '/azurapi_data/names.json', 'r', encoding='utf-8') as fp:
         load_dict = await fp.read()
         data = json.loads(load_dict)
-        data = json.loads(data)
 
     # data = {}
     retvalue = {}
     for item in data.items():
         if nickname in item[1]:
             retvalue = {
                 'id': item[0],
@@ -211,15 +207,14 @@
 return:
     返回一个数组，里面包含这个舰船的所有名称
 
 根据舰船的标准名，返回这个舰船的所有名称
 '''
 async def GetAllNickname(id: str):
 
-    async with aiofiles.open(PATH + '/azurapi_data/names.json', 'r', encoding='utf-8') as fp:
+    async with aiofiles.open(DATA_PATH_STR + '/azurapi_data/names.json', 'r', encoding='utf-8') as fp:
         load_dict = await fp.read()
         data = json.loads(load_dict)
-        data = json.loads(data)
 
     return data[id]
```

### Comparing `nonebot_plugin_al-0.3.0/nonebot_plugin_al/send_message.py` & `nonebot_plugin_al-0.3.1/nonebot_plugin_al/send_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     async def send_ship_skin_or_info(
         matcher:Matcher,
         event:Event,
         bot:Bot,
         arg:Message = CommandArg()
         ):
-        SAVE_PATH = str(SAVE_PATH)
+        SAVE_PATH = Path().cwd().joinpath('data/al')
         try:
             args = arg.extract_plain_text().split()
             if len(args) == 2:
                 ship_name = str(args[0])
                 skin_name = str(args[1]).replace("_", (" "))
                 ship_nickname_data = await GetIDByNickname(ship_name)
                 if ship_nickname_data == -1 :
@@ -85,46 +85,46 @@
             await bot.send(event=event,message="查询出错", at_sender=True)
 
     async def send_random_gallery(
         matcher:Matcher,
         event:Event,
         bot:Bot
         ):
-        SAVE_PATH = str('data/al')
-        msg = MessageSegment.image("file:///" + SAVE_PATH + "/ship_html/images/gallery/" + get_random_gallery())
+        SAVE_PATH = Path().cwd().joinpath('data/al/ship_html/images/gallery/' / get_random_gallery())
+        msg = MessageSegment.image("file:///" + str(SAVE_PATH))
         await bot.send(event=event,message=msg, at_sender=True)
 
 
     async def send_blhx_help(
         matcher:Matcher,
         event:Event,
         bot:Bot
         ):
-        msg = "1.查询舰船信息命令：”blhx [无需和谐的中文船名]“\n" \
-            "2.查询舰船皮肤命令：”blhx [无需和谐的中文船名] [皮肤名]“ 皮肤名为”原皮”则查询原皮，为“婚纱”则查询婚纱，如果皮肤名有空格则用_替代\n" \
-            "3.查询加载时的过场动画：“blhx过场”" \
-            "4.查询强度榜：“blhx强度榜”"
+        msg = """
+        1.查询舰船信息命令：”blhx [无需和谐的中文船名]
+        2.查询舰船皮肤命令：”blhx [无需和谐的中文船名] [皮肤名]“ 皮肤名为”原皮”则查询原皮，为“婚纱”则查询婚纱，如果皮肤名有空格则用_替代
+        3.查询加载时的过场动画：“blhx过场
+        4.查询强度榜：“blhx强度榜"""
         await bot.send(event=event,message=msg,at_sender=True)
 
 
     async def send_pve_recommendation(        
         matcher:Matcher,
         event:Event,
         bot:Bot
         ):
         div_list = await get_pve_recommendation()
-        div_text = ["认知觉醒推荐榜(主线)\n", "认知觉醒推荐榜(大世界)\n", "装备榜\n", "萌新入坑舰船推荐榜\n", "萌新初期装备榜\n",
-                    "兵装推荐榜\n", "专武推荐榜\n", "兑换装备推荐榜\n", "研发装备推荐榜\n", "改造推荐榜\n", "跨队舰船推荐榜\n",
-                    "氪金榜\n"]
+        # div_text = ["认知觉醒推荐榜(主线)\n", "认知觉醒推荐榜(大世界)\n", "装备榜\n", "萌新入坑舰船推荐榜\n", "萌新初期装备榜\n",
+        #             "兵装推荐榜\n", "专武推荐榜\n", "兑换装备推荐榜\n", "研发装备推荐榜\n", "改造推荐榜\n", "跨队舰船推荐榜\n",
+        #             "氪金榜\n" , "打捞主线榜\n","打捞作战榜'\n"]
         msg = "仅代表个人观点，完全不等于绝对客观，可能存在各种主观评判或者真爱加成，不过目标是努力去进行符合环境需求的客观评定\n"
         msg_list = []
         if len(div_list) != 0:
             for i in range(0, len(div_list)):
-                msg += (div_text[i] + MessageSegment.image(file=str(div_list[i].find('img')['src'])) + "\n")
-                print(str(div_list[i].find('img')['src']))
+                msg += Message(str(div_list[i].find('img')['alt']) + MessageSegment.image(file=str(div_list[i].find('img')['src'])) + "\n")
             msg_list.append(msg)
             forward_msg = render_forward_msg(msg_list)
             if isinstance(event,GroupMessageEvent):
                 await bot.call_api('send_group_forward_msg',group_id=event.group_id, messages=forward_msg)
                 return
         else:
             await bot.send(event=event,message='暂无信息', at_sender=True)
```

### Comparing `nonebot_plugin_al-0.3.0/nonebot_plugin_al/utils.py` & `nonebot_plugin_al-0.3.1/nonebot_plugin_al/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import imgkit
 import cv2
 import pypinyin
 import json
 import aiofiles
 
 from pathlib import Path
+from nonebot.adapters.onebot.v11 import Bot
 
 SAVE_PATH = Path().joinpath('data/al')
 tool_path = SAVE_PATH.joinpath('wkhtmltopdf', 'bin', 'wkhtmltoimage.exe')
 """
 方法名：print_img
 参数列表：无
 用处：调用打印工具，打印ship_info.html成图片
@@ -160,15 +161,20 @@
     async with aiofiles.open(SAVE_PATH.joinpath('azurapi_data', 'version-info.json'), 'r',
               encoding='utf-8') as load_f:
         load_dict = await load_f.read()
         load_dict:dict = json.loads(load_dict)
         load_dict:dict = json.loads(load_dict) # 别删除，否则会有类型错误
     return load_dict['ships']
 
-def render_forward_msg(msg_list: list, uid=1916714922, name='小加加(VC装甲钢36D版)'):
+def render_forward_msg(msg_list: list, uid=1916714922, name='小加加(VC装甲钢36D版)',bot:Bot = None):
+    try:
+        uid = bot.self_id
+        name = list(bot.config.nickname)[0]
+    except:
+        pass
     forward_msg = []
     for msg in msg_list:
         forward_msg.append({
             "type": "node",
             "data": {
                 "name": str(name),
                 "uin": str(uid),
```

### Comparing `nonebot_plugin_al-0.3.0/pyproject.toml` & `nonebot_plugin_al-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_al"
-version = "0.3.0"
+version = "0.3.1"
 description = "Azuer L plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_AL"
 repository = "https://github.com/Agnes4m/nonebot_plugin_AL"
 keywords = ["game", "nonebot2", "plugin","bilibili"]
@@ -26,11 +26,12 @@
 nonebot-adapter-onebot = ">=2.2.1"
 nonebot_plugin_htmlrender = "^0.2.0.3"
 aiohttp = ">=3.8.3"
 bs4 = "^0.0.1"
 aiofiles = "^23.1.0"
 pypinyin = "^0.49.0"
 imgkit = "^1.2.3"
+opencv-python = "^4.7.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_al-0.3.0/PKG-INFO` & `nonebot_plugin_al-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-al
-Version: 0.3.0
+Version: 0.3.1
 Summary: Azuer L plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: MIT
 Keywords: game,nonebot2,plugin,bilibili
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -18,14 +18,15 @@
 Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: aiohttp (>=3.8.3)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: imgkit (>=1.2.3,<2.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.1)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
 Requires-Dist: nonebot_plugin_htmlrender (>=0.2.0.3,<0.3.0.0)
+Requires-Dist: opencv-python (>=4.7.0,<5.0.0)
 Requires-Dist: pypinyin (>=0.49.0,<0.50.0)
 Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_AL
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
@@ -63,15 +64,15 @@
 
 ## 功能
 
 1、b站wiki井号榜一图流
 
 2、舰船装备图鉴
 
-3、(50%完成)移植大部分[blhx](https://github.com/Gaylone/blhx_wiki)（原hoshino改项目）的大部分功能
+3、(70%完成)移植大部分[blhx](https://github.com/Gaylone/blhx_wiki)（原hoshino改项目）的大部分功能
 
 
 ## 安装
 
 以下命令选其一即可
 
 ```sh
@@ -82,15 +83,18 @@
 ```
 ```sh
 git clone https://github.com/Agnes4m/nonebot_plugin_AL.git
 ```
 
 ## 资源包
 
-本项的图片资源基本都来源于本地，具体在项目的ship_html/images文件夹里，大小在2.7G左右，项目在[api](https://github.com/AzurAPI/azurapi-js-setup) 打包下载，将下载来的项目里的images文件夹放入本项目的ship_html里面，这点十分重要，blhx_wiki功能90%依赖这个资源包，请自行留意它的更新
+本项的图片资源基本都来源于本地，具体在项目的images文件夹里，大小在3.5G左右，项目在[api](https://github.com/AzurAPI/azurapi-js-setup) 打包下载，将下载来的项目里的images文件夹放入bot目录下`data/al/ship_html`里面，也就是说路径为`data/al/ship_html/images/`这点十分重要，blhx_wiki功能90%依赖这个资源包，请自行留意它的更新
+
+百度云盘：链接：https://pan.baidu.com/s/1ppLW3rkygLovXIG_Y58Qrg?pwd=57uk 
+提取码：57uk
 
 ## 指令
 
 ### 【总】碧蓝帮助 | 碧蓝指令
 
 - 1、碧蓝+['强度榜','装备榜','金部件榜','萌新榜','兵器榜','专武榜',
         '兑换榜','研发榜','改造榜','跨队榜','pt榜','氪金榜','打捞主线榜','打捞作战榜']
```

#### html2text {}

```diff
@@ -1,37 +1,41 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.3.0 Summary: Azuer L
+Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.3.1 Summary: Azuer L
 plugin for NoneBot2 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: MIT Keywords: game,nonebot2,plugin,bilibili Author: Agnes_Digital
 Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: aiofiles (>=23.1.0,<24.0.0) Requires-
 Dist: aiohttp (>=3.8.3) Requires-Dist: bs4 (>=0.0.1,<0.0.2) Requires-Dist:
 imgkit (>=1.2.3,<2.0.0) Requires-Dist: nonebot-adapter-onebot (>=2.2.1)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist:
-nonebot_plugin_htmlrender (>=0.2.0.3,<0.3.0.0) Requires-Dist: pypinyin
-(>=0.49.0,<0.50.0) Project-URL: Repository, https://github.com/Agnes4m/
-nonebot_plugin_AL Description-Content-Type: text/markdown
+nonebot_plugin_htmlrender (>=0.2.0.3,<0.3.0.0) Requires-Dist: opencv-python
+(>=4.7.0,<5.0.0) Requires-Dist: pypinyin (>=0.49.0,<0.50.0) Project-URL:
+Repository, https://github.com/Agnes4m/nonebot_plugin_AL Description-Content-
+Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
 # nonebot_plugin_al 0.3.0 __â¨Nonebot & ç¢§èèªçº¿æ»ç¥â¨__ [GitHub_stars]
            [GitHub_issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
 ## åè½ 1ãbç«wikiäºå·æ¦ä¸å¾æµ 2ãè°è¹è£å¤å¾é´ 3ã
-(50%å®æ)ç§»æ¤å¤§é¨å[blhx](https://github.com/Gaylone/
+(70%å®æ)ç§»æ¤å¤§é¨å[blhx](https://github.com/Gaylone/
 blhx_wiki)ï¼åhoshinoæ¹é¡¹ç®ï¼çå¤§é¨ååè½ ## å®è£
 ä»¥ä¸å½ä»¤éå¶ä¸å³å¯ ```sh nb plugin install nonebot_plugin_al ``` ```sh
 pip install nonebot_plugin_al ``` ```sh git clone https://github.com/Agnes4m/
 nonebot_plugin_AL.git ``` ## èµæºå
-æ¬é¡¹çå¾çèµæºåºæ¬é½æ¥æºäºæ¬å°ï¼å·ä½å¨é¡¹ç®çship_html/
-imagesæä»¶å¤¹éï¼å¤§å°å¨2.7Gå·¦å³ï¼é¡¹ç®å¨[api](https://github.com/
-AzurAPI/azurapi-js-setup)
-æåä¸è½½ï¼å°ä¸è½½æ¥çé¡¹ç®éçimagesæä»¶å¤¹æ¾å¥æ¬é¡¹ç®çship_htmléé¢ï¼è¿ç¹ååéè¦ï¼blhx_wikiåè½90%ä¾èµè¿ä¸ªèµæºåï¼è¯·èªè¡çæå®çæ´æ°
-## æä»¤ ### ãæ»ãç¢§èå¸®å© | ç¢§èæä»¤ - 1ãç¢§è+
+æ¬é¡¹çå¾çèµæºåºæ¬é½æ¥æºäºæ¬å°ï¼å·ä½å¨é¡¹ç®çimagesæä»¶å¤¹éï¼å¤§å°å¨3.5Gå·¦å³ï¼é¡¹ç®å¨
+[api](https://github.com/AzurAPI/azurapi-js-setup)
+æåä¸è½½ï¼å°ä¸è½½æ¥çé¡¹ç®éçimagesæä»¶å¤¹æ¾å¥botç®å½ä¸`data/
+al/ship_html`éé¢ï¼ä¹å°±æ¯è¯´è·¯å¾ä¸º`data/al/ship_html/images/
+`è¿ç¹ååéè¦ï¼blhx_wikiåè½90%ä¾èµè¿ä¸ªèµæºåï¼è¯·èªè¡çæå®çæ´æ°
+ç¾åº¦äºçï¼é¾æ¥ï¼https://pan.baidu.com/s/
+1ppLW3rkygLovXIG_Y58Qrg?pwd=57uk æåç ï¼57uk ## æä»¤ ###
+ãæ»ãç¢§èå¸®å© | ç¢§èæä»¤ - 1ãç¢§è+
 ['å¼ºåº¦æ¦','è£å¤æ¦','éé¨ä»¶æ¦','èæ°æ¦','åµå¨æ¦','ä¸æ­¦æ¦',
 'åæ¢æ¦','ç åæ¦','æ¹é æ¦','è·¨éæ¦','ptæ¦','æ°ªéæ¦','ææä¸»çº¿æ¦','ææä½ææ¦']
 - 2ãç¢§èè§è²ãè§è²åç§°ã - 3ãç¢§èè£å¤ãè£å¤åç§°ã ###
 ãblhx_wikiãï¼é¤äºæ¥è¹ï¼å¶ä»ä¸ç¨ç©ºæ ¼ï¼ 0.å¸®å©ä¿¡æ¯
 å½ä»¤ç¤ºèï¼blhx å¸®å© 1.æ ¹æ®è¹åæ¥è°è¹ä¿¡æ¯ å½ä»¤ç¤ºèï¼ blhx
 é¿é¨ 2.æ ¹æ®è¹ååç®è¤åæ¥è¯¢ç®è¤ç«ç» å½ä»¤ç¤ºèï¼blhx
 å£è·¯ææ¯ Luxury_Handle å½ä»¤ç¤ºèï¼blhx é¿é¨ å¾¡ççè¾æ¯è¢
```

