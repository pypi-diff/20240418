# Comparing `tmp/nonebot_plugin_steam_info-0.1.1.tar.gz` & `tmp/nonebot_plugin_steam_info-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_steam_info-0.1.1.tar", last modified: Fri Mar 15 13:55:28 2024, max compression
+gzip compressed data, was "nonebot_plugin_steam_info-0.1.2.tar", last modified: Thu Apr 18 08:54:29 2024, max compression
```

## Comparing `nonebot_plugin_steam_info-0.1.1.tar` & `nonebot_plugin_steam_info-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1062 2024-03-15 13:55:00.029406 nonebot_plugin_steam_info-0.1.1/LICENSE
--rw-r--r--   0        0        0     2015 2024-03-15 13:55:00.029406 nonebot_plugin_steam_info-0.1.1/README.md
--rw-r--r--   0        0        0     7964 2024-03-15 13:55:00.189406 nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/__init__.py
--rw-r--r--   0        0        0      152 2024-03-15 13:55:00.189406 nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/config.py
--rw-r--r--   0        0        0     4933 2024-03-15 13:55:00.189406 nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/data_source.py
--rw-r--r--   0        0        0    12891 2024-03-15 13:55:00.189406 nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/draw.py
--rw-r--r--   0        0        0      572 2024-03-15 13:55:00.189406 nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/models.py
--rw-r--r--   0        0        0      552 2024-03-15 13:55:00.189406 nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/res/busy.png
--rw-r--r--   0        0        0     1847 2024-03-15 13:55:00.189406 nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/res/friends_search.png
--rw-r--r--   0        0        0     7467 2024-03-15 13:55:00.189406 nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/res/parent_status.png
--rw-r--r--   0        0        0     3409 2024-03-15 13:55:00.189406 nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/res/unknown_avatar.jpg
--rw-r--r--   0        0        0      533 2024-03-15 13:55:00.189406 nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/res/zzz_gaming.png
--rw-r--r--   0        0        0      536 2024-03-15 13:55:00.189406 nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/res/zzz_online.png
--rw-r--r--   0        0        0     1209 2024-03-15 13:55:00.189406 nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/steam.py
--rw-r--r--   0        0        0      580 2024-03-15 13:55:28.297370 nonebot_plugin_steam_info-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2482 1970-01-01 00:00:00.000000 nonebot_plugin_steam_info-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-18 08:54:04.252059 nonebot_plugin_steam_info-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2089 2024-04-18 08:54:04.252059 nonebot_plugin_steam_info-0.1.2/README.md
+-rw-r--r--   0        0        0     7964 2024-04-18 08:54:04.408060 nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-18 08:54:04.408060 nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/config.py
+-rw-r--r--   0        0        0     5091 2024-04-18 08:54:04.408060 nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/data_source.py
+-rw-r--r--   0        0        0    12891 2024-04-18 08:54:04.408060 nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/draw.py
+-rw-r--r--   0        0        0      572 2024-04-18 08:54:04.408060 nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/models.py
+-rw-r--r--   0        0        0      552 2024-04-18 08:54:04.408060 nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/res/busy.png
+-rw-r--r--   0        0        0     1847 2024-04-18 08:54:04.408060 nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/res/friends_search.png
+-rw-r--r--   0        0        0     7467 2024-04-18 08:54:04.408060 nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/res/parent_status.png
+-rw-r--r--   0        0        0     3409 2024-04-18 08:54:04.408060 nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/res/unknown_avatar.jpg
+-rw-r--r--   0        0        0      533 2024-04-18 08:54:04.408060 nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/res/zzz_gaming.png
+-rw-r--r--   0        0        0      536 2024-04-18 08:54:04.408060 nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/res/zzz_online.png
+-rw-r--r--   0        0        0     1209 2024-04-18 08:54:04.408060 nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/steam.py
+-rw-r--r--   0        0        0      580 2024-04-18 08:54:29.224241 nonebot_plugin_steam_info-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2556 1970-01-01 00:00:00.000000 nonebot_plugin_steam_info-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_steam_info-0.1.1/LICENSE` & `nonebot_plugin_steam_info-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.1/README.md` & `nonebot_plugin_steam_info-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 ✨ Steam 好友状态播报 NoneBot 插件 ✨
 
 ## 功能
 - [x] 绑定 Steam ID
 - [x] 群友状态变更播报
 - [x] 主动查询群友状态
 
