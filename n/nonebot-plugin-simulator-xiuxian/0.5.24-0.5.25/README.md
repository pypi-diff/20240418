# Comparing `tmp/nonebot_plugin_simulator_xiuxian-0.5.24.tar.gz` & `tmp/nonebot_plugin_simulator_xiuxian-0.5.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_simulator_xiuxian-0.5.24.tar", last modified: Fri Apr 12 14:21:16 2024, max compression
+gzip compressed data, was "nonebot_plugin_simulator_xiuxian-0.5.25.tar", last modified: Thu Apr 18 19:05:24 2024, max compression
```

## Comparing `nonebot_plugin_simulator_xiuxian-0.5.24.tar` & `nonebot_plugin_simulator_xiuxian-0.5.25.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 14:21:16.035685 nonebot_plugin_simulator_xiuxian-0.5.24/
--rw-rw-rw-   0        0        0      264 2024-04-12 14:21:16.035685 nonebot_plugin_simulator_xiuxian-0.5.24/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-12 14:21:16.026684 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/
--rw-rw-rw-   0        0        0     2028 2023-03-16 11:20:54.000000 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/__init__.py
--rw-rw-rw-   0        0        0     1960 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/cd_manager.py
--rw-rw-rw-   0        0        0      358 2023-03-13 16:40:54.000000 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/config.py
--rw-rw-rw-   0        0        0     2849 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/data_source.py
--rw-rw-rw-   0        0        0     1787 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/exp_util.py
--rw-rw-rw-   0        0        0      101 2023-07-14 16:18:51.000000 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/help.py
--rw-rw-rw-   0        0        0     4430 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/item_json.py
--rw-rw-rw-   0        0        0    50728 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/player_fight.py
--rw-rw-rw-   0        0        0     8141 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/read_buff.py
--rw-rw-rw-   0        0        0     8555 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/utils.py
--rw-rw-rw-   0        0        0    55510 2023-06-22 17:42:27.000000 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/xiuxian2_handle.py
--rw-rw-rw-   0        0        0     5814 2023-07-14 16:11:36.000000 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/xiuxian_config.py
--rw-rw-rw-   0        0        0      787 2023-03-13 15:11:10.000000 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/xiuxian_opertion.py
--rw-rw-rw-   0        0        0     2475 2024-04-12 14:05:42.000000 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/xiuxian_xiazaishuju.py
-drwxrwxrwx   0        0        0        0 2024-04-12 14:21:16.034685 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian.egg-info/
--rw-rw-rw-   0        0        0      264 2024-04-12 14:21:15.000000 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      951 2024-04-12 14:21:15.000000 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 14:21:15.000000 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-04-12 14:21:15.000000 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2024-04-12 14:21:15.000000 nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 14:21:16.035685 nonebot_plugin_simulator_xiuxian-0.5.24/setup.cfg
--rw-rw-rw-   0        0        0      592 2024-04-12 14:16:47.000000 nonebot_plugin_simulator_xiuxian-0.5.24/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:05:24.225834 nonebot_plugin_simulator_xiuxian-0.5.25/
+-rw-rw-rw-   0        0        0      265 2024-04-18 19:05:24.225834 nonebot_plugin_simulator_xiuxian-0.5.25/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-18 19:05:24.208930 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/
+-rw-rw-rw-   0        0        0     2040 2024-04-17 16:39:11.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/__init__.py
+-rw-rw-rw-   0        0        0     1960 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/cd_manager.py
+-rw-rw-rw-   0        0        0      358 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/config.py
+-rw-rw-rw-   0        0        0     2849 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/data_source.py
+-rw-rw-rw-   0        0        0     1787 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/exp_util.py
+-rw-rw-rw-   0        0        0     1354 2024-04-18 19:00:35.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/help.py
+-rw-rw-rw-   0        0        0     4430 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/item_json.py
+-rw-rw-rw-   0        0        0    50728 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/player_fight.py
+-rw-rw-rw-   0        0        0     8141 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/read_buff.py
+-rw-rw-rw-   0        0        0     8555 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/utils.py
+-rw-rw-rw-   0        0        0    54291 2024-04-18 18:05:50.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/xiuxian2_handle.py
+-rw-rw-rw-   0        0        0     5780 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/xiuxian_config.py
+-rw-rw-rw-   0        0        0      787 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/xiuxian_opertion.py
+-rw-rw-rw-   0        0        0     2477 2023-08-18 15:32:44.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/xiuxian_xiazaishuju.py
+drwxrwxrwx   0        0        0        0 2024-04-18 19:05:24.224834 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian.egg-info/
+-rw-rw-rw-   0        0        0      265 2024-04-18 19:05:24.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      951 2024-04-18 19:05:24.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 19:05:24.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-04-18 19:05:24.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       33 2024-04-18 19:05:24.000000 nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-18 19:05:24.226836 nonebot_plugin_simulator_xiuxian-0.5.25/setup.cfg
+-rw-rw-rw-   0        0        0      593 2024-04-18 19:04:58.000000 nonebot_plugin_simulator_xiuxian-0.5.25/setup.py
```

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/__init__.py` & `nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,27 +31,27 @@
     logger.info(f"下载配置文件失败，修仙插件无法加载，{e}!")
     raise ImportError
 
 
 require('nonebot_plugin_apscheduler')
 
 
-src = ''                              # src = ''内应当是插件上级目录+插件保存地址,注意地址之接连接用. 
+src = 'src.plugins.'                              # src = ''内应当是插件上级目录+插件保存地址,注意地址之接连接用. 
 load_all_plugins(
         [
             f'{src}nonebot_plugin_simulator_xiuxian.xiuxian_boss',
             f'{src}nonebot_plugin_simulator_xiuxian.xiuxian_bank',
             f'{src}nonebot_plugin_simulator_xiuxian.xiuxian_sect',
-            f'{src}nonebot_plugin_simulator_xiuxian.xiuxian_base',
             f'{src}nonebot_plugin_simulator_xiuxian.xiuxian_info',
             f'{src}nonebot_plugin_simulator_xiuxian.xiuxian_buff',
             f'{src}nonebot_plugin_simulator_xiuxian.xiuxian_back',
             f'{src}nonebot_plugin_simulator_xiuxian.xiuxian_rift',
             f'{src}nonebot_plugin_simulator_xiuxian.xiuxian_mixelixir',
             f'{src}nonebot_plugin_simulator_xiuxian.xiuxian_work',
+            f'{src}nonebot_plugin_simulator_xiuxian.xiuxian_base',
         ],
         [],
     )
 
 
 
 __plugin_meta__ = PluginMetadata(
```

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/cd_manager.py` & `nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/cd_manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/data_source.py` & `nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/exp_util.py` & `nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/exp_util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/item_json.py` & `nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/item_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/player_fight.py` & `nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/player_fight.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/read_buff.py` & `nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/read_buff.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/utils.py` & `nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/xiuxian2_handle.py` & `nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/xiuxian2_handle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1086,14 +1086,32 @@
         goods_num = back.goods_num - num
         now_time = datetime.datetime.now()
         sql_str = f"UPDATE back set update_time='{now_time}',action_time='{now_time}',goods_num={goods_num},day_num={day_num},all_num={all_num},bind_num={bind_num} WHERE user_id={user_id} and goods_id={goods_id}"
         cur = self.conn.cursor()
         cur.execute(sql_str)
         self.conn.commit()
 
