# Comparing `tmp/grabberlib-0.0.1.tar.gz` & `tmp/grabberlib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grabberlib-0.0.1.tar", max compression
+gzip compressed data, was "grabberlib-0.0.3.tar", max compression
```

## Comparing `grabberlib-0.0.1.tar` & `grabberlib-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,19 @@
--rw-r--r--   0        0        0        0 2024-04-18 15:32:29.439621 grabberlib-0.0.1/README.md
--rw-r--r--   0        0        0     5679 2024-04-17 22:31:34.748201 grabberlib-0.0.1/assets/telegraph_pages.txt
--rw-r--r--   0        0        0        0 2024-04-15 17:38:47.146959 grabberlib-0.0.1/grabber/__init__.py
--rw-r--r--   0        0        0       76 2024-04-18 15:49:34.558594 grabberlib-0.0.1/grabber/__main__.py
--rw-r--r--   0        0        0     5479 2024-04-18 15:45:37.870025 grabberlib-0.0.1/grabber/entrypoint.py
--rw-r--r--   0        0        0     3563 2024-04-18 15:44:52.496605 grabberlib-0.0.1/grabber/graph.py
--rw-r--r--   0        0        0     3967 2024-04-18 15:45:10.597010 grabberlib-0.0.1/grabber/khd.py
--rw-r--r--   0        0        0      181 2024-04-17 22:05:44.064553 grabberlib-0.0.1/grabber/settings.py
--rw-r--r--   0        0        0     9424 2024-04-18 15:45:24.759556 grabberlib-0.0.1/grabber/utils.py
--rw-r--r--   0        0        0     1967 2024-04-18 15:45:16.870319 grabberlib-0.0.1/grabber/yellow.py
--rw-r--r--   0        0        0      974 2024-04-18 15:57:36.231481 grabberlib-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1189 1970-01-01 00:00:00.000000 grabberlib-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-18 15:32:29.439621 grabberlib-0.0.3/README.md
+-rw-r--r--   0        0        0     6140 2024-04-18 21:16:51.421239 grabberlib-0.0.3/assets/pages.txt
+-rw-r--r--   0        0        0        0 2024-04-15 17:38:47.146959 grabberlib-0.0.3/grabber/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-18 21:14:28.281973 grabberlib-0.0.3/grabber/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-18 20:26:25.002814 grabberlib-0.0.3/grabber/controllers/__init__.py
+-rw-r--r--   0        0        0     2831 2024-04-18 21:14:28.281125 grabberlib-0.0.3/grabber/controllers/base.py
+-rw-r--r--   0        0        0        0 2024-04-18 20:26:36.846498 grabberlib-0.0.3/grabber/core/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-18 21:14:28.281820 grabberlib-0.0.3/grabber/core/exc.py
+-rw-r--r--   0        0        0      181 2024-04-17 22:05:44.064553 grabberlib-0.0.3/grabber/core/settings.py
+-rw-r--r--   0        0        0        0 2024-04-18 20:50:40.150458 grabberlib-0.0.3/grabber/core/sources/__init__.py
+-rw-r--r--   0        0        0     3545 2024-04-18 21:14:28.282154 grabberlib-0.0.3/grabber/core/sources/graph.py
+-rw-r--r--   0        0        0     4083 2024-04-18 21:14:28.282411 grabberlib-0.0.3/grabber/core/sources/khd.py
+-rw-r--r--   0        0        0     3671 2024-04-18 21:14:28.282077 grabberlib-0.0.3/grabber/core/sources/xasiat.py
+-rw-r--r--   0        0        0     1721 2024-04-18 21:14:28.281979 grabberlib-0.0.3/grabber/core/sources/yellow.py
+-rw-r--r--   0        0        0     9248 2024-04-18 21:14:28.282016 grabberlib-0.0.3/grabber/core/utils.py
+-rw-r--r--   0        0        0      175 2024-04-18 21:14:28.281457 grabberlib-0.0.3/grabber/core/version.py
+-rw-r--r--   0        0        0        0 2024-04-18 20:28:10.854369 grabberlib-0.0.3/grabber/templates/__init__.py
+-rw-r--r--   0        0        0     1017 2024-04-18 21:17:12.932509 grabberlib-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1308 1970-01-01 00:00:00.000000 grabberlib-0.0.3/PKG-INFO
```

### Comparing `grabberlib-0.0.1/assets/telegraph_pages.txt` & `grabberlib-0.0.3/assets/pages.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,54 +27,50 @@
 Xingyan Vol 218: https://telegra.ph/Xingyan-Vol-218-04-16
 Xingyan Vol 210: https://telegra.ph/Xingyan-Vol-210-04-16
 Xingyan Vol 166: https://telegra.ph/Xingyan-Vol-166-04-16
 Xingyan星颜社Vol: https://telegra.ph/Xingyan星颜社Vol-04-16
 Xingyan Vol 201: https://telegra.ph/Xingyan-Vol-201-04-16
 Xiuren Vol 8332: https://telegra.ph/Xiuren-Vol-8332-04-16
 Xingyan Vol 199: https://telegra.ph/Xingyan-Vol-199-04-16