+## 预览
+仿照了 Steam 好友列表的样式
+
+![image](./preview.png)
+
 ## 使用
 steambind [Steam ID 或 Steam好友代码] -绑定 Steam   
 steaminfo -查看绑定信息   
 steamcheck -查询群友 Steam 状态   
 steamupdate [名称] [图片] -更新群聊头像和名称
 
 > 记得加上你配置的命令头哦
```

### Comparing `nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/__init__.py` & `nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/data_source.py` & `nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/data_source.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,22 @@
             if data["user_id"] == user_id:
                 return data
         return None
 
     def get_all(self, parent_id: str) -> List[str]:
         if parent_id not in self.content:
             return []
-        return [data["steam_id"] for data in self.content[parent_id]]
+
+        result = []
+
+        for data in self.content[parent_id]:
+            if not data["steam_id"] in result:
+                result.append(data["steam_id"])
+
+        return result
 
 
 class SteamInfoData:
     def __init__(self, save_path: Path) -> None:
         self.content: Dict[str, PlayerSummariesResponse] = {}
         self._save_path = save_path
 
@@ -106,27 +113,28 @@
         self.content: Dict[str, str] = {}  # parent_id: name
         self._save_path = save_path
 
         if not save_path.exists():
             save_path.parent.mkdir(parents=True, exist_ok=True)
             self.save()
         else:
-            self.content = json.loads(
-                save_path.read_text("utf-8")
-            )
+            self.content = json.loads(save_path.read_text("utf-8"))
 
     def save(self) -> None:
         with open(self._save_path, "w", encoding="utf-8") as f:
             json.dump(self.content, f, indent=4)
 
     def update(self, parent_id: str, avatar: Image.Image, name: str) -> None:
         self.content[parent_id] = name
         self.save()
         # 保存图片
         avatar_path = self._save_path.parent / f"{parent_id}.png"
         avatar.save(avatar_path)
 
     def get(self, parent_id: str) -> Tuple[Image.Image, str]:
         if parent_id not in self.content:
-            return Image.open("res/unknown_avatar.jpg"), parent_id
+            return (
+                Image.open(Path(__file__).parent / "res/unknown_avatar.jpg"),
+                parent_id,
+            )
         avatar_path = self._save_path.parent / f"{parent_id}.png"
         return Image.open(avatar_path), self.content[parent_id]
```

### Comparing `nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/draw.py` & `nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/models.py` & `nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/res/busy.png` & `nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/res/busy.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/res/friends_search.png` & `nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/res/friends_search.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/res/parent_status.png` & `nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/res/parent_status.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/res/unknown_avatar.jpg` & `nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/res/unknown_avatar.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/res/zzz_gaming.png` & `nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/res/zzz_gaming.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/res/zzz_online.png` & `nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/res/zzz_online.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.1/nonebot_plugin_steam_info/steam.py` & `nonebot_plugin_steam_info-0.1.2/nonebot_plugin_steam_info/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_steam_info-0.1.1/pyproject.toml` & `nonebot_plugin_steam_info-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-steam-info"
-version = "0.1.1"
+version = "0.1.2"
 description = "Default template for PDM package"
 authors = [
     { name = "zhaomaoniu", email = "2667292003@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.2.0",
     "nonebot-plugin-alconna>=0.37.0",
```

### Comparing `nonebot_plugin_steam_info-0.1.1/PKG-INFO` & `nonebot_plugin_steam_info-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-steam-info
-Version: 0.1.1
+Version: 0.1.2
 Summary: Default template for PDM package
 Author-Email: zhaomaoniu <2667292003@qq.com>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: nonebot2>=2.2.0
 Requires-Dist: nonebot-plugin-alconna>=0.37.0
 Requires-Dist: aiohttp>=3.9.3
@@ -17,14 +17,19 @@
 ✨ Steam 好友状态播报 NoneBot 插件 ✨
 
 ## 功能
 - [x] 绑定 Steam ID
 - [x] 群友状态变更播报
 - [x] 主动查询群友状态
 
+## 预览
+仿照了 Steam 好友列表的样式
+
+![image](./preview.png)
+
 ## 使用
 steambind [Steam ID 或 Steam好友代码] -绑定 Steam   
 steaminfo -查看绑定信息   
 steamcheck -查询群友 Steam 状态   
 steamupdate [名称] [图片] -更新群聊头像和名称
 
 > 记得加上你配置的命令头哦
```