+
+
+    def xito(self):
+        uba = random.randint(1,2)
+        ubb = random.randint(1,2)
+        ubs = int(uba - ubb) 
+        return int(ubs)   
+
+    def lingg(self, user_id):
+        cur = self.conn.cursor()
+        print(user_id)
+        sql = f"UPDATE user_xiuxian SET root=?,root_type=? where user_id=?"
+        cur.execute(sql, ("玄灵根", "五相灵根", user_id))
+        self.conn.commit()
+        return "系统修改了你的灵根，新的灵根为：玄灵根，类型为：五相灵根"
+
+
+
 class XiuxianJsonDate:
     def __init__(self):
         self.root_jsonpath = DATABASE / "灵根.json"
         self.level_jsonpath = DATABASE / "突破概率.json"
         self.do_work_jsonpath = DATABASE / "悬赏令.json"
 
     def beifen_linggen_get(self):
@@ -1413,53 +1431,7 @@
     user_data[17] = int(user_data[17] * (user_data[18] * 0.04 + 1) * (1 + main_atk_buff) * (1 + weapon_atk_buff)) + user_buff_data.atk_buff#每级+10%攻击
     user_data = tuple(user_data)
     return user_data
     
     
 if __name__ == '__main__':
     print(OtherSet().date_diff("2022-09-08 00:42:56.740255", "2022-09-08 00:42:56.740255"))
