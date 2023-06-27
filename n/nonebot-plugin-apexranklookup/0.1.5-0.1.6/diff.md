# Comparing `tmp/nonebot_plugin_apexranklookup-0.1.5.tar.gz` & `tmp/nonebot_plugin_apexranklookup-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_apexranklookup-0.1.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_apexranklookup-0.1.6.tar", max compression
```

## Comparing `nonebot_plugin_apexranklookup-0.1.5.tar` & `nonebot_plugin_apexranklookup-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1239 2023-03-16 08:25:08.420682 nonebot_plugin_apexranklookup-0.1.5/README.md
--rw-r--r--   0        0        0     3207 2023-03-16 08:25:08.412681 nonebot_plugin_apexranklookup-0.1.5/nonebot_plugin_apexranklookup/__init__.py
--rw-r--r--   0        0        0     3409 2023-03-16 08:25:08.412681 nonebot_plugin_apexranklookup-0.1.5/nonebot_plugin_apexranklookup/api.py
--rw-r--r--   0        0        0      140 2023-03-16 08:25:08.412681 nonebot_plugin_apexranklookup-0.1.5/nonebot_plugin_apexranklookup/config.py
--rwxr-xr-x   0        0        0 10435748 2023-03-16 08:25:08.420682 nonebot_plugin_apexranklookup-0.1.5/nonebot_plugin_apexranklookup/data/font/SourceHanSansCN-Normal.ttf
--rw-r--r--   0        0        0     3215 2023-03-16 08:25:08.420682 nonebot_plugin_apexranklookup-0.1.5/nonebot_plugin_apexranklookup/data/image/base.png
--rw-r--r--   0        0        0     4513 2023-03-16 08:25:08.420682 nonebot_plugin_apexranklookup-0.1.5/nonebot_plugin_apexranklookup/draw.py
--rw-r--r--   0        0        0       85 2023-03-16 08:25:08.420682 nonebot_plugin_apexranklookup-0.1.5/nonebot_plugin_apexranklookup/zh_cn.json
--rw-r--r--   0        0        0      453 2023-03-16 11:20:58.129222 nonebot_plugin_apexranklookup-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2124 1970-01-01 00:00:00.000000 nonebot_plugin_apexranklookup-0.1.5/setup.py
--rw-r--r--   0        0        0     1920 1970-01-01 00:00:00.000000 nonebot_plugin_apexranklookup-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1391 2023-06-26 11:43:51.187627 nonebot_plugin_apexranklookup-0.1.6/README.md
+-rw-r--r--   0        0        0     5923 2023-06-26 11:43:51.195628 nonebot_plugin_apexranklookup-0.1.6/nonebot_plugin_apexranklookup/__init__.py
+-rw-r--r--   0        0        0     2984 2023-06-26 11:43:51.195628 nonebot_plugin_apexranklookup-0.1.6/nonebot_plugin_apexranklookup/api.py
+-rw-r--r--   0        0        0      140 2023-06-27 06:18:43.737089 nonebot_plugin_apexranklookup-0.1.6/nonebot_plugin_apexranklookup/config.py
+-rwxr-xr-x   0        0        0 10435748 2023-03-16 08:25:08.420682 nonebot_plugin_apexranklookup-0.1.6/nonebot_plugin_apexranklookup/data/font/SourceHanSansCN-Normal.ttf
+-rw-r--r--   0        0        0     3215 2023-03-16 08:25:08.420682 nonebot_plugin_apexranklookup-0.1.6/nonebot_plugin_apexranklookup/data/image/base.png
+-rw-r--r--   0        0        0        2 2023-06-26 11:43:51.195628 nonebot_plugin_apexranklookup-0.1.6/nonebot_plugin_apexranklookup/data/user_info.json
+-rw-r--r--   0        0        0     4623 2023-06-26 11:43:51.195628 nonebot_plugin_apexranklookup-0.1.6/nonebot_plugin_apexranklookup/draw.py
+-rw-r--r--   0        0        0       85 2023-03-16 08:25:08.420682 nonebot_plugin_apexranklookup-0.1.6/nonebot_plugin_apexranklookup/zh_cn.json
+-rw-r--r--   0        0        0      453 2023-06-27 06:18:54.293141 nonebot_plugin_apexranklookup-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 nonebot_plugin_apexranklookup-0.1.6/setup.py
+-rw-r--r--   0        0        0     2072 1970-01-01 00:00:00.000000 nonebot_plugin_apexranklookup-0.1.6/PKG-INFO
```

### Comparing `nonebot_plugin_apexranklookup-0.1.5/README.md` & `nonebot_plugin_apexranklookup-0.1.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -28,28 +28,37 @@
 查询当前复制器轮换物品。
 ![](./image/crafting.png)
 
 #### .pd/.猎杀
 查询全平台大逃杀、竞技场猎杀最低分和大师段位以上的人数。
 ![](./image/pd.png)
 
