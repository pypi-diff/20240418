# Comparing `tmp/omuplugin_onecomme-0.2.4.tar.gz` & `tmp/omuplugin_onecomme-0.2.5.tar.gz`

## Comparing `omuplugin_onecomme-0.2.4.tar` & `omuplugin_onecomme-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.4/.python-version
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.4/src/omuplugin_onecomme/__init__.py
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.4/src/omuplugin_onecomme/plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.4/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.4/README.md
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.5/src/omuplugin_onecomme/__init__.py
+-rw-r--r--   0        0        0     5934 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.5/src/omuplugin_onecomme/plugin.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.5/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.5/README.md
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.5/PKG-INFO
```

### Comparing `omuplugin_onecomme-0.2.4/src/omuplugin_onecomme/plugin.py` & `omuplugin_onecomme-0.2.5/src/omuplugin_onecomme/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,32 +108,32 @@
                 Badge(
                     label=badge.name,
                     url=badge.icon_url,
                 )
             )
     return Comment(
         id=room.key(),
-        service=room.provider_id,
+        service=room.provider_id.key(),
         name=metadata.get("title", ""),
         url=metadata.get("url", ""),
         color={"r": 190, "g": 44, "b": 255},
         data=CommentData(
             id=message.key(),
-            liveId=room.id,
+            liveId=room.id.key(),
             userId=author.key(),
-            name=author.name,
-            screenName=author.name,
+            name=author.name or "",
+            screenName=author.name or "",
             hasGift=False,
             isOwner=False,
             isAnonymous=False,
             profileImage=author.avatar_url or "",
             badges=badges,
             timestamp=message.created_at and message.created_at.isoformat() or "",
             comment=format_content(message.content),
-            displayName=author.name,
+            displayName=author.name or "",
             originalProfileImage=author.avatar_url or "",
             isFirstTime=False,
         ),
         meta={"no": 1, "tc": 1},
         serviceData=CommentServiceData(
             id=room.key(),
             name=metadata.get("title", ""),
```