-
-    # paths = r"G:\yuzi_bot\yuzi_bot\data\xiuxian\悬赏令.json"
-    # with open(paths, 'r', encoding='utf-8') as e:
-    #     a = e.read()
-    #     data = json.loads(a)
-    #     get_work_list = []
-    #     for i in data:
-    #         name = random.choice(list(data[i].keys()))
-    #         get_work_list.append([name,data[i][name]["rate"],data[i][name]["succeed_thank"]])
-    #     print(get_work_list)
-    #
-    #     work_event = None
-    #     for i, v in data.items():
-    #         for vk, vv in v.items():
-    #             if vk == get_work_list[0][0]:
-    #                 work_event = vv
-    #
-    #     print(work_event["rate"])
-    #     if random.randint(1, 100) <= work_event["rate"]:
-    #         print(random.choice( work_event["succeed"]), work_event["succeed_thank"])
-    #     else:
-    #         print (random.choice(work_event["fail"]), work_event["fail_thank"])
-
-#     apath = r"G:\yuzi_bot\yuzi_bot\data\xiuxian\xiuxian.db"
-#     conn = sqlite3.connect(apath)
-#     sql = f"""SELECT user_name,level,exp FROM user_xiuxian
-# WHERE user_name is NOT NULL
-# ORDER BY CASE
-# WHEN level = '筑基境圆满' THEN '1'
-# WHEN level = '筑基境中期' THEN '2'
-# WHEN level = '筑基境初期' THEN '3'
-# WHEN level = '练气境圆满' THEN '4'
-# WHEN level = '练气境中期' THEN '5'
-# WHEN level = '练气境初期' THEN '6'
-# WHEN level = '江湖好手' THEN '7'
-# ELSE level END ASC,exp DESC LIMIT 5"""
-#     cur = conn.cursor()
-#     cur.execute(sql,)
-#     result = cur.fetchall()
-#     mess = f"位面境界排行榜TOP5\n"
-#     num=0
-#     for i in result:
-#         num+=1
-#         mess += F"TOP{num}:{i[0]},境界：{i[1]},修为：{i[2]}\n"
-#
-#     print(mess)
```

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/xiuxian_config.py` & `nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/xiuxian_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,59 +2,14 @@
     import ujson as json
 except ImportError:
     import json
 from pathlib import Path
 
 DATABASE = Path() / "data" / "xiuxian"
 
-
-USERRANK = {
-    '江湖好手':50,
-    '练气境初期':49,
-    '练气境中期':48,
-    '练气境圆满':47,
-    '筑基境初期':46,
-    '筑基境中期':45,
-    '筑基境圆满':44,
-    '结丹境初期':43,
-    '结丹境中期':42,
-    '结丹境圆满':41,
-    '元婴境初期':40,
-    '元婴境中期':39,
-    '元婴境圆满':38,
-    '化神境初期':37,
-    '化神境中期':36,
-    '化神境圆满':35,
-    '炼虚境初期':34,
-    '炼虚境中期':33,
-    '炼虚境圆满':32,
-    '合体境初期':31,
-    '合体境中期':30,
-    '合体境圆满':29,
-    '大乘境初期':28,
-    '大乘境中期':27,
-    '大乘境圆满':26,
-    '渡劫境初期':25,
-    '渡劫境中期':24,
-    '渡劫境圆满':23,
-    '半步真仙':22,
-    '真仙境初期':21,
-    '真仙境中期':20,
-    '真仙境圆满':19,
-    '金仙境初期':18,
-    '金仙境中期':17,
-    '金仙境圆满':16,
-    '太乙境初期':15,
-    '太乙境中期':14,
-    '太乙境圆满':13,
-    '真仙境初期':12,
-    '悟道境': 11,
-}
-
-
 class XiuConfig:
 
     def __init__(self):
 
 
         self.level = list(USERRANK.keys())
         self.level_up_cd = 60  # 突破CD(分钟)
@@ -74,15 +29,15 @@
         self.sect_min_level = "渡劫境初期"  # 创建宗门的最低修为等级要求
         self.sect_create_cost = 25  # 创建宗门的最低修为等级要求
         self.user_info_cd = 10  # 我的修仙信息查询cd
         self.user_info_cd_msg = 5
         self.dufang_cd_msg = 5
         self.tou_cd = 5  # 偷灵石CD
         self.battle_boss_cd = 60  # 讨伐bossCD
-        self.version = "xinxian_1.1"
+        self.version = "xiuxian_1.1"
 
         self.sql_table = ["user_xiuxian", "user_cd", "sects", "back", "BuffInfo"]  # 数据库表校验
         self.sql_user_xiuxian = ["level_up_rate","sect_id","sect_position"
                                  ,"hp", "mp", "atk", "atkpractice", "sect_task",
                                 "sect_contribution","sect_elixir_get", 
                                 "blessed_spot_flag","blessed_spot_name"]   # 数据库字段校验
         self.sql_sects = ["sect_materials", "mainbuff", "secbuff", "elixir_room_level"]
@@ -136,15 +91,55 @@
                         return False
             except KeyError:
                 json_data['group'] = [group_id]
 
         with open(self.config_jsonpath, 'w', encoding='utf-8') as f:
             json.dump(json_data, f)
 
-
+USERRANK = {
+    '江湖好手':50,
+    '练气境初期':49,
+    '练气境中期':48,
+    '练气境圆满':47,
+    '筑基境初期':46,
+    '筑基境中期':45,
+    '筑基境圆满':44,
+    '结丹境初期':43,
+    '结丹境中期':42,
+    '结丹境圆满':41,
+    '元婴境初期':40,
+    '元婴境中期':39,
+    '元婴境圆满':38,
+    '化神境初期':37,
+    '化神境中期':36,
+    '化神境圆满':35,
+    '炼虚境初期':34,
+    '炼虚境中期':33,
+    '炼虚境圆满':32,
+    '合体境初期':31,
+    '合体境中期':30,
+    '合体境圆满':29,
+    '大乘境初期':28,
+    '大乘境中期':27,
+    '大乘境圆满':26,
+    '渡劫境初期':25,
+    '渡劫境中期':24,
+    '渡劫境圆满':23,
+    '半步真仙':22,
+    '真仙境初期':21,
+    '真仙境中期':20,
+    '真仙境圆满':19,
+    '金仙境初期':18,
+    '金仙境中期':17,
+    '金仙境圆满':16,
+    '太乙境初期':15,
+    '太乙境中期':14,
+    '太乙境圆满':13,
+    '悟道境':12,
+}
 
 if __name__ == '__main__':
     pathname = r""
     with open(pathname, 'r', encoding='utf-8') as e:
         data = json.load(e)
 
     key = 4
@@ -164,8 +159,8 @@
                     dd.remove('123')
                 except ValueError:
                     print('bbbb')
         except KeyError:
             data['group'] = []
 
     with open(pathname, 'w', encoding='utf-8') as f:
-        json.dump(data, f)
+        json.dump(data, f)
```

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/xiuxian_opertion.py` & `nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/xiuxian_opertion.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian/xiuxian_xiazaishuju.py` & `nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian/xiuxian_xiazaishuju.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .xiuxian_config import XiuConfig
 
 
 def download_xiuxian_data():
     path_data = Path() / "data"
     zipPath = str(path_data / "xiuxian_data_temp.zip")  # 压缩包的绝对路径
     version = "xiuxian_version.txt"
