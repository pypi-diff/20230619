# Comparing `tmp/nonebot_plugin_bilichat-2.7.2.tar.gz` & `tmp/nonebot_plugin_bilichat-2.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.7.2.tar", last modified: Mon Jun 19 03:28:03 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.7.3.tar", last modified: Mon Jun 19 10:35:39 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.7.2.tar` & `nonebot_plugin_bilichat-2.7.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    34523 2023-06-19 03:27:53.285987 nonebot_plugin_bilichat-2.7.2/LICENSE
--rw-r--r--   0        0        0    13119 2023-06-19 03:27:53.285987 nonebot_plugin_bilichat-2.7.2/README.md
--rw-r--r--   0        0        0     9598 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     5512 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6502 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0    15476 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3812 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      555 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1187 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    14952 2023-06-19 03:27:53.305988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf
--rw-r--r--   0        0        0    93905 2023-06-19 03:27:53.309988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7114 2023-06-19 03:27:53.309988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     1363 2023-06-19 03:27:53.309988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     6899 2023-06-19 03:27:53.309988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-06-19 03:27:53.309988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2363 2023-06-19 03:27:53.309988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-06-19 03:27:53.309988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-06-19 03:27:53.309988 nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1583 2023-06-19 03:28:03.958270 nonebot_plugin_bilichat-2.7.2/pyproject.toml
--rw-r--r--   0        0        0    14694 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.7.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-19 10:35:28.958203 nonebot_plugin_bilichat-2.7.3/LICENSE
+-rw-r--r--   0        0        0    13119 2023-06-19 10:35:28.958203 nonebot_plugin_bilichat-2.7.3/README.md
+-rw-r--r--   0        0        0     9598 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     5512 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6502 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0    16205 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3812 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      555 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-06-19 10:35:28.978203 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1187 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    14952 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf
+-rw-r--r--   0        0        0    93905 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7279 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     1363 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     6899 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2363 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-06-19 10:35:28.982204 nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1583 2023-06-19 10:35:39.650212 nonebot_plugin_bilichat-2.7.3/pyproject.toml
+-rw-r--r--   0        0        0    14694 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.7.3/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.7.2/LICENSE` & `nonebot_plugin_bilichat-2.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/README.md` & `nonebot_plugin_bilichat-2.7.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,48 +27,60 @@
         name: str,
         face: Union[bytes, BytesIO],
         level: int,
         fans: str,
         video_counts: int,
         title: str = "UP主",
         name_color: str = "black",
+        official_verify: int = -1,
     ) -> None:
         self.name: str = name
+        """UP名"""
         self.face: BytesIO = face if isinstance(face, BytesIO) else BytesIO(face)
+        """UP头像"""
         self.level: int = level
+        """UP等级"""
         self.name_color: str = name_color or "black"
+        """UP名字颜色"""
         self.fans: str = fans
+        """粉丝数"""
         self.video_counts: int = video_counts
+        """视频投稿数量"""
         self.title: str = title
+        """合作视频中的角色"""
+        self.official_verify: int = official_verify
+        """小闪电认证：-1 为无，0 为个人，1 为企业"""
 
     @classmethod
     async def from_id(cls, client: AsyncClient, mid: int, name: str, title: str):
         try:
             up_data = await get_user_space_info(mid)
         except ResponseCodeError as e:
             if e.code in [-404, 404]:
                 up_data = None
             else:
                 raise e
         bg_color = up_data["card"]["vip"]["label"]["bg_color"] if up_data else "black"
         level = up_data["card"]["level_info"]["current_level"] if up_data else 0
         video_counts = up_data["archive"]["count"] if up_data else 0
         face_url = up_data["card"]["face"] if up_data else "https://i0.hdslb.com/bfs/face/member/noface.jpg"
+        official_verify = up_data["card"]["official_verify"]["type"] if up_data else -1
         face_req = await client.get(face_url)
         if face_req.status_code == 404:
             face_req = await client.get(f"{face_url}@160w_160h_1c_1s.webp")
         face = face_req.content
         return cls(
             name=name,
             name_color=bg_color,
             level=level,
             face=face,
             fans=num_fmt(up_data["card"]["fans"]) if up_data else "N/A",
             video_counts=video_counts,
             title=title,
+            official_verify=official_verify,
         )
 
 
 class BiliVideoImage:
     def __init__(
         self,
         cover: Union[bytes, BytesIO],
@@ -85,30 +97,45 @@
         pubdate: datetime,
         uploaders: List[UP],
         b23_url: str,
         aid: str,
         desc: Optional[str] = None,
     ):
         self.cover: BytesIO = cover if isinstance(cover, BytesIO) else BytesIO(cover)
+        """视频封面"""
         minutes, self.seconds = divmod(duration, 60)
         self.hours, self.minutes = divmod(minutes, 60)
         self.type_name: str = type_name
+        """视频分区"""
         self.title: str = title
+        """视频标题"""
         self.desc: str = desc or "该视频没有简介"
+        """视频简介"""
         self.view: str = view
+        """播放量"""
         self.danmaku: str = danmaku
+        """弹幕数"""
         self.favorite: str = favorite
+        """收藏"""
         self.coin: str = coin
+        """投币"""
         self.like: str = like