-
-
 Xingyan Vol 225: https://telegra.ph/Xingyan-Vol-225-04-16
 Xingyan Vol 198: https://telegra.ph/Xingyan-Vol-198-04-16
 Xingyan Vol 191: https://telegra.ph/Xingyan-Vol-191-04-16
 
-
 03-09: https://telegra.ph/03-09-04-16
 01-16: https://telegra.ph/01-16-04-16
 02-16: https://telegra.ph/02-16-04-16
 
 
-04-[cosplay] Heroine K Macchima: https://telegra.ph/04-cosplay-Heroine-K-Macchima-04-16
-03-[cosplay] Heroine K hypnotizes the arrogant senior: https://telegra.ph/03-cosplay-Heroine-K-hypnotizes-the-arrogant-senior-04-16
-02-[cosplay]  Heroine K morning without makeup: https://telegra.ph/02-cosplay-Heroine-K-morning-without-makeup-04-16
-01-[cosplay] Heroine K witch: https://telegra.ph/01-cosplay-Heroine-K-witch-04-16
+Heroine K Macchima: https://telegra.ph/04-cosplay-Heroine-K-Macchima-04-16
+Heroine K hypnotizes the arrogant senior: https://telegra.ph/03-cosplay-Heroine-K-hypnotizes-the-arrogant-senior-04-16
+Heroine K morning without makeup: https://telegra.ph/02-cosplay-Heroine-K-morning-without-makeup-04-16
+Heroine K witch: https://telegra.ph/01-cosplay-Heroine-K-witch-04-16
+
 Kokuhui(Yuuhui玉汇)   雪兔[830Mb 100Photos] : https://telegra.ph/KokuhuiYuuhui玉汇-雪兔830Mb-100Photos-04-16
 Yuuhui玉汇 靡烟 黑纱旗袍[1448Mb 117Photos] : https://telegra.ph/Yuuhui玉汇-靡烟-黑纱旗袍1448Mb-117Photos-04-16
 Yuuhui玉汇   埃罗芬·雷·马科[947Mb 82Photos] : https://telegra.ph/Yuuhui玉汇-埃罗芬雷马科947Mb-82Photos-04-16
 Yuuhui玉汇 (Kokuhui)   埃罗芬·雷·马科[947Mb 82Photos] : https://telegra.ph/Yuuhui玉汇-Kokuhui-埃罗芬雷马科947Mb-82Photos-04-16