+#### .bind/.绑定
+origin id 与qq绑定，实现更方便的查询。
+![](./image/bind.png)
+
+#### .unbind/.解绑
+解除绑定
+
 ### 图片自定义
 /data/image/base.png 为玩家信息的背景底色，可以660*750大小替换。
 
 /data/font/SourceHanSansCN-Normal.ttf 为默认字体，也可替换，之后去draw.py修改路径。
 
 更多样式修改详见draw.py
 
 ## TODO
 > 中文文本翻译
 > 
 > ~~输出美化~~
 > 
-> 追踪器输出优化
+> ~~追踪器输出优化~~
+> 
+> ~~添加绑定功能~~
 > 
-> 添加绑定、订阅功能
+> 添加订阅功能
 
 ## 致谢
 
 https://apexlegendsapi.com/
 
 https://github.com/Shennoter/ApexRankLookUp
```

### Comparing `nonebot_plugin_apexranklookup-0.1.5/nonebot_plugin_apexranklookup/api.py` & `nonebot_plugin_apexranklookup-0.1.6/nonebot_plugin_apexranklookup/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,18 +17,18 @@
         elif platform.lower() == "pc":
             platform = "PC"
         else:
             return "请输入正确的平台(pc,xbox,ps)"
         try:
             r = requests.get(f"{self.url}/bridge?auth={self.api_key}&player={user_id}&platform={platform}&merge=True&removeMerged=True&version=5")
         except Exception:
-            return "网络爆炸了，请稍后重试或联系管理员"
+            return "Error:" + "网络爆炸了，请稍后重试或联系管理员"
         result = json.loads(r.text)
         if result.get("Error"):
-            return result.get("Error")
+            return "Error: " + result.get("Error")
         msg = str(MessageSegment.image(draw_profile(result)))
         return msg
 
     def map_query(self):
         try:
             r = requests.get(f"{self.url}/maprotation?auth={self.api_key}&version=2")
         except Exception:
@@ -48,19 +48,15 @@
         if result.get("Error"):
             return result.get("Error")
         msg = f"""大逃杀：
 PC: 最低分 {result.get("RP").get("PC").get("val")}, 大师 {result.get("RP").get("PC").get("totalMastersAndPreds")}
 PS: 最低分 {result.get("RP").get("PS4").get("val")}, 大师 {result.get("RP").get("PS4").get("totalMastersAndPreds")}
 Xbox: 最低分 {result.get("RP").get("X1").get("val")}, 大师 {result.get("RP").get("X1").get("totalMastersAndPreds")}
 Switch: 最低分 {result.get("RP").get("SWITCH").get("val")}, 大师 {result.get("RP").get("SWITCH").get("totalMastersAndPreds")}
-竞技场：
-PC: 最低分 {result.get("AP").get("PC").get("val")}, 大师 {result.get("AP").get("PC").get("totalMastersAndPreds")}
-PS: 最低分 {result.get("AP").get("PS4").get("val")}, 大师 {result.get("AP").get("PS4").get("totalMastersAndPreds")}
-Xbox: 最低分 {result.get("AP").get("X1").get("val")}, 大师 {result.get("AP").get("X1").get("totalMastersAndPreds")}
-Switch: 最低分 {result.get("AP").get("SWITCH").get("val")}, 大师 {result.get("AP").get("SWITCH").get("totalMastersAndPreds")}"""
+"""
         return msg
 
     def store_query(self):
         try:
             r = requests.get(f"{self.url}/crafting?auth={self.api_key}")
         except Exception:
             return "网络爆炸了，请稍后重试或联系管理员"
@@ -69,9 +65,10 @@
 {" ".join(str(MessageSegment.image(i.get("itemType").get("asset"))) for i in result[0].get("bundleContent"))}
 {" ".join(str(MessageSegment.image(i.get("itemType").get("asset"))) for i in result[1].get("bundleContent"))}"""
         return msg
 
 
 if __name__ == "__main__":
     api = apexApi("")