-    URL = "https://codeload.github.com/luoyefufeng/xiuxian/zip/refs/heads/main"
+    URL = "https://huggingface.co/luoyefufeng/xiuxian_1/resolve/main/xiuxian.zip"
 
     def get_data():
         wget.download(URL, out=zipPath)  # 获取内容
 
     def _main_():
         if not os.path.exists(path_data):
             os.makedirs(path_data)
```

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.24/nonebot_plugin_simulator_xiuxian.egg-info/SOURCES.txt` & `nonebot_plugin_simulator_xiuxian-0.5.25/nonebot_plugin_simulator_xiuxian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_simulator_xiuxian-0.5.24/setup.py` & `nonebot_plugin_simulator_xiuxian-0.5.25/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_namespace_packages,find_packages
 
 setup(
 name='nonebot_plugin_simulator_xiuxian',
-version='0.5.24',
+version='0.5.25',
 description='修仙',
 #long_description=open('README.md','r').read(),
-author='luoyefufeng',
+author='甘城菜月',
 author_email='2859385794@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_simulator_xiuxian"]),
 platforms='all',
 install_requires=["nonebot2","nonebot-adapter-onebot",'wget',"nonebot_plugin_apscheduler"],
 url='https://github.com/luoyefufeng/nonebot_plugin_simulator_xiuxian',
```