-
-
 Yuuhui玉汇   高级护理[692Mb 72Photos] : https://telegra.ph/Yuuhui玉汇-高级护理692Mb-72Photos-04-16
 Yuuhui玉汇 (Kokuhui)   茶的故事[1196Mb 115Photos] : https://telegra.ph/Yuuhui玉汇-Kokuhui-茶的故事1196Mb-115Photos-04-16
 Yuuhui玉汇   祝巫神女[1521Mb 120Photos] : https://telegra.ph/Yuuhui玉汇-祝巫神女1521Mb-120Photos-04-17
 Yuuhui玉汇   2023 Leohex泳装系列 Part I[302Mb 42Photos] : https://telegra.ph/Yuuhui玉汇-2023-Leohex泳装系列-Part-I302Mb-42Photos-04-17
-
-
 Yuuhui玉汇   祝巫神女[1521Mb 120Photos] : https://telegra.ph/Yuuhui玉汇-祝巫神女1521Mb-120Photos-04-17-3
 Yuuhui玉汇 (Kokuhui)   麦当劳的女服务员[1616Mb 122Photos] : https://telegra.ph/Yuuhui玉汇-Kokuhui-麦当劳的女服务员1616Mb-122Photos-04-17
 Yuuhui玉汇   2023 Leohex泳装系列 Part I[302Mb 42Photos] : https://telegra.ph/Yuuhui玉汇-2023-Leohex泳装系列-Part-I302Mb-42Photos-04-17-2
-
-
-
 Yuuhui玉汇   Mako Oiled Kimono[930Mb 82Photos] : https://telegra.ph/Yuuhui玉汇-Mako-Oiled-Kimono930Mb-82Photos-04-17
 Yuuhui玉汇   蜡狐[1877Mb 163Photos] : https://telegra.ph/Yuuhui玉汇-蜡狐1877Mb-163Photos-04-17
 [Cosplay] Yuuhui玉汇   圣女の史莱姆修行计划[986Mb 106Photos] : https://telegra.ph/Cosplay-Yuuhui玉汇-圣女の史莱姆修行计划986Mb-106Photos-04-17
 Yuuhui玉汇 No.022 游泳部学妹[646Mb 89Photos] : https://telegra.ph/Yuuhui玉汇-No022-游泳部学妹646Mb-89Photos-04-17
 Cosplay Yuuhui玉汇 – 游泳部学妹[646Mb 89Photos] : https://telegra.ph/Cosplay-Yuuhui玉汇--游泳部学妹646Mb-89Photos-04-17
 Yuuhui玉汇 No.020 女仆假日[1383Mb 74Photos] : https://telegra.ph/Yuuhui玉汇-No020-女仆假日1383Mb-74Photos-04-17
 Cosplay Yuuhui玉汇 – 游泳部学妹[646Mb 89Photos] : https://telegra.ph/Cosplay-Yuuhui玉汇--游泳部学妹646Mb-89Photos-04-17-2
 (Cosplay) Yuuhui玉汇 – 爱欲之神[1175Mb 103Photos] : https://telegra.ph/Cosplay-Yuuhui玉汇--爱欲之神1175Mb-103Photos-04-17
 Yuuhui玉汇 No.021 爱欲之神[1175Mb 104Photos] : https://telegra.ph/Yuuhui玉汇-No021-爱欲之神1175Mb-104Photos-04-17
 Cosplay Yuuhui玉汇 – 粉兔束缚[506Mb 51Photos] : https://telegra.ph/Cosplay-Yuuhui玉汇--粉兔束缚506Mb-51Photos-04-17
 
 
+Xingyan星颜社Vol: https://telegra.ph/Xingyan星颜社Vol-04-18
+
 
+01 Yuuhui玉汇 No.019 间谍过家家 约尔·福杰[402Mb 44Photos] : https://telegra.ph/01-Yuuhui玉汇-No019-间谍过家家-约尔福杰402Mb-44Photos-04-18
+02 Yuuhui玉汇 No.018 圣女の史莱姆修行计划(986Mb)(106Photos) : https://telegra.ph/02-Yuuhui玉汇-No018-圣女の史莱姆修行计划986Mb106Photos-04-18
+03 Yuuhui玉汇 No.017 熊猫女仆(510Mb)(30Photos) : https://telegra.ph/03-Yuuhui玉汇-No017-熊猫女仆510Mb30Photos-04-18
```

### Comparing `grabberlib-0.0.1/grabber/graph.py` & `grabberlib-0.0.3/grabber/core/sources/xasiat.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,100 +1,105 @@
 import multiprocessing
 import pathlib
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
-from typing import List, Optional
+from typing import List
 