-    api.player_query("", "PC")
-    # print(api.map_query())
+    # api.player_query("Paradisesssssa", "PC")
+    # api.player_query("TTV_WeThePeople1", "PC")
+    api.map_query()
```

### Comparing `nonebot_plugin_apexranklookup-0.1.5/nonebot_plugin_apexranklookup/data/font/SourceHanSansCN-Normal.ttf` & `nonebot_plugin_apexranklookup-0.1.6/nonebot_plugin_apexranklookup/data/font/SourceHanSansCN-Normal.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_apexranklookup-0.1.5/nonebot_plugin_apexranklookup/data/image/base.png` & `nonebot_plugin_apexranklookup-0.1.6/nonebot_plugin_apexranklookup/data/image/base.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_apexranklookup-0.1.5/nonebot_plugin_apexranklookup/draw.py` & `nonebot_plugin_apexranklookup-0.1.6/nonebot_plugin_apexranklookup/draw.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from PIL import Image
 from PIL import ImageDraw, ImageFont
 import os
 import requests
 import io
 
 dirname, filename = os.path.split(os.path.abspath(__file__))
-font = ImageFont.truetype(f"{dirname}/data/font/SourceHanSansCN-Normal.ttf", 50)
+font = ImageFont.truetype(f"{dirname}/data/font/SourceHanSansCN-Normal.ttf", 80)
 
 
 def image_cache(url):
     filename = url.split("/")[-1]
+    if not filename:
+        filename = "Olympus.png"
     if not os.path.exists(f"{dirname}/data/image/{filename}"):
         with open(f"{dirname}/data/image/{filename}", "wb") as f:
             r = requests.get(url, stream=True)
             for chunk in r.iter_content(chunk_size=32):
                 f.write(chunk)
     return Image.open(f"{dirname}/data/image/{filename}")
 
@@ -25,56 +27,57 @@
         h = int((max_widen/iw) * ih)
         result.append(image.resize((max_widen, h), Image.BICUBIC))
     return result
 
 
 def draw_rank(img, rank):
     draw = ImageDraw.Draw(img)