+        """点赞"""
         self.reply: str = reply
+        """评论"""
         self.share: str = share
+        """分享"""
         self.pubdate: datetime = pubdate
+        """发布时间"""
         self.uploaders: List[UP] = uploaders
+        """up主列表"""
         self.b23_url: str = b23_url
+        """b23短链"""
         self.aid: str = aid
+        """av号"""
 
     @classmethod
     async def from_view_rely(cls, video_view: ViewReply, b23_url: str) -> "BiliVideoImage":
         video_info = video_view.activity_season if video_view.activity_season.arc.aid else video_view
         # 获取封面
         client = hc
         client.headers.update(
@@ -332,15 +359,14 @@
         return image.getvalue()
 
     async def style_blue(self):
         import jinja2
         from nonebot_plugin_htmlrender.browser import get_new_page
 
         style_bule = Path(__file__).parent.parent.joinpath("static", "style_blue")
-        assets = style_bule.joinpath("assets")
         video_time = (
             f"{self.hours:02d}:{self.minutes:02d}:{self.seconds:02d}"
             if self.hours
             else f"{self.minutes:02d}:{self.seconds:02d}"
         )
         qr = qrcode.QRCode(border=1)
         qr.add_data(self.b23_url)
@@ -354,39 +380,38 @@
                 "avatar_image": f"data:image/png;base64,{base64.b64encode(up.face.getvalue()).decode()}",
                 "name": up.name,
                 "level": level,
                 "name_color": up.name_color,
                 "level_color": f"rgba{level_color}",
                 "fans_count": up.fans,
                 "video_count": up.video_counts,
+                "icon": up.official_verify,
+                "condition": up.title,
             }
-            if up.title:
-                info["condition"] = up.title
             ups.append(info)
 
         template_env = jinja2.Environment(
             loader=jinja2.FileSystemLoader(style_bule),
             enable_async=True,
         )
         template_path = f"file:///{style_bule.joinpath('video-details.html').absolute()}".replace("////", "///")
         template = template_env.get_template("video-details.html")
         html = await template.render_async(
             **{
-                "vanfont": f"file:///{font_vanfont}".replace("////", "///"),
                 "cover_image": f"data:image/png;base64,{base64.b64encode(self.cover.getvalue()).decode()}",
                 "video_category": self.type_name,
                 "video_duration": video_time,
                 "up_infos": ups,
                 "video_title": self.title,
                 "view_count": self.view,
                 "dm_count": self.danmaku,
                 "reply_count": self.reply,
                 "upload_date": self.pubdate.strftime("%Y-%m-%d"),
                 "av_number": self.aid,
-                "video_summary": self.desc.replace("\n","<br>"),
+                "video_summary": self.desc.replace("\n", "<br>"),
                 "like_count": self.like,
                 "coin_count": self.coin,
                 "fav_count": self.favorite,
                 "share_count": self.share,
                 "qr_code_image": f"data:image/png;base64,{base64.b64encode(qr_image.getvalue()).decode()}",
             }
         )
```

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/assets/vanfont.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files 3% similar despite different names*

```diff
@@ -218,17 +218,19 @@
         <img class="cover" src="{{ cover_image }}" />
         <span class="category">{{ video_category }}</span>
         <span class="time">{{ video_duration }}</span>
       </div>
       {% for up_info in up_infos %}
       <div class="up">
         <span class="avatar">
-          <img class="img" src="{{ up_info.avatar_image }}" />
-          {% if up_info.icon %}
-          <img class="icon" src="{{ up_info.icon }}" />
+          <img class="img" src="{{ up_info.avatar_image }}" alt="UP头像" />
+          {% if up_info.icon == 0 %}
+          <img class="icon" src="./assets/personal.png" alt="小闪电认证" />
+          {% elif up_info.icon == 1 %}
+          <img class="icon" src="./assets/business.png" alt="小闪电认证" />
           {% endif %}
         </span>
         <div class="info">
           <span class="name" style="color: {{ up_info.name_color }};"
             >{{ up_info.name }}</span
           >
           <span class="level" style="color: {{ up_info.level_color }};"
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 
 [{{ cover_image }}] {{ video_category }} {{ video_duration }}
 {% for up_info in up_infos %}
- [{{ up_info.avatar_image }}] {% if up_info.icon %} [{{ up_info.icon }}] {%
-endif %}
+ [UPå¤´å] {% if up_info.icon == 0 %} [å°éªçµè®¤è¯] {% elif up_info.icon
+== 1 %} [å°éªçµè®¤è¯] {% endif %}
 {{ up_info.name }} {{ up_info.level }}
 {{ up_info.fans_count }}ç²ä¸ {{ up_info.video_count }}è§é¢
 {% if up_info.condition %}
 {{ up_info.condition }}
 {% endif %}
 {% endfor %}
 {{ video_title }}
```

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.7.3/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.7.2/pyproject.toml` & `nonebot_plugin_bilichat-2.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.7.2"
+version = "2.7.3"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.4",
```

### Comparing `nonebot_plugin_bilichat-2.7.2/PKG-INFO` & `nonebot_plugin_bilichat-2.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.7.2
+Version: 2.7.3
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.7.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.7.3 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-Dist: nonebot-plugin-
 segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-
```