-from casefy.casefy import snakecase
 from tqdm import tqdm
 
-from grabber.settings import MEDIA_ROOT
-from grabber.utils import (
+from grabber.core.settings import MEDIA_ROOT
+from grabber.core.utils import (
     query_mapping,
     headers_mapping,
-    get_url,
+    get_tags,
     download_images,
     upload_to_telegraph,
 )
 
 DEFAULT_THREADS_NUMBER = multiprocessing.cpu_count()
 
 
-def get_for_telegraph(
+def get_for_xasiat(
     sources: List[str],
     entity: str,
     final_dest: str | pathlib.Path = "",
-    save_to_telegraph: Optional[bool] = False,
+    save_to_telegraph: bool | None = False,
 ) -> None:
-    images_data = {}
-    titles = []
+    titles = set()
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
     )
     query, src_attr = query_mapping[entity]
     headers = headers_mapping.get(entity, None)
-    folders = []
+    folders = set()
+    titles_and_folders = set()
+    title_folder_mapping = {}
 
     if final_dest:
         final_dest_folder = MEDIA_ROOT / final_dest
         if not final_dest_folder.exists():
             final_dest_folder.mkdir(parents=True, exist_ok=True)
             final_dest = final_dest_folder
 
     for idx, source_url in tqdm_sources_iterable:
+        folder_name = ""
         tqdm_sources_iterable.set_description(f"Retrieving URLs from {source_url}")
-        _, tags, soup = get_url(
+        tags, soup = get_tags(
             source_url,
             headers=headers,
             query=query,
         )
 
         title_tag = soup.select("title")[0]  # type: ignore
-        title = title_tag.get_text().strip().rstrip()
-        titles.append(title)
-
-        folder_name = snakecase(title)
-        folder_name = folder_name.replace("_", "-")
+        folder_name = title_tag.get_text().strip().rstrip()
         image_index = f"{idx + 1}".zfill(2)
+        title = folder_name
         folder_name = f"{image_index}-{folder_name}"
+        titles.add(title)
+        titles_and_folders.add((title, folder_name))
 
         if final_dest:
-            new_folder = final_dest / pathlib.Path(folder_name)
+            new_folder = MEDIA_ROOT / final_dest / folder_name
         else:
-            new_folder = MEDIA_ROOT / pathlib.Path(folder_name)
-        print(f"New folder: {new_folder}")
+            new_folder = MEDIA_ROOT / folder_name
 
         if not new_folder.exists():
             new_folder.mkdir(parents=True, exist_ok=True)
-            print(f"Folder {new_folder} created\n")
 
-        folders.append(new_folder)
+        folders.add(new_folder)
         unique_img_urls = set()
 
-        for idx, img_tag in enumerate(tags):
+        for idx, img_tag in enumerate(tags or []):
             img_src = img_tag.attrs[src_attr]
-            img_name: str = img_src.split("/")[-1]
-            img_name = img_name.strip().rstrip()
-            if "images.hotgirl.asia" not in img_src:
-                unique_img_urls.add(
-                    (title, f"{idx + 1}-{img_name}", f"https://telegra.ph{img_src}"),
-                )
+
+            if "xasiat" in img_src:
+                img_name: str = img_src.split("/")[-2]
+                img_name = img_name.strip().rstrip()
+                img_extension: str = img_name.split(".")[-1]
             else:
-                unique_img_urls.add(
-                    (title, f"{idx + 1}-{img_name}", img_src),
-                )
+                img_name: str = img_src.split("/")[-1]
+                img_name = img_name.strip().rstrip()
+                img_extension: str = img_name.split(".")[-1]
+
+            unique_img_urls.add(
+                (title, f"{idx + 1}.{img_extension}", img_src),
+            )
 
-        images_data[title] = (unique_img_urls, new_folder)
+        title_folder_mapping[title] = (unique_img_urls, new_folder)
 
     futures = []
     with ThreadPoolExecutor(max_workers=DEFAULT_THREADS_NUMBER) as executor:
-        for title in titles:
-            images_set, folder = images_data[title]
-            partial_download = partial(download_images, new_folder=folder)
+        for title, (images_set, folder_dest) in title_folder_mapping.items():
+            partial_download = partial(
+                download_images,
+                new_folder=folder_dest,
+                headers=headers,
+                title=title,
+            )
             future = executor.submit(partial_download, images_set, title=title)
             futures.append(future)
 
     for future in tqdm(
         futures,
         total=len(futures),
         desc="Finishing download...",
@@ -102,14 +107,14 @@
         future.result()
 
     if save_to_telegraph:
         for folder in folders:
             print(f"Uploading to telegraph {folder}")
             upload_to_telegraph(folder)
 
-    albums_message = ''.join([f'- {title}\n' for title in titles])
+    albums_message = "".join([f"- {title}\n" for title in titles])
     message = f"""
     All images have been downloaded and saved to the specified folder.
     Albums saved are the following:
         {albums_message}
     """
     print(message)
```

### Comparing `grabberlib-0.0.1/grabber/khd.py` & `grabberlib-0.0.3/grabber/core/sources/khd.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,37 +2,37 @@
 import pathlib
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
 from typing import List, Optional
 
 from tqdm import tqdm
 
-from grabber.settings import MEDIA_ROOT
-from grabber.utils import (
+from grabber.core.settings import MEDIA_ROOT
+from grabber.core.utils import (
     query_mapping,
     headers_mapping,
-    get_url,
+    get_tags,
     download_images,
     upload_to_telegraph,
 )
 
 DEFAULT_THREADS_NUMBER = multiprocessing.cpu_count()
 page_nav_query = "div.page-link-box li a.page-numbers"
 
 
 def get_pages_from_pagination(url: str, headers: Optional[dict] = None) -> List[str]:
-    _, tags, _ = get_url(url, headers=headers, query=page_nav_query)
-    return [a.attrs["href"] for a in tags]
+    tags, _ = get_tags(url, headers=headers, query=page_nav_query)
+    return [a.attrs["href"] for a in tags if tags]
 
 
 def get_sources_for_4khd(
     sources: List[str],
     entity: str,
     final_dest: str | pathlib.Path = "",
-    save_to_telegraph: Optional[bool] = False,
+    save_to_telegraph: bool | None = False,
 ) -> None:
     titles = set()
     tqdm_sources_iterable = tqdm(
         enumerate(sources),
         total=len(sources),
         desc="Retrieving URLs...",
     )
@@ -52,35 +52,37 @@
         current_folder = None
         current_title = None
         folder_name = ""
         urls = [source_url, *get_pages_from_pagination(url=source_url, headers=headers)]
         image_tags = []
 
         for index, url in enumerate(urls):
-            _, tags, soup = get_url(
+            tags, soup = get_tags(
                 url,
                 headers=headers,
                 query=query,
             )
-            image_tags.extend(tags)
+            image_tags.extend(tags or [])
 
             if index == 0:
                 folder_name = soup.select("title")[0].get_text()  # type: ignore
                 title = folder_name.strip().rstrip()
                 titles.add(title)
+                image_index = f"{idx + 1}".zfill(2)
+                folder_name = f"{image_index}-{folder_name}"
                 titles_and_folders.add((title, folder_name))
                 current_title = title
 
         image_index = f"{idx + 1}".zfill(2)
         folder_name = f"{image_index}-{folder_name}"
 
         if final_dest:
-            new_folder = final_dest / pathlib.Path(folder_name)
+            new_folder = MEDIA_ROOT / final_dest / folder_name
         else:
-            new_folder = MEDIA_ROOT / pathlib.Path(folder_name)
+            new_folder = MEDIA_ROOT / folder_name
 
         if not new_folder.exists():
             new_folder.mkdir(parents=True, exist_ok=True)
 
         current_folder = new_folder
         folders.add(current_folder)
         unique_img_urls = set()
@@ -111,14 +113,14 @@
     ):
         future.result()
 
     if save_to_telegraph:
         for title, (_, folder_dest) in title_folder_mapping.items():
             upload_to_telegraph(folder_dest, page_title=title)
 
-    albums_message = ''.join([f'- {title}\n' for title in titles])
+    albums_message = "".join([f"- {title}\n" for title in titles])
     message = f"""
     All images have been downloaded and saved to the specified folder.
     Albums saved are the following:
         {albums_message}
     """
     print(message)
```

### Comparing `grabberlib-0.0.1/grabber/utils.py` & `grabberlib-0.0.3/grabber/core/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from casefy.casefy import snakecase
 from PIL import Image
 from telegraph import Telegraph
 from telegraph.exceptions import TelegraphException
 from tenacity import retry, wait_chain, wait_fixed
 from tqdm import tqdm
 
-from grabber.settings import MEDIA_ROOT
+from grabber.core.settings import MEDIA_ROOT
 
 DEFAULT_THREADS_NUMBER = multiprocessing.cpu_count()
 first_query = "div.content-inner img"
 
 
 query_mapping = {
     "xiuren": ("div.content-inner img", "src"),
@@ -69,58 +69,65 @@
         *[wait_fixed(3) for _ in range(5)]
         + [wait_fixed(7) for _ in range(4)]
         + [wait_fixed(9) for _ in range(3)]
         + [wait_fixed(15)],
     ),
     reraise=True,
 )
-def get_url(
+def get_image_stream(
     url,
     headers: Optional[Dict[str, Any]] = None,
-    query: Optional[str] = None,
-    stream: Optional[bool] = None,
-    ) -> Tuple[requests.Response, Optional[List[Tag]], BeautifulSoup]:
+) -> requests.Response:
     """Wait 3s for 5 attempts
     7s for the next 4 attempts
     9s for the next 3 attempts
     then 15 for all attempts thereafter
     """
-    if stream is not None:
-        if headers is not None:
-            if stream is not None:
-                r = requests.get(url, headers=headers, stream=True)
-            else:
-                r = requests.get(url, headers=headers)
-        else:
-            if stream is not None:
-                r = requests.get(url, stream=True)
-            else:
-                r = requests.get(url)
-
-        if r.status_code >= 300:
-            print(f"Not able to retrieve {url}: {r.status_code}\n")
-
-        return r, [], None
+    if headers is not None:
+        r = requests.get(url, headers=headers, stream=True)
     else:
-        if headers is not None:
-            r = requests.get(url, headers=headers)
-        else:
-            r = requests.get(url)
+        r = requests.get(url, stream=True)
 
-    if r.status_code > 200:
-        print(f"Not able to retrieve {url}: {r.status_code}\n")
+    if r.status_code >= 300:
+        raise Exception(f"Not able to retrieve {url}: {r.status_code}\n")
 
-    soup = BeautifulSoup(r.content, features="lxml")
+    return r
 
-    if query is None:
-        return r, [], soup
 
+@retry(
+    wait=wait_chain(
+        *[wait_fixed(3) for _ in range(5)]
+        + [wait_fixed(7) for _ in range(4)]
+        + [wait_fixed(9) for _ in range(3)]
+        + [wait_fixed(15)],
+    ),
+    reraise=True,
+)
+def get_tags(
+    url,
+    query: str,
+    headers: Optional[Dict[str, Any]] = None,
+) -> Tuple[List[Tag], BeautifulSoup]:
+    """Wait 3s for 5 attempts
+    7s for the next 4 attempts
+    9s for the next 3 attempts
+    then 15 for all attempts thereafter
+    """
+    soup = get_soup(target_url=url, headers=headers)
     tags = soup.select(query)
 
-    return r, tags, soup
+    return tags, soup
+
+
+def get_soup(
+    target_url: str,
+    headers: dict[str, str] | None = None,
+) -> BeautifulSoup:
+    response = requests.get(target_url, headers=headers)
+    return BeautifulSoup(response.content, features="lxml")
 
 
 def download_images(
     images_set,
     new_folder: pathlib.Path,
     title: str,
     headers: Optional[Dict[str, str]] = None,
@@ -142,25 +149,15 @@
 
     for img_name, image_url in tqdm_iterable:
         filename = new_folder / f"{img_name}"
 
         if filename.exists():
             continue
 
-        if headers is None:
-            resp, _, _ = get_url(
-                image_url,
-                stream=True,
-            )
-        else:
-            resp, _, _ = get_url(
-                image_url,
-                headers=headers,
-                stream=True,
-            )
+        resp = get_image_stream(image_url, headers=headers)
 
         with open(filename.as_posix(), "wb") as img_file:
             resp.raw.decode_content = True
             shutil.copyfileobj(resp.raw, img_file)
 
     convert_from_webp_to_jpg(new_folder)
     return "Done"
@@ -223,15 +220,17 @@
     contents = []
     html_template = """<figure contenteditable="false"><img src="{file_path}"><figcaption dir="auto" class="editable_text" data-placeholder="{title}"></figcaption></figure>"""
 
     content_file = pathlib.Path(f"{snakecase(title)}.html")
     if content_file.exists():
         content = content_file.read_text()
     else:
-        iterable_files = tqdm(files, total=len(files), desc=f"Uploading files for {folder.name}")
+        iterable_files = tqdm(
+            files, total=len(files), desc=f"Uploading files for {folder.name}"
+        )
         for file in iterable_files:
             uploaded = upload_file(file, telegraph_client=telegraph_client)
             uploaded_files.append(uploaded)
 
         for idx, uploaded_file in enumerate(uploaded_files):
             image_title = f"{title} - {idx + 1}"
             contents.append(
@@ -243,15 +242,15 @@
             f.write(content)
 
     print(f"Creating page for {title}")
     page_url = create_page(
         title=title, html_content=content, telegraph_client=telegraph_client
     )
 
-    with open("assets/telegraph_pages.txt", "a") as f:
+    with open("assets/pages.txt", "a") as f:
         f.write(f"{title}: {page_url}\n")
 
     print(f"Page URL: {page_url}")
     return page_url
 
 
 def upload_folders_to_telegraph(folder_name: Optional[str] = "") -> None:
@@ -269,9 +268,9 @@
                     folders += nested_folders
                 else:
                     folders = root_folders
 
     for folder in folders:
         upload_to_telegraph(folder)
 
-    with open("assets/telegraph_pages.txt", "a") as f:
+    with open("assets/pages.txt", "a") as f:
         f.write("\n\n\n")
```

### Comparing `grabberlib-0.0.1/grabber/yellow.py` & `grabberlib-0.0.3/grabber/core/sources/yellow.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,14 @@
 import multiprocessing
-import pathlib
-from concurrent.futures import ThreadPoolExecutor
-from functools import partial
-from typing import Any, Dict, List, Optional
+from typing import List
 
 from lxml import etree
-from tqdm import tqdm
 
-from grabber.settings import MEDIA_ROOT
-from grabber.utils import (
-    query_mapping,
-    headers_mapping,
-    get_url,
-    download_images,
-    upload_to_telegraph,
+from grabber.core.utils import (
+    get_soup,
 )
 
 DEFAULT_THREADS_NUMBER = multiprocessing.cpu_count()
 PAGINATION_QUERY = "div.jeg_navigation.jeg_pagination"
 PAGINATION_PAGES_COUNT_QUERY = f"{PAGINATION_QUERY} span.page_info"
 BASE_URL = "https://yellowfever18.com"
 TAG_BASE_URL = f"{BASE_URL}/tag"
@@ -26,15 +17,15 @@
 CSP_TAG_PAGINATION_BASE_URL = f"{CSP_TAG_BASE_URL}/page"
 PAGINATION_BASE_URL_QUERY = "div.jeg_navigation.jeg_pagination a.page_number"
 POSTS_QUERY_XPATH = "/html/body/div[3]/div[4]/div/div[1]/div/div/div[2]/div[1]/div/div[2]/div/div[1]/div/div/div/article/div/div[1]/a[1]"
 
 
 def get_pages_from_pagination(url: str) -> List[str]:
     source_urls = []
-    _, _, soup = get_url(url)
+    soup = get_soup(url)
     dom = etree.HTML(str(soup))
     pagination = soup.select(PAGINATION_PAGES_COUNT_QUERY)[0]
     pagination_text = pagination.text
     first, last = pagination_text.split("Page")[-1].strip().split("of")
     first_page, last_page = int(first), int(last)
 
     first_link_pagination = soup.select(PAGINATION_BASE_URL_QUERY)[0]
@@ -46,12 +37,14 @@
 
     for index in range(first_page, last_page + 1):
         if index == 1:
             continue
 
         target_url = f"{base_pagination_url}/{index}/"
 
-        _, _, soup = get_url(target_url)
+        soup = get_soup(target_url)
         dom = etree.HTML(str(soup))
-        source_urls.extend([a_tag.attrib["href"] for a_tag in dom.xpath(POSTS_QUERY_XPATH)])
+        source_urls.extend(
+            [a_tag.attrib["href"] for a_tag in dom.xpath(POSTS_QUERY_XPATH)]
+        )
 
     return source_urls
```

### Comparing `grabberlib-0.0.1/pyproject.toml` & `grabberlib-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "grabberlib"
-version = "0.0.1"
+version = "0.0.3"
 description = ""
 authors = ["grabber"]
 readme = "README.md"
 packages = [
     { include = "grabber/**/*.py" },
-    { include = "assets/telegraph_pages.txt" },
+    { include = "assets/pages.txt" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 alive-progress = "^3.1.5"
 beautifulsoup4 = "^4.12.3"
 casefy = "^0.1.7"
@@ -26,22 +26,25 @@
 tqdm = "^4.66.2"
 unipath = "^1.1"
 cement = "^3.0.8"
 defusedxml = "^0.7.1"
 olefile = "^0.47"
 pillow = "^10.3.0"
 telegraph = "^2.2.0"
-cleo = "^2.1.0"
+lxml = "^5.2.1"
+rich = "^13.7.1"
+colorlog = "^6.8.2"
+jinja2 = "^3.1.3"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.18.0"
 nest-asyncio = "^1.5.6"
 pendulum = "3.0.0b1"
 ruff = "^0.3.7"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-grabber = "grabber.entrypoint:main"
+grabber = "grabber.__main__:main"
```

### Comparing `grabberlib-0.0.1/PKG-INFO` & `grabberlib-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: grabberlib
-Version: 0.0.1
+Version: 0.0.3
 Summary: 
 Author: grabber
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: alive-progress (>=3.1.5,<4.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: casefy (>=0.1.7,<0.2.0)
 Requires-Dist: cement (>=3.0.8,<4.0.0)
-Requires-Dist: cleo (>=2.1.0,<3.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: colorlog (>=6.8.2,<7.0.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: environs (>=8.0.0,<9.0.0)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
+Requires-Dist: lxml (>=5.2.1,<6.0.0)
 Requires-Dist: olefile (>=0.47,<0.48)
 Requires-Dist: patool (>=2.1.1,<3.0.0)
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
 Requires-Dist: psycopg[binary,pool] (>=3.1.13,<4.0.0)
 Requires-Dist: python-twitter (>=3.5,<4.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: requests-html (>=0.10.0,<0.11.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: telegraph (>=2.2.0,<3.0.0)
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: unipath (>=1.1,<2.0)
 Description-Content-Type: text/markdown
```