-    draw.text(xy=(img.size[0] // 2 - 50, img.size[1] // 2 + 90), text="#" + str(rank), fill='white', font=font)
+    text = "#" + str(rank)
+    if rank > 750:
+        draw.text(xy=((img.size[0]-font.getsize(text)[0]) // 2, (img.size[1]-font.getsize(text)[1]) // 2 + 250), text=text, fill='white', font=font)
+    else:
+        pred_font = ImageFont.truetype(f"{dirname}/data/font/SourceHanSansCN-Normal.ttf", 50)
+        draw.text(xy=((img.size[0]-pred_font.getsize(text)[0]) // 2, (img.size[1]-pred_font.getsize(text)[1]) // 2 + 120), text=text, fill='white', font=pred_font)
     return img
 
 
 def draw_profile(data):
     img_leged = image_trans(image_cache(data.get("legends").get("selected").get("ImgAssets").get("icon")))
     result = Image.open(f"{dirname}/data/image/base.png")
     result.paste(img_leged, box=(0, 0), mask=img_leged)
     img_rank = image_cache(data.get("global").get("rank").get("rankImg"))
-    if data.get("global").get("rank").get("rankName") == "Apex Predator":
+    if data.get("global").get("rank").get("rankName") in ["Apex Predator", "Master"]:
         img_rank = draw_rank(img_rank, data.get("global").get("rank").get("ladderPosPlatform"))
     # img_rank.show()
     draw = ImageDraw.Draw(result)
     profile_font = ImageFont.truetype(f"{dirname}/data/font/SourceHanSansCN-Normal.ttf", 20)
     img_rank = image_trans(pad_image([img_rank], 150)[0])
     result.paste(img_rank, box=(0, 0), mask=img_rank)
     draw.text(xy=(40, 150), text=str(data.get("global").get("rank").get("rankScore")) + "pt", fill='white', font=profile_font)
-    img_arena = image_cache(data.get("global").get("arena").get("rankImg"))
-    if data.get("global").get("arena").get("rankName") == "Apex Predator":
-        img_arena = draw_rank(img_arena, data.get("global").get("arena").get("ladderPosPlatform"))
-    img_arena = image_trans(pad_image([img_arena], 150)[0])
-    result.paste(img_arena, box=(0, 200), mask=img_arena)
-    draw.text(xy=(40, 350), text=str(data.get("global").get("arena").get("rankScore")) + "pt", fill='white', font=profile_font)
     level_text = f'id： {data.get("global").get("name")}\n等级：{data.get("global").get("level")}\n{data.get("realtime").get("currentStateAsText")}'
-    draw.text(xy=(result.size[0]-200, 0), text=level_text, fill='white', font=profile_font)
+    draw.text(xy=(result.size[0]-draw.textsize(level_text, profile_font)[0], 0), text=level_text, fill='white', font=profile_font)
     badges_text = "\n".join([f'{i.get("name")}:{i.get("value")}' for i in data.get("legends").get("selected").get("gameInfo").get("badges")])
-    draw.text(xy=(result.size[0] - 200, result.size[1] - 150), text="追踪器:\n" + ("无" if not badges_text else badges_text), fill='white', font=profile_font)
+    draw.text(xy=(result.size[0]-draw.textsize(badges_text, profile_font)[0], result.size[1]-draw.textsize(badges_text, profile_font)[1]), text="追踪器:\n" + ("无" if not badges_text else badges_text), fill='white', font=profile_font)
     b = io.BytesIO()
     result.save(b, 'png')
+    with open("test.png", "wb") as f:
+        result.save(f, "png")
     return b.getvalue()
 
 
 def image_trans(image):
     image = image.convert("RGBA")
     fg_img_trans = Image.new("RGBA", image.size)
     fg_img_trans = Image.blend(fg_img_trans, image, 1)
     return fg_img_trans
 
 
 def draw_map(data):  # 3840*1200
     images = []
-    map_type = ["battle_royale", "arenas", "ranked", "arenasRanked"]
+    map_type = ["battle_royale", "ranked", "ltm"]
     for index in map_type:
         images.append(image_cache(data.get(index).get("current").get("asset")))
     length = 0  # 空白长图的长
     max_widen = 999999  # 空白长图的宽
     for i in images:
         if max_widen > i.size[0]:
             max_widen = i.size[0]
@@ -86,15 +89,15 @@
     length = 0
     for i in range(len(images)):
         image = images[i]
         result.paste(image, box=(0, length))
         text = f'模式:{map_type[i]}\n当前地图：{data.get(map_type[i]).get("current").get("map")}\n下张地图：{data.get(map_type[i]).get("next").get("map")}\n剩余时间：{data.get(map_type[i]).get("current").get("remainingTimer")}'
         length += image.size[1]
         # 在图片上写字：位置(x左右，y上下)，文字，颜色，字体
-        draw.text(xy=(0, length - 250), text=text, fill='white', font=font)
+        draw.text(xy=(0, length - draw.textsize(text, font)[1]), text=text, fill='white', font=font)
     result = pad_image([result], 800)[0]
     b = io.BytesIO()
     result.save(b, 'png')
     return b.getvalue()
 
 
 if __name__ == "__main__":
```

### Comparing `nonebot_plugin_apexranklookup-0.1.5/setup.py` & `nonebot_plugin_apexranklookup-0.1.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['nonebot_plugin_apexranklookup']
 
 package_data = \
-{'': ['*'], 'nonebot_plugin_apexranklookup': ['data/font/*', 'data/image/*']}
+{'': ['*'],
+ 'nonebot_plugin_apexranklookup': ['data/*', 'data/font/*', 'data/image/*']}
 
 install_requires = \
 ['Pillow>=9.4.0,<10.0.0',
  'loguru>=0.6.0,<0.7.0',
  'nonebot-adapter-onebot>=2.2.1,<3.0.0',
  'nonebot2>=2.0.0rc3,<3.0.0',
  'pydantic>=1.10.6,<2.0.0',
  'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-apexranklookup',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': '',
-    'long_description': '## nonebot_plugin_apexranklookup\n\n一个基于nonebot的插件，用于查询Apex英雄的\n\n> 地图轮换\n> \n> 玩家信息\n> \n> 复制器\n> \n> 猎杀门槛\n\n## api key申请\n在https://apexlegendsapi.com/ 获取APIkey填入.env 或者config.py中\n`apex_api_token`\n\n## 使用\n#### .map/.地图\n查看当前大逃杀、竞技场模式轮换地图，以及地图剩余时间。\n![](./image/map.png)\n#### .stat/.查询 origin_id (平台)\n根据origin_id查询玩家信息（id、等级、段位、当前状态）\n\n可查询多平台(PC、PS4、X1)，不添加默认PC\n![](./image/stat.png)\n\n#### .crafting/.复制器\n查询当前复制器轮换物品。\n![](./image/crafting.png)\n\n#### .pd/.猎杀\n查询全平台大逃杀、竞技场猎杀最低分和大师段位以上的人数。\n![](./image/pd.png)\n\n### 图片自定义\n/data/image/base.png 为玩家信息的背景底色，可以660*750大小替换。\n\n/data/font/SourceHanSansCN-Normal.ttf 为默认字体，也可替换，之后去draw.py修改路径。\n\n更多样式修改详见draw.py\n\n## TODO\n> 中文文本翻译\n> \n> ~~输出美化~~\n> \n> 追踪器输出优化\n> \n> 添加绑定、订阅功能\n\n## 致谢\n\nhttps://apexlegendsapi.com/\n\nhttps://github.com/Shennoter/ApexRankLookUp\n',
+    'long_description': '## nonebot_plugin_apexranklookup\n\n一个基于nonebot的插件，用于查询Apex英雄的\n\n> 地图轮换\n> \n> 玩家信息\n> \n> 复制器\n> \n> 猎杀门槛\n\n## api key申请\n在https://apexlegendsapi.com/ 获取APIkey填入.env 或者config.py中\n`apex_api_token`\n\n## 使用\n#### .map/.地图\n查看当前大逃杀、竞技场模式轮换地图，以及地图剩余时间。\n![](./image/map.png)\n#### .stat/.查询 origin_id (平台)\n根据origin_id查询玩家信息（id、等级、段位、当前状态）\n\n可查询多平台(PC、PS4、X1)，不添加默认PC\n![](./image/stat.png)\n\n#### .crafting/.复制器\n查询当前复制器轮换物品。\n![](./image/crafting.png)\n\n#### .pd/.猎杀\n查询全平台大逃杀、竞技场猎杀最低分和大师段位以上的人数。\n![](./image/pd.png)\n\n#### .bind/.绑定\norigin id 与qq绑定，实现更方便的查询。\n![](./image/bind.png)\n\n#### .unbind/.解绑\n解除绑定\n\n### 图片自定义\n/data/image/base.png 为玩家信息的背景底色，可以660*750大小替换。\n\n/data/font/SourceHanSansCN-Normal.ttf 为默认字体，也可替换，之后去draw.py修改路径。\n\n更多样式修改详见draw.py\n\n## TODO\n> 中文文本翻译\n> \n> ~~输出美化~~\n> \n> ~~追踪器输出优化~~\n> \n> ~~添加绑定功能~~\n> \n> 添加订阅功能\n\n## 致谢\n\nhttps://apexlegendsapi.com/\n\nhttps://github.com/Shennoter/ApexRankLookUp\n',
     'author': 'Windylh',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `nonebot_plugin_apexranklookup-0.1.5/PKG-INFO` & `nonebot_plugin_apexranklookup-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-apexranklookup
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Windylh
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -47,29 +47,38 @@
 查询当前复制器轮换物品。
 ![](./image/crafting.png)
 
 #### .pd/.猎杀
 查询全平台大逃杀、竞技场猎杀最低分和大师段位以上的人数。
 ![](./image/pd.png)
 
+#### .bind/.绑定
+origin id 与qq绑定，实现更方便的查询。
+![](./image/bind.png)
+
+#### .unbind/.解绑
+解除绑定
+
 ### 图片自定义
 /data/image/base.png 为玩家信息的背景底色，可以660*750大小替换。
 
 /data/font/SourceHanSansCN-Normal.ttf 为默认字体，也可替换，之后去draw.py修改路径。
 
 更多样式修改详见draw.py
 
 ## TODO
 > 中文文本翻译
 > 
 > ~~输出美化~~
 > 
-> 追踪器输出优化
+> ~~追踪器输出优化~~
+> 
+> ~~添加绑定功能~~
 > 
-> 添加绑定、订阅功能
+> 添加订阅功能
 
 ## 致谢
 
 https://apexlegendsapi.com/
 
 https://github.com/Shennoter/ApexRankLookUp
```

